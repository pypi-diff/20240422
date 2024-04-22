# Comparing `tmp/screwdriver-cd-python-sdk-1.0.0.tar.gz` & `tmp/screwdriver-cd-python-sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screwdriver-cd-python-sdk-1.0.0.tar", last modified: Sun Apr  7 10:09:33 2024, max compression
+gzip compressed data, was "screwdriver-cd-python-sdk-1.0.1.tar", last modified: Mon Apr 22 05:01:16 2024, max compression
```

## Comparing `screwdriver-cd-python-sdk-1.0.0.tar` & `screwdriver-cd-python-sdk-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:09:33.011651 screwdriver-cd-python-sdk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 10:09:33.011651 screwdriver-cd-python-sdk-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:09:33.011651 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/screwdriver_initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:09:33.011651 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 10:09:32.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-07 10:09:32.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:09:32.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:09:32.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 10:09:32.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:09:33.011651 screwdriver-cd-python-sdk-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:01:16.761373 screwdriver-cd-python-sdk-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 05:01:10.000000 screwdriver-cd-python-sdk-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-22 05:01:16.761373 screwdriver-cd-python-sdk-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-22 05:01:10.000000 screwdriver-cd-python-sdk-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:01:16.761373 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 05:01:10.000000 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-22 05:01:10.000000 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-22 05:01:10.000000 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-22 05:01:10.000000 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk/screwdriver_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-22 05:01:10.000000 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:01:16.761373 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-22 05:01:16.000000 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-22 05:01:16.000000 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:01:16.000000 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:01:16.000000 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 05:01:16.000000 screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 05:01:16.761373 screwdriver-cd-python-sdk-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-22 05:01:11.000000 screwdriver-cd-python-sdk-1.0.1/setup.py
```

### Comparing `screwdriver-cd-python-sdk-1.0.0/LICENSE` & `screwdriver-cd-python-sdk-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-1.0.0/README.md` & `screwdriver-cd-python-sdk-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Screwdriver CD Python SDK
 =========================
 
 ![Python Version][Python Version Badge]
+[![Read the Docs][Read the Docs badge]][Read the Docs URL]
 [![PyPI][PyPI project badge]][PyPI project url]
 [![GitHub Workflow Status][GitHub Workflow Status badge]][GitHub Workflow Status URL]
 [![Apache License badge]][Apache License URL]
 
 Documentation
 -------------
 
@@ -35,7 +36,10 @@
 
 [GitHub Workflow Status badge]: https://img.shields.io/github/actions/workflow/status/QubitPi/screwdriver-cd-python-sdk/ci-cd.yml?logo=github&style=for-the-badge
 [GitHub Workflow Status URL]: https://github.com/QubitPi/screwdriver-cd-python-sdk/actions/workflows/ci-cd.yml
 
 [Python Version Badge]: https://img.shields.io/badge/Python-3.10-brightgreen?style=for-the-badge&logo=python&logoColor=white
 [PyPI project badge]: https://img.shields.io/pypi/v/screwdriver-cd-python-sdk?logo=pypi&logoColor=white&style=for-the-badge
 [PyPI project url]: https://pypi.org/project/screwdriver-cd-python-sdk/
+
+[Read the Docs badge]: https://img.shields.io/readthedocs/screwdriver-cd-python-sdk?style=for-the-badge&logo=readthedocs&logoColor=white&label=Read%20the%20Docs&labelColor=8CA1AF
+[Read the Docs URL]: https://screwdriver-cd-python-sdk.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,22 +1,26 @@
 Screwdriver CD Python SDK ========================= ![Python Version][Python
-Version Badge] [![PyPI][PyPI project badge]][PyPI project url] [![GitHub
-Workflow Status][GitHub Workflow Status badge]][GitHub Workflow Status URL] [!
-[Apache License badge]][Apache License URL] Documentation ------------- Coming
-soon Troubleshooting --------------- ### PyCharm Doesn't Detect Newly Installed
-screwdriver-cd-python-sdk Simply close your project and open it with PyCharm
-again. The re-indexing should make it work License ------- The use and
-distribution terms for Screwdriver CD Python SDK are covered by the [Apache
-License, Version 2.0].
+Version Badge] [![Read the Docs][Read the Docs badge]][Read the Docs URL] [!
+[PyPI][PyPI project badge]][PyPI project url] [![GitHub Workflow Status][GitHub
+Workflow Status badge]][GitHub Workflow Status URL] [![Apache License badge]]
+[Apache License URL] Documentation ------------- Coming soon Troubleshooting --
+------------- ### PyCharm Doesn't Detect Newly Installed screwdriver-cd-python-
+sdk Simply close your project and open it with PyCharm again. The re-indexing
+should make it work License ------- The use and distribution terms for
+Screwdriver CD Python SDK are covered by the [Apache License, Version 2.0].
                             _[_L_i_c_e_n_s_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]
 [Apache License badge]: https://img.shields.io/badge/Apache%202.0-
 F25910.svg?style=for-the-badge&logo=Apache&logoColor=white [Apache License
 URL]: https://www.apache.org/licenses/LICENSE-2.0 [Apache License, Version
 2.0]: http://www.apache.org/licenses/LICENSE-2.0.html [GitHub Workflow Status
 badge]: https://img.shields.io/github/actions/workflow/status/QubitPi/
 screwdriver-cd-python-sdk/ci-cd.yml?logo=github&style=for-the-badge [GitHub
 Workflow Status URL]: https://github.com/QubitPi/screwdriver-cd-python-sdk/
 actions/workflows/ci-cd.yml [Python Version Badge]: https://img.shields.io/
 badge/Python-3.10-brightgreen?style=for-the-badge&logo=python&logoColor=white
 [PyPI project badge]: https://img.shields.io/pypi/v/screwdriver-cd-python-
 sdk?logo=pypi&logoColor=white&style=for-the-badge [PyPI project url]: https://
-pypi.org/project/screwdriver-cd-python-sdk/
+pypi.org/project/screwdriver-cd-python-sdk/ [Read the Docs badge]: https://
+img.shields.io/readthedocs/screwdriver-cd-python-sdk?style=for-the-
+badge&logo=readthedocs&logoColor=white&label=Read%20the%20Docs&labelColor=8CA1AF
+[Read the Docs URL]: https://screwdriver-cd-python-sdk.readthedocs.io/en/
+latest/
```

### Comparing `screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/events.py` & `screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,44 +8,50 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+import sys
+
 import requests
-import sys, os
+
 
 def start_build(pipeline_id: int, screwdriver_api_url: str, token: str) -> object:
     """
     Creates and starts a pipeline build.
 
     :param pipeline_id:  The ID of the pipeline to trigger the build
-    :param screwdriver_api_url:  The URL of the Screwdriver API server. For example: http://192.168.7.2:9001 or https://mysd.com
+    :param screwdriver_api_url:  The URL of the Screwdriver API server. For example: http://192.168.7.2:9001 or
+           https://mysd.com
     :param token:  The Screwdriver API token
 
     :return:  The exact same response body as the "POST /v4/events" Swagger API in JSON
     """
     return create_and_start_event(
         screwdriver_api_url,
         {
             'pipelineId': pipeline_id,
             'startFrom': '~commit',
             'causeMessage': 'Run on create',
         },
         token
     )
 
+
 def create_and_start_event(screwdriver_api_url: str, body: object, token: str) -> object:
     """
     Creates and starts a specific event.
 
     If an error occurs, this function returns nothing but throws the causing error.
 
-    :param screwdriver_api_url:  The URL of the Screwdriver API server. For example: http://192.168.7.2:9001 or https://mysd.com
+    :param screwdriver_api_url:  The URL of the Screwdriver API server. For example: http://192.168.7.2:9001 or
+           https://mysd.com
     :param body:  The exact same body as the one used in "POST /v4/events" Swagger API
     :param token:  The Screwdriver API token
 
     :return:  The exact same response body as the "POST /v4/events" Swagger API in JSON
     """
     headers = {
         'accept': 'application/json',
```

### Comparing `screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/pipeline.py` & `screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+import os
+import sys
+
 import requests
-import sys, os
+
 
 def search_pipelines_by_name(name: str, screwdriver_api_url: str, token: str) -> list[object]:
     """
     Returns, at most 50 entries, all pipelines whose name contains a specified pipeline name
 
     :param name:  The pipeline name to search. e.g. "QubitPi/my-project"
     :param screwdriver_api_url:  The URL of the Screwdriver API server
@@ -85,14 +88,15 @@
     response = requests.get('{}/v4/pipelines'.format(screwdriver_api_url), params=params, headers=headers)
 
     if response.status_code != 200:
         sys.exit(os.EX_CONFIG)
 
     return response.json()
 
+
 def create_pipeline(checkout_url: str, screwdriver_api_url: str, token: str, source_directory: object = None) -> object:
     """
     Creates a new Screwdriver pipeline for a particular repo and an optional source directory.
 
     If the source_directory is not specified, it defaults to the repo root.
 
     :param checkout_url:  The URL of the repository containing the screwdriver.yaml file of the pipeline created
```

### Comparing `screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/screwdriver_initializer.py` & `screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk/screwdriver_initializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,43 +8,48 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import logging
-import os
-import json
 import csv
-from screwdriver_cd_python_sdk.pipeline import create_pipeline
-from screwdriver_cd_python_sdk.pipeline import search_pipelines_by_name
-from screwdriver_cd_python_sdk.secrets import create_or_update_secret
+import json
+import logging
+
 from screwdriver_cd_python_sdk.events import start_build
+from screwdriver_cd_python_sdk.pipeline import (create_pipeline,
+                                                search_pipelines_by_name)
+from screwdriver_cd_python_sdk.secrets import create_or_update_secret
+
 
 def initialize(pipelines_config_path: str, screwdriver_api_url: str, token: str) -> None:
     with open(pipelines_config_path, 'r') as file:
         pipelines = json.load(file)
 
     for pipeline in pipelines:
 
         git_url = pipeline["git"]
-        repo_name = git_url[git_url.find(":")+1 : git_url.find(".git")]
+        repo_name = git_url[git_url.find(":") + 1:git_url.find(".git")]
 
-        pipeline_id=None
+        pipeline_id = None
         for match in search_pipelines_by_name(name=repo_name, screwdriver_api_url=screwdriver_api_url, token=token):
             if match["name"] == repo_name:
                 pipeline_id = match["id"]
                 logging.debug("{} is already created.".format(repo_name))
 
                 break
 
         if pipeline_id is None:
             logging.debug("Creating {}...".format(repo_name))
-            pipeline_id = create_pipeline(checkout_url=pipeline["git"], screwdriver_api_url=screwdriver_api_url, token=token)["id"]
+            pipeline_id = create_pipeline(
+                checkout_url=pipeline["git"],
+                screwdriver_api_url=screwdriver_api_url,
+                token=token
+            )["id"]
 
         if "awsCredentialFile" in pipeline:
             with open(pipeline["awsCredentialFile"], 'r') as file:
                 lines = csv.reader(file)
                 for i, row in enumerate(lines):
                     if i == 1:
                         create_or_update_secret(
@@ -82,8 +87,8 @@
 
         if pipeline["runOnCreate"]:
             start_build(pipeline_id=pipeline_id, screwdriver_api_url=screwdriver_api_url, token=token)
 
 
 def _file_content(file_path: str) -> str:
     with open(file_path, 'r') as file:
-        return file.read().rstrip('\n') # https://stackoverflow.com/a/70233945
+        return file.read().rstrip('\n')  # https://stackoverflow.com/a/70233945
```

### Comparing `screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/secrets.py` & `screwdriver-cd-python-sdk-1.0.1/screwdriver_cd_python_sdk/secrets.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,28 +9,37 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+import os
+import sys
+
 import requests
-import sys, os
 
 logging.basicConfig(level=logging.DEBUG)
 
+
 def _headers(token: str) -> object:
     return {
         'accept': 'application/json',
         'Authorization': token,
         'Content-Type': 'application/json',
     }
 
 
-def create_or_update_secret(secret_name: str, secret_value: str, pipeline_id: int, screwdriver_api_url: str, token: str) -> None:
+def create_or_update_secret(
+        secret_name: str,
+        secret_value: str,
+        pipeline_id: int,
+        screwdriver_api_url: str,
+        token: str
+) -> None:
     """
     "allowInPR" is set to be false by default
 
     :param secret_name:
     :param secret_value:
     :param pipeline_id:
     :param token:
@@ -49,21 +58,27 @@
         for secrete in response.json():
             if secrete["name"] == secret_name:
                 json_data = {
                     'value': secret_value,
                     'allowInPR': False,
                 }
 
-                if requests.put('{}/v4/secrets/{}'.format(screwdriver_api_url, secrete["id"]), headers=_headers(token), json=json_data).status_code != 200:
+                if requests.put(
+                        '{}/v4/secrets/{}'.format(screwdriver_api_url, secrete["id"]),
+                        headers=_headers(token),
+                        json=json_data
+                ).status_code != 200:
                     sys.exit(os.EX_CONFIG)
     else:
         logging.debug("Creating secret '{}'".format(secret_name))
 
         json_data = {
             'pipelineId': pipeline_id,
             'name': secret_name,
             'value': secret_value,
             'allowInPR': False,
         }
 
-        if requests.post('{}/v4/secrets'.format(screwdriver_api_url), headers=_headers(token), json=json_data).status_code != 201:
+        if requests.post(
+                '{}/v4/secrets'.format(screwdriver_api_url), headers=_headers(token), json=json_data
+        ).status_code != 201:
             sys.exit(os.EX_CONFIG)
```

