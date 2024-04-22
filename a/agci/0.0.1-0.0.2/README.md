# Comparing `tmp/agci-0.0.1.tar.gz` & `tmp/agci-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agci-0.0.1.tar", last modified: Mon Apr 11 03:59:34 2022, max compression
+gzip compressed data, was "agci-0.0.2.tar", last modified: Mon Apr 22 08:26:21 2024, max compression
```

## Comparing `agci-0.0.1.tar` & `agci-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-11 03:59:34.401072 agci-0.0.1/
--rw-r--r--   0 yt        (1000) yt        (1000)     1192 2022-04-11 03:59:34.401072 agci-0.0.1/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      691 2022-04-11 03:24:33.000000 agci-0.0.1/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2022-04-11 03:59:34.401072 agci-0.0.1/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      909 2022-04-11 03:08:27.000000 agci-0.0.1/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-11 03:59:34.393783 agci-0.0.1/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-11 03:59:34.401072 agci-0.0.1/src/agci.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1192 2022-04-11 03:59:33.000000 agci-0.0.1/src/agci.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      193 2022-04-11 03:59:33.000000 agci-0.0.1/src/agci.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2022-04-11 03:59:33.000000 agci-0.0.1/src/agci.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       36 2022-04-11 03:59:33.000000 agci-0.0.1/src/agci.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        5 2022-04-11 03:59:33.000000 agci-0.0.1/src/agci.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     2812 2022-04-11 03:19:21.000000 agci-0.0.1/src/agci.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:26:21.069394 agci-0.0.2/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1629 2024-04-22 08:26:21.069394 agci-0.0.2/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1126 2024-04-22 08:25:08.000000 agci-0.0.2/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 08:26:21.069394 agci-0.0.2/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      911 2024-04-22 08:25:44.000000 agci-0.0.2/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:26:21.059394 agci-0.0.2/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:26:21.059394 agci-0.0.2/src/agci.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1629 2024-04-22 08:26:21.000000 agci-0.0.2/src/agci.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      193 2024-04-22 08:26:21.000000 agci-0.0.2/src/agci.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 08:26:21.000000 agci-0.0.2/src/agci.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       36 2024-04-22 08:26:21.000000 agci-0.0.2/src/agci.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        5 2024-04-22 08:26:21.000000 agci-0.0.2/src/agci.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2812 2022-04-11 03:19:21.000000 agci-0.0.2/src/agci.py
```

### Comparing `agci-0.0.1/PKG-INFO` & `agci-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: agci
-Version: 0.0.1
+Version: 0.0.2
 Summary: how to debut a PyPI for chemistry
-Home-page: https://github.com/ytakefuji/agci
+Home-page: https://github.com/y-takefuji/agci
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/agci
+Project-URL: Bug Tracker, https://github.com/y-takefuji/agci
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # agci
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/9562303/tree)
+
+takefuji (2022) agci for a reproducible PyPI application [Source Code]. https://doi.org/10.24433/CO.8712645.v1
+
+Takefuji, Y. An Updated Tutorial on Reproducible PyPI Applications for Advancing Chemometrics and Boosting Learner Motivation. Chemometrics and Intelligent Laboratory Systems (2023).
+
 This is a tutorial on how to debut a PyPI application and how to validate software reproducibility.
 This agci is renamed and modified from "Symmetric GC integration.py" at https://github.com/1mikegrn/pyGC/blob/master/JCE-supplemental/Asymmetric%20GC%20integration.py
 The modification is used to show how to debut a PyPI application and how to validate software reproducibility 
 via Code Ocean.
 
 # how to install agci
 
@@ -27,10 +33,10 @@
 # how to run agci
 The result picture will be saved in result.png.
 
 $ agci "csv data filename"
 
 $ agci Sample\ GC\ data\ 1\ pt\ acetone\ 1\ pt\ cyclohexane.csv
 
-<img src='https://github.com/ytakefuji/agci/raw/main/result.png' width=640 hight=480>
+<img src='https://github.com/y-takefuji/agci/raw/main/result.png' width=640 hight=480>
```

### Comparing `agci-0.0.1/src/agci.egg-info/PKG-INFO` & `agci-0.0.2/src/agci.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: agci
-Version: 0.0.1
+Version: 0.0.2
 Summary: how to debut a PyPI for chemistry
-Home-page: https://github.com/ytakefuji/agci
+Home-page: https://github.com/y-takefuji/agci
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/agci
+Project-URL: Bug Tracker, https://github.com/y-takefuji/agci
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # agci
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/9562303/tree)
+
+takefuji (2022) agci for a reproducible PyPI application [Source Code]. https://doi.org/10.24433/CO.8712645.v1
+
+Takefuji, Y. An Updated Tutorial on Reproducible PyPI Applications for Advancing Chemometrics and Boosting Learner Motivation. Chemometrics and Intelligent Laboratory Systems (2023).
+
 This is a tutorial on how to debut a PyPI application and how to validate software reproducibility.
 This agci is renamed and modified from "Symmetric GC integration.py" at https://github.com/1mikegrn/pyGC/blob/master/JCE-supplemental/Asymmetric%20GC%20integration.py
 The modification is used to show how to debut a PyPI application and how to validate software reproducibility 
 via Code Ocean.
 
 # how to install agci
 
@@ -27,10 +33,10 @@
 # how to run agci
 The result picture will be saved in result.png.
 
 $ agci "csv data filename"
 
 $ agci Sample\ GC\ data\ 1\ pt\ acetone\ 1\ pt\ cyclohexane.csv
 
-<img src='https://github.com/ytakefuji/agci/raw/main/result.png' width=640 hight=480>
+<img src='https://github.com/y-takefuji/agci/raw/main/result.png' width=640 hight=480>
```

### Comparing `agci-0.0.1/src/agci.py` & `agci-0.0.2/src/agci.py`

 * *Files identical despite different names*

