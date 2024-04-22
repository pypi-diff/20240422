# Comparing `tmp/pure_utils-0.6.0.tar.gz` & `tmp/pure_utils-0.7.0.tar.gz`

## Comparing `pure_utils-0.6.0.tar` & `pure_utils-0.7.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 pure_utils-0.6.0/Makefile
--rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 pure_utils-0.6.0/.docs/Makefile
--rwxr-xr-x   0        0        0     1412 2020-02-02 00:00:00.000000 pure_utils-0.6.0/.docs/conf.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pure_utils-0.6.0/.docs/source/changelog.rst
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pure_utils-0.6.0/.docs/source/commands.rst
--rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 pure_utils-0.6.0/.docs/source/index.rst
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pure_utils-0.6.0/.docs/source/license.rst
--rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 pure_utils-0.6.0/.docs/source/refs/index.rst
--rwxr-xr-x   0        0        0     8643 2020-02-02 00:00:00.000000 pure_utils-0.6.0/.docs/templates/page.html
--rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 pure_utils-0.6.0/.docs/templates/autosummary/module.rst
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 pure_utils-0.6.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pure_utils-0.6.0/pure_utils/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pure_utils-0.6.0/pure_utils/common.py
--rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 pure_utils-0.6.0/pure_utils/containers.py
--rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 pure_utils-0.6.0/pure_utils/debug.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 pure_utils-0.6.0/pure_utils/profiler.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 pure_utils-0.6.0/pure_utils/strings.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 pure_utils-0.6.0/pure_utils/times.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pure_utils-0.6.0/pure_utils/_internal/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pure_utils-0.6.0/pure_utils/_internal/_profile_stats.py
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pure_utils-0.6.0/pure_utils/_internal/_profile_stats_serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pure_utils-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pure_utils-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pure_utils-0.6.0/tests/test_common.py
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 pure_utils-0.6.0/tests/test_containers.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 pure_utils-0.6.0/tests/test_debug.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pure_utils-0.6.0/tests/test_profiler.py
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 pure_utils-0.6.0/tests/test_strings.py
--rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 pure_utils-0.6.0/tests/test_times.py
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pure_utils-0.6.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pure_utils-0.6.0/LICENSE
--rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 pure_utils-0.6.0/README.md
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 pure_utils-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 pure_utils-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 pure_utils-0.7.0/Makefile
+-rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/Makefile
+-rwxr-xr-x   0        0        0     1412 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/conf.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/source/changelog.rst
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/source/commands.rst
+-rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/source/index.rst
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/source/license.rst
+-rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/source/refs/index.rst
+-rwxr-xr-x   0        0        0     8643 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/templates/page.html
+-rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/templates/autosummary/module.rst
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/common.py
+-rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/containers.py
+-rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/debug.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/profiler.py
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/repeaters.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/strings.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/times.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/_internal/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/_internal/_profile_stats.py
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/_internal/_profile_stats_serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_common.py
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_containers.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_debug.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_profiler.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_repeaters.py
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_strings.py
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_times.py
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pure_utils-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 pure_utils-0.7.0/README.md
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 pure_utils-0.7.0/PKG-INFO
```

### Comparing `pure_utils-0.6.0/Makefile` & `pure_utils-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/.docs/Makefile` & `pure_utils-0.7.0/.docs/Makefile`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/.docs/conf.py` & `pure_utils-0.7.0/.docs/conf.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/.docs/source/changelog.rst` & `pure_utils-0.7.0/.docs/source/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+v0.7.0 - [2024-04-22]
+---------------------
+* Add new module - ``repeaters`` (utilities for repeat functions).
+* Update development dependencies.
+
 v0.6.0 - [2024-03-01]
 ---------------------
 * Add ``unpack`` utility in ``containers`` module.
 * Add function synopsis in README short descriptions.
 * Fix examples in docstrings.
 * Fix tests for ``debug.caller``.
 * Fix ``containers`` function signatures.
```

### Comparing `pure_utils-0.6.0/.docs/source/commands.rst` & `pure_utils-0.7.0/.docs/source/commands.rst`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/.docs/source/index.rst` & `pure_utils-0.7.0/.docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/.docs/source/license.rst` & `pure_utils-0.7.0/.docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/.docs/templates/page.html` & `pure_utils-0.7.0/.docs/templates/page.html`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/.docs/templates/autosummary/module.rst` & `pure_utils-0.7.0/.docs/templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/.github/workflows/ci.yaml` & `pure_utils-0.7.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/pure_utils/common.py` & `pure_utils-0.7.0/pure_utils/common.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/pure_utils/containers.py` & `pure_utils-0.7.0/pure_utils/containers.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/pure_utils/debug.py` & `pure_utils-0.7.0/pure_utils/debug.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/pure_utils/profiler.py` & `pure_utils-0.7.0/pure_utils/profiler.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/pure_utils/strings.py` & `pure_utils-0.7.0/pure_utils/strings.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/pure_utils/times.py` & `pure_utils-0.7.0/pure_utils/times.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/pure_utils/_internal/_profile_stats.py` & `pure_utils-0.7.0/pure_utils/_internal/_profile_stats.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/pure_utils/_internal/_profile_stats_serializers.py` & `pure_utils-0.7.0/pure_utils/_internal/_profile_stats_serializers.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/tests/test_containers.py` & `pure_utils-0.7.0/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/tests/test_debug.py` & `pure_utils-0.7.0/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/tests/test_profiler.py` & `pure_utils-0.7.0/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/tests/test_strings.py` & `pure_utils-0.7.0/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/tests/test_times.py` & `pure_utils-0.7.0/tests/test_times.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/LICENSE` & `pure_utils-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_utils-0.6.0/README.md` & `pure_utils-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 * [debug](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html) - Utilities for debugging and development.
   * [around](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.around)(*[, before, after]) - Add additional behavior before and after execution of decorated function.
   * [caller](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.caller)(*[, at_frame]) - Get the name of calling function/method (from current function/method context).
   * [deltatime](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.deltatime)(*[, logger]) - Measure execution time of decorated function and print it to log.
   * [profileit](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.profileit)(*[, logger, stack_size]) - Profile decorated function being with 'cProfile'.
 * [profiler](https://p3t3rbr0.github.io/py3-pure-utils/refs/profiler.html) - Helper classes for working with the cProfile.
   * [Profiler](https://p3t3rbr0.github.io/py3-pure-utils/refs/profiler.html#profiler.Profiler) - A class provides a simple interface for profiling code.
+* [repeaters](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html) - Utilities for repeatedly execute custom logic.
+  * [Repeater](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.Repeater) - Base Repeater, implements a main logic, such as constructor and execute method.
+  * [ExceptionBasedRepeater](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.ExceptionBasedRepeater) - Repeater based on catching targeted exceptions.
+  * [PredicateBasedRepeater](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.PredicateBasedRepeater) - Repeater based on predicate function.
+  * [repeat](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.repeat)(repeater: Repeater) - Repeat wrapped function by `repeater` logic.
 * [strings](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html) - Utilities for working with strings.
   * [genstr](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.genstr)([length, is_uppercase]) - Generate ASCII-string with random letters.
   * [gunzip](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.gzip)(compressed_string, /) - Compress string (or bytes string) with gzip compression level.
   * [gzip](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.gunzip)(string, /, *[, level]) - Decompress bytes (earlier compressed with gzip) to string.
 * [times](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html) - Utilities for working with datetime objects.
   * [apply_tz](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.apply_tz)(dt[, tz]) - Apply timezone context to datetime object.
   * [iso2format](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.iso2format)(isostr, fmt, /) - Convert ISO-8601 datetime string into a string of specified format.
```

### Comparing `pure_utils-0.6.0/pyproject.toml` & `pure_utils-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.setuptools.packages.find]
 include = ["pure_utils*"]
 exclude = ["tests*"]
 
 [project]
 name = "pure-utils"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   {name="Peter Bro", email="p3t3rbr0@gmail.com"},
 ]
 description = "Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place ;)."
 keywords = ["utilities", "bicycle", "crutches"]
 readme = "README.md"
 requires-python = ">=3.10"
@@ -37,25 +37,25 @@
 Homepage = "https://github.com/p3t3rbr0/py3-pure-utils"
 Documentation = "https://p3t3rbr0.github.io/py3-pure-utils/"
 Repository = "https://github.com/p3t3rbr0/py3-pure-utils.git"
 Issues = "https://github.com/p3t3rbr0/py3-pure-utils/issues"
 Changelog = "https://github.com/p3t3rbr0/py3-pure-utils/blob/master/.docs/source/changelog.rst"
 
 [project.optional-dependencies]
-build = ["build==1.0.3", "twine==5.0.0"]
+build = ["build==1.2.1", "twine==5.0.0"]
 docs = ["Sphinx==7.2.6", "furo==2024.1.29"]
 dev = [
-    "mypy==1.8.0",
+    "mypy==1.9.0",
     "isort==5.13.2",
     "flake8==7.0.0",
-    "black==24.2.0",
+    "black==24.4.0",
     "pydocstyle==6.3.0",
-    "pytest==8.0.1",
-    "pytest-cov==4.1.0",
-    "pytest-mock==3.12.0",
+    "pytest==8.1.1",
+    "pytest-cov==5.0.0",
+    "pytest-mock==3.14.0",
 ]
 
 [tool.mypy]
 exclude = ["tests"]
 ignore_missing_imports = true
 
 [tool.isort]
```

### Comparing `pure_utils-0.6.0/PKG-INFO` & `pure_utils-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-utils
-Version: 0.6.0
+Version: 0.7.0
 Summary: Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place ;).
 Project-URL: Homepage, https://github.com/p3t3rbr0/py3-pure-utils
 Project-URL: Documentation, https://p3t3rbr0.github.io/py3-pure-utils/
 Project-URL: Repository, https://github.com/p3t3rbr0/py3-pure-utils.git
 Project-URL: Issues, https://github.com/p3t3rbr0/py3-pure-utils/issues
 Project-URL: Changelog, https://github.com/p3t3rbr0/py3-pure-utils/blob/master/.docs/source/changelog.rst
 Author-email: Peter Bro <p3t3rbr0@gmail.com>
@@ -19,25 +19,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Provides-Extra: build
-Requires-Dist: build==1.0.3; extra == 'build'
+Requires-Dist: build==1.2.1; extra == 'build'
 Requires-Dist: twine==5.0.0; extra == 'build'
 Provides-Extra: dev
-Requires-Dist: black==24.2.0; extra == 'dev'
+Requires-Dist: black==24.4.0; extra == 'dev'
 Requires-Dist: flake8==7.0.0; extra == 'dev'
 Requires-Dist: isort==5.13.2; extra == 'dev'
-Requires-Dist: mypy==1.8.0; extra == 'dev'
+Requires-Dist: mypy==1.9.0; extra == 'dev'
 Requires-Dist: pydocstyle==6.3.0; extra == 'dev'
-Requires-Dist: pytest-cov==4.1.0; extra == 'dev'
-Requires-Dist: pytest-mock==3.12.0; extra == 'dev'
-Requires-Dist: pytest==8.0.1; extra == 'dev'
+Requires-Dist: pytest-cov==5.0.0; extra == 'dev'
+Requires-Dist: pytest-mock==3.14.0; extra == 'dev'
+Requires-Dist: pytest==8.1.1; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo==2024.1.29; extra == 'docs'
 Requires-Dist: sphinx==7.2.6; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # pure-utils
 
@@ -76,14 +76,19 @@
 * [debug](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html) - Utilities for debugging and development.
   * [around](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.around)(*[, before, after]) - Add additional behavior before and after execution of decorated function.
   * [caller](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.caller)(*[, at_frame]) - Get the name of calling function/method (from current function/method context).
   * [deltatime](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.deltatime)(*[, logger]) - Measure execution time of decorated function and print it to log.
   * [profileit](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.profileit)(*[, logger, stack_size]) - Profile decorated function being with 'cProfile'.
 * [profiler](https://p3t3rbr0.github.io/py3-pure-utils/refs/profiler.html) - Helper classes for working with the cProfile.
   * [Profiler](https://p3t3rbr0.github.io/py3-pure-utils/refs/profiler.html#profiler.Profiler) - A class provides a simple interface for profiling code.
+* [repeaters](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html) - Utilities for repeatedly execute custom logic.
+  * [Repeater](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.Repeater) - Base Repeater, implements a main logic, such as constructor and execute method.
+  * [ExceptionBasedRepeater](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.ExceptionBasedRepeater) - Repeater based on catching targeted exceptions.
+  * [PredicateBasedRepeater](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.PredicateBasedRepeater) - Repeater based on predicate function.
+  * [repeat](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.repeat)(repeater: Repeater) - Repeat wrapped function by `repeater` logic.
 * [strings](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html) - Utilities for working with strings.
   * [genstr](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.genstr)([length, is_uppercase]) - Generate ASCII-string with random letters.
   * [gunzip](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.gzip)(compressed_string, /) - Compress string (or bytes string) with gzip compression level.
   * [gzip](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.gunzip)(string, /, *[, level]) - Decompress bytes (earlier compressed with gzip) to string.
 * [times](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html) - Utilities for working with datetime objects.
   * [apply_tz](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.apply_tz)(dt[, tz]) - Apply timezone context to datetime object.
   * [iso2format](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.iso2format)(isostr, fmt, /) - Convert ISO-8601 datetime string into a string of specified format.
```

