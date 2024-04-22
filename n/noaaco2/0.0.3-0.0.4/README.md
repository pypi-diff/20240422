# Comparing `tmp/noaaco2-0.0.3.tar.gz` & `tmp/noaaco2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noaaco2-0.0.3.tar", last modified: Mon Apr 18 01:41:21 2022, max compression
+gzip compressed data, was "noaaco2-0.0.4.tar", last modified: Mon Apr 22 08:21:43 2024, max compression
```

## Comparing `noaaco2-0.0.3.tar` & `noaaco2-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-18 01:41:21.685890 noaaco2-0.0.3/
--rw-r--r--   0 yt        (1000) yt        (1000)     2863 2022-04-18 01:41:21.685890 noaaco2-0.0.3/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     2338 2022-04-15 10:54:36.000000 noaaco2-0.0.3/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2022-04-18 01:41:21.685890 noaaco2-0.0.3/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      942 2022-04-18 01:40:58.000000 noaaco2-0.0.3/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-18 01:41:21.672292 noaaco2-0.0.3/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-18 01:41:21.685890 noaaco2-0.0.3/src/noaaco2.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     2863 2022-04-18 01:41:21.000000 noaaco2-0.0.3/src/noaaco2.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      211 2022-04-18 01:41:21.000000 noaaco2-0.0.3/src/noaaco2.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2022-04-18 01:41:21.000000 noaaco2-0.0.3/src/noaaco2.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       42 2022-04-18 01:41:21.000000 noaaco2-0.0.3/src/noaaco2.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        8 2022-04-18 01:41:21.000000 noaaco2-0.0.3/src/noaaco2.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1228 2022-04-18 01:40:45.000000 noaaco2-0.0.3/src/noaaco2.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:21:43.099392 noaaco2-0.0.4/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4612 2024-04-22 08:21:43.099392 noaaco2-0.0.4/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4085 2024-04-22 08:20:31.000000 noaaco2-0.0.4/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 08:21:43.099392 noaaco2-0.0.4/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      944 2024-04-22 08:21:21.000000 noaaco2-0.0.4/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:21:43.099392 noaaco2-0.0.4/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:21:43.099392 noaaco2-0.0.4/src/noaaco2.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4612 2024-04-22 08:21:43.000000 noaaco2-0.0.4/src/noaaco2.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      211 2024-04-22 08:21:43.000000 noaaco2-0.0.4/src/noaaco2.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 08:21:43.000000 noaaco2-0.0.4/src/noaaco2.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       42 2024-04-22 08:21:43.000000 noaaco2-0.0.4/src/noaaco2.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        8 2024-04-22 08:21:43.000000 noaaco2-0.0.4/src/noaaco2.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1228 2022-04-18 01:40:45.000000 noaaco2-0.0.4/src/noaaco2.py
```

### Comparing `noaaco2-0.0.3/PKG-INFO` & `noaaco2-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,77 @@
 Metadata-Version: 2.1
 Name: noaaco2
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for displaying co2 graph based on NOAA
-Home-page: https://github.com/ytakefuji/noaaco2
+Home-page: https://github.com/y-takefuji/noaaco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/noaaco2
+Project-URL: Bug Tracker, https://github.com/y-takefuji/noaaco2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # noaaco2
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/1444046/tree)
+
+Takefuji Y. (2022) noaaco2: PyPI application for displaying a CO2 graph based on NOAA [Source Code]. https://doi.org/10.24433/CO.7957917.v1
+
+This is under review.
+
 This is a tutorial to debut a PyPI application and to validate software reproducibility for climate professions.
 
 noaaco2 is a PyPI application that scrapes the latest dataset from NOAA via the Internet and 
 displays a graph for a specified number of months.
 
 The PyPI environment allows PyPI applications to run on Windows, MacOS, and Linux operating systems.
 As long as Python is installed on the system, you can use it without being aware of the operating system.
 
 noaaco2 scrapes the latest csv file from the following NOAA site:
 
 ftp://aftp.cmdl.noaa.gov/products/trends/co2/co2_mm_mlo.csv
+<pre>
+# --------------------------------------------------------------------							
+# USE OF NOAA GML DATA							
+#							
+# These data are made freely available to the public and the							
+# scientific community in the belief that their wide dissemination							
+# will lead to greater understanding and new scientific insights.							
+...
+# Scripps data downloaded from http://scrippsco2.ucsd.edu/data/atmospheric_co2							
+# Monthly values are corrected to center of month based on average seasonal							
+# cycle. Missing days can be asymmetric which would produce a high or low bias.							
+# Missing months have been interpolated	 for NOAA data indicated by negative stdev						
+# and uncertainty. We have no information for SIO data about Ndays	 stdv	 unc					
+# so that they are also indicated by negative numbers							
+# Monthly values are corrected to center of month based on average seasonal,,,,,,,
+# cycle. Missing days can be asymmetric which would produce a high or low bias.,,,,,,,
+# Missing months have been interpolated, for NOAA data indicated by negative stdev,,,,,,
+# and uncertainty. We have no information for SIO data about Ndays, stdv, unc,,,,,
+# so that they are also indicated by negative numbers,,,,,,,
+year,month,decimal date,average,interpolated,trend,ndays,
+1958,3,1958.2027,315.7,314.43,-1,-9.99,-0.99
+1958,4,1958.2877,317.45,315.16,-1,-9.99,-0.99
+1958,5,1958.3699,317.51,314.71,-1,-9.99,-0.99
+...
+</pre>
 
 noaaco2 can generate a graph with specified months and save it in result.csv and noaaco2.png.
 
 In order to run noaaco2 application, Python must be installed on your system.
 # How to install Python and noaaco2
 <pre>
 Follow the Python installation steps for Windows, WSL on Windows, MacOS, and Linux operating systems.
 1. Download a right installation file from miniconda site:
 https://docs.conda.io/en/latest/miniconda.html
 
-2. X-server installation is needed.
+2. X-server installation may be needed.
 For Windows 11 or 10,WSL on Windows 11 or 10, MacOS, X-server must be installed.
 X-server for Windows and WSL on Windows, install VcXsrv Windows X Server.
 You can download it from the following site:
 https://sourceforge.net/projects/vcxsrv/
 For MacOS, you must install XQuartz via Homebrew or brew command.
 For Linux operating systems, X-server is ready so that you don't need to install it.
 
@@ -63,11 +94,11 @@
 
 $ noaaco2
 
 For example, 24 months, run the following command.
 
 $ noaaco2 24
 
-<img src='https://github.com/ytakefuji/noaaco2/raw/main/noaaco2.png' width=850 height=340 >
+<img src='https://github.com/y-takefuji/noaaco2/raw/main/noaaco2.png' width=850 height=340 >
```

### Comparing `noaaco2-0.0.3/README.md` & `noaaco2-0.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,61 @@
 # noaaco2
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/1444046/tree)
+
+Takefuji Y. (2022) noaaco2: PyPI application for displaying a CO2 graph based on NOAA [Source Code]. https://doi.org/10.24433/CO.7957917.v1
+
+This is under review.
+
 This is a tutorial to debut a PyPI application and to validate software reproducibility for climate professions.
 
 noaaco2 is a PyPI application that scrapes the latest dataset from NOAA via the Internet and 
 displays a graph for a specified number of months.
 
 The PyPI environment allows PyPI applications to run on Windows, MacOS, and Linux operating systems.
 As long as Python is installed on the system, you can use it without being aware of the operating system.
 
 noaaco2 scrapes the latest csv file from the following NOAA site:
 
 ftp://aftp.cmdl.noaa.gov/products/trends/co2/co2_mm_mlo.csv
+<pre>
+# --------------------------------------------------------------------							
+# USE OF NOAA GML DATA							
+#							
+# These data are made freely available to the public and the							
+# scientific community in the belief that their wide dissemination							
+# will lead to greater understanding and new scientific insights.							
+...
+# Scripps data downloaded from http://scrippsco2.ucsd.edu/data/atmospheric_co2							
+# Monthly values are corrected to center of month based on average seasonal							
+# cycle. Missing days can be asymmetric which would produce a high or low bias.							
+# Missing months have been interpolated	 for NOAA data indicated by negative stdev						
+# and uncertainty. We have no information for SIO data about Ndays	 stdv	 unc					
+# so that they are also indicated by negative numbers							
+# Monthly values are corrected to center of month based on average seasonal,,,,,,,
+# cycle. Missing days can be asymmetric which would produce a high or low bias.,,,,,,,
+# Missing months have been interpolated, for NOAA data indicated by negative stdev,,,,,,
+# and uncertainty. We have no information for SIO data about Ndays, stdv, unc,,,,,
+# so that they are also indicated by negative numbers,,,,,,,
+year,month,decimal date,average,interpolated,trend,ndays,
+1958,3,1958.2027,315.7,314.43,-1,-9.99,-0.99
+1958,4,1958.2877,317.45,315.16,-1,-9.99,-0.99
+1958,5,1958.3699,317.51,314.71,-1,-9.99,-0.99
+...
+</pre>
 
 noaaco2 can generate a graph with specified months and save it in result.csv and noaaco2.png.
 
 In order to run noaaco2 application, Python must be installed on your system.
 # How to install Python and noaaco2
 <pre>
 Follow the Python installation steps for Windows, WSL on Windows, MacOS, and Linux operating systems.
 1. Download a right installation file from miniconda site:
 https://docs.conda.io/en/latest/miniconda.html
 
-2. X-server installation is needed.
+2. X-server installation may be needed.
 For Windows 11 or 10,WSL on Windows 11 or 10, MacOS, X-server must be installed.
 X-server for Windows and WSL on Windows, install VcXsrv Windows X Server.
 You can download it from the following site:
 https://sourceforge.net/projects/vcxsrv/
 For MacOS, you must install XQuartz via Homebrew or brew command.
 For Linux operating systems, X-server is ready so that you don't need to install it.
 
@@ -47,9 +78,9 @@
 
 $ noaaco2
 
 For example, 24 months, run the following command.
 
 $ noaaco2 24
 
-<img src='https://github.com/ytakefuji/noaaco2/raw/main/noaaco2.png' width=850 height=340 >
+<img src='https://github.com/y-takefuji/noaaco2/raw/main/noaaco2.png' width=850 height=340 >
```

### Comparing `noaaco2-0.0.3/setup.py` & `noaaco2-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="noaaco2",
-    version="0.0.3",
+    version="0.0.4",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for displaying co2 graph based on NOAA",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/noaaco2",
+    url="https://github.com/y-takefuji/noaaco2",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/noaaco2",
+        "Bug Tracker": "https://github.com/y-takefuji/noaaco2",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['noaaco2'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'noaaco2 = noaaco2:main'
         ]
     },
 )
```

### Comparing `noaaco2-0.0.3/src/noaaco2.egg-info/PKG-INFO` & `noaaco2-0.0.4/src/noaaco2.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,77 @@
 Metadata-Version: 2.1
 Name: noaaco2
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for displaying co2 graph based on NOAA
-Home-page: https://github.com/ytakefuji/noaaco2
+Home-page: https://github.com/y-takefuji/noaaco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/noaaco2
+Project-URL: Bug Tracker, https://github.com/y-takefuji/noaaco2
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # noaaco2
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/1444046/tree)
+
+Takefuji Y. (2022) noaaco2: PyPI application for displaying a CO2 graph based on NOAA [Source Code]. https://doi.org/10.24433/CO.7957917.v1
+
+This is under review.
+
 This is a tutorial to debut a PyPI application and to validate software reproducibility for climate professions.
 
 noaaco2 is a PyPI application that scrapes the latest dataset from NOAA via the Internet and 
 displays a graph for a specified number of months.
 
 The PyPI environment allows PyPI applications to run on Windows, MacOS, and Linux operating systems.
 As long as Python is installed on the system, you can use it without being aware of the operating system.
 
 noaaco2 scrapes the latest csv file from the following NOAA site:
 
 ftp://aftp.cmdl.noaa.gov/products/trends/co2/co2_mm_mlo.csv
+<pre>
+# --------------------------------------------------------------------							
+# USE OF NOAA GML DATA							
+#							
+# These data are made freely available to the public and the							
+# scientific community in the belief that their wide dissemination							
+# will lead to greater understanding and new scientific insights.							
+...
+# Scripps data downloaded from http://scrippsco2.ucsd.edu/data/atmospheric_co2							
+# Monthly values are corrected to center of month based on average seasonal							
+# cycle. Missing days can be asymmetric which would produce a high or low bias.							
+# Missing months have been interpolated	 for NOAA data indicated by negative stdev						
+# and uncertainty. We have no information for SIO data about Ndays	 stdv	 unc					
+# so that they are also indicated by negative numbers							
+# Monthly values are corrected to center of month based on average seasonal,,,,,,,
+# cycle. Missing days can be asymmetric which would produce a high or low bias.,,,,,,,
+# Missing months have been interpolated, for NOAA data indicated by negative stdev,,,,,,
+# and uncertainty. We have no information for SIO data about Ndays, stdv, unc,,,,,
+# so that they are also indicated by negative numbers,,,,,,,
+year,month,decimal date,average,interpolated,trend,ndays,
+1958,3,1958.2027,315.7,314.43,-1,-9.99,-0.99
+1958,4,1958.2877,317.45,315.16,-1,-9.99,-0.99
+1958,5,1958.3699,317.51,314.71,-1,-9.99,-0.99
+...
+</pre>
 
 noaaco2 can generate a graph with specified months and save it in result.csv and noaaco2.png.
 
 In order to run noaaco2 application, Python must be installed on your system.
 # How to install Python and noaaco2
 <pre>
 Follow the Python installation steps for Windows, WSL on Windows, MacOS, and Linux operating systems.
 1. Download a right installation file from miniconda site:
 https://docs.conda.io/en/latest/miniconda.html
 
-2. X-server installation is needed.
+2. X-server installation may be needed.
 For Windows 11 or 10,WSL on Windows 11 or 10, MacOS, X-server must be installed.
 X-server for Windows and WSL on Windows, install VcXsrv Windows X Server.
 You can download it from the following site:
 https://sourceforge.net/projects/vcxsrv/
 For MacOS, you must install XQuartz via Homebrew or brew command.
 For Linux operating systems, X-server is ready so that you don't need to install it.
 
@@ -63,11 +94,11 @@
 
 $ noaaco2
 
 For example, 24 months, run the following command.
 
 $ noaaco2 24
 
-<img src='https://github.com/ytakefuji/noaaco2/raw/main/noaaco2.png' width=850 height=340 >
+<img src='https://github.com/y-takefuji/noaaco2/raw/main/noaaco2.png' width=850 height=340 >
```

### Comparing `noaaco2-0.0.3/src/noaaco2.py` & `noaaco2-0.0.4/src/noaaco2.py`

 * *Files identical despite different names*

