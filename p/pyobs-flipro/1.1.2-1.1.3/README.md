# Comparing `tmp/pyobs_flipro-1.1.2.tar.gz` & `tmp/pyobs_flipro-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_flipro-1.1.2.tar", max compression
+gzip compressed data, was "pyobs_flipro-1.1.3.tar", max compression
```

## Comparing `pyobs_flipro-1.1.2.tar` & `pyobs_flipro-1.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1099 2024-04-22 00:21:56.117705 pyobs_flipro-1.1.2/LICENSE
--rw-r--r--   0        0        0     1253 2024-04-22 00:21:56.117705 pyobs_flipro-1.1.2/build.py
--rw-r--r--   0        0        0   178979 2024-04-22 00:21:56.117705 pyobs_flipro-1.1.2/lib/libflipro.h
--rwxr-xr-x   0        0        0   300776 2024-04-22 00:21:56.121705 pyobs_flipro-1.1.2/lib/liblibflialgo.so
--rwxr-xr-x   0        0        0   519928 2024-04-22 00:21:56.121705 pyobs_flipro-1.1.2/lib/liblibflipro.so
--rw-r--r--   0        0        0       39 2024-04-22 00:21:56.121705 pyobs_flipro-1.1.2/pyobs_flipro/__init__.py
--rw-r--r--   0        0        0    13259 2024-04-22 00:21:56.121705 pyobs_flipro-1.1.2/pyobs_flipro/fliprocamera.py
--rw-r--r--   0        0        0     9246 2024-04-22 00:21:56.121705 pyobs_flipro-1.1.2/pyobs_flipro/fliprodriver.pyx
--rw-r--r--   0        0        0     5812 2024-04-22 00:21:56.125705 pyobs_flipro-1.1.2/pyobs_flipro/libflipro.pxd
--rw-r--r--   0        0        0      711 2024-04-22 00:21:56.125705 pyobs_flipro-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 pyobs_flipro-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-22 00:22:39.479527 pyobs_flipro-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1253 2024-04-22 00:22:39.479527 pyobs_flipro-1.1.3/build.py
+-rw-r--r--   0        0        0   178979 2024-04-22 00:22:39.479527 pyobs_flipro-1.1.3/lib/libflipro.h
+-rwxr-xr-x   0        0        0   300776 2024-04-22 00:22:39.479527 pyobs_flipro-1.1.3/lib/liblibflialgo.so
+-rwxr-xr-x   0        0        0   519928 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/lib/liblibflipro.so
+-rw-r--r--   0        0        0       39 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/pyobs_flipro/__init__.py
+-rw-r--r--   0        0        0    13259 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/pyobs_flipro/fliprocamera.py
+-rw-r--r--   0        0        0     9247 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/pyobs_flipro/fliprodriver.pyx
+-rw-r--r--   0        0        0     5812 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/pyobs_flipro/libflipro.pxd
+-rw-r--r--   0        0        0      711 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 pyobs_flipro-1.1.3/PKG-INFO
```

### Comparing `pyobs_flipro-1.1.2/LICENSE` & `pyobs_flipro-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.2/build.py` & `pyobs_flipro-1.1.3/build.py`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.2/lib/libflipro.h` & `pyobs_flipro-1.1.3/lib/libflipro.h`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.2/lib/liblibflialgo.so` & `pyobs_flipro-1.1.3/lib/liblibflialgo.so`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.2/lib/liblibflipro.so` & `pyobs_flipro-1.1.3/lib/liblibflipro.so`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.2/pyobs_flipro/fliprocamera.py` & `pyobs_flipro-1.1.3/pyobs_flipro/fliprocamera.py`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.2/pyobs_flipro/fliprodriver.pyx` & `pyobs_flipro-1.1.3/pyobs_flipro/fliprodriver.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         return self.__decode(self.obj.cSerialNo)
 
     @property
     def device_path(self):
         return self.__decode(self.obj.cDevicePath)
 
     @property
-    def conn_type(self)
+    def conn_type(self):
         return "USB" if self.obj.eConnType == FPRO_CONNECTION_USB else "FIBRE"
 
     @property
     def vendor_id(self):
         return self.obj.uiVendorId
 
     @property
```

### Comparing `pyobs_flipro-1.1.2/pyobs_flipro/libflipro.pxd` & `pyobs_flipro-1.1.3/pyobs_flipro/libflipro.pxd`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.2/pyproject.toml` & `pyobs_flipro-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobs-flipro"
-version = "1.1.2"
+version = "1.1.3"
 description = "pyobs module for FLIPRO cameras"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 include = ['lib']
 
 [tool.poetry.build]
 script = "build.py"
```

### Comparing `pyobs_flipro-1.1.2/PKG-INFO` & `pyobs_flipro-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobs-flipro
-Version: 1.1.2
+Version: 1.1.3
 Summary: pyobs module for FLIPRO cameras
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

