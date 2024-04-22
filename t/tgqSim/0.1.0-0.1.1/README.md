# Comparing `tmp/tgqSim-0.1.0.tar.gz` & `tmp/tgqSim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgqSim-0.1.0.tar", last modified: Fri Apr 19 06:00:22 2024, max compression
+gzip compressed data, was "tgqSim-0.1.1.tar", last modified: Mon Apr 22 05:59:12 2024, max compression
```

## Comparing `tgqSim-0.1.0.tar` & `tgqSim-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:00:22.816327 tgqSim-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-04-19 06:00:21.000000 tgqSim-0.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-19 06:00:21.000000 tgqSim-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      752 2024-04-19 06:00:22.816327 tgqSim-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-19 06:00:21.000000 tgqSim-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 06:00:22.816327 tgqSim-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-19 06:00:22.000000 tgqSim-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:00:22.813327 tgqSim-0.1.0/tgqSim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:00:22.815327 tgqSim-0.1.0/tgqSim/GateSimulation/
--rw-rw-rw-   0 root         (0) root         (0)     3793 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/GateSimulation/DoubleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/GateSimulation/SingleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/GateSimulation/TripleGate.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/GateSimulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16505 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/QuantumCircuit.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/draw_circuit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:00:22.815327 tgqSim-0.1.0/tgqSim/lib/
--rw-rw-rw-   0 root         (0) root         (0)    67288 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/lib/tgq_simulator.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:00:22.814327 tgqSim-0.1.0/tgqSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)      752 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      430 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:59:12.418388 tgqSim-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-04-22 05:59:11.000000 tgqSim-0.1.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-22 05:59:11.000000 tgqSim-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      752 2024-04-22 05:59:12.418388 tgqSim-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-22 05:59:11.000000 tgqSim-0.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 05:59:12.418388 tgqSim-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-22 05:59:11.000000 tgqSim-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:59:12.415388 tgqSim-0.1.1/tgqSim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:59:12.417388 tgqSim-0.1.1/tgqSim/GateSimulation/
+-rw-rw-rw-   0 root         (0) root         (0)     3793 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/GateSimulation/DoubleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/GateSimulation/SingleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/GateSimulation/TripleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/GateSimulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16519 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/QuantumCircuit.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/draw_circuit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:59:12.418388 tgqSim-0.1.1/tgqSim/lib/
+-rw-rw-rw-   0 root         (0) root         (0)    67288 2024-04-22 05:59:11.000000 tgqSim-0.1.1/tgqSim/lib/tgq_simulator.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:59:12.417388 tgqSim-0.1.1/tgqSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      752 2024-04-22 05:59:12.000000 tgqSim-0.1.1/tgqSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-22 05:59:12.000000 tgqSim-0.1.1/tgqSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 05:59:12.000000 tgqSim-0.1.1/tgqSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-22 05:59:12.000000 tgqSim-0.1.1/tgqSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-22 05:59:12.000000 tgqSim-0.1.1/tgqSim.egg-info/top_level.txt
```

### Comparing `tgqSim-0.1.0/LICENSE` & `tgqSim-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.0/PKG-INFO` & `tgqSim-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.0
+Version: 0.1.1
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,cetc,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.1.0/setup.py` & `tgqSim-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tgqSim',
-    version='0.1.0',
+    version='0.1.1',
     description='TGQ量子模拟器',  # 包描述
     long_description="Python for quantum simulation http://www.tiangongqs.com",  # 详细描述
     long_description_content_type='text/markdown',
     author='tiangongqs',  # 作者姓名
     license='MIT',  # 许可证
     package=find_packages(),
     include_package_data=True,
```

### Comparing `tgqSim-0.1.0/tgqSim/GateSimulation/DoubleGate.py` & `tgqSim-0.1.1/tgqSim/GateSimulation/DoubleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.0/tgqSim/GateSimulation/SingleGate.py` & `tgqSim-0.1.1/tgqSim/GateSimulation/SingleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.0/tgqSim/GateSimulation/TripleGate.py` & `tgqSim-0.1.1/tgqSim/GateSimulation/TripleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.0/tgqSim/QuantumCircuit.py` & `tgqSim-0.1.1/tgqSim/QuantumCircuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 """
 @author: Yuchen He
 @contact: heyuchen@tgqs.net
 @version: 1.0.1
 @file: QuantumCircuit.py
 @time: 2024/1/16 17:16
 """
-from GateSimulation import SingleGate, DoubleGate, TripleGate
+from tgqSim.GateSimulation import SingleGate, DoubleGate, TripleGate
 from typing import Union
 import random, os, ctypes
 import numpy as np
-import draw_circuit_tools as tools
+import tgqSim.draw_circuit_tools as tools
 import matplotlib.pyplot as plt
 import GPUtil
 # from numba import njit, prange
 
 class Float2(ctypes.Structure):
     _fields_ = [("x", ctypes.c_float),
                 ("y", ctypes.c_float)]
```

### Comparing `tgqSim-0.1.0/tgqSim/draw_circuit_tools.py` & `tgqSim-0.1.1/tgqSim/draw_circuit_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.0/tgqSim/lib/tgq_simulator.so` & `tgqSim-0.1.1/tgqSim/lib/tgq_simulator.so`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.0/tgqSim.egg-info/PKG-INFO` & `tgqSim-0.1.1/tgqSim.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.0
+Version: 0.1.1
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,cetc,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

