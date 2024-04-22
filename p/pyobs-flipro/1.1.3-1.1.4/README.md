# Comparing `tmp/pyobs_flipro-1.1.3.tar.gz` & `tmp/pyobs_flipro-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_flipro-1.1.3.tar", max compression
+gzip compressed data, was "pyobs_flipro-1.1.4.tar", max compression
```

## Comparing `pyobs_flipro-1.1.3.tar` & `pyobs_flipro-1.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1099 2024-04-22 00:22:39.479527 pyobs_flipro-1.1.3/LICENSE
--rw-r--r--   0        0        0     1253 2024-04-22 00:22:39.479527 pyobs_flipro-1.1.3/build.py
--rw-r--r--   0        0        0   178979 2024-04-22 00:22:39.479527 pyobs_flipro-1.1.3/lib/libflipro.h
--rwxr-xr-x   0        0        0   300776 2024-04-22 00:22:39.479527 pyobs_flipro-1.1.3/lib/liblibflialgo.so
--rwxr-xr-x   0        0        0   519928 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/lib/liblibflipro.so
--rw-r--r--   0        0        0       39 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/pyobs_flipro/__init__.py
--rw-r--r--   0        0        0    13259 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/pyobs_flipro/fliprocamera.py
--rw-r--r--   0        0        0     9247 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/pyobs_flipro/fliprodriver.pyx
--rw-r--r--   0        0        0     5812 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/pyobs_flipro/libflipro.pxd
--rw-r--r--   0        0        0      711 2024-04-22 00:22:39.483527 pyobs_flipro-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 pyobs_flipro-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-22 00:23:40.265881 pyobs_flipro-1.1.4/LICENSE
+-rw-r--r--   0        0        0     1253 2024-04-22 00:23:40.265881 pyobs_flipro-1.1.4/build.py
+-rw-r--r--   0        0        0   178979 2024-04-22 00:23:40.265881 pyobs_flipro-1.1.4/lib/libflipro.h
+-rwxr-xr-x   0        0        0   300776 2024-04-22 00:23:40.265881 pyobs_flipro-1.1.4/lib/liblibflialgo.so
+-rwxr-xr-x   0        0        0   519928 2024-04-22 00:23:40.269881 pyobs_flipro-1.1.4/lib/liblibflipro.so
+-rw-r--r--   0        0        0       39 2024-04-22 00:23:40.269881 pyobs_flipro-1.1.4/pyobs_flipro/__init__.py
+-rw-r--r--   0        0        0    13245 2024-04-22 00:23:40.269881 pyobs_flipro-1.1.4/pyobs_flipro/fliprocamera.py
+-rw-r--r--   0        0        0     9247 2024-04-22 00:23:40.269881 pyobs_flipro-1.1.4/pyobs_flipro/fliprodriver.pyx
+-rw-r--r--   0        0        0     5812 2024-04-22 00:23:40.269881 pyobs_flipro-1.1.4/pyobs_flipro/libflipro.pxd
+-rw-r--r--   0        0        0      711 2024-04-22 00:23:40.269881 pyobs_flipro-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 pyobs_flipro-1.1.4/PKG-INFO
```

### Comparing `pyobs_flipro-1.1.3/LICENSE` & `pyobs_flipro-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.3/build.py` & `pyobs_flipro-1.1.4/build.py`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.3/lib/libflipro.h` & `pyobs_flipro-1.1.4/lib/libflipro.h`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.3/lib/liblibflialgo.so` & `pyobs_flipro-1.1.4/lib/liblibflialgo.so`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.3/lib/liblibflipro.so` & `pyobs_flipro-1.1.4/lib/liblibflipro.so`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.3/pyobs_flipro/fliprocamera.py` & `pyobs_flipro-1.1.4/pyobs_flipro/fliprocamera.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,17 @@
 
     def _log_device_info(self):
         log.info("Device info:")
         log.info(f"  Friendly Name: {self._device.friendly_name}")
         log.info(f"      Serial No: {self._device.serial_number}")
         log.info(f"    Device Path: {self._device.device_path}")
         log.info(f"      Conn Type: {self._device.conn_type}")
-        log.info(f"      Vendor ID: {self._device.obj.uiVendorId}")
-        log.info(f"        Prod ID: {self._device.obj.uiProdId}")
-        log.info(f"      USB Speed: {self._device.obj.eUSBSpeed}")
+        log.info(f"      Vendor ID: {self._device.vendor_id}")
+        log.info(f"        Prod ID: {self._device.prod_id}")
+        log.info(f"      USB Speed: {self._device.usb_speed}")
 
     def _log_capabilities(self):
         log.info("Capabilities:")
         log.info(f"                     Version: {self._caps.uiCapVersion}")
         log.info(f"                 Device Type: {self._caps.uiDeviceType}")
         log.info(f"       Max Pixel Image Width: {self._caps.uiMaxPixelImageWidth}")
         log.info(f"      Max Pixel Image Height: {self._caps.uiMaxPixelImageHeight}")
```

### Comparing `pyobs_flipro-1.1.3/pyobs_flipro/fliprodriver.pyx` & `pyobs_flipro-1.1.4/pyobs_flipro/fliprodriver.pyx`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.3/pyobs_flipro/libflipro.pxd` & `pyobs_flipro-1.1.4/pyobs_flipro/libflipro.pxd`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.3/pyproject.toml` & `pyobs_flipro-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobs-flipro"
-version = "1.1.3"
+version = "1.1.4"
 description = "pyobs module for FLIPRO cameras"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 include = ['lib']
 
 [tool.poetry.build]
 script = "build.py"
```

### Comparing `pyobs_flipro-1.1.3/PKG-INFO` & `pyobs_flipro-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobs-flipro
-Version: 1.1.3
+Version: 1.1.4
 Summary: pyobs module for FLIPRO cameras
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

