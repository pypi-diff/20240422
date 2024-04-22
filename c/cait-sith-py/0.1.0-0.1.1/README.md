# Comparing `tmp/cait_sith_py-0.1.0.tar.gz` & `tmp/cait_sith_py-0.1.1.tar.gz`

## Comparing `cait_sith_py-0.1.0.tar` & `cait_sith_py-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 cait_sith_py-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     2650 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     1884 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/.gitignore
--rw-r--r--   0     1001      127    11357 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/LICENSE
--rw-r--r--   0     1001      127     1572 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/src/action.rs
--rw-r--r--   0     1001      127     1995 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/src/arithmetic.rs
--rw-r--r--   0     1001      127     3158 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/src/keyshare.rs
--rw-r--r--   0     1001      127     1698 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     1551 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/src/participant.rs
--rw-r--r--   0     1001      127     4118 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/src/presign.rs
--rw-r--r--   0     1001      127     1728 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/src/protocol.rs
--rw-r--r--   0     1001      127     4020 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/src/sign.rs
--rw-r--r--   0     1001      127     4259 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/src/triples.rs
--rw-r--r--   0     1001      127    35142 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      923 2024-04-22 04:04:56.000000 cait_sith_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 cait_sith_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 cait_sith_py-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     2650 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     1890 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/.gitignore
+-rw-r--r--   0     1001      127    11357 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/LICENSE
+-rw-r--r--   0     1001      127     1572 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/src/action.rs
+-rw-r--r--   0     1001      127     1995 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/src/arithmetic.rs
+-rw-r--r--   0     1001      127     3158 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/src/keyshare.rs
+-rw-r--r--   0     1001      127     1698 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127     1551 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/src/participant.rs
+-rw-r--r--   0     1001      127     4118 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/src/presign.rs
+-rw-r--r--   0     1001      127     1728 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/src/protocol.rs
+-rw-r--r--   0     1001      127     4020 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/src/sign.rs
+-rw-r--r--   0     1001      127     4259 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/src/triples.rs
+-rw-r--r--   0     1001      127    35142 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127      923 2024-04-22 04:23:38.000000 cait_sith_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 cait_sith_py-0.1.1/PKG-INFO
```

### Comparing `cait_sith_py-0.1.0/.github/workflows/CI.yml` & `cait_sith_py-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/.gitignore` & `cait_sith_py-0.1.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 wheels/
 pip-wheel-metadata/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
+myenv
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `cait_sith_py-0.1.0/LICENSE` & `cait_sith_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/src/action.rs` & `cait_sith_py-0.1.1/src/action.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/src/arithmetic.rs` & `cait_sith_py-0.1.1/src/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/src/keyshare.rs` & `cait_sith_py-0.1.1/src/keyshare.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/src/lib.rs` & `cait_sith_py-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/src/participant.rs` & `cait_sith_py-0.1.1/src/participant.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/src/presign.rs` & `cait_sith_py-0.1.1/src/presign.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/src/protocol.rs` & `cait_sith_py-0.1.1/src/protocol.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/src/sign.rs` & `cait_sith_py-0.1.1/src/sign.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/src/triples.rs` & `cait_sith_py-0.1.1/src/triples.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/Cargo.lock` & `cait_sith_py-0.1.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.1.0/pyproject.toml` & `cait_sith_py-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cait_sith_py"
-version = "0.1.0"
+version = "0.1.1"
 description = "Cait Sith rust wrapper on python"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 maturin = "0.14.3"
@@ -19,15 +19,15 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 
 [project]
 name = "cait_sith_py"
-version = "0.1.0"
+version = "0.1.1"
 description = "Cait Sith rust wrapper on python"
 license = {file = "LICENSE"} # relative to the package/ directory
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
```

