# Comparing `tmp/noaatsi-0.0.1.tar.gz` & `tmp/noaatsi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noaatsi-0.0.1.tar", last modified: Sun Apr 10 09:38:09 2022, max compression
+gzip compressed data, was "noaatsi-0.0.2.tar", last modified: Mon Apr 22 08:33:52 2024, max compression
```

## Comparing `noaatsi-0.0.1.tar` & `noaatsi-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-10 09:38:09.266849 noaatsi-0.0.1/
--rw-r--r--   0 yt        (1000) yt        (1000)     1312 2022-04-10 09:38:09.265009 noaatsi-0.0.1/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      787 2022-04-10 09:33:17.000000 noaatsi-0.0.1/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2022-04-10 09:38:09.266849 noaatsi-0.0.1/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      942 2022-04-10 02:29:33.000000 noaatsi-0.0.1/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-10 09:38:09.251807 noaatsi-0.0.1/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-10 09:38:09.264251 noaatsi-0.0.1/src/noaatsi.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1312 2022-04-10 09:38:08.000000 noaatsi-0.0.1/src/noaatsi.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      211 2022-04-10 09:38:08.000000 noaatsi-0.0.1/src/noaatsi.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2022-04-10 09:38:08.000000 noaatsi-0.0.1/src/noaatsi.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       42 2022-04-10 09:38:08.000000 noaatsi-0.0.1/src/noaatsi.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        8 2022-04-10 09:38:08.000000 noaatsi-0.0.1/src/noaatsi.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1130 2022-04-10 09:37:04.000000 noaatsi-0.0.1/src/noaatsi.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:33:52.029398 noaatsi-0.0.2/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1603 2024-04-22 08:33:52.029398 noaatsi-0.0.2/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1076 2024-04-22 08:33:00.000000 noaatsi-0.0.2/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 08:33:52.029398 noaatsi-0.0.2/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      944 2024-04-22 08:33:36.000000 noaatsi-0.0.2/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:33:52.029398 noaatsi-0.0.2/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:33:52.029398 noaatsi-0.0.2/src/noaatsi.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1603 2024-04-22 08:33:52.000000 noaatsi-0.0.2/src/noaatsi.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      211 2024-04-22 08:33:52.000000 noaatsi-0.0.2/src/noaatsi.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 08:33:52.000000 noaatsi-0.0.2/src/noaatsi.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       42 2024-04-22 08:33:52.000000 noaatsi-0.0.2/src/noaatsi.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        8 2024-04-22 08:33:52.000000 noaatsi-0.0.2/src/noaatsi.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1130 2022-04-10 09:37:04.000000 noaatsi-0.0.2/src/noaatsi.py
```

### Comparing `noaatsi-0.0.1/PKG-INFO` & `noaatsi-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: noaatsi
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for displaying TSI graph based on NOAA
-Home-page: https://github.com/ytakefuji/noaatsi
+Home-page: https://github.com/y-takefuji/noaatsi
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/noaatsi
+Project-URL: Bug Tracker, https://github.com/y-takefuji/noaatsi
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # noaatsi
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/5710884/tree )
+
+takefuji (2022) noaatsi: a PyPI for displaying TSI graph based on NOAA [Source Code]. https://doi.org/10.24433/CO.6916537.v1
+
+This is under review.
+
 noaatsi is a PyPI package application to scrape the updated data from NOAA on TSI and to display the TSI graph.
 Data is stored in the following site which will be automatically scraped by noaatsi:
 
 https://www.ncei.noaa.gov/data/total-solar-irradiance/access/yearly/tsi_v02r01_yearly_s1610_e2021_c20220202.nc
 
 NOAA file is based on netCDF4.
 In order to read .nc file, netCDF4 library is needed. To install it, run the following command.
@@ -32,10 +38,10 @@
 To generate TSI file (tsi.csv) and the graph on the screen (tsi.png), run the following command.
 
 $ noaatsi
 
 
 noaatsi.png is finally generated.
 
-<img src='https://github.com/ytakefuji/noaatsi/raw/main/noaatsi.png' height=300 width=900>
+<img src='https://github.com/y-takefuji/noaatsi/raw/main/noaatsi.png' height=300 width=900>
```

### Comparing `noaatsi-0.0.1/setup.py` & `noaatsi-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="noaatsi",
-    version="0.0.1",
+    version="0.0.2",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for displaying TSI graph based on NOAA",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/noaatsi",
+    url="https://github.com/y-takefuji/noaatsi",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/noaatsi",
+        "Bug Tracker": "https://github.com/y-takefuji/noaatsi",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['noaatsi'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'noaatsi = noaatsi:main'
         ]
     },
 )
```

### Comparing `noaatsi-0.0.1/src/noaatsi.egg-info/PKG-INFO` & `noaatsi-0.0.2/src/noaatsi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: noaatsi
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for displaying TSI graph based on NOAA
-Home-page: https://github.com/ytakefuji/noaatsi
+Home-page: https://github.com/y-takefuji/noaatsi
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/noaatsi
+Project-URL: Bug Tracker, https://github.com/y-takefuji/noaatsi
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # noaatsi
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/5710884/tree )
+
+takefuji (2022) noaatsi: a PyPI for displaying TSI graph based on NOAA [Source Code]. https://doi.org/10.24433/CO.6916537.v1
+
+This is under review.
+
 noaatsi is a PyPI package application to scrape the updated data from NOAA on TSI and to display the TSI graph.
 Data is stored in the following site which will be automatically scraped by noaatsi:
 
 https://www.ncei.noaa.gov/data/total-solar-irradiance/access/yearly/tsi_v02r01_yearly_s1610_e2021_c20220202.nc
 
 NOAA file is based on netCDF4.
 In order to read .nc file, netCDF4 library is needed. To install it, run the following command.
@@ -32,10 +38,10 @@
 To generate TSI file (tsi.csv) and the graph on the screen (tsi.png), run the following command.
 
 $ noaatsi
 
 
 noaatsi.png is finally generated.
 
-<img src='https://github.com/ytakefuji/noaatsi/raw/main/noaatsi.png' height=300 width=900>
+<img src='https://github.com/y-takefuji/noaatsi/raw/main/noaatsi.png' height=300 width=900>
```

### Comparing `noaatsi-0.0.1/src/noaatsi.py` & `noaatsi-0.0.2/src/noaatsi.py`

 * *Files identical despite different names*

