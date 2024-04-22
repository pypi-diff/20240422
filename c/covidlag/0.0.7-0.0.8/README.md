# Comparing `tmp/covidlag-0.0.7.tar.gz` & `tmp/covidlag-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/covidlag-0.0.7.tar", last modified: Sun Oct 10 03:00:03 2021, max compression
+gzip compressed data, was "covidlag-0.0.8.tar", last modified: Mon Apr 22 07:31:09 2024, max compression
```

## Comparing `covidlag-0.0.7.tar` & `covidlag-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-10-10 03:00:03.770979 covidlag-0.0.7/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     5759 2021-10-10 03:00:03.770979 covidlag-0.0.7/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     5242 2021-10-10 02:58:07.000000 covidlag-0.0.7/README.md
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2021-10-10 03:00:03.770979 covidlag-0.0.7/setup.cfg
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      937 2021-10-10 02:58:47.000000 covidlag-0.0.7/setup.py
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-10-10 03:00:03.754981 covidlag-0.0.7/src/
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-10-10 03:00:03.767003 covidlag-0.0.7/src/covidlag.egg-info/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     5759 2021-10-10 03:00:02.000000 covidlag-0.0.7/src/covidlag.egg-info/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      217 2021-10-10 03:00:02.000000 covidlag-0.0.7/src/covidlag.egg-info/SOURCES.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2021-10-10 03:00:02.000000 covidlag-0.0.7/src/covidlag.egg-info/dependency_links.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       44 2021-10-10 03:00:02.000000 covidlag-0.0.7/src/covidlag.egg-info/entry_points.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        9 2021-10-10 03:00:02.000000 covidlag-0.0.7/src/covidlag.egg-info/top_level.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4248 2021-10-10 02:39:10.000000 covidlag-0.0.7/src/covidlag.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:31:09.569365 covidlag-0.0.8/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     6570 2024-04-22 07:31:09.569365 covidlag-0.0.8/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     6051 2024-04-22 07:30:29.000000 covidlag-0.0.8/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 07:31:09.569365 covidlag-0.0.8/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      939 2024-04-22 07:29:41.000000 covidlag-0.0.8/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:31:09.569365 covidlag-0.0.8/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:31:09.569365 covidlag-0.0.8/src/covidlag.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     6570 2024-04-22 07:31:09.000000 covidlag-0.0.8/src/covidlag.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      217 2024-04-22 07:31:09.000000 covidlag-0.0.8/src/covidlag.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 07:31:09.000000 covidlag-0.0.8/src/covidlag.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       44 2024-04-22 07:31:09.000000 covidlag-0.0.8/src/covidlag.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        9 2024-04-22 07:31:09.000000 covidlag-0.0.8/src/covidlag.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4248 2021-10-10 02:39:10.000000 covidlag-0.0.8/src/covidlag.py
```

### Comparing `covidlag-0.0.7/PKG-INFO` & `covidlag-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1
-Name: covidlag
-Version: 0.0.7
-Summary: lag time and case fatality rate (CFR)
-Home-page: https://github.com/ytakefuji/covidlag
-Author: yoshiyasu takefuji
-Author-email: takefuji@keio.jp
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/covidlag
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+# covidlag 
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/40b2361d-b5c9-43b4-820c-b767ea1a6e9a/tree)
+
+DOI: https://doi.org/10.24433/CO.8676218.v1
+
+Published papers on covidlag:
+Takefuji Y. Python Programming in PyPI for Translational Medicine. International Journal of Translational Medicine. 2021; 1(3):323-331. https://doi.org/10.3390/ijtm1030019 
+
+Takefuji, Y. COVID-19 lag time and case fatality rate calculation tool, as well as a tool to identify when policymakers made mistakes. Netw Model Anal Health Inform Bioinforma 12, 33 (2023). https://doi.org/10.1007/s13721-023-00430-5
+
+covidlag has been downloaded 21400 times worldwide.
+
+Another is under review.
 
-# covidlag
 Data science is useful to investigate the progression of the pandemic. 
 
 covidlag is an open-source program which is available in public and 
 can be installed by the PyPI package command (pip).
 covidlag can calculate the lag time between infection peaks and death peaks.
 covidlag can also compute death rate per infection or case fatality ratio (CFR).
 CFR is the proportion of individuals diagnosed with a disease who die from 
@@ -55,24 +52,26 @@
 
 # How to install covidlag
 Covidlag is available in public and can be installed by the following 
 PyPI packaging command:
 
 $ pip install covidlag
 
+$ pip install covidlag --force-reinstall --no-cache-dir --no-binary :all:
+
 # How to run covidlag
 covidlag needs at least three parameters (country name, sampled days, 
 regression polinomial degree).
 
 Run the following command composed of the country name, sampled days, the degree
 of polynomial curve-fitting, and options (L: left, R: right, C: center):
 
 $ covidlag 'United States' 600 13 L
 
-<img src='https://github.com/ytakefuji/covidlag/raw/main/United States.png' height=480 width=640>
+<img src='https://github.com/y-takefuji/covidlag/raw/main/United States.png' height=480 width=640>
 This example shows that r-squared of infections:0.803 and r-squared of deaths:0.733
 
 The death peaks are [ 66, 182, 332, 464, 574].
 The case peaks are [ 47, 150, 309, 441, 562].
 <pre>
 maxima information
 death peak: 2020-04-23
@@ -149,27 +148,25 @@
 The number of every case peak is [526 4421 5902 20029]
 
 Therefore, death rate of peaks or CFR is 88/4421=0.019, 92/5902=0.015, and
 54/20029=0.0026 respectively.
 
 The CFR is significantly decreasing.
 
-<img src='https://github.com/ytakefuji/covidlag/raw/main/Japan.png' height=480 width=640>
+<img src='https://github.com/y-takefuji/covidlag/raw/main/Japan.png' height=480 width=640>
 
 $ covidlag Canada 400 13 L
 
-<img src='https://github.com/ytakefuji/covidlag/raw/main/Canada.png' height=480 width=640>
+<img src='https://github.com/y-takefuji/covidlag/raw/main/Canada.png' height=480 width=640>
 <pre>
 death peak: 2020-09-07
 death peak: 2021-01-06
 death peak: 2021-05-08
 death peak: 2021-09-25
 case peak: 2020-09-07
 case peak: 2020-12-26
 case peak: 2021-04-21
 case peak: 2021-09-19
 </pre>
 The lag time is 11 days, 17 days,...
 
 The death rate per infection is 0.018,0.006,...
-
-
```

### Comparing `covidlag-0.0.7/setup.py` & `covidlag-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="covidlag",
-    version="0.0.7",
+    version="0.0.8",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="lag time and case fatality rate (CFR)",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/covidlag",
+    url="https://github.com/y-takefuji/covidlag",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/covidlag",
+        "Bug Tracker": "https://github.com/y-takefuji/covidlag",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['covidlag'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'covidlag = covidlag:main'
         ]
     },
 )
```

### Comparing `covidlag-0.0.7/src/covidlag.egg-info/PKG-INFO` & `covidlag-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 Metadata-Version: 2.1
 Name: covidlag
-Version: 0.0.7
+Version: 0.0.8
 Summary: lag time and case fatality rate (CFR)
-Home-page: https://github.com/ytakefuji/covidlag
+Home-page: https://github.com/y-takefuji/covidlag
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/covidlag
+Project-URL: Bug Tracker, https://github.com/y-takefuji/covidlag
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# covidlag
+# covidlag 
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/40b2361d-b5c9-43b4-820c-b767ea1a6e9a/tree)
+
+DOI: https://doi.org/10.24433/CO.8676218.v1
+
+Published papers on covidlag:
+Takefuji Y. Python Programming in PyPI for Translational Medicine. International Journal of Translational Medicine. 2021; 1(3):323-331. https://doi.org/10.3390/ijtm1030019 
+
+Takefuji, Y. COVID-19 lag time and case fatality rate calculation tool, as well as a tool to identify when policymakers made mistakes. Netw Model Anal Health Inform Bioinforma 12, 33 (2023). https://doi.org/10.1007/s13721-023-00430-5
+
+covidlag has been downloaded 21400 times worldwide.
+
+Another is under review.
+
 Data science is useful to investigate the progression of the pandemic. 
 
 covidlag is an open-source program which is available in public and 
 can be installed by the PyPI package command (pip).
 covidlag can calculate the lag time between infection peaks and death peaks.
 covidlag can also compute death rate per infection or case fatality ratio (CFR).
 CFR is the proportion of individuals diagnosed with a disease who die from 
@@ -55,24 +68,26 @@
 
 # How to install covidlag
 Covidlag is available in public and can be installed by the following 
 PyPI packaging command:
 
 $ pip install covidlag
 
+$ pip install covidlag --force-reinstall --no-cache-dir --no-binary :all:
+
 # How to run covidlag
 covidlag needs at least three parameters (country name, sampled days, 
 regression polinomial degree).
 
 Run the following command composed of the country name, sampled days, the degree
 of polynomial curve-fitting, and options (L: left, R: right, C: center):
 
 $ covidlag 'United States' 600 13 L
 
-<img src='https://github.com/ytakefuji/covidlag/raw/main/United States.png' height=480 width=640>
+<img src='https://github.com/y-takefuji/covidlag/raw/main/United States.png' height=480 width=640>
 This example shows that r-squared of infections:0.803 and r-squared of deaths:0.733
 
 The death peaks are [ 66, 182, 332, 464, 574].
 The case peaks are [ 47, 150, 309, 441, 562].
 <pre>
 maxima information
 death peak: 2020-04-23
@@ -149,19 +164,19 @@
 The number of every case peak is [526 4421 5902 20029]
 
 Therefore, death rate of peaks or CFR is 88/4421=0.019, 92/5902=0.015, and
 54/20029=0.0026 respectively.
 
 The CFR is significantly decreasing.
 
-<img src='https://github.com/ytakefuji/covidlag/raw/main/Japan.png' height=480 width=640>
+<img src='https://github.com/y-takefuji/covidlag/raw/main/Japan.png' height=480 width=640>
 
 $ covidlag Canada 400 13 L
 
-<img src='https://github.com/ytakefuji/covidlag/raw/main/Canada.png' height=480 width=640>
+<img src='https://github.com/y-takefuji/covidlag/raw/main/Canada.png' height=480 width=640>
 <pre>
 death peak: 2020-09-07
 death peak: 2021-01-06
 death peak: 2021-05-08
 death peak: 2021-09-25
 case peak: 2020-09-07
 case peak: 2020-12-26
```

### Comparing `covidlag-0.0.7/src/covidlag.py` & `covidlag-0.0.8/src/covidlag.py`

 * *Files identical despite different names*

