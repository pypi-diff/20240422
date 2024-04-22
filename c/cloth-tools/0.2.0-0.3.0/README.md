# Comparing `tmp/cloth-tools-0.2.0.tar.gz` & `tmp/cloth_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloth-tools-0.2.0.tar", last modified: Fri Mar 29 16:17:36 2024, max compression
+gzip compressed data, was "cloth_tools-0.3.0.tar", last modified: Mon Apr 22 09:30:21 2024, max compression
```

## Comparing `cloth-tools-0.2.0.tar` & `cloth_tools-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:17:36.323678 cloth-tools-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-29 16:17:36.323678 cloth-tools-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:17:36.319678 cloth-tools-0.2.0/cloth_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-29 16:17:32.000000 cloth-tools-0.2.0/cloth_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-29 16:17:32.000000 cloth-tools-0.2.0/cloth_tools/bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-29 16:17:32.000000 cloth-tools-0.2.0/cloth_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-03-29 16:17:32.000000 cloth-tools-0.2.0/cloth_tools/motion_blur_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-03-29 16:17:32.000000 cloth-tools-0.2.0/cloth_tools/trajectory_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-29 16:17:32.000000 cloth-tools-0.2.0/cloth_tools/wrench_smoother.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:17:36.323678 cloth-tools-0.2.0/cloth_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-29 16:17:36.000000 cloth-tools-0.2.0/cloth_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-29 16:17:36.000000 cloth-tools-0.2.0/cloth_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:17:36.000000 cloth-tools-0.2.0/cloth_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 16:17:36.000000 cloth-tools-0.2.0/cloth_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 16:17:36.000000 cloth-tools-0.2.0/cloth_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-29 16:17:32.000000 cloth-tools-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 16:17:36.323678 cloth-tools-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-29 16:17:32.000000 cloth-tools-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:17:36.323678 cloth-tools-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-29 16:17:32.000000 cloth-tools-0.2.0/test/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:21.235496 cloth_tools-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-22 09:30:21.235496 cloth_tools-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:21.235496 cloth_tools-0.3.0/cloth_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-22 09:30:17.000000 cloth_tools-0.3.0/cloth_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-22 09:30:17.000000 cloth_tools-0.3.0/cloth_tools/bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-22 09:30:17.000000 cloth_tools-0.3.0/cloth_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-04-22 09:30:17.000000 cloth_tools-0.3.0/cloth_tools/motion_blur_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-22 09:30:17.000000 cloth_tools-0.3.0/cloth_tools/trajectory_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-22 09:30:17.000000 cloth_tools-0.3.0/cloth_tools/wrench_smoother.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:21.235496 cloth_tools-0.3.0/cloth_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-22 09:30:21.000000 cloth_tools-0.3.0/cloth_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-22 09:30:21.000000 cloth_tools-0.3.0/cloth_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:30:21.000000 cloth_tools-0.3.0/cloth_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 09:30:21.000000 cloth_tools-0.3.0/cloth_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 09:30:21.000000 cloth_tools-0.3.0/cloth_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-22 09:30:17.000000 cloth_tools-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:30:21.235496 cloth_tools-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-22 09:30:17.000000 cloth_tools-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:30:21.235496 cloth_tools-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-22 09:30:17.000000 cloth_tools-0.3.0/test/test_dummy.py
```

### Comparing `cloth-tools-0.2.0/PKG-INFO` & `cloth_tools-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloth-tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Official package for the ICRA 2024 Cloth Competition
 Author-email: Victor-Louis De Gusseme <victorlouisdg@gmail.com>
 Project-URL: Homepage, https://github.com/Victorlouisdg/cloth-competition
 Project-URL: Issues, https://github.com/Victorlouisdg/cloth-competition/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cloth-tools-0.2.0/cloth_tools/bounding_boxes.py` & `cloth_tools-0.3.0/cloth_tools/bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `cloth-tools-0.2.0/cloth_tools/config.py` & `cloth_tools-0.3.0/cloth_tools/config.py`

 * *Files identical despite different names*

### Comparing `cloth-tools-0.2.0/cloth_tools/motion_blur_detector.py` & `cloth_tools-0.3.0/cloth_tools/motion_blur_detector.py`

 * *Files identical despite different names*

### Comparing `cloth-tools-0.2.0/cloth_tools/trajectory_execution.py` & `cloth_tools-0.3.0/cloth_tools/trajectory_execution.py`

 * *Files identical despite different names*

### Comparing `cloth-tools-0.2.0/cloth_tools/wrench_smoother.py` & `cloth_tools-0.3.0/cloth_tools/wrench_smoother.py`

 * *Files identical despite different names*

### Comparing `cloth-tools-0.2.0/cloth_tools.egg-info/PKG-INFO` & `cloth_tools-0.3.0/cloth_tools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloth-tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Official package for the ICRA 2024 Cloth Competition
 Author-email: Victor-Louis De Gusseme <victorlouisdg@gmail.com>
 Project-URL: Homepage, https://github.com/Victorlouisdg/cloth-competition
 Project-URL: Issues, https://github.com/Victorlouisdg/cloth-competition/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cloth-tools-0.2.0/pyproject.toml` & `cloth_tools-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cloth-tools"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name = "Victor-Louis De Gusseme", email = "victorlouisdg@gmail.com" },
 ]
 description = "Official package for the ICRA 2024 Cloth Competition"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

