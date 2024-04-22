# Comparing `tmp/datable_ai-0.0.4.tar.gz` & `tmp/datable_ai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datable_ai-0.0.4.tar", max compression
+gzip compressed data, was "datable_ai-0.0.5.tar", max compression
```

## Comparing `datable_ai-0.0.4.tar` & `datable_ai-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1068 2024-04-16 04:28:26.214655 datable_ai-0.0.4/LICENSE
--rw-r--r--   0        0        0       24 2024-04-16 04:28:26.214775 datable_ai-0.0.4/README.md
--rw-r--r--   0        0        0      137 2024-04-22 02:56:10.143859 datable_ai-0.0.4/datable_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 07:16:32.282582 datable_ai-0.0.4/datable_ai/core/__init__.py
--rw-r--r--   0        0        0     2276 2024-04-19 04:23:17.212551 datable_ai-0.0.4/datable_ai/core/llm.py
--rw-r--r--   0        0        0     3480 2024-04-22 04:22:38.693866 datable_ai-0.0.4/datable_ai/output.py
--rw-r--r--   0        0        0     1736 2024-04-22 00:24:12.885367 datable_ai-0.0.4/datable_ai/structured_output.py
--rw-r--r--   0        0        0      546 2024-04-22 04:16:43.631474 datable_ai-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 datable_ai-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-16 04:28:26.214655 datable_ai-0.0.5/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-16 04:28:26.214775 datable_ai-0.0.5/README.md
+-rw-r--r--   0        0        0      137 2024-04-22 02:56:10.143859 datable_ai-0.0.5/datable_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:16:32.282582 datable_ai-0.0.5/datable_ai/core/__init__.py
+-rw-r--r--   0        0        0     2276 2024-04-19 04:23:17.212551 datable_ai-0.0.5/datable_ai/core/llm.py
+-rw-r--r--   0        0        0     3480 2024-04-22 04:22:38.693866 datable_ai-0.0.5/datable_ai/output.py
+-rw-r--r--   0        0        0     1736 2024-04-22 00:24:12.885367 datable_ai-0.0.5/datable_ai/structured_output.py
+-rw-r--r--   0        0        0      517 2024-04-22 04:07:33.279168 datable_ai-0.0.5/models.json
+-rw-r--r--   0        0        0      572 2024-04-22 04:29:43.899453 datable_ai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 datable_ai-0.0.5/PKG-INFO
```

### Comparing `datable_ai-0.0.4/LICENSE` & `datable_ai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.4/datable_ai/core/llm.py` & `datable_ai-0.0.5/datable_ai/core/llm.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.4/datable_ai/output.py` & `datable_ai-0.0.5/datable_ai/output.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.4/datable_ai/structured_output.py` & `datable_ai-0.0.5/datable_ai/structured_output.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.4/pyproject.toml` & `datable_ai-0.0.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "datable-ai"
-version = "0.0.4"
+version = "0.0.5"
 description = "datable-ai"
 authors = ["datable <dev@datable.jp>"]
 license = "MIT"
 readme = "README.md"
+include = ["models.json"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^1.23.1"
 langchain-openai = "^0.1.3"
 python-dotenv = "^1.0.1"
 langchain-anthropic = "^0.1.11"
```

### Comparing `datable_ai-0.0.4/PKG-INFO` & `datable_ai-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datable-ai
-Version: 0.0.4
+Version: 0.0.5
 Summary: datable-ai
 License: MIT
 Author: datable
 Author-email: dev@datable.jp
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

