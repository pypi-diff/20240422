# Comparing `tmp/datable_ai-0.0.2.tar.gz` & `tmp/datable_ai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datable_ai-0.0.2.tar", max compression
+gzip compressed data, was "datable_ai-0.0.3.tar", max compression
```

## Comparing `datable_ai-0.0.2.tar` & `datable_ai-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-04-16 04:28:26.214655 datable_ai-0.0.2/LICENSE
--rw-r--r--   0        0        0       24 2024-04-16 04:28:26.214775 datable_ai-0.0.2/README.md
--rw-r--r--   0        0        0       90 2024-04-21 13:42:23.051850 datable_ai-0.0.2/datable_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 07:16:32.282582 datable_ai-0.0.2/datable_ai/core/__init__.py
--rw-r--r--   0        0        0     2276 2024-04-19 04:23:17.212551 datable_ai-0.0.2/datable_ai/core/llm.py
--rw-r--r--   0        0        0     1735 2024-04-22 00:14:22.049473 datable_ai-0.0.2/datable_ai/structured_output.py
--rw-r--r--   0        0        0      504 2024-04-21 13:57:19.623659 datable_ai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 datable_ai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-16 04:28:26.214655 datable_ai-0.0.3/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-16 04:28:26.214775 datable_ai-0.0.3/README.md
+-rw-r--r--   0        0        0      137 2024-04-22 02:56:10.143859 datable_ai-0.0.3/datable_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:16:32.282582 datable_ai-0.0.3/datable_ai/core/__init__.py
+-rw-r--r--   0        0        0     2276 2024-04-19 04:23:17.212551 datable_ai-0.0.3/datable_ai/core/llm.py
+-rw-r--r--   0        0        0     2741 2024-04-22 02:55:37.096259 datable_ai-0.0.3/datable_ai/output.py
+-rw-r--r--   0        0        0     1736 2024-04-22 00:24:12.885367 datable_ai-0.0.3/datable_ai/structured_output.py
+-rw-r--r--   0        0        0      546 2024-04-22 02:57:14.858607 datable_ai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 datable_ai-0.0.3/PKG-INFO
```

### Comparing `datable_ai-0.0.2/LICENSE` & `datable_ai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.2/datable_ai/core/llm.py` & `datable_ai-0.0.3/datable_ai/core/llm.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.2/datable_ai/structured_output.py` & `datable_ai-0.0.3/datable_ai/structured_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Dict, List, Type, Optional
+from typing import Any, Dict, List, Optional, Type
+
 from langchain_core.pydantic_v1 import BaseModel, Field, create_model
 
 from datable_ai.core.llm import LLM_TYPE, create_llm
 
 
 class StructuredOutput:
     def __init__(
```

### Comparing `datable_ai-0.0.2/PKG-INFO` & `datable_ai-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: datable-ai
-Version: 0.0.2
+Version: 0.0.3
 Summary: datable-ai
 License: MIT
 Author: datable
 Author-email: dev@datable.jp
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: langchain (>=0.1.16,<0.2.0)
 Requires-Dist: langchain-anthropic (>=0.1.11,<0.2.0)
 Requires-Dist: langchain-openai (>=0.1.3,<0.2.0)
 Requires-Dist: openai (>=1.23.1,<2.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Description-Content-Type: text/markdown
 
 # datable-ai
 datable-ai
```

