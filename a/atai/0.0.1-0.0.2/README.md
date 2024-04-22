# Comparing `tmp/atai-0.0.1.tar.gz` & `tmp/atai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atai-0.0.1.tar", last modified: Mon Apr 22 03:13:19 2024, max compression
+gzip compressed data, was "atai-0.0.2.tar", last modified: Mon Apr 22 03:58:09 2024, max compression
```

## Comparing `atai-0.0.1.tar` & `atai-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 frenio     (501) staff       (20)        0 2024-04-22 03:13:19.960564 atai-0.0.1/
--rw-r--r--   0 frenio     (501) staff       (20)    11357 2024-04-19 16:03:06.000000 atai-0.0.1/LICENSE
--rw-rw-r--   0 frenio     (501) staff       (20)      111 2023-04-27 10:12:58.000000 atai-0.0.1/MANIFEST.in
--rw-r--r--   0 frenio     (501) staff       (20)    25170 2024-04-22 03:13:19.960305 atai-0.0.1/PKG-INFO
--rw-r--r--   0 frenio     (501) staff       (20)    24345 2024-04-22 02:33:49.000000 atai-0.0.1/README.md
-drwxr-xr-x   0 frenio     (501) staff       (20)        0 2024-04-22 03:13:19.958445 atai-0.0.1/atai/
--rw-r--r--   0 frenio     (501) staff       (20)       22 2024-04-22 02:35:23.000000 atai-0.0.1/atai/__init__.py
--rw-r--r--   0 frenio     (501) staff       (20)    10985 2024-04-22 02:35:23.000000 atai-0.0.1/atai/_modidx.py
--rw-r--r--   0 frenio     (501) staff       (20)    17753 2024-04-22 02:35:23.000000 atai-0.0.1/atai/core.py
-drwxr-xr-x   0 frenio     (501) staff       (20)        0 2024-04-22 03:13:19.960029 atai-0.0.1/atai.egg-info/
--rw-r--r--   0 frenio     (501) staff       (20)    25170 2024-04-22 03:13:19.000000 atai-0.0.1/atai.egg-info/PKG-INFO
--rw-r--r--   0 frenio     (501) staff       (20)      294 2024-04-22 03:13:19.000000 atai-0.0.1/atai.egg-info/SOURCES.txt
--rw-r--r--   0 frenio     (501) staff       (20)        1 2024-04-22 03:13:19.000000 atai-0.0.1/atai.egg-info/dependency_links.txt
--rw-r--r--   0 frenio     (501) staff       (20)       30 2024-04-22 03:13:19.000000 atai-0.0.1/atai.egg-info/entry_points.txt
--rw-r--r--   0 frenio     (501) staff       (20)        1 2024-04-21 18:31:41.000000 atai-0.0.1/atai.egg-info/not-zip-safe
--rw-r--r--   0 frenio     (501) staff       (20)        7 2024-04-22 03:13:19.000000 atai-0.0.1/atai.egg-info/requires.txt
--rw-r--r--   0 frenio     (501) staff       (20)        5 2024-04-22 03:13:19.000000 atai-0.0.1/atai.egg-info/top_level.txt
--rw-r--r--   0 frenio     (501) staff       (20)     1016 2024-04-19 16:45:23.000000 atai-0.0.1/settings.ini
--rw-r--r--   0 frenio     (501) staff       (20)       38 2024-04-22 03:13:19.960626 atai-0.0.1/setup.cfg
--rw-rw-r--   0 frenio     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 atai-0.0.1/setup.py
+drwxr-xr-x   0 frenio     (501) staff       (20)        0 2024-04-22 03:58:09.209456 atai-0.0.2/
+-rw-r--r--   0 frenio     (501) staff       (20)    11357 2024-04-19 16:03:06.000000 atai-0.0.2/LICENSE
+-rw-rw-r--   0 frenio     (501) staff       (20)      111 2023-04-27 10:12:58.000000 atai-0.0.2/MANIFEST.in
+-rw-r--r--   0 frenio     (501) staff       (20)    25363 2024-04-22 03:58:09.209224 atai-0.0.2/PKG-INFO
+-rw-r--r--   0 frenio     (501) staff       (20)    24345 2024-04-22 02:33:49.000000 atai-0.0.2/README.md
+drwxr-xr-x   0 frenio     (501) staff       (20)        0 2024-04-22 03:58:09.207569 atai-0.0.2/atai/
+-rw-r--r--   0 frenio     (501) staff       (20)       22 2024-04-22 03:39:48.000000 atai-0.0.2/atai/__init__.py
+-rw-r--r--   0 frenio     (501) staff       (20)    10985 2024-04-22 03:57:04.000000 atai-0.0.2/atai/_modidx.py
+-rw-r--r--   0 frenio     (501) staff       (20)    17753 2024-04-22 03:39:48.000000 atai-0.0.2/atai/core.py
+drwxr-xr-x   0 frenio     (501) staff       (20)        0 2024-04-22 03:58:09.208975 atai-0.0.2/atai.egg-info/
+-rw-r--r--   0 frenio     (501) staff       (20)    25363 2024-04-22 03:58:09.000000 atai-0.0.2/atai.egg-info/PKG-INFO
+-rw-r--r--   0 frenio     (501) staff       (20)      294 2024-04-22 03:58:09.000000 atai-0.0.2/atai.egg-info/SOURCES.txt
+-rw-r--r--   0 frenio     (501) staff       (20)        1 2024-04-22 03:58:09.000000 atai-0.0.2/atai.egg-info/dependency_links.txt
+-rw-r--r--   0 frenio     (501) staff       (20)       30 2024-04-22 03:58:09.000000 atai-0.0.2/atai.egg-info/entry_points.txt
+-rw-r--r--   0 frenio     (501) staff       (20)        1 2024-04-21 18:31:41.000000 atai-0.0.2/atai.egg-info/not-zip-safe
+-rw-r--r--   0 frenio     (501) staff       (20)       80 2024-04-22 03:58:09.000000 atai-0.0.2/atai.egg-info/requires.txt
+-rw-r--r--   0 frenio     (501) staff       (20)        5 2024-04-22 03:58:09.000000 atai-0.0.2/atai.egg-info/top_level.txt
+-rw-r--r--   0 frenio     (501) staff       (20)     1071 2024-04-22 03:39:40.000000 atai-0.0.2/settings.ini
+-rw-r--r--   0 frenio     (501) staff       (20)       38 2024-04-22 03:58:09.209504 atai-0.0.2/setup.cfg
+-rw-rw-r--   0 frenio     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 atai-0.0.2/setup.py
```

### Comparing `atai-0.0.1/LICENSE` & `atai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atai-0.0.1/PKG-INFO` & `atai-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Atomic AI – An attempt at a minimalist, flexible deep learning framework for diverse models.
 Home-page: https://github.com/frenio/atai
 Author: Frenio Redeker
 Author-email: f.redeker@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: math
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: torch
+Requires-Dist: torcheval
+Requires-Dist: torchmetrics
+Requires-Dist: fastcore
+Requires-Dist: fastprogress
 Provides-Extra: dev
 
 # atai
 
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
```

### Comparing `atai-0.0.1/README.md` & `atai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `atai-0.0.1/atai/_modidx.py` & `atai-0.0.2/atai/_modidx.py`

 * *Files identical despite different names*

### Comparing `atai-0.0.1/atai/core.py` & `atai-0.0.2/atai/core.py`

 * *Files identical despite different names*

### Comparing `atai-0.0.1/atai.egg-info/PKG-INFO` & `atai-0.0.2/atai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Atomic AI – An attempt at a minimalist, flexible deep learning framework for diverse models.
 Home-page: https://github.com/frenio/atai
 Author: Frenio Redeker
 Author-email: f.redeker@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: math
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: torch
+Requires-Dist: torcheval
+Requires-Dist: torchmetrics
+Requires-Dist: fastcore
+Requires-Dist: fastprogress
 Provides-Extra: dev
 
 # atai
 
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
```

### Comparing `atai-0.0.1/settings.ini` & `atai-0.0.2/settings.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = atai 
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = %(lib_name)s
@@ -34,10 +34,10 @@
 description = Atomic AI – An attempt at a minimalist, flexible deep learning framework for diverse models.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = frenio
 
 ### Optional ###
-# requirements = fastcore pandas
+requirements = math matplotlib numpy torch torcheval torchmetrics fastcore fastprogress
 # dev_requirements = 
 # console_scripts =
```

### Comparing `atai-0.0.1/setup.py` & `atai-0.0.2/setup.py`

 * *Files identical despite different names*

