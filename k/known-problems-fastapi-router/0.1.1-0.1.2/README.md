# Comparing `tmp/known_problems_fastapi_router-0.1.1.tar.gz` & `tmp/known_problems_fastapi_router-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "known_problems_fastapi_router-0.1.1.tar", max compression
+gzip compressed data, was "known_problems_fastapi_router-0.1.2.tar", max compression
```

## Comparing `known_problems_fastapi_router-0.1.1.tar` & `known_problems_fastapi_router-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1140 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/README.md
--rw-r--r--   0        0        0      649 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      230 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/__init__.py
--rw-r--r--   0        0        0      826 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/exception_handlers.py
--rw-r--r--   0        0        0    35069 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/routing.py
--rw-r--r--   0        0        0     1270 2024-04-16 08:26:20.497014 known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/types.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 known_problems_fastapi_router-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-22 09:18:19.644998 known_problems_fastapi_router-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     1140 2024-04-22 09:18:19.644998 known_problems_fastapi_router-0.1.2/README.md
+-rw-r--r--   0        0        0      649 2024-04-22 09:18:19.648998 known_problems_fastapi_router-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      230 2024-04-22 09:18:19.648998 known_problems_fastapi_router-0.1.2/src/known_problems_fastapi_router/__init__.py
+-rw-r--r--   0        0        0      826 2024-04-22 09:18:19.648998 known_problems_fastapi_router-0.1.2/src/known_problems_fastapi_router/exception_handlers.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:18:19.648998 known_problems_fastapi_router-0.1.2/src/known_problems_fastapi_router/py.typed
+-rw-r--r--   0        0        0    35069 2024-04-22 09:18:19.648998 known_problems_fastapi_router-0.1.2/src/known_problems_fastapi_router/routing.py
+-rw-r--r--   0        0        0     1270 2024-04-22 09:18:19.648998 known_problems_fastapi_router-0.1.2/src/known_problems_fastapi_router/types.py
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 known_problems_fastapi_router-0.1.2/PKG-INFO
```

### Comparing `known_problems_fastapi_router-0.1.1/LICENSE.txt` & `known_problems_fastapi_router-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `known_problems_fastapi_router-0.1.1/README.md` & `known_problems_fastapi_router-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `known_problems_fastapi_router-0.1.1/pyproject.toml` & `known_problems_fastapi_router-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "known-problems-fastapi-router"
-version = "0.1.1"
+version = "0.1.2"
 description = "A known problem API router package"
 authors = [
     "Fabian Haenel <fabian.haenel@fastlane.net>",
     "Simone Renesto <simone.renesto@fastlane.net>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/exception_handlers.py` & `known_problems_fastapi_router-0.1.2/src/known_problems_fastapi_router/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/routing.py` & `known_problems_fastapi_router-0.1.2/src/known_problems_fastapi_router/routing.py`

 * *Files identical despite different names*

### Comparing `known_problems_fastapi_router-0.1.1/src/known_problems_fastapi_router/types.py` & `known_problems_fastapi_router-0.1.2/src/known_problems_fastapi_router/types.py`

 * *Files identical despite different names*

### Comparing `known_problems_fastapi_router-0.1.1/PKG-INFO` & `known_problems_fastapi_router-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: known-problems-fastapi-router
-Version: 0.1.1
+Version: 0.1.2
 Summary: A known problem API router package
 License: MIT
 Author: Fabian Haenel
 Author-email: fabian.haenel@fastlane.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

