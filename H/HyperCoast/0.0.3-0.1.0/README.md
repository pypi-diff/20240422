# Comparing `tmp/hypercoast-0.0.3.tar.gz` & `tmp/hypercoast-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercoast-0.0.3.tar", last modified: Sat Apr 20 15:28:00 2024, max compression
+gzip compressed data, was "hypercoast-0.1.0.tar", last modified: Mon Apr 22 02:58:36 2024, max compression
```

## Comparing `hypercoast-0.0.3.tar` & `hypercoast-0.1.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.765577 hypercoast-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.753577 hypercoast-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.757577 hypercoast-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.757577 hypercoast-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-20 15:27:50.000000 hypercoast-0.0.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.765577 hypercoast-0.0.3/HyperCoast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 15:28:00.000000 hypercoast-0.0.3/HyperCoast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-20 15:27:50.000000 hypercoast-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-20 15:27:50.000000 hypercoast-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-20 15:28:00.765577 hypercoast-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 15:27:50.000000 hypercoast-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.761577 hypercoast-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/emit.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.761577 hypercoast-0.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/hypercoast.md
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.761577 hypercoast-0.0.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-20 15:27:50.000000 hypercoast-0.0.3/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.765577 hypercoast-0.0.3/hypercoast/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-20 15:27:50.000000 hypercoast-0.0.3/hypercoast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-20 15:27:50.000000 hypercoast-0.0.3/hypercoast/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    37734 2024-04-20 15:27:50.000000 hypercoast-0.0.3/hypercoast/emit.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-20 15:27:50.000000 hypercoast-0.0.3/hypercoast/hypercoast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-20 15:27:50.000000 hypercoast-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-20 15:27:50.000000 hypercoast-0.0.3/pyproject-codespell.precommit-toml
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-20 15:27:50.000000 hypercoast-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-20 15:27:50.000000 hypercoast-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-20 15:27:50.000000 hypercoast-0.0.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 15:28:00.765577 hypercoast-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 15:28:00.765577 hypercoast-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 15:27:50.000000 hypercoast-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-20 15:27:50.000000 hypercoast-0.0.3/tests/test_hypercoast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:58:36.426568 hypercoast-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:58:36.418568 hypercoast-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:58:36.422568 hypercoast-0.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:58:36.422568 hypercoast-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-22 02:58:19.000000 hypercoast-0.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:58:36.426568 hypercoast-0.1.0/HyperCoast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-22 02:58:36.000000 hypercoast-0.1.0/HyperCoast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-22 02:58:36.000000 hypercoast-0.1.0/HyperCoast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 02:58:36.000000 hypercoast-0.1.0/HyperCoast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 02:58:36.000000 hypercoast-0.1.0/HyperCoast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-22 02:58:36.000000 hypercoast-0.1.0/HyperCoast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 02:58:36.000000 hypercoast-0.1.0/HyperCoast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 02:58:19.000000 hypercoast-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 02:58:19.000000 hypercoast-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-22 02:58:36.426568 hypercoast-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-22 02:58:19.000000 hypercoast-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:58:36.426568 hypercoast-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/emit.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:58:36.426568 hypercoast-0.1.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/hypercoast.md
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:58:36.426568 hypercoast-0.1.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/ui.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-22 02:58:19.000000 hypercoast-0.1.0/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:58:36.426568 hypercoast-0.1.0/hypercoast/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-22 02:58:19.000000 hypercoast-0.1.0/hypercoast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-22 02:58:19.000000 hypercoast-0.1.0/hypercoast/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37734 2024-04-22 02:58:19.000000 hypercoast-0.1.0/hypercoast/emit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-22 02:58:19.000000 hypercoast-0.1.0/hypercoast/hypercoast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-22 02:58:19.000000 hypercoast-0.1.0/hypercoast/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-22 02:58:19.000000 hypercoast-0.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-22 02:58:19.000000 hypercoast-0.1.0/pyproject-codespell.precommit-toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-22 02:58:19.000000 hypercoast-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 02:58:19.000000 hypercoast-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-22 02:58:19.000000 hypercoast-0.1.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 02:58:36.426568 hypercoast-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:58:36.426568 hypercoast-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 02:58:19.000000 hypercoast-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-22 02:58:19.000000 hypercoast-0.1.0/tests/test_hypercoast.py
```

### Comparing `hypercoast-0.0.3/.github/workflows/docs-build.yml` & `hypercoast-0.1.0/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/.github/workflows/docs.yml` & `hypercoast-0.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/.github/workflows/installation.yml` & `hypercoast-0.1.0/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/.github/workflows/macos.yml` & `hypercoast-0.1.0/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/.github/workflows/pypi.yml` & `hypercoast-0.1.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/.github/workflows/ubuntu.yml` & `hypercoast-0.1.0/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/.github/workflows/windows.yml` & `hypercoast-0.1.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/.gitignore` & `hypercoast-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/.pre-commit-config.yaml` & `hypercoast-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/HyperCoast.egg-info/PKG-INFO` & `hypercoast-0.1.0/HyperCoast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.0.3
+Version: 0.1.0
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hypercoast-0.0.3/HyperCoast.egg-info/SOURCES.txt` & `hypercoast-0.1.0/HyperCoast.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -30,16 +30,18 @@
 docs/common.md
 docs/contributing.md
 docs/emit.md
 docs/faq.md
 docs/hypercoast.md
 docs/index.md
 docs/installation.md
+docs/ui.md
 docs/usage.md
 docs/examples/intro.ipynb
 docs/overrides/main.html
 hypercoast/__init__.py
 hypercoast/common.py
 hypercoast/emit.py
 hypercoast/hypercoast.py
+hypercoast/ui.py
 tests/__init__.py
 tests/test_hypercoast.py
```

### Comparing `hypercoast-0.0.3/LICENSE` & `hypercoast-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/PKG-INFO` & `hypercoast-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.0.3
+Version: 0.1.0
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hypercoast-0.0.3/README.md` & `hypercoast-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/docs/contributing.md` & `hypercoast-0.1.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/docs/index.md` & `hypercoast-0.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/docs/installation.md` & `hypercoast-0.1.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/hypercoast/emit.py` & `hypercoast-0.1.0/hypercoast/emit.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.0.3/mkdocs.yml` & `hypercoast-0.1.0/mkdocs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -81,7 +81,8 @@
     - Report Issues: https://github.com/opengeos/HyperCoast/issues
     - Examples:
           - examples/intro.ipynb
     - API Reference:
           - common module: common.md
           - emit module: emit.md
           - hypercoast module: hypercoast.md
+          - ui module: ui.md
```

### Comparing `hypercoast-0.0.3/pyproject.toml` & `hypercoast-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HyperCoast"
-version = "0.0.3"
+version = "0.1.0"
 dynamic = [
     "dependencies",
 ]
 description = "A Python package for processing hyperspectral data in coastal regions"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.3"
+current_version = "0.1.0"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

