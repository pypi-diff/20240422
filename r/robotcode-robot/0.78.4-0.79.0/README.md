# Comparing `tmp/robotcode_robot-0.78.4.tar.gz` & `tmp/robotcode_robot-0.79.0.tar.gz`

## Comparing `robotcode_robot-0.78.4.tar` & `robotcode_robot-0.79.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    88642 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/__init__.py
--rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/document_cache_helper.py
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/entities.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/errors.py
--rw-r--r--   0        0        0    56185 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    97035 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/library_doc.py
--rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/model_helper.py
--rw-r--r--   0        0        0    89792 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/namespace.py
--rw-r--r--   0        0        0    50086 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/namespace_analyzer.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/workspace_config.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/utils/__init__.py
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/utils/ast.py
--rw-r--r--   0        0        0    11621 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/utils/markdownformatter.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/utils/match.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/utils/robot_path.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/utils/stubs.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/utils/variables.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/src/robotcode/robot/utils/visitor.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/LICENSE.txt
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/README.md
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/pyproject.toml
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 robotcode_robot-0.78.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    88642 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/__init__.py
+-rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/document_cache_helper.py
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/entities.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/errors.py
+-rw-r--r--   0        0        0    56251 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    97124 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/model_helper.py
+-rw-r--r--   0        0        0    89792 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/namespace.py
+-rw-r--r--   0        0        0    50086 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/namespace_analyzer.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/workspace_config.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/utils/__init__.py
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/utils/ast.py
+-rw-r--r--   0        0        0    11621 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/utils/markdownformatter.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/utils/match.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/utils/robot_path.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/utils/stubs.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/utils/variables.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/src/robotcode/robot/utils/visitor.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/LICENSE.txt
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/README.md
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/pyproject.toml
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 robotcode_robot-0.79.0/PKG-INFO
```

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.79.0/src/robotcode/robot/config/loader.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/config/model.py` & `robotcode_robot-0.79.0/src/robotcode/robot/config/model.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.79.0/src/robotcode/robot/config/utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/document_cache_helper.py` & `robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/document_cache_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/entities.py` & `robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/errors.py` & `robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/errors.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/imports_manager.py` & `robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/imports_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from robotcode.core.lsp.types import DocumentUri, FileChangeType, FileEvent
 from robotcode.core.text_document import TextDocument
 from robotcode.core.uri import Uri
 from robotcode.core.utils.caching import SimpleLRUCache
 from robotcode.core.utils.dataclasses import as_json, from_json
 from robotcode.core.utils.glob_path import Pattern, iter_files
 from robotcode.core.utils.logging import LoggingDescriptor
-from robotcode.core.utils.path import path_is_relative_to
+from robotcode.core.utils.path import normalized_path, path_is_relative_to
 
 from ..__version__ import __version__
 from ..utils import get_robot_version, get_robot_version_str
 from ..utils.robot_path import find_file_ex
 from .entities import (
     CommandLineVariableDefinition,
     VariableDefinition,
@@ -179,29 +179,29 @@
 
                 path = uri.to_path()
                 if self._lib_doc is not None and (
                     (
                         self._lib_doc.module_spec is not None
                         and self._lib_doc.module_spec.submodule_search_locations is not None
                         and any(
-                            path_is_relative_to(path, Path(e).resolve())
+                            path_is_relative_to(path, normalized_path(Path(e)))
                             for e in self._lib_doc.module_spec.submodule_search_locations
                         )
                     )
                     or (
                         self._lib_doc.module_spec is not None
                         and self._lib_doc.module_spec.origin is not None
                         and path_is_relative_to(path, Path(self._lib_doc.module_spec.origin).parent)
                     )
                     or (self._lib_doc.source and path_is_relative_to(path, Path(self._lib_doc.source).parent))
                     or (
                         self._lib_doc.module_spec is None
                         and not self._lib_doc.source
                         and self._lib_doc.python_path
-                        and any(path_is_relative_to(path, Path(e).resolve()) for e in self._lib_doc.python_path)
+                        and any(path_is_relative_to(path, normalized_path(Path(e))) for e in self._lib_doc.python_path)
                     )
                 ):
                     self._invalidate()
 
                     return change.type
 
             return None
@@ -217,22 +217,22 @@
 
         # we are a module, so add the module path into file watchers
         if self._lib_doc.module_spec is not None and self._lib_doc.module_spec.submodule_search_locations is not None:
             self.file_watchers.append(
                 self.parent.file_watcher_manager.add_file_watchers(
                     self.parent.did_change_watched_files,
                     [
-                        str(Path(location).resolve().joinpath("**"))
+                        str(normalized_path(Path(location)).joinpath("**"))
                         for location in self._lib_doc.module_spec.submodule_search_locations
                     ],
                 )
             )
 
             if source_or_origin is not None and Path(source_or_origin).parent in [
-                Path(loc).resolve() for loc in self._lib_doc.module_spec.submodule_search_locations
+                normalized_path(Path(loc)) for loc in self._lib_doc.module_spec.submodule_search_locations
             ]:
                 return
 
         # we are a file, so put the parent path to filewatchers
         if source_or_origin is not None:
             self.file_watchers.append(
                 self.parent.file_watcher_manager.add_file_watchers(
@@ -303,15 +303,15 @@
                 uri = Uri(change.uri)
                 if uri.scheme != "file":
                     continue
 
                 path = uri.to_path()
                 if (
                     self._document is not None
-                    and (path.resolve() == self._document.uri.to_path().resolve())
+                    and (normalized_path(path) == normalized_path(self._document.uri.to_path()))
                     or self._document is None
                 ):
                     self._invalidate()
 
                     return change.type
 
             return None
@@ -1453,15 +1453,15 @@
         variables: Optional[Dict[str, Any]] = None,
     ) -> _ResourcesEntry:
         source = self.find_resource(name, base_dir, variables=variables)
 
         def _get_document() -> TextDocument:
             self._logger.debug(lambda: f"Load resource {name} from source {source}")
 
-            source_path = Path(source).resolve()
+            source_path = normalized_path(Path(source))
             extension = source_path.suffix
             if extension.lower() not in RESOURCE_EXTENSIONS:
                 raise ImportError(
                     f"Invalid resource file extension '{extension}'. "
                     f"Supported extensions are {', '.join(repr(s) for s in RESOURCE_EXTENSIONS)}."
                 )
```

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/library_doc.py` & `robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/library_doc.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 from robot.utils.importer import Importer
 from robot.utils.robotpath import find_file as robot_find_file
 from robot.variables import Variables
 from robot.variables.filesetter import PythonImporter, YamlImporter
 from robot.variables.finders import VariableFinder
 from robot.variables.search import contains_variable
 from robotcode.core.lsp.types import Position, Range
+from robotcode.core.utils.path import normalized_path
 from robotcode.robot.diagnostics.entities import (
     ArgumentDefinition,
     ImportedVariableDefinition,
     LibraryArgumentDefinition,
     NativeValue,
     SourceEntity,
     single_call,
@@ -1486,15 +1487,15 @@
 
 def _get_default_variables() -> Any:
 
     global __default_variables
     if __default_variables is None:
         __default_variables = Variables()
         for k, v in {
-            "${TEMPDIR}": str(Path(tempfile.gettempdir()).resolve()),
+            "${TEMPDIR}": str(normalized_path(Path(tempfile.gettempdir()))),
             "${/}": os.sep,
             "${:}": os.pathsep,
             "${\\n}": os.linesep,
             "${EMPTY}": "",
             "${SPACE}": " ",
             "${True}": True,
             "${False}": False,
@@ -2472,15 +2473,15 @@
             paths = [
                 Path(base_dir, name) if name else Path(base_dir),
                 *((Path(s) for s in sys.path) if not name else []),
                 *((Path(s, name) for s in sys.path) if name and not name.startswith(".") else []),
             ]
 
         for p in paths:
-            path = p.resolve()
+            path = normalized_path(p)
 
             if path.exists() and path.is_dir():
                 result += [
                     CompleteResult(
                         str(f.name),
                         CompleteResultKind.FILE if f.is_file() else CompleteResultKind.FOLDER,
                     )
@@ -2537,17 +2538,17 @@
 
     if name is None or not name.startswith(".") and not name.startswith("/") and not name.startswith(os.sep):
         result += list(iter_resources_from_python_path(name))
 
     if name is None or name.startswith((".", "/", os.sep)):
         name_path = Path(name if name else base_dir)
         if name_path.is_absolute():
-            path = name_path.resolve()
+            path = normalized_path(name_path)
         else:
-            path = Path(base_dir, name if name else base_dir).resolve()
+            path = normalized_path(Path(base_dir, name if name else base_dir))
 
         if path.exists() and (path.is_dir()):
             result += [
                 CompleteResult(
                     str(f.name),
                     CompleteResultKind.RESOURCE if f.is_file() else CompleteResultKind.FOLDER,
                 )
@@ -2588,15 +2589,15 @@
             paths = [
                 Path(base_dir, name) if name else Path(base_dir),
                 *((Path(s) for s in sys.path) if not name else []),
                 *((Path(s, name) for s in sys.path) if name and not name.startswith(".") else []),
             ]
 
         for p in paths:
-            path = p.resolve()
+            path = normalized_path(p)
 
             if path.exists() and path.is_dir():
                 result += [
                     CompleteResult(
                         str(f.name),
                         CompleteResultKind.FILE if f.is_file() else CompleteResultKind.FOLDER,
                     )
```

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/model_helper.py` & `robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/namespace.py` & `robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/namespace_analyzer.py` & `robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/namespace_analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/diagnostics/workspace_config.py` & `robotcode_robot-0.79.0/src/robotcode/robot/diagnostics/workspace_config.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/utils/ast.py` & `robotcode_robot-0.79.0/src/robotcode/robot/utils/ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/utils/markdownformatter.py` & `robotcode_robot-0.79.0/src/robotcode/robot/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/utils/match.py` & `robotcode_robot-0.79.0/src/robotcode/robot/utils/match.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/utils/robot_path.py` & `robotcode_robot-0.79.0/src/robotcode/robot/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/utils/stubs.py` & `robotcode_robot-0.79.0/src/robotcode/robot/utils/stubs.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/utils/variables.py` & `robotcode_robot-0.79.0/src/robotcode/robot/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/src/robotcode/robot/utils/visitor.py` & `robotcode_robot-0.79.0/src/robotcode/robot/utils/visitor.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/.gitignore` & `robotcode_robot-0.79.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/LICENSE.txt` & `robotcode_robot-0.79.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/README.md` & `robotcode_robot-0.79.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.78.4/pyproject.toml` & `robotcode_robot-0.79.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
   "platformdirs>=3.2.0,<4.2.0",
-  "robotcode-core==0.78.4",
+  "robotcode-core==0.79.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
```

### Comparing `robotcode_robot-0.78.4/PKG-INFO` & `robotcode_robot-0.79.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-robot
-Version: 0.78.4
+Version: 0.79.0
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: platformdirs<4.2.0,>=3.2.0
-Requires-Dist: robotcode-core==0.78.4
+Requires-Dist: robotcode-core==0.79.0
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```

