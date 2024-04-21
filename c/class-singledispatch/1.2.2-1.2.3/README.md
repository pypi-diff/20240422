# Comparing `tmp/class_singledispatch-1.2.2.tar.gz` & `tmp/class_singledispatch-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_singledispatch-1.2.2.tar", max compression
+gzip compressed data, was "class_singledispatch-1.2.3.tar", max compression
```

## Comparing `class_singledispatch-1.2.2.tar` & `class_singledispatch-1.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2024-04-21 12:28:16.699356 class_singledispatch-1.2.2/LICENSE
--rw-r--r--   0        0        0     5257 2024-04-21 12:28:16.699356 class_singledispatch-1.2.2/README.md
--rw-r--r--   0        0        0     5895 2024-04-21 12:28:16.699356 class_singledispatch-1.2.2/class_singledispatch/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 12:28:16.699356 class_singledispatch-1.2.2/class_singledispatch/py.typed
--rw-r--r--   0        0        0     5970 2024-04-21 12:28:16.699356 class_singledispatch-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     6425 1970-01-01 00:00:00.000000 class_singledispatch-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-21 12:36:09.963048 class_singledispatch-1.2.3/LICENSE
+-rw-r--r--   0        0        0     5257 2024-04-21 12:36:09.963048 class_singledispatch-1.2.3/README.md
+-rw-r--r--   0        0        0     5895 2024-04-21 12:36:09.963048 class_singledispatch-1.2.3/class_singledispatch/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 12:36:09.963048 class_singledispatch-1.2.3/class_singledispatch/py.typed
+-rw-r--r--   0        0        0     5929 2024-04-21 12:36:09.967048 class_singledispatch-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6406 1970-01-01 00:00:00.000000 class_singledispatch-1.2.3/PKG-INFO
```

### Comparing `class_singledispatch-1.2.2/LICENSE` & `class_singledispatch-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `class_singledispatch-1.2.2/README.md` & `class_singledispatch-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `class_singledispatch-1.2.2/class_singledispatch/__init__.py` & `class_singledispatch-1.2.3/class_singledispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `class_singledispatch-1.2.2/pyproject.toml` & `class_singledispatch-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was generated from skeleton-ci/skeleton-python@0.0.2rc-218-g8123b8a.
 # Instead of changing this particular file, you might want to alter the template:
 # https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a/project/pyproject.toml.jinja
 
 [tool.poetry]
 name = "class_singledispatch"
-version = "1.2.2"
+version = "1.2.3"
 description = "A ``singledispatch()`` for arguments that are classes annotated as specific types."
 authors = ["bswck <bartoszpiotrslawecki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "class_singledispatch/" }]
 homepage = "https://github.com/bswck/class_singledispatch"
 
@@ -16,17 +16,15 @@
 Documentation = "https://class-singledispatch.readthedocs.io/en/latest/"
 Issues = "https://github.com/bswck/class_singledispatch/issues"
 Distribution = "https://pypi.org/project/class-singledispatch/"
 Coverage = "https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/class_singledispatch"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-eval-type-backport = { version = ">=0.2.0", optional = true, extras = [
-    "modern-type-hints",
-] }
+eval-type-backport = { version = ">=0.2.0", optional = true }
 
 [tool.poetry.extras]
 modern-type-hints = ["eval-type-backport"]
 
 [tool.poetry.group.dev.dependencies]
 
 [tool.poetry.group.dev-skeleton.dependencies]
@@ -45,16 +43,14 @@
 pre-commit = "<3.6.0"
 smokeshow = ">=0.4.0"
 keyring = ">=25.0.0"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 
-
-
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 markdown-exec = ">=1.3.0"
 mkdocs-material = ">=8.2,<10.0.0"
 mkdocstrings = { version = ">=0.19.0", extras = ["python"] }
```

### Comparing `class_singledispatch-1.2.2/PKG-INFO` & `class_singledispatch-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: class_singledispatch
-Version: 1.2.2
+Version: 1.2.3
 Summary: A ``singledispatch()`` for arguments that are classes annotated as specific types.
 Home-page: https://github.com/bswck/class_singledispatch
 License: MIT
 Author: bswck
 Author-email: bartoszpiotrslawecki@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: modern-type-hints
-Requires-Dist: eval-type-backport[modern-type-hints] (>=0.2.0) ; extra == "modern-type-hints"
+Requires-Dist: eval-type-backport (>=0.2.0) ; extra == "modern-type-hints"
 Project-URL: Coverage, https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/class_singledispatch
 Project-URL: Documentation, https://class-singledispatch.readthedocs.io/en/latest/
 Project-URL: Distribution, https://pypi.org/project/class-singledispatch/
 Project-URL: Issues, https://github.com/bswck/class_singledispatch/issues
 Description-Content-Type: text/markdown
 
 # <div align="center">class_singledispatch<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–218–g8123b8a-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a) [![Supported Python versions](https://img.shields.io/pypi/pyversions/class-singledispatch.svg?logo=python&label=Python)](https://pypi.org/project/class-singledispatch/) [![Package version](https://img.shields.io/pypi/v/class-singledispatch?label=PyPI)](https://pypi.org/project/class-singledispatch/)</div>
```

