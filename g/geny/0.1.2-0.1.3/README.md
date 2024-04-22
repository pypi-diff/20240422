# Comparing `tmp/geny-0.1.2.tar.gz` & `tmp/geny-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geny-0.1.2.tar", last modified: Thu Apr 18 01:15:48 2024, max compression
+gzip compressed data, was "geny-0.1.3.tar", last modified: Mon Apr 22 01:29:40 2024, max compression
```

## Comparing `geny-0.1.2.tar` & `geny-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.962913 geny-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-18 01:15:34.000000 geny-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-18 01:15:48.962913 geny-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-18 01:15:34.000000 geny-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.954913 geny-0.1.2/geny/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-18 01:15:34.000000 geny-0.1.2/geny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 01:15:34.000000 geny-0.1.2/geny/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2737 2024-04-18 01:15:34.000000 geny-0.1.2/geny/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/commands/destroy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/destroy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/destroy/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/destroy/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/destroy/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/commands/generate/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/generate/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/generate/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/generate/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/core/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/decorators/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/decorators/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/core/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.962913 geny-0.1.2/geny/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/templates/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/templates/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.962913 geny-0.1.2/geny/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 01:15:34.000000 geny-0.1.2/geny/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-18 01:15:34.000000 geny-0.1.2/geny/extensions/aliased.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 01:15:34.000000 geny-0.1.2/geny/extensions/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-18 01:15:34.000000 geny-0.1.2/geny/extensions/discoverable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.962913 geny-0.1.2/geny/template_files/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 01:15:34.000000 geny-0.1.2/geny/template_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.962913 geny-0.1.2/geny.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-18 01:15:34.000000 geny-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:15:48.962913 geny-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.731482 geny-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-22 01:29:27.000000 geny-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-22 01:29:40.731482 geny-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-22 01:29:27.000000 geny-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.723482 geny-0.1.3/geny/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-22 01:29:27.000000 geny-0.1.3/geny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.727482 geny-0.1.3/geny/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 01:29:27.000000 geny-0.1.3/geny/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2737 2024-04-22 01:29:27.000000 geny-0.1.3/geny/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.727482 geny-0.1.3/geny/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 01:29:27.000000 geny-0.1.3/geny/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-22 01:29:27.000000 geny-0.1.3/geny/commands/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.727482 geny-0.1.3/geny/commands/destroy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:27.000000 geny-0.1.3/geny/commands/destroy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-22 01:29:27.000000 geny-0.1.3/geny/commands/destroy/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-22 01:29:27.000000 geny-0.1.3/geny/commands/destroy/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-22 01:29:27.000000 geny-0.1.3/geny/commands/destroy/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.727482 geny-0.1.3/geny/commands/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-22 01:29:27.000000 geny-0.1.3/geny/commands/generate/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-22 01:29:27.000000 geny-0.1.3/geny/commands/generate/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-22 01:29:27.000000 geny-0.1.3/geny/commands/generate/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.727482 geny-0.1.3/geny/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.727482 geny-0.1.3/geny/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/decorators/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/decorators/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.731482 geny-0.1.3/geny/core/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/filesystem/directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/filesystem/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/filesystem/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/filesystem/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/filesystem/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/filesystem/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.731482 geny-0.1.3/geny/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/templates/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/templates/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-22 01:29:27.000000 geny-0.1.3/geny/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.731482 geny-0.1.3/geny/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 01:29:27.000000 geny-0.1.3/geny/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-22 01:29:27.000000 geny-0.1.3/geny/extensions/aliased.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-22 01:29:27.000000 geny-0.1.3/geny/extensions/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-22 01:29:27.000000 geny-0.1.3/geny/extensions/discoverable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.731482 geny-0.1.3/geny/template_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 01:29:27.000000 geny-0.1.3/geny/template_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:40.731482 geny-0.1.3/geny.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-22 01:29:40.000000 geny-0.1.3/geny.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-22 01:29:40.000000 geny-0.1.3/geny.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 01:29:40.000000 geny-0.1.3/geny.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-22 01:29:40.000000 geny-0.1.3/geny.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 01:29:40.000000 geny-0.1.3/geny.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 01:29:40.000000 geny-0.1.3/geny.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-22 01:29:27.000000 geny-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 01:29:40.731482 geny-0.1.3/setup.cfg
```

### Comparing `geny-0.1.2/LICENSE` & `geny-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/PKG-INFO` & `geny-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geny
-Version: 0.1.2
+Version: 0.1.3
 Summary: An extendable file generator
 Author-email: Leo Neto <leo@ekletik.com>
 Maintainer-email: Leo Neto <leo@ekletik.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Leo
```

### Comparing `geny-0.1.2/README.md` & `geny-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny/cli/cli.py` & `geny-0.1.3/geny/cli/cli.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny/commands/destroy/template.py` & `geny-0.1.3/geny/commands/destroy/template.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny/commands/generate/dockerfile.py` & `geny-0.1.3/geny/commands/generate/dockerfile.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny/commands/generate/template.py` & `geny-0.1.3/geny/commands/generate/template.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny/core/filesystem/directories.py` & `geny-0.1.3/geny/core/filesystem/directories.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny/core/filesystem/files.py` & `geny-0.1.3/geny/core/filesystem/files.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # core:filesystem
 from typing import Callable
 from pathlib import Path
 
 from geny.core.logger import logger
 from geny.core.templates.template import TemplateParser
 from geny.core.decorators.error_handler import halt_on_error
+from geny.core.filesystem.transformations import FileTransformation
 
 
 class File:
     def __init__(self, name: str, template: str = "", content="", context: dict = None):
         self.context = context if context is not None else {}
         self._name = name
         self._template = template
@@ -38,15 +39,15 @@
         return content
 
     def path(self, parent: Path = None) -> Path:
         value = Path(self.name) if parent is None else parent / self.name
         return value
 
     @halt_on_error
-    def create(self, parent: Path = None, after_hooks: list[Callable] = None, **kwargs):
+    def create(self, parent: Path = None, after_hooks: list[FileTransformation] = None, **kwargs):
         if after_hooks is None:
             after_hooks = []
 
         path = self.path(parent)
 
         if path.exists():
             if not kwargs.get('GENY_ENABLE_FORCE', False):
@@ -72,30 +73,32 @@
         path.touch(exist_ok=True)
 
         if contents != "":
             path.write_text(f"{contents}\n")
 
             logger.debug(f"Add contents to {path.absolute()}")
 
-            [hook(parent, **kwargs) for hook in after_hooks]
+            for hook in after_hooks:
+                hook.run()
 
     @halt_on_error
     def destroy(
-        self, parent: Path = None, after_hooks: list[Callable] = None, **kwargs
+        self, parent: Path = None, after_hooks: list[FileTransformation] = None, **kwargs
     ):
         if after_hooks is None:
             after_hooks = []
 
         path = self.path(parent)
 
         logger.info(f"delete: {path}")
 
         path.unlink(missing_ok=True)
 
-        [hook(parent, **kwargs) for hook in after_hooks]
+        for hook in after_hooks:
+            hook.run()
 
     def __str__(self) -> str:
         return self.name
 
     # Implements Sortable
 
     def __lt__(self, other):
```

### Comparing `geny-0.1.2/geny/core/filesystem/finder.py` & `geny-0.1.3/geny/core/filesystem/finder.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny/core/filesystem/transformations.py` & `geny-0.1.3/geny/core/filesystem/transformations.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,22 +16,31 @@
     def run(self):
         from_ = Path(self.file)
         to_ = Path(self.target)
         from_.rename(to_)
 
 
 class DeleteFile(FileTransformation):
-    def __init__(self, file: str):
-        self.file = file
+    def __init__(self, filename: str):
+        self.filename = filename
 
     def run(self):
-        file = Path(self.file)
+        file = Path(self.filename)
         file.unlink(missing_ok=True)
 
 
+class TouchFile(FileTransformation):
+    def __init__(self, filename: str):
+        self.filename = filename
+
+    def run(self):
+        file = Path(self.filename)
+        file.touch(exist_ok=True)
+
+
 class AddLineToFile(FileTransformation):
     def __init__(self, target: Path, statement: str, prevent_duplicates: bool = True):
         self.target = target
         self.statement = statement
         self.prevent_duplicates = prevent_duplicates
 
     def run(self):
```

### Comparing `geny-0.1.2/geny/core/templates/template.py` & `geny-0.1.3/geny/core/templates/template.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny/core/utils.py` & `geny-0.1.3/geny/core/utils.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny/extensions/aliased.py` & `geny-0.1.3/geny/extensions/aliased.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny/extensions/combined.py` & `geny-0.1.3/geny/extensions/combined.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny/extensions/discoverable.py` & `geny-0.1.3/geny/extensions/discoverable.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/geny.egg-info/PKG-INFO` & `geny-0.1.3/geny.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geny
-Version: 0.1.2
+Version: 0.1.3
 Summary: An extendable file generator
 Author-email: Leo Neto <leo@ekletik.com>
 Maintainer-email: Leo Neto <leo@ekletik.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Leo
```

### Comparing `geny-0.1.2/geny.egg-info/SOURCES.txt` & `geny-0.1.3/geny.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geny-0.1.2/pyproject.toml` & `geny-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "geny"
 description = "An extendable file generator"
 authors = [{ name = "Leo Neto", email = "leo@ekletik.com" }]
 maintainers = [{ name = "Leo Neto", email = "leo@ekletik.com" }]
 requires-python = ">=3.6"
 license = { file = "LICENSE" }
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 keywords = [
   "automation",
   "files",
   "generators",
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
```

