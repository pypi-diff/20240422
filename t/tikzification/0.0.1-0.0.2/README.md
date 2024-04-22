# Comparing `tmp/tikzification-0.0.1.tar.gz` & `tmp/tikzification-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikzification-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tikzification-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tikzification-0.0.1.tar` & `tikzification-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1157 2024-04-12 16:38:08.017919 tikzification-0.0.1/LICENSE
--rw-r--r--   0        0        0       66 2024-04-12 16:42:27.579918 tikzification-0.0.1/README.md
--rw-r--r--   0        0        0     1012 2024-04-14 16:07:31.666902 tikzification-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-12 16:23:51.719375 tikzification-0.0.1/src/tikzification/__about__.py
--rw-r--r--   0        0        0      312 2024-04-12 19:37:30.338530 tikzification-0.0.1/src/tikzification/__init__.py
--rw-r--r--   0        0        0    33784 2024-04-12 17:10:06.412977 tikzification-0.0.1/src/tikzification/_axes.py
--rw-r--r--   0        0        0    43178 2024-04-12 16:50:10.823491 tikzification-0.0.1/src/tikzification/_cleanfigure.py
--rw-r--r--   0        0        0     2602 2024-04-12 16:23:51.719375 tikzification-0.0.1/src/tikzification/_color.py
--rw-r--r--   0        0        0     1115 2024-04-13 21:15:59.747505 tikzification-0.0.1/src/tikzification/_config.py
--rw-r--r--   0        0        0     1193 2024-04-12 19:39:39.191537 tikzification-0.0.1/src/tikzification/_files.py
--rw-r--r--   0        0        0     4308 2024-04-12 16:45:00.993101 tikzification-0.0.1/src/tikzification/_hatches.py
--rw-r--r--   0        0        0     2029 2024-04-12 16:45:00.993101 tikzification-0.0.1/src/tikzification/_image.py
--rw-r--r--   0        0        0     6612 2024-04-12 17:19:02.989173 tikzification-0.0.1/src/tikzification/_legend.py
--rw-r--r--   0        0        0    10257 2024-04-12 17:18:24.064869 tikzification-0.0.1/src/tikzification/_line2d.py
--rw-r--r--   0        0        0     2203 2024-04-12 16:23:51.719375 tikzification-0.0.1/src/tikzification/_markers.py
--rw-r--r--   0        0        0     6712 2024-04-12 17:17:35.312488 tikzification-0.0.1/src/tikzification/_patch.py
--rw-r--r--   0        0        0    18683 2024-04-12 17:16:59.664210 tikzification-0.0.1/src/tikzification/_path.py
--rw-r--r--   0        0        0     2060 2024-04-12 16:23:51.719375 tikzification-0.0.1/src/tikzification/_quadmesh.py
--rw-r--r--   0        0        0    20084 2024-04-14 15:43:18.642846 tikzification-0.0.1/src/tikzification/_save.py
--rw-r--r--   0        0        0    10411 2024-04-12 16:23:51.723374 tikzification-0.0.1/src/tikzification/_text.py
--rw-r--r--   0        0        0     2662 2024-04-12 17:27:17.433027 tikzification-0.0.1/src/tikzification/_util.py
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 tikzification-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1157 2024-04-12 16:38:08.017919 tikzification-0.0.2/LICENSE
+-rw-r--r--   0        0        0       66 2024-04-12 16:42:27.579918 tikzification-0.0.2/README.md
+-rw-r--r--   0        0        0     1012 2024-04-22 07:56:20.845338 tikzification-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-12 16:23:51.719375 tikzification-0.0.2/src/tikzification/__about__.py
+-rw-r--r--   0        0        0      312 2024-04-12 19:37:30.338530 tikzification-0.0.2/src/tikzification/__init__.py
+-rw-r--r--   0        0        0    33784 2024-04-12 17:10:06.412977 tikzification-0.0.2/src/tikzification/_axes.py
+-rw-r--r--   0        0        0    43178 2024-04-12 16:50:10.823491 tikzification-0.0.2/src/tikzification/_cleanfigure.py
+-rw-r--r--   0        0        0     2602 2024-04-12 16:23:51.719375 tikzification-0.0.2/src/tikzification/_color.py
+-rw-r--r--   0        0        0     1305 2024-04-22 07:46:41.448314 tikzification-0.0.2/src/tikzification/_config.py
+-rw-r--r--   0        0        0     1193 2024-04-12 19:39:39.191537 tikzification-0.0.2/src/tikzification/_files.py
+-rw-r--r--   0        0        0     4308 2024-04-12 16:45:00.993101 tikzification-0.0.2/src/tikzification/_hatches.py
+-rw-r--r--   0        0        0     2029 2024-04-12 16:45:00.993101 tikzification-0.0.2/src/tikzification/_image.py
+-rw-r--r--   0        0        0     6612 2024-04-12 17:19:02.989173 tikzification-0.0.2/src/tikzification/_legend.py
+-rw-r--r--   0        0        0    10257 2024-04-12 17:18:24.064869 tikzification-0.0.2/src/tikzification/_line2d.py
+-rw-r--r--   0        0        0     2203 2024-04-12 16:23:51.719375 tikzification-0.0.2/src/tikzification/_markers.py
+-rw-r--r--   0        0        0     6712 2024-04-12 17:17:35.312488 tikzification-0.0.2/src/tikzification/_patch.py
+-rw-r--r--   0        0        0    18683 2024-04-12 17:16:59.664210 tikzification-0.0.2/src/tikzification/_path.py
+-rw-r--r--   0        0        0     2060 2024-04-12 16:23:51.719375 tikzification-0.0.2/src/tikzification/_quadmesh.py
+-rw-r--r--   0        0        0    20084 2024-04-14 15:43:18.642846 tikzification-0.0.2/src/tikzification/_save.py
+-rw-r--r--   0        0        0    10411 2024-04-12 16:23:51.723374 tikzification-0.0.2/src/tikzification/_text.py
+-rw-r--r--   0        0        0     2662 2024-04-12 17:27:17.433027 tikzification-0.0.2/src/tikzification/_util.py
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 tikzification-0.0.2/PKG-INFO
```

### Comparing `tikzification-0.0.1/LICENSE` & `tikzification-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/pyproject.toml` & `tikzification-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [tool.isort]
 profile = "black"
 
 [project]
 name = "tikzification"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{name = "Leander Kurscheidt", email = "Leander.Kurscheidt@gmx.de"}]
 description = "Convert matplotlib figures into TikZ/PGFPlots. Based on tikzplotlib"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Framework :: Matplotlib",
```

### Comparing `tikzification-0.0.1/src/tikzification/_axes.py` & `tikzification-0.0.2/src/tikzification/_axes.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_cleanfigure.py` & `tikzification-0.0.2/src/tikzification/_cleanfigure.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_color.py` & `tikzification-0.0.2/src/tikzification/_color.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_files.py` & `tikzification-0.0.2/src/tikzification/_files.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_hatches.py` & `tikzification-0.0.2/src/tikzification/_hatches.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_image.py` & `tikzification-0.0.2/src/tikzification/_image.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_legend.py` & `tikzification-0.0.2/src/tikzification/_legend.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_line2d.py` & `tikzification-0.0.2/src/tikzification/_line2d.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_markers.py` & `tikzification-0.0.2/src/tikzification/_markers.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_patch.py` & `tikzification-0.0.2/src/tikzification/_patch.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_path.py` & `tikzification-0.0.2/src/tikzification/_path.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_quadmesh.py` & `tikzification-0.0.2/src/tikzification/_quadmesh.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_save.py` & `tikzification-0.0.2/src/tikzification/_save.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_text.py` & `tikzification-0.0.2/src/tikzification/_text.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/src/tikzification/_util.py` & `tikzification-0.0.2/src/tikzification/_util.py`

 * *Files identical despite different names*

### Comparing `tikzification-0.0.1/PKG-INFO` & `tikzification-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikzification
-Version: 0.0.1
+Version: 0.0.2
 Summary: Convert matplotlib figures into TikZ/PGFPlots. Based on tikzplotlib
 Keywords: latex,tikz,matplotlib,graphics
 Author-email: Leander Kurscheidt <Leander.Kurscheidt@gmx.de>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Matplotlib
```

