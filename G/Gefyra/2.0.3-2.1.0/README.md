# Comparing `tmp/gefyra-2.0.3.tar.gz` & `tmp/gefyra-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gefyra-2.0.3.tar", max compression
+gzip compressed data, was "gefyra-2.1.0.tar", max compression
```

## Comparing `gefyra-2.0.3.tar` & `gefyra-2.1.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0     2151 2024-04-15 16:00:54.898460 gefyra-2.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/__init__.py
--rw-r--r--   0        0        0      239 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/__init__.py
--rw-r--r--   0        0        0     8859 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/bridge.py
--rw-r--r--   0        0        0     3981 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/clients.py
--rw-r--r--   0        0        0    10466 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/connect.py
--rw-r--r--   0        0        0     5845 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/install.py
--rw-r--r--   0        0        0     3066 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/list.py
--rw-r--r--   0        0        0     2797 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/reflect.py
--rw-r--r--   0        0        0     4422 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/run.py
--rw-r--r--   0        0        0     5375 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/status.py
--rw-r--r--   0        0        0     2179 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/api/utils.py
--rw-r--r--   0        0        0        0 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/__init__.py
--rw-r--r--   0        0        0     4298 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/bridge.py
--rw-r--r--   0        0        0     3763 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/clients.py
--rw-r--r--   0        0        0     5310 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/connections.py
--rw-r--r--   0        0        0      268 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/console.py
--rw-r--r--   0        0        0     2800 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/installation.py
--rw-r--r--   0        0        0     2937 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/list.py
--rw-r--r--   0        0        0     2293 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/main.py
--rw-r--r--   0        0        0     2261 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/run.py
--rw-r--r--   0        0        0      217 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/status.py
--rw-r--r--   0        0        0     4859 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/telemetry.py
--rw-r--r--   0        0        0     7345 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/updown.py
--rw-r--r--   0        0        0     7961 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/utils.py
--rw-r--r--   0        0        0     1024 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cli/version.py
--rw-r--r--   0        0        0        0 2024-04-15 16:00:54.898460 gefyra-2.0.3/gefyra/cluster/__init__.py
--rw-r--r--   0        0        0     4642 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/cluster/resources.py
--rw-r--r--   0        0        0     5385 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/cluster/utils.py
--rw-r--r--   0        0        0    13270 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/configuration.py
--rw-r--r--   0        0        0      516 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/exceptions.py
--rw-r--r--   0        0        0      441 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/__init__.py
--rw-r--r--   0        0        0     6579 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/bridge.py
--rw-r--r--   0        0        0     1927 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/cargo.py
--rw-r--r--   0        0        0     4167 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/clients.py
--rw-r--r--   0        0        0     2237 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/minikube.py
--rw-r--r--   0        0        0     4594 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/networking.py
--rw-r--r--   0        0        0     4354 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/local/utils.py
--rw-r--r--   0        0        0        0 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/__init__.py
--rw-r--r--   0        0        0      214 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/__init__.py
--rw-r--r--   0        0        0     4741 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/deployment.py
--rw-r--r--   0        0        0      331 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/namespace.py
--rw-r--r--   0        0        0     3200 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/rbac.py
--rw-r--r--   0        0        0     2106 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/service.py
--rw-r--r--   0        0        0     4530 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/comps/webhook.py
--rw-r--r--   0        0        0     1583 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/install.py
--rw-r--r--   0        0        0     2887 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/uninstall.py
--rw-r--r--   0        0        0      486 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/misc/utils.py
--rw-r--r--   0        0        0    10557 2024-04-15 16:00:54.902460 gefyra-2.0.3/gefyra/types.py
--rw-r--r--   0        0        0     1849 2024-04-15 16:00:54.902460 gefyra-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 gefyra-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2151 2024-04-22 07:14:08.776777 gefyra-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 07:14:08.776777 gefyra-2.1.0/gefyra/__init__.py
+-rw-r--r--   0        0        0      239 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/__init__.py
+-rw-r--r--   0        0        0     8859 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/bridge.py
+-rw-r--r--   0        0        0     3981 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/clients.py
+-rw-r--r--   0        0        0    10597 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/connect.py
+-rw-r--r--   0        0        0     5845 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/install.py
+-rw-r--r--   0        0        0     3066 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/list.py
+-rw-r--r--   0        0        0     2797 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/reflect.py
+-rw-r--r--   0        0        0     4422 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/run.py
+-rw-r--r--   0        0        0     5375 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/status.py
+-rw-r--r--   0        0        0     2179 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/utils.py
+-rw-r--r--   0        0        0        0 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/__init__.py
+-rw-r--r--   0        0        0     4298 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/bridge.py
+-rw-r--r--   0        0        0     3763 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/clients.py
+-rw-r--r--   0        0        0     5310 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/connections.py
+-rw-r--r--   0        0        0      268 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/console.py
+-rw-r--r--   0        0        0     2800 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/installation.py
+-rw-r--r--   0        0        0     2937 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/list.py
+-rw-r--r--   0        0        0     2367 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/main.py
+-rw-r--r--   0        0        0     2261 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/run.py
+-rw-r--r--   0        0        0      384 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/self.py
+-rw-r--r--   0        0        0      217 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/status.py
+-rw-r--r--   0        0        0     4859 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/telemetry.py
+-rw-r--r--   0        0        0     7345 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/updown.py
+-rw-r--r--   0        0        0     7961 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/utils.py
+-rw-r--r--   0        0        0     1024 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/version.py
+-rw-r--r--   0        0        0        0 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cluster/__init__.py
+-rw-r--r--   0        0        0     4642 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cluster/resources.py
+-rw-r--r--   0        0        0     5385 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cluster/utils.py
+-rw-r--r--   0        0        0    13270 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/configuration.py
+-rw-r--r--   0        0        0      516 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/exceptions.py
+-rw-r--r--   0        0        0      441 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/__init__.py
+-rw-r--r--   0        0        0     6579 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/bridge.py
+-rw-r--r--   0        0        0     1927 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/cargo.py
+-rw-r--r--   0        0        0     4167 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/clients.py
+-rw-r--r--   0        0        0     2237 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/minikube.py
+-rw-r--r--   0        0        0     4594 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/networking.py
+-rw-r--r--   0        0        0     4354 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/utils.py
+-rw-r--r--   0        0        0        0 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/__init__.py
+-rw-r--r--   0        0        0      214 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/__init__.py
+-rw-r--r--   0        0        0     4741 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/deployment.py
+-rw-r--r--   0        0        0      331 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/namespace.py
+-rw-r--r--   0        0        0     3200 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/rbac.py
+-rw-r--r--   0        0        0     2106 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/service.py
+-rw-r--r--   0        0        0     4530 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/webhook.py
+-rw-r--r--   0        0        0     1583 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/install.py
+-rw-r--r--   0        0        0     2887 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/uninstall.py
+-rw-r--r--   0        0        0      486 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/utils.py
+-rw-r--r--   0        0        0    10557 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/types.py
+-rw-r--r--   0        0        0     1849 2024-04-22 07:14:08.780777 gefyra-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 gefyra-2.1.0/PKG-INFO
```

### Comparing `gefyra-2.0.3/README.md` & `gefyra-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/api/bridge.py` & `gefyra-2.1.0/gefyra/api/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/api/clients.py` & `gefyra-2.1.0/gefyra/api/clients.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/api/connect.py` & `gefyra-2.1.0/gefyra/api/connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 import socket
 import time
 
 from typing import IO, List, Optional, TYPE_CHECKING
 from gefyra.api.clients import get_client
 from gefyra.exceptions import GefyraConnectionError
+from gefyra.local.clients import handle_get_gefyraclient
 from gefyra.local.minikube import detect_minikube_config
 from .utils import stopwatch
 
 if TYPE_CHECKING:
     from docker.models.networks import Network
 
 
@@ -22,15 +23,20 @@
     probe_wireguard_connection,
 )
 from gefyra.local.networking import get_or_create_gefyra_network, handle_remove_network
 from gefyra.local.utils import (
     compose_kubeconfig_for_serviceaccount,
     handle_docker_get_or_create_container,
 )
-from gefyra.types import GefyraClientConfig, GefyraClientState, GefyraConnectionItem
+from gefyra.types import (
+    GefyraClient,
+    GefyraClientConfig,
+    GefyraClientState,
+    GefyraConnectionItem,
+)
 
 
 logger = logging.getLogger(__name__)
 
 
 @stopwatch
 def connect(  # noqa: C901
@@ -55,26 +61,26 @@
             raise GefyraConnectionError(
                 "Connection is not yet created and no client configuration has been provided."
             )
         logger.debug(f"Creating new connection {connection_name}")
         file_str = client_config.read()
         client_config.close()
         gclient_conf = GefyraClientConfig.from_json_str(file_str)
-        client = get_client(gclient_conf.client_id, connection_name=connection_name)
-        loc = os.path.join(
-            get_gefyra_config_location(),
-            f"{connection_name}.yaml",
-        )
+
         # this kubeconfig is being used by the client to operate in the cluster
         kubeconfig_str = compose_kubeconfig_for_serviceaccount(
             gclient_conf.kubernetes_server,
             gclient_conf.ca_crt,
             "gefyra",
             base64.b64decode(gclient_conf.token).decode("utf-8"),
         )
+        loc = os.path.join(
+            get_gefyra_config_location(),
+            f"{connection_name}.yaml",
+        )
         with open(loc, "w") as f:
             f.write(kubeconfig_str)
             logger.info(f"Client kubeconfig saved to {loc}")
 
         if minikube_profile:
             logger.debug(f"Minikube profile detected: {minikube_profile}")
             mini_conf = detect_minikube_config(minikube_profile)
@@ -87,14 +93,18 @@
             connection_name=connection_name,
             kube_config_file=Path(loc),
             client_id=gclient_conf.client_id,
             cargo_endpoint_host=gclient_conf.gefyra_server.split(":")[0],
             cargo_endpoint_port=gclient_conf.gefyra_server.split(":")[1],
             cargo_container_name=f"gefyra-cargo-{connection_name}",
         )
+
+        gclient = handle_get_gefyraclient(config, gclient_conf.client_id)
+        client = GefyraClient(gclient, config)
+
         config.CARGO_PROBE_TIMEOUT = probe_timeout
 
     _retry = 0
     while _retry < 5:
         gefyra_network = get_or_create_gefyra_network(config)
         try:
             client.activate_connection(
```

### Comparing `gefyra-2.0.3/gefyra/api/install.py` & `gefyra-2.1.0/gefyra/api/install.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/api/list.py` & `gefyra-2.1.0/gefyra/api/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/api/reflect.py` & `gefyra-2.1.0/gefyra/api/reflect.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/api/run.py` & `gefyra-2.1.0/gefyra/api/run.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/api/status.py` & `gefyra-2.1.0/gefyra/api/status.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/api/utils.py` & `gefyra-2.1.0/gefyra/api/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cli/bridge.py` & `gefyra-2.1.0/gefyra/cli/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cli/clients.py` & `gefyra-2.1.0/gefyra/cli/clients.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cli/connections.py` & `gefyra-2.1.0/gefyra/cli/connections.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cli/installation.py` & `gefyra-2.1.0/gefyra/cli/installation.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cli/list.py` & `gefyra-2.1.0/gefyra/cli/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cli/main.py` & `gefyra-2.1.0/gefyra/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import click
 
+from gefyra.cli.self import _self
 from gefyra.cli.version import version
 from gefyra.cli.run import run
 from gefyra.cli.bridge import create_bridge, unbridge
 from gefyra.cli.clients import clients
 from gefyra.cli.connections import connections
 from gefyra.cli.installation import install, uninstall
 from gefyra.cli.status import status_command
@@ -60,14 +61,15 @@
 cli.add_command(cmd=cluster_down, name="down")
 cli.add_command(cmd=status_command, name="status")
 cli.add_command(cmd=create_bridge, name="bridge")
 cli.add_command(cmd=unbridge, name="unbridge")
 cli.add_command(cmd=run, name="run")
 cli.add_command(cmd=version, name="version")
 cli.add_command(cmd=list, name="list")
+cli.add_command(cmd=_self, name="self")
 
 
 def main():
     cli(obj={})
 
 
 if __name__ == "__main__":
```

### Comparing `gefyra-2.0.3/gefyra/cli/run.py` & `gefyra-2.1.0/gefyra/cli/run.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cli/telemetry.py` & `gefyra-2.1.0/gefyra/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cli/updown.py` & `gefyra-2.1.0/gefyra/cli/updown.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cli/utils.py` & `gefyra-2.1.0/gefyra/cli/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cli/version.py` & `gefyra-2.1.0/gefyra/cli/version.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cluster/resources.py` & `gefyra-2.1.0/gefyra/cluster/resources.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/cluster/utils.py` & `gefyra-2.1.0/gefyra/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/configuration.py` & `gefyra-2.1.0/gefyra/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     CARGO_ENDPOINT_LABEL,
     ACTIVE_KUBECONFIG_LABEL,
     CLIENT_ID_LABEL,
 )
 
 logger = logging.getLogger("gefyra")
 
-__VERSION__ = "2.0.3"
+__VERSION__ = "2.1.0"
 USER_HOME = os.path.expanduser("~")
 
 
 def fix_pywin32_in_frozen_build() -> None:  # pragma: no cover
     import os
     import site
```

### Comparing `gefyra-2.0.3/gefyra/exceptions.py` & `gefyra-2.1.0/gefyra/exceptions.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/local/bridge.py` & `gefyra-2.1.0/gefyra/local/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/local/cargo.py` & `gefyra-2.1.0/gefyra/local/cargo.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/local/clients.py` & `gefyra-2.1.0/gefyra/local/clients.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/local/minikube.py` & `gefyra-2.1.0/gefyra/local/minikube.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/local/networking.py` & `gefyra-2.1.0/gefyra/local/networking.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/local/utils.py` & `gefyra-2.1.0/gefyra/local/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/misc/comps/deployment.py` & `gefyra-2.1.0/gefyra/misc/comps/deployment.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/misc/comps/rbac.py` & `gefyra-2.1.0/gefyra/misc/comps/rbac.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/misc/comps/service.py` & `gefyra-2.1.0/gefyra/misc/comps/service.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/misc/comps/webhook.py` & `gefyra-2.1.0/gefyra/misc/comps/webhook.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/misc/install.py` & `gefyra-2.1.0/gefyra/misc/install.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/misc/uninstall.py` & `gefyra-2.1.0/gefyra/misc/uninstall.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/gefyra/types.py` & `gefyra-2.1.0/gefyra/types.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.0.3/pyproject.toml` & `gefyra-2.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Gefyra"
-version = "2.0.3"
+version = "2.1.0"
 description = "Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure"
 authors = ["Michael Schilonka <michael@blueshoe.io>"]
 readme = "README.md"
 homepage = "https://gefyra.dev"
 repository = "https://github.com/gefyrahq/gefyra"
 documentation = "https://gefyra.dev"
 keywords = [
```

### Comparing `gefyra-2.0.3/PKG-INFO` & `gefyra-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Gefyra
-Version: 2.0.3
+Version: 2.1.0
 Summary: Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure
 Home-page: https://gefyra.dev
 Keywords: Kubernetes,Development,Cloud-native
 Author: Michael Schilonka
 Author-email: michael@blueshoe.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

