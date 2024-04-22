# Comparing `tmp/torch-fem-0.1.8.tar.gz` & `tmp/torch-fem-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-fem-0.1.8.tar", last modified: Mon Mar 25 06:40:38 2024, max compression
+gzip compressed data, was "torch-fem-0.1.9.tar", last modified: Mon Mar 25 11:52:38 2024, max compression
```

## Comparing `torch-fem-0.1.8.tar` & `torch-fem-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:40:38.412865 torch-fem-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-25 06:40:34.000000 torch-fem-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-25 06:40:38.412865 torch-fem-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-25 06:40:34.000000 torch-fem-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-25 06:40:34.000000 torch-fem-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 06:40:38.412865 torch-fem-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:40:38.404865 torch-fem-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:40:38.412865 torch-fem-0.1.8/src/torch_fem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-25 06:40:38.000000 torch-fem-0.1.8/src/torch_fem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-25 06:40:38.000000 torch-fem-0.1.8/src/torch_fem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 06:40:38.000000 torch-fem-0.1.8/src/torch_fem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-25 06:40:38.000000 torch-fem-0.1.8/src/torch_fem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 06:40:38.000000 torch-fem-0.1.8/src/torch_fem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:40:38.408865 torch-fem-0.1.8/src/torchfem/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:40:38.408865 torch-fem-0.1.8/src/torchfem/data/
--rw-r--r--   0 runner    (1001) docker     (127)    42692 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/data/plate_hole.vtk
--rw-r--r--   0 runner    (1001) docker     (127)   613525 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/data/tensile.vtu
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    14191 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/homogenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/materials.py
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/planar.py
--rw-r--r--   0 runner    (1001) docker     (127)    12886 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/solid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-03-25 06:40:34.000000 torch-fem-0.1.8/src/torchfem/truss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 06:40:38.408865 torch-fem-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-25 06:40:34.000000 torch-fem-0.1.8/tests/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:52:38.712629 torch-fem-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-25 11:52:34.000000 torch-fem-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-25 11:52:38.708629 torch-fem-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-25 11:52:34.000000 torch-fem-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-25 11:52:34.000000 torch-fem-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 11:52:38.712629 torch-fem-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:52:38.704629 torch-fem-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:52:38.708629 torch-fem-0.1.9/src/torch_fem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-25 11:52:38.000000 torch-fem-0.1.9/src/torch_fem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-25 11:52:38.000000 torch-fem-0.1.9/src/torch_fem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:52:38.000000 torch-fem-0.1.9/src/torch_fem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-25 11:52:38.000000 torch-fem-0.1.9/src/torch_fem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 11:52:38.000000 torch-fem-0.1.9/src/torch_fem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:52:38.708629 torch-fem-0.1.9/src/torchfem/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:52:38.708629 torch-fem-0.1.9/src/torchfem/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    42692 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/data/plate_hole.vtk
+-rw-r--r--   0 runner    (1001) docker     (127)   613525 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/data/tensile.vtu
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/homogenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/planar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12886 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/solid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-03-25 11:52:34.000000 torch-fem-0.1.9/src/torchfem/truss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:52:38.708629 torch-fem-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-25 11:52:34.000000 torch-fem-0.1.9/tests/test_notebooks.py
```

### Comparing `torch-fem-0.1.8/LICENSE` & `torch-fem-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/PKG-INFO` & `torch-fem-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-fem
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple finite element assemblers with torch.
 Author-email: Nils Meyer <nils.meyer@uni-a.de>
 License: Copyright 2024 Nils Meyer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `torch-fem-0.1.8/README.md` & `torch-fem-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/pyproject.toml` & `torch-fem-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "torch-fem"
-version = "0.1.8"
+version = "0.1.9"
 authors = [{ name = "Nils Meyer", email = "nils.meyer@uni-a.de" }]
 description = "Simple finite element assemblers with torch."
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["finite elements", "automatic differentiation"]
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `torch-fem-0.1.8/src/torch_fem.egg-info/PKG-INFO` & `torch-fem-0.1.9/src/torch_fem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-fem
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple finite element assemblers with torch.
 Author-email: Nils Meyer <nils.meyer@uni-a.de>
 License: Copyright 2024 Nils Meyer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `torch-fem-0.1.8/src/torch_fem.egg-info/SOURCES.txt` & `torch-fem-0.1.9/src/torch_fem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/src/torchfem/base.py` & `torch-fem-0.1.9/src/torchfem/base.py`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/src/torchfem/data/plate_hole.vtk` & `torch-fem-0.1.9/src/torchfem/data/plate_hole.vtk`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/src/torchfem/data/tensile.vtu` & `torch-fem-0.1.9/src/torchfem/data/tensile.vtu`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/src/torchfem/elements.py` & `torch-fem-0.1.9/src/torchfem/elements.py`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/src/torchfem/homogenization.py` & `torch-fem-0.1.9/src/torchfem/homogenization.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,21 +331,21 @@
 
     C = torch.zeros(_C.shape[0], 6, 6)
     C[:, 0, 0] = _C[:, 0, 0, 0, 0]
     C[:, 0, 1] = _C[:, 0, 0, 1, 1]
     C[:, 0, 2] = _C[:, 0, 0, 2, 2]
     C[:, 1, 0] = _C[:, 1, 1, 0, 0]
     C[:, 1, 1] = _C[:, 1, 1, 1, 1]
-    C[:, 1, 2] = _C[:, 1, 1, 1, 1]
+    C[:, 1, 2] = _C[:, 1, 1, 2, 2]
     C[:, 2, 0] = _C[:, 2, 2, 0, 0]
     C[:, 2, 1] = _C[:, 2, 2, 1, 1]
     C[:, 2, 2] = _C[:, 2, 2, 2, 2]
-    C[:, 3, 3] = _C[:, 0, 1, 0, 1]
+    C[:, 3, 3] = _C[:, 1, 2, 1, 2]
     C[:, 4, 4] = _C[:, 0, 2, 0, 2]
-    C[:, 5, 5] = _C[:, 1, 2, 1, 2]
+    C[:, 5, 5] = _C[:, 0, 1, 0, 1]
     return C
 
 
 def tandon_weng_homogenization(
     matrix: Isotropic, fiber: Isotropic, a, volfrac
 ) -> Orthotropic:
     """Compute transversly isotropic material based on Tandon-Wengs's paper [1]. See
@@ -403,20 +403,15 @@
         -1 / (2 * c) * (1 - 2 * nu0 + 1 / b)
         + 1 / (2 * c) * (1 - 2 * nu0 + 3 / (2 * b)) * g
     )
     S[1, 2, 1, 2] = 1 / (4 * c) * (a**2 / (2 * b) + (1 - 2 * nu0 - 3 / (4 * b)) * g)
     S[0, 1, 0, 1] = (
         1
         / (4 * c)
-        * (
-            1
-            - 2 * nu0
-            - (a**2 + 1) / b
-            - 0.5 * (1 - 2 * nu0 - 3 * (a**2 + 1) / b) * g
-        )
+        * (1 - 2 * nu0 - (a**2 + 1) / b - 0.5 * (1 - 2 * nu0 - 3 * (a**2 + 1) / b) * g)
     )
     S[2, 2, 2, 2] = S[1, 1, 1, 1]
     S[2, 2, 1, 1] = S[1, 1, 2, 2]
     S[0, 0, 2, 2] = S[0, 0, 1, 1]
     S[2, 1, 2, 1] = S[1, 2, 1, 2]
     S[2, 2, 0, 0] = S[1, 1, 0, 0]
     S[0, 2, 0, 2] = S[0, 1, 0, 1]
```

### Comparing `torch-fem-0.1.8/src/torchfem/io.py` & `torch-fem-0.1.9/src/torchfem/io.py`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/src/torchfem/materials.py` & `torch-fem-0.1.9/src/torchfem/materials.py`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/src/torchfem/planar.py` & `torch-fem-0.1.9/src/torchfem/planar.py`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/src/torchfem/shell.py` & `torch-fem-0.1.9/src/torchfem/shell.py`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/src/torchfem/solid.py` & `torch-fem-0.1.9/src/torchfem/solid.py`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/src/torchfem/truss.py` & `torch-fem-0.1.9/src/torchfem/truss.py`

 * *Files identical despite different names*

### Comparing `torch-fem-0.1.8/tests/test_notebooks.py` & `torch-fem-0.1.9/tests/test_notebooks.py`

 * *Files identical despite different names*

