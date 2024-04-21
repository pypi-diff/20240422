# Comparing `tmp/robotcode_core-0.78.4.tar.gz` & `tmp/robotcode_core-0.79.0.tar.gz`

## Comparing `robotcode_core-0.78.4.tar` & `robotcode_core-0.79.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/__version__.py
--rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/async_tools.py
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/concurrent.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/documents_manager.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/event.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/filewatcher.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/language.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/py.typed
--rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/text_document.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/types.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/uri.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/lsp/__init__.py
--rw-r--r--   0        0        0   233360 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/lsp/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/__init__.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/caching.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/cli.py
--rw-r--r--   0        0        0    21972 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/dataclasses.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/debugpy.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/glob_path.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/inspect.py
--rw-r--r--   0        0        0    16387 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/logging.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/net.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/path.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/process.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/safe_eval.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/src/robotcode/core/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/LICENSE.txt
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/README.md
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/pyproject.toml
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 robotcode_core-0.78.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/__version__.py
+-rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/async_tools.py
+-rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/concurrent.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/documents_manager.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/event.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/filewatcher.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/language.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/py.typed
+-rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/text_document.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/types.py
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/uri.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/lsp/__init__.py
+-rw-r--r--   0        0        0   233360 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/lsp/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/__init__.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/caching.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/cli.py
+-rw-r--r--   0        0        0    21972 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/dataclasses.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/debugpy.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/glob_path.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/inspect.py
+-rw-r--r--   0        0        0    16387 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/logging.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/net.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/path.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/process.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/safe_eval.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/src/robotcode/core/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/LICENSE.txt
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/README.md
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/pyproject.toml
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 robotcode_core-0.79.0/PKG-INFO
```

### Comparing `robotcode_core-0.78.4/src/robotcode/core/async_tools.py` & `robotcode_core-0.79.0/src/robotcode/core/async_tools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/concurrent.py` & `robotcode_core-0.79.0/src/robotcode/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/documents_manager.py` & `robotcode_core-0.79.0/src/robotcode/core/documents_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/event.py` & `robotcode_core-0.79.0/src/robotcode/core/event.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/filewatcher.py` & `robotcode_core-0.79.0/src/robotcode/core/filewatcher.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/language.py` & `robotcode_core-0.79.0/src/robotcode/core/language.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/text_document.py` & `robotcode_core-0.79.0/src/robotcode/core/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/uri.py` & `robotcode_core-0.79.0/src/robotcode/core/uri.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import os
 import re
 from dataclasses import astuple, dataclass, fields
 from pathlib import Path
 from typing import Any, Iterator, Mapping, Optional, Union, overload
 from urllib import parse
 
+from .utils.path import normalized_path
+
 _IS_WIN = os.name == "nt"
 
 _RE_DRIVE_LETTER_PATH = re.compile(r"^\/[a-zA-Z]:")
 
 _DEFAULT_SCHEME = "file"
 
 
@@ -154,14 +156,18 @@
     def params(self) -> str:
         return self._parts.params
 
     @property
     def query(self) -> str:
         return self._parts.query
 
+    @property
+    def fragment(self) -> str:
+        return self._parts.fragment
+
     @staticmethod
     def from_path(path: Union[str, Path, os.PathLike[str]]) -> Uri:
         result = Uri(Path(path).as_uri())
 
         result._parts.path = parse.quote(parse.unquote(result._parts.path))
         return result
 
@@ -184,10 +190,30 @@
 
     def __iter__(self) -> Iterator[str]:
         for f in fields(self._parts):
             yield f.name
 
     def normalized(self) -> Uri:
         if self.scheme == "file":
-            return Uri.from_path(self.to_path().resolve())
+            return Uri.from_path(normalized_path(self.to_path()))
 
         return Uri(str(self))
+
+    def change(
+        self,
+        *,
+        scheme: Optional[str] = None,
+        netloc: Optional[str] = None,
+        path: Optional[str] = None,
+        params: Optional[str] = None,
+        query: Optional[str] = None,
+        fragment: Optional[str] = None,
+    ) -> Uri:
+
+        return Uri(
+            scheme=scheme if scheme is not None else self.scheme,
+            netloc=netloc if netloc is not None else self.netloc,
+            path=path if path is not None else self.path,
+            params=params if params is not None else self.params,
+            query=query if query is not None else self.query,
+            fragment=fragment if fragment is not None else self.fragment,
+        )
```

### Comparing `robotcode_core-0.78.4/src/robotcode/core/workspace.py` & `robotcode_core-0.79.0/src/robotcode/core/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/lsp/types.py` & `robotcode_core-0.79.0/src/robotcode/core/lsp/types.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/utils/caching.py` & `robotcode_core-0.79.0/src/robotcode/core/utils/caching.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/utils/dataclasses.py` & `robotcode_core-0.79.0/src/robotcode/core/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/utils/debugpy.py` & `robotcode_core-0.79.0/src/robotcode/core/utils/debugpy.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/utils/glob_path.py` & `robotcode_core-0.79.0/src/robotcode/core/utils/glob_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/utils/inspect.py` & `robotcode_core-0.79.0/src/robotcode/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/utils/logging.py` & `robotcode_core-0.79.0/src/robotcode/core/utils/logging.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/utils/net.py` & `robotcode_core-0.79.0/src/robotcode/core/utils/net.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/utils/process.py` & `robotcode_core-0.79.0/src/robotcode/core/utils/process.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/utils/safe_eval.py` & `robotcode_core-0.79.0/src/robotcode/core/utils/safe_eval.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/src/robotcode/core/utils/version.py` & `robotcode_core-0.79.0/src/robotcode/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/.gitignore` & `robotcode_core-0.79.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/LICENSE.txt` & `robotcode_core-0.79.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/README.md` & `robotcode_core-0.79.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/pyproject.toml` & `robotcode_core-0.79.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.78.4/PKG-INFO` & `robotcode_core-0.79.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-core
-Version: 0.78.4
+Version: 0.79.0
 Summary: Some core classes for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
```

