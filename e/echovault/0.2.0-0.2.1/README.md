# Comparing `tmp/echovault-0.2.0.tar.gz` & `tmp/echovault-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echovault-0.2.0.tar", max compression
+gzip compressed data, was "echovault-0.2.1.tar", max compression
```

## Comparing `echovault-0.2.0.tar` & `echovault-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.0/echovault/__init__.py
--rw-r--r--   0        0        0      472 2024-04-11 19:33:04.149986 echovault-0.2.0/echovault/db.py
--rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.0/echovault/db.py~
--rw-r--r--   0        0        0     3884 2024-04-19 19:14:39.971313 echovault-0.2.0/echovault/table.py
--rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.0/echovault/table.py~
--rw-r--r--   0        0        0     3446 2024-04-19 19:10:36.808660 echovault-0.2.0/echovault/vault.py
--rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.0/echovault/vault.py~
--rw-r--r--   0        0        0      380 2024-04-19 19:06:05.399416 echovault-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.1/echovault/__init__.py
+-rw-r--r--   0        0        0      472 2024-04-11 19:33:04.149986 echovault-0.2.1/echovault/db.py
+-rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.1/echovault/db.py~
+-rw-r--r--   0        0        0     3884 2024-04-19 19:14:39.971313 echovault-0.2.1/echovault/table.py
+-rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.1/echovault/table.py~
+-rw-r--r--   0        0        0     3519 2024-04-20 19:07:08.353727 echovault-0.2.1/echovault/vault.py
+-rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.1/echovault/vault.py~
+-rw-r--r--   0        0        0      380 2024-04-21 19:41:43.512483 echovault-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.1/PKG-INFO
```

### Comparing `echovault-0.2.0/README.md` & `echovault-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `echovault-0.2.0/echovault/table.py` & `echovault-0.2.1/echovault/table.py`

 * *Files identical despite different names*

### Comparing `echovault-0.2.0/echovault/table.py~` & `echovault-0.2.1/echovault/table.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.0/echovault/vault.py` & `echovault-0.2.1/echovault/vault.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,27 @@
 class Vault:
     @staticmethod
     def encode(string):
         return string.encode('utf-8')
 
     @staticmethod
     def decode(value):
-        return b64decode(value).decode('utf-8')
+        return value.decode('utf-8')
     
     def __init__(self, object_store, refs, *, tree:Tree=None, ref=None):
         self.object_store = object_store
         self.refs = refs
-        self.ref = ref
 
         if ref is not None:
-            if ('refs/heads/' + ref) in self.refs and tree is None:
-                tree = self.object_store[self.refs['refs/heads/' + ref]]
+            ref = b'refs/heads/' + ref.encode('utf-8')
+            
+            if ref in self.refs and tree is None:
+                tree = self.object_store[self.object_store[self.refs[ref]].tree]
+        
+        self.ref = ref
         
         if tree is None:
             self._tree = Tree()
         else:
             self._tree = tree
 
     def _update(self):
@@ -65,16 +68,17 @@
                author:Optional[str]=None,
                committer:Optional[str]=None,
                time_:Optional[int]=None,
                timezone:Optional[int]=None,
                ):
         if ref is None:
             ref = self.ref
+        else:
+            ref = b'refs/heads/' + ref.encode('utf-8')
             
-        ref = ('refs/heads/' + ref).encode('utf-8')
         commit = Commit()
         
         commit.message = message.encode('utf-8')
         commit.tree = self._tree
 
         if committer is None:
             committer = ('_'.join((getfqdn(), gethostname(),
```

### Comparing `echovault-0.2.0/echovault/vault.py~` & `echovault-0.2.1/echovault/vault.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.0/PKG-INFO` & `echovault-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echovault
-Version: 0.2.0
+Version: 0.2.1
 Summary: echovault is git data storage
 Author: Charles Bajeux
 Author-email: charles.bajeux@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

