# Comparing `tmp/iap_cli-2024.3a2.tar.gz` & `tmp/iap_cli-2024.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iap_cli-2024.3a2.tar", last modified: Tue Mar 26 15:27:07 2024, max compression
+gzip compressed data, was "iap_cli-2024.4a1.tar", last modified: Mon Apr 22 08:30:44 2024, max compression
```

## Comparing `iap_cli-2024.3a2.tar` & `iap_cli-2024.4a1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-03-26 15:27:07.409692 iap_cli-2024.3a2/
--rw-r--r--   0 jfrauchi   (502) staff       (20)     1072 2024-01-12 11:29:07.000000 iap_cli-2024.3a2/LICENSE
--rw-r--r--   0 jfrauchi   (502) staff       (20)       79 2024-01-12 11:29:07.000000 iap_cli-2024.3a2/MANIFEST.in
--rw-r--r--   0 jfrauchi   (502) staff       (20)    13605 2024-03-26 15:27:07.409014 iap_cli-2024.3a2/PKG-INFO
--rw-r--r--   0 jfrauchi   (502) staff       (20)    12340 2024-01-12 16:25:03.000000 iap_cli-2024.3a2/README.md
-drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-03-26 15:27:07.401886 iap_cli-2024.3a2/iap_cli/
--rw-r--r--   0 jfrauchi   (502) staff       (20)       42 2024-01-12 11:29:07.000000 iap_cli-2024.3a2/iap_cli/__init__.py
--rw-r--r--   0 jfrauchi   (502) staff       (20)      129 2024-01-12 11:29:07.000000 iap_cli-2024.3a2/iap_cli/__main__.py
-drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-03-26 15:27:07.404679 iap_cli-2024.3a2/iap_cli/commands/
--rw-r--r--   0 jfrauchi   (502) staff       (20)        0 2024-01-12 11:29:07.000000 iap_cli-2024.3a2/iap_cli/commands/__init__.py
--rw-r--r--   0 jfrauchi   (502) staff       (20)      743 2024-03-26 15:25:46.000000 iap_cli-2024.3a2/iap_cli/commands/app.py
-drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-03-26 15:27:07.405648 iap_cli-2024.3a2/iap_cli/commands/config/
--rw-r--r--   0 jfrauchi   (502) staff       (20)        0 2024-01-12 11:29:07.000000 iap_cli-2024.3a2/iap_cli/commands/config/__init__.py
--rw-r--r--   0 jfrauchi   (502) staff       (20)     3234 2024-03-23 12:41:10.000000 iap_cli-2024.3a2/iap_cli/commands/config/add.py
--rw-r--r--   0 jfrauchi   (502) staff       (20)      934 2024-03-23 12:26:11.000000 iap_cli-2024.3a2/iap_cli/commands/config/app.py
-drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-03-26 15:27:07.406296 iap_cli-2024.3a2/iap_cli/commands/get/
--rw-r--r--   0 jfrauchi   (502) staff       (20)        0 2024-01-12 11:29:07.000000 iap_cli-2024.3a2/iap_cli/commands/get/__init__.py
--rw-r--r--   0 jfrauchi   (502) staff       (20)     5630 2024-03-26 15:21:48.000000 iap_cli-2024.3a2/iap_cli/commands/get/app.py
-drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-03-26 15:27:07.406936 iap_cli-2024.3a2/iap_cli/commands/restart/
--rw-r--r--   0 jfrauchi   (502) staff       (20)        0 2024-01-12 11:29:07.000000 iap_cli-2024.3a2/iap_cli/commands/restart/__init__.py
--rw-r--r--   0 jfrauchi   (502) staff       (20)     3250 2024-03-23 12:51:22.000000 iap_cli-2024.3a2/iap_cli/commands/restart/app.py
--rw-r--r--   0 jfrauchi   (502) staff       (20)      311 2024-03-23 12:21:55.000000 iap_cli-2024.3a2/iap_cli/config.py
--rw-r--r--   0 jfrauchi   (502) staff       (20)      584 2024-03-23 12:21:38.000000 iap_cli-2024.3a2/iap_cli/enums.py
-drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-03-26 15:27:07.407645 iap_cli-2024.3a2/iap_cli/models/
--rw-r--r--   0 jfrauchi   (502) staff       (20)      470 2024-03-23 12:22:28.000000 iap_cli-2024.3a2/iap_cli/models/enums.py
--rw-r--r--   0 jfrauchi   (502) staff       (20)     2139 2024-03-23 12:28:41.000000 iap_cli-2024.3a2/iap_cli/models/iap.py
--rw-r--r--   0 jfrauchi   (502) staff       (20)     4936 2024-03-23 12:41:57.000000 iap_cli-2024.3a2/iap_cli/utils.py
-drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-03-26 15:27:07.408183 iap_cli-2024.3a2/iap_cli.egg-info/
--rw-r--r--   0 jfrauchi   (502) staff       (20)    13605 2024-03-26 15:27:07.000000 iap_cli-2024.3a2/iap_cli.egg-info/PKG-INFO
--rw-r--r--   0 jfrauchi   (502) staff       (20)      660 2024-03-26 15:27:07.000000 iap_cli-2024.3a2/iap_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jfrauchi   (502) staff       (20)        1 2024-03-26 15:27:07.000000 iap_cli-2024.3a2/iap_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jfrauchi   (502) staff       (20)       36 2024-03-26 15:27:07.000000 iap_cli-2024.3a2/iap_cli.egg-info/entry_points.txt
--rw-r--r--   0 jfrauchi   (502) staff       (20)      147 2024-03-26 15:27:07.000000 iap_cli-2024.3a2/iap_cli.egg-info/requires.txt
--rw-r--r--   0 jfrauchi   (502) staff       (20)        8 2024-03-26 15:27:07.000000 iap_cli-2024.3a2/iap_cli.egg-info/top_level.txt
--rw-r--r--   0 jfrauchi   (502) staff       (20)      107 2024-01-12 11:29:07.000000 iap_cli-2024.3a2/pyproject.toml
--rw-r--r--   0 jfrauchi   (502) staff       (20)       38 2024-03-26 15:27:07.409754 iap_cli-2024.3a2/setup.cfg
--rw-r--r--   0 jfrauchi   (502) staff       (20)     1654 2024-03-26 15:25:22.000000 iap_cli-2024.3a2/setup.py
+drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-04-22 08:30:44.352030 iap_cli-2024.4a1/
+-rw-r--r--   0 jfrauchi   (502) staff       (20)     1072 2024-01-12 11:29:07.000000 iap_cli-2024.4a1/LICENSE
+-rw-r--r--   0 jfrauchi   (502) staff       (20)       79 2024-01-12 11:29:07.000000 iap_cli-2024.4a1/MANIFEST.in
+-rw-r--r--   0 jfrauchi   (502) staff       (20)    13605 2024-04-22 08:30:44.351512 iap_cli-2024.4a1/PKG-INFO
+-rw-r--r--   0 jfrauchi   (502) staff       (20)    12340 2024-01-12 16:25:03.000000 iap_cli-2024.4a1/README.md
+drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-04-22 08:30:44.344556 iap_cli-2024.4a1/iap_cli/
+-rw-r--r--   0 jfrauchi   (502) staff       (20)       42 2024-01-12 11:29:07.000000 iap_cli-2024.4a1/iap_cli/__init__.py
+-rw-r--r--   0 jfrauchi   (502) staff       (20)      129 2024-01-12 11:29:07.000000 iap_cli-2024.4a1/iap_cli/__main__.py
+drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-04-22 08:30:44.347195 iap_cli-2024.4a1/iap_cli/commands/
+-rw-r--r--   0 jfrauchi   (502) staff       (20)        0 2024-01-12 11:29:07.000000 iap_cli-2024.4a1/iap_cli/commands/__init__.py
+-rw-r--r--   0 jfrauchi   (502) staff       (20)      743 2024-04-22 08:28:51.000000 iap_cli-2024.4a1/iap_cli/commands/app.py
+drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-04-22 08:30:44.348232 iap_cli-2024.4a1/iap_cli/commands/config/
+-rw-r--r--   0 jfrauchi   (502) staff       (20)        0 2024-01-12 11:29:07.000000 iap_cli-2024.4a1/iap_cli/commands/config/__init__.py
+-rw-r--r--   0 jfrauchi   (502) staff       (20)     3234 2024-03-23 12:41:10.000000 iap_cli-2024.4a1/iap_cli/commands/config/add.py
+-rw-r--r--   0 jfrauchi   (502) staff       (20)      934 2024-03-23 12:26:11.000000 iap_cli-2024.4a1/iap_cli/commands/config/app.py
+drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-04-22 08:30:44.348877 iap_cli-2024.4a1/iap_cli/commands/get/
+-rw-r--r--   0 jfrauchi   (502) staff       (20)        0 2024-01-12 11:29:07.000000 iap_cli-2024.4a1/iap_cli/commands/get/__init__.py
+-rw-r--r--   0 jfrauchi   (502) staff       (20)     5630 2024-03-26 15:21:48.000000 iap_cli-2024.4a1/iap_cli/commands/get/app.py
+drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-04-22 08:30:44.349641 iap_cli-2024.4a1/iap_cli/commands/restart/
+-rw-r--r--   0 jfrauchi   (502) staff       (20)        0 2024-01-12 11:29:07.000000 iap_cli-2024.4a1/iap_cli/commands/restart/__init__.py
+-rw-r--r--   0 jfrauchi   (502) staff       (20)     3250 2024-03-23 12:51:22.000000 iap_cli-2024.4a1/iap_cli/commands/restart/app.py
+-rw-r--r--   0 jfrauchi   (502) staff       (20)      311 2024-03-23 12:21:55.000000 iap_cli-2024.4a1/iap_cli/config.py
+-rw-r--r--   0 jfrauchi   (502) staff       (20)      584 2024-03-23 12:21:38.000000 iap_cli-2024.4a1/iap_cli/enums.py
+drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-04-22 08:30:44.350369 iap_cli-2024.4a1/iap_cli/models/
+-rw-r--r--   0 jfrauchi   (502) staff       (20)      500 2024-04-22 08:22:43.000000 iap_cli-2024.4a1/iap_cli/models/enums.py
+-rw-r--r--   0 jfrauchi   (502) staff       (20)     2139 2024-03-23 12:28:41.000000 iap_cli-2024.4a1/iap_cli/models/iap.py
+-rw-r--r--   0 jfrauchi   (502) staff       (20)     4936 2024-03-23 12:41:57.000000 iap_cli-2024.4a1/iap_cli/utils.py
+drwxr-xr-x   0 jfrauchi   (502) staff       (20)        0 2024-04-22 08:30:44.351073 iap_cli-2024.4a1/iap_cli.egg-info/
+-rw-r--r--   0 jfrauchi   (502) staff       (20)    13605 2024-04-22 08:30:44.000000 iap_cli-2024.4a1/iap_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jfrauchi   (502) staff       (20)      660 2024-04-22 08:30:44.000000 iap_cli-2024.4a1/iap_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jfrauchi   (502) staff       (20)        1 2024-04-22 08:30:44.000000 iap_cli-2024.4a1/iap_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jfrauchi   (502) staff       (20)       36 2024-04-22 08:30:44.000000 iap_cli-2024.4a1/iap_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jfrauchi   (502) staff       (20)      147 2024-04-22 08:30:44.000000 iap_cli-2024.4a1/iap_cli.egg-info/requires.txt
+-rw-r--r--   0 jfrauchi   (502) staff       (20)        8 2024-04-22 08:30:44.000000 iap_cli-2024.4a1/iap_cli.egg-info/top_level.txt
+-rw-r--r--   0 jfrauchi   (502) staff       (20)      107 2024-01-12 11:29:07.000000 iap_cli-2024.4a1/pyproject.toml
+-rw-r--r--   0 jfrauchi   (502) staff       (20)       38 2024-04-22 08:30:44.352085 iap_cli-2024.4a1/setup.cfg
+-rw-r--r--   0 jfrauchi   (502) staff       (20)     1654 2024-04-22 08:28:11.000000 iap_cli-2024.4a1/setup.py
```

### Comparing `iap_cli-2024.3a2/LICENSE` & `iap_cli-2024.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `iap_cli-2024.3a2/PKG-INFO` & `iap_cli-2024.4a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iap_cli
-Version: 2024.3a2
+Version: 2024.4a1
 Summary: Lightweight CLI tool to simplify the process of interacting with the Itential Automation Platform.
 Home-page: https://github.com/awetomate/itential-iap-cli
 Author: John Frauchiger
 Author-email: john@awetomate.net
 License: MIT
 Project-URL: Documentation, https://github.com/awetomate/itential-iap-cli
 Project-URL: Source, https://github.com/awetomate/itential-iap-cli
```

### Comparing `iap_cli-2024.3a2/README.md` & `iap_cli-2024.4a1/README.md`

 * *Files identical despite different names*

### Comparing `iap_cli-2024.3a2/iap_cli/commands/app.py` & `iap_cli-2024.4a1/iap_cli/commands/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Main Typer app for root commands
 """
 
-__version__ = "2024.3a2"
+__version__ = "2024.4a1"
 
 import typer
 from rich import print
 
 from iap_cli.commands.config.app import config_app
 from iap_cli.commands.get.app import get_app
 from iap_cli.commands.restart.app import restart_app
```

### Comparing `iap_cli-2024.3a2/iap_cli/commands/config/add.py` & `iap_cli-2024.4a1/iap_cli/commands/config/add.py`

 * *Files identical despite different names*

### Comparing `iap_cli-2024.3a2/iap_cli/commands/config/app.py` & `iap_cli-2024.4a1/iap_cli/commands/config/app.py`

 * *Files identical despite different names*

### Comparing `iap_cli-2024.3a2/iap_cli/commands/get/app.py` & `iap_cli-2024.4a1/iap_cli/commands/get/app.py`

 * *Files identical despite different names*

### Comparing `iap_cli-2024.3a2/iap_cli/commands/restart/app.py` & `iap_cli-2024.4a1/iap_cli/commands/restart/app.py`

 * *Files identical despite different names*

### Comparing `iap_cli-2024.3a2/iap_cli/enums.py` & `iap_cli-2024.4a1/iap_cli/enums.py`

 * *Files identical despite different names*

### Comparing `iap_cli-2024.3a2/iap_cli/models/iap.py` & `iap_cli-2024.4a1/iap_cli/models/iap.py`

 * *Files identical despite different names*

### Comparing `iap_cli-2024.3a2/iap_cli/utils.py` & `iap_cli-2024.4a1/iap_cli/utils.py`

 * *Files identical despite different names*

### Comparing `iap_cli-2024.3a2/iap_cli.egg-info/PKG-INFO` & `iap_cli-2024.4a1/iap_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iap_cli
-Version: 2024.3a2
+Version: 2024.4a1
 Summary: Lightweight CLI tool to simplify the process of interacting with the Itential Automation Platform.
 Home-page: https://github.com/awetomate/itential-iap-cli
 Author: John Frauchiger
 Author-email: john@awetomate.net
 License: MIT
 Project-URL: Documentation, https://github.com/awetomate/itential-iap-cli
 Project-URL: Source, https://github.com/awetomate/itential-iap-cli
```

### Comparing `iap_cli-2024.3a2/iap_cli.egg-info/SOURCES.txt` & `iap_cli-2024.4a1/iap_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iap_cli-2024.3a2/setup.py` & `iap_cli-2024.4a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 import setuptools
 
 setuptools.setup(
     name="iap_cli",
-    version="2024.3a2",
+    version="2024.4a1",
     description="Lightweight CLI tool to simplify the process of interacting with the Itential Automation Platform.",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/awetomate/itential-iap-cli",
     author="John Frauchiger",
     author_email="john@awetomate.net",
     license="MIT",
```

