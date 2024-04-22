# Comparing `tmp/datable_ai-0.0.3.tar.gz` & `tmp/datable_ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datable_ai-0.0.3.tar", max compression
+gzip compressed data, was "datable_ai-0.0.4.tar", max compression
```

## Comparing `datable_ai-0.0.3.tar` & `datable_ai-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-04-16 04:28:26.214655 datable_ai-0.0.3/LICENSE
--rw-r--r--   0        0        0       24 2024-04-16 04:28:26.214775 datable_ai-0.0.3/README.md
--rw-r--r--   0        0        0      137 2024-04-22 02:56:10.143859 datable_ai-0.0.3/datable_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 07:16:32.282582 datable_ai-0.0.3/datable_ai/core/__init__.py
--rw-r--r--   0        0        0     2276 2024-04-19 04:23:17.212551 datable_ai-0.0.3/datable_ai/core/llm.py
--rw-r--r--   0        0        0     2741 2024-04-22 02:55:37.096259 datable_ai-0.0.3/datable_ai/output.py
--rw-r--r--   0        0        0     1736 2024-04-22 00:24:12.885367 datable_ai-0.0.3/datable_ai/structured_output.py
--rw-r--r--   0        0        0      546 2024-04-22 02:57:14.858607 datable_ai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 datable_ai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-16 04:28:26.214655 datable_ai-0.0.4/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-16 04:28:26.214775 datable_ai-0.0.4/README.md
+-rw-r--r--   0        0        0      137 2024-04-22 02:56:10.143859 datable_ai-0.0.4/datable_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:16:32.282582 datable_ai-0.0.4/datable_ai/core/__init__.py
+-rw-r--r--   0        0        0     2276 2024-04-19 04:23:17.212551 datable_ai-0.0.4/datable_ai/core/llm.py
+-rw-r--r--   0        0        0     3480 2024-04-22 04:22:38.693866 datable_ai-0.0.4/datable_ai/output.py
+-rw-r--r--   0        0        0     1736 2024-04-22 00:24:12.885367 datable_ai-0.0.4/datable_ai/structured_output.py
+-rw-r--r--   0        0        0      546 2024-04-22 04:16:43.631474 datable_ai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 datable_ai-0.0.4/PKG-INFO
```

### Comparing `datable_ai-0.0.3/LICENSE` & `datable_ai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.3/datable_ai/core/llm.py` & `datable_ai-0.0.4/datable_ai/core/llm.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.3/datable_ai/structured_output.py` & `datable_ai-0.0.4/datable_ai/structured_output.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.3/pyproject.toml` & `datable_ai-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datable-ai"
-version = "0.0.3"
+version = "0.0.4"
 description = "datable-ai"
 authors = ["datable <dev@datable.jp>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `datable_ai-0.0.3/PKG-INFO` & `datable_ai-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datable-ai
-Version: 0.0.3
+Version: 0.0.4
 Summary: datable-ai
 License: MIT
 Author: datable
 Author-email: dev@datable.jp
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

