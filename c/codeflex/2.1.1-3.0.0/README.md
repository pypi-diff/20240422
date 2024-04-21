# Comparing `tmp/codeflex-2.1.1.tar.gz` & `tmp/codeflex-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflex-2.1.1.tar", last modified: Sun Apr 21 21:52:09 2024, max compression
+gzip compressed data, was "codeflex-3.0.0.tar", last modified: Sun Apr 21 22:24:54 2024, max compression
```

## Comparing `codeflex-2.1.1.tar` & `codeflex-3.0.0.tar`

### file list

```diff
@@ -1,42 +1,68 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.563444 codeflex-2.1.1/
--rw-rw-rw-   0        0        0     1913 2024-04-18 01:41:25.000000 codeflex-2.1.1/LICENSE
--rw-rw-rw-   0        0        0     6238 2024-04-21 21:52:09.561457 codeflex-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5362 2024-04-19 21:58:32.000000 codeflex-2.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 21:52:09.563444 codeflex-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1041 2024-04-21 21:51:36.000000 codeflex-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.222191 codeflex-2.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.252117 codeflex-2.1.1/src/codeflex/
--rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-2.1.1/src/codeflex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.298985 codeflex-2.1.1/src/codeflex/company/
--rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-2.1.1/src/codeflex/company/__init__.py
--rw-rw-rw-   0        0        0     6303 2024-04-18 19:18:54.000000 codeflex-2.1.1/src/codeflex/company/mysql.py
--rw-rw-rw-   0        0        0     1217 2024-04-19 18:42:33.000000 codeflex-2.1.1/src/codeflex/company/polly.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.521391 codeflex-2.1.1/src/codeflex/server/
--rw-rw-rw-   0        0        0     2625 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/__init__.py
--rw-rw-rw-   0        0        0       30 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/__main__.py
--rw-rw-rw-   0        0        0    59706 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/app.py
--rw-rw-rw-   0        0        0     3160 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/blueprints.py
--rw-rw-rw-   0        0        0    35833 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/cli.py
--rw-rw-rw-   0        0        0    13328 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/config.py
--rw-rw-rw-   0        0        0    15120 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/ctx.py
--rw-rw-rw-   0        0        0     6080 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/debughelpers.py
--rw-rw-rw-   0        0        0     1713 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/globals.py
--rw-rw-rw-   0        0        0    23084 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.551313 codeflex-2.1.1/src/codeflex/server/json/
--rw-rw-rw-   0        0        0     5602 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/json/__init__.py
--rw-rw-rw-   0        0        0     7646 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/json/provider.py
--rw-rw-rw-   0        0        0     9280 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/json/tag.py
--rw-rw-rw-   0        0        0     2377 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/logging.py
--rw-rw-rw-   0        0        0        0 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/py.typed
--rw-rw-rw-   0        0        0    14518 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/sessions.py
--rw-rw-rw-   0        0        0      750 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/signals.py
--rw-rw-rw-   0        0        0     7537 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/templating.py
--rw-rw-rw-   0        0        0    10163 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/testing.py
--rw-rw-rw-   0        0        0     3190 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/typing.py
--rw-rw-rw-   0        0        0     6939 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/views.py
--rw-rw-rw-   0        0        0     5831 2024-02-14 20:44:10.000000 codeflex-2.1.1/src/codeflex/server/wrappers.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:52:09.554303 codeflex-2.1.1/src/codeflex.egg-info/
--rw-rw-rw-   0        0        0     6238 2024-04-21 21:52:09.000000 codeflex-2.1.1/src/codeflex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      980 2024-04-21 21:52:09.000000 codeflex-2.1.1/src/codeflex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 21:52:09.000000 codeflex-2.1.1/src/codeflex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 21:52:09.000000 codeflex-2.1.1/src/codeflex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 22:24:54.609236 codeflex-3.0.0/
+-rw-rw-rw-   0        0        0     1913 2024-04-18 01:41:25.000000 codeflex-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     6238 2024-04-21 22:24:54.607242 codeflex-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5362 2024-04-19 21:58:32.000000 codeflex-3.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-21 22:24:54.610233 codeflex-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2024-04-21 22:10:26.000000 codeflex-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:24:54.247205 codeflex-3.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-21 22:24:54.275129 codeflex-3.0.0/src/codeflex/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-3.0.0/src/codeflex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:24:54.314025 codeflex-3.0.0/src/codeflex/company/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-3.0.0/src/codeflex/company/__init__.py
+-rw-rw-rw-   0        0        0     6303 2024-04-18 19:18:54.000000 codeflex-3.0.0/src/codeflex/company/mysql.py
+-rw-rw-rw-   0        0        0     1217 2024-04-19 18:42:33.000000 codeflex-3.0.0/src/codeflex/company/polly.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:24:54.431711 codeflex-3.0.0/src/codeflex/server/
+-rw-rw-rw-   0        0        0     2625 2024-04-21 22:18:00.000000 codeflex-3.0.0/src/codeflex/server/__init__.py
+-rw-rw-rw-   0        0        0       30 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/__main__.py
+-rw-rw-rw-   0        0        0    59702 2024-04-21 22:18:02.000000 codeflex-3.0.0/src/codeflex/server/app.py
+-rw-rw-rw-   0        0        0     3156 2024-04-21 22:18:03.000000 codeflex-3.0.0/src/codeflex/server/blueprints.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:24:54.478585 codeflex-3.0.0/src/codeflex/server/cero/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-3.0.0/src/codeflex/server/cero/__init__.py
+-rw-rw-rw-   0        0        0    38209 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/cero/app.py
+-rw-rw-rw-   0        0        0    24637 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/cero/blueprints.py
+-rw-rw-rw-   0        0        0    30879 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/cero/scaffold.py
+-rw-rw-rw-   0        0        0    35833 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/cli.py
+-rw-rw-rw-   0        0        0    13326 2024-04-21 22:18:04.000000 codeflex-3.0.0/src/codeflex/server/config.py
+-rw-rw-rw-   0        0        0    15120 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/ctx.py
+-rw-rw-rw-   0        0        0     6076 2024-04-21 22:18:05.000000 codeflex-3.0.0/src/codeflex/server/debughelpers.py
+-rw-rw-rw-   0        0        0     1713 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/globals.py
+-rw-rw-rw-   0        0        0    23084 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:24:54.494547 codeflex-3.0.0/src/codeflex/server/json/
+-rw-rw-rw-   0        0        0     5602 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/json/__init__.py
+-rw-rw-rw-   0        0        0     7646 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/json/provider.py
+-rw-rw-rw-   0        0        0     9280 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/json/tag.py
+-rw-rw-rw-   0        0        0     2375 2024-04-21 22:18:07.000000 codeflex-3.0.0/src/codeflex/server/logging.py
+-rw-rw-rw-   0        0        0        0 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/py.typed
+-rw-rw-rw-   0        0        0    14518 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/sessions.py
+-rw-rw-rw-   0        0        0      750 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/signals.py
+-rw-rw-rw-   0        0        0     7533 2024-04-21 22:18:08.000000 codeflex-3.0.0/src/codeflex/server/templating.py
+-rw-rw-rw-   0        0        0    10163 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/testing.py
+-rw-rw-rw-   0        0        0     3190 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/typing.py
+-rw-rw-rw-   0        0        0     6939 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/views.py
+-rw-rw-rw-   0        0        0     5831 2024-02-14 20:44:10.000000 codeflex-3.0.0/src/codeflex/server/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:24:54.503519 codeflex-3.0.0/src/codeflex/url/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-3.0.0/src/codeflex/url/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:24:54.597269 codeflex-3.0.0/src/codeflex/url/connect/
+-rw-rw-rw-   0        0        0     4963 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/__init__.py
+-rw-rw-rw-   0        0        0      435 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/__version__.py
+-rw-rw-rw-   0        0        0     1495 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/_internal_utils.py
+-rw-rw-rw-   0        0        0    19553 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/adapters.py
+-rw-rw-rw-   0        0        0     6449 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/api.py
+-rw-rw-rw-   0        0        0    10187 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/auth.py
+-rw-rw-rw-   0        0        0      429 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/certs.py
+-rw-rw-rw-   0        0        0     1451 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/compat.py
+-rw-rw-rw-   0        0        0    18560 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/cookies.py
+-rw-rw-rw-   0        0        0     3811 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/exceptions.py
+-rw-rw-rw-   0        0        0     3875 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/help.py
+-rw-rw-rw-   0        0        0      733 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/hooks.py
+-rw-rw-rw-   0        0        0    35223 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/models.py
+-rw-rw-rw-   0        0        0      957 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/packages.py
+-rw-rw-rw-   0        0        0    30373 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/sessions.py
+-rw-rw-rw-   0        0        0     4235 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/structures.py
+-rw-rw-rw-   0        0        0    33448 2024-02-14 20:45:27.000000 codeflex-3.0.0/src/codeflex/url/connect/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:24:54.601257 codeflex-3.0.0/src/codeflex.egg-info/
+-rw-rw-rw-   0        0        0     6238 2024-04-21 22:24:54.000000 codeflex-3.0.0/src/codeflex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1811 2024-04-21 22:24:54.000000 codeflex-3.0.0/src/codeflex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 22:24:54.000000 codeflex-3.0.0/src/codeflex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 22:24:54.000000 codeflex-3.0.0/src/codeflex.egg-info/top_level.txt
```

### Comparing `codeflex-2.1.1/LICENSE` & `codeflex-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/PKG-INFO` & `codeflex-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflex
-Version: 2.1.1
+Version: 3.0.0
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
-Metadata-Version: 2.1 Name: codeflex Version: 2.1.1 Summary: Â¡Conecta a los
+Metadata-Version: 2.1 Name: codeflex Version: 3.0.0 Summary: Â¡Conecta a los
 Microservicios de CodeFlex desde una Sola LibrerÃ­a! Home-page: https://
 codeflex.com.co/ Author: CODEFLEX S.A.S. Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by
 applicable copyright laws. The distribution and use of this software are
 subject to the terms and conditions outlined below. Project-URL: Bug Tracker,
 https://docs.codeflex.com.co/ Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `codeflex-2.1.1/README.md` & `codeflex-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/setup.py` & `codeflex-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="codeflex",
-    version="2.1.1",
+    version="3.0.0",
     author="CODEFLEX S.A.S.", 
     author_email="info@codeflex.com.co",
     license="This software is owned by CodeFlex S.A.S. and is protected by applicable copyright laws. The distribution and use of this software are subject to the terms and conditions outlined below.",
     description="¡Conecta a los Microservicios de CodeFlex desde una Sola Librería!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://codeflex.com.co/",
```

### Comparing `codeflex-2.1.1/src/codeflex/company/mysql.py` & `codeflex-3.0.0/src/codeflex/company/mysql.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/company/polly.py` & `codeflex-3.0.0/src/codeflex/company/polly.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/__init__.py` & `codeflex-3.0.0/src/codeflex/server/__init__.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/app.py` & `codeflex-3.0.0/src/codeflex/server/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 from .globals import request
 from .globals import request_ctx
 from .globals import session
 from .helpers import get_debug_flag
 from .helpers import get_flashed_messages
 from .helpers import get_load_dotenv
 from .helpers import send_from_directory
-from .sansio.app import App
-from .sansio.scaffold import _sentinel
+from .cero.app import App
+from .cero.scaffold import _sentinel
 from .sessions import SecureCookieSessionInterface
 from .sessions import SessionInterface
 from .signals import appcontext_tearing_down
 from .signals import got_request_exception
 from .signals import request_finished
 from .signals import request_started
 from .signals import request_tearing_down
```

### Comparing `codeflex-2.1.1/src/codeflex/server/blueprints.py` & `codeflex-3.0.0/src/codeflex/server/blueprints.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import os
 import typing as t
 from datetime import timedelta
 
 from .globals import current_app
 from .helpers import send_from_directory
-from .sansio.blueprints import Blueprint as SansioBlueprint
-from .sansio.blueprints import BlueprintSetupState as BlueprintSetupState  # noqa
+from .cero.blueprints import Blueprint as SansioBlueprint
+from .cero.blueprints import BlueprintSetupState as BlueprintSetupState  # noqa
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from .wrappers import Response
 
 
 class Blueprint(SansioBlueprint):
     def get_send_file_max_age(self, filename: str | None) -> int | None:
```

### Comparing `codeflex-2.1.1/src/codeflex/server/cli.py` & `codeflex-3.0.0/src/codeflex/server/cli.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/config.py` & `codeflex-3.0.0/src/codeflex/server/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import typing as t
 
 from werkzeug.utils import import_string
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
 
-    from .sansio.app import App
+    from .cero.app import App
 
 
 T = t.TypeVar("T")
 
 
 class ConfigAttribute(t.Generic[T]):
     """Makes an attribute forward to the config"""
```

### Comparing `codeflex-2.1.1/src/codeflex/server/ctx.py` & `codeflex-3.0.0/src/codeflex/server/ctx.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/debughelpers.py` & `codeflex-3.0.0/src/codeflex/server/debughelpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import typing as t
 
 from jinja2.loaders import BaseLoader
 from werkzeug.routing import RequestRedirect
 
 from .blueprints import Blueprint
 from .globals import request_ctx
-from .sansio.app import App
+from .cero.app import App
 
 if t.TYPE_CHECKING:
-    from .sansio.scaffold import Scaffold
+    from .cero.scaffold import Scaffold
     from .wrappers import Request
 
 
 class UnexpectedUnicodeError(AssertionError, UnicodeError):
     """Raised in places where we want some better error reporting for
     unexpected unicode or binary data.
     """
```

### Comparing `codeflex-2.1.1/src/codeflex/server/globals.py` & `codeflex-3.0.0/src/codeflex/server/globals.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/helpers.py` & `codeflex-3.0.0/src/codeflex/server/helpers.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/json/__init__.py` & `codeflex-3.0.0/src/codeflex/server/json/__init__.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/json/provider.py` & `codeflex-3.0.0/src/codeflex/server/json/provider.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/json/tag.py` & `codeflex-3.0.0/src/codeflex/server/json/tag.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/logging.py` & `codeflex-3.0.0/src/codeflex/server/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import typing as t
 
 from werkzeug.local import LocalProxy
 
 from .globals import request
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from .sansio.app import App
+    from .cero.app import App
 
 
 @LocalProxy
 def wsgi_errors_stream() -> t.TextIO:
     """Find the most appropriate error stream for the application. If a request
     is active, log to ``wsgi.errors``, otherwise use ``sys.stderr``.
```

### Comparing `codeflex-2.1.1/src/codeflex/server/sessions.py` & `codeflex-3.0.0/src/codeflex/server/sessions.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/signals.py` & `codeflex-3.0.0/src/codeflex/server/signals.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/templating.py` & `codeflex-3.0.0/src/codeflex/server/templating.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from .globals import request
 from .helpers import stream_with_context
 from .signals import before_render_template
 from .signals import template_rendered
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from .app import Flask
-    from .sansio.app import App
-    from .sansio.scaffold import Scaffold
+    from .cero.app import App
+    from .cero.scaffold import Scaffold
 
 
 def _default_template_ctx_processor() -> dict[str, t.Any]:
     """Default template context processor.  Injects `request`,
     `session` and `g`.
     """
     appctx = _cv_app.get(None)
```

### Comparing `codeflex-2.1.1/src/codeflex/server/testing.py` & `codeflex-3.0.0/src/codeflex/server/testing.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/typing.py` & `codeflex-3.0.0/src/codeflex/server/typing.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/views.py` & `codeflex-3.0.0/src/codeflex/server/views.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex/server/wrappers.py` & `codeflex-3.0.0/src/codeflex/server/wrappers.py`

 * *Files identical despite different names*

### Comparing `codeflex-2.1.1/src/codeflex.egg-info/PKG-INFO` & `codeflex-3.0.0/src/codeflex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflex
-Version: 2.1.1
+Version: 3.0.0
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
-Metadata-Version: 2.1 Name: codeflex Version: 2.1.1 Summary: Â¡Conecta a los
+Metadata-Version: 2.1 Name: codeflex Version: 3.0.0 Summary: Â¡Conecta a los
 Microservicios de CodeFlex desde una Sola LibrerÃ­a! Home-page: https://
 codeflex.com.co/ Author: CODEFLEX S.A.S. Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by
 applicable copyright laws. The distribution and use of this software are
 subject to the terms and conditions outlined below. Project-URL: Bug Tracker,
 https://docs.codeflex.com.co/ Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

