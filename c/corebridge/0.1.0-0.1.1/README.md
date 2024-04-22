# Comparing `tmp/corebridge-0.1.0.tar.gz` & `tmp/corebridge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.1.0.tar", last modified: Wed Apr 17 14:53:26 2024, max compression
+gzip compressed data, was "corebridge-0.1.1.tar", last modified: Mon Apr 22 08:18:29 2024, max compression
```

## Comparing `corebridge-0.1.0.tar` & `corebridge-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-17 14:53:26.860277 corebridge-0.1.0/
--rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.1.0/LICENSE
--rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.1.0/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-17 14:53:26.860277 corebridge-0.1.0/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      435 2024-04-17 14:51:56.000000 corebridge-0.1.0/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-17 14:53:26.860277 corebridge-0.1.0/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)       22 2024-04-17 14:52:06.000000 corebridge-0.1.0/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)     3300 2024-04-17 14:52:06.000000 corebridge-0.1.0/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)     8155 2024-04-17 14:52:06.000000 corebridge-0.1.0/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)     3766 2024-04-17 14:52:06.000000 corebridge-0.1.0/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-17 14:53:26.860277 corebridge-0.1.0/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.1.0/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      225 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2024-04-17 14:53:26.000000 corebridge-0.1.0/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1146 2024-04-17 14:47:59.000000 corebridge-0.1.0/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2024-04-17 14:53:26.860277 corebridge-0.1.0/setup.cfg
--rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.1.0/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-22 08:18:29.386892 corebridge-0.1.1/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.1.1/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.1.1/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-22 08:18:29.386892 corebridge-0.1.1/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      435 2024-04-17 14:51:56.000000 corebridge-0.1.1/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-22 08:18:29.386892 corebridge-0.1.1/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)       22 2024-04-22 08:18:10.000000 corebridge-0.1.1/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     3300 2024-04-22 08:18:10.000000 corebridge-0.1.1/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     8155 2024-04-22 08:18:10.000000 corebridge-0.1.1/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     3766 2024-04-22 08:18:10.000000 corebridge-0.1.1/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-22 08:18:29.386892 corebridge-0.1.1/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.1.1/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      225 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-04-22 08:18:29.000000 corebridge-0.1.1/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1146 2024-04-22 08:17:53.000000 corebridge-0.1.1/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-04-22 08:18:29.386892 corebridge-0.1.1/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.1.1/setup.py
```

### Comparing `corebridge-0.1.0/LICENSE` & `corebridge-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.1.0/PKG-INFO` & `corebridge-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.1.0
+Version: 0.1.1
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.1.0/corebridge/_modidx.py` & `corebridge-0.1.1/corebridge/_modidx.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.1.0/corebridge/aicorebridge.py` & `corebridge-0.1.1/corebridge/aicorebridge.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 
 # %% ../nbs/01_aicorebridge.ipynb 6
 class AICoreModule(): pass
 
 # %% ../nbs/01_aicorebridge.ipynb 7
 @patch
 def __init__(self:AICoreModule, 
+             processor:typing.Callable, # data processing function
              save_dir:str, # path where the module can keep files 
              assets_dir:str,
-             processor:typing.Callable, # data processing function
              *args, **kwargs):
     
     self.save_dir  = save_dir
     self.assets_dir  = assets_dir
     self._init_processor(processor)
 
     self.init_args = args
```

### Comparing `corebridge-0.1.0/corebridge/core.py` & `corebridge-0.1.1/corebridge/core.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.1.0/corebridge.egg-info/PKG-INFO` & `corebridge-0.1.1/corebridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.1.0
+Version: 0.1.1
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.1.0/settings.ini` & `corebridge-0.1.1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.1.0
+version = 0.1.1
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
```

### Comparing `corebridge-0.1.0/setup.py` & `corebridge-0.1.1/setup.py`

 * *Files identical despite different names*

