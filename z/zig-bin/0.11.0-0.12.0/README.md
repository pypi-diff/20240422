# Comparing `tmp/zig_bin-0.11.0.tar.gz` & `tmp/zig_bin-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zig_bin-0.11.0.tar", last modified: Thu Feb  1 06:21:44 2024, max compression
+gzip compressed data, was "zig_bin-0.12.0.tar", last modified: Mon Apr 22 05:24:29 2024, max compression
```

## Comparing `zig_bin-0.11.0.tar` & `zig_bin-0.12.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2024-02-01 06:21:37.778586 zig_bin-0.11.0/LICENSE
--rw-r--r--   0        0        0      347 2024-02-01 06:21:37.778586 zig_bin-0.11.0/README.md
--rw-r--r--   0        0        0     3221 2024-02-01 06:21:37.778586 zig_bin-0.11.0/pdm_build.py
--rw-r--r--   0        0        0     1198 2024-02-01 06:21:44.622634 zig_bin-0.11.0/pyproject.toml
--rw-r--r--   0        0        0      236 2024-02-01 06:21:37.778586 zig_bin-0.11.0/zig.py
--rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 zig_bin-0.11.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-22 05:24:25.960533 zig_bin-0.12.0/LICENSE
+-rw-r--r--   0        0        0      347 2024-04-22 05:24:25.960533 zig_bin-0.12.0/README.md
+-rw-r--r--   0        0        0     3221 2024-04-22 05:24:25.960533 zig_bin-0.12.0/pdm_build.py
+-rw-r--r--   0        0        0     1198 2024-04-22 05:24:29.040535 zig_bin-0.12.0/pyproject.toml
+-rw-r--r--   0        0        0      236 2024-04-22 05:24:25.960533 zig_bin-0.12.0/zig.py
+-rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 zig_bin-0.12.0/PKG-INFO
```

### Comparing `zig_bin-0.11.0/LICENSE` & `zig_bin-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zig_bin-0.11.0/pdm_build.py` & `zig_bin-0.12.0/pdm_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import requests
 from wheel.cli.tags import tags
 
 if TYPE_CHECKING:
     from pdm.backend.hooks import Context
 
 NAME = "zig"
-VERSION = "0.11.0"
+VERSION = "0.12.0"
 
 ZIG_VERSION_INFO_URL = "https://ziglang.org/download/index.json"
 ZIG_PYTHON_PLATFORMS = {
     # windows
     "x86_64-windows": "win_amd64",
     "aarch64-windows": "win_arm64",
     "x86-windows": "win32",
```

### Comparing `zig_bin-0.11.0/pyproject.toml` & `zig_bin-0.12.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "zig-bin"
 description = "Zig is a general-purpose programming language and toolchain for maintaining robust, optimal, and reusable software."
-version = "0.11.0"
+version = "0.12.0"
 authors = [
     { name = "dowon", email = "ks2515@naver.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
```

### Comparing `zig_bin-0.11.0/PKG-INFO` & `zig_bin-0.12.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zig-bin
-Version: 0.11.0
+Version: 0.12.0
 Summary: Zig is a general-purpose programming language and toolchain for maintaining robust, optimal, and reusable software.
 Keywords: zig
 Author-Email: dowon <ks2515@naver.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Other
 Project-URL: Repository, https://github.com/Bing-su/pip-binary-factory
```

