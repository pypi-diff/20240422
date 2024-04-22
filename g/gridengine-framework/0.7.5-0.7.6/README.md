# Comparing `tmp/gridengine_framework-0.7.5.tar.gz` & `tmp/gridengine_framework-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridengine_framework-0.7.5.tar", last modified: Mon Apr 22 05:08:33 2024, max compression
+gzip compressed data, was "gridengine_framework-0.7.6.tar", last modified: Mon Apr 22 05:11:27 2024, max compression
```

## Comparing `gridengine_framework-0.7.5.tar` & `gridengine_framework-0.7.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.788689 gridengine_framework-0.7.5/
--rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.7.5/LICENSE
--rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 05:08:33.788689 gridengine_framework-0.7.5/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     5278 2023-11-02 07:42:03.000000 gridengine_framework-0.7.5/README.md
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.785356 gridengine_framework-0.7.5/grid_engine/
--rw-r--r--   0 boss      (1000) boss      (1002)      135 2023-11-25 03:11:25.000000 gridengine_framework-0.7.5/grid_engine/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     1293 2023-11-28 08:03:58.000000 gridengine_framework-0.7.5/grid_engine/__log__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4931 2023-12-10 21:45:39.000000 gridengine_framework-0.7.5/grid_engine/__main__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.785356 gridengine_framework-0.7.5/grid_engine/_blueprint/
--rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.7.5/grid_engine/_blueprint/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3624 2024-04-22 04:56:11.000000 gridengine_framework-0.7.5/grid_engine/_blueprint/__main__.py
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2024-01-11 22:32:29.000000 gridengine_framework-0.7.5/grid_engine/_blueprint/_floorplan_classes.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5608 2024-02-11 03:43:12.000000 gridengine_framework-0.7.5/grid_engine/_blueprint/_floorplan_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)    17805 2024-04-22 05:07:37.000000 gridengine_framework-0.7.5/grid_engine/_blueprint/_grid_blueprint.py
--rw-r--r--   0 boss      (1000) boss      (1002)    18503 2024-02-12 03:03:41.000000 gridengine_framework-0.7.5/grid_engine/_blueprint/_grid_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)    10946 2024-04-22 05:08:00.000000 gridengine_framework-0.7.5/grid_engine/_blueprint/_terrain_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)      272 2024-04-22 02:43:45.000000 gridengine_framework-0.7.5/grid_engine/_blueprint/objects.json
--rw-r--r--   0 boss      (1000) boss      (1002)     1615 2024-04-22 04:53:36.000000 gridengine_framework-0.7.5/grid_engine/_blueprint/terrains.json
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.785356 gridengine_framework-0.7.5/grid_engine/_cell/
--rw-r--r--   0 boss      (1000) boss      (1002)       22 2023-10-31 05:21:50.000000 gridengine_framework-0.7.5/grid_engine/_cell/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    32323 2024-04-22 01:48:00.000000 gridengine_framework-0.7.5/grid_engine/_cell/cell.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4756 2023-11-25 03:11:01.000000 gridengine_framework-0.7.5/grid_engine/_dungeon.py
--rw-r--r--   0 boss      (1000) boss      (1002)    54707 2024-04-22 01:43:28.000000 gridengine_framework-0.7.5/grid_engine/_grid.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.785356 gridengine_framework-0.7.5/grid_engine/_grid_feature/
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.5/grid_engine/_grid_feature/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2442 2023-10-31 05:21:50.000000 gridengine_framework-0.7.5/grid_engine/_grid_feature/grid_feature.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.785356 gridengine_framework-0.7.5/grid_engine/_grid_group/
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.5/grid_engine/_grid_group/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3642 2023-10-31 05:21:50.000000 gridengine_framework-0.7.5/grid_engine/_grid_group/grid_group.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.785356 gridengine_framework-0.7.5/grid_engine/_grid_object/
--rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.7.5/grid_engine/_grid_object/__init__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.788689 gridengine_framework-0.7.5/grid_engine/_grid_object/grid_item/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.5/grid_engine/_grid_object/grid_item/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.7.5/grid_engine/_grid_object/grid_item/grid_item.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2283 2023-11-12 05:05:46.000000 gridengine_framework-0.7.5/grid_engine/_grid_object/grid_object.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.788689 gridengine_framework-0.7.5/grid_engine/_grid_object/grid_structure/
--rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.7.5/grid_engine/_grid_object/grid_structure/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2216 2023-10-31 05:21:50.000000 gridengine_framework-0.7.5/grid_engine/_grid_object/grid_structure/grid_structure.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.788689 gridengine_framework-0.7.5/grid_engine/_grid_object/grid_zone/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.5/grid_engine/_grid_object/grid_zone/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.7.5/grid_engine/_grid_object/grid_zone/grid_zone.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.788689 gridengine_framework-0.7.5/grid_engine/_terraform/
--rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.7.5/grid_engine/_terraform/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    10775 2024-02-12 03:10:30.000000 gridengine_framework-0.7.5/grid_engine/_terraform/terraformer.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5714 2024-02-24 16:00:59.000000 gridengine_framework-0.7.5/grid_engine/_utility.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2925 2024-02-12 03:13:00.000000 gridengine_framework-0.7.5/grid_engine/layout_test.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:08:33.788689 gridengine_framework-0.7.5/gridengine_framework.egg-info/
--rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 05:08:33.000000 gridengine_framework-0.7.5/gridengine_framework.egg-info/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     1439 2024-04-22 05:08:33.000000 gridengine_framework-0.7.5/gridengine_framework.egg-info/SOURCES.txt
--rw-r--r--   0 boss      (1000) boss      (1002)        1 2024-04-22 05:08:33.000000 gridengine_framework-0.7.5/gridengine_framework.egg-info/dependency_links.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-22 05:08:33.000000 gridengine_framework-0.7.5/gridengine_framework.egg-info/requires.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       12 2024-04-22 05:08:33.000000 gridengine_framework-0.7.5/gridengine_framework.egg-info/top_level.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       38 2024-04-22 05:08:33.788689 gridengine_framework-0.7.5/setup.cfg
--rw-r--r--   0 boss      (1000) boss      (1002)      903 2024-04-22 05:08:17.000000 gridengine_framework-0.7.5/setup.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/
+-rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.7.6/LICENSE
+-rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     5278 2023-11-02 07:42:03.000000 gridengine_framework-0.7.6/README.md
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/
+-rw-r--r--   0 boss      (1000) boss      (1002)      135 2023-11-25 03:11:25.000000 gridengine_framework-0.7.6/grid_engine/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     1293 2023-11-28 08:03:58.000000 gridengine_framework-0.7.6/grid_engine/__log__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4931 2023-12-10 21:45:39.000000 gridengine_framework-0.7.6/grid_engine/__main__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_blueprint/
+-rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3624 2024-04-22 04:56:11.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/__main__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2024-01-11 22:32:29.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/_floorplan_classes.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5608 2024-02-11 03:43:12.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/_floorplan_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    17503 2024-04-22 05:11:05.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/_grid_blueprint.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    18503 2024-02-12 03:03:41.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/_grid_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    10946 2024-04-22 05:08:00.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/_terrain_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)      272 2024-04-22 02:43:45.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/objects.json
+-rw-r--r--   0 boss      (1000) boss      (1002)     1615 2024-04-22 04:53:36.000000 gridengine_framework-0.7.6/grid_engine/_blueprint/terrains.json
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_cell/
+-rw-r--r--   0 boss      (1000) boss      (1002)       22 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_cell/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    32323 2024-04-22 01:48:00.000000 gridengine_framework-0.7.6/grid_engine/_cell/cell.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4756 2023-11-25 03:11:01.000000 gridengine_framework-0.7.6/grid_engine/_dungeon.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    54707 2024-04-22 01:43:28.000000 gridengine_framework-0.7.6/grid_engine/_grid.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_grid_feature/
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_feature/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2442 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_feature/grid_feature.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_grid_group/
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_group/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3642 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_group/grid_group.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_grid_object/
+-rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/__init__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.043467 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_item/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_item/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_item/grid_item.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2283 2023-11-12 05:05:46.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_object.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_structure/
+-rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_structure/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2216 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_structure/grid_structure.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_zone/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_zone/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.7.6/grid_engine/_grid_object/grid_zone/grid_zone.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/grid_engine/_terraform/
+-rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.7.6/grid_engine/_terraform/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    10775 2024-02-12 03:10:30.000000 gridengine_framework-0.7.6/grid_engine/_terraform/terraformer.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5714 2024-02-24 16:00:59.000000 gridengine_framework-0.7.6/grid_engine/_utility.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2925 2024-02-12 03:13:00.000000 gridengine_framework-0.7.6/grid_engine/layout_test.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/gridengine_framework.egg-info/
+-rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 05:11:27.000000 gridengine_framework-0.7.6/gridengine_framework.egg-info/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     1439 2024-04-22 05:11:27.000000 gridengine_framework-0.7.6/gridengine_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)        1 2024-04-22 05:11:27.000000 gridengine_framework-0.7.6/gridengine_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-22 05:11:27.000000 gridengine_framework-0.7.6/gridengine_framework.egg-info/requires.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       12 2024-04-22 05:11:27.000000 gridengine_framework-0.7.6/gridengine_framework.egg-info/top_level.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       38 2024-04-22 05:11:27.046800 gridengine_framework-0.7.6/setup.cfg
+-rw-r--r--   0 boss      (1000) boss      (1002)      903 2024-04-22 05:11:14.000000 gridengine_framework-0.7.6/setup.py
```

### Comparing `gridengine_framework-0.7.5/LICENSE` & `gridengine_framework-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/PKG-INFO` & `gridengine_framework-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridengine_framework
-Version: 0.7.5
+Version: 0.7.6
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gridengine_framework-0.7.5/README.md` & `gridengine_framework-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/__log__.py` & `gridengine_framework-0.7.6/grid_engine/__log__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/__main__.py` & `gridengine_framework-0.7.6/grid_engine/__main__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_blueprint/__main__.py` & `gridengine_framework-0.7.6/grid_engine/_blueprint/__main__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_blueprint/_floorplan_processing.py` & `gridengine_framework-0.7.6/grid_engine/_blueprint/_floorplan_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_blueprint/_grid_blueprint.py` & `gridengine_framework-0.7.6/grid_engine/_blueprint/_grid_blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,20 +410,14 @@
             self, cell_size: int, grid_dimensions: tuple[int, int], grid_id: str = None, noise_scale: int = None,
             noise_octaves: int = None, noise_roughness: float = None
     ):
         super(TerrainGridBlueprint, self).__init__(cell_size, grid_dimensions, grid_id)
         for cell in self.dictGrid:
             self.dictGrid[cell]['passable'] = None
         self._init_terrain(noise_scale, noise_octaves, noise_roughness)
-        for cell in self.cells:
-            for k, v in self.dictObject[cell].items():
-                for ok, ov in v.items():
-                    if v[ok] is not None:
-                        self.cells[cell].terrain_color = v[ok]['color']
-                        self.cells[cell].terrain_char = '^'
 
     def _init_terrain(self, noise_scale, noise_octaves, noise_roughness):
         self._noise_scale = noise_scale if noise_scale is not None else 350
         self._noise_octaves = noise_octaves if noise_octaves is not None else 88
         self._noise_roughness = noise_roughness if noise_roughness is not None else 0.65
         self.dictTerrain = process_noise(
             self._noise_scale, self._noise_octaves, self._noise_roughness, self._row_count, self._col_count,
```

### Comparing `gridengine_framework-0.7.5/grid_engine/_blueprint/_grid_processing.py` & `gridengine_framework-0.7.6/grid_engine/_blueprint/_grid_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_blueprint/_terrain_processing.py` & `gridengine_framework-0.7.6/grid_engine/_blueprint/_terrain_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_blueprint/terrains.json` & `gridengine_framework-0.7.6/grid_engine/_blueprint/terrains.json`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_cell/cell.py` & `gridengine_framework-0.7.6/grid_engine/_cell/cell.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_dungeon.py` & `gridengine_framework-0.7.6/grid_engine/_dungeon.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_grid.py` & `gridengine_framework-0.7.6/grid_engine/_grid.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_grid_feature/grid_feature.py` & `gridengine_framework-0.7.6/grid_engine/_grid_feature/grid_feature.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_grid_group/grid_group.py` & `gridengine_framework-0.7.6/grid_engine/_grid_group/grid_group.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_grid_object/grid_item/grid_item.py` & `gridengine_framework-0.7.6/grid_engine/_grid_object/grid_item/grid_item.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_grid_object/grid_object.py` & `gridengine_framework-0.7.6/grid_engine/_grid_object/grid_object.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_grid_object/grid_structure/grid_structure.py` & `gridengine_framework-0.7.6/grid_engine/_grid_object/grid_structure/grid_structure.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_grid_object/grid_zone/grid_zone.py` & `gridengine_framework-0.7.6/grid_engine/_grid_object/grid_zone/grid_zone.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_terraform/terraformer.py` & `gridengine_framework-0.7.6/grid_engine/_terraform/terraformer.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/_utility.py` & `gridengine_framework-0.7.6/grid_engine/_utility.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/grid_engine/layout_test.py` & `gridengine_framework-0.7.6/grid_engine/layout_test.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/gridengine_framework.egg-info/PKG-INFO` & `gridengine_framework-0.7.6/gridengine_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridengine-framework
-Version: 0.7.5
+Version: 0.7.6
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gridengine_framework-0.7.5/gridengine_framework.egg-info/SOURCES.txt` & `gridengine_framework-0.7.6/gridengine_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.5/setup.py` & `gridengine_framework-0.7.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
     
 setup(
     name='gridengine_framework',
-    version='0.7.5',
+    version='0.7.6',
     description='A framework for generating and manipulating grid-based game worlds',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='James Evans',
     author_email='joesaysahoy@gmail.com',
     url='https://github.com/primal-coder/grid-engine',
     packages=find_packages(),
```

