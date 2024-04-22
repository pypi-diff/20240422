# Comparing `tmp/cs.resources-20240412.tar.gz` & `tmp/cs.resources-20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.resources-20240412.tar", last modified: Fri Apr 12 04:43:02 2024, max compression
+gzip compressed data, was "cs.resources-20240422.tar", last modified: Mon Apr 22 02:52:25 2024, max compression
```

## Comparing `cs.resources-20240412.tar` & `cs.resources-20240422.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:43:02.148893 cs.resources-20240412/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 04:42:35.000000 cs.resources-20240412/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    17683 2024-04-12 04:43:02.147971 cs.resources-20240412/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    16926 2024-04-12 04:42:44.000000 cs.resources-20240412/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:43:02.141777 cs.resources-20240412/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:43:02.142080 cs.resources-20240412/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:43:02.144666 cs.resources-20240412/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    27453 2024-04-12 04:42:21.000000 cs.resources-20240412/lib/python/cs/resources.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:43:02.147381 cs.resources-20240412/lib/python/cs.resources.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    17683 2024-04-12 04:43:01.000000 cs.resources-20240412/lib/python/cs.resources.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-04-12 04:43:02.000000 cs.resources-20240412/lib/python/cs.resources.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 04:43:01.000000 cs.resources-20240412/lib/python/cs.resources.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      210 2024-04-12 04:43:01.000000 cs.resources-20240412/lib/python/cs.resources.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 04:43:01.000000 cs.resources-20240412/lib/python/cs.resources.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    18297 2024-04-12 04:43:00.000000 cs.resources-20240412/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 04:43:02.149007 cs.resources-20240412/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:52:25.693492 cs.resources-20240422/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 02:51:51.000000 cs.resources-20240422/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17383 2024-04-22 02:52:25.693095 cs.resources-20240422/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    16626 2024-04-22 02:52:01.000000 cs.resources-20240422/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:52:25.686981 cs.resources-20240422/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:52:25.687277 cs.resources-20240422/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:52:25.689590 cs.resources-20240422/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    27536 2024-04-22 02:51:38.000000 cs.resources-20240422/lib/python/cs/resources.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:52:25.692511 cs.resources-20240422/lib/python/cs.resources.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17383 2024-04-22 02:52:24.000000 cs.resources-20240422/lib/python/cs.resources.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-04-22 02:52:25.000000 cs.resources-20240422/lib/python/cs.resources.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 02:52:25.000000 cs.resources-20240422/lib/python/cs.resources.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      210 2024-04-22 02:52:25.000000 cs.resources-20240422/lib/python/cs.resources.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 02:52:25.000000 cs.resources-20240422/lib/python/cs.resources.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17997 2024-04-22 02:52:23.000000 cs.resources-20240422/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 02:52:25.693602 cs.resources-20240422/setup.cfg
```

### Comparing `cs.resources-20240412/PKG-INFO` & `cs.resources-20240422/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.resources
-Version: 20240412
+Version: 20240422
 Summary: Resource management classes and functions.
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
 
 Resource management classes and functions.
 
-*Latest release 20240412*:
-* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
-* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
-* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
-* RunState.__init__: make most parameters keyword only.
+*Latest release 20240422*:
+dataclass backport for Python < 3.10.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -348,15 +345,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x104ae5d80>)`*:
+*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d3c5f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -375,14 +372,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240422*:
+dataclass backport for Python < 3.10.
+
 *Release 20240412*:
 * RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
 * RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
 * MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
 * RunState.__init__: make most parameters keyword only.
 
 *Release 20240316*:
```

### Comparing `cs.resources-20240412/README.md` & `cs.resources-20240422/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 Resource management classes and functions.
 
-*Latest release 20240412*:
-* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
-* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
-* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
-* RunState.__init__: make most parameters keyword only.
+*Latest release 20240422*:
+dataclass backport for Python < 3.10.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -330,15 +327,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x104ae5d80>)`*:
+*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d3c5f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -357,14 +354,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240422*:
+dataclass backport for Python < 3.10.
+
 *Release 20240412*:
 * RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
 * RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
 * MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
 * RunState.__init__: make most parameters keyword only.
 
 *Release 20240316*:
```

### Comparing `cs.resources-20240412/lib/python/cs/resources.py` & `cs.resources-20240422/lib/python/cs/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ''' Resource management classes and functions.
 '''
 
 from collections import defaultdict
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from functools import partial
+import sys
 from threading import Lock, current_thread, main_thread
 import time
 from typing import Any, Callable, Mapping, Optional, Tuple, Union
 
 from typeguard import typechecked
 
 from cs.context import contextif, stackattrs, setup_cmgr, ContextManagerMixin
@@ -24,15 +25,15 @@
 from cs.pfx import pfx_call, pfx_method
 from cs.psutils import signal_handlers
 from cs.py.func import prop
 from cs.py.stack import caller, frames as stack_frames, stack_dump, StackSummary
 from cs.result import CancellationError
 from cs.threads import ThreadState, HasThreadState, NRLock
 
-__version__ = '20240412'
+__version__ = '20240422'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -69,15 +70,20 @@
       )
     return func(self, *a, **kw)
 
   not_closed_wrapper.__name__ = "not_closed_wrapper(%s)" % (func.__name__,)
   return not_closed_wrapper
 
 # pylint: disable=too-few-public-methods,too-many-instance-attributes
-@dataclass(slots=True)
+if sys.version_info >= (3, 10):
+  _mdc = dataclass(slots=True)
+else:
+  _mdc = dataclass
+
+@_mdc
 class _MultiOpenMixinOpenCloseState:
 
   mom: "MultiOpenMixin"
   opened: bool = False
   opens: int = 0
   opens_from: Mapping = field(default_factory=lambda: defaultdict(int))
   final_close_from: StackSummary = None
```

### Comparing `cs.resources-20240412/lib/python/cs.resources.egg-info/PKG-INFO` & `cs.resources-20240422/lib/python/cs.resources.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.resources
-Version: 20240412
+Version: 20240422
 Summary: Resource management classes and functions.
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
 
 Resource management classes and functions.
 
-*Latest release 20240412*:
-* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
-* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
-* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
-* RunState.__init__: make most parameters keyword only.
+*Latest release 20240422*:
+dataclass backport for Python < 3.10.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -348,15 +345,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x104ae5d80>)`*:
+*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d3c5f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -375,14 +372,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240422*:
+dataclass backport for Python < 3.10.
+
 *Release 20240412*:
 * RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
 * RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
 * MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
 * RunState.__init__: make most parameters keyword only.
 
 *Release 20240316*:
```

### Comparing `cs.resources-20240412/pyproject.toml` & `cs.resources-20240422/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -14,43 +14,40 @@
     "cs.gimmicks>=20240316",
     "cs.obj>=20220918",
     "cs.pfx>=20240412",
     "cs.psutils>=20240316",
     "cs.py.func>=20230331",
     "cs.py.stack>=20240412",
     "cs.result>=20240412",
-    "cs.threads>=20240412",
+    "cs.threads>=20240422",
     "typeguard",
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
 Resource management classes and functions.
 
-*Latest release 20240412*:
-* RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
-* RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
-* MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
-* RunState.__init__: make most parameters keyword only.
+*Latest release 20240422*:
+dataclass backport for Python < 3.10.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -372,15 +369,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x104ae5d80>)`*:
+*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d3c5f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -399,14 +396,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240422*:
+dataclass backport for Python < 3.10.
+
 *Release 20240412*:
 * RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
 * RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
 * MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
 * RunState.__init__: make most parameters keyword only.
 
 *Release 20240316*:
```

