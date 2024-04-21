# Comparing `tmp/osin-2.2.2.tar.gz` & `tmp/osin-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osin-2.2.2.tar", max compression
+gzip compressed data, was "osin-2.2.3.tar", max compression
```

## Comparing `osin-2.2.2.tar` & `osin-2.2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1064 2023-12-22 08:13:43.741738 osin-2.2.2/LICENSE
--rw-r--r--   0        0        0     1367 2023-12-22 08:13:43.741738 osin-2.2.2/README.md
--rw-r--r--   0        0        0       93 2023-12-22 08:13:43.745738 osin-2.2.2/osin/__init__.py
--rw-r--r--   0        0        0     2651 2023-12-22 08:13:43.745738 osin-2.2.2/osin/__main__.py
--rw-r--r--   0        0        0        0 2023-12-22 08:13:43.745738 osin-2.2.2/osin/apis/__init__.py
--rw-r--r--   0        0        0     1537 2023-12-22 08:13:43.745738 osin-2.2.2/osin/apis/local_osin.py
--rw-r--r--   0        0        0    11387 2023-12-22 08:13:43.745738 osin-2.2.2/osin/apis/osin.py
--rw-r--r--   0        0        0     1808 2023-12-22 08:13:43.745738 osin-2.2.2/osin/apis/remote_exp.py
--rw-r--r--   0        0        0     6226 2023-12-22 08:13:43.745738 osin-2.2.2/osin/apis/remote_osin.py
--rw-r--r--   0        0        0      865 2023-12-22 08:13:43.745738 osin-2.2.2/osin/app.py
--rw-r--r--   0        0        0      243 2023-12-22 08:13:43.745738 osin-2.2.2/osin/config.py
--rw-r--r--   0        0        0        0 2023-12-22 08:13:43.745738 osin-2.2.2/osin/controllers/__init__.py
--rw-r--r--   0        0        0     5727 2023-12-22 08:13:43.745738 osin-2.2.2/osin/controllers/exp.py
--rw-r--r--   0        0        0    10281 2023-12-22 08:13:43.745738 osin-2.2.2/osin/controllers/report.py
--rw-r--r--   0        0        0      195 2023-12-22 08:13:43.745738 osin-2.2.2/osin/controllers/views.py
--rw-r--r--   0        0        0       41 2023-12-22 08:13:43.745738 osin-2.2.2/osin/formats/__init__.py
--rw-r--r--   0        0        0    10512 2023-12-22 08:13:43.745738 osin-2.2.2/osin/formats/hdf5.py
--rw-r--r--   0        0        0        0 2023-12-22 08:13:43.745738 osin-2.2.2/osin/integrations/__init__.py
--rw-r--r--   0        0        0     5258 2023-12-22 08:13:43.745738 osin-2.2.2/osin/integrations/ream.py
--rw-r--r--   0        0        0     3066 2023-12-22 08:13:43.745738 osin-2.2.2/osin/misc.py
--rw-r--r--   0        0        0      459 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/__init__.py
--rw-r--r--   0        0        0      904 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/base.py
--rw-r--r--   0        0        0     2896 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/exp.py
--rw-r--r--   0        0        0     1274 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/exp_data.py
--rw-r--r--   0        0        0        0 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/migration/__init__.py
--rw-r--r--   0        0        0      795 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/migration/v_1_6_2_1_7_0.backup
--rw-r--r--   0        0        0      536 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/report/__init__.py
--rw-r--r--   0        0        0     5450 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/report/auto_table.py
--rw-r--r--   0        0        0     3238 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/report/base_report.py
--rw-r--r--   0        0        0     1802 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/report/dbmodel.py
--rw-r--r--   0        0        0    15138 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/report/index_schema.py
--rw-r--r--   0        0        0     6765 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/report.py.backup
--rw-r--r--   0        0        0      411 2023-12-22 08:13:43.745738 osin-2.2.2/osin/models/views.py
--rw-r--r--   0        0        0     4763 2023-12-22 08:13:43.745738 osin-2.2.2/osin/params_helper.py
--rw-r--r--   0        0        0     2348 2023-12-22 08:13:43.745738 osin-2.2.2/osin/repository.py
--rw-r--r--   0        0        0      508 2023-12-22 08:13:43.745738 osin-2.2.2/osin/types/__init__.py
--rw-r--r--   0        0        0     2204 2023-12-22 08:13:43.745738 osin-2.2.2/osin/types/param_schema.py
--rw-r--r--   0        0        0     3845 2023-12-22 08:13:43.745738 osin-2.2.2/osin/types/primitive_type.py
--rw-r--r--   0        0        0     4029 2023-12-22 08:13:43.745738 osin-2.2.2/osin/types/pyobject/__init__.py
--rw-r--r--   0        0        0     1238 2023-12-22 08:13:43.745738 osin-2.2.2/osin/types/pyobject/base.py
--rw-r--r--   0        0        0     2229 2023-12-22 08:13:43.745738 osin-2.2.2/osin/types/pyobject/html.py
--rw-r--r--   0        0        0     3953 2023-12-22 08:13:43.745738 osin-2.2.2/osin/types/pyobject_type.py
--rw-r--r--   0        0        0      594 2023-12-22 08:13:43.745738 osin-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 osin-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-21 22:19:24.825613 osin-2.2.3/LICENSE
+-rw-r--r--   0        0        0     1367 2024-04-21 22:19:24.825613 osin-2.2.3/README.md
+-rw-r--r--   0        0        0       93 2024-04-21 22:19:24.825613 osin-2.2.3/osin/__init__.py
+-rw-r--r--   0        0        0     2651 2024-04-21 22:19:24.825613 osin-2.2.3/osin/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:19:24.825613 osin-2.2.3/osin/apis/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-21 22:19:24.825613 osin-2.2.3/osin/apis/local_osin.py
+-rw-r--r--   0        0        0    11387 2024-04-21 22:19:24.825613 osin-2.2.3/osin/apis/osin.py
+-rw-r--r--   0        0        0     1808 2024-04-21 22:19:24.825613 osin-2.2.3/osin/apis/remote_exp.py
+-rw-r--r--   0        0        0     6226 2024-04-21 22:19:24.825613 osin-2.2.3/osin/apis/remote_osin.py
+-rw-r--r--   0        0        0      865 2024-04-21 22:19:24.825613 osin-2.2.3/osin/app.py
+-rw-r--r--   0        0        0      243 2024-04-21 22:19:24.825613 osin-2.2.3/osin/config.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:19:24.825613 osin-2.2.3/osin/controllers/__init__.py
+-rw-r--r--   0        0        0     5727 2024-04-21 22:19:24.825613 osin-2.2.3/osin/controllers/exp.py
+-rw-r--r--   0        0        0    10281 2024-04-21 22:19:24.825613 osin-2.2.3/osin/controllers/report.py
+-rw-r--r--   0        0        0      195 2024-04-21 22:19:24.825613 osin-2.2.3/osin/controllers/views.py
+-rw-r--r--   0        0        0       41 2024-04-21 22:19:24.825613 osin-2.2.3/osin/formats/__init__.py
+-rw-r--r--   0        0        0    10512 2024-04-21 22:19:24.825613 osin-2.2.3/osin/formats/hdf5.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:19:24.825613 osin-2.2.3/osin/integrations/__init__.py
+-rw-r--r--   0        0        0     5258 2024-04-21 22:19:24.825613 osin-2.2.3/osin/integrations/ream.py
+-rw-r--r--   0        0        0     3066 2024-04-21 22:19:24.825613 osin-2.2.3/osin/misc.py
+-rw-r--r--   0        0        0      459 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/__init__.py
+-rw-r--r--   0        0        0      904 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/base.py
+-rw-r--r--   0        0        0     2896 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/exp.py
+-rw-r--r--   0        0        0     1274 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/exp_data.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/migration/__init__.py
+-rw-r--r--   0        0        0      795 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/migration/v_1_6_2_1_7_0.backup
+-rw-r--r--   0        0        0      536 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/report/__init__.py
+-rw-r--r--   0        0        0     5450 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/report/auto_table.py
+-rw-r--r--   0        0        0     3238 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/report/base_report.py
+-rw-r--r--   0        0        0     1802 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/report/dbmodel.py
+-rw-r--r--   0        0        0    15138 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/report/index_schema.py
+-rw-r--r--   0        0        0     6765 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/report.py.backup
+-rw-r--r--   0        0        0      411 2024-04-21 22:19:24.825613 osin-2.2.3/osin/models/views.py
+-rw-r--r--   0        0        0     4763 2024-04-21 22:19:24.825613 osin-2.2.3/osin/params_helper.py
+-rw-r--r--   0        0        0     2348 2024-04-21 22:19:24.825613 osin-2.2.3/osin/repository.py
+-rw-r--r--   0        0        0      508 2024-04-21 22:19:24.825613 osin-2.2.3/osin/types/__init__.py
+-rw-r--r--   0        0        0     2204 2024-04-21 22:19:24.825613 osin-2.2.3/osin/types/param_schema.py
+-rw-r--r--   0        0        0     3845 2024-04-21 22:19:24.825613 osin-2.2.3/osin/types/primitive_type.py
+-rw-r--r--   0        0        0     4029 2024-04-21 22:19:24.825613 osin-2.2.3/osin/types/pyobject/__init__.py
+-rw-r--r--   0        0        0     1238 2024-04-21 22:19:24.825613 osin-2.2.3/osin/types/pyobject/base.py
+-rw-r--r--   0        0        0     2229 2024-04-21 22:19:24.825613 osin-2.2.3/osin/types/pyobject/html.py
+-rw-r--r--   0        0        0     4134 2024-04-21 22:19:24.825613 osin-2.2.3/osin/types/pyobject_type.py
+-rw-r--r--   0        0        0      594 2024-04-21 22:19:24.825613 osin-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 osin-2.2.3/PKG-INFO
```

### Comparing `osin-2.2.2/LICENSE` & `osin-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/README.md` & `osin-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/__main__.py` & `osin-2.2.3/osin/__main__.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/apis/local_osin.py` & `osin-2.2.3/osin/apis/local_osin.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/apis/osin.py` & `osin-2.2.3/osin/apis/osin.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/apis/remote_exp.py` & `osin-2.2.3/osin/apis/remote_exp.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/apis/remote_osin.py` & `osin-2.2.3/osin/apis/remote_osin.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/app.py` & `osin-2.2.3/osin/app.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/controllers/exp.py` & `osin-2.2.3/osin/controllers/exp.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/controllers/report.py` & `osin-2.2.3/osin/controllers/report.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/formats/hdf5.py` & `osin-2.2.3/osin/formats/hdf5.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/integrations/ream.py` & `osin-2.2.3/osin/integrations/ream.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/misc.py` & `osin-2.2.3/osin/misc.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/models/base.py` & `osin-2.2.3/osin/models/base.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/models/exp.py` & `osin-2.2.3/osin/models/exp.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/models/exp_data.py` & `osin-2.2.3/osin/models/exp_data.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/models/migration/v_1_6_2_1_7_0.backup` & `osin-2.2.3/osin/models/migration/v_1_6_2_1_7_0.backup`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/models/report/__init__.py` & `osin-2.2.3/osin/models/report/__init__.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/models/report/auto_table.py` & `osin-2.2.3/osin/models/report/auto_table.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/models/report/base_report.py` & `osin-2.2.3/osin/models/report/base_report.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/models/report/dbmodel.py` & `osin-2.2.3/osin/models/report/dbmodel.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/models/report/index_schema.py` & `osin-2.2.3/osin/models/report/index_schema.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/models/report.py.backup` & `osin-2.2.3/osin/models/report.py.backup`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/params_helper.py` & `osin-2.2.3/osin/params_helper.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/repository.py` & `osin-2.2.3/osin/repository.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/types/param_schema.py` & `osin-2.2.3/osin/types/param_schema.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/types/primitive_type.py` & `osin-2.2.3/osin/types/primitive_type.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/types/pyobject/__init__.py` & `osin-2.2.3/osin/types/pyobject/__init__.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/types/pyobject/base.py` & `osin-2.2.3/osin/types/pyobject/base.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/types/pyobject/html.py` & `osin-2.2.3/osin/types/pyobject/html.py`

 * *Files identical despite different names*

### Comparing `osin-2.2.2/osin/types/pyobject_type.py` & `osin-2.2.3/osin/types/pyobject_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
+import types
 from dataclasses import dataclass
-from typing import Any, List, Union, get_args
+from typing import Any, List, Union, get_args, get_origin
 
 Number = Union[int, float]
 NoneType = type(None)
 TYPE_ALIASES = {"typing.List": "list", "typing.Dict": "dict", "typing.Set": "set"}
 INSTANCE_OF = {
     "str": lambda ptype, x: isinstance(x, str),
     "int": lambda ptype, x: isinstance(x, int),
@@ -37,15 +38,19 @@
             # typically a class from the typing module
             if hasattr(hint, "_name") and hint._name is not None:
                 path = hint.__module__ + "." + hint._name
             elif hasattr(hint, "__origin__") and hasattr(hint.__origin__, "_name"):
                 # found one case which is typing.Union
                 path = hint.__module__ + "." + hint.__origin__._name
             else:
-                raise NotImplementedError(hint)
+                origin = get_origin(hint)
+                if origin is types.UnionType:
+                    path = "typing.Union"
+                else:
+                    raise NotImplementedError(hint)
 
         if path in TYPE_ALIASES:
             # do it here because in python 3.10 typing.Dict has __qualname__
             path = TYPE_ALIASES[path]
 
         if path != "typing.Literal":
             args = [PyObjectType.from_type_hint(arg) for arg in get_args(hint)]
```

### Comparing `osin-2.2.2/pyproject.toml` & `osin-2.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "osin"
-version = "2.2.2"
+version = "2.2.3"
 description = "Research and Experiments"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `osin-2.2.2/PKG-INFO` & `osin-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osin
-Version: 2.2.2
+Version: 2.2.3
 Summary: Research and Experiments
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

