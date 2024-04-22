# Comparing `tmp/tsico2-0.0.3.tar.gz` & `tmp/tsico2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsico2-0.0.3.tar", last modified: Sun Aug 20 07:55:45 2023, max compression
+gzip compressed data, was "tsico2-0.0.4.tar", last modified: Mon Apr 22 07:44:47 2024, max compression
```

## Comparing `tsico2-0.0.3.tar` & `tsico2-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-20 07:55:45.564942 tsico2-0.0.3/
--rw-r--r--   0 yt        (1000) yt        (1000)     1688 2023-08-20 07:55:45.563942 tsico2-0.0.3/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1157 2023-08-20 07:36:34.000000 tsico2-0.0.3/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-08-20 07:55:45.564942 tsico2-0.0.3/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      945 2023-08-20 07:55:07.000000 tsico2-0.0.3/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-20 07:55:45.548373 tsico2-0.0.3/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-20 07:55:45.562931 tsico2-0.0.3/src/tsico2.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1688 2023-08-20 07:55:45.000000 tsico2-0.0.3/src/tsico2.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      205 2023-08-20 07:55:45.000000 tsico2-0.0.3/src/tsico2.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-08-20 07:55:45.000000 tsico2-0.0.3/src/tsico2.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       40 2023-08-20 07:55:45.000000 tsico2-0.0.3/src/tsico2.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        7 2023-08-20 07:55:45.000000 tsico2-0.0.3/src/tsico2.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     6598 2023-08-20 07:54:46.000000 tsico2-0.0.3/src/tsico2.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:44:47.849372 tsico2-0.0.4/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1690 2024-04-22 07:44:47.849372 tsico2-0.0.4/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1157 2024-04-22 07:43:52.000000 tsico2-0.0.4/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 07:44:47.849372 tsico2-0.0.4/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      947 2024-04-22 07:44:20.000000 tsico2-0.0.4/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:44:47.849372 tsico2-0.0.4/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:44:47.849372 tsico2-0.0.4/src/tsico2.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1690 2024-04-22 07:44:47.000000 tsico2-0.0.4/src/tsico2.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      205 2024-04-22 07:44:47.000000 tsico2-0.0.4/src/tsico2.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 07:44:47.000000 tsico2-0.0.4/src/tsico2.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       40 2024-04-22 07:44:47.000000 tsico2-0.0.4/src/tsico2.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        7 2024-04-22 07:44:47.000000 tsico2-0.0.4/src/tsico2.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     6598 2023-08-20 07:54:46.000000 tsico2-0.0.4/src/tsico2.py
```

### Comparing `tsico2-0.0.3/PKG-INFO` & `tsico2-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tsico2
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for visualizing TSI and CO2 with r2 and p-value
-Home-page: https://github.com/ytakefuji/tsico2
+Home-page: https://github.com/y-takefuji/tsico2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/tsico2
+Project-URL: Bug Tracker, https://github.com/y-takefuji/tsico2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -36,11 +36,11 @@
 Enter end-date for March 2014
 
 Enter the end year-month (e.g. 2023-3): 2014-3
 
 The result will be popped on the screen. 
 The solid lines are the original and regression lines for CO2 and the dotted lines are the original and regression lines for TSI.
 
-<img src="https://github.com/ytakefuji/tsico2/blob/main/2007-3-2014-3.png" width=640 height=480>
+<img src="https://github.com/y-takefuji/tsico2/raw/main/2007-3-2014-3.png" width=640 height=480>
```

### Comparing `tsico2-0.0.3/README.md` & `tsico2-0.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 Enter end-date for March 2014
 
 Enter the end year-month (e.g. 2023-3): 2014-3
 
 The result will be popped on the screen. 
 The solid lines are the original and regression lines for CO2 and the dotted lines are the original and regression lines for TSI.
 
-<img src="https://github.com/ytakefuji/tsico2/blob/main/2007-3-2014-3.png" width=640 height=480>
+<img src="https://github.com/y-takefuji/tsico2/raw/main/2007-3-2014-3.png" width=640 height=480>
```

### Comparing `tsico2-0.0.3/setup.py` & `tsico2-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tsico2",
-    version="0.0.3",
+    version="0.0.4",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for visualizing TSI and CO2 with r2 and p-value",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/tsico2",
+    url="https://github.com/y-takefuji/tsico2",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/tsico2",
+        "Bug Tracker": "https://github.com/y-takefuji/tsico2",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
```

### Comparing `tsico2-0.0.3/src/tsico2.egg-info/PKG-INFO` & `tsico2-0.0.4/src/tsico2.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tsico2
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for visualizing TSI and CO2 with r2 and p-value
-Home-page: https://github.com/ytakefuji/tsico2
+Home-page: https://github.com/y-takefuji/tsico2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/tsico2
+Project-URL: Bug Tracker, https://github.com/y-takefuji/tsico2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -36,11 +36,11 @@
 Enter end-date for March 2014
 
 Enter the end year-month (e.g. 2023-3): 2014-3
 
 The result will be popped on the screen. 
 The solid lines are the original and regression lines for CO2 and the dotted lines are the original and regression lines for TSI.
 
-<img src="https://github.com/ytakefuji/tsico2/blob/main/2007-3-2014-3.png" width=640 height=480>
+<img src="https://github.com/y-takefuji/tsico2/raw/main/2007-3-2014-3.png" width=640 height=480>
```

### Comparing `tsico2-0.0.3/src/tsico2.py` & `tsico2-0.0.4/src/tsico2.py`

 * *Files identical despite different names*

