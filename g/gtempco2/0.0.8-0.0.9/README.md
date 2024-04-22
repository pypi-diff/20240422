# Comparing `tmp/gtempco2-0.0.8.tar.gz` & `tmp/gtempco2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtempco2-0.0.8.tar", last modified: Sun Jul 30 21:10:50 2023, max compression
+gzip compressed data, was "gtempco2-0.0.9.tar", last modified: Mon Apr 22 08:00:45 2024, max compression
```

## Comparing `gtempco2-0.0.8.tar` & `gtempco2-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-30 21:10:50.674186 gtempco2-0.0.8/
--rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-07-30 21:10:50.672271 gtempco2-0.0.8/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1249 2023-06-12 04:59:29.000000 gtempco2-0.0.8/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-07-30 21:10:50.674186 gtempco2-0.0.8/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      951 2023-07-30 21:09:37.000000 gtempco2-0.0.8/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-30 21:10:50.666629 gtempco2-0.0.8/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-30 21:10:50.671274 gtempco2-0.0.8/src/gtempco2.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-07-30 21:10:50.000000 gtempco2-0.0.8/src/gtempco2.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-07-30 21:10:50.000000 gtempco2-0.0.8/src/gtempco2.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-07-30 21:10:50.000000 gtempco2-0.0.8/src/gtempco2.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-07-30 21:10:50.000000 gtempco2-0.0.8/src/gtempco2.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-07-30 21:10:50.000000 gtempco2-0.0.8/src/gtempco2.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     3117 2023-07-30 21:08:29.000000 gtempco2-0.0.8/src/gtempco2.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:00:45.979381 gtempco2-0.0.9/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1792 2024-04-22 08:00:45.979381 gtempco2-0.0.9/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1259 2024-04-22 07:59:59.000000 gtempco2-0.0.9/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 08:00:45.979381 gtempco2-0.0.9/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      953 2024-04-22 08:00:26.000000 gtempco2-0.0.9/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:00:45.979381 gtempco2-0.0.9/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:00:45.979381 gtempco2-0.0.9/src/gtempco2.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1792 2024-04-22 08:00:45.000000 gtempco2-0.0.9/src/gtempco2.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      217 2024-04-22 08:00:45.000000 gtempco2-0.0.9/src/gtempco2.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 08:00:45.000000 gtempco2-0.0.9/src/gtempco2.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       44 2024-04-22 08:00:45.000000 gtempco2-0.0.9/src/gtempco2.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        9 2024-04-22 08:00:45.000000 gtempco2-0.0.9/src/gtempco2.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     3117 2023-07-30 21:08:29.000000 gtempco2-0.0.9/src/gtempco2.py
```

### Comparing `gtempco2-0.0.8/PKG-INFO` & `gtempco2-0.0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: gtempco2
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for displaying global temperature and co2
-Home-page: https://github.com/ytakefuji/gtempco2
+Home-page: https://github.com/y-takefuji/gtempco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/gtempco2
+Project-URL: Bug Tracker, https://github.com/y-takefuji/gtempco2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # gtempco2
 
 gtempco2 is a PyPI application to display global temperature and co2 of land and ocean with NOAA datasets.
 
 NOAA monthly datasets on the global temperature of land and ocean and the global co2 will be automatically downloaded. 
 
-gtempco2 is to plot a graph for a user-specified time period with two lines representing global temperature and global CO2 levels. The graph includes first-order regression lines with coefficients and R-squared values.
+gtempco2 is to plot a graph for a user-specified time period with two lines representing global temperature and global CO2 levels. The graph includes first-order regression lines with coefficients, p-value and R-squared values.
 
 To install gtempco2, use the following pip command.
 
 $ pip install gtempco2
 
 To run gtempco2, the user-specified time period such as start-date and end-date is needed to plot a graph of the global temperature and co2 from start-date to end-date. 
 
@@ -32,19 +32,19 @@
 
 For example, 1958-03 indicates March 1958 when NOAA started the measurement of the global co2.
 
 <pre>
 $ gtempco2
 enter start_date: e.g. 1960-04
 co2 measurement started from 1958-03
-yyyy-mo: 1960-06
+yyyy-mo: 1958-03
 enter end_date: e.g. 2023-04
-yyyy-mo: 1965-06
-start_date= 1960-06 end_date= 1965-06
+yyyy-mo: 1965-03
+start_date= 1958-03 end_date= 1965-03
 </pre>
 
 The system will ask the start-date and end-date. The result will be shown and saved in the directory as follows.
 
-<img src='https://github.com/ytakefuji/gtempco2/raw/main/1960-06_1965-06.png' height=450 width=600>
+<img src='https://github.com/y-takefuji/gtempco2/raw/main/1958-03_1965-03.png' height=450 width=600>
```

### Comparing `gtempco2-0.0.8/README.md` & `gtempco2-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # gtempco2
 
 gtempco2 is a PyPI application to display global temperature and co2 of land and ocean with NOAA datasets.
 
 NOAA monthly datasets on the global temperature of land and ocean and the global co2 will be automatically downloaded. 
 
-gtempco2 is to plot a graph for a user-specified time period with two lines representing global temperature and global CO2 levels. The graph includes first-order regression lines with coefficients and R-squared values.
+gtempco2 is to plot a graph for a user-specified time period with two lines representing global temperature and global CO2 levels. The graph includes first-order regression lines with coefficients, p-value and R-squared values.
 
 To install gtempco2, use the following pip command.
 
 $ pip install gtempco2
 
 To run gtempco2, the user-specified time period such as start-date and end-date is needed to plot a graph of the global temperature and co2 from start-date to end-date. 
 
@@ -16,17 +16,17 @@
 
 For example, 1958-03 indicates March 1958 when NOAA started the measurement of the global co2.
 
 <pre>
 $ gtempco2
 enter start_date: e.g. 1960-04
 co2 measurement started from 1958-03
-yyyy-mo: 1960-06
+yyyy-mo: 1958-03
 enter end_date: e.g. 2023-04
-yyyy-mo: 1965-06
-start_date= 1960-06 end_date= 1965-06
+yyyy-mo: 1965-03
+start_date= 1958-03 end_date= 1965-03
 </pre>
 
 The system will ask the start-date and end-date. The result will be shown and saved in the directory as follows.
 
-<img src='https://github.com/ytakefuji/gtempco2/raw/main/1960-06_1965-06.png' height=450 width=600>
+<img src='https://github.com/y-takefuji/gtempco2/raw/main/1958-03_1965-03.png' height=450 width=600>
```

### Comparing `gtempco2-0.0.8/setup.py` & `gtempco2-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gtempco2",
-    version="0.0.8",
+    version="0.0.9",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for displaying global temperature and co2",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/gtempco2",
+    url="https://github.com/y-takefuji/gtempco2",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/gtempco2",
+        "Bug Tracker": "https://github.com/y-takefuji/gtempco2",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
```

### Comparing `gtempco2-0.0.8/src/gtempco2.egg-info/PKG-INFO` & `gtempco2-0.0.9/src/gtempco2.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: gtempco2
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for displaying global temperature and co2
-Home-page: https://github.com/ytakefuji/gtempco2
+Home-page: https://github.com/y-takefuji/gtempco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/gtempco2
+Project-URL: Bug Tracker, https://github.com/y-takefuji/gtempco2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # gtempco2
 
 gtempco2 is a PyPI application to display global temperature and co2 of land and ocean with NOAA datasets.
 
 NOAA monthly datasets on the global temperature of land and ocean and the global co2 will be automatically downloaded. 
 
-gtempco2 is to plot a graph for a user-specified time period with two lines representing global temperature and global CO2 levels. The graph includes first-order regression lines with coefficients and R-squared values.
+gtempco2 is to plot a graph for a user-specified time period with two lines representing global temperature and global CO2 levels. The graph includes first-order regression lines with coefficients, p-value and R-squared values.
 
 To install gtempco2, use the following pip command.
 
 $ pip install gtempco2
 
 To run gtempco2, the user-specified time period such as start-date and end-date is needed to plot a graph of the global temperature and co2 from start-date to end-date. 
 
@@ -32,19 +32,19 @@
 
 For example, 1958-03 indicates March 1958 when NOAA started the measurement of the global co2.
 
 <pre>
 $ gtempco2
 enter start_date: e.g. 1960-04
 co2 measurement started from 1958-03
-yyyy-mo: 1960-06
+yyyy-mo: 1958-03
 enter end_date: e.g. 2023-04
-yyyy-mo: 1965-06
-start_date= 1960-06 end_date= 1965-06
+yyyy-mo: 1965-03
+start_date= 1958-03 end_date= 1965-03
 </pre>
 
 The system will ask the start-date and end-date. The result will be shown and saved in the directory as follows.
 
-<img src='https://github.com/ytakefuji/gtempco2/raw/main/1960-06_1965-06.png' height=450 width=600>
+<img src='https://github.com/y-takefuji/gtempco2/raw/main/1958-03_1965-03.png' height=450 width=600>
```

### Comparing `gtempco2-0.0.8/src/gtempco2.py` & `gtempco2-0.0.9/src/gtempco2.py`

 * *Files identical despite different names*

