# Comparing `tmp/slap2_utils-0.0.5.tar.gz` & `tmp/slap2_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slap2_utils-0.0.5.tar", last modified: Sun Apr 21 23:50:48 2024, max compression
+gzip compressed data, was "slap2_utils-0.0.6.tar", last modified: Mon Apr 22 03:18:05 2024, max compression
```

## Comparing `slap2_utils-0.0.5.tar` & `slap2_utils-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,57 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-21 23:50:48.630770 slap2_utils-0.0.5/
--rw-rw-r--   0 peter     (1000) peter     (1000)    16725 2023-10-19 02:37:53.000000 slap2_utils-0.0.5/LICENSE
--rw-r--r--   0 peter     (1000) peter     (1000)     2770 2024-04-21 23:50:48.630770 slap2_utils-0.0.5/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     2118 2024-04-21 18:20:08.000000 slap2_utils-0.0.5/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-21 23:50:48.630770 slap2_utils-0.0.5/SLAP2_UTILS.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     2770 2024-04-21 23:50:48.000000 slap2_utils-0.0.5/SLAP2_UTILS.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     1170 2024-04-21 23:50:48.000000 slap2_utils-0.0.5/SLAP2_UTILS.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2024-04-21 23:50:48.000000 slap2_utils-0.0.5/SLAP2_UTILS.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       12 2024-04-21 23:50:48.000000 slap2_utils-0.0.5/SLAP2_UTILS.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)      580 2024-04-21 19:25:26.000000 slap2_utils-0.0.5/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       79 2024-04-21 23:50:48.630770 slap2_utils-0.0.5/setup.cfg
--rw-rw-r--   0 peter     (1000) peter     (1000)     1013 2024-04-21 19:33:41.000000 slap2_utils-0.0.5/setup.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-21 23:50:48.630770 slap2_utils-0.0.5/slap2_utils/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2023-10-19 03:25:21.000000 slap2_utils-0.0.5/slap2_utils/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6004 2024-02-05 17:47:20.000000 slap2_utils-0.0.5/slap2_utils/datafile.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-21 23:50:48.630770 slap2_utils-0.0.5/slap2_utils/dataviewer/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2023-11-03 16:30:49.000000 slap2_utils-0.0.5/slap2_utils/dataviewer/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6721 2024-02-20 15:10:00.000000 slap2_utils-0.0.5/slap2_utils/dataviewer/dataviewer.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-21 23:50:48.630770 slap2_utils-0.0.5/slap2_utils/experiments/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2024-01-10 19:34:18.000000 slap2_utils-0.0.5/slap2_utils/experiments/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1888 2024-02-04 17:57:18.000000 slap2_utils-0.0.5/slap2_utils/experiments/somaROI.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2298 2024-02-04 17:57:18.000000 slap2_utils-0.0.5/slap2_utils/experiments/somaROIsys.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-21 23:50:48.630770 slap2_utils-0.0.5/slap2_utils/filters/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2023-11-09 20:51:56.000000 slap2_utils-0.0.5/slap2_utils/filters/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4189 2023-11-09 20:56:02.000000 slap2_utils-0.0.5/slap2_utils/filters/filters.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-21 23:50:48.630770 slap2_utils-0.0.5/slap2_utils/functions/
--rw-rw-r--   0 peter     (1000) peter     (1000)      930 2021-07-23 20:30:15.000000 slap2_utils-0.0.5/slap2_utils/functions/DouglasPeucker.py
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2023-10-25 19:07:27.000000 slap2_utils-0.0.5/slap2_utils/functions/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    13597 2024-03-14 04:37:55.000000 slap2_utils-0.0.5/slap2_utils/functions/_masked_phase_cross_correlation.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    18096 2024-03-15 17:47:01.000000 slap2_utils-0.0.5/slap2_utils/functions/_phase_cross_correlation.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7811 2024-03-27 18:19:11.000000 slap2_utils-0.0.5/slap2_utils/functions/autoROI.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2480 2024-02-21 05:06:10.000000 slap2_utils-0.0.5/slap2_utils/functions/imagestacks.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    16769 2024-02-04 17:57:18.000000 slap2_utils-0.0.5/slap2_utils/functions/otsuROI.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      586 2023-11-30 00:32:56.000000 slap2_utils-0.0.5/slap2_utils/functions/stim.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2577 2024-01-29 17:00:38.000000 slap2_utils-0.0.5/slap2_utils/functions/tracefunctions.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    16990 2024-02-04 17:57:18.000000 slap2_utils-0.0.5/slap2_utils/functions/unetROI.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      775 2024-03-14 15:57:28.000000 slap2_utils-0.0.5/slap2_utils/functions/xyzshift.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1695 2024-03-27 18:22:33.000000 slap2_utils-0.0.5/slap2_utils/functions/xyzshift_ui.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-21 23:50:48.630770 slap2_utils-0.0.5/slap2_utils/segmentation/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2023-11-27 18:06:36.000000 slap2_utils-0.0.5/slap2_utils/segmentation/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      341 2023-11-27 18:07:54.000000 slap2_utils-0.0.5/slap2_utils/segmentation/segmentation.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2024-04-21 23:50:48.630770 slap2_utils-0.0.5/slap2_utils/subclasses/
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2023-10-19 03:48:33.000000 slap2_utils-0.0.5/slap2_utils/subclasses/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2058 2024-01-26 18:30:05.000000 slap2_utils-0.0.5/slap2_utils/subclasses/acquisitionContainer.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1386 2024-01-24 16:18:33.000000 slap2_utils-0.0.5/slap2_utils/subclasses/metadata.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      811 2023-11-02 02:43:17.000000 slap2_utils-0.0.5/slap2_utils/subclasses/slapROI.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:05.161986 slap2_utils-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-22 03:18:05.161986 slap2_utils-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:05.161986 slap2_utils-0.0.6/SLAP2_UTILS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-22 03:18:05.000000 slap2_utils-0.0.6/SLAP2_UTILS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-22 03:18:05.000000 slap2_utils-0.0.6/SLAP2_UTILS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 03:18:05.000000 slap2_utils-0.0.6/SLAP2_UTILS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-22 03:18:05.000000 slap2_utils-0.0.6/SLAP2_UTILS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 03:18:05.000000 slap2_utils-0.0.6/SLAP2_UTILS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 03:18:05.161986 slap2_utils-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:05.153986 slap2_utils-0.0.6/slap2_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/datafile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:05.153986 slap2_utils-0.0.6/slap2_utils/dataviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/dataviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/dataviewer/dataviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:05.153986 slap2_utils-0.0.6/slap2_utils/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/experiments/somaROI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/experiments/somaROIsys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:05.153986 slap2_utils-0.0.6/slap2_utils/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:05.157986 slap2_utils-0.0.6/slap2_utils/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/functions/DouglasPeucker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/functions/_masked_phase_cross_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18096 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/functions/_phase_cross_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/functions/autoROI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-22 03:17:59.000000 slap2_utils-0.0.6/slap2_utils/functions/imagestacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16769 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/functions/otsuROI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/functions/stim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/functions/tracefunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16990 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/functions/unetROI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/functions/xyzshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/functions/xyzshift_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:05.157986 slap2_utils-0.0.6/slap2_utils/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/segmentation/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:05.157986 slap2_utils-0.0.6/slap2_utils/subclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/subclasses/acquisitionContainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/subclasses/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/subclasses/slapROI.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:05.157986 slap2_utils-0.0.6/slap2_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/utils/file_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/utils/file_header_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/utils/roi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/utils/trace_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-22 03:18:01.000000 slap2_utils-0.0.6/slap2_utils/utils/trace_pixel.py
```

### Comparing `slap2_utils-0.0.5/LICENSE` & `slap2_utils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/PKG-INFO` & `slap2_utils-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: SLAP2_UTILS
-Version: 0.0.5
+Version: 0.0.6
 Summary: Code to support using a SLAP2 Microscope
 Home-page: https://github.com/Peter-Hogg/SLAP2_Utils
 Author: Peter Hogg
 Author-email: Peter Hogg <peter.hogg@ubc.ca>, Jerry Tong <jerrytong0810@gmail.com>
 Project-URL: Homepage, https://github.com/Peter-Hogg/SLAP2_Utils
 Project-URL: Issues, https://github.com/Peter-Hogg/SLAP2_Utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: h5py
+Requires-Dist: scikit-image
+Requires-Dist: cupy
 
 # SLAP2_Utils
 
 ## Overview
 The `SLAP2_Utils` library is designed to facilitate the reading of SLAP2 (Scanned Line Projection Microscopy version 2) binary files using Python. This utility aims to support researchers and developers working with data from SLAP2 two-photon microscopes by providing an interface to directly manipulate and analyze these files in Python as an alternative a Matlab based workflow. The SLAP2 microscope is a commerically avaliable kit from MBF bioscience (https://www.mbfbioscience.com/products/slap2).
 
 ## Features
@@ -32,14 +37,20 @@
 - NumPy
 - SciPy
 - h5py
 - scikit-image
 - cupy
 
 ## Installation
+Install with pip
+```bash
+pip install SLAP2-UTILS
+```
+
+
 Clone this repository
 
 ```bash
 git clone https://github.com/Peter-Hogg/SLAP2_Utils.git
 ```
 ## Contributing
```

### Comparing `slap2_utils-0.0.5/README.md` & `slap2_utils-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 - NumPy
 - SciPy
 - h5py
 - scikit-image
 - cupy
 
 ## Installation
+Install with pip
+```bash
+pip install SLAP2-UTILS
+```
+
+
 Clone this repository
 
 ```bash
 git clone https://github.com/Peter-Hogg/SLAP2_Utils.git
 ```
 ## Contributing
```

### Comparing `slap2_utils-0.0.5/SLAP2_UTILS.egg-info/PKG-INFO` & `slap2_utils-0.0.6/SLAP2_UTILS.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: SLAP2_UTILS
-Version: 0.0.5
+Version: 0.0.6
 Summary: Code to support using a SLAP2 Microscope
 Home-page: https://github.com/Peter-Hogg/SLAP2_Utils
 Author: Peter Hogg
 Author-email: Peter Hogg <peter.hogg@ubc.ca>, Jerry Tong <jerrytong0810@gmail.com>
 Project-URL: Homepage, https://github.com/Peter-Hogg/SLAP2_Utils
 Project-URL: Issues, https://github.com/Peter-Hogg/SLAP2_Utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: h5py
+Requires-Dist: scikit-image
+Requires-Dist: cupy
 
 # SLAP2_Utils
 
 ## Overview
 The `SLAP2_Utils` library is designed to facilitate the reading of SLAP2 (Scanned Line Projection Microscopy version 2) binary files using Python. This utility aims to support researchers and developers working with data from SLAP2 two-photon microscopes by providing an interface to directly manipulate and analyze these files in Python as an alternative a Matlab based workflow. The SLAP2 microscope is a commerically avaliable kit from MBF bioscience (https://www.mbfbioscience.com/products/slap2).
 
 ## Features
@@ -32,14 +37,20 @@
 - NumPy
 - SciPy
 - h5py
 - scikit-image
 - cupy
 
 ## Installation
+Install with pip
+```bash
+pip install SLAP2-UTILS
+```
+
+
 Clone this repository
 
 ```bash
 git clone https://github.com/Peter-Hogg/SLAP2_Utils.git
 ```
 ## Contributing
```

### Comparing `slap2_utils-0.0.5/SLAP2_UTILS.egg-info/SOURCES.txt` & `slap2_utils-0.0.6/SLAP2_UTILS.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
 SLAP2_UTILS.egg-info/PKG-INFO
 SLAP2_UTILS.egg-info/SOURCES.txt
 SLAP2_UTILS.egg-info/dependency_links.txt
+SLAP2_UTILS.egg-info/requires.txt
 SLAP2_UTILS.egg-info/top_level.txt
 slap2_utils/__init__.py
 slap2_utils/datafile.py
 slap2_utils/dataviewer/__init__.py
 slap2_utils/dataviewer/dataviewer.py
 slap2_utils/experiments/__init__.py
 slap2_utils/experiments/somaROI.py
@@ -29,8 +32,15 @@
 slap2_utils/functions/xyzshift.py
 slap2_utils/functions/xyzshift_ui.py
 slap2_utils/segmentation/__init__.py
 slap2_utils/segmentation/segmentation.py
 slap2_utils/subclasses/__init__.py
 slap2_utils/subclasses/acquisitionContainer.py
 slap2_utils/subclasses/metadata.py
-slap2_utils/subclasses/slapROI.py
+slap2_utils/subclasses/slapROI.py
+slap2_utils/utils/__init__.py
+slap2_utils/utils/file_header.py
+slap2_utils/utils/file_header_v1.py
+slap2_utils/utils/roi_utils.py
+slap2_utils/utils/trace.py
+slap2_utils/utils/trace_average.py
+slap2_utils/utils/trace_pixel.py
```

### Comparing `slap2_utils-0.0.5/setup.py` & `slap2_utils-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
-with open('requirements.txt', 'r') as f:
+with open(path.join(here, 'requirements.txt'), 'r') as f:
     required = f.read().splitlines()
 
 
 
 setup(
 
-    name='slap2utils', 
-    version='0.0.3',  
+    name='slap2_utils', 
+    version='0.0.6',  
 
     
     description='Code to support using a SLAP2 Microscope',  
 
     url='https://github.com/Peter-Hogg/SLAP2_Utils',  
 
     
@@ -46,8 +46,8 @@
     
     packages=find_packages(exclude=['*.test']), 
 
 
     install_requires=required,  
 
 
-)
+)
```

### Comparing `slap2_utils-0.0.5/slap2_utils/datafile.py` & `slap2_utils-0.0.6/slap2_utils/datafile.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/dataviewer/dataviewer.py` & `slap2_utils-0.0.6/slap2_utils/dataviewer/dataviewer.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/experiments/somaROI.py` & `slap2_utils-0.0.6/slap2_utils/experiments/somaROI.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/experiments/somaROIsys.py` & `slap2_utils-0.0.6/slap2_utils/experiments/somaROIsys.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/filters/filters.py` & `slap2_utils-0.0.6/slap2_utils/filters/filters.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/functions/DouglasPeucker.py` & `slap2_utils-0.0.6/slap2_utils/functions/DouglasPeucker.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/functions/_masked_phase_cross_correlation.py` & `slap2_utils-0.0.6/slap2_utils/functions/_masked_phase_cross_correlation.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/functions/_phase_cross_correlation.py` & `slap2_utils-0.0.6/slap2_utils/functions/_phase_cross_correlation.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/functions/autoROI.py` & `slap2_utils-0.0.6/slap2_utils/functions/autoROI.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/functions/imagestacks.py` & `slap2_utils-0.0.6/slap2_utils/functions/imagestacks.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/functions/otsuROI.py` & `slap2_utils-0.0.6/slap2_utils/functions/otsuROI.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/functions/stim.py` & `slap2_utils-0.0.6/slap2_utils/functions/stim.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/functions/tracefunctions.py` & `slap2_utils-0.0.6/slap2_utils/functions/tracefunctions.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/functions/unetROI.py` & `slap2_utils-0.0.6/slap2_utils/functions/unetROI.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/functions/xyzshift.py` & `slap2_utils-0.0.6/slap2_utils/functions/xyzshift.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/functions/xyzshift_ui.py` & `slap2_utils-0.0.6/slap2_utils/functions/xyzshift_ui.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/subclasses/acquisitionContainer.py` & `slap2_utils-0.0.6/slap2_utils/subclasses/acquisitionContainer.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/subclasses/metadata.py` & `slap2_utils-0.0.6/slap2_utils/subclasses/metadata.py`

 * *Files identical despite different names*

### Comparing `slap2_utils-0.0.5/slap2_utils/subclasses/slapROI.py` & `slap2_utils-0.0.6/slap2_utils/subclasses/slapROI.py`

 * *Files identical despite different names*

