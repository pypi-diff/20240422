# Comparing `tmp/cdcdeaths-0.0.1.tar.gz` & `tmp/cdcdeaths-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdcdeaths-0.0.1.tar", last modified: Tue Mar 15 06:08:41 2022, max compression
+gzip compressed data, was "cdcdeaths-0.0.2.tar", last modified: Mon Apr 22 09:00:17 2024, max compression
```

## Comparing `cdcdeaths-0.0.1.tar` & `cdcdeaths-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-03-15 06:08:41.679951 cdcdeaths-0.0.1/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1120 2022-03-15 06:08:41.673426 cdcdeaths-0.0.1/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      577 2022-03-15 06:00:58.000000 cdcdeaths-0.0.1/README.md
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2022-03-15 06:08:41.679951 cdcdeaths-0.0.1/setup.cfg
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      966 2022-03-15 06:07:17.000000 cdcdeaths-0.0.1/setup.py
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-03-15 06:08:41.657796 cdcdeaths-0.0.1/src/
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-03-15 06:08:41.673426 cdcdeaths-0.0.1/src/cdcdeaths.egg-info/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1120 2022-03-15 06:08:41.000000 cdcdeaths-0.0.1/src/cdcdeaths.egg-info/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      223 2022-03-15 06:08:41.000000 cdcdeaths-0.0.1/src/cdcdeaths.egg-info/SOURCES.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2022-03-15 06:08:41.000000 cdcdeaths-0.0.1/src/cdcdeaths.egg-info/dependency_links.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       46 2022-03-15 06:08:41.000000 cdcdeaths-0.0.1/src/cdcdeaths.egg-info/entry_points.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       10 2022-03-15 06:08:41.000000 cdcdeaths-0.0.1/src/cdcdeaths.egg-info/top_level.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      533 2022-03-15 05:29:30.000000 cdcdeaths-0.0.1/src/cdcdeaths.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 09:00:17.589412 cdcdeaths-0.0.2/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1335 2024-04-22 09:00:17.589412 cdcdeaths-0.0.2/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      790 2024-04-22 08:58:51.000000 cdcdeaths-0.0.2/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 09:00:17.589412 cdcdeaths-0.0.2/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      968 2024-04-22 08:59:28.000000 cdcdeaths-0.0.2/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 09:00:17.589412 cdcdeaths-0.0.2/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 09:00:17.589412 cdcdeaths-0.0.2/src/cdcdeaths.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1335 2024-04-22 09:00:17.000000 cdcdeaths-0.0.2/src/cdcdeaths.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      223 2024-04-22 09:00:17.000000 cdcdeaths-0.0.2/src/cdcdeaths.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 09:00:17.000000 cdcdeaths-0.0.2/src/cdcdeaths.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       46 2024-04-22 09:00:17.000000 cdcdeaths-0.0.2/src/cdcdeaths.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       10 2024-04-22 09:00:17.000000 cdcdeaths-0.0.2/src/cdcdeaths.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      533 2022-03-15 05:29:30.000000 cdcdeaths-0.0.2/src/cdcdeaths.py
```

### Comparing `cdcdeaths-0.0.1/PKG-INFO` & `cdcdeaths-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: cdcdeaths
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for visualizing the number of deaths by age groups
-Home-page: https://github.com/ytakefuji/cdcdeaths
+Home-page: https://github.com/y-takefuji/cdcdeaths
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/cdcdeaths
+Project-URL: Bug Tracker, https://github.com/y-takefuji/cdcdeaths
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # cdcdeaths
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/a32b3cd5-c35e-417e-a047-75fc0ad20bc3/tree)
+
+DOI: https://doi.org/10.24433/CO.8698120.v1
+
 cdcdeaths is a PyPI package for displaying the number of deaths in the US due to COVID-19 by age groups.
 cdcdeaths can scrape the latest data from cdc.
 result.png file will be generated.
 
 # how to install cdcdeaths
 On WSL on Windows, MacOS, and Linux operating systems, run the following command to install it:
 
@@ -28,11 +32,11 @@
 
 $ pip install cdcdeaths --force-reinstall --no-cache-dir --no-binary :all:
 
 # how to run cdcdeaths
 
 $ cdcdeaths
 
-<img src='https://github.com/ytakefuji/cdcdeaths/raw/main/result.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/cdcdeaths/raw/main/result.png' width=640 height=480>
```

### Comparing `cdcdeaths-0.0.1/README.md` & `cdcdeaths-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # cdcdeaths
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/a32b3cd5-c35e-417e-a047-75fc0ad20bc3/tree)
+
+DOI: https://doi.org/10.24433/CO.8698120.v1
+
 cdcdeaths is a PyPI package for displaying the number of deaths in the US due to COVID-19 by age groups.
 cdcdeaths can scrape the latest data from cdc.
 result.png file will be generated.
 
 # how to install cdcdeaths
 On WSL on Windows, MacOS, and Linux operating systems, run the following command to install it:
 
@@ -12,9 +16,9 @@
 
 $ pip install cdcdeaths --force-reinstall --no-cache-dir --no-binary :all:
 
 # how to run cdcdeaths
 
 $ cdcdeaths
 
-<img src='https://github.com/ytakefuji/cdcdeaths/raw/main/result.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/cdcdeaths/raw/main/result.png' width=640 height=480>
```

### Comparing `cdcdeaths-0.0.1/setup.py` & `cdcdeaths-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cdcdeaths",
-    version="0.0.1",
+    version="0.0.2",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for visualizing the number of deaths by age groups",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/cdcdeaths",
+    url="https://github.com/y-takefuji/cdcdeaths",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/cdcdeaths",
+        "Bug Tracker": "https://github.com/y-takefuji/cdcdeaths",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
```

### Comparing `cdcdeaths-0.0.1/src/cdcdeaths.egg-info/PKG-INFO` & `cdcdeaths-0.0.2/src/cdcdeaths.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: cdcdeaths
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for visualizing the number of deaths by age groups
-Home-page: https://github.com/ytakefuji/cdcdeaths
+Home-page: https://github.com/y-takefuji/cdcdeaths
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/cdcdeaths
+Project-URL: Bug Tracker, https://github.com/y-takefuji/cdcdeaths
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # cdcdeaths
+[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/a32b3cd5-c35e-417e-a047-75fc0ad20bc3/tree)
+
+DOI: https://doi.org/10.24433/CO.8698120.v1
+
 cdcdeaths is a PyPI package for displaying the number of deaths in the US due to COVID-19 by age groups.
 cdcdeaths can scrape the latest data from cdc.
 result.png file will be generated.
 
 # how to install cdcdeaths
 On WSL on Windows, MacOS, and Linux operating systems, run the following command to install it:
 
@@ -28,11 +32,11 @@
 
 $ pip install cdcdeaths --force-reinstall --no-cache-dir --no-binary :all:
 
 # how to run cdcdeaths
 
 $ cdcdeaths
 
-<img src='https://github.com/ytakefuji/cdcdeaths/raw/main/result.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/cdcdeaths/raw/main/result.png' width=640 height=480>
```

### Comparing `cdcdeaths-0.0.1/src/cdcdeaths.py` & `cdcdeaths-0.0.2/src/cdcdeaths.py`

 * *Files identical despite different names*

