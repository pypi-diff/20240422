# Comparing `tmp/that_depends-1.6.2.tar.gz` & `tmp/that_depends-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.6.2.tar", max compression
+gzip compressed data, was "that_depends-1.6.3.tar", max compression
```

## Comparing `that_depends-1.6.2.tar` & `that_depends-1.6.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     6711 2024-04-16 18:31:17.949107 that_depends-1.6.2/README.md
--rw-r--r--   0        0        0     1482 2024-04-21 14:49:28.883474 that_depends-1.6.2/pyproject.toml
--rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.6.2/that_depends/__init__.py
--rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.6.2/that_depends/container.py
--rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.6.2/that_depends/injection.py
--rw-r--r--   0        0        0      670 2024-04-21 11:20:54.815386 that_depends-1.6.2/that_depends/providers/__init__.py
--rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.6.2/that_depends/providers/base.py
--rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.6.2/that_depends/providers/collections.py
--rw-r--r--   0        0        0     2945 2024-04-21 14:48:19.135992 that_depends-1.6.2/that_depends/providers/context_resources.py
--rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.6.2/that_depends/providers/factories.py
--rw-r--r--   0        0        0     2508 2024-04-21 14:47:01.630728 that_depends-1.6.2/that_depends/providers/resources.py
--rw-r--r--   0        0        0      993 2024-04-17 05:36:03.299156 that_depends-1.6.2/that_depends/providers/singleton.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.6.2/that_depends/py.typed
--rw-r--r--   0        0        0     7191 1970-01-01 00:00:00.000000 that_depends-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.6.3/LICENSE
+-rw-r--r--   0        0        0     7268 2024-04-21 16:47:48.481078 that_depends-1.6.3/README.md
+-rw-r--r--   0        0        0     1482 2024-04-21 21:10:48.451782 that_depends-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.6.3/that_depends/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.6.3/that_depends/container.py
+-rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.6.3/that_depends/injection.py
+-rw-r--r--   0        0        0      670 2024-04-21 11:20:54.815386 that_depends-1.6.3/that_depends/providers/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.6.3/that_depends/providers/base.py
+-rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.6.3/that_depends/providers/collections.py
+-rw-r--r--   0        0        0     2945 2024-04-21 14:48:19.135992 that_depends-1.6.3/that_depends/providers/context_resources.py
+-rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.6.3/that_depends/providers/factories.py
+-rw-r--r--   0        0        0     2948 2024-04-21 21:10:28.406639 that_depends-1.6.3/that_depends/providers/resources.py
+-rw-r--r--   0        0        0      993 2024-04-17 05:36:03.299156 that_depends-1.6.3/that_depends/providers/singleton.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.6.3/that_depends/py.typed
+-rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 that_depends-1.6.3/PKG-INFO
```

### Comparing `that_depends-1.6.2/README.md` & `that_depends-1.6.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 "That Depends"
 ==
+[![GitHub issues](https://img.shields.io/github/issues/modern-python/that-depends)](https://github.com/modern-python/that-depends/issues)
+[![GitHub forks](https://img.shields.io/github/forks/modern-python/that-depends)](https://github.com/modern-python/that-depends/network)
+[![GitHub stars](https://img.shields.io/github/stars/modern-python/that-depends)](https://github.com/modern-python/that-depends/stargazers)
+[![GitHub license](https://img.shields.io/github/license/modern-python/that-depends)](https://github.com/modern-python/that-depends/blob/main/LICENSE)
+
 This package is dependency injection framework for Python, mostly inspired by `python-dependency-injector`.
 
 It is production-ready and gives you the following:
 - Fully-async simple DI framework with IOC-container.
 - Python 3.10-3.12 support.
 - Full coverage by types annotations (mypy in strict mode).
 - FastAPI and Litestar compatibility.
@@ -78,16 +83,16 @@
 @dataclasses.dataclass(kw_only=True, slots=True)
 class AsyncDependentFactory:
     independent_factory: IndependentFactory
     async_resource: str
 
 
 class DIContainer(BaseContainer):
-    sync_resource = providers.Resource[str](create_sync_resource)
-    async_resource = providers.AsyncResource[str](create_async_resource)
+    sync_resource = providers.Resource(create_sync_resource)
+    async_resource = providers.AsyncResource(create_async_resource)
 
     independent_factory = providers.Factory(IndependentFactory, dep1="text", dep2=123)
     sync_dependent_factory = providers.Factory(
         SyncDependentFactory,
         independent_factory=independent_factory,
         sync_resource=sync_resource,
     )
```

### Comparing `that_depends-1.6.2/pyproject.toml` & `that_depends-1.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.6.2"
+version = "1.6.3"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
```

### Comparing `that_depends-1.6.2/that_depends/container.py` & `that_depends-1.6.3/that_depends/container.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.2/that_depends/injection.py` & `that_depends-1.6.3/that_depends/injection.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.2/that_depends/providers/__init__.py` & `that_depends-1.6.3/that_depends/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.2/that_depends/providers/base.py` & `that_depends-1.6.3/that_depends/providers/base.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.2/that_depends/providers/context_resources.py` & `that_depends-1.6.3/that_depends/providers/context_resources.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.2/that_depends/providers/factories.py` & `that_depends-1.6.3/that_depends/providers/factories.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.2/that_depends/providers/resources.py` & `that_depends-1.6.3/that_depends/providers/resources.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import contextlib
 import inspect
 import typing
 
-from that_depends.providers.base import AbstractResource
+from that_depends.providers.base import AbstractProvider, AbstractResource
 
 
 T = typing.TypeVar("T")
 P = typing.ParamSpec("P")
 
 
 class Resource(AbstractResource[T]):
@@ -37,15 +37,18 @@
         if self._override:
             return typing.cast(T, self._override)
 
         if self._instance is None:
             self._instance = typing.cast(
                 T,
                 self._context_stack.enter_context(
-                    contextlib.contextmanager(self._creator)(*self._args, **self._kwargs),
+                    contextlib.contextmanager(self._creator)(
+                        *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
+                        **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
+                    ),
                 ),
             )
         return self._instance
 
 
 class AsyncResource(AbstractResource[T]):
     def __init__(
@@ -75,11 +78,14 @@
         if self._override:
             return typing.cast(T, self._override)
 
         if self._instance is None:
             self._instance = typing.cast(
                 T,
                 await self._context_stack.enter_async_context(
-                    contextlib.asynccontextmanager(self._creator)(*self._args, **self._kwargs),
+                    contextlib.asynccontextmanager(self._creator)(
+                        *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
+                        **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
+                    ),
                 ),
             )
         return self._instance
```

### Comparing `that_depends-1.6.2/that_depends/providers/singleton.py` & `that_depends-1.6.3/that_depends/providers/singleton.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.2/PKG-INFO` & `that_depends-1.6.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: that-depends
-Version: 1.6.2
+Version: 1.6.3
 Summary: Simple Dependency Injection framework
 Home-page: https://github.com/modern-python/that-depends
 Author: Artur Shiriev
 Author-email: me@shiriev.ru
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 "That Depends"
 ==
+[![GitHub issues](https://img.shields.io/github/issues/modern-python/that-depends)](https://github.com/modern-python/that-depends/issues)
+[![GitHub forks](https://img.shields.io/github/forks/modern-python/that-depends)](https://github.com/modern-python/that-depends/network)
+[![GitHub stars](https://img.shields.io/github/stars/modern-python/that-depends)](https://github.com/modern-python/that-depends/stargazers)
+[![GitHub license](https://img.shields.io/github/license/modern-python/that-depends)](https://github.com/modern-python/that-depends/blob/main/LICENSE)
+
 This package is dependency injection framework for Python, mostly inspired by `python-dependency-injector`.
 
 It is production-ready and gives you the following:
 - Fully-async simple DI framework with IOC-container.
 - Python 3.10-3.12 support.
 - Full coverage by types annotations (mypy in strict mode).
 - FastAPI and Litestar compatibility.
@@ -92,16 +97,16 @@
 @dataclasses.dataclass(kw_only=True, slots=True)
 class AsyncDependentFactory:
     independent_factory: IndependentFactory
     async_resource: str
 
 
 class DIContainer(BaseContainer):
-    sync_resource = providers.Resource[str](create_sync_resource)
-    async_resource = providers.AsyncResource[str](create_async_resource)
+    sync_resource = providers.Resource(create_sync_resource)
+    async_resource = providers.AsyncResource(create_async_resource)
 
     independent_factory = providers.Factory(IndependentFactory, dep1="text", dep2=123)
     sync_dependent_factory = providers.Factory(
         SyncDependentFactory,
         independent_factory=independent_factory,
         sync_resource=sync_resource,
     )
```

