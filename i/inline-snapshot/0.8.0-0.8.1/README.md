# Comparing `tmp/inline_snapshot-0.8.0.tar.gz` & `tmp/inline_snapshot-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inline_snapshot-0.8.0.tar", max compression
+gzip compressed data, was "inline_snapshot-0.8.1.tar", max compression
```

## Comparing `inline_snapshot-0.8.0.tar` & `inline_snapshot-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1082 2024-02-18 19:11:48.706993 inline_snapshot-0.8.0/LICENSE
--rw-r--r--   0        0        0     4300 2024-04-06 14:15:44.827781 inline_snapshot-0.8.0/README.md
--rw-r--r--   0        0        0      176 2024-04-09 10:01:42.306682 inline_snapshot-0.8.0/inline_snapshot/__init__.py
--rw-r--r--   0        0        0     1400 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_align.py
--rw-r--r--   0        0        0     5733 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_change.py
--rw-r--r--   0        0        0      539 2024-02-27 18:46:50.343219 inline_snapshot-0.8.0/inline_snapshot/_config.py
--rw-r--r--   0        0        0     4944 2024-02-27 18:46:50.343219 inline_snapshot-0.8.0/inline_snapshot/_external.py
--rw-r--r--   0        0        0     2779 2024-02-27 18:46:50.343219 inline_snapshot-0.8.0/inline_snapshot/_find_external.py
--rw-r--r--   0        0        0      372 2024-02-27 18:46:50.343219 inline_snapshot-0.8.0/inline_snapshot/_format.py
--rw-r--r--   0        0        0    21488 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_inline_snapshot.py
--rw-r--r--   0        0        0      452 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_location.py
--rw-r--r--   0        0        0     5911 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_rewrite_code.py
--rw-r--r--   0        0        0       64 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_sentinels.py
--rw-r--r--   0        0        0     3565 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_utils.py
--rw-r--r--   0        0        0        0 2024-02-27 18:46:50.343219 inline_snapshot-0.8.0/inline_snapshot/py.typed
--rw-r--r--   0        0        0     6477 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/pytest_plugin.py
--rw-r--r--   0        0        0     2618 2024-04-09 10:01:42.330682 inline_snapshot-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6169 1970-01-01 00:00:00.000000 inline_snapshot-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-02-18 19:11:48.706993 inline_snapshot-0.8.1/LICENSE
+-rw-r--r--   0        0        0     4642 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/README.md
+-rw-r--r--   0        0        0      176 2024-04-22 06:54:14.689618 inline_snapshot-0.8.1/inline_snapshot/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-09 10:01:00.849766 inline_snapshot-0.8.1/inline_snapshot/_align.py
+-rw-r--r--   0        0        0     5733 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/inline_snapshot/_change.py
+-rw-r--r--   0        0        0      539 2024-02-27 18:46:50.343219 inline_snapshot-0.8.1/inline_snapshot/_config.py
+-rw-r--r--   0        0        0     4944 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/inline_snapshot/_external.py
+-rw-r--r--   0        0        0     2779 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/inline_snapshot/_find_external.py
+-rw-r--r--   0        0        0      372 2024-02-27 18:46:50.343219 inline_snapshot-0.8.1/inline_snapshot/_format.py
+-rw-r--r--   0        0        0    21627 2024-04-22 06:53:50.245080 inline_snapshot-0.8.1/inline_snapshot/_inline_snapshot.py
+-rw-r--r--   0        0        0      452 2024-04-09 10:01:00.849766 inline_snapshot-0.8.1/inline_snapshot/_location.py
+-rw-r--r--   0        0        0     5911 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/inline_snapshot/_rewrite_code.py
+-rw-r--r--   0        0        0       64 2024-04-09 10:01:00.849766 inline_snapshot-0.8.1/inline_snapshot/_sentinels.py
+-rw-r--r--   0        0        0     3565 2024-04-09 10:01:00.849766 inline_snapshot-0.8.1/inline_snapshot/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-27 18:46:50.343219 inline_snapshot-0.8.1/inline_snapshot/py.typed
+-rw-r--r--   0        0        0     6477 2024-04-21 20:44:07.304452 inline_snapshot-0.8.1/inline_snapshot/pytest_plugin.py
+-rw-r--r--   0        0        0     2640 2024-04-22 06:54:14.713618 inline_snapshot-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 inline_snapshot-0.8.1/PKG-INFO
```

### Comparing `inline_snapshot-0.8.0/LICENSE` & `inline_snapshot-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.0/README.md` & `inline_snapshot-0.8.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -104,15 +104,27 @@
 
 <!-- -8<- [start:Feedback] -->
 ## Feedback
 
 inline-snapshot provides some advanced ways to work with snapshots.
 
 I would like to know how these features are used to further improve this small library.
-Let me know if you've found interesting use cases for this library via [twitter](https://twitter.com/15r10nk) or in the github [discussions](https://github.com/15r10nk/inline-snapshot/discussions/new?category=show-and-tell).
+Let me know if you've found interesting use cases for this library via [twitter](https://twitter.com/15r10nk), [fosstodon](https://fosstodon.org/deck/@15r10nk) or in the github [discussions](https://github.com/15r10nk/inline-snapshot/discussions/new?category=show-and-tell).
+
+## Sponsors
+
+I would like to thank my sponsors. Without them, I would not be able to invest so much time in my projects.
+
+### Bronze sponsor 🥉
+
+<p align="center">
+  <a href="https://pydantic.dev/">
+    <img src="docs/assets/sponsors/pydantic.png" alt="pydantic" width="300"/>
+  </a>
+</p>
 
 ## Issues
 
 If you encounter any problems, please [report an issue](https://github.com/15r10nk/inline-snapshot/issues) along with a detailed description.
 <!-- -8<- [end:Feedback] -->
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `inline_snapshot-0.8.0/inline_snapshot/_align.py` & `inline_snapshot-0.8.1/inline_snapshot/_align.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.0/inline_snapshot/_change.py` & `inline_snapshot-0.8.1/inline_snapshot/_change.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.0/inline_snapshot/_config.py` & `inline_snapshot-0.8.1/inline_snapshot/_config.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.0/inline_snapshot/_external.py` & `inline_snapshot-0.8.1/inline_snapshot/_external.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.0/inline_snapshot/_find_external.py` & `inline_snapshot-0.8.1/inline_snapshot/_find_external.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.0/inline_snapshot/_inline_snapshot.py` & `inline_snapshot-0.8.1/inline_snapshot/_inline_snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 import tokenize
 from collections import defaultdict
 from pathlib import Path
 from typing import Any
 from typing import Dict  # noqa
 from typing import Iterator
-from typing import overload
+from typing import Set
 from typing import Tuple  # noqa
 from typing import TypeVar
 
 from executing import Source
 
 from ._align import add_x
 from ._align import align
@@ -37,15 +37,15 @@
     pass
 
 
 snapshots = {}  # type: Dict[Tuple[int, int], Snapshot]
 
 _active = False
 
-_files_with_snapshots = set()
+_files_with_snapshots: Set[str] = set()
 
 
 class Flags:
     """
     fix: the value needs to be changed to pass the tests
     update: the value should be updated because the token-stream has changed
     create: the snapshot is empty `snapshot()`
@@ -624,24 +624,16 @@
 _T = TypeVar("_T")
 
 
 def repr_wrapper(func: _T) -> _T:
     return ReprWrapper(func)  # type: ignore
 
 
-@overload
-def snapshot() -> Any: ...
-
-
-@overload
-def snapshot(obj: T) -> T: ...
-
-
 @repr_wrapper
-def snapshot(obj=undefined):
+def snapshot(obj: Any = undefined) -> Any:
     """`snapshot()` is a placeholder for some value.
 
     `pytest --inline-snapshot=create` will create the value which matches your conditions.
 
     >>> assert 5 == snapshot()
     >>> assert 5 <= snapshot()
     >>> assert 5 >= snapshot()
@@ -659,29 +651,36 @@
         if obj is undefined:
             raise AssertionError(
                 "your snapshot is missing a value run pytest with --inline-snapshot=create"
             )
         else:
             return obj
 
-    frame = inspect.currentframe().f_back.f_back
+    frame = inspect.currentframe()
+    assert frame is not None
+    frame = frame.f_back
+    assert frame is not None
+    frame = frame.f_back
+    assert frame is not None
+
     expr = Source.executing(frame)
 
     module = inspect.getmodule(frame)
-    if module is not None:
+    if module is not None and module.__file__ is not None:
         _files_with_snapshots.add(module.__file__)
 
     key = id(frame.f_code), frame.f_lasti
 
     if key not in snapshots:
         node = expr.node
         if node is None:
             # we can run without knowing of the calling expression but we will not be able to fix code
             snapshots[key] = Snapshot(obj, None)
         else:
+            assert isinstance(node, ast.Call)
             assert isinstance(node.func, ast.Name)
             assert node.func.id == "snapshot"
             snapshots[key] = Snapshot(obj, expr)
         found_snapshots.append(snapshots[key])
 
     return snapshots[key]._value
```

### Comparing `inline_snapshot-0.8.0/inline_snapshot/_rewrite_code.py` & `inline_snapshot-0.8.1/inline_snapshot/_rewrite_code.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.0/inline_snapshot/_utils.py` & `inline_snapshot-0.8.1/inline_snapshot/_utils.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.0/inline_snapshot/pytest_plugin.py` & `inline_snapshot-0.8.1/inline_snapshot/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.8.0/pyproject.toml` & `inline_snapshot-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 ]
 description = "golden master/snapshot/approval testing library which puts the values right into your source code"
 keywords = ["pytest", "testing", "snapshot", "approval", "golden-master"]
 license = "MIT"
 name = "inline-snapshot"
 readme = "README.md"
 repository = "https://github.com/15r10nk/inline-snapshots"
-version = "0.8.0"
+version = "0.8.1"
 
 [tool.poetry.dependencies]
 asttokens = ">=2.0.5"
 black = ">=23.3.0"
 click = ">=8.1.4"
 executing = ">=2.0.0"
 python = ">=3.7"
@@ -62,14 +62,15 @@
 
 [tool.poetry.group.dev.dependencies]
 coverage = ">=7.2.3"
 coverage-enable-subprocess = ">=1.0"
 dirty-equals = ">=0.7.0"
 hypothesis = ">=6.75.5"
 mypy = ">=1.2.0"
+pyright = ">=1.1.359"
 pytest = ">=7.1"
 pytest-subtests = ">=0.11.0"
 pytest-xdist = {extras = ["psutil"], version = ">=3.2.1"}
 time-machine = ">=2.10.0"
 
 [tool.poetry.group.doc.dependencies]
 mkdocs = ">=1.4.2"
```

### Comparing `inline_snapshot-0.8.0/PKG-INFO` & `inline_snapshot-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inline-snapshot
-Version: 0.8.0
+Version: 0.8.1
 Summary: golden master/snapshot/approval testing library which puts the values right into your source code
 Home-page: https://github.com/15r10nk/inline-snapshots
 License: MIT
 Keywords: pytest,testing,snapshot,approval,golden-master
 Author: Frank Hoffmann
 Author-email: 15r10nk@polarbit.de
 Requires-Python: >=3.7
@@ -144,15 +144,27 @@
 
 <!-- -8<- [start:Feedback] -->
 ## Feedback
 
 inline-snapshot provides some advanced ways to work with snapshots.
 
 I would like to know how these features are used to further improve this small library.
-Let me know if you've found interesting use cases for this library via [twitter](https://twitter.com/15r10nk) or in the github [discussions](https://github.com/15r10nk/inline-snapshot/discussions/new?category=show-and-tell).
+Let me know if you've found interesting use cases for this library via [twitter](https://twitter.com/15r10nk), [fosstodon](https://fosstodon.org/deck/@15r10nk) or in the github [discussions](https://github.com/15r10nk/inline-snapshot/discussions/new?category=show-and-tell).
+
+## Sponsors
+
+I would like to thank my sponsors. Without them, I would not be able to invest so much time in my projects.
+
+### Bronze sponsor 🥉
+
+<p align="center">
+  <a href="https://pydantic.dev/">
+    <img src="docs/assets/sponsors/pydantic.png" alt="pydantic" width="300"/>
+  </a>
+</p>
 
 ## Issues
 
 If you encounter any problems, please [report an issue](https://github.com/15r10nk/inline-snapshot/issues) along with a detailed description.
 <!-- -8<- [end:Feedback] -->
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

