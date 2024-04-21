# Comparing `tmp/competitorx-0.1.3.tar.gz` & `tmp/competitorx-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "competitorx-0.1.3.tar", last modified: Sun Apr 21 21:52:34 2024, max compression
+gzip compressed data, was "competitorx-0.1.4.tar", last modified: Sun Apr 21 22:02:14 2024, max compression
```

## Comparing `competitorx-0.1.3.tar` & `competitorx-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-21 21:52:34.840271 competitorx-0.1.3/
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1052 2024-04-21 20:35:54.000000 competitorx-0.1.3/LICENSE
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       25 2024-04-21 17:17:02.000000 competitorx-0.1.3/MANIFEST.in
--rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2235 2024-04-21 21:52:34.840271 competitorx-0.1.3/PKG-INFO
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1900 2024-04-21 19:43:24.000000 competitorx-0.1.3/README.md
-drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-21 21:52:34.840271 competitorx-0.1.3/competitorx/
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       27 2024-04-21 20:53:10.000000 competitorx-0.1.3/competitorx/__init__.py
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     2294 2024-04-21 20:52:57.000000 competitorx-0.1.3/competitorx/main.py
-drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-21 21:52:34.840271 competitorx-0.1.3/competitorx.egg-info/
--rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2235 2024-04-21 21:52:34.000000 competitorx-0.1.3/competitorx.egg-info/PKG-INFO
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      228 2024-04-21 21:52:34.000000 competitorx-0.1.3/competitorx.egg-info/SOURCES.txt
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)        1 2024-04-21 21:52:34.000000 competitorx-0.1.3/competitorx.egg-info/dependency_links.txt
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       12 2024-04-21 21:52:34.000000 competitorx-0.1.3/competitorx.egg-info/top_level.txt
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      372 2024-04-21 21:52:27.000000 competitorx-0.1.3/pyproject.toml
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       38 2024-04-21 21:52:34.840271 competitorx-0.1.3/setup.cfg
+drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-21 22:02:14.180960 competitorx-0.1.4/
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1052 2024-04-21 20:35:54.000000 competitorx-0.1.4/LICENSE
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       25 2024-04-21 17:17:02.000000 competitorx-0.1.4/MANIFEST.in
+-rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2235 2024-04-21 22:02:14.180960 competitorx-0.1.4/PKG-INFO
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1900 2024-04-21 19:43:24.000000 competitorx-0.1.4/README.md
+drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-21 22:02:14.176960 competitorx-0.1.4/competitorx/
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       27 2024-04-21 20:53:10.000000 competitorx-0.1.4/competitorx/__init__.py
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     2294 2024-04-21 20:52:57.000000 competitorx-0.1.4/competitorx/main.py
+drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-21 22:02:14.176960 competitorx-0.1.4/competitorx.egg-info/
+-rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2235 2024-04-21 22:02:14.000000 competitorx-0.1.4/competitorx.egg-info/PKG-INFO
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      228 2024-04-21 22:02:14.000000 competitorx-0.1.4/competitorx.egg-info/SOURCES.txt
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)        1 2024-04-21 22:02:14.000000 competitorx-0.1.4/competitorx.egg-info/dependency_links.txt
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       12 2024-04-21 22:02:14.000000 competitorx-0.1.4/competitorx.egg-info/top_level.txt
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      372 2024-04-21 22:02:09.000000 competitorx-0.1.4/pyproject.toml
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       38 2024-04-21 22:02:14.180960 competitorx-0.1.4/setup.cfg
```

### Comparing `competitorx-0.1.3/LICENSE` & `competitorx-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `competitorx-0.1.3/PKG-INFO` & `competitorx-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: competitorx
-Version: 0.1.3
+Version: 0.1.4
 Author-email: Sike Brothers <sikebros@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `competitorx-0.1.3/README.md` & `competitorx-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `competitorx-0.1.3/competitorx/main.py` & `competitorx-0.1.4/competitorx/main.py`

 * *Files identical despite different names*

### Comparing `competitorx-0.1.3/competitorx.egg-info/PKG-INFO` & `competitorx-0.1.4/competitorx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: competitorx
-Version: 0.1.3
+Version: 0.1.4
 Author-email: Sike Brothers <sikebros@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

