# Comparing `tmp/trevorproxy_serverless-0.0.1.tar.gz` & `tmp/trevorproxy_serverless-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trevorproxy_serverless-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "trevorproxy_serverless-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `trevorproxy_serverless-0.0.1.tar` & `trevorproxy_serverless-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1831 2024-01-30 11:50:58.200681 trevorproxy_serverless-0.0.1/README.md
--rwxr-xr-x   0        0        0      543 2024-01-30 11:52:50.306781 trevorproxy_serverless-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-01-30 11:42:21.532770 trevorproxy_serverless-0.0.1/trevorproxy_serverless/__init__.py
--rwxr-xr-x   0        0        0     2643 2024-01-30 12:04:41.212065 trevorproxy_serverless-0.0.1/trevorproxy_serverless/cli.py
--rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 trevorproxy_serverless-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     2055 2024-04-19 10:59:04.348855 trevorproxy_serverless-0.0.2/README.md
+-rwxr-xr-x   0        0        0      543 2024-04-22 06:26:08.839544 trevorproxy_serverless-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-01-30 11:42:21.532770 trevorproxy_serverless-0.0.2/trevorproxy_serverless/__init__.py
+-rwxr-xr-x   0        0        0     3095 2024-04-22 06:24:46.752164 trevorproxy_serverless-0.0.2/trevorproxy_serverless/cli.py
+-rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 trevorproxy_serverless-0.0.2/PKG-INFO
```

### Comparing `trevorproxy_serverless-0.0.1/README.md` & `trevorproxy_serverless-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 TREVORproxy_serverless
 ==
 
 <br/>
 
-Sets up an autoscaling fargate cluster of SOCKS proxies to use along with [TREVORproxy](https://github.com/blacklanternsecurity/TREVORproxy).
+Sets up an autoscaling cluster of SOCKS proxies to use along with [TREVORproxy](https://github.com/blacklanternsecurity/TREVORproxy).
 
-`trevorproxy_serverless` puts a `proxy-intent` message in an sqs queue which causes the proxy cluster to scale up if it is not already up.
+- `trevorproxy_serverless` uses an SQS queue to control the autoscaling of the proxy cluster
+- as long as there is a `proxy-intent` message in the queue the cluster will stay up.
+- when running the cli it adds a message to the queue to signal it needs a running cluster of proxies
+- when the cli terminates gracefully it removes the message from the queue
+- if the cli is terminated non gracefully, the message will remain in the queue until the message retention period of the queue passes
+- while the cli is running it is using a sliding window approach to ensure the proxy intent message will not expire while the cli is running.
 
-when stopped `trevorproxy_serverless` deletes the `proxy-intent` message to signal that it does not need the proxies anymore.
-
-the sqs queue has a message retention limit which acts as a hard timeout to prevent proxies from running too long.
-
-the message retention & proxy count can be adjusted trough [terraform variables](https://github.com/aristosMiliaressis/TREVORproxy_serverless/blob/master/infra/variables.tf).
+the proxy count can be adjusted trough [terraform variables](https://github.com/aristosMiliaressis/TREVORproxy_serverless/blob/master/infra/variables.tf).
 
 <p align="center">
   <img src="https://github.com/aristosMiliaressis/TREVORproxy_serverless/blob/master/img/demo.png?raw=true">
 </p>
 
 <br/>
```

### Comparing `trevorproxy_serverless-0.0.1/pyproject.toml` & `trevorproxy_serverless-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trevorproxy_serverless"
-version = "0.0.1"
+version = "0.0.2"
 description = "TREVORproxy wrapper that integrates with aws fargate based proxy cluster"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
   "boto3",
   "threadlocal_aws",
   "trevorproxy",
```

### Comparing `trevorproxy_serverless-0.0.1/trevorproxy_serverless/cli.py` & `trevorproxy_serverless-0.0.2/trevorproxy_serverless/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,83 @@
 #!/usr/bin/python3
 from threadlocal_aws.clients import ecs, ec2
 from trevorproxy.cli import main as trevorproxy
 
 import argparse
+import threading
 import boto3
 import os
 import signal
 import sys
 import time
 import uuid
 
+queue = None
+message_id = None
+
+def terminate(sig, frame):
+    message = queue.receive_messages(MaxNumberOfMessages=1)[0]
+    queue.delete_messages(Entries=[{'Id':message_id,'ReceiptHandle':message.receipt_handle}])
+    exit(0)
+
+def send_proxy_intent():
+    global message_id
+    dedup_id = str(uuid.uuid4())
+    message_id = queue.send_message(MessageBody='{}', 
+            MessageDeduplicationId=dedup_id,
+            MessageGroupId=dedup_id)['MessageId']
+
 def main():
-    def terminate(sig, frame):
-        message = queue.receive_messages(MaxNumberOfMessages=1)[0]
-        queue.delete_messages(Entries=[{'Id':response['MessageId'],'ReceiptHandle':message.receipt_handle}])
-        exit(0)
-    
+    global queue
+
+    if os.getuid() != 0:
+        print("Please run as root")
+        exit(1)
+
     parser = argparse.ArgumentParser()
     parser.add_argument("-k", "--key", help="Use this SSH key when connecting to proxy hosts", required=True)
     parser.add_argument("-p", "--port", type=int, default=1080,
         help="Port for SOCKS server to listen on (default: 1080)")
     parser.add_argument("-l", "--listen-address", default="127.0.0.1",
         help="Listen address for SOCKS server (default: 127.0.0.1)")
     parser.add_argument("--base-port", default=32482, type=int, 
         help="Base listening port to use for SOCKS proxies (default: 32482)")
     args = parser.parse_args()
 
-    if os.getuid() != 0:
-        print("Please run as root")
-        exit(1)
-
     session = boto3.Session()
-
     sqs = session.resource('sqs')
-
     queue = sqs.get_queue_by_name(QueueName='proxy-intents.fifo')
-
-    dedup_id = str(uuid.uuid4())
-
-    response = queue.send_message(MessageBody='{}', 
-            MessageDeduplicationId=dedup_id,
-            MessageGroupId=dedup_id)
+    send_proxy_intent(queue)
+    
+    # setup graceful termination to remove proxy-intent message
+    signal.signal(signal.SIGINT, terminate)
+    signal.signal(signal.SIGTERM, terminate)
+    
+    # sliding window, to ensure messages don't expire while the tool is running
+    interval = int(queue.attributes['MessageRetentionPeriod']) / 2
+    threading.Timer(interval, send_proxy_intent).start()
 
     ecs_client = ecs()
     cluster = ecs_client.describe_clusters(clusters=['proxy-cluster'])['clusters'][0]
 
     print('Waiting for proxies to spin up..')
     while True:
         taskArns = ecs_client.list_tasks(cluster=cluster['clusterArn'], family='proxy-def')["taskArns"]
         if taskArns:
             tasks = ecs_client.describe_tasks(cluster=cluster['clusterArn'], tasks=taskArns)
             if not [t for t in tasks['tasks'] if t['containers'][0]['lastStatus'] != 'RUNNING']:
                 break
-
         time.sleep(10)
 
     ec2_client = ec2()
-
     taskENIIds = [t['attachments'][0]['details'][1]['value'] for t in tasks['tasks']]
     taskENIs = ec2_client.describe_network_interfaces(NetworkInterfaceIds=taskENIIds)['NetworkInterfaces']
     proxyIps=['root@'+e['Association']['PublicIp'] for e in taskENIs]
 
+    # prepare sys.argv for the call into trevorproxy
     trevorArgs = [sys.argv[0], '-p', str(args.port), '-l', args.listen_address,
                 'ssh', '-k', args.key,  '--base-port', str(args.base_port)]
     for i in range(len(trevorArgs), len(trevorArgs) + len(proxyIps)):
         trevorArgs.append(proxyIps[i-11])
     sys.argv = trevorArgs
 
-    signal.signal(signal.SIGINT, terminate)
-    signal.signal(signal.SIGTERM, terminate)
-
     trevorproxy()
```

### Comparing `trevorproxy_serverless-0.0.1/PKG-INFO` & `trevorproxy_serverless-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: trevorproxy_serverless
-Version: 0.0.1
+Version: 0.0.2
 Summary: TREVORproxy wrapper that integrates with aws fargate based proxy cluster
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: boto3
 Requires-Dist: threadlocal_aws
 Requires-Dist: trevorproxy
 Project-URL: repository, https://github.com/aristosMiliaressis/TREVORproxy_serverless/
 
 TREVORproxy_serverless
 ==
 
 <br/>
 
-Sets up an autoscaling fargate cluster of SOCKS proxies to use along with [TREVORproxy](https://github.com/blacklanternsecurity/TREVORproxy).
+Sets up an autoscaling cluster of SOCKS proxies to use along with [TREVORproxy](https://github.com/blacklanternsecurity/TREVORproxy).
 
-`trevorproxy_serverless` puts a `proxy-intent` message in an sqs queue which causes the proxy cluster to scale up if it is not already up.
+- `trevorproxy_serverless` uses an SQS queue to control the autoscaling of the proxy cluster
+- as long as there is a `proxy-intent` message in the queue the cluster will stay up.
+- when running the cli it adds a message to the queue to signal it needs a running cluster of proxies
+- when the cli terminates gracefully it removes the message from the queue
+- if the cli is terminated non gracefully, the message will remain in the queue until the message retention period of the queue passes
+- while the cli is running it is using a sliding window approach to ensure the proxy intent message will not expire while the cli is running.
 
-when stopped `trevorproxy_serverless` deletes the `proxy-intent` message to signal that it does not need the proxies anymore.
-
-the sqs queue has a message retention limit which acts as a hard timeout to prevent proxies from running too long.
-
-the message retention & proxy count can be adjusted trough [terraform variables](https://github.com/aristosMiliaressis/TREVORproxy_serverless/blob/master/infra/variables.tf).
+the proxy count can be adjusted trough [terraform variables](https://github.com/aristosMiliaressis/TREVORproxy_serverless/blob/master/infra/variables.tf).
 
 <p align="center">
   <img src="https://github.com/aristosMiliaressis/TREVORproxy_serverless/blob/master/img/demo.png?raw=true">
 </p>
 
 <br/>
```

