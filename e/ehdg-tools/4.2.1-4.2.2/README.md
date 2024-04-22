# Comparing `tmp/ehdg_tools-4.2.1.tar.gz` & `tmp/ehdg_tools-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_tools-4.2.1.tar", last modified: Wed Apr 17 02:36:08 2024, max compression
+gzip compressed data, was "ehdg_tools-4.2.2.tar", last modified: Mon Apr 22 04:37:30 2024, max compression
```

## Comparing `ehdg_tools-4.2.1.tar` & `ehdg_tools-4.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 02:36:08.925077 ehdg_tools-4.2.1/
--rw-rw-rw-   0        0        0    11558 2023-11-17 13:32:14.000000 ehdg_tools-4.2.1/LICENSE
--rw-rw-rw-   0        0        0     3001 2024-04-17 02:36:08.924078 ehdg_tools-4.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2436 2023-11-22 03:02:06.000000 ehdg_tools-4.2.1/README.md
--rw-rw-rw-   0        0        0      699 2024-04-17 02:35:26.000000 ehdg_tools-4.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 02:36:08.925077 ehdg_tools-4.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 02:36:08.896775 ehdg_tools-4.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 02:36:08.906657 ehdg_tools-4.2.1/src/ehdg_tools/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_tools-4.2.1/src/ehdg_tools/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-11-21 22:16:22.000000 ehdg_tools-4.2.1/src/ehdg_tools/ehdg_buffers.py
--rw-rw-rw-   0        0        0      530 2023-12-04 12:16:10.000000 ehdg_tools-4.2.1/src/ehdg_tools/ehdg_functions.py
--rw-rw-rw-   0        0        0     5831 2024-01-30 22:28:51.000000 ehdg_tools-4.2.1/src/ehdg_tools/ehdg_okn_checker.py
--rw-rw-rw-   0        0        0   117333 2024-04-17 02:32:38.000000 ehdg_tools-4.2.1/src/ehdg_tools/ehdg_plotter.py
--rw-rw-rw-   0        0        0    13490 2023-11-29 22:43:57.000000 ehdg_tools-4.2.1/src/ehdg_tools/ehdg_updater.py
-drwxrwxrwx   0        0        0        0 2024-04-17 02:36:08.922084 ehdg_tools-4.2.1/src/ehdg_tools.egg-info/
--rw-rw-rw-   0        0        0     3001 2024-04-17 02:36:08.000000 ehdg_tools-4.2.1/src/ehdg_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-04-17 02:36:08.000000 ehdg_tools-4.2.1/src/ehdg_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:36:08.000000 ehdg_tools-4.2.1/src/ehdg_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-17 02:36:08.000000 ehdg_tools-4.2.1/src/ehdg_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 04:37:30.838505 ehdg_tools-4.2.2/
+-rw-rw-rw-   0        0        0    11558 2023-11-17 13:32:14.000000 ehdg_tools-4.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3001 2024-04-22 04:37:30.837508 ehdg_tools-4.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2436 2023-11-22 03:02:06.000000 ehdg_tools-4.2.2/README.md
+-rw-rw-rw-   0        0        0      699 2024-04-22 04:35:48.000000 ehdg_tools-4.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-22 04:37:30.838505 ehdg_tools-4.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-22 04:37:30.812773 ehdg_tools-4.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 04:37:30.822746 ehdg_tools-4.2.2/src/ehdg_tools/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_tools-4.2.2/src/ehdg_tools/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-11-21 22:16:22.000000 ehdg_tools-4.2.2/src/ehdg_tools/ehdg_buffers.py
+-rw-rw-rw-   0        0        0     6886 2024-04-22 04:34:47.000000 ehdg_tools-4.2.2/src/ehdg_tools/ehdg_functions.py
+-rw-rw-rw-   0        0        0     5831 2024-01-30 22:28:51.000000 ehdg_tools-4.2.2/src/ehdg_tools/ehdg_okn_checker.py
+-rw-rw-rw-   0        0        0   117333 2024-04-17 02:32:38.000000 ehdg_tools-4.2.2/src/ehdg_tools/ehdg_plotter.py
+-rw-rw-rw-   0        0        0    13490 2023-11-29 22:43:57.000000 ehdg_tools-4.2.2/src/ehdg_tools/ehdg_updater.py
+drwxrwxrwx   0        0        0        0 2024-04-22 04:37:30.836510 ehdg_tools-4.2.2/src/ehdg_tools.egg-info/
+-rw-rw-rw-   0        0        0     3001 2024-04-22 04:37:30.000000 ehdg_tools-4.2.2/src/ehdg_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-04-22 04:37:30.000000 ehdg_tools-4.2.2/src/ehdg_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 04:37:30.000000 ehdg_tools-4.2.2/src/ehdg_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-22 04:37:30.000000 ehdg_tools-4.2.2/src/ehdg_tools.egg-info/top_level.txt
```

### Comparing `ehdg_tools-4.2.1/LICENSE` & `ehdg_tools-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.1/PKG-INFO` & `ehdg_tools-4.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_tools
-Version: 4.2.1
+Version: 4.2.2
 Summary: Python library useful tools for ABI Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/ehdg_tools
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/ehdg_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_tools-4.2.1/README.md` & `ehdg_tools-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.1/pyproject.toml` & `ehdg_tools-4.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ehdg_tools"
-version = "4.2.1"
+version = "4.2.2"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python library useful tools for ABI Eye Health Diagnostic Group"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ehdg_tools-4.2.1/src/ehdg_tools/ehdg_buffers.py` & `ehdg_tools-4.2.2/src/ehdg_tools/ehdg_buffers.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.1/src/ehdg_tools/ehdg_okn_checker.py` & `ehdg_tools-4.2.2/src/ehdg_tools/ehdg_okn_checker.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.1/src/ehdg_tools/ehdg_plotter.py` & `ehdg_tools-4.2.2/src/ehdg_tools/ehdg_plotter.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.1/src/ehdg_tools/ehdg_updater.py` & `ehdg_tools-4.2.2/src/ehdg_tools/ehdg_updater.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.1/src/ehdg_tools.egg-info/PKG-INFO` & `ehdg_tools-4.2.2/src/ehdg_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_tools
-Version: 4.2.1
+Version: 4.2.2
 Summary: Python library useful tools for ABI Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/ehdg_tools
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/ehdg_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

