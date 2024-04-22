# Comparing `tmp/robotframework_parrot_dtmf-1.0.0.tar.gz` & `tmp/robotframework_parrot_dtmf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_parrot_dtmf-1.0.0.tar", last modified: Tue Apr 16 10:38:37 2024, max compression
+gzip compressed data, was "robotframework_parrot_dtmf-1.0.1.tar", last modified: Mon Apr 22 06:28:01 2024, max compression
```

## Comparing `robotframework_parrot_dtmf-1.0.0.tar` & `robotframework_parrot_dtmf-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-16 10:38:37.199500 robotframework_parrot_dtmf-1.0.0/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-15 11:33:40.000000 robotframework_parrot_dtmf-1.0.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      796 2024-04-16 10:38:37.199500 robotframework_parrot_dtmf-1.0.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      324 2024-04-15 11:32:19.000000 robotframework_parrot_dtmf-1.0.0/README.asciidoc
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-16 10:38:37.191500 robotframework_parrot_dtmf-1.0.0/dtmf/
--rw-rw-r--   0 user      (1000) user      (1000)    10140 2024-04-15 11:31:38.000000 robotframework_parrot_dtmf-1.0.0/dtmf/DTMF.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-15 11:30:30.000000 robotframework_parrot_dtmf-1.0.0/dtmf/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-15 11:35:06.000000 robotframework_parrot_dtmf-1.0.0/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-16 10:38:37.199500 robotframework_parrot_dtmf-1.0.0/robotframework_parrot_dtmf.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      796 2024-04-16 10:38:37.000000 robotframework_parrot_dtmf-1.0.0/robotframework_parrot_dtmf.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      327 2024-04-16 10:38:37.000000 robotframework_parrot_dtmf-1.0.0/robotframework_parrot_dtmf.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-16 10:38:37.000000 robotframework_parrot_dtmf-1.0.0/robotframework_parrot_dtmf.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       27 2024-04-16 10:38:37.000000 robotframework_parrot_dtmf-1.0.0/robotframework_parrot_dtmf.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        5 2024-04-16 10:38:37.000000 robotframework_parrot_dtmf-1.0.0/robotframework_parrot_dtmf.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      567 2024-04-16 10:38:37.199500 robotframework_parrot_dtmf-1.0.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:28:01.214660 robotframework_parrot_dtmf-1.0.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-15 11:33:40.000000 robotframework_parrot_dtmf-1.0.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      788 2024-04-22 06:28:01.214660 robotframework_parrot_dtmf-1.0.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      316 2024-04-16 10:40:33.000000 robotframework_parrot_dtmf-1.0.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:28:01.214660 robotframework_parrot_dtmf-1.0.1/dtmf/
+-rw-rw-r--   0 user      (1000) user      (1000)    10140 2024-04-15 11:31:38.000000 robotframework_parrot_dtmf-1.0.1/dtmf/DTMF.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-15 11:30:30.000000 robotframework_parrot_dtmf-1.0.1/dtmf/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-15 11:35:06.000000 robotframework_parrot_dtmf-1.0.1/pyproject.toml
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:28:01.214660 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      788 2024-04-22 06:28:01.000000 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      321 2024-04-22 06:28:01.000000 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-22 06:28:01.000000 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       27 2024-04-22 06:28:01.000000 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        5 2024-04-22 06:28:01.000000 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      561 2024-04-22 06:28:01.214660 robotframework_parrot_dtmf-1.0.1/setup.cfg
```

### Comparing `robotframework_parrot_dtmf-1.0.0/LICENSE` & `robotframework_parrot_dtmf-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_dtmf-1.0.0/PKG-INFO` & `robotframework_parrot_dtmf-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-dtmf
-Version: 1.0.0
+Version: 1.0.1
 Summary: DTMF (Dual tone multi frequency) Library used to generate and verify DTMF tone
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydub
 Requires-Dist: numpy
 Requires-Dist: robotframework
 
-= DTMF Library
+# DTMF Library
 
-== Installation
+## Installation
 
 To install from package registry use the following command:
 
------
+```
 $ pip install robotframework-parrot-dtmf
------
+```
 
 To install from git repo use the following command:
 
------
+```
 $ pip install .
------
+```
     
-== Example
+## Example
 
 Example of using the library in Robot Framework is available `example.robot`.
```

### Comparing `robotframework_parrot_dtmf-1.0.0/dtmf/DTMF.py` & `robotframework_parrot_dtmf-1.0.1/dtmf/DTMF.py`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_dtmf-1.0.0/robotframework_parrot_dtmf.egg-info/PKG-INFO` & `robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-dtmf
-Version: 1.0.0
+Version: 1.0.1
 Summary: DTMF (Dual tone multi frequency) Library used to generate and verify DTMF tone
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydub
 Requires-Dist: numpy
 Requires-Dist: robotframework
 
-= DTMF Library
+# DTMF Library
 
-== Installation
+## Installation
 
 To install from package registry use the following command:
 
------
+```
 $ pip install robotframework-parrot-dtmf
------
+```
 
 To install from git repo use the following command:
 
------
+```
 $ pip install .
------
+```
     
-== Example
+## Example
 
 Example of using the library in Robot Framework is available `example.robot`.
```

### Comparing `robotframework_parrot_dtmf-1.0.0/setup.cfg` & `robotframework_parrot_dtmf-1.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = robotframework-parrot-dtmf
-version = 1.0.0
+version = 1.0.1
 author = Zilogic Systems
 author_email = code@zilogic.com
 description = DTMF (Dual tone multi frequency) Library used to generate and verify DTMF tone
-long_description = file: README.asciidoc
+long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/zilogic-systems/parrot
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 install_requires =
```

