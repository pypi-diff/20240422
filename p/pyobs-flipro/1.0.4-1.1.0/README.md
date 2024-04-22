# Comparing `tmp/pyobs_flipro-1.0.4.tar.gz` & `tmp/pyobs_flipro-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_flipro-1.0.4.tar", max compression
+gzip compressed data, was "pyobs_flipro-1.1.0.tar", max compression
```

## Comparing `pyobs_flipro-1.0.4.tar` & `pyobs_flipro-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1099 2024-04-21 16:57:03.148179 pyobs_flipro-1.0.4/LICENSE
--rw-r--r--   0        0        0     1253 2024-04-21 16:57:03.148179 pyobs_flipro-1.0.4/build.py
--rw-r--r--   0        0        0   178979 2024-04-21 16:57:03.148179 pyobs_flipro-1.0.4/lib/libflipro.h
--rwxr-xr-x   0        0        0   300776 2024-04-21 16:57:03.152179 pyobs_flipro-1.0.4/lib/liblibflialgo.so
--rwxr-xr-x   0        0        0   519928 2024-04-21 16:57:03.156179 pyobs_flipro-1.0.4/lib/liblibflipro.so
--rw-r--r--   0        0        0       39 2024-04-21 16:57:03.156179 pyobs_flipro-1.0.4/pyobs_flipro/__init__.py
--rw-r--r--   0        0        0    10933 2024-04-21 16:57:03.156179 pyobs_flipro-1.0.4/pyobs_flipro/fliprocamera.py
--rw-r--r--   0        0        0     8669 2024-04-21 16:57:03.156179 pyobs_flipro-1.0.4/pyobs_flipro/fliprodriver.pyx
--rw-r--r--   0        0        0     5812 2024-04-21 16:57:03.156179 pyobs_flipro-1.0.4/pyobs_flipro/libflipro.pxd
--rw-r--r--   0        0        0      711 2024-04-21 16:57:03.156179 pyobs_flipro-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 pyobs_flipro-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-21 21:02:39.607560 pyobs_flipro-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1253 2024-04-21 21:02:39.607560 pyobs_flipro-1.1.0/build.py
+-rw-r--r--   0        0        0   178979 2024-04-21 21:02:39.607560 pyobs_flipro-1.1.0/lib/libflipro.h
+-rwxr-xr-x   0        0        0   300776 2024-04-21 21:02:39.607560 pyobs_flipro-1.1.0/lib/liblibflialgo.so
+-rwxr-xr-x   0        0        0   519928 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/lib/liblibflipro.so
+-rw-r--r--   0        0        0       39 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/pyobs_flipro/__init__.py
+-rw-r--r--   0        0        0    11070 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/pyobs_flipro/fliprocamera.py
+-rw-r--r--   0        0        0     8669 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/pyobs_flipro/fliprodriver.pyx
+-rw-r--r--   0        0        0     5812 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/pyobs_flipro/libflipro.pxd
+-rw-r--r--   0        0        0      711 2024-04-21 21:02:39.611560 pyobs_flipro-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 pyobs_flipro-1.1.0/PKG-INFO
```

### Comparing `pyobs_flipro-1.0.4/LICENSE` & `pyobs_flipro-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.4/build.py` & `pyobs_flipro-1.1.0/build.py`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.4/lib/libflipro.h` & `pyobs_flipro-1.1.0/lib/libflipro.h`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.4/lib/liblibflialgo.so` & `pyobs_flipro-1.1.0/lib/liblibflialgo.so`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.4/lib/liblibflipro.so` & `pyobs_flipro-1.1.0/lib/liblibflipro.so`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.4/pyobs_flipro/fliprocamera.py` & `pyobs_flipro-1.1.0/pyobs_flipro/fliprocamera.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 
 
 class FliProCamera(BaseCamera, ICamera, IAbortable, IWindow, IBinning, ICooling):
     """A pyobs module for FLIPRO cameras."""
 
     __module__ = "pyobs_flipro"
 
-    def __init__(self, **kwargs: Any):
+    def __init__(self, setpoint: float, **kwargs: Any):
         """Initializes a new FliProCamera.
 
         Args:
             setpoint: Cooling temperature setpoint.
-            keep_alive_ping: Interval in seconds to ping camera.
         """
         BaseCamera.__init__(self, **kwargs)
         from .fliprodriver import FliProDriver, DeviceInfo  # type: ignore
 
         # variables
         self._driver: Optional[FliProDriver] = None
         self._device: Optional[DeviceInfo] = None
         self._caps: Optional[DeviceCaps] = None
+        self._temp_setpoint: Optional[float] = setpoint
 
         # window and binning
         self._window = (0, 0, 0, 0)
         self._binning = (1, 1)
 
     async def open(self) -> None:
         """Open module."""
@@ -58,14 +58,18 @@
             self._driver.open()
         except ValueError as e:
             raise ValueError("Could not open FLIPRO camera: %s", e)
 
         # get caps
         self._caps = self._driver.get_capabilities()
 
+        # set cooling
+        if self._temp_setpoint is not None:
+            await self.set_cooling(True, self._temp_setpoint)
+
         # get window and binning
         self._window = self._driver.get_image_area()
         self._binning = self._driver.get_binning()
 
     async def close(self) -> None:
         """Close the module."""
         await BaseCamera.close(self)
```

### Comparing `pyobs_flipro-1.0.4/pyobs_flipro/fliprodriver.pyx` & `pyobs_flipro-1.1.0/pyobs_flipro/fliprodriver.pyx`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.4/pyobs_flipro/libflipro.pxd` & `pyobs_flipro-1.1.0/pyobs_flipro/libflipro.pxd`

 * *Files identical despite different names*

### Comparing `pyobs_flipro-1.0.4/pyproject.toml` & `pyobs_flipro-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobs-flipro"
-version = "1.0.4"
+version = "1.1.0"
 description = "pyobs module for FLIPRO cameras"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 include = ['lib']
 
 [tool.poetry.build]
 script = "build.py"
```

### Comparing `pyobs_flipro-1.0.4/PKG-INFO` & `pyobs_flipro-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobs-flipro
-Version: 1.0.4
+Version: 1.1.0
 Summary: pyobs module for FLIPRO cameras
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

