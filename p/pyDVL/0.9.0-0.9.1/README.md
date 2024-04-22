# Comparing `tmp/pydvl-0.9.tar.gz` & `tmp/pydvl-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydvl-0.9.tar", last modified: Fri Apr 12 18:13:02 2024, max compression
+gzip compressed data, was "pydvl-0.9.1.tar", last modified: Mon Apr 22 09:35:46 2024, max compression
```

## Comparing `pydvl-0.9.tar` & `pydvl-0.9.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.111592 pydvl-0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-12 18:11:37.000000 pydvl-0.9/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 18:11:37.000000 pydvl-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 18:11:37.000000 pydvl-0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-04-12 18:13:02.111592 pydvl-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-04-12 18:11:37.000000 pydvl-0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-12 18:11:37.000000 pydvl-0.9/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-12 18:11:37.000000 pydvl-0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-12 18:11:37.000000 pydvl-0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:13:02.111592 pydvl-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-12 18:11:37.000000 pydvl-0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.091592 pydvl-0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.107592 pydvl-0.9/src/pyDVL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.095592 pydvl-0.9/src/pydvl/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/influence/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/base_influence_function_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    28378 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/influence_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/influence/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38897 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/torch/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    64011 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/torch/influence_function_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/torch/pre_conditioner.py
--rw-r--r--   0 runner    (1001) docker     (127)    17841 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/torch/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/parallel/backends/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/backends/joblib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/backends/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/parallel/futures/
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/futures/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/reporting/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/reporting/scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.103592 pydvl-0.9/src/pydvl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.103592 pydvl-0.9/src/pydvl/utils/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/memcached.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.103592 pydvl-0.9/src/pydvl/value/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/games.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.103592 pydvl-0.9/src/pydvl/value/least_core/
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/least_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/least_core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/least_core/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/least_core/naive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.107592 pydvl-0.9/src/pydvl/value/loo/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/loo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/loo/loo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.107592 pydvl-0.9/src/pydvl/value/oob/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/oob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/oob/oob.py
--rw-r--r--   0 runner    (1001) docker     (127)    31283 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    33246 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/semivalues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.107592 pydvl-0.9/src/pydvl/value/shapley/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25074 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/classwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/gt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/knn.py
--rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/owen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/truncated.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28615 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.107592 pydvl-0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-12 18:11:37.000000 pydvl-0.9/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-04-12 18:11:37.000000 pydvl-0.9/tests/test_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.826394 pydvl-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-22 09:34:20.000000 pydvl-0.9.1/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 09:34:20.000000 pydvl-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-22 09:34:20.000000 pydvl-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-22 09:35:46.826394 pydvl-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-22 09:34:20.000000 pydvl-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-22 09:34:21.000000 pydvl-0.9.1/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-22 09:34:21.000000 pydvl-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-22 09:34:21.000000 pydvl-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:35:46.826394 pydvl-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-22 09:34:21.000000 pydvl-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.806394 pydvl-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.826394 pydvl-0.9.1/src/pyDVL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 09:35:46.000000 pydvl-0.9.1/src/pyDVL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/influence/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/base_influence_function_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28378 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/influence_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/influence/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38897 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/torch/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64263 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/torch/influence_function_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/torch/pre_conditioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17841 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/influence/torch/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/parallel/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/backends/joblib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/backends/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.814394 pydvl-0.9.1/src/pydvl/parallel/futures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/futures/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/parallel/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.818394 pydvl-0.9.1/src/pydvl/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/reporting/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/reporting/scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.818394 pydvl-0.9.1/src/pydvl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.818394 pydvl-0.9.1/src/pydvl/utils/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/caching/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/utils/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/src/pydvl/value/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/games.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/src/pydvl/value/least_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/least_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/least_core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/least_core/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/least_core/naive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/src/pydvl/value/loo/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/loo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/loo/loo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/src/pydvl/value/oob/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/oob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/oob/oob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31283 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33246 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/semivalues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/src/pydvl/value/shapley/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25074 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/classwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/owen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/shapley/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28615 2024-04-22 09:34:21.000000 pydvl-0.9.1/src/pydvl/value/stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:35:46.822394 pydvl-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-22 09:34:21.000000 pydvl-0.9.1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-04-22 09:34:21.000000 pydvl-0.9.1/tests/test_results.py
```

### Comparing `pydvl-0.9/COPYING.LESSER` & `pydvl-0.9.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/LICENSE` & `pydvl-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/PKG-INFO` & `pydvl-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDVL
-Version: 0.9.0
+Version: 0.9.1
 Summary: The Python Data Valuation Library
 Author: appliedAI Institute gGmbH
 Project-URL: Source, https://github.com/aai-institute/pydvl
 Project-URL: Documentation, https://pydvl.org
 Project-URL: TransferLab, https://transferlab.ai
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -57,28 +57,26 @@
     <a href="https://pydvl.org"><img src="https://img.shields.io/badge/docs-All%20versions-009485" alt="documentation"></a>
     <a href="https://raw.githubusercontent.com/aai-institute/pyDVL/master/LICENSE"><img alt="License" src="https://img.shields.io/pypi/l/pydvl"></a>
     <a href="https://github.com/aai-institute/pyDVL/actions/workflows/main.yaml"><img src="https://github.com/aai-institute/pyDVL/actions/workflows/main.yaml/badge.svg" alt="Build status" ></a>
     <a href="https://codecov.io/gh/aai-institute/pyDVL"><img src="https://codecov.io/gh/aai-institute/pyDVL/graph/badge.svg?token=VN7DNDE0FV"/></a>
     <a href="https://zenodo.org/badge/latestdoi/354117916"><img src="https://zenodo.org/badge/354117916.svg" alt="DOI"></a>
 </p>
 
-**pyDVL** collects algorithms for **Data Valuation** and **Influence Function** computation.
-
-Refer to the [Methods](https://pydvl.org/devel/getting-started/methods/)
-page of our documentation for a list of all implemented methods. 
+**pyDVL** collects algorithms for **Data Valuation** and **Influence Function**
+computation. Here is the list of [all methods implemented](https://pydvl.org/devel/getting-started/methods/).
 
 **Data Valuation** for machine learning is the task of assigning a scalar
 to each element of a training set which reflects its contribution to the final
 performance or outcome of some model trained on it. Some concepts of
 value depend on a specific model of interest, while others are model-agnostic.
 pyDVL focuses on model-dependent methods.
 
 <div align="center" style="text-align:center;">
     <img
-        width="70%"
+        width="60%"
         align="center"
         style="display: block; margin-left: auto; margin-right: auto;"
         src="https://pydvl.org/devel/value/img/mclc-best-removal-10k-natural.svg"
         alt="best sample removal"
     />
     <p align="center" style="text-align:center;">
         Comparison of different data valuation methods
@@ -89,15 +87,15 @@
 The **Influence Function** is an infinitesimal measure of the effect that single
 training points have over the parameters of a model, or any function thereof.
 In particular, in machine learning they are also used to compute the effect
 of training samples over individual test points.
 
 <div align="center" style="text-align:center;">
     <img
-        width="70%"
+        width="60%"
         align="center"
         style="display: block; margin-left: auto; margin-right: auto;"
         src="https://pydvl.org/devel/examples/img/influence_functions_example.png"
         alt="best sample removal"
     />
     <p align="center" style="text-align:center;">
         Influences of input points with corrupted data.
@@ -123,188 +121,141 @@
 pyDVL has also extra dependencies for certain functionalities, 
 e.g. for using influence functions run
 ```shell
 $ pip install pyDVL[influence]
 ```
 
 For more instructions and information refer to [Installing pyDVL
-](https://pydvl.org/stable/getting-started/#installation) in the
-documentation.
+](https://pydvl.org/stable/getting-started/#installation) in the documentation.
 
 # Usage
 
-In the following subsections, we will showcase the usage of pyDVL
-for Data Valuation and Influence Functions using simple examples.
-
-For more instructions and information refer to [Getting
-Started](https://pydvl.org/stable/getting-started/first-steps/) in
-the documentation.
-We provide several examples for data valuation
-(e.g. [Shapley Data Valuation](https://pydvl.org/stable/examples/shapley_basic_spotify/))
-and for influence functions
-(e.g. [Influence Functions for Neural Networks](https://pydvl.org/stable/examples/influence_imagenet/))
-with details on the algorithms and their applications.
+Please read [Getting
+Started](https://pydvl.org/stable/getting-started/first-steps/) in the
+documentation for more instructions. We provide several examples for data
+valuation and for influence functions in our [Example
+Gallery](https://pydvl.org/stable/examples/).
 
 ## Influence Functions
 
-For influence computation, follow these steps:
-
-1. Import the necessary packages (The exact packages depend on your specific use case).
-
-   ```python
-   import torch
-   from torch import nn
-   from torch.utils.data import DataLoader, TensorDataset
-   
-   from pydvl.influence.torch import DirectInfluence
-   from pydvl.influence.torch.util import NestedTorchCatAggregator, TorchNumpyConverter
-   from pydvl.influence import SequentialInfluenceCalculator
-   ```
-
+1. Import the necessary packages (the exact ones depend on your specific use case).
 2. Create PyTorch data loaders for your train and test splits.
-
-   ```python
-   input_dim = (5, 5, 5)
-   output_dim = 3
-   train_x = torch.rand((10, *input_dim))
-   train_y = torch.rand((10, output_dim))
-   test_x = torch.rand((5, *input_dim))
-   test_y = torch.rand((5, output_dim))
-
-   train_data_loader = DataLoader(TensorDataset(train_x, train_y), batch_size=2)
-   test_data_loader = DataLoader(TensorDataset(test_x, test_y), batch_size=1)
-   ```
-
-3. Instantiate your neural network model.
-
-   ```python
-   nn_architecture = nn.Sequential(
-     nn.Conv2d(in_channels=5, out_channels=3, kernel_size=3),
-     nn.Flatten(),
-     nn.Linear(27, 3),
+3. Instantiate your neural network model and define your loss function.
+4. Instantiate an `InfluenceFunctionModel` and fit it to the training data
+5. For small input data, you can call the `influences()` method on the fitted
+   instance. The result is a tensor of shape `(training samples, test samples)`
+   that contains at index `(i, j`) the influence of training sample `i` on
+   test sample `j`.
+6. For larger datasets, wrap the model into a "calculator" and call methods on
+   it. This splits the computation into smaller chunks and allows for lazy
+   evaluation and out-of-core computation.
+
+The higher the absolute value of the influence of a training sample
+on a test sample, the more influential it is for the chosen test sample, model
+and data loaders. The sign of the influence determines whether it is 
+useful (positive) or harmful (negative).
+
+> **Note** pyDVL currently only support PyTorch for Influence Functions. We plan
+> to add support for Jax next.
+
+```python
+import torch
+from torch import nn
+from torch.utils.data import DataLoader, TensorDataset
+
+from pydvl.influence import SequentialInfluenceCalculator
+from pydvl.influence.torch import DirectInfluence
+from pydvl.influence.torch.util import (
+   NestedTorchCatAggregator,
+   TorchNumpyConverter,
    )
-   ```
-
-4. Define your loss:
-
-   ```python
-   loss = nn.MSELoss()
-   ```
 
-5. Instantiate an `InfluenceFunctionModel` and fit it to the training data
+input_dim = (5, 5, 5)
+output_dim = 3
+train_x, train_y = torch.rand((10, *input_dim)), torch.rand((10, output_dim))
+test_x, test_y = torch.rand((5, *input_dim)), torch.rand((5, output_dim))
+train_data_loader = DataLoader(TensorDataset(train_x, train_y), batch_size=2)
+test_data_loader = DataLoader(TensorDataset(test_x, test_y), batch_size=1)
+model = nn.Sequential(
+  nn.Conv2d(in_channels=5, out_channels=3, kernel_size=3),
+  nn.Flatten(),
+  nn.Linear(27, 3),
+  )
+loss = nn.MSELoss()
+
+infl_model = DirectInfluence(model, loss, hessian_regularization=0.01)
+infl_model = infl_model.fit(train_data_loader)
+
+# For small datasets, instantiate the full influence matrix:
+influences = infl_model.influences(test_x, test_y, train_x, train_y)
+
+# For larger datasets, use the Influence calculators:
+infl_calc = SequentialInfluenceCalculator(infl_model)
 
-   ```python
-   infl_model = DirectInfluence(nn_architecture, loss, hessian_regularization=0.01)
-   infl_model = infl_model.fit(train_data_loader)
-   ```
+# Lazy object providing arrays batch-wise in a sequential manner
+lazy_influences = infl_calc.influences(test_data_loader, train_data_loader)
 
-6. For small input data call influence method on the fitted instance. 
-
-   ```python
-   influences = infl_model.influences(test_x, test_y, train_x, train_y)
-   ```
-   The result is a tensor of shape `(training samples x test samples)`
-   that contains at index `(i, j`) the influence of training sample `i` on
-   test sample `j`.
+# Trigger computation and pull results to memory
+influences = lazy_influences.compute(aggregator=NestedTorchCatAggregator())
 
-7. For larger data, wrap the model into a
-   calculator and call methods on the calculator.
-   ```python
-   infl_calc = SequentialInfluenceCalculator(infl_model)
-   
-    # Lazy object providing arrays batch-wise in a sequential manner
-   lazy_influences = infl_calc.influences(test_data_loader, train_data_loader)
-
-   # Trigger computation and pull results to memory
-   influences = lazy_influences.compute(aggregator=NestedTorchCatAggregator())
-
-   # Trigger computation and write results batch-wise to disk
-   lazy_influences.to_zarr("influences_result", TorchNumpyConverter())
-   ```
-   
-
-   The higher the absolute value of the influence of a training sample
-   on a test sample, the more influential it is for the chosen test sample, model
-   and data loaders. The sign of the influence determines whether it is 
-   useful (positive) or harmful (negative).
-
-> **Note** pyDVL currently only support PyTorch for Influence Functions. 
-> We are planning to add support for Jax and perhaps TensorFlow or even Keras.
+# Trigger computation and write results batch-wise to disk
+lazy_influences.to_zarr("influences_result", TorchNumpyConverter())
+```
 
 ## Data Valuation
 
 The steps required to compute data values for your samples are:
 
-1. Import the necessary packages (The exact packages depend on your specific use case).
-
-   ```python
-   import matplotlib.pyplot as plt
-   from sklearn.datasets import load_breast_cancer
-   from sklearn.linear_model import LogisticRegression
-   from pydvl.utils import Dataset, Scorer, Utility
-   from pydvl.value import (
-      compute_shapley_values,
-      ShapleyMode,
-      MaxUpdates,
-   )
-   ```
- 
+1. Import the necessary packages (the exact ones will depend on your specific
+   use case).
 2. Create a `Dataset` object with your train and test splits.
-
-   ```python
-   data = Dataset.from_sklearn(
-       load_breast_cancer(),
-       train_size=10,
-       stratify_by_target=True,
-       random_state=16,
-   )
-   ```
-
 3. Create an instance of a `SupervisedModel` (basically any sklearn compatible
-   predictor).
-
-   ```python
-   model = LogisticRegression()
-   ```  
-
-4. Create a `Utility` object to wrap the Dataset, the model and a scoring
-   function.
-
-   ```python
-   u = Utility(
-      model,
-      data,
-      Scorer("accuracy", default=0.0)
-   )
-   ```
-
-5. Use one of the methods defined in the library to compute the values.
-   In our example, we will use *Permutation Montecarlo Shapley*,
-   an approximate method for computing Data Shapley values.
-
-   ```python
-   values = compute_shapley_values(
-      u,
-      mode=ShapleyMode.PermutationMontecarlo,
-      done=MaxUpdates(100),
-      seed=16,  
-      progress=True
-   )
-   ```
-   The result is a variable of type `ValuationResult` that contains
-   the indices and their values as well as other attributes.
-
-   The higher the value for an index, the more important it is for the chosen
-   model, dataset and scorer.
-
-6. (Optional) Convert the valuation result to a dataframe and analyze and visualize the values.
-
-   ```python
-   df = values.to_dataframe(column="data_value")
-   ```
+   predictor), and wrap it in a `Utility` object together with the data and a
+   scoring function.
+4. Use one of the methods defined in the library to compute the values. In the
+   example below, we will use *Permutation Montecarlo Shapley*, an approximate
+   method for computing Data Shapley values. The result is a variable of type
+   `ValuationResult` that contains the indices and their values as well as other
+   attributes.
+5. Convert the valuation result to a dataframe, and analyze and visualize the
+   values.
+
+The higher the value for an index, the more important it is for the chosen
+model, dataset and scorer. Reciprocally, low-value points could be mislabelled,
+or out-of-distribution, and dropping them can improve the model's performance.
+
+```python
+from sklearn.datasets import load_breast_cancer
+from sklearn.linear_model import LogisticRegression
+
+from pydvl.utils import Dataset, Scorer, Utility
+from pydvl.value import (MaxUpdates, RelativeTruncation,
+                         permutation_montecarlo_shapley)
+
+data = Dataset.from_sklearn(
+  load_breast_cancer(),
+  train_size=10,
+  stratify_by_target=True,
+  random_state=16,
+  )
+model = LogisticRegression()
+u = Utility(
+  model,
+  data,
+  Scorer("accuracy", default=0.0)
+  )
+values = permutation_montecarlo_shapley(
+  u,
+  truncation=RelativeTruncation(u, 0.05),
+  done=MaxUpdates(1000),
+  seed=16,
+  progress=True
+  )
+df = values.to_dataframe(column="data_value")
+```
 
 # Contributing
 
 Please open new issues for bugs, feature requests and extensions. You can read
 about the structure of the project, the toolchain and workflow in the [guide for
 contributions](CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyDVL Version: 0.9.0 Summary: The Python Data
+Metadata-Version: 2.1 Name: pyDVL Version: 0.9.1 Summary: The Python Data
 Valuation Library Author: appliedAI Institute gGmbH Project-URL: Source, https:
 //github.com/aai-institute/pydvl Project-URL: Documentation, https://pydvl.org
 Project-URL: TransferLab, https://transferlab.ai Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Science/Research Classifier: Topic
 :: Scientific/Engineering :: Artificial Intelligence Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
@@ -22,21 +22,20 @@
 Requires-Dist: zarr>=2.16.1; extra == "influence" Provides-Extra: ray Requires-
 Dist: ray>=0.8; extra == "ray"
                                  [pyDVL Logo]
                          A library for data valuation.
  _[_P_y_P_I_]_[_V_e_r_s_i_o_n_]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_[_L_i_c_e_n_s_e_]_[_B_u_i_l_d_ _s_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/
           _a_a_i_-_i_n_s_t_i_t_u_t_e_/_p_y_D_V_L_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_V_N_7_D_N_D_E_0_F_V_]_[_D_O_I_]
 **pyDVL** collects algorithms for **Data Valuation** and **Influence Function**
-computation. Refer to the [Methods](https://pydvl.org/devel/getting-started/
-methods/) page of our documentation for a list of all implemented methods.
-**Data Valuation** for machine learning is the task of assigning a scalar to
-each element of a training set which reflects its contribution to the final
-performance or outcome of some model trained on it. Some concepts of value
-depend on a specific model of interest, while others are model-agnostic. pyDVL
-focuses on model-dependent methods.
+computation. Here is the list of [all methods implemented](https://pydvl.org/
+devel/getting-started/methods/). **Data Valuation** for machine learning is the
+task of assigning a scalar to each element of a training set which reflects its
+contribution to the final performance or outcome of some model trained on it.
+Some concepts of value depend on a specific model of interest, while others are
+model-agnostic. pyDVL focuses on model-dependent methods.
                              [best sample removal]
     Comparison of different data valuation methods on best sample removal.
 The **Influence Function** is an infinitesimal measure of the effect that
 single training points have over the parameters of a model, or any function
 thereof. In particular, in machine learning they are also used to compute the
 effect of training samples over individual test points.
                              [best sample removal]
@@ -45,78 +44,75 @@
 # Installation To install the latest release use: ```shell $ pip install pyDVL
 ``` You can also install the latest development version from [TestPyPI](https:/
 /test.pypi.org/project/pyDVL/): ```shell pip install pyDVL --index-url https://
 test.pypi.org/simple/ ``` pyDVL has also extra dependencies for certain
 functionalities, e.g. for using influence functions run ```shell $ pip install
 pyDVL[influence] ``` For more instructions and information refer to [Installing
 pyDVL ](https://pydvl.org/stable/getting-started/#installation) in the
-documentation. # Usage In the following subsections, we will showcase the usage
-of pyDVL for Data Valuation and Influence Functions using simple examples. For
-more instructions and information refer to [Getting Started](https://pydvl.org/
-stable/getting-started/first-steps/) in the documentation. We provide several
-examples for data valuation (e.g. [Shapley Data Valuation](https://pydvl.org/
-stable/examples/shapley_basic_spotify/)) and for influence functions (e.g.
-[Influence Functions for Neural Networks](https://pydvl.org/stable/examples/
-influence_imagenet/)) with details on the algorithms and their applications. ##
-Influence Functions For influence computation, follow these steps: 1. Import
-the necessary packages (The exact packages depend on your specific use case).
-```python import torch from torch import nn from torch.utils.data import
-DataLoader, TensorDataset from pydvl.influence.torch import DirectInfluence
-from pydvl.influence.torch.util import NestedTorchCatAggregator,
-TorchNumpyConverter from pydvl.influence import SequentialInfluenceCalculator
-``` 2. Create PyTorch data loaders for your train and test splits. ```python
-input_dim = (5, 5, 5) output_dim = 3 train_x = torch.rand((10, *input_dim))
-train_y = torch.rand((10, output_dim)) test_x = torch.rand((5, *input_dim))
-test_y = torch.rand((5, output_dim)) train_data_loader = DataLoader
-(TensorDataset(train_x, train_y), batch_size=2) test_data_loader = DataLoader
-(TensorDataset(test_x, test_y), batch_size=1) ``` 3. Instantiate your neural
-network model. ```python nn_architecture = nn.Sequential( nn.Conv2d
-(in_channels=5, out_channels=3, kernel_size=3), nn.Flatten(), nn.Linear(27, 3),
-) ``` 4. Define your loss: ```python loss = nn.MSELoss() ``` 5. Instantiate an
-`InfluenceFunctionModel` and fit it to the training data ```python infl_model =
-DirectInfluence(nn_architecture, loss, hessian_regularization=0.01) infl_model
-= infl_model.fit(train_data_loader) ``` 6. For small input data call influence
-method on the fitted instance. ```python influences = infl_model.influences
-(test_x, test_y, train_x, train_y) ``` The result is a tensor of shape `
-(training samples x test samples)` that contains at index `(i, j`) the
-influence of training sample `i` on test sample `j`. 7. For larger data, wrap
-the model into a calculator and call methods on the calculator. ```python
-infl_calc = SequentialInfluenceCalculator(infl_model) # Lazy object providing
-arrays batch-wise in a sequential manner lazy_influences = infl_calc.influences
+documentation. # Usage Please read [Getting Started](https://pydvl.org/stable/
+getting-started/first-steps/) in the documentation for more instructions. We
+provide several examples for data valuation and for influence functions in our
+[Example Gallery](https://pydvl.org/stable/examples/). ## Influence Functions
+1. Import the necessary packages (the exact ones depend on your specific use
+case). 2. Create PyTorch data loaders for your train and test splits. 3.
+Instantiate your neural network model and define your loss function. 4.
+Instantiate an `InfluenceFunctionModel` and fit it to the training data 5. For
+small input data, you can call the `influences()` method on the fitted
+instance. The result is a tensor of shape `(training samples, test samples)`
+that contains at index `(i, j`) the influence of training sample `i` on test
+sample `j`. 6. For larger datasets, wrap the model into a "calculator" and call
+methods on it. This splits the computation into smaller chunks and allows for
+lazy evaluation and out-of-core computation. The higher the absolute value of
+the influence of a training sample on a test sample, the more influential it is
+for the chosen test sample, model and data loaders. The sign of the influence
+determines whether it is useful (positive) or harmful (negative). > **Note**
+pyDVL currently only support PyTorch for Influence Functions. We plan > to add
+support for Jax next. ```python import torch from torch import nn from
+torch.utils.data import DataLoader, TensorDataset from pydvl.influence import
+SequentialInfluenceCalculator from pydvl.influence.torch import DirectInfluence
+from pydvl.influence.torch.util import ( NestedTorchCatAggregator,
+TorchNumpyConverter, ) input_dim = (5, 5, 5) output_dim = 3 train_x, train_y =
+torch.rand((10, *input_dim)), torch.rand((10, output_dim)) test_x, test_y =
+torch.rand((5, *input_dim)), torch.rand((5, output_dim)) train_data_loader =
+DataLoader(TensorDataset(train_x, train_y), batch_size=2) test_data_loader =
+DataLoader(TensorDataset(test_x, test_y), batch_size=1) model = nn.Sequential
+( nn.Conv2d(in_channels=5, out_channels=3, kernel_size=3), nn.Flatten(),
+nn.Linear(27, 3), ) loss = nn.MSELoss() infl_model = DirectInfluence(model,
+loss, hessian_regularization=0.01) infl_model = infl_model.fit
+(train_data_loader) # For small datasets, instantiate the full influence
+matrix: influences = infl_model.influences(test_x, test_y, train_x, train_y) #
+For larger datasets, use the Influence calculators: infl_calc =
+SequentialInfluenceCalculator(infl_model) # Lazy object providing arrays batch-
+wise in a sequential manner lazy_influences = infl_calc.influences
 (test_data_loader, train_data_loader) # Trigger computation and pull results to
 memory influences = lazy_influences.compute(aggregator=NestedTorchCatAggregator
 ()) # Trigger computation and write results batch-wise to disk
-lazy_influences.to_zarr("influences_result", TorchNumpyConverter()) ``` The
-higher the absolute value of the influence of a training sample on a test
-sample, the more influential it is for the chosen test sample, model and data
-loaders. The sign of the influence determines whether it is useful (positive)
-or harmful (negative). > **Note** pyDVL currently only support PyTorch for
-Influence Functions. > We are planning to add support for Jax and perhaps
-TensorFlow or even Keras. ## Data Valuation The steps required to compute data
-values for your samples are: 1. Import the necessary packages (The exact
-packages depend on your specific use case). ```python import matplotlib.pyplot
-as plt from sklearn.datasets import load_breast_cancer from
-sklearn.linear_model import LogisticRegression from pydvl.utils import Dataset,
-Scorer, Utility from pydvl.value import ( compute_shapley_values, ShapleyMode,
-MaxUpdates, ) ``` 2. Create a `Dataset` object with your train and test splits.
-```python data = Dataset.from_sklearn( load_breast_cancer(), train_size=10,
-stratify_by_target=True, random_state=16, ) ``` 3. Create an instance of a
-`SupervisedModel` (basically any sklearn compatible predictor). ```python model
-= LogisticRegression() ``` 4. Create a `Utility` object to wrap the Dataset,
-the model and a scoring function. ```python u = Utility( model, data, Scorer
-("accuracy", default=0.0) ) ``` 5. Use one of the methods defined in the
-library to compute the values. In our example, we will use *Permutation
-Montecarlo Shapley*, an approximate method for computing Data Shapley values.
-```python values = compute_shapley_values( u,
-mode=ShapleyMode.PermutationMontecarlo, done=MaxUpdates(100), seed=16,
-progress=True ) ``` The result is a variable of type `ValuationResult` that
-contains the indices and their values as well as other attributes. The higher
-the value for an index, the more important it is for the chosen model, dataset
-and scorer. 6. (Optional) Convert the valuation result to a dataframe and
-analyze and visualize the values. ```python df = values.to_dataframe
+lazy_influences.to_zarr("influences_result", TorchNumpyConverter()) ``` ## Data
+Valuation The steps required to compute data values for your samples are: 1.
+Import the necessary packages (the exact ones will depend on your specific use
+case). 2. Create a `Dataset` object with your train and test splits. 3. Create
+an instance of a `SupervisedModel` (basically any sklearn compatible
+predictor), and wrap it in a `Utility` object together with the data and a
+scoring function. 4. Use one of the methods defined in the library to compute
+the values. In the example below, we will use *Permutation Montecarlo Shapley*,
+an approximate method for computing Data Shapley values. The result is a
+variable of type `ValuationResult` that contains the indices and their values
+as well as other attributes. 5. Convert the valuation result to a dataframe,
+and analyze and visualize the values. The higher the value for an index, the
+more important it is for the chosen model, dataset and scorer. Reciprocally,
+low-value points could be mislabelled, or out-of-distribution, and dropping
+them can improve the model's performance. ```python from sklearn.datasets
+import load_breast_cancer from sklearn.linear_model import LogisticRegression
+from pydvl.utils import Dataset, Scorer, Utility from pydvl.value import
+(MaxUpdates, RelativeTruncation, permutation_montecarlo_shapley) data =
+Dataset.from_sklearn( load_breast_cancer(), train_size=10,
+stratify_by_target=True, random_state=16, ) model = LogisticRegression() u =
+Utility( model, data, Scorer("accuracy", default=0.0) ) values =
+permutation_montecarlo_shapley( u, truncation=RelativeTruncation(u, 0.05),
+done=MaxUpdates(1000), seed=16, progress=True ) df = values.to_dataframe
 (column="data_value") ``` # Contributing Please open new issues for bugs,
 feature requests and extensions. You can read about the structure of the
 project, the toolchain and workflow in the [guide for contributions]
 (CONTRIBUTING.md). # License pyDVL is distributed under [LGPL-3.0](https://
 www.gnu.org/licenses/lgpl-3.0.html). A complete version can be found in two
 files: [here](LICENSE) and [here](COPYING.LESSER). All contributions will be
 distributed under this license.
```

### Comparing `pydvl-0.9/README.md` & `pydvl-0.9.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -12,28 +12,26 @@
     <a href="https://pydvl.org"><img src="https://img.shields.io/badge/docs-All%20versions-009485" alt="documentation"></a>
     <a href="https://raw.githubusercontent.com/aai-institute/pyDVL/master/LICENSE"><img alt="License" src="https://img.shields.io/pypi/l/pydvl"></a>
     <a href="https://github.com/aai-institute/pyDVL/actions/workflows/main.yaml"><img src="https://github.com/aai-institute/pyDVL/actions/workflows/main.yaml/badge.svg" alt="Build status" ></a>
     <a href="https://codecov.io/gh/aai-institute/pyDVL"><img src="https://codecov.io/gh/aai-institute/pyDVL/graph/badge.svg?token=VN7DNDE0FV"/></a>
     <a href="https://zenodo.org/badge/latestdoi/354117916"><img src="https://zenodo.org/badge/354117916.svg" alt="DOI"></a>
 </p>
 
-**pyDVL** collects algorithms for **Data Valuation** and **Influence Function** computation.
-
-Refer to the [Methods](https://pydvl.org/devel/getting-started/methods/)
-page of our documentation for a list of all implemented methods. 
+**pyDVL** collects algorithms for **Data Valuation** and **Influence Function**
+computation. Here is the list of [all methods implemented](https://pydvl.org/devel/getting-started/methods/).
 
 **Data Valuation** for machine learning is the task of assigning a scalar
 to each element of a training set which reflects its contribution to the final
 performance or outcome of some model trained on it. Some concepts of
 value depend on a specific model of interest, while others are model-agnostic.
 pyDVL focuses on model-dependent methods.
 
 <div align="center" style="text-align:center;">
     <img
-        width="70%"
+        width="60%"
         align="center"
         style="display: block; margin-left: auto; margin-right: auto;"
         src="https://pydvl.org/devel/value/img/mclc-best-removal-10k-natural.svg"
         alt="best sample removal"
     />
     <p align="center" style="text-align:center;">
         Comparison of different data valuation methods
@@ -44,15 +42,15 @@
 The **Influence Function** is an infinitesimal measure of the effect that single
 training points have over the parameters of a model, or any function thereof.
 In particular, in machine learning they are also used to compute the effect
 of training samples over individual test points.
 
 <div align="center" style="text-align:center;">
     <img
-        width="70%"
+        width="60%"
         align="center"
         style="display: block; margin-left: auto; margin-right: auto;"
         src="https://pydvl.org/devel/examples/img/influence_functions_example.png"
         alt="best sample removal"
     />
     <p align="center" style="text-align:center;">
         Influences of input points with corrupted data.
@@ -78,188 +76,141 @@
 pyDVL has also extra dependencies for certain functionalities, 
 e.g. for using influence functions run
 ```shell
 $ pip install pyDVL[influence]
 ```
 
 For more instructions and information refer to [Installing pyDVL
-](https://pydvl.org/stable/getting-started/#installation) in the
-documentation.
+](https://pydvl.org/stable/getting-started/#installation) in the documentation.
 
 # Usage
 
-In the following subsections, we will showcase the usage of pyDVL
-for Data Valuation and Influence Functions using simple examples.
-
-For more instructions and information refer to [Getting
-Started](https://pydvl.org/stable/getting-started/first-steps/) in
-the documentation.
-We provide several examples for data valuation
-(e.g. [Shapley Data Valuation](https://pydvl.org/stable/examples/shapley_basic_spotify/))
-and for influence functions
-(e.g. [Influence Functions for Neural Networks](https://pydvl.org/stable/examples/influence_imagenet/))
-with details on the algorithms and their applications.
+Please read [Getting
+Started](https://pydvl.org/stable/getting-started/first-steps/) in the
+documentation for more instructions. We provide several examples for data
+valuation and for influence functions in our [Example
+Gallery](https://pydvl.org/stable/examples/).
 
 ## Influence Functions
 
-For influence computation, follow these steps:
-
-1. Import the necessary packages (The exact packages depend on your specific use case).
-
-   ```python
-   import torch
-   from torch import nn
-   from torch.utils.data import DataLoader, TensorDataset
-   
-   from pydvl.influence.torch import DirectInfluence
-   from pydvl.influence.torch.util import NestedTorchCatAggregator, TorchNumpyConverter
-   from pydvl.influence import SequentialInfluenceCalculator
-   ```
-
+1. Import the necessary packages (the exact ones depend on your specific use case).
 2. Create PyTorch data loaders for your train and test splits.
-
-   ```python
-   input_dim = (5, 5, 5)
-   output_dim = 3
-   train_x = torch.rand((10, *input_dim))
-   train_y = torch.rand((10, output_dim))
-   test_x = torch.rand((5, *input_dim))
-   test_y = torch.rand((5, output_dim))
-
-   train_data_loader = DataLoader(TensorDataset(train_x, train_y), batch_size=2)
-   test_data_loader = DataLoader(TensorDataset(test_x, test_y), batch_size=1)
-   ```
-
-3. Instantiate your neural network model.
-
-   ```python
-   nn_architecture = nn.Sequential(
-     nn.Conv2d(in_channels=5, out_channels=3, kernel_size=3),
-     nn.Flatten(),
-     nn.Linear(27, 3),
+3. Instantiate your neural network model and define your loss function.
+4. Instantiate an `InfluenceFunctionModel` and fit it to the training data
+5. For small input data, you can call the `influences()` method on the fitted
+   instance. The result is a tensor of shape `(training samples, test samples)`
+   that contains at index `(i, j`) the influence of training sample `i` on
+   test sample `j`.
+6. For larger datasets, wrap the model into a "calculator" and call methods on
+   it. This splits the computation into smaller chunks and allows for lazy
+   evaluation and out-of-core computation.
+
+The higher the absolute value of the influence of a training sample
+on a test sample, the more influential it is for the chosen test sample, model
+and data loaders. The sign of the influence determines whether it is 
+useful (positive) or harmful (negative).
+
+> **Note** pyDVL currently only support PyTorch for Influence Functions. We plan
+> to add support for Jax next.
+
+```python
+import torch
+from torch import nn
+from torch.utils.data import DataLoader, TensorDataset
+
+from pydvl.influence import SequentialInfluenceCalculator
+from pydvl.influence.torch import DirectInfluence
+from pydvl.influence.torch.util import (
+   NestedTorchCatAggregator,
+   TorchNumpyConverter,
    )
-   ```
-
-4. Define your loss:
-
-   ```python
-   loss = nn.MSELoss()
-   ```
 
-5. Instantiate an `InfluenceFunctionModel` and fit it to the training data
+input_dim = (5, 5, 5)
+output_dim = 3
+train_x, train_y = torch.rand((10, *input_dim)), torch.rand((10, output_dim))
+test_x, test_y = torch.rand((5, *input_dim)), torch.rand((5, output_dim))
+train_data_loader = DataLoader(TensorDataset(train_x, train_y), batch_size=2)
+test_data_loader = DataLoader(TensorDataset(test_x, test_y), batch_size=1)
+model = nn.Sequential(
+  nn.Conv2d(in_channels=5, out_channels=3, kernel_size=3),
+  nn.Flatten(),
+  nn.Linear(27, 3),
+  )
+loss = nn.MSELoss()
+
+infl_model = DirectInfluence(model, loss, hessian_regularization=0.01)
+infl_model = infl_model.fit(train_data_loader)
+
+# For small datasets, instantiate the full influence matrix:
+influences = infl_model.influences(test_x, test_y, train_x, train_y)
+
+# For larger datasets, use the Influence calculators:
+infl_calc = SequentialInfluenceCalculator(infl_model)
 
-   ```python
-   infl_model = DirectInfluence(nn_architecture, loss, hessian_regularization=0.01)
-   infl_model = infl_model.fit(train_data_loader)
-   ```
+# Lazy object providing arrays batch-wise in a sequential manner
+lazy_influences = infl_calc.influences(test_data_loader, train_data_loader)
 
-6. For small input data call influence method on the fitted instance. 
-
-   ```python
-   influences = infl_model.influences(test_x, test_y, train_x, train_y)
-   ```
-   The result is a tensor of shape `(training samples x test samples)`
-   that contains at index `(i, j`) the influence of training sample `i` on
-   test sample `j`.
+# Trigger computation and pull results to memory
+influences = lazy_influences.compute(aggregator=NestedTorchCatAggregator())
 
-7. For larger data, wrap the model into a
-   calculator and call methods on the calculator.
-   ```python
-   infl_calc = SequentialInfluenceCalculator(infl_model)
-   
-    # Lazy object providing arrays batch-wise in a sequential manner
-   lazy_influences = infl_calc.influences(test_data_loader, train_data_loader)
-
-   # Trigger computation and pull results to memory
-   influences = lazy_influences.compute(aggregator=NestedTorchCatAggregator())
-
-   # Trigger computation and write results batch-wise to disk
-   lazy_influences.to_zarr("influences_result", TorchNumpyConverter())
-   ```
-   
-
-   The higher the absolute value of the influence of a training sample
-   on a test sample, the more influential it is for the chosen test sample, model
-   and data loaders. The sign of the influence determines whether it is 
-   useful (positive) or harmful (negative).
-
-> **Note** pyDVL currently only support PyTorch for Influence Functions. 
-> We are planning to add support for Jax and perhaps TensorFlow or even Keras.
+# Trigger computation and write results batch-wise to disk
+lazy_influences.to_zarr("influences_result", TorchNumpyConverter())
+```
 
 ## Data Valuation
 
 The steps required to compute data values for your samples are:
 
-1. Import the necessary packages (The exact packages depend on your specific use case).
-
-   ```python
-   import matplotlib.pyplot as plt
-   from sklearn.datasets import load_breast_cancer
-   from sklearn.linear_model import LogisticRegression
-   from pydvl.utils import Dataset, Scorer, Utility
-   from pydvl.value import (
-      compute_shapley_values,
-      ShapleyMode,
-      MaxUpdates,
-   )
-   ```
- 
+1. Import the necessary packages (the exact ones will depend on your specific
+   use case).
 2. Create a `Dataset` object with your train and test splits.
-
-   ```python
-   data = Dataset.from_sklearn(
-       load_breast_cancer(),
-       train_size=10,
-       stratify_by_target=True,
-       random_state=16,
-   )
-   ```
-
 3. Create an instance of a `SupervisedModel` (basically any sklearn compatible
-   predictor).
-
-   ```python
-   model = LogisticRegression()
-   ```  
-
-4. Create a `Utility` object to wrap the Dataset, the model and a scoring
-   function.
-
-   ```python
-   u = Utility(
-      model,
-      data,
-      Scorer("accuracy", default=0.0)
-   )
-   ```
-
-5. Use one of the methods defined in the library to compute the values.
-   In our example, we will use *Permutation Montecarlo Shapley*,
-   an approximate method for computing Data Shapley values.
-
-   ```python
-   values = compute_shapley_values(
-      u,
-      mode=ShapleyMode.PermutationMontecarlo,
-      done=MaxUpdates(100),
-      seed=16,  
-      progress=True
-   )
-   ```
-   The result is a variable of type `ValuationResult` that contains
-   the indices and their values as well as other attributes.
-
-   The higher the value for an index, the more important it is for the chosen
-   model, dataset and scorer.
-
-6. (Optional) Convert the valuation result to a dataframe and analyze and visualize the values.
-
-   ```python
-   df = values.to_dataframe(column="data_value")
-   ```
+   predictor), and wrap it in a `Utility` object together with the data and a
+   scoring function.
+4. Use one of the methods defined in the library to compute the values. In the
+   example below, we will use *Permutation Montecarlo Shapley*, an approximate
+   method for computing Data Shapley values. The result is a variable of type
+   `ValuationResult` that contains the indices and their values as well as other
+   attributes.
+5. Convert the valuation result to a dataframe, and analyze and visualize the
+   values.
+
+The higher the value for an index, the more important it is for the chosen
+model, dataset and scorer. Reciprocally, low-value points could be mislabelled,
+or out-of-distribution, and dropping them can improve the model's performance.
+
+```python
+from sklearn.datasets import load_breast_cancer
+from sklearn.linear_model import LogisticRegression
+
+from pydvl.utils import Dataset, Scorer, Utility
+from pydvl.value import (MaxUpdates, RelativeTruncation,
+                         permutation_montecarlo_shapley)
+
+data = Dataset.from_sklearn(
+  load_breast_cancer(),
+  train_size=10,
+  stratify_by_target=True,
+  random_state=16,
+  )
+model = LogisticRegression()
+u = Utility(
+  model,
+  data,
+  Scorer("accuracy", default=0.0)
+  )
+values = permutation_montecarlo_shapley(
+  u,
+  truncation=RelativeTruncation(u, 0.05),
+  done=MaxUpdates(1000),
+  seed=16,
+  progress=True
+  )
+df = values.to_dataframe(column="data_value")
+```
 
 # Contributing
 
 Please open new issues for bugs, feature requests and extensions. You can read
 about the structure of the project, the toolchain and workflow in the [guide for
 contributions](CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
                                  [pyDVL Logo]
                          A library for data valuation.
  _[_P_y_P_I_]_[_V_e_r_s_i_o_n_]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_[_L_i_c_e_n_s_e_]_[_B_u_i_l_d_ _s_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/
           _a_a_i_-_i_n_s_t_i_t_u_t_e_/_p_y_D_V_L_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_V_N_7_D_N_D_E_0_F_V_]_[_D_O_I_]
 **pyDVL** collects algorithms for **Data Valuation** and **Influence Function**
-computation. Refer to the [Methods](https://pydvl.org/devel/getting-started/
-methods/) page of our documentation for a list of all implemented methods.
-**Data Valuation** for machine learning is the task of assigning a scalar to
-each element of a training set which reflects its contribution to the final
-performance or outcome of some model trained on it. Some concepts of value
-depend on a specific model of interest, while others are model-agnostic. pyDVL
-focuses on model-dependent methods.
+computation. Here is the list of [all methods implemented](https://pydvl.org/
+devel/getting-started/methods/). **Data Valuation** for machine learning is the
+task of assigning a scalar to each element of a training set which reflects its
+contribution to the final performance or outcome of some model trained on it.
+Some concepts of value depend on a specific model of interest, while others are
+model-agnostic. pyDVL focuses on model-dependent methods.
                              [best sample removal]
     Comparison of different data valuation methods on best sample removal.
 The **Influence Function** is an infinitesimal measure of the effect that
 single training points have over the parameters of a model, or any function
 thereof. In particular, in machine learning they are also used to compute the
 effect of training samples over individual test points.
                              [best sample removal]
@@ -22,78 +21,75 @@
 # Installation To install the latest release use: ```shell $ pip install pyDVL
 ``` You can also install the latest development version from [TestPyPI](https:/
 /test.pypi.org/project/pyDVL/): ```shell pip install pyDVL --index-url https://
 test.pypi.org/simple/ ``` pyDVL has also extra dependencies for certain
 functionalities, e.g. for using influence functions run ```shell $ pip install
 pyDVL[influence] ``` For more instructions and information refer to [Installing
 pyDVL ](https://pydvl.org/stable/getting-started/#installation) in the
-documentation. # Usage In the following subsections, we will showcase the usage
-of pyDVL for Data Valuation and Influence Functions using simple examples. For
-more instructions and information refer to [Getting Started](https://pydvl.org/
-stable/getting-started/first-steps/) in the documentation. We provide several
-examples for data valuation (e.g. [Shapley Data Valuation](https://pydvl.org/
-stable/examples/shapley_basic_spotify/)) and for influence functions (e.g.
-[Influence Functions for Neural Networks](https://pydvl.org/stable/examples/
-influence_imagenet/)) with details on the algorithms and their applications. ##
-Influence Functions For influence computation, follow these steps: 1. Import
-the necessary packages (The exact packages depend on your specific use case).
-```python import torch from torch import nn from torch.utils.data import
-DataLoader, TensorDataset from pydvl.influence.torch import DirectInfluence
-from pydvl.influence.torch.util import NestedTorchCatAggregator,
-TorchNumpyConverter from pydvl.influence import SequentialInfluenceCalculator
-``` 2. Create PyTorch data loaders for your train and test splits. ```python
-input_dim = (5, 5, 5) output_dim = 3 train_x = torch.rand((10, *input_dim))
-train_y = torch.rand((10, output_dim)) test_x = torch.rand((5, *input_dim))
-test_y = torch.rand((5, output_dim)) train_data_loader = DataLoader
-(TensorDataset(train_x, train_y), batch_size=2) test_data_loader = DataLoader
-(TensorDataset(test_x, test_y), batch_size=1) ``` 3. Instantiate your neural
-network model. ```python nn_architecture = nn.Sequential( nn.Conv2d
-(in_channels=5, out_channels=3, kernel_size=3), nn.Flatten(), nn.Linear(27, 3),
-) ``` 4. Define your loss: ```python loss = nn.MSELoss() ``` 5. Instantiate an
-`InfluenceFunctionModel` and fit it to the training data ```python infl_model =
-DirectInfluence(nn_architecture, loss, hessian_regularization=0.01) infl_model
-= infl_model.fit(train_data_loader) ``` 6. For small input data call influence
-method on the fitted instance. ```python influences = infl_model.influences
-(test_x, test_y, train_x, train_y) ``` The result is a tensor of shape `
-(training samples x test samples)` that contains at index `(i, j`) the
-influence of training sample `i` on test sample `j`. 7. For larger data, wrap
-the model into a calculator and call methods on the calculator. ```python
-infl_calc = SequentialInfluenceCalculator(infl_model) # Lazy object providing
-arrays batch-wise in a sequential manner lazy_influences = infl_calc.influences
+documentation. # Usage Please read [Getting Started](https://pydvl.org/stable/
+getting-started/first-steps/) in the documentation for more instructions. We
+provide several examples for data valuation and for influence functions in our
+[Example Gallery](https://pydvl.org/stable/examples/). ## Influence Functions
+1. Import the necessary packages (the exact ones depend on your specific use
+case). 2. Create PyTorch data loaders for your train and test splits. 3.
+Instantiate your neural network model and define your loss function. 4.
+Instantiate an `InfluenceFunctionModel` and fit it to the training data 5. For
+small input data, you can call the `influences()` method on the fitted
+instance. The result is a tensor of shape `(training samples, test samples)`
+that contains at index `(i, j`) the influence of training sample `i` on test
+sample `j`. 6. For larger datasets, wrap the model into a "calculator" and call
+methods on it. This splits the computation into smaller chunks and allows for
+lazy evaluation and out-of-core computation. The higher the absolute value of
+the influence of a training sample on a test sample, the more influential it is
+for the chosen test sample, model and data loaders. The sign of the influence
+determines whether it is useful (positive) or harmful (negative). > **Note**
+pyDVL currently only support PyTorch for Influence Functions. We plan > to add
+support for Jax next. ```python import torch from torch import nn from
+torch.utils.data import DataLoader, TensorDataset from pydvl.influence import
+SequentialInfluenceCalculator from pydvl.influence.torch import DirectInfluence
+from pydvl.influence.torch.util import ( NestedTorchCatAggregator,
+TorchNumpyConverter, ) input_dim = (5, 5, 5) output_dim = 3 train_x, train_y =
+torch.rand((10, *input_dim)), torch.rand((10, output_dim)) test_x, test_y =
+torch.rand((5, *input_dim)), torch.rand((5, output_dim)) train_data_loader =
+DataLoader(TensorDataset(train_x, train_y), batch_size=2) test_data_loader =
+DataLoader(TensorDataset(test_x, test_y), batch_size=1) model = nn.Sequential
+( nn.Conv2d(in_channels=5, out_channels=3, kernel_size=3), nn.Flatten(),
+nn.Linear(27, 3), ) loss = nn.MSELoss() infl_model = DirectInfluence(model,
+loss, hessian_regularization=0.01) infl_model = infl_model.fit
+(train_data_loader) # For small datasets, instantiate the full influence
+matrix: influences = infl_model.influences(test_x, test_y, train_x, train_y) #
+For larger datasets, use the Influence calculators: infl_calc =
+SequentialInfluenceCalculator(infl_model) # Lazy object providing arrays batch-
+wise in a sequential manner lazy_influences = infl_calc.influences
 (test_data_loader, train_data_loader) # Trigger computation and pull results to
 memory influences = lazy_influences.compute(aggregator=NestedTorchCatAggregator
 ()) # Trigger computation and write results batch-wise to disk
-lazy_influences.to_zarr("influences_result", TorchNumpyConverter()) ``` The
-higher the absolute value of the influence of a training sample on a test
-sample, the more influential it is for the chosen test sample, model and data
-loaders. The sign of the influence determines whether it is useful (positive)
-or harmful (negative). > **Note** pyDVL currently only support PyTorch for
-Influence Functions. > We are planning to add support for Jax and perhaps
-TensorFlow or even Keras. ## Data Valuation The steps required to compute data
-values for your samples are: 1. Import the necessary packages (The exact
-packages depend on your specific use case). ```python import matplotlib.pyplot
-as plt from sklearn.datasets import load_breast_cancer from
-sklearn.linear_model import LogisticRegression from pydvl.utils import Dataset,
-Scorer, Utility from pydvl.value import ( compute_shapley_values, ShapleyMode,
-MaxUpdates, ) ``` 2. Create a `Dataset` object with your train and test splits.
-```python data = Dataset.from_sklearn( load_breast_cancer(), train_size=10,
-stratify_by_target=True, random_state=16, ) ``` 3. Create an instance of a
-`SupervisedModel` (basically any sklearn compatible predictor). ```python model
-= LogisticRegression() ``` 4. Create a `Utility` object to wrap the Dataset,
-the model and a scoring function. ```python u = Utility( model, data, Scorer
-("accuracy", default=0.0) ) ``` 5. Use one of the methods defined in the
-library to compute the values. In our example, we will use *Permutation
-Montecarlo Shapley*, an approximate method for computing Data Shapley values.
-```python values = compute_shapley_values( u,
-mode=ShapleyMode.PermutationMontecarlo, done=MaxUpdates(100), seed=16,
-progress=True ) ``` The result is a variable of type `ValuationResult` that
-contains the indices and their values as well as other attributes. The higher
-the value for an index, the more important it is for the chosen model, dataset
-and scorer. 6. (Optional) Convert the valuation result to a dataframe and
-analyze and visualize the values. ```python df = values.to_dataframe
+lazy_influences.to_zarr("influences_result", TorchNumpyConverter()) ``` ## Data
+Valuation The steps required to compute data values for your samples are: 1.
+Import the necessary packages (the exact ones will depend on your specific use
+case). 2. Create a `Dataset` object with your train and test splits. 3. Create
+an instance of a `SupervisedModel` (basically any sklearn compatible
+predictor), and wrap it in a `Utility` object together with the data and a
+scoring function. 4. Use one of the methods defined in the library to compute
+the values. In the example below, we will use *Permutation Montecarlo Shapley*,
+an approximate method for computing Data Shapley values. The result is a
+variable of type `ValuationResult` that contains the indices and their values
+as well as other attributes. 5. Convert the valuation result to a dataframe,
+and analyze and visualize the values. The higher the value for an index, the
+more important it is for the chosen model, dataset and scorer. Reciprocally,
+low-value points could be mislabelled, or out-of-distribution, and dropping
+them can improve the model's performance. ```python from sklearn.datasets
+import load_breast_cancer from sklearn.linear_model import LogisticRegression
+from pydvl.utils import Dataset, Scorer, Utility from pydvl.value import
+(MaxUpdates, RelativeTruncation, permutation_montecarlo_shapley) data =
+Dataset.from_sklearn( load_breast_cancer(), train_size=10,
+stratify_by_target=True, random_state=16, ) model = LogisticRegression() u =
+Utility( model, data, Scorer("accuracy", default=0.0) ) values =
+permutation_montecarlo_shapley( u, truncation=RelativeTruncation(u, 0.05),
+done=MaxUpdates(1000), seed=16, progress=True ) df = values.to_dataframe
 (column="data_value") ``` # Contributing Please open new issues for bugs,
 feature requests and extensions. You can read about the structure of the
 project, the toolchain and workflow in the [guide for contributions]
 (CONTRIBUTING.md). # License pyDVL is distributed under [LGPL-3.0](https://
 www.gnu.org/licenses/lgpl-3.0.html). A complete version can be found in two
 files: [here](LICENSE) and [here](COPYING.LESSER). All contributions will be
 distributed under this license.
```

### Comparing `pydvl-0.9/logo.svg` & `pydvl-0.9.1/logo.svg`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/pyproject.toml` & `pydvl-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/setup.py` & `pydvl-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setup(
     name="pyDVL",
     package_dir={"": "src"},
     package_data={"pydvl": ["py.typed"]},
     packages=find_packages(where="src"),
     include_package_data=True,
-    version="0.9.0",
+    version="0.9.1",
     description="The Python Data Valuation Library",
     install_requires=[
         line
         for line in open("requirements.txt").readlines()
         if not line.startswith("--")
     ],
     setup_requires=["wheel"],
```

### Comparing `pydvl-0.9/src/pyDVL.egg-info/PKG-INFO` & `pydvl-0.9.1/src/pyDVL.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDVL
-Version: 0.9.0
+Version: 0.9.1
 Summary: The Python Data Valuation Library
 Author: appliedAI Institute gGmbH
 Project-URL: Source, https://github.com/aai-institute/pydvl
 Project-URL: Documentation, https://pydvl.org
 Project-URL: TransferLab, https://transferlab.ai
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -57,28 +57,26 @@
     <a href="https://pydvl.org"><img src="https://img.shields.io/badge/docs-All%20versions-009485" alt="documentation"></a>
     <a href="https://raw.githubusercontent.com/aai-institute/pyDVL/master/LICENSE"><img alt="License" src="https://img.shields.io/pypi/l/pydvl"></a>
     <a href="https://github.com/aai-institute/pyDVL/actions/workflows/main.yaml"><img src="https://github.com/aai-institute/pyDVL/actions/workflows/main.yaml/badge.svg" alt="Build status" ></a>
     <a href="https://codecov.io/gh/aai-institute/pyDVL"><img src="https://codecov.io/gh/aai-institute/pyDVL/graph/badge.svg?token=VN7DNDE0FV"/></a>
     <a href="https://zenodo.org/badge/latestdoi/354117916"><img src="https://zenodo.org/badge/354117916.svg" alt="DOI"></a>
 </p>
 
-**pyDVL** collects algorithms for **Data Valuation** and **Influence Function** computation.
-
-Refer to the [Methods](https://pydvl.org/devel/getting-started/methods/)
-page of our documentation for a list of all implemented methods. 
+**pyDVL** collects algorithms for **Data Valuation** and **Influence Function**
+computation. Here is the list of [all methods implemented](https://pydvl.org/devel/getting-started/methods/).
 
 **Data Valuation** for machine learning is the task of assigning a scalar
 to each element of a training set which reflects its contribution to the final
 performance or outcome of some model trained on it. Some concepts of
 value depend on a specific model of interest, while others are model-agnostic.
 pyDVL focuses on model-dependent methods.
 
 <div align="center" style="text-align:center;">
     <img
-        width="70%"
+        width="60%"
         align="center"
         style="display: block; margin-left: auto; margin-right: auto;"
         src="https://pydvl.org/devel/value/img/mclc-best-removal-10k-natural.svg"
         alt="best sample removal"
     />
     <p align="center" style="text-align:center;">
         Comparison of different data valuation methods
@@ -89,15 +87,15 @@
 The **Influence Function** is an infinitesimal measure of the effect that single
 training points have over the parameters of a model, or any function thereof.
 In particular, in machine learning they are also used to compute the effect
 of training samples over individual test points.
 
 <div align="center" style="text-align:center;">
     <img
-        width="70%"
+        width="60%"
         align="center"
         style="display: block; margin-left: auto; margin-right: auto;"
         src="https://pydvl.org/devel/examples/img/influence_functions_example.png"
         alt="best sample removal"
     />
     <p align="center" style="text-align:center;">
         Influences of input points with corrupted data.
@@ -123,188 +121,141 @@
 pyDVL has also extra dependencies for certain functionalities, 
 e.g. for using influence functions run
 ```shell
 $ pip install pyDVL[influence]
 ```
 
 For more instructions and information refer to [Installing pyDVL
-](https://pydvl.org/stable/getting-started/#installation) in the
-documentation.
+](https://pydvl.org/stable/getting-started/#installation) in the documentation.
 
 # Usage
 
-In the following subsections, we will showcase the usage of pyDVL
-for Data Valuation and Influence Functions using simple examples.
-
-For more instructions and information refer to [Getting
-Started](https://pydvl.org/stable/getting-started/first-steps/) in
-the documentation.
-We provide several examples for data valuation
-(e.g. [Shapley Data Valuation](https://pydvl.org/stable/examples/shapley_basic_spotify/))
-and for influence functions
-(e.g. [Influence Functions for Neural Networks](https://pydvl.org/stable/examples/influence_imagenet/))
-with details on the algorithms and their applications.
+Please read [Getting
+Started](https://pydvl.org/stable/getting-started/first-steps/) in the
+documentation for more instructions. We provide several examples for data
+valuation and for influence functions in our [Example
+Gallery](https://pydvl.org/stable/examples/).
 
 ## Influence Functions
 
-For influence computation, follow these steps:
-
-1. Import the necessary packages (The exact packages depend on your specific use case).
-
-   ```python
-   import torch
-   from torch import nn
-   from torch.utils.data import DataLoader, TensorDataset
-   
-   from pydvl.influence.torch import DirectInfluence
-   from pydvl.influence.torch.util import NestedTorchCatAggregator, TorchNumpyConverter
-   from pydvl.influence import SequentialInfluenceCalculator
-   ```
-
+1. Import the necessary packages (the exact ones depend on your specific use case).
 2. Create PyTorch data loaders for your train and test splits.
-
-   ```python
-   input_dim = (5, 5, 5)
-   output_dim = 3
-   train_x = torch.rand((10, *input_dim))
-   train_y = torch.rand((10, output_dim))
-   test_x = torch.rand((5, *input_dim))
-   test_y = torch.rand((5, output_dim))
-
-   train_data_loader = DataLoader(TensorDataset(train_x, train_y), batch_size=2)
-   test_data_loader = DataLoader(TensorDataset(test_x, test_y), batch_size=1)
-   ```
-
-3. Instantiate your neural network model.
-
-   ```python
-   nn_architecture = nn.Sequential(
-     nn.Conv2d(in_channels=5, out_channels=3, kernel_size=3),
-     nn.Flatten(),
-     nn.Linear(27, 3),
+3. Instantiate your neural network model and define your loss function.
+4. Instantiate an `InfluenceFunctionModel` and fit it to the training data
+5. For small input data, you can call the `influences()` method on the fitted
+   instance. The result is a tensor of shape `(training samples, test samples)`
+   that contains at index `(i, j`) the influence of training sample `i` on
+   test sample `j`.
+6. For larger datasets, wrap the model into a "calculator" and call methods on
+   it. This splits the computation into smaller chunks and allows for lazy
+   evaluation and out-of-core computation.
+
+The higher the absolute value of the influence of a training sample
+on a test sample, the more influential it is for the chosen test sample, model
+and data loaders. The sign of the influence determines whether it is 
+useful (positive) or harmful (negative).
+
+> **Note** pyDVL currently only support PyTorch for Influence Functions. We plan
+> to add support for Jax next.
+
+```python
+import torch
+from torch import nn
+from torch.utils.data import DataLoader, TensorDataset
+
+from pydvl.influence import SequentialInfluenceCalculator
+from pydvl.influence.torch import DirectInfluence
+from pydvl.influence.torch.util import (
+   NestedTorchCatAggregator,
+   TorchNumpyConverter,
    )
-   ```
-
-4. Define your loss:
-
-   ```python
-   loss = nn.MSELoss()
-   ```
 
-5. Instantiate an `InfluenceFunctionModel` and fit it to the training data
+input_dim = (5, 5, 5)
+output_dim = 3
+train_x, train_y = torch.rand((10, *input_dim)), torch.rand((10, output_dim))
+test_x, test_y = torch.rand((5, *input_dim)), torch.rand((5, output_dim))
+train_data_loader = DataLoader(TensorDataset(train_x, train_y), batch_size=2)
+test_data_loader = DataLoader(TensorDataset(test_x, test_y), batch_size=1)
+model = nn.Sequential(
+  nn.Conv2d(in_channels=5, out_channels=3, kernel_size=3),
+  nn.Flatten(),
+  nn.Linear(27, 3),
+  )
+loss = nn.MSELoss()
+
+infl_model = DirectInfluence(model, loss, hessian_regularization=0.01)
+infl_model = infl_model.fit(train_data_loader)
+
+# For small datasets, instantiate the full influence matrix:
+influences = infl_model.influences(test_x, test_y, train_x, train_y)
+
+# For larger datasets, use the Influence calculators:
+infl_calc = SequentialInfluenceCalculator(infl_model)
 
-   ```python
-   infl_model = DirectInfluence(nn_architecture, loss, hessian_regularization=0.01)
-   infl_model = infl_model.fit(train_data_loader)
-   ```
+# Lazy object providing arrays batch-wise in a sequential manner
+lazy_influences = infl_calc.influences(test_data_loader, train_data_loader)
 
-6. For small input data call influence method on the fitted instance. 
-
-   ```python
-   influences = infl_model.influences(test_x, test_y, train_x, train_y)
-   ```
-   The result is a tensor of shape `(training samples x test samples)`
-   that contains at index `(i, j`) the influence of training sample `i` on
-   test sample `j`.
+# Trigger computation and pull results to memory
+influences = lazy_influences.compute(aggregator=NestedTorchCatAggregator())
 
-7. For larger data, wrap the model into a
-   calculator and call methods on the calculator.
-   ```python
-   infl_calc = SequentialInfluenceCalculator(infl_model)
-   
-    # Lazy object providing arrays batch-wise in a sequential manner
-   lazy_influences = infl_calc.influences(test_data_loader, train_data_loader)
-
-   # Trigger computation and pull results to memory
-   influences = lazy_influences.compute(aggregator=NestedTorchCatAggregator())
-
-   # Trigger computation and write results batch-wise to disk
-   lazy_influences.to_zarr("influences_result", TorchNumpyConverter())
-   ```
-   
-
-   The higher the absolute value of the influence of a training sample
-   on a test sample, the more influential it is for the chosen test sample, model
-   and data loaders. The sign of the influence determines whether it is 
-   useful (positive) or harmful (negative).
-
-> **Note** pyDVL currently only support PyTorch for Influence Functions. 
-> We are planning to add support for Jax and perhaps TensorFlow or even Keras.
+# Trigger computation and write results batch-wise to disk
+lazy_influences.to_zarr("influences_result", TorchNumpyConverter())
+```
 
 ## Data Valuation
 
 The steps required to compute data values for your samples are:
 
-1. Import the necessary packages (The exact packages depend on your specific use case).
-
-   ```python
-   import matplotlib.pyplot as plt
-   from sklearn.datasets import load_breast_cancer
-   from sklearn.linear_model import LogisticRegression
-   from pydvl.utils import Dataset, Scorer, Utility
-   from pydvl.value import (
-      compute_shapley_values,
-      ShapleyMode,
-      MaxUpdates,
-   )
-   ```
- 
+1. Import the necessary packages (the exact ones will depend on your specific
+   use case).
 2. Create a `Dataset` object with your train and test splits.
-
-   ```python
-   data = Dataset.from_sklearn(
-       load_breast_cancer(),
-       train_size=10,
-       stratify_by_target=True,
-       random_state=16,
-   )
-   ```
-
 3. Create an instance of a `SupervisedModel` (basically any sklearn compatible
-   predictor).
-
-   ```python
-   model = LogisticRegression()
-   ```  
-
-4. Create a `Utility` object to wrap the Dataset, the model and a scoring
-   function.
-
-   ```python
-   u = Utility(
-      model,
-      data,
-      Scorer("accuracy", default=0.0)
-   )
-   ```
-
-5. Use one of the methods defined in the library to compute the values.
-   In our example, we will use *Permutation Montecarlo Shapley*,
-   an approximate method for computing Data Shapley values.
-
-   ```python
-   values = compute_shapley_values(
-      u,
-      mode=ShapleyMode.PermutationMontecarlo,
-      done=MaxUpdates(100),
-      seed=16,  
-      progress=True
-   )
-   ```
-   The result is a variable of type `ValuationResult` that contains
-   the indices and their values as well as other attributes.
-
-   The higher the value for an index, the more important it is for the chosen
-   model, dataset and scorer.
-
-6. (Optional) Convert the valuation result to a dataframe and analyze and visualize the values.
-
-   ```python
-   df = values.to_dataframe(column="data_value")
-   ```
+   predictor), and wrap it in a `Utility` object together with the data and a
+   scoring function.
+4. Use one of the methods defined in the library to compute the values. In the
+   example below, we will use *Permutation Montecarlo Shapley*, an approximate
+   method for computing Data Shapley values. The result is a variable of type
+   `ValuationResult` that contains the indices and their values as well as other
+   attributes.
+5. Convert the valuation result to a dataframe, and analyze and visualize the
+   values.
+
+The higher the value for an index, the more important it is for the chosen
+model, dataset and scorer. Reciprocally, low-value points could be mislabelled,
+or out-of-distribution, and dropping them can improve the model's performance.
+
+```python
+from sklearn.datasets import load_breast_cancer
+from sklearn.linear_model import LogisticRegression
+
+from pydvl.utils import Dataset, Scorer, Utility
+from pydvl.value import (MaxUpdates, RelativeTruncation,
+                         permutation_montecarlo_shapley)
+
+data = Dataset.from_sklearn(
+  load_breast_cancer(),
+  train_size=10,
+  stratify_by_target=True,
+  random_state=16,
+  )
+model = LogisticRegression()
+u = Utility(
+  model,
+  data,
+  Scorer("accuracy", default=0.0)
+  )
+values = permutation_montecarlo_shapley(
+  u,
+  truncation=RelativeTruncation(u, 0.05),
+  done=MaxUpdates(1000),
+  seed=16,
+  progress=True
+  )
+df = values.to_dataframe(column="data_value")
+```
 
 # Contributing
 
 Please open new issues for bugs, feature requests and extensions. You can read
 about the structure of the project, the toolchain and workflow in the [guide for
 contributions](CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyDVL Version: 0.9.0 Summary: The Python Data
+Metadata-Version: 2.1 Name: pyDVL Version: 0.9.1 Summary: The Python Data
 Valuation Library Author: appliedAI Institute gGmbH Project-URL: Source, https:
 //github.com/aai-institute/pydvl Project-URL: Documentation, https://pydvl.org
 Project-URL: TransferLab, https://transferlab.ai Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Science/Research Classifier: Topic
 :: Scientific/Engineering :: Artificial Intelligence Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
@@ -22,21 +22,20 @@
 Requires-Dist: zarr>=2.16.1; extra == "influence" Provides-Extra: ray Requires-
 Dist: ray>=0.8; extra == "ray"
                                  [pyDVL Logo]
                          A library for data valuation.
  _[_P_y_P_I_]_[_V_e_r_s_i_o_n_]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_[_L_i_c_e_n_s_e_]_[_B_u_i_l_d_ _s_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/
           _a_a_i_-_i_n_s_t_i_t_u_t_e_/_p_y_D_V_L_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_V_N_7_D_N_D_E_0_F_V_]_[_D_O_I_]
 **pyDVL** collects algorithms for **Data Valuation** and **Influence Function**
-computation. Refer to the [Methods](https://pydvl.org/devel/getting-started/
-methods/) page of our documentation for a list of all implemented methods.
-**Data Valuation** for machine learning is the task of assigning a scalar to
-each element of a training set which reflects its contribution to the final
-performance or outcome of some model trained on it. Some concepts of value
-depend on a specific model of interest, while others are model-agnostic. pyDVL
-focuses on model-dependent methods.
+computation. Here is the list of [all methods implemented](https://pydvl.org/
+devel/getting-started/methods/). **Data Valuation** for machine learning is the
+task of assigning a scalar to each element of a training set which reflects its
+contribution to the final performance or outcome of some model trained on it.
+Some concepts of value depend on a specific model of interest, while others are
+model-agnostic. pyDVL focuses on model-dependent methods.
                              [best sample removal]
     Comparison of different data valuation methods on best sample removal.
 The **Influence Function** is an infinitesimal measure of the effect that
 single training points have over the parameters of a model, or any function
 thereof. In particular, in machine learning they are also used to compute the
 effect of training samples over individual test points.
                              [best sample removal]
@@ -45,78 +44,75 @@
 # Installation To install the latest release use: ```shell $ pip install pyDVL
 ``` You can also install the latest development version from [TestPyPI](https:/
 /test.pypi.org/project/pyDVL/): ```shell pip install pyDVL --index-url https://
 test.pypi.org/simple/ ``` pyDVL has also extra dependencies for certain
 functionalities, e.g. for using influence functions run ```shell $ pip install
 pyDVL[influence] ``` For more instructions and information refer to [Installing
 pyDVL ](https://pydvl.org/stable/getting-started/#installation) in the
-documentation. # Usage In the following subsections, we will showcase the usage
-of pyDVL for Data Valuation and Influence Functions using simple examples. For
-more instructions and information refer to [Getting Started](https://pydvl.org/
-stable/getting-started/first-steps/) in the documentation. We provide several
-examples for data valuation (e.g. [Shapley Data Valuation](https://pydvl.org/
-stable/examples/shapley_basic_spotify/)) and for influence functions (e.g.
-[Influence Functions for Neural Networks](https://pydvl.org/stable/examples/
-influence_imagenet/)) with details on the algorithms and their applications. ##
-Influence Functions For influence computation, follow these steps: 1. Import
-the necessary packages (The exact packages depend on your specific use case).
-```python import torch from torch import nn from torch.utils.data import
-DataLoader, TensorDataset from pydvl.influence.torch import DirectInfluence
-from pydvl.influence.torch.util import NestedTorchCatAggregator,
-TorchNumpyConverter from pydvl.influence import SequentialInfluenceCalculator
-``` 2. Create PyTorch data loaders for your train and test splits. ```python
-input_dim = (5, 5, 5) output_dim = 3 train_x = torch.rand((10, *input_dim))
-train_y = torch.rand((10, output_dim)) test_x = torch.rand((5, *input_dim))
-test_y = torch.rand((5, output_dim)) train_data_loader = DataLoader
-(TensorDataset(train_x, train_y), batch_size=2) test_data_loader = DataLoader
-(TensorDataset(test_x, test_y), batch_size=1) ``` 3. Instantiate your neural
-network model. ```python nn_architecture = nn.Sequential( nn.Conv2d
-(in_channels=5, out_channels=3, kernel_size=3), nn.Flatten(), nn.Linear(27, 3),
-) ``` 4. Define your loss: ```python loss = nn.MSELoss() ``` 5. Instantiate an
-`InfluenceFunctionModel` and fit it to the training data ```python infl_model =
-DirectInfluence(nn_architecture, loss, hessian_regularization=0.01) infl_model
-= infl_model.fit(train_data_loader) ``` 6. For small input data call influence
-method on the fitted instance. ```python influences = infl_model.influences
-(test_x, test_y, train_x, train_y) ``` The result is a tensor of shape `
-(training samples x test samples)` that contains at index `(i, j`) the
-influence of training sample `i` on test sample `j`. 7. For larger data, wrap
-the model into a calculator and call methods on the calculator. ```python
-infl_calc = SequentialInfluenceCalculator(infl_model) # Lazy object providing
-arrays batch-wise in a sequential manner lazy_influences = infl_calc.influences
+documentation. # Usage Please read [Getting Started](https://pydvl.org/stable/
+getting-started/first-steps/) in the documentation for more instructions. We
+provide several examples for data valuation and for influence functions in our
+[Example Gallery](https://pydvl.org/stable/examples/). ## Influence Functions
+1. Import the necessary packages (the exact ones depend on your specific use
+case). 2. Create PyTorch data loaders for your train and test splits. 3.
+Instantiate your neural network model and define your loss function. 4.
+Instantiate an `InfluenceFunctionModel` and fit it to the training data 5. For
+small input data, you can call the `influences()` method on the fitted
+instance. The result is a tensor of shape `(training samples, test samples)`
+that contains at index `(i, j`) the influence of training sample `i` on test
+sample `j`. 6. For larger datasets, wrap the model into a "calculator" and call
+methods on it. This splits the computation into smaller chunks and allows for
+lazy evaluation and out-of-core computation. The higher the absolute value of
+the influence of a training sample on a test sample, the more influential it is
+for the chosen test sample, model and data loaders. The sign of the influence
+determines whether it is useful (positive) or harmful (negative). > **Note**
+pyDVL currently only support PyTorch for Influence Functions. We plan > to add
+support for Jax next. ```python import torch from torch import nn from
+torch.utils.data import DataLoader, TensorDataset from pydvl.influence import
+SequentialInfluenceCalculator from pydvl.influence.torch import DirectInfluence
+from pydvl.influence.torch.util import ( NestedTorchCatAggregator,
+TorchNumpyConverter, ) input_dim = (5, 5, 5) output_dim = 3 train_x, train_y =
+torch.rand((10, *input_dim)), torch.rand((10, output_dim)) test_x, test_y =
+torch.rand((5, *input_dim)), torch.rand((5, output_dim)) train_data_loader =
+DataLoader(TensorDataset(train_x, train_y), batch_size=2) test_data_loader =
+DataLoader(TensorDataset(test_x, test_y), batch_size=1) model = nn.Sequential
+( nn.Conv2d(in_channels=5, out_channels=3, kernel_size=3), nn.Flatten(),
+nn.Linear(27, 3), ) loss = nn.MSELoss() infl_model = DirectInfluence(model,
+loss, hessian_regularization=0.01) infl_model = infl_model.fit
+(train_data_loader) # For small datasets, instantiate the full influence
+matrix: influences = infl_model.influences(test_x, test_y, train_x, train_y) #
+For larger datasets, use the Influence calculators: infl_calc =
+SequentialInfluenceCalculator(infl_model) # Lazy object providing arrays batch-
+wise in a sequential manner lazy_influences = infl_calc.influences
 (test_data_loader, train_data_loader) # Trigger computation and pull results to
 memory influences = lazy_influences.compute(aggregator=NestedTorchCatAggregator
 ()) # Trigger computation and write results batch-wise to disk
-lazy_influences.to_zarr("influences_result", TorchNumpyConverter()) ``` The
-higher the absolute value of the influence of a training sample on a test
-sample, the more influential it is for the chosen test sample, model and data
-loaders. The sign of the influence determines whether it is useful (positive)
-or harmful (negative). > **Note** pyDVL currently only support PyTorch for
-Influence Functions. > We are planning to add support for Jax and perhaps
-TensorFlow or even Keras. ## Data Valuation The steps required to compute data
-values for your samples are: 1. Import the necessary packages (The exact
-packages depend on your specific use case). ```python import matplotlib.pyplot
-as plt from sklearn.datasets import load_breast_cancer from
-sklearn.linear_model import LogisticRegression from pydvl.utils import Dataset,
-Scorer, Utility from pydvl.value import ( compute_shapley_values, ShapleyMode,
-MaxUpdates, ) ``` 2. Create a `Dataset` object with your train and test splits.
-```python data = Dataset.from_sklearn( load_breast_cancer(), train_size=10,
-stratify_by_target=True, random_state=16, ) ``` 3. Create an instance of a
-`SupervisedModel` (basically any sklearn compatible predictor). ```python model
-= LogisticRegression() ``` 4. Create a `Utility` object to wrap the Dataset,
-the model and a scoring function. ```python u = Utility( model, data, Scorer
-("accuracy", default=0.0) ) ``` 5. Use one of the methods defined in the
-library to compute the values. In our example, we will use *Permutation
-Montecarlo Shapley*, an approximate method for computing Data Shapley values.
-```python values = compute_shapley_values( u,
-mode=ShapleyMode.PermutationMontecarlo, done=MaxUpdates(100), seed=16,
-progress=True ) ``` The result is a variable of type `ValuationResult` that
-contains the indices and their values as well as other attributes. The higher
-the value for an index, the more important it is for the chosen model, dataset
-and scorer. 6. (Optional) Convert the valuation result to a dataframe and
-analyze and visualize the values. ```python df = values.to_dataframe
+lazy_influences.to_zarr("influences_result", TorchNumpyConverter()) ``` ## Data
+Valuation The steps required to compute data values for your samples are: 1.
+Import the necessary packages (the exact ones will depend on your specific use
+case). 2. Create a `Dataset` object with your train and test splits. 3. Create
+an instance of a `SupervisedModel` (basically any sklearn compatible
+predictor), and wrap it in a `Utility` object together with the data and a
+scoring function. 4. Use one of the methods defined in the library to compute
+the values. In the example below, we will use *Permutation Montecarlo Shapley*,
+an approximate method for computing Data Shapley values. The result is a
+variable of type `ValuationResult` that contains the indices and their values
+as well as other attributes. 5. Convert the valuation result to a dataframe,
+and analyze and visualize the values. The higher the value for an index, the
+more important it is for the chosen model, dataset and scorer. Reciprocally,
+low-value points could be mislabelled, or out-of-distribution, and dropping
+them can improve the model's performance. ```python from sklearn.datasets
+import load_breast_cancer from sklearn.linear_model import LogisticRegression
+from pydvl.utils import Dataset, Scorer, Utility from pydvl.value import
+(MaxUpdates, RelativeTruncation, permutation_montecarlo_shapley) data =
+Dataset.from_sklearn( load_breast_cancer(), train_size=10,
+stratify_by_target=True, random_state=16, ) model = LogisticRegression() u =
+Utility( model, data, Scorer("accuracy", default=0.0) ) values =
+permutation_montecarlo_shapley( u, truncation=RelativeTruncation(u, 0.05),
+done=MaxUpdates(1000), seed=16, progress=True ) df = values.to_dataframe
 (column="data_value") ``` # Contributing Please open new issues for bugs,
 feature requests and extensions. You can read about the structure of the
 project, the toolchain and workflow in the [guide for contributions]
 (CONTRIBUTING.md). # License pyDVL is distributed under [LGPL-3.0](https://
 www.gnu.org/licenses/lgpl-3.0.html). A complete version can be found in two
 files: [here](LICENSE) and [here](COPYING.LESSER). All contributions will be
 distributed under this license.
```

### Comparing `pydvl-0.9/src/pyDVL.egg-info/SOURCES.txt` & `pydvl-0.9.1/src/pyDVL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/influence/__init__.py` & `pydvl-0.9.1/src/pydvl/influence/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/influence/array.py` & `pydvl-0.9.1/src/pydvl/influence/array.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 and lazily evaluated. It includes abstract base classes for converting between tensor
 types and NumPy arrays, aggregating blocks of data, and abstract representations of
 lazy arrays. Concrete implementations are provided for handling chunked lazy arrays
 (chunked in one resp. two dimensions), with support for efficient storage and retrieval
 using the Zarr library.
 """
 
+import logging
 from abc import ABC, abstractmethod
 from typing import Callable, Generator, Generic, List, Optional, Tuple, Union
 
 import zarr
 from numpy.typing import NDArray
 from zarr.storage import StoreLike
 
+from ..utils import log_duration
 from .base_influence_function_model import TensorType
 
 
 class NumpyConverter(Generic[TensorType], ABC):
     """
     Base class for converting TensorType objects into numpy arrays and vice versa.
     """
@@ -115,14 +117,15 @@
     """
 
     def __init__(
         self, generator_factory: Callable[[], Generator[TensorType, None, None]]
     ):
         self.generator_factory = generator_factory
 
+    @log_duration(log_level=logging.INFO)
     def compute(self, aggregator: Optional[SequenceAggregator] = None):
         """
         Computes and optionally aggregates the chunks of the array using the provided
         aggregator. This method initiates the generation of chunks and then
         combines them according to the aggregator's logic.
 
         Args:
@@ -135,14 +138,15 @@
                 depends on the aggregator used.
 
         """
         if aggregator is None:
             aggregator = ListAggregator()
         return aggregator(self.generator_factory())
 
+    @log_duration(log_level=logging.INFO)
     def to_zarr(
         self,
         path_or_url: Union[str, StoreLike],
         converter: NumpyConverter,
         return_stored: bool = False,
         overwrite: bool = False,
     ) -> Optional[zarr.Array]:
@@ -219,14 +223,15 @@
         self,
         generator_factory: Callable[
             [], Generator[Generator[TensorType, None, None], None, None]
         ],
     ):
         self.generator_factory = generator_factory
 
+    @log_duration(log_level=logging.INFO)
     def compute(self, aggregator: Optional[NestedSequenceAggregator] = None):
         """
         Computes and optionally aggregates the chunks of the array using the provided
         aggregator. This method initiates the generation of chunks and then
         combines them according to the aggregator's logic.
 
         Args:
@@ -240,14 +245,15 @@
             depends on the aggregator used.
 
         """
         if aggregator is None:
             aggregator = NestedListAggregator()
         return aggregator(self.generator_factory())
 
+    @log_duration(log_level=logging.INFO)
     def to_zarr(
         self,
         path_or_url: Union[str, StoreLike],
         converter: NumpyConverter,
         return_stored: bool = False,
         overwrite: bool = False,
     ) -> Optional[zarr.Array]:
```

### Comparing `pydvl-0.9/src/pydvl/influence/base_influence_function_model.py` & `pydvl-0.9.1/src/pydvl/influence/base_influence_function_model.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/influence/influence_calculator.py` & `pydvl-0.9.1/src/pydvl/influence/influence_calculator.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/influence/torch/functional.py` & `pydvl-0.9.1/src/pydvl/influence/torch/functional.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/influence/torch/influence_function_model.py` & `pydvl-0.9.1/src/pydvl/influence/torch/influence_function_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,14 +359,15 @@
     @property
     def is_fitted(self):
         try:
             return self.hessian is not None
         except AttributeError:
             return False
 
+    @log_duration(log_level=logging.INFO)
     def fit(self, data: DataLoader) -> DirectInfluence:
         """
         Compute the hessian matrix based on a provided dataloader.
 
         Args:
             data: The data to compute the Hessian with.
 
@@ -496,14 +497,15 @@
     @property
     def is_fitted(self):
         try:
             return self.train_dataloader is not None
         except AttributeError:
             return False
 
+    @log_duration(log_level=logging.INFO)
     def fit(self, data: DataLoader) -> CgInfluence:
         self.train_dataloader = data
         if self.pre_conditioner is not None:
             hvp = create_hvp_function(
                 self.model,
                 self.loss,
                 self.train_dataloader,
@@ -812,14 +814,15 @@
     @property
     def is_fitted(self):
         try:
             return self.train_dataloader is not None
         except AttributeError:
             return False
 
+    @log_duration(log_level=logging.INFO)
     def fit(self, data: DataLoader) -> LissaInfluence:
         self.train_dataloader = data
         return self
 
     @log_duration
     def _solve_hvp(self, rhs: torch.Tensor) -> torch.Tensor:
         h_estimate = self.h0 if self.h0 is not None else torch.clone(rhs)
@@ -944,14 +947,15 @@
     @property
     def is_fitted(self):
         try:
             return self.low_rank_representation is not None
         except AttributeError:
             return False
 
+    @log_duration(log_level=logging.INFO)
     def fit(self, data: DataLoader) -> ArnoldiInfluence:
         r"""
         Fitting corresponds to the computation of the low rank decomposition
 
         \[ V D^{-1} V^T \]
 
         of the Hessian defined by the provided data loader.
@@ -1200,14 +1204,15 @@
             grad_y[key] /= data_len
 
         for hook in hooks:
             hook.remove()
 
         return forward_x, grad_y
 
+    @log_duration(log_level=logging.INFO)
     def fit(self, data: DataLoader) -> EkfacInfluence:
         """
         Compute the KFAC blocks for each layer of the model, using the provided data.
         It then creates an EkfacRepresentation object that stores the KFAC blocks for
         each layer, their eigenvalue decomposition and diagonal values.
         """
         forward_x, grad_y = self._get_kfac_blocks(data)
@@ -1708,12 +1713,13 @@
     @property
     def is_fitted(self):
         try:
             return self.low_rank_representation is not None
         except AttributeError:
             return False
 
+    @log_duration(log_level=logging.INFO)
     def fit(self, data: DataLoader):
         self.low_rank_representation = model_hessian_nystroem_approximation(
             self.model, self.loss, data, self.rank
         )
         return self
```

### Comparing `pydvl-0.9/src/pydvl/influence/torch/pre_conditioner.py` & `pydvl-0.9.1/src/pydvl/influence/torch/pre_conditioner.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/influence/torch/util.py` & `pydvl-0.9.1/src/pydvl/influence/torch/util.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/parallel/__init__.py` & `pydvl-0.9.1/src/pydvl/parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/parallel/backend.py` & `pydvl-0.9.1/src/pydvl/parallel/backend.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/parallel/backends/joblib.py` & `pydvl-0.9.1/src/pydvl/parallel/backends/joblib.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/parallel/backends/ray.py` & `pydvl-0.9.1/src/pydvl/parallel/backends/ray.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/parallel/config.py` & `pydvl-0.9.1/src/pydvl/parallel/config.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/parallel/futures/__init__.py` & `pydvl-0.9.1/src/pydvl/parallel/futures/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 @deprecated(
     target=None,
     deprecated_in="0.9.0",
     remove_in="0.10.0",
 )
 def init_executor(
     max_workers: Optional[int] = None,
-    config: ParallelConfig = ParallelConfig(),
+    config: Optional[ParallelConfig] = None,
     **kwargs,
 ) -> Generator[Executor, None, None]:
     """Initializes a futures executor for the given parallel configuration.
 
     Args:
         max_workers: Maximum number of concurrent tasks.
         config: instance of [ParallelConfig][pydvl.utils.config.ParallelConfig]
@@ -46,13 +46,17 @@
         ``` python
         from pydvl.parallel.futures import init_executor
         with init_executor() as executor:
             results = list(executor.map(lambda x: x + 1, range(5)))
         assert results == [1, 2, 3, 4, 5]
         ```
     """
+
+    if config is None:
+        config = ParallelConfig()
+
     try:
         cls = ParallelBackend.BACKENDS[config.backend]
         with cls.executor(max_workers=max_workers, config=config, **kwargs) as e:
             yield e
     except KeyError:
         raise NotImplementedError(f"Unexpected parallel backend {config.backend}")
```

### Comparing `pydvl-0.9/src/pydvl/parallel/futures/ray.py` & `pydvl-0.9.1/src/pydvl/parallel/futures/ray.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/parallel/map_reduce.py` & `pydvl-0.9.1/src/pydvl/parallel/map_reduce.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/reporting/plots.py` & `pydvl-0.9.1/src/pydvl/reporting/plots.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/reporting/scores.py` & `pydvl-0.9.1/src/pydvl/reporting/scores.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/caching/__init__.py` & `pydvl-0.9.1/src/pydvl/utils/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/caching/base.py` & `pydvl-0.9.1/src/pydvl/utils/caching/base.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/caching/config.py` & `pydvl-0.9.1/src/pydvl/utils/caching/config.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/caching/disk.py` & `pydvl-0.9.1/src/pydvl/utils/caching/disk.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/caching/memcached.py` & `pydvl-0.9.1/src/pydvl/utils/caching/memcached.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/caching/memory.py` & `pydvl-0.9.1/src/pydvl/utils/caching/memory.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/dataset.py` & `pydvl-0.9.1/src/pydvl/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/functional.py` & `pydvl-0.9.1/src/pydvl/utils/functional.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/numeric.py` & `pydvl-0.9.1/src/pydvl/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/progress.py` & `pydvl-0.9.1/src/pydvl/utils/progress.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,23 +35,37 @@
         it = takewhile(lambda _: not done(result), cycle(indices))
         for i in it:
             yield i
             pbar.update(100 * done.completion() - pbar.n)
             pbar.refresh()
 
 
-def log_duration(func):
+def log_duration(_func=None, *, log_level=logging.DEBUG):
     """
-    Decorator to log execution time of a function
+    Decorator to log execution time of a function with a configurable logging level.
+    It can be used with or without specifying a log level.
     """
 
-    @wraps(func)
-    def wrapper_log_duration(*args, **kwargs):
-        func_name = func.__qualname__
-        logger.info(f"Function '{func_name}' is starting.")
-        start_time = time()
-        result = func(*args, **kwargs)
-        duration = time() - start_time
-        logger.info(f"Function '{func_name}' completed. Duration: {duration:.2f} sec")
-        return result
+    def decorator_log_duration(func):
+        @wraps(func)
+        def wrapper_log_duration(*args, **kwargs):
+            func_name = func.__qualname__
+            duration_logger = logging.getLogger(func_name)
+            duration_logger.setLevel(log_level)
+            duration_logger.log(log_level, f"Function '{func_name}' is starting.")
+            start_time = time()
+            result = func(*args, **kwargs)
+            duration = time() - start_time
+            duration_logger.log(
+                log_level,
+                f"Function '{func_name}' completed. " f"Duration: {duration:.2f} sec",
+            )
+            return result
 
-    return wrapper_log_duration
+        return wrapper_log_duration
+
+    if _func is None:
+        # If log_duration was called without arguments, return decorator
+        return decorator_log_duration
+    else:
+        # If log_duration was called with a function, apply decorator directly
+        return decorator_log_duration(_func)
```

### Comparing `pydvl-0.9/src/pydvl/utils/score.py` & `pydvl-0.9.1/src/pydvl/utils/score.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/status.py` & `pydvl-0.9.1/src/pydvl/utils/status.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/types.py` & `pydvl-0.9.1/src/pydvl/utils/types.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/utils/utility.py` & `pydvl-0.9.1/src/pydvl/utils/utility.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/games.py` & `pydvl-0.9.1/src/pydvl/value/games.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/least_core/__init__.py` & `pydvl-0.9.1/src/pydvl/value/least_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/least_core/common.py` & `pydvl-0.9.1/src/pydvl/value/least_core/common.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/least_core/montecarlo.py` & `pydvl-0.9.1/src/pydvl/value/least_core/montecarlo.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/least_core/naive.py` & `pydvl-0.9.1/src/pydvl/value/least_core/naive.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/loo/loo.py` & `pydvl-0.9.1/src/pydvl/value/loo/loo.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/oob/oob.py` & `pydvl-0.9.1/src/pydvl/value/oob/oob.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/result.py` & `pydvl-0.9.1/src/pydvl/value/result.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/sampler.py` & `pydvl-0.9.1/src/pydvl/value/sampler.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/semivalues.py` & `pydvl-0.9.1/src/pydvl/value/semivalues.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/shapley/__init__.py` & `pydvl-0.9.1/src/pydvl/value/shapley/__init__.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/shapley/classwise.py` & `pydvl-0.9.1/src/pydvl/value/shapley/classwise.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/shapley/common.py` & `pydvl-0.9.1/src/pydvl/value/shapley/common.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/shapley/gt.py` & `pydvl-0.9.1/src/pydvl/value/shapley/gt.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/shapley/knn.py` & `pydvl-0.9.1/src/pydvl/value/shapley/knn.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/shapley/montecarlo.py` & `pydvl-0.9.1/src/pydvl/value/shapley/montecarlo.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/shapley/naive.py` & `pydvl-0.9.1/src/pydvl/value/shapley/naive.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/shapley/owen.py` & `pydvl-0.9.1/src/pydvl/value/shapley/owen.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/shapley/truncated.py` & `pydvl-0.9.1/src/pydvl/value/shapley/truncated.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/shapley/types.py` & `pydvl-0.9.1/src/pydvl/value/shapley/types.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/src/pydvl/value/stopping.py` & `pydvl-0.9.1/src/pydvl/value/stopping.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/tests/test_plugin.py` & `pydvl-0.9.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pydvl-0.9/tests/test_results.py` & `pydvl-0.9.1/tests/test_results.py`

 * *Files identical despite different names*

