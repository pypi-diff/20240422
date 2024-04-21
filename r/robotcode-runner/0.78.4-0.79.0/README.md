# Comparing `tmp/robotcode_runner-0.78.4.tar.gz` & `tmp/robotcode_runner-0.79.0.tar.gz`

## Comparing `robotcode_runner-0.78.4.tar` & `robotcode_runner-0.79.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    29901 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/README.md
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/pyproject.toml
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 robotcode_runner-0.78.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    29976 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/README.md
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/pyproject.toml
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/PKG-INFO
```

### Comparing `robotcode_runner-0.78.4/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.79.0/src/robotcode/runner/cli/libdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.78.4/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.79.0/src/robotcode/runner/cli/rebot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.78.4/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.79.0/src/robotcode/runner/cli/robot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.78.4/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.79.0/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.78.4/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.79.0/src/robotcode/runner/cli/discover/discover.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     DocumentUri,
     Position,
     Range,
 )
 from robotcode.core.uri import Uri
 from robotcode.core.utils.cli import show_hidden_arguments
 from robotcode.core.utils.dataclasses import from_json
+from robotcode.core.utils.path import normalized_path
 from robotcode.plugin import (
     Application,
     OutputFormat,
     UnknownError,
     pass_application,
 )
 from robotcode.plugin.click_helper.types import add_options
@@ -269,15 +270,15 @@
                 )
                 + f"Multiple suites with name '{suite.name}' in suite '{suite.parent.longname}'."
             )
 
         self._collected[-1][suite.name] = True
         self._collected.append(NormalizedDict(ignore="_"))
         try:
-            absolute_path = Path(suite.source).resolve() if suite.source else None
+            absolute_path = normalized_path(Path(suite.source)) if suite.source else None
             item = TestItem(
                 type="suite",
                 id=f"{absolute_path or ''};{suite.longname}",
                 name=suite.name,
                 longname=suite.longname,
                 uri=str(Uri.from_path(absolute_path)) if absolute_path else None,
                 source=str(suite.source),
@@ -324,15 +325,15 @@
                 f"'{test.parent.longname}'."
             )
         self._collected[-1][test.name] = True
 
         if self._current.children is None:
             self._current.children = []
         try:
-            absolute_path = Path(test.source).resolve() if test.source is not None else None
+            absolute_path = normalized_path(Path(test.source)) if test.source is not None else None
             item = TestItem(
                 type="test",
                 id=f"{absolute_path or ''};{test.longname};{test.lineno}",
                 name=test.name,
                 longname=test.longname,
                 uri=str(Uri.from_path(absolute_path)) if absolute_path else None,
                 source=str(test.source),
@@ -413,15 +414,15 @@
 
     def add_diagnostic(
         message: Message,
         source_uri: Optional[str] = None,
         line: Optional[int] = None,
         text: Optional[str] = None,
     ) -> None:
-        source_uri = str(Uri.from_path(Path(source_uri).resolve() if source_uri else Path.cwd()))
+        source_uri = str(Uri.from_path(normalized_path(Path(source_uri)) if source_uri else Path.cwd()))
 
         if source_uri not in result:
             result[source_uri] = []
 
         result[source_uri].append(
             Diagnostic(
                 range=Range(
```

### Comparing `robotcode_runner-0.78.4/.gitignore` & `robotcode_runner-0.79.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.78.4/LICENSE.txt` & `robotcode_runner-0.79.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.78.4/README.md` & `robotcode_runner-0.79.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.78.4/pyproject.toml` & `robotcode_runner-0.79.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -24,18 +24,18 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.78.4",
-  "robotcode-modifiers==0.78.4",
-  "robotcode-plugin==0.78.4",
-  "robotcode==0.78.4",
+  "robotcode-robot==0.79.0",
+  "robotcode-modifiers==0.79.0",
+  "robotcode-plugin==0.79.0",
+  "robotcode==0.79.0",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.78.4/PKG-INFO` & `robotcode_runner-0.79.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-runner
-Version: 0.78.4
+Version: 0.79.0
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,18 +21,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.78.4
-Requires-Dist: robotcode-plugin==0.78.4
-Requires-Dist: robotcode-robot==0.78.4
-Requires-Dist: robotcode==0.78.4
+Requires-Dist: robotcode-modifiers==0.79.0
+Requires-Dist: robotcode-plugin==0.79.0
+Requires-Dist: robotcode-robot==0.79.0
+Requires-Dist: robotcode==0.79.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

