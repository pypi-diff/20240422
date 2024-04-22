# Comparing `tmp/BDMLtools-0.4.2.tar.gz` & `tmp/BDMLtools-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDMLtools-0.4.2.tar", last modified: Fri Mar 29 07:38:08 2024, max compression
+gzip compressed data, was "BDMLtools-0.4.3.tar", last modified: Mon Apr 22 07:19:00 2024, max compression
```

## Comparing `BDMLtools-0.4.2.tar` & `BDMLtools-0.4.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-03-29 07:38:08.946517 BDMLtools-0.4.2/
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-03-29 07:38:08.920940 BDMLtools-0.4.2/BDMLtools/
--rwxr-xr-x   0 zengke     (501) staff       (20)     1546 2024-03-28 08:32:26.000000 BDMLtools-0.4.2/BDMLtools/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     7976 2024-02-29 06:22:45.000000 BDMLtools-0.4.2/BDMLtools/base.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-03-29 07:38:08.925170 BDMLtools-0.4.2/BDMLtools/clearner/
--rw-r--r--   0 zengke     (501) staff       (20)      303 2022-05-30 05:46:05.000000 BDMLtools-0.4.2/BDMLtools/clearner/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)    21515 2024-02-27 09:59:11.000000 BDMLtools-0.4.2/BDMLtools/clearner/cleaner.py
--rw-r--r--   0 zengke     (501) staff       (20)      798 2024-02-29 06:24:49.000000 BDMLtools-0.4.2/BDMLtools/config.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-03-29 07:38:08.926667 BDMLtools-0.4.2/BDMLtools/encoder/
--rw-r--r--   0 zengke     (501) staff       (20)      230 2022-09-09 08:32:26.000000 BDMLtools-0.4.2/BDMLtools/encoder/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    13143 2023-10-11 03:12:00.000000 BDMLtools-0.4.2/BDMLtools/encoder/woe.py
--rw-r--r--   0 zengke     (501) staff       (20)      617 2022-05-30 05:46:05.000000 BDMLtools-0.4.2/BDMLtools/exception.py
--rwxr-xr-x   0 zengke     (501) staff       (20)     5965 2022-07-22 07:30:31.000000 BDMLtools-0.4.2/BDMLtools/fun.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-03-29 07:38:08.928646 BDMLtools-0.4.2/BDMLtools/plotter/
--rw-r--r--   0 zengke     (501) staff       (20)      280 2022-07-08 09:08:07.000000 BDMLtools-0.4.2/BDMLtools/plotter/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)    34798 2024-02-28 08:29:18.000000 BDMLtools-0.4.2/BDMLtools/plotter/base.py
--rw-r--r--   0 zengke     (501) staff       (20)    17121 2024-02-28 08:25:09.000000 BDMLtools-0.4.2/BDMLtools/plotter/eval.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-03-29 07:38:08.929825 BDMLtools-0.4.2/BDMLtools/report/
--rw-r--r--   0 zengke     (501) staff       (20)      379 2022-05-30 05:46:05.000000 BDMLtools-0.4.2/BDMLtools/report/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    51860 2024-02-27 09:56:35.000000 BDMLtools-0.4.2/BDMLtools/report/report.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-03-29 07:38:08.934470 BDMLtools-0.4.2/BDMLtools/selector/
--rw-r--r--   0 zengke     (501) staff       (20)      902 2022-11-22 04:09:12.000000 BDMLtools-0.4.2/BDMLtools/selector/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    30545 2024-03-29 02:50:52.000000 BDMLtools-0.4.2/BDMLtools/selector/bin.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    61666 2024-02-28 05:59:28.000000 BDMLtools-0.4.2/BDMLtools/selector/bin_fun.py
--rw-r--r--   0 zengke     (501) staff       (20)    12002 2024-03-29 06:56:50.000000 BDMLtools-0.4.2/BDMLtools/selector/embeded.py
--rw-r--r--   0 zengke     (501) staff       (20)    16466 2023-10-11 02:30:44.000000 BDMLtools-0.4.2/BDMLtools/selector/fa.py
--rw-r--r--   0 zengke     (501) staff       (20)    24815 2024-03-28 08:26:36.000000 BDMLtools-0.4.2/BDMLtools/selector/lgbm.py
--rw-r--r--   0 zengke     (501) staff       (20)    27646 2023-10-12 10:01:30.000000 BDMLtools-0.4.2/BDMLtools/selector/logtit.py
--rw-r--r--   0 zengke     (501) staff       (20)    30324 2023-10-11 02:31:45.000000 BDMLtools-0.4.2/BDMLtools/selector/simple.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-03-29 07:38:08.937922 BDMLtools-0.4.2/BDMLtools/tuner/
--rw-r--r--   0 zengke     (501) staff       (20)      438 2023-05-23 09:53:29.000000 BDMLtools-0.4.2/BDMLtools/tuner/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     5738 2023-08-08 06:18:50.000000 BDMLtools-0.4.2/BDMLtools/tuner/base.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    35296 2024-03-28 08:27:45.000000 BDMLtools-0.4.2/BDMLtools/tuner/bayesian.py
--rwxr-xr-x   0 zengke     (501) staff       (20)     5848 2024-02-29 06:25:31.000000 BDMLtools-0.4.2/BDMLtools/tuner/fun.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    47294 2023-11-21 07:51:14.000000 BDMLtools-0.4.2/BDMLtools/tuner/gridcv.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    26408 2023-11-20 10:06:25.000000 BDMLtools-0.4.2/BDMLtools/tuner/halvingcv.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-03-29 07:38:08.924007 BDMLtools-0.4.2/BDMLtools.egg-info/
--rw-r--r--   0 zengke     (501) staff       (20)     3224 2024-03-29 07:38:08.000000 BDMLtools-0.4.2/BDMLtools.egg-info/PKG-INFO
--rw-r--r--   0 zengke     (501) staff       (20)     1066 2024-03-29 07:38:08.000000 BDMLtools-0.4.2/BDMLtools.egg-info/SOURCES.txt
--rw-r--r--   0 zengke     (501) staff       (20)        1 2024-03-29 07:38:08.000000 BDMLtools-0.4.2/BDMLtools.egg-info/dependency_links.txt
--rw-r--r--   0 zengke     (501) staff       (20)      503 2024-03-29 07:38:08.000000 BDMLtools-0.4.2/BDMLtools.egg-info/requires.txt
--rw-r--r--   0 zengke     (501) staff       (20)       15 2024-03-29 07:38:08.000000 BDMLtools-0.4.2/BDMLtools.egg-info/top_level.txt
--rw-r--r--   0 zengke     (501) staff       (20)     1062 2022-09-07 02:01:45.000000 BDMLtools-0.4.2/LICENSE
--rw-r--r--   0 zengke     (501) staff       (20)     3224 2024-03-29 07:38:08.945621 BDMLtools-0.4.2/PKG-INFO
--rw-r--r--   0 zengke     (501) staff       (20)     1363 2024-03-29 07:27:05.000000 BDMLtools-0.4.2/README.md
--rw-r--r--   0 zengke     (501) staff       (20)       38 2024-03-29 07:38:08.946682 BDMLtools-0.4.2/setup.cfg
--rwxr-xr-x   0 zengke     (501) staff       (20)     4747 2024-03-28 08:40:53.000000 BDMLtools-0.4.2/setup.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-03-29 07:38:08.941761 BDMLtools-0.4.2/test/
--rwxr-xr-x   0 zengke     (501) staff       (20)        0 2022-07-12 06:58:12.000000 BDMLtools-0.4.2/test/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     9172 2024-02-29 06:22:13.000000 BDMLtools-0.4.2/test/test_base.py
--rw-r--r--   0 zengke     (501) staff       (20)     4500 2022-09-06 10:08:22.000000 BDMLtools-0.4.2/test/test_clearner.py
--rw-r--r--   0 zengke     (501) staff       (20)     2068 2024-02-28 08:22:18.000000 BDMLtools-0.4.2/test/test_eval.py
--rw-r--r--   0 zengke     (501) staff       (20)     4899 2023-08-07 08:07:53.000000 BDMLtools-0.4.2/test/test_report.py
--rw-r--r--   0 zengke     (501) staff       (20)    18957 2024-02-27 08:52:55.000000 BDMLtools-0.4.2/test/test_selector.py
--rw-r--r--   0 zengke     (501) staff       (20)    26185 2024-02-29 03:02:46.000000 BDMLtools-0.4.2/test/test_tunner.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-04-22 07:19:00.246847 BDMLtools-0.4.3/
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-04-22 07:19:00.208346 BDMLtools-0.4.3/BDMLtools/
+-rwxr-xr-x   0 zengke     (501) staff       (20)     1546 2024-04-19 07:50:41.000000 BDMLtools-0.4.3/BDMLtools/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     7976 2024-02-29 06:22:45.000000 BDMLtools-0.4.3/BDMLtools/base.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-04-22 07:19:00.210908 BDMLtools-0.4.3/BDMLtools/clearner/
+-rw-r--r--   0 zengke     (501) staff       (20)      303 2022-05-30 05:46:05.000000 BDMLtools-0.4.3/BDMLtools/clearner/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)    21515 2024-02-27 09:59:11.000000 BDMLtools-0.4.3/BDMLtools/clearner/cleaner.py
+-rw-r--r--   0 zengke     (501) staff       (20)      798 2024-02-29 06:24:49.000000 BDMLtools-0.4.3/BDMLtools/config.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-04-22 07:19:00.212606 BDMLtools-0.4.3/BDMLtools/encoder/
+-rw-r--r--   0 zengke     (501) staff       (20)      230 2022-09-09 08:32:26.000000 BDMLtools-0.4.3/BDMLtools/encoder/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    13143 2023-10-11 03:12:00.000000 BDMLtools-0.4.3/BDMLtools/encoder/woe.py
+-rw-r--r--   0 zengke     (501) staff       (20)      617 2022-05-30 05:46:05.000000 BDMLtools-0.4.3/BDMLtools/exception.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)     5965 2022-07-22 07:30:31.000000 BDMLtools-0.4.3/BDMLtools/fun.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-04-22 07:19:00.215357 BDMLtools-0.4.3/BDMLtools/plotter/
+-rw-r--r--   0 zengke     (501) staff       (20)      280 2022-07-08 09:08:07.000000 BDMLtools-0.4.3/BDMLtools/plotter/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)    34798 2024-02-28 08:29:18.000000 BDMLtools-0.4.3/BDMLtools/plotter/base.py
+-rw-r--r--   0 zengke     (501) staff       (20)    17121 2024-02-28 08:25:09.000000 BDMLtools-0.4.3/BDMLtools/plotter/eval.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-04-22 07:19:00.217019 BDMLtools-0.4.3/BDMLtools/report/
+-rw-r--r--   0 zengke     (501) staff       (20)      379 2022-05-30 05:46:05.000000 BDMLtools-0.4.3/BDMLtools/report/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    51860 2024-02-27 09:56:35.000000 BDMLtools-0.4.3/BDMLtools/report/report.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-04-22 07:19:00.225130 BDMLtools-0.4.3/BDMLtools/selector/
+-rw-r--r--   0 zengke     (501) staff       (20)      902 2022-11-22 04:09:12.000000 BDMLtools-0.4.3/BDMLtools/selector/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    30562 2024-04-19 07:08:16.000000 BDMLtools-0.4.3/BDMLtools/selector/bin.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    62038 2024-04-19 07:01:03.000000 BDMLtools-0.4.3/BDMLtools/selector/bin_fun.py
+-rw-r--r--   0 zengke     (501) staff       (20)    12170 2024-04-19 01:54:36.000000 BDMLtools-0.4.3/BDMLtools/selector/embeded.py
+-rw-r--r--   0 zengke     (501) staff       (20)    16466 2023-10-11 02:30:44.000000 BDMLtools-0.4.3/BDMLtools/selector/fa.py
+-rw-r--r--   0 zengke     (501) staff       (20)    24815 2024-04-09 10:08:45.000000 BDMLtools-0.4.3/BDMLtools/selector/lgbm.py
+-rw-r--r--   0 zengke     (501) staff       (20)    27646 2023-10-12 10:01:30.000000 BDMLtools-0.4.3/BDMLtools/selector/logtit.py
+-rw-r--r--   0 zengke     (501) staff       (20)    32595 2024-04-19 09:55:48.000000 BDMLtools-0.4.3/BDMLtools/selector/simple.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-04-22 07:19:00.232968 BDMLtools-0.4.3/BDMLtools/tuner/
+-rw-r--r--   0 zengke     (501) staff       (20)      438 2023-05-23 09:53:29.000000 BDMLtools-0.4.3/BDMLtools/tuner/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     5738 2023-08-08 06:18:50.000000 BDMLtools-0.4.3/BDMLtools/tuner/base.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    35296 2024-03-28 08:27:45.000000 BDMLtools-0.4.3/BDMLtools/tuner/bayesian.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)     5848 2024-02-29 06:25:31.000000 BDMLtools-0.4.3/BDMLtools/tuner/fun.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    47294 2023-11-21 07:51:14.000000 BDMLtools-0.4.3/BDMLtools/tuner/gridcv.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    26408 2023-11-20 10:06:25.000000 BDMLtools-0.4.3/BDMLtools/tuner/halvingcv.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-04-22 07:19:00.210085 BDMLtools-0.4.3/BDMLtools.egg-info/
+-rw-r--r--   0 zengke     (501) staff       (20)     3516 2024-04-22 07:19:00.000000 BDMLtools-0.4.3/BDMLtools.egg-info/PKG-INFO
+-rw-r--r--   0 zengke     (501) staff       (20)     1066 2024-04-22 07:19:00.000000 BDMLtools-0.4.3/BDMLtools.egg-info/SOURCES.txt
+-rw-r--r--   0 zengke     (501) staff       (20)        1 2024-04-22 07:19:00.000000 BDMLtools-0.4.3/BDMLtools.egg-info/dependency_links.txt
+-rw-r--r--   0 zengke     (501) staff       (20)      503 2024-04-22 07:19:00.000000 BDMLtools-0.4.3/BDMLtools.egg-info/requires.txt
+-rw-r--r--   0 zengke     (501) staff       (20)       15 2024-04-22 07:19:00.000000 BDMLtools-0.4.3/BDMLtools.egg-info/top_level.txt
+-rw-r--r--   0 zengke     (501) staff       (20)     1062 2022-09-07 02:01:45.000000 BDMLtools-0.4.3/LICENSE
+-rw-r--r--   0 zengke     (501) staff       (20)     3516 2024-04-22 07:19:00.246075 BDMLtools-0.4.3/PKG-INFO
+-rw-r--r--   0 zengke     (501) staff       (20)     1655 2024-04-22 06:58:18.000000 BDMLtools-0.4.3/README.md
+-rw-r--r--   0 zengke     (501) staff       (20)       38 2024-04-22 07:19:00.247273 BDMLtools-0.4.3/setup.cfg
+-rwxr-xr-x   0 zengke     (501) staff       (20)     4798 2024-04-22 06:50:08.000000 BDMLtools-0.4.3/setup.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2024-04-22 07:19:00.240959 BDMLtools-0.4.3/test/
+-rwxr-xr-x   0 zengke     (501) staff       (20)        0 2022-07-12 06:58:12.000000 BDMLtools-0.4.3/test/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     9172 2024-02-29 06:22:13.000000 BDMLtools-0.4.3/test/test_base.py
+-rw-r--r--   0 zengke     (501) staff       (20)     4500 2022-09-06 10:08:22.000000 BDMLtools-0.4.3/test/test_clearner.py
+-rw-r--r--   0 zengke     (501) staff       (20)     2068 2024-02-28 08:22:18.000000 BDMLtools-0.4.3/test/test_eval.py
+-rw-r--r--   0 zengke     (501) staff       (20)     4899 2023-08-07 08:07:53.000000 BDMLtools-0.4.3/test/test_report.py
+-rw-r--r--   0 zengke     (501) staff       (20)    19102 2024-04-22 02:56:09.000000 BDMLtools-0.4.3/test/test_selector.py
+-rw-r--r--   0 zengke     (501) staff       (20)    26185 2024-02-29 03:02:46.000000 BDMLtools-0.4.3/test/test_tunner.py
```

### Comparing `BDMLtools-0.4.2/BDMLtools/__init__.py` & `BDMLtools-0.4.3/BDMLtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from BDMLtools.plotter import BaseWoePlotter
 from BDMLtools.plotter import perfEval,perfEval2
 from BDMLtools.encoder import woeTransformer,binTransformer
 from BDMLtools.tuner import gridTuner,hgridTuner,FLgridTuner
 from BDMLtools.tuner import BayesianCVTuner,FLBSTuner,shapCheck
 
 
-__version__ = '0.4.2'
+__version__ = '0.4.3'
 
 __all__ = (    
     dtStandardization,
     outliersTransformer,
     dtypeAllocator,
     nanTransformer,
     FLBSTuner,
```

### Comparing `BDMLtools-0.4.2/BDMLtools/base.py` & `BDMLtools-0.4.3/BDMLtools/base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/clearner/cleaner.py` & `BDMLtools-0.4.3/BDMLtools/clearner/cleaner.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/config.py` & `BDMLtools-0.4.3/BDMLtools/config.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/encoder/woe.py` & `BDMLtools-0.4.3/BDMLtools/encoder/woe.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/exception.py` & `BDMLtools-0.4.3/BDMLtools/exception.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/fun.py` & `BDMLtools-0.4.3/BDMLtools/fun.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/plotter/base.py` & `BDMLtools-0.4.3/BDMLtools/plotter/base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/plotter/eval.py` & `BDMLtools-0.4.3/BDMLtools/plotter/eval.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/report/report.py` & `BDMLtools-0.4.3/BDMLtools/report/report.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/selector/__init__.py` & `BDMLtools-0.4.3/BDMLtools/selector/__init__.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/selector/bin.py` & `BDMLtools-0.4.3/BDMLtools/selector/bin.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             + 'tree':决策树,递归分裂iv/ks增益最高的切分点形成新分箱直到达到终止条件
             + 'chi2':卡方,先等频预分箱,再递归合并低于卡方值(交叉表卡方检验的差异不显著)的分箱
         max_bin:int,预分箱数,越多的预分箱数越有可能得到越好的分箱点，但会增加计算量,不适用于method=‘freq’
             + method=‘pretty’时代表pretty预分箱数 
             + method=‘freq-kmeans’时代表freq预分箱数               
             + method='tree'时,代表pretty预分箱数        
             + method='chi2'时,代表pretty预分箱数        
-        distr_limit,最终箱样本占比限制,不适用于method=‘freq’
+        distr_limit,最终箱样本占比限制,不适用于method=‘freq’ or 'freq-kmeans'
             + method='pretty'时，箱最终箱样本占比限制,
             + method='freq-kmeans'时，箱最终箱样本占比限制
             + method='tree'时,箱最终箱样本占比限制
             + method='chi2':时,箱最终箱样本占比限制
         bin_num_limit,
             + method=‘freq’时代表等频分箱数
             + method='freq-kmeans'时，合并分箱最低限制,bin_num_limit<max_bin时才有效果
```

### Comparing `BDMLtools-0.4.2/BDMLtools/selector/bin_fun.py` & `BDMLtools-0.4.3/BDMLtools/selector/bin_fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -856,18 +856,23 @@
                     # g=count_g-b
     
                     # interim=pd.DataFrame({'count':count,'y':y}).groupby(col_group).sum()
                     # count_g=interim['count'].ravel()
                     # b=interim['y'].ravel()
                     # g=count_g-b
         
-                    #if no good or bad sample in cut of the point,then pass the iteration 
-                    if 0 in b.tolist() or 0 in g.tolist():
+                    # #if no nan in col and no good or bad sample in cut of the point,then pass the iteration 
+                    if (0 in b.tolist() or 0 in g.tolist()) and (not nan_sum):
+                                                   
+                        cuts_remain=cuts_remain[cuts_remain!=point]  
+        
+                    # #if nan in col and no good or bad sample in cut of the non nan point,then pass the iteration 
+                    elif (0 in b[:-1].tolist() or 0 in g[:-1].tolist()) and (nan_sum):
                         
-                        cuts_remain=cuts_remain[cuts_remain!=point]    
+                        cuts_remain=cuts_remain[cuts_remain!=point]  
                     
                     #if cuts_tree with current point shows no monotonic trend,then pass the iteration(no nans in col) 
                     elif coerce_monotonic and (not is_str_dtype) and (not is_monotonic(bad_prob)) and (not nan_sum):                    
 
                         cuts_remain=cuts_remain[cuts_remain!=point]
                 
                     #if cuts_tree with current point shows no monotonic trend,then pass the iteration(nans in col)
```

### Comparing `BDMLtools-0.4.2/BDMLtools/selector/embeded.py` & `BDMLtools-0.4.3/BDMLtools/selector/embeded.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         '''
         最优参数下的模型的预测
         Parameters:
         --
         X:pd.DataFrame对象
         '''      
         self._check_is_fitted()
-        pred = self.model_refit.predict_proba(np.array(X))[:,1]        
+        pred = self.model_refit.predict_proba(X)[:,1]        
         return pred
 
     
     def transform(self,X,y=None): 
         
         self._check_is_fitted()
         self._check_X(X)
@@ -105,15 +105,15 @@
         --
         X:pd.DataFrame对象
         y:目标变量,pd.Series对象
         '''   
         self._check_data(X,y)
         self._check_ws(y,sample_weight)
         
-        self.feature_names_=X.columns.tolist()
+        self.feature_names_=X.columns.tolist()       
         
         X=np.array(X)
         y=np.array(y)
         
         if sample_weight is not None:
         
             sample_weight=np.array(sample_weight)
@@ -122,21 +122,23 @@
         if self.standard:
             
             X=StandardScaler().fit_transform(X)
         
         out_mods_,cv_path_,cv_res_=self._logit_cv(X,y,sample_weight)
         max_s,max_s_se=cv_res_[cv_res_['valscore_avg']==cv_res_['valscore_avg'].max()].to_numpy()[0][[2,4]]
         
+        cv_path_.columns=['log(C)']+self.feature_names_+['coef_cnt']  
+        
         self.plot_path=self._plot_path(cv_path_,figure_size)
         self.plot_valscore=self._plot_valscore(cv_res_,figure_size)
         
         self.c_best=cv_res_[cv_res_['valscore_avg']==cv_res_['valscore_avg'].max()]['C'].ravel()[0]
         self.c_1se=cv_res_[(cv_res_['valscore_avg']<=max_s) & \
                            (cv_res_['valscore_avg']>=max_s-max_s_se)].sort_values('log(C)').iloc[0,0]
-            
+        
         self.cv_path_=cv_path_
         self.cv_res_=cv_res_
         self.out_mods_=out_mods_
             
         self._is_fitted=True
         
         if self.method=='best':    
@@ -173,15 +175,15 @@
                         for c in cs),dtype=object)
         
         cs_cv=out_list[:,0]
         val_score_cv=out_list[:,1]
         
         cv_path_=pd.DataFrame(out_mods_[:,0:2],columns=['C','log(C)'],dtype='float64').join(
             pd.Series(out_mods_[:,2]).apply(pd.Series)).join(
-            pd.Series(out_mods_[:,2],name='coef_cnt').apply(lambda x:sum(x!=0))).set_index('C')
+            pd.Series(out_mods_[:,2],name='coef_cnt').apply(lambda x:sum(x!=0))).set_index('C')                              
 
         cv_res_=pd.DataFrame([(
           c,np.log10(c),
           np.mean(np.array(val_score_cv)[np.array(cs_cv)==c]),
           np.std(np.array(val_score_cv)[np.array(cs_cv)==c]),
           np.std(np.array(val_score_cv)[np.array(cs_cv)==c])/np.sqrt(n-1)) for c in sorted(np.unique(cs_cv))
             ],columns=['C','log(C)','valscore_avg','valscore_std','valscore_err']).set_index('C',drop=False).join(cv_path_['coef_cnt'])
@@ -234,14 +236,16 @@
             tol=1e-6,
             max_iter=int(1e6),
             random_state=self.random_state,
         ).fit(X,y,ws) 
         
         coefs=clf_refit.coef_.ravel().copy()
         
+        clf_refit.feature_names_in_=self.feature_names_
+        
         return c,np.log10(c),coefs,clf_refit
     
     
     def select_C(self,C):
         
         self._check_is_fitted()
```

### Comparing `BDMLtools-0.4.2/BDMLtools/selector/fa.py` & `BDMLtools-0.4.3/BDMLtools/selector/fa.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/selector/lgbm.py` & `BDMLtools-0.4.3/BDMLtools/selector/lgbm.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
         from skopt.space import Categorical,Real,Integer
 
         para_space={
             'boosting_type':Categorical(['goss','gbdt']),
             'n_estimators': Integer(low=200, high=300, prior='uniform', transform='identity'),
             'learning_rate': Real(low=0.05, high=0.2, prior='uniform', transform='identity'),
-            'max_depth': Integer(low=2, high=4, prior='uniform', transform='identity')            
+            'max_depth': Integer(low=1, high=4, prior='uniform', transform='identity')            
         }
         
         return para_space
     
     
  
 class LgbmShapRFECVSelector(TransformerMixin,Base,BaseTunner):
```

### Comparing `BDMLtools-0.4.2/BDMLtools/selector/logtit.py` & `BDMLtools-0.4.3/BDMLtools/selector/logtit.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/selector/simple.py` & `BDMLtools-0.4.3/BDMLtools/selector/simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from category_encoders.ordinal import OrdinalEncoder
 from category_encoders import WOEEncoder
 from sklearn.linear_model import LogisticRegression
 from sklearn.impute import SimpleImputer
 from BDMLtools.fun import Specials
 from BDMLtools.selector.bin_fun import binFreq
 from sklearn.preprocessing import StandardScaler
+from sklearn.ensemble import RandomForestClassifier
 import numpy as np
 import pandas as pd
 import os
 from glob import glob
 from lightgbm import LGBMClassifier
 from BDMLtools.base import Base
 #from lofo import LOFOImportance, Dataset
@@ -30,71 +31,75 @@
     """ 
     预拟合数据，在不进行任何特征工程的前提下，使用全量特征预拟合数据并输出模型指标
     此功能用于在建模之前预估现有取数范围下模型的最终的性能，为取数、y定义的合理性提供参考
     若X存在object或number以外类型的列，那么这些列将被算法忽略
     
     Parameters:
     ----------
-        method='ceiling',预拟合数据方法，可选‘floor’,‘ceiling’
-            floor:地板算法，这里使用线性模型(sklearn对的logit回归(C=0.1 & solver='saga'))进行prefit  
+        method='lgbm',预拟合数据算法，可选‘lr’,lgbm‘,'rf'
+            lr,这里使用线性模型(sklearn对的logit回归(C=0.1 & solver='saga'))进行prefit  
                  + 分类变量处理方式:进行woe编码
                  + 数值特征缺失值:均值填补,当数据缺失值较多时，建议使用ceiling的lightbgm,其可应对缺失数据
-            ceiling:天花板算法,这里使用lightgbm进行prefit，且不进行任何交叉验证
+            lgbm,这里使用lightgbm进行prefit，且不进行任何交叉验证
                 + 分类变量处理方式:进行woe编码
                 + 数值特征缺失值:不处理        
+            rf,这里使用sklearn的rf进行prefit，且不进行任何交叉验证
+                + 分类变量处理方式:进行woe编码
+                + 数值特征缺失值:不处理                                 
         max_iter:100,logit回归最大迭代次数
-        tree_params={'max_depth':3,'learning_rate':0.05,'n_estimators':100},method='ceiling'时lightgbm的参数设定        
+        tree_params={'max_depth':3,'learning_rate':0.05,'n_estimators':100},method='lgbm'时lightgbm的参数设定,当method='rf'时将忽略learning_rate
         col_rm=None or list,需要移除的列名list，例如id类       
         
     Attribute:
     ----------
         encoder:category_encoders.WOEEncoder object,使用回归时分类变量的woe编码器
         imputer:sklearn.impute.SimpleImputer object,使用回归时数值特征缺失值处理器
         model:sklearn.linear_model.LogisticRegression or lightgbm.LGBMClassifier object拟合的模型对象
     """      
-    def __init__(self,method='ceiling',max_iter=100,tree_params={'max_depth':3,'learning_rate':0.05,'n_estimators':100},
-                 col_rm=None):
+    def __init__(self,method='lgbm',max_iter=100,tree_params={'max_depth':3,'learning_rate':0.05,'n_estimators':100},
+                 col_rm=None,random_state=123):
 
         self.method=method
         self.tree_params=tree_params
         self.max_iter=max_iter
         self.col_rm=col_rm 
+        self.random_state=random_state
         
         self._is_fitted=False
 
         
     def transform(self,X,y=None):
         
         self._check_is_fitted()
            
-        f_names=self.model.feature_names_in_ if self.method=='floor' else self.model.feature_name_
+        f_names=self.model.feature_name_ if self.method=='lgbm' else self.model.feature_names_in_
         
         X=X[f_names]
         
         X_numeric=X.select_dtypes('number')
         X_categoty=X.select_dtypes('object')
         
-        if self.method=='floor':
+        if self.method=='lr':
             
             X_numeric=pd.DataFrame(self.imputer.transform(X_numeric),
                                    columns=self.imputer.feature_names_in_,
-                                   index=X_numeric.index,dtype='float32') #downcast to save memory
+                                   index=X_numeric.index,dtype='float64') 
             
 
         if self.encoder:
             
             X_categoty=self.encoder.transform(X_categoty)
 
         
         X_new=pd.concat([X_numeric,X_categoty],axis=1)[f_names]
         
-        if self.method=='floor':
+        if self.method=='lr':
             
             X_new=pd.DataFrame(self._scaler.transform(X_new),columns=self._scaler.feature_names_in_,
-                                       index=X_new.index,dtype='float32') #downcast to save memory
+                                       index=X_new.index,dtype='float64')
         
         return X_new
     
     
     def predict_proba(self,X,y=None):
         
         X_model=self.transform(X)
@@ -110,25 +115,29 @@
         
         X=X.dropna(how='all',axis=1)
         
         if X.columns.size==0:
             
             raise ValueError('All columns in X are nan.')
         
-        if self.method=='ceiling':
+        if self.method=='lgbm':
             
             self.model=self._fit_lgbm(X,y,self.tree_params,sample_weight)
             
-        elif self.method=='floor':
+        elif self.method=='rf':
+            
+            self.model=self._fit_rf(X,y,self.tree_params,sample_weight)
+            
+        elif self.method=='lr':
             
             self.model=self._fit_reg(X,y,self.max_iter,sample_weight)
             
         else:
             
-            raise ValueError("method in ('ceiling','floor')")   
+            raise ValueError("method in ('lgbm','lr','rf')")   
             
         self._is_fitted=True
         
         return self
         
     
     def _fit_lgbm(self,X,y,params,sample_weight):
@@ -146,44 +155,65 @@
         lgb=LGBMClassifier(
                 boosting_type='gbdt',
                 objective = 'binary',
                 verbose=-1,
                 learning_rate=learning_rate,
                 n_estimators=n_estimators,
                 max_depth=max_depth,
+                random_state=self.random_state,
                 n_jobs=effective_n_jobs(n_jobs)
             ).fit(X_new,y,sample_weight=sample_weight)         
             
         return lgb
     
+    def _fit_rf(self,X,y,params,sample_weight):
+        
+        X_numeric,X_categoty_encode=self._get_X(X,y)
+        
+        X_new=pd.concat([X_numeric,X_categoty_encode],axis=1)
+        
+        
+        max_depth=params['max_depth'] if 'max_depth' in params else 3
+        n_estimators=params['n_estimators'] if 'n_estimators' in params else 100
+        n_jobs=params['n_jobs'] if 'n_jobs' in params else -1
+
+        rf=RandomForestClassifier(
+                n_estimators=n_estimators,
+                max_depth=max_depth,
+                n_jobs=effective_n_jobs(n_jobs),
+                random_state=self.random_state
+            ).fit(X_new,y,sample_weight=sample_weight)         
+            
+        return rf
+    
     
     def _fit_reg(self,X,y,max_iter,sample_weight):
         
         X_numeric,X_categoty_encode=self._get_X(X,y)
         
         X_new=pd.concat([X_numeric,X_categoty_encode],axis=1)
         
         self._scaler=StandardScaler().fit(X_new)
 
         X_new=pd.DataFrame(self._scaler.transform(X_new),
                        columns=X_new.columns,
                        index=X_numeric.index,dtype='float32') #downcast to save memory
 
-        logit=LogisticRegression(C=0.1,penalty='l2',solver='saga',max_iter=max_iter).fit(X_new,y,
+        logit=LogisticRegression(C=0.1,penalty='l2',solver='saga',max_iter=max_iter,random_state=self.random_state).fit(X_new,y,
                                                                                          sample_weight=sample_weight)  
         
         return logit
                 
     
     def _get_X(self,X,y):
         
         X_numeric=X.select_dtypes('number')
         X_categoty=X.select_dtypes('object')
         
-        if self.method=='floor':
+        if self.method=='lr':
             
             self.imputer=SimpleImputer(missing_values=np.nan,
                       strategy='median').fit(X_numeric)
             
             X_numeric=pd.DataFrame(self.imputer.transform(X_numeric),
                                             columns=self.imputer.feature_names_in_,
                                             index=X_numeric.index,dtype='float32') #downcast to save memory
@@ -209,62 +239,65 @@
     线性预筛选,适用于二分类模型
     
     筛选过程(设定为None时代表跳过相应步骤,相应序号会被重置):
     Step 1.缺失值(所有):缺失率高于用户定义值的列将被筛除
     Step 2.唯一值(所有):唯一值占比高于用户定义值列将被筛除
     Step 3.方差(数值特征):方差低于用户定义值列的列将被筛除
     Step 4.卡方独立性检验p值(字符)/方差分析p值(数值):p值大于用户定义值的列将被剔除(不支持样本权重)
-    Step 5.Lightgbm筛选(所有):split重要性低于用户定义值的列将被剔除
+    Step 5.树模型筛选(所有):重要性低于用户定义值的列将被剔除
     Step 6.Iv值筛选(所有):等频30箱后iv值低于用户定义值的列将被剔除
     
     目前Step 4不支持sample weight(样本权重)
     
     Parameters:
     ----------
         na_pct:float or None,(0,1),默认0.99,缺失率高于na_pct的列将被筛除，设定为None将跳过此步骤
         unique_pct:float or None,(0,1),默认0.99,唯一值占比高于unique_pct的列将被筛除,unique_pct与variance需同时输入，任一设定为None将跳过此步骤
         variance:float or None,默认0,方差低于variance的列将被筛除,将忽略缺失值,unique_pct与variance需同时输入，任一设定为None将跳过此步骤
         chif_pvalue:float or None,(0,1),默认0.05,大于chif_pvalue的列将被剔除,该步骤不支持样本权重。为None将跳过此步骤
                     + 卡方计算中，缺失值将被视为单独一类,
                     + f值计算中，缺失值将被填补为接近+inf和-inf，计算两次，两次结果都不显著的列都将被剔除   
                     + 不支持样本权重
-        tree_imps:int or None,lightgbm树的split_gan小于等于tree_imps的列将被剔除,默认1，设定为None将跳过此步骤
-        tree_size:int,lightgbm树个数,若数据量较大可降低树个数，若tree_imps为None时该参数将被忽略
+        tree_alg:string,默认'lgbm'，树模型算法，可选'lgbm'、'rf'            
+        tree_imps:float or None,lightgbm树的split_gan小于等于tree_imps的列将被剔除,默认1e-3，设定为None将跳过此步骤
+        tree_size:int,lightgbm树个数,若数据量较大可降低树个数，若tree_imps为None时该参数将被忽略       
         iv_limit:float or None使用进行iv快速筛选的iv阈值(数值等频30箱，分类则按照类别分箱)
-        n_jobs:int,默认-1,Lightgbm筛选过程中线程并行控制参数
+        n_jobs:int,默认-1,树模型筛选过程中线程并行控制参数
         out_path:str or None,模型报告路径,将预筛选过程每一步的筛选过程输出到模型报告中
         missing_values:缺失值指代值
                 + None
                 + list=[value1,value2,...],数据中所有列的值在[value1,value2,...]中都会被替换
                 + dict={col_name1:[value1,value2,...],...},数据中指定列替换，被指定的列的值在[value1,value2,...]中都会被替换且会被计入na_pct
         keep:list or None,需保留列的列名list
         
     Attribute:
     ----------
         features_info:dict,每一步筛选的特征进入记录
         preSelector_report:pd.DataFrame,outpath非None时产生的features_info数据框格式
     """    
     
     
-    def __init__(self,na_pct=0.99,unique_pct=0.99,variance=0,chif_pvalue=0.05,tree_imps=1,random_state=123,
+    def __init__(self,na_pct=0.99,unique_pct=0.99,variance=0,chif_pvalue=0.05,tree_alg='lgbm',tree_imps=1e-4,random_state=123,
                  tree_size=250,iv_limit=0.02,out_path=None,missing_values=None,keep=None,n_jobs=-1
                  ):
 
         self.na_pct=na_pct
         self.unique_pct=unique_pct #
         self.variance=variance
         self.chif_pvalue=chif_pvalue #
+        self.tree_alg=tree_alg
         self.tree_imps=tree_imps #
         self.tree_size=tree_size
         self.iv_limit=iv_limit
         self.out_path=out_path
         self.missing_values=missing_values
         self.random_state=random_state
         self.keep=keep
         self.n_jobs=n_jobs
+
         
         self._is_fitted=False
         
     def transform(self,X,y=None):
         """ 
         变量筛选
         """  
@@ -665,58 +698,78 @@
         list,筛选后的列名
         """
 
         X_numeric=X.select_dtypes(include='number')
         X_category=X.select_dtypes(include='object')
         X_oth=X.select_dtypes(exclude=['number','object'])
         
+        if self.tree_alg=='lgbm':
         
-        if X_category.columns.size:
-            
-            X_category_encode=OrdinalEncoder().fit_transform(X_category).sub(1)
-            
-            X_new=pd.concat([X_numeric,X_category_encode],axis=1)
-
-            lgb=LGBMClassifier(
-                boosting_type='gbdt',
-                objective = 'binary',
-                learning_rate=0.1,
-                n_estimators=tree_size,
-                random_state=123,
-                subsample=0.7,
-                colsample_bytree=1,
-                verbose=-1,
-                n_jobs=effective_n_jobs(self.n_jobs)
-            ).fit(X_new,y,sample_weight=sample_weight,categorical_feature=X_category_encode.columns.tolist())         
-
-            lgb_imps=lgb.booster_.feature_importance(importance_type='split')
+            if X_category.columns.size:
+                
+                X_category_encode=OrdinalEncoder().fit_transform(X_category).sub(1)
+                
+                X_new=pd.concat([X_numeric,X_category_encode],axis=1)
+                    
+                clf=LGBMClassifier(
+                    boosting_type='gbdt',
+                    objective = 'binary',
+                    learning_rate=0.1,
+                    n_estimators=tree_size,
+                    random_state=self.random_state,
+                    subsample=0.7,
+                    colsample_bytree=1,
+                    verbose=-1,
+                    n_jobs=effective_n_jobs(self.n_jobs)
+                ).fit(X_new,y,sample_weight=sample_weight,categorical_feature=X_category_encode.columns.tolist())         
+    
+                clf_imps=clf.booster_.feature_importance(importance_type='split')
+                
+                return X_new.columns[clf_imps>tree_imps].tolist()+X_oth.columns.tolist()
+                               
+            
+            elif X_numeric.columns.size:
+                
+                clf=LGBMClassifier(
+                    boosting_type='gbdt',
+                    objective = 'binary',
+                    learning_rate=0.1,
+                    n_estimators=tree_size,
+                    random_state=self.random_state,
+                    subsample=0.7,
+                    colsample_bytree=1,
+                    verbose=-1,
+                    n_jobs=effective_n_jobs(self.n_jobs)
+                ).fit(X_numeric,y,sample_weight=sample_weight)         
+    
+                clf_imps=clf.booster_.feature_importance(importance_type='split')
+                
         
-            return X_new.columns[lgb_imps>tree_imps].tolist()+X_oth.columns.tolist()
+                return X_numeric.columns[clf_imps>tree_imps].tolist()+X_oth.columns.tolist()
         
-        elif X_numeric.columns.size:
-            
-            lgb=LGBMClassifier(
-                boosting_type='gbdt',
-                objective = 'binary',
-                learning_rate=0.1,
+            else:
+                
+                return X_oth.columns.tolist()
+        
+        elif self.tree_alg=='rf':
+                
+            clf=RandomForestClassifier(                    
                 n_estimators=tree_size,
-                random_state=123,
-                subsample=0.7,
-                colsample_bytree=1,
-                verbose=-1,
+                random_state=self.random_state,
+                max_depth=3,
                 n_jobs=effective_n_jobs(self.n_jobs)
-            ).fit(X_numeric,y,sample_weight=sample_weight)         
+            ).fit(X_numeric,y,sample_weight=sample_weight)    
 
-            lgb_imps=lgb.booster_.feature_importance(importance_type='split')
+            clf_imps=clf.feature_importances_             
         
-            return X_numeric.columns[lgb_imps>tree_imps].tolist()+X_oth.columns.tolist()
+            return X_numeric.columns[clf_imps>tree_imps].tolist()+X_oth.columns.tolist()+X_category.columns.tolist()
         
         else:
             
-            return X_oth.columns.tolist()
+            raise ValueError('tree_alg in ("lgbm","rf")')          
         
         
     # def _filterbyLofoimp(self,X,y,lofo_imp=0,sample_weight=None):
         
     #     """
     #     使用Leave one out重要性筛选特征:
     #         + 特征x的重要性=全量特征模型表在交叉验证集表现的均值-移除特征x后的模型在交叉验证集表现的均值
```

### Comparing `BDMLtools-0.4.2/BDMLtools/tuner/base.py` & `BDMLtools-0.4.3/BDMLtools/tuner/base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/tuner/bayesian.py` & `BDMLtools-0.4.3/BDMLtools/tuner/bayesian.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/tuner/fun.py` & `BDMLtools-0.4.3/BDMLtools/tuner/fun.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/tuner/gridcv.py` & `BDMLtools-0.4.3/BDMLtools/tuner/gridcv.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools/tuner/halvingcv.py` & `BDMLtools-0.4.3/BDMLtools/tuner/halvingcv.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/BDMLtools.egg-info/PKG-INFO` & `BDMLtools-0.4.3/BDMLtools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDMLtools
-Version: 0.4.2
+Version: 0.4.3
 Summary: Ml learning tools for busniess data mining
 Author: 曾珂
 Author-email: zengke403@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastparquet>=0.7.1
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: plotnine>=0.12.4
-Requires-Dist: scikit-learn>=1.0.2
+Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: category_encoders>=2.3.0
 Requires-Dist: lightgbm>=3.3.0
 Requires-Dist: probatus>=2.0.0
 Requires-Dist: mlxtend>=0.19.0
 Requires-Dist: scikit-optimize>=0.9.0
 Requires-Dist: shap<0.43.0,>=0.41.0
 Requires-Dist: IPython
 Requires-Dist: openpyxl
 Provides-Extra: all
 Requires-Dist: fastparquet>=0.7.1; extra == "all"
 Requires-Dist: pandas>=1.3.5; extra == "all"
 Requires-Dist: plotnine>=0.12.4; extra == "all"
-Requires-Dist: scikit-learn>=1.0.2; extra == "all"
+Requires-Dist: scikit-learn>=1.4.0; extra == "all"
 Requires-Dist: category_encoders>=2.3.0; extra == "all"
 Requires-Dist: lightgbm>=3.3.0; extra == "all"
 Requires-Dist: probatus>=2.0.0; extra == "all"
 Requires-Dist: mlxtend>=0.19.0; extra == "all"
 Requires-Dist: scikit-optimize>=0.9.0; extra == "all"
 Requires-Dist: shap<0.43.0,>=0.41.0; extra == "all"
 Requires-Dist: IPython; extra == "all"
@@ -76,12 +76,15 @@
 
 ```
 pip uninstall BDMLtools
 ```
 
 更新
 ```
-v0.4.2
-1.支持py3.12
-2.修复skopt的载入bug
-3.更新单元测试脚本,更新部分代码说明
+v0.4.3
+1.prefitModel中加入sklearn的随机森林算法，并修改参数配置
+2.prefitSelector中加入sklearn的随机森林算法，并修改参数配置
+3.完善了LassoLogit中列名的显示
+4.修复了决策树分箱(binTree)中，缺失值分箱好坏频数为0时无法产生分箱点的bug
+5.sklearn版本依赖改为>=1.4.0
+6.更新单元测试脚本，更新部分代码说明
 ```
```

### Comparing `BDMLtools-0.4.2/BDMLtools.egg-info/SOURCES.txt` & `BDMLtools-0.4.3/BDMLtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/LICENSE` & `BDMLtools-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/PKG-INFO` & `BDMLtools-0.4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDMLtools
-Version: 0.4.2
+Version: 0.4.3
 Summary: Ml learning tools for busniess data mining
 Author: 曾珂
 Author-email: zengke403@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastparquet>=0.7.1
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: plotnine>=0.12.4
-Requires-Dist: scikit-learn>=1.0.2
+Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: category_encoders>=2.3.0
 Requires-Dist: lightgbm>=3.3.0
 Requires-Dist: probatus>=2.0.0
 Requires-Dist: mlxtend>=0.19.0
 Requires-Dist: scikit-optimize>=0.9.0
 Requires-Dist: shap<0.43.0,>=0.41.0
 Requires-Dist: IPython
 Requires-Dist: openpyxl
 Provides-Extra: all
 Requires-Dist: fastparquet>=0.7.1; extra == "all"
 Requires-Dist: pandas>=1.3.5; extra == "all"
 Requires-Dist: plotnine>=0.12.4; extra == "all"
-Requires-Dist: scikit-learn>=1.0.2; extra == "all"
+Requires-Dist: scikit-learn>=1.4.0; extra == "all"
 Requires-Dist: category_encoders>=2.3.0; extra == "all"
 Requires-Dist: lightgbm>=3.3.0; extra == "all"
 Requires-Dist: probatus>=2.0.0; extra == "all"
 Requires-Dist: mlxtend>=0.19.0; extra == "all"
 Requires-Dist: scikit-optimize>=0.9.0; extra == "all"
 Requires-Dist: shap<0.43.0,>=0.41.0; extra == "all"
 Requires-Dist: IPython; extra == "all"
@@ -76,12 +76,15 @@
 
 ```
 pip uninstall BDMLtools
 ```
 
 更新
 ```
-v0.4.2
-1.支持py3.12
-2.修复skopt的载入bug
-3.更新单元测试脚本,更新部分代码说明
+v0.4.3
+1.prefitModel中加入sklearn的随机森林算法，并修改参数配置
+2.prefitSelector中加入sklearn的随机森林算法，并修改参数配置
+3.完善了LassoLogit中列名的显示
+4.修复了决策树分箱(binTree)中，缺失值分箱好坏频数为0时无法产生分箱点的bug
+5.sklearn版本依赖改为>=1.4.0
+6.更新单元测试脚本，更新部分代码说明
 ```
```

### Comparing `BDMLtools-0.4.2/README.md` & `BDMLtools-0.4.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -28,12 +28,15 @@
 
 ```
 pip uninstall BDMLtools
 ```
 
 更新
 ```
-v0.4.2
-1.支持py3.12
-2.修复skopt的载入bug
-3.更新单元测试脚本,更新部分代码说明
+v0.4.3
+1.prefitModel中加入sklearn的随机森林算法，并修改参数配置
+2.prefitSelector中加入sklearn的随机森林算法，并修改参数配置
+3.完善了LassoLogit中列名的显示
+4.修复了决策树分箱(binTree)中，缺失值分箱好坏频数为0时无法产生分箱点的bug
+5.sklearn版本依赖改为>=1.4.0
+6.更新单元测试脚本，更新部分代码说明
 ```
```

### Comparing `BDMLtools-0.4.2/setup.py` & `BDMLtools-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,30 +35,29 @@
 base_pkgs=[       #'numpy>=1.18,<=1.23.5',#https://github.com/numpy/numpy
                   #'matplotlib>=3.5.0,<=3.5.3',
                   #'lofo-importance>=0.3.1',#https://github.com/aerdem4/lofo-importance
                   'fastparquet>=0.7.1',#https://github.com/dask/fastparquet
                   'pandas>=1.3.5',#https://github.com/pandas-dev/pandas
                   #'statsmodels>=0.13.2',#https://github.com/statsmodels/statsmodels
                   'plotnine==0.12.4' if python_ver() == "3.8" else 'plotnine>=0.12.4',#https://github.com/has2k1/plotnine
-                  'scikit-learn>=1.0.2',#https://github.com/scikit-learn/scikit-learn
+                  'scikit-learn>=1.0.0' if python_ver() == "3.8" else 'scikit-learn>=1.4.0',#https://github.com/scikit-learn/scikit-learn
                   'category_encoders>=2.3.0',#https://github.com/scikit-learn-contrib/category_encoders
                   'lightgbm>=3.3.0',#https://github.com/microsoft/LightGBM 
                   'probatus>=2.0.0',#https://github.com/ing-bank/probatus
                   'mlxtend>=0.19.0',#https://github.com/rasbt/mlxtend
                   'scikit-optimize>=0.9.0',#https://github.com/scikit-optimize/scikit-optimize
                   'shap>=0.41.0,<0.43.0',
                   "IPython",
                   'openpyxl'
                  ]
 
 #warning msg:
 #%category_encoders 2.6.2/pandas 2.1.1: is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead
 #plotnine 0.10.1/pandas 2.1.1: is_categorical_dtype is deprecated and will be removed in a future version. Use isinstance(dtype, CategoricalDtype) instead 
 
-
 dev_dep = [
     "pytest>=6.0.0",
     "pytest-cov>=2.10.0",
     "mock",
     "threadpoolctl>=3.0.0",#kmeans:https://stackoverflow.com/questions/71352354/sklearn-kmeans-is-not-working-as-i-only-get-nonetype-object-has-no-attribute
     #'shap>=0.41.0',
     'xgboost>=1.5.0',#https://github.com/dmlc/xgboost
```

### Comparing `BDMLtools-0.4.2/test/test_base.py` & `BDMLtools-0.4.3/test/test_base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/test/test_clearner.py` & `BDMLtools-0.4.3/test/test_clearner.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/test/test_eval.py` & `BDMLtools-0.4.3/test/test_eval.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/test/test_report.py` & `BDMLtools-0.4.3/test/test_report.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.4.2/test/test_selector.py` & `BDMLtools-0.4.3/test/test_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,20 +178,22 @@
     X=pd.DataFrame(
         {'a':[1,2,2,4,5],'b':[1,2,3,4,5],'c':[1,1,1,2,1],'d':['a','a','a','a','b']}
         )
     y=pd.Series([0,0,1,1,1],name='y')
 
     pm=prefitModel(
         tree_params={'max_depth': 2, 'learning_rate': 0.05, 'n_estimators': 10,'n_jobs':1},
-        method='ceiling',
+        method='lgbm',
                    ).fit(X,y)    
     
-    pm=prefitModel(method='floor',max_iter=10).fit(X,y)    
+    pm=prefitModel(method='lr',max_iter=10).fit(X,y)    
     
-    pm=prefitModel(method='floor',col_rm='a').fit(X,y)    
+    pm=prefitModel(method='lr',col_rm='a').fit(X,y)    
+    
+    pm=prefitModel(method='rf',tree_params={'max_depth': 2,'n_estimators': 10}).fit(X,y)    
     
     pm.predict_proba(X)
     
 
 def test_preSelector():
     
     X=pd.DataFrame(
@@ -204,14 +206,15 @@
     ws=pd.Series(np.ones(100),name='ws')
     
     y=pd.Series(np.append(np.zeros(50),np.ones(50)),name='y')
     
     res=preSelector().fit_transform(X,y)   
     res=preSelector().fit(X,y,cat_features=['b'])   
     res=preSelector().fit(X,y,sample_weight=ws).transform(X)   
+    res=preSelector(tree_alg='rf').fit_transform(X,y)  
     res=preSelector(keep=['a']).fit_transform(X,y)  
     assert 'a' in res.columns
     res=preSelector(out_path='tmp').fit_transform(X,y) 
 
 def test_lassologit():
     
     from sklearn.datasets import load_breast_cancer
```

### Comparing `BDMLtools-0.4.2/test/test_tunner.py` & `BDMLtools-0.4.3/test/test_tunner.py`

 * *Files identical despite different names*

