# Comparing `tmp/pyastroweatherio-0.43.1.dev5.tar.gz` & `tmp/pyastroweatherio-0.43.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.43.1.dev5.tar", last modified: Mon Apr 22 08:43:57 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.43.1.dev6.tar", last modified: Mon Apr 22 09:06:04 2024, max compression
```

## Comparing `pyastroweatherio-0.43.1.dev5.tar` & `pyastroweatherio-0.43.1.dev6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 08:43:57.588369 pyastroweatherio-0.43.1.dev5/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev5/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-22 08:43:57.588369 pyastroweatherio-0.43.1.dev5/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev5/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 08:43:57.584369 pyastroweatherio-0.43.1.dev5/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    32637 2024-04-22 08:43:32.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3639 2024-04-17 18:18:53.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    20074 2024-04-14 12:24:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    32312 2023-11-12 10:53:43.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 08:43:57.588369 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-22 08:43:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-22 08:43:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-22 08:43:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-22 08:43:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-22 08:43:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-22 08:43:57.588369 pyastroweatherio-0.43.1.dev5/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-22 08:43:53.000000 pyastroweatherio-0.43.1.dev5/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 09:06:04.007578 pyastroweatherio-0.43.1.dev6/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev6/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-22 09:06:04.007578 pyastroweatherio-0.43.1.dev6/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev6/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 09:06:04.003578 pyastroweatherio-0.43.1.dev6/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev6/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    32723 2024-04-22 09:05:25.000000 pyastroweatherio-0.43.1.dev6/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3639 2024-04-17 18:18:53.000000 pyastroweatherio-0.43.1.dev6/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20074 2024-04-14 12:24:57.000000 pyastroweatherio-0.43.1.dev6/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev6/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    32312 2023-11-12 10:53:43.000000 pyastroweatherio-0.43.1.dev6/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 09:06:04.003578 pyastroweatherio-0.43.1.dev6/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-22 09:06:03.000000 pyastroweatherio-0.43.1.dev6/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-22 09:06:03.000000 pyastroweatherio-0.43.1.dev6/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-22 09:06:03.000000 pyastroweatherio-0.43.1.dev6/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-22 09:06:03.000000 pyastroweatherio-0.43.1.dev6/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-22 09:06:03.000000 pyastroweatherio-0.43.1.dev6/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-22 09:06:04.007578 pyastroweatherio-0.43.1.dev6/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-22 09:06:00.000000 pyastroweatherio-0.43.1.dev6/setup.py
```

### Comparing `pyastroweatherio-0.43.1.dev5/LICENSE` & `pyastroweatherio-0.43.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev5/PKG-INFO` & `pyastroweatherio-0.43.1.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev5
+Version: 0.43.1.dev6
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.43.1.dev5/README.md` & `pyastroweatherio-0.43.1.dev6/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev5/pyastroweatherio/client.py` & `pyastroweatherio-0.43.1.dev6/pyastroweatherio/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,14 +618,16 @@
 
             if astro_dataseries != {}:
                 self._weather_data_seventimer = astro_dataseries
                 self._weather_data_seventimer_init = json_data_astro.get("init")
             else:
                 # Fake 7timer weather data if service is broken
                 # This eliminates consideration of seeing, transparency, and lifted_index
+                self._seeing_weight = 0
+                self._transparency_weight = 0
                 self._weather_data_seventimer = []
                 for index in range(0, 20):
                     self._weather_data_seventimer.append({"timepoint": index * 3, "seeing": 0, "transparency": 0, "lifted_index": 0})
                 self._weather_data_seventimer_init = datetime.now().strftime("%Y%m%d%H")
         else:
             _LOGGER.debug("Using cached data for 7Timer")
```

### Comparing `pyastroweatherio-0.43.1.dev5/pyastroweatherio/const.py` & `pyastroweatherio-0.43.1.dev6/pyastroweatherio/const.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev5/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.43.1.dev6/pyastroweatherio/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev5/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.43.1.dev6/pyastroweatherio/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.43.1.dev6/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev5
+Version: 0.43.1.dev6
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.43.1.dev5/setup.py` & `pyastroweatherio-0.43.1.dev6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.43.1.dev5",
+    version="0.43.1.dev6",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

