# Comparing `tmp/cs.fs-20240412.tar.gz` & `tmp/cs.fs-20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.fs-20240412.tar", last modified: Fri Apr 12 05:22:15 2024, max compression
+gzip compressed data, was "cs.fs-20240422.tar", last modified: Mon Apr 22 02:50:34 2024, max compression
```

## Comparing `cs.fs-20240412.tar` & `cs.fs-20240422.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:22:15.279561 cs.fs-20240412/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:22:03.000000 cs.fs-20240412/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     7320 2024-04-12 05:22:15.279341 cs.fs-20240412/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     6506 2024-04-12 05:22:07.000000 cs.fs-20240412/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:22:15.276446 cs.fs-20240412/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:22:15.276669 cs.fs-20240412/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:22:15.277697 cs.fs-20240412/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    12685 2024-04-12 05:21:50.000000 cs.fs-20240412/lib/python/cs/fs.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:22:15.279002 cs.fs-20240412/lib/python/cs.fs.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     7320 2024-04-12 05:22:14.000000 cs.fs-20240412/lib/python/cs.fs.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      255 2024-04-12 05:22:15.000000 cs.fs-20240412/lib/python/cs.fs.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:22:14.000000 cs.fs-20240412/lib/python/cs.fs.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       62 2024-04-12 05:22:15.000000 cs.fs-20240412/lib/python/cs.fs.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:22:15.000000 cs.fs-20240412/lib/python/cs.fs.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     7724 2024-04-12 05:22:13.000000 cs.fs-20240412/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:22:15.279646 cs.fs-20240412/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:50:34.952857 cs.fs-20240422/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 02:50:19.000000 cs.fs-20240422/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     8337 2024-04-22 02:50:34.952527 cs.fs-20240422/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     7523 2024-04-22 02:50:24.000000 cs.fs-20240422/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:50:34.947802 cs.fs-20240422/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:50:34.948092 cs.fs-20240422/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:50:34.949849 cs.fs-20240422/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    14257 2024-04-22 02:50:00.000000 cs.fs-20240422/lib/python/cs/fs.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:50:34.952052 cs.fs-20240422/lib/python/cs.fs.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     8337 2024-04-22 02:50:34.000000 cs.fs-20240422/lib/python/cs.fs.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      255 2024-04-22 02:50:34.000000 cs.fs-20240422/lib/python/cs.fs.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 02:50:34.000000 cs.fs-20240422/lib/python/cs.fs.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       62 2024-04-22 02:50:34.000000 cs.fs-20240422/lib/python/cs.fs.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 02:50:34.000000 cs.fs-20240422/lib/python/cs.fs.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     8741 2024-04-22 02:50:33.000000 cs.fs-20240422/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 02:50:34.952961 cs.fs-20240422/setup.cfg
```

### Comparing `cs.fs-20240412/PKG-INFO` & `cs.fs-20240422/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-Metadata-Version: 2.1
-Name: cs.fs
-Version: 20240412
-Summary: Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240412*:
-HasFSPath: explain that the __init__ is optional in the docstring.
+*Latest release 20240422*:
+New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -113,26 +95,50 @@
 Parameters:
 * `dirpath`: the required directory path
 * `mode`: the permissions mode, default `0o777`
 * `log`: log `makedirs` or `mkdir` call
 * `use_makedirs`: optional creation mode, default `False`;
   if true, use `os.makedirs`, otherwise `os.mkdir`
 
-## Function `rpaths(dirpath='.', *, only_suffixes=None, skip_suffixes=None, sort_paths=False)`
+## Function `rpaths(dirpath='.', **scan_kw)`
+
+A shim for `scandirtree` to yield relative file paths from a directory.
+
+Parameters:
+* `dirpath`: optional top directory, default `'.'`
+
+Other keyword arguments are passed to `scandirtree`.
+
+## Function `scandirpaths(dirpath='.', **scan_kw)`
 
-Yield relative file paths from a directory.
+A shim for `scandirtree` to yield filesystem paths from a directory.
 
 Parameters:
 * `dirpath`: optional top directory, default `'.'`
-* `only_suffixes`: optional iterable of suffixes of interest;
-  if provided only files ending in these suffixes will be yielded
-* `skip_suffixes`: optional iterable if suffixes to ignore;
-  if provided files ending in these suffixes will not be yielded
-* `sort_paths`: optional flag specifying that filenames should be sorted,
-  default `False`
+
+Other keyword arguments are passed to `scandirtree`.
+
+## Function `scandirtree(dirpath='.', *, include_dirs=False, name_selector=None, only_suffixes=None, skip_suffixes=None, sort_names=False, follow_symlinks=False, recurse=True)`
+
+Generator to recurse over `dirpath`, yielding `(is_dir,subpath)`
+for all selected subpaths.
+
+Parameters:
+* `dirpath`: the directory to scan, default `'.'`
+* `include_dirs`: if true yield directories; default `False`
+* `name_selector`: optional callable to select particular names;
+  the default is to select names no starting with a dot (`'.'`)
+* `only_suffixes`: if supplied, skip entries whose extension
+  is not in `only_suffixes`
+* `skip_suffixes`: if supplied, skip entries whose extension
+  is in `skip_suffixes`
+* `sort_names`: option flag, default `False`; yield entires
+  in lexical order if true
+* `follow_symlinks`: optional flag, default `False`; passed to `scandir`
+* `recurse`: optional flag, default `True`; if true, recurse into subdrectories
 
 ## Function `shortpath(path, prefixes=None)`
 
 Return `path` with the first matching leading prefix replaced.
 
 Parameters:
 * `environ`: environment mapping if not os.environ
@@ -158,14 +164,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240422*:
+New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
+
 *Release 20240412*:
 HasFSPath: explain that the __init__ is optional in the docstring.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
@@ -205,8 +214,7 @@
 * Add longpath and shortpath from cs.fileutils.
 * New is_clean_subpath(subpath).
 * New needdir(path).
 * New fnmatchdir(dirpath,fnglob) pulled out from HasFSPath.fnmatch(fnglob).
 
 *Release 20220327*:
 New module cs.fs to contain more filesystem focussed functions than cs.fileutils, which is feeling a bit bloated.
-
```

### Comparing `cs.fs-20240412/README.md` & `cs.fs-20240422/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,47 @@
+[project]
+name = "cs.fs"
+description = "Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long."
+authors = [
+    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
+]
+keywords = [
+    "python2",
+    "python3",
+]
+dependencies = [
+    "cs.deco>=20240412",
+    "cs.obj>=20220918",
+    "cs.pfx>=20240412",
+    "icontract",
+]
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+]
+version = "20240422"
+
+[project.license]
+text = "GNU General Public License v3 or later (GPLv3+)"
+
+[project.urls]
+URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
+
+[project.readme]
+text = """
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240412*:
-HasFSPath: explain that the __init__ is optional in the docstring.
+*Latest release 20240422*:
+New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -95,37 +130,61 @@
 Parameters:
 * `dirpath`: the required directory path
 * `mode`: the permissions mode, default `0o777`
 * `log`: log `makedirs` or `mkdir` call
 * `use_makedirs`: optional creation mode, default `False`;
   if true, use `os.makedirs`, otherwise `os.mkdir`
 
-## Function `rpaths(dirpath='.', *, only_suffixes=None, skip_suffixes=None, sort_paths=False)`
+## Function `rpaths(dirpath='.', **scan_kw)`
+
+A shim for `scandirtree` to yield relative file paths from a directory.
+
+Parameters:
+* `dirpath`: optional top directory, default `'.'`
+
+Other keyword arguments are passed to `scandirtree`.
 
-Yield relative file paths from a directory.
+## Function `scandirpaths(dirpath='.', **scan_kw)`
+
+A shim for `scandirtree` to yield filesystem paths from a directory.
 
 Parameters:
 * `dirpath`: optional top directory, default `'.'`
-* `only_suffixes`: optional iterable of suffixes of interest;
-  if provided only files ending in these suffixes will be yielded
-* `skip_suffixes`: optional iterable if suffixes to ignore;
-  if provided files ending in these suffixes will not be yielded
-* `sort_paths`: optional flag specifying that filenames should be sorted,
-  default `False`
+
+Other keyword arguments are passed to `scandirtree`.
+
+## Function `scandirtree(dirpath='.', *, include_dirs=False, name_selector=None, only_suffixes=None, skip_suffixes=None, sort_names=False, follow_symlinks=False, recurse=True)`
+
+Generator to recurse over `dirpath`, yielding `(is_dir,subpath)`
+for all selected subpaths.
+
+Parameters:
+* `dirpath`: the directory to scan, default `'.'`
+* `include_dirs`: if true yield directories; default `False`
+* `name_selector`: optional callable to select particular names;
+  the default is to select names no starting with a dot (`'.'`)
+* `only_suffixes`: if supplied, skip entries whose extension
+  is not in `only_suffixes`
+* `skip_suffixes`: if supplied, skip entries whose extension
+  is in `skip_suffixes`
+* `sort_names`: option flag, default `False`; yield entires
+  in lexical order if true
+* `follow_symlinks`: optional flag, default `False`; passed to `scandir`
+* `recurse`: optional flag, default `True`; if true, recurse into subdrectories
 
 ## Function `shortpath(path, prefixes=None)`
 
 Return `path` with the first matching leading prefix replaced.
 
 Parameters:
 * `environ`: environment mapping if not os.environ
 * `prefixes`: optional iterable of `(prefix,subst)` to consider for replacement;
   each `prefix` is subject to environment variable
   substitution before consideration
-  The default considers "$HOME/" for replacement by "~/".
+  The default considers \"$HOME/\" for replacement by \"~/\".
 
 ## Function `validate_rpath(rpath: str)`
 
 Test that `rpath` is a clean relative path with no funny business;
 raise `ValueError` if the test fails.
 
 Tests:
@@ -140,14 +199,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240422*:
+New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
+
 *Release 20240412*:
 HasFSPath: explain that the __init__ is optional in the docstring.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
@@ -186,8 +248,25 @@
 * New HasFSPath and FSPathBasedSingleton.
 * Add longpath and shortpath from cs.fileutils.
 * New is_clean_subpath(subpath).
 * New needdir(path).
 * New fnmatchdir(dirpath,fnglob) pulled out from HasFSPath.fnmatch(fnglob).
 
 *Release 20220327*:
-New module cs.fs to contain more filesystem focussed functions than cs.fileutils, which is feeling a bit bloated.
+New module cs.fs to contain more filesystem focussed functions than cs.fileutils, which is feeling a bit bloated."""
+content-type = "text/markdown"
+
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+    "setuptools >= 61.2",
+    "trove-classifiers",
+    "wheel",
+]
+
+[tool.setuptools]
+py-modules = [
+    "cs.fs",
+]
+
+[tool.setuptools.package-dir]
+"" = "lib/python"
```

### Comparing `cs.fs-20240412/lib/python/cs/fs.py` & `cs.fs-20240422/lib/python/cs/fs.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,26 +16,27 @@
     expandvars,
     isabs as isabspath,
     isdir as isdirpath,
     join as joinpath,
     normpath,
     realpath,
     relpath,
+    splitext,
 )
 from tempfile import TemporaryDirectory
 from threading import Lock
 from typing import Any, Callable, Optional, Union
 
 from icontract import require
 
 from cs.deco import decorator
 from cs.obj import SingletonMixin
 from cs.pfx import pfx, pfx_call
 
-__version__ = '20240412'
+__version__ = '20240422'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -117,42 +118,93 @@
       if remove_placeholder and isdirpath(dirpath):
         pfx_rmdir(dirpath)
       raise
     return result
 
   return atomic_directory_wrapper
 
-def rpaths(
-    dirpath='.', *, only_suffixes=None, skip_suffixes=None, sort_paths=False
+@pfx
+def scandirtree(
+    dirpath='.',
+    *,
+    include_dirs=False,
+    name_selector=None,
+    only_suffixes=None,
+    skip_suffixes=None,
+    sort_names=False,
+    follow_symlinks=False,
+    recurse=True,
 ):
-  ''' Yield relative file paths from a directory.
+  ''' Generator to recurse over `dirpath`, yielding `(is_dir,subpath)`
+      for all selected subpaths.
 
       Parameters:
-      * `dirpath`: optional top directory, default `'.'`
-      * `only_suffixes`: optional iterable of suffixes of interest;
-        if provided only files ending in these suffixes will be yielded
-      * `skip_suffixes`: optional iterable if suffixes to ignore;
-        if provided files ending in these suffixes will not be yielded
-      * `sort_paths`: optional flag specifying that filenames should be sorted,
-        default `False`
-  '''
-  if only_suffixes is not None:
-    only_suffixes = tuple(only_suffixes)
-  if skip_suffixes is not None:
-    skip_suffixes = tuple(skip_suffixes)
-  for subpath, subdirnames, filenames in os.walk(dirpath):
-    if sort_paths:
-      subdirnames[:] = sorted(subdirnames)
-      filenames = sorted(filenames)
-    for filename in filenames:
-      if skip_suffixes is not None and filename.endswith(skip_suffixes):
-        continue
-      if only_suffixes is not None and not filename.endswith(only_suffixes):
+      * `dirpath`: the directory to scan, default `'.'`
+      * `include_dirs`: if true yield directories; default `False`
+      * `name_selector`: optional callable to select particular names;
+        the default is to select names no starting with a dot (`'.'`)
+      * `only_suffixes`: if supplied, skip entries whose extension
+        is not in `only_suffixes`
+      * `skip_suffixes`: if supplied, skip entries whose extension
+        is in `skip_suffixes`
+      * `sort_names`: option flag, default `False`; yield entires
+        in lexical order if true
+      * `follow_symlinks`: optional flag, default `False`; passed to `scandir`
+      * `recurse`: optional flag, default `True`; if true, recurse into subdrectories
+  '''
+  if name_selector is None:
+    name_selector = lambda name: name and not name.startswith('.')
+  pending = [dirpath]
+  while pending:
+    path = pending.pop(0)
+    try:
+      dirents = pfx_call(os.scandir, path)
+    except NotADirectoryError:
+      yield False, path
+      continue
+    if include_dirs:
+      yield True, path
+    if sort_names:
+      dirents = sorted(dirents, key=lambda entry: entry.name)
+    for entry in dirents:
+      if recurse and entry.is_dir(follow_symlinks=follow_symlinks):
+        pending.append(entry.path)
+      name = entry.name
+      if not name_selector(name):
         continue
-      yield relpath(joinpath(subpath, filename), dirpath)
+      if only_suffixes or skip_suffixes:
+        base, ext = splitext(name)
+        if only_suffixes and ext[1:] not in only_suffixes:
+          continue
+        if skip_suffixes and ext[1:] in skip_suffixes:
+          continue
+      if include_dirs or not entry.is_dir(follow_symlinks=follow_symlinks):
+        yield False, entry.path
+
+def scandirpaths(dirpath='.', **scan_kw):
+  ''' A shim for `scandirtree` to yield filesystem paths from a directory.
+
+      Parameters:
+      * `dirpath`: optional top directory, default `'.'`
+
+      Other keyword arguments are passed to `scandirtree`.
+  '''
+  for _, fspath in scandirtree(dirpath, **scan_kw):
+    yield fspath
+
+def rpaths(dirpath='.', **scan_kw):
+  ''' A shim for `scandirtree` to yield relative file paths from a directory.
+
+      Parameters:
+      * `dirpath`: optional top directory, default `'.'`
+
+      Other keyword arguments are passed to `scandirtree`.
+  '''
+  for fspath in scandirpaths(dirpath, **scan_kw):
+    yield relpath(fspath, dirpath)
 
 def fnmatchdir(dirpath, fnglob):
   ''' Return a list of the names in `dirpath` matching the glob `fnglob`.
   '''
   return fnfilter(pfx_listdir(dirpath), fnglob)
 
 # pylint: disable=too-few-public-methods
@@ -174,22 +226,24 @@
     ''' The short version of `self.fspath`.
     '''
     try:
       return shortpath(self.fspath)
     except AttributeError:
       return "<no-fspath>"
 
-  @require(lambda subpaths: len(subpaths) > 0)
-  @require(lambda subpaths: not any(map(isabspath, subpaths)))
   def pathto(self, *subpaths):
     ''' The full path to `subpaths`, comprising a relative path
         below `self.fspath`.
         This is a shim for `os.path.join` which requires that all
         the `subpaths` be relative paths.
     '''
+    if not subpaths:
+      raise ValueError('missing subpaths')
+    if any(map(isabspath, subpaths)):
+      raise ValueError('all subpaths must be relative paths')
     return joinpath(self.fspath, *subpaths)
 
   def fnmatch(self, fnglob):
     ''' Return a list of the names in `self.fspath` matching the glob `fnglob`.
     '''
     return fnmatchdir(self.fspath, fnglob)
```

### Comparing `cs.fs-20240412/lib/python/cs.fs.egg-info/PKG-INFO` & `cs.fs-20240422/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.fs
-Version: 20240412
+Version: 20240422
 Summary: Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,16 +15,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240412*:
-HasFSPath: explain that the __init__ is optional in the docstring.
+*Latest release 20240422*:
+New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -113,26 +113,50 @@
 Parameters:
 * `dirpath`: the required directory path
 * `mode`: the permissions mode, default `0o777`
 * `log`: log `makedirs` or `mkdir` call
 * `use_makedirs`: optional creation mode, default `False`;
   if true, use `os.makedirs`, otherwise `os.mkdir`
 
-## Function `rpaths(dirpath='.', *, only_suffixes=None, skip_suffixes=None, sort_paths=False)`
+## Function `rpaths(dirpath='.', **scan_kw)`
+
+A shim for `scandirtree` to yield relative file paths from a directory.
+
+Parameters:
+* `dirpath`: optional top directory, default `'.'`
+
+Other keyword arguments are passed to `scandirtree`.
+
+## Function `scandirpaths(dirpath='.', **scan_kw)`
 
-Yield relative file paths from a directory.
+A shim for `scandirtree` to yield filesystem paths from a directory.
 
 Parameters:
 * `dirpath`: optional top directory, default `'.'`
-* `only_suffixes`: optional iterable of suffixes of interest;
-  if provided only files ending in these suffixes will be yielded
-* `skip_suffixes`: optional iterable if suffixes to ignore;
-  if provided files ending in these suffixes will not be yielded
-* `sort_paths`: optional flag specifying that filenames should be sorted,
-  default `False`
+
+Other keyword arguments are passed to `scandirtree`.
+
+## Function `scandirtree(dirpath='.', *, include_dirs=False, name_selector=None, only_suffixes=None, skip_suffixes=None, sort_names=False, follow_symlinks=False, recurse=True)`
+
+Generator to recurse over `dirpath`, yielding `(is_dir,subpath)`
+for all selected subpaths.
+
+Parameters:
+* `dirpath`: the directory to scan, default `'.'`
+* `include_dirs`: if true yield directories; default `False`
+* `name_selector`: optional callable to select particular names;
+  the default is to select names no starting with a dot (`'.'`)
+* `only_suffixes`: if supplied, skip entries whose extension
+  is not in `only_suffixes`
+* `skip_suffixes`: if supplied, skip entries whose extension
+  is in `skip_suffixes`
+* `sort_names`: option flag, default `False`; yield entires
+  in lexical order if true
+* `follow_symlinks`: optional flag, default `False`; passed to `scandir`
+* `recurse`: optional flag, default `True`; if true, recurse into subdrectories
 
 ## Function `shortpath(path, prefixes=None)`
 
 Return `path` with the first matching leading prefix replaced.
 
 Parameters:
 * `environ`: environment mapping if not os.environ
@@ -158,14 +182,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240422*:
+New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
+
 *Release 20240412*:
 HasFSPath: explain that the __init__ is optional in the docstring.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
```

### Comparing `cs.fs-20240412/pyproject.toml` & `cs.fs-20240422/lib/python/cs.fs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,30 @@
-[project]
-name = "cs.fs"
-description = "Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long."
-authors = [
-    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
-]
-keywords = [
-    "python2",
-    "python3",
-]
-dependencies = [
-    "cs.deco>=20240412",
-    "cs.obj>=20220918",
-    "cs.pfx>=20240412",
-    "icontract",
-]
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
-version = "20240412"
+Metadata-Version: 2.1
+Name: cs.fs
+Version: 20240422
+Summary: Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
 
-[project.license]
-text = "GNU General Public License v3 or later (GPLv3+)"
-
-[project.urls]
-URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
-
-[project.readme]
-text = """
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240412*:
-HasFSPath: explain that the __init__ is optional in the docstring.
+*Latest release 20240422*:
+New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -130,37 +113,61 @@
 Parameters:
 * `dirpath`: the required directory path
 * `mode`: the permissions mode, default `0o777`
 * `log`: log `makedirs` or `mkdir` call
 * `use_makedirs`: optional creation mode, default `False`;
   if true, use `os.makedirs`, otherwise `os.mkdir`
 
-## Function `rpaths(dirpath='.', *, only_suffixes=None, skip_suffixes=None, sort_paths=False)`
+## Function `rpaths(dirpath='.', **scan_kw)`
+
+A shim for `scandirtree` to yield relative file paths from a directory.
+
+Parameters:
+* `dirpath`: optional top directory, default `'.'`
+
+Other keyword arguments are passed to `scandirtree`.
 
-Yield relative file paths from a directory.
+## Function `scandirpaths(dirpath='.', **scan_kw)`
+
+A shim for `scandirtree` to yield filesystem paths from a directory.
 
 Parameters:
 * `dirpath`: optional top directory, default `'.'`
-* `only_suffixes`: optional iterable of suffixes of interest;
-  if provided only files ending in these suffixes will be yielded
-* `skip_suffixes`: optional iterable if suffixes to ignore;
-  if provided files ending in these suffixes will not be yielded
-* `sort_paths`: optional flag specifying that filenames should be sorted,
-  default `False`
+
+Other keyword arguments are passed to `scandirtree`.
+
+## Function `scandirtree(dirpath='.', *, include_dirs=False, name_selector=None, only_suffixes=None, skip_suffixes=None, sort_names=False, follow_symlinks=False, recurse=True)`
+
+Generator to recurse over `dirpath`, yielding `(is_dir,subpath)`
+for all selected subpaths.
+
+Parameters:
+* `dirpath`: the directory to scan, default `'.'`
+* `include_dirs`: if true yield directories; default `False`
+* `name_selector`: optional callable to select particular names;
+  the default is to select names no starting with a dot (`'.'`)
+* `only_suffixes`: if supplied, skip entries whose extension
+  is not in `only_suffixes`
+* `skip_suffixes`: if supplied, skip entries whose extension
+  is in `skip_suffixes`
+* `sort_names`: option flag, default `False`; yield entires
+  in lexical order if true
+* `follow_symlinks`: optional flag, default `False`; passed to `scandir`
+* `recurse`: optional flag, default `True`; if true, recurse into subdrectories
 
 ## Function `shortpath(path, prefixes=None)`
 
 Return `path` with the first matching leading prefix replaced.
 
 Parameters:
 * `environ`: environment mapping if not os.environ
 * `prefixes`: optional iterable of `(prefix,subst)` to consider for replacement;
   each `prefix` is subject to environment variable
   substitution before consideration
-  The default considers \"$HOME/\" for replacement by \"~/\".
+  The default considers "$HOME/" for replacement by "~/".
 
 ## Function `validate_rpath(rpath: str)`
 
 Test that `rpath` is a clean relative path with no funny business;
 raise `ValueError` if the test fails.
 
 Tests:
@@ -175,14 +182,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240422*:
+New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
+
 *Release 20240412*:
 HasFSPath: explain that the __init__ is optional in the docstring.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
@@ -221,25 +231,9 @@
 * New HasFSPath and FSPathBasedSingleton.
 * Add longpath and shortpath from cs.fileutils.
 * New is_clean_subpath(subpath).
 * New needdir(path).
 * New fnmatchdir(dirpath,fnglob) pulled out from HasFSPath.fnmatch(fnglob).
 
 *Release 20220327*:
-New module cs.fs to contain more filesystem focussed functions than cs.fileutils, which is feeling a bit bloated."""
-content-type = "text/markdown"
-
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = [
-    "setuptools >= 61.2",
-    "trove-classifiers",
-    "wheel",
-]
-
-[tool.setuptools]
-py-modules = [
-    "cs.fs",
-]
+New module cs.fs to contain more filesystem focussed functions than cs.fileutils, which is feeling a bit bloated.
 
-[tool.setuptools.package-dir]
-"" = "lib/python"
```

