# Comparing `tmp/deathdaily-0.1.5.tar.gz` & `tmp/deathdaily-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deathdaily-0.1.5.tar", last modified: Tue Jun 27 06:30:23 2023, max compression
+gzip compressed data, was "deathdaily-0.1.6.tar", last modified: Mon Apr 22 07:15:31 2024, max compression
```

## Comparing `deathdaily-0.1.5.tar` & `deathdaily-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-27 06:30:23.833418 deathdaily-0.1.5/
--rw-r--r--   0 yt        (1000) yt        (1000)     2377 2023-06-27 06:30:23.832538 deathdaily-0.1.5/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1835 2021-10-15 03:28:03.000000 deathdaily-0.1.5/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-06-27 06:30:23.834421 deathdaily-0.1.5/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)     1005 2023-06-27 06:08:01.000000 deathdaily-0.1.5/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-27 06:30:23.819556 deathdaily-0.1.5/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-27 06:30:23.831436 deathdaily-0.1.5/src/deathdaily.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     2377 2023-06-27 06:30:23.000000 deathdaily-0.1.5/src/deathdaily.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      229 2023-06-27 06:30:23.000000 deathdaily-0.1.5/src/deathdaily.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-06-27 06:30:23.000000 deathdaily-0.1.5/src/deathdaily.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       47 2023-06-27 06:30:23.000000 deathdaily-0.1.5/src/deathdaily.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       11 2023-06-27 06:30:23.000000 deathdaily-0.1.5/src/deathdaily.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     2220 2023-06-27 06:19:00.000000 deathdaily-0.1.5/src/deathdaily.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:15:31.499356 deathdaily-0.1.6/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2416 2024-04-22 07:15:31.499356 deathdaily-0.1.6/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1835 2021-10-15 03:28:03.000000 deathdaily-0.1.6/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 07:15:31.499356 deathdaily-0.1.6/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1007 2024-04-22 07:11:16.000000 deathdaily-0.1.6/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:15:31.499356 deathdaily-0.1.6/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:15:31.499356 deathdaily-0.1.6/src/deathdaily.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2416 2024-04-22 07:15:31.000000 deathdaily-0.1.6/src/deathdaily.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      229 2024-04-22 07:15:31.000000 deathdaily-0.1.6/src/deathdaily.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 07:15:31.000000 deathdaily-0.1.6/src/deathdaily.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       48 2024-04-22 07:15:31.000000 deathdaily-0.1.6/src/deathdaily.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       11 2024-04-22 07:15:31.000000 deathdaily-0.1.6/src/deathdaily.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2220 2023-06-27 06:19:00.000000 deathdaily-0.1.6/src/deathdaily.py
```

### Comparing `deathdaily-0.1.5/PKG-INFO` & `deathdaily-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: deathdaily
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for predicting the number of daily deaths
-Home-page: https://github.com/ytakefuji/covid-19_daily_death_prediction
+Home-page: https://github.com/y-takefuji/covid-19_daily_death_prediction
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
-Project-URL: Bug Tracker, https://github.com/ytakefuji/covid-19_daily_death_prediction
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/y-takefuji/covid-19_daily_death_prediction
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # COVID-19 daily death prediction
@@ -57,7 +59,9 @@
 $ deathdaily Israel 200 9
 
 <img src="https://github.com/ytakefuji/covid-19_daily_death_prediction/raw/main/Israel.png" width=320 height=240 >
 
 $ deathdaily 'United Kingdom' 100 11
 
 <img src="https://github.com/ytakefuji/covid-19_daily_death_prediction/raw/main/United Kingdom.png" width=320 height=240 >
+
+
```

### Comparing `deathdaily-0.1.5/README.md` & `deathdaily-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `deathdaily-0.1.5/setup.py` & `deathdaily-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="deathdaily",
-    version="0.1.5",
+    version="0.1.6",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for predicting the number of daily deaths",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/covid-19_daily_death_prediction",
+    url="https://github.com/y-takefuji/covid-19_daily_death_prediction",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/covid-19_daily_death_prediction",
+        "Bug Tracker": "https://github.com/y-takefuji/covid-19_daily_death_prediction",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
```

### Comparing `deathdaily-0.1.5/src/deathdaily.egg-info/PKG-INFO` & `deathdaily-0.1.6/src/deathdaily.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: deathdaily
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for predicting the number of daily deaths
-Home-page: https://github.com/ytakefuji/covid-19_daily_death_prediction
+Home-page: https://github.com/y-takefuji/covid-19_daily_death_prediction
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
-Project-URL: Bug Tracker, https://github.com/ytakefuji/covid-19_daily_death_prediction
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/y-takefuji/covid-19_daily_death_prediction
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # COVID-19 daily death prediction
@@ -57,7 +59,9 @@
 $ deathdaily Israel 200 9
 
 <img src="https://github.com/ytakefuji/covid-19_daily_death_prediction/raw/main/Israel.png" width=320 height=240 >
 
 $ deathdaily 'United Kingdom' 100 11
 
 <img src="https://github.com/ytakefuji/covid-19_daily_death_prediction/raw/main/United Kingdom.png" width=320 height=240 >
+
+
```

### Comparing `deathdaily-0.1.5/src/deathdaily.py` & `deathdaily-0.1.6/src/deathdaily.py`

 * *Files identical despite different names*

