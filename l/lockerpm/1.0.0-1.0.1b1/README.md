# Comparing `tmp/lockerpm-1.0.0.tar.gz` & `tmp/lockerpm-1.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockerpm-1.0.0.tar", last modified: Wed Apr 17 05:36:27 2024, max compression
+gzip compressed data, was "lockerpm-1.0.1b1.tar", last modified: Mon Apr 22 07:27:40 2024, max compression
```

## Comparing `lockerpm-1.0.0.tar` & `lockerpm-1.0.1b1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.188693 lockerpm-1.0.0/
--rw-rw-r--   0 root         (0) root         (0)      288 2023-11-21 08:47:01.000000 lockerpm-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12566 2024-04-17 05:36:27.188693 lockerpm-1.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    11480 2024-04-08 04:15:59.000000 lockerpm-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.184693 lockerpm-1.0.0/docs/
--rw-rw-r--   0 root         (0) root         (0)     1578 2024-01-22 10:32:54.000000 lockerpm-1.0.0/docs/standard.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.184693 lockerpm-1.0.0/locker/
--rw-rw-r--   0 root         (0) root         (0)      160 2024-04-17 05:35:29.000000 lockerpm-1.0.0/locker/__about__.json
--rw-rw-r--   0 root         (0) root         (0)      226 2024-04-17 05:35:29.000000 lockerpm-1.0.0/locker/__about__.py
--rw-rw-r--   0 root         (0) root         (0)     4394 2024-04-07 16:22:07.000000 lockerpm-1.0.0/locker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6458 2024-02-29 03:03:49.000000 lockerpm-1.0.0/locker/atomic_locking.py
--rw-rw-r--   0 root         (0) root         (0)    10159 2024-04-08 04:15:59.000000 lockerpm-1.0.0/locker/binary_adapter.py
--rw-rw-r--   0 root         (0) root         (0)     7073 2024-04-08 04:15:59.000000 lockerpm-1.0.0/locker/client.py
--rw-rw-r--   0 root         (0) root         (0)     4313 2024-02-19 04:59:40.000000 lockerpm-1.0.0/locker/error.py
--rw-rw-r--   0 root         (0) root         (0)     1931 2023-12-06 07:39:00.000000 lockerpm-1.0.0/locker/logger.py
--rw-rw-r--   0 root         (0) root         (0)     1997 2024-04-08 04:15:59.000000 lockerpm-1.0.0/locker/ls_logger.py
--rw-rw-r--   0 root         (0) root         (0)    13071 2024-04-08 04:15:59.000000 lockerpm-1.0.0/locker/ls_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.188693 lockerpm-1.0.0/locker/ls_resources/
--rw-rw-r--   0 root         (0) root         (0)      251 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/ls_resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.188693 lockerpm-1.0.0/locker/ls_resources/abstract/
--rw-rw-r--   0 root         (0) root         (0)      701 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/ls_resources/abstract/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5039 2024-04-08 04:15:59.000000 lockerpm-1.0.0/locker/ls_resources/abstract/api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      543 2024-01-22 10:32:54.000000 lockerpm-1.0.0/locker/ls_resources/abstract/createable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      644 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/ls_resources/abstract/deletable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      354 2024-01-22 10:32:54.000000 lockerpm-1.0.0/locker/ls_resources/abstract/detailable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      690 2024-01-22 10:32:54.000000 lockerpm-1.0.0/locker/ls_resources/abstract/listable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      826 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/ls_resources/abstract/singleton_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      456 2023-12-05 08:56:19.000000 lockerpm-1.0.0/locker/ls_resources/abstract/updateable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     2548 2024-02-15 10:26:50.000000 lockerpm-1.0.0/locker/ls_resources/environment.py
--rw-rw-r--   0 root         (0) root         (0)     1274 2024-01-22 10:32:54.000000 lockerpm-1.0.0/locker/ls_resources/error_object.py
--rw-rw-r--   0 root         (0) root         (0)     2965 2024-02-27 07:14:42.000000 lockerpm-1.0.0/locker/ls_resources/secret.py
--rw-rw-r--   0 root         (0) root         (0)      909 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/ls_response.py
--rw-rw-r--   0 root         (0) root         (0)      422 2023-09-20 11:33:43.000000 lockerpm-1.0.0/locker/object_classes.py
--rw-rw-r--   0 root         (0) root         (0)     4166 2024-01-22 10:32:54.000000 lockerpm-1.0.0/locker/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.188693 lockerpm-1.0.0/lockerpm.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12566 2024-04-17 05:36:27.000000 lockerpm-1.0.0/lockerpm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1221 2024-04-17 05:36:27.000000 lockerpm-1.0.0/lockerpm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 05:36:27.000000 lockerpm-1.0.0/lockerpm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-17 05:36:27.000000 lockerpm-1.0.0/lockerpm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 05:36:27.000000 lockerpm-1.0.0/lockerpm.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      108 2023-09-20 11:33:43.000000 lockerpm-1.0.0/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-09-20 11:33:43.000000 lockerpm-1.0.0/requirements-dev.txt
--rw-rw-r--   0 root         (0) root         (0)       39 2023-09-20 11:33:43.000000 lockerpm-1.0.0/requirements-test.txt
--rw-rw-r--   0 root         (0) root         (0)       28 2023-11-28 06:52:28.000000 lockerpm-1.0.0/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)       61 2024-04-17 05:36:27.192693 lockerpm-1.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     4471 2024-04-17 05:35:29.000000 lockerpm-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:36:27.188693 lockerpm-1.0.0/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-09-20 11:33:43.000000 lockerpm-1.0.0/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1377 2024-01-22 10:32:54.000000 lockerpm-1.0.0/tests/test_binary_adapter.py
--rw-rw-r--   0 root         (0) root         (0)     2636 2024-01-22 10:32:54.000000 lockerpm-1.0.0/tests/test_client.py
--rw-rw-r--   0 root         (0) root         (0)      547 2023-09-20 11:33:43.000000 lockerpm-1.0.0/tests/test_logger.py
--rw-rw-r--   0 root         (0) root         (0)     2788 2024-01-22 10:32:54.000000 lockerpm-1.0.0/tests/test_util.py
--rw-rw-r--   0 root         (0) root         (0)     1219 2023-09-20 11:33:43.000000 lockerpm-1.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:27:40.059685 lockerpm-1.0.1b1/
+-rw-rw-r--   0 root         (0) root         (0)      288 2023-11-21 08:47:01.000000 lockerpm-1.0.1b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12571 2024-04-22 07:27:40.059685 lockerpm-1.0.1b1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    11495 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:27:40.051685 lockerpm-1.0.1b1/docs/
+-rw-rw-r--   0 root         (0) root         (0)     1578 2024-01-22 10:32:54.000000 lockerpm-1.0.1b1/docs/standard.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:27:40.055685 lockerpm-1.0.1b1/locker/
+-rw-rw-r--   0 root         (0) root         (0)      521 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/locker/__about__.json
+-rw-rw-r--   0 root         (0) root         (0)      228 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/locker/__about__.py
+-rw-rw-r--   0 root         (0) root         (0)     6582 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/locker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6458 2024-02-29 03:03:49.000000 lockerpm-1.0.1b1/locker/atomic_locking.py
+-rw-rw-r--   0 root         (0) root         (0)    10691 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/locker/binary_adapter.py
+-rw-rw-r--   0 root         (0) root         (0)     7304 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/locker/client.py
+-rw-rw-r--   0 root         (0) root         (0)     4313 2024-02-19 04:59:40.000000 lockerpm-1.0.1b1/locker/error.py
+-rw-rw-r--   0 root         (0) root         (0)     1931 2023-12-06 07:39:00.000000 lockerpm-1.0.1b1/locker/logger.py
+-rw-rw-r--   0 root         (0) root         (0)     1997 2024-04-08 04:15:59.000000 lockerpm-1.0.1b1/locker/ls_logger.py
+-rw-rw-r--   0 root         (0) root         (0)    13185 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/locker/ls_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:27:40.055685 lockerpm-1.0.1b1/locker/ls_resources/
+-rw-rw-r--   0 root         (0) root         (0)      251 2023-09-20 11:33:43.000000 lockerpm-1.0.1b1/locker/ls_resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:27:40.055685 lockerpm-1.0.1b1/locker/ls_resources/abstract/
+-rw-rw-r--   0 root         (0) root         (0)      701 2023-09-20 11:33:43.000000 lockerpm-1.0.1b1/locker/ls_resources/abstract/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5204 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/locker/ls_resources/abstract/api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      543 2024-01-22 10:32:54.000000 lockerpm-1.0.1b1/locker/ls_resources/abstract/createable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      644 2023-09-20 11:33:43.000000 lockerpm-1.0.1b1/locker/ls_resources/abstract/deletable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      354 2024-01-22 10:32:54.000000 lockerpm-1.0.1b1/locker/ls_resources/abstract/detailable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      690 2024-01-22 10:32:54.000000 lockerpm-1.0.1b1/locker/ls_resources/abstract/listable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      826 2023-09-20 11:33:43.000000 lockerpm-1.0.1b1/locker/ls_resources/abstract/singleton_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      456 2023-12-05 08:56:19.000000 lockerpm-1.0.1b1/locker/ls_resources/abstract/updateable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     3359 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/locker/ls_resources/environment.py
+-rw-rw-r--   0 root         (0) root         (0)     1274 2024-01-22 10:32:54.000000 lockerpm-1.0.1b1/locker/ls_resources/error_object.py
+-rw-rw-r--   0 root         (0) root         (0)     4010 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/locker/ls_resources/secret.py
+-rw-rw-r--   0 root         (0) root         (0)      909 2023-09-20 11:33:43.000000 lockerpm-1.0.1b1/locker/ls_response.py
+-rw-rw-r--   0 root         (0) root         (0)      422 2023-09-20 11:33:43.000000 lockerpm-1.0.1b1/locker/object_classes.py
+-rw-rw-r--   0 root         (0) root         (0)     4166 2024-01-22 10:32:54.000000 lockerpm-1.0.1b1/locker/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:27:40.055685 lockerpm-1.0.1b1/lockerpm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12571 2024-04-22 07:27:40.000000 lockerpm-1.0.1b1/lockerpm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1221 2024-04-22 07:27:40.000000 lockerpm-1.0.1b1/lockerpm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 07:27:40.000000 lockerpm-1.0.1b1/lockerpm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-22 07:27:40.000000 lockerpm-1.0.1b1/lockerpm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-22 07:27:40.000000 lockerpm-1.0.1b1/lockerpm.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      108 2023-09-20 11:33:43.000000 lockerpm-1.0.1b1/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-09-20 11:33:43.000000 lockerpm-1.0.1b1/requirements-dev.txt
+-rw-rw-r--   0 root         (0) root         (0)       39 2023-09-20 11:33:43.000000 lockerpm-1.0.1b1/requirements-test.txt
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-11-28 06:52:28.000000 lockerpm-1.0.1b1/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)       61 2024-04-22 07:27:40.059685 lockerpm-1.0.1b1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3057 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:27:40.059685 lockerpm-1.0.1b1/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-09-20 11:33:43.000000 lockerpm-1.0.1b1/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1377 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/tests/test_binary_adapter.py
+-rw-rw-r--   0 root         (0) root         (0)     4562 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/tests/test_client.py
+-rw-rw-r--   0 root         (0) root         (0)      547 2023-09-20 11:33:43.000000 lockerpm-1.0.1b1/tests/test_logger.py
+-rw-rw-r--   0 root         (0) root         (0)     3012 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/tests/test_util.py
+-rw-rw-r--   0 root         (0) root         (0)     1267 2024-04-22 07:27:15.000000 lockerpm-1.0.1b1/tox.ini
```

### Comparing `lockerpm-1.0.0/PKG-INFO` & `lockerpm-1.0.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockerpm
-Version: 1.0.0
+Version: 1.0.1b1
 Summary: Locker Secret Python SDK
 Home-page: https://locker.io
 Download-URL: 
 Author: CyStack
 Author-email: contact@locker.io
 Keywords: django,vault management,security
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Locker Secret Python SDK
 
 <p align="center">
   <img src="https://cystack.net/images/logo-black.svg" alt="CyStack" width="50%"/>
@@ -155,15 +155,15 @@
 ```
 
 
 ### Retrieve a secret
 
 Use `.retrieve()` function to retrieve the secret object.
 ```
-secret = locker.retieve("REDIS_CONNECTION", environment_name="staging")
+secret = locker.retrieve("REDIS_CONNECTION", environment_name="staging")
 print(secret)
 print(secret.id, secret.key, secret.value)
 ```
 
 
 ### Create new secret
 
@@ -327,14 +327,16 @@
 
 Test by using tox. We test against the following versions.
 - 3.6
 - 3.7
 - 3.8
 - 3.9
 - 3.10
+- 3.11
+- 3.12
 
 To run all tests against all versions, use:
 ```
 tox
 ```
 
 Run all tests for a specific Python version:
```

### Comparing `lockerpm-1.0.0/README.md` & `lockerpm-1.0.1b1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 ```
 
 
 ### Retrieve a secret
 
 Use `.retrieve()` function to retrieve the secret object.
 ```
-secret = locker.retieve("REDIS_CONNECTION", environment_name="staging")
+secret = locker.retrieve("REDIS_CONNECTION", environment_name="staging")
 print(secret)
 print(secret.id, secret.key, secret.value)
 ```
 
 
 ### Create new secret
 
@@ -300,14 +300,16 @@
 
 Test by using tox. We test against the following versions.
 - 3.6
 - 3.7
 - 3.8
 - 3.9
 - 3.10
+- 3.11
+- 3.12
 
 To run all tests against all versions, use:
 ```
 tox
 ```
 
 Run all tests for a specific Python version:
```

### Comparing `lockerpm-1.0.0/docs/standard.md` & `lockerpm-1.0.1b1/docs/standard.md`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/atomic_locking.py` & `lockerpm-1.0.1b1/locker/atomic_locking.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/binary_adapter.py` & `lockerpm-1.0.1b1/locker/binary_adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 
     def call(
         self,
         cli,
         params=None,
         asjson=True,
         timeout=DEFAULT_TIMEOUT,
-        skip_cli_lines=0
+        skip_cli_lines=0,
+        output_format="json"
     ):
         binary_file = self.get_binary_file()
         my_access_key_id = self.access_key_id
         my_secret_access_key = self.secret_access_key
         # if my_access_key_id is None or my_secret_access_key is None:
         #     raise error.AuthenticationError(
         #         "No Access key provided. (HINT: set your API key using "
@@ -90,16 +91,18 @@
                 '--secret-access-key', f'{my_secret_access_key}'
             ]
 
         command_arr += [
             '--api-base', f'{self.api_base}',
             '--agent', f'{default_client_agent}',
             '--resttime', f'{self.resttime}',
-            '--verbose'
+            # '--verbose'
         ]
+        if output_format:
+            command_arr += [f"--{output_format}"]
         if self.fetch is True:
             command_arr += ['--fetch']
 
         if my_headers:
             if isinstance(my_headers, dict):
                 my_headers_list = [f"{k}:{v}" for k, v in my_headers.items()]
                 my_headers = ",".join(my_headers_list)
@@ -116,17 +119,24 @@
             # makes these parameter strings easier to read.
             encoded_params = encoded_params.replace("%5B", "[").replace("%5D", "]")
             # TODO: Build api url by passing filter params to command
             # if params:
             #     abs_url = _build_api_url(abs_url, encoded_params)
             pass
         elif "update" in cli or "create" in cli:
-            post_data = json.dumps(params or {})
-        if post_data:
-            command_arr += ['--data', f'{post_data}']
+            params_data = params or {}
+            for k, v in params_data.items():
+                if k in ["key", "value", "description", "new_key", "new_value", "new_description", "env",
+                         "name", "url", "new_name", "new_url",
+                         "new-key", "new-value", "new-description", "new-name", "new-url"]:
+                    command_arr += [f'--{k.replace("_", "-")}', f'{v}']
+
+        #     post_data = json.dumps(params or {})
+        # if post_data:
+        #     command_arr += ['--data', f'{post_data}']
 
         self.logger.debug(f"[+] Running with timeout {timeout} cli command: {command_arr}")
         try:
             raw = subprocess.check_output(
                 command_arr,
                 stderr=subprocess.STDOUT, shell=False, universal_newlines=True, timeout=timeout
             )
```

### Comparing `lockerpm-1.0.0/locker/client.py` & `lockerpm-1.0.1b1/locker/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,19 @@
         _params = copy.deepcopy(self._options)
         _params.update(params)
         return _params
 
     def list(self, **params):
         return Secret.list(**self._translate_options(params))
 
+    def export(self, environment_name=None, output_format="dotenv",  **params):
+        return Secret.export(
+            environment_name=environment_name, output_format=output_format, **self._translate_options(params)
+        )
+
     def get(self, key, environment_name=None, default_value=None, **params):
         return Secret.get_secret(
             key,
             environment_name=environment_name,
             default_value=default_value,
             **self._translate_options(params)
         )
```

### Comparing `lockerpm-1.0.0/locker/error.py` & `lockerpm-1.0.1b1/locker/error.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/logger.py` & `lockerpm-1.0.1b1/locker/logger.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/ls_logger.py` & `lockerpm-1.0.1b1/locker/ls_logger.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/ls_object.py` & `lockerpm-1.0.1b1/locker/ls_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,22 +195,22 @@
             super().__setitem__(
                 k,
                 util.convert_to_ls_object(v, access_key_id, secret_access_key, api_base, api_version),
             )
 
         self._previous = values
 
-    def call(self, cli, asjson=True, timeout=DEFAULT_TIMEOUT, params=None):
+    def call(self, cli, asjson=True, timeout=DEFAULT_TIMEOUT, output_format="json", params=None):
         return LSObject._call(
-            self, cli, asjson=asjson, timeout=timeout, params=params
+            self, cli, asjson=asjson, timeout=timeout, output_format=output_format, params=params
         )
 
     # The 'cli_' is suffixed with an underscore to avoid conflicting with request parameters in `params`
     def _call(self, cli_, access_key_id=None, secret_access_key=None, api_base=None, api_version=None,
-              asjson=True, timeout=DEFAULT_TIMEOUT, params=None):
+              asjson=True, timeout=DEFAULT_TIMEOUT, output_format="json", params=None):
         params = None if params is None else params.copy()
 
         access_key_id = util.read_special_variable(params, "access_key_id", access_key_id)
         secret_access_key = util.read_special_variable(params, "secret_access_key", secret_access_key)
         api_base = util.read_special_variable(params, "api_base", api_base)
         api_version = util.read_special_variable(params, "api_version", api_version)
         headers = util.read_special_variable(params, "headers", None)
@@ -232,15 +232,16 @@
             api_version=api_version,
             headers=headers,
             logger=logger,
             resttime=resttime,
             fetch=fetch,
         )
         res_data = binary_executor.call(
-            cli=cli_, params=params, asjson=asjson, timeout=timeout, skip_cli_lines=skip_cli_lines
+            cli=cli_, params=params, asjson=asjson, timeout=timeout, skip_cli_lines=skip_cli_lines,
+            output_format=output_format
         )
         return util.convert_to_ls_object(
             res_data, access_key_id, secret_access_key, api_base, api_version, params
         )
 
     def __repr__(self):
         ident_parts = [type(self).__name__]
```

### Comparing `lockerpm-1.0.0/locker/ls_resources/abstract/__init__.py` & `lockerpm-1.0.1b1/locker/ls_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/ls_resources/abstract/api_resource.py` & `lockerpm-1.0.1b1/locker/ls_resources/abstract/api_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,25 +57,27 @@
         cli_,
         access_key_id=None,
         secret_access_key=None,
         api_base=None,
         api_version=None,
         asjson=True,
         timeout=DEFAULT_TIMEOUT,
+        output_format="json",
         params=None,
     ):
         obj = LSObject._call(
             self,
             cli_,
             access_key_id,
             secret_access_key,
             api_base,
             api_version,
             asjson,
             timeout,
+            output_format,
             params,
         )
 
         if type(self) is type(obj):
             self.refresh_from(obj)
             return self
         else:
@@ -85,20 +87,20 @@
     def _call_and_refresh(
         self,
         cli,
         access_key_id=None,
         secret_access_key=None,
         api_base=None,
         api_version=None,
-        asjson=True, timeout=DEFAULT_TIMEOUT, params=None
+        asjson=True, timeout=DEFAULT_TIMEOUT, output_format="json", params=None
     ):
         obj = LSObject._call(
             self,
             cli, access_key_id, secret_access_key, api_base, api_version,
-            asjson, timeout, params
+            asjson, timeout, output_format, params
         )
         self.refresh_from(obj)
         return self
 
     # The 'cli_' is suffixed with an underscore to avoid conflicting with request parameters in `params`
     @classmethod
     def _static_call(
@@ -106,14 +108,15 @@
         cli_,
         access_key_id=None,
         secret_access_key=None,
         api_base=None,
         api_version=None,
         asjson=True,
         timeout=DEFAULT_TIMEOUT,
+        output_format="json",
         params=None,
     ):
         params = None if params is None else params.copy()
         access_key_id = util.read_special_variable(params, "access_key_id", access_key_id)
         secret_access_key = util.read_special_variable(params, "secret_access_key", secret_access_key)
         api_base = util.read_special_variable(params, "api_base", api_base)
         api_version = util.read_special_variable(params, "api_version", api_version)
@@ -130,13 +133,14 @@
             api_version=api_version,
             headers=headers,
             logger=logger,
             resttime=resttime,
             fetch=fetch
         )
         res_data = binary_executor.call(
-            cli=cli_, params=params, asjson=asjson, timeout=timeout, skip_cli_lines=skip_cli_lines
+            cli=cli_, params=params, asjson=asjson, timeout=timeout, skip_cli_lines=skip_cli_lines,
+            output_format=output_format
         )
         return util.convert_to_ls_object(
             res_data, access_key_id, secret_access_key, api_base, api_version, params
         )
```

### Comparing `lockerpm-1.0.0/locker/ls_resources/abstract/createable_api_resource.py` & `lockerpm-1.0.1b1/locker/ls_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/ls_resources/abstract/deletable_api_resource.py` & `lockerpm-1.0.1b1/locker/ls_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/ls_resources/abstract/listable_api_resource.py` & `lockerpm-1.0.1b1/locker/ls_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/ls_resources/abstract/singleton_api_resource.py` & `lockerpm-1.0.1b1/locker/ls_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/ls_resources/environment.py` & `lockerpm-1.0.1b1/locker/ls_resources/environment.py`

 * *Files 21% similar despite different names*

```diff
@@ -63,8 +63,30 @@
         #     return None
         return instance
 
     @classmethod
     def modify(cls, **params):
         name = params.get("name")
         cli = [f"{cls.class_cli()}", "update", "--name", f"{quote_plus(name)}"]
+
+        if "external_url" in params:
+            cli += ["--new-url", f"{params.get('external_url')}"]
+        # if "new_name" in params:
+        #     cli += ["--new-name", f"{params.get('new_name')}"]
+        # if "new_description" in params:
+        #     cli += ["--new-description", f"{params.get('new_description')}"]
+
         return cls._static_call(cli, params=params)
+
+    @classmethod
+    def create(cls, access_key_id=None, secret_access_key=None, api_base=None, api_version=None, **params):
+        cli = [f"{cls.class_cli()}", "create"]
+        if "external_url" in params:
+            cli += ["--url", f"{params.get('external_url')}"]
+        return cls._static_call(
+            cli,
+            access_key_id,
+            secret_access_key,
+            api_base=api_base,
+            api_version=api_version,
+            params=params,
+        )
```

### Comparing `lockerpm-1.0.0/locker/ls_resources/error_object.py` & `lockerpm-1.0.1b1/locker/ls_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/ls_resources/secret.py` & `lockerpm-1.0.1b1/locker/ls_resources/secret.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 class Secret(ListableAPIResource, CreateableAPIResource, UpdateableAPIResource, DeletableAPIResource):
     OBJECT_NAME = "secret"
 
     @classmethod
     def get_secret(cls, key, environment_name=None, default_value=None,
                    access_key_id=None, secret_access_key=None, api_base=None, api_version=None, **params):
         base = cls.class_cli()
-        cli_ = [base, 'get', '--name', f'{key}']
+        cli_ = [base, 'get', '--key', f'{key}']
         if environment_name:
-            cli_ += ['--env', f'{environment_name}']
+            cli_ += ['--environment', f'{environment_name}']
         instance = cls(None, access_key_id, secret_access_key, **params)
         try:
             instance._call_and_refresh(
                 cli_, access_key_id=access_key_id, secret_access_key=secret_access_key,
                 api_base=api_base, api_version=api_version, params=params
             )
         except CliRunError as e:
@@ -31,42 +31,71 @@
         except AttributeError:
             return default_value
 
     @classmethod
     def retrieve_secret(cls, key, environment_name=None,
                         access_key_id=None, secret_access_key=None, api_base=None, api_version=None, **params):
         base = cls.class_cli()
-        cli_ = [base, 'get', '--name', f'{key}']
+        cli_ = [base, 'get', '--key', f'{key}']
         if environment_name:
             cli_ += ['--env', f'{environment_name}']
         instance = cls(None, access_key_id, secret_access_key, **params)
         instance._call_and_refresh(
             cli_, access_key_id=access_key_id, secret_access_key=secret_access_key,
             api_base=api_base, api_version=api_version, params=params
         )
         return instance
 
     @classmethod
     def modify(cls, **params):
         key = params.get("key")
-        cli = [f"{cls.class_cli()}", "update", "--name", f"{key}"]
+        value = params.get("value")
+        cli = [f"{cls.class_cli()}", "update", "--key", f"{key}"]
         environment_name = params.get("environment_name")
+        if value:
+            cli += ["--new-value", f"{value}"]
+            params.pop("value", None)
         if environment_name:
-            cli += ['--env', f'{environment_name}']
+            cli += ['--environment', f'{environment_name}']
             params.pop("environment_name", None)
 
         return cls._static_call(cli, params=params)
 
     @classmethod
     def create(cls, access_key_id=None, secret_access_key=None, api_base=None, api_version=None, **params):
         cli = [f"{cls.class_cli()}", "create"]
-        environment_name = params.get("environment_name")
-        if not environment_name:
-            params.update({"environment_name": None})
+
+        if "environment_name" in params:
+            environment_name = params.get("environment_name") or None
+            cli += ['--environment', f'{environment_name}']
+
+        # environment_name = params.get("environment_name")
+        # if not environment_name:
+        #     params.update({"environment_name": None})
+        # else:
+
         return cls._static_call(
             cli,
             access_key_id,
             secret_access_key,
             api_base=api_base,
             api_version=api_version,
             params=params,
         )
+
+    @classmethod
+    def export(cls, environment_name=None, output_format="dotenv",
+               access_key_id=None, secret_access_key=None, api_base=None, api_version=None, **params):
+        assert output_format in ["dotenv", "json"]
+        cli = [f"{cls.class_cli()}", "list", "--output"]
+        if environment_name:
+            cli += ['--environment', f'{environment_name}']
+        return cls._static_call(
+            cli,
+            access_key_id=access_key_id,
+            secret_access_key=secret_access_key,
+            api_base=api_base,
+            api_version=api_version,
+            asjson=False,
+            output_format=output_format,
+            params=params,
+        )
```

### Comparing `lockerpm-1.0.0/locker/ls_response.py` & `lockerpm-1.0.1b1/locker/ls_response.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/locker/util.py` & `lockerpm-1.0.1b1/locker/util.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/lockerpm.egg-info/PKG-INFO` & `lockerpm-1.0.1b1/lockerpm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockerpm
-Version: 1.0.0
+Version: 1.0.1b1
 Summary: Locker Secret Python SDK
 Home-page: https://locker.io
 Download-URL: 
 Author: CyStack
 Author-email: contact@locker.io
 Keywords: django,vault management,security
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Locker Secret Python SDK
 
 <p align="center">
   <img src="https://cystack.net/images/logo-black.svg" alt="CyStack" width="50%"/>
@@ -155,15 +155,15 @@
 ```
 
 
 ### Retrieve a secret
 
 Use `.retrieve()` function to retrieve the secret object.
 ```
-secret = locker.retieve("REDIS_CONNECTION", environment_name="staging")
+secret = locker.retrieve("REDIS_CONNECTION", environment_name="staging")
 print(secret)
 print(secret.id, secret.key, secret.value)
 ```
 
 
 ### Create new secret
 
@@ -327,14 +327,16 @@
 
 Test by using tox. We test against the following versions.
 - 3.6
 - 3.7
 - 3.8
 - 3.9
 - 3.10
+- 3.11
+- 3.12
 
 To run all tests against all versions, use:
 ```
 tox
 ```
 
 Run all tests for a specific Python version:
```

### Comparing `lockerpm-1.0.0/lockerpm.egg-info/SOURCES.txt` & `lockerpm-1.0.1b1/lockerpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/tests/test_binary_adapter.py` & `lockerpm-1.0.1b1/tests/test_binary_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         access_key_id = os.getenv("ACCESS_KEY_ID")
         secret_access_key = os.getenv("SECRET_ACCESS_KEY")
 
         binary_adapter = BinaryAdapter(
             access_key_id=access_key_id, secret_access_key=secret_access_key
         )
         platform = binary_adapter.get_platform()
-        return platform == sys.platform
+        assert platform == sys.platform
 
     def test_get_sdk_version(self):
         load_dotenv()
         access_key_id = os.getenv("ACCESS_KEY_ID")
         secret_access_key = os.getenv("SECRET_ACCESS_KEY")
 
         binary_adapter = BinaryAdapter(
```

### Comparing `lockerpm-1.0.0/tests/test_logger.py` & `lockerpm-1.0.1b1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `lockerpm-1.0.0/tests/test_util.py` & `lockerpm-1.0.1b1/tests/test_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,7 +63,15 @@
         assert utc_ts <= 1672506000 + 60
 
     def test_api_encode(self):
         data = {"search": "live_search_text", "page": "1", "size": 10}
         encoded_params = list(util.api_encode(data))
         for encoded_param in encoded_params:
             assert encoded_param[1] == data.get(encoded_param[0])
+
+    def test_merge_dicts(self):
+        x = {"x_key": "x_value"}
+        y = {"y_key": "y_value"}
+        z_expected = x.copy()
+        z_expected.update(y)
+        z = util.merge_dicts(x, y)
+        assert z == z_expected
```

### Comparing `lockerpm-1.0.0/tox.ini` & `lockerpm-1.0.1b1/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Tox (http://tox.testrun.org/) is a tool for running tests in multiple virtualenvs.
 # This configuration file will run the test suite on all supported python versions.
 # To use it, "pip install tox" and then run "tox" from this directory.
 
 
 [tox]
-envlist = py{310,39,38},python{3.7,3.6}
+envlist = py{312,311,310,39,38},python{3.7,3.6}
 skip_missing_interpreters = true
 # skipsdist = true
 
 
 [gh-actions]
 python =
+    3.12: py312
+    3.11: py311
     3.10: py310
     3.9: py39
     3.8: py38
 
 
 
 [tool:pytest]
@@ -25,15 +27,15 @@
 
 [testenv]
 description = run the unit tests under {basepython}
 setenv =
     COVERAGE_FILE = {toxworkdir}/.coverage.{envname}
 deps =
     coverage >= 4.5.3
-    py{310,39,38}: pytest >= 6.0.0
+    py{312,311,310,39,38}: pytest >= 6.0.0
     python{3.7,3.6}: pytest >= 6.0.0
     pytest-cov
     pytest-mock >= 2.0.0
     pytest-xdist >= 1.31.0
     python-dotenv
 # ignore locker directory as all tests are inside ./tests
 commands = pytest --cov {posargs:-n auto} --ignore locker
```

