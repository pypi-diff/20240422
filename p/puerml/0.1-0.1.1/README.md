# Comparing `tmp/puerml-0.1.tar.gz` & `tmp/puerml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puerml-0.1.tar", last modified: Mon Apr 22 09:02:41 2024, max compression
+gzip compressed data, was "puerml-0.1.1.tar", last modified: Mon Apr 22 09:21:53 2024, max compression
```

## Comparing `puerml-0.1.tar` & `puerml-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 09:02:41.894847 puerml-0.1/
--rw-r--r--   0 Alexander   (502) staff       (20)     1070 2024-04-22 09:02:31.000000 puerml-0.1/LICENSE
--rw-r--r--   0 Alexander   (502) staff       (20)      151 2024-04-22 09:02:41.894488 puerml-0.1/PKG-INFO
--rw-r--r--   0 Alexander   (502) staff       (20)        4 2024-04-22 09:02:31.000000 puerml-0.1/README.md
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 09:02:41.891294 puerml-0.1/puerml/
--rw-r--r--   0 Alexander   (502) staff       (20)       45 2024-04-22 09:02:31.000000 puerml-0.1/puerml/__init__.py
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 09:02:41.893930 puerml-0.1/puerml/library/
--rw-r--r--   0 Alexander   (502) staff       (20)       77 2024-04-22 09:02:31.000000 puerml-0.1/puerml/library/__init__.py
--rw-r--r--   0 Alexander   (502) staff       (20)      824 2024-04-22 09:02:31.000000 puerml-0.1/puerml/library/benchmark.py
--rw-r--r--   0 Alexander   (502) staff       (20)     8349 2024-04-22 09:02:31.000000 puerml-0.1/puerml/library/data_frame.py
--rw-r--r--   0 Alexander   (502) staff       (20)     1693 2024-04-22 09:02:31.000000 puerml-0.1/puerml/library/jsonl.py
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 09:02:41.892716 puerml-0.1/puerml.egg-info/
--rw-r--r--   0 Alexander   (502) staff       (20)      151 2024-04-22 09:02:41.000000 puerml-0.1/puerml.egg-info/PKG-INFO
--rw-r--r--   0 Alexander   (502) staff       (20)      273 2024-04-22 09:02:41.000000 puerml-0.1/puerml.egg-info/SOURCES.txt
--rw-r--r--   0 Alexander   (502) staff       (20)        1 2024-04-22 09:02:41.000000 puerml-0.1/puerml.egg-info/dependency_links.txt
--rw-r--r--   0 Alexander   (502) staff       (20)        7 2024-04-22 09:02:41.000000 puerml-0.1/puerml.egg-info/top_level.txt
--rw-r--r--   0 Alexander   (502) staff       (20)       38 2024-04-22 09:02:41.894997 puerml-0.1/setup.cfg
--rw-r--r--   0 Alexander   (502) staff       (20)      147 2024-04-22 09:02:31.000000 puerml-0.1/setup.py
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 09:21:53.347128 puerml-0.1.1/
+-rw-r--r--   0 Alexander   (502) staff       (20)     1070 2024-04-22 09:02:31.000000 puerml-0.1.1/LICENSE
+-rw-r--r--   0 Alexander   (502) staff       (20)      153 2024-04-22 09:21:53.346818 puerml-0.1.1/PKG-INFO
+-rw-r--r--   0 Alexander   (502) staff       (20)        4 2024-04-22 09:02:31.000000 puerml-0.1.1/README.md
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 09:21:53.341971 puerml-0.1.1/puerml/
+-rw-r--r--   0 Alexander   (502) staff       (20)       77 2024-04-22 09:10:49.000000 puerml-0.1.1/puerml/__init__.py
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 09:21:53.346184 puerml-0.1.1/puerml/library/
+-rw-r--r--   0 Alexander   (502) staff       (20)       97 2024-04-22 09:10:49.000000 puerml-0.1.1/puerml/library/__init__.py
+-rw-r--r--   0 Alexander   (502) staff       (20)      850 2024-04-22 09:10:49.000000 puerml-0.1.1/puerml/library/benchmark.py
+-rw-r--r--   0 Alexander   (502) staff       (20)     8390 2024-04-22 09:10:49.000000 puerml-0.1.1/puerml/library/data_frame.py
+-rw-r--r--   0 Alexander   (502) staff       (20)     1714 2024-04-22 09:10:49.000000 puerml-0.1.1/puerml/library/jsonl.py
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 09:21:53.343994 puerml-0.1.1/puerml.egg-info/
+-rw-r--r--   0 Alexander   (502) staff       (20)      153 2024-04-22 09:21:53.000000 puerml-0.1.1/puerml.egg-info/PKG-INFO
+-rw-r--r--   0 Alexander   (502) staff       (20)      273 2024-04-22 09:21:53.000000 puerml-0.1.1/puerml.egg-info/SOURCES.txt
+-rw-r--r--   0 Alexander   (502) staff       (20)        1 2024-04-22 09:21:53.000000 puerml-0.1.1/puerml.egg-info/dependency_links.txt
+-rw-r--r--   0 Alexander   (502) staff       (20)        7 2024-04-22 09:21:53.000000 puerml-0.1.1/puerml.egg-info/top_level.txt
+-rw-r--r--   0 Alexander   (502) staff       (20)       38 2024-04-22 09:21:53.347221 puerml-0.1.1/setup.cfg
+-rw-r--r--   0 Alexander   (502) staff       (20)      149 2024-04-22 09:21:52.000000 puerml-0.1.1/setup.py
```

### Comparing `puerml-0.1/LICENSE` & `puerml-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `puerml-0.1/puerml/library/benchmark.py` & `puerml-0.1.1/puerml/library/benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import time
 import json
 
+__all__ = ['Benchmark']
+
+
 class Benchmark:
     data = {}
 
     @staticmethod
     def time(func):
         def wrapper(*args, **kwargs):
             start_time = time.time()
```

### Comparing `puerml-0.1/puerml/library/data_frame.py` & `puerml-0.1.1/puerml/library/data_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import csv
 
+__all__ = ['DataFrameRow', 'DataFrame']
+
 
 class DataFrameRow(list):
 	def __init__(self, *args, **kwargs):
 		self.df = kwargs['df']
 		super().__init__(*args)
 
 	def set(self, col, value):
```

### Comparing `puerml-0.1/puerml/library/jsonl.py` & `puerml-0.1.1/puerml/library/jsonl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import json
 
+__all__ = ['Jsonl']
+
 
 class Jsonl:
 	@staticmethod
 	def save(data, name, file_dir, max_file_size=52428800):
 		'Writes data to jsonl files ensuring each file does not exceed the specified max_file_size'
 		chunk_num    = 0
 		current_size = 0
```

