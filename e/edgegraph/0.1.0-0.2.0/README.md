# Comparing `tmp/edgegraph-0.1.0.tar.gz` & `tmp/edgegraph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegraph-0.1.0.tar", last modified: Sat Feb  3 18:59:06 2024, max compression
+gzip compressed data, was "edgegraph-0.2.0.tar", last modified: Mon Apr 22 02:31:57 2024, max compression
```

## Comparing `edgegraph-0.1.0.tar` & `edgegraph-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,40 @@
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-02-03 18:59:06.177860 edgegraph-0.1.0/
--rw-r--r--   0 misha     (1000) misha     (1000)     7653 2024-02-03 17:29:08.000000 edgegraph-0.1.0/LICENSE.txt
--rw-r--r--   0 misha     (1000) misha     (1000)    11342 2024-02-03 18:59:06.177860 edgegraph-0.1.0/PKG-INFO
--rw-r--r--   0 misha     (1000) misha     (1000)     1974 2024-01-30 01:55:27.000000 edgegraph-0.1.0/README.md
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-02-03 18:59:06.173860 edgegraph-0.1.0/edgegraph/
--rw-r--r--   0 misha     (1000) misha     (1000)       80 2023-11-23 23:59:00.000000 edgegraph-0.1.0/edgegraph/__init__.py
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-02-03 18:59:06.173860 edgegraph-0.1.0/edgegraph/builder/
--rw-r--r--   0 misha     (1000) misha     (1000)       98 2024-01-13 17:42:47.000000 edgegraph-0.1.0/edgegraph/builder/__init__.py
--rw-r--r--   0 misha     (1000) misha     (1000)     2475 2024-02-03 18:09:31.000000 edgegraph-0.1.0/edgegraph/builder/adjlist.py
--rw-r--r--   0 misha     (1000) misha     (1000)     4631 2024-02-03 18:10:08.000000 edgegraph-0.1.0/edgegraph/builder/adjmatrix.py
--rw-r--r--   0 misha     (1000) misha     (1000)     2854 2024-02-03 18:09:45.000000 edgegraph-0.1.0/edgegraph/builder/explicit.py
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-02-03 18:59:06.177860 edgegraph-0.1.0/edgegraph/structure/
--rw-r--r--   0 misha     (1000) misha     (1000)      321 2024-01-06 22:51:15.000000 edgegraph-0.1.0/edgegraph/structure/__init__.py
--rw-r--r--   0 misha     (1000) misha     (1000)     7022 2024-01-21 18:34:41.000000 edgegraph-0.1.0/edgegraph/structure/base.py
--rw-r--r--   0 misha     (1000) misha     (1000)     2458 2024-01-07 18:11:08.000000 edgegraph-0.1.0/edgegraph/structure/directededge.py
--rw-r--r--   0 misha     (1000) misha     (1000)     4010 2024-01-04 22:18:37.000000 edgegraph-0.1.0/edgegraph/structure/link.py
--rw-r--r--   0 misha     (1000) misha     (1000)     4082 2024-01-06 23:41:34.000000 edgegraph-0.1.0/edgegraph/structure/twoendedlink.py
--rw-r--r--   0 misha     (1000) misha     (1000)      955 2024-01-07 18:11:08.000000 edgegraph-0.1.0/edgegraph/structure/undirectededge.py
--rw-r--r--   0 misha     (1000) misha     (1000)     8462 2024-01-13 22:25:13.000000 edgegraph-0.1.0/edgegraph/structure/universe.py
--rw-r--r--   0 misha     (1000) misha     (1000)     3974 2024-01-04 22:18:37.000000 edgegraph-0.1.0/edgegraph/structure/vertex.py
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-02-03 18:59:06.177860 edgegraph-0.1.0/edgegraph/traversal/
--rw-r--r--   0 misha     (1000) misha     (1000)       86 2024-01-15 02:49:14.000000 edgegraph-0.1.0/edgegraph/traversal/__init__.py
--rw-r--r--   0 misha     (1000) misha     (1000)     3054 2024-02-03 18:07:34.000000 edgegraph-0.1.0/edgegraph/traversal/breadthfirst.py
--rw-r--r--   0 misha     (1000) misha     (1000)     3993 2024-02-03 18:14:35.000000 edgegraph-0.1.0/edgegraph/traversal/helpers.py
--rw-r--r--   0 misha     (1000) misha     (1000)      470 2024-02-03 17:42:52.000000 edgegraph-0.1.0/edgegraph/version.py
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-02-03 18:59:06.177860 edgegraph-0.1.0/edgegraph.egg-info/
--rw-r--r--   0 misha     (1000) misha     (1000)    11342 2024-02-03 18:59:06.000000 edgegraph-0.1.0/edgegraph.egg-info/PKG-INFO
--rw-r--r--   0 misha     (1000) misha     (1000)      712 2024-02-03 18:59:06.000000 edgegraph-0.1.0/edgegraph.egg-info/SOURCES.txt
--rw-r--r--   0 misha     (1000) misha     (1000)        1 2024-02-03 18:59:06.000000 edgegraph-0.1.0/edgegraph.egg-info/dependency_links.txt
--rw-r--r--   0 misha     (1000) misha     (1000)       10 2024-02-03 18:59:06.000000 edgegraph-0.1.0/edgegraph.egg-info/top_level.txt
--rw-r--r--   0 misha     (1000) misha     (1000)     1471 2024-02-03 17:53:21.000000 edgegraph-0.1.0/pyproject.toml
--rw-r--r--   0 misha     (1000) misha     (1000)       38 2024-02-03 18:59:06.177860 edgegraph-0.1.0/setup.cfg
-drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-02-03 18:59:06.177860 edgegraph-0.1.0/tests/
--rw-r--r--   0 misha     (1000) misha     (1000)     1030 2024-02-03 17:45:46.000000 edgegraph-0.1.0/tests/test_version.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.891065 edgegraph-0.2.0/
+-rw-r--r--   0 misha     (1000) misha     (1000)     7653 2024-02-03 17:29:08.000000 edgegraph-0.2.0/LICENSE.txt
+-rw-r--r--   0 misha     (1000) misha     (1000)    11342 2024-04-22 02:31:57.891065 edgegraph-0.2.0/PKG-INFO
+-rw-r--r--   0 misha     (1000) misha     (1000)     1974 2024-04-22 02:31:28.000000 edgegraph-0.2.0/README.md
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph/
+-rw-r--r--   0 misha     (1000) misha     (1000)       80 2023-11-23 23:59:00.000000 edgegraph-0.2.0/edgegraph/__init__.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph/builder/
+-rw-r--r--   0 misha     (1000) misha     (1000)       98 2024-01-13 17:42:47.000000 edgegraph-0.2.0/edgegraph/builder/__init__.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     2511 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/builder/adjlist.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     4667 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/builder/adjmatrix.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     2890 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/builder/explicit.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     1698 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/builder/randgraph.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph/output/
+-rw-r--r--   0 misha     (1000) misha     (1000)      119 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/output/__init__.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     3006 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/output/plaintext.py
+-rw-r--r--   0 misha     (1000) misha     (1000)    13381 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/output/plantuml.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph/structure/
+-rw-r--r--   0 misha     (1000) misha     (1000)      321 2024-01-06 22:51:15.000000 edgegraph-0.2.0/edgegraph/structure/__init__.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     7022 2024-01-21 18:34:41.000000 edgegraph-0.2.0/edgegraph/structure/base.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     2458 2024-01-07 18:11:08.000000 edgegraph-0.2.0/edgegraph/structure/directededge.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     4010 2024-01-04 22:18:37.000000 edgegraph-0.2.0/edgegraph/structure/link.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     4082 2024-01-06 23:41:34.000000 edgegraph-0.2.0/edgegraph/structure/twoendedlink.py
+-rw-r--r--   0 misha     (1000) misha     (1000)      955 2024-01-07 18:11:08.000000 edgegraph-0.2.0/edgegraph/structure/undirectededge.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     8462 2024-01-13 22:25:13.000000 edgegraph-0.2.0/edgegraph/structure/universe.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     3974 2024-01-04 22:18:37.000000 edgegraph-0.2.0/edgegraph/structure/vertex.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph/traversal/
+-rw-r--r--   0 misha     (1000) misha     (1000)       86 2024-01-15 02:49:14.000000 edgegraph-0.2.0/edgegraph/traversal/__init__.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     3207 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/traversal/breadthfirst.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     9283 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/traversal/depthfirst.py
+-rw-r--r--   0 misha     (1000) misha     (1000)     3993 2024-02-08 03:50:53.000000 edgegraph-0.2.0/edgegraph/traversal/helpers.py
+-rw-r--r--   0 misha     (1000) misha     (1000)      470 2024-04-22 02:31:28.000000 edgegraph-0.2.0/edgegraph/version.py
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/edgegraph.egg-info/
+-rw-r--r--   0 misha     (1000) misha     (1000)    11342 2024-04-22 02:31:57.000000 edgegraph-0.2.0/edgegraph.egg-info/PKG-INFO
+-rw-r--r--   0 misha     (1000) misha     (1000)      865 2024-04-22 02:31:57.000000 edgegraph-0.2.0/edgegraph.egg-info/SOURCES.txt
+-rw-r--r--   0 misha     (1000) misha     (1000)        1 2024-04-22 02:31:57.000000 edgegraph-0.2.0/edgegraph.egg-info/dependency_links.txt
+-rw-r--r--   0 misha     (1000) misha     (1000)       10 2024-04-22 02:31:57.000000 edgegraph-0.2.0/edgegraph.egg-info/top_level.txt
+-rw-r--r--   0 misha     (1000) misha     (1000)     1471 2024-02-03 17:53:21.000000 edgegraph-0.2.0/pyproject.toml
+-rw-r--r--   0 misha     (1000) misha     (1000)       38 2024-04-22 02:31:57.891065 edgegraph-0.2.0/setup.cfg
+drwxr-xr-x   0 misha     (1000) misha     (1000)        0 2024-04-22 02:31:57.887065 edgegraph-0.2.0/tests/
+-rw-r--r--   0 misha     (1000) misha     (1000)     1030 2024-02-03 17:45:46.000000 edgegraph-0.2.0/tests/test_version.py
```

### Comparing `edgegraph-0.1.0/LICENSE.txt` & `edgegraph-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgegraph-0.1.0/PKG-INFO` & `edgegraph-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegraph
-Version: 0.1.0
+Version: 0.2.0
 Summary: Object oriented edge-vertex graph library.
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -202,20 +202,20 @@
 * [x] Vertex-edge graphs
 * [x] "Universe" class to contain graphs as a single unit
 * [x] Class-based edges, can associate arbitrary data with edges
 * [x] Automatic edge update propagation to necessary endpoints
 * [x] Adjacency list / matrix build-a-graph
 * [ ] Build-an-adjlist / build-an-adjmat from graphs
 * [x] Breadth-first search and traversal
-* [ ] Depth-first search and traversal
+* [x] Depth-first search and traversal
 * [ ] Topological sorting
 * [ ] Strongly connected component detection
 * [ ] Universe island detection
 * [ ] Shortest path detection
-* [ ] Graph drawing generation via PlantUML
+* [x] Graph drawing generation via PlantUML
 * [ ] Formal automata modelling (DFA, NFA, etc)
 * [ ] Operation flow graph modelling (nodes as operations instead of states)
 * [ ] "Functional graphs" -- attach executable code to nodes and run a graph as
       a program
 * [ ] Object serialization, save-to- and load-from-file
 
 These features, as with the API, may be changed or dropped at any time without
```

### Comparing `edgegraph-0.1.0/README.md` & `edgegraph-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 * [x] Vertex-edge graphs
 * [x] "Universe" class to contain graphs as a single unit
 * [x] Class-based edges, can associate arbitrary data with edges
 * [x] Automatic edge update propagation to necessary endpoints
 * [x] Adjacency list / matrix build-a-graph
 * [ ] Build-an-adjlist / build-an-adjmat from graphs
 * [x] Breadth-first search and traversal
-* [ ] Depth-first search and traversal
+* [x] Depth-first search and traversal
 * [ ] Topological sorting
 * [ ] Strongly connected component detection
 * [ ] Universe island detection
 * [ ] Shortest path detection
-* [ ] Graph drawing generation via PlantUML
+* [x] Graph drawing generation via PlantUML
 * [ ] Formal automata modelling (DFA, NFA, etc)
 * [ ] Operation flow graph modelling (nodes as operations instead of states)
 * [ ] "Functional graphs" -- attach executable code to nodes and run a graph as
       a program
 * [ ] Object serialization, save-to- and load-from-file
 
 These features, as with the API, may be changed or dropped at any time without
```

### Comparing `edgegraph-0.1.0/edgegraph/builder/adjlist.py` & `edgegraph-0.2.0/edgegraph/builder/adjlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 adjacency list structure, as is common in graph algorithms and software.
 
 .. seealso::
 
    * https://en.wikipedia.org/wiki/Adjacency_list
 """
 
+from __future__ import annotations
+
 from edgegraph.structure import Universe, UnDirectedEdge
 from edgegraph.builder import explicit
 
 def load_adj_dict(adjdict: dict,
         linktype: type=UnDirectedEdge,
         ) -> Universe:
     """
```

### Comparing `edgegraph-0.1.0/edgegraph/builder/adjmatrix.py` & `edgegraph-0.2.0/edgegraph/builder/adjmatrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 adjacency matrix structure, as is common in graph algorithms and software.
 
 .. seealso::
 
    * https://en.wikipedia.org/wiki/Adjacency_matrix
 """
 
+from __future__ import annotations
+
 from edgegraph.structure import Universe, Vertex, DirectedEdge
 from edgegraph.builder import explicit
 
 def load_adj_matrix(matrix: list[list[bool]],
         vertices: list[Vertex],
         linktype: type=DirectedEdge,
         ) -> Universe:
```

### Comparing `edgegraph-0.1.0/edgegraph/builder/explicit.py` & `edgegraph-0.2.0/edgegraph/builder/explicit.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 Most of the functions in this module are one-liners.  Seriously.  It exists to
 standardize the methods by which links are associated, so that changes to the
 structure classes can occur without breaking everyone's code -- instead, these
 functions will get the necessary updates to match, and the API stays unchanged.
 """
 
+from __future__ import annotations
+
 from edgegraph.structure import Vertex, DirectedEdge, UnDirectedEdge
 
 def link_from_to(v1: Vertex, lnktype: type, v2: Vertex):
     """
     Create a link of type ``lnktype`` from ``v1`` to ``v2``.
 
     This function instantiates a new link type (a subclass of
```

### Comparing `edgegraph-0.1.0/edgegraph/structure/base.py` & `edgegraph-0.2.0/edgegraph/structure/base.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.1.0/edgegraph/structure/directededge.py` & `edgegraph-0.2.0/edgegraph/structure/directededge.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.1.0/edgegraph/structure/link.py` & `edgegraph-0.2.0/edgegraph/structure/link.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.1.0/edgegraph/structure/twoendedlink.py` & `edgegraph-0.2.0/edgegraph/structure/twoendedlink.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.1.0/edgegraph/structure/undirectededge.py` & `edgegraph-0.2.0/edgegraph/structure/undirectededge.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.1.0/edgegraph/structure/universe.py` & `edgegraph-0.2.0/edgegraph/structure/universe.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.1.0/edgegraph/structure/vertex.py` & `edgegraph-0.2.0/edgegraph/structure/vertex.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.1.0/edgegraph/traversal/breadthfirst.py` & `edgegraph-0.2.0/edgegraph/traversal/breadthfirst.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 #!/usr/env/python3
 # -*- coding: utf-8 -*-
 
 """
 Breadth-first search and traversal functions.
+
+.. todo::
+
+   document this module better
+
+.. seealso::
+
+   * :py:mod:`edgegraph.traversal.depthfirst`: depth-first search and traverse
+     operations
 """
 
 from __future__ import annotations
 
 import collections
 
 from edgegraph.structure import Universe, Vertex
```

### Comparing `edgegraph-0.1.0/edgegraph/traversal/helpers.py` & `edgegraph-0.2.0/edgegraph/traversal/helpers.py`

 * *Files identical despite different names*

### Comparing `edgegraph-0.1.0/edgegraph.egg-info/PKG-INFO` & `edgegraph-0.2.0/edgegraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegraph
-Version: 0.1.0
+Version: 0.2.0
 Summary: Object oriented edge-vertex graph library.
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -202,20 +202,20 @@
 * [x] Vertex-edge graphs
 * [x] "Universe" class to contain graphs as a single unit
 * [x] Class-based edges, can associate arbitrary data with edges
 * [x] Automatic edge update propagation to necessary endpoints
 * [x] Adjacency list / matrix build-a-graph
 * [ ] Build-an-adjlist / build-an-adjmat from graphs
 * [x] Breadth-first search and traversal
-* [ ] Depth-first search and traversal
+* [x] Depth-first search and traversal
 * [ ] Topological sorting
 * [ ] Strongly connected component detection
 * [ ] Universe island detection
 * [ ] Shortest path detection
-* [ ] Graph drawing generation via PlantUML
+* [x] Graph drawing generation via PlantUML
 * [ ] Formal automata modelling (DFA, NFA, etc)
 * [ ] Operation flow graph modelling (nodes as operations instead of states)
 * [ ] "Functional graphs" -- attach executable code to nodes and run a graph as
       a program
 * [ ] Object serialization, save-to- and load-from-file
 
 These features, as with the API, may be changed or dropped at any time without
```

### Comparing `edgegraph-0.1.0/edgegraph.egg-info/SOURCES.txt` & `edgegraph-0.2.0/edgegraph.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,19 +7,24 @@
 edgegraph.egg-info/SOURCES.txt
 edgegraph.egg-info/dependency_links.txt
 edgegraph.egg-info/top_level.txt
 edgegraph/builder/__init__.py
 edgegraph/builder/adjlist.py
 edgegraph/builder/adjmatrix.py
 edgegraph/builder/explicit.py
+edgegraph/builder/randgraph.py
+edgegraph/output/__init__.py
+edgegraph/output/plaintext.py
+edgegraph/output/plantuml.py
 edgegraph/structure/__init__.py
 edgegraph/structure/base.py
 edgegraph/structure/directededge.py
 edgegraph/structure/link.py
 edgegraph/structure/twoendedlink.py
 edgegraph/structure/undirectededge.py
 edgegraph/structure/universe.py
 edgegraph/structure/vertex.py
 edgegraph/traversal/__init__.py
 edgegraph/traversal/breadthfirst.py
+edgegraph/traversal/depthfirst.py
 edgegraph/traversal/helpers.py
 tests/test_version.py
```

### Comparing `edgegraph-0.1.0/pyproject.toml` & `edgegraph-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edgegraph-0.1.0/tests/test_version.py` & `edgegraph-0.2.0/tests/test_version.py`

 * *Files identical despite different names*

