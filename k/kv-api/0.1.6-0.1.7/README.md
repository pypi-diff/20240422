# Comparing `tmp/kv_api-0.1.6.tar.gz` & `tmp/kv_api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_api-0.1.6.tar", last modified: Sun Apr 21 07:39:16 2024, max compression
+gzip compressed data, was "kv_api-0.1.7.tar", last modified: Sun Apr 21 18:03:42 2024, max compression
```

## Comparing `kv_api-0.1.6.tar` & `kv_api-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-21 07:39:16.777275 kv_api-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-05 12:42:30.000000 kv_api-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      646 2024-04-21 07:39:14.000000 kv_api-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 07:39:16.777275 kv_api-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/kv/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      122 2024-04-20 17:32:30.000000 kv_api-0.1.6/src/kv/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2491 2024-04-20 17:54:31.000000 kv_api-0.1.6/src/kv/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/kv/api/append/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       79 2024-04-20 17:37:34.000000 kv_api-0.1.6/src/kv/api/append/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      818 2024-04-20 17:34:19.000000 kv_api-0.1.6/src/kv/api/append/append.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      646 2024-04-20 17:38:48.000000 kv_api-0.1.6/src/kv/api/append/simple.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/kv/api/errors/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       81 2024-04-10 05:52:43.000000 kv_api-0.1.6/src/kv/api/errors/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      791 2024-04-20 05:01:50.000000 kv_api-0.1.6/src/kv/api/errors/errors.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1598 2024-04-20 17:32:02.000000 kv_api-0.1.6/src/kv/api/simple.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 07:39:16.777275 kv_api-0.1.6/src/kv_api.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-21 07:39:16.000000 kv_api-0.1.6/src/kv_api.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      399 2024-04-21 07:39:16.000000 kv_api-0.1.6/src/kv_api.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 07:39:16.000000 kv_api-0.1.6/src/kv_api.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       55 2024-04-21 07:39:16.000000 kv_api-0.1.6/src/kv_api.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-21 07:39:16.000000 kv_api-0.1.6/src/kv_api.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:42.819883 kv_api-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-04-21 18:03:42.819883 kv_api-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-05 12:42:30.000000 kv_api-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      596 2024-04-21 18:03:40.000000 kv_api-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 18:03:42.819883 kv_api-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:42.809883 kv_api-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:42.809883 kv_api-0.1.7/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:42.809883 kv_api-0.1.7/src/kv/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      122 2024-04-20 17:32:30.000000 kv_api-0.1.7/src/kv/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2421 2024-04-21 17:38:38.000000 kv_api-0.1.7/src/kv/api/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:42.819883 kv_api-0.1.7/src/kv/api/append/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       79 2024-04-20 17:37:34.000000 kv_api-0.1.7/src/kv/api/append/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      775 2024-04-21 17:38:56.000000 kv_api-0.1.7/src/kv/api/append/append.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      616 2024-04-21 17:39:10.000000 kv_api-0.1.7/src/kv/api/append/simple.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:42.819883 kv_api-0.1.7/src/kv/api/errors/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       81 2024-04-10 05:52:43.000000 kv_api-0.1.7/src/kv/api/errors/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      791 2024-04-20 05:01:50.000000 kv_api-0.1.7/src/kv/api/errors/errors.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1559 2024-04-21 17:46:17.000000 kv_api-0.1.7/src/kv/api/simple.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:03:42.819883 kv_api-0.1.7/src/kv_api.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-04-21 18:03:42.000000 kv_api-0.1.7/src/kv_api.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      399 2024-04-21 18:03:42.000000 kv_api-0.1.7/src/kv_api.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 18:03:42.000000 kv_api-0.1.7/src/kv_api.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-21 18:03:42.000000 kv_api-0.1.7/src/kv_api.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-21 18:03:42.000000 kv_api-0.1.7/src/kv_api.egg-info/top_level.txt
```

### Comparing `kv_api-0.1.6/pyproject.toml` & `kv_api-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-api"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "API spec for an async Key-Value DB"
 dependencies = [
-  "haskellian-either", "haskellian-asyn", "haskellian-asyn-iter"
+  "haskellian"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/python-kv"
 home = "https://github.com/moveread/python-kv/tree/main/kv-api"
```

### Comparing `kv_api-0.1.6/src/kv/api/api.py` & `kv_api-0.1.7/src/kv/api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import TypeVar, Generic, overload, Literal
 from abc import ABC, abstractmethod
-from haskellian.either import Either, Right, Left, IsLeft
-from haskellian.asyn.promises import Promise, lift
-from haskellian.asyn.iter import AsyncIter
+from haskellian import Either, Left, IsLeft, Promise, promise as P, AsyncIter
 from .errors import ExistentItem, InexistentItem, DBError, InvalidData, ReadError
 
 T = TypeVar('T')
 
 class KV(ABC, Generic[T]):
   
   @overload
@@ -37,26 +35,26 @@
   @abstractmethod
   def rollback(self) -> Promise[Either[DBError, None]]: ...
 
   @overload
   def copy(self, key: str, to: 'KV[T]', to_key: str, *, replace: Literal[False]) -> Promise[Either[DBError|InexistentItem|ExistentItem, None]]: ...
   @overload
   def copy(self, key: str, to: 'KV[T]', to_key: str, *, replace: bool = True) -> Promise[Either[DBError|InexistentItem, None]]: ...
-  @lift
+  @P.lift
   async def copy(self, key: str, to: 'KV[T]', to_key: str, *, replace: bool = True):
     try:
       value = (await self.read(key)).unsafe()
       return await to.insert(to_key, value, replace=replace)
     except IsLeft as e:
       return Left(e.value)
 
   @overload
   def move(self, key: str, to: 'KV[T]', to_key: str, *, replace: Literal[False]) -> Promise[Either[DBError|InexistentItem|ExistentItem, None]]: ...
   @overload
   def move(self, key: str, to: 'KV[T]', to_key: str, *, replace: bool = True) -> Promise[Either[DBError|InexistentItem, None]]: ...
-  @lift
+  @P.lift
   async def move(self, key: str, to: 'KV[T]', to_key: str, *, replace: bool = True):
     try:
       (await self.copy(key, to, to_key, replace=replace)).unsafe()
       (await self.delete(key)).unsafe()
     except IsLeft as e:
       return Left(e.value)
```

### Comparing `kv_api-0.1.6/src/kv/api/append/append.py` & `kv_api-0.1.7/src/kv/api/append/append.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Generic, TypeVar, overload, Literal
 from abc import ABC, abstractmethod
-from haskellian.either import Either
-from haskellian.asyn.promises import Promise
+from haskellian import Either, Promise
 from ..errors import DBError, InexistentItem
 from ..api import KV
 
 T = TypeVar('T')
 
 class Appendable(ABC, Generic[T]):
   @overload
```

### Comparing `kv_api-0.1.6/src/kv/api/append/simple.py` & `kv_api-0.1.7/src/kv/api/append/simple.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Generic, TypeVar
-from haskellian.either import Left, Right, Either
-import haskellian.asyn.promises as P
+from haskellian import Left, Right, Either, promise as P
 from ..simple import SimpleKV
 from ..errors import InexistentItem, DBError
 from .append import AppendableKV
 
 T = TypeVar('T')
 
 class SimpleAppendKV(AppendableKV[T], SimpleKV[list[T]], Generic[T]):
```

### Comparing `kv_api-0.1.6/src/kv/api/errors/errors.py` & `kv_api-0.1.7/src/kv/api/errors/errors.py`

 * *Files identical despite different names*

### Comparing `kv_api-0.1.6/src/kv/api/simple.py` & `kv_api-0.1.7/src/kv/api/simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from typing import Generic, TypeVar, AsyncIterable
-from haskellian.either import Left, Right, Either, maybe
-import haskellian.asyn.promises as P
-import haskellian.asyn.iter as AI
+from haskellian import Left, Right, Either, either as E, promise as P, asyn_iter as AI
 from .api import KV
 from .errors import ExistentItem, InexistentItem, DBError, InvalidData, ReadError
 
 T = TypeVar('T')
 
 class SimpleKV(KV[T], Generic[T]):
   """Simple `KV` using a `dict`"""
@@ -19,15 +17,15 @@
       return Left(ExistentItem(key))
     else:
       self.xs[key] = value
       return Right(None)
 
   @P.lift
   async def read(self, key: str) -> Either[ReadError, T]:
-    return maybe(self.xs.get(key)).mapl(lambda _: InexistentItem(key))
+    return E.maybe(self.xs.get(key)).mapl(lambda _: InexistentItem(key))
 
   @P.lift
   async def delete(self, key: str) -> Either[DBError | InexistentItem, None]:
     if not key in self.xs:
       return Left(InexistentItem(key))
     else:
       del self.xs[key]
```

