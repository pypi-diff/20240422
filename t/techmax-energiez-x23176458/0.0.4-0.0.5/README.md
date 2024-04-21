# Comparing `tmp/techmax_energiez_x23176458-0.0.4.tar.gz` & `tmp/techmax_energiez_x23176458-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "techmax_energiez_x23176458-0.0.4.tar", last modified: Sun Apr 21 21:46:22 2024, max compression
+gzip compressed data, was "techmax_energiez_x23176458-0.0.5.tar", last modified: Sun Apr 21 21:57:28 2024, max compression
```

## Comparing `techmax_energiez_x23176458-0.0.4.tar` & `techmax_energiez_x23176458-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 21:46:22.350750 techmax_energiez_x23176458-0.0.4/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      456 2024-04-21 21:46:22.350750 techmax_energiez_x23176458-0.0.4/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 19:48:23.000000 techmax_energiez_x23176458-0.0.4/README.md
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-21 21:46:22.350750 techmax_energiez_x23176458-0.0.4/setup.cfg
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      902 2024-04-21 21:46:10.000000 techmax_energiez_x23176458-0.0.4/setup.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 21:46:22.350750 techmax_energiez_x23176458-0.0.4/techmax_energiez_pkg/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 18:39:16.000000 techmax_energiez_x23176458-0.0.4/techmax_energiez_pkg/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      784 2024-04-21 21:45:50.000000 techmax_energiez_x23176458-0.0.4/techmax_energiez_pkg/server_status.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      805 2024-04-21 21:03:34.000000 techmax_energiez_x23176458-0.0.4/techmax_energiez_pkg/validations.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 21:46:22.350750 techmax_energiez_x23176458-0.0.4/techmax_energiez_x23176458.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      456 2024-04-21 21:46:22.000000 techmax_energiez_x23176458-0.0.4/techmax_energiez_x23176458.egg-info/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      325 2024-04-21 21:46:22.000000 techmax_energiez_x23176458-0.0.4/techmax_energiez_x23176458.egg-info/SOURCES.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-21 21:46:22.000000 techmax_energiez_x23176458-0.0.4/techmax_energiez_x23176458.egg-info/dependency_links.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       21 2024-04-21 21:46:22.000000 techmax_energiez_x23176458-0.0.4/techmax_energiez_x23176458.egg-info/top_level.txt
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 21:57:28.022743 techmax_energiez_x23176458-0.0.5/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      456 2024-04-21 21:57:28.022743 techmax_energiez_x23176458-0.0.5/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 19:48:23.000000 techmax_energiez_x23176458-0.0.5/README.md
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-21 21:57:28.022743 techmax_energiez_x23176458-0.0.5/setup.cfg
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      902 2024-04-21 21:57:22.000000 techmax_energiez_x23176458-0.0.5/setup.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 21:57:28.022743 techmax_energiez_x23176458-0.0.5/techmax_energiez_pkg/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 18:39:16.000000 techmax_energiez_x23176458-0.0.5/techmax_energiez_pkg/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1075 2024-04-21 21:56:14.000000 techmax_energiez_x23176458-0.0.5/techmax_energiez_pkg/server_status.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      805 2024-04-21 21:03:34.000000 techmax_energiez_x23176458-0.0.5/techmax_energiez_pkg/validations.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-21 21:57:28.022743 techmax_energiez_x23176458-0.0.5/techmax_energiez_x23176458.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      456 2024-04-21 21:57:27.000000 techmax_energiez_x23176458-0.0.5/techmax_energiez_x23176458.egg-info/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      325 2024-04-21 21:57:28.000000 techmax_energiez_x23176458-0.0.5/techmax_energiez_x23176458.egg-info/SOURCES.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-21 21:57:27.000000 techmax_energiez_x23176458-0.0.5/techmax_energiez_x23176458.egg-info/dependency_links.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       21 2024-04-21 21:57:27.000000 techmax_energiez_x23176458-0.0.5/techmax_energiez_x23176458.egg-info/top_level.txt
```

### Comparing `techmax_energiez_x23176458-0.0.4/setup.py` & `techmax_energiez_x23176458-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="techmax_energiez_x23176458",
     # Replace with your own username above
-    version="0.0.4",
+    version="0.0.5",
     author="AnilgovindKA",
     author_email="anilgovindk@gmail.com",
     description="Package for validations, techmax project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/anilgovind-nci/techmax-energiez-package",
     packages=setuptools.find_packages(),
```

### Comparing `techmax_energiez_x23176458-0.0.4/techmax_energiez_pkg/validations.py` & `techmax_energiez_x23176458-0.0.5/techmax_energiez_pkg/validations.py`

 * *Files identical despite different names*

