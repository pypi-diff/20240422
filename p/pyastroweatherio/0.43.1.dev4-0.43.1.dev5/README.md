# Comparing `tmp/pyastroweatherio-0.43.1.dev4.tar.gz` & `tmp/pyastroweatherio-0.43.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.43.1.dev4.tar", last modified: Wed Apr 17 12:35:14 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.43.1.dev5.tar", last modified: Mon Apr 22 08:43:57 2024, max compression
```

## Comparing `pyastroweatherio-0.43.1.dev4.tar` & `pyastroweatherio-0.43.1.dev5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-17 12:35:14.156187 pyastroweatherio-0.43.1.dev4/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev4/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-17 12:35:14.156187 pyastroweatherio-0.43.1.dev4/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev4/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-17 12:35:14.156187 pyastroweatherio-0.43.1.dev4/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    32193 2024-04-17 12:34:37.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3638 2024-04-14 12:30:04.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    20074 2024-04-14 12:24:57.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    32312 2023-11-12 10:53:43.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-17 12:35:14.156187 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-17 12:35:14.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-17 12:35:14.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-17 12:35:14.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-17 12:35:14.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-17 12:35:14.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-17 12:35:14.156187 pyastroweatherio-0.43.1.dev4/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-17 12:35:06.000000 pyastroweatherio-0.43.1.dev4/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 08:43:57.588369 pyastroweatherio-0.43.1.dev5/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev5/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-22 08:43:57.588369 pyastroweatherio-0.43.1.dev5/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev5/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 08:43:57.584369 pyastroweatherio-0.43.1.dev5/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    32637 2024-04-22 08:43:32.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3639 2024-04-17 18:18:53.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20074 2024-04-14 12:24:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    32312 2023-11-12 10:53:43.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 08:43:57.588369 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-22 08:43:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-22 08:43:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-22 08:43:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-22 08:43:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-22 08:43:57.000000 pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-22 08:43:57.588369 pyastroweatherio-0.43.1.dev5/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-22 08:43:53.000000 pyastroweatherio-0.43.1.dev5/setup.py
```

### Comparing `pyastroweatherio-0.43.1.dev4/LICENSE` & `pyastroweatherio-0.43.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev4/PKG-INFO` & `pyastroweatherio-0.43.1.dev5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev4
+Version: 0.43.1.dev5
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.43.1.dev4/README.md` & `pyastroweatherio-0.43.1.dev5/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev4/pyastroweatherio/client.py` & `pyastroweatherio-0.43.1.dev5/pyastroweatherio/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         cnt = 0
 
         # Anchor timestamp
         init_ts = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
 
         utc_to_local_diff = self._astro_routines.utc_to_local_diff()
         _LOGGER.debug("UTC to local diff: %s", str(utc_to_local_diff))
-        _LOGGER.debug("Forecast length: %s", str(len(self._weather_data_seventimer)))
+        _LOGGER.debug("Forecast length 7timer: %s", str(len(self._weather_data_seventimer)))
 
         # Met.no
         metno_index = -1
         for row in self._weather_data_seventimer:
             # 7Timer: Skip over past forecasts
             forecast_time = init_ts + timedelta(hours=row["timepoint"])
             if now > forecast_time:
@@ -425,14 +425,15 @@
 
         sun_next_setting = await self._astro_routines.sun_next_setting()
         sun_next_rising = await self._astro_routines.sun_next_rising()
         night_duration_astronomical = await self._astro_routines.night_duration_astronomical()
 
         start_indexes = []
         # Find start index for two nights and store the indexes
+        _LOGGER.debug("Forecast data length: %s", str(len(self._forecast_data)))
         for idx, row in enumerate(self._forecast_data):
             if row.forecast_time.hour % 24 == sun_next_rising.hour and len(start_indexes) == 0:
                 start_indexes.append(0)
             if row.forecast_time.hour % 24 == sun_next_setting.hour:
                 start_indexes.append(idx)
 
         forecast_data_len = len(self._forecast_data)
@@ -539,24 +540,15 @@
                 + self._calm_weight * 8
                 - self._cloudcover_weight
                 - self._seeing_weight
                 - self._transparency_weight
                 - self._calm_weight
             )
         )
-        # _LOGGER.debug(
-        #     "Calc condition cloudcover: %d(%d), seeing %d(%d), transparency: %d(%d), condition %d",
-        #     cloudcover,
-        #     self._cloudcover_weight,
-        #     seeing,
-        #     self._seeing_weight,
-        #     transparency,
-        #     self._transparency_weight,
-        #     condition,
-        # )
+
         return condition
 
     async def calc_dewpoint2m(self, rh2m, temp2m):
         """Calculate 2m Dew Point."""
         # α(T,RH) = ln(RH/100) + aT/(b+T)
         # Ts = (b × α(T,RH)) / (a - α(T,RH))
         alpha = float(Decimal(str(rh2m / 100)).ln()) + MAGNUS_COEFFICIENT_A * temp2m / (MAGNUS_COEFFICIENT_B + temp2m)
@@ -620,16 +612,24 @@
                 else:
                     json_data_astro = await self.async_request_seventimer("astro", "get")
                     astro_dataseries = json_data_astro.get("dataseries", {})
             else:
                 json_data_astro = await self.async_request_seventimer("astro", "get")
                 astro_dataseries = json_data_astro.get("dataseries", {})
 
-            self._weather_data_seventimer = astro_dataseries
-            self._weather_data_seventimer_init = json_data_astro.get("init")
+            if astro_dataseries != {}:
+                self._weather_data_seventimer = astro_dataseries
+                self._weather_data_seventimer_init = json_data_astro.get("init")
+            else:
+                # Fake 7timer weather data if service is broken
+                # This eliminates consideration of seeing, transparency, and lifted_index
+                self._weather_data_seventimer = []
+                for index in range(0, 20):
+                    self._weather_data_seventimer.append({"timepoint": index * 3, "seeing": 0, "transparency": 0, "lifted_index": 0})
+                self._weather_data_seventimer_init = datetime.now().strftime("%Y%m%d%H")
         else:
             _LOGGER.debug("Using cached data for 7Timer")
 
     async def async_request_seventimer(self, product="astro", method="get") -> dict:
         """Make a request against the 7timer API."""
 
         use_running_session = self._session and not self._session.closed
@@ -664,17 +664,21 @@
                 if self._test_mode:
                     json_string = json.dumps(data)
                     with open("debug/" + product + ".json", "w") as outfile:
                         outfile.write(json_string)
 
                 return data
         except asyncio.TimeoutError as tex:
-            raise RequestError(f"Request to endpoint timed out: {tex}") from None
+            _LOGGER.error(f"Request to endpoint timed out: {tex}")
+            return {}
+            # raise RequestError(f"Request to endpoint timed out: {tex}") from None
         except ClientError as err:
-            raise RequestError(f"Error requesting data: {err}") from None
+            _LOGGER.error(f"Error requesting data: {err}")
+            return {}
+            # raise RequestError(f"Error requesting data: {err}") from None
 
         finally:
             if not use_running_session:
                 await session.close()
 
     async def retrieve_data_metno(self):
         """Retrieves current data from met"""
```

### Comparing `pyastroweatherio-0.43.1.dev4/pyastroweatherio/const.py` & `pyastroweatherio-0.43.1.dev5/pyastroweatherio/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Constant Definitions for AstroWeather."""
 
-BASE_URL_SEVENTIMER = "https://www.7timer.info/bin/api.pl"
+BASE_URL_SEVENTIMER = "https://www.7timer.info2/bin/api.pl"
 BASE_URL_MET = "https://api.met.no/weatherapi/locationforecast/2.0/complete"
 HEADERS = {"User-Agent": "AstroWeather github.com/mawinkler/astroweather"}
 STIMER_OUTPUT = "json"
 
 DEFAULT_TIMEOUT = 10
 DEFAULT_CACHE_TIMEOUT = 1770
 DEFAULT_ELEVATION = 0
```

### Comparing `pyastroweatherio-0.43.1.dev4/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.43.1.dev5/pyastroweatherio/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev4/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.43.1.dev5/pyastroweatherio/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.43.1.dev5/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev4
+Version: 0.43.1.dev5
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.43.1.dev4/setup.py` & `pyastroweatherio-0.43.1.dev5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.43.1.dev4",
+    version="0.43.1.dev5",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

