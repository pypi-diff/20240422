# Comparing `tmp/ocp_tessellate-2.3.1.tar.gz` & `tmp/ocp_tessellate-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_tessellate-2.3.1.tar", last modified: Thu Apr 18 06:18:43 2024, max compression
+gzip compressed data, was "ocp_tessellate-2.3.2.tar", last modified: Mon Apr 22 06:39:28 2024, max compression
```

## Comparing `ocp_tessellate-2.3.1.tar` & `ocp_tessellate-2.3.2.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-18 06:18:43.316141 ocp_tessellate-2.3.1/
--rw-r--r--   0 bernhard   (501) staff       (20)     1109 2024-04-18 06:18:43.316051 ocp_tessellate-2.3.1/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-2.3.1/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-18 06:18:43.313071 ocp_tessellate-2.3.1/ocp_tessellate/
--rw-r--r--   0 bernhard   (501) staff       (20)     2942 2024-04-14 10:24:20.000000 ocp_tessellate-2.3.1/ocp_tessellate/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1123 2024-04-18 06:18:31.000000 ocp_tessellate-2.3.1/ocp_tessellate/_version.py
--rw-r--r--   0 bernhard   (501) staff       (20)    15980 2024-04-18 06:14:39.000000 ocp_tessellate-2.3.1/ocp_tessellate/cad_objects.py
--rw-r--r--   0 bernhard   (501) staff       (20)    35114 2024-04-17 06:20:41.000000 ocp_tessellate-2.3.1/ocp_tessellate/convert.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10683 2024-03-17 10:14:02.000000 ocp_tessellate-2.3.1/ocp_tessellate/defaults.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-06-19 18:39:04.000000 ocp_tessellate-2.3.1/ocp_tessellate/mp_tess.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3048 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.1/ocp_tessellate/mp_tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)    25136 2024-03-14 07:11:29.000000 ocp_tessellate-2.3.1/ocp_tessellate/ocp_utils.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-06-19 19:00:22.000000 ocp_tessellate-2.3.1/ocp_tessellate/stepreader.py
--rw-r--r--   0 bernhard   (501) staff       (20)    18140 2024-04-18 06:17:42.000000 ocp_tessellate-2.3.1/ocp_tessellate/tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1065 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.1/ocp_tessellate/trace.py
--rw-r--r--   0 bernhard   (501) staff       (20)     6177 2024-04-14 10:38:44.000000 ocp_tessellate-2.3.1/ocp_tessellate/utils.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-18 06:18:43.315606 ocp_tessellate-2.3.1/ocp_tessellate.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)     1109 2024-04-18 06:18:43.000000 ocp_tessellate-2.3.1/ocp_tessellate.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      975 2024-04-18 06:18:43.000000 ocp_tessellate-2.3.1/ocp_tessellate.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-18 06:18:43.000000 ocp_tessellate-2.3.1/ocp_tessellate.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-18 06:18:43.000000 ocp_tessellate-2.3.1/ocp_tessellate.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)      112 2024-04-18 06:18:43.000000 ocp_tessellate-2.3.1/ocp_tessellate.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       15 2024-04-18 06:18:43.000000 ocp_tessellate-2.3.1/ocp_tessellate.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      671 2024-04-18 06:18:43.316393 ocp_tessellate-2.3.1/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1627 2024-04-18 06:18:31.000000 ocp_tessellate-2.3.1/setup.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-18 06:18:43.315411 ocp_tessellate-2.3.1/tests/
--rw-r--r--   0 bernhard   (501) staff       (20)     1419 2024-03-21 20:20:19.000000 ocp_tessellate-2.3.1/tests/test_cache.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1100 2024-01-17 07:33:06.000000 ocp_tessellate-2.3.1/tests/test_cadquery_sketch.py
--rw-r--r--   0 bernhard   (501) staff       (20)      895 2023-06-17 10:13:33.000000 ocp_tessellate-2.3.1/tests/test_color.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1200 2023-06-19 17:26:20.000000 ocp_tessellate-2.3.1/tests/test_coordsystem.py
--rw-r--r--   0 bernhard   (501) staff       (20)     2027 2024-04-18 06:18:09.000000 ocp_tessellate-2.3.1/tests/test_instances.py
--rw-r--r--   0 bernhard   (501) staff       (20)      516 2023-06-19 19:05:58.000000 ocp_tessellate-2.3.1/tests/test_parallel.py
--rw-r--r--   0 bernhard   (501) staff       (20)      870 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.1/tests/test_partgroup.py
--rw-r--r--   0 bernhard   (501) staff       (20)      637 2023-06-19 17:37:19.000000 ocp_tessellate-2.3.1/tests/test_stl.py
--rw-r--r--   0 bernhard   (501) staff       (20)      811 2024-03-21 20:15:15.000000 ocp_tessellate-2.3.1/tests/tests_build123d assembly.py
--rw-r--r--   0 bernhard   (501) staff       (20)     8564 2024-01-17 07:33:06.000000 ocp_tessellate-2.3.1/tests/tests_build123d hinge.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3328 2023-11-28 20:16:07.000000 ocp_tessellate-2.3.1/tests/tests_build123d.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1879 2023-07-21 16:20:28.000000 ocp_tessellate-2.3.1/tests/tests_cadquery.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3022 2023-06-19 17:42:50.000000 ocp_tessellate-2.3.1/tests/tests_cadquery_boxes.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3697 2023-07-21 16:20:28.000000 ocp_tessellate-2.3.1/tests/tests_cadquery_door.py
--rw-r--r--   0 bernhard   (501) staff       (20)     8496 2023-11-21 06:59:53.000000 ocp_tessellate-2.3.1/tests/tests_cadquery_hexapod.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:39:28.569401 ocp_tessellate-2.3.2/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1109 2024-04-22 06:39:28.569320 ocp_tessellate-2.3.2/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-2.3.2/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:39:28.566524 ocp_tessellate-2.3.2/ocp_tessellate/
+-rw-r--r--   0 bernhard   (501) staff       (20)     2942 2024-04-14 10:24:20.000000 ocp_tessellate-2.3.2/ocp_tessellate/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1123 2024-04-20 11:53:24.000000 ocp_tessellate-2.3.2/ocp_tessellate/_version.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4452 2024-04-20 12:24:45.000000 ocp_tessellate-2.3.2/ocp_tessellate/b123d_assembly.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    15298 2024-04-22 06:38:46.000000 ocp_tessellate-2.3.2/ocp_tessellate/cad_objects.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    34183 2024-04-22 06:38:46.000000 ocp_tessellate-2.3.2/ocp_tessellate/convert.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10324 2024-04-20 16:35:57.000000 ocp_tessellate-2.3.2/ocp_tessellate/defaults.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    25136 2024-03-14 07:11:29.000000 ocp_tessellate-2.3.2/ocp_tessellate/ocp_utils.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13711 2024-04-20 12:25:36.000000 ocp_tessellate-2.3.2/ocp_tessellate/stepreader.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    18104 2024-04-22 06:38:46.000000 ocp_tessellate-2.3.2/ocp_tessellate/tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1065 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.2/ocp_tessellate/trace.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     6177 2024-04-14 10:38:44.000000 ocp_tessellate-2.3.2/ocp_tessellate/utils.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:39:28.568910 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1109 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      949 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)      112 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       15 2024-04-22 06:39:28.000000 ocp_tessellate-2.3.2/ocp_tessellate.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      671 2024-04-22 06:39:28.569654 ocp_tessellate-2.3.2/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1627 2024-04-21 12:51:04.000000 ocp_tessellate-2.3.2/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:39:28.568755 ocp_tessellate-2.3.2/tests/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1419 2024-03-21 20:20:19.000000 ocp_tessellate-2.3.2/tests/test_cache.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1100 2024-04-18 07:02:00.000000 ocp_tessellate-2.3.2/tests/test_cadquery_sketch.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      895 2024-04-18 06:37:27.000000 ocp_tessellate-2.3.2/tests/test_color.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1200 2023-06-19 17:26:20.000000 ocp_tessellate-2.3.2/tests/test_coordsystem.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1999 2024-04-18 06:38:50.000000 ocp_tessellate-2.3.2/tests/test_instances.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      486 2024-04-20 16:35:15.000000 ocp_tessellate-2.3.2/tests/test_parallel.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      870 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.2/tests/test_partgroup.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      766 2024-04-20 11:45:07.000000 ocp_tessellate-2.3.2/tests/test_stl.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      811 2024-04-18 06:53:11.000000 ocp_tessellate-2.3.2/tests/tests_build123d assembly.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     8564 2024-04-22 06:37:55.000000 ocp_tessellate-2.3.2/tests/tests_build123d hinge.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3328 2023-11-28 20:16:07.000000 ocp_tessellate-2.3.2/tests/tests_build123d.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1879 2023-07-21 16:20:28.000000 ocp_tessellate-2.3.2/tests/tests_cadquery.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3022 2023-06-19 17:42:50.000000 ocp_tessellate-2.3.2/tests/tests_cadquery_boxes.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3697 2023-07-21 16:20:28.000000 ocp_tessellate-2.3.2/tests/tests_cadquery_door.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     8496 2023-11-21 06:59:53.000000 ocp_tessellate-2.3.2/tests/tests_cadquery_hexapod.py
```

### Comparing `ocp_tessellate-2.3.1/PKG-INFO` & `ocp_tessellate-2.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_tessellate
-Version: 2.3.1
+Version: 2.3.2
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -18,14 +18,14 @@
 Requires-Python: >=3.9
 Requires-Dist: webcolors~=1.12
 Requires-Dist: numpy
 Requires-Dist: numpy-quaternion
 Requires-Dist: cachetools~=5.2.0
 Requires-Dist: imagesize
 Provides-Extra: dev
+Requires-Dist: bumpversion; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pyYaml; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: twine; extra == "dev"
-Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: pyYaml; extra == "dev"
 
 Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs
```

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate/__init__.py` & `ocp_tessellate-2.3.2/ocp_tessellate/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate/_version.py` & `ocp_tessellate-2.3.2/ocp_tessellate/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     r = re.compile(
         r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\-{0,1}(?P<release>\D*)(?P<build>\d*)"
     )
     major, minor, patch, release, build = r.match(version).groups()
     return VersionInfo(major, minor, patch, release, build)
 
 
-__version__ = "2.3.1"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "2.3.2"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
```

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate/cad_objects.py` & `ocp_tessellate-2.3.2/ocp_tessellate/cad_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     discretize_edges,
     tessellate,
     compute_quality,
     face_mapper,
     edge_mapper,
     vertex_mapper,
 )
-from .mp_tessellator import is_apply_result, mp_tessellate, init_pool, keymap
 from .defaults import get_default
 import imagesize
 
 UNSELECTED = 0
 SELECTED = 1
 EMPTY = 3
 
@@ -78,15 +77,14 @@
         instances,
         meshed_instances,
         loc,
         deviation,
         angular_tolerance,
         edge_accuracy,
         render_edges,
-        parallel,
         progress,
         timeit,
     ):
         raise NotImplementedError("not implemented yet")
 
 
 class OCP_Part(CADObject):
@@ -127,15 +125,14 @@
         instances,
         meshed_instances,
         loc,
         deviation,
         angular_tolerance,
         edge_accuracy,
         render_edges,
-        parallel=False,
         progress=None,
         timeit=False,
     ):
         self.id = f"{path}/{self.name}"
 
         if isinstance(self.shape, dict):
             ind = self.shape["ref"]
@@ -159,16 +156,15 @@
                 # A first rough estimate of the bounding box.
                 # Will be too large, but is sufficient for computing the quality
                 bb = bounding_box(shape, loc=get_location(loc), optimal=False)
                 quality = compute_quality(bb, deviation=deviation)
                 t.info = str(bb)
 
             with Timer(timeit, self.name, "tessellate:     ", 2) as t:
-                func = mp_tessellate if parallel else tessellate
-                mesh = func(
+                mesh = tessellate(
                     shape,
                     self.cache_id,
                     deviation=deviation,
                     quality=quality,
                     angular_tolerance=angular_tolerance,
                     debug=timeit,
                     compute_edges=render_edges,
@@ -179,31 +175,22 @@
                 t.info = f"{{quality:{quality:.4f}, angular_tolerance:{angular_tolerance:.2f}}}"
 
         with Timer(timeit, self.name, "bounding box:   ", 2):
             combined_loc = get_location(loc, False)
             if self.loc is not None:
                 combined_loc = combined_loc * self.loc
             t, q = loc_to_tq(combined_loc)
+            bb = np_bbox(mesh["vertices"], t, q)
+            # store the instance mesh
+            if ind is not None and meshed_instances[ind].mesh is None:
+                meshed_instances[ind].mesh = mesh
+                meshed_instances[ind].quality = quality
 
-            if parallel and is_apply_result(mesh):
-                # store the instance mesh
-                if ind is not None and meshed_instances[ind].mesh is None:
-                    meshed_instances[ind].mesh = mesh
-                    meshed_instances[ind].quality = quality
-                mesh = {"ref": ind, "t": t, "q": q}
-                bb = {}
-            else:
-                bb = np_bbox(mesh["vertices"], t, q)
-                # store the instance mesh
-                if ind is not None and meshed_instances[ind].mesh is None:
-                    meshed_instances[ind].mesh = mesh
-                    meshed_instances[ind].quality = quality
-
-                if isinstance(self.shape, dict):
-                    mesh = self.shape  # return the instance id
+            if isinstance(self.shape, dict):
+                mesh = self.shape  # return the instance id
 
         if isinstance(self.color, tuple):
             color = [c.web_color for c in self.color]  # pylint: disable=not-an-iterable
             alpha = 1.0
         else:
             color = self.color.web_color
             alpha = self.color.a
@@ -286,15 +273,14 @@
         instances,
         meshed_instances,
         loc,
         deviation,
         angular_tolerance,
         edge_accuracy,
         render_edges,
-        parallel=False,
         progress=None,
         timeit=False,
     ):
         self.id = f"{path}/{self.name}"
 
         with Timer(timeit, self.name, "bounding box:", 2) as t:
             bb = bounding_box(self.shape, loc=get_location(loc))
@@ -349,15 +335,14 @@
         instances,
         meshed_instances,
         loc,
         deviation,
         angular_tolerance,
         edge_accuracy,
         render_edges,
-        parallel=False,
         progress=None,
         timeit=False,
     ):
         self.id = f"{path}/{self.name}"
 
         bb = bounding_box(self.shape, loc=get_location(loc))
         vertices = convert_vertices(self.shape, self.id)
@@ -408,15 +393,14 @@
         instances,
         meshed_instances,
         loc,
         deviation,
         angular_tolerance,
         edge_accuracy,
         render_edges,
-        parallel=False,
         progress=None,
         timeit=False,
     ):
         self.id = f"{path}/{self.name}"
 
         if loc is None and self.loc is None:
             combined_loc = None
@@ -441,15 +425,14 @@
                 instances,
                 meshed_instances,
                 combined_loc,
                 deviation,
                 angular_tolerance,
                 edge_accuracy,
                 render_edges,
-                parallel,
                 progress,
                 timeit,
             )
             result["parts"].append(mesh)
             map["parts"].append(mapping)
         return map, result
```

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate/convert.py` & `ocp_tessellate-2.3.2/ocp_tessellate/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     OCP_Edges,
     OCP_Faces,
     OCP_Part,
     OCP_PartGroup,
     OCP_Vertices,
 )
 from .defaults import get_default, preset
-from .mp_tessellator import get_mp_result, is_apply_result
 from .ocp_utils import (
     BoundingBox,
     copy_shape,
     downcast,
     get_downcasted_shape,
     get_edges,
     get_faces,
@@ -124,15 +123,14 @@
         instances,
         meshed_instances,
         None,
         deviation=preset("deviation", kwargs.get("deviation")),
         angular_tolerance=preset("angular_tolerance", kwargs.get("angular_tolerance")),
         edge_accuracy=preset("edge_accuracy", kwargs.get("edge_accuracy")),
         render_edges=preset("render_edges", kwargs.get("render_edges")),
-        parallel=kwargs.get("parallel"),
         progress=progress,
         timeit=timeit,
     )
     states = group.to_state()
 
     return [instance.mesh for instance in meshed_instances], shapes, states, mapping
 
@@ -156,39 +154,14 @@
                 bb = c_bb(shape, bb)
         return bb
 
     bb = c_bb(shapes, None)
     return bb
 
 
-def mp_get_results(instances, shapes, progress):
-    def walk(shapes):
-        for shape in shapes["parts"]:
-            if shape.get("parts") is None:
-                if shape.get("type") == "shapes":
-                    mesh = instances[shape["shape"]["ref"]]
-                    t = shape["shape"].get("t")
-                    q = shape["shape"].get("q")
-                    shape["shape"] = {"ref": shape["shape"]["ref"]}  # remove t and q
-                    shape["bb"] = np_bbox(mesh["vertices"], t, q)
-
-                    if progress is not None:
-                        progress.update("r")
-            else:
-                walk(shape)
-
-    for i in range(len(instances)):
-        if is_apply_result(instances[i]):
-            instances[i] = get_mp_result(instances[i])
-
-    walk(shapes)
-
-    return instances, shapes
-
-
 def get_accuracies(shapes):
     def _get_accuracies(shapes, lengths):
         if shapes.get("parts"):
             for shape in shapes["parts"]:
                 _get_accuracies(shape, lengths)
         elif shapes.get("type") == "shapes":
             accuracies[shapes["id"]] = shapes["accuracy"]
```

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate/defaults.py` & `ocp_tessellate-2.3.2/ocp_tessellate/defaults.py`

 * *Files 13% similar despite different names*

```diff
@@ -77,32 +77,26 @@
         - direct_intensity    Intensity of direct lights (default=0.15)
         - show_parent:        Show the parent for edges, faces and vertices objects (default=False)
         - show_sketch_local:  In build123d show local sketch in addition to relocate sketch (default=True)
         - show_bbox:          Show bounding box (default=False)
         - tools:              Show the viewer tools like the object tree (default=True)
         - glass:              Show the viewer in glass mode, i.e (CAD navigation as transparent overlay (default=False)
         - timeit:             Show rendering times, levels = False, 0,1,2,3,4,5 (default=False)
-        - parallel:           (Linux only) Whether to use multiprocessing for parallel tessellation
         - js_debug:           Enable debug output in browser console (default=False)
 
         NOT SUPPORTED ANY MORE:
         - mac_scrollbar       The default now
         - bb_factor:          Removed
         - display             Use 'viewer="<viewer title>"' (for sidecar display) or 'viewer=None' (for cell display)
         - quality             Use 'deviation'to control smoothness of rendered edges
         """
 
         for k, v in kwargs.items():
             if self.get_default(k, float("nan")) == float("nan"):
                 print(f"Paramater {k} is not a valid argument for show()")
-
-            # elif k == "parallel" and v and platform.system() != "Linux":
-            #     warn("parallel=True only works on Linux. Setting parallel=False")
-            #     self.defaults[k] = False
-
             else:
                 self.defaults[k] = v
 
     def reset_defaults(self):
         self.defaults = {
             #
             # display options
@@ -124,15 +118,14 @@
             "default_edgecolor": "#707070",
             "default_opacity": 0.5,
             "optimal_bb": False,
             "render_normals": False,
             "render_edges": True,
             "render_mates": False,
             "render_joints": False,
-            "parallel": False,
             "helper_scale": 1,
             #
             # viewer options
             #
             "control": "trackball",
             "up": "Z",
             "axes": False,
@@ -285,15 +278,14 @@
             "optimal_bb",
             "render_normals",
             "render_edges",
             "render_mates",
             "render_joints",
             "helper_scale",
             "quality",
-            "parallel",
         ]
     }
 
 
 def show_args(config):
     args = create_args(config)
     args.update(add_shape_args(config))
```

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate/ocp_utils.py` & `ocp_tessellate-2.3.2/ocp_tessellate/ocp_utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate/stepreader.py` & `ocp_tessellate-2.3.2/ocp_tessellate/stepreader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 import os
 import time
 import unicodedata
 
-import cadquery as cq
+try:
+    import cadquery as cq
+except:
+    pass
+
+try:
+    from build123d import *
+    from .b123d_assembly import Assembly, reference
+
+except:
+    pass
+
 from OCP.Quantity import Quantity_ColorRGBA
 from OCP.STEPCAFControl import STEPCAFControl_Reader
 from OCP.TCollection import TCollection_AsciiString, TCollection_ExtendedString
 from OCP.TDataStd import TDataStd_Name
 from OCP.TDF import TDF_ChildIterator, TDF_Label, TDF_LabelSequence
 from OCP.TDocStd import TDocStd_Document
 from OCP.TopAbs import TopAbs_COMPOUND, TopAbs_COMPSOLID, TopAbs_FACE, TopAbs_SOLID
@@ -300,17 +311,19 @@
                 if names.get(name) is None:
                     names[name] = 0
                 else:
                     names[name] += 1
                 name = f"{obj['name']}_{names[name]}"
 
                 a.add(
-                    to_workplane(obj["shape"])
-                    if obj["shapes"] is None
-                    else walk(obj["shapes"]),
+                    (
+                        to_workplane(obj["shape"])
+                        if obj["shapes"] is None
+                        else walk(obj["shapes"])
+                    ),
                     name=name,
                     color=None if obj["color"] is None else cq.Color(*obj["color"]),
                     loc=cq.Location(obj.get("loc")),
                 )
 
             return a
 
@@ -337,58 +350,62 @@
                 )
 
         if path != None:
             result = result.objects[path].obj
 
         return result
 
-    # def save_assembly(self, filename):
-    #     """
-    #     Cache the STEP file in a pickle file with binary BRep buffers
-    #     :param filename: name of the cache object
-    #     """
-
-    #     def _save_assembly(assemblies):
-    #         if assemblies is None:
-    #             return None
-
-    #         result = []
-    #         for assembly in assemblies:
-    #             obj = self._create_assembly_object(
-    #                 assembly["name"],
-    #                 loc_to_tq(assembly["loc"]),
-    #                 assembly["color"],
-    #                 serialize(assembly["shape"]),
-    #                 _save_assembly(assembly["shapes"]),
-    #             )
-    #             result.append(obj)
-    #         return result
-
-    #     objs = _save_assembly(self.assemblies)
-    #     with open(filename, "wb") as fd:
-    #         pickle.dump(objs, fd)
-
-    # def load_assembly(self, filename):
-    #     """
-    #     Load the STEP file from a pickle file with binary BRep buffers.
-    #     The result will be stores as a list of AssemblyObjects in self.assemblies
-    #     :param filename: name of the cache object
-    #     """
-
-    #     def _load_assembly(objs):
-    #         if objs is None:
-    #             return None
-
-    #         result = []
-    #         for obj in objs:
-    #             assembly = self._create_assembly_object(
-    #                 obj["name"],
-    #                 tq_to_loc(*obj["loc"]),
-    #                 obj["color"],
-    #                 deserialize(obj["shape"]),
-    #                 _load_assembly(obj["shapes"]),
-    #             )
-    #             result.append(assembly)
-    #         return result
+    def to_build123d(self):
+        """
+        Convert internal AssemblyObjects format to build123d Assemblies
+        :return: buiild123d assembly
+        """
+
+        def walk(objs, label=None, loc=None):
+            a = []
+            names = {}
+            for obj in objs:
+                label = obj["name"]
+
+                # Create a unique name by postfixing the enumerator index if needed
+                if names.get(label) is None:
+                    names[label] = 0
+                else:
+                    names[label] += 1
+                label = f"{obj['name']}_{names[label]}"
+
+                a.append(
+                    reference(
+                        (
+                            Compound(obj["shape"])
+                            if obj["shapes"] is None
+                            else walk(obj["shapes"])
+                        ),
+                        label=label,
+                        color=None if obj["color"] is None else Color(*obj["color"]),
+                        location=Location(obj.get("loc")),
+                    )
+                )
+            return Assembly(label=label, children=a, location=loc)
+
+        if len(self.assemblies) == 0 or (
+            self.assemblies[0]["shapes"] is not None
+            and len(self.assemblies[0]["shapes"]) == 0
+        ):
+            raise ValueError("Empty assembly list")
+
+        if len(self.assemblies) == 1:
+            assembly = self.assemblies[0]
+            return walk(assembly["shapes"], assembly["name"], Location(assembly["loc"]))
+        else:
+            children = []
+            for assembly in self.assemblies:
+                children.append(
+                    walk(
+                        assembly["shapes"],
+                        assembly["name"],
+                        Location(assembly["loc"]),
+                    )
+                )
+            result = Assembly(label="Group", children=children)
 
-    #     with open(filename, "rb") as fd:
-    #         self.assemblies = _load_assembly(pickle.load(fd))
+        return result
```

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate/tessellator.py` & `ocp_tessellate-2.3.2/ocp_tessellate/tessellator.py`

 * *Files 2% similar despite different names*

```diff
@@ -386,18 +386,19 @@
         quality,
         angular_tolerance,
         compute_faces=True,
         compute_edges=True,
         debug=False,
     ):
         self.mesh = tessellate_c(
-            # shape, quality, angular_tolerance, parallel=True, debug=debug, timeit=debug
             shape,
             quality,
             angular_tolerance,
+            compute_faces,
+            compute_edges,
             True,
             0,
             debug,
         )
 
     def get_vertices(self):
         return self.mesh.vertices
```

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate/trace.py` & `ocp_tessellate-2.3.2/ocp_tessellate/trace.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate/utils.py` & `ocp_tessellate-2.3.2/ocp_tessellate/utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate.egg-info/PKG-INFO` & `ocp_tessellate-2.3.2/ocp_tessellate.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_tessellate
-Version: 2.3.1
+Version: 2.3.2
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -18,14 +18,14 @@
 Requires-Python: >=3.9
 Requires-Dist: webcolors~=1.12
 Requires-Dist: numpy
 Requires-Dist: numpy-quaternion
 Requires-Dist: cachetools~=5.2.0
 Requires-Dist: imagesize
 Provides-Extra: dev
+Requires-Dist: bumpversion; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pyYaml; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: twine; extra == "dev"
-Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: pyYaml; extra == "dev"
 
 Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs
```

### Comparing `ocp_tessellate-2.3.1/ocp_tessellate.egg-info/SOURCES.txt` & `ocp_tessellate-2.3.2/ocp_tessellate.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 README.md
 setup.cfg
 setup.py
 ocp_tessellate/__init__.py
 ocp_tessellate/_version.py
+ocp_tessellate/b123d_assembly.py
 ocp_tessellate/cad_objects.py
 ocp_tessellate/convert.py
 ocp_tessellate/defaults.py
-ocp_tessellate/mp_tess.py
-ocp_tessellate/mp_tessellator.py
 ocp_tessellate/ocp_utils.py
 ocp_tessellate/stepreader.py
 ocp_tessellate/tessellator.py
 ocp_tessellate/trace.py
 ocp_tessellate/utils.py
 ocp_tessellate.egg-info/PKG-INFO
 ocp_tessellate.egg-info/SOURCES.txt
```

### Comparing `ocp_tessellate-2.3.1/setup.cfg` & `ocp_tessellate-2.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.3.1
+current_version = 2.3.2
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_tessellate-2.3.1/setup.py` & `ocp_tessellate-2.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 LONG_DESCRIPTION = (
     "Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs"
 )
 
 setup_args = {
     "name": "ocp_tessellate",
-    "version": "2.3.1",
+    "version": "2.3.2",
     "description": "Tessellate OCP objects",
     "long_description": LONG_DESCRIPTION,
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "webcolors~=1.12",
         "numpy",
```

### Comparing `ocp_tessellate-2.3.1/tests/test_cache.py` & `ocp_tessellate-2.3.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/tests/test_cadquery_sketch.py` & `ocp_tessellate-2.3.2/tests/test_cadquery_sketch.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/tests/test_color.py` & `ocp_tessellate-2.3.2/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/tests/test_coordsystem.py` & `ocp_tessellate-2.3.2/tests/test_coordsystem.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/tests/test_instances.py` & `ocp_tessellate-2.3.2/tests/test_instances.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 # %%
 
 b = Box(0.1, 0.1, 1)
 c = Cylinder(1, 0.5)
 p = Plane(c.faces().sort_by().last)
 b = [p * loc * b for loc in PolarLocations(0.7, 12)]
-c = Compound.make_compound(b + [c])
+c = Compound(b + [c])
 
 show(c, timeit=False)
 
 # %%
 
 show(*c.solids(), timeit=False)
 
@@ -111,11 +111,11 @@
 p = Plane(c.faces().sort_by().last)
 b = [copy.copy(b).move(p.location * loc) for loc in PolarLocations(0.7, 12)]
 
 show(*b, timeit=False)
 
 
 # %%
-c = Compound.make_compound(b + [c])
+c = Compound(b + [c])
 show(*c.solids(), timeit=False)
 
 # %%
```

### Comparing `ocp_tessellate-2.3.1/tests/test_partgroup.py` & `ocp_tessellate-2.3.2/tests/test_partgroup.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/tests/tests_build123d assembly.py` & `ocp_tessellate-2.3.2/tests/tests_build123d assembly.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/tests/tests_build123d hinge.py` & `ocp_tessellate-2.3.2/tests/tests_build123d hinge.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/tests/tests_build123d.py` & `ocp_tessellate-2.3.2/tests/tests_build123d.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/tests/tests_cadquery.py` & `ocp_tessellate-2.3.2/tests/tests_cadquery.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/tests/tests_cadquery_boxes.py` & `ocp_tessellate-2.3.2/tests/tests_cadquery_boxes.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/tests/tests_cadquery_door.py` & `ocp_tessellate-2.3.2/tests/tests_cadquery_door.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.3.1/tests/tests_cadquery_hexapod.py` & `ocp_tessellate-2.3.2/tests/tests_cadquery_hexapod.py`

 * *Files identical despite different names*

