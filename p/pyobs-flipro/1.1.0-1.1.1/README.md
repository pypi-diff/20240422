# Comparing `tmp/pyobs_flipro-1.1.0.tar.gz` & `tmp/pyobs_flipro-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_flipro-1.1.0.tar", max compression
+gzip compressed data, was "pyobs_flipro-1.1.1.tar", max compression
```

## Comparing `pyobs_flipro-1.1.0.tar` & `pyobs_flipro-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1099 2024-04-21 21:02:39.607560 pyobs_flipro-1.1.0/LICENSE
--rw-r--r--   0        0        0     1253 2024-04-21 21:02:39.607560 pyobs_flipro-1.1.0/build.py
--rw-r--r--   0        0        0   178979 2024-04-21 21:02:39.607560 pyobs_flipro-1.1.0/lib/libflipro.h
--rwxr-xr-x   0        0        0   300776 2024-04-21 21:02:39.607560 pyobs_flipro-1.1.0/lib/liblibflialgo.so
--rwxr-xr-x   0        0        0   519928 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/lib/liblibflipro.so
--rw-r--r--   0        0        0       39 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/pyobs_flipro/__init__.py
--rw-r--r--   0        0        0    11070 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/pyobs_flipro/fliprocamera.py
--rw-r--r--   0        0        0     8669 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/pyobs_flipro/fliprodriver.pyx
--rw-r--r--   0        0        0     5812 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/pyobs_flipro/libflipro.pxd
--rw-r--r--   0        0        0      711 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 pyobs_flipro-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-22 00:16:41.211152 pyobs_flipro-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1253 2024-04-22 00:16:41.211152 pyobs_flipro-1.1.1/build.py
+-rw-r--r--   0        0        0   178979 2024-04-22 00:16:41.211152 pyobs_flipro-1.1.1/lib/libflipro.h
+-rwxr-xr-x   0        0        0   300776 2024-04-22 00:16:41.215152 pyobs_flipro-1.1.1/lib/liblibflialgo.so
+-rwxr-xr-x   0        0        0   519928 2024-04-22 00:16:41.215152 pyobs_flipro-1.1.1/lib/liblibflipro.so
+-rw-r--r--   0        0        0       39 2024-04-22 00:16:41.215152 pyobs_flipro-1.1.1/pyobs_flipro/__init__.py
+-rw-r--r--   0        0        0    13271 2024-04-22 00:16:41.215152 pyobs_flipro-1.1.1/pyobs_flipro/fliprocamera.py
+-rw-r--r--   0        0        0     8669 2024-04-22 00:16:41.219152 pyobs_flipro-1.1.1/pyobs_flipro/fliprodriver.pyx
+-rw-r--r--   0        0        0     5812 2024-04-22 00:16:41.219152 pyobs_flipro-1.1.1/pyobs_flipro/libflipro.pxd
+-rw-r--r--   0        0        0      711 2024-04-22 00:16:41.219152 pyobs_flipro-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 pyobs_flipro-1.1.1/PKG-INFO
```

### Comparing `pyobs_flipro-1.1.0/LICENSE` & `pyobs_flipro-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.0/build.py` & `pyobs_flipro-1.1.1/build.py`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.0/lib/libflipro.h` & `pyobs_flipro-1.1.1/lib/libflipro.h`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.0/lib/liblibflialgo.so` & `pyobs_flipro-1.1.1/lib/liblibflialgo.so`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.0/lib/liblibflipro.so` & `pyobs_flipro-1.1.1/lib/liblibflipro.so`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.0/pyobs_flipro/fliprocamera.py` & `pyobs_flipro-1.1.1/pyobs_flipro/fliprocamera.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,23 +48,25 @@
         # list devices
         devices = FliProDriver.list_devices()
         if len(devices) == 0:
             raise ValueError("No camera found.")
 
         # open first one
         self._device = devices[0]
+        self._log_device_info()
         log.info('Opening connection to "%s"...', self._device.friendly_name)
         self._driver = FliProDriver(self._device)
         try:
             self._driver.open()
         except ValueError as e:
             raise ValueError("Could not open FLIPRO camera: %s", e)
 
         # get caps
         self._caps = self._driver.get_capabilities()
+        self._log_capabilities()
 
         # set cooling
         if self._temp_setpoint is not None:
             await self.set_cooling(True, self._temp_setpoint)
 
         # get window and binning
         self._window = self._driver.get_image_area()
@@ -76,14 +78,46 @@
 
         # not open?
         if self._driver is not None:
             # close connection
             self._driver.close()
             self._driver = None
 
+    def _log_device_info(self):
+        log.info("Device info:")
+        log.info(f"  Friendly Name: {self._device.obj.cFriendlyName}")
+        log.info(f"      Serial No: {self._device.obj.cSerialNo}")
+        log.info(f"    Device Path: {self._device.obj.cDevicePath}")
+        log.info(f"      Conn Type: {self._device.obj.eConnType}")
+        log.info(f"      Vendor ID: {self._device.obj.uiVendorId}")
+        log.info(f"        Prod ID: {self._device.obj.uiProdId}")
+        log.info(f"      USB Speed: {self._device.obj.eUSBSpeed}")
+
+    def _log_capabilities(self):
+        log.info("Capabilities:")
+        log.info(f"                     Version: {self._caps.uiCapVersion}")
+        log.info(f"                 Device Type: {self._caps.uiDeviceType}")
+        log.info(f"       Max Pixel Image Width: {self._caps.uiMaxPixelImageWidth}")
+        log.info(f"      Max Pixel Image Height: {self._caps.uiMaxPixelImageHeight}")
+        log.info(f"      Available Pixel Depths: {self._caps.uiAvailablePixelDepths}")
+        log.info(f"          Binning Table Size: {self._caps.uiBinningsTableSize}")
+        log.info(f"             Black Level Max: {self._caps.uiBlackLevelMax}")
+        log.info(f"               Black Sun Max: {self._caps.uiBlackSunMax}")
+        log.info(f"                    Low Gain: {self._caps.uiLowGain}")
+        log.info(f"                   High Gain: {self._caps.uiHighGain}")
+        # log.info(f"{self._caps.uiReserved}")
+        log.info(f"               Row Scan Time: {self._caps.uiRowScanTime}")
+        log.info(f"             Dummy Pixel Num: {self._caps.uiDummyPixelNum}")
+        log.info(f"  Horizontal Scan Invertable: {self._caps.bHorizontalScanInvertable}")
+        log.info(f"    Vertical Scan Invertable: {self._caps.bVerticalScanInvertable}")
+        log.info(f"        NV Storage Available: {self._caps.uiNVStorageAvailable}")
+        log.info(f"    Pre Frame Reference Rows: {self._caps.uiPreFrameReferenceRows}")
+        log.info(f"   Post Frame Reference Rows: {self._caps.uiPostFrameReferenceRows}")
+        log.info(f"              Meta Data Size: {self._caps.uiMetaDataSize}")
+
     async def _expose(self, exposure_time: float, open_shutter: bool, abort_event: asyncio.Event) -> Image:
         """Actually do the exposure, should be implemented by derived classes.
 
         Args:
             exposure_time: The requested exposure time in seconds.
             open_shutter: Whether or not to open the shutter.
             abort_event: Event that gets triggered when exposure should be aborted.
```

### Comparing `pyobs_flipro-1.1.0/pyobs_flipro/fliprodriver.pyx` & `pyobs_flipro-1.1.1/pyobs_flipro/fliprodriver.pyx`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.0/pyobs_flipro/libflipro.pxd` & `pyobs_flipro-1.1.1/pyobs_flipro/libflipro.pxd`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.1.0/pyproject.toml` & `pyobs_flipro-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobs-flipro"
-version = "1.1.0"
+version = "1.1.1"
 description = "pyobs module for FLIPRO cameras"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 include = ['lib']
 
 [tool.poetry.build]
 script = "build.py"
```

### Comparing `pyobs_flipro-1.1.0/PKG-INFO` & `pyobs_flipro-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobs-flipro
-Version: 1.1.0
+Version: 1.1.1
 Summary: pyobs module for FLIPRO cameras
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

