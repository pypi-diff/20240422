# Comparing `tmp/koyo-0.2.7.tar.gz` & `tmp/koyo-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koyo-0.2.7.tar", last modified: Fri Feb  2 10:28:59 2024, max compression
+gzip compressed data, was "koyo-0.2.8.tar", last modified: Wed Feb 21 22:32:11 2024, max compression
```

## Comparing `koyo-0.2.7.tar` & `koyo-0.2.8.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:28:59.930637 koyo-0.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:28:59.918637 koyo-0.2.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-02 10:28:45.000000 koyo-0.2.7/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-02 10:28:45.000000 koyo-0.2.7/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-02 10:28:45.000000 koyo-0.2.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:28:59.918637 koyo-0.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-02-02 10:28:45.000000 koyo-0.2.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-02 10:28:45.000000 koyo-0.2.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-02 10:28:45.000000 koyo-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-02 10:28:45.000000 koyo-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-02-02 10:28:59.930637 koyo-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-02 10:28:45.000000 koyo-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-02-02 10:28:45.000000 koyo-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 10:28:59.930637 koyo-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:28:59.914637 koyo-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:28:59.926637 koyo-0.2.7/src/koyo/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-02 10:28:59.000000 koyo-0.2.7/src/koyo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/color.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/faulthandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/json_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/multicore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/pdf_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/rand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/release.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/spectrum_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/toml.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23970 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-02-02 10:28:45.000000 koyo-0.2.7/src/koyo/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:28:59.926637 koyo-0.2.7/src/koyo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-02-02 10:28:59.000000 koyo-0.2.7/src/koyo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-02 10:28:59.000000 koyo-0.2.7/src/koyo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 10:28:59.000000 koyo-0.2.7/src/koyo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-02 10:28:59.000000 koyo-0.2.7/src/koyo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-02 10:28:59.000000 koyo-0.2.7/src/koyo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 10:28:59.926637 koyo-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_koyo.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_rand.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-02-02 10:28:45.000000 koyo-0.2.7/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:32:11.280300 koyo-0.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:32:11.272300 koyo-0.2.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-21 22:31:58.000000 koyo-0.2.8/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-21 22:31:58.000000 koyo-0.2.8/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-21 22:31:58.000000 koyo-0.2.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:32:11.272300 koyo-0.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-02-21 22:31:58.000000 koyo-0.2.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-21 22:31:58.000000 koyo-0.2.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-21 22:31:58.000000 koyo-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-21 22:31:58.000000 koyo-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-02-21 22:32:11.280300 koyo-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-21 22:31:58.000000 koyo-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-02-21 22:31:58.000000 koyo-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 22:32:11.280300 koyo-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:32:11.268300 koyo-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:32:11.276300 koyo-0.2.8/src/koyo/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-21 22:32:11.000000 koyo-0.2.8/src/koyo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16000 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/faulthandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/json_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/multicore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/pdf_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/spectrum_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24388 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-02-21 22:31:58.000000 koyo-0.2.8/src/koyo/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:32:11.280300 koyo-0.2.8/src/koyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-02-21 22:32:11.000000 koyo-0.2.8/src/koyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-02-21 22:32:11.000000 koyo-0.2.8/src/koyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 22:32:11.000000 koyo-0.2.8/src/koyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-21 22:32:11.000000 koyo-0.2.8/src/koyo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-21 22:32:11.000000 koyo-0.2.8/src/koyo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:32:11.280300 koyo-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_koyo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-02-21 22:31:58.000000 koyo-0.2.8/tests/test_utilities.py
```

### Comparing `koyo-0.2.7/.github/workflows/ci.yml` & `koyo-0.2.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/.pre-commit-config.yaml` & `koyo-0.2.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/LICENSE` & `koyo-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/PKG-INFO` & `koyo-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koyo
-Version: 0.2.7
+Version: 0.2.8
 Summary: Simple python ulitities for various projects.
 Author-email: "Lukasz G. Migas" <lukas.migas@yahoo.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/vandeplaslab/koyo
 Project-URL: repository, https://github.com/vandeplaslab/koyo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `koyo-0.2.7/README.md` & `koyo-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/pyproject.toml` & `koyo-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/click.py` & `koyo-0.2.8/src/koyo/click.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Override click group to enable ordering."""
+
 import glob
 import os
 import sys
 import traceback
 import typing as ty
 from ast import literal_eval
 from pathlib import Path
@@ -207,14 +208,18 @@
     for cell in closure:
         if isinstance(cell.cell_contents, tuple):
             break
     ret = ""
     for value in cell.cell_contents:
         if isinstance(value, str) and value.startswith("-"):
             ret += value
+    # check if we can split the arguments
+    if "--" in ret:
+        rets = ret.split("--")
+        ret = "/".join(rets)
     return ret
 
 
 class Parameter:
     """Parameter object."""
 
     __slots__ = ["description", "args", "value"]
```

### Comparing `koyo-0.2.7/src/koyo/color.py` & `koyo-0.2.8/src/koyo/color.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/compression.py` & `koyo-0.2.8/src/koyo/compression.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/config.py` & `koyo-0.2.8/src/koyo/config.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/containers.py` & `koyo-0.2.8/src/koyo/containers.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/decorators.py` & `koyo-0.2.8/src/koyo/decorators.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/download.py` & `koyo-0.2.8/src/koyo/download.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/faulthandler.py` & `koyo-0.2.8/src/koyo/faulthandler.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/hooks.py` & `koyo-0.2.8/src/koyo/hooks.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/image.py` & `koyo-0.2.8/src/koyo/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,16 +103,20 @@
 ):
     """Batch reshape image."""
     if array.ndim != 2:
         raise ValueError("Expected 2-D array.")
     n = array.shape[1]
     dtype = np.float32 if np.isnan(fill_value) else array.dtype
     im = np.full((n, *image_shape), fill_value=fill_value, dtype=dtype)
-    for i in range(n):
-        im[i, coordinates[:, 1] - 1, coordinates[:, 0] - 1] = array[:, i]
+    try:
+        for i in range(n):
+            im[i, coordinates[:, 1] - 1, coordinates[:, 0] - 1] = array[:, i]
+    except IndexError:
+        for i in range(n):
+            im[i, coordinates[:, 0] - 1, coordinates[:, 1] - 1] = array[:, i]
     return im
 
 
 def get_coordinates_from_index(index: np.ndarray, shape: ty.Tuple[int, int]) -> np.ndarray:
     """Convert frame index to xy coordinates."""
     index = np.asarray(index)
     # generate image shape
```

### Comparing `koyo-0.2.7/src/koyo/json.py` & `koyo-0.2.8/src/koyo/json.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/json_cache.py` & `koyo-0.2.8/src/koyo/json_cache.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/mosaic.py` & `koyo-0.2.8/src/koyo/mosaic.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/multicore.py` & `koyo-0.2.8/src/koyo/multicore.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/numpy.py` & `koyo-0.2.8/src/koyo/numpy.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/path.py` & `koyo-0.2.8/src/koyo/path.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/pdf.py` & `koyo-0.2.8/src/koyo/pdf.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/pdf_mixin.py` & `koyo-0.2.8/src/koyo/pdf_mixin.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/release.py` & `koyo-0.2.8/src/koyo/release.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Check for latest release."""
+
 from __future__ import annotations
 
 import typing as ty
 
 import requests
 from loguru import logger
 
@@ -28,14 +29,15 @@
         return "win_amd64"
     elif platform.system() == "Darwin":
         if platform.processor() == "arm":
             return "macosx_arm64"
         return "macosx_x86_64"
     return None
 
+
 def get_latest_release(user: str = "vandeplaslab", package: str = "koyo") -> str:
     """Get latest release from GitHub."""
     data = get_latest_git(user, package)
     if "tag_name" in data:
         return data["tag_name"]
     return ""
```

### Comparing `koyo-0.2.7/src/koyo/secret.py` & `koyo-0.2.8/src/koyo/secret.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/sparse.py` & `koyo-0.2.8/src/koyo/sparse.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/spectrum.py` & `koyo-0.2.8/src/koyo/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Utilities for spectrum analysis."""
+
 import typing as ty
 from bisect import bisect_left, bisect_right
 
 import numba
 import numpy as np
-import scipy.signal
 import scipy.ndimage
+import scipy.signal
 
 from koyo.typing import SimpleArrayLike
 from koyo.utilities import find_nearest_index, find_nearest_index_batch
 
 
 def running_average(x: np.ndarray, size: int) -> np.ndarray:
     """Running average."""
```

### Comparing `koyo-0.2.7/src/koyo/spectrum_filters.py` & `koyo-0.2.8/src/koyo/spectrum_filters.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/timer.py` & `koyo-0.2.8/src/koyo/timer.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/toml.py` & `koyo-0.2.8/src/koyo/toml.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/typing.py` & `koyo-0.2.8/src/koyo/typing.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/src/koyo/utilities.py` & `koyo-0.2.8/src/koyo/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,39 @@
 """Generic utilities."""
+
 import re
 import typing as ty
 import unicodedata
 from collections.abc import Iterable
 from difflib import get_close_matches
 from math import ceil, floor
 
 import numba as nb
 import numpy as np
 from natsort import natsorted
 
 from koyo.typing import SimpleArrayLike
 
 
+def is_installed(module: str) -> bool:
+    """Try to import module."""
+    import importlib.util
+
+    try:
+        loader = importlib.util.find_spec(module)
+    except ModuleNotFoundError:
+        return False
+    return loader is not None
+
+
+def get_format(fmt: str) -> str:
+    """Parse format."""
+    return fmt if fmt.startswith(".") else f".{fmt}"
+
+
 def find_nearest_divisor(
     value: ty.Union[int, float],
     divisor: ty.Union[int, float] = 1,
     increment: ty.Union[int, float] = 1,
     max_iters: int = 1000,
 ) -> ty.Union[int, float]:
     """Find nearest divisor.
@@ -459,14 +476,15 @@
     zvals: np.array
         (potentially) transposed 2D heatmap
     """
     shape = array.shape
     if len(shape) == 3:
         return np.swapaxes(array, 1, 2) if shape[1] > shape[2] else array
     return array.T if shape[0] > shape[1] else array
+    # return np.rot90(array) if shape[0] > shape[1] else array
 
 
 def slugify(value, allow_unicode=False):
     """Convert to ASCII if 'allow_unicode' is False.
 
     Convert spaces or repeated dashes to single dashes. Remove characters that aren't alphanumerics, underscores,
     or hyphens. Convert to lowercase. Also strip leading and trailing whitespace, dashes, and underscores.
```

### Comparing `koyo-0.2.7/src/koyo/visuals.py` & `koyo-0.2.8/src/koyo/visuals.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,14 +100,18 @@
         divider = divider / 1000
     return len(str(int(divider))) - len(str(int(divider)).rstrip("0"))
 
 
 def convert_divider_to_str(value, exp_value):
     value = float(value)
     if exp_value in [0, 1, 2]:
+        if abs(value) < 0.0001:
+            return f"{value:.6G}"
+        if abs(value) < 0.01:
+            return f"{value:.4G}"
         if abs(value) <= 1:
             return f"{value:.2G}"
         elif abs(value) <= 1000:
             if value.is_integer():
                 return f"{value:.0F}"
             return f"{value:.1F}"
     elif exp_value in [3, 4, 5]:
@@ -146,14 +150,46 @@
     divider = make_axes_locatable(ax)
     cax = divider.append_axes("right", size="5%", pad=0.05)
     cbar = fig.colorbar(mappable, cax=cax)
     plt.sca(last_axes)
     return cbar
 
 
+def make_legend_handles(
+    names: list[str],
+    colors: list[str],
+    kind: list[str] = "line",
+    width: list[float] = 3,
+    extra_kws: dict = None,
+):
+    """Create custom legend."""
+    from matplotlib.lines import Line2D
+    from matplotlib.patches import Patch
+
+    extra_kws = extra_kws or {}
+    if isinstance(colors, (str, np.ndarray)):
+        colors = [colors] * len(names)
+    if isinstance(kind, str):
+        kind = [kind] * len(names)
+    if isinstance(width, (float, int)):
+        width = [width] * len(names)
+    handles = []
+    for name, color, kind_, width_ in zip(names, colors, kind, width):
+        kws = extra_kws.get(name, {})
+        if kind_ == "line":
+            handles.append(Line2D([0], [0], color=color, lw=width_, label=name, **kws))
+        elif kind_ == "patch":
+            handles.append(Patch(facecolor=color, edgecolor=color, label=name, **kws))
+        elif kind_ == "patch":
+            handles.append(Patch(facecolor=color, edgecolor=color, label=name, **kws))
+        else:
+            raise ValueError(f"Unknown kind {kind_}")
+    return handles
+
+
 def add_legend(
     fig,
     ax,
     legend_palettes: dict[str, dict[str, str]],
     fontsize: float = 14,
     labelsize: float = 16,
     x_pad: float = 0.01,
@@ -379,7 +415,27 @@
         style = "seaborn-ticks"
     if style.startswith("seaborn"):
         if "v0_8" not in style and "seaborn-v0_8" in available:
             style = style.replace("seaborn", "seaborn-v0_8")
     if style != "default":
         assert style in available, f"Style '{style}' not available. Available styles: {available}"
     return style
+
+
+def _annotate_heatmap(g, ax, mesh):
+    from seaborn.utils import relative_luminance
+
+    mesh.update_scalarmappable()
+    height, width = g.annot_data.shape
+    xpos, ypos = np.meshgrid(np.arange(width) + 0.5, np.arange(height) + 0.5)
+    for x, y, m, color, val in zip(xpos.flat, ypos.flat, mesh.get_array(), mesh.get_facecolors(), g.annot_data.flat):
+        if m is not np.ma.masked:
+            lum = relative_luminance(color)
+            text_color = ".15" if lum > 0.408 else "w"
+            annotation = f"{val:.2f}"
+            if val > 0:
+                annotation = "1" if annotation in "1.00" else annotation.replace("0.", ".")
+            else:
+                annotation = "-1" if annotation in "-1.00" else annotation.replace("0.", ".")
+            text_kwargs = dict(color=text_color, ha="center", va="center")
+            text_kwargs.update(g.annot_kws)
+            ax.text(x, y, annotation, **text_kwargs)
```

### Comparing `koyo-0.2.7/src/koyo.egg-info/PKG-INFO` & `koyo-0.2.8/src/koyo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koyo
-Version: 0.2.7
+Version: 0.2.8
 Summary: Simple python ulitities for various projects.
 Author-email: "Lukasz G. Migas" <lukas.migas@yahoo.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/vandeplaslab/koyo
 Project-URL: repository, https://github.com/vandeplaslab/koyo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `koyo-0.2.7/src/koyo.egg-info/SOURCES.txt` & `koyo-0.2.8/src/koyo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/koyo/logging.py
 src/koyo/mosaic.py
 src/koyo/multicore.py
 src/koyo/numpy.py
 src/koyo/path.py
 src/koyo/pdf.py
 src/koyo/pdf_mixin.py
+src/koyo/project.py
 src/koyo/py.typed
 src/koyo/rand.py
 src/koyo/release.py
 src/koyo/secret.py
 src/koyo/sparse.py
 src/koyo/spectrum.py
 src/koyo/spectrum_filters.py
```

### Comparing `koyo-0.2.7/tests/test_color.py` & `koyo-0.2.8/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/tests/test_containers.py` & `koyo-0.2.8/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/tests/test_image.py` & `koyo-0.2.8/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/tests/test_numpy.py` & `koyo-0.2.8/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/tests/test_secret.py` & `koyo-0.2.8/tests/test_secret.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/tests/test_timer.py` & `koyo-0.2.8/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/tests/test_toml.py` & `koyo-0.2.8/tests/test_toml.py`

 * *Files identical despite different names*

### Comparing `koyo-0.2.7/tests/test_utilities.py` & `koyo-0.2.8/tests/test_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,28 @@
     find_nearest_index_batch,
     find_nearest_index_single,
     find_nearest_value_single,
     format_size,
     get_kws,
     get_min_max,
     is_between,
+    is_installed,
     is_number,
     rescale,
     view_as_blocks,
 )
 from numpy.testing import assert_equal
 
 
+def test_is_installed():
+    assert is_installed("numpy")
+    assert is_installed("numpy.linalg")
+    assert not is_installed("not_installed_package")
+
+
 class TestViewAsBlocks:
     @staticmethod
     def test_wrong_block_dimension():
         A = np.arange(10)
         with pytest.raises(ValueError):
             view_as_blocks(A, 2, 2)
 
@@ -152,12 +159,12 @@
     good_shape = (2, 10)
     zvals = check_image_orientation(np.zeros(shape))
     assert zvals.shape == good_shape
 
 
 def test_format_size():
     assert "100" == format_size(100)
-    assert "1.0K" == format_size(2 ** 10)
-    assert "1.0M" == format_size(2 ** 20)
-    assert "1.0G" == format_size(2 ** 30)
-    assert "1.0T" == format_size(2 ** 40)
-    assert "1.0P" == format_size(2 ** 50)
+    assert "1.0K" == format_size(2**10)
+    assert "1.0M" == format_size(2**20)
+    assert "1.0G" == format_size(2**30)
+    assert "1.0T" == format_size(2**40)
+    assert "1.0P" == format_size(2**50)
```

