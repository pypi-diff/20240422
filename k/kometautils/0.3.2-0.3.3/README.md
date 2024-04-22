# Comparing `tmp/kometautils-0.3.2.tar.gz` & `tmp/kometautils-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kometautils-0.3.2.tar", last modified: Sun Apr 21 19:32:08 2024, max compression
+gzip compressed data, was "kometautils-0.3.3.tar", last modified: Sun Apr 21 19:43:21 2024, max compression
```

## Comparing `kometautils-0.3.2.tar` & `kometautils-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:32:08.759146 kometautils-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 19:31:58.000000 kometautils-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-21 19:32:08.759146 kometautils-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-21 19:31:58.000000 kometautils-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:32:08.759146 kometautils-0.3.2/kometautils/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/args.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    31561 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-21 19:31:58.000000 kometautils-0.3.2/kometautils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:32:08.759146 kometautils-0.3.2/kometautils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-21 19:32:08.000000 kometautils-0.3.2/kometautils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-21 19:32:08.000000 kometautils-0.3.2/kometautils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:32:08.000000 kometautils-0.3.2/kometautils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-21 19:32:08.000000 kometautils-0.3.2/kometautils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 19:32:08.000000 kometautils-0.3.2/kometautils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:32:08.759146 kometautils-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-21 19:31:58.000000 kometautils-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:43:21.089740 kometautils-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 19:43:09.000000 kometautils-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-21 19:43:21.089740 kometautils-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-21 19:43:09.000000 kometautils-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:43:21.085740 kometautils-0.3.3/kometautils/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-21 19:43:09.000000 kometautils-0.3.3/kometautils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-21 19:43:09.000000 kometautils-0.3.3/kometautils/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-21 19:43:09.000000 kometautils-0.3.3/kometautils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-04-21 19:43:09.000000 kometautils-0.3.3/kometautils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31561 2024-04-21 19:43:09.000000 kometautils-0.3.3/kometautils/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-21 19:43:09.000000 kometautils-0.3.3/kometautils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-21 19:43:09.000000 kometautils-0.3.3/kometautils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:43:21.089740 kometautils-0.3.3/kometautils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-21 19:43:21.000000 kometautils-0.3.3/kometautils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-21 19:43:21.000000 kometautils-0.3.3/kometautils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:43:21.000000 kometautils-0.3.3/kometautils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-21 19:43:21.000000 kometautils-0.3.3/kometautils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 19:43:21.000000 kometautils-0.3.3/kometautils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:43:21.089740 kometautils-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-21 19:43:09.000000 kometautils-0.3.3/setup.py
```

### Comparing `kometautils-0.3.2/LICENSE` & `kometautils-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.2/PKG-INFO` & `kometautils-0.3.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kometautils
-Version: 0.3.2
+Version: 0.3.3
 Summary: Util Methods for Kometa
 Home-page: https://github.com/Kometa-Team/Kometa-Utils
 Author: Nathan Taggart
 Author-email: kometateam@proton.me
 License: MIT License
 Project-URL: Documentation, https://github.com/Kometa-Team/Kometa-Utils
 Project-URL: Funding, https://github.com/sponsors/meisnate12
@@ -31,20 +31,20 @@
 Kometa Utils
 ==========================================================
 
 .. image:: https://img.shields.io/github/v/release/Kometa-Team/Kometa-Utils?style=plastic
     :target: https://github.com/Kometa-Team/Kometa-Utils/releases
     :alt: GitHub release (latest by date)
 
-.. image:: https://img.shields.io/pypi/v/kometa-utils?style=plastic
-    :target: https://pypi.org/project/kometa-utils/
+.. image:: https://img.shields.io/pypi/v/kometautils?style=plastic
+    :target: https://pypi.org/project/kometautils/
     :alt: PyPI
 
-.. image:: https://img.shields.io/pypi/dm/kometa-utils.svg?style=plastic
-    :target: https://pypi.org/project/kometa-utils/
+.. image:: https://img.shields.io/pypi/dm/kometautils.svg?style=plastic
+    :target: https://pypi.org/project/kometautils/
     :alt: Downloads
 
 .. image:: https://img.shields.io/github/commits-since/Kometa-Team/Kometa-Utils/latest?style=plastic
     :target: https://github.com/Kometa-Team/Kometa-Utils/commits/master
     :alt: GitHub commits since latest release (by date) for a branch
 
 .. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
```

### Comparing `kometautils-0.3.2/README.rst` & `kometautils-0.3.3/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Kometa Utils
 ==========================================================
 
 .. image:: https://img.shields.io/github/v/release/Kometa-Team/Kometa-Utils?style=plastic
     :target: https://github.com/Kometa-Team/Kometa-Utils/releases
     :alt: GitHub release (latest by date)
 
-.. image:: https://img.shields.io/pypi/v/kometa-utils?style=plastic
-    :target: https://pypi.org/project/kometa-utils/
+.. image:: https://img.shields.io/pypi/v/kometautils?style=plastic
+    :target: https://pypi.org/project/kometautils/
     :alt: PyPI
 
-.. image:: https://img.shields.io/pypi/dm/kometa-utils.svg?style=plastic
-    :target: https://pypi.org/project/kometa-utils/
+.. image:: https://img.shields.io/pypi/dm/kometautils.svg?style=plastic
+    :target: https://pypi.org/project/kometautils/
     :alt: Downloads
 
 .. image:: https://img.shields.io/github/commits-since/Kometa-Team/Kometa-Utils/latest?style=plastic
     :target: https://github.com/Kometa-Team/Kometa-Utils/commits/master
     :alt: GitHub commits since latest release (by date) for a branch
 
 .. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
```

### Comparing `kometautils-0.3.2/kometautils/__init__.py` & `kometautils-0.3.3/kometautils/__init__.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.2/kometautils/args.py` & `kometautils-0.3.3/kometautils/args.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.2/kometautils/logging.py` & `kometautils-0.3.3/kometautils/logging.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.2/kometautils/schedule.py` & `kometautils-0.3.3/kometautils/schedule.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.2/kometautils/util.py` & `kometautils-0.3.3/kometautils/util.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.2/kometautils/yaml.py` & `kometautils-0.3.3/kometautils/yaml.py`

 * *Files identical despite different names*

### Comparing `kometautils-0.3.2/kometautils.egg-info/PKG-INFO` & `kometautils-0.3.3/kometautils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kometautils
-Version: 0.3.2
+Version: 0.3.3
 Summary: Util Methods for Kometa
 Home-page: https://github.com/Kometa-Team/Kometa-Utils
 Author: Nathan Taggart
 Author-email: kometateam@proton.me
 License: MIT License
 Project-URL: Documentation, https://github.com/Kometa-Team/Kometa-Utils
 Project-URL: Funding, https://github.com/sponsors/meisnate12
@@ -31,20 +31,20 @@
 Kometa Utils
 ==========================================================
 
 .. image:: https://img.shields.io/github/v/release/Kometa-Team/Kometa-Utils?style=plastic
     :target: https://github.com/Kometa-Team/Kometa-Utils/releases
     :alt: GitHub release (latest by date)
 
-.. image:: https://img.shields.io/pypi/v/kometa-utils?style=plastic
-    :target: https://pypi.org/project/kometa-utils/
+.. image:: https://img.shields.io/pypi/v/kometautils?style=plastic
+    :target: https://pypi.org/project/kometautils/
     :alt: PyPI
 
-.. image:: https://img.shields.io/pypi/dm/kometa-utils.svg?style=plastic
-    :target: https://pypi.org/project/kometa-utils/
+.. image:: https://img.shields.io/pypi/dm/kometautils.svg?style=plastic
+    :target: https://pypi.org/project/kometautils/
     :alt: Downloads
 
 .. image:: https://img.shields.io/github/commits-since/Kometa-Team/Kometa-Utils/latest?style=plastic
     :target: https://github.com/Kometa-Team/Kometa-Utils/commits/master
     :alt: GitHub commits since latest release (by date) for a branch
 
 .. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
```

### Comparing `kometautils-0.3.2/setup.py` & `kometautils-0.3.3/setup.py`

 * *Files identical despite different names*

