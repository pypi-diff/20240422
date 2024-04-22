# Comparing `tmp/llama_index_llms_watsonx-0.1.5.tar.gz` & `tmp/llama_index_llms_watsonx-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_watsonx-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_llms_watsonx-0.1.6.tar", max compression
```

## Comparing `llama_index_llms_watsonx-0.1.5.tar` & `llama_index_llms_watsonx-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       39 2024-04-02 20:58:46.838598 llama_index_llms_watsonx-0.1.5/README.md
--rw-r--r--   0        0        0       73 2024-04-02 20:58:46.838598 llama_index_llms_watsonx-0.1.5/llama_index/llms/watsonx/__init__.py
--rw-r--r--   0        0        0     7907 2024-04-02 20:58:46.838598 llama_index_llms_watsonx-0.1.5/llama_index/llms/watsonx/base.py
--rw-r--r--   0        0        0     1518 2024-04-02 20:58:46.838598 llama_index_llms_watsonx-0.1.5/llama_index/llms/watsonx/utils.py
--rw-r--r--   0        0        0     1472 2024-04-02 20:58:46.838598 llama_index_llms_watsonx-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 llama_index_llms_watsonx-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-04-02 21:03:18.265304 llama_index_llms_watsonx-0.1.6/README.md
+-rw-r--r--   0        0        0       73 2024-04-02 21:03:18.265304 llama_index_llms_watsonx-0.1.6/llama_index/llms/watsonx/__init__.py
+-rw-r--r--   0        0        0     7910 2024-04-02 21:03:18.265304 llama_index_llms_watsonx-0.1.6/llama_index/llms/watsonx/base.py
+-rw-r--r--   0        0        0     1518 2024-04-02 21:03:18.265304 llama_index_llms_watsonx-0.1.6/llama_index/llms/watsonx/utils.py
+-rw-r--r--   0        0        0     1472 2024-04-02 21:03:18.265304 llama_index_llms_watsonx-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 llama_index_llms_watsonx-0.1.6/PKG-INFO
```

### Comparing `llama_index_llms_watsonx-0.1.5/llama_index/llms/watsonx/base.py` & `llama_index_llms_watsonx-0.1.6/llama_index/llms/watsonx/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     )
 
     _model = PrivateAttr()
 
     def __init__(
         self,
         credentials: Dict[str, Any],
-        model_id: Optional[str] = "ibm/mpt-7b-instruct2",
+        model_id: Optional[str] = "ibm/granite-13b-chat-v2",
         project_id: Optional[str] = None,
         space_id: Optional[str] = None,
         max_new_tokens: Optional[int] = 512,
         temperature: Optional[float] = 0.1,
         additional_kwargs: Optional[Dict[str, Any]] = None,
         callback_manager: Optional[CallbackManager] = None,
         system_prompt: Optional[str] = None,
```

### Comparing `llama_index_llms_watsonx-0.1.5/llama_index/llms/watsonx/utils.py` & `llama_index_llms_watsonx-0.1.6/llama_index/llms/watsonx/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_watsonx-0.1.5/pyproject.toml` & `llama_index_llms_watsonx-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms watsonx integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-watsonx"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 llama-index-core = "^0.10.11.post1"
 ibm-watson-machine-learning = "^1.0.342"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_llms_watsonx-0.1.5/PKG-INFO` & `llama_index_llms_watsonx-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-watsonx
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index llms watsonx integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

