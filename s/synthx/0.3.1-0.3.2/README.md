# Comparing `tmp/synthx-0.3.1.tar.gz` & `tmp/synthx-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthx-0.3.1.tar", max compression
+gzip compressed data, was "synthx-0.3.2.tar", max compression
```

## Comparing `synthx-0.3.1.tar` & `synthx-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7163 2024-03-25 15:42:05.698171 synthx-0.3.1/README.md
--rw-r--r--   0        0        0     1242 2024-04-19 06:33:17.570540 synthx-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      371 2024-03-25 05:20:00.886950 synthx-0.3.1/synthx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-0.3.1/synthx/core/__init__.py
--rw-r--r--   0        0        0     7302 2024-04-18 01:31:14.755205 synthx-0.3.1/synthx/core/dataset.py
--rw-r--r--   0        0        0     4718 2024-03-25 05:07:58.244991 synthx-0.3.1/synthx/core/result.py
--rw-r--r--   0        0        0     7004 2024-04-18 01:31:14.755420 synthx-0.3.1/synthx/core/sample.py
--rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-0.3.1/synthx/errors/__init__.py
--rw-r--r--   0        0        0     6003 2024-04-19 06:33:17.570783 synthx-0.3.1/synthx/method.py
--rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-0.3.1/synthx/stats/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-0.3.1/synthx/stats/norm.py
--rw-r--r--   0        0        0     1026 2024-03-25 05:14:52.967319 synthx-0.3.1/synthx/stats/p.py
--rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 synthx-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     7163 2024-03-25 15:42:05.698171 synthx-0.3.2/README.md
+-rw-r--r--   0        0        0     1242 2024-04-22 08:16:30.556375 synthx-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      371 2024-03-25 05:20:00.886950 synthx-0.3.2/synthx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-0.3.2/synthx/core/__init__.py
+-rw-r--r--   0        0        0     7302 2024-04-18 01:31:14.755205 synthx-0.3.2/synthx/core/dataset.py
+-rw-r--r--   0        0        0     4718 2024-03-25 05:07:58.244991 synthx-0.3.2/synthx/core/result.py
+-rw-r--r--   0        0        0     7004 2024-04-18 01:31:14.755420 synthx-0.3.2/synthx/core/sample.py
+-rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-0.3.2/synthx/errors/__init__.py
+-rw-r--r--   0        0        0     6345 2024-04-22 08:16:30.556687 synthx-0.3.2/synthx/method.py
+-rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-0.3.2/synthx/stats/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-0.3.2/synthx/stats/norm.py
+-rw-r--r--   0        0        0     1026 2024-03-25 05:14:52.967319 synthx-0.3.2/synthx/stats/p.py
+-rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 synthx-0.3.2/PKG-INFO
```

### Comparing `synthx-0.3.1/README.md` & `synthx-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `synthx-0.3.1/pyproject.toml` & `synthx-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synthx"
-version = "0.3.1"
+version = "0.3.2"
 description = "A Python Library for Advanced Synthetic Control Analysis"
 authors = ["kenki931128 <kenki.nkmr@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `synthx-0.3.1/synthx/core/dataset.py` & `synthx-0.3.2/synthx/core/dataset.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.1/synthx/core/result.py` & `synthx-0.3.2/synthx/core/result.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.1/synthx/core/sample.py` & `synthx-0.3.2/synthx/core/sample.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.1/synthx/errors/__init__.py` & `synthx-0.3.2/synthx/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.1/synthx/method.py` & `synthx-0.3.2/synthx/method.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Synthetic Control Method."""
 
+import sys
+
 import numpy as np
 import scipy.optimize
 from tqdm import tqdm
 
 import synthx as sx
 from synthx.errors import NoFeasibleModelError
 
@@ -107,36 +109,43 @@
             - effect_test (float): The estimated effect of the intervention in the test area.
             - effects_placebo (List[float]): The estimated placebo effects for each control area.
             - sc_test (sx.SyntheticControlResult): The synthetic control result for the test area.
             - scs_placebo (List[sx.SyntheticControlResult]): The synthetic control results
                 for each control area.
     """
     # placebo effect in test area
-    sc_test = synthetic_control(dataset)
+    try:
+        sc_test = synthetic_control(dataset)
+    except NoFeasibleModelError:
+        raise NoFeasibleModelError('synthetic control optimization failed for test units.')
     effect_test = sc_test.estimate_effects()
 
     # placebo effects in control areas
     effects_placebo: list[float] = []
     scs_placebo: list[sx.SyntheticControlResult] = []
     control_units = (
         dataset.data.filter(~dataset.data[dataset.unit_column].is_in(dataset.intervention_units))[
             dataset.unit_column
         ]
         .unique()
         .to_list()
     )
     df_placebo = dataset.data.filter(dataset.data[dataset.unit_column].is_in(control_units))
-    for test_unit_placebo in tqdm(control_units):
+    for test_unit_placebo in tqdm(control_units, file=sys.stdout):
         dataset_placebo = sx.Dataset(
             df_placebo,
             unit_column=dataset.unit_column,
             time_column=dataset.time_column,
             y_column=dataset.y_column,
             covariate_columns=dataset.covariate_columns,
             intervention_units=test_unit_placebo,
             intervention_time=dataset.intervention_time,
         )
-        sc_placebo = synthetic_control(dataset_placebo)
+        try:
+            sc_placebo = synthetic_control(dataset_placebo)
+        except NoFeasibleModelError:
+            tqdm.write(f'placebo synthetic control optimization failed: unit {test_unit_placebo}.')
+            continue
         effects_placebo.append(sc_placebo.estimate_effects())
         scs_placebo.append(sc_placebo)
 
     return effect_test, effects_placebo, sc_test, scs_placebo
```

### Comparing `synthx-0.3.1/synthx/stats/norm.py` & `synthx-0.3.2/synthx/stats/norm.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.1/synthx/stats/p.py` & `synthx-0.3.2/synthx/stats/p.py`

 * *Files identical despite different names*

### Comparing `synthx-0.3.1/PKG-INFO` & `synthx-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthx
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python Library for Advanced Synthetic Control Analysis
 License: MIT
 Author: kenki931128
 Author-email: kenki.nkmr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

