# Comparing `tmp/vuc3-0.0.1.tar.gz` & `tmp/vuc3-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vuc3-0.0.1.tar", last modified: Sat Mar  4 02:05:11 2023, max compression
+gzip compressed data, was "vuc3-0.0.2.tar", last modified: Mon Apr 22 08:11:46 2024, max compression
```

## Comparing `vuc3-0.0.1.tar` & `vuc3-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-03-04 02:05:11.689613 vuc3-0.0.1/
--rw-r--r--   0 yt        (1000) yt        (1000)     1317 2023-03-04 02:05:11.689613 vuc3-0.0.1/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      791 2023-03-04 02:04:08.000000 vuc3-0.0.1/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-03-04 02:05:11.689613 vuc3-0.0.1/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      934 2023-03-04 01:56:05.000000 vuc3-0.0.1/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-03-04 02:05:11.667960 vuc3-0.0.1/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-03-04 02:05:11.689613 vuc3-0.0.1/src/vuc3.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1317 2023-03-04 02:05:10.000000 vuc3-0.0.1/src/vuc3.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      193 2023-03-04 02:05:10.000000 vuc3-0.0.1/src/vuc3.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-03-04 02:05:10.000000 vuc3-0.0.1/src/vuc3.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       36 2023-03-04 02:05:10.000000 vuc3-0.0.1/src/vuc3.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        5 2023-03-04 02:05:10.000000 vuc3-0.0.1/src/vuc3.egg-info/top_level.txt
--rwxr-xr-x   0 yt        (1000) yt        (1000)     2198 2023-03-04 01:53:17.000000 vuc3-0.0.1/src/vuc3.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:11:46.009386 vuc3-0.0.2/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1459 2024-04-22 08:11:46.009386 vuc3-0.0.2/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      931 2024-04-22 08:11:16.000000 vuc3-0.0.2/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 08:11:46.009386 vuc3-0.0.2/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      936 2024-04-22 08:10:38.000000 vuc3-0.0.2/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:11:46.009386 vuc3-0.0.2/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:11:46.009386 vuc3-0.0.2/src/vuc3.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1459 2024-04-22 08:11:45.000000 vuc3-0.0.2/src/vuc3.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      193 2024-04-22 08:11:45.000000 vuc3-0.0.2/src/vuc3.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 08:11:45.000000 vuc3-0.0.2/src/vuc3.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       36 2024-04-22 08:11:45.000000 vuc3-0.0.2/src/vuc3.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        5 2024-04-22 08:11:45.000000 vuc3-0.0.2/src/vuc3.egg-info/top_level.txt
+-rwxr-xr-x   0 takefuji  (1000) takefuji  (1000)     2198 2023-03-04 01:53:17.000000 vuc3-0.0.2/src/vuc3.py
```

### Comparing `vuc3-0.0.1/PKG-INFO` & `vuc3-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: vuc3
-Version: 0.0.1
+Version: 0.0.2
 Summary: effects of vaccines on COVID-19 infection and mortality
-Home-page: https://github.com/ytakefuji/patient
+Home-page: https://github.com/y-takefuji/patient
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/vuc3
+Project-URL: Bug Tracker, https://github.com/y-takefuji/vuc3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # vuc3
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/6096647/tree)
+
 This is under review.
 
-vuc3.py is a Python program to invesitigate effects of vaccines on COVID-19 mortality and infection between the second booster, the fist booster, fully vaccinated and unvaccinated.
+vuc3.py is a Python program to invesitigate effects of vaccines on COVID-19 mortality and infection between the second booster, the first booster, fully vaccinated and unvaccinated.
 
 CDC dataset is used for this study:
 https://data.cdc.gov/api/views/ukww-au2k/rows.csv
 
 vuc3 is a PyPI application which runs on Windows, MacOS, and Linux Operating Systems
 as long as Python is installed on the system. Three determinants should be given to uvc3 such as age group (50-64, 65+ or all_ages), product (Pfizer, Moderna, Janssen, and all_types), and outcome (death or case).
 
 # How to install vuc3
 $ pip install vuc3
 
 # How to run vuc3
 $ vuc3 all_ages Pfizer death
 
-<img src='https://github.com/ytakefuji/vuc3/raw/main/death_Pfizer_all_ages.png' width=534 height=470 >
+<img src='https://github.com/y-takefuji/vuc3/raw/main/death_Pfizer_all_ages.png' width=534 height=470 >
```

### Comparing `vuc3-0.0.1/setup.py` & `vuc3-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vuc3",
-    version="0.0.1",
+    version="0.0.2",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="effects of vaccines on COVID-19 infection and mortality",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/patient",
+    url="https://github.com/y-takefuji/patient",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/vuc3",
+        "Bug Tracker": "https://github.com/y-takefuji/vuc3",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
```

### Comparing `vuc3-0.0.1/src/vuc3.egg-info/PKG-INFO` & `vuc3-0.0.2/src/vuc3.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: vuc3
-Version: 0.0.1
+Version: 0.0.2
 Summary: effects of vaccines on COVID-19 infection and mortality
-Home-page: https://github.com/ytakefuji/patient
+Home-page: https://github.com/y-takefuji/patient
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/vuc3
+Project-URL: Bug Tracker, https://github.com/y-takefuji/vuc3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # vuc3
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/6096647/tree)
+
 This is under review.
 
-vuc3.py is a Python program to invesitigate effects of vaccines on COVID-19 mortality and infection between the second booster, the fist booster, fully vaccinated and unvaccinated.
+vuc3.py is a Python program to invesitigate effects of vaccines on COVID-19 mortality and infection between the second booster, the first booster, fully vaccinated and unvaccinated.
 
 CDC dataset is used for this study:
 https://data.cdc.gov/api/views/ukww-au2k/rows.csv
 
 vuc3 is a PyPI application which runs on Windows, MacOS, and Linux Operating Systems
 as long as Python is installed on the system. Three determinants should be given to uvc3 such as age group (50-64, 65+ or all_ages), product (Pfizer, Moderna, Janssen, and all_types), and outcome (death or case).
 
 # How to install vuc3
 $ pip install vuc3
 
 # How to run vuc3
 $ vuc3 all_ages Pfizer death
 
-<img src='https://github.com/ytakefuji/vuc3/raw/main/death_Pfizer_all_ages.png' width=534 height=470 >
+<img src='https://github.com/y-takefuji/vuc3/raw/main/death_Pfizer_all_ages.png' width=534 height=470 >
```

### Comparing `vuc3-0.0.1/src/vuc3.py` & `vuc3-0.0.2/src/vuc3.py`

 * *Files identical despite different names*

