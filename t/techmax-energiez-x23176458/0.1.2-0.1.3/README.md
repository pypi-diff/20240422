# Comparing `tmp/techmax_energiez_x23176458-0.1.2.tar.gz` & `tmp/techmax_energiez_x23176458-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "techmax_energiez_x23176458-0.1.2.tar", last modified: Sun Apr 21 22:51:20 2024, max compression
+gzip compressed data, was "techmax_energiez_x23176458-0.1.3.tar", last modified: Sun Apr 21 23:41:48 2024, max compression
```

## Comparing `techmax_energiez_x23176458-0.1.2.tar` & `techmax_energiez_x23176458-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 22:51:20.222325 techmax_energiez_x23176458-0.1.2/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      456 2024-04-21 22:51:20.222325 techmax_energiez_x23176458-0.1.2/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 19:48:23.000000 techmax_energiez_x23176458-0.1.2/README.md
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-21 22:51:20.222325 techmax_energiez_x23176458-0.1.2/setup.cfg
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      902 2024-04-21 22:51:12.000000 techmax_energiez_x23176458-0.1.2/setup.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 22:51:20.212325 techmax_energiez_x23176458-0.1.2/techmax_energiez_pkg/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 18:39:16.000000 techmax_energiez_x23176458-0.1.2/techmax_energiez_pkg/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1075 2024-04-21 21:56:14.000000 techmax_energiez_x23176458-0.1.2/techmax_energiez_pkg/server_status.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1471 2024-04-21 22:50:44.000000 techmax_energiez_x23176458-0.1.2/techmax_energiez_pkg/validations.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 22:51:20.222325 techmax_energiez_x23176458-0.1.2/techmax_energiez_x23176458.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      456 2024-04-21 22:51:20.000000 techmax_energiez_x23176458-0.1.2/techmax_energiez_x23176458.egg-info/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      325 2024-04-21 22:51:20.000000 techmax_energiez_x23176458-0.1.2/techmax_energiez_x23176458.egg-info/SOURCES.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-21 22:51:20.000000 techmax_energiez_x23176458-0.1.2/techmax_energiez_x23176458.egg-info/dependency_links.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       21 2024-04-21 22:51:20.000000 techmax_energiez_x23176458-0.1.2/techmax_energiez_x23176458.egg-info/top_level.txt
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 23:41:48.531305 techmax_energiez_x23176458-0.1.3/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      456 2024-04-21 23:41:48.531305 techmax_energiez_x23176458-0.1.3/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 19:48:23.000000 techmax_energiez_x23176458-0.1.3/README.md
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-21 23:41:48.531305 techmax_energiez_x23176458-0.1.3/setup.cfg
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      902 2024-04-21 23:41:43.000000 techmax_energiez_x23176458-0.1.3/setup.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 23:41:48.531305 techmax_energiez_x23176458-0.1.3/techmax_energiez_pkg/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 18:39:16.000000 techmax_energiez_x23176458-0.1.3/techmax_energiez_pkg/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      903 2024-04-21 23:40:24.000000 techmax_energiez_x23176458-0.1.3/techmax_energiez_pkg/server_status.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1471 2024-04-21 23:41:35.000000 techmax_energiez_x23176458-0.1.3/techmax_energiez_pkg/validations.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 23:41:48.531305 techmax_energiez_x23176458-0.1.3/techmax_energiez_x23176458.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      456 2024-04-21 23:41:48.000000 techmax_energiez_x23176458-0.1.3/techmax_energiez_x23176458.egg-info/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      325 2024-04-21 23:41:48.000000 techmax_energiez_x23176458-0.1.3/techmax_energiez_x23176458.egg-info/SOURCES.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-21 23:41:48.000000 techmax_energiez_x23176458-0.1.3/techmax_energiez_x23176458.egg-info/dependency_links.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       21 2024-04-21 23:41:48.000000 techmax_energiez_x23176458-0.1.3/techmax_energiez_x23176458.egg-info/top_level.txt
```

### Comparing `techmax_energiez_x23176458-0.1.2/setup.py` & `techmax_energiez_x23176458-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="techmax_energiez_x23176458",
     # Replace with your own username above
-    version="0.1.2",
+    version="0.1.3",
     author="AnilgovindKA",
     author_email="anilgovindk@gmail.com",
     description="Package for validations, techmax project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/anilgovind-nci/techmax-energiez-package",
     packages=setuptools.find_packages(),
```

### Comparing `techmax_energiez_x23176458-0.1.2/techmax_energiez_pkg/validations.py` & `techmax_energiez_x23176458-0.1.3/techmax_energiez_pkg/validations.py`

 * *Files identical despite different names*

