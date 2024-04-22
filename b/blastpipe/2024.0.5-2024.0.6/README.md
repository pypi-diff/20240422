# Comparing `tmp/blastpipe-2024.0.5.tar.gz` & `tmp/blastpipe-2024.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.0.5.tar", last modified: Sun Apr 21 17:42:48 2024, max compression
+gzip compressed data, was "blastpipe-2024.0.6.tar", last modified: Mon Apr 22 01:17:15 2024, max compression
```

## Comparing `blastpipe-2024.0.5.tar` & `blastpipe-2024.0.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:42:48.214041 blastpipe-2024.0.5/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5869 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)    74141 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-21 17:42:48.214041 blastpipe-2024.0.5/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/mixin.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3175 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      122 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-21 17:37:06.000000 blastpipe-2024.0.5/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:17:15.121287 blastpipe-2024.0.6/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5869 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)    74391 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-22 01:17:15.121287 blastpipe-2024.0.6/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/mixin.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3183 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      122 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-22 01:11:29.000000 blastpipe-2024.0.6/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.0.5/.github/workflows/codeql.yml` & `blastpipe-2024.0.6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/.github/workflows/dependency-review.yml` & `blastpipe-2024.0.6/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/.github/workflows/ozi.yml` & `blastpipe-2024.0.6/.github/workflows/ozi.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/.github/workflows/scorecards.yml` & `blastpipe-2024.0.6/.github/workflows/scorecards.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/.gitignore` & `blastpipe-2024.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/CHANGELOG.md` & `blastpipe-2024.0.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # CHANGELOG
 
 
 
+## v2024.0.6 (2024-04-22)
+
+### :bug:
+
+* :bug: Fix minor rendering issues with requirements.
+
+Signed-off-by: rjdbcm &lt;rjdbcm@mail.umkc.edu&gt; ([`2143ed6`](https://github.com/OZI-Project/blastpipe/commit/2143ed6f989eb7c405464d014b0e5a1339c22e93))
+
+
 ## v2024.0.5 (2024-04-21)
 
 ### :arrow_up:
 
 * :arrow_up: Bump actions/checkout from 4.1.1 to 4.1.3
 
 Bumps [actions/checkout](https://github.com/actions/checkout) from 4.1.1 to 4.1.3.
```

### Comparing `blastpipe-2024.0.5/LICENSE.txt` & `blastpipe-2024.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/NOTICE.md` & `blastpipe-2024.0.6/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/PKG-INFO` & `blastpipe-2024.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.0.5
+Version: 2024.0.6
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.5.tar.gz
+Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.6.tar.gz
 Requires-Python: >=3.10, <3.13
 Keywords: ozi,meson
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `blastpipe-2024.0.5/README.rst` & `blastpipe-2024.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/blastpipe/__init__.py` & `blastpipe-2024.0.6/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/blastpipe/backports.py` & `blastpipe-2024.0.6/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/blastpipe/backports.pyi` & `blastpipe-2024.0.6/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/blastpipe/buffer.py` & `blastpipe-2024.0.6/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/blastpipe/loop.py` & `blastpipe-2024.0.6/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/blastpipe/malloc.py` & `blastpipe-2024.0.6/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/blastpipe/meson.build` & `blastpipe-2024.0.6/blastpipe/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/blastpipe/mixin.py` & `blastpipe-2024.0.6/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/blastpipe/sequence.py` & `blastpipe-2024.0.6/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/blastpipe/tailcall.py` & `blastpipe-2024.0.6/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/meson.build` & `blastpipe-2024.0.6/meson.build`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     ]
 )
 python = pymod.find_installation()
 pkg_info_req = 'Requires-Dist: @0@'
 required = []
 foreach requirement : fs.read('requirements.in').split('\n')
     if requirement != '' and not requirement.startswith('#')
-        required += pkg_info_req.format(requirement)
+        required += pkg_info_req.format(requirement.strip())
     endif
 endforeach
 pyproject_config = configuration_data()
 pyproject_config.set(
     'PYTHON_VERSION_DIST',
     'py'+''.join(python.language_version().split('.'))
 )
```

### Comparing `blastpipe-2024.0.5/meson.options` & `blastpipe-2024.0.6/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/pyproject.toml` & `blastpipe-2024.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/subprojects/docs/LICENSE.txt` & `blastpipe-2024.0.6/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.0.6/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.0.6/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/subprojects/docs/_static/meson.build` & `blastpipe-2024.0.6/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/subprojects/docs/_templates/layout.html` & `blastpipe-2024.0.6/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/subprojects/docs/_templates/meson.build` & `blastpipe-2024.0.6/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/subprojects/docs/conf.cfg` & `blastpipe-2024.0.6/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/subprojects/docs/index.rst` & `blastpipe-2024.0.6/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/subprojects/docs/meson.build` & `blastpipe-2024.0.6/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/subprojects/docs/meson.options` & `blastpipe-2024.0.6/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/tests/meson.build` & `blastpipe-2024.0.6/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/tests/test_backports.py` & `blastpipe-2024.0.6/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/tests/test_fuzz.py` & `blastpipe-2024.0.6/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.5/tests/test_tailcall.py` & `blastpipe-2024.0.6/tests/test_tailcall.py`

 * *Files identical despite different names*

