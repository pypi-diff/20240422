# Comparing `tmp/niquests-3.6.0.tar.gz` & `tmp/niquests-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Apr 20 06:44:55 2024, max compression
+gzip compressed data, last modified: Mon Apr 22 05:40:24 2024, max compression
```

## Comparing `niquests-3.6.0.tar` & `niquests-3.6.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      718 2024-04-20 06:44:55.000000 niquests-3.6.0/AUTHORS.rst
--rw-r--r--   0        0        0    85857 2024-04-20 06:44:55.000000 niquests-3.6.0/HISTORY.md
--rw-r--r--   0        0        0      377 2024-04-20 06:44:55.000000 niquests-3.6.0/Makefile
--rw-r--r--   0        0        0       38 2024-04-20 06:44:55.000000 niquests-3.6.0/NOTICE
--rw-r--r--   0        0        0        1 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/.nojekyll
--rw-r--r--   0        0        0     7664 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/Makefile
--rw-r--r--   0        0        0     5355 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/api.rst
--rw-r--r--   0        0        0    12305 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/conf.py
--rw-r--r--   0        0        0     4084 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/index.rst
--rw-r--r--   0        0        0     7253 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/make.bat
--rw-r--r--   0        0        0      185 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/requirements.txt
--rw-r--r--   0        0        0     2990 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/_static/custom.css
--rw-r--r--   0        0        0   306086 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/_static/requests-sidebar.png
--rw-r--r--   0        0        0     7360 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/faq.rst
--rw-r--r--   0        0        0     2720 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/recommended.rst
--rw-r--r--   0        0        0     1782 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/release-process.rst
--rw-r--r--   0        0        0      285 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/support.rst
--rw-r--r--   0        0        0      324 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/updates.rst
--rw-r--r--   0        0        0      945 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/community/vulnerabilities.rst
--rw-r--r--   0        0        0       48 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/dev/authors.rst
--rw-r--r--   0        0        0     5768 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/dev/contributing.rst
--rw-r--r--   0        0        0     1885 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/dev/migrate.rst
--rw-r--r--   0        0        0    52818 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/user/advanced.rst
--rw-r--r--   0        0        0     6315 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/user/authentication.rst
--rw-r--r--   0        0        0     1046 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/user/install.rst
--rw-r--r--   0        0        0    34594 2024-04-20 06:44:55.000000 niquests-3.6.0/docs/user/quickstart.rst
--rw-r--r--   0        0        0     3071 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/__init__.py
--rw-r--r--   0        0        0      534 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/__version__.py
--rw-r--r--   0        0        0    47149 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/_async.py
--rw-r--r--   0        0        0     2189 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/_compat.py
--rw-r--r--   0        0        0      480 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/_constant.py
--rw-r--r--   0        0        0     5942 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/_typing.py
--rw-r--r--   0        0        0    86853 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/adapters.py
--rw-r--r--   0        0        0    27567 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/api.py
--rw-r--r--   0        0        0     9906 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/auth.py
--rw-r--r--   0        0        0    19797 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/cookies.py
--rw-r--r--   0        0        0     4363 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/exceptions.py
--rw-r--r--   0        0        0     5119 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/help.py
--rw-r--r--   0        0        0     2776 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/hooks.py
--rw-r--r--   0        0        0    62438 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/models.py
--rw-r--r--   0        0        0        0 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/py.typed
--rw-r--r--   0        0        0    69113 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/sessions.py
--rw-r--r--   0        0        0     4284 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/status_codes.py
--rw-r--r--   0        0        0     6973 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/structures.py
--rw-r--r--   0        0        0    37300 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/utils.py
--rw-r--r--   0        0        0      119 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/extensions/__init__.py
--rw-r--r--   0        0        0    22384 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/extensions/_async_ocsp.py
--rw-r--r--   0        0        0    21009 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/extensions/_ocsp.py
--rw-r--r--   0        0        0    16942 2024-04-20 06:44:55.000000 niquests-3.6.0/src/niquests/extensions/_picotls.py
--rw-r--r--   0        0        0       80 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/__init__.py
--rw-r--r--   0        0        0     2193 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/conftest.py
--rw-r--r--   0        0        0     7540 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_async.py
--rw-r--r--   0        0        0      875 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_help.py
--rw-r--r--   0        0        0      893 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_hooks.py
--rw-r--r--   0        0        0     4022 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_live.py
--rw-r--r--   0        0        0    15985 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_lowlevel.py
--rw-r--r--   0        0        0     3722 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_multiplexed.py
--rw-r--r--   0        0        0    98955 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_requests.py
--rw-r--r--   0        0        0     2593 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_structures.py
--rw-r--r--   0        0        0     6213 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_testserver.py
--rw-r--r--   0        0        0    26728 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/test_utils.py
--rw-r--r--   0        0        0      613 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/utils.py
--rw-r--r--   0        0        0        0 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/testserver/__init__.py
--rw-r--r--   0        0        0     3882 2024-04-20 06:44:55.000000 niquests-3.6.0/tests/testserver/server.py
--rw-r--r--   0        0        0      362 2024-04-20 06:44:55.000000 niquests-3.6.0/.gitignore
--rw-r--r--   0        0        0    10142 2024-04-20 06:44:55.000000 niquests-3.6.0/LICENSE
--rw-r--r--   0        0        0    10931 2024-04-20 06:44:55.000000 niquests-3.6.0/README.md
--rw-r--r--   0        0        0     3660 2024-04-20 06:44:55.000000 niquests-3.6.0/pyproject.toml
--rw-r--r--   0        0        0    13292 2024-04-20 06:44:55.000000 niquests-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0      718 2024-04-22 05:40:24.000000 niquests-3.6.1/AUTHORS.rst
+-rw-r--r--   0        0        0    85995 2024-04-22 05:40:24.000000 niquests-3.6.1/HISTORY.md
+-rw-r--r--   0        0        0      377 2024-04-22 05:40:24.000000 niquests-3.6.1/Makefile
+-rw-r--r--   0        0        0       38 2024-04-22 05:40:24.000000 niquests-3.6.1/NOTICE
+-rw-r--r--   0        0        0        1 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/.nojekyll
+-rw-r--r--   0        0        0     7664 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/Makefile
+-rw-r--r--   0        0        0     5355 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/api.rst
+-rw-r--r--   0        0        0    12305 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/conf.py
+-rw-r--r--   0        0        0     4084 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/index.rst
+-rw-r--r--   0        0        0     7253 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/make.bat
+-rw-r--r--   0        0        0      185 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/requirements.txt
+-rw-r--r--   0        0        0     2990 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/_static/custom.css
+-rw-r--r--   0        0        0   306086 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/_static/requests-sidebar.png
+-rw-r--r--   0        0        0     7360 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/faq.rst
+-rw-r--r--   0        0        0     2720 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/recommended.rst
+-rw-r--r--   0        0        0     1782 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/release-process.rst
+-rw-r--r--   0        0        0      285 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/support.rst
+-rw-r--r--   0        0        0      324 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/updates.rst
+-rw-r--r--   0        0        0      945 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/community/vulnerabilities.rst
+-rw-r--r--   0        0        0       48 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/dev/authors.rst
+-rw-r--r--   0        0        0     5768 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/dev/contributing.rst
+-rw-r--r--   0        0        0     1885 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/dev/migrate.rst
+-rw-r--r--   0        0        0    52818 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/user/advanced.rst
+-rw-r--r--   0        0        0     6315 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/user/authentication.rst
+-rw-r--r--   0        0        0     1046 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/user/install.rst
+-rw-r--r--   0        0        0    34594 2024-04-22 05:40:24.000000 niquests-3.6.1/docs/user/quickstart.rst
+-rw-r--r--   0        0        0     3071 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/__init__.py
+-rw-r--r--   0        0        0      534 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/__version__.py
+-rw-r--r--   0        0        0    47149 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/_async.py
+-rw-r--r--   0        0        0     2852 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/_compat.py
+-rw-r--r--   0        0        0      480 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/_constant.py
+-rw-r--r--   0        0        0     5942 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/_typing.py
+-rw-r--r--   0        0        0    86853 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/adapters.py
+-rw-r--r--   0        0        0    27567 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/api.py
+-rw-r--r--   0        0        0     9906 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/auth.py
+-rw-r--r--   0        0        0    19797 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/cookies.py
+-rw-r--r--   0        0        0     4363 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/exceptions.py
+-rw-r--r--   0        0        0     5245 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/help.py
+-rw-r--r--   0        0        0     2776 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/hooks.py
+-rw-r--r--   0        0        0    62438 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/models.py
+-rw-r--r--   0        0        0        0 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/py.typed
+-rw-r--r--   0        0        0    69113 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/sessions.py
+-rw-r--r--   0        0        0     4284 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/status_codes.py
+-rw-r--r--   0        0        0     6973 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/structures.py
+-rw-r--r--   0        0        0    37300 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/utils.py
+-rw-r--r--   0        0        0      119 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/extensions/__init__.py
+-rw-r--r--   0        0        0    22384 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/extensions/_async_ocsp.py
+-rw-r--r--   0        0        0    21009 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/extensions/_ocsp.py
+-rw-r--r--   0        0        0    16942 2024-04-22 05:40:24.000000 niquests-3.6.1/src/niquests/extensions/_picotls.py
+-rw-r--r--   0        0        0       80 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     2193 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/conftest.py
+-rw-r--r--   0        0        0     7540 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_async.py
+-rw-r--r--   0        0        0      875 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_help.py
+-rw-r--r--   0        0        0      893 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_hooks.py
+-rw-r--r--   0        0        0     4022 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_live.py
+-rw-r--r--   0        0        0    15985 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_lowlevel.py
+-rw-r--r--   0        0        0     3722 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_multiplexed.py
+-rw-r--r--   0        0        0    99099 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_requests.py
+-rw-r--r--   0        0        0     2725 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_structures.py
+-rw-r--r--   0        0        0     6213 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_testserver.py
+-rw-r--r--   0        0        0    26728 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/test_utils.py
+-rw-r--r--   0        0        0      613 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/testserver/__init__.py
+-rw-r--r--   0        0        0     3882 2024-04-22 05:40:24.000000 niquests-3.6.1/tests/testserver/server.py
+-rw-r--r--   0        0        0      362 2024-04-22 05:40:24.000000 niquests-3.6.1/.gitignore
+-rw-r--r--   0        0        0    10142 2024-04-22 05:40:24.000000 niquests-3.6.1/LICENSE
+-rw-r--r--   0        0        0    10931 2024-04-22 05:40:24.000000 niquests-3.6.1/README.md
+-rw-r--r--   0        0        0     3660 2024-04-22 05:40:24.000000 niquests-3.6.1/pyproject.toml
+-rw-r--r--   0        0        0    13292 2024-04-22 05:40:24.000000 niquests-3.6.1/PKG-INFO
```

### Comparing `niquests-3.6.0/AUTHORS.rst` & `niquests-3.6.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/HISTORY.md` & `niquests-3.6.1/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Release History
 ===============
 
+3.6.1 (2024-04-22)
+------------------
+
+**Fixed**
+- Handling broken environments with a graceful exception with a detailed error message.
+
 3.6.0 (2024-04-20)
 ------------------
 
 **Added**
 - Support for qh3 version 1.0.0
   This qh3 release enable a greater flexibility by dropping cryptography. We had to adapt the OCSP code as we
   relied on cryptography. HTTP/3 experience is greatly improved.
```

### Comparing `niquests-3.6.0/docs/Makefile` & `niquests-3.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/api.rst` & `niquests-3.6.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/conf.py` & `niquests-3.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/index.rst` & `niquests-3.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/make.bat` & `niquests-3.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/_static/custom.css` & `niquests-3.6.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/_static/requests-sidebar.png` & `niquests-3.6.1/docs/_static/requests-sidebar.png`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/community/faq.rst` & `niquests-3.6.1/docs/community/faq.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/community/recommended.rst` & `niquests-3.6.1/docs/community/recommended.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/community/release-process.rst` & `niquests-3.6.1/docs/community/release-process.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/community/vulnerabilities.rst` & `niquests-3.6.1/docs/community/vulnerabilities.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/dev/contributing.rst` & `niquests-3.6.1/docs/dev/contributing.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/dev/migrate.rst` & `niquests-3.6.1/docs/dev/migrate.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/user/advanced.rst` & `niquests-3.6.1/docs/user/advanced.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/user/authentication.rst` & `niquests-3.6.1/docs/user/authentication.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/user/install.rst` & `niquests-3.6.1/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/docs/user/quickstart.rst` & `niquests-3.6.1/docs/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/__init__.py` & `niquests-3.6.1/src/niquests/__init__.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/__version__.py` & `niquests-3.6.1/src/niquests/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 __title__: str = "niquests"
 __description__: str = "Python HTTP for Humans."
 __url__: str = "https://niquests.readthedocs.io"
 
 __version__: str
-__version__ = "3.6.0"
+__version__ = "3.6.1"
 
-__build__: int = 0x030600
+__build__: int = 0x030601
 __author__: str = "Kenneth Reitz"
 __author_email__: str = "me@kennethreitz.org"
 __license__: str = "Apache-2.0"
 __copyright__: str = "Copyright Kenneth Reitz"
 __cake__: str = "\u2728 \U0001f370 \u2728"
```

### Comparing `niquests-3.6.0/src/niquests/_async.py` & `niquests-3.6.1/src/niquests/_async.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/_compat.py` & `niquests-3.6.1/src/niquests/_compat.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,18 +15,37 @@
 if HAS_LEGACY_URLLIB3:
     import urllib3_future
 else:
     urllib3_future = None  # type: ignore[assignment]
 
 try:
     import urllib3
-except ImportError:
+
+    # force detect broken or dummy urllib3 package
+    urllib3.Timeout  # noqa
+    urllib3.Retry  # noqa
+    urllib3.__version__  # noqa
+except (ImportError, AttributeError):
     urllib3 = None  # type: ignore[assignment]
 
-T = typing.TypeVar("T", urllib3.Timeout, urllib3.Retry)
+
+if (urllib3 is None and urllib3_future is None) or (
+    HAS_LEGACY_URLLIB3 and urllib3_future is None
+):
+    raise RuntimeError(
+        "This is awkward but your environment is missing urllib3-future. "
+        "Your environment seems broken. "
+        "You may fix this issue by running `python -m pip install niquests -U` "
+        "to force reinstall its dependencies."
+    )
+
+if urllib3 is not None:
+    T = typing.TypeVar("T", urllib3.Timeout, urllib3.Retry)
+else:
+    T = typing.TypeVar("T", urllib3_future.Timeout, urllib3_future.Retry)  # type: ignore
 
 
 def urllib3_ensure_type(o: T) -> T:
     """Retry, Timeout must be the one in urllib3_future."""
     if urllib3 is None:
         return o
```

### Comparing `niquests-3.6.0/src/niquests/_typing.py` & `niquests-3.6.1/src/niquests/_typing.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/adapters.py` & `niquests-3.6.1/src/niquests/adapters.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/api.py` & `niquests-3.6.1/src/niquests/api.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/auth.py` & `niquests-3.6.1/src/niquests/auth.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/cookies.py` & `niquests-3.6.1/src/niquests/cookies.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/exceptions.py` & `niquests-3.6.1/src/niquests/exceptions.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/help.py` & `niquests-3.6.1/src/niquests/help.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 from . import RequestException
 from . import __version__ as niquests_version
 from . import get
 from ._compat import HAS_LEGACY_URLLIB3
 
 if HAS_LEGACY_URLLIB3 is True:
     import urllib3_future as urllib3
-    from urllib3 import __version__ as __legacy_urllib3_version__
+
+    try:
+        from urllib3 import __version__ as __legacy_urllib3_version__
+    except (ImportError, AttributeError):
+        __legacy_urllib3_version__ = None  # type: ignore[assignment]
 else:
     import urllib3  # type: ignore[no-redef]
 
     __legacy_urllib3_version__ = None  # type: ignore[assignment]
 
 try:
     import qh3  # type: ignore
```

### Comparing `niquests-3.6.0/src/niquests/hooks.py` & `niquests-3.6.1/src/niquests/hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/models.py` & `niquests-3.6.1/src/niquests/models.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/sessions.py` & `niquests-3.6.1/src/niquests/sessions.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/status_codes.py` & `niquests-3.6.1/src/niquests/status_codes.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/structures.py` & `niquests-3.6.1/src/niquests/structures.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/utils.py` & `niquests-3.6.1/src/niquests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/extensions/_async_ocsp.py` & `niquests-3.6.1/src/niquests/extensions/_async_ocsp.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/extensions/_ocsp.py` & `niquests-3.6.1/src/niquests/extensions/_ocsp.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/src/niquests/extensions/_picotls.py` & `niquests-3.6.1/src/niquests/extensions/_picotls.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/tests/conftest.py` & `niquests-3.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/tests/test_async.py` & `niquests-3.6.1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/tests/test_help.py` & `niquests-3.6.1/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/tests/test_hooks.py` & `niquests-3.6.1/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/tests/test_live.py` & `niquests-3.6.1/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/tests/test_lowlevel.py` & `niquests-3.6.1/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/tests/test_multiplexed.py` & `niquests-3.6.1/tests/test_multiplexed.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/tests/test_requests.py` & `niquests-3.6.1/tests/test_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -2628,15 +2628,20 @@
         p.prepare(**kwargs)
     copy = p.copy()
     for attr in ("method", "url", "headers", "_cookies", "body", "hooks"):
         assert getattr(p, attr) == getattr(copy, attr)
 
 
 def test_urllib3_retries(httpbin):
-    from urllib3.util import Retry
+    from niquests._compat import HAS_LEGACY_URLLIB3
+
+    if not HAS_LEGACY_URLLIB3:
+        from urllib3.util import Retry
+    else:
+        from urllib3_future.util import Retry
 
     s = niquests.Session()
     s.mount("http://", HTTPAdapter(max_retries=Retry(total=2, status_forcelist=[500])))
 
     with pytest.raises(RetryError):
         s.get(httpbin("status/500"))
```

### Comparing `niquests-3.6.0/tests/test_structures.py` & `niquests-3.6.1/tests/test_structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from __future__ import annotations
 
 import pytest
 
 from niquests.structures import CaseInsensitiveDict, LookupDict
-from urllib3 import HTTPHeaderDict
+from niquests._compat import HAS_LEGACY_URLLIB3
+
+if not HAS_LEGACY_URLLIB3:
+    from urllib3 import HTTPHeaderDict
+else:
+    from urllib3_future import HTTPHeaderDict
 
 
 class TestCaseInsensitiveDict:
     @pytest.fixture(autouse=True)
     def setup(self):
         """CaseInsensitiveDict instance with "Accept" header."""
         self.case_insensitive_dict = CaseInsensitiveDict()
```

### Comparing `niquests-3.6.0/tests/test_testserver.py` & `niquests-3.6.1/tests/test_testserver.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/tests/test_utils.py` & `niquests-3.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/tests/utils.py` & `niquests-3.6.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/tests/testserver/server.py` & `niquests-3.6.1/tests/testserver/server.py`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/LICENSE` & `niquests-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/README.md` & `niquests-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/pyproject.toml` & `niquests-3.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `niquests-3.6.0/PKG-INFO` & `niquests-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: niquests
-Version: 3.6.0
+Version: 3.6.1
 Summary: Niquests is a simple, yet elegant, HTTP library. It is a drop-in replacement for Requests, which is under feature freeze.
 Project-URL: Changelog, https://github.com/jawah/niquests/blob/main/HISTORY.md
 Project-URL: Documentation, https://niquests.readthedocs.io
 Project-URL: Code, https://github.com/jawah/niquests
 Project-URL: Issue tracker, https://github.com/jawah/niquests/issues
 Author-email: Kenneth Reitz <me@kennethreitz.org>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
```

