# Comparing `tmp/datable_ai-0.0.1.tar.gz` & `tmp/datable_ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datable_ai-0.0.1.tar", max compression
+gzip compressed data, was "datable_ai-0.0.2.tar", max compression
```

## Comparing `datable_ai-0.0.1.tar` & `datable_ai-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-04-16 04:28:26.214655 datable_ai-0.0.1/LICENSE
--rw-r--r--   0        0        0       24 2024-04-16 04:28:26.214775 datable_ai-0.0.1/README.md
--rw-r--r--   0        0        0       90 2024-04-21 13:42:23.051850 datable_ai-0.0.1/datable_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 07:16:32.282582 datable_ai-0.0.1/datable_ai/core/__init__.py
--rw-r--r--   0        0        0     2276 2024-04-19 04:23:17.212551 datable_ai-0.0.1/datable_ai/core/llm.py
--rw-r--r--   0        0        0     1093 2024-04-21 13:27:56.465001 datable_ai-0.0.1/datable_ai/main.py
--rw-r--r--   0        0        0     1380 2024-04-21 13:39:37.835911 datable_ai-0.0.1/datable_ai/structured_output.py
--rw-r--r--   0        0        0      504 2024-04-19 04:10:09.031997 datable_ai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 datable_ai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-16 04:28:26.214655 datable_ai-0.0.2/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-16 04:28:26.214775 datable_ai-0.0.2/README.md
+-rw-r--r--   0        0        0       90 2024-04-21 13:42:23.051850 datable_ai-0.0.2/datable_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:16:32.282582 datable_ai-0.0.2/datable_ai/core/__init__.py
+-rw-r--r--   0        0        0     2276 2024-04-19 04:23:17.212551 datable_ai-0.0.2/datable_ai/core/llm.py
+-rw-r--r--   0        0        0     1735 2024-04-22 00:14:22.049473 datable_ai-0.0.2/datable_ai/structured_output.py
+-rw-r--r--   0        0        0      504 2024-04-21 13:57:19.623659 datable_ai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 datable_ai-0.0.2/PKG-INFO
```

### Comparing `datable_ai-0.0.1/LICENSE` & `datable_ai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.1/datable_ai/core/llm.py` & `datable_ai-0.0.2/datable_ai/core/llm.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.1/datable_ai/structured_output.py` & `datable_ai-0.0.2/datable_ai/structured_output.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Type
+from typing import Any, Dict, List, Type, Optional
 from langchain_core.pydantic_v1 import BaseModel, Field, create_model
 
 from datable_ai.core.llm import LLM_TYPE, create_llm
 
 
 class StructuredOutput:
     def __init__(
@@ -15,15 +15,19 @@
         self.prompt_template = prompt_template
         self.output_fields = output_fields
         self.llm = create_llm(self.llm_type)
         self.output_model = self._create_dynamic_model()
 
     def invoke(self, **kwargs) -> str:
         prompt = self.prompt_template.format(**kwargs)
-        return self.llm.with_structured_output(self.output_model).invoke(prompt)
+        return (
+            self.llm.with_structured_output(self.output_model)
+            .invoke(prompt)
+            .json(ensure_ascii=False)
+        )
 
     def _create_dynamic_model(self) -> Type[BaseModel]:
         field_definitions = {}
 
         for field in self.output_fields:
             field_name = field["name"]
             field_type = field["type"]
@@ -37,7 +41,12 @@
         return create_model(
             "Output",
             **field_definitions,
             __base__=BaseModel,
             __module__=__name__,
             __doc__="A model representing the output of the LLM",
         )
+
+    # For the Optional import in this file, there is a possibility of using it inside the `create_model` function.
+    # Therefore, a dummy function is created to utilize the Optional import within this file.
+    def _dummy(self, _: Optional[str]) -> str:
+        pass
```

### Comparing `datable_ai-0.0.1/PKG-INFO` & `datable_ai-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datable-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: datable-ai
 License: MIT
 Author: datable
 Author-email: dev@datable.jp
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

