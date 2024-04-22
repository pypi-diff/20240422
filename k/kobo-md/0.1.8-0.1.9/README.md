# Comparing `tmp/kobo-md-0.1.8.tar.gz` & `tmp/kobo-md-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kobo-md-0.1.8.tar", last modified: Thu Aug 24 08:04:22 2023, max compression
+gzip compressed data, was "kobo-md-0.1.9.tar", last modified: Thu Aug 24 08:08:26 2023, max compression
```

## Comparing `kobo-md-0.1.8.tar` & `kobo-md-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:04:22.273067 kobo-md-0.1.8/
--rw-r--r--   0 dwall      (501) staff       (20)     1086 2023-07-26 20:39:20.000000 kobo-md-0.1.8/LICENSE.txt
--rw-r--r--   0 dwall      (501) staff       (20)       46 2023-07-27 04:51:30.000000 kobo-md-0.1.8/MANIFEST.in
--rw-r--r--   0 dwall      (501) staff       (20)      802 2023-08-24 08:04:22.273120 kobo-md-0.1.8/PKG-INFO
--rw-r--r--   0 dwall      (501) staff       (20)      560 2023-07-27 09:20:37.000000 kobo-md-0.1.8/README.md
--rw-r--r--   0 dwall      (501) staff       (20)      106 2023-08-24 08:04:22.273408 kobo-md-0.1.8/setup.cfg
--rw-r--r--   0 dwall      (501) staff       (20)      862 2023-08-24 08:03:27.000000 kobo-md-0.1.8/setup.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:04:22.268522 kobo-md-0.1.8/src/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:04:22.270538 kobo-md-0.1.8/src/kobo/
--rw-r--r--   0 dwall      (501) staff       (20)       42 2023-07-27 05:04:42.000000 kobo-md-0.1.8/src/kobo/__init__.py
--rw-r--r--   0 dwall      (501) staff       (20)     2563 2023-08-24 08:01:43.000000 kobo-md-0.1.8/src/kobo/__main__.py
--rw-r--r--   0 dwall      (501) staff       (20)      791 2023-07-26 08:48:12.000000 kobo-md-0.1.8/src/kobo/helper.py
--rw-r--r--   0 dwall      (501) staff       (20)     6809 2023-08-24 08:01:43.000000 kobo-md-0.1.8/src/kobo/parser.py
--rw-r--r--   0 dwall      (501) staff       (20)      344 2023-07-26 07:12:37.000000 kobo-md-0.1.8/src/kobo/redirects.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:04:22.268467 kobo-md-0.1.8/src/kobo/resources/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:04:22.270810 kobo-md-0.1.8/src/kobo/resources/content/
--rw-r--r--   0 dwall      (501) staff       (20)       94 2023-07-26 08:39:44.000000 kobo-md-0.1.8/src/kobo/resources/content/index.md
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:04:22.268411 kobo-md-0.1.8/src/kobo/resources/static/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:04:22.271347 kobo-md-0.1.8/src/kobo/resources/static/css/
--rw-r--r--   0 dwall      (501) staff       (20)     2527 2023-07-26 07:01:14.000000 kobo-md-0.1.8/src/kobo/resources/static/css/grid.css
--rw-r--r--   0 dwall      (501) staff       (20)      608 2023-07-26 07:01:14.000000 kobo-md-0.1.8/src/kobo/resources/static/css/main.css
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:04:22.272309 kobo-md-0.1.8/src/kobo/resources/templates/
--rw-r--r--   0 dwall      (501) staff       (20)      296 2023-07-26 07:01:18.000000 kobo-md-0.1.8/src/kobo/resources/templates/404.html
--rw-r--r--   0 dwall      (501) staff       (20)      383 2023-07-26 07:01:18.000000 kobo-md-0.1.8/src/kobo/resources/templates/index-list.html
--rw-r--r--   0 dwall      (501) staff       (20)      381 2023-07-26 07:01:18.000000 kobo-md-0.1.8/src/kobo/resources/templates/index.html
--rw-r--r--   0 dwall      (501) staff       (20)      375 2023-07-26 07:01:18.000000 kobo-md-0.1.8/src/kobo/resources/templates/page.html
--rw-r--r--   0 dwall      (501) staff       (20)     3163 2023-07-27 09:20:37.000000 kobo-md-0.1.8/src/kobo/server.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:04:22.272968 kobo-md-0.1.8/src/kobo_md.egg-info/
--rw-r--r--   0 dwall      (501) staff       (20)      802 2023-08-24 08:04:22.000000 kobo-md-0.1.8/src/kobo_md.egg-info/PKG-INFO
--rw-r--r--   0 dwall      (501) staff       (20)      623 2023-08-24 08:04:22.000000 kobo-md-0.1.8/src/kobo_md.egg-info/SOURCES.txt
--rw-r--r--   0 dwall      (501) staff       (20)        1 2023-08-24 08:04:22.000000 kobo-md-0.1.8/src/kobo_md.egg-info/dependency_links.txt
--rw-r--r--   0 dwall      (501) staff       (20)       34 2023-08-24 08:04:22.000000 kobo-md-0.1.8/src/kobo_md.egg-info/requires.txt
--rw-r--r--   0 dwall      (501) staff       (20)        5 2023-08-24 08:04:22.000000 kobo-md-0.1.8/src/kobo_md.egg-info/top_level.txt
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:08:26.920233 kobo-md-0.1.9/
+-rw-r--r--   0 dwall      (501) staff       (20)     1086 2023-07-26 20:39:20.000000 kobo-md-0.1.9/LICENSE.txt
+-rw-r--r--   0 dwall      (501) staff       (20)       46 2023-07-27 04:51:30.000000 kobo-md-0.1.9/MANIFEST.in
+-rw-r--r--   0 dwall      (501) staff       (20)      802 2023-08-24 08:08:26.920291 kobo-md-0.1.9/PKG-INFO
+-rw-r--r--   0 dwall      (501) staff       (20)      560 2023-07-27 09:20:37.000000 kobo-md-0.1.9/README.md
+-rw-r--r--   0 dwall      (501) staff       (20)      106 2023-08-24 08:08:26.920576 kobo-md-0.1.9/setup.cfg
+-rw-r--r--   0 dwall      (501) staff       (20)      862 2023-08-24 08:07:30.000000 kobo-md-0.1.9/setup.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:08:26.915384 kobo-md-0.1.9/src/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:08:26.917577 kobo-md-0.1.9/src/kobo/
+-rw-r--r--   0 dwall      (501) staff       (20)       42 2023-07-27 05:04:42.000000 kobo-md-0.1.9/src/kobo/__init__.py
+-rw-r--r--   0 dwall      (501) staff       (20)     2563 2023-08-24 08:01:43.000000 kobo-md-0.1.9/src/kobo/__main__.py
+-rw-r--r--   0 dwall      (501) staff       (20)      791 2023-07-26 08:48:12.000000 kobo-md-0.1.9/src/kobo/helper.py
+-rw-r--r--   0 dwall      (501) staff       (20)     6811 2023-08-24 08:08:12.000000 kobo-md-0.1.9/src/kobo/parser.py
+-rw-r--r--   0 dwall      (501) staff       (20)      344 2023-07-26 07:12:37.000000 kobo-md-0.1.9/src/kobo/redirects.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:08:26.915328 kobo-md-0.1.9/src/kobo/resources/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:08:26.917828 kobo-md-0.1.9/src/kobo/resources/content/
+-rw-r--r--   0 dwall      (501) staff       (20)       94 2023-07-26 08:39:44.000000 kobo-md-0.1.9/src/kobo/resources/content/index.md
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:08:26.915265 kobo-md-0.1.9/src/kobo/resources/static/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:08:26.918495 kobo-md-0.1.9/src/kobo/resources/static/css/
+-rw-r--r--   0 dwall      (501) staff       (20)     2527 2023-07-26 07:01:14.000000 kobo-md-0.1.9/src/kobo/resources/static/css/grid.css
+-rw-r--r--   0 dwall      (501) staff       (20)      608 2023-07-26 07:01:14.000000 kobo-md-0.1.9/src/kobo/resources/static/css/main.css
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:08:26.919515 kobo-md-0.1.9/src/kobo/resources/templates/
+-rw-r--r--   0 dwall      (501) staff       (20)      296 2023-07-26 07:01:18.000000 kobo-md-0.1.9/src/kobo/resources/templates/404.html
+-rw-r--r--   0 dwall      (501) staff       (20)      383 2023-07-26 07:01:18.000000 kobo-md-0.1.9/src/kobo/resources/templates/index-list.html
+-rw-r--r--   0 dwall      (501) staff       (20)      381 2023-07-26 07:01:18.000000 kobo-md-0.1.9/src/kobo/resources/templates/index.html
+-rw-r--r--   0 dwall      (501) staff       (20)      375 2023-07-26 07:01:18.000000 kobo-md-0.1.9/src/kobo/resources/templates/page.html
+-rw-r--r--   0 dwall      (501) staff       (20)     3163 2023-07-27 09:20:37.000000 kobo-md-0.1.9/src/kobo/server.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-08-24 08:08:26.920147 kobo-md-0.1.9/src/kobo_md.egg-info/
+-rw-r--r--   0 dwall      (501) staff       (20)      802 2023-08-24 08:08:26.000000 kobo-md-0.1.9/src/kobo_md.egg-info/PKG-INFO
+-rw-r--r--   0 dwall      (501) staff       (20)      623 2023-08-24 08:08:26.000000 kobo-md-0.1.9/src/kobo_md.egg-info/SOURCES.txt
+-rw-r--r--   0 dwall      (501) staff       (20)        1 2023-08-24 08:08:26.000000 kobo-md-0.1.9/src/kobo_md.egg-info/dependency_links.txt
+-rw-r--r--   0 dwall      (501) staff       (20)       34 2023-08-24 08:08:26.000000 kobo-md-0.1.9/src/kobo_md.egg-info/requires.txt
+-rw-r--r--   0 dwall      (501) staff       (20)        5 2023-08-24 08:08:26.000000 kobo-md-0.1.9/src/kobo_md.egg-info/top_level.txt
```

### Comparing `kobo-md-0.1.8/LICENSE.txt` & `kobo-md-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.8/PKG-INFO` & `kobo-md-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobo-md
-Version: 0.1.8
+Version: 0.1.9
 Summary: Markdown Compiler + Server
 Home-page: https://github.com/dwLG00/kobo/
 Author: Dylan Wallace
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kobo-md-0.1.8/README.md` & `kobo-md-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.8/setup.py` & `kobo-md-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 import setuptools
 import os
 import sys
 import pathlib
 
 package_dir = {'': 'src'}
```

### Comparing `kobo-md-0.1.8/src/kobo/__main__.py` & `kobo-md-0.1.9/src/kobo/__main__.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.8/src/kobo/helper.py` & `kobo-md-0.1.9/src/kobo/helper.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.8/src/kobo/parser.py` & `kobo-md-0.1.9/src/kobo/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         write_tree = []
     for root, dirs, files in os.walk(contents_path):
         root_routes = []
         for file in files:
             if file == 'index-blurb.md':
                 continue
             if file.endswith('.md'): # only parse mds!
-                if verbose: print('Found ``' % os.path.join(root, file))
+                if verbose: print('Found `%s`' % os.path.join(root, file))
                 (html, title, isdraft, route, template) = parse(os.path.join(root, file))
                 html_path = os.path.join(root, file).replace('.md', '.html')
 
                 if not route:
                     if file == 'index.md': # index -> parent dir should be the endpoint
                         route = os.path.relpath(root, contents_path)
                         if route == '.':
```

### Comparing `kobo-md-0.1.8/src/kobo/resources/static/css/grid.css` & `kobo-md-0.1.9/src/kobo/resources/static/css/grid.css`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.8/src/kobo/resources/static/css/main.css` & `kobo-md-0.1.9/src/kobo/resources/static/css/main.css`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.8/src/kobo/server.py` & `kobo-md-0.1.9/src/kobo/server.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.8/src/kobo_md.egg-info/PKG-INFO` & `kobo-md-0.1.9/src/kobo_md.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobo-md
-Version: 0.1.8
+Version: 0.1.9
 Summary: Markdown Compiler + Server
 Home-page: https://github.com/dwLG00/kobo/
 Author: Dylan Wallace
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kobo-md-0.1.8/src/kobo_md.egg-info/SOURCES.txt` & `kobo-md-0.1.9/src/kobo_md.egg-info/SOURCES.txt`

 * *Files identical despite different names*

