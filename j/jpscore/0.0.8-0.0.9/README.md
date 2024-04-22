# Comparing `tmp/jpscore-0.0.8.tar.gz` & `tmp/jpscore-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jpscore-0.0.8.tar", last modified: Mon Oct 17 23:56:33 2022, max compression
+gzip compressed data, was "jpscore-0.0.9.tar", last modified: Mon Apr 22 08:30:32 2024, max compression
```

## Comparing `jpscore-0.0.8.tar` & `jpscore-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-10-17 23:56:33.119073 jpscore-0.0.8/
--rw-r--r--   0 yt        (1000) yt        (1000)     2191 2022-10-17 23:56:33.119073 jpscore-0.0.8/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1635 2022-10-17 23:37:04.000000 jpscore-0.0.8/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2022-10-17 23:56:33.119073 jpscore-0.0.8/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      973 2022-10-17 23:55:13.000000 jpscore-0.0.8/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-10-17 23:56:33.099848 jpscore-0.0.8/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-10-17 23:56:33.119073 jpscore-0.0.8/src/jpscore.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     2191 2022-10-17 23:56:33.000000 jpscore-0.0.8/src/jpscore.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      221 2022-10-17 23:56:33.000000 jpscore-0.0.8/src/jpscore.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2022-10-17 23:56:33.000000 jpscore-0.0.8/src/jpscore.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       42 2022-10-17 23:56:33.000000 jpscore-0.0.8/src/jpscore.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        8 2022-10-17 23:56:33.000000 jpscore-0.0.8/src/jpscore.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1870 2022-10-17 23:54:12.000000 jpscore-0.0.8/src/jpscore.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:30:32.019396 jpscore-0.0.9/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2691 2024-04-22 08:30:32.019396 jpscore-0.0.9/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2133 2024-04-22 08:29:02.000000 jpscore-0.0.9/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 08:30:32.019396 jpscore-0.0.9/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      975 2024-04-22 08:30:02.000000 jpscore-0.0.9/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:30:32.019396 jpscore-0.0.9/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:30:32.019396 jpscore-0.0.9/src/jpscore.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2691 2024-04-22 08:30:31.000000 jpscore-0.0.9/src/jpscore.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      211 2024-04-22 08:30:31.000000 jpscore-0.0.9/src/jpscore.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 08:30:31.000000 jpscore-0.0.9/src/jpscore.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       42 2024-04-22 08:30:31.000000 jpscore-0.0.9/src/jpscore.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        8 2024-04-22 08:30:31.000000 jpscore-0.0.9/src/jpscore.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1870 2022-10-17 23:54:12.000000 jpscore-0.0.9/src/jpscore.py
```

### Comparing `jpscore-0.0.8/PKG-INFO` & `jpscore-0.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,17 @@
-Metadata-Version: 2.1
-Name: jpscore
-Version: 0.0.8
-Summary: A package for scoring prefecture COVID-19 policies in Japan
-Home-page: https://github.com/ytakefuji/covid_score_japan
-Author: yoshiyasu takefuji
-Author-email: takefuji@keio.jp
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/covid_score_japan
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# Scoring covid-19 policies by prefecture in Japan
+# Scoring covid-19 policies by prefecture in Japan 
 [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/2570c898-d60b-41ec-bd42-25d0a0629ba9/tree)
 
 DOI: https://doi.org/10.24433/CO.2522268.v1
 
-This is under review.
+Y. Takefuji, "The Best and Sustainable COVID-19 Policy in the World," in IEEE Transactions on Computational Social Systems, doi: 10.1109/TCSS.2022.3227926.
+
+Takefuji, Y. Policy analysis and data mining tools for controlling COVID-19 policies. Netw Model Anal Health Inform Bioinforma 12, 4 (2023). https://doi.org/10.1007/s13721-022-00400-3
 
-# dataset of NHK is not updated so that the following dataset will be used.
+# Since the NHK dataset is not updated, the following dataset will be used.
 
 https://covid19.mhlw.go.jp/public/opendata/deaths_cumulative_daily.csv
 
 or
 
 https://covid19.mhlw.go.jp/public/opendata/number_of_deaths_daily.csv
 
@@ -51,15 +37,21 @@
 
 # How to run jpscore
 The result.csv will be generated by the following command:
 as of march 19, 2022
 
 $ jpscore
 
-<img src='https://github.com/ytakefuji/covid_score_japan/raw/main/result.png' width=397 height=1393>
+This is with after version 0.7 or 0.8.
+
+<img src='https://github.com/y-takefuji/covid_score_japan/raw/main/jpscoreEN.jpg' width=397 height=1393>
+
+This is with version 0.1~0.6.
+
+<img src='https://github.com/y-takefuji/covid_score_japan/raw/main/result.png' width=397 height=1393>
 
 # Exercises
 <pre>
 1. Make a csv file of the total deaths by prefecture using the latest data.
 Hints:
 Use pandas DataFrame.
 Prefecture deaths population score
@@ -68,9 +60,7 @@
 Find the latest date on the total deaths by prefecture in the csv file.
 Make a list of prefectures.
 Make the total deaths data by prefecture.
 Find the latest population csv.
 Make the latest population by prefecture.
 Calculate a score by prefecture.
 
-
-
```

### Comparing `jpscore-0.0.8/setup.py` & `jpscore-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jpscore",
-    version="0.0.8",
+    version="0.0.9",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for scoring prefecture COVID-19 policies in Japan",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/covid_score_japan",
+    url="https://github.com/y-takefuji/covid_score_japan",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/covid_score_japan",
+        "Bug Tracker": "https://github.com/y-takefuji/covid_score_japan",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['jpscore'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'jpscore = jpscore:main'
         ]
     },
 )
```

### Comparing `jpscore-0.0.8/src/jpscore.egg-info/PKG-INFO` & `jpscore-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: jpscore
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for scoring prefecture COVID-19 policies in Japan
-Home-page: https://github.com/ytakefuji/covid_score_japan
+Home-page: https://github.com/y-takefuji/covid_score_japan
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/covid_score_japan
+Project-URL: Bug Tracker, https://github.com/y-takefuji/covid_score_japan
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# Scoring covid-19 policies by prefecture in Japan
+# Scoring covid-19 policies by prefecture in Japan 
 [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/2570c898-d60b-41ec-bd42-25d0a0629ba9/tree)
 
 DOI: https://doi.org/10.24433/CO.2522268.v1
 
-This is under review.
+Y. Takefuji, "The Best and Sustainable COVID-19 Policy in the World," in IEEE Transactions on Computational Social Systems, doi: 10.1109/TCSS.2022.3227926.
 
-# dataset of NHK is not updated so that the following dataset will be used.
+Takefuji, Y. Policy analysis and data mining tools for controlling COVID-19 policies. Netw Model Anal Health Inform Bioinforma 12, 4 (2023). https://doi.org/10.1007/s13721-022-00400-3
+
+# Since the NHK dataset is not updated, the following dataset will be used.
 
 https://covid19.mhlw.go.jp/public/opendata/deaths_cumulative_daily.csv
 
 or
 
 https://covid19.mhlw.go.jp/public/opendata/number_of_deaths_daily.csv
 
@@ -51,15 +53,21 @@
 
 # How to run jpscore
 The result.csv will be generated by the following command:
 as of march 19, 2022
 
 $ jpscore
 
-<img src='https://github.com/ytakefuji/covid_score_japan/raw/main/result.png' width=397 height=1393>
+This is with after version 0.7 or 0.8.
+
+<img src='https://github.com/y-takefuji/covid_score_japan/raw/main/jpscoreEN.jpg' width=397 height=1393>
+
+This is with version 0.1~0.6.
+
+<img src='https://github.com/y-takefuji/covid_score_japan/raw/main/result.png' width=397 height=1393>
 
 # Exercises
 <pre>
 1. Make a csv file of the total deaths by prefecture using the latest data.
 Hints:
 Use pandas DataFrame.
 Prefecture deaths population score
```

### Comparing `jpscore-0.0.8/src/jpscore.py` & `jpscore-0.0.9/src/jpscore.py`

 * *Files identical despite different names*

