# Comparing `tmp/pyqqq_cli-0.2.5.tar.gz` & `tmp/pyqqq_cli-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq_cli-0.2.5.tar", max compression
+gzip compressed data, was "pyqqq_cli-0.2.6.tar", max compression
```

## Comparing `pyqqq_cli-0.2.5.tar` & `pyqqq_cli-0.2.6.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-03-22 07:02:26.408726 pyqqq_cli-0.2.5/LICENSE
--rw-r--r--   0        0        0      937 2024-03-22 07:01:48.074678 pyqqq_cli-0.2.5/README.md
--rw-r--r--   0        0        0      655 2024-04-16 05:36:10.806078 pyqqq_cli-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      358 2024-04-01 04:44:33.805339 pyqqq_cli-0.2.5/qupiato/cli/config.py
--rw-r--r--   0        0        0     6509 2024-04-15 01:50:45.209668 pyqqq_cli-0.2.5/qupiato/cli/main.py
--rw-r--r--   0        0        0     4459 2024-04-12 07:48:42.606234 pyqqq_cli-0.2.5/qupiato/cli/utils.py
--rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 pyqqq_cli-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      937 2024-03-26 03:56:47.680900 pyqqq_cli-0.2.6/README.md
+-rw-r--r--   0        0        0      655 2024-04-22 08:16:49.081048 pyqqq_cli-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-04-12 09:23:39.993237 pyqqq_cli-0.2.6/qupiato/cli/config.py
+-rw-r--r--   0        0        0     8659 2024-04-22 08:15:00.066397 pyqqq_cli-0.2.6/qupiato/cli/main.py
+-rw-r--r--   0        0        0     5675 2024-04-22 08:12:36.529460 pyqqq_cli-0.2.6/qupiato/cli/utils.py
+-rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 pyqqq_cli-0.2.6/PKG-INFO
```

### Comparing `pyqqq_cli-0.2.5/README.md` & `pyqqq_cli-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.2.5/pyproject.toml` & `pyqqq_cli-0.2.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq-cli"
-version = "0.2.5"
+version = "0.2.6"
 description = "CLI tool for controlling strategies deployed on the PyQQQ platform."
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qupiato"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq_cli-0.2.5/qupiato/cli/utils.py` & `pyqqq_cli-0.2.6/qupiato/cli/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -100,14 +100,55 @@
         print(f"done. {object_key}")
         return object_key
 
 def get_version():
     version = importlib.metadata.version('pyqqq-cli')
     return version
 
+def search_strategies(params=''):
+    url = f"{c.API_SERVER_URL}/deployments/search"
+    headers = {
+        'Authorization': f'Bearer {get_token()}'
+    }
+    response = requests.get(url, headers=headers, params=params)
+
+    if response.status_code != 200:
+        if response.status_code == 404:
+            return None
+        else:
+            raise Exception("Failed to search strategies")
+
+    return response.json()
+
+def pull_strategy(name, filename):
+    url = f"{c.API_SERVER_URL}/deployments/download"
+    headers = {
+        'Authorization': f'Bearer {get_token()}'
+    }
+    response = requests.get(url, headers=headers, params={'file': filename}, stream=True)
+
+    if response.status_code != 200:
+        raise Exception("Failed to search strategies")
+
+    with open(f"{name}.zip", mode='wb') as file:
+        for chunk in response.iter_content(None):
+            file.write(chunk)
+
+def get_user(uid):
+    url = f"{c.API_SERVER_URL}/user"
+    headers = {
+        'Authorization': f'Bearer {get_token()}'
+    }
+    response = requests.get(url, headers=headers, params={'uid': uid})
+
+    if response.status_code != 200:
+        raise Exception("Failed to search strategies")
+
+    return response.json()
+
 # websocket 메시지에 추가될 agent 정보
 def get_agent():
     operating_system = {
         'Linux': 'linux',
         'Darwin': 'mac',
         'Windows': 'win',
     }
@@ -128,8 +169,8 @@
             with open(c.CREDENTIAL_FILE_PATH, 'r') as f:
                 return f.read().strip()
 
     else:
         print("ERROR: Key not found.")
         print("")
         print("Please set PYQQQ_API_KEY environment variable or create a file at ~/.qred with the API key.")
-        sys.exit(1)
+        sys.exit(1)
```

### Comparing `pyqqq_cli-0.2.5/PKG-INFO` & `pyqqq_cli-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq-cli
-Version: 0.2.5
+Version: 0.2.6
 Summary: CLI tool for controlling strategies deployed on the PyQQQ platform.
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

