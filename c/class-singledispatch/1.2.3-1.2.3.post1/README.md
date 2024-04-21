# Comparing `tmp/class_singledispatch-1.2.3.tar.gz` & `tmp/class_singledispatch-1.2.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_singledispatch-1.2.3.tar", max compression
+gzip compressed data, was "class_singledispatch-1.2.3.post1.tar", max compression
```

## Comparing `class_singledispatch-1.2.3.tar` & `class_singledispatch-1.2.3.post1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2024-04-21 12:36:09.963048 class_singledispatch-1.2.3/LICENSE
--rw-r--r--   0        0        0     5257 2024-04-21 12:36:09.963048 class_singledispatch-1.2.3/README.md
--rw-r--r--   0        0        0     5895 2024-04-21 12:36:09.963048 class_singledispatch-1.2.3/class_singledispatch/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 12:36:09.963048 class_singledispatch-1.2.3/class_singledispatch/py.typed
--rw-r--r--   0        0        0     5929 2024-04-21 12:36:09.967048 class_singledispatch-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     6406 1970-01-01 00:00:00.000000 class_singledispatch-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-21 22:57:29.875497 class_singledispatch-1.2.3.post1/LICENSE
+-rw-r--r--   0        0        0     5257 2024-04-21 22:57:29.875497 class_singledispatch-1.2.3.post1/README.md
+-rw-r--r--   0        0        0     5965 2024-04-21 22:57:29.875497 class_singledispatch-1.2.3.post1/class_singledispatch/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:57:29.875497 class_singledispatch-1.2.3.post1/class_singledispatch/py.typed
+-rw-r--r--   0        0        0     5943 2024-04-21 22:57:29.875497 class_singledispatch-1.2.3.post1/pyproject.toml
+-rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 class_singledispatch-1.2.3.post1/PKG-INFO
```

### Comparing `class_singledispatch-1.2.3/LICENSE` & `class_singledispatch-1.2.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `class_singledispatch-1.2.3/README.md` & `class_singledispatch-1.2.3.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# <div align="center">class_singledispatch<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–218–g8123b8a-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a) [![Supported Python versions](https://img.shields.io/pypi/pyversions/class-singledispatch.svg?logo=python&label=Python)](https://pypi.org/project/class-singledispatch/) [![Package version](https://img.shields.io/pypi/v/class-singledispatch?label=PyPI)](https://pypi.org/project/class-singledispatch/)</div>
+# <div align="center">class_singledispatch<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–224–ge16504a-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-224-ge16504a) [![Supported Python versions](https://img.shields.io/pypi/pyversions/class-singledispatch.svg?logo=python&label=Python)](https://pypi.org/project/class-singledispatch/) [![Package version](https://img.shields.io/pypi/v/class-singledispatch?label=PyPI)](https://pypi.org/project/class-singledispatch/)</div>
 
 [![Tests](https://github.com/bswck/class_singledispatch/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/class_singledispatch/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/class_singledispatch.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/class_singledispatch)
 [![Documentation Status](https://readthedocs.org/projects/class-singledispatch/badge/?version=latest)](https://class-singledispatch.readthedocs.io/en/latest/?badge=latest)
 
 A [``singledispatch()``](https://docs.python.org/3/library/functools.html#functools.singledispatch) for arguments that are classes annotated as specific types.
 
@@ -66,17 +66,17 @@
 ```
 
 ## For Contributors
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 <!--
-This section was generated from skeleton-ci/skeleton-python@0.0.2rc-218-g8123b8a.
+This section was generated from skeleton-ci/skeleton-python@0.0.2rc-224-ge16504a.
 Instead of changing this particular file, you might want to alter the template:
-https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a/project/README.md.jinja
+https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-224-ge16504a/project/README.md.jinja
 -->
 > [!Note]
 > If you use Windows, it is highly recommended to complete the installation in the way presented below through [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).
 1.  Fork the [class_singledispatch repository](https://github.com/bswck/class_singledispatch) on GitHub.
 
 1.  [Install Poetry](https://python-poetry.org/docs/#installation).<br/>
     Poetry is an amazing tool for managing dependencies & virtual environments, building packages and publishing them.
```

### Comparing `class_singledispatch-1.2.3/class_singledispatch/__init__.py` & `class_singledispatch-1.2.3.post1/class_singledispatch/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,15 +140,16 @@
         cls: type[Any] | Callable[..., _R],
         /,
         func: Callable[_P, _R] | None = None,
     ) -> Callable[_P, _R] | partial[Callable[_P, _R]]:
         """
         Register a new function as a dispatcher for `cls`.
 
-        For usage guide, please see the [`class_singledispatch`][class_singledispatch]
+        For usage guide, please see the
+        [`class_singledispatch`][class_singledispatch.class_singledispatch]
         documentation.
         """
         if isinstance(cls, type):
             if func is None:
                 return partial(self.register, cls)
         else:
             if func is not None:
@@ -171,20 +172,21 @@
 
 
 def class_singledispatch(
     func: Callable[..., _R],
     /,
 ) -> _ClassSingleDispatchCallable[_R]:
     """
-    Use [`functools.singledispatch`][functools.singledispatch] to singledispatch
+    Use [`functools.singledispatch`][functools.singledispatch] to dispatch
     classes as parameters.
 
     While `singledispatch` examines the class of the first user argument,
-    [class_singledispatch][] uses the first argument as the class itself and performs
-    the same task with it as `singledispatch`.
+    [`class_singledispatch`][class_singledispatch.class_singledispatch] uses
+    the first argument as the class itself and performs the same task with it
+    as `singledispatch`.
 
     ```python
     class T:
         pass
 
     class OtherT:
         pass
```

### Comparing `class_singledispatch-1.2.3/pyproject.toml` & `class_singledispatch-1.2.3.post1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# This file was generated from skeleton-ci/skeleton-python@0.0.2rc-218-g8123b8a.
+# This file was generated from skeleton-ci/skeleton-python@0.0.2rc-224-ge16504a.
 # Instead of changing this particular file, you might want to alter the template:
-# https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a/project/pyproject.toml.jinja
+# https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-224-ge16504a/project/pyproject.toml.jinja
 
 [tool.poetry]
 name = "class_singledispatch"
-version = "1.2.3"
+version = "1.2.3.post1"
 description = "A ``singledispatch()`` for arguments that are classes annotated as specific types."
 authors = ["bswck <bartoszpiotrslawecki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "class_singledispatch/" }]
 homepage = "https://github.com/bswck/class_singledispatch"
 
@@ -24,17 +24,17 @@
 
 [tool.poetry.extras]
 modern-type-hints = ["eval-type-backport"]
 
 [tool.poetry.group.dev.dependencies]
 
 [tool.poetry.group.dev-skeleton.dependencies]
-# This dependency group was generated from skeleton-ci/skeleton-python@0.0.2rc-218-g8123b8a.
+# This dependency group was generated from skeleton-ci/skeleton-python@0.0.2rc-224-ge16504a.
 # Instead of changing this particular file, you might want to alter the template:
-# https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a/project/pyproject.toml.jinja
+# https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-224-ge16504a/project/pyproject.toml.jinja
 mypy = ">=1.9.0"
 ruff = ">=0.3.4"
 towncrier = ">=23.11.0"
 coverage = ">=7.4.4"
 pytest = ">=8.1.1"
 pytest-doctestplus = ">=1.2.1"
 pytest-sugar = ">=1.0.0"
@@ -43,27 +43,31 @@
 pre-commit = "<3.6.0"
 smokeshow = ">=0.4.0"
 keyring = ">=25.0.0"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 
+
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 markdown-exec = ">=1.3.0"
 mkdocs-material = ">=8.2,<10.0.0"
 mkdocstrings = { version = ">=0.19.0", extras = ["python"] }
 
 [tool.poe.tasks]
 test = "pytest -v"
 lint = "ruff check ."
-skeleton = "scripts/skeleton.0.0.2rc-218-g8123b8a.bash"
-check = [{ ref = "test" }, { ref = "lint" }]
+skeleton = "scripts/skeleton.0.0.2rc-224-ge16504a.bash"
+check = [
+    { ref="test" },
+    { ref="lint" },
+]
 release.script = "scripts.release:main"
 
 [tool.poe.tasks.added]
 shell = "towncrier create $TICKET.added.md --edit"
 args = [{ name = "TICKET", default = "+", positional = true }]
 
 [tool.poe.tasks.changed]
```

### Comparing `class_singledispatch-1.2.3/PKG-INFO` & `class_singledispatch-1.2.3.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: class_singledispatch
-Version: 1.2.3
+Version: 1.2.3.post1
 Summary: A ``singledispatch()`` for arguments that are classes annotated as specific types.
 Home-page: https://github.com/bswck/class_singledispatch
 License: MIT
 Author: bswck
 Author-email: bartoszpiotrslawecki@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Requires-Dist: eval-type-backport (>=0.2.0) ; extra == "modern-type-hints"
 Project-URL: Coverage, https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/class_singledispatch
 Project-URL: Documentation, https://class-singledispatch.readthedocs.io/en/latest/
 Project-URL: Distribution, https://pypi.org/project/class-singledispatch/
 Project-URL: Issues, https://github.com/bswck/class_singledispatch/issues
 Description-Content-Type: text/markdown
 
-# <div align="center">class_singledispatch<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–218–g8123b8a-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a) [![Supported Python versions](https://img.shields.io/pypi/pyversions/class-singledispatch.svg?logo=python&label=Python)](https://pypi.org/project/class-singledispatch/) [![Package version](https://img.shields.io/pypi/v/class-singledispatch?label=PyPI)](https://pypi.org/project/class-singledispatch/)</div>
+# <div align="center">class_singledispatch<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–224–ge16504a-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-224-ge16504a) [![Supported Python versions](https://img.shields.io/pypi/pyversions/class-singledispatch.svg?logo=python&label=Python)](https://pypi.org/project/class-singledispatch/) [![Package version](https://img.shields.io/pypi/v/class-singledispatch?label=PyPI)](https://pypi.org/project/class-singledispatch/)</div>
 
 [![Tests](https://github.com/bswck/class_singledispatch/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/class_singledispatch/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/class_singledispatch.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/class_singledispatch)
 [![Documentation Status](https://readthedocs.org/projects/class-singledispatch/badge/?version=latest)](https://class-singledispatch.readthedocs.io/en/latest/?badge=latest)
 
 A [``singledispatch()``](https://docs.python.org/3/library/functools.html#functools.singledispatch) for arguments that are classes annotated as specific types.
 
@@ -90,17 +90,17 @@
 ```
 
 ## For Contributors
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 <!--
-This section was generated from skeleton-ci/skeleton-python@0.0.2rc-218-g8123b8a.
+This section was generated from skeleton-ci/skeleton-python@0.0.2rc-224-ge16504a.
 Instead of changing this particular file, you might want to alter the template:
-https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-218-g8123b8a/project/README.md.jinja
+https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-224-ge16504a/project/README.md.jinja
 -->
 > [!Note]
 > If you use Windows, it is highly recommended to complete the installation in the way presented below through [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).
 1.  Fork the [class_singledispatch repository](https://github.com/bswck/class_singledispatch) on GitHub.
 
 1.  [Install Poetry](https://python-poetry.org/docs/#installation).<br/>
     Poetry is an amazing tool for managing dependencies & virtual environments, building packages and publishing them.
```

