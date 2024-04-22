# Comparing `tmp/plpygis-0.3.0.tar.gz` & `tmp/plpygis-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plpygis-0.3.0.tar", last modified: Mon Apr  8 19:26:07 2024, max compression
+gzip compressed data, was "plpygis-0.4.0.tar", last modified: Mon Apr 22 00:59:21 2024, max compression
```

## Comparing `plpygis-0.3.0.tar` & `plpygis-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,22 @@
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.497663 plpygis-0.3.0/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.490996 plpygis-0.3.0/.github/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.490996 plpygis-0.3.0/.github/workflows/
--rw-r--r--   0 ben       (1000) ben       (1000)      606 2024-03-08 17:37:46.000000 plpygis-0.3.0/.github/workflows/pythonpackage.yml
--rw-r--r--   0 ben       (1000) ben       (1000)     1172 2024-03-08 10:22:13.000000 plpygis-0.3.0/.gitignore
--rw-r--r--   0 ben       (1000) ben       (1000)      828 2024-04-08 19:20:38.000000 plpygis-0.3.0/.readthedocs.yaml
--rw-r--r--   0 ben       (1000) ben       (1000)     1107 2024-04-08 19:23:50.000000 plpygis-0.3.0/CHANGELOG.md
--rw-r--r--   0 ben       (1000) ben       (1000)    35142 2024-03-08 10:22:13.000000 plpygis-0.3.0/LICENSE
--rw-r--r--   0 ben       (1000) ben       (1000)      102 2024-03-08 10:22:13.000000 plpygis-0.3.0/MANIFEST.in
--rw-r--r--   0 ben       (1000) ben       (1000)      203 2024-03-08 10:22:13.000000 plpygis-0.3.0/Makefile
--rw-r--r--   0 ben       (1000) ben       (1000)     2335 2024-04-08 19:26:07.494330 plpygis-0.3.0/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)     1860 2024-03-08 10:22:13.000000 plpygis-0.3.0/README.rst
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.490996 plpygis-0.3.0/doc/
--rw-r--r--   0 ben       (1000) ben       (1000)      610 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/Makefile
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.494330 plpygis-0.3.0/doc/source/
--rw-r--r--   0 ben       (1000) ben       (1000)     4903 2024-04-08 19:14:37.000000 plpygis-0.3.0/doc/source/conf.py
--rw-r--r--   0 ben       (1000) ben       (1000)     8289 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/source/examples.rst
--rw-r--r--   0 ben       (1000) ben       (1000)      678 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/source/index.rst
--rw-r--r--   0 ben       (1000) ben       (1000)     1395 2024-04-03 07:00:40.000000 plpygis-0.3.0/doc/source/installation.rst
--rw-r--r--   0 ben       (1000) ben       (1000)      240 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/source/plpygis.rst
--rw-r--r--   0 ben       (1000) ben       (1000)     9484 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/source/plpython.rst
--rw-r--r--   0 ben       (1000) ben       (1000)     8671 2024-04-08 19:14:37.000000 plpygis-0.3.0/doc/source/subclasses.rst
--rw-r--r--   0 ben       (1000) ben       (1000)     3918 2024-03-08 10:22:13.000000 plpygis-0.3.0/doc/source/usage.rst
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.494330 plpygis-0.3.0/plpygis/
--rw-r--r--   0 ben       (1000) ben       (1000)      156 2024-03-08 10:22:13.000000 plpygis-0.3.0/plpygis/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)       22 2024-04-08 19:14:37.000000 plpygis-0.3.0/plpygis/_version.py
--rw-r--r--   0 ben       (1000) ben       (1000)     1233 2024-03-08 10:22:13.000000 plpygis-0.3.0/plpygis/exceptions.py
--rw-r--r--   0 ben       (1000) ben       (1000)    30983 2024-04-08 19:14:37.000000 plpygis-0.3.0/plpygis/geometry.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2676 2024-03-08 10:22:13.000000 plpygis-0.3.0/plpygis/hex.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.494330 plpygis-0.3.0/plpygis.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)     2335 2024-04-08 19:26:07.000000 plpygis-0.3.0/plpygis.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)      719 2024-04-08 19:26:07.000000 plpygis-0.3.0/plpygis.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        1 2024-04-08 19:26:07.000000 plpygis-0.3.0/plpygis.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       34 2024-04-08 19:26:07.000000 plpygis-0.3.0/plpygis.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        8 2024-04-08 19:26:07.000000 plpygis-0.3.0/plpygis.egg-info/top_level.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       28 2024-03-08 11:17:40.000000 plpygis-0.3.0/requirements-test.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       32 2024-03-08 11:03:58.000000 plpygis-0.3.0/requirements.txt
--rw-r--r--   0 ben       (1000) ben       (1000)       38 2024-04-08 19:26:07.497663 plpygis-0.3.0/setup.cfg
--rw-r--r--   0 ben       (1000) ben       (1000)      750 2024-03-08 11:04:02.000000 plpygis-0.3.0/setup.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.494330 plpygis-0.3.0/test/
--rw-r--r--   0 ben       (1000) ben       (1000)       23 2024-03-08 10:22:13.000000 plpygis-0.3.0/test/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)       56 2024-03-08 10:22:13.000000 plpygis-0.3.0/test/__main__.py
--rw-r--r--   0 ben       (1000) ben       (1000)      180 2024-03-08 10:22:13.000000 plpygis-0.3.0/test/multipoint.shp
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-08 19:26:07.494330 plpygis-0.3.0/test/plpygis/
--rw-r--r--   0 ben       (1000) ben       (1000)      252 2024-03-08 10:22:13.000000 plpygis-0.3.0/test/plpygis/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)    22629 2024-04-08 19:14:37.000000 plpygis-0.3.0/test/plpygis/geometry.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-22 00:59:21.690892 plpygis-0.4.0/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2492 2024-04-22 00:53:22.000000 plpygis-0.4.0/CHANGELOG.md
+-rw-r--r--   0 ben       (1000) ben       (1000)    35142 2024-03-08 10:22:13.000000 plpygis-0.4.0/LICENSE
+-rw-r--r--   0 ben       (1000) ben       (1000)      101 2024-04-22 00:53:22.000000 plpygis-0.4.0/MANIFEST.in
+-rw-r--r--   0 ben       (1000) ben       (1000)     2472 2024-04-22 00:59:21.690892 plpygis-0.4.0/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)     1671 2024-04-22 00:53:22.000000 plpygis-0.4.0/README.md
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-22 00:59:21.690892 plpygis-0.4.0/plpygis/
+-rw-r--r--   0 ben       (1000) ben       (1000)      436 2024-04-22 00:53:22.000000 plpygis-0.4.0/plpygis/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)       22 2024-04-22 00:53:22.000000 plpygis-0.4.0/plpygis/_version.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     1615 2024-04-22 00:53:22.000000 plpygis-0.4.0/plpygis/exceptions.py
+-rw-r--r--   0 ben       (1000) ben       (1000)    32122 2024-04-22 00:53:22.000000 plpygis-0.4.0/plpygis/geometry.py
+-rw-r--r--   0 ben       (1000) ben       (1000)     3085 2024-04-22 00:53:22.000000 plpygis-0.4.0/plpygis/hex.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-22 00:59:21.690892 plpygis-0.4.0/plpygis.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)     2472 2024-04-22 00:59:21.000000 plpygis-0.4.0/plpygis.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)      330 2024-04-22 00:59:21.000000 plpygis-0.4.0/plpygis.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2024-04-22 00:59:21.000000 plpygis-0.4.0/plpygis.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)       70 2024-04-22 00:59:21.000000 plpygis-0.4.0/plpygis.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        8 2024-04-22 00:59:21.000000 plpygis-0.4.0/plpygis.egg-info/top_level.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)      841 2024-04-22 00:53:22.000000 plpygis-0.4.0/pyproject.toml
+-rw-r--r--   0 ben       (1000) ben       (1000)       38 2024-04-22 00:59:21.690892 plpygis-0.4.0/setup.cfg
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2024-04-22 00:59:21.690892 plpygis-0.4.0/test/
+-rw-r--r--   0 ben       (1000) ben       (1000)    23345 2024-04-22 00:53:22.000000 plpygis-0.4.0/test/test_geometry.py
```

### Comparing `plpygis-0.3.0/LICENSE` & `plpygis-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plpygis-0.3.0/PKG-INFO` & `plpygis-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 Metadata-Version: 2.1
 Name: plpygis
-Version: 0.3.0
-Summary: PostGIS Python tools
-Home-page: https://github.com/bosth/plpygis
-Author: Benjamin Trigona-Harany
-Author-email: plpygis@jaxartes.net
+Version: 0.4.0
+Summary: Python tools for PostGIS
+Author-email: Benjamin Trigona-Harany <plpygis@jaxartes.net>
 License: GPL-3.0-only
-Keywords: gis geospatial postgis postgresql plpython
-Platform: any
+Project-URL: Homepage, https://github.com/bosth/plpygis
+Project-URL: Issues, https://github.com/bosth/plpygis/issues
+Project-URL: Documentation, https://plpygis.readthedocs.io/
+Keywords: gis,geospatial,postgis,postgresql,pl/python
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: GIS
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pyshp; extra == "test"
+Requires-Dist: Shapely>=2.0.2; extra == "test"
 Provides-Extra: shapely-support
 Requires-Dist: Shapely>=2.0.2; extra == "shapely-support"
 
-=======
-plpygis
-=======
-
-``plpygis`` is a Python tool that can convert a `PostGIS <https://postgis.net/>`_ ``geometry`` into an equivalent WKB, EWKB, GeoJSON or Shapely geometry. ``plpygis`` is intended for use in PostgreSQL `PL/Python <https://www.postgresql.org/docs/current/plpython.html>`_ functions.
-
-Basic usage
-===========
-
-The ``Geometry`` class and its subclasses can be used to convert to and from PostGIS geometries. The following example will take a PostGIS multipolygon geometry named ``geom`` and find its largest component polygon.
-
-``Geometry()`` can convert a PostGIS ``geometry`` that has been passed as a parameter to a PL/Python function. A ``Geometry`` that is returned from the PL/Python function will automatically be converted back to a PostGIS ``geometry``.
-
-.. code-block:: postgres
- 
-    CREATE OR REPLACE FUNCTION largest_poly(geom geometry)
-      RETURNS geometry 
-    AS $$
-      from plpygis import Geometry
-      polygons = Geometry(geom)
-      if polygons.type == "Polygon":
-          return polygons
-      elif polygons.type == "MultiPolygon":
-          largest = max(polygons.shapely, key=lambda polygon: polygon.area)
-          return Geometry.from_shapely(largest)
-      else:
-          return None
-    $$ LANGUAGE plpython3u;
+# plpygis
+
+`plpygis` is a Python tool that can convert a [PostGIS](https://postgis.net/) `geometry` into an equivalent WKB, EWKB, GeoJSON or Shapely geometry. `plpygis` is intended for use in PostgreSQL [PL/Python](https://www.postgresql.org/docs/current/plpython.html) functions.
+
+## Basic usage
+
+The `Geometry` class and its subclasses can be used to convert to and from PostGIS geometries. The following example will take a PostGIS multipolygon geometry named `geom` and find its largest component polygon.
+
+`Geometry()` can convert a PostGIS `geometry` that has been passed as a parameter to a PL/Python function. A `Geometry` that is returned from the PL/Python function will automatically be converted back to a PostGIS `geometry`.
+
+``` postgres
+CREATE OR REPLACE FUNCTION largest_poly(geom geometry)
+  RETURNS geometry 
+AS $$
+  from plpygis import Geometry
+  polygons = Geometry(geom)
+  if polygons.type == "Polygon":
+      return polygons
+  elif polygons.type == "MultiPolygon":
+      largest = max(polygons.shapely, key=lambda polygon: polygon.area)
+      return Geometry.from_shapely(largest)
+  else:
+      return None
+$$ LANGUAGE plpython3u;
+```
 
 This can then be called as part of an SQL query:
 
-.. code-block:: postgres
+``` postgres
+SELECT largest_poly(geom) FROM countries;
+```
 
-    SELECT largest_poly(geom) FROM countries;
+## Documentation
 
-Documentation
-=============
+Full `plpygis` documentation is available at <http://plpygis.readthedocs.io/>.
 
-Full ``plpygis`` documentation is available at http://plpygis.readthedocs.io/.
+[![Continuous Integration](https://github.com/bosth/plpygis/workflows/tests/badge.svg)](https://github.com/bosth/plpygis/actions?query=workflow%3A%22tests%22) [![Documentation Status](https://readthedocs.org/projects/plpygis/badge/?version=latest)](http://plpygis.readthedocs.io/en/latest/?badge=latest)
 
-.. image:: https://readthedocs.org/projects/plpygis/badge/?version=latest
-    :target: http://plpygis.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-    
-.. image:: https://github.com/bosth/plpygis/workflows/tests/badge.svg
-    :target: https://github.com/bosth/plpygis/actions?query=workflow%3A%22tests%22
-    :alt: Continuous Integration
```

### Comparing `plpygis-0.3.0/README.rst` & `plpygis-0.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,38 @@
-=======
-plpygis
-=======
-
-``plpygis`` is a Python tool that can convert a `PostGIS <https://postgis.net/>`_ ``geometry`` into an equivalent WKB, EWKB, GeoJSON or Shapely geometry. ``plpygis`` is intended for use in PostgreSQL `PL/Python <https://www.postgresql.org/docs/current/plpython.html>`_ functions.
-
-Basic usage
-===========
-
-The ``Geometry`` class and its subclasses can be used to convert to and from PostGIS geometries. The following example will take a PostGIS multipolygon geometry named ``geom`` and find its largest component polygon.
-
-``Geometry()`` can convert a PostGIS ``geometry`` that has been passed as a parameter to a PL/Python function. A ``Geometry`` that is returned from the PL/Python function will automatically be converted back to a PostGIS ``geometry``.
-
-.. code-block:: postgres
- 
-    CREATE OR REPLACE FUNCTION largest_poly(geom geometry)
-      RETURNS geometry 
-    AS $$
-      from plpygis import Geometry
-      polygons = Geometry(geom)
-      if polygons.type == "Polygon":
-          return polygons
-      elif polygons.type == "MultiPolygon":
-          largest = max(polygons.shapely, key=lambda polygon: polygon.area)
-          return Geometry.from_shapely(largest)
-      else:
-          return None
-    $$ LANGUAGE plpython3u;
+# plpygis
+
+`plpygis` is a Python tool that can convert a [PostGIS](https://postgis.net/) `geometry` into an equivalent WKB, EWKB, GeoJSON or Shapely geometry. `plpygis` is intended for use in PostgreSQL [PL/Python](https://www.postgresql.org/docs/current/plpython.html) functions.
+
+## Basic usage
+
+The `Geometry` class and its subclasses can be used to convert to and from PostGIS geometries. The following example will take a PostGIS multipolygon geometry named `geom` and find its largest component polygon.
+
+`Geometry()` can convert a PostGIS `geometry` that has been passed as a parameter to a PL/Python function. A `Geometry` that is returned from the PL/Python function will automatically be converted back to a PostGIS `geometry`.
+
+``` postgres
+CREATE OR REPLACE FUNCTION largest_poly(geom geometry)
+  RETURNS geometry 
+AS $$
+  from plpygis import Geometry
+  polygons = Geometry(geom)
+  if polygons.type == "Polygon":
+      return polygons
+  elif polygons.type == "MultiPolygon":
+      largest = max(polygons.shapely, key=lambda polygon: polygon.area)
+      return Geometry.from_shapely(largest)
+  else:
+      return None
+$$ LANGUAGE plpython3u;
+```
 
 This can then be called as part of an SQL query:
 
-.. code-block:: postgres
+``` postgres
+SELECT largest_poly(geom) FROM countries;
+```
 
-    SELECT largest_poly(geom) FROM countries;
+## Documentation
 
-Documentation
-=============
+Full `plpygis` documentation is available at <http://plpygis.readthedocs.io/>.
 
-Full ``plpygis`` documentation is available at http://plpygis.readthedocs.io/.
+[![Continuous Integration](https://github.com/bosth/plpygis/workflows/tests/badge.svg)](https://github.com/bosth/plpygis/actions?query=workflow%3A%22tests%22) [![Documentation Status](https://readthedocs.org/projects/plpygis/badge/?version=latest)](http://plpygis.readthedocs.io/en/latest/?badge=latest)
 
-.. image:: https://readthedocs.org/projects/plpygis/badge/?version=latest
-    :target: http://plpygis.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-    
-.. image:: https://github.com/bosth/plpygis/workflows/tests/badge.svg
-    :target: https://github.com/bosth/plpygis/actions?query=workflow%3A%22tests%22
-    :alt: Continuous Integration
```

### Comparing `plpygis-0.3.0/plpygis/exceptions.py` & `plpygis-0.4.0/plpygis/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,66 @@
 class PlpygisError(Exception):
     """
     Basic exception for ``plpygis``.
     """
     def __init__(self, msg):
-        super(PlpygisError, self).__init__(msg)
-      
+        super().__init__(msg)
+
+
+class CoordinateError(PlpygisError):
+    """
+    Exception for problems in the coordinates of geometries.
+    """
+    def __init__(self, geom, msg=None):
+        if msg is None:
+            msg = f"Geometry has invalid coordinates: {geom}"
+        super().__init__(msg)
+
 
 class DependencyError(PlpygisError, ImportError):
     """
     Exception for a missing dependency.
     """
     def __init__(self, dep, msg=None):
         if msg is None:
-            msg = "Dependency '{}' is not available.".format(dep)
-        super(DependencyError, self).__init__(msg)
+            msg = f"Dependency '{dep}' is not available."
+        super().__init__(msg)
 
 
 class WkbError(PlpygisError):
     """
     Exception for problems in parsing WKBs.
     """
     def __init__(self, msg=None):
         if msg is None:
             msg = "Unreadable WKB."
-        super(WkbError, self).__init__(msg)
+        super().__init__(msg)
 
 
 class DimensionalityError(PlpygisError):
     """
     Exception for problems in dimensionality of geometries.
     """
     def __init__(self, msg=None):
         if msg is None:
             msg = "Geometry has invalid dimensionality."
-        super(DimensionalityError, self).__init__(msg)
+        super().__init__(msg)
 
 
 class SridError(PlpygisError):
     """
     Exception for problems in dimensionality of geometries.
     """
     def __init__(self, msg=None):
         if msg is None:
             msg = "Geometry has invalid SRID."
-        super(SridError, self).__init__(msg)
+        super().__init__(msg)
+
+
+class GeojsonError(PlpygisError):
+    """
+    Exception for problems in GeoJSONs.
+    """
+    def __init__(self, msg=None):
+        if msg is None:
+            msg = "Invalid GeoJSON."
+        super().__init__(msg)
```

### Comparing `plpygis-0.3.0/plpygis/geometry.py` & `plpygis-0.4.0/plpygis/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from .exceptions import DependencyError, WkbError, SridError, DimensionalityError
+import numbers
+from copy import copy
+from .exceptions import DependencyError, WkbError, SridError, DimensionalityError, CoordinateError, GeojsonError
 from .hex import HexReader, HexWriter, HexBytes
 
 try:
-    import shapely, shapely.wkb
+    import shapely
+    import shapely.wkb
     SHAPELY = True
 except ImportError:
     SHAPELY = False
 
 
-class Geometry(object):
+class Geometry():
     r"""A representation of a PostGIS geometry.
 
     PostGIS geometries are either an OpenGIS Consortium Simple Features for SQL
     specification type or a PostGIS extended type. The object's canonical form
     is stored in WKB or EWKB format along with an SRID and flags indicating
     whether the coordinates are 3DZ, 3DM or 4D.
 
@@ -64,68 +67,72 @@
 
     def __new__(cls, wkb, srid=None, dimz=False, dimm=False):
         if cls == Geometry:
             if not wkb:
                 raise WkbError("No EWKB provided")
             wkb = HexBytes(wkb)
             newcls, dimz, dimm, srid, reader = Geometry._from_wkb(wkb)
-            geom = super(Geometry, cls).__new__(newcls)
+            geom = super().__new__(newcls)
             geom._wkb = wkb
             geom._reader = reader
             geom._srid = srid
             geom._dimz = dimz
             geom._dimm = dimm
         else:
-            geom = super(Geometry, cls).__new__(cls)
+            geom = super().__new__(cls)
             geom._wkb = None
             geom._reader = None
         return geom
 
+    def __copy__(self):
+        cls = self.__class__
+        return cls(self.coordinates, self.srid, self.dimz, self.dimm)
+
     @staticmethod
     def from_geojson(geojson, srid=4326):
         """
         Create a Geometry from a GeoJSON. The SRID can be overridden from the
         expected 4326.
         """
         type_ = geojson["type"].lower()
         if type_ == "geometrycollection":
             geometries = []
             for geometry in geojson["geometries"]:
                 geometries.append(Geometry.from_geojson(geometry, srid=None))
             return GeometryCollection(geometries, srid)
-        elif type_ == "point":
+        if type_ == "point":
             return Point(geojson["coordinates"], srid=srid)
-        elif type_ == "linestring":
+        if type_ == "linestring":
             return LineString(geojson["coordinates"], srid=srid)
-        elif type_ == "polygon":
+        if type_ == "polygon":
             return Polygon(geojson["coordinates"], srid=srid)
-        elif type_ == "multipoint":
+        if type_ == "multipoint":
             geometries = _MultiGeometry._multi_from_geojson(geojson, Point)
             return MultiPoint(geometries, srid=srid)
-        elif type_ == "multilinestring":
+        if type_ == "multilinestring":
             geometries = _MultiGeometry._multi_from_geojson(geojson, LineString)
             return MultiLineString(geometries, srid=srid)
-        elif type_ == "multipolygon":
+        if type_ == "multipolygon":
             geometries = _MultiGeometry._multi_from_geojson(geojson, Polygon)
             return MultiPolygon(geometries, srid=srid)
+        raise GeojsonError(f"Invalid GeoJSON type: {type_}")
 
     @staticmethod
     def from_shapely(sgeom, srid=None):
         """
         Create a Geometry from a Shapely geometry and the specified SRID.
 
         The Shapely geometry will not be modified.
         """
         if SHAPELY:
             if srid:
                 sgeom = shapely.set_srid(sgeom, srid)
             wkb_hex = shapely.to_wkb(sgeom, include_srid=True, hex=True)
             return Geometry(wkb_hex)
-        else:
-            raise DependencyError("Shapely")
+        raise DependencyError("Shapely")
 
     @staticmethod
     def shape(shape, srid=None):
         """
         Create a Geometry using ``__geo_interface__`` and the specified SRID.
         """
         return Geometry.from_geojson(shape.__geo_interface__, srid)
@@ -146,20 +153,24 @@
 
     @srid.setter
     def srid(self, value):
         self._check_cache()
         self._srid = value
 
     @property
+    def coordinates(self):
+        return self._coordinates()
+
+    @property
     def geojson(self):
         """
         Get the geometry as a GeoJSON dict. There is no check that the
         GeoJSON is using an SRID of 4326.
         """
-        return self._to_geojson(dimz=self.dimz)
+        return self._to_geojson()
 
     @property
     def wkb(self):
         """
         Get the geometry as an (E)WKB.
         """
         return self._to_wkb(use_srid=True, dimz=self.dimz, dimm=self.dimm)
@@ -185,29 +196,28 @@
         """
         Get the type of the geometry in PostGIS format, including additional
         dimensions and SRID if they exist.
         """
         dimz = "Z" if self.dimz else ""
         dimm = "M" if self.dimm else ""
         if self.srid:
-            return "geometry({}{}{},{})".format(self.type, dimz, dimm, self.srid)
-        else:
-            return "geometry({}{}{})".format(self.type, dimz, dimm)
+            return f"geometry({self.type}{dimz}{dimm},{self.srid})"
+        return f"geometry({self.type}{dimz}{dimm})"
 
     @staticmethod
     def _from_wkb(wkb):
         try:
             if wkb.startswith(b"\x00"):
                 reader = HexReader(wkb, ">")  # big-endian reader
             elif wkb.startswith(b"\x01"):
                 reader = HexReader(wkb, "<")  # little-endian reader
             else:
                 raise WkbError("First byte in WKB must be 0 or 1.")
-        except TypeError:
-            raise WkbError()
+        except TypeError as e:
+            raise WkbError() from e
         return Geometry._get_wkb_type(reader) + (reader,)
 
     def _check_cache(self):
         if self._reader is not None:
             self._load_geometry()
             self._wkb = None
             self._reader = None
@@ -223,29 +233,28 @@
     def _to_shapely(self):
         if SHAPELY:
             sgeom = shapely.wkb.loads(self.wkb)
             srid = shapely.get_srid(sgeom)
             if srid == 0:
                 srid = None
             if (srid or self.srid) and srid != self.srid:
-                raise SridError("SRID mismatch: {} {}".format(srid, self.srid))
+                raise SridError(f"SRID mismatch: {srid} {self.srid}")
             return sgeom
-        else:
-            raise DependencyError("Shapely")
+        raise DependencyError("Shapely")
 
-    def _to_geojson(self, dimz):
-        coordinates = self._to_geojson_coordinates(dimz)
+    def _to_geojson(self):
+        coordinates = self._to_geojson_coordinates()
         geojson = {
                 "type": self.type,
                 "coordinates": coordinates
         }
         return geojson
 
     def __repr__(self):
-        return "<{}: '{}'>".format(self.type, self.postgis_type)
+        return f"<{self.type}: '{self.postgis_type}'>"
 
     def __str__(self):
         return self.wkb.__str__()
 
     @property
     def __geo_interface__(self):
         return self.geojson
@@ -277,31 +286,31 @@
         elif lwgeomtype == 5:
             cls = MultiLineString
         elif lwgeomtype == 6:
             cls = MultiPolygon
         elif lwgeomtype == 7:
             cls = GeometryCollection
         else:
-            raise WkbError("Unsupported WKB type: {}".format(lwgeomtype))
+            raise WkbError(f"Unsupported WKB type: {lwgeomtype}")
         return cls, dimz, dimm, srid
 
     @staticmethod
     def _read_wkb_header(reader):
         try:
             reader.get_char()
             header = reader.get_int()
             lwgeomtype = header & Geometry._WKBTYPE
             dimz = bool(header & Geometry._WKBZFLAG)
             dimm = bool(header & Geometry._WKBMFLAG)
             if header & Geometry._WKBSRIDFLAG:
                 srid = reader.get_int()
             else:
                 srid = None
-        except TypeError:
-            raise WkbError()
+        except TypeError as e:
+            raise WkbError() from e
         return lwgeomtype, dimz, dimm, srid
 
     def _write_wkb_header(self, writer, use_srid, dimz, dimm):
         writer.add_order()
         header = (self._LWGEOMTYPE |
                   (Geometry._WKBZFLAG if dimz else 0) |
                   (Geometry._WKBMFLAG if dimm else 0) |
@@ -309,14 +318,19 @@
         writer.add_int(header)
         if use_srid and self.srid:
             writer.add_int(self.srid)
         return writer
 
 
 class _MultiGeometry(Geometry):
+    def __copy__(self):
+        cls = self.__class__
+        geometries = [copy(geometry) for geometry in self.geometries]
+        return cls(geometries, self.srid)
+
     @property
     def dimz(self):
         """
         Whether the geometry has a Z dimension.
 
         :getter: ``True`` if the geometry has a Z dimension.
         :setter: Add or remove the Z dimension from this and all geometries in the collection.
@@ -349,18 +363,18 @@
             return
         for geometry in self.geometries:
             geometry.dimm = value
         self._dimm = value
 
     def _bounds(self):
         bounds = [g.bounds for g in self.geometries]
-        minx = min([b[0] for b in bounds])
-        miny = min([b[1] for b in bounds])
-        maxx = max([b[2] for b in bounds])
-        maxy = max([b[3] for b in bounds])
+        minx = min(b[0] for b in bounds)
+        miny = min(b[1] for b in bounds)
+        maxx = max(b[2] for b in bounds)
+        maxy = max(b[3] for b in bounds)
         return (minx, miny, maxx, maxy)
 
     @staticmethod
     def _multi_from_geojson(geojson, cls):
         geometries = []
         for coordinates in geojson["coordinates"]:
             geometry = cls(coordinates, srid=None)
@@ -381,32 +395,33 @@
             if self._dimm is None:
                 self._dimm = geometry.dimm
             elif self._dimm != geometry.dimm:
                 raise DimensionalityError("Mixed dimensionality in MultiGeometry")
             if geometry._srid is not None:
                 if self._srid != geometry._srid:
                     raise SridError("Geometry can not be different from SRID in MultiGeometry")
-                else:
-                    geometry._srid = None
+                geometry._srid = None
+
+    def _coordinates(self, dimz=True, dimm=True, tpl=True):
+        return [g._coordinates(dimz, dimm, tpl) for g in self.geometries]
 
-    def _to_geojson_coordinates(self, dimz):
-        coordinates = [g._to_geojson_coordinates(dimz=dimz) for g in self.geometries]
-        return coordinates
+    def _to_geojson_coordinates(self):
+        return self._coordinates(dimm=False, tpl=False)
 
     @staticmethod
     def _read_wkb(reader, dimz, dimm):
         geometries = []
         try:
             for _ in range(reader.get_int()):
                 cls, dimz, dimm, srid = Geometry._get_wkb_type(reader)
                 coordinates = cls._read_wkb(reader, dimz, dimm)
                 geometry = cls(coordinates, srid=srid, dimz=dimz, dimm=dimm)
                 geometries.append(geometry)
-        except TypeError:
-            raise WkbError()
+        except TypeError as e:
+            raise WkbError() from e
         return geometries
 
     def _write_wkb(self, writer, dimz, dimm):
         writer.add_int(len(self.geometries))
         for geometry in self.geometries:
             geometry._write_wkb_header(writer, False, dimz, dimm)
             geometry._write_wkb(writer, dimz, dimm)
@@ -432,22 +447,26 @@
     def __init__(self, coordinates=None, srid=None, dimz=False, dimm=False):
         if self._wkb:
             self._x = None
             self._y = None
             self._z = None
             self._m = None
         else:
+            for c in coordinates:
+                if c is None:
+                    continue
+                if not isinstance(c, numbers.Number):
+                    raise CoordinateError(f"Coordinates must be numeric: {coordinates}", coordinates)
             self._srid = srid
-            coordinates = list(coordinates)
             self._x = coordinates[0]
             self._y = coordinates[1]
             num = len(coordinates)
             if num > 4:
-                raise DimensionalityError("Maximum dimensionality supported for coordinates is 4: {}".format(coordinates))
-            elif num == 2:  # fill in Z and M if we are supposed to have them, else None
+                raise DimensionalityError(f"Maximum dimensionality supported for coordinates is 4: {coordinates}")
+            if num == 2:  # fill in Z and M if we are supposed to have them, else None
                 if dimz and dimm:
                     self._z = 0
                     self._m = 0
                 elif dimz:
                     self._z = 0
                     self._m = None
                 elif dimm:
@@ -463,16 +482,16 @@
                 elif dimm:
                     self._z = None
                     self._m = coordinates[2]
                 else:
                     self._z = coordinates[2]
                     self._m = None
             else:  # use both the 3rd and 4th coordinates, ensure not None
-                    self._z = coordinates[2]
-                    self._m = coordinates[3]
+                self._z = coordinates[2]
+                self._m = coordinates[3]
 
             self._dimz = self._z is not None
             self._dimm = self._m is not None
 
     @property
     def x(self):
         """
@@ -547,15 +566,15 @@
         :rtype: bool
         """
         return self._dimz
 
     @dimz.setter
     def dimz(self, value):
         if self._dimz == value:
-            return None
+            return
         self._check_cache()
         if value and self._z is None:
             self._z = 0
         elif value is None:
             self._z = None
         self._dimz = value
 
@@ -569,27 +588,41 @@
         :rtype: bool
         """
         return self._dimm
 
     @dimm.setter
     def dimm(self, value):
         if self._dimm == value:
-            return None
+            return
         self._check_cache()
         if value and self._m is None:
             self._m = 0
         elif value is None:
             self._m = None
         self._dimm = value
 
-    def _to_geojson_coordinates(self, dimz):
-        coordinates = [self.x, self.y]
-        if dimz:
-            coordinates.append(self.z)
-        return coordinates
+    def _coordinates(self, dimz=True, dimm=True, tpl=True):
+        dimz = dimz & self.dimz
+        dimm = dimm & self.dimm
+
+        if dimz and dimm:
+            coordinates = (self.x, self.y, self.z, self.m)
+        elif dimz:
+            coordinates = (self.x, self.y, self.z)
+        elif dimm:
+            coordinates = (self.x, self.y, self.m)
+        else:
+            coordinates = (self.x, self.y)
+
+        if tpl:
+            return coordinates
+        return list(coordinates)
+
+    def _to_geojson_coordinates(self):
+        return self._coordinates(dimm=False, tpl=False)
 
     def _bounds(self):
         return (self.x, self.y, self.x, self.y)
 
     def _load_geometry(self):
         self._x, self._y, self._z, self._m = Point._read_wkb(self._reader, self._dimz, self._dimm)
 
@@ -606,16 +639,16 @@
                 m = None
             elif dimm:
                 z = None
                 m = reader.get_double()
             else:
                 z = None
                 m = None
-        except TypeError:
-            raise WkbError()
+        except TypeError as e:
+            raise WkbError() from e
         return x, y, z, m
 
     def _write_wkb(self, writer, dimz, dimm):
         writer.add_double(self.x)
         writer.add_double(self.y)
         if dimz and dimm:
             writer.add_double(self.z)
@@ -695,17 +728,19 @@
     def dimm(self, value):
         if self.dimm == value:
             return
         for vertex in self.vertices:
             vertex.dimm = value
         self._dimm = value
 
-    def _to_geojson_coordinates(self, dimz):
-        coordinates = [v._to_geojson_coordinates(dimz=dimz) for v in self.vertices]
-        return coordinates
+    def _coordinates(self, dimz=True, dimm=True, tpl=True):
+        return [v._coordinates(dimz, dimm, tpl) for v in self.vertices]
+
+    def _to_geojson_coordinates(self):
+        return self._coordinates(dimz=False, tpl=False)
 
     def _bounds(self):
         x = [v.x for v in self.vertices]
         y = [v.y for v in self.vertices]
         return (min(x), min(y), max(x), max(y))
 
     @staticmethod
@@ -719,16 +754,16 @@
     @staticmethod
     def _read_wkb(reader, dimz, dimm):
         vertices = []
         try:
             for _ in range(reader.get_int()):
                 coordinates = Point._read_wkb(reader, dimz, dimm)
                 vertices.append(coordinates)
-        except TypeError:
-            raise WkbError()
+        except TypeError as e:
+            raise WkbError() from e
         return vertices
 
     def _write_wkb(self, writer, dimz, dimm):
         writer.add_int(len(self.vertices))
         for vertex in self.vertices:
             vertex._write_wkb(writer, dimz, dimm)
 
@@ -819,17 +854,19 @@
     def dimm(self, value):
         if self._dimm == value:
             return
         for ring in self.rings:
             ring.dimm = value
         self._dimm = value
 
-    def _to_geojson_coordinates(self, dimz):
-        coordinates = [r._to_geojson_coordinates(dimz=dimz) for r in self.rings]
-        return coordinates
+    def _coordinates(self, dimz=True, dimm=True, tpl=True):
+        return [r._coordinates(dimz, dimm, tpl) for r in self.rings]
+
+    def _to_geojson_coordinates(self):
+        return self._coordinates(dimz=False, tpl=False)
 
     def _bounds(self):
         return self.exterior.bounds
 
     @staticmethod
     def _from_coordinates(rings, dimz, dimm):
         return [LineString(vertices, dimz, dimm) for vertices in rings]
@@ -841,16 +878,16 @@
     @staticmethod
     def _read_wkb(reader, dimz, dimm):
         rings = []
         try:
             for _ in range(reader.get_int()):
                 vertices = LineString._read_wkb(reader, dimz, dimm)
                 rings.append(vertices)
-        except TypeError:
-            raise WkbError()
+        except TypeError as e:
+            raise WkbError() from e
         return rings
 
     def _write_wkb(self, writer, dimz, dimm):
         writer.add_int(len(self.rings))
         for ring in self.rings:
             ring._write_wkb(writer, dimz, dimm)
 
@@ -966,16 +1003,16 @@
     _LWGEOMTYPE = 6
     __slots__ = ["__polygons__"]
 
     def __init__(self, polygons=None, srid=None):
         if self._wkb:
             self._polygons = None
         else:
-            self._srid = srid
             self._polygons = polygons
+            self._srid = srid
             self._set_multi_metadata()
 
     @property
     def polygons(self):
         """
         List of all component polygons.
         """
@@ -1008,15 +1045,15 @@
     The SRID and dimensionality of all geometries in the collection must be
     identical.
     """
 
     _LWGEOMTYPE = 7
     __slots__ = ["_geometries"]
 
-    def __init__(self, geometries=None, srid=None, dimz=False, dimm=False):
+    def __init__(self, geometries=None, srid=None):
         if self._wkb:
             self._geometries = None
         else:
             self._geometries = geometries
             self._srid = srid
             self._set_multi_metadata()
 
@@ -1024,14 +1061,14 @@
     def geometries(self):
         """
         List of all component geometries.
         """
         self._check_cache()
         return self._geometries
 
-    def _to_geojson(self, dimz):
-        geometries = [g._to_geojson(dimz=dimz) for g in self.geometries]
+    def _to_geojson(self):
+        geometries = [g._to_geojson() for g in self.geometries]
         geojson = {
                 "type": self.__class__.__name__,
                 "geometries": geometries
         }
         return geojson
```

### Comparing `plpygis-0.3.0/plpygis.egg-info/PKG-INFO` & `plpygis-0.4.0/plpygis.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 Metadata-Version: 2.1
 Name: plpygis
-Version: 0.3.0
-Summary: PostGIS Python tools
-Home-page: https://github.com/bosth/plpygis
-Author: Benjamin Trigona-Harany
-Author-email: plpygis@jaxartes.net
+Version: 0.4.0
+Summary: Python tools for PostGIS
+Author-email: Benjamin Trigona-Harany <plpygis@jaxartes.net>
 License: GPL-3.0-only
-Keywords: gis geospatial postgis postgresql plpython
-Platform: any
+Project-URL: Homepage, https://github.com/bosth/plpygis
+Project-URL: Issues, https://github.com/bosth/plpygis/issues
+Project-URL: Documentation, https://plpygis.readthedocs.io/
+Keywords: gis,geospatial,postgis,postgresql,pl/python
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: GIS
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pyshp; extra == "test"
+Requires-Dist: Shapely>=2.0.2; extra == "test"
 Provides-Extra: shapely-support
 Requires-Dist: Shapely>=2.0.2; extra == "shapely-support"
 
-=======
-plpygis
-=======
-
-``plpygis`` is a Python tool that can convert a `PostGIS <https://postgis.net/>`_ ``geometry`` into an equivalent WKB, EWKB, GeoJSON or Shapely geometry. ``plpygis`` is intended for use in PostgreSQL `PL/Python <https://www.postgresql.org/docs/current/plpython.html>`_ functions.
-
-Basic usage
-===========
-
-The ``Geometry`` class and its subclasses can be used to convert to and from PostGIS geometries. The following example will take a PostGIS multipolygon geometry named ``geom`` and find its largest component polygon.
-
-``Geometry()`` can convert a PostGIS ``geometry`` that has been passed as a parameter to a PL/Python function. A ``Geometry`` that is returned from the PL/Python function will automatically be converted back to a PostGIS ``geometry``.
-
-.. code-block:: postgres
- 
-    CREATE OR REPLACE FUNCTION largest_poly(geom geometry)
-      RETURNS geometry 
-    AS $$
-      from plpygis import Geometry
-      polygons = Geometry(geom)
-      if polygons.type == "Polygon":
-          return polygons
-      elif polygons.type == "MultiPolygon":
-          largest = max(polygons.shapely, key=lambda polygon: polygon.area)
-          return Geometry.from_shapely(largest)
-      else:
-          return None
-    $$ LANGUAGE plpython3u;
+# plpygis
+
+`plpygis` is a Python tool that can convert a [PostGIS](https://postgis.net/) `geometry` into an equivalent WKB, EWKB, GeoJSON or Shapely geometry. `plpygis` is intended for use in PostgreSQL [PL/Python](https://www.postgresql.org/docs/current/plpython.html) functions.
+
+## Basic usage
+
+The `Geometry` class and its subclasses can be used to convert to and from PostGIS geometries. The following example will take a PostGIS multipolygon geometry named `geom` and find its largest component polygon.
+
+`Geometry()` can convert a PostGIS `geometry` that has been passed as a parameter to a PL/Python function. A `Geometry` that is returned from the PL/Python function will automatically be converted back to a PostGIS `geometry`.
+
+``` postgres
+CREATE OR REPLACE FUNCTION largest_poly(geom geometry)
+  RETURNS geometry 
+AS $$
+  from plpygis import Geometry
+  polygons = Geometry(geom)
+  if polygons.type == "Polygon":
+      return polygons
+  elif polygons.type == "MultiPolygon":
+      largest = max(polygons.shapely, key=lambda polygon: polygon.area)
+      return Geometry.from_shapely(largest)
+  else:
+      return None
+$$ LANGUAGE plpython3u;
+```
 
 This can then be called as part of an SQL query:
 
-.. code-block:: postgres
+``` postgres
+SELECT largest_poly(geom) FROM countries;
+```
 
-    SELECT largest_poly(geom) FROM countries;
+## Documentation
 
-Documentation
-=============
+Full `plpygis` documentation is available at <http://plpygis.readthedocs.io/>.
 
-Full ``plpygis`` documentation is available at http://plpygis.readthedocs.io/.
+[![Continuous Integration](https://github.com/bosth/plpygis/workflows/tests/badge.svg)](https://github.com/bosth/plpygis/actions?query=workflow%3A%22tests%22) [![Documentation Status](https://readthedocs.org/projects/plpygis/badge/?version=latest)](http://plpygis.readthedocs.io/en/latest/?badge=latest)
 
-.. image:: https://readthedocs.org/projects/plpygis/badge/?version=latest
-    :target: http://plpygis.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-    
-.. image:: https://github.com/bosth/plpygis/workflows/tests/badge.svg
-    :target: https://github.com/bosth/plpygis/actions?query=workflow%3A%22tests%22
-    :alt: Continuous Integration
```

