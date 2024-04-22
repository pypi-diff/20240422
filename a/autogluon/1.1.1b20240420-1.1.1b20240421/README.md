# Comparing `tmp/autogluon-1.1.1b20240420.tar.gz` & `tmp/autogluon-1.1.1b20240421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.1.1b20240420.tar", last modified: Sat Apr 20 09:05:05 2024, max compression
+gzip compressed data, was "autogluon-1.1.1b20240421.tar", last modified: Sun Apr 21 09:04:59 2024, max compression
```

## Comparing `autogluon-1.1.1b20240420.tar` & `autogluon-1.1.1b20240421.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:05:05.312713 autogluon-1.1.1b20240420/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-20 09:05:05.312713 autogluon-1.1.1b20240420/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 09:05:05.312713 autogluon-1.1.1b20240420/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-20 09:03:29.000000 autogluon-1.1.1b20240420/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:05:05.312713 autogluon-1.1.1b20240420/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:05:05.312713 autogluon-1.1.1b20240420/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:05:05.312713 autogluon-1.1.1b20240420/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 09:03:29.000000 autogluon-1.1.1b20240420/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:05:05.312713 autogluon-1.1.1b20240420/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-20 09:05:05.000000 autogluon-1.1.1b20240420/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-20 09:05:05.000000 autogluon-1.1.1b20240420/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:05:05.000000 autogluon-1.1.1b20240420/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 09:05:05.000000 autogluon-1.1.1b20240420/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-20 09:05:05.000000 autogluon-1.1.1b20240420/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 09:05:05.000000 autogluon-1.1.1b20240420/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:05:05.000000 autogluon-1.1.1b20240420/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:04:59.001351 autogluon-1.1.1b20240421/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-21 09:04:59.001351 autogluon-1.1.1b20240421/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:04:59.001351 autogluon-1.1.1b20240421/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-21 09:03:31.000000 autogluon-1.1.1b20240421/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:04:59.001351 autogluon-1.1.1b20240421/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:04:59.001351 autogluon-1.1.1b20240421/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:04:59.001351 autogluon-1.1.1b20240421/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:03:31.000000 autogluon-1.1.1b20240421/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:04:59.001351 autogluon-1.1.1b20240421/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-21 09:04:58.000000 autogluon-1.1.1b20240421/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-21 09:04:58.000000 autogluon-1.1.1b20240421/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:04:58.000000 autogluon-1.1.1b20240421/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 09:04:58.000000 autogluon-1.1.1b20240421/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-21 09:04:58.000000 autogluon-1.1.1b20240421/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 09:04:58.000000 autogluon-1.1.1b20240421/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:04:58.000000 autogluon-1.1.1b20240421/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.1.1b20240420/PKG-INFO` & `autogluon-1.1.1b20240421/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240420
+Version: 1.1.1b20240421
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-1.1.1b20240420/setup.py` & `autogluon-1.1.1b20240421/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.1.1b20240420/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.1.1b20240421/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240420
+Version: 1.1.1b20240421
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

