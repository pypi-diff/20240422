# Comparing `tmp/competex-0.1.tar.gz` & `tmp/competex-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "competex-0.1.tar", last modified: Mon Apr 22 04:26:00 2024, max compression
+gzip compressed data, was "competex-0.5.tar", last modified: Mon Apr 22 07:59:44 2024, max compression
```

## Comparing `competex-0.1.tar` & `competex-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 04:26:00.190116 competex-0.1/
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1052 2024-04-21 20:35:54.000000 competex-0.1/LICENSE
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       25 2024-04-21 17:17:02.000000 competex-0.1/MANIFEST.in
--rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2188 2024-04-22 04:26:00.190116 competex-0.1/PKG-INFO
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1858 2024-04-22 04:24:41.000000 competex-0.1/README.md
-drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 04:26:00.190116 competex-0.1/competex/
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       27 2024-04-21 20:53:10.000000 competex-0.1/competex/__init__.py
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     2294 2024-04-21 20:52:57.000000 competex-0.1/competex/main.py
-drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 04:26:00.190116 competex-0.1/competex.egg-info/
--rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2188 2024-04-22 04:26:00.000000 competex-0.1/competex.egg-info/PKG-INFO
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      210 2024-04-22 04:26:00.000000 competex-0.1/competex.egg-info/SOURCES.txt
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)        1 2024-04-22 04:26:00.000000 competex-0.1/competex.egg-info/dependency_links.txt
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)        9 2024-04-22 04:26:00.000000 competex-0.1/competex.egg-info/top_level.txt
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      307 2024-04-22 04:24:55.000000 competex-0.1/pyproject.toml
--rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       38 2024-04-22 04:26:00.190116 competex-0.1/setup.cfg
+drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 07:59:44.067776 competex-0.5/
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1052 2024-04-21 20:35:54.000000 competex-0.5/LICENSE
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       25 2024-04-21 17:17:02.000000 competex-0.5/MANIFEST.in
+-rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2188 2024-04-22 07:59:44.067776 competex-0.5/PKG-INFO
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     1858 2024-04-22 04:26:58.000000 competex-0.5/README.md
+drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 07:59:44.067776 competex-0.5/competex/
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       22 2024-04-22 07:47:37.000000 competex-0.5/competex/__init__.py
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)     7161 2024-04-22 07:59:04.000000 competex-0.5/competex/main.py
+drwxrwxr-x   0 vaxraxd   (1000) vaxraxd   (1000)        0 2024-04-22 07:59:44.067776 competex-0.5/competex.egg-info/
+-rw-r--r--   0 vaxraxd   (1000) vaxraxd   (1000)     2188 2024-04-22 07:59:44.000000 competex-0.5/competex.egg-info/PKG-INFO
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      210 2024-04-22 07:59:44.000000 competex-0.5/competex.egg-info/SOURCES.txt
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)        1 2024-04-22 07:59:44.000000 competex-0.5/competex.egg-info/dependency_links.txt
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)        9 2024-04-22 07:59:44.000000 competex-0.5/competex.egg-info/top_level.txt
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)      307 2024-04-22 07:59:16.000000 competex-0.5/pyproject.toml
+-rw-rw-r--   0 vaxraxd   (1000) vaxraxd   (1000)       38 2024-04-22 07:59:44.067776 competex-0.5/setup.cfg
```

### Comparing `competex-0.1/LICENSE` & `competex-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `competex-0.1/PKG-INFO` & `competex-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: competex
-Version: 0.1
+Version: 0.5
 Author-email: Sike Brothers <sikebros@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CompeteX Library
 CompeteX is a Python library designed for analyzing competitors using data from social media platforms. It provides a set of tools and functionalities to gather, process, and analyze social media data to gain insights into competitors' activities, audience engagement, content performance, and more.
 
 ## Installation
 You can install CompeteX using pip:
 ```bash
-pip install CompeteX
+pip install competex
 ```
 
 ## Getting Started
 To start using CompeteX, import it into your Python environment:
 ```python
 import competeX as cx
 ```
```

### Comparing `competex-0.1/README.md` & `competex-0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # CompeteX Library
 CompeteX is a Python library designed for analyzing competitors using data from social media platforms. It provides a set of tools and functionalities to gather, process, and analyze social media data to gain insights into competitors' activities, audience engagement, content performance, and more.
 
 ## Installation
 You can install CompeteX using pip:
 ```bash
-pip install CompeteX
+pip install competex
 ```
 
 ## Getting Started
 To start using CompeteX, import it into your Python environment:
 ```python
 import competeX as cx
 ```
```

### Comparing `competex-0.1/competex.egg-info/PKG-INFO` & `competex-0.5/competex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: competex
-Version: 0.1
+Version: 0.5
 Author-email: Sike Brothers <sikebros@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CompeteX Library
 CompeteX is a Python library designed for analyzing competitors using data from social media platforms. It provides a set of tools and functionalities to gather, process, and analyze social media data to gain insights into competitors' activities, audience engagement, content performance, and more.
 
 ## Installation
 You can install CompeteX using pip:
 ```bash
-pip install CompeteX
+pip install competex
 ```
 
 ## Getting Started
 To start using CompeteX, import it into your Python environment:
 ```python
 import competeX as cx
 ```
```

