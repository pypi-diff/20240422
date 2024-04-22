# Comparing `tmp/dotpack-0.3.5.tar.gz` & `tmp/dotpack-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotpack-0.3.5.tar", last modified: Thu Nov 16 04:10:51 2023, max compression
+gzip compressed data, was "dotpack-0.3.6.tar", last modified: Mon Apr 22 05:51:12 2024, max compression
```

## Comparing `dotpack-0.3.5.tar` & `dotpack-0.3.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 xavierchan   (501) staff       (20)        0 2023-11-16 04:10:51.291708 dotpack-0.3.5/
--rw-r--r--   0 xavierchan   (501) staff       (20)      147 2023-08-05 09:39:41.000000 dotpack-0.3.5/AUTHORS.rst
--rw-r--r--   0 xavierchan   (501) staff       (20)      298 2023-11-16 04:07:57.000000 dotpack-0.3.5/HISTORY.rst
--rw-r--r--   0 xavierchan   (501) staff       (20)     1596 2023-08-05 09:39:41.000000 dotpack-0.3.5/LICENSE
--rw-r--r--   0 xavierchan   (501) staff       (20)      303 2023-08-05 09:39:41.000000 dotpack-0.3.5/MANIFEST.in
--rw-r--r--   0 xavierchan   (501) staff       (20)     1713 2023-11-16 04:10:51.291568 dotpack-0.3.5/PKG-INFO
--rw-r--r--   0 xavierchan   (501) staff       (20)      500 2023-08-05 09:39:41.000000 dotpack-0.3.5/README.rst
-drwxr-xr-x   0 xavierchan   (501) staff       (20)        0 2023-11-16 04:10:51.282193 dotpack-0.3.5/dotpack/
--rw-r--r--   0 xavierchan   (501) staff       (20)      148 2023-08-07 04:10:05.000000 dotpack-0.3.5/dotpack/__init__.py
--rw-r--r--   0 xavierchan   (501) staff       (20)    25561 2023-11-16 04:01:08.000000 dotpack-0.3.5/dotpack/ledbag.py
--rw-r--r--   0 xavierchan   (501) staff       (20)    22160 2023-08-17 07:10:08.000000 dotpack-0.3.5/dotpack/ledpanel.py
--rw-r--r--   0 xavierchan   (501) staff       (20)     5592 2023-08-05 09:39:41.000000 dotpack-0.3.5/dotpack/microblocks_client.py
-drwxr-xr-x   0 xavierchan   (501) staff       (20)        0 2023-11-16 04:10:51.285870 dotpack-0.3.5/dotpack/src/
--rw-r--r--   0 xavierchan   (501) staff       (20)   676304 2023-08-05 09:39:41.000000 dotpack-0.3.5/dotpack/src/seguiemj.ttf
--rw-r--r--   0 xavierchan   (501) staff       (20)      549 2023-08-05 09:39:41.000000 dotpack-0.3.5/dotpack/utils.py
-drwxr-xr-x   0 xavierchan   (501) staff       (20)        0 2023-11-16 04:10:51.285549 dotpack-0.3.5/dotpack.egg-info/
--rw-r--r--   0 xavierchan   (501) staff       (20)     1713 2023-11-16 04:10:51.000000 dotpack-0.3.5/dotpack.egg-info/PKG-INFO
--rw-r--r--   0 xavierchan   (501) staff       (20)      419 2023-11-16 04:10:51.000000 dotpack-0.3.5/dotpack.egg-info/SOURCES.txt
--rw-r--r--   0 xavierchan   (501) staff       (20)        1 2023-11-16 04:10:51.000000 dotpack-0.3.5/dotpack.egg-info/dependency_links.txt
--rw-r--r--   0 xavierchan   (501) staff       (20)        1 2023-08-07 04:15:26.000000 dotpack-0.3.5/dotpack.egg-info/not-zip-safe
--rw-r--r--   0 xavierchan   (501) staff       (20)      100 2023-11-16 04:10:51.000000 dotpack-0.3.5/dotpack.egg-info/requires.txt
--rw-r--r--   0 xavierchan   (501) staff       (20)        8 2023-11-16 04:10:51.000000 dotpack-0.3.5/dotpack.egg-info/top_level.txt
--rw-r--r--   0 xavierchan   (501) staff       (20)     1184 2023-08-05 09:39:41.000000 dotpack-0.3.5/readme.md
--rw-r--r--   0 xavierchan   (501) staff       (20)      449 2023-11-16 04:10:51.292317 dotpack-0.3.5/setup.cfg
--rw-r--r--   0 xavierchan   (501) staff       (20)     1629 2023-11-16 04:07:34.000000 dotpack-0.3.5/setup.py
-drwxr-xr-x   0 xavierchan   (501) staff       (20)        0 2023-11-16 04:10:51.290727 dotpack-0.3.5/tests/
--rw-r--r--   0 xavierchan   (501) staff       (20)      622 2023-08-05 09:39:41.000000 dotpack-0.3.5/tests/test_dotpack.py
+drwxrwxr-x   0 xavierchan  (1000) xavierchan  (1000)        0 2024-04-22 05:51:12.448000 dotpack-0.3.6/
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)      147 2024-04-22 04:36:10.000000 dotpack-0.3.6/AUTHORS.rst
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)      298 2024-04-22 04:36:10.000000 dotpack-0.3.6/HISTORY.rst
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)     1596 2024-04-22 04:36:10.000000 dotpack-0.3.6/LICENSE
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)      303 2024-04-22 04:36:10.000000 dotpack-0.3.6/MANIFEST.in
+-rw-r--r--   0 xavierchan  (1000) xavierchan  (1000)     1713 2024-04-22 05:51:12.448000 dotpack-0.3.6/PKG-INFO
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)      500 2024-04-22 04:36:10.000000 dotpack-0.3.6/README.rst
+drwxrwxr-x   0 xavierchan  (1000) xavierchan  (1000)        0 2024-04-22 05:51:12.448000 dotpack-0.3.6/dotpack/
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)      148 2024-04-22 05:33:48.000000 dotpack-0.3.6/dotpack/__init__.py
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)    25566 2024-04-22 05:33:40.000000 dotpack-0.3.6/dotpack/ledbag.py
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)    22160 2024-04-22 05:42:16.000000 dotpack-0.3.6/dotpack/ledpanel.py
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)     5592 2024-04-22 04:36:10.000000 dotpack-0.3.6/dotpack/microblocks_client.py
+drwxrwxr-x   0 xavierchan  (1000) xavierchan  (1000)        0 2024-04-22 05:51:12.448000 dotpack-0.3.6/dotpack/src/
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)   676304 2024-04-22 04:36:10.000000 dotpack-0.3.6/dotpack/src/seguiemj.ttf
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)      549 2024-04-22 04:36:10.000000 dotpack-0.3.6/dotpack/utils.py
+drwxrwxr-x   0 xavierchan  (1000) xavierchan  (1000)        0 2024-04-22 05:51:12.448000 dotpack-0.3.6/dotpack.egg-info/
+-rw-r--r--   0 xavierchan  (1000) xavierchan  (1000)     1713 2024-04-22 05:51:12.000000 dotpack-0.3.6/dotpack.egg-info/PKG-INFO
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)      419 2024-04-22 05:51:12.000000 dotpack-0.3.6/dotpack.egg-info/SOURCES.txt
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)        1 2024-04-22 05:51:12.000000 dotpack-0.3.6/dotpack.egg-info/dependency_links.txt
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)        1 2024-04-22 05:28:26.000000 dotpack-0.3.6/dotpack.egg-info/not-zip-safe
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)      100 2024-04-22 05:51:12.000000 dotpack-0.3.6/dotpack.egg-info/requires.txt
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)        8 2024-04-22 05:51:12.000000 dotpack-0.3.6/dotpack.egg-info/top_level.txt
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)     1184 2024-04-22 04:36:10.000000 dotpack-0.3.6/readme.md
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)      449 2024-04-22 05:51:12.452000 dotpack-0.3.6/setup.cfg
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)     1629 2024-04-22 05:33:56.000000 dotpack-0.3.6/setup.py
+drwxrwxr-x   0 xavierchan  (1000) xavierchan  (1000)        0 2024-04-22 05:51:12.448000 dotpack-0.3.6/tests/
+-rw-rw-r--   0 xavierchan  (1000) xavierchan  (1000)      622 2024-04-22 04:36:10.000000 dotpack-0.3.6/tests/test_dotpack.py
```

### Comparing `dotpack-0.3.5/LICENSE` & `dotpack-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.5/PKG-INFO` & `dotpack-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotpack
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/longan-link/dotpack_pyclient
 Author: Wenjie Wu
 Author-email: wuwenjie718@gmail.com
 License: GNU General Public License v3
 Keywords: dotpack
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dotpack-0.3.5/dotpack/ledbag.py` & `dotpack-0.3.6/dotpack/ledbag.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             print("connected!")
             return True
 
         if self._get_client_type(self.address) == "C_firmware":
             # fix win7 bleak bug
             from .ledpanel import DotPackClient
 
-            address = self._execute(self._get_address(address))
+            address = self._execute(self._get_address(self.address))
             self._ledpanel = DotPackClient(address)
             self._execute(self._ledpanel.connect())
             print("connected!")
             return True
 
     def disconnect(self):
         # print('disconnect')
```

### Comparing `dotpack-0.3.5/dotpack/ledpanel.py` & `dotpack-0.3.6/dotpack/ledpanel.py`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.5/dotpack/microblocks_client.py` & `dotpack-0.3.6/dotpack/microblocks_client.py`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.5/dotpack/src/seguiemj.ttf` & `dotpack-0.3.6/dotpack/src/seguiemj.ttf`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.5/dotpack/utils.py` & `dotpack-0.3.6/dotpack/utils.py`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.5/dotpack.egg-info/PKG-INFO` & `dotpack-0.3.6/dotpack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotpack
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/longan-link/dotpack_pyclient
 Author: Wenjie Wu
 Author-email: wuwenjie718@gmail.com
 License: GNU General Public License v3
 Keywords: dotpack
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dotpack-0.3.5/readme.md` & `dotpack-0.3.6/readme.md`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.5/setup.py` & `dotpack-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,10 +50,10 @@
             # 'dotpack-scan = dotpack.tools.scan:scan',
         ],
     },
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/longan-link/dotpack_pyclient",
-    version="0.3.5",
+    version="0.3.6",
     zip_safe=False,
 )
```

### Comparing `dotpack-0.3.5/tests/test_dotpack.py` & `dotpack-0.3.6/tests/test_dotpack.py`

 * *Files identical despite different names*

