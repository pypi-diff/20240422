# Comparing `tmp/chainhashing-1.0.0.tar.gz` & `tmp/chainhashing-1.0.1.tar.gz`

## Comparing `chainhashing-1.0.0.tar` & `chainhashing-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chainhashing-1.0.0/src/chainhashing/__init__.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 chainhashing-1.0.0/src/chainhashing/hasharray.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 chainhashing-1.0.0/tests/test_haFunctions.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 chainhashing-1.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 chainhashing-1.0.0/LICENSE
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chainhashing-1.0.0/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 chainhashing-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 chainhashing-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chainhashing-1.0.1/src/chainhashing/__init__.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 chainhashing-1.0.1/src/chainhashing/hasharray.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 chainhashing-1.0.1/tests/test_haFunctions.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 chainhashing-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 chainhashing-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 chainhashing-1.0.1/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 chainhashing-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 chainhashing-1.0.1/PKG-INFO
```

### Comparing `chainhashing-1.0.0/src/chainhashing/hasharray.py` & `chainhashing-1.0.1/src/chainhashing/hasharray.py`

 * *Files identical despite different names*

### Comparing `chainhashing-1.0.0/tests/test_haFunctions.py` & `chainhashing-1.0.1/tests/test_haFunctions.py`

 * *Files identical despite different names*

### Comparing `chainhashing-1.0.0/LICENSE` & `chainhashing-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chainhashing-1.0.0/pyproject.toml` & `chainhashing-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chainhashing"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Ruxton", email="rt.kellar@gmail.com" },
 ]
-description = "A package for closed/open addressing hashing tables that require chaining with linked lists."
+description = "A package for closed addressing hash tables that require chaining with linked lists."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `chainhashing-1.0.0/PKG-INFO` & `chainhashing-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.3
 Name: chainhashing
-Version: 1.0.0
-Summary: A package for closed/open addressing hashing tables that require chaining with linked lists.
+Version: 1.0.1
+Summary: A package for closed addressing hash tables that require chaining with linked lists.
 Project-URL: Homepage, https://github.com/Ruxton07/chainhashing
 Project-URL: Issues, https://github.com/Ruxton07/chainhashing/issues
 Author-email: Ruxton <rt.kellar@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# Closed/Open Address Hashing (Chaining) with hasharray
+# Closed Address Hashing (Chaining) with hasharray
 
 ## Overview
 
 The hasharray package provides an implementation of closed address hashing (chaining) using a hash array data structure. Closed address hashing is a way of efficiently store and retrieve key-value pairs in a hash table.
 
 ## Features
 
 - Efficient storage and retrieval of key-value pairs using closed address hashing (chaining)
-- Support for a wide range of data types as keys and values
-- Toggling open addressing allowing automatic resizing of the hash array to maintain optimal performance
 - Collision resolution through chaining, where multiple key-value pairs with the same hash value are stored in a linked list
 
 ## Installation
 
 To use the hasharray package, you need to have Python installed. You can install the package using pip:
 
 ```
-pip install hasharray
-```
+pip install chainhashing
+```
+
+Then, simply type
+
+```
+import chainhashing
+```
+
+in your program and you're ready to go.
+
+Message from the creator: This was my first deployed python package (aside from my practice one on TestPyPI that had no real implementation). I know there are probably many issues with this and the documentation isn't nearly as good as it should be, but hopefully people looking to use this library still find use out of it! I've run many test and my conclusion is that there are no functionality errors with this library. Any advice/change recommendations are greatly appreciated; feel free to email me at rt.kellar@gmail.com or open an issue on the GitHub page for this library, https://github.com/Ruxton07/chainhashing. Enjoy!
```

