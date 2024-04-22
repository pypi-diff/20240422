# Comparing `tmp/one4all_iop_models-0.1.6.tar.gz` & `tmp/one4all_iop_models-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one4all_iop_models-0.1.6.tar", max compression
+gzip compressed data, was "one4all_iop_models-0.1.7.tar", max compression
```

## Comparing `one4all_iop_models-0.1.6.tar` & `one4all_iop_models-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      364 2024-04-09 08:49:13.446196 one4all_iop_models-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:49:13.446196 one4all_iop_models-0.1.6/one4all_iop_models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 08:49:13.446196 one4all_iop_models-0.1.6/one4all_iop_models/ros_models/__init__.py
--rw-r--r--   0        0        0     1518 2024-04-09 08:49:13.446196 one4all_iop_models-0.1.6/one4all_iop_models/ros_models/robot.py
--rw-r--r--   0        0        0      547 2024-04-09 08:49:13.446196 one4all_iop_models-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 one4all_iop_models-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      364 2024-04-22 06:18:47.078490 one4all_iop_models-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 06:18:47.078490 one4all_iop_models-0.1.7/one4all_iop_models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 06:18:47.078490 one4all_iop_models-0.1.7/one4all_iop_models/ros_models/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-22 06:18:47.078490 one4all_iop_models-0.1.7/one4all_iop_models/ros_models/robot.py
+-rw-r--r--   0        0        0      547 2024-04-22 06:18:47.078490 one4all_iop_models-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 one4all_iop_models-0.1.7/PKG-INFO
```

### Comparing `one4all_iop_models-0.1.6/pyproject.toml` & `one4all_iop_models-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "one4all-iop-models"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Ignacio Jimenez <ignacio.jimenez@idener.ai>"]
 readme = "README.md"
 packages = [{include = "one4all_iop_models"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `one4all_iop_models-0.1.6/PKG-INFO` & `one4all_iop_models-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one4all-iop-models
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Ignacio Jimenez
 Author-email: ignacio.jimenez@idener.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

