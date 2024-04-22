# Comparing `tmp/adafruit_circuitpython_irremote-5.0.0.tar.gz` & `tmp/adafruit_circuitpython_irremote-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_irremote-5.0.0.tar", last modified: Sun Apr 21 14:24:39 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_irremote-5.0.1.tar", last modified: Mon Apr 22 01:21:07 2024, max compression
```

## Comparing `adafruit_circuitpython_irremote-5.0.0.tar` & `adafruit_circuitpython_irremote-5.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.798521 adafruit_circuitpython_irremote-5.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.786522 adafruit_circuitpython_irremote-5.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.790521 adafruit_circuitpython_irremote-5.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.790521 adafruit_circuitpython_irremote-5.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-21 14:24:39.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-21 14:24:39.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 14:24:39.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 14:24:39.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-21 14:24:39.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-04-21 14:24:37.000000 adafruit_circuitpython_irremote-5.0.0/adafruit_irremote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:24:39.794521 adafruit_circuitpython_irremote-5.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-21 14:24:37.000000 adafruit_circuitpython_irremote-5.0.0/examples/irremote_nonblocking.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-21 14:24:37.000000 adafruit_circuitpython_irremote-5.0.0/examples/irremote_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-21 14:24:37.000000 adafruit_circuitpython_irremote-5.0.0/examples/irremote_transmit.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-21 14:24:37.000000 adafruit_circuitpython_irremote-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 14:24:29.000000 adafruit_circuitpython_irremote-5.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 14:24:39.798521 adafruit_circuitpython_irremote-5.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:21:07.903505 adafruit_circuitpython_irremote-5.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:21:07.895505 adafruit_circuitpython_irremote-5.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:21:07.899505 adafruit_circuitpython_irremote-5.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:21:07.899505 adafruit_circuitpython_irremote-5.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:21:07.899505 adafruit_circuitpython_irremote-5.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-22 01:21:07.903505 adafruit_circuitpython_irremote-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:21:07.903505 adafruit_circuitpython_irremote-5.0.1/adafruit_circuitpython_irremote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-22 01:21:07.000000 adafruit_circuitpython_irremote-5.0.1/adafruit_circuitpython_irremote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-22 01:21:07.000000 adafruit_circuitpython_irremote-5.0.1/adafruit_circuitpython_irremote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 01:21:07.000000 adafruit_circuitpython_irremote-5.0.1/adafruit_circuitpython_irremote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 01:21:07.000000 adafruit_circuitpython_irremote-5.0.1/adafruit_circuitpython_irremote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 01:21:07.000000 adafruit_circuitpython_irremote-5.0.1/adafruit_circuitpython_irremote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-04-22 01:21:05.000000 adafruit_circuitpython_irremote-5.0.1/adafruit_irremote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:21:07.903505 adafruit_circuitpython_irremote-5.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:21:07.903505 adafruit_circuitpython_irremote-5.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:21:07.903505 adafruit_circuitpython_irremote-5.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-22 01:21:05.000000 adafruit_circuitpython_irremote-5.0.1/examples/irremote_nonblocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-22 01:21:05.000000 adafruit_circuitpython_irremote-5.0.1/examples/irremote_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-22 01:21:05.000000 adafruit_circuitpython_irremote-5.0.1/examples/irremote_transmit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-22 01:21:05.000000 adafruit_circuitpython_irremote-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 01:20:56.000000 adafruit_circuitpython_irremote-5.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 01:21:07.903505 adafruit_circuitpython_irremote-5.0.1/setup.cfg
```

### Comparing `adafruit_circuitpython_irremote-5.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_irremote-5.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/.gitignore` & `adafruit_circuitpython_irremote-5.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/.pre-commit-config.yaml` & `adafruit_circuitpython_irremote-5.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/.pylintrc` & `adafruit_circuitpython_irremote-5.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_irremote-5.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/LICENSE` & `adafruit_circuitpython_irremote-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_irremote-5.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/LICENSES/MIT.txt` & `adafruit_circuitpython_irremote-5.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_irremote-5.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/PKG-INFO` & `adafruit_circuitpython_irremote-5.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-irremote
-Version: 5.0.0
+Version: 5.0.1
 Summary: CircuitPython library for infrared transmit and receive.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IRRemote
 Keywords: adafruit,infrared,transmit,receive,tx,rx,ir,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_irremote-5.0.0/README.rst` & `adafruit_circuitpython_irremote-5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/PKG-INFO` & `adafruit_circuitpython_irremote-5.0.1/adafruit_circuitpython_irremote.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-irremote
-Version: 5.0.0
+Version: 5.0.1
 Summary: CircuitPython library for infrared transmit and receive.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IRRemote
 Keywords: adafruit,infrared,transmit,receive,tx,rx,ir,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_irremote-5.0.0/adafruit_circuitpython_irremote.egg-info/SOURCES.txt` & `adafruit_circuitpython_irremote-5.0.1/adafruit_circuitpython_irremote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/adafruit_irremote.py` & `adafruit_circuitpython_irremote-5.0.1/adafruit_irremote.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the ESP8622 and M0-based boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
-__version__ = "5.0.0"
+__version__ = "5.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_IRRemote.git"
 
 
 class IRDecodeException(Exception):
     """Generic decode exception"""
```

### Comparing `adafruit_circuitpython_irremote-5.0.0/docs/_static/favicon.ico` & `adafruit_circuitpython_irremote-5.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/docs/conf.py` & `adafruit_circuitpython_irremote-5.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/docs/index.rst` & `adafruit_circuitpython_irremote-5.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/examples/irremote_nonblocking.py` & `adafruit_circuitpython_irremote-5.0.1/examples/irremote_nonblocking.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/examples/irremote_simpletest.py` & `adafruit_circuitpython_irremote-5.0.1/examples/irremote_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_irremote-5.0.0/examples/irremote_transmit.py` & `adafruit_circuitpython_irremote-5.0.1/examples/irremote_transmit.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 button.direction = digitalio.Direction.INPUT
 button.pull = digitalio.Pull.DOWN
 
 # Create a 'PulseOut' to send infrared signals on the IR transmitter @ 38KHz
 pulseout = pulseio.PulseOut(board.IR_TX, frequency=38000, duty_cycle=2**15)
 # Create an encoder that will take numbers and turn them into NEC IR pulses
 encoder = adafruit_irremote.GenericTransmit(
-    header=[9000, 4500], one=[560, 1700], zero=[560, 1700], trail=560
+    header=[9000, 4500], one=[560, 1700], zero=[560, 560], trail=560
 )
 
 while True:
     if button.value:
         print("IR signal sent!")
         encoder.transmit(pulseout, [255, 2, 255, 0])
         time.sleep(0.2)
```

### Comparing `adafruit_circuitpython_irremote-5.0.0/pyproject.toml` & `adafruit_circuitpython_irremote-5.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-irremote"
 description = "CircuitPython library for infrared transmit and receive."
-version = "5.0.0"
+version = "5.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_IRRemote"}
 keywords = [
     "adafruit",
```

