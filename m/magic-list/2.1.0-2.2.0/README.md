# Comparing `tmp/magic_list-2.1.0.tar.gz` & `tmp/magic_list-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic_list-2.1.0.tar", last modified: Sun Apr 21 18:32:26 2024, max compression
+gzip compressed data, was "magic_list-2.2.0.tar", last modified: Sun Apr 21 21:55:54 2024, max compression
```

## Comparing `magic_list-2.1.0.tar` & `magic_list-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 18:32:26.074646 magic_list-2.1.0/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2024-03-28 11:39:46.000000 magic_list-2.1.0/LICENSE
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3590 2024-04-21 18:32:26.071312 magic_list-2.1.0/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1309 2024-04-21 17:07:10.000000 magic_list-2.1.0/README.md
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 18:32:26.071312 magic_list-2.1.0/magic_list/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      362 2024-04-21 17:00:11.000000 magic_list-2.1.0/magic_list/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    27475 2024-04-21 17:00:11.000000 magic_list-2.1.0/magic_list/prelude.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     5149 2024-04-21 17:00:11.000000 magic_list-2.1.0/magic_list/prelude.pyi
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2024-03-27 16:41:35.000000 magic_list-2.1.0/magic_list/py.typed
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 18:32:26.071312 magic_list-2.1.0/magic_list.egg-info/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     3590 2024-04-21 18:32:26.000000 magic_list-2.1.0/magic_list.egg-info/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      289 2024-04-21 18:32:26.000000 magic_list-2.1.0/magic_list.egg-info/SOURCES.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2024-04-21 18:32:26.000000 magic_list-2.1.0/magic_list.egg-info/dependency_links.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       91 2024-04-21 18:32:26.000000 magic_list-2.1.0/magic_list.egg-info/requires.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       11 2024-04-21 18:32:26.000000 magic_list-2.1.0/magic_list.egg-info/top_level.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1012 2024-04-21 18:32:14.000000 magic_list-2.1.0/pyproject.toml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2024-04-21 18:32:26.074646 magic_list-2.1.0/setup.cfg
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 21:55:54.732601 magic_list-2.2.0/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2024-03-28 11:39:46.000000 magic_list-2.2.0/LICENSE
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4384 2024-04-21 21:55:54.732601 magic_list-2.2.0/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2100 2024-04-21 21:30:24.000000 magic_list-2.2.0/README.md
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 21:55:54.729268 magic_list-2.2.0/magic_list/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      362 2024-04-21 21:30:24.000000 magic_list-2.2.0/magic_list/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    27562 2024-04-21 21:48:23.000000 magic_list-2.2.0/magic_list/prelude.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     9486 2024-04-21 21:48:23.000000 magic_list-2.2.0/magic_list/prelude.pyi
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2024-03-27 16:41:35.000000 magic_list-2.2.0/magic_list/py.typed
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 21:55:54.729268 magic_list-2.2.0/magic_list.egg-info/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4384 2024-04-21 21:55:54.000000 magic_list-2.2.0/magic_list.egg-info/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      289 2024-04-21 21:55:54.000000 magic_list-2.2.0/magic_list.egg-info/SOURCES.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2024-04-21 21:55:54.000000 magic_list-2.2.0/magic_list.egg-info/dependency_links.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       94 2024-04-21 21:55:54.000000 magic_list-2.2.0/magic_list.egg-info/requires.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       11 2024-04-21 21:55:54.000000 magic_list-2.2.0/magic_list.egg-info/top_level.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1015 2024-04-21 21:55:30.000000 magic_list-2.2.0/pyproject.toml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2024-04-21 21:55:54.732601 magic_list-2.2.0/setup.cfg
```

### Comparing `magic_list-2.1.0/LICENSE` & `magic_list-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_list-2.1.0/PKG-INFO` & `magic_list-2.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-list
-Version: 2.1.0
+Version: 2.2.0
 Summary: Magic List is a module that extends the built-in list type.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,34 +38,82 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: build==1.2.*; extra == "dev"
 Requires-Dist: coverage==7.4.*; extra == "dev"
 Requires-Dist: pdoc==14.4.*; extra == "dev"
-Requires-Dist: pytest==7.4.*; extra == "dev"
+Requires-Dist: pytest<8.2,>=7.4; extra == "dev"
 Requires-Dist: pyright==1.1.*; extra == "dev"
 Requires-Dist: twine==5.0.*; extra == "dev"
 
-<!-- markdownlint-disable MD028 -->
+<!-- markdownlint-disable MD028, MD033 -->
 
 # Magic List
 
 [![Palestine support banner](https://raw.githubusercontent.com/Safouene1/support-palestine-banner/master/banner-support.svg)](https://irusa.org/middle-east/palestine/)
 
+[![PyPI badge](https://img.shields.io/pypi/v/magic-list)](<https://pypi.org/project/magic-list/>)
+[![Downloads](https://static.pepy.tech/badge/magic-list)](https://pepy.tech/project/magic-list)
+[![Tests](https://github.com/qexat/magic-list/actions/workflows/tests.yml/badge.svg)](https://github.com/qexat/magic-list/actions)
+[![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
+
 Magic List is a module that extends the built-in list type.
 
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
 > test coverage of 100%. It also provides typing stub files.
 
 ## Documentation
 
 Documentation can be found [here](https://qexat.github.io/magic-list/).
 
+## Installation
+
+### Pip
+
+```sh
+pip install magic-list
+```
+
+<details>
+<summary>Package managers</summary>
+
+### Conda
+
+```sh
+conda install magic-list
+```
+
+### Pipenv
+
+```sh
+pipenv install magic-list
+```
+
+### pipx
+
+```sh
+pipx install magic-list
+```
+
+### Poetry
+
+```sh
+poetry add magic-list
+```
+
+### uv
+
+```sh
+uv pip install magic-list
+```
+
+</details>
+
 ## Examples
 
 ### Fibonacci sequence
 
 In the functional programming spirit, let's write a function that given an integer `n`, returns the fibonacci sequence up to the `n`-th member.
 
 For example, `fibonacci_sequence(10)` would return `[0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55]`.
```

### Comparing `magic_list-2.1.0/magic_list/prelude.py` & `magic_list-2.2.0/magic_list/prelude.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     "list",
     "L",
 ]
 
 _T = typing.TypeVar("_T")
 _U = typing.TypeVar("_U")
 _V = typing.TypeVar("_V")
-_NumberT = typing.TypeVar("_NumberT", int, float, complex)
 
 
 class list(collections.UserList[_T]):
     """
     Mutable homogeneous sequence.
     Drop-in replacement for the built-in `list` type.
     """
@@ -513,15 +512,15 @@
         """
 
         if not self:
             raise TypeError("cannot perform summation on an empty list")
 
         return self.reduce(operator.add)
 
-    def mean(self: list[_NumberT]) -> _NumberT | float:
+    def mean(self: list[int] | list[float] | list[complex]) -> float | complex:
         """
         Return the mean of the list. The elements must be numbers.
 
         .. warning:: The list must contain numbers and be non-empty.
 
         >>> L[3, 5, 2].mean()
         3.3333333333333335
@@ -603,31 +602,31 @@
         returned_list = self.copy()
 
         for _ in range(n):
             returned_list.append(filler(returned_list) if callable(filler) else filler)
 
         return returned_list
 
-    def gap_fill(
+    def interleave(
         self,
         filler: _T | collections.abc.Callable[[_T, _T], _T],
     ) -> typing_extensions.Self:
         """
         Fill in-between the items with `filler` and return the result.
 
         If `filler` is a function, it takes the two items surrounding the gap
         that is about to be filled and produces a new value to be inserted.
 
         .. warning:: The list must be non-empty.
 
-        >>> L[3, 5, 2].gap_fill(0)
+        >>> L[3, 5, 2].interleave(0)
         [3, 0, 5, 0, 2]
-        >>> L[3, 5, 2].gap_fill(operator.add)
+        >>> L[3, 5, 2].interleave(operator.add)
         [3, 8, 5, 7, 2]
-        >>> list().gap_fill(0)
+        >>> list().interleave(0)
         *- ValueError: empty list has no gap to be filled -*
         """
 
         if not self:
             raise ValueError("empty list has no gap to be filled")
 
         returned_list = self.__class__([self.head])
@@ -636,14 +635,21 @@
             returned_list.append(
                 filler(self[i - 1], self[i]) if callable(filler) else filler,
             )
             returned_list.append(self[i])
 
         return returned_list
 
+    gap_fill = interleave
+    """
+    .. warning:: This alias is deprecated.
+
+    Alias of `interleave`.
+    """
+
     def select(
         self,
         indexes: collections.abc.Sequence[int],
     ) -> typing_extensions.Self:
         """
         Select items at provided indexes. If an index is present several
         times, this will be reflected in the resulting list.
```

### Comparing `magic_list-2.1.0/magic_list.egg-info/PKG-INFO` & `magic_list-2.2.0/magic_list.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-list
-Version: 2.1.0
+Version: 2.2.0
 Summary: Magic List is a module that extends the built-in list type.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,34 +38,82 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: build==1.2.*; extra == "dev"
 Requires-Dist: coverage==7.4.*; extra == "dev"
 Requires-Dist: pdoc==14.4.*; extra == "dev"
-Requires-Dist: pytest==7.4.*; extra == "dev"
+Requires-Dist: pytest<8.2,>=7.4; extra == "dev"
 Requires-Dist: pyright==1.1.*; extra == "dev"
 Requires-Dist: twine==5.0.*; extra == "dev"
 
-<!-- markdownlint-disable MD028 -->
+<!-- markdownlint-disable MD028, MD033 -->
 
 # Magic List
 
 [![Palestine support banner](https://raw.githubusercontent.com/Safouene1/support-palestine-banner/master/banner-support.svg)](https://irusa.org/middle-east/palestine/)
 
+[![PyPI badge](https://img.shields.io/pypi/v/magic-list)](<https://pypi.org/project/magic-list/>)
+[![Downloads](https://static.pepy.tech/badge/magic-list)](https://pepy.tech/project/magic-list)
+[![Tests](https://github.com/qexat/magic-list/actions/workflows/tests.yml/badge.svg)](https://github.com/qexat/magic-list/actions)
+[![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
+
 Magic List is a module that extends the built-in list type.
 
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
 > test coverage of 100%. It also provides typing stub files.
 
 ## Documentation
 
 Documentation can be found [here](https://qexat.github.io/magic-list/).
 
+## Installation
+
+### Pip
+
+```sh
+pip install magic-list
+```
+
+<details>
+<summary>Package managers</summary>
+
+### Conda
+
+```sh
+conda install magic-list
+```
+
+### Pipenv
+
+```sh
+pipenv install magic-list
+```
+
+### pipx
+
+```sh
+pipx install magic-list
+```
+
+### Poetry
+
+```sh
+poetry add magic-list
+```
+
+### uv
+
+```sh
+uv pip install magic-list
+```
+
+</details>
+
 ## Examples
 
 ### Fibonacci sequence
 
 In the functional programming spirit, let's write a function that given an integer `n`, returns the fibonacci sequence up to the `n`-th member.
 
 For example, `fibonacci_sequence(10)` would return `[0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55]`.
```

### Comparing `magic_list-2.1.0/pyproject.toml` & `magic_list-2.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "magic-list"
 description = "Magic List is a module that extends the built-in list type."
-version = "2.1.0"
+version = "2.2.0"
 keywords = ["collections", "list", "built-in", "extension"]
 
 authors = [{ name = "Qexat", email = "contact@qexat.com" }]
 
 requires-python = ">=3.9"
 
 readme = "README.md"
@@ -26,15 +26,15 @@
 repository = "https://github.com/qexat/magic-list"
 
 [project.optional-dependencies]
 dev = [
     "build==1.2.*",
     "coverage==7.4.*",
     "pdoc==14.4.*",
-    "pytest==7.4.*",
+    "pytest>=7.4,<8.2",
     "pyright==1.1.*",
     "twine==5.0.*",
 ]
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

