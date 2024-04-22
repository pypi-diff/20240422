# Comparing `tmp/chainhashing-0.0.2.tar.gz` & `tmp/chainhashing-1.0.0.tar.gz`

## Comparing `chainhashing-0.0.2.tar` & `chainhashing-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chainhashing-0.0.2/src/chainhashing/__init__.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 chainhashing-0.0.2/src/chainhashing/example.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 chainhashing-0.0.2/tests/test_func.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 chainhashing-0.0.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 chainhashing-0.0.2/LICENSE
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 chainhashing-0.0.2/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chainhashing-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 chainhashing-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chainhashing-1.0.0/src/chainhashing/__init__.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 chainhashing-1.0.0/src/chainhashing/hasharray.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 chainhashing-1.0.0/tests/test_haFunctions.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 chainhashing-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 chainhashing-1.0.0/LICENSE
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chainhashing-1.0.0/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 chainhashing-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 chainhashing-1.0.0/PKG-INFO
```

### Comparing `chainhashing-0.0.2/LICENSE` & `chainhashing-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainhashing-0.0.2/README.md` & `chainhashing-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Closed Address Hashing (Chaining) with HashArray
+# Closed/Open Address Hashing (Chaining) with hasharray
 
 ## Overview
 
 The hasharray package provides an implementation of closed address hashing (chaining) using a hash array data structure. Closed address hashing is a way of efficiently store and retrieve key-value pairs in a hash table.
 
 ## Features
```

### Comparing `chainhashing-0.0.2/pyproject.toml` & `chainhashing-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chainhashing"
-version = "0.0.2"
+version = "1.0.0"
 authors = [
   { name="Ruxton", email="rt.kellar@gmail.com" },
 ]
-description = "A package for closed addressing hashing tables that require chaining with link lists."
+description = "A package for closed/open addressing hashing tables that require chaining with linked lists."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `chainhashing-0.0.2/PKG-INFO` & `chainhashing-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: chainhashing
-Version: 0.0.2
-Summary: A package for closed addressing hashing tables that require chaining with link lists.
+Version: 1.0.0
+Summary: A package for closed/open addressing hashing tables that require chaining with linked lists.
 Project-URL: Homepage, https://github.com/Ruxton07/chainhashing
 Project-URL: Issues, https://github.com/Ruxton07/chainhashing/issues
 Author-email: Ruxton <rt.kellar@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# Closed Address Hashing (Chaining) with HashArray
+# Closed/Open Address Hashing (Chaining) with hasharray
 
 ## Overview
 
 The hasharray package provides an implementation of closed address hashing (chaining) using a hash array data structure. Closed address hashing is a way of efficiently store and retrieve key-value pairs in a hash table.
 
 ## Features
```

