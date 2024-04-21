# Comparing `tmp/lichesspy-6.0.4.dev4.tar.gz` & `tmp/lichesspy-6.0.4.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichesspy-6.0.4.dev4.tar", last modified: Sun Apr 21 19:41:32 2024, max compression
+gzip compressed data, was "lichesspy-6.0.4.dev5.tar", last modified: Sun Apr 21 19:52:57 2024, max compression
```

## Comparing `lichesspy-6.0.4.dev4.tar` & `lichesspy-6.0.4.dev5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:41:32.213632 lichesspy-6.0.4.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-21 19:41:32.213632 lichesspy-6.0.4.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:41:32.213632 lichesspy-6.0.4.dev4/lichesspy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/lichesspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/lichesspy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/lichesspy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/lichesspy/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/lichesspy/pgn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:41:32.213632 lichesspy-6.0.4.dev4/lichesspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-21 19:41:32.000000 lichesspy-6.0.4.dev4/lichesspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 19:41:32.000000 lichesspy-6.0.4.dev4/lichesspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:41:32.000000 lichesspy-6.0.4.dev4/lichesspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-21 19:41:32.000000 lichesspy-6.0.4.dev4/lichesspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 19:41:32.000000 lichesspy-6.0.4.dev4/lichesspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:41:32.213632 lichesspy-6.0.4.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-21 19:41:24.000000 lichesspy-6.0.4.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:52:57.807653 lichesspy-6.0.4.dev5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 19:52:52.000000 lichesspy-6.0.4.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-21 19:52:57.803653 lichesspy-6.0.4.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-21 19:52:52.000000 lichesspy-6.0.4.dev5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:52:57.803653 lichesspy-6.0.4.dev5/lichesspy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:52:52.000000 lichesspy-6.0.4.dev5/lichesspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-04-21 19:52:52.000000 lichesspy-6.0.4.dev5/lichesspy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 19:52:52.000000 lichesspy-6.0.4.dev5/lichesspy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-21 19:52:52.000000 lichesspy-6.0.4.dev5/lichesspy/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-21 19:52:52.000000 lichesspy-6.0.4.dev5/lichesspy/pgn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:52:57.803653 lichesspy-6.0.4.dev5/lichesspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-21 19:52:57.000000 lichesspy-6.0.4.dev5/lichesspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 19:52:57.000000 lichesspy-6.0.4.dev5/lichesspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:52:57.000000 lichesspy-6.0.4.dev5/lichesspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 19:52:57.000000 lichesspy-6.0.4.dev5/lichesspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 19:52:57.000000 lichesspy-6.0.4.dev5/lichesspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:52:57.807653 lichesspy-6.0.4.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-21 19:52:52.000000 lichesspy-6.0.4.dev5/setup.py
```

### Comparing `lichesspy-6.0.4.dev4/LICENSE` & `lichesspy-6.0.4.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev4/PKG-INFO` & `lichesspy-6.0.4.dev5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.4.dev4
+Version: 6.0.4.dev5
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik+lichesspy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.0.0
+Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
 Requires-Dist: chess==1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
```

### Comparing `lichesspy-6.0.4.dev4/README.rst` & `lichesspy-6.0.4.dev5/README.rst`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev4/lichesspy/api.py` & `lichesspy-6.0.4.dev5/lichesspy/api.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev4/lichesspy/format.py` & `lichesspy-6.0.4.dev5/lichesspy/format.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev4/lichesspy/pgn.py` & `lichesspy-6.0.4.dev5/lichesspy/pgn.py`

 * *Files identical despite different names*

### Comparing `lichesspy-6.0.4.dev4/lichesspy.egg-info/PKG-INFO` & `lichesspy-6.0.4.dev5/lichesspy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: lichesspy
-Version: 6.0.4.dev4
+Version: 6.0.4.dev5
 Summary: Python wrapper for lichess
 Home-page: https://github.com/eskopp/lichesspy
 Author: eskopp
 Author-email: skopp.erik+lichesspy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.0.0
+Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
 Requires-Dist: chess==1.10.0
 
 A client for the lichess.org API
 ================================================
 This is a client library for the Lichess API.
 It is designed to be:
```

### Comparing `lichesspy-6.0.4.dev4/setup.py` & `lichesspy-6.0.4.dev5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     if readme_path.exists():
         return readme_path.read_text(encoding="utf-8")
     return "Long description could not be read from README.rst"
 
 
 setuptools.setup(
     name="lichesspy",
-    version="6.0.4.dev4",
+    version="6.0.4.dev5",
     author="eskopp",
     author_email="skopp.erik+lichesspy@gmail.com",
     description="Python wrapper for lichess",
     long_description=load_readme(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/eskopp/lichesspy",
@@ -25,9 +25,13 @@
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.10",
-    install_requires=["requests==2.0.0", "six==1.16.0", "chess==1.10.0"],
+    install_requires=[
+        'requests==2.31.0',
+        'six==1.16.0',
+        'chess==1.10.0'
+    ]
 )
```

