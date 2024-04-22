# Comparing `tmp/node_graph-0.0.4.tar.gz` & `tmp/node_graph-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "node_graph-0.0.4.tar", last modified: Mon Apr 15 12:08:01 2024, max compression
+gzip compressed data, was "node_graph-0.0.5.tar", last modified: Mon Apr 22 08:58:37 2024, max compression
```

## Comparing `node_graph-0.0.4.tar` & `node_graph-0.0.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2023-12-03 08:36:19.000000 node_graph-0.0.4/LICENSE
--rw-r--r--   0 xing      (1000) xing      (1000)     1268 2024-04-15 12:08:01.495976 node_graph-0.0.4/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      827 2023-12-03 08:36:19.000000 node_graph-0.0.4/README.md
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.491976 node_graph-0.0.4/node_graph/
--rw-rw-r--   0 xing      (1000) xing      (1000)       34 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    13105 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/analysis.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11972 2024-04-15 12:06:25.000000 node_graph-0.0.4/node_graph/collection.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    10311 2024-04-15 12:06:25.000000 node_graph-0.0.4/node_graph/decorator.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3473 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/link.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    18230 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11430 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/node_graph.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/node_graph/nodes/
--rw-rw-r--   0 xing      (1000) xing      (1000)       85 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/nodes/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4600 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/nodes/test_nodes.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/node_graph/properties/
--rw-rw-r--   0 xing      (1000) xing      (1000)       93 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/properties/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11956 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/properties/builtin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3032 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1541 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/serializer.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4066 2024-04-15 12:06:25.000000 node_graph-0.0.4/node_graph/socket.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/node_graph/sockets/
--rw-rw-r--   0 xing      (1000) xing      (1000)       89 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/sockets/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3332 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/sockets/builtin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2550 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/utils.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      103 2023-12-03 08:36:19.000000 node_graph-0.0.4/node_graph/version.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/node_graph.egg-info/
--rw-r--r--   0 xing      (1000) xing      (1000)     1268 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      889 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      212 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/entry_points.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       50 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       11 2024-04-15 12:08:01.000000 node_graph-0.0.4/node_graph.egg-info/top_level.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-04-15 12:08:01.495976 node_graph-0.0.4/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     1361 2024-04-15 12:07:57.000000 node_graph-0.0.4/setup.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-15 12:08:01.495976 node_graph-0.0.4/tests/
--rw-rw-r--   0 xing      (1000) xing      (1000)      597 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_collection.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2231 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_decorator.py
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_entry_point.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      632 2024-04-15 12:06:25.000000 node_graph-0.0.4/tests/test_hooks.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1731 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      616 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2506 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2152 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_socket.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      378 2023-12-03 08:36:19.000000 node_graph-0.0.4/tests/test_yaml.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 08:58:37.807189 node_graph-0.0.5/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2023-12-03 08:36:19.000000 node_graph-0.0.5/LICENSE
+-rw-r--r--   0 xing      (1000) xing      (1000)     1268 2024-04-22 08:58:37.803189 node_graph-0.0.5/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)      827 2023-12-03 08:36:19.000000 node_graph-0.0.5/README.md
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 08:58:37.803189 node_graph-0.0.5/node_graph/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       34 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    13105 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/analysis.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    13072 2024-04-22 08:55:14.000000 node_graph-0.0.5/node_graph/collection.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    10441 2024-04-20 12:12:39.000000 node_graph-0.0.5/node_graph/decorator.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3473 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/link.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    18403 2024-04-22 08:55:14.000000 node_graph-0.0.5/node_graph/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11430 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/node_graph.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 08:58:37.803189 node_graph-0.0.5/node_graph/nodes/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       85 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/nodes/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4600 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/nodes/test_nodes.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 08:58:37.803189 node_graph-0.0.5/node_graph/properties/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       93 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/properties/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11956 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/properties/builtin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3331 2024-04-22 08:55:14.000000 node_graph-0.0.5/node_graph/property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1541 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/serializer.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4066 2024-04-15 12:06:25.000000 node_graph-0.0.5/node_graph/socket.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 08:58:37.803189 node_graph-0.0.5/node_graph/sockets/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       89 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/sockets/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3332 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/sockets/builtin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2550 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/utils.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      103 2023-12-03 08:36:19.000000 node_graph-0.0.5/node_graph/version.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 08:58:37.803189 node_graph-0.0.5/node_graph.egg-info/
+-rw-r--r--   0 xing      (1000) xing      (1000)     1268 2024-04-22 08:58:37.000000 node_graph-0.0.5/node_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)      889 2024-04-22 08:58:37.000000 node_graph-0.0.5/node_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-04-22 08:58:37.000000 node_graph-0.0.5/node_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      212 2024-04-22 08:58:37.000000 node_graph-0.0.5/node_graph.egg-info/entry_points.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       50 2024-04-22 08:58:37.000000 node_graph-0.0.5/node_graph.egg-info/requires.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       11 2024-04-22 08:58:37.000000 node_graph-0.0.5/node_graph.egg-info/top_level.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-04-22 08:58:37.807189 node_graph-0.0.5/setup.cfg
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1361 2024-04-22 08:57:29.000000 node_graph-0.0.5/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-22 08:58:37.803189 node_graph-0.0.5/tests/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      597 2023-12-03 08:36:19.000000 node_graph-0.0.5/tests/test_collection.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2231 2023-12-03 08:36:19.000000 node_graph-0.0.5/tests/test_decorator.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-12-03 08:36:19.000000 node_graph-0.0.5/tests/test_entry_point.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      632 2024-04-15 12:06:25.000000 node_graph-0.0.5/tests/test_hooks.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1731 2023-12-03 08:36:19.000000 node_graph-0.0.5/tests/test_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      616 2023-12-03 08:36:19.000000 node_graph-0.0.5/tests/test_nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2506 2023-12-03 08:36:19.000000 node_graph-0.0.5/tests/test_property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2152 2023-12-03 08:36:19.000000 node_graph-0.0.5/tests/test_socket.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      378 2023-12-03 08:36:19.000000 node_graph-0.0.5/tests/test_yaml.py
```

### Comparing `node_graph-0.0.4/LICENSE` & `node_graph-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/PKG-INFO` & `node_graph-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node_graph
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create node-based workflow
 Home-page: https://github.com/scinode/node-graph
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `node_graph-0.0.4/README.md` & `node_graph-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/node_graph/analysis.py` & `node_graph-0.0.5/node_graph/analysis.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/node_graph/collection.py` & `node_graph-0.0.5/node_graph/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,22 @@
     Attributes:
         path (str): path to import the module.
     """
 
     path: str = ""
     parent_name: str = "parent"
 
-    def __init__(self, parent=None, pool=None, entry_point=None,
-                 post_creation_hooks=None,
-                 post_deletion_hooks=None) -> None:
+    def __init__(
+        self,
+        parent=None,
+        pool=None,
+        entry_point=None,
+        post_creation_hooks=None,
+        post_deletion_hooks=None,
+    ) -> None:
         """Init a collection instance
 
         Args:
             parent (unknow): object this collection belongs to.
         """
         self._items = []
         self.parent = parent
@@ -153,15 +158,15 @@
         coll._items = [item.copy() for item in self._items]
         return coll
 
     def execute_post_creation_hooks(self, item):
         """Execute all functions in post_creation_hooks with the given item."""
         for func in self.post_creation_hooks:
             func(self, item)
-    
+
     def execute_post_deletion_hooks(self, item):
         """Execute all functions in post_deletion_hooks with the given item."""
         for func in self.post_deletion_hooks:
             func(self, item)
 
 
 def decorator_check_identifier_name(func):
@@ -199,16 +204,27 @@
 
 
 class NodeCollection(Collection):
     """Node colleciton"""
 
     parent_name = "node_graph"
 
-    def __init__(self, parent=None, pool=None, entry_point="node_graph.node", post_creation_hooks=None) -> None:
-        super().__init__(parent, pool=pool, entry_point=entry_point, post_creation_hooks=post_creation_hooks)
+    def __init__(
+        self,
+        parent=None,
+        pool=None,
+        entry_point="node_graph.node",
+        post_creation_hooks=None,
+    ) -> None:
+        super().__init__(
+            parent,
+            pool=pool,
+            entry_point=entry_point,
+            post_creation_hooks=post_creation_hooks,
+        )
 
     @decorator_check_identifier_name
     def new(self, identifier, name=None, uuid=None, **kwargs):
         from node_graph.node import Node
 
         inner_id = self.get_inner_id()
         if isinstance(identifier, str):
@@ -250,16 +266,24 @@
     def __init__(
         self, parent=None, pool=None, entry_point="node_graph.property"
     ) -> None:
         super().__init__(parent, pool=pool, entry_point=entry_point)
 
     @decorator_check_identifier_name
     def new(self, identifier, name=None, **kwargs):
+        from node_graph.property import NodeProperty
 
-        ItemClass = self.pool[identifier]
+        if isinstance(identifier, str):
+            ItemClass = self.pool[identifier]
+        elif isinstance(identifier, type) and issubclass(identifier, NodeProperty):
+            ItemClass = identifier
+        else:
+            raise Exception(
+                f"Identifier {identifier} is not a property or property name."
+            )
         item = ItemClass(name, **kwargs)
         self.append(item)
         return item
 
     def __repr__(self) -> str:
         s = ""
         node_name = self.parent.name if self.parent else ""
@@ -275,16 +299,22 @@
     parent_name = "node"
 
     def __init__(self, parent=None, pool=None, entry_point="node_graph.socket") -> None:
         super().__init__(parent, pool=pool, entry_point=entry_point)
 
     @decorator_check_identifier_name
     def new(self, identifier, name=None, **kwargs):
+        from node_graph.socket import NodeSocket
 
-        ItemClass = self.pool[identifier]
+        if isinstance(identifier, str):
+            ItemClass = self.pool[identifier]
+        elif isinstance(identifier, type) and issubclass(identifier, NodeSocket):
+            ItemClass = identifier
+        else:
+            raise Exception(f"Identifier {identifier} is not a socket or socket name.")
         inner_id = self.get_inner_id()
         item = ItemClass(name, type="INPUT", index=inner_id, **kwargs)
         self.append(item)
         return item
 
     def copy(self, parent=None, is_ref=False):
         """Copy the input socket collection.
@@ -316,15 +346,22 @@
 
     def __init__(self, parent=None, pool=None, entry_point="node_graph.socket") -> None:
         super().__init__(parent, pool=pool, entry_point=entry_point)
 
     @decorator_check_identifier_name
     def new(self, identifier, name=None):
 
-        ItemClass = self.pool[identifier]
+        from node_graph.socket import NodeSocket
+
+        if isinstance(identifier, str):
+            ItemClass = self.pool[identifier]
+        elif isinstance(identifier, type) and issubclass(identifier, NodeSocket):
+            ItemClass = identifier
+        else:
+            raise Exception(f"Identifier {identifier} is not a socket or socket name.")
         item = ItemClass(name, type="OUTPUT", index=len(self._items))
         self.append(item)
         return item
 
     def copy(self, parent=None, is_ref=False):
         coll = self.__class__(parent=parent)
         coll._items = [item.copy(node=parent, is_ref=is_ref) for item in self._items]
```

### Comparing `node_graph-0.0.4/node_graph/decorator.py` & `node_graph-0.0.5/node_graph/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,27 +96,30 @@
 
     Returns:
         _type_: _description_
     """
     from node_graph.node import Node
 
     Node = ndata.get("node_class", Node)
+    print("Node: ", Node)
 
     class DecoratedNode(Node):
         identifier: str = ndata["identifier"]
         node_type: str = ndata.get("node_type", "NORMAL")
         catalog = ndata.get("catalog", "Others")
 
         def create_properties(self):
             for prop in ndata.get("properties", []):
                 kwargs = prop[2] if len(prop) > 2 else {}
                 self.properties.new(prop[0], prop[1], **kwargs)
 
         def create_sockets(self):
             for input in ndata.get("inputs", []):
+                print("self: ", self)
+                print("inputs: ", self.inputs.__class__.__name__)
                 inp = self.inputs.new(input[0], input[1])
                 setting = input[2] if len(input) > 2 else {}
                 prop = setting.get("property", None)
                 if prop is not None:
                     kwargs = prop[1] if len(prop) > 1 else {}
                     # identifer, name, kwargs
                     inp.add_property(prop[0], input[1], **kwargs)
```

### Comparing `node_graph-0.0.4/node_graph/link.py` & `node_graph-0.0.5/node_graph/link.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/node_graph/node.py` & `node_graph-0.0.5/node_graph/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,22 +65,25 @@
 
     def __init__(
         self,
         inner_id=0,
         name=None,
         uuid=None,
         parent=None,
+        property_collection_class=PropertyCollection,
+        input_collection_class=InputSocketCollection,
+        output_collection_class=OutputSocketCollection,
     ) -> None:
         self.inner_id = inner_id
         self.name = name or "{}{}".format(self.identifier, inner_id)
         self.uuid = uuid or str(uuid1())
         self.parent = parent
-        self.properties = PropertyCollection(self, pool=self.property_pool)
-        self.inputs = InputSocketCollection(self, pool=self.socket_pool)
-        self.outputs = OutputSocketCollection(self, pool=self.socket_pool)
+        self.properties = property_collection_class(self, pool=self.property_pool)
+        self.inputs = input_collection_class(self, pool=self.socket_pool)
+        self.outputs = output_collection_class(self, pool=self.socket_pool)
         self.ctrl_inputs = InputSocketCollection(self, pool=self.socket_pool)
         self.ctrl_outputs = OutputSocketCollection(self, pool=self.socket_pool)
         self.executor = None
         self.state = "CREATED"
         self.action = "NONE"
         self.position = [30 * self.inner_id, 30 * self.inner_id]
         self.description = ""
```

### Comparing `node_graph-0.0.4/node_graph/node_graph.py` & `node_graph-0.0.5/node_graph/node_graph.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/node_graph/nodes/test_nodes.py` & `node_graph-0.0.5/node_graph/nodes/test_nodes.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/node_graph/properties/builtin.py` & `node_graph-0.0.5/node_graph/properties/builtin.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/node_graph/property.py` & `node_graph-0.0.5/node_graph/property.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,16 +77,23 @@
     def new(cls, identifier, name=None, data={}, property_pool=None):
         """Create a property from a identifier.
         When a plugin create a property, it should provide its own property pool.
         Then call super().new(identifier, name, property_pool) to create a property.
         """
         if property_pool is None:
             from node_graph.properties import property_pool
+        if isinstance(identifier, str):
+            ItemClass = property_pool[identifier]
+        elif isinstance(identifier, type) and issubclass(identifier, NodeProperty):
+            ItemClass = identifier
+        else:
+            raise Exception(
+                f"Identifier {identifier} is not a property or property name."
+            )
 
-        ItemClass = property_pool[identifier]
         item = ItemClass(name, **data)
         return item
 
     def __str__(self):
         return '{}(name="{}", value={})'.format(
             self.__class__.__name__, self.name, self._value
         )
```

### Comparing `node_graph-0.0.4/node_graph/serializer.py` & `node_graph-0.0.5/node_graph/serializer.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/node_graph/socket.py` & `node_graph-0.0.5/node_graph/socket.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/node_graph/sockets/builtin.py` & `node_graph-0.0.5/node_graph/sockets/builtin.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/node_graph/utils.py` & `node_graph-0.0.5/node_graph/utils.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/node_graph.egg-info/PKG-INFO` & `node_graph-0.0.5/node_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node_graph
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create node-based workflow
 Home-page: https://github.com/scinode/node-graph
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `node_graph-0.0.4/node_graph.egg-info/SOURCES.txt` & `node_graph-0.0.5/node_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/setup.py` & `node_graph-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="node_graph",
-    version="0.0.4",
+    version="0.0.5",
     description="Create node-based workflow",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/scinode/node-graph",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
```

### Comparing `node_graph-0.0.4/tests/test_collection.py` & `node_graph-0.0.5/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/tests/test_decorator.py` & `node_graph-0.0.5/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/tests/test_hooks.py` & `node_graph-0.0.5/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/tests/test_node.py` & `node_graph-0.0.5/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/tests/test_nodetree.py` & `node_graph-0.0.5/tests/test_nodetree.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/tests/test_property.py` & `node_graph-0.0.5/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `node_graph-0.0.4/tests/test_socket.py` & `node_graph-0.0.5/tests/test_socket.py`

 * *Files identical despite different names*

