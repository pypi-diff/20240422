# Comparing `tmp/llm_anyscale_endpoints-0.5.tar.gz` & `tmp/llm_anyscale_endpoints-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_anyscale_endpoints-0.5.tar", last modified: Wed Apr 17 22:58:01 2024, max compression
+gzip compressed data, was "llm_anyscale_endpoints-0.6.tar", last modified: Sun Apr 21 23:36:01 2024, max compression
```

## Comparing `llm_anyscale_endpoints-0.5.tar` & `llm_anyscale_endpoints-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:58:01.253223 llm_anyscale_endpoints-0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 22:57:55.000000 llm_anyscale_endpoints-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-17 22:58:01.253223 llm_anyscale_endpoints-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-17 22:57:55.000000 llm_anyscale_endpoints-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:58:01.253223 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 22:58:01.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-17 22:57:55.000000 llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 22:57:55.000000 llm_anyscale_endpoints-0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 22:58:01.253223 llm_anyscale_endpoints-0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:58:01.253223 llm_anyscale_endpoints-0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-17 22:57:55.000000 llm_anyscale_endpoints-0.5/tests/test_llm_anyscale_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:36:01.195681 llm_anyscale_endpoints-0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 23:35:55.000000 llm_anyscale_endpoints-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-21 23:36:01.195681 llm_anyscale_endpoints-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-21 23:35:55.000000 llm_anyscale_endpoints-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:36:01.191681 llm_anyscale_endpoints-0.6/llm_anyscale_endpoints.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-21 23:36:01.000000 llm_anyscale_endpoints-0.6/llm_anyscale_endpoints.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-21 23:36:01.000000 llm_anyscale_endpoints-0.6/llm_anyscale_endpoints.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 23:36:01.000000 llm_anyscale_endpoints-0.6/llm_anyscale_endpoints.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 23:36:01.000000 llm_anyscale_endpoints-0.6/llm_anyscale_endpoints.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-21 23:36:01.000000 llm_anyscale_endpoints-0.6/llm_anyscale_endpoints.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 23:36:01.000000 llm_anyscale_endpoints-0.6/llm_anyscale_endpoints.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-21 23:35:55.000000 llm_anyscale_endpoints-0.6/llm_anyscale_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-21 23:35:55.000000 llm_anyscale_endpoints-0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 23:36:01.195681 llm_anyscale_endpoints-0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:36:01.191681 llm_anyscale_endpoints-0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-21 23:35:55.000000 llm_anyscale_endpoints-0.6/tests/test_llm_anyscale_endpoints.py
```

### Comparing `llm_anyscale_endpoints-0.5/LICENSE` & `llm_anyscale_endpoints-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_anyscale_endpoints-0.5/PKG-INFO` & `llm_anyscale_endpoints-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-anyscale-endpoints
-Version: 0.5
+Version: 0.6
 Summary:  LLM plugin for models hosted by Anyscale Endpoints
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-anyscale-endpoints
 Project-URL: Changelog, https://github.com/simonw/llm-anyscale-endpoints/releases
 Project-URL: Issues, https://github.com/simonw/llm-anyscale-endpoints/issues
 Project-URL: CI, https://github.com/simonw/llm-anyscale-endpoints/actions
```

### Comparing `llm_anyscale_endpoints-0.5/README.md` & `llm_anyscale_endpoints-0.6/README.md`

 * *Files identical despite different names*

### Comparing `llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.egg-info/PKG-INFO` & `llm_anyscale_endpoints-0.6/llm_anyscale_endpoints.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-anyscale-endpoints
-Version: 0.5
+Version: 0.6
 Summary:  LLM plugin for models hosted by Anyscale Endpoints
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/llm-anyscale-endpoints
 Project-URL: Changelog, https://github.com/simonw/llm-anyscale-endpoints/releases
 Project-URL: Issues, https://github.com/simonw/llm-anyscale-endpoints/issues
 Project-URL: CI, https://github.com/simonw/llm-anyscale-endpoints/actions
```

### Comparing `llm_anyscale_endpoints-0.5/llm_anyscale_endpoints.py` & `llm_anyscale_endpoints-0.6/llm_anyscale_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import click
 import httpx
 import json
 import llm
 from llm.default_plugins.openai_models import Chat
 
 MODELS = (
-    "codellama/CodeLlama-70b-Instruct-hf",
-    "google/gemma-7b-it",
-    "meta-llama/Llama-2-13b-chat-hf",
-    "meta-llama/Llama-2-70b-chat-hf",
     "meta-llama/Llama-2-7b-chat-hf",
+    "meta-llama/Llama-2-13b-chat-hf",
+    "mistralai/Mixtral-8x7B-Instruct-v0.1",
     "mistralai/Mistral-7B-Instruct-v0.1",
+    "meta-llama/Llama-2-70b-chat-hf",
+    "meta-llama/Llama-3-8b-chat-hf",
+    "meta-llama/Llama-3-70b-chat-hf",
+    "codellama/CodeLlama-70b-Instruct-hf",
     "mistralai/Mixtral-8x22B-Instruct-v0.1",
-    "mistralai/Mixtral-8x7B-Instruct-v0.1",
     "mlabonne/NeuralHermes-2.5-Mistral-7B",
+    "google/gemma-7b-it"
 )
 
 
 class AnyscaleEndpointChat(Chat):
     needs_key = "anyscale-endpoints"
 
     def __str__(self):
```

### Comparing `llm_anyscale_endpoints-0.5/pyproject.toml` & `llm_anyscale_endpoints-0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-anyscale-endpoints"
-version = "0.5"
+version = "0.6"
 description = " LLM plugin for models hosted by Anyscale Endpoints"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `llm_anyscale_endpoints-0.5/tests/test_llm_anyscale_endpoints.py` & `llm_anyscale_endpoints-0.6/tests/test_llm_anyscale_endpoints.py`

 * *Files identical despite different names*

