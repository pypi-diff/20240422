# Comparing `tmp/ropt_dakota-0.1.0.tar.gz` & `tmp/ropt_dakota-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt_dakota-0.1.0.tar", last modified: Fri Apr 19 13:21:11 2024, max compression
+gzip compressed data, was "ropt_dakota-0.1.1.tar", last modified: Mon Apr 22 06:57:04 2024, max compression
```

## Comparing `ropt_dakota-0.1.0.tar` & `ropt_dakota-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 13:21:11.616441 ropt_dakota-0.1.0/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 13:21:11.612441 ropt_dakota-0.1.0/.github/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 13:21:11.612441 ropt_dakota-0.1.0/.github/workflows/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      974 2024-04-19 12:39:55.000000 ropt_dakota-0.1.0/.github/workflows/static-checks.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      766 2024-04-19 13:16:05.000000 ropt_dakota-0.1.0/.github/workflows/tests.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       63 2024-04-19 12:37:21.000000 ropt_dakota-0.1.0/.gitignore
--rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     1322 2024-04-19 13:21:11.616441 ropt_dakota-0.1.0/PKG-INFO
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      480 2024-04-19 12:38:37.000000 ropt_dakota-0.1.0/README-PyPI.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      671 2024-04-19 12:36:23.000000 ropt_dakota-0.1.0/README.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1983 2024-04-19 13:16:05.000000 ropt_dakota-0.1.0/pyproject.toml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       38 2024-04-19 13:21:11.616441 ropt_dakota-0.1.0/setup.cfg
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 13:21:11.612441 ropt_dakota-0.1.0/src/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 13:21:11.612441 ropt_dakota-0.1.0/src/ropt_dakota/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       42 2024-04-19 12:40:07.000000 ropt_dakota-0.1.0/src/ropt_dakota/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    18308 2024-04-19 12:40:20.000000 ropt_dakota-0.1.0/src/ropt_dakota/dakota.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 12:33:56.000000 ropt_dakota-0.1.0/src/ropt_dakota/py.typed
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      411 2024-04-19 13:21:11.000000 ropt_dakota-0.1.0/src/ropt_dakota/version.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 13:21:11.616441 ropt_dakota-0.1.0/src/ropt_dakota.egg-info/
--rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     1322 2024-04-19 13:21:11.000000 ropt_dakota-0.1.0/src/ropt_dakota.egg-info/PKG-INFO
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      521 2024-04-19 13:21:11.000000 ropt_dakota-0.1.0/src/ropt_dakota.egg-info/SOURCES.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        1 2024-04-19 13:21:11.000000 ropt_dakota-0.1.0/src/ropt_dakota.egg-info/dependency_links.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       69 2024-04-19 13:21:11.000000 ropt_dakota-0.1.0/src/ropt_dakota.egg-info/entry_points.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       40 2024-04-19 13:21:11.000000 ropt_dakota-0.1.0/src/ropt_dakota.egg-info/requires.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       12 2024-04-19 13:21:11.000000 ropt_dakota-0.1.0/src/ropt_dakota.egg-info/top_level.txt
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 13:21:11.616441 ropt_dakota-0.1.0/tests/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 12:33:56.000000 ropt_dakota-0.1.0/tests/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2496 2024-04-19 12:40:23.000000 ropt_dakota-0.1.0/tests/conftest.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    12950 2024-04-19 12:41:17.000000 ropt_dakota-0.1.0/tests/test_dakota_backend.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.848228 ropt_dakota-0.1.1/
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.840228 ropt_dakota-0.1.1/.github/
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.844228 ropt_dakota-0.1.1/.github/workflows/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      974 2024-04-19 12:39:55.000000 ropt_dakota-0.1.1/.github/workflows/static-checks.yml
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      766 2024-04-19 13:16:05.000000 ropt_dakota-0.1.1/.github/workflows/tests.yml
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       63 2024-04-19 12:37:21.000000 ropt_dakota-0.1.1/.gitignore
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    35149 2024-04-19 14:26:30.000000 ropt_dakota-0.1.1/LICENSE
+-rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     1927 2024-04-22 06:57:04.844228 ropt_dakota-0.1.1/PKG-INFO
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1063 2024-04-22 06:56:12.000000 ropt_dakota-0.1.1/README.md
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1978 2024-04-22 06:52:17.000000 ropt_dakota-0.1.1/pyproject.toml
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       38 2024-04-22 06:57:04.848228 ropt_dakota-0.1.1/setup.cfg
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.840228 ropt_dakota-0.1.1/src/
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.844228 ropt_dakota-0.1.1/src/ropt_dakota/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       42 2024-04-19 12:40:07.000000 ropt_dakota-0.1.1/src/ropt_dakota/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    18308 2024-04-19 12:40:20.000000 ropt_dakota-0.1.1/src/ropt_dakota/dakota.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 12:33:56.000000 ropt_dakota-0.1.1/src/ropt_dakota/py.typed
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      411 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota/version.py
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.844228 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/
+-rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     1927 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/PKG-INFO
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      514 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/SOURCES.txt
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        1 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/dependency_links.txt
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       69 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/entry_points.txt
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       40 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/requires.txt
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       12 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/top_level.txt
+drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.844228 ropt_dakota-0.1.1/tests/
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 12:33:56.000000 ropt_dakota-0.1.1/tests/__init__.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2496 2024-04-19 12:40:23.000000 ropt_dakota-0.1.1/tests/conftest.py
+-rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    12950 2024-04-19 12:41:17.000000 ropt_dakota-0.1.1/tests/test_dakota_backend.py
```

### Comparing `ropt_dakota-0.1.0/.github/workflows/static-checks.yml` & `ropt_dakota-0.1.1/.github/workflows/static-checks.yml`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.1.0/.github/workflows/tests.yml` & `ropt_dakota-0.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.1.0/PKG-INFO` & `ropt_dakota-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,62 @@
 Metadata-Version: 2.1
 Name: ropt-dakota
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Dakota optimizer plugin for ropt
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: carolina
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 # A Dakota optimizer plugin for `ropt`
-This package installs a plugin for the `ropt` robust optimizer package, giving
-access to algorithms from the Dakota optimization package.
+This package installs a plugin for the `ropt` robust optimization package,
+providing access to algorithms from the Dakota optimization package.
+
+`ropt-dakota` is developed by the Netherlands Organisation for Applied
+Scientific Research (TNO). All files in this repository are released under the
+GNU General Public License v3.0 (a copy is provided in the LICENSE file).
 
 
 ## Dependencies
-This code has been tested with Python versions 3.8, 3.9, 3.10 and 3.11.
+This code has been tested with Python versions 3.8-3.12.
 
-The backend is based on the [Dakota](https://dakota.sandia.gov/) optimizer and
+The plugin is based on the [Dakota](https://dakota.sandia.gov/) optimizer and
 depends on the [Carolina](https://github.com/equinor/Carolina) Python wrapper.
 
 
 ## Installation
 ```bash
 pip install ropt-dakota
 ```
+
+
+## Development
+The `ropt-dakota` source distribution can be found on
+[GitHub](https://github.com/tno-ropt/ropt-dakota). To install from source, enter
+the `ropt` distribution directory and execute:
+
+```bash
+pip install .
+```
+
+## Running the tests
+To run the test suite, install the necessary dependencies and execute `pytest`:
+
+```bash
+pip install .[test]
+pytest
+```
```

### Comparing `ropt_dakota-0.1.0/pyproject.toml` & `ropt_dakota-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ropt-dakota"
 description = "A Dakota optimizer plugin for ropt"
-readme = "README-PyPI.md"
+readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `ropt_dakota-0.1.0/src/ropt_dakota/dakota.py` & `ropt_dakota-0.1.1/src/ropt_dakota/dakota.py`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.1.0/src/ropt_dakota.egg-info/PKG-INFO` & `ropt_dakota-0.1.1/src/ropt_dakota.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,62 @@
 Metadata-Version: 2.1
 Name: ropt-dakota
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Dakota optimizer plugin for ropt
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: carolina
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 # A Dakota optimizer plugin for `ropt`
-This package installs a plugin for the `ropt` robust optimizer package, giving
-access to algorithms from the Dakota optimization package.
+This package installs a plugin for the `ropt` robust optimization package,
+providing access to algorithms from the Dakota optimization package.
+
+`ropt-dakota` is developed by the Netherlands Organisation for Applied
+Scientific Research (TNO). All files in this repository are released under the
+GNU General Public License v3.0 (a copy is provided in the LICENSE file).
 
 
 ## Dependencies
-This code has been tested with Python versions 3.8, 3.9, 3.10 and 3.11.
+This code has been tested with Python versions 3.8-3.12.
 
-The backend is based on the [Dakota](https://dakota.sandia.gov/) optimizer and
+The plugin is based on the [Dakota](https://dakota.sandia.gov/) optimizer and
 depends on the [Carolina](https://github.com/equinor/Carolina) Python wrapper.
 
 
 ## Installation
 ```bash
 pip install ropt-dakota
 ```
+
+
+## Development
+The `ropt-dakota` source distribution can be found on
+[GitHub](https://github.com/tno-ropt/ropt-dakota). To install from source, enter
+the `ropt` distribution directory and execute:
+
+```bash
+pip install .
+```
+
+## Running the tests
+To run the test suite, install the necessary dependencies and execute `pytest`:
+
+```bash
+pip install .[test]
+pytest
+```
```

### Comparing `ropt_dakota-0.1.0/src/ropt_dakota.egg-info/SOURCES.txt` & `ropt_dakota-0.1.1/src/ropt_dakota.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .gitignore
-README-PyPI.md
+LICENSE
 README.md
 pyproject.toml
 .github/workflows/static-checks.yml
 .github/workflows/tests.yml
 src/ropt_dakota/__init__.py
 src/ropt_dakota/dakota.py
 src/ropt_dakota/py.typed
```

### Comparing `ropt_dakota-0.1.0/tests/conftest.py` & `ropt_dakota-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.1.0/tests/test_dakota_backend.py` & `ropt_dakota-0.1.1/tests/test_dakota_backend.py`

 * *Files identical despite different names*

