# Comparing `tmp/cs.py.doc-20240412.tar.gz` & `tmp/cs.py.doc-20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.py.doc-20240412.tar", last modified: Fri Apr 12 04:57:47 2024, max compression
+gzip compressed data, was "cs.py.doc-20240422.tar", last modified: Mon Apr 22 02:53:57 2024, max compression
```

## Comparing `cs.py.doc-20240412.tar` & `cs.py.doc-20240422.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.638689 cs.py.doc-20240412/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 04:57:40.000000 cs.py.doc-20240412/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     2683 2024-04-12 04:57:47.638310 cs.py.doc-20240412/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     1912 2024-04-12 04:57:42.000000 cs.py.doc-20240412/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.633975 cs.py.doc-20240412/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.634311 cs.py.doc-20240412/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.634428 cs.py.doc-20240412/lib/python/cs/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.637807 cs.py.doc-20240412/lib/python/cs/py/
--rw-r--r--   0 cameron    (501) cameron    (502)     6136 2024-04-12 04:57:25.000000 cs.py.doc-20240412/lib/python/cs/py/doc.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.637440 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     2683 2024-04-12 04:57:47.000000 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-04-12 04:57:47.000000 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 04:57:47.000000 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       80 2024-04-12 04:57:47.000000 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 04:57:47.000000 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     3105 2024-04-12 04:57:46.000000 cs.py.doc-20240412/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 04:57:47.638809 cs.py.doc-20240412/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:53:57.778276 cs.py.doc-20240422/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 02:53:48.000000 cs.py.doc-20240422/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2729 2024-04-22 02:53:57.777973 cs.py.doc-20240422/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1958 2024-04-22 02:53:51.000000 cs.py.doc-20240422/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:53:57.774064 cs.py.doc-20240422/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:53:57.774382 cs.py.doc-20240422/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:53:57.774496 cs.py.doc-20240422/lib/python/cs/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:53:57.777491 cs.py.doc-20240422/lib/python/cs/py/
+-rw-r--r--   0 cameron    (501) cameron    (502)     6231 2024-04-22 02:53:35.000000 cs.py.doc-20240422/lib/python/cs/py/doc.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:53:57.777062 cs.py.doc-20240422/lib/python/cs.py.doc.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2729 2024-04-22 02:53:57.000000 cs.py.doc-20240422/lib/python/cs.py.doc.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-04-22 02:53:57.000000 cs.py.doc-20240422/lib/python/cs.py.doc.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 02:53:57.000000 cs.py.doc-20240422/lib/python/cs.py.doc.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       80 2024-04-22 02:53:57.000000 cs.py.doc-20240422/lib/python/cs.py.doc.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 02:53:57.000000 cs.py.doc-20240422/lib/python/cs.py.doc.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3151 2024-04-22 02:53:56.000000 cs.py.doc-20240422/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 02:53:57.778391 cs.py.doc-20240422/setup.cfg
```

### Comparing `cs.py.doc-20240412/PKG-INFO` & `cs.py.doc-20240422/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.py.doc
-Version: 20240412
+Version: 20240422
 Summary: Create documentation from python modules and other objects.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,22 +14,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Create documentation from python modules and other objects.
 
-*Latest release 20240412*:
-module_doc: classes: MRO: suppress classes which are not immediate superclasses.
+*Latest release 20240422*:
+module_doc: only list things in __all__ if provided.
 
 ## Function `is_dunder(name)`
 
 Test whether a name is a dunder name (`__`*foo*`__`).
 
-## Function `module_doc(module, *, sort_key=<function <lambda> at 0x11128cf70>, filter_key=<function <lambda> at 0x11128d000>, method_names=None)`
+## Function `module_doc(module, *, sort_key=<function <lambda> at 0x102b29000>, filter_key=<function <lambda> at 0x102b29090>, method_names=None)`
 
 Fetch the docstrings from a module and assemble a MarkDown document.
 
 Parameters:
 * `module`: the module or module name to inspect
 * `sort_key`: optional key for sorting names in the documentation;
   default: `name`
@@ -48,14 +48,17 @@
 otherwise `''`.
 The chosen string is passed through `stripped_dedent` before return.
 
 # Release Log
 
 
 
+*Release 20240422*:
+module_doc: only list things in __all__ if provided.
+
 *Release 20240412*:
 module_doc: classes: MRO: suppress classes which are not immediate superclasses.
 
 *Release 20220311*:
 module_doc: class members no longer rendered as headings, too verbose.
 
 *Release 20210306*:
```

### Comparing `cs.py.doc-20240412/README.md` & `cs.py.doc-20240422/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Create documentation from python modules and other objects.
 
-*Latest release 20240412*:
-module_doc: classes: MRO: suppress classes which are not immediate superclasses.
+*Latest release 20240422*:
+module_doc: only list things in __all__ if provided.
 
 ## Function `is_dunder(name)`
 
 Test whether a name is a dunder name (`__`*foo*`__`).
 
-## Function `module_doc(module, *, sort_key=<function <lambda> at 0x11128cf70>, filter_key=<function <lambda> at 0x11128d000>, method_names=None)`
+## Function `module_doc(module, *, sort_key=<function <lambda> at 0x102b29000>, filter_key=<function <lambda> at 0x102b29090>, method_names=None)`
 
 Fetch the docstrings from a module and assemble a MarkDown document.
 
 Parameters:
 * `module`: the module or module name to inspect
 * `sort_key`: optional key for sorting names in the documentation;
   default: `name`
@@ -30,14 +30,17 @@
 otherwise `''`.
 The chosen string is passed through `stripped_dedent` before return.
 
 # Release Log
 
 
 
+*Release 20240422*:
+module_doc: only list things in __all__ if provided.
+
 *Release 20240412*:
 module_doc: classes: MRO: suppress classes which are not immediate superclasses.
 
 *Release 20220311*:
 module_doc: class members no longer rendered as headings, too verbose.
 
 *Release 20210306*:
```

### Comparing `cs.py.doc-20240412/lib/python/cs/py/doc.py` & `cs.py.doc-20240422/lib/python/cs/py/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 from itertools import chain
 from cs.lex import cutprefix, stripped_dedent
 from cs.logutils import warning
 from cs.pfx import Pfx
 from cs.py.modules import module_attributes
 
-__version__ = '20240412'
+__version__ = '20240422'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -51,16 +51,19 @@
         dunders, then other public names
   '''
   if isinstance(module, str):
     module_name = module
     with Pfx("import_module(%r)", module_name):
       module = importlib.import_module(module_name)
   full_doc = obj_docstring(module)
+  ALL = getattr(module, '__all__', None)
   for Mname, obj in sorted(module_attributes(module), key=sort_key):
     with Pfx(Mname):
+      if ALL and Mname not in ALL:
+        continue
       if not filter_key(Mname):
         continue
       obj_module = getmodule(obj)
       if obj_module is not module:
         # name imported from another module
         continue
       obj_doc = obj_docstring(obj) if obj_module else ''
@@ -118,15 +121,15 @@
                              '__getnewargs__', '__module__', '__new__',
                              '__repr__', '__weakref__'):
               continue
             # prune private names which are not dunder names
             if attr_name.startswith('_') and not is_dunder(attr_name):
               continue
           if attr_name not in direct_attrs:
-            print("  skip, not in direct_attrs", direct_attrs)
+            ##print("  skip, not in direct_attrs", direct_attrs)
             continue
           attr = getattr(obj, attr_name)
           attr_doc = obj_docstring(attr)
           if not attr_doc:
             continue
           # Class.name is a function, not a method
           if ismethod(attr) or isfunction(attr):
```

### Comparing `cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/PKG-INFO` & `cs.py.doc-20240422/lib/python/cs.py.doc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.py.doc
-Version: 20240412
+Version: 20240422
 Summary: Create documentation from python modules and other objects.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,22 +14,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Create documentation from python modules and other objects.
 
-*Latest release 20240412*:
-module_doc: classes: MRO: suppress classes which are not immediate superclasses.
+*Latest release 20240422*:
+module_doc: only list things in __all__ if provided.
 
 ## Function `is_dunder(name)`
 
 Test whether a name is a dunder name (`__`*foo*`__`).
 
-## Function `module_doc(module, *, sort_key=<function <lambda> at 0x11128cf70>, filter_key=<function <lambda> at 0x11128d000>, method_names=None)`
+## Function `module_doc(module, *, sort_key=<function <lambda> at 0x102b29000>, filter_key=<function <lambda> at 0x102b29090>, method_names=None)`
 
 Fetch the docstrings from a module and assemble a MarkDown document.
 
 Parameters:
 * `module`: the module or module name to inspect
 * `sort_key`: optional key for sorting names in the documentation;
   default: `name`
@@ -48,14 +48,17 @@
 otherwise `''`.
 The chosen string is passed through `stripped_dedent` before return.
 
 # Release Log
 
 
 
+*Release 20240422*:
+module_doc: only list things in __all__ if provided.
+
 *Release 20240412*:
 module_doc: classes: MRO: suppress classes which are not immediate superclasses.
 
 *Release 20220311*:
 module_doc: class members no longer rendered as headings, too verbose.
 
 *Release 20210306*:
```

### Comparing `cs.py.doc-20240412/pyproject.toml` & `cs.py.doc-20240422/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,34 +19,34 @@
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
 Create documentation from python modules and other objects.
 
-*Latest release 20240412*:
-module_doc: classes: MRO: suppress classes which are not immediate superclasses.
+*Latest release 20240422*:
+module_doc: only list things in __all__ if provided.
 
 ## Function `is_dunder(name)`
 
 Test whether a name is a dunder name (`__`*foo*`__`).
 
-## Function `module_doc(module, *, sort_key=<function <lambda> at 0x11128cf70>, filter_key=<function <lambda> at 0x11128d000>, method_names=None)`
+## Function `module_doc(module, *, sort_key=<function <lambda> at 0x102b29000>, filter_key=<function <lambda> at 0x102b29090>, method_names=None)`
 
 Fetch the docstrings from a module and assemble a MarkDown document.
 
 Parameters:
 * `module`: the module or module name to inspect
 * `sort_key`: optional key for sorting names in the documentation;
   default: `name`
@@ -65,14 +65,17 @@
 otherwise `''`.
 The chosen string is passed through `stripped_dedent` before return.
 
 # Release Log
 
 
 
+*Release 20240422*:
+module_doc: only list things in __all__ if provided.
+
 *Release 20240412*:
 module_doc: classes: MRO: suppress classes which are not immediate superclasses.
 
 *Release 20220311*:
 module_doc: class members no longer rendered as headings, too verbose.
 
 *Release 20210306*:
```

