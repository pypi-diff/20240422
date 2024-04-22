# Comparing `tmp/robotframework_parrot_ocrlib-1.0.1.tar.gz` & `tmp/robotframework_parrot_ocrlib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_parrot_ocrlib-1.0.1.tar", last modified: Mon Apr 22 06:20:58 2024, max compression
+gzip compressed data, was "robotframework_parrot_ocrlib-1.0.2.tar", last modified: Mon Apr 22 06:24:18 2024, max compression
```

## Comparing `robotframework_parrot_ocrlib-1.0.1.tar` & `robotframework_parrot_ocrlib-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:20:58.897593 robotframework_parrot_ocrlib-1.0.1/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework_parrot_ocrlib-1.0.1/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      475 2024-04-22 06:20:58.897593 robotframework_parrot_ocrlib-1.0.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      486 2024-04-22 06:11:01.000000 robotframework_parrot_ocrlib-1.0.1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:20:58.897593 robotframework_parrot_ocrlib-1.0.1/ocr/
--rw-rw-r--   0 user      (1000) user      (1000)     2042 2024-04-10 06:17:16.000000 robotframework_parrot_ocrlib-1.0.1/ocr/OCRLib.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-15 11:22:39.000000 robotframework_parrot_ocrlib-1.0.1/ocr/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-10 12:39:25.000000 robotframework_parrot_ocrlib-1.0.1/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:20:58.897593 robotframework_parrot_ocrlib-1.0.1/robotframework_parrot_ocrlib.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      475 2024-04-22 06:20:58.000000 robotframework_parrot_ocrlib-1.0.1/robotframework_parrot_ocrlib.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      331 2024-04-22 06:20:58.000000 robotframework_parrot_ocrlib-1.0.1/robotframework_parrot_ocrlib.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-22 06:20:58.000000 robotframework_parrot_ocrlib-1.0.1/robotframework_parrot_ocrlib.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       40 2024-04-22 06:20:58.000000 robotframework_parrot_ocrlib-1.0.1/robotframework_parrot_ocrlib.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-22 06:20:58.000000 robotframework_parrot_ocrlib-1.0.1/robotframework_parrot_ocrlib.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      557 2024-04-22 06:20:58.897593 robotframework_parrot_ocrlib-1.0.1/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:24:18.364442 robotframework_parrot_ocrlib-1.0.2/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework_parrot_ocrlib-1.0.2/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      962 2024-04-22 06:24:18.364442 robotframework_parrot_ocrlib-1.0.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      486 2024-04-22 06:11:01.000000 robotframework_parrot_ocrlib-1.0.2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:24:18.364442 robotframework_parrot_ocrlib-1.0.2/ocr/
+-rw-rw-r--   0 user      (1000) user      (1000)     2042 2024-04-10 06:17:16.000000 robotframework_parrot_ocrlib-1.0.2/ocr/OCRLib.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-15 11:22:39.000000 robotframework_parrot_ocrlib-1.0.2/ocr/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-10 12:39:25.000000 robotframework_parrot_ocrlib-1.0.2/pyproject.toml
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:24:18.364442 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      962 2024-04-22 06:24:18.000000 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      331 2024-04-22 06:24:18.000000 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-22 06:24:18.000000 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       40 2024-04-22 06:24:18.000000 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-22 06:24:18.000000 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      551 2024-04-22 06:24:18.364442 robotframework_parrot_ocrlib-1.0.2/setup.cfg
```

### Comparing `robotframework_parrot_ocrlib-1.0.1/LICENSE` & `robotframework_parrot_ocrlib-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_ocrlib-1.0.1/ocr/OCRLib.py` & `robotframework_parrot_ocrlib-1.0.2/ocr/OCRLib.py`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_ocrlib-1.0.1/setup.cfg` & `robotframework_parrot_ocrlib-1.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = robotframework-parrot-ocrlib
-version = 1.0.1
+version = 1.0.2
 author = Zilogic Systems
 author_email = code@zilogic.com
 description = OCR Library to recognize text within a digital image
-long_description = file: README.asciidoc
+long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/zilogic-systems/parrot
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 install_requires =
```

