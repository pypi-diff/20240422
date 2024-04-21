# Comparing `tmp/report_creator-1.0.6.tar.gz` & `tmp/report_creator-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report_creator-1.0.6.tar", last modified: Fri Apr 19 17:55:08 2024, max compression
+gzip compressed data, was "report_creator-1.0.7.tar", last modified: Sun Apr 21 23:57:03 2024, max compression
```

## Comparing `report_creator-1.0.6.tar` & `report_creator-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:55:08.985565 report_creator-1.0.6/
--rw-r--r--   0 drace      (501) staff       (20)     1066 2024-04-19 17:26:07.000000 report_creator-1.0.6/LICENSE
--rw-r--r--   0 drace      (501) staff       (20)       69 2024-04-19 17:18:24.000000 report_creator-1.0.6/MANIFEST.in
--rw-r--r--   0 drace      (501) staff       (20)     4124 2024-04-19 17:55:08.985488 report_creator-1.0.6/PKG-INFO
--rw-r--r--   0 drace      (501) staff       (20)     3300 2024-04-19 17:44:05.000000 report_creator-1.0.6/README.md
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:55:08.983705 report_creator-1.0.6/report_creator/
--rw-r--r--   0 drace      (501) staff       (20)      478 2024-04-19 17:18:24.000000 report_creator-1.0.6/report_creator/__init__.py
--rw-r--r--   0 drace      (501) staff       (20)      174 2024-04-19 17:54:45.000000 report_creator-1.0.6/report_creator/__meta__.py
--rw-r--r--   0 drace      (501) staff       (20)    45428 2024-04-19 17:18:24.000000 report_creator-1.0.6/report_creator/report_creator.py
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:55:08.984675 report_creator-1.0.6/report_creator/templates/
--rw-r--r--   0 drace      (501) staff       (20)    10528 2024-04-19 17:18:24.000000 report_creator-1.0.6/report_creator/templates/default.html
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:55:08.985172 report_creator-1.0.6/report_creator.egg-info/
--rw-r--r--   0 drace      (501) staff       (20)     4124 2024-04-19 17:55:08.000000 report_creator-1.0.6/report_creator.egg-info/PKG-INFO
--rw-r--r--   0 drace      (501) staff       (20)      325 2024-04-19 17:55:08.000000 report_creator-1.0.6/report_creator.egg-info/SOURCES.txt
--rw-r--r--   0 drace      (501) staff       (20)        1 2024-04-19 17:55:08.000000 report_creator-1.0.6/report_creator.egg-info/dependency_links.txt
--rw-r--r--   0 drace      (501) staff       (20)       15 2024-04-19 17:55:08.000000 report_creator-1.0.6/report_creator.egg-info/top_level.txt
--rw-r--r--   0 drace      (501) staff       (20)     1079 2024-04-19 17:55:08.985903 report_creator-1.0.6/setup.cfg
--rw-r--r--   0 drace      (501) staff       (20)     1616 2024-04-19 17:54:29.000000 report_creator-1.0.6/setup.py
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-21 23:57:03.469687 report_creator-1.0.7/
+-rw-r--r--   0 drace      (501) staff       (20)     1066 2024-04-20 05:46:16.000000 report_creator-1.0.7/LICENSE
+-rw-r--r--   0 drace      (501) staff       (20)       69 2024-04-19 02:06:16.000000 report_creator-1.0.7/MANIFEST.in
+-rw-r--r--   0 drace      (501) staff       (20)     4124 2024-04-21 23:57:03.469635 report_creator-1.0.7/PKG-INFO
+-rw-r--r--   0 drace      (501) staff       (20)     3300 2024-04-20 05:46:16.000000 report_creator-1.0.7/README.md
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-21 23:57:03.468551 report_creator-1.0.7/report_creator/
+-rw-r--r--   0 drace      (501) staff       (20)      478 2024-04-19 02:06:16.000000 report_creator-1.0.7/report_creator/__init__.py
+-rw-r--r--   0 drace      (501) staff       (20)      174 2024-04-21 23:56:35.000000 report_creator-1.0.7/report_creator/__meta__.py
+-rw-r--r--   0 drace      (501) staff       (20)    45428 2024-04-19 02:06:16.000000 report_creator-1.0.7/report_creator/report_creator.py
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-21 23:57:03.469147 report_creator-1.0.7/report_creator/templates/
+-rw-r--r--   0 drace      (501) staff       (20)    10528 2024-04-19 02:06:16.000000 report_creator-1.0.7/report_creator/templates/default.html
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-21 23:57:03.469458 report_creator-1.0.7/report_creator.egg-info/
+-rw-r--r--   0 drace      (501) staff       (20)     4124 2024-04-21 23:57:03.000000 report_creator-1.0.7/report_creator.egg-info/PKG-INFO
+-rw-r--r--   0 drace      (501) staff       (20)      325 2024-04-21 23:57:03.000000 report_creator-1.0.7/report_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 drace      (501) staff       (20)        1 2024-04-21 23:57:03.000000 report_creator-1.0.7/report_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 drace      (501) staff       (20)       15 2024-04-21 23:57:03.000000 report_creator-1.0.7/report_creator.egg-info/top_level.txt
+-rw-r--r--   0 drace      (501) staff       (20)     1079 2024-04-21 23:57:03.469910 report_creator-1.0.7/setup.cfg
+-rw-r--r--   0 drace      (501) staff       (20)     1701 2024-04-21 23:57:00.000000 report_creator-1.0.7/setup.py
```

### Comparing `report_creator-1.0.6/LICENSE` & `report_creator-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.6/PKG-INFO` & `report_creator-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report_creator
-Version: 1.0.6
+Version: 1.0.7
 Summary: Produce self-contained HTML reports from Python
 Home-page: https://github.com/darenr/report_creator
 Author: Daren Race
 Author-email: daren.race@gmail.com
 License: MIT
 Keywords: python,html,reports,report,creator,generator,markdown,yaml,plot,chart,table
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `report_creator-1.0.6/README.md` & `report_creator-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.6/report_creator/report_creator.py` & `report_creator-1.0.7/report_creator/report_creator.py`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.6/report_creator/templates/default.html` & `report_creator-1.0.7/report_creator/templates/default.html`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.6/report_creator.egg-info/PKG-INFO` & `report_creator-1.0.7/report_creator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report_creator
-Version: 1.0.6
+Version: 1.0.7
 Summary: Produce self-contained HTML reports from Python
 Home-page: https://github.com/darenr/report_creator
 Author: Daren Race
 Author-email: daren.race@gmail.com
 License: MIT
 Keywords: python,html,reports,report,creator,generator,markdown,yaml,plot,chart,table
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `report_creator-1.0.6/setup.cfg` & `report_creator-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.6/setup.py` & `report_creator-1.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,20 +31,22 @@
     author=metadata["__authors__"],
     author_email=metadata["__contact__"],
     description=metadata["__description__"],
     license=metadata["__license__"],
     keywords="python, html, reports, report, creator, generator, markdown, yaml, plot, chart, table",
     url="https://github.com/darenr/report_creator",
     packages=find_packages(),
+    include_package_data=True,
+    package_data={"report_creator": ["templates/*"]},
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
-        'License :: OSI Approved :: MIT License',
+        "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
 )
```

