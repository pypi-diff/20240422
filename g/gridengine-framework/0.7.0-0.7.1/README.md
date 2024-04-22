# Comparing `tmp/gridengine_framework-0.7.0.tar.gz` & `tmp/gridengine_framework-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridengine_framework-0.7.0.tar", last modified: Tue Nov 28 08:06:44 2023, max compression
+gzip compressed data, was "gridengine_framework-0.7.1.tar", last modified: Mon Apr 22 02:22:06 2024, max compression
```

## Comparing `gridengine_framework-0.7.0.tar` & `gridengine_framework-0.7.1.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.826474 gridengine_framework-0.7.0/
--rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.7.0/LICENSE
--rw-r--r--   0 boss      (1000) boss      (1002)     5810 2023-11-28 08:06:44.826474 gridengine_framework-0.7.0/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     5278 2023-11-02 07:42:03.000000 gridengine_framework-0.7.0/README.md
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.823141 gridengine_framework-0.7.0/grid_engine/
--rw-r--r--   0 boss      (1000) boss      (1002)      135 2023-11-25 03:11:25.000000 gridengine_framework-0.7.0/grid_engine/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     1293 2023-11-28 08:03:58.000000 gridengine_framework-0.7.0/grid_engine/__log__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4985 2023-11-25 03:11:01.000000 gridengine_framework-0.7.0/grid_engine/__main__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.823141 gridengine_framework-0.7.0/grid_engine/_blueprint/
--rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.7.0/grid_engine/_blueprint/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3584 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_blueprint/__main__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    17502 2023-11-25 05:51:29.000000 gridengine_framework-0.7.0/grid_engine/_blueprint/_grid_blueprint.py
--rw-r--r--   0 boss      (1000) boss      (1002)    18712 2023-11-24 08:52:19.000000 gridengine_framework-0.7.0/grid_engine/_blueprint/_grid_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)     9045 2023-11-04 02:46:22.000000 gridengine_framework-0.7.0/grid_engine/_blueprint/_terrain_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)     1615 2023-11-24 08:52:41.000000 gridengine_framework-0.7.0/grid_engine/_blueprint/terrains.json
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.823141 gridengine_framework-0.7.0/grid_engine/_cell/
--rw-r--r--   0 boss      (1000) boss      (1002)       22 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_cell/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    32322 2023-11-24 08:52:46.000000 gridengine_framework-0.7.0/grid_engine/_cell/cell.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4756 2023-11-25 03:11:01.000000 gridengine_framework-0.7.0/grid_engine/_dungeon.py
--rw-r--r--   0 boss      (1000) boss      (1002)    53380 2023-11-28 08:04:07.000000 gridengine_framework-0.7.0/grid_engine/_grid.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.823141 gridengine_framework-0.7.0/grid_engine/_grid_feature/
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_grid_feature/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_grid_feature/__main__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2442 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_grid_feature/grid_feature.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.826474 gridengine_framework-0.7.0/grid_engine/_grid_group/
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_grid_group/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3642 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_grid_group/grid_group.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.826474 gridengine_framework-0.7.0/grid_engine/_grid_object/
--rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_grid_object/__init__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.826474 gridengine_framework-0.7.0/grid_engine/_grid_object/grid_item/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_grid_object/grid_item/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.7.0/grid_engine/_grid_object/grid_item/grid_item.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2283 2023-11-12 05:05:46.000000 gridengine_framework-0.7.0/grid_engine/_grid_object/grid_object.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.826474 gridengine_framework-0.7.0/grid_engine/_grid_object/grid_structure/
--rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_grid_object/grid_structure/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2216 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_grid_object/grid_structure/grid_structure.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.826474 gridengine_framework-0.7.0/grid_engine/_grid_object/grid_zone/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_grid_object/grid_zone/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.7.0/grid_engine/_grid_object/grid_zone/grid_zone.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.826474 gridengine_framework-0.7.0/grid_engine/_terraform/
--rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.7.0/grid_engine/_terraform/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    10646 2023-11-12 05:01:09.000000 gridengine_framework-0.7.0/grid_engine/_terraform/terraformer.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5609 2023-11-08 03:23:26.000000 gridengine_framework-0.7.0/grid_engine/_utility.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2023-11-28 08:06:44.826474 gridengine_framework-0.7.0/gridengine_framework.egg-info/
--rw-r--r--   0 boss      (1000) boss      (1002)     5810 2023-11-28 08:06:44.000000 gridengine_framework-0.7.0/gridengine_framework.egg-info/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     1321 2023-11-28 08:06:44.000000 gridengine_framework-0.7.0/gridengine_framework.egg-info/SOURCES.txt
--rw-r--r--   0 boss      (1000) boss      (1002)        1 2023-11-28 08:06:44.000000 gridengine_framework-0.7.0/gridengine_framework.egg-info/dependency_links.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       33 2023-11-28 08:06:44.000000 gridengine_framework-0.7.0/gridengine_framework.egg-info/requires.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       12 2023-11-28 08:06:44.000000 gridengine_framework-0.7.0/gridengine_framework.egg-info/top_level.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       38 2023-11-28 08:06:44.826474 gridengine_framework-0.7.0/setup.cfg
--rw-r--r--   0 boss      (1000) boss      (1002)      876 2023-11-28 08:06:36.000000 gridengine_framework-0.7.0/setup.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.140027 gridengine_framework-0.7.1/
+-rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.7.1/LICENSE
+-rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 02:22:06.140027 gridengine_framework-0.7.1/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     5278 2023-11-02 07:42:03.000000 gridengine_framework-0.7.1/README.md
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.136694 gridengine_framework-0.7.1/grid_engine/
+-rw-r--r--   0 boss      (1000) boss      (1002)      135 2023-11-25 03:11:25.000000 gridengine_framework-0.7.1/grid_engine/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     1293 2023-11-28 08:03:58.000000 gridengine_framework-0.7.1/grid_engine/__log__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4931 2023-12-10 21:45:39.000000 gridengine_framework-0.7.1/grid_engine/__main__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.136694 gridengine_framework-0.7.1/grid_engine/_blueprint/
+-rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.7.1/grid_engine/_blueprint/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3584 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_blueprint/__main__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2024-01-11 22:32:29.000000 gridengine_framework-0.7.1/grid_engine/_blueprint/_floorplan_classes.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5608 2024-02-11 03:43:12.000000 gridengine_framework-0.7.1/grid_engine/_blueprint/_floorplan_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    17490 2024-04-22 01:01:14.000000 gridengine_framework-0.7.1/grid_engine/_blueprint/_grid_blueprint.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    18503 2024-02-12 03:03:41.000000 gridengine_framework-0.7.1/grid_engine/_blueprint/_grid_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     9045 2023-11-04 02:46:22.000000 gridengine_framework-0.7.1/grid_engine/_blueprint/_terrain_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     1615 2023-11-24 08:52:41.000000 gridengine_framework-0.7.1/grid_engine/_blueprint/terrains.json
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.136694 gridengine_framework-0.7.1/grid_engine/_cell/
+-rw-r--r--   0 boss      (1000) boss      (1002)       22 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_cell/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    32323 2024-04-22 01:48:00.000000 gridengine_framework-0.7.1/grid_engine/_cell/cell.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4756 2023-11-25 03:11:01.000000 gridengine_framework-0.7.1/grid_engine/_dungeon.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    54707 2024-04-22 01:43:28.000000 gridengine_framework-0.7.1/grid_engine/_grid.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.136694 gridengine_framework-0.7.1/grid_engine/_grid_feature/
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_grid_feature/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2442 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_grid_feature/grid_feature.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.140027 gridengine_framework-0.7.1/grid_engine/_grid_group/
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_grid_group/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3642 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_grid_group/grid_group.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.140027 gridengine_framework-0.7.1/grid_engine/_grid_object/
+-rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_grid_object/__init__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.140027 gridengine_framework-0.7.1/grid_engine/_grid_object/grid_item/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_grid_object/grid_item/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.7.1/grid_engine/_grid_object/grid_item/grid_item.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2283 2023-11-12 05:05:46.000000 gridengine_framework-0.7.1/grid_engine/_grid_object/grid_object.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.140027 gridengine_framework-0.7.1/grid_engine/_grid_object/grid_structure/
+-rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_grid_object/grid_structure/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2216 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_grid_object/grid_structure/grid_structure.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.140027 gridengine_framework-0.7.1/grid_engine/_grid_object/grid_zone/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_grid_object/grid_zone/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.7.1/grid_engine/_grid_object/grid_zone/grid_zone.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.140027 gridengine_framework-0.7.1/grid_engine/_terraform/
+-rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.7.1/grid_engine/_terraform/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    10775 2024-02-12 03:10:30.000000 gridengine_framework-0.7.1/grid_engine/_terraform/terraformer.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5714 2024-02-24 16:00:59.000000 gridengine_framework-0.7.1/grid_engine/_utility.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2925 2024-02-12 03:13:00.000000 gridengine_framework-0.7.1/grid_engine/layout_test.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 02:22:06.140027 gridengine_framework-0.7.1/gridengine_framework.egg-info/
+-rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 02:22:06.000000 gridengine_framework-0.7.1/gridengine_framework.egg-info/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     1403 2024-04-22 02:22:06.000000 gridengine_framework-0.7.1/gridengine_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)        1 2024-04-22 02:22:06.000000 gridengine_framework-0.7.1/gridengine_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-22 02:22:06.000000 gridengine_framework-0.7.1/gridengine_framework.egg-info/requires.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       12 2024-04-22 02:22:06.000000 gridengine_framework-0.7.1/gridengine_framework.egg-info/top_level.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       38 2024-04-22 02:22:06.140027 gridengine_framework-0.7.1/setup.cfg
+-rw-r--r--   0 boss      (1000) boss      (1002)      876 2024-04-22 02:21:54.000000 gridengine_framework-0.7.1/setup.py
```

### Comparing `gridengine_framework-0.7.0/LICENSE` & `gridengine_framework-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/PKG-INFO` & `gridengine_framework-0.7.1/gridengine_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gridengine_framework
-Version: 0.7.0
+Name: gridengine-framework
+Version: 0.7.1
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gridengine_framework-0.7.0/README.md` & `gridengine_framework-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/__log__.py` & `gridengine_framework-0.7.1/grid_engine/__log__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/__main__.py` & `gridengine_framework-0.7.1/grid_engine/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,48 +49,48 @@
         blueprint = blueprint.load_blueprint(f'{blueprints}{args.blueprint}.pkl',  blueprint.BaseGridBlueprint)
     print('Success! Blueprint loaded.')
 else:
     if args.rows*args.columns > 1000000:
         print(f'{colorama.Fore.RED}WARNING{colorama.Fore.RESET}: The provided parameters will generate a grid composed of {colorama.Fore.LIGHTWHITE_EX}{round((args.rows*args.columns)/1000000, 1)} million{colorama.Fore.RESET} cells. \nThis will consume a significant amount of memory/resources/time. \nIf you have limited amount of memory this could cause your system to hang or crash. \nIf you understand the risks, continue by pressing {colorama.Fore.LIGHTGREEN_EX}ENTER{colorama.Fore.RESET}. Otherwise, press {colorama.Fore.LIGHTRED_EX}CTRL+C{colorama.Fore.RESET} to exit.')
         input()
     print(f'Generating blueprint with cell size {args.size}, {args.rows} rows and {args.columns} columns. Total_cells: {args.rows*args.columns} ...')
-    blueprint = blueprint.TerrainGridBlueprint(cell_size=args.size, grid_dimensions=(args.columns*args.size, args.rows*args.size), noise_scale=args.noise_scale, noise_octaves=args.noise_octaves, noise_roughness=args.noise_roughness)
-    print(f'Success! Blueprint generated. Dimensions: {blueprint.grid_dimensions}')
+    bp = blueprint.TerrainGridBlueprint(cell_size=args.size, grid_dimensions=(args.columns*args.size, args.rows*args.size), noise_scale=args.noise_scale, noise_octaves=args.noise_octaves, noise_roughness=args.noise_roughness)
+    print(f'Success! Blueprint generated. Dimensions: {bp.grid_dimensions}')
 
 print('Building grid from blueprint ...')
-grid = grid.Grid(blueprint=blueprint, with_terrain=True)
+g = grid.Grid(gblueprint=bp, with_terrain=True)
 print('Success! Grid generated.')
 
 if args.save:
     print('Pickling grid ...')
-    grid.save_grid(grid=grid)
+    grid.save_grid(grid=g)
     print('Success!')
     print('Pickling blueprint ...')
-    blueprint.save_blueprint(blueprint=blueprint)
+    blueprint.save_blueprint(blueprint=bp)
     print('Success!')
     
 if args.ascii:
     print('Writing ascii to file ...')
-    with open(f'{saves_dir}{grid.grid_id[-5:]}/grid.txt', 'w') as f:
+    with open(f'{saves_dir}{g.grid_id[-5:]}/grid.txt', 'w') as f:
         rows = []
         string = ''
         for row in grid.rows:
             for cell in row:
                 string += cell.terrain_char
             rows.append(string)
             string = ''
         f.write('\n'.join(rows))
     print('Success!')
     
-cdata = grid.extract_cell_data(grid)
-cell_size = grid.cell_size
-grid_id = grid.grid_id[-5:]
-height = grid.blueprint.grid_height
-width = grid.blueprint.grid_width
+cdata = grid.extract_cell_data(g)
+cell_size = g.cell_size
+grid_id = g.grid_id[-5:]
+height = g.blueprint.grid_height
+width = g.blueprint.grid_width
 del blueprint
-del grid
+del g
 
 from grid_engine import _utility as utility
     
 utility.generate_images((width, height), cdata, cell_size, grid_id, animate=args.animate)
```

### Comparing `gridengine_framework-0.7.0/grid_engine/_blueprint/__main__.py` & `gridengine_framework-0.7.1/grid_engine/_blueprint/__main__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/_blueprint/_grid_blueprint.py` & `gridengine_framework-0.7.1/grid_engine/_blueprint/_grid_blueprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from screeninfo import get_monitors as _get_monitors
-
-from ..__log__ import log_method as _log_method
+#from screeninfo import get_monitors as _get_monitors
 
 from ._grid_processing import *
 from ._terrain_processing import *
 from ._terrain_processing import _COLORS
+from ._floorplan_processing import *
 import numpy as np
 from collections import defaultdict
 from uuid import uuid4
 import pickle
 import os as _os
 
 saves_dir = 'grid_engine/_saves/'
 
 _OCEAN_BLUE = _COLORS['OCEAN_BLUE']
 
-_SCRX, _SCRY = _SCR_DIMS = _get_monitors()[0].width, _get_monitors()[0].height
+#_SCRX, _SCRY = _SCR_DIMS = _get_monitors()[0].width, _get_monitors()[0].height
 
 def save_blueprint(blueprint):
     import os
     if not os.path.exists(f'{saves_dir}{blueprint.blueprint_id[-5:]}'):
         os.makedirs(f'{saves_dir}{blueprint.blueprint_id[-5:]}')
     with open(f'{saves_dir}{blueprint.blueprint_id[-5:]}/blueprint.{blueprint.blueprint_id[-5:]}.pkl', 'wb') as f:
         pickle.dump(blueprint, f)
@@ -350,14 +349,15 @@
         self.cell_size = cell_size if cell_size is not None else 3
         self.grid_dimensions = grid_dimensions if grid_dimensions is not None else (_SCRX, _SCRY)
         self._array = np.array(
                 [0 for _ in list(range((self._col_count * self._row_count) * (len(_levels) - 1)))],
                 dtype=type(any),
         ).reshape((self._col_count, self._row_count, len(_levels) - 1))
         self._init()
+        self.layer_attributes = _layer_attributes
 
     def _init(self):
         grid_info = process_grid(self._row_count, self._col_count, self.cell_size)
         self.rank = grid_info['row_strings']
         self.file = grid_info['col_strings']
         self.cell_list = grid_info['cell_strings']
         self.cell_coordinates = grid_info['cell_coordinates']
@@ -411,27 +411,25 @@
             noise_octaves: int = None, noise_roughness: float = None
     ):
         super(TerrainGridBlueprint, self).__init__(cell_size, grid_dimensions, grid_id)
         for cell in self.dictGrid:
             self.dictGrid[cell]['passable'] = None
         self._init_terrain(noise_scale, noise_octaves, noise_roughness)
 
-    @_log_method
     def _init_terrain(self, noise_scale, noise_octaves, noise_roughness):
         self._noise_scale = noise_scale if noise_scale is not None else 350
         self._noise_octaves = noise_octaves if noise_octaves is not None else 88
         self._noise_roughness = noise_roughness if noise_roughness is not None else 0.65
         self.dictTerrain = process_noise(
             self._noise_scale, self._noise_octaves, self._noise_roughness, self._row_count, self._col_count,
             self._cell_size, self.dictGrid
             )
         self._set_base_terrain()
         self._adjust_passability()
 
-    @_log_method
     def _set_base_terrain(self):
         base_terrain = {
                 'str':      'OCEAN',
                 'raw':      None,
                 'int':      9,
                 'color':    _OCEAN_BLUE,
                 'cost_in':  float('inf'),
@@ -441,15 +439,14 @@
         dictTerrain = self.dictTerrain.copy()
         for cell in self.cell_list:
             if self.dictTerrain[cell]['raw'] is None:
                 dictTerrain[cell] = base_terrain
                 self.dictGrid[cell]['passable'] = False
         self.dictTerrain = dictTerrain
 
-    @_log_method
     def _adjust_passability(self):
         passable = []
         unpassable = []
         for c, info in self.dictTerrain.items():
             if info['str'] in _UNPASSABLE_TERRAIN:
                 self.dictGrid[c]['passable'] = False
                 unpassable.append(c)
@@ -469,8 +466,8 @@
                 'dict_grid':        self.dictGrid,
                 'dict_terrain':     self.dictTerrain,
                 'noise_scale':      self._noise_scale,
                 'noise_octaves':    self._noise_octaves,
                 'noise_roughness':  self._noise_roughness,
                 'quadrants':        self.quadrants,
                 'graph':            self.graph,
-        }
+        }
```

### Comparing `gridengine_framework-0.7.0/grid_engine/_blueprint/_grid_processing.py` & `gridengine_framework-0.7.1/grid_engine/_blueprint/_grid_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from ..__log__ import log_method as _log_method
-
 from typing import Optional, List, Tuple, Dict, Any
 import itertools
 import numpy as np
 
 
-@_log_method
 def generate_row_strings(row_count: int) -> List[str]:
     """
     Generate a list of strings representing rows.
 
     This function generates a list of strings representing rows. The number of rows to generate is specified by the `row_count` parameter.
 
     Args:
@@ -38,15 +35,14 @@
     )
     rows.extend(
         chr(i + 97) + chr(j + 97) + chr(k + 97)
         for i, j, k in itertools.product(range(26), range(26), range(26))
     )
     return rows[:row_count]
 
-@_log_method
 def generate_column_strings(col_count: int) -> List[str]:
     """
     Generate a list of strings representing columns.
 
     This function generates a list of strings representing columns. The number of columns to generate is specified by the `col_count` parameter. Each column is represented by a string that is zero-padded to a width of 5 characters.
 
     Args:
@@ -65,27 +61,24 @@
     print(f'Column count: {col_count}')
     cols = [str(r + 1) for r in range(col_count)][::-1]
     for i in range(col_count):
         cols[i] = cols[i].zfill(5)
     cols.reverse()
     return cols
 
-@_log_method
 def get_row_strings(row_count: Optional[int] = None) -> List[str]:
     if row_count is None or row_count < 1:
         raise ValueError("row_count must be an integer > 1")
     return generate_row_strings(row_count)
 
-@_log_method
 def get_column_strings(col_count: Optional[int] = None) -> List[str]:
     if col_count is None or col_count < 1:
         raise ValueError("col_count must be an integer > 1")
     return generate_column_strings(col_count)
 
-@_log_method
 def generate_cell_strings(row_strings: List[str], col_strings: List[str]) -> List[str]:
     """
     Generate a list of strings representing cells.
 
     This function generates a list of strings representing cells by combining each row string from `row_strings` with each column string from `col_strings`. The resulting list contains all possible combinations of row and column strings.
 
     Args:
@@ -102,19 +95,17 @@
         cell_strings = generate_cell_strings(row_strings, col_strings)
         print(cell_strings)
         # Output: ['a1', 'a2', 'a3', 'b1', 'b2', 'b3', 'c1', 'c2', 'c3']
         ```
     """
     return [r + f for r, f in itertools.product(row_strings, col_strings)]
 
-@_log_method
 def get_cell_strings(row_strings: List[str], col_strings: List[str]) -> List[str]:
     return generate_cell_strings(row_strings, col_strings)
 
-@_log_method
 def get_cell_coordinates(cell_size: int, row_count: int, col_count: int) -> List[Tuple[int, int]]:
     """
     Get the coordinates of each cell in a grid.
 
     This function calculates the coordinates of each cell in a grid based on the provided `cell_size`, `row_count`, and `col_count` parameters. The coordinates are returned as a list of tuples, where each tuple represents the x and y coordinates of a cell.
 
     Args:
@@ -136,15 +127,14 @@
         (
             abs(0 - ((num % col_count) * cell_size)),
             abs(0 - ((num // col_count) * cell_size)),
        )
         for num in range(row_count*col_count)
     ]
 
-@_log_method
 def get_grid_dict(cell_strings: List[str], row_strings: List[str], col_strings: List[str], cell_coordinates: List[Tuple[int, int]]) -> Dict[str, Any]:
     """
     Get a dictionary representing a grid.
 
     This function creates a dictionary representing a grid based on the provided `cell_strings`, `row_strings`, `col_strings`, and `cell_coordinates`. Each cell in the grid is represented by a key-value pair in the dictionary, where the key is the cell string and the value is a dictionary containing various properties of the cell.
 
     Args:
@@ -183,15 +173,14 @@
             "col_index": col_strings.index(cell[-5:]),
             "coordinates": cell_coordinates[i],
             "quadrant_index": None,
             "adjacent": []
         } for i, cell in enumerate(cell_strings)
     }
     
-@_log_method
 def generate_quadrant_coordinates(row_count: int, col_count: int) -> List[List[Tuple[int, int]]]:
     """
     Get the coordinates of each quadrant in a grid.
 
     This function calculates the coordinates of each quadrant in a grid based on the provided `row_count` and `col_count` parameters. The grid is divided into four quadrants, and the coordinates of each quadrant are returned as a list of lists, where each inner list represents the coordinates of a quadrant.
 
     Args:
@@ -222,15 +211,14 @@
             (quad_x[i+1], quad_y[j])[::-1],
             (quad_x[i+1], quad_y[j+1])[::-1],
             (quad_x[i], quad_y[j+1])[::-1]
         ]
         for i, j in itertools.product(range(2), range(2))
     ]
     
-@_log_method
 def get_quadrant_indices(quadrant_coords: List[List[Tuple[int,int]]], grid_dict: Dict[str, Any]) -> Dict[str, Any]:
     """
     Assign quadrant indices to cells in a grid.
 
     This function assigns quadrant indices to cells in a grid based on the provided `quadrant_coords` and `grid_dict`. Each cell in the grid is checked against the coordinates of each quadrant, and if the cell falls within a quadrant, its `quadrant_index` property in the `grid_dict` is updated accordingly.
 
     Args:
@@ -252,15 +240,14 @@
                 quad[0][0] <= grid_dict[cell]['col_index'] < quad[2][0] 
                 and 
                 quad[0][1] <= grid_dict[cell]['row_index'] < quad[1][1]
             ):
                 grid_dict[cell]['quadrant_index'] = i
     return grid_dict
 
-@_log_method
 def generate_adjacency(grid_dict: Dict[str, any], row_count: int, col_count: int) -> Dict[str, Any]:
     """
     Assign adjacent cells to each cell in a grid.
 
     This function assigns adjacent cells to each cell in a grid based on the provided `grid_dict`, `row_count`, and `col_count`. The adjacency is determined based on the position of each cell within the grid. The adjacent cells are stored as a list in the `adjacent` property of each cell in the `grid_dict`.
 
     Args:
@@ -349,15 +336,14 @@
     """
 
     return {
         cell: list(info['adjacent'])
         for cell, info in grid_dict.items()
     }
 
-@_log_method    
 def process_grid(row_count: int, col_count: int, cell_size: int) -> Dict[str, Any]:
     """
     Process a grid.
 
     This function processes a grid based on the provided `row_count`, `col_count`, and `cell_size`. It performs the following steps:
     1. Generates row strings.
     2. Generates column strings.
```

### Comparing `gridengine_framework-0.7.0/grid_engine/_blueprint/_terrain_processing.py` & `gridengine_framework-0.7.1/grid_engine/_blueprint/_terrain_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/_blueprint/terrains.json` & `gridengine_framework-0.7.1/grid_engine/_blueprint/terrains.json`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/_cell/cell.py` & `gridengine_framework-0.7.1/grid_engine/_cell/cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,35 +135,35 @@
             self._up_left = self.parentgrid[self.adjacent[0]]
             # self._up_left = self.parentgrid.get_cell_by_position(self.x - self.size, self.y + self.size)
         return self._up_left
 
     @property
     def up(self):
         """Returns the cell adjacent in the up direction"""
-        if self.row == self.parentgrid.last_row:
+        if self.row == self.parentgrid.first_row:
             self._up = None
         else:
             self._up = self.parentgrid[self.adjacent[1]]
             # self._up = self.col[self.col.index(self)+1]
         return self._up
     
     @property
     def up_right(self):
         """Returns the cell adjacent in the up-right direction"""
-        if self.row == self.parentgrid.last_row or self.col == self.parentgrid.last_col:
+        if self.row == self.parentgrid.first_row or self.col == self.parentgrid.last_col:
             self._up_right = None
         else:
             self._up_right = self.parentgrid[self.adjacent[2]]
             # self._up_right = self.parentgrid.get_cell_by_position(self.x + self.size, self.y + self.size)
         return self._up_right
     
     @property
     def clearance_up(self):
         """Returns the number of cells in the up direction that are passable"""
-        if self.row == self.parentgrid.last_row:
+        if self.row == self.parentgrid.first_row:
             self._clearance_up = 0
         else:
             clearance = 0
             place_in_col = self.col.index(self)
             col_len = len(self.col)
             steps_to_top = col_len - place_in_col
             for step in range(steps_to_top):
@@ -193,25 +193,25 @@
             self._down = self.parentgrid[self.adjacent[5]]
             # self._down = self.col[self.col.index(self) - 1]
         return self._down
 
     @property
     def down_left(self):
         """Returns the cell adjacent in the down-left direction"""
-        if self.row == self.parentgrid.first_row or self.col == self.parentgrid.first_col:
+        if self.row == self.parentgrid.last_row or self.col == self.parentgrid.first_col:
             self._down_left = None
         else:
             self._down_left = self.parentgrid[self.adjacent[6]]
             self._down_left = self.parentgrid.get_cell_by_position(self.x - self.size, self.y - self.size)
         return self._down_left
 
     @property
     def clearance_down(self):
         """Returns the number of cells in the down direction that are passable"""
-        if self.row == self.parentgrid.first_row:
+        if self.row == self.parentgrid.last_row:
             self._clearance_down = 0
         else:
             clearance = 0
             place_in_col = self.col.index(self)
             steps_to_bottom = place_in_col
             for step in range(steps_to_bottom):
                 if self.col[steps_to_bottom - step].passable:
```

### Comparing `gridengine_framework-0.7.0/grid_engine/_dungeon.py` & `gridengine_framework-0.7.1/grid_engine/_dungeon.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/_grid.py` & `gridengine_framework-0.7.1/grid_engine/_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,15 +395,15 @@
 
 
 class Grid(_AbstractGrid, _ABC):
     """The grid object. Contains all cells, rows, columns, and quadrants."""
 
     def __init__(
             self,
-            blueprint: _Optional[type[_Blueprint.AbstractGridBlueprint]] = None,
+            gblueprint: _Optional[type[_Blueprint.AbstractGridBlueprint]] = None,
             cell_size: _Optional[int] = None,
             dimensions: _Optional[tuple[int, int]] = None,
             with_terrain: _Optional[bool] = None,
             noise_scale: _Optional[float] = None,
             noise_octaves: _Optional[int] = None,
             noise_roughness: _Optional[float] = None
     ):
@@ -416,29 +416,29 @@
             cell_size (_Optional[int], optional): The size of each cell in the grid. Defaults to None.
             dimensions (_Optional[tuple[int, int]], optional): The dimensions of the grid. Defaults to None.
             with_terrain (_Optional[bool], optional): Whether the grid has terrain. Defaults to None.
             noise_scale (_Optional[float], optional): The scale of the Perlin noise. Defaults to None.
             noise_octaves (_Optional[int],optional): The number of octaves for the Perlin noise. Defaults to None.
             noise_roughness (_Optional[float],optional): The roughness of the Perlin noise. Defaults to None.
         """
-        if blueprint is not None:
-            x, y = blueprint.grid_dimensions
+        if gblueprint is not None:
+            x, y = gblueprint.grid_dimensions
         elif dimensions is not None:
             x, y = dimensions
         elif cell_size is None:
             dimensions = (500, 500)
             x, y = dimensions
             cell_size = 1
-        cell_count = (x * y) / cell_size if cell_size is not None else (x * y) / blueprint._cell_size
+        cell_count = (x * y) / cell_size if cell_size is not None else (x * y) / gblueprint._cell_size
         if dimensions is not None and (cell_count > 1000000) and not self._size_warning(cell_count):
             return
 
-        self.grid_id = _uuid4().hex if blueprint is None else blueprint.blueprint_id
+        self.grid_id = _uuid4().hex if gblueprint is None else gblueprint.blueprint_id
         self.with_terrain = with_terrain if with_terrain is not None else True
-        self.blueprint = blueprint if blueprint is not None else \
+        self.blueprint = gblueprint if gblueprint is not None else \
             _Blueprint.TerrainGridBlueprint(
                     cell_size,
                     dimensions,
                     self.grid_id,
                     noise_scale,
                     noise_octaves,
                     noise_roughness
@@ -491,14 +491,15 @@
             self.sea_count = len(self.seas)
             self.lake_count = len(self.lakes)
             self._set_water_cells()
             self.river_count = 0
             self.rivers: list[list[_Cell,]] = []
             self._terraformer = Terraformer(self)
             self.terraformer.set_rivers(2)
+            self._fix_minute_water_bodies()
 
         # self.town = GridZone(self, 'Town', 'town', self.random_cell(attr=('passable', True)), (45, 45, 45), 2)
 
     def _size_warning(self, cell_count):
         import colorama
         quit = input(
             f'{colorama.Fore.RED}WARNING{colorama.Fore.RESET}: The provided parameters will generate a grid composed '
@@ -1202,14 +1203,35 @@
                                 queue.append(neighbor_cell)
         return list(body_of_water_cells)
 
     def _set_water_cells(self):
         for i, body_of_water in self.bodies_of_water.items():
             for cell in body_of_water['body_of_water_cells']:
                 cell.body_of_water_index = i
+                
+    def _fix_minute_water_bodies(self):
+        for i, cell in enumerate(self.cells.values()):
+            if not cell.passable:
+                total_neighbors = 0
+                passable_neighbors = 0
+                model_cell = None
+                for neighbor in cell.adjacent:
+                    if neighbor is not None:
+                        total_neighbors += 1
+                        if self.cells[neighbor].passable:
+                            passable_neighbors += 1
+                            model_cell = self.cells[neighbor]
+                if passable_neighbors == total_neighbors:
+                    cell.passable = True
+                    cell.terrain_str = self.dictTerrain[model_cell.designation]['str']
+                    cell.terrain_raw = self.dictTerrain[model_cell.designation]['raw']
+                    cell.terrain_int = self.dictTerrain[model_cell.designation]['int']
+                    cell.terrain_color = self.dictTerrain[model_cell.designation]['color']
+                    cell._cost_in = self.dictTerrain[model_cell.designation]['cost_in']
+                    cell._cost_out = self.dictTerrain[model_cell.designation]['cost_out']
 
     def _heuristic(self, cella: _Union[str, _Cell], cellb: _Union[str, _Cell]):
         """Estimates the distance between two cells using Manhattan distance"""
         _logger.gridengine(f'Calculating heuristic from {cella} --> {cellb}')
         if isinstance(cella, _Cell):
             cella = cella.designation
         if isinstance(cellb, _Cell):
@@ -1251,24 +1273,25 @@
                 while current in came_from:
                     current = came_from[current]
                     path.append(current)
                 path.reverse()
                 return (path, cost_so_far[goal])
 
             for next_step in graph[current]:
-                # For each neighbor of the current node, 
-                # calculate the _cost of the path from the start node to that neighbor
-                new_cost = cost_so_far[current] + self._cost(current, next_step)
-                if next_step not in cost_so_far or new_cost < cost_so_far[
-                    next_step  # If the new path is better than the old path
-                ]:
-                    cost_so_far[next_step] = new_cost  # Update the cost of the path to the neighbor
-                    priority = new_cost + self._heuristic(goal, next_step)  # Calculate the priority of the neighbor
-                    _heapq.heappush(frontier, (priority, next_step))  # Add the neighbor to the frontier
-                    came_from[next_step] = current  # Update the neighbor's parent to the current node
+                if next_step is not None:
+                    # For each neighbor of the current node, 
+                    # calculate the _cost of the path from the start node to that neighbor
+                    new_cost = cost_so_far[current] + self._cost(current, next_step)
+                    if next_step not in cost_so_far or new_cost < cost_so_far[
+                        next_step  # If the new path is better than the old path
+                    ]:
+                        cost_so_far[next_step] = new_cost  # Update the cost of the path to the neighbor
+                        priority = new_cost + self._heuristic(goal, next_step)  # Calculate the priority of the neighbor
+                        _heapq.heappush(frontier, (priority, next_step))  # Add the neighbor to the frontier
+                        came_from[next_step] = current  # Update the neighbor's parent to the current node
 
         return None  # We didn't find a path
 
     def _cast_grid(self, scene):
         """Cast the grid to the scene. Each cell is represented as a _pyglet.shapes.Rectangle object."""
         for cell in self.cells.values():
             x, y, w, h, c = cell._request_shape()
```

### Comparing `gridengine_framework-0.7.0/grid_engine/_grid_feature/grid_feature.py` & `gridengine_framework-0.7.1/grid_engine/_grid_feature/grid_feature.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/_grid_group/grid_group.py` & `gridengine_framework-0.7.1/grid_engine/_grid_group/grid_group.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/_grid_object/grid_item/grid_item.py` & `gridengine_framework-0.7.1/grid_engine/_grid_object/grid_item/grid_item.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/_grid_object/grid_object.py` & `gridengine_framework-0.7.1/grid_engine/_grid_object/grid_object.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/_grid_object/grid_structure/grid_structure.py` & `gridengine_framework-0.7.1/grid_engine/_grid_object/grid_structure/grid_structure.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/_grid_object/grid_zone/grid_zone.py` & `gridengine_framework-0.7.1/grid_engine/_grid_object/grid_zone/grid_zone.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.7.0/grid_engine/_terraform/terraformer.py` & `gridengine_framework-0.7.1/grid_engine/_terraform/terraformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,28 +56,32 @@
         print('Getting river cells by walk ...')
         path = self.get_river_by_walk(start_cell, end_cell)
         path = list(itertools.chain.from_iterable(path))
         path = [self.cells[cell] for cell in path]
         print(f'River steps: {len(path)}')
         if path is not None:
             path = self.expand_river_path(path)
+            step = 0
+            total_steps = len(path)
+            split = False
             # shaped_path = self.shape_river_path(expanded_path)
             for cell in path:
+                step += 1
                 cell.terrain_str = 'RIVER'
                 cell.terrain_raw = 0.0
                 cell.terrain_int = 9
                 cell.terrain_color = RIVER_BLUE
                 self.dictTerrain[cell.designation] = {
                     'str': cell.terrain_str, 
                     'raw': cell.terrain_raw, 
                     'int': cell.terrain_int, 
                     'color': cell.terrain_color, 
                     'cost_in': 2, 
                     'cost_out': 2
-                    }        
+                    }                            
             self.grid.river_count += 1
             self.grid.rivers.append(path)
         else:
             print("No path found between the start and end cells.")
 
     @_log_method
     def expand_river_path(self, path):
```

### Comparing `gridengine_framework-0.7.0/grid_engine/_utility.py` & `gridengine_framework-0.7.1/grid_engine/_utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,26 +80,31 @@
                 draw.rectangle((x, y, x+cell_size, y+cell_size), fill=color)
             frames.append(image.copy())
         print('Saving grid animation ...')
         grid_id = grid_id[-5:]
         grid_dir = get_grid_dir(grid_id)
         frames[0].save(f'{grid_dir}grid.gif', format='GIF', append_images=frames[1:], save_all=True, duration=0.001, loop=0)
         print(f'grid.gif saved to {grid_dir}.')
+        print('Press ')
     else:
         for i, cell in enumerate(cells):
             print(f'Drawing cells         {round((i/total_cell_count)*100)}%', end='\r')
             x = cell[0]
             y = cell[1]
             color = cell[2]
             draw.rectangle((x, y, x+cell_size, y+cell_size), fill=color)
         print('Cells drawn.                                   ')
     print('Saving grid image ...')
     image.save(f'{grid_dir}grid.png')
     print(f'grid.png saved to {grid_dir}.')
     
+    import matplotlib.pyplot as plt
+    
+    plt.imshow(image)
+    plt.show()   
     
 # Define the QuietDict class
 
 from typing import Union
 
 class QuietDict:
     def __init__(self):
```

### Comparing `gridengine_framework-0.7.0/gridengine_framework.egg-info/PKG-INFO` & `gridengine_framework-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gridengine-framework
-Version: 0.7.0
+Name: gridengine_framework
+Version: 0.7.1
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gridengine_framework-0.7.0/gridengine_framework.egg-info/SOURCES.txt` & `gridengine_framework-0.7.1/gridengine_framework.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 setup.py
 grid_engine/__init__.py
 grid_engine/__log__.py
 grid_engine/__main__.py
 grid_engine/_dungeon.py
 grid_engine/_grid.py
 grid_engine/_utility.py
+grid_engine/layout_test.py
 grid_engine/_blueprint/__init__.py
 grid_engine/_blueprint/__main__.py
+grid_engine/_blueprint/_floorplan_classes.py
+grid_engine/_blueprint/_floorplan_processing.py
 grid_engine/_blueprint/_grid_blueprint.py
 grid_engine/_blueprint/_grid_processing.py
 grid_engine/_blueprint/_terrain_processing.py
 grid_engine/_blueprint/terrains.json
 grid_engine/_cell/__init__.py
 grid_engine/_cell/cell.py
 grid_engine/_grid_feature/__init__.py
-grid_engine/_grid_feature/__main__.py
 grid_engine/_grid_feature/grid_feature.py
 grid_engine/_grid_group/__init__.py
 grid_engine/_grid_group/grid_group.py
 grid_engine/_grid_object/__init__.py
 grid_engine/_grid_object/grid_object.py
 grid_engine/_grid_object/grid_item/__init__.py
 grid_engine/_grid_object/grid_item/grid_item.py
```

### Comparing `gridengine_framework-0.7.0/setup.py` & `gridengine_framework-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
     
 setup(
     name='gridengine_framework',
-    version='0.7.0',
+    version='0.7.1',
     description='A framework for generating and manipulating grid-based game worlds',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='James Evans',
     author_email='joesaysahoy@gmail.com',
     url='https://github.com/primal-coder/grid-engine',
     packages=find_packages(),
```

