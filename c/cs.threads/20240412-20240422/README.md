# Comparing `tmp/cs.threads-20240412.tar.gz` & `tmp/cs.threads-20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.threads-20240412.tar", last modified: Fri Apr 12 03:32:19 2024, max compression
+gzip compressed data, was "cs.threads-20240422.tar", last modified: Mon Apr 22 02:46:37 2024, max compression
```

## Comparing `cs.threads-20240412.tar` & `cs.threads-20240422.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 03:32:19.224279 cs.threads-20240412/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 03:31:53.000000 cs.threads-20240412/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    18084 2024-04-12 03:32:19.223940 cs.threads-20240412/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    17315 2024-04-12 03:32:01.000000 cs.threads-20240412/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 03:32:19.219894 cs.threads-20240412/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 03:32:19.220210 cs.threads-20240412/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 03:32:19.221620 cs.threads-20240412/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    27102 2024-04-12 03:25:42.000000 cs.threads-20240412/lib/python/cs/threads.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 03:32:19.223453 cs.threads-20240412/lib/python/cs.threads.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    18084 2024-04-12 03:32:18.000000 cs.threads-20240412/lib/python/cs.threads.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      285 2024-04-12 03:32:19.000000 cs.threads-20240412/lib/python/cs.threads.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 03:32:18.000000 cs.threads-20240412/lib/python/cs.threads.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      140 2024-04-12 03:32:18.000000 cs.threads-20240412/lib/python/cs.threads.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 03:32:19.000000 cs.threads-20240412/lib/python/cs.threads.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    18608 2024-04-12 03:32:17.000000 cs.threads-20240412/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 03:32:19.224381 cs.threads-20240412/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:46:37.707535 cs.threads-20240422/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 02:46:07.000000 cs.threads-20240422/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17806 2024-04-22 02:46:37.707158 cs.threads-20240422/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17037 2024-04-22 02:46:17.000000 cs.threads-20240422/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:46:37.702297 cs.threads-20240422/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:46:37.702612 cs.threads-20240422/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:46:37.704365 cs.threads-20240422/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    27177 2024-04-22 02:45:53.000000 cs.threads-20240422/lib/python/cs/threads.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:46:37.706642 cs.threads-20240422/lib/python/cs.threads.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17806 2024-04-22 02:46:37.000000 cs.threads-20240422/lib/python/cs.threads.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      285 2024-04-22 02:46:37.000000 cs.threads-20240422/lib/python/cs.threads.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 02:46:37.000000 cs.threads-20240422/lib/python/cs.threads.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      162 2024-04-22 02:46:37.000000 cs.threads-20240422/lib/python/cs.threads.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 02:46:37.000000 cs.threads-20240422/lib/python/cs.threads.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18359 2024-04-22 02:46:35.000000 cs.threads-20240422/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 02:46:37.707639 cs.threads-20240422/setup.cfg
```

### Comparing `cs.threads-20240412/PKG-INFO` & `cs.threads-20240422/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.threads
-Version: 20240412
+Version: 20240422
 Summary: threading and communication/synchronisation conveniences
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,19 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Thread related convenience classes and functions.
 
-*Latest release 20240412*:
-* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
-* bg: rename thread_class to thread_factory for clarity.
-* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
-* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
+*Latest release 20240422*:
+HasThreadState.default: make factory and raise_on keyword only.
 
 ## Class `AdjustableSemaphore`
 
 A semaphore whose value may be tuned after instantiation.
 
 *Method `AdjustableSemaphore.acquire(self, blocking=True)`*:
 The acquire() method calls the base acquire() method if not blocking.
@@ -131,15 +128,15 @@
 in the child `Thread` while running `func` as follows:
 - `None`: the default, meaning `(self,)`
 - `False`: no object contexts are entered
 - `True`: all current `HasThreadState` object contexts will be entered
 - an iterable of objects whose contexts will be entered;
   pass `()` to enter no objects
 
-*Method `HasThreadState.default(factory=None, raise_on_None=False)`*:
+*Method `HasThreadState.default(*, factory=None, raise_on_None=False)`*:
 The default instance of this class from `cls.perthread_state.current`.
 
 Parameters:
 * `factory`: optional callable to create an instance of `cls`
   if `cls.perthread_state.current` is `None` or missing;
   if `factory` is `True` then `cls` is used as the factory
 * `raise_on_None`: if `cls.perthread_state.current` is `None` or missing
@@ -188,15 +185,15 @@
 Exposes the `._lock` as the property `.lock`.
 Presents a context manager interface for obtaining an object's lock.
 
 *Method `LockableMixin.__exit__(self, exc_type, exc_value, traceback)`*:
 pylint: disable=unused-argument
 
 *Property `LockableMixin.lock`*:
-Return the lock.
+The internal lock object.
 
 ## Function `locked(*da, **dkw)`
 
 A decorator for instance methods that must run within a lock.
 
 Decorator keyword arguments:
 * `initial_timeout`:
@@ -358,21 +355,24 @@
 Calling a `ThreadState` returns a context manager which stacks some state.
 The context manager yields the previous values
 for the attributes which were stacked.
 
 ## Function `via(cmanager, func, *a, **kw)`
 
 Return a callable that calls the supplied `func` inside a
-with statement using the context manager `cmanager`.
+`with` statement using the context manager `cmanager`.
 This intended use case is aimed at deferred function calls.
 
 # Release Log
 
 
 
+*Release 20240422*:
+HasThreadState.default: make factory and raise_on keyword only.
+
 *Release 20240412*:
 * New NRLock, an nonrecursive Lock and associated exception DeadlockError.
 * bg: rename thread_class to thread_factory for clarity.
 * HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
 * HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
 
 *Release 20240316*:
```

### Comparing `cs.threads-20240412/README.md` & `cs.threads-20240422/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 Thread related convenience classes and functions.
 
-*Latest release 20240412*:
-* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
-* bg: rename thread_class to thread_factory for clarity.
-* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
-* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
+*Latest release 20240422*:
+HasThreadState.default: make factory and raise_on keyword only.
 
 ## Class `AdjustableSemaphore`
 
 A semaphore whose value may be tuned after instantiation.
 
 *Method `AdjustableSemaphore.acquire(self, blocking=True)`*:
 The acquire() method calls the base acquire() method if not blocking.
@@ -113,15 +110,15 @@
 in the child `Thread` while running `func` as follows:
 - `None`: the default, meaning `(self,)`
 - `False`: no object contexts are entered
 - `True`: all current `HasThreadState` object contexts will be entered
 - an iterable of objects whose contexts will be entered;
   pass `()` to enter no objects
 
-*Method `HasThreadState.default(factory=None, raise_on_None=False)`*:
+*Method `HasThreadState.default(*, factory=None, raise_on_None=False)`*:
 The default instance of this class from `cls.perthread_state.current`.
 
 Parameters:
 * `factory`: optional callable to create an instance of `cls`
   if `cls.perthread_state.current` is `None` or missing;
   if `factory` is `True` then `cls` is used as the factory
 * `raise_on_None`: if `cls.perthread_state.current` is `None` or missing
@@ -170,15 +167,15 @@
 Exposes the `._lock` as the property `.lock`.
 Presents a context manager interface for obtaining an object's lock.
 
 *Method `LockableMixin.__exit__(self, exc_type, exc_value, traceback)`*:
 pylint: disable=unused-argument
 
 *Property `LockableMixin.lock`*:
-Return the lock.
+The internal lock object.
 
 ## Function `locked(*da, **dkw)`
 
 A decorator for instance methods that must run within a lock.
 
 Decorator keyword arguments:
 * `initial_timeout`:
@@ -340,21 +337,24 @@
 Calling a `ThreadState` returns a context manager which stacks some state.
 The context manager yields the previous values
 for the attributes which were stacked.
 
 ## Function `via(cmanager, func, *a, **kw)`
 
 Return a callable that calls the supplied `func` inside a
-with statement using the context manager `cmanager`.
+`with` statement using the context manager `cmanager`.
 This intended use case is aimed at deferred function calls.
 
 # Release Log
 
 
 
+*Release 20240422*:
+HasThreadState.default: make factory and raise_on keyword only.
+
 *Release 20240412*:
 * New NRLock, an nonrecursive Lock and associated exception DeadlockError.
 * bg: rename thread_class to thread_factory for clarity.
 * HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
 * HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
 
 *Release 20240316*:
```

### Comparing `cs.threads-20240412/lib/python/cs/threads.py` & `cs.threads-20240422/lib/python/cs/threads.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from cs.excutils import logexc, transmute
 from cs.gimmicks import error, warning
 from cs.pfx import Pfx  # prefix
 from cs.py.func import funcname, prop
 from cs.py.stack import caller
 from cs.seq import Seq
 
-__version__ = '20240412'
+__version__ = '20240422'
 
 DISTINFO = {
     'description':
     "threading and communication/synchronisation conveniences",
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
@@ -48,14 +48,15 @@
     'install_requires': [
         'cs.context',
         'cs.deco',
         'cs.excutils',
         'cs.gimmicks',
         'cs.pfx',
         'cs.py.func',
+        'cs.py.stack',
         'cs.seq',
     ],
 }
 
 class ThreadState(thread_local):
   ''' A `Thread` local object with attributes
       which can be used as a context manager to stack attribute values.
@@ -122,15 +123,15 @@
   _HasThreadState_lock = Lock()
   _HasThreadState_classes = set()
 
   # the default name for the Thread state attribute
   THREAD_STATE_ATTR = 'perthread_state'
 
   @classmethod
-  def default(cls, factory=None, raise_on_None=False):
+  def default(cls, *, factory=None, raise_on_None=False):
     ''' The default instance of this class from `cls.perthread_state.current`.
 
         Parameters:
         * `factory`: optional callable to create an instance of `cls`
           if `cls.perthread_state.current` is `None` or missing;
           if `factory` is `True` then `cls` is used as the factory
         * `raise_on_None`: if `cls.perthread_state.current` is `None` or missing
@@ -538,16 +539,16 @@
       The default "unset" value for the cache is `None`.
   '''
   if prop_name is None:
     prop_name = '_' + func.__name__
 
   @transmute(exc_from=AttributeError)
   def locked_property_getprop(self):
-    ''' Attempt lockless fetch of property first.
-        Use lock if property is unset.
+    ''' Attempt lockless fetch of the property first.
+        Use lock if the property is unset.
     '''
     p = getattr(self, prop_name, unset_object)
     if p is unset_object:
       try:
         lock = getattr(self, lock_name)
       except AttributeError:
         error("no %s.%s attribute", type(self).__name__, lock_name)
@@ -579,29 +580,29 @@
 
   # pylint: disable=unused-argument
   def __exit__(self, exc_type, exc_value, traceback):
     self._lock.release()
 
   @property
   def lock(self):
-    ''' Return the lock.
+    ''' The internal lock object.
     '''
     return self._lock
 
 def via(cmanager, func, *a, **kw):
   ''' Return a callable that calls the supplied `func` inside a
-      with statement using the context manager `cmanager`.
+      `with` statement using the context manager `cmanager`.
       This intended use case is aimed at deferred function calls.
   '''
 
-  def f():
+  def via_func_wrapper():
     with cmanager:
       return func(*a, **kw)
 
-  return f
+  return via_func_wrapper
 
 class PriorityLockSubLock(namedtuple('PriorityLockSubLock',
                                      'name priority lock priority_lock')):
   ''' The record for the per-`acquire`r `Lock` held by `PriorityLock.acquire`.
   '''
 
   def __str__(self):
```

### Comparing `cs.threads-20240412/lib/python/cs.threads.egg-info/PKG-INFO` & `cs.threads-20240422/lib/python/cs.threads.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.threads
-Version: 20240412
+Version: 20240422
 Summary: threading and communication/synchronisation conveniences
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,19 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Thread related convenience classes and functions.
 
-*Latest release 20240412*:
-* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
-* bg: rename thread_class to thread_factory for clarity.
-* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
-* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
+*Latest release 20240422*:
+HasThreadState.default: make factory and raise_on keyword only.
 
 ## Class `AdjustableSemaphore`
 
 A semaphore whose value may be tuned after instantiation.
 
 *Method `AdjustableSemaphore.acquire(self, blocking=True)`*:
 The acquire() method calls the base acquire() method if not blocking.
@@ -131,15 +128,15 @@
 in the child `Thread` while running `func` as follows:
 - `None`: the default, meaning `(self,)`
 - `False`: no object contexts are entered
 - `True`: all current `HasThreadState` object contexts will be entered
 - an iterable of objects whose contexts will be entered;
   pass `()` to enter no objects
 
-*Method `HasThreadState.default(factory=None, raise_on_None=False)`*:
+*Method `HasThreadState.default(*, factory=None, raise_on_None=False)`*:
 The default instance of this class from `cls.perthread_state.current`.
 
 Parameters:
 * `factory`: optional callable to create an instance of `cls`
   if `cls.perthread_state.current` is `None` or missing;
   if `factory` is `True` then `cls` is used as the factory
 * `raise_on_None`: if `cls.perthread_state.current` is `None` or missing
@@ -188,15 +185,15 @@
 Exposes the `._lock` as the property `.lock`.
 Presents a context manager interface for obtaining an object's lock.
 
 *Method `LockableMixin.__exit__(self, exc_type, exc_value, traceback)`*:
 pylint: disable=unused-argument
 
 *Property `LockableMixin.lock`*:
-Return the lock.
+The internal lock object.
 
 ## Function `locked(*da, **dkw)`
 
 A decorator for instance methods that must run within a lock.
 
 Decorator keyword arguments:
 * `initial_timeout`:
@@ -358,21 +355,24 @@
 Calling a `ThreadState` returns a context manager which stacks some state.
 The context manager yields the previous values
 for the attributes which were stacked.
 
 ## Function `via(cmanager, func, *a, **kw)`
 
 Return a callable that calls the supplied `func` inside a
-with statement using the context manager `cmanager`.
+`with` statement using the context manager `cmanager`.
 This intended use case is aimed at deferred function calls.
 
 # Release Log
 
 
 
+*Release 20240422*:
+HasThreadState.default: make factory and raise_on keyword only.
+
 *Release 20240412*:
 * New NRLock, an nonrecursive Lock and associated exception DeadlockError.
 * bg: rename thread_class to thread_factory for clarity.
 * HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
 * HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
 
 *Release 20240316*:
```

### Comparing `cs.threads-20240412/pyproject.toml` & `cs.threads-20240422/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,42 +11,40 @@
 dependencies = [
     "cs.context>=20240412",
     "cs.deco>=20240412",
     "cs.excutils>=20230212.1",
     "cs.gimmicks>=20240316",
     "cs.pfx>=20240412",
     "cs.py.func>=20230331",
+    "cs.py.stack>=20240412",
     "cs.seq>=20221118",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240412"
+version = "20240422"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Thread related convenience classes and functions.
 
-*Latest release 20240412*:
-* New NRLock, an nonrecursive Lock and associated exception DeadlockError.
-* bg: rename thread_class to thread_factory for clarity.
-* HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
-* HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
+*Latest release 20240422*:
+HasThreadState.default: make factory and raise_on keyword only.
 
 ## Class `AdjustableSemaphore`
 
 A semaphore whose value may be tuned after instantiation.
 
 *Method `AdjustableSemaphore.acquire(self, blocking=True)`*:
 The acquire() method calls the base acquire() method if not blocking.
@@ -151,15 +149,15 @@
 in the child `Thread` while running `func` as follows:
 - `None`: the default, meaning `(self,)`
 - `False`: no object contexts are entered
 - `True`: all current `HasThreadState` object contexts will be entered
 - an iterable of objects whose contexts will be entered;
   pass `()` to enter no objects
 
-*Method `HasThreadState.default(factory=None, raise_on_None=False)`*:
+*Method `HasThreadState.default(*, factory=None, raise_on_None=False)`*:
 The default instance of this class from `cls.perthread_state.current`.
 
 Parameters:
 * `factory`: optional callable to create an instance of `cls`
   if `cls.perthread_state.current` is `None` or missing;
   if `factory` is `True` then `cls` is used as the factory
 * `raise_on_None`: if `cls.perthread_state.current` is `None` or missing
@@ -208,15 +206,15 @@
 Exposes the `._lock` as the property `.lock`.
 Presents a context manager interface for obtaining an object's lock.
 
 *Method `LockableMixin.__exit__(self, exc_type, exc_value, traceback)`*:
 pylint: disable=unused-argument
 
 *Property `LockableMixin.lock`*:
-Return the lock.
+The internal lock object.
 
 ## Function `locked(*da, **dkw)`
 
 A decorator for instance methods that must run within a lock.
 
 Decorator keyword arguments:
 * `initial_timeout`:
@@ -378,21 +376,24 @@
 Calling a `ThreadState` returns a context manager which stacks some state.
 The context manager yields the previous values
 for the attributes which were stacked.
 
 ## Function `via(cmanager, func, *a, **kw)`
 
 Return a callable that calls the supplied `func` inside a
-with statement using the context manager `cmanager`.
+`with` statement using the context manager `cmanager`.
 This intended use case is aimed at deferred function calls.
 
 # Release Log
 
 
 
+*Release 20240422*:
+HasThreadState.default: make factory and raise_on keyword only.
+
 *Release 20240412*:
 * New NRLock, an nonrecursive Lock and associated exception DeadlockError.
 * bg: rename thread_class to thread_factory for clarity.
 * HasThreadState: big refactor to separate the mapping of default instances from the previously automatic opening of a context for each.
 * HasThreadState.bg: new optional pre_enter_objects to supply objects which should be opened before the Thread starts (before bg returns) and closed when the Thread exits.
 
 *Release 20240316*:
```

