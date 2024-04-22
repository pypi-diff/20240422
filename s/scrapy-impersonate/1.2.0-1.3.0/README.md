# Comparing `tmp/scrapy-impersonate-1.2.0.tar.gz` & `tmp/scrapy_impersonate-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-impersonate-1.2.0.tar", last modified: Thu Feb 22 17:49:29 2024, max compression
+gzip compressed data, was "scrapy_impersonate-1.3.0.tar", last modified: Mon Apr 22 00:23:27 2024, max compression
```

## Comparing `scrapy-impersonate-1.2.0.tar` & `scrapy_impersonate-1.3.0.tar`

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
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:23:27.864638 scrapy_impersonate-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 00:23:18.000000 scrapy_impersonate-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-22 00:23:27.864638 scrapy_impersonate-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-22 00:23:18.000000 scrapy_impersonate-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-22 00:23:18.000000 scrapy_impersonate-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:23:27.864638 scrapy_impersonate-1.3.0/scrapy_impersonate/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 00:23:18.000000 scrapy_impersonate-1.3.0/scrapy_impersonate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-22 00:23:18.000000 scrapy_impersonate-1.3.0/scrapy_impersonate/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-22 00:23:18.000000 scrapy_impersonate-1.3.0/scrapy_impersonate/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:23:27.864638 scrapy_impersonate-1.3.0/scrapy_impersonate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-22 00:23:27.000000 scrapy_impersonate-1.3.0/scrapy_impersonate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-22 00:23:27.000000 scrapy_impersonate-1.3.0/scrapy_impersonate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 00:23:27.000000 scrapy_impersonate-1.3.0/scrapy_impersonate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 00:23:27.000000 scrapy_impersonate-1.3.0/scrapy_impersonate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 00:23:27.000000 scrapy_impersonate-1.3.0/scrapy_impersonate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 00:23:27.864638 scrapy_impersonate-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-22 00:23:18.000000 scrapy_impersonate-1.3.0/setup.py
```

### Comparing `scrapy-impersonate-1.2.0/LICENSE` & `scrapy_impersonate-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-impersonate-1.2.0/PKG-INFO` & `scrapy_impersonate-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: scrapy-impersonate
-Version: 1.2.0
+Version: 1.3.0
 Summary: Scrapy download handler that can impersonate browser fingerprints
 Home-page: https://github.com/jxlil/scrapy-impersonate
 Author: Jalil SA (jxlil)
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: curl-cffi>=0.6.0
+Requires-Dist: curl-cffi>=0.7.0
 Requires-Dist: scrapy>=2.10.1
 
 # scrapy-impersonate
 [![version](https://img.shields.io/pypi/v/scrapy-impersonate.svg)](https://pypi.python.org/pypi/scrapy-impersonate)
 
 `scrapy-impersonate` is a Scrapy download handler. This project integrates [curl_cffi](https://github.com/yifeikong/curl_cffi) to perform HTTP requests, so it can impersonate browsers' TLS signatures or JA3 fingerprints.
 
@@ -91,14 +91,16 @@
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 101 | 101.0.4951.67 | Windows 10 | `chrome101` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 104 | 104.0.5112.81 | Windows 10 | `chrome104` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 107 | 107.0.5304.107 | Windows 10 | `chrome107` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 110 | 110.0.5481.177 | Windows 10 | `chrome110` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 116 | 116.0.5845.180 | Windows 10 | `chrome116` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 119 | 119.0.6045.199 | macOS Sonoma | `chrome119` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 120 | 120.0.6099.109 | macOS Sonoma | `chrome120` |
+| ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 123 | 123.0.6312.124	| macOS Sonoma | `chrome123` |
+| ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 124 | 124.0.6367.60 | macOS Sonoma | `chrome124` |
 | ![Edge](https://raw.githubusercontent.com/alrra/browser-logos/main/src/edge/edge_24x24.png "Edge") | 99 | 99.0.1150.30 | Windows 10 | `edge99` |
 | ![Edge](https://raw.githubusercontent.com/alrra/browser-logos/main/src/edge/edge_24x24.png "Edge") | 101 | 101.0.1210.47 | Windows 10 | `edge101` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 15.3 | 16612.4.9.1.8 | MacOS Big Sur | `safari15_3` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 15.5 | 17613.2.7.1.8 | MacOS Monterey | `safari15_5` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 17.0 | unclear | MacOS Sonoma | `safari17_0` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 17.2 | unclear | iOS 17.2 | `safari17_2_ios` |
```

### Comparing `scrapy-impersonate-1.2.0/README.md` & `scrapy_impersonate-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 101 | 101.0.4951.67 | Windows 10 | `chrome101` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 104 | 104.0.5112.81 | Windows 10 | `chrome104` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 107 | 107.0.5304.107 | Windows 10 | `chrome107` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 110 | 110.0.5481.177 | Windows 10 | `chrome110` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 116 | 116.0.5845.180 | Windows 10 | `chrome116` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 119 | 119.0.6045.199 | macOS Sonoma | `chrome119` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 120 | 120.0.6099.109 | macOS Sonoma | `chrome120` |
+| ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 123 | 123.0.6312.124	| macOS Sonoma | `chrome123` |
+| ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 124 | 124.0.6367.60 | macOS Sonoma | `chrome124` |
 | ![Edge](https://raw.githubusercontent.com/alrra/browser-logos/main/src/edge/edge_24x24.png "Edge") | 99 | 99.0.1150.30 | Windows 10 | `edge99` |
 | ![Edge](https://raw.githubusercontent.com/alrra/browser-logos/main/src/edge/edge_24x24.png "Edge") | 101 | 101.0.1210.47 | Windows 10 | `edge101` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 15.3 | 16612.4.9.1.8 | MacOS Big Sur | `safari15_3` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 15.5 | 17613.2.7.1.8 | MacOS Monterey | `safari15_5` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 17.0 | unclear | MacOS Sonoma | `safari17_0` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 17.2 | unclear | iOS 17.2 | `safari17_2_ios` |
```

### Comparing `scrapy-impersonate-1.2.0/scrapy_impersonate/handler.py` & `scrapy_impersonate-1.3.0/scrapy_impersonate/handler.py`

 * *Files identical despite different names*

### Comparing `scrapy-impersonate-1.2.0/scrapy_impersonate/parser.py` & `scrapy_impersonate-1.3.0/scrapy_impersonate/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,13 +88,17 @@
     def max_redirects(self) -> int:
         return self._impersonate_args.get("max_redirects", -1)
 
     @property
     def verify(self) -> Optional[bool]:
         return self._impersonate_args.get("verify")
 
+    @property
+    def http_version(self) -> Optional[bool]:
+        return self._impersonate_args.get("http_version")
+
     def as_dict(self) -> dict:
         return {
             property_name: getattr(self, property_name)
             for property_name, method in self.__class__.__dict__.items()
             if isinstance(method, property)
         }
```

### Comparing `scrapy-impersonate-1.2.0/scrapy_impersonate.egg-info/PKG-INFO` & `scrapy_impersonate-1.3.0/scrapy_impersonate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: scrapy-impersonate
-Version: 1.2.0
+Version: 1.3.0
 Summary: Scrapy download handler that can impersonate browser fingerprints
 Home-page: https://github.com/jxlil/scrapy-impersonate
 Author: Jalil SA (jxlil)
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: curl-cffi>=0.6.0
+Requires-Dist: curl-cffi>=0.7.0
 Requires-Dist: scrapy>=2.10.1
 
 # scrapy-impersonate
 [![version](https://img.shields.io/pypi/v/scrapy-impersonate.svg)](https://pypi.python.org/pypi/scrapy-impersonate)
 
 `scrapy-impersonate` is a Scrapy download handler. This project integrates [curl_cffi](https://github.com/yifeikong/curl_cffi) to perform HTTP requests, so it can impersonate browsers' TLS signatures or JA3 fingerprints.
 
@@ -91,14 +91,16 @@
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 101 | 101.0.4951.67 | Windows 10 | `chrome101` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 104 | 104.0.5112.81 | Windows 10 | `chrome104` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 107 | 107.0.5304.107 | Windows 10 | `chrome107` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 110 | 110.0.5481.177 | Windows 10 | `chrome110` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 116 | 116.0.5845.180 | Windows 10 | `chrome116` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 119 | 119.0.6045.199 | macOS Sonoma | `chrome119` |
 | ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 120 | 120.0.6099.109 | macOS Sonoma | `chrome120` |
+| ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 123 | 123.0.6312.124	| macOS Sonoma | `chrome123` |
+| ![Chrome](https://raw.githubusercontent.com/alrra/browser-logos/main/src/chrome/chrome_24x24.png "Chrome") | 124 | 124.0.6367.60 | macOS Sonoma | `chrome124` |
 | ![Edge](https://raw.githubusercontent.com/alrra/browser-logos/main/src/edge/edge_24x24.png "Edge") | 99 | 99.0.1150.30 | Windows 10 | `edge99` |
 | ![Edge](https://raw.githubusercontent.com/alrra/browser-logos/main/src/edge/edge_24x24.png "Edge") | 101 | 101.0.1210.47 | Windows 10 | `edge101` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 15.3 | 16612.4.9.1.8 | MacOS Big Sur | `safari15_3` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 15.5 | 17613.2.7.1.8 | MacOS Monterey | `safari15_5` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 17.0 | unclear | MacOS Sonoma | `safari17_0` |
 | ![Safari](https://github.com/alrra/browser-logos/blob/main/src/safari/safari_24x24.png "Safari") | 17.2 | unclear | iOS 17.2 | `safari17_2_ios` |
```

### Comparing `scrapy-impersonate-1.2.0/setup.py` & `scrapy_impersonate-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="scrapy-impersonate",
-    version="1.2.0",
+    version="1.3.0",
     author="Jalil SA (jxlil)",
     description="Scrapy download handler that can impersonate browser fingerprints",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jxlil/scrapy-impersonate",
     packages=find_packages(),
```

