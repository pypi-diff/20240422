# Comparing `tmp/vud4-0.0.3.tar.gz` & `tmp/vud4-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vud4-0.0.3.tar", last modified: Sun Feb 26 23:13:10 2023, max compression
+gzip compressed data, was "vud4-0.0.4.tar", last modified: Mon Apr 22 08:17:56 2024, max compression
```

## Comparing `vud4-0.0.3.tar` & `vud4-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-02-26 23:13:10.343896 vud4-0.0.3/
--rw-r--r--   0 yt        (1000) yt        (1000)     1236 2023-02-26 23:13:10.343896 vud4-0.0.3/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      678 2023-02-26 23:11:40.000000 vud4-0.0.3/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-02-26 23:13:10.343896 vud4-0.0.3/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      966 2023-02-26 23:11:07.000000 vud4-0.0.3/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-02-26 23:13:10.328002 vud4-0.0.3/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-02-26 23:13:10.328002 vud4-0.0.3/src/vud4.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1236 2023-02-26 23:13:09.000000 vud4-0.0.3/src/vud4.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      193 2023-02-26 23:13:09.000000 vud4-0.0.3/src/vud4.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-02-26 23:13:09.000000 vud4-0.0.3/src/vud4.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       36 2023-02-26 23:13:09.000000 vud4-0.0.3/src/vud4.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        5 2023-02-26 23:13:09.000000 vud4-0.0.3/src/vud4.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     2020 2023-02-23 07:20:43.000000 vud4-0.0.3/src/vud4.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:17:56.669390 vud4-0.0.4/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1702 2024-04-22 08:17:56.669390 vud4-0.0.4/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1142 2024-04-22 08:16:35.000000 vud4-0.0.4/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 08:17:56.669390 vud4-0.0.4/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      968 2024-04-22 08:15:58.000000 vud4-0.0.4/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:17:56.669390 vud4-0.0.4/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:17:56.669390 vud4-0.0.4/src/vud4.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1702 2024-04-22 08:17:56.000000 vud4-0.0.4/src/vud4.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      193 2024-04-22 08:17:56.000000 vud4-0.0.4/src/vud4.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 08:17:56.000000 vud4-0.0.4/src/vud4.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       36 2024-04-22 08:17:56.000000 vud4-0.0.4/src/vud4.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        5 2024-04-22 08:17:56.000000 vud4-0.0.4/src/vud4.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2020 2023-02-23 07:20:43.000000 vud4-0.0.4/src/vud4.py
```

### Comparing `vud4-0.0.3/PKG-INFO` & `vud4-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 Metadata-Version: 2.1
 Name: vud4
-Version: 0.0.3
+Version: 0.0.4
 Summary: comparing effects on mortality between bivalent booster, fully vaccinated and unvaccinated
-Home-page: https://github.com/ytakefuji/vud4
+Home-page: https://github.com/y-takefuji/vud4
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/vud4
+Project-URL: Bug Tracker, https://github.com/y-takefuji/vud4
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # vud4
-This is under review.
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/1960114/tree)
+
+
+Takefuji Y. Vaccine effects on COVID-19 infection with bivalent boosting by age group. Drug Resist Updat. 2023 Dec 27;73:101039. doi: 10.1016/j.drup.2023.101039. Epub ahead of print. PMID: 38169273.
 
 vud4.py is to calculate the time-series effect of vaccination on mortality in six age groups (18-29 years, 30-49 years, 50-64 years, 65-79 years, 80+ years, and all ages) for three vaccination types: bivalent booster, fully vaccinated, and unvaccinated. The CDC dataset for the period October 1, 2021 through January 23, 2023 was used for this study:
 https://data.cdc.gov/api/views/54ys-qyzm/rows.csv
+
+vud4 is a PyPI application. PyPI allows vud4 to run on Windows, MacOS and Linux Operating Systems as long as Python is installed on the system.
+
 # How to install vud4
 $ pip install vud4
+
 # How to run vud4
 $ vud4
 
 enter one of age groups: vud4 80+
 
 18-29,30-49,50-64,65-79,80+,all_ages
 
 $ vud4 80+
 
-<img src='https://github.com/ytakefuji/vud4/raw/main/bivalent_80%2B.png' height=240 width=280>
+<img src='https://github.com/y-takefuji/vud4/raw/main/bivalent_80%2B.png' height=240 width=280>
```

### Comparing `vud4-0.0.3/setup.py` & `vud4-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vud4",
-    version="0.0.3",
+    version="0.0.4",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="comparing effects on mortality between bivalent booster, fully vaccinated and unvaccinated",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/vud4",
+    url="https://github.com/y-takefuji/vud4",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/vud4",
+        "Bug Tracker": "https://github.com/y-takefuji/vud4",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['vud4'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'vud4 = vud4:main'
         ]
     },
 )
```

### Comparing `vud4-0.0.3/src/vud4.egg-info/PKG-INFO` & `vud4-0.0.4/src/vud4.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 Metadata-Version: 2.1
 Name: vud4
-Version: 0.0.3
+Version: 0.0.4
 Summary: comparing effects on mortality between bivalent booster, fully vaccinated and unvaccinated
-Home-page: https://github.com/ytakefuji/vud4
+Home-page: https://github.com/y-takefuji/vud4
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/vud4
+Project-URL: Bug Tracker, https://github.com/y-takefuji/vud4
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # vud4
-This is under review.
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/1960114/tree)
+
+
+Takefuji Y. Vaccine effects on COVID-19 infection with bivalent boosting by age group. Drug Resist Updat. 2023 Dec 27;73:101039. doi: 10.1016/j.drup.2023.101039. Epub ahead of print. PMID: 38169273.
 
 vud4.py is to calculate the time-series effect of vaccination on mortality in six age groups (18-29 years, 30-49 years, 50-64 years, 65-79 years, 80+ years, and all ages) for three vaccination types: bivalent booster, fully vaccinated, and unvaccinated. The CDC dataset for the period October 1, 2021 through January 23, 2023 was used for this study:
 https://data.cdc.gov/api/views/54ys-qyzm/rows.csv
+
+vud4 is a PyPI application. PyPI allows vud4 to run on Windows, MacOS and Linux Operating Systems as long as Python is installed on the system.
+
 # How to install vud4
 $ pip install vud4
+
 # How to run vud4
 $ vud4
 
 enter one of age groups: vud4 80+
 
 18-29,30-49,50-64,65-79,80+,all_ages
 
 $ vud4 80+
 
-<img src='https://github.com/ytakefuji/vud4/raw/main/bivalent_80%2B.png' height=240 width=280>
+<img src='https://github.com/y-takefuji/vud4/raw/main/bivalent_80%2B.png' height=240 width=280>
```

### Comparing `vud4-0.0.3/src/vud4.py` & `vud4-0.0.4/src/vud4.py`

 * *Files identical despite different names*

