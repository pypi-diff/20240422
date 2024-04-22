# Comparing `tmp/ansi-string-1.0.0.tar.gz` & `tmp/ansi-string-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansi-string-1.0.0.tar", last modified: Sun Apr 21 19:18:06 2024, max compression
+gzip compressed data, was "ansi-string-1.0.1.tar", last modified: Sun Apr 21 22:02:49 2024, max compression
```

## Comparing `ansi-string-1.0.0.tar` & `ansi-string-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:18:06.539337 ansi-string-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 19:17:55.000000 ansi-string-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-21 19:17:55.000000 ansi-string-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-21 19:18:06.539337 ansi-string-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-21 19:17:55.000000 ansi-string-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 19:17:55.000000 ansi-string-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 19:18:06.539337 ansi-string-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-21 19:17:55.000000 ansi-string-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:18:06.535338 ansi-string-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:18:06.535338 ansi-string-1.0.0/src/ansi_string/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-21 19:17:55.000000 ansi-string-1.0.0/src/ansi_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71474 2024-04-21 19:17:55.000000 ansi-string-1.0.0/src/ansi_string/ansi_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:18:06.539337 ansi-string-1.0.0/src/ansi_string.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-21 19:18:06.000000 ansi-string-1.0.0/src/ansi_string.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-21 19:18:06.000000 ansi-string-1.0.0/src/ansi_string.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:18:06.000000 ansi-string-1.0.0/src/ansi_string.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 19:18:06.000000 ansi-string-1.0.0/src/ansi_string.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 19:18:06.000000 ansi-string-1.0.0/src/ansi_string.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:02:49.074780 ansi-string-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 22:02:42.000000 ansi-string-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-21 22:02:42.000000 ansi-string-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-21 22:02:49.074780 ansi-string-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-21 22:02:42.000000 ansi-string-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 22:02:42.000000 ansi-string-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 22:02:49.078780 ansi-string-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-21 22:02:42.000000 ansi-string-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:02:49.074780 ansi-string-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:02:49.074780 ansi-string-1.0.1/src/ansi_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-21 22:02:42.000000 ansi-string-1.0.1/src/ansi_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72102 2024-04-21 22:02:42.000000 ansi-string-1.0.1/src/ansi_string/ansi_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:02:49.074780 ansi-string-1.0.1/src/ansi_string.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-21 22:02:49.000000 ansi-string-1.0.1/src/ansi_string.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-21 22:02:49.000000 ansi-string-1.0.1/src/ansi_string.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:02:49.000000 ansi-string-1.0.1/src/ansi_string.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 22:02:49.000000 ansi-string-1.0.1/src/ansi_string.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 22:02:49.000000 ansi-string-1.0.1/src/ansi_string.egg-info/top_level.txt
```

### Comparing `ansi-string-1.0.0/LICENSE` & `ansi-string-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.0/setup.py` & `ansi-string-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.0/src/ansi_string/ansi_string.py` & `ansi-string-1.0.1/src/ansi_string/ansi_string.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import sys
 import re
 import math
 from enum import Enum, auto as enum_auto
 import io
 from typing import Any, Union, List, Dict, Tuple
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 PACKAGE_NAME = 'ansi-string'
 
 WHITESPACE_CHARS = ' \t\n\r\v\f'
 
 IS_WINDOWS = sys.platform.lower().startswith('win')
 
 if IS_WINDOWS:
@@ -1065,14 +1065,28 @@
         '''
         Apply formatting using a match object generated from re
         '''
         s = match_object.start(group)
         e = match_object.end(group)
         self.apply_formatting(setting_or_settings, s, e)
 
+    def format_matching(self, matchspec:str, *format, regex:bool=False, match_case=False):
+        '''
+        Apply formatting for anything matching the matchspec
+        matchspec: the string to match
+        format: 0 to many format specifiers
+        regex: set to True to treat matchspec as a regex string
+        match_case: set to True to make matching case-sensitive (false by default)
+        '''
+        if not regex:
+            matchspec = re.escape(matchspec)
+
+        for match in re.finditer(matchspec, self._s, re.IGNORECASE if not match_case else 0):
+            self.apply_formatting_for_match(format, match)
+
     def clear_formatting(self):
         '''
         Clears all internal formatting.
         '''
         self._fmts = {}
 
     @staticmethod
```

