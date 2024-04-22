# Comparing `tmp/acenav_api-1.0.4.tar.gz` & `tmp/acenav_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/acenav_api-1.0.4.tar", last modified: Mon Apr  1 07:23:56 2024, max compression
+gzip compressed data, was "dist/acenav_api-1.0.5.tar", last modified: Mon Apr 22 08:37:55 2024, max compression
```

## Comparing `acenav_api-1.0.4.tar` & `acenav_api-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 songyiwei   (501) staff       (20)        0 2024-04-01 07:23:56.000000 acenav_api-1.0.4/
--rw-r--r--   0 songyiwei   (501) staff       (20)     4195 2024-04-01 07:23:56.000000 acenav_api-1.0.4/PKG-INFO
--rw-r--r--   0 songyiwei   (501) staff       (20)     3143 2024-03-29 01:58:30.000000 acenav_api-1.0.4/README.md
-drwxr-xr-x   0 songyiwei   (501) staff       (20)        0 2024-04-01 07:23:56.000000 acenav_api-1.0.4/acenav_api/
--rw-r--r--   0 songyiwei   (501) staff       (20)      840 2024-03-29 01:03:49.000000 acenav_api-1.0.4/acenav_api/__init__.py
--rw-r--r--   0 songyiwei   (501) staff       (20)     3122 2024-03-29 01:03:44.000000 acenav_api-1.0.4/acenav_api/command_builder.py
-drwxr-xr-x   0 songyiwei   (501) staff       (20)        0 2024-04-01 07:23:56.000000 acenav_api-1.0.4/acenav_api/configs/
--rw-r--r--   0 songyiwei   (501) staff       (20)    40766 2024-04-01 07:20:42.000000 acenav_api-1.0.4/acenav_api/configs/INS502.json
--rw-r--r--   0 songyiwei   (501) staff       (20)    13043 2024-04-01 07:11:44.000000 acenav_api-1.0.4/acenav_api/field_parser.py
--rw-r--r--   0 songyiwei   (501) staff       (20)     9192 2024-04-01 07:21:31.000000 acenav_api-1.0.4/acenav_api/message_protocol.py
--rw-r--r--   0 songyiwei   (501) staff       (20)       45 2024-04-01 07:21:56.000000 acenav_api-1.0.4/acenav_api/package.py
--rw-r--r--   0 songyiwei   (501) staff       (20)     7947 2024-04-01 07:21:20.000000 acenav_api-1.0.4/acenav_api/packet_parser.py
--rw-r--r--   0 songyiwei   (501) staff       (20)     1603 2024-03-29 01:03:08.000000 acenav_api-1.0.4/acenav_api/utils.py
-drwxr-xr-x   0 songyiwei   (501) staff       (20)        0 2024-04-01 07:23:56.000000 acenav_api-1.0.4/acenav_api.egg-info/
--rw-r--r--   0 songyiwei   (501) staff       (20)     4195 2024-04-01 07:23:56.000000 acenav_api-1.0.4/acenav_api.egg-info/PKG-INFO
--rw-r--r--   0 songyiwei   (501) staff       (20)      382 2024-04-01 07:23:56.000000 acenav_api-1.0.4/acenav_api.egg-info/SOURCES.txt
--rw-r--r--   0 songyiwei   (501) staff       (20)        1 2024-04-01 07:23:56.000000 acenav_api-1.0.4/acenav_api.egg-info/dependency_links.txt
--rw-r--r--   0 songyiwei   (501) staff       (20)       11 2024-04-01 07:23:56.000000 acenav_api-1.0.4/acenav_api.egg-info/top_level.txt
--rw-r--r--   0 songyiwei   (501) staff       (20)       38 2024-04-01 07:23:56.000000 acenav_api-1.0.4/setup.cfg
--rw-r--r--   0 songyiwei   (501) staff       (20)     2094 2024-03-27 06:55:55.000000 acenav_api-1.0.4/setup.py
+drwxr-xr-x   0 songyiwei   (501) staff       (20)        0 2024-04-22 08:37:55.000000 acenav_api-1.0.5/
+-rw-r--r--   0 songyiwei   (501) staff       (20)     4195 2024-04-22 08:37:55.000000 acenav_api-1.0.5/PKG-INFO
+-rw-r--r--   0 songyiwei   (501) staff       (20)     3143 2024-03-29 01:58:30.000000 acenav_api-1.0.5/README.md
+drwxr-xr-x   0 songyiwei   (501) staff       (20)        0 2024-04-22 08:37:55.000000 acenav_api-1.0.5/acenav_api/
+-rw-r--r--   0 songyiwei   (501) staff       (20)      840 2024-03-29 01:03:49.000000 acenav_api-1.0.5/acenav_api/__init__.py
+-rw-r--r--   0 songyiwei   (501) staff       (20)     3122 2024-03-29 01:03:44.000000 acenav_api-1.0.5/acenav_api/command_builder.py
+drwxr-xr-x   0 songyiwei   (501) staff       (20)        0 2024-04-22 08:37:55.000000 acenav_api-1.0.5/acenav_api/configs/
+-rw-r--r--   0 songyiwei   (501) staff       (20)    37436 2024-04-22 08:25:22.000000 acenav_api-1.0.5/acenav_api/configs/INS502.json
+-rw-r--r--   0 songyiwei   (501) staff       (20)    14301 2024-04-22 08:28:58.000000 acenav_api-1.0.5/acenav_api/field_parser.py
+-rw-r--r--   0 songyiwei   (501) staff       (20)     9192 2024-04-01 07:21:31.000000 acenav_api-1.0.5/acenav_api/message_protocol.py
+-rw-r--r--   0 songyiwei   (501) staff       (20)       45 2024-04-22 08:36:22.000000 acenav_api-1.0.5/acenav_api/package.py
+-rw-r--r--   0 songyiwei   (501) staff       (20)     7947 2024-04-22 01:01:54.000000 acenav_api-1.0.5/acenav_api/packet_parser.py
+-rw-r--r--   0 songyiwei   (501) staff       (20)     1603 2024-03-29 01:03:08.000000 acenav_api-1.0.5/acenav_api/utils.py
+drwxr-xr-x   0 songyiwei   (501) staff       (20)        0 2024-04-22 08:37:55.000000 acenav_api-1.0.5/acenav_api.egg-info/
+-rw-r--r--   0 songyiwei   (501) staff       (20)     4195 2024-04-22 08:37:55.000000 acenav_api-1.0.5/acenav_api.egg-info/PKG-INFO
+-rw-r--r--   0 songyiwei   (501) staff       (20)      382 2024-04-22 08:37:55.000000 acenav_api-1.0.5/acenav_api.egg-info/SOURCES.txt
+-rw-r--r--   0 songyiwei   (501) staff       (20)        1 2024-04-22 08:37:55.000000 acenav_api-1.0.5/acenav_api.egg-info/dependency_links.txt
+-rw-r--r--   0 songyiwei   (501) staff       (20)       11 2024-04-22 08:37:55.000000 acenav_api-1.0.5/acenav_api.egg-info/top_level.txt
+-rw-r--r--   0 songyiwei   (501) staff       (20)       38 2024-04-22 08:37:55.000000 acenav_api-1.0.5/setup.cfg
+-rw-r--r--   0 songyiwei   (501) staff       (20)     2094 2024-03-27 06:55:55.000000 acenav_api-1.0.5/setup.py
```

### Comparing `acenav_api-1.0.4/PKG-INFO` & `acenav_api-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acenav_api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Aceinna Navigation System API
 Home-page: https://github.com/Aceinna
 Author: Aceinna, Inc
 Author-email: info@aceinna.com
 License: Apache 2.0
 Description: # A library to decode and encode data packet for Aceinna Devices
```

### Comparing `acenav_api-1.0.4/README.md` & `acenav_api-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `acenav_api-1.0.4/acenav_api/__init__.py` & `acenav_api-1.0.5/acenav_api/__init__.py`

 * *Files identical despite different names*

### Comparing `acenav_api-1.0.4/acenav_api/command_builder.py` & `acenav_api-1.0.5/acenav_api/command_builder.py`

 * *Files identical despite different names*

### Comparing `acenav_api-1.0.4/acenav_api/configs/INS502.json` & `acenav_api-1.0.5/acenav_api/configs/INS502.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944203320254492%*

 * *Differences: {"'payloads'": "{'S2': {0: {delete: ['unit', 'format']}, 1: {delete: ['format']}, 2: {'name': "*

 * *               "'accel_x', delete: ['format']}, 3: {'name': 'accel_y', delete: ['format']}, 4: "*

 * *               "{'name': 'accel_z', delete: ['format']}, 5: {'name': 'gyro_x', delete: "*

 * *               "['format']}, 6: {'name': 'gyro_y', delete: ['format']}, 7: {'name': 'gyro_z', "*

 * *               "delete: ['format']}, 8: {delete: ['format']}, 9: {'unit': 'bitmask', delete: "*

 * *               "['format']}, 10: {delet […]*

```diff
@@ -16,370 +16,320 @@
         "//rD_RESP": [],
         "//sC_REQ": [],
         "//sC_RESP": [],
         "//sR_REQ": [],
         "//sR_RESP": [],
         "DIAGNOSTIC": [
             {
-                "format": "",
                 "name": "gps_week",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
                 "name": "gps_millisecs",
                 "type": "uint32",
                 "unit": "ms"
             },
             {
-                "format": "",
                 "name": "master_BIT_status",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
                 "name": "hardware_BIT_status",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
                 "name": "hardware_error_code1",
-                "type": "uint8",
-                "unit": ""
+                "type": "uint8"
             },
             {
-                "format": "",
                 "name": "hardware_error_code2",
-                "type": "uint8",
-                "unit": ""
+                "type": "uint8"
             },
             {
-                "format": "",
                 "name": "software_BIT_status",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
                 "name": "software_error_code1",
-                "type": "uint8",
-                "unit": ""
+                "type": "uint8"
             },
             {
-                "format": "",
                 "name": "software_error_code2",
-                "type": "uint8",
-                "unit": ""
+                "type": "uint8"
+            },
+            {
+                "name": "reserved",
+                "type": "uint8_array"
             }
         ],
         "GI": [
             {
                 "name": "gps_week",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
                 "name": "gps_millisecs",
                 "type": "uint32",
                 "unit": "ms"
             },
             {
                 "name": "spp_fail_rate",
                 "scaling": "rate",
-                "type": "uint32",
-                "unit": ""
+                "type": "uint32"
             },
             {
                 "name": "rtk_fail_rate",
                 "scaling": "rate",
-                "type": "uint32",
-                "unit": ""
+                "type": "uint32"
             },
             {
                 "name": "spp_horizon_position_pl",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m"
             },
             {
                 "name": "spp_vertical_position_pl",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m"
             },
             {
                 "name": "spp_horizon_velocity_pl",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m/s"
             },
             {
                 "name": "spp_vertical_velocity_pl",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m/s"
             },
             {
                 "name": "rtk_horizon_position_pl",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m"
             },
             {
                 "name": "rtk_vertical_position_pl",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m"
             },
             {
                 "name": "rtk_horizon_velocity_pl",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m/s"
             },
             {
                 "name": "rtk_vertical_velocity_pl",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m/s"
             },
             {
                 "name": "rtk_heading_pl",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "deg"
             },
             {
                 "name": "spp_horizon_position_al",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m"
             },
             {
                 "name": "spp_vertical_position_al",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m"
             },
             {
                 "name": "spp_horizon_velocity_al",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m/s"
             },
             {
                 "name": "spp_vertical_velocity_al",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m/s"
             },
             {
                 "name": "rtk_horizon_position_al",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m"
             },
             {
                 "name": "rtk_vertical_position_al",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m"
             },
             {
                 "name": "rtk_horizon_velocity_al",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m/s"
             },
             {
                 "name": "rtk_vertical_velocity_al",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "m/s"
             },
             {
                 "name": "rtk_heading_al",
                 "scaling": "hundred",
                 "type": "uint16",
-                "unit": ""
+                "unit": "deg"
             },
             {
-                "name": "status",
-                "type": "uint16",
-                "unit": ""
+                "name": "pl_status",
+                "type": "uint16"
             }
         ],
         "GN": [
             {
-                "format": "",
                 "name": "gps_week",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
                 "name": "gps_millisecs",
                 "type": "uint32",
                 "unit": "ms"
             },
             {
-                "format": "",
-                "name": "solution_type",
-                "type": "uint8",
-                "unit": ""
+                "name": "gnss_solution_type",
+                "type": "uint8"
             },
             {
-                "format": "",
                 "name": "latitude",
                 "scaling": "position",
                 "type": "int32",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "longitude",
                 "scaling": "position",
                 "type": "int32",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "height",
                 "type": "float",
                 "unit": "m"
             },
             {
-                "format": "",
-                "name": "number_of_SVs",
-                "type": "uint8",
-                "unit": ""
+                "name": "satellite_count_in_view",
+                "type": "uint8"
             },
             {
-                "format": "",
-                "name": "number_of_SVs_in_solution",
-                "type": "uint8",
-                "unit": ""
+                "name": "satellite_count_in_solution",
+                "type": "uint8"
             },
             {
-                "format": "",
                 "name": "rtcm_correction_status",
-                "type": "uint8",
-                "unit": ""
+                "type": "uint8"
             },
             {
-                "format": "",
                 "name": "hdop",
                 "scaling": "hundred",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
                 "name": "vdop",
                 "scaling": "hundred",
-                "type": "float",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
                 "name": "tdop",
                 "scaling": "hundred",
-                "type": "float",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
-                "name": "diffage",
+                "name": "diff_age",
                 "type": "uint16",
                 "unit": "s"
             },
             {
-                "format": "",
                 "name": "north_vel",
                 "scaling": "hundred",
                 "type": "int16",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "east_vel",
                 "scaling": "hundred",
                 "type": "int16",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "up_vel",
                 "scaling": "hundred",
                 "type": "int16",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "latitude_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "longitude_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "height_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "m"
             },
             {
-                "format": "",
                 "name": "north_vel_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "east_vel_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "up_vel_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "m/s"
             },
             {
-                "format": "",
-                "name": "primary_snr",
+                "name": "primary_cn0",
                 "type": "uint8",
                 "unit": "db-Hz"
             },
             {
-                "format": "",
-                "name": "secondary_snr",
+                "name": "secondary_cn0",
                 "type": "uint8",
                 "unit": "db-Hz"
             }
         ],
         "HS": [
             {
                 "name": "gps_week",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
                 "name": "gps_millisecs",
                 "type": "uint32",
                 "unit": "ms"
             },
             {
@@ -389,60 +339,53 @@
             {
                 "name": "length",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "m"
             },
             {
-                "name": "heading",
                 "scaling": "hundred",
                 "type": "uint16",
                 "unit": "deg"
             },
             {
                 "name": "pitch",
                 "scaling": "hundred",
                 "type": "int16",
                 "unit": "deg"
             },
             {
-                "name": "roll",
                 "scaling": "hundred",
                 "type": "int16",
                 "unit": "deg"
             },
             {
                 "name": "heading_std",
-                "scaling": "hundred",
+                "scaling": "thousand",
                 "type": "uint16",
                 "unit": "deg"
             },
             {
                 "name": "length_std",
-                "scaling": "hundred",
-                "type": "uint16",
-                "unit": "m"
+                "scaling": "thousand",
+                "type": "uint16"
             },
             {
-                "name": "numberOfSVsInView",
-                "type": "uint8",
-                "unit": ""
+                "name": "secondary_satellite_count_in_view",
+                "type": "uint8"
             },
             {
-                "name": "numberOfSVInDualAntenna",
-                "scaling": "hundred",
-                "type": "uint8",
-                "unit": "m"
+                "name": "secondary_satellite_count_in_solution",
+                "type": "uint8"
             }
         ],
         "II": [
             {
                 "name": "gps_week",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
                 "name": "gps_millisecs",
                 "type": "uint32",
                 "unit": "ms"
             },
             {
@@ -466,384 +409,316 @@
             {
                 "name": "vertical_velocity_pl",
                 "scaling": "hundred",
                 "type": "uint16",
                 "unit": "m/s"
             },
             {
-                "name": "pitch_pl",
                 "scaling": "hundred",
                 "type": "uint16",
                 "unit": "deg"
             },
             {
-                "name": "roll_pl",
                 "scaling": "hundred",
                 "type": "uint16",
                 "unit": "deg"
             },
             {
                 "name": "heading_pl",
                 "scaling": "hundred",
                 "type": "uint16",
                 "unit": "deg"
             },
             {
                 "name": "status",
-                "type": "uint8",
-                "unit": ""
+                "type": "uint8"
             }
         ],
         "IN": [
             {
-                "format": "",
                 "name": "gps_week",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
                 "name": "gps_millisecs",
                 "type": "uint32",
                 "unit": "ms"
             },
             {
-                "format": "",
                 "name": "ins_status",
-                "type": "uint8",
-                "unit": ""
+                "type": "uint8"
             },
             {
-                "format": "",
-                "name": "solution_type",
-                "type": "uint8",
-                "unit": ""
+                "name": "gnss_solution_type",
+                "type": "uint8"
             },
             {
-                "format": "",
                 "name": "latitude",
                 "scaling": "position",
                 "type": "int32",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "longitude",
                 "scaling": "position",
                 "type": "int32",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "height",
                 "type": "float",
                 "unit": "m"
             },
             {
-                "format": "",
                 "name": "north_vel",
                 "scaling": "hundred",
                 "type": "int16",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "east_vel",
                 "scaling": "hundred",
                 "type": "int16",
                 "unit": "m/s"
             },
             {
-                "format": "10.4f",
-                "name": "up_velocity",
+                "name": "up_vel",
+                "scaling": "hundred",
                 "type": "int16",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "roll",
                 "scaling": "hundred",
-                "type": "uint16",
+                "type": "int16",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "pitch",
                 "scaling": "hundred",
-                "type": "uint16",
+                "type": "int16",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "heading",
                 "scaling": "hundred",
                 "type": "uint16",
                 "unit": "deg"
             },
             {
-                "format": "",
-                "name": "longitudinal_velocity",
+                "name": "long_vel",
                 "scaling": "hundred",
                 "type": "int16",
                 "unit": "m/s"
             },
             {
-                "format": "",
-                "name": "lateral_velocity",
+                "name": "lat_vel",
                 "scaling": "hundred",
                 "type": "int16",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "latitude_std",
                 "scaling": "thousand",
                 "type": "uint16",
-                "unit": "m"
+                "unit": "deg"
             },
             {
-                "format": "",
                 "name": "longitude_std",
                 "scaling": "thousand",
                 "type": "uint16",
-                "unit": "m"
+                "unit": "deg"
             },
             {
-                "format": "",
                 "name": "height_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "m"
             },
             {
-                "format": "",
-                "name": "north_velocity_std",
+                "name": "north_vel_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "m/s"
             },
             {
-                "format": "",
-                "name": "east_velocity_std",
+                "name": "east_vel_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "m/s"
             },
             {
-                "format": "",
-                "name": "up_velocity_std",
+                "name": "up_vel_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "long_vel_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "lat_vel_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "roll_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "pitch_std",
-                "scaling": "hundred",
+                "scaling": "thousand",
                 "type": "uint16",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "heading_std",
                 "scaling": "thousand",
                 "type": "uint16",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "ins_stage_and_gnss_rejection_status",
-                "type": "uint8",
-                "unit": ""
+                "type": "uint8"
             }
         ],
         "IR": [
             {
-                "name": "algorithm_buf",
+                "name": "algorithmBuf",
                 "type": "uint8_array"
             }
         ],
         "ODO": [
             {
-                "format": "",
                 "name": "gps_week",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
                 "name": "gps_millisecs",
                 "type": "uint32",
                 "unit": "ms"
             },
             {
-                "format": "",
                 "name": "mode",
-                "type": "uint8",
-                "unit": ""
+                "type": "uint8"
             },
             {
-                "format": "",
                 "name": "speed",
                 "type": "double",
                 "unit": "m/s"
             },
             {
-                "format": "",
                 "name": "fwd",
-                "type": "uint8",
-                "unit": ""
+                "type": "int8"
             },
             {
-                "format": "16",
                 "name": "wheel_tick",
-                "type": "uint64",
-                "unit": ""
+                "type": "uint64"
             }
         ],
         "RR": [
             {
                 "name": "piece_data",
                 "type": "uint8_array"
             }
         ],
         "S2": [
             {
-                "format": "",
                 "name": "gps_week",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
                 "name": "gps_millisecs",
                 "type": "uint32",
                 "unit": "ms"
             },
             {
-                "format": "",
-                "name": "x_accel",
+                "name": "accel_x",
                 "type": "float",
                 "unit": "m/s^2"
             },
             {
-                "format": "",
-                "name": "y_accel",
+                "name": "accel_y",
                 "type": "float",
                 "unit": "m/s^2"
             },
             {
-                "format": "",
-                "name": "z_accel",
+                "name": "accel_z",
                 "type": "float",
                 "unit": "m/s^2"
             },
             {
-                "format": "",
-                "name": "x_gyro",
+                "name": "gyro_x",
                 "type": "float",
                 "unit": "deg/s"
             },
             {
-                "format": "",
-                "name": "y_gyro",
+                "name": "gyro_y",
                 "type": "float",
                 "unit": "deg/s"
             },
             {
-                "format": "",
-                "name": "z_gyro",
+                "name": "gyro_z",
                 "type": "float",
                 "unit": "deg/s"
             },
             {
-                "format": "",
                 "name": "temperature",
                 "type": "float",
                 "unit": "deg C"
             },
             {
-                "format": "",
                 "name": "masterStatus",
                 "type": "uint16",
-                "unit": ""
+                "unit": "bitmask"
             },
             {
-                "format": "",
                 "name": "reserved",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             }
         ],
         "SV": [
             {
-                "format": "",
                 "name": "gps_week",
-                "type": "uint16",
-                "unit": ""
+                "type": "uint16"
             },
             {
-                "format": "",
                 "name": "gps_millisecs",
                 "type": "uint32",
                 "unit": "ms"
             },
             {
-                "format": "",
                 "name": "system_id",
-                "type": "uint8",
-                "unit": "ms"
+                "type": "uint8"
             },
             {
-                "format": "",
                 "name": "satellite_id",
-                "type": "uint8",
-                "unit": ""
+                "type": "uint8"
             },
             {
-                "format": "",
                 "name": "antenna_type",
-                "type": "uint8",
-                "unit": ""
+                "type": "uint8"
             },
             {
-                "format": "",
                 "name": "cn0",
                 "type": "uint8",
                 "unit": "db-Hz"
             },
             {
-                "format": "",
                 "name": "azimuth",
                 "type": "float",
                 "unit": "deg"
             },
             {
-                "format": "",
                 "name": "elevation",
                 "type": "float",
                 "unit": "deg"
             }
         ],
         "T1": [
             {
@@ -851,35 +726,35 @@
                 "type": "uint16"
             },
             {
                 "name": "total",
                 "type": "uint16"
             },
             {
-                "name": "trace_buf",
+                "name": "traceBuf",
                 "type": "uint8_array"
             }
         ],
         "T2": [
             {
                 "name": "sequence",
                 "type": "uint16"
             },
             {
                 "name": "total",
                 "type": "uint16"
             },
             {
-                "name": "trace_buf",
+                "name": "traceBuf",
                 "type": "uint8_array"
             }
         ],
         "aV_RESP": [
             {
-                "name": "version",
+                "name": "algorithmVersion",
                 "type": "string"
             }
         ],
         "cA_REQ": [
             {
                 "name": "speed",
                 "type": "float"
@@ -895,25 +770,25 @@
             {
                 "name": "result",
                 "type": "int8"
             }
         ],
         "gB_REQ": [
             {
-                "name": "param_nums",
+                "name": "paramNums",
                 "type": "uint8"
             },
             {
                 "name": "param_ids",
                 "type": "uint8_array"
             }
         ],
         "gB_RESP": [
             {
-                "name": "param_nums",
+                "name": "paramNums",
                 "type": "uint8"
             },
             {
                 "name": "parameters",
                 "type": "parameter_array"
             }
         ],
@@ -979,14 +854,18 @@
             {
                 "name": "interface_type",
                 "type": "uint8"
             }
         ],
         "lO_RESP": [
             {
+                "name": "packetNums",
+                "type": "uint8"
+            },
+            {
                 "name": "outputs",
                 "type": "output_array"
             }
         ],
         "oT_REQ": [
             {
                 "name": "operation",
@@ -1009,34 +888,42 @@
                 "type": "uint8"
             },
             {
                 "name": "reserve",
                 "type": "uint8"
             },
             {
-                "name": "time_of_interrupt",
+                "name": "timeOfInterrupt",
                 "type": "uint16"
             }
         ],
         "rG_RESP": [
             {
                 "name": "gps_millisecs",
                 "type": "uint32"
             }
         ],
         "sO_REQ": [
             {
+                "name": "packetNums",
+                "type": "uint8"
+            },
+            {
                 "name": "outputs",
                 "type": "output_update_array"
             }
         ],
         "sO_RESP": [
             {
-                "name": "result",
-                "type": "int8"
+                "name": "packetNums",
+                "type": "uint8"
+            },
+            {
+                "name": "outputs",
+                "type": "output_update_result_array"
             }
         ],
         "sV_REQ": [
             {
                 "name": "component",
                 "type": "uint8"
             }
@@ -1049,95 +936,95 @@
             {
                 "name": "version",
                 "type": "string"
             }
         ],
         "uB_REQ": [
             {
-                "name": "param_count",
+                "name": "paramNums",
                 "type": "uint8"
             },
             {
                 "name": "parameters",
                 "type": "parameter_array"
             }
         ],
         "uB_RESP": [
             {
-                "name": "param_count",
+                "name": "paramNums",
                 "type": "uint8"
             },
             {
                 "name": "parameters",
                 "type": "update_result_array"
             }
         ],
         "wA_data_REQ": [
             {
-                "name": "packet_type",
+                "name": "packetType",
                 "type": "uint8"
             },
             {
-                "name": "packet_index",
+                "name": "packetIndex",
                 "type": "uint8"
             },
             {
-                "name": "algorithm_payload",
+                "name": "algorithmPayload",
                 "type": "uint8_array"
             }
         ],
         "wA_data_RESP": [
             {
-                "name": "packet_type",
+                "name": "packetType",
                 "type": "uint8"
             },
             {
-                "name": "packet_index",
+                "name": "packetIndex",
                 "type": "uint8"
             },
             {
-                "name": "error_code",
+                "name": "errorCode",
                 "type": "uint16"
             }
         ],
         "wA_start_REQ": [
             {
-                "name": "packet_type",
+                "name": "packetType",
                 "type": "uint8"
             },
             {
-                "name": "total_packet",
+                "name": "totalPacket",
                 "type": "uint8"
             },
             {
-                "name": "total_size",
+                "name": "totalSize",
                 "type": "uint16"
             }
         ],
         "wA_start_RESP": [
             {
-                "name": "packet_type",
+                "name": "packetType",
                 "type": "uint8"
             },
             {
-                "name": "error_code",
+                "name": "errorCode",
                 "type": "uint16"
             }
         ],
         "wS_REQ": [
             {
                 "name": "content_type",
                 "type": "uint8"
             },
             {
                 "name": "serial_number",
                 "type": "uint32"
             }
         ],
-        "ws_RESP": [
+        "wS_RESP": [
             {
                 "name": "result",
                 "type": "int8"
             }
         ]
     },
     "scaling": {
```

### Comparing `acenav_api-1.0.4/acenav_api/field_parser.py` & `acenav_api-1.0.5/acenav_api/field_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1,401 @@
-import randomimport structimport decimalfrom typing import List, Any,Unionfrom .message_protocol import ParameterConfBASIC_DATA_TYPES = [    'int8','uint8','int16','uint16','int32','uint32','int64','uint64','float','double']EXTEND_DATA_TYPES = [    'string',     'uint8_array',    'output_array', # List of packet_type(uint16), odr(uint8)    'output_update_array',]PARAMETERS_DATA_TYPES = ['parameter_array','update_result_array']PARAMETER_DATA_TYPES = ['orientation','IPV4','IPV6','mac_address']    ORIENTATION_MAPPING = {  '+Ux+Uy+Uz': 0x0000,  '-Ux-Uy+Uz': 0x0009,  '-Uy+Ux+Uz': 0x0023,  '+Uy-Ux+Uz': 0x002A,  '-Ux+Uy-Uz': 0x0041,  '+Ux-Uy-Uz': 0x0048,  '+Uy+Ux-Uz': 0x0062,  '-Uy-Ux-Uz': 0x006B,  '-Uz+Uy+Ux': 0x0085,  '+Uz-Uy+Ux': 0x008C,  '+Uy+Uz+Ux': 0x0092,  '-Uy-Uz+Ux': 0x009B,  '+Uz+Uy-Ux': 0x00C4,  '-Uz-Uy-Ux': 0x00CD,  '-Uy+Uz-Ux': 0x00D3,  '+Uy-Uz-Ux': 0x00DA,  '-Ux+Uz+Uy': 0x0111,  '+Ux-Uz+Uy': 0x0118,  '+Uz+Ux+Uy': 0x0124,  '-Uz-Ux+Uy': 0x012D,  '+Ux+Uz-Uy': 0x0150,  '-Ux-Uz-Uy': 0x0159,  '-Uz+Ux-Uy': 0x0165,  '+Uz-Ux-Uy': 0x016C,}def build_fmt(fmt:str, endian:str)->str:    if endian == 'lsb':        return '<'+fmt    else:        return '>'+fmtdef decode_field(data_type:str, endian:str, payload:bytes, start:int, precision:int=0)->Union[int,float,str,bytes]:    result = None    if data_type == 'uint64':        result = (struct.unpack(build_fmt('Q',endian), payload[start:start+8])[0],8)    elif data_type == 'int64':        result = (struct.unpack(build_fmt('q',endian), payload[start:start+8])[0],8)    elif data_type == 'double':        result = (struct.unpack(build_fmt('d',endian), payload[start:start+8])[0],8)    elif data_type == 'uint32':        result = (struct.unpack(build_fmt('I',endian), payload[start:start+4])[0],4)    elif data_type == 'int32':        result = (struct.unpack(build_fmt('i',endian), payload[start:start+4])[0],4)    elif data_type == 'float':        # use decimal, float type is a special case        unpack_value = struct.unpack(build_fmt('f',endian), payload[start:start+4])[0]        if precision > 0 :            decimal_wrapped = decimal.Decimal(unpack_value)            try:                unpack_value = float(round(decimal_wrapped, precision))            except:                unpack_value = 0        result = (unpack_value, 4)    elif data_type == 'uint16':        result = (struct.unpack(build_fmt('H',endian), payload[start:start+2])[0],2)    elif data_type == 'int16':        result = (struct.unpack(build_fmt('h',endian), payload[start:start+2])[0],2)    elif data_type == 'uint8':        result = (struct.unpack('B', payload[start:start+1])[0],1)    elif data_type == 'int8':        result = (struct.unpack('b', payload[start:start+1])[0],1)    else:        raise ValueError('Decode failed, unknown data type: {0}'.format(data_type))    return resultdef encode_field(data_type:str, endian:str, value:int)->bytes:    payload = bytearray()    if data_type == 'uint64':        payload = struct.pack(build_fmt('Q',endian), value)    elif data_type == 'int64':        payload = struct.pack(build_fmt('q',endian), value)    elif data_type == 'double':        payload = struct.pack(build_fmt('d',endian), value)    elif data_type == 'uint32':        payload = struct.pack(build_fmt('I',endian), value)    elif data_type == 'int32':        payload = struct.pack(build_fmt('i',endian), value)    elif data_type == 'float':        payload = struct.pack(build_fmt('f',endian), value)    elif data_type == 'uint16':        payload = struct.pack(build_fmt('H',endian), value)    elif data_type == 'int16':        payload = struct.pack(build_fmt('h',endian), value)    elif data_type == 'uint8':        payload = struct.pack(build_fmt('B',endian), value)    elif data_type == 'int8':        payload = struct.pack(build_fmt('b',endian), value)    else:        raise ValueError('Encode failed, unknown data type: {0}'.format(data_type))    return payloaddef decode_extend_field(data_type:str, payload:bytes, start:int):    '''Cover string, uint8_array, output_array, output_update_array, orientation    '''    result = None    field_payload = payload[start:]    if data_type == 'string':        result = (field_payload.decode('utf-8'), len(field_payload))    elif data_type == 'uint8_array':        result = (list(field_payload), len(field_payload))    elif data_type == 'output_array':        result = __decode_output_array(field_payload)    elif data_type == 'output_update_array':        result = __decode_output_update_array(field_payload)    else:        raise ValueError('Decode failed, unknown extend data type: {0}'.format(data_type))        return resultdef encode_extend_field(data_type:str, value:Any)->bytes:    '''Cover string, uint8_array, output_array, output_update_array, orientation    '''    payload = bytearray()        if data_type == 'string':        payload = value.encode('utf-8')    elif data_type == 'uint8_array':        payload = bytes(value)    elif data_type == 'output_array':        payload = __encode_output_array(value)    elif data_type == 'output_update_array':        payload = __encode_output_update_array(value)    else:        raise ValueError('Encode failed, unknown extend data type: {0}'.format(data_type))        return payloaddef decode_parameters_field(data_type:str, parameters: List[ParameterConf], payload:bytes, start:int)->bytes:    '''parameter_array, update_result_array    '''    result = None    if data_type == 'parameter_array':        result = __decode_parameter_array(parameters, payload[start:])    elif data_type == 'update_result_array':        result =__decode_update_result(parameters, payload[start:])    else:        raise ValueError('Decode failed, unknown parameters data type: {0}'.format(data_type))        return resultdef encode_parameters_field(data_type:str, parameters: List[ParameterConf], value:int)->bytes:    '''parameter_array, update_result_array    '''    payload = bytearray()        if data_type == 'parameter_array':        payload = __encode_parameter_array(parameters, value)    elif data_type == 'update_result_array':        payload = __encode_update_result(parameters, value)    else:        raise ValueError('Encode failed, unknown parameters data type: {0}'.format(data_type))        return payloaddef __decode_output_array(payload:bytes):    '''List of packet_type(uint16), odr(uint8)    '''    result = []    for i in range(0, len(payload), 3):        packet_type = decode_field('uint16', 'lsb', payload, i)[0]        odr = decode_field('uint8', 'lsb', payload, i+2)[0]        result.append({'packet_type':packet_type, 'odr':odr})        return result,len(payload)def __encode_output_array(value:dict):    payload = bytearray()    for item in value:        packet_type = encode_field('uint16', 'lsb', item['packet_type'])        odr = encode_field('uint8', 'lsb', item['odr'])        payload.extend(packet_type)        payload.extend(odr)            return payloaddef __decode_output_update_array(payload:bytes):    '''List of packet_type(uint16), interface_type(uint8), odr(uint8)    '''    result = []        for i in range(0, len(payload), 4):        packet_type = decode_field('uint16', 'lsb', payload, i)[0]        interface = decode_field('uint8', 'lsb', payload, i+2)[0]        odr = decode_field('uint8', 'lsb', payload, i+3)[0]        result.append({'packet_type':packet_type, 'interface_type':interface, 'odr':odr})        return result,len(payload)def __encode_output_update_array(value:dict):    payload = bytearray()        for item in value:        packet_type = encode_field('uint16', 'lsb', item['packet_type'])        interface = encode_field('uint8', 'lsb', item['interface_type'])        odr = encode_field('uint8', 'lsb', item['odr'])                payload.extend(packet_type)        payload.extend(interface)        payload.extend(odr)        return payloaddef __decode_parameter_array(parameters: List[ParameterConf], payload:bytes):    '''parameter_array = List of parameter_id(uint8), parameter_len(uint8), parameter_value(length is parameter_len)    '''    result = []    start = 0    while start < len(payload):        param_id = payload[start]        param_len = payload[start+1]        param_value_start = start+2        param_conf = next((p for p in parameters if p.param_id == param_id), None)        # TODO: handle param_conf is None        value, data_len = __decode_parameter_field(param_conf, payload[param_value_start:param_value_start+param_len])        result.append({            'param_id':param_id,            'name': param_conf.name,            'value':value        })        start = start + param_value_start + data_len        return result, len(payload)def __encode_parameter_array(parameters: List[ParameterConf], value:List[Any])->bytes:    '''parameter_array    '''    payload = bytearray()    for item in value:        param_conf = next((p for p in parameters if p.param_id == item['param_id']), None)        # TODO: handle param_conf is None        param_id = encode_field('uint8', 'lsb', item['param_id'])        param_value = __encode_parameter_field(param_conf, item['value'])        param_len = encode_field('uint8', 'lsb', len(param_value))         payload.extend(param_id)        payload.extend(param_len)        payload.extend(param_value)        return payloaddef __decode_update_result(parameters: List[ParameterConf], payload:bytes):    '''update_result_array = List of parameter_id(uint8), update_result(int8)    '''    result = []    start = 0    while start < len(payload):        param_id = payload[start]        update_result = decode_field('int8','lsb', payload,1)[0]        result.append({            'param_id':param_id,            'result':update_result        })        start = start + 2        return result,len(payload)def __encode_update_result(parameters: List[ParameterConf], value:List[Any])->bytes:    '''update_result_array = List of parameter_id(uint8), update_result(uint8)    '''    payload = bytearray()    for item in value:        param_id = encode_field('uint8', 'lsb', item['param_id'])        update_result = encode_field('int8', 'lsb', item['result'])                payload.extend(param_id)        payload.extend(update_result)        return payloaddef __decode_parameter_field(param_conf: ParameterConf, payload:bytes):    '''payattention to IPv4, IPv6, mac_address    '''    data_type = param_conf.type    if data_type in BASIC_DATA_TYPES:        return decode_field(data_type, param_conf.endian, payload, 0, param_conf.precision)    elif data_type == 'orientation':        return __decode_orientation(payload)    else:        raise ValueError('Decode failed, unknown parameter field data type: {0}'.format(data_type))def __encode_parameter_field(param_conf: ParameterConf, value:Any)->bytes:    '''payattention to IPv4, IPv6, mac_address    '''    data_type = param_conf.type    if data_type in BASIC_DATA_TYPES:        return encode_field(data_type, param_conf.endian, value)    elif data_type == 'orientation':        return __encode_orientation(value)    else:        raise ValueError('Encode failed, unknown parameter field data type: {0}'.format(data_type))def __decode_orientation(payload:bytes):    '''orienation(uint16), convert to a string value    '''    value = decode_field('uint16', 'lsb', payload, 0)[0]    #find value in ORIENTATION_MAPPING, and get the key    for key in ORIENTATION_MAPPING:        if ORIENTATION_MAPPING[key] == value:            return key,2        return '+Ux+Uy+Uz',2def __encode_orientation(value:str):    '''From a string value to orientation(uint16)    '''    if value in ORIENTATION_MAPPING:        return encode_field('uint16', 'lsb', ORIENTATION_MAPPING[value])    return bytes([0x00, 0x00])def build_random_value(data_type:str)->Union[int,float]:    if data_type == 'uint64':        return random.randint(0,18446744073709551615)    elif data_type == 'int64':        return random.randint(-9223372036854775808,9223372036854775807)    elif data_type == 'uint32':        return random.randint(0,4294967295)    elif data_type == 'int32':        return random.randint(-2147483648,2147483647)    elif data_type == 'uint16':        return random.randint(0,65535)    elif data_type == 'int16':        return random.randint(-32768,32767)    elif data_type == 'uint8':        return random.randint(0,255)    elif data_type == 'int8':        return random.randint(-128,127)    elif data_type == 'double':        return random.random()    elif data_type == 'float':        return random.random()    elif data_type == 'uint8_array':        return bytes([random.randint(0,255) for i in range(0,20)])    else:        raise ValueError('Build random value failed, unknown data type: {0}'.format(data_type))
+import random
+import struct
+import decimal
+from typing import List, Any,Union
+from .message_protocol import ParameterConf
+
+BASIC_DATA_TYPES = [
+    'int8','uint8','int16','uint16','int32','uint32','int64','uint64','float','double'
+]
+
+EXTEND_DATA_TYPES = [
+    'string', 
+    'uint8_array',
+    'output_array', # List of packet_type(uint16), odr(uint8)
+    'output_update_array',
+    'output_update_result_array'
+]
+
+PARAMETERS_DATA_TYPES = ['parameter_array','update_result_array']
+
+PARAMETER_DATA_TYPES = ['orientation','IPV4','IPV6','mac_address']
+    
+ORIENTATION_MAPPING = {
+  '+Ux+Uy+Uz': 0x0000,
+  '-Ux-Uy+Uz': 0x0009,
+  '-Uy+Ux+Uz': 0x0023,
+  '+Uy-Ux+Uz': 0x002A,
+  '-Ux+Uy-Uz': 0x0041,
+  '+Ux-Uy-Uz': 0x0048,
+  '+Uy+Ux-Uz': 0x0062,
+  '-Uy-Ux-Uz': 0x006B,
+  '-Uz+Uy+Ux': 0x0085,
+  '+Uz-Uy+Ux': 0x008C,
+  '+Uy+Uz+Ux': 0x0092,
+  '-Uy-Uz+Ux': 0x009B,
+  '+Uz+Uy-Ux': 0x00C4,
+  '-Uz-Uy-Ux': 0x00CD,
+  '-Uy+Uz-Ux': 0x00D3,
+  '+Uy-Uz-Ux': 0x00DA,
+  '-Ux+Uz+Uy': 0x0111,
+  '+Ux-Uz+Uy': 0x0118,
+  '+Uz+Ux+Uy': 0x0124,
+  '-Uz-Ux+Uy': 0x012D,
+  '+Ux+Uz-Uy': 0x0150,
+  '-Ux-Uz-Uy': 0x0159,
+  '-Uz+Ux-Uy': 0x0165,
+  '+Uz-Ux-Uy': 0x016C,
+}
+
+def build_fmt(fmt:str, endian:str)->str:
+    if endian == 'lsb':
+        return '<'+fmt
+    else:
+        return '>'+fmt
+
+def decode_field(data_type:str, endian:str, payload:bytes, start:int, precision:int=0)->Union[int,float,str,bytes]:
+    result = None
+    if data_type == 'uint64':
+        result = (struct.unpack(build_fmt('Q',endian), payload[start:start+8])[0],8)
+    elif data_type == 'int64':
+        result = (struct.unpack(build_fmt('q',endian), payload[start:start+8])[0],8)
+    elif data_type == 'double':
+        result = (struct.unpack(build_fmt('d',endian), payload[start:start+8])[0],8)
+    elif data_type == 'uint32':
+        result = (struct.unpack(build_fmt('I',endian), payload[start:start+4])[0],4)
+    elif data_type == 'int32':
+        result = (struct.unpack(build_fmt('i',endian), payload[start:start+4])[0],4)
+    elif data_type == 'float':
+        # use decimal, float type is a special case
+        unpack_value = struct.unpack(build_fmt('f',endian), payload[start:start+4])[0]
+        if precision > 0 :
+            decimal_wrapped = decimal.Decimal(unpack_value)
+            try:
+                unpack_value = float(round(decimal_wrapped, precision))
+            except:
+                unpack_value = 0
+        result = (unpack_value, 4)
+    elif data_type == 'uint16':
+        result = (struct.unpack(build_fmt('H',endian), payload[start:start+2])[0],2)
+    elif data_type == 'int16':
+        result = (struct.unpack(build_fmt('h',endian), payload[start:start+2])[0],2)
+    elif data_type == 'uint8':
+        result = (struct.unpack('B', payload[start:start+1])[0],1)
+    elif data_type == 'int8':
+        result = (struct.unpack('b', payload[start:start+1])[0],1)
+    else:
+        raise ValueError('Decode failed, unknown data type: {0}'.format(data_type))
+
+    return result
+
+def encode_field(data_type:str, endian:str, value:int)->bytes:
+    payload = bytearray()
+
+    if data_type == 'uint64':
+        payload = struct.pack(build_fmt('Q',endian), value)
+    elif data_type == 'int64':
+        payload = struct.pack(build_fmt('q',endian), value)
+    elif data_type == 'double':
+        payload = struct.pack(build_fmt('d',endian), value)
+    elif data_type == 'uint32':
+        payload = struct.pack(build_fmt('I',endian), value)
+    elif data_type == 'int32':
+        payload = struct.pack(build_fmt('i',endian), value)
+    elif data_type == 'float':
+        payload = struct.pack(build_fmt('f',endian), value)
+    elif data_type == 'uint16':
+        payload = struct.pack(build_fmt('H',endian), value)
+    elif data_type == 'int16':
+        payload = struct.pack(build_fmt('h',endian), value)
+    elif data_type == 'uint8':
+        payload = struct.pack(build_fmt('B',endian), value)
+    elif data_type == 'int8':
+        payload = struct.pack(build_fmt('b',endian), value)
+    else:
+        raise ValueError('Encode failed, unknown data type: {0}'.format(data_type))
+    return payload
+
+def decode_extend_field(data_type:str, payload:bytes, start:int):
+    '''Cover string, uint8_array, output_array, output_update_array, orientation
+    '''
+    result = None
+
+    field_payload = payload[start:]
+    if data_type == 'string':
+        result = (field_payload.decode('utf-8'), len(field_payload))
+    elif data_type == 'uint8_array':
+        result = (list(field_payload), len(field_payload))
+    elif data_type == 'output_array':
+        result = __decode_output_array(field_payload)
+    elif data_type == 'output_update_array':
+        result = __decode_output_update_array(field_payload)
+    elif data_type == 'output_update_result_array':
+        result = __decode_output_update_result_array(field_payload)
+    else:
+        raise ValueError('Decode failed, unknown extend data type: {0}'.format(data_type))
+    
+    return result
+
+def encode_extend_field(data_type:str, value:Any)->bytes:
+    '''Cover string, uint8_array, output_array, output_update_array, orientation
+    '''
+    payload = bytearray()
+    
+    if data_type == 'string':
+        payload = value.encode('utf-8')
+    elif data_type == 'uint8_array':
+        payload = bytes(value)
+    elif data_type == 'output_array':
+        payload = __encode_output_array(value)
+    elif data_type == 'output_update_array':
+        payload = __encode_output_update_array(value)
+    elif data_type == 'output_update_result_array':
+        payload = __encode_output_update_result_array(value)
+    else:
+        raise ValueError('Encode failed, unknown extend data type: {0}'.format(data_type))
+    
+    return payload
+
+def decode_parameters_field(data_type:str, parameters: List[ParameterConf], payload:bytes, start:int)->bytes:
+    '''parameter_array, update_result_array
+    '''
+    result = None
+    if data_type == 'parameter_array':
+        result = __decode_parameter_array(parameters, payload[start:])
+    elif data_type == 'update_result_array':
+        result =__decode_update_result(parameters, payload[start:])
+    else:
+        raise ValueError('Decode failed, unknown parameters data type: {0}'.format(data_type))
+    
+    return result
+
+def encode_parameters_field(data_type:str, parameters: List[ParameterConf], value:int)->bytes:
+    '''parameter_array, update_result_array
+    '''
+    payload = bytearray()
+    
+    if data_type == 'parameter_array':
+        payload = __encode_parameter_array(parameters, value)
+    elif data_type == 'update_result_array':
+        payload = __encode_update_result(parameters, value)
+    else:
+        raise ValueError('Encode failed, unknown parameters data type: {0}'.format(data_type))
+    
+    return payload
+
+def __decode_output_array(payload:bytes):
+    '''List of packet_type(uint16), odr(uint8)
+    '''
+    result = []
+    for i in range(0, len(payload), 3):
+        packet_type = decode_field('uint16', 'lsb', payload, i)[0]
+        odr = decode_field('uint8', 'lsb', payload, i+2)[0]
+
+        result.append({'packet_type':packet_type, 'odr':odr})
+    
+    return result,len(payload)
+
+def __encode_output_array(value:dict):
+    payload = bytearray()
+    for item in value:
+        packet_type = encode_field('uint16', 'lsb', item['packet_type'])
+        odr = encode_field('uint8', 'lsb', item['odr'])
+        payload.extend(packet_type)
+        payload.extend(odr)
+        
+    return payload
+
+def __decode_output_update_array(payload:bytes):
+    '''List of packet_type(uint16), interface_type(uint8), odr(uint8)
+    '''
+    result = []
+    
+    for i in range(0, len(payload), 4):
+        packet_type = decode_field('uint16', 'lsb', payload, i)[0]
+        interface = decode_field('uint8', 'lsb', payload, i+2)[0]
+        odr = decode_field('uint8', 'lsb', payload, i+3)[0]
+
+        result.append({'packet_type':packet_type, 'interface_type':interface, 'odr':odr})
+    
+    return result,len(payload)
+
+def __encode_output_update_array(value:dict):
+    payload = bytearray()
+    
+    for item in value:
+        packet_type = encode_field('uint16', 'lsb', item['packet_type'])
+        interface = encode_field('uint8', 'lsb', item['interface_type'])
+        odr = encode_field('uint8', 'lsb', item['odr'])
+        
+        payload.extend(packet_type)
+        payload.extend(interface)
+        payload.extend(odr)
+    
+    return payload
+
+def __decode_output_update_result_array(payload:bytes):
+    '''List of packet_type(uint16), interface_type(uint8), result(uint8)
+    '''
+    result = []
+    
+    for i in range(0, len(payload), 4):
+        packet_type = decode_field('uint16', 'lsb', payload, i)[0]
+        interface = decode_field('uint8', 'lsb', payload, i+2)[0]
+        update_result = decode_field('uint8', 'lsb', payload, i+3)[0]
+
+        result.append({'packet_type':packet_type, 'interface_type':interface, 'result':update_result})
+    
+    return result,len(payload)
+
+def __encode_output_update_result_array(value:dict):
+    payload = bytearray()
+    
+    for item in value:
+        packet_type = encode_field('uint16', 'lsb', item['packet_type'])
+        interface = encode_field('uint8', 'lsb', item['interface_type'])
+        result = encode_field('uint8', 'lsb', item['result'])
+        
+        payload.extend(packet_type)
+        payload.extend(interface)
+        payload.extend(result)
+    
+    return payload
+
+def __decode_parameter_array(parameters: List[ParameterConf], payload:bytes):
+    '''parameter_array = List of parameter_id(uint8), parameter_len(uint8), parameter_value(length is parameter_len)
+    '''
+    result = []
+    start = 0
+    while start < len(payload):
+        param_id = payload[start]
+        param_len = payload[start+1]
+        param_value_start = start+2
+
+        param_conf = next((p for p in parameters if p.param_id == param_id), None)
+        # TODO: handle param_conf is None
+
+        value, data_len = __decode_parameter_field(param_conf, payload[param_value_start:param_value_start+param_len])
+        result.append({
+            'param_id':param_id,
+            'name': param_conf.name,
+            'value':value
+        })
+        start = start + param_value_start + data_len
+    
+    return result, len(payload)
+
+def __encode_parameter_array(parameters: List[ParameterConf], value:List[Any])->bytes:
+    '''parameter_array
+    '''
+    payload = bytearray()
+
+    for item in value:
+        param_conf = next((p for p in parameters if p.param_id == item['param_id']), None)
+        # TODO: handle param_conf is None
+
+        param_id = encode_field('uint8', 'lsb', item['param_id'])
+        param_value = __encode_parameter_field(param_conf, item['value'])
+        param_len = encode_field('uint8', 'lsb', len(param_value)) 
+
+        payload.extend(param_id)
+        payload.extend(param_len)
+        payload.extend(param_value)
+    
+    return payload
+
+def __decode_update_result(parameters: List[ParameterConf], payload:bytes):
+    '''update_result_array = List of parameter_id(uint8), update_result(int8)
+    '''
+    result = []
+    start = 0
+
+    while start < len(payload):
+        param_id = payload[start]
+        update_result = decode_field('int8','lsb', payload,1)[0]
+        result.append({
+            'param_id':param_id,
+            'result':update_result
+        })
+        start = start + 2
+    
+    return result,len(payload)
+
+def __encode_update_result(parameters: List[ParameterConf], value:List[Any])->bytes:
+    '''update_result_array = List of parameter_id(uint8), update_result(uint8)
+    '''
+    payload = bytearray()
+    for item in value:
+        param_id = encode_field('uint8', 'lsb', item['param_id'])
+        update_result = encode_field('int8', 'lsb', item['result'])
+        
+        payload.extend(param_id)
+        payload.extend(update_result)
+    
+    return payload
+
+def __decode_parameter_field(param_conf: ParameterConf, payload:bytes):
+    '''payattention to IPv4, IPv6, mac_address
+    '''
+    data_type = param_conf.type
+    if data_type in BASIC_DATA_TYPES:
+        return decode_field(data_type, param_conf.endian, payload, 0, param_conf.precision)
+    elif data_type == 'orientation':
+        return __decode_orientation(payload)
+    else:
+        raise ValueError('Decode failed, unknown parameter field data type: {0}'.format(data_type))
+
+def __encode_parameter_field(param_conf: ParameterConf, value:Any)->bytes:
+    '''payattention to IPv4, IPv6, mac_address
+    '''
+    data_type = param_conf.type
+    if data_type in BASIC_DATA_TYPES:
+        return encode_field(data_type, param_conf.endian, value)
+    elif data_type == 'orientation':
+        return __encode_orientation(value)
+    else:
+        raise ValueError('Encode failed, unknown parameter field data type: {0}'.format(data_type))
+
+def __decode_orientation(payload:bytes):
+    '''orienation(uint16), convert to a string value
+    '''
+    value = decode_field('uint16', 'lsb', payload, 0)[0]
+    #find value in ORIENTATION_MAPPING, and get the key
+    for key in ORIENTATION_MAPPING:
+        if ORIENTATION_MAPPING[key] == value:
+            return key,2
+    
+    return '+Ux+Uy+Uz',2
+
+def __encode_orientation(value:str):
+    '''From a string value to orientation(uint16)
+    '''
+    if value in ORIENTATION_MAPPING:
+        return encode_field('uint16', 'lsb', ORIENTATION_MAPPING[value])
+
+    return bytes([0x00, 0x00])
+
+def build_random_value(data_type:str)->Union[int,float]:
+    if data_type == 'uint64':
+        return random.randint(0,18446744073709551615)
+    elif data_type == 'int64':
+        return random.randint(-9223372036854775808,9223372036854775807)
+    elif data_type == 'uint32':
+        return random.randint(0,4294967295)
+    elif data_type == 'int32':
+        return random.randint(-2147483648,2147483647)
+    elif data_type == 'uint16':
+        return random.randint(0,65535)
+    elif data_type == 'int16':
+        return random.randint(-32768,32767)
+    elif data_type == 'uint8':
+        return random.randint(0,255)
+    elif data_type == 'int8':
+        return random.randint(-128,127)
+    elif data_type == 'double':
+        return random.random()
+    elif data_type == 'float':
+        return random.random()
+    elif data_type == 'uint8_array':
+        return bytes([random.randint(0,255) for i in range(0,20)])
+    else:
+        raise ValueError('Build random value failed, unknown data type: {0}'.format(data_type))
```

### Comparing `acenav_api-1.0.4/acenav_api/message_protocol.py` & `acenav_api-1.0.5/acenav_api/message_protocol.py`

 * *Files identical despite different names*

### Comparing `acenav_api-1.0.4/acenav_api/packet_parser.py` & `acenav_api-1.0.5/acenav_api/packet_parser.py`

 * *Files identical despite different names*

### Comparing `acenav_api-1.0.4/acenav_api/utils.py` & `acenav_api-1.0.5/acenav_api/utils.py`

 * *Files identical despite different names*

### Comparing `acenav_api-1.0.4/acenav_api.egg-info/PKG-INFO` & `acenav_api-1.0.5/acenav_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acenav-api
-Version: 1.0.4
+Version: 1.0.5
 Summary: Aceinna Navigation System API
 Home-page: https://github.com/Aceinna
 Author: Aceinna, Inc
 Author-email: info@aceinna.com
 License: Apache 2.0
 Description: # A library to decode and encode data packet for Aceinna Devices
```

### Comparing `acenav_api-1.0.4/setup.py` & `acenav_api-1.0.5/setup.py`

 * *Files identical despite different names*

