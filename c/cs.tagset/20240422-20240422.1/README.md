# Comparing `tmp/cs.tagset-20240422.tar.gz` & `tmp/cs.tagset-20240422.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.tagset-20240422.tar", last modified: Mon Apr 22 03:00:29 2024, max compression
+gzip compressed data, was "cs.tagset-20240422.1.tar", last modified: Mon Apr 22 04:37:43 2024, max compression
```

## Comparing `cs.tagset-20240422.tar` & `cs.tagset-20240422.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:00:29.538258 cs.tagset-20240422/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 02:59:59.000000 cs.tagset-20240422/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    66713 2024-04-22 03:00:29.537890 cs.tagset-20240422/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    65929 2024-04-22 03:00:09.000000 cs.tagset-20240422/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:00:29.533013 cs.tagset-20240422/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:00:29.533338 cs.tagset-20240422/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:00:29.534994 cs.tagset-20240422/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)   134320 2024-04-22 02:59:42.000000 cs.tagset-20240422/lib/python/cs/tagset.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:00:29.537196 cs.tagset-20240422/lib/python/cs.tagset.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    66713 2024-04-22 03:00:28.000000 cs.tagset-20240422/lib/python/cs.tagset.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-04-22 03:00:29.000000 cs.tagset-20240422/lib/python/cs.tagset.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 03:00:28.000000 cs.tagset-20240422/lib/python/cs.tagset.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      296 2024-04-22 03:00:29.000000 cs.tagset-20240422/lib/python/cs.tagset.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 03:00:29.000000 cs.tagset-20240422/lib/python/cs.tagset.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    67585 2024-04-22 03:00:27.000000 cs.tagset-20240422/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 03:00:29.538361 cs.tagset-20240422/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 04:37:43.781668 cs.tagset-20240422.1/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 04:37:11.000000 cs.tagset-20240422.1/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    66550 2024-04-22 04:37:43.780432 cs.tagset-20240422.1/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    65764 2024-04-22 04:37:21.000000 cs.tagset-20240422.1/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 04:37:43.773369 cs.tagset-20240422.1/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 04:37:43.773663 cs.tagset-20240422.1/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 04:37:43.776513 cs.tagset-20240422.1/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)   134333 2024-04-22 04:36:57.000000 cs.tagset-20240422.1/lib/python/cs/tagset.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 04:37:43.779938 cs.tagset-20240422.1/lib/python/cs.tagset.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    66550 2024-04-22 04:37:43.000000 cs.tagset-20240422.1/lib/python/cs.tagset.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-04-22 04:37:43.000000 cs.tagset-20240422.1/lib/python/cs.tagset.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 04:37:43.000000 cs.tagset-20240422.1/lib/python/cs.tagset.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      296 2024-04-22 04:37:43.000000 cs.tagset-20240422.1/lib/python/cs.tagset.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 04:37:43.000000 cs.tagset-20240422.1/lib/python/cs.tagset.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    67422 2024-04-22 04:37:41.000000 cs.tagset-20240422.1/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 04:37:43.781779 cs.tagset-20240422.1/setup.cfg
```

### Comparing `cs.tagset-20240422/PKG-INFO` & `cs.tagset-20240422.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.tagset
-Version: 20240422
+Version: 20240422.1
 Summary: Tags and sets of tags with __format__ support and optional ontology information.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,18 +15,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Tags and sets of tags
 with __format__ support and optional ontology information.
 
-*Latest release 20240422*:
-* New jsonable(obj) function to return a deep copy of `obj` which can be transcribed as JSON.
-* Tag.transcribe_value: pass jsonable(value) to the JSON encoder, drop special checks now done by jsonable().
-* Tag.__str__: do not catch TypeError any more, was embedding Python repr()s in .fstags files - now Tag.transcribe_value() does the correct thing where that is possible.
+*Latest release 20240422.1*:
+jsonable: convert pathlib.PurePath to str, hoping this isn't too open ended a can of worms.
 
 See `cs.fstags` for support for applying these to filesystem objects
 such as directories and files.
 
 See `cs.sqltags` for support for databases of entities with tags,
 not directly associated with filesystem objects.
 This is suited to both log entries (entities with no "name")
@@ -1614,14 +1612,17 @@
 {cmd} type_name + entity_name [tags...]
   Create type_name.entity_name and apply the tags.
 
 # Release Log
 
 
 
+*Release 20240422.1*:
+jsonable: convert pathlib.PurePath to str, hoping this isn't too open ended a can of worms.
+
 *Release 20240422*:
 * New jsonable(obj) function to return a deep copy of `obj` which can be transcribed as JSON.
 * Tag.transcribe_value: pass jsonable(value) to the JSON encoder, drop special checks now done by jsonable().
 * Tag.__str__: do not catch TypeError any more, was embedding Python repr()s in .fstags files - now Tag.transcribe_value() does the correct thing where that is possible.
 
 *Release 20240316*:
 Fixed release upload artifacts.
```

### Comparing `cs.tagset-20240422/README.md` & `cs.tagset-20240422.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Tags and sets of tags
 with __format__ support and optional ontology information.
 
-*Latest release 20240422*:
-* New jsonable(obj) function to return a deep copy of `obj` which can be transcribed as JSON.
-* Tag.transcribe_value: pass jsonable(value) to the JSON encoder, drop special checks now done by jsonable().
-* Tag.__str__: do not catch TypeError any more, was embedding Python repr()s in .fstags files - now Tag.transcribe_value() does the correct thing where that is possible.
+*Latest release 20240422.1*:
+jsonable: convert pathlib.PurePath to str, hoping this isn't too open ended a can of worms.
 
 See `cs.fstags` for support for applying these to filesystem objects
 such as directories and files.
 
 See `cs.sqltags` for support for databases of entities with tags,
 not directly associated with filesystem objects.
 This is suited to both log entries (entities with no "name")
@@ -1596,14 +1594,17 @@
 {cmd} type_name + entity_name [tags...]
   Create type_name.entity_name and apply the tags.
 
 # Release Log
 
 
 
+*Release 20240422.1*:
+jsonable: convert pathlib.PurePath to str, hoping this isn't too open ended a can of worms.
+
 *Release 20240422*:
 * New jsonable(obj) function to return a deep copy of `obj` which can be transcribed as JSON.
 * Tag.transcribe_value: pass jsonable(value) to the JSON encoder, drop special checks now done by jsonable().
 * Tag.__str__: do not catch TypeError any more, was embedding Python repr()s in .fstags files - now Tag.transcribe_value() does the correct thing where that is possible.
 
 *Release 20240316*:
 Fixed release upload artifacts.
```

### Comparing `cs.tagset-20240422/lib/python/cs/tagset.py` & `cs.tagset-20240422.1/lib/python/cs/tagset.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,14 +198,15 @@
 from getopt import GetoptError
 from json import JSONEncoder, JSONDecoder
 from json.decoder import JSONDecodeError
 import os
 from os.path import (
     dirname, isdir as isdirpath, isfile as isfilepath, join as joinpath
 )
+import pathlib
 from pprint import pformat
 import re
 import sys
 import time
 from typing import Mapping, Optional, Tuple, Union
 from uuid import UUID, uuid4
 
@@ -219,26 +220,26 @@
 from cs.fileutils import shortpath
 from cs.fs import FSPathBasedSingleton
 from cs.lex import (
     cropped_repr, cutprefix, cutsuffix, get_dotted_identifier, get_nonwhite,
     is_dotted_identifier, is_identifier, skipwhite, FormatableMixin,
     has_format_attributes, format_attribute, FStr, r, s
 )
-from cs.logutils import setup_logging, debug, warning, error, ifverbose
+from cs.logutils import setup_logging, warning, error, ifverbose
 from cs.mappings import (
     AttrableMappingMixin, IndexedMapping, PrefixedMappingProxy,
     RemappedMappingProxy
 )
 from cs.obj import SingletonMixin
 from cs.pfx import Pfx, pfx, pfx_call, pfx_method
 from cs.py3 import date_fromisoformat, datetime_fromisoformat
 from cs.resources import MultiOpenMixin
 from cs.threads import locked_property
 
-__version__ = '20240422'
+__version__ = '20240422.1'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -377,14 +378,16 @@
     return converted[id(obj)]
   except KeyError:
     pass
   t = type(obj)
   if t in (int, float, str, bool):
     # return unchanged - no need to record the convobj
     return obj
+  if isinstance(obj, pathlib.PurePath):
+    return str(obj)
   if isinstance(t, (set, tuple, list)):
     # convert to list
     converted[id(obj)] = convobj = []
     convobj.extend(jsonable(item, converted) for item in obj)
     return convobj
   # a mapping?
   try:
@@ -1063,15 +1066,14 @@
         This should return a value if `attr` is inferrable
         and raise `ValueError` if not.
 
         The default implementation returns the direct tag value for `attr`
         if present.
     '''
     if attr in self:
-      ##debug("returning direct tag value for %r", attr)
       return self[attr]
     raise ValueError("cannot infer value for %r" % (attr,))
 
   #############################################################################
   # Edit tags.
 
   def edit(self, editor=None, verbose=None, comments=()):
```

### Comparing `cs.tagset-20240422/lib/python/cs.tagset.egg-info/PKG-INFO` & `cs.tagset-20240422.1/lib/python/cs.tagset.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.tagset
-Version: 20240422
+Version: 20240422.1
 Summary: Tags and sets of tags with __format__ support and optional ontology information.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,18 +15,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Tags and sets of tags
 with __format__ support and optional ontology information.
 
-*Latest release 20240422*:
-* New jsonable(obj) function to return a deep copy of `obj` which can be transcribed as JSON.
-* Tag.transcribe_value: pass jsonable(value) to the JSON encoder, drop special checks now done by jsonable().
-* Tag.__str__: do not catch TypeError any more, was embedding Python repr()s in .fstags files - now Tag.transcribe_value() does the correct thing where that is possible.
+*Latest release 20240422.1*:
+jsonable: convert pathlib.PurePath to str, hoping this isn't too open ended a can of worms.
 
 See `cs.fstags` for support for applying these to filesystem objects
 such as directories and files.
 
 See `cs.sqltags` for support for databases of entities with tags,
 not directly associated with filesystem objects.
 This is suited to both log entries (entities with no "name")
@@ -1614,14 +1612,17 @@
 {cmd} type_name + entity_name [tags...]
   Create type_name.entity_name and apply the tags.
 
 # Release Log
 
 
 
+*Release 20240422.1*:
+jsonable: convert pathlib.PurePath to str, hoping this isn't too open ended a can of worms.
+
 *Release 20240422*:
 * New jsonable(obj) function to return a deep copy of `obj` which can be transcribed as JSON.
 * Tag.transcribe_value: pass jsonable(value) to the JSON encoder, drop special checks now done by jsonable().
 * Tag.__str__: do not catch TypeError any more, was embedding Python repr()s in .fstags files - now Tag.transcribe_value() does the correct thing where that is possible.
 
 *Release 20240316*:
 Fixed release upload artifacts.
```

### Comparing `cs.tagset-20240422/pyproject.toml` & `cs.tagset-20240422.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,31 +30,29 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240422"
+version = "20240422.1"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Tags and sets of tags
 with __format__ support and optional ontology information.
 
-*Latest release 20240422*:
-* New jsonable(obj) function to return a deep copy of `obj` which can be transcribed as JSON.
-* Tag.transcribe_value: pass jsonable(value) to the JSON encoder, drop special checks now done by jsonable().
-* Tag.__str__: do not catch TypeError any more, was embedding Python repr()s in .fstags files - now Tag.transcribe_value() does the correct thing where that is possible.
+*Latest release 20240422.1*:
+jsonable: convert pathlib.PurePath to str, hoping this isn't too open ended a can of worms.
 
 See `cs.fstags` for support for applying these to filesystem objects
 such as directories and files.
 
 See `cs.sqltags` for support for databases of entities with tags,
 not directly associated with filesystem objects.
 This is suited to both log entries (entities with no \"name\")
@@ -1642,14 +1640,17 @@
 {cmd} type_name + entity_name [tags...]
   Create type_name.entity_name and apply the tags.
 
 # Release Log
 
 
 
+*Release 20240422.1*:
+jsonable: convert pathlib.PurePath to str, hoping this isn't too open ended a can of worms.
+
 *Release 20240422*:
 * New jsonable(obj) function to return a deep copy of `obj` which can be transcribed as JSON.
 * Tag.transcribe_value: pass jsonable(value) to the JSON encoder, drop special checks now done by jsonable().
 * Tag.__str__: do not catch TypeError any more, was embedding Python repr()s in .fstags files - now Tag.transcribe_value() does the correct thing where that is possible.
 
 *Release 20240316*:
 Fixed release upload artifacts.
```

