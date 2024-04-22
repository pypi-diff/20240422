# Comparing `tmp/django_img_optimizer-0.1.tar.gz` & `tmp/django_img_optimizer-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_img_optimizer-0.1.tar", last modified: Mon Apr 22 00:11:26 2024, max compression
+gzip compressed data, was "django_img_optimizer-1.0.tar", last modified: Mon Apr 22 00:16:43 2024, max compression
```

## Comparing `django_img_optimizer-0.1.tar` & `django_img_optimizer-1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:11:26.879919 django_img_optimizer-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-22 00:11:07.000000 django_img_optimizer-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-22 00:11:26.879919 django_img_optimizer-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-22 00:11:07.000000 django_img_optimizer-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:11:26.875919 django_img_optimizer-0.1/django_img_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 00:11:07.000000 django_img_optimizer-0.1/django_img_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-22 00:11:07.000000 django_img_optimizer-0.1/django_img_optimizer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:11:26.875919 django_img_optimizer-0.1/django_img_optimizer/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 00:11:07.000000 django_img_optimizer-0.1/django_img_optimizer/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:11:26.875919 django_img_optimizer-0.1/django_img_optimizer/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 00:11:07.000000 django_img_optimizer-0.1/django_img_optimizer/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-22 00:11:07.000000 django_img_optimizer-0.1/django_img_optimizer/management/commands/optimize_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:11:26.875919 django_img_optimizer-0.1/django_img_optimizer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-22 00:11:07.000000 django_img_optimizer-0.1/django_img_optimizer/templatetags/image_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-22 00:11:07.000000 django_img_optimizer-0.1/django_img_optimizer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:11:26.879919 django_img_optimizer-0.1/django_img_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-22 00:11:26.000000 django_img_optimizer-0.1/django_img_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-22 00:11:26.000000 django_img_optimizer-0.1/django_img_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 00:11:26.000000 django_img_optimizer-0.1/django_img_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 00:11:26.000000 django_img_optimizer-0.1/django_img_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 00:11:26.000000 django_img_optimizer-0.1/django_img_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-22 00:11:07.000000 django_img_optimizer-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 00:11:26.879919 django_img_optimizer-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:11:26.875919 django_img_optimizer-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-22 00:11:07.000000 django_img_optimizer-0.1/tests/test_build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:16:43.766286 django_img_optimizer-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-22 00:16:35.000000 django_img_optimizer-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-22 00:16:43.766286 django_img_optimizer-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-22 00:16:35.000000 django_img_optimizer-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:16:43.766286 django_img_optimizer-1.0/django_img_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 00:16:35.000000 django_img_optimizer-1.0/django_img_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-22 00:16:35.000000 django_img_optimizer-1.0/django_img_optimizer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:16:43.766286 django_img_optimizer-1.0/django_img_optimizer/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 00:16:35.000000 django_img_optimizer-1.0/django_img_optimizer/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:16:43.766286 django_img_optimizer-1.0/django_img_optimizer/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 00:16:35.000000 django_img_optimizer-1.0/django_img_optimizer/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-22 00:16:35.000000 django_img_optimizer-1.0/django_img_optimizer/management/commands/optimize_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:16:43.766286 django_img_optimizer-1.0/django_img_optimizer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-22 00:16:35.000000 django_img_optimizer-1.0/django_img_optimizer/templatetags/image_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-22 00:16:35.000000 django_img_optimizer-1.0/django_img_optimizer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:16:43.766286 django_img_optimizer-1.0/django_img_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-22 00:16:43.000000 django_img_optimizer-1.0/django_img_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-22 00:16:43.000000 django_img_optimizer-1.0/django_img_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 00:16:43.000000 django_img_optimizer-1.0/django_img_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 00:16:43.000000 django_img_optimizer-1.0/django_img_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 00:16:43.000000 django_img_optimizer-1.0/django_img_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-22 00:16:35.000000 django_img_optimizer-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 00:16:43.766286 django_img_optimizer-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:16:43.766286 django_img_optimizer-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-22 00:16:35.000000 django_img_optimizer-1.0/tests/test_build.py
```

### Comparing `django_img_optimizer-0.1/LICENSE` & `django_img_optimizer-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-0.1/PKG-INFO` & `django_img_optimizer-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-img-optimizer
-Version: 0.1
+Version: 1.0
 Summary: Image optimizer for Django.
 Author: Peter Stavrou
 License: MIT
 Project-URL: Homepage, https://github.com/peterstavrou/django-img-optimizer
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `django_img_optimizer-0.1/README.md` & `django_img_optimizer-1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-0.1/django_img_optimizer/management/commands/optimize_images.py` & `django_img_optimizer-1.0/django_img_optimizer/management/commands/optimize_images.py`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-0.1/django_img_optimizer/templatetags/image_optimizer.py` & `django_img_optimizer-1.0/django_img_optimizer/templatetags/image_optimizer.py`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-0.1/django_img_optimizer/utils.py` & `django_img_optimizer-1.0/django_img_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-0.1/django_img_optimizer.egg-info/PKG-INFO` & `django_img_optimizer-1.0/django_img_optimizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-img-optimizer
-Version: 0.1
+Version: 1.0
 Summary: Image optimizer for Django.
 Author: Peter Stavrou
 License: MIT
 Project-URL: Homepage, https://github.com/peterstavrou/django-img-optimizer
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `django_img_optimizer-0.1/django_img_optimizer.egg-info/SOURCES.txt` & `django_img_optimizer-1.0/django_img_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_img_optimizer-0.1/tests/test_build.py` & `django_img_optimizer-1.0/tests/test_build.py`

 * *Files identical despite different names*

