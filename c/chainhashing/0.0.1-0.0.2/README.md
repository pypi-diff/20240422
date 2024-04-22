# Comparing `tmp/chainhashing-0.0.1.tar.gz` & `tmp/chainhashing-0.0.2.tar.gz`

## Comparing `chainhashing-0.0.1.tar` & `chainhashing-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chainhashing-0.0.1/.venv/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chainhashing-0.0.1/src/chainhashing/__init__.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 chainhashing-0.0.1/src/chainhashing/example.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 chainhashing-0.0.1/tests/test_func.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 chainhashing-0.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 chainhashing-0.0.1/LICENSE
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 chainhashing-0.0.1/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chainhashing-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 chainhashing-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chainhashing-0.0.2/src/chainhashing/__init__.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 chainhashing-0.0.2/src/chainhashing/example.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 chainhashing-0.0.2/tests/test_func.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 chainhashing-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 chainhashing-0.0.2/LICENSE
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 chainhashing-0.0.2/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chainhashing-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 chainhashing-0.0.2/PKG-INFO
```

### Comparing `chainhashing-0.0.1/LICENSE` & `chainhashing-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chainhashing-0.0.1/pyproject.toml` & `chainhashing-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chainhashing"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ruxton", email="rt.kellar@gmail.com" },
 ]
 description = "A package for closed addressing hashing tables that require chaining with link lists."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

