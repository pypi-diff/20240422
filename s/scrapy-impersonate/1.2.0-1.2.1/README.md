# Comparing `tmp/scrapy-impersonate-1.2.0.tar.gz` & `tmp/scrapy_impersonate-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-impersonate-1.2.0.tar", last modified: Thu Feb 22 17:49:29 2024, max compression
+gzip compressed data, was "scrapy_impersonate-1.2.1.tar", last modified: Mon Apr 22 01:29:34 2024, max compression
```

## Comparing `scrapy-impersonate-1.2.0.tar` & `scrapy_impersonate-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:49:29.784386 scrapy-impersonate-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-22 17:49:20.000000 scrapy-impersonate-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-02-22 17:49:29.784386 scrapy-impersonate-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-02-22 17:49:20.000000 scrapy-impersonate-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-22 17:49:20.000000 scrapy-impersonate-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:49:29.780386 scrapy-impersonate-1.2.0/scrapy_impersonate/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-22 17:49:20.000000 scrapy-impersonate-1.2.0/scrapy_impersonate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-02-22 17:49:20.000000 scrapy-impersonate-1.2.0/scrapy_impersonate/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-02-22 17:49:20.000000 scrapy-impersonate-1.2.0/scrapy_impersonate/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 17:49:29.780386 scrapy-impersonate-1.2.0/scrapy_impersonate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-02-22 17:49:29.000000 scrapy-impersonate-1.2.0/scrapy_impersonate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-22 17:49:29.000000 scrapy-impersonate-1.2.0/scrapy_impersonate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 17:49:29.000000 scrapy-impersonate-1.2.0/scrapy_impersonate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-22 17:49:29.000000 scrapy-impersonate-1.2.0/scrapy_impersonate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-22 17:49:29.000000 scrapy-impersonate-1.2.0/scrapy_impersonate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 17:49:29.784386 scrapy-impersonate-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-02-22 17:49:20.000000 scrapy-impersonate-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:34.962652 scrapy_impersonate-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-22 01:29:34.962652 scrapy_impersonate-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:34.962652 scrapy_impersonate-1.2.1/scrapy_impersonate/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/scrapy_impersonate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/scrapy_impersonate/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/scrapy_impersonate/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:29:34.962652 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-22 01:29:34.000000 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-22 01:29:34.000000 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 01:29:34.000000 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 01:29:34.000000 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 01:29:34.000000 scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 01:29:34.962652 scrapy_impersonate-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-22 01:29:27.000000 scrapy_impersonate-1.2.1/setup.py
```

### Comparing `scrapy-impersonate-1.2.0/LICENSE` & `scrapy_impersonate-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-impersonate-1.2.0/PKG-INFO` & `scrapy_impersonate-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-impersonate
-Version: 1.2.0
+Version: 1.2.1
 Summary: Scrapy download handler that can impersonate browser fingerprints
 Home-page: https://github.com/jxlil/scrapy-impersonate
 Author: Jalil SA (jxlil)
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scrapy-impersonate-1.2.0/README.md` & `scrapy_impersonate-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `scrapy-impersonate-1.2.0/scrapy_impersonate/handler.py` & `scrapy_impersonate-1.2.1/scrapy_impersonate/handler.py`

 * *Files identical despite different names*

### Comparing `scrapy-impersonate-1.2.0/scrapy_impersonate/parser.py` & `scrapy_impersonate-1.2.1/scrapy_impersonate/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import base64
 from typing import Optional, Tuple, Union
 from urllib.parse import urlparse
+from curl_cffi import CurlHttpVersion
 
 from scrapy.http import Request
 
 
 class RequestParser:
     def __init__(self, request: Request) -> None:
         self._request = request
@@ -88,13 +89,17 @@
     def max_redirects(self) -> int:
         return self._impersonate_args.get("max_redirects", -1)
 
     @property
     def verify(self) -> Optional[bool]:
         return self._impersonate_args.get("verify")
 
+    @property
+    def http_version(self) -> Optional[CurlHttpVersion]:
+        return self._impersonate_args.get("http_version")
+
     def as_dict(self) -> dict:
         return {
             property_name: getattr(self, property_name)
             for property_name, method in self.__class__.__dict__.items()
             if isinstance(method, property)
         }
```

### Comparing `scrapy-impersonate-1.2.0/scrapy_impersonate.egg-info/PKG-INFO` & `scrapy_impersonate-1.2.1/scrapy_impersonate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-impersonate
-Version: 1.2.0
+Version: 1.2.1
 Summary: Scrapy download handler that can impersonate browser fingerprints
 Home-page: https://github.com/jxlil/scrapy-impersonate
 Author: Jalil SA (jxlil)
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `scrapy-impersonate-1.2.0/setup.py` & `scrapy_impersonate-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="scrapy-impersonate",
-    version="1.2.0",
+    version="1.2.1",
     author="Jalil SA (jxlil)",
     description="Scrapy download handler that can impersonate browser fingerprints",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jxlil/scrapy-impersonate",
     packages=find_packages(),
```

