# Comparing `tmp/ommx-0.1.0.tar.gz` & `tmp/ommx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ommx-0.1.0.tar", last modified: Tue Apr  9 07:59:20 2024, max compression
+gzip compressed data, was "ommx-0.1.1.tar", last modified: Mon Apr 22 01:32:30 2024, max compression
```

## Comparing `ommx-0.1.0.tar` & `ommx-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:20.870624 ommx-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 07:59:15.000000 ommx-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-09 07:59:20.870624 ommx-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-09 07:59:15.000000 ommx-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:20.866624 ommx-0.1.0/ommx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:20.870624 ommx-0.1.0/ommx/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/constraint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/constraint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/decision_variables_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/decision_variables_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/function_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/instance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/instance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/linear_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/linear_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/polynomial_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/polynomial_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/quadratic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/quadratic_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/solution_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/solution_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-09 07:59:15.000000 ommx-0.1.0/ommx/v1/sparse_matrix_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:59:20.870624 ommx-0.1.0/ommx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-09 07:59:20.000000 ommx-0.1.0/ommx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 07:59:20.000000 ommx-0.1.0/ommx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:59:20.000000 ommx-0.1.0/ommx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-09 07:59:20.000000 ommx-0.1.0/ommx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 07:59:20.000000 ommx-0.1.0/ommx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 07:59:15.000000 ommx-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:59:20.870624 ommx-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:30.541496 ommx-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 01:32:24.000000 ommx-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-22 01:32:30.541496 ommx-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-22 01:32:24.000000 ommx-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:30.537496 ommx-0.1.1/ommx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:30.541496 ommx-0.1.1/ommx/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/constraint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/constraint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/decision_variables_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/decision_variables_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/function_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/instance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/instance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/linear_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/linear_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/polynomial_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/polynomial_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/quadratic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/quadratic_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/solution_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/solution_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/sparse_matrix_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:30.541496 ommx-0.1.1/ommx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-22 01:32:30.000000 ommx-0.1.1/ommx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-22 01:32:30.000000 ommx-0.1.1/ommx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 01:32:30.000000 ommx-0.1.1/ommx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 01:32:30.000000 ommx-0.1.1/ommx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 01:32:30.000000 ommx-0.1.1/ommx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-22 01:32:24.000000 ommx-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 01:32:30.541496 ommx-0.1.1/setup.cfg
```

### Comparing `ommx-0.1.0/PKG-INFO` & `ommx-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ommx
-Version: 0.1.0
+Version: 0.1.1
 Summary: Open Mathematical prograMming eXchange (OMMX)
 Author-email: "Jij Inc." <info@j-ij.com>
 Project-URL: Homepage, https://github.com/Jij-Inc/ommx
 Project-URL: Issues, https://github.com/Jij-Inc/ommx/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: numpy<2.0.0,>=1.23.0
 Requires-Dist: protobuf<6.0.0,>=5.26.1
 Provides-Extra: dev
 Requires-Dist: mypy>=0.910; extra == "dev"
 Requires-Dist: mypy-protobuf; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
@@ -35,14 +36,16 @@
 
 # API Reference
 
 - [Protobuf](https://jij-inc.github.io/ommx/protobuf.html)
 - [Rust](https://jij-inc.github.io/ommx/rust/ommx/index.html)
 - [Python](https://jij-inc.github.io/ommx/python/index.html)
 
+See [DEVELOPMENT.md](./DEVELOPMENT.md) about developing this project.
+
 # Compatibility
 
 This project manages several versions as follows:
 
 ## Protocol buffers schema
 
 - OMMX defines a protocol buffers schema with version like `v1`, `v2`, etc. `v1` schema has a namesapce `ommx.v1`.
@@ -61,7 +64,11 @@
 - Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or <https://www.apache.org/licenses/LICENSE-2.0>)
 - MIT license ([LICENSE-MIT](LICENSE-MIT) or <https://opensource.org/licenses/MIT>)
 
 at your option.
 
 # Contribution
 TBW
+
+# Acknowledgement
+![BRIDGE](./BRIDGE.png)
+This work was performed for Council for Science, Technology and Innovation (CSTI), Cross-ministerial Strategic Innovation Promotion Program (SIP), “Promoting the application of advanced quantum technology platforms to social issues”(Funding agency : QST).
```

### Comparing `ommx-0.1.0/README.md` & `ommx-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 # API Reference
 
 - [Protobuf](https://jij-inc.github.io/ommx/protobuf.html)
 - [Rust](https://jij-inc.github.io/ommx/rust/ommx/index.html)
 - [Python](https://jij-inc.github.io/ommx/python/index.html)
 
+See [DEVELOPMENT.md](./DEVELOPMENT.md) about developing this project.
+
 # Compatibility
 
 This project manages several versions as follows:
 
 ## Protocol buffers schema
 
 - OMMX defines a protocol buffers schema with version like `v1`, `v2`, etc. `v1` schema has a namesapce `ommx.v1`.
@@ -32,7 +34,11 @@
 - Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or <https://www.apache.org/licenses/LICENSE-2.0>)
 - MIT license ([LICENSE-MIT](LICENSE-MIT) or <https://opensource.org/licenses/MIT>)
 
 at your option.
 
 # Contribution
 TBW
+
+# Acknowledgement
+![BRIDGE](./BRIDGE.png)
+This work was performed for Council for Science, Technology and Innovation (CSTI), Cross-ministerial Strategic Innovation Promotion Program (SIP), “Promoting the application of advanced quantum technology platforms to social issues”(Funding agency : QST).
```

### Comparing `ommx-0.1.0/ommx/v1/constraint_pb2.py` & `ommx-0.1.1/ommx/v1/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/constraint_pb2.pyi` & `ommx-0.1.1/ommx/v1/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/decision_variables_pb2.py` & `ommx-0.1.1/ommx/v1/decision_variables_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/decision_variables_pb2.pyi` & `ommx-0.1.1/ommx/v1/decision_variables_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/function_pb2.py` & `ommx-0.1.1/ommx/v1/function_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/function_pb2.pyi` & `ommx-0.1.1/ommx/v1/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/instance_pb2.py` & `ommx-0.1.1/ommx/v1/instance_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/instance_pb2.pyi` & `ommx-0.1.1/ommx/v1/instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/linear_pb2.py` & `ommx-0.1.1/ommx/v1/linear_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/linear_pb2.pyi` & `ommx-0.1.1/ommx/v1/linear_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/polynomial_pb2.py` & `ommx-0.1.1/ommx/v1/polynomial_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/polynomial_pb2.pyi` & `ommx-0.1.1/ommx/v1/polynomial_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/quadratic_pb2.py` & `ommx-0.1.1/ommx/v1/quadratic_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/quadratic_pb2.pyi` & `ommx-0.1.1/ommx/v1/quadratic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/solution_pb2.py` & `ommx-0.1.1/ommx/v1/solution_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/solution_pb2.pyi` & `ommx-0.1.1/ommx/v1/solution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx/v1/sparse_matrix_pb2.py` & `ommx-0.1.1/ommx/v1/sparse_matrix_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.0/ommx.egg-info/PKG-INFO` & `ommx-0.1.1/ommx.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ommx
-Version: 0.1.0
+Version: 0.1.1
 Summary: Open Mathematical prograMming eXchange (OMMX)
 Author-email: "Jij Inc." <info@j-ij.com>
 Project-URL: Homepage, https://github.com/Jij-Inc/ommx
 Project-URL: Issues, https://github.com/Jij-Inc/ommx/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: numpy<2.0.0,>=1.23.0
 Requires-Dist: protobuf<6.0.0,>=5.26.1
 Provides-Extra: dev
 Requires-Dist: mypy>=0.910; extra == "dev"
 Requires-Dist: mypy-protobuf; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
@@ -35,14 +36,16 @@
 
 # API Reference
 
 - [Protobuf](https://jij-inc.github.io/ommx/protobuf.html)
 - [Rust](https://jij-inc.github.io/ommx/rust/ommx/index.html)
 - [Python](https://jij-inc.github.io/ommx/python/index.html)
 
+See [DEVELOPMENT.md](./DEVELOPMENT.md) about developing this project.
+
 # Compatibility
 
 This project manages several versions as follows:
 
 ## Protocol buffers schema
 
 - OMMX defines a protocol buffers schema with version like `v1`, `v2`, etc. `v1` schema has a namesapce `ommx.v1`.
@@ -61,7 +64,11 @@
 - Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or <https://www.apache.org/licenses/LICENSE-2.0>)
 - MIT license ([LICENSE-MIT](LICENSE-MIT) or <https://opensource.org/licenses/MIT>)
 
 at your option.
 
 # Contribution
 TBW
+
+# Acknowledgement
+![BRIDGE](./BRIDGE.png)
+This work was performed for Council for Science, Technology and Innovation (CSTI), Cross-ministerial Strategic Innovation Promotion Program (SIP), “Promoting the application of advanced quantum technology platforms to social issues”(Funding agency : QST).
```

### Comparing `ommx-0.1.0/ommx.egg-info/SOURCES.txt` & `ommx-0.1.1/ommx.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 README.md
 pyproject.toml
 ommx/__init__.py
+ommx/testing.py
 ommx.egg-info/PKG-INFO
 ommx.egg-info/SOURCES.txt
 ommx.egg-info/dependency_links.txt
 ommx.egg-info/requires.txt
 ommx.egg-info/top_level.txt
 ommx/v1/__init__.py
 ommx/v1/constraint_pb2.py
```

### Comparing `ommx-0.1.0/pyproject.toml` & `ommx-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ommx"
-version = "0.1.0"
+version = "0.1.1"
 description = "Open Mathematical prograMming eXchange (OMMX)"
 authors = [
     { name="Jij Inc.", email="info@j-ij.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -14,14 +14,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
+    "numpy>=1.23.0, <2.0.0",
     "protobuf>=5.26.1, <6.0.0",
 ]
 
 
 [project.optional-dependencies]
 dev = [
     "mypy>=0.910",
```

