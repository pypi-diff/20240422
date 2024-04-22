# Comparing `tmp/django_ratelimiter-0.1.1.tar.gz` & `tmp/django_ratelimiter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ratelimiter-0.1.1.tar", max compression
+gzip compressed data, was "django_ratelimiter-0.1.2.tar", max compression
```

## Comparing `django_ratelimiter-0.1.1.tar` & `django_ratelimiter-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/LICENSE
--rw-r--r--   0        0        0     3722 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/README.md
--rw-r--r--   0        0        0      144 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/django_ratelimiter/__init__.py
--rw-r--r--   0        0        0     3323 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/django_ratelimiter/decorator.py
--rw-r--r--   0        0        0        0 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/django_ratelimiter/py.typed
--rw-r--r--   0        0        0     1607 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/django_ratelimiter/storage.py
--rw-r--r--   0        0        0      315 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/django_ratelimiter/types.py
--rw-r--r--   0        0        0      668 2024-04-15 20:21:16.364309 django_ratelimiter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4386 1970-01-01 00:00:00.000000 django_ratelimiter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4038 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/README.md
+-rw-r--r--   0        0        0      144 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/django_ratelimiter/__init__.py
+-rw-r--r--   0        0        0     4283 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/django_ratelimiter/decorator.py
+-rw-r--r--   0        0        0        0 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/django_ratelimiter/py.typed
+-rw-r--r--   0        0        0     1666 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/django_ratelimiter/storage.py
+-rw-r--r--   0        0        0      315 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/django_ratelimiter/types.py
+-rw-r--r--   0        0        0      966 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 django_ratelimiter-0.1.2/PKG-INFO
```

### Comparing `django_ratelimiter-0.1.1/LICENSE` & `django_ratelimiter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ratelimiter-0.1.1/README.md` & `django_ratelimiter-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # django-ratelimiter
 
 [![PyPI version](https://badge.fury.io/py/django-ratelimiter.svg)](https://pypi.org/project/django-ratelimiter/)
-[![CI](https://github.com/andriykohut/django-ratelimiter/actions/workflows/workflow.yml/badge.svg)](https://github.com/andriykohut/django-ratelimiter/actions/workflows/workflow.yml?query=branch%3Amain)
+[![CI](https://github.com/andriykohut/django-ratelimiter/actions/workflows/ci.yml/badge.svg)](https://github.com/andriykohut/django-ratelimiter/actions/workflows/ci.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/andriykohut/django-ratelimiter/branch/main/graph/badge.svg)](https://codecov.io/gh/andriykohut/django-ratelimiter)
 [![Python Versions](https://img.shields.io/pypi/pyversions/django-ratelimiter)](https://pypi.python.org/pypi/django-ratelimiter/)
 [![license](https://img.shields.io/pypi/l/django-ratelimiter.svg)](https://pypi.python.org/pypi/django-ratelimiter)
 [![docs](https://readthedocs.org/projects/django-ratelimiter/badge/?version=latest)](https://django-ratelimiter.readthedocs.io/)
 
 Rate limiting for django using [limits](https://limits.readthedocs.io/en/stable/).
 
@@ -48,15 +48,15 @@
 
 For more details on storages refer to limits [documentation](https://limits.readthedocs.io/en/stable/storage.html).
 
 ### Rate limiting strategies
 
 - [Fixed window](https://limits.readthedocs.io/en/stable/strategies.html#fixed-window)
 - [Fixed Window with Elastic Expiry](https://limits.readthedocs.io/en/stable/strategies.html#fixed-window-with-elastic-expiry)
-- [Moving Window](https://limits.readthedocs.io/en/stable/strategies.html#moving-window). Only supported with `limits` storage by setting `DJANGO_RATELIMITER_STORAGE`.
+- [Moving Window](https://limits.readthedocs.io/en/stable/strategies.html#moving-window) - Only supported with `limits` storage by setting `DJANGO_RATELIMITER_STORAGE`
 
 ### View decorator
 
 By default all requests are rate limited
 
 ```py
 from django_ratelimiter import ratelimit
@@ -115,7 +115,14 @@
 
 from limits.storage import RedisStorage
 
 @ratelimit("5/minute", storage=RedisStorage(uri="redis://localhost:6379/0"))
 def view(request):
     return HttpResponse("OK")
 ```
+
+### DRF/ninja/class-based views
+
+`django-ratelimiter` is framework-agnostic, it should work with DRF/ninja out of the box.
+Class-based views are also supported with [method_decorator](https://docs.djangoproject.com/en/5.0/topics/class-based-views/intro/#decorating-the-class).
+
+See examples in [test_app](./test_app/views.py).
```

### Comparing `django_ratelimiter-0.1.1/django_ratelimiter/decorator.py` & `django_ratelimiter-0.1.2/django_ratelimiter/decorator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Sequence, Union, Optional
+from typing import Callable, Literal, Sequence, Union, Optional
 from functools import wraps, partial
 
 from django.db import models
 from django.conf import settings
 from django.http import HttpRequest, HttpResponse
 from limits.strategies import STRATEGIES, RateLimiter
 from limits.storage import Storage
@@ -10,14 +10,15 @@
 from django_ratelimiter.storage import CacheStorage
 from django_ratelimiter.types import ViewFunc, P
 
 
 def build_identifiers(
     func: ViewFunc, methods: Union[str, Sequence[str], None] = None
 ) -> list[str]:
+    """Build view identifiers for storage cache key using function signature and list of methods."""
     if isinstance(func, partial):
         # method_decorator scenario
         identifiers = [
             func.func.__self__.__class__.__module__,
             f"{func.func.__self__.__class__.__qualname__}.{func.func.__name__}",
         ]
     else:
@@ -25,41 +26,59 @@
     if methods:
         methods_ = methods if isinstance(methods, str) else "|".join(sorted(methods))
         identifiers.append(methods_)
     return identifiers
 
 
 def get_storage() -> Storage:
+    """Returns a default storage backend instance, defined by either `DJANGO_RATELIMITER_CACHE`
+    or `DJANGO_RATELIMITER_STORAGE`."""
     cache_name: Optional[str] = getattr(settings, "DJANGO_RATELIMITER_CACHE", None)
     storage: Optional[Storage] = getattr(settings, "DJANGO_RATELIMITER_STORAGE", None)
     if cache_name and storage:
         raise ValueError(
             "DJANGO_RATELIMITER_CACHE and DJANGO_RATELIMITER_STORAGE can't be used together"
         )
     return storage or CacheStorage(cache_name or "default")
 
 
 def get_rate_limiter(strategy: str, storage: Optional[Storage] = None) -> RateLimiter:
+    """Return a ratelimiter instance for given strategy."""
     if strategy not in STRATEGIES:
         raise ValueError(
             f"Unknown strategy {strategy}, must be one of {STRATEGIES.keys()}"
         )
     storage = storage or get_storage()
     return STRATEGIES[strategy](storage)
 
 
 def ratelimit(
     rate: Union[str, Callable[[HttpRequest], str]],
     key: Union[str, Callable[[HttpRequest], str], None] = None,
     methods: Union[str, Sequence[str], None] = None,
-    strategy: str = "fixed-window",
+    strategy: Literal[
+        "fixed-window",
+        "fixed-window-elastic-expiry",
+        "moving-window",
+    ] = "fixed-window",
     response: Optional[HttpResponse] = None,
     storage: Optional[Storage] = None,
     cache: Optional[str] = None,
 ) -> Callable[[ViewFunc], ViewFunc]:
+    """Rate limiting decorator for wrapping views.
+
+    Arguments:
+        rate: rate string (i.e. `5/second`) or a callable that takes a request and returns a rate
+        key: request attribute or callable that returns a string to be used as identifier
+        methods: only rate limit specified method(s)
+        strategy: a name of rate limiting strategy
+        response: custom rate limit response instance
+        storage: override default rate limit storage
+        cache: override default cache name if using django cache storage backend
+    """
     if storage and cache:
         raise ValueError("Can't use both cache and storage")
     rate_limiter = get_rate_limiter(strategy, storage)
 
     def decorator(func: ViewFunc) -> ViewFunc:
         @wraps(func)
         def wrapper(
```

### Comparing `django_ratelimiter-0.1.1/django_ratelimiter/storage.py` & `django_ratelimiter-0.1.2/django_ratelimiter/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from django.core.cache import caches, BaseCache
 
 from limits.storage import Storage
 
 
 class CacheStorage(Storage):
+    """Rate limiting storage with django cache backend."""
 
     def __init__(
         self,
         cache: str,
         wrap_exceptions: bool = False,
         **options: Union[float, str, bool],
     ) -> None:
```

### Comparing `django_ratelimiter-0.1.1/PKG-INFO` & `django_ratelimiter-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ratelimiter
-Version: 0.1.1
+Version: 0.1.2
 Summary: Rate-limiting for django
 License: MIT
 Author: Andrii Kohut
 Author-email: kogut.andriy@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Requires-Dist: limits (>=3.10)
 Requires-Dist: typing-extensions (>=4.11.0,<5.0.0) ; python_version == "3.9"
 Description-Content-Type: text/markdown
 
 # django-ratelimiter
 
 [![PyPI version](https://badge.fury.io/py/django-ratelimiter.svg)](https://pypi.org/project/django-ratelimiter/)
-[![CI](https://github.com/andriykohut/django-ratelimiter/actions/workflows/workflow.yml/badge.svg)](https://github.com/andriykohut/django-ratelimiter/actions/workflows/workflow.yml?query=branch%3Amain)
+[![CI](https://github.com/andriykohut/django-ratelimiter/actions/workflows/ci.yml/badge.svg)](https://github.com/andriykohut/django-ratelimiter/actions/workflows/ci.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/andriykohut/django-ratelimiter/branch/main/graph/badge.svg)](https://codecov.io/gh/andriykohut/django-ratelimiter)
 [![Python Versions](https://img.shields.io/pypi/pyversions/django-ratelimiter)](https://pypi.python.org/pypi/django-ratelimiter/)
 [![license](https://img.shields.io/pypi/l/django-ratelimiter.svg)](https://pypi.python.org/pypi/django-ratelimiter)
 [![docs](https://readthedocs.org/projects/django-ratelimiter/badge/?version=latest)](https://django-ratelimiter.readthedocs.io/)
 
 Rate limiting for django using [limits](https://limits.readthedocs.io/en/stable/).
 
@@ -67,15 +67,15 @@
 
 For more details on storages refer to limits [documentation](https://limits.readthedocs.io/en/stable/storage.html).
 
 ### Rate limiting strategies
 
 - [Fixed window](https://limits.readthedocs.io/en/stable/strategies.html#fixed-window)
 - [Fixed Window with Elastic Expiry](https://limits.readthedocs.io/en/stable/strategies.html#fixed-window-with-elastic-expiry)
-- [Moving Window](https://limits.readthedocs.io/en/stable/strategies.html#moving-window). Only supported with `limits` storage by setting `DJANGO_RATELIMITER_STORAGE`.
+- [Moving Window](https://limits.readthedocs.io/en/stable/strategies.html#moving-window) - Only supported with `limits` storage by setting `DJANGO_RATELIMITER_STORAGE`
 
 ### View decorator
 
 By default all requests are rate limited
 
 ```py
 from django_ratelimiter import ratelimit
@@ -135,7 +135,14 @@
 from limits.storage import RedisStorage
 
 @ratelimit("5/minute", storage=RedisStorage(uri="redis://localhost:6379/0"))
 def view(request):
     return HttpResponse("OK")
 ```
 
+### DRF/ninja/class-based views
+
+`django-ratelimiter` is framework-agnostic, it should work with DRF/ninja out of the box.
+Class-based views are also supported with [method_decorator](https://docs.djangoproject.com/en/5.0/topics/class-based-views/intro/#decorating-the-class).
+
+See examples in [test_app](./test_app/views.py).
+
```

