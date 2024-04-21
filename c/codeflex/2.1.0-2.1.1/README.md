# Comparing `tmp/codeflex-2.1.0.tar.gz` & `tmp/codeflex-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflex-2.1.0.tar", last modified: Fri Apr 19 22:00:41 2024, max compression
+gzip compressed data, was "codeflex-2.1.1.tar", last modified: Sun Apr 21 21:52:09 2024, max compression
```

## Comparing `codeflex-2.1.0.tar` & `codeflex-2.1.1.tar`

### file list

```diff
@@ -1,18 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 22:00:41.808132 codeflex-2.1.0/
--rw-rw-rw-   0        0        0     1913 2024-04-18 01:41:25.000000 codeflex-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     6238 2024-04-19 22:00:41.792514 codeflex-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5362 2024-04-19 21:58:32.000000 codeflex-2.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 22:00:41.808132 codeflex-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1040 2024-04-19 21:48:45.000000 codeflex-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 22:00:41.745647 codeflex-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 22:00:41.761269 codeflex-2.1.0/src/codeflex/
--rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-2.1.0/src/codeflex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 22:00:41.792514 codeflex-2.1.0/src/codeflex/company/
--rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-2.1.0/src/codeflex/company/__init__.py
--rw-rw-rw-   0        0        0     6303 2024-04-18 19:18:54.000000 codeflex-2.1.0/src/codeflex/company/mysql.py
--rw-rw-rw-   0        0        0     1217 2024-04-19 18:42:33.000000 codeflex-2.1.0/src/codeflex/company/polly.py
-drwxrwxrwx   0        0        0        0 2024-04-19 22:00:41.792514 codeflex-2.1.0/src/codeflex.egg-info/
--rw-rw-rw-   0        0        0     6238 2024-04-19 22:00:41.000000 codeflex-2.1.0/src/codeflex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-04-19 22:00:41.000000 codeflex-2.1.0/src/codeflex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 22:00:41.000000 codeflex-2.1.0/src/codeflex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-19 22:00:41.000000 codeflex-2.1.0/src/codeflex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.563444 codeflex-2.1.1/
+-rw-rw-rw-   0        0        0     1913 2024-04-18 01:41:25.000000 codeflex-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6238 2024-04-21 21:52:09.561457 codeflex-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5362 2024-04-19 21:58:32.000000 codeflex-2.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 21:52:09.563444 codeflex-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2024-04-21 21:51:36.000000 codeflex-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.222191 codeflex-2.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.252117 codeflex-2.1.1/src/codeflex/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-2.1.1/src/codeflex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.298985 codeflex-2.1.1/src/codeflex/company/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-2.1.1/src/codeflex/company/__init__.py
+-rw-rw-rw-   0        0        0     6303 2024-04-18 19:18:54.000000 codeflex-2.1.1/src/codeflex/company/mysql.py
+-rw-rw-rw-   0        0        0     1217 2024-04-19 18:42:33.000000 codeflex-2.1.1/src/codeflex/company/polly.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.521391 codeflex-2.1.1/src/codeflex/server/
+-rw-rw-rw-   0        0        0     2625 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/__init__.py
+-rw-rw-rw-   0        0        0       30 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/__main__.py
+-rw-rw-rw-   0        0        0    59706 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/app.py
+-rw-rw-rw-   0        0        0     3160 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/blueprints.py
+-rw-rw-rw-   0        0        0    35833 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/cli.py
+-rw-rw-rw-   0        0        0    13328 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/config.py
+-rw-rw-rw-   0        0        0    15120 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/ctx.py
+-rw-rw-rw-   0        0        0     6080 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/debughelpers.py
+-rw-rw-rw-   0        0        0     1713 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/globals.py
+-rw-rw-rw-   0        0        0    23084 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.551313 codeflex-2.1.1/src/codeflex/server/json/
+-rw-rw-rw-   0        0        0     5602 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/json/__init__.py
+-rw-rw-rw-   0        0        0     7646 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/json/provider.py
+-rw-rw-rw-   0        0        0     9280 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/json/tag.py
+-rw-rw-rw-   0        0        0     2377 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/logging.py
+-rw-rw-rw-   0        0        0        0 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/py.typed
+-rw-rw-rw-   0        0        0    14518 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/sessions.py
+-rw-rw-rw-   0        0        0      750 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/signals.py
+-rw-rw-rw-   0        0        0     7537 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/templating.py
+-rw-rw-rw-   0        0        0    10163 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/testing.py
+-rw-rw-rw-   0        0        0     3190 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/typing.py
+-rw-rw-rw-   0        0        0     6939 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/views.py
+-rw-rw-rw-   0        0        0     5831 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.554303 codeflex-2.1.1/src/codeflex.egg-info/
+-rw-rw-rw-   0        0        0     6238 2024-04-21 21:52:09.000000 codeflex-2.1.1/src/codeflex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2024-04-21 21:52:09.000000 codeflex-2.1.1/src/codeflex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 21:52:09.000000 codeflex-2.1.1/src/codeflex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 21:52:09.000000 codeflex-2.1.1/src/codeflex.egg-info/top_level.txt
```

### Comparing `codeflex-2.1.0/LICENSE` & `codeflex-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.0/PKG-INFO` & `codeflex-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflex
-Version: 2.1.0
+Version: 2.1.1
 Summary: ¡Conecta a los Microservicios de CodeFlex desde una Sola Librería!
 Home-page: https://codeflex.com.co/
 Author: CODEFLEX S.A.S.
 Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by applicable copyright laws. The distribution and use of this software are subject to the terms and conditions outlined below.
 Project-URL: Bug Tracker, https://docs.codeflex.com.co/
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: codeflex Version: 2.1.0 Summary: Â¡Conecta a los
+Metadata-Version: 2.1 Name: codeflex Version: 2.1.1 Summary: Â¡Conecta a los
 Microservicios de CodeFlex desde una Sola LibrerÃ­a! Home-page: https://
 codeflex.com.co/ Author: CODEFLEX S.A.S. Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by
 applicable copyright laws. The distribution and use of this software are
 subject to the terms and conditions outlined below. Project-URL: Bug Tracker,
 https://docs.codeflex.com.co/ Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `codeflex-2.1.0/README.md` & `codeflex-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.0/setup.py` & `codeflex-2.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
-
+ 
 setuptools.setup(
     name="codeflex",
-    version="2.1.0",
+    version="2.1.1",
     author="CODEFLEX S.A.S.", 
     author_email="info@codeflex.com.co",
     license="This software is owned by CodeFlex S.A.S. and is protected by applicable copyright laws. The distribution and use of this software are subject to the terms and conditions outlined below.",
     description="¡Conecta a los Microservicios de CodeFlex desde una Sola Librería!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://codeflex.com.co/",
```

### Comparing `codeflex-2.1.0/src/codeflex/company/mysql.py` & `codeflex-2.1.1/src/codeflex/company/mysql.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.0/src/codeflex/company/polly.py` & `codeflex-2.1.1/src/codeflex/company/polly.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.0/src/codeflex.egg-info/PKG-INFO` & `codeflex-2.1.1/src/codeflex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflex
-Version: 2.1.0
+Version: 2.1.1
 Summary: ¡Conecta a los Microservicios de CodeFlex desde una Sola Librería!
 Home-page: https://codeflex.com.co/
 Author: CODEFLEX S.A.S.
 Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by applicable copyright laws. The distribution and use of this software are subject to the terms and conditions outlined below.
 Project-URL: Bug Tracker, https://docs.codeflex.com.co/
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: codeflex Version: 2.1.0 Summary: Â¡Conecta a los
+Metadata-Version: 2.1 Name: codeflex Version: 2.1.1 Summary: Â¡Conecta a los
 Microservicios de CodeFlex desde una Sola LibrerÃ­a! Home-page: https://
 codeflex.com.co/ Author: CODEFLEX S.A.S. Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by
 applicable copyright laws. The distribution and use of this software are
 subject to the terms and conditions outlined below. Project-URL: Bug Tracker,
 https://docs.codeflex.com.co/ Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

