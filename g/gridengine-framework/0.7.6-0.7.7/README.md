# Comparing `tmp/gridengine_framework-0.7.6.tar.gz` & `tmp/gridengine_framework-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridengine_framework-0.7.6.tar", last modified: Mon Apr 22 05:11:27 2024, max compression
+gzip compressed data, was "gridengine_framework-0.7.7.tar", last modified: Mon Apr 22 06:04:05 2024, max compression
```

## Comparing `gridengine_framework-0.7.6.tar` & `gridengine_framework-0.7.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/
--rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.7.6/LICENSE
--rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     5278 2023-11-02 07:42:03.000000 gridengine_framework-0.7.6/README.md
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/
--rw-r--r--   0 boss      (1000) boss      (1002)      135 2023-11-25 03:11:25.000000 gridengine_framework-0.7.6/grid_engine/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     1293 2023-11-28 08:03:58.000000 gridengine_framework-0.7.6/grid_engine/__log__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4931 2023-12-10 21:45:39.000000 gridengine_framework-0.7.6/grid_engine/__main__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_blueprint/
--rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3624 2024-04-22 04:56:11.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/__main__.py
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2024-01-11 22:32:29.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/_floorplan_classes.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5608 2024-02-11 03:43:12.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/_floorplan_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)    17503 2024-04-22 05:11:05.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/_grid_blueprint.py
--rw-r--r--   0 boss      (1000) boss      (1002)    18503 2024-02-12 03:03:41.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/_grid_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)    10946 2024-04-22 05:08:00.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/_terrain_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)      272 2024-04-22 02:43:45.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/objects.json
--rw-r--r--   0 boss      (1000) boss      (1002)     1615 2024-04-22 04:53:36.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/terrains.json
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_cell/
--rw-r--r--   0 boss      (1000) boss      (1002)       22 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_cell/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    32323 2024-04-22 01:48:00.000000 gridengine_framework-0.7.6/grid_engine/_cell/cell.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4756 2023-11-25 03:11:01.000000 gridengine_framework-0.7.6/grid_engine/_dungeon.py
--rw-r--r--   0 boss      (1000) boss      (1002)    54707 2024-04-22 01:43:28.000000 gridengine_framework-0.7.6/grid_engine/_grid.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_grid_feature/
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_feature/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2442 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_feature/grid_feature.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_grid_group/
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_group/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3642 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_group/grid_group.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_grid_object/
--rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/__init__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_item/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_item/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_item/grid_item.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2283 2023-11-12 05:05:46.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_object.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_structure/
--rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_structure/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2216 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_structure/grid_structure.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_zone/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_zone/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_zone/grid_zone.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/grid_engine/_terraform/
--rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_terraform/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    10775 2024-02-12 03:10:30.000000 gridengine_framework-0.7.6/grid_engine/_terraform/terraformer.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5714 2024-02-24 16:00:59.000000 gridengine_framework-0.7.6/grid_engine/_utility.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2925 2024-02-12 03:13:00.000000 gridengine_framework-0.7.6/grid_engine/layout_test.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/gridengine_framework.egg-info/
--rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 05:11:27.000000 gridengine_framework-0.7.6/gridengine_framework.egg-info/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     1439 2024-04-22 05:11:27.000000 gridengine_framework-0.7.6/gridengine_framework.egg-info/SOURCES.txt
--rw-r--r--   0 boss      (1000) boss      (1002)        1 2024-04-22 05:11:27.000000 gridengine_framework-0.7.6/gridengine_framework.egg-info/dependency_links.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-22 05:11:27.000000 gridengine_framework-0.7.6/gridengine_framework.egg-info/requires.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       12 2024-04-22 05:11:27.000000 gridengine_framework-0.7.6/gridengine_framework.egg-info/top_level.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       38 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/setup.cfg
--rw-r--r--   0 boss      (1000) boss      (1002)      903 2024-04-22 05:11:14.000000 gridengine_framework-0.7.6/setup.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.609880 gridengine_framework-0.7.7/
+-rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.7.7/LICENSE
+-rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 06:04:05.609880 gridengine_framework-0.7.7/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     5278 2023-11-02 07:42:03.000000 gridengine_framework-0.7.7/README.md
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.606546 gridengine_framework-0.7.7/grid_engine/
+-rw-r--r--   0 boss      (1000) boss      (1002)      135 2023-11-25 03:11:25.000000 gridengine_framework-0.7.7/grid_engine/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     1293 2023-11-28 08:03:58.000000 gridengine_framework-0.7.7/grid_engine/__log__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4931 2023-12-10 21:45:39.000000 gridengine_framework-0.7.7/grid_engine/__main__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.606546 gridengine_framework-0.7.7/grid_engine/_blueprint/
+-rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.7.7/grid_engine/_blueprint/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3624 2024-04-22 04:56:11.000000 gridengine_framework-0.7.7/grid_engine/_blueprint/__main__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2024-01-11 22:32:29.000000 gridengine_framework-0.7.7/grid_engine/_blueprint/_floorplan_classes.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5608 2024-02-11 03:43:12.000000 gridengine_framework-0.7.7/grid_engine/_blueprint/_floorplan_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    17503 2024-04-22 05:11:05.000000 gridengine_framework-0.7.7/grid_engine/_blueprint/_grid_blueprint.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    18503 2024-02-12 03:03:41.000000 gridengine_framework-0.7.7/grid_engine/_blueprint/_grid_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    10946 2024-04-22 05:08:00.000000 gridengine_framework-0.7.7/grid_engine/_blueprint/_terrain_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)      272 2024-04-22 02:43:45.000000 gridengine_framework-0.7.7/grid_engine/_blueprint/objects.json
+-rw-r--r--   0 boss      (1000) boss      (1002)     1615 2024-04-22 04:53:36.000000 gridengine_framework-0.7.7/grid_engine/_blueprint/terrains.json
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.606546 gridengine_framework-0.7.7/grid_engine/_cell/
+-rw-r--r--   0 boss      (1000) boss      (1002)       22 2024-04-22 05:54:10.000000 gridengine_framework-0.7.7/grid_engine/_cell/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    32374 2024-04-22 05:54:03.000000 gridengine_framework-0.7.7/grid_engine/_cell/cell.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4756 2023-11-25 03:11:01.000000 gridengine_framework-0.7.7/grid_engine/_dungeon.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    54735 2024-04-22 06:03:38.000000 gridengine_framework-0.7.7/grid_engine/_grid.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.606546 gridengine_framework-0.7.7/grid_engine/_grid_feature/
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.7/grid_engine/_grid_feature/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2442 2023-10-31 05:21:50.000000 gridengine_framework-0.7.7/grid_engine/_grid_feature/grid_feature.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.609880 gridengine_framework-0.7.7/grid_engine/_grid_group/
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.7/grid_engine/_grid_group/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3642 2023-10-31 05:21:50.000000 gridengine_framework-0.7.7/grid_engine/_grid_group/grid_group.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.609880 gridengine_framework-0.7.7/grid_engine/_grid_object/
+-rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.7.7/grid_engine/_grid_object/__init__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.609880 gridengine_framework-0.7.7/grid_engine/_grid_object/grid_item/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.7/grid_engine/_grid_object/grid_item/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.7.7/grid_engine/_grid_object/grid_item/grid_item.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2283 2023-11-12 05:05:46.000000 gridengine_framework-0.7.7/grid_engine/_grid_object/grid_object.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.609880 gridengine_framework-0.7.7/grid_engine/_grid_object/grid_structure/
+-rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.7.7/grid_engine/_grid_object/grid_structure/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2216 2023-10-31 05:21:50.000000 gridengine_framework-0.7.7/grid_engine/_grid_object/grid_structure/grid_structure.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.609880 gridengine_framework-0.7.7/grid_engine/_grid_object/grid_zone/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.7/grid_engine/_grid_object/grid_zone/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.7.7/grid_engine/_grid_object/grid_zone/grid_zone.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.609880 gridengine_framework-0.7.7/grid_engine/_terraform/
+-rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.7.7/grid_engine/_terraform/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    11793 2024-04-22 06:03:14.000000 gridengine_framework-0.7.7/grid_engine/_terraform/terraformer.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5714 2024-02-24 16:00:59.000000 gridengine_framework-0.7.7/grid_engine/_utility.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2925 2024-02-12 03:13:00.000000 gridengine_framework-0.7.7/grid_engine/layout_test.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:04:05.609880 gridengine_framework-0.7.7/gridengine_framework.egg-info/
+-rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 06:04:05.000000 gridengine_framework-0.7.7/gridengine_framework.egg-info/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     1439 2024-04-22 06:04:05.000000 gridengine_framework-0.7.7/gridengine_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)        1 2024-04-22 06:04:05.000000 gridengine_framework-0.7.7/gridengine_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-22 06:04:05.000000 gridengine_framework-0.7.7/gridengine_framework.egg-info/requires.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       12 2024-04-22 06:04:05.000000 gridengine_framework-0.7.7/gridengine_framework.egg-info/top_level.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       38 2024-04-22 06:04:05.609880 gridengine_framework-0.7.7/setup.cfg
+-rw-r--r--   0 boss      (1000) boss      (1002)      903 2024-04-22 06:03:55.000000 gridengine_framework-0.7.7/setup.py
```

### Comparing `gridengine_framework-0.7.6/LICENSE` & `gridengine_framework-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/PKG-INFO` & `gridengine_framework-0.7.7/gridengine_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gridengine_framework
-Version: 0.7.6
+Name: gridengine-framework
+Version: 0.7.7
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gridengine_framework-0.7.6/README.md` & `gridengine_framework-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/__log__.py` & `gridengine_framework-0.7.7/grid_engine/__log__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/__main__.py` & `gridengine_framework-0.7.7/grid_engine/__main__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_blueprint/__main__.py` & `gridengine_framework-0.7.7/grid_engine/_blueprint/__main__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_blueprint/_floorplan_processing.py` & `gridengine_framework-0.7.7/grid_engine/_blueprint/_floorplan_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_blueprint/_grid_blueprint.py` & `gridengine_framework-0.7.7/grid_engine/_blueprint/_grid_blueprint.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_blueprint/_grid_processing.py` & `gridengine_framework-0.7.7/grid_engine/_blueprint/_grid_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_blueprint/_terrain_processing.py` & `gridengine_framework-0.7.7/grid_engine/_blueprint/_terrain_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_blueprint/terrains.json` & `gridengine_framework-0.7.7/grid_engine/_blueprint/terrains.json`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_cell/cell.py` & `gridengine_framework-0.7.7/grid_engine/_cell/cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 from collections import deque
 
+from .._grid_group import GridGroup
+
 import logging as _logging
 
 from abc import ABC
 from typing import Optional as _Optional, Union as _Union
 import weakref
 import numpy as np
 import pyglet
 
+
 _ZONE_COLOR_MAP = {
         'regions' : (255, 0, 0, 255)
 }
 
 
 def capture_parentgrid(cls):
     def decorator(cell=None,  parentgrid=None):
@@ -764,14 +767,15 @@
         elif otype == 'structures':
             self.on_construct(grid_object)
             if hasattr(grid_object, 'tile_color') and getattr(self.parentgrid, 'scene', None) is not None:
                 self.overlay_color = grid_object.tile_color
                 self.overlay = self.paint_overlay(batch=self.parentgrid.scene.batch_delegate.cell_batch)
             if hasattr(grid_object, 'passable'):
                 self.passable = grid_object.passable
+            
         
     def remove_object(self, grid_object):
         """Removes a GridObject from the cell. Updates the entry_object attribute. Also updates the grid array.
         """
         otype = f'{grid_object.object_type}s'
         if self.entry_object[f'{otype}'][grid_object.name] is not None:
             self.entry_object[f'{otype}'][grid_object.name] = None
```

### Comparing `gridengine_framework-0.7.6/grid_engine/_dungeon.py` & `gridengine_framework-0.7.7/grid_engine/_dungeon.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_grid.py` & `gridengine_framework-0.7.7/grid_engine/_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,14 +492,15 @@
             self.lake_count = len(self.lakes)
             self._set_water_cells()
             self.river_count = 0
             self.rivers: list[list[_Cell,]] = []
             self._terraformer = Terraformer(self)
             self.terraformer.set_rivers(2)
             self._fix_minute_water_bodies()
+            self.set_forests()
 
         # self.town = GridZone(self, 'Town', 'town', self.random_cell(attr=('passable', True)), (45, 45, 45), 2)
 
     def _size_warning(self, cell_count):
         import colorama
         quit = input(
             f'{colorama.Fore.RED}WARNING{colorama.Fore.RESET}: The provided parameters will generate a grid composed '
@@ -693,15 +694,15 @@
                 nearest['distance'] = distance
             elif nearest['distance'] == distance:
                 nearest['cell'].append(cellb)
             return nearest
 
         def check_qualifications(qualifications, cellb):
             for entry, qualifier in qualifications.items():
-                if qualifier == '_any' and _any(getattr(cellb, f'entry_{entry}').values()):
+                if qualifier == 'any' and any(getattr(cellb, f'entry_{entry}').values()):
                     return True
                 elif qualifier == 'all' and all(getattr(cellb, f'entry_{entry}').values()):
                     return True
                 elif isinstance(  # check if qualifications[entry] is a dict
                         qualifier,  # and if so
                         dict
                 ) and (
@@ -803,15 +804,15 @@
         #         return cell
         return self.cells[self.grid_array[rank, file, 0]['designation']]
 
     @_log_method
     def random_cell(
             self,
             attr: _Optional[tuple[str, _Any]] = None,
-            attrs: _Optional[tuple[tuple[str, _any]]] = None,
+            attrs: _Optional[tuple[tuple[str, _Any]]] = None,
             landmass_index: _Optional[int] = None
     ) -> _Optional[_Cell]:
         """Returns a _random cell. If an attribute is provided, the cell must have that attribute. If multiple
         attributes are provided, the cell must have all attributes. If a landmass index is provided, the cell must be
         in that landmass.
         
         Args:
@@ -825,15 +826,15 @@
             cell with terrain string 'GRASS'.
             ```grid.random_cell(landmass_index=0)``` returns a _random cell in the first landmass.
         """
         if landmass_index is not None:
             cell = _choice(self.landmasses[landmass_index]['landmass_cells'])
         elif attrs is not None:
             cell = self.cells[_choice(self.blueprint.cell_list)]
-            while _any(getattr(cell, attr[0]) != attr[1] for attr in attrs):
+            while any(getattr(cell, attr[0]) != attr[1] for attr in attrs):
                 cell = self.cells[_choice(self.blueprint.cell_list)]
         elif attr is not None:
             cell = self.cells[_choice(self.blueprint.cell_list)]
             while getattr(cell, attr[0]) != attr[1]:
                 cell = self.cells[_choice(self.blueprint.cell_list)]
         else:
             cell = self.cells[_choice(self.blueprint.cell_list)]
```

### Comparing `gridengine_framework-0.7.6/grid_engine/_grid_feature/grid_feature.py` & `gridengine_framework-0.7.7/grid_engine/_grid_feature/grid_feature.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_grid_group/grid_group.py` & `gridengine_framework-0.7.7/grid_engine/_grid_group/grid_group.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_grid_object/grid_item/grid_item.py` & `gridengine_framework-0.7.7/grid_engine/_grid_object/grid_item/grid_item.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_grid_object/grid_object.py` & `gridengine_framework-0.7.7/grid_engine/_grid_object/grid_object.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_grid_object/grid_structure/grid_structure.py` & `gridengine_framework-0.7.7/grid_engine/_grid_object/grid_structure/grid_structure.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_grid_object/grid_zone/grid_zone.py` & `gridengine_framework-0.7.7/grid_engine/_grid_object/grid_zone/grid_zone.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/_terraform/terraformer.py` & `gridengine_framework-0.7.7/grid_engine/_terraform/terraformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -240,8 +240,31 @@
                     print(f'Start cell: {start}, End cell: {end}', end = '\r')
             print(f'Start cell: {start}, End cell: {end}')
             print('Building river ...')
             self.generate_realistic_river(start.designation, end.designation)
         riverbanks = self.get_river_banks()
         self.expand_riverbanks(riverbanks)
         print('done')            
- 
+ 
+    def set_forests(self, forest_count=1):
+        for forest in range(forest_count):
+            center = self.grid.random_cell(('passable', True))
+            while center.clearance_y < 5 or center.clearance_x < 5:
+                center = self.grid.random_cell(('passable', True))
+            area = self.grid.get_area(center, 4)
+            for cell in area:
+                cell.terrain_str = 'FOREST'
+                cell.terrain_char = '^'
+                cell.terrain_raw = 0.0
+                cell.terrain_int = None
+                cell.terrain_color = 'GRASS_GREEN'
+                cell.cost_in = 2
+                cell.cost_out = 2
+                self.dictTerrain[cell.designation] = {
+                    'str': cell.terrain_str, 
+                    'raw': cell.terrain_raw, 
+                    'int': cell.terrain_int, 
+                    'color': cell.terrain_color, 
+                    'cost_in': cell.cost_in, 
+                    'cost_out': cell.cost_out
+                    }
+
```

### Comparing `gridengine_framework-0.7.6/grid_engine/_utility.py` & `gridengine_framework-0.7.7/grid_engine/_utility.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/grid_engine/layout_test.py` & `gridengine_framework-0.7.7/grid_engine/layout_test.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/gridengine_framework.egg-info/PKG-INFO` & `gridengine_framework-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gridengine-framework
-Version: 0.7.6
+Name: gridengine_framework
+Version: 0.7.7
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gridengine_framework-0.7.6/gridengine_framework.egg-info/SOURCES.txt` & `gridengine_framework-0.7.7/gridengine_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.6/setup.py` & `gridengine_framework-0.7.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
     
 setup(
     name='gridengine_framework',
-    version='0.7.6',
+    version='0.7.7',
     description='A framework for generating and manipulating grid-based game worlds',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='James Evans',
     author_email='joesaysahoy@gmail.com',
     url='https://github.com/primal-coder/grid-engine',
     packages=find_packages(),
```

