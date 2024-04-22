# Comparing `tmp/magic_list-2.2.0.tar.gz` & `tmp/magic_list-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magic_list-2.2.0.tar", last modified: Sun Apr 21 21:55:54 2024, max compression
+gzip compressed data, was "magic_list-2.2.1.tar", last modified: Sun Apr 21 22:05:01 2024, max compression
```

## Comparing `magic_list-2.2.0.tar` & `magic_list-2.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 21:55:54.732601 magic_list-2.2.0/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2024-03-28 11:39:46.000000 magic_list-2.2.0/LICENSE
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4384 2024-04-21 21:55:54.732601 magic_list-2.2.0/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2100 2024-04-21 21:30:24.000000 magic_list-2.2.0/README.md
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 21:55:54.729268 magic_list-2.2.0/magic_list/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      362 2024-04-21 21:30:24.000000 magic_list-2.2.0/magic_list/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    27562 2024-04-21 21:48:23.000000 magic_list-2.2.0/magic_list/prelude.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     9486 2024-04-21 21:48:23.000000 magic_list-2.2.0/magic_list/prelude.pyi
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2024-03-27 16:41:35.000000 magic_list-2.2.0/magic_list/py.typed
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2024-04-21 21:55:54.729268 magic_list-2.2.0/magic_list.egg-info/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4384 2024-04-21 21:55:54.000000 magic_list-2.2.0/magic_list.egg-info/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      289 2024-04-21 21:55:54.000000 magic_list-2.2.0/magic_list.egg-info/SOURCES.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2024-04-21 21:55:54.000000 magic_list-2.2.0/magic_list.egg-info/dependency_links.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       94 2024-04-21 21:55:54.000000 magic_list-2.2.0/magic_list.egg-info/requires.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       11 2024-04-21 21:55:54.000000 magic_list-2.2.0/magic_list.egg-info/top_level.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1015 2024-04-21 21:55:30.000000 magic_list-2.2.0/pyproject.toml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2024-04-21 21:55:54.732601 magic_list-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:05:01.458161 magic_list-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-21 22:04:43.000000 magic_list-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-21 22:05:01.458161 magic_list-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-21 22:04:43.000000 magic_list-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:05:01.454161 magic_list-2.2.1/magic_list/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-21 22:04:43.000000 magic_list-2.2.1/magic_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27562 2024-04-21 22:04:43.000000 magic_list-2.2.1/magic_list/prelude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-21 22:04:43.000000 magic_list-2.2.1/magic_list/prelude.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 22:04:43.000000 magic_list-2.2.1/magic_list/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:05:01.454161 magic_list-2.2.1/magic_list.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-21 22:05:01.000000 magic_list-2.2.1/magic_list.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-21 22:05:01.000000 magic_list-2.2.1/magic_list.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:05:01.000000 magic_list-2.2.1/magic_list.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 22:05:01.000000 magic_list-2.2.1/magic_list.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 22:05:01.000000 magic_list-2.2.1/magic_list.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-21 22:04:43.000000 magic_list-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:05:01.458161 magic_list-2.2.1/setup.cfg
```

### Comparing `magic_list-2.2.0/LICENSE` & `magic_list-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_list-2.2.0/PKG-INFO` & `magic_list-2.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-list
-Version: 2.2.0
+Version: 2.2.1
 Summary: Magic List is a module that extends the built-in list type.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,22 +55,20 @@
 [![PyPI badge](https://img.shields.io/pypi/v/magic-list)](<https://pypi.org/project/magic-list/>)
 [![Downloads](https://static.pepy.tech/badge/magic-list)](https://pepy.tech/project/magic-list)
 [![Tests](https://github.com/qexat/magic-list/actions/workflows/tests.yml/badge.svg)](https://github.com/qexat/magic-list/actions)
 [![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
 
 Magic List is a module that extends the built-in list type.
 
+[Documentation](https://qexat.github.io/magic-list/) · [PyPI package](https://pypi.org/project/magic-list/) · [How to install](#installation)
+
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
 > test coverage of 100%. It also provides typing stub files.
 
-## Documentation
-
-Documentation can be found [here](https://qexat.github.io/magic-list/).
-
 ## Installation
 
 ### Pip
 
 ```sh
 pip install magic-list
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `magic_list-2.2.0/README.md` & `magic_list-2.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,20 @@
 [![PyPI badge](https://img.shields.io/pypi/v/magic-list)](<https://pypi.org/project/magic-list/>)
 [![Downloads](https://static.pepy.tech/badge/magic-list)](https://pepy.tech/project/magic-list)
 [![Tests](https://github.com/qexat/magic-list/actions/workflows/tests.yml/badge.svg)](https://github.com/qexat/magic-list/actions)
 [![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
 
 Magic List is a module that extends the built-in list type.
 
+[Documentation](https://qexat.github.io/magic-list/) · [PyPI package](https://pypi.org/project/magic-list/) · [How to install](#installation)
+
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
 > test coverage of 100%. It also provides typing stub files.
 
-## Documentation
-
-Documentation can be found [here](https://qexat.github.io/magic-list/).
-
 ## Installation
 
 ### Pip
 
 ```sh
 pip install magic-list
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `magic_list-2.2.0/magic_list/prelude.py` & `magic_list-2.2.1/magic_list/prelude.py`

 * *Files identical despite different names*

### Comparing `magic_list-2.2.0/magic_list/prelude.pyi` & `magic_list-2.2.1/magic_list/prelude.pyi`

 * *Files identical despite different names*

### Comparing `magic_list-2.2.0/magic_list.egg-info/PKG-INFO` & `magic_list-2.2.1/magic_list.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-list
-Version: 2.2.0
+Version: 2.2.1
 Summary: Magic List is a module that extends the built-in list type.
 Author-email: Qexat <contact@qexat.com>
 License: MIT License
         
         Copyright (c) 2024 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,22 +55,20 @@
 [![PyPI badge](https://img.shields.io/pypi/v/magic-list)](<https://pypi.org/project/magic-list/>)
 [![Downloads](https://static.pepy.tech/badge/magic-list)](https://pepy.tech/project/magic-list)
 [![Tests](https://github.com/qexat/magic-list/actions/workflows/tests.yml/badge.svg)](https://github.com/qexat/magic-list/actions)
 [![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
 
 Magic List is a module that extends the built-in list type.
 
+[Documentation](https://qexat.github.io/magic-list/) · [PyPI package](https://pypi.org/project/magic-list/) · [How to install](#installation)
+
 > [!NOTE]
 > Its development is entirely test-driven: it is battery-tested and requires a
 > test coverage of 100%. It also provides typing stub files.
 
-## Documentation
-
-Documentation can be found [here](https://qexat.github.io/magic-list/).
-
 ## Installation
 
 ### Pip
 
 ```sh
 pip install magic-list
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `magic_list-2.2.0/pyproject.toml` & `magic_list-2.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "magic-list"
 description = "Magic List is a module that extends the built-in list type."
-version = "2.2.0"
+version = "2.2.1"
 keywords = ["collections", "list", "built-in", "extension"]
 
 authors = [{ name = "Qexat", email = "contact@qexat.com" }]
 
 requires-python = ">=3.9"
 
 readme = "README.md"
```

