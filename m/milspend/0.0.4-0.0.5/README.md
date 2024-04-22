# Comparing `tmp/milspend-0.0.4.tar.gz` & `tmp/milspend-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milspend-0.0.4.tar", last modified: Mon Jun 26 11:47:29 2023, max compression
+gzip compressed data, was "milspend-0.0.5.tar", last modified: Mon Apr 22 08:06:47 2024, max compression
```

## Comparing `milspend-0.0.4.tar` & `milspend-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-26 11:47:29.468096 milspend-0.0.4/
--rw-r--r--   0 yt        (1000) yt        (1000)     1689 2023-06-26 11:47:29.468096 milspend-0.0.4/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1147 2022-02-27 14:19:58.000000 milspend-0.0.4/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-06-26 11:47:29.468096 milspend-0.0.4/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      962 2023-06-26 11:45:39.000000 milspend-0.0.4/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-26 11:47:29.462125 milspend-0.0.4/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-26 11:47:29.468096 milspend-0.0.4/src/milspend.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1689 2023-06-26 11:47:28.000000 milspend-0.0.4/src/milspend.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      227 2023-06-26 11:47:28.000000 milspend-0.0.4/src/milspend.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-06-26 11:47:28.000000 milspend-0.0.4/src/milspend.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-06-26 11:47:28.000000 milspend-0.0.4/src/milspend.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-06-26 11:47:28.000000 milspend-0.0.4/src/milspend.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1579 2023-06-26 11:43:09.000000 milspend-0.0.4/src/milspend.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:06:47.389384 milspend-0.0.5/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2400 2024-04-22 08:06:47.389384 milspend-0.0.5/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1856 2024-04-22 08:05:50.000000 milspend-0.0.5/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 08:06:47.389384 milspend-0.0.5/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      964 2024-04-22 08:03:18.000000 milspend-0.0.5/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:06:47.389384 milspend-0.0.5/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:06:47.389384 milspend-0.0.5/src/milspend.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2400 2024-04-22 08:06:47.000000 milspend-0.0.5/src/milspend.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      217 2024-04-22 08:06:47.000000 milspend-0.0.5/src/milspend.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 08:06:47.000000 milspend-0.0.5/src/milspend.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       44 2024-04-22 08:06:47.000000 milspend-0.0.5/src/milspend.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        9 2024-04-22 08:06:47.000000 milspend-0.0.5/src/milspend.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1579 2023-06-26 11:43:09.000000 milspend-0.0.5/src/milspend.py
```

### Comparing `milspend-0.0.4/PKG-INFO` & `milspend-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-Metadata-Version: 2.1
-Name: milspend
-Version: 0.0.4
-Summary: A package for visualizing military spending of up to 4 countries
-Home-page: https://github.com/ytakefuji/defense
-Author: yoshiyasu takefuji
-Author-email: takefuji@keio.jp
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/defense
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # defense
+This is under review.
+
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/a01e51d9-0f62-40c5-bc9e-b4c8b16b421e/tree)
+
+DOI: https://doi.org/10.24433/CO.7896039.v1
+
+This is under review.
 
 The goal of this project is to visualize military spending of countries.
 
 Using a SIPRI dataset, milspend can visualize military spending of up to four countries.
 
 The SIPRI dataset is downloadable from:
 
 https://sipri.org/sites/default/files/SIPRI-Milex-data-1949-2020_0.xlsx
 
+or the latest dataset from:
+
+https://www.sipri.org/sites/default/files/SIPRI-Milex-data-1949-2022.xlsx
+
 The number of the vertical axis indicates the US dollars in millions.
 
-<img src='https://github.com/ytakefuji/defense/raw/main/result.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/defense/raw/main/result.png' width=640 height=480>
 
-# How to install milspend
+# How to install milspend on Linux, MacOS, or WSL on Windows
 You may need matplotlib library.
 
 $ pip install matplotlib
 
-$ pip install milspend
+$ pip install -U milspend
+
+
+# How to install milspend if you have a trouble.
+$ pip install milspend --force-reinstall --no-cache-dir --no-binary :all:
 
 # How to run milspend
 Milspend program allows user to specify up to four countries to plot military spending of the specified countries.
 For example, the following command can display military spending of the US, China, Russia and Japan in the graph.
 
+For 0.0.1 and 0.0.2 with 1949-2020 dataset: Seperate countries with spaces.
+
 $ milspend USA China Russia Japan
 
-<img src='https://github.com/ytakefuji/defense/raw/main/uscnrujp.png' height=480 width=640>
+<img src='https://github.com/y-takefuji/defense/raw/main/uscnrujp.png' height=480 width=640>
 The following command can display military spending of Japan and South Korea.
 
-$ milspend Japan 'Korea, South'
 
-<img src='https://github.com/ytakefuji/defense/raw/main/koreajapan.png' height=480 width=640>
+For 0.0.3 with with 1949-2022: Enclose up to four countries in single quotes and separate them with colons.
+
+$ milspend 'Japan:Korea, South'
 
+<img src='https://github.com/y-takefuji/defense/raw/main/jpkr.png' height=480 width=640>
```

### Comparing `milspend-0.0.4/setup.py` & `milspend-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="milspend",
-    version="0.0.4",
+    version="0.0.5",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for visualizing military spending of up to 4 countries",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/defense",
+    url="https://github.com/y-takefuji/defense",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/defense",
+        "Bug Tracker": "https://github.com/y-takefuji/defense",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
```

### Comparing `milspend-0.0.4/src/milspend.py` & `milspend-0.0.5/src/milspend.py`

 * *Files identical despite different names*

