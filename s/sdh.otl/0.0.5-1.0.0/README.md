# Comparing `tmp/sdh.otl-0.0.5.tar.gz` & `tmp/sdh_otl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdh.otl-0.0.5.tar", last modified: Sat Oct 31 11:48:37 2020, max compression
+gzip compressed data, was "sdh_otl-1.0.0.tar", last modified: Mon Apr 22 08:16:55 2024, max compression
```

## Comparing `sdh.otl-0.0.5.tar` & `sdh_otl-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 vic        (501) staff       (20)        0 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/
--rw-r--r--   0 vic        (501) staff       (20)       41 2014-07-19 22:05:24.000000 sdh.otl-0.0.5/MANIFEST.in
--rw-r--r--   0 vic        (501) staff       (20)      752 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/PKG-INFO
--rw-r--r--   0 vic        (501) staff       (20)     1530 2020-10-31 11:01:04.000000 sdh.otl-0.0.5/README.rst
--rw-r--r--   0 vic        (501) staff       (20)       38 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/setup.cfg
--rwxr-xr-x   0 vic        (501) staff       (20)     1023 2020-10-31 11:38:46.000000 sdh.otl-0.0.5/setup.py
-drwxr-xr-x   0 vic        (501) staff       (20)        0 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/src/
-drwxr-xr-x   0 vic        (501) staff       (20)        0 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/src/sdh/
--rw-r--r--   0 vic        (501) staff       (20)      168 2018-06-20 14:19:35.000000 sdh.otl-0.0.5/src/sdh/__init__.py
-drwxr-xr-x   0 vic        (501) staff       (20)        0 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/src/sdh/otl/
--rw-rw-r--   0 vic        (501) staff       (20)       35 2016-02-11 16:36:17.000000 sdh.otl-0.0.5/src/sdh/otl/__init__.py
--rw-rw-r--   0 vic        (501) staff       (20)     5250 2020-10-31 11:27:58.000000 sdh.otl-0.0.5/src/sdh/otl/generator.py
--rw-rw-r--   0 vic        (501) staff       (20)      144 2020-03-23 16:14:48.000000 sdh.otl-0.0.5/src/sdh/otl/urls.py
--rw-rw-r--   0 vic        (501) staff       (20)      409 2016-02-11 16:36:17.000000 sdh.otl-0.0.5/src/sdh/otl/views.py
-drwxr-xr-x   0 vic        (501) staff       (20)        0 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/src/sdh.otl.egg-info/
--rw-r--r--   0 vic        (501) staff       (20)      752 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/src/sdh.otl.egg-info/PKG-INFO
--rw-r--r--   0 vic        (501) staff       (20)      400 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/src/sdh.otl.egg-info/SOURCES.txt
--rw-r--r--   0 vic        (501) staff       (20)        1 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/src/sdh.otl.egg-info/dependency_links.txt
--rw-r--r--   0 vic        (501) staff       (20)        4 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/src/sdh.otl.egg-info/eager_resources.txt
--rw-r--r--   0 vic        (501) staff       (20)        4 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/src/sdh.otl.egg-info/namespace_packages.txt
--rw-r--r--   0 vic        (501) staff       (20)        1 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/src/sdh.otl.egg-info/not-zip-safe
--rw-r--r--   0 vic        (501) staff       (20)        4 2020-10-31 11:48:37.000000 sdh.otl-0.0.5/src/sdh.otl.egg-info/top_level.txt
+drwxr-xr-x   0 vic        (501) staff       (20)        0 2024-04-22 08:16:55.869349 sdh_otl-1.0.0/
+-rw-r--r--   0 vic        (501) staff       (20)     1290 2024-01-27 15:19:38.000000 sdh_otl-1.0.0/LICENSE
+-rw-r--r--   0 vic        (501) staff       (20)       41 2014-07-19 22:05:24.000000 sdh_otl-1.0.0/MANIFEST.in
+-rw-r--r--   0 vic        (501) staff       (20)     2527 2024-04-22 08:16:55.869164 sdh_otl-1.0.0/PKG-INFO
+-rw-r--r--   0 vic        (501) staff       (20)     1533 2024-04-22 08:12:37.000000 sdh_otl-1.0.0/README.rst
+-rw-r--r--   0 vic        (501) staff       (20)     1300 2024-04-22 08:12:37.000000 sdh_otl-1.0.0/pyproject.toml
+-rw-r--r--   0 vic        (501) staff       (20)       38 2024-04-22 08:16:55.869398 sdh_otl-1.0.0/setup.cfg
+drwxr-xr-x   0 vic        (501) staff       (20)        0 2024-04-22 08:16:55.866124 sdh_otl-1.0.0/src/
+drwxr-xr-x   0 vic        (501) staff       (20)        0 2024-04-22 08:16:55.867077 sdh_otl-1.0.0/src/sdh/
+-rw-r--r--   0 vic        (501) staff       (20)      168 2018-06-20 14:19:35.000000 sdh_otl-1.0.0/src/sdh/__init__.py
+drwxr-xr-x   0 vic        (501) staff       (20)        0 2024-04-22 08:16:55.868773 sdh_otl-1.0.0/src/sdh/otl/
+-rw-r--r--   0 vic        (501) staff       (20)       35 2016-02-11 16:36:17.000000 sdh_otl-1.0.0/src/sdh/otl/__init__.py
+-rw-r--r--   0 vic        (501) staff       (20)     5250 2020-10-31 11:27:58.000000 sdh_otl-1.0.0/src/sdh/otl/generator.py
+-rw-r--r--   0 vic        (501) staff       (20)      147 2024-04-22 08:15:22.000000 sdh_otl-1.0.0/src/sdh/otl/urls.py
+-rw-r--r--   0 vic        (501) staff       (20)      409 2016-02-11 16:36:17.000000 sdh_otl-1.0.0/src/sdh/otl/views.py
+drwxr-xr-x   0 vic        (501) staff       (20)        0 2024-04-22 08:16:55.868970 sdh_otl-1.0.0/src/sdh.otl.egg-info/
+-rw-r--r--   0 vic        (501) staff       (20)     2527 2024-04-22 08:16:55.000000 sdh_otl-1.0.0/src/sdh.otl.egg-info/PKG-INFO
+-rw-r--r--   0 vic        (501) staff       (20)      329 2024-04-22 08:16:55.000000 sdh_otl-1.0.0/src/sdh.otl.egg-info/SOURCES.txt
+-rw-r--r--   0 vic        (501) staff       (20)        1 2024-04-22 08:16:55.000000 sdh_otl-1.0.0/src/sdh.otl.egg-info/dependency_links.txt
+-rw-r--r--   0 vic        (501) staff       (20)       12 2024-04-22 08:16:55.000000 sdh_otl-1.0.0/src/sdh.otl.egg-info/requires.txt
+-rw-r--r--   0 vic        (501) staff       (20)        4 2024-04-22 08:16:55.000000 sdh_otl-1.0.0/src/sdh.otl.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sdh.otl-0.0.5/README.rst` & `sdh_otl-1.0.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 Example with callback and authorization:
 
 .. code-block:: python
 
 	from sdh.otl import OntTimeLink
 
 	def auth_callback(request, user_email):
-	    user = get_object_or_404(User,
+        user = get_object_or_404(User,
                                  email=user_email)
 	    login(request, user)
 
     @login_required
 	def password_restore(request):
 		....
```

### Comparing `sdh.otl-0.0.5/src/sdh/otl/generator.py` & `sdh_otl-1.0.0/src/sdh/otl/generator.py`

 * *Files identical despite different names*

