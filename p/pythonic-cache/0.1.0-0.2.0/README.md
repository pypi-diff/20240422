# Comparing `tmp/pythonic_cache-0.1.0.tar.gz` & `tmp/pythonic_cache-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonic_cache-0.1.0.tar", last modified: Mon Apr 22 00:58:53 2024, max compression
+gzip compressed data, was "pythonic_cache-0.2.0.tar", last modified: Mon Apr 22 01:06:05 2024, max compression
```

## Comparing `pythonic_cache-0.1.0.tar` & `pythonic_cache-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 00:58:53.283938 pythonic_cache-0.1.0/
--rw-rw-r--   0 alim      (1000) alim      (1000)     1057 2024-04-21 16:00:28.000000 pythonic_cache-0.1.0/LICENSE.md
--rw-r--r--   0 alim      (1000) alim      (1000)      897 2024-04-22 00:58:53.283938 pythonic_cache-0.1.0/PKG-INFO
--rw-rw-r--   0 alim      (1000) alim      (1000)     4685 2024-04-22 00:57:23.000000 pythonic_cache-0.1.0/README.md
--rw-rw-r--   0 alim      (1000) alim      (1000)     1129 2024-04-22 00:58:49.000000 pythonic_cache-0.1.0/pyproject.toml
--rw-rw-r--   0 alim      (1000) alim      (1000)       38 2024-04-22 00:58:53.283938 pythonic_cache-0.1.0/setup.cfg
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 00:58:53.275938 pythonic_cache-0.1.0/src/
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 00:58:53.275938 pythonic_cache-0.1.0/src/pythonic_cache/
--rw-rw-r--   0 alim      (1000) alim      (1000)      208 2024-04-22 00:54:48.000000 pythonic_cache-0.1.0/src/pythonic_cache/__init__.py
--rw-rw-r--   0 alim      (1000) alim      (1000)     1495 2024-04-22 00:54:48.000000 pythonic_cache-0.1.0/src/pythonic_cache/client.py
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 00:58:53.279938 pythonic_cache-0.1.0/src/pythonic_cache/integrations/
--rw-rw-r--   0 alim      (1000) alim      (1000)        0 2024-04-21 15:59:49.000000 pythonic_cache-0.1.0/src/pythonic_cache/integrations/__init__.py
--rw-rw-r--   0 alim      (1000) alim      (1000)     2208 2024-04-22 00:54:48.000000 pythonic_cache-0.1.0/src/pythonic_cache/integrations/fastapi.py
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 00:58:53.283938 pythonic_cache-0.1.0/src/pythonic_cache/storage/
--rw-rw-r--   0 alim      (1000) alim      (1000)      102 2024-04-22 00:54:48.000000 pythonic_cache-0.1.0/src/pythonic_cache/storage/__init__.py
--rw-rw-r--   0 alim      (1000) alim      (1000)     1917 2024-04-21 22:29:24.000000 pythonic_cache-0.1.0/src/pythonic_cache/storage/base.py
--rw-rw-r--   0 alim      (1000) alim      (1000)     2493 2024-04-22 00:54:48.000000 pythonic_cache-0.1.0/src/pythonic_cache/storage/memory.py
--rw-rw-r--   0 alim      (1000) alim      (1000)     2126 2024-04-22 00:54:48.000000 pythonic_cache-0.1.0/src/pythonic_cache/storage/redis.py
--rw-rw-r--   0 alim      (1000) alim      (1000)      209 2024-04-21 21:31:50.000000 pythonic_cache-0.1.0/src/pythonic_cache/storage/utils.py
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 00:58:53.283938 pythonic_cache-0.1.0/src/pythonic_cache.egg-info/
--rw-r--r--   0 alim      (1000) alim      (1000)      897 2024-04-22 00:58:53.000000 pythonic_cache-0.1.0/src/pythonic_cache.egg-info/PKG-INFO
--rw-rw-r--   0 alim      (1000) alim      (1000)      574 2024-04-22 00:58:53.000000 pythonic_cache-0.1.0/src/pythonic_cache.egg-info/SOURCES.txt
--rw-rw-r--   0 alim      (1000) alim      (1000)        1 2024-04-22 00:58:53.000000 pythonic_cache-0.1.0/src/pythonic_cache.egg-info/dependency_links.txt
--rw-rw-r--   0 alim      (1000) alim      (1000)      148 2024-04-22 00:58:53.000000 pythonic_cache-0.1.0/src/pythonic_cache.egg-info/requires.txt
--rw-rw-r--   0 alim      (1000) alim      (1000)       15 2024-04-22 00:58:53.000000 pythonic_cache-0.1.0/src/pythonic_cache.egg-info/top_level.txt
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 01:06:05.491085 pythonic_cache-0.2.0/
+-rw-rw-r--   0 alim      (1000) alim      (1000)     1057 2024-04-21 16:00:28.000000 pythonic_cache-0.2.0/LICENSE.md
+-rw-r--r--   0 alim      (1000) alim      (1000)     5623 2024-04-22 01:06:05.491085 pythonic_cache-0.2.0/PKG-INFO
+-rw-rw-r--   0 alim      (1000) alim      (1000)     4685 2024-04-22 00:57:23.000000 pythonic_cache-0.2.0/README.md
+-rw-rw-r--   0 alim      (1000) alim      (1000)     1150 2024-04-22 01:05:02.000000 pythonic_cache-0.2.0/pyproject.toml
+-rw-rw-r--   0 alim      (1000) alim      (1000)       38 2024-04-22 01:06:05.491085 pythonic_cache-0.2.0/setup.cfg
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 01:06:05.479085 pythonic_cache-0.2.0/src/
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 01:06:05.483085 pythonic_cache-0.2.0/src/pythonic_cache/
+-rw-rw-r--   0 alim      (1000) alim      (1000)      208 2024-04-22 01:05:10.000000 pythonic_cache-0.2.0/src/pythonic_cache/__init__.py
+-rw-rw-r--   0 alim      (1000) alim      (1000)     1495 2024-04-22 00:54:48.000000 pythonic_cache-0.2.0/src/pythonic_cache/client.py
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 01:06:05.483085 pythonic_cache-0.2.0/src/pythonic_cache/integrations/
+-rw-rw-r--   0 alim      (1000) alim      (1000)        0 2024-04-21 15:59:49.000000 pythonic_cache-0.2.0/src/pythonic_cache/integrations/__init__.py
+-rw-rw-r--   0 alim      (1000) alim      (1000)     2208 2024-04-22 00:54:48.000000 pythonic_cache-0.2.0/src/pythonic_cache/integrations/fastapi.py
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 01:06:05.487085 pythonic_cache-0.2.0/src/pythonic_cache/storage/
+-rw-rw-r--   0 alim      (1000) alim      (1000)      102 2024-04-22 00:54:48.000000 pythonic_cache-0.2.0/src/pythonic_cache/storage/__init__.py
+-rw-rw-r--   0 alim      (1000) alim      (1000)     1917 2024-04-21 22:29:24.000000 pythonic_cache-0.2.0/src/pythonic_cache/storage/base.py
+-rw-rw-r--   0 alim      (1000) alim      (1000)     2493 2024-04-22 00:54:48.000000 pythonic_cache-0.2.0/src/pythonic_cache/storage/memory.py
+-rw-rw-r--   0 alim      (1000) alim      (1000)     2126 2024-04-22 00:54:48.000000 pythonic_cache-0.2.0/src/pythonic_cache/storage/redis.py
+-rw-rw-r--   0 alim      (1000) alim      (1000)      209 2024-04-21 21:31:50.000000 pythonic_cache-0.2.0/src/pythonic_cache/storage/utils.py
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-22 01:06:05.487085 pythonic_cache-0.2.0/src/pythonic_cache.egg-info/
+-rw-r--r--   0 alim      (1000) alim      (1000)     5623 2024-04-22 01:06:05.000000 pythonic_cache-0.2.0/src/pythonic_cache.egg-info/PKG-INFO
+-rw-rw-r--   0 alim      (1000) alim      (1000)      574 2024-04-22 01:06:05.000000 pythonic_cache-0.2.0/src/pythonic_cache.egg-info/SOURCES.txt
+-rw-rw-r--   0 alim      (1000) alim      (1000)        1 2024-04-22 01:06:05.000000 pythonic_cache-0.2.0/src/pythonic_cache.egg-info/dependency_links.txt
+-rw-rw-r--   0 alim      (1000) alim      (1000)      148 2024-04-22 01:06:05.000000 pythonic_cache-0.2.0/src/pythonic_cache.egg-info/requires.txt
+-rw-rw-r--   0 alim      (1000) alim      (1000)       15 2024-04-22 01:06:05.000000 pythonic_cache-0.2.0/src/pythonic_cache.egg-info/top_level.txt
```

### Comparing `pythonic_cache-0.1.0/LICENSE.md` & `pythonic_cache-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pythonic_cache-0.1.0/README.md` & `pythonic_cache-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pythonic_cache-0.1.0/pyproject.toml` & `pythonic_cache-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 authors = [{name = "Alim Abrekov", email = "alimabrekov@outlook.com"}]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 name = "pythonic-cache"
+readme = "README.md"
 requires-python = ">=3.11.0"
-version = "0.1.0"
+version = "0.2.0"
 
 [project.optional-dependencies]
 lint = [
   "black>=24.3.0",
   "isort>=5.13.2",
   "mypy>=1.9.0",
   "flake8>=7.0.0",
```

### Comparing `pythonic_cache-0.1.0/src/pythonic_cache/client.py` & `pythonic_cache-0.2.0/src/pythonic_cache/client.py`

 * *Files identical despite different names*

### Comparing `pythonic_cache-0.1.0/src/pythonic_cache/integrations/fastapi.py` & `pythonic_cache-0.2.0/src/pythonic_cache/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `pythonic_cache-0.1.0/src/pythonic_cache/storage/base.py` & `pythonic_cache-0.2.0/src/pythonic_cache/storage/base.py`

 * *Files identical despite different names*

### Comparing `pythonic_cache-0.1.0/src/pythonic_cache/storage/memory.py` & `pythonic_cache-0.2.0/src/pythonic_cache/storage/memory.py`

 * *Files identical despite different names*

### Comparing `pythonic_cache-0.1.0/src/pythonic_cache/storage/redis.py` & `pythonic_cache-0.2.0/src/pythonic_cache/storage/redis.py`

 * *Files identical despite different names*

### Comparing `pythonic_cache-0.1.0/src/pythonic_cache.egg-info/SOURCES.txt` & `pythonic_cache-0.2.0/src/pythonic_cache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

