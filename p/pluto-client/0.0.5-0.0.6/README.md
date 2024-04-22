# Comparing `tmp/pluto_client-0.0.5.tar.gz` & `tmp/pluto_client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluto_client-0.0.5.tar", max compression
+gzip compressed data, was "pluto_client-0.0.6.tar", max compression
```

## Comparing `pluto_client-0.0.5.tar` & `pluto_client-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    10139 2024-03-22 03:06:50.256126 pluto_client-0.0.5/LICENSE
--rw-r--r--   0        0        0      241 2024-03-22 03:06:50.261224 pluto_client-0.0.5/README.md
--rw-r--r--   0        0        0      213 2024-03-22 03:06:50.263830 pluto_client-0.0.5/pluto_client/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 03:06:50.264201 pluto_client-0.0.5/pluto_client/clients/__init__.py
--rw-r--r--   0        0        0      153 2024-03-22 03:06:50.267637 pluto_client-0.0.5/pluto_client/clients/aws/__init__.py
--rw-r--r--   0        0        0     2788 2024-03-22 03:06:50.270114 pluto_client-0.0.5/pluto_client/clients/aws/function_lambda.py
--rw-r--r--   0        0        0     1018 2024-03-25 12:43:18.628466 pluto_client-0.0.5/pluto_client/clients/aws/kvstore_dynamodb.py
--rw-r--r--   0        0        0     1198 2024-03-22 03:06:50.273165 pluto_client-0.0.5/pluto_client/clients/aws/queue_sns.py
--rw-r--r--   0        0        0     1137 2024-03-22 03:06:50.274687 pluto_client-0.0.5/pluto_client/clients/aws/sagemaker.py
--rw-r--r--   0        0        0      566 2024-03-22 03:06:50.276066 pluto_client-0.0.5/pluto_client/clients/aws/utils.py
--rw-r--r--   0        0        0      187 2024-03-22 03:06:50.277629 pluto_client-0.0.5/pluto_client/clients/errors.py
--rw-r--r--   0        0        0       33 2024-03-22 03:06:50.279344 pluto_client-0.0.5/pluto_client/clients/shared/__init__.py
--rw-r--r--   0        0        0      407 2024-03-22 03:06:50.281053 pluto_client-0.0.5/pluto_client/clients/shared/router.py
--rw-r--r--   0        0        0     1811 2024-03-22 03:06:50.282386 pluto_client-0.0.5/pluto_client/function.py
--rw-r--r--   0        0        0     1703 2024-03-25 12:43:18.630810 pluto_client-0.0.5/pluto_client/kvstore.py
--rw-r--r--   0        0        0     1889 2024-03-22 03:06:50.285147 pluto_client-0.0.5/pluto_client/queue.py
--rw-r--r--   0        0        0     2059 2024-04-01 03:42:12.388520 pluto_client-0.0.5/pluto_client/router.py
--rw-r--r--   0        0        0     3610 2024-03-25 12:43:18.634467 pluto_client-0.0.5/pluto_client/sagemaker.py
--rw-r--r--   0        0        0      796 2024-04-03 08:24:36.909155 pluto_client-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 pluto_client-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    10139 2024-04-12 09:11:51.818491 pluto_client-0.0.6/LICENSE
+-rw-r--r--   0        0        0      241 2024-04-12 09:11:51.818491 pluto_client-0.0.6/README.md
+-rw-r--r--   0        0        0      213 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/aws/__init__.py
+-rw-r--r--   0        0        0     2788 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/aws/function_lambda.py
+-rw-r--r--   0        0        0     1018 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/aws/kvstore_dynamodb.py
+-rw-r--r--   0        0        0     1198 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/aws/queue_sns.py
+-rw-r--r--   0        0        0     1058 2024-04-22 07:59:31.588729 pluto_client-0.0.6/pluto_client/clients/aws/sagemaker.py
+-rw-r--r--   0        0        0      566 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/aws/utils.py
+-rw-r--r--   0        0        0      187 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/errors.py
+-rw-r--r--   0        0        0       33 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/shared/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/clients/shared/router.py
+-rw-r--r--   0        0        0     1811 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/function.py
+-rw-r--r--   0        0        0     1703 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/kvstore.py
+-rw-r--r--   0        0        0     1889 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/queue.py
+-rw-r--r--   0        0        0     2059 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/router.py
+-rw-r--r--   0        0        0     3610 2024-04-12 09:11:51.818491 pluto_client-0.0.6/pluto_client/sagemaker.py
+-rw-r--r--   0        0        0      796 2024-04-22 08:01:10.773787 pluto_client-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 pluto_client-0.0.6/PKG-INFO
```

### Comparing `pluto_client-0.0.5/LICENSE` & `pluto_client-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.5/pluto_client/clients/aws/function_lambda.py` & `pluto_client-0.0.6/pluto_client/clients/aws/function_lambda.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.5/pluto_client/clients/aws/kvstore_dynamodb.py` & `pluto_client-0.0.6/pluto_client/clients/aws/kvstore_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.5/pluto_client/clients/aws/queue_sns.py` & `pluto_client-0.0.6/pluto_client/clients/aws/queue_sns.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.5/pluto_client/clients/aws/sagemaker.py` & `pluto_client-0.0.6/pluto_client/clients/aws/sagemaker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import boto3
 import json
-import base64
 from typing import Any, Optional
 from pluto_base.utils import gen_resource_id, get_env_val_for_property
 from .utils import gen_aws_resource_name
 from ...sagemaker import ISageMakerClient, SageMakerOptions, SageMaker as SageMakerProto
 
 
 class SageMaker(ISageMakerClient):
@@ -21,12 +20,11 @@
     def invoke(self, input_data: Any) -> Any:
         response = self.client.invoke_endpoint(
             EndpointName=self.endpoint_name,
             Body=json.dumps(input_data),
             ContentType="application/json",
             Accept="application/json",
         )
-        response_body = base64.b64decode(response["Body"]).decode("utf-8")
-        return json.loads(response_body)
+        return json.loads(response["Body"].read())
 
     def endpoint_url(self) -> str:
         return get_env_val_for_property(self.__id, "endpointUrl")
```

### Comparing `pluto_client-0.0.5/pluto_client/clients/aws/utils.py` & `pluto_client-0.0.6/pluto_client/clients/aws/utils.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.5/pluto_client/function.py` & `pluto_client-0.0.6/pluto_client/function.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.5/pluto_client/kvstore.py` & `pluto_client-0.0.6/pluto_client/kvstore.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.5/pluto_client/queue.py` & `pluto_client-0.0.6/pluto_client/queue.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.5/pluto_client/router.py` & `pluto_client-0.0.6/pluto_client/router.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.5/pluto_client/sagemaker.py` & `pluto_client-0.0.6/pluto_client/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.5/pyproject.toml` & `pluto_client-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pluto-client"
-version = "0.0.5"
+version = "0.0.6"
 description = "The Client Library for Pluto Programming Language."
 authors = ["Jade Zheng <zheng.shoujian@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 classifiers = [
     'Development Status :: 1 - Planning',
     'Environment :: Console',
```

### Comparing `pluto_client-0.0.5/PKG-INFO` & `pluto_client-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluto-client
-Version: 0.0.5
+Version: 0.0.6
 Summary: The Client Library for Pluto Programming Language.
 License: Apache-2.0
 Author: Jade Zheng
 Author-email: zheng.shoujian@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

