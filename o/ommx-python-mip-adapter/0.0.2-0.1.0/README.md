# Comparing `tmp/ommx_python_mip_adapter-0.0.2.tar.gz` & `tmp/ommx_python_mip_adapter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ommx_python_mip_adapter-0.0.2.tar", last modified: Wed Apr 17 03:02:32 2024, max compression
+gzip compressed data, was "ommx_python_mip_adapter-0.1.0.tar", last modified: Mon Apr 22 06:27:48 2024, max compression
```

## Comparing `ommx_python_mip_adapter-0.0.2.tar` & `ommx_python_mip_adapter-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:02:32.512555 ommx_python_mip_adapter-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:02:32.504555 ommx_python_mip_adapter-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:02:32.508555 ommx_python_mip_adapter-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-17 03:02:26.000000 ommx_python_mip_adapter-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-17 03:02:26.000000 ommx_python_mip_adapter-0.0.2/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-17 03:02:26.000000 ommx_python_mip_adapter-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-04-17 03:02:26.000000 ommx_python_mip_adapter-0.0.2/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-17 03:02:26.000000 ommx_python_mip_adapter-0.0.2/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-17 03:02:32.512555 ommx_python_mip_adapter-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-17 03:02:26.000000 ommx_python_mip_adapter-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:02:32.508555 ommx_python_mip_adapter-0.0.2/ommx_python_mip_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:02:26.000000 ommx_python_mip_adapter-0.0.2/ommx_python_mip_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 03:02:32.000000 ommx_python_mip_adapter-0.0.2/ommx_python_mip_adapter/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 03:02:26.000000 ommx_python_mip_adapter-0.0.2/ommx_python_mip_adapter/ommx_to_python_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:02:32.508555 ommx_python_mip_adapter-0.0.2/ommx_python_mip_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-17 03:02:32.000000 ommx_python_mip_adapter-0.0.2/ommx_python_mip_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-17 03:02:32.000000 ommx_python_mip_adapter-0.0.2/ommx_python_mip_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 03:02:32.000000 ommx_python_mip_adapter-0.0.2/ommx_python_mip_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 03:02:32.000000 ommx_python_mip_adapter-0.0.2/ommx_python_mip_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 03:02:32.000000 ommx_python_mip_adapter-0.0.2/ommx_python_mip_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 03:02:26.000000 ommx_python_mip_adapter-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 03:02:32.512555 ommx_python_mip_adapter-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:02:32.508555 ommx_python_mip_adapter-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:02:26.000000 ommx_python_mip_adapter-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 03:02:26.000000 ommx_python_mip_adapter-0.0.2/tests/test_omm_to_python_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.794463 ommx_python_mip_adapter-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.786463 ommx_python_mip_adapter-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.790463 ommx_python_mip_adapter-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-22 06:27:48.794463 ommx_python_mip_adapter-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.786463 ommx_python_mip_adapter-0.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.790463 ommx_python_mip_adapter-0.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.790463 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.794463 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 06:27:48.000000 ommx_python_mip_adapter-0.1.0/ommx_python_mip_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 06:27:48.794463 ommx_python_mip_adapter-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:48.794463 ommx_python_mip_adapter-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-22 06:27:40.000000 ommx_python_mip_adapter-0.1.0/tests/test_integration.py
```

### Comparing `ommx_python_mip_adapter-0.0.2/.github/workflows/publish.yml` & `ommx_python_mip_adapter-0.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ommx_python_mip_adapter-0.0.2/.github/workflows/test_and_lint.yml` & `ommx_python_mip_adapter-0.1.0/.github/workflows/test_and_lint.yml`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
       - name: Install Dependencies
         run: |
           python -m pip install ".[dev]"
 
       - name: Run Tests
         run: |
-          python -m pytest
+          python -m pytest --doctest-modules -vv
 
   lint:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
@@ -46,9 +46,30 @@
 
       - name: Install Dependencies
         run: |
           python -m pip install ".[dev]"
 
       - name: Lint
         run: |
-          python -m mypy ./ommx_python_mip_adapter
           python -m pyright ./ommx_python_mip_adapter
+
+  markdown-code-runner:
+    runs-on: ubuntu-latest
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+    steps:
+      - uses: actions/checkout@v4
+
+      - name: Setup Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v5
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Install Dependencies
+        run: |
+          python -m pip install ".[dev]"
+
+      - name: Lint
+        run: |
+          markdown-code-runner --verbose README.md
```

### Comparing `ommx_python_mip_adapter-0.0.2/.gitignore` & `ommx_python_mip_adapter-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ommx_python_mip_adapter-0.0.2/LICENSE-APACHE` & `ommx_python_mip_adapter-0.1.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `ommx_python_mip_adapter-0.0.2/LICENSE-MIT` & `ommx_python_mip_adapter-0.1.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `ommx_python_mip_adapter-0.0.2/pyproject.toml` & `ommx_python_mip_adapter-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -14,23 +14,30 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
-    "ommx >= 0.1.0",
+    "ommx >= 0.1.1, < 0.2.0",
+    "mip",
 ]
 
 
 [project.optional-dependencies]
 dev = [
-    "pytest",
+    "markdown-code-runner",
     "mypy",
+    "numpy",
     "pyright",
+    "pytest",
+    "sphinx",
+    "sphinx_rtd_theme",
+    "sphinx_fontawesome",
+    "sphinx-autoapi",
 ]
 
 
 [project.urls]
 Repository = "https://github.com/Jij-Inc/ommx-python-mip-adapter"
 Issues = "https://github.com/Jij-Inc/ommx-python-mip-adapter/issues"
```

