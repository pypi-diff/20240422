# Comparing `tmp/ts3l-0.21.tar.gz` & `tmp/ts3l-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts3l-0.21.tar", last modified: Tue Mar 12 07:41:54 2024, max compression
+gzip compressed data, was "ts3l-0.30.tar", last modified: Mon Apr 22 05:18:57 2024, max compression
```

## Comparing `ts3l-0.21.tar` & `ts3l-0.30.tar`

### file list

```diff
@@ -1,56 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.178120 ts3l-0.21/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-12 07:41:46.000000 ts3l-0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14218 2024-03-12 07:41:54.178120 ts3l-0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13634 2024-03-12 07:41:46.000000 ts3l-0.21/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 07:41:54.178120 ts3l-0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-12 07:41:46.000000 ts3l-0.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.170120 ts3l-0.21/test/
--rw-r--r--   0 runner    (1001) docker     (127)    14769 2024-03-12 07:41:46.000000 ts3l-0.21/test/test_scarf.py
--rw-r--r--   0 runner    (1001) docker     (127)    16538 2024-03-12 07:41:46.000000 ts3l-0.21/test/test_subtab.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-03-12 07:41:46.000000 ts3l-0.21/test/test_vime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.170120 ts3l-0.21/ts3l/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.174120 ts3l-0.21/ts3l/models/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.174120 ts3l-0.21/ts3l/models/scarf/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/models/scarf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/models/scarf/scarf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.174120 ts3l-0.21/ts3l/models/subtab/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/models/subtab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/models/subtab/subtab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.174120 ts3l-0.21/ts3l/models/vime/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/models/vime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/models/vime/vime.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/models/vime/vime_self.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/models/vime/vime_semi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.174120 ts3l-0.21/ts3l/pl_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/pl_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/pl_modules/base_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/pl_modules/scarf_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/pl_modules/subtab_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/pl_modules/vime_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.174120 ts3l-0.21/ts3l/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.178120 ts3l-0.21/ts3l/utils/scarf_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/scarf_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/scarf_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/scarf_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/scarf_utils/scarf_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.178120 ts3l-0.21/ts3l/utils/subtab_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/subtab_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/subtab_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/subtab_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/subtab_utils/subtab_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.178120 ts3l-0.21/ts3l/utils/vime_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/vime_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/vime_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-03-12 07:41:46.000000 ts3l-0.21/ts3l/utils/vime_utils/vime_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 07:41:54.178120 ts3l-0.21/ts3l.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14218 2024-03-12 07:41:54.000000 ts3l-0.21/ts3l.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-12 07:41:54.000000 ts3l-0.21/ts3l.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 07:41:54.000000 ts3l-0.21/ts3l.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-12 07:41:54.000000 ts3l-0.21/ts3l.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-12 07:41:54.000000 ts3l-0.21/ts3l.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 05:18:49.000000 ts3l-0.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-04-22 05:18:57.393371 ts3l-0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-04-22 05:18:49.000000 ts3l-0.30/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 05:18:57.393371 ts3l-0.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-22 05:18:49.000000 ts3l-0.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.385371 ts3l-0.30/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-22 05:18:49.000000 ts3l-0.30/test/test_dae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-22 05:18:49.000000 ts3l-0.30/test/test_scarf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-22 05:18:49.000000 ts3l-0.30/test/test_subtab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-22 05:18:49.000000 ts3l-0.30/test/test_vime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.385371 ts3l-0.30/ts3l/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/common/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/dae/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/dae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/dae/dae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/scarf/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/scarf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/scarf/scarf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/subtab/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/subtab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/subtab/subtab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/models/vime/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/vime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/vime/vime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/vime/vime_self.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/models/vime/vime_semi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.389371 ts3l-0.30/ts3l/pl_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/dae_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/scarf_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/subtab_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/pl_modules/vime_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/base_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l/utils/dae_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/dae_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/dae_utils/dae_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/dae_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l/utils/scarf_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/scarf_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/scarf_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/scarf_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/scarf_utils/scarf_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l/utils/subtab_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/subtab_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/subtab_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/subtab_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/subtab_utils/subtab_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l/utils/vime_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/vime_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/vime_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-22 05:18:49.000000 ts3l-0.30/ts3l/utils/vime_utils/vime_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:18:57.393371 ts3l-0.30/ts3l.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-04-22 05:18:57.000000 ts3l-0.30/ts3l.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-22 05:18:57.000000 ts3l-0.30/ts3l.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:18:57.000000 ts3l-0.30/ts3l.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 05:18:57.000000 ts3l-0.30/ts3l.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 05:18:57.000000 ts3l-0.30/ts3l.egg-info/top_level.txt
```

### Comparing `ts3l-0.21/LICENSE` & `ts3l-0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `ts3l-0.21/PKG-INFO` & `ts3l-0.30/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ts3l
-Version: 0.21
+Version: 0.30
 Summary: A PyTorch Lightning-based library for self- and semi-supervised learning on tabular data.
 Home-page: https://github.com/Alcoholrithm/TabularS3L
 Author: Minwook Kim
 Author-email: kmiiiaa@pusan.ac.kr
-Keywords: tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF
+Keywords: tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF DenoisingAutoEncoder
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: torch
@@ -17,14 +17,15 @@
 Requires-Dist: torchmetrics
 
 # TabularS3L
 
 [**Overview**](#tabulars3l)
 | [**Installation**](#installation)
 | [**Available Models with Quick Start Guides**](#available-models-with-quick-start)
+| [**Benchmark**](#benchmark)
 | [**To DO**](#to-do)
 | [**Contributing**](#contributing)
 | [**Credit**](#credit)
 
 
 [![pypi](https://img.shields.io/pypi/v/ts3l)](https://pypi.org/project/ts3l/0.20/)
 [![DOI](https://zenodo.org/badge/756740921.svg)](https://zenodo.org/doi/10.5281/zenodo.10776537)
@@ -41,26 +42,121 @@
 
 ## Available Models with Quick Start
 
 TabularS3L employs a two-phase learning approach, where the learning strategies differ between phases. Below is an overview of the models available within TabularS3L, highlighting the learning strategies employed in each phase. The abbreviations 'Self-SL', 'Semi-SL', and 'SL' represent self-supervised learning, semi-supervised learning, and supervised learning, respectively.
 
 | Model | First Phase | Second Phase |
 |:---:|:---:|:---:|
+| **DAE** ([GitHub](https://github.com/ryancheunggit/tabular_dae))| Self-SL | SL |
 | **VIME** ([NeurIPS'20](https://proceedings.neurips.cc/paper/2020/hash/7d97667a3e056acab9aaf653807b4a03-Abstract.html)) | Self-SL | Semi-SL or SL |
 | **SubTab** ([NeurIPS'21](https://proceedings.neurips.cc/paper/2021/hash/9c8661befae6dbcd08304dbf4dcaf0db-Abstract.html)) | Self-SL | SL |
 | **SCARF** ([ICLR'22](https://iclr.cc/virtual/2022/spotlight/6297))| Self-SL | SL |
 
+#### Denoising AutoEncoder (DAE)
+DAE processes input data that has been partially corrupted, producing clean data and predicting which features are corrupted during the self-supervised learning.
+The denoising task enables the model to learn the input distribution and generate latent representations that are robust to corruption. 
+These latent representations can be utilized for a variety of downstream tasks.
+
+<details close>
+  <summary>Quick Start</summary>
+  
+  ```python
+  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
+
+  # Prepare the DAELightning Module
+  from ts3l.pl_modules import DAELightning
+  from ts3l.utils.dae_utils import DAEDataset, DAECollateFN
+  from ts3l.utils import TS3LDataModule
+  from ts3l.utils.dae_utils import DAEConfig
+  from pytorch_lightning import Trainer
+  
+  metric = "accuracy_score"
+  input_dim = X_train.shape[1]
+  hidden_dim = 1024
+  output_dim = 2
+  encoder_depth=4
+  head_depth = 2
+  noise_type = "Swap"
+  noise_ratio = 0.3
+  
+  max_epochs = 20
+  batch_size = 128
+  
+  X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
+  
+  config = DAEConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
+  input_dim=input_dim, hidden_dim=hidden_dim,
+  output_dim=output_dim, encoder_depth=encoder_depth,
+  head_depth = head_depth,
+  noise_type = noise_type,
+  noise_ratio = noise_ratio,
+  num_categoricals=len(category_cols), num_continuous=len(continuous_cols)
+  )
+  
+  pl_dae = DAELightning(config)
+  
+  ### First Phase Learning
+  train_ds = DAEDataset(X = X_train, unlabeled_data = X_unlabeled, continuous_cols = continuous_cols, category_cols = category_cols)
+  valid_ds = DAEDataset(X = X_valid, continuous_cols = continuous_cols, category_cols = category_cols)
+  
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=DAECollateFN(config), valid_collate_fn=DAECollateFN(config))
+  
+  trainer = Trainer(
+                      accelerator = 'cpu',
+                      max_epochs = max_epochs,
+                      num_sanity_val_steps = 2,
+      )
+  
+  trainer.fit(pl_dae, datamodule)
+  
+  ### Second Phase Learning
+  
+  pl_dae.set_second_phase()
+  
+  train_ds = DAEDataset(X = X_train, Y = y_train.values, unlabeled_data=X_unlabeled, continuous_cols=continuous_cols, category_cols=category_cols)
+  valid_ds = DAEDataset(X = X_valid, Y = y_valid.values, continuous_cols=continuous_cols, category_cols=category_cols)
+          
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted")
+  
+  trainer = Trainer(
+                      accelerator = 'cpu',
+                      max_epochs = max_epochs,
+                      num_sanity_val_steps = 2,
+      )
+  
+  trainer.fit(pl_dae, datamodule)
+  
+  # Evaluation
+  from sklearn.metrics import accuracy_score
+  import torch
+  from torch.nn import functional as F
+  from torch.utils.data import DataLoader, SequentialSampler
+  
+  test_ds = DAEDataset(X_test, category_cols=category_cols, continuous_cols=continuous_cols)
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds))
+  
+  preds = trainer.predict(pl_dae, test_dl)
+          
+  preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
+  
+  accuracy = accuracy_score(y_test, preds.argmax(1))
+  
+  print("Accuracy %.2f" % accuracy)
+  ```
+
+</details>
+
 #### VIME: Extending the Success of Self- and Semi-supervised Learning to Tabular Domain
 VIME enhances tabular data learning through a dual approach. In its first phase, it utilize a pretext task of estimating mask vectors from corrupted tabular data, alongside a reconstruction pretext task for self-supervised learning. The second phase leverages consistency regularization on unlabeled data.
 
 <details close>
   <summary>Quick Start</summary>
   
   ```python
-  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, category_cols, and continuous_cols
+  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
 
   # Prepare the VIMELightning Module
   from ts3l.pl_modules import VIMELightning
   from ts3l.utils.vime_utils import VIMEDataset
   from ts3l.utils import TS3LDataModule
   from ts3l.utils.vime_utils import VIMEConfig
   from pytorch_lightning import Trainer
@@ -71,65 +167,60 @@
   output_dim = 2
   alpha1 = 2.0
   alpha2 = 2.0
   beta = 1.0
   K = 3
   p_m = 0.2
 
-  data_hparams = {
-              "K" : K,
-              "p_m" : p_m
-          }
-
   batch_size = 128
 
   X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
 
   config = VIMEConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
   input_dim=input_dim, hidden_dim=hidden_dim,
   output_dim=output_dim, alpha1=alpha1, alpha2=alpha2, 
-  beta=beta, K=K,
+  beta=beta, K=K, p_m = p_m,
   num_categoricals=len(category_cols), num_continuous=len(continuous_cols)
   )
 
   pl_vime = VIMELightning(config)
 
   ### First Phase Learning
-  train_ds = VIMEDataset(X = X_train, unlabeled_data = X_unlabeled, data_hparams=data_hparams, continous_cols = continuous_cols, category_cols = category_cols)
-  valid_ds = VIMEDataset(X = X_valid, data_hparams=data_hparams, continous_cols = continuous_cols, category_cols = category_cols)
+  train_ds = VIMEDataset(X = X_train, unlabeled_data = X_unlabeled, config=config, continuous_cols = continuous_cols, category_cols = category_cols)
+  valid_ds = VIMEDataset(X = X_valid, config=config, continuous_cols = continuous_cols, category_cols = category_cols)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', n_jobs = 4)
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random')
 
   trainer = Trainer(
                       accelerator = 'cpu',
-                      max_epochs = 10,
+                      max_epochs = 20,
                       num_sanity_val_steps = 2,
       )
 
   trainer.fit(pl_vime, datamodule)
 
   ### Second Phase Learning
   from ts3l.utils.vime_utils import VIMESemiSLCollateFN
 
   pl_vime.set_second_phase()
 
-  train_ds = VIMEDataset(X_train, y_train.values, data_hparams, unlabeled_data=X_unlabeled, continous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
-  valid_ds = VIMEDataset(X_valid, y_valid.values, data_hparams, continous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  train_ds = VIMEDataset(X_train, y_train.values, config, unlabeled_data=X_unlabeled, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  valid_ds = VIMEDataset(X_valid, y_valid.values, config, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
           
   datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=VIMESemiSLCollateFN())
 
   trainer.fit(pl_vime, datamodule)
 
   # Evaluation
   from sklearn.metrics import accuracy_score
   import torch
   from torch.nn import functional as F
   from torch.utils.data import DataLoader, SequentialSampler
 
-  test_ds = VIMEDataset(X_test, category_cols=category_cols, continous_cols=continuous_cols, is_second_phase=True)
+  test_ds = VIMEDataset(X_test, category_cols=category_cols, continuous_cols=continuous_cols, is_second_phase=True)
   test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds))
 
   preds = trainer.predict(pl_vime, test_dl)
           
   preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
 
   accuracy = accuracy_score(y_test, preds.argmax(1))
@@ -167,41 +258,32 @@
   n_subsets = 4
   overlap_ratio = 0.75
 
   mask_ratio = 0.1
   noise_type = "Swap"
   noise_level = 0.1
 
-  data_hparams = {
-              "n_subsets" : n_subsets,
-              "overlap_ratio" : overlap_ratio,
-              "mask_ratio" : mask_ratio,
-              "noise_type" : noise_type,
-              "noise_level" : noise_level,
-              "n_column" : input_dim
-          }
-
   batch_size = 128
   max_epochs = 3
 
   X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
 
   config = SubTabConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
   input_dim=input_dim, hidden_dim=hidden_dim,
   output_dim=output_dim, tau=tau, use_cosine_similarity= use_cosine_similarity, use_contrastive=use_contrastive, use_distance=use_distance, 
-  n_subsets=n_subsets, overlap_ratio=overlap_ratio
+  n_subsets=n_subsets, overlap_ratio=overlap_ratio, mask_ratio=mask_ratio, noise_type=noise_type, noise_level=noise_level
   )
 
   pl_subtab = SubTabLightning(config)
 
   ### First Phase Learning
   train_ds = SubTabDataset(X_train, unlabeled_data=X_unlabeled)
   valid_ds = SubTabDataset(X_valid)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams), n_jobs = 4)
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=SubTabCollateFN(config), valid_collate_fn=SubTabCollateFN(config), n_jobs = 4)
 
   trainer = Trainer(
                       accelerator = 'cpu',
                       max_epochs = max_epochs,
                       num_sanity_val_steps = 2,
       )
 
@@ -210,26 +292,26 @@
   ### Second Phase Learning
 
   pl_subtab.set_second_phase()
 
   train_ds = SubTabDataset(X_train, y_train.values)
   valid_ds = SubTabDataset(X_valid, y_valid.values)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams))
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=SubTabCollateFN(config), valid_collate_fn=SubTabCollateFN(config))
 
   trainer.fit(pl_subtab, datamodule)
 
   # Evaluation
   from sklearn.metrics import accuracy_score
   import torch
   from torch.nn import functional as F
   from torch.utils.data import DataLoader, SequentialSampler
 
   test_ds = SubTabDataset(X_test)
-  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4, collate_fn=SubTabCollateFN(data_hparams))
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4, collate_fn=SubTabCollateFN(config))
 
   preds = trainer.predict(pl_subtab, test_dl)
           
   preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
 
   accuracy = accuracy_score(y_test, preds.argmax(1))
 
@@ -243,139 +325,148 @@
 
 <details close>
   <summary>Quick Start</summary>
   
   ```python
   # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
 
-  # Prepare the SubTabLightning Module
-  from ts3l.pl_modules import SubTabLightning
-  from ts3l.utils.subtab_utils import SubTabDataset, SubTabCollateFN
+  # Prepare the SCARFLightning Module
+  from ts3l.pl_modules import SCARFLightning
+  from ts3l.utils.scarf_utils import SCARFDataset
   from ts3l.utils import TS3LDataModule
-  from ts3l.utils.subtab_utils import SubTabConfig
+  from ts3l.utils.scarf_utils import SCARFConfig
   from pytorch_lightning import Trainer
 
   metric = "accuracy_score"
   input_dim = X_train.shape[1]
   hidden_dim = 1024
   output_dim = 2
-  tau = 1.0
-  use_cosine_similarity = True
-  use_contrastive = True
-  use_distance = True
-  n_subsets = 4
-  overlap_ratio = 0.75
+  encoder_depth = 3
+  head_depth = 1
+  dropout_rate = 0.04
 
-  mask_ratio = 0.1
-  noise_type = "Swap"
-  noise_level = 0.1
-
-  data_hparams = {
-              "n_subsets" : n_subsets,
-              "overlap_ratio" : overlap_ratio,
-              "mask_ratio" : mask_ratio,
-              "noise_type" : noise_type,
-              "noise_level" : noise_level,
-              "n_column" : input_dim
-          }
+  corruption_rate = 0.6
 
   batch_size = 128
-  max_epochs = 3
+  max_epochs = 10
 
   X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
 
-  config = SubTabConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
+  config = SCARFConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
   input_dim=input_dim, hidden_dim=hidden_dim,
-  output_dim=output_dim, tau=tau, use_cosine_similarity= use_cosine_similarity, use_contrastive=use_contrastive, use_distance=use_distance, 
-  n_subsets=n_subsets, overlap_ratio=overlap_ratio
+  output_dim=output_dim, encoder_depth=encoder_depth, head_depth=head_depth,
+  dropout_rate=dropout_rate, corruption_rate = corruption_rate
   )
 
-  pl_subtab = SubTabLightning(config)
+  pl_scarf = SCARFLightning(config)
 
   ### First Phase Learning
-  train_ds = SubTabDataset(X_train, unlabeled_data=X_unlabeled)
-  valid_ds = SubTabDataset(X_valid)
+  train_ds = SCARFDataset(X_train, unlabeled_data=X_unlabeled, config = config)
+  valid_ds = SCARFDataset(X_valid, config=config)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams), n_jobs = 4)
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size=batch_size, train_sampler="random")
 
   trainer = Trainer(
                       accelerator = 'cpu',
                       max_epochs = max_epochs,
                       num_sanity_val_steps = 2,
       )
 
-  trainer.fit(pl_subtab, datamodule)
+  trainer.fit(pl_scarf, datamodule)
 
   ### Second Phase Learning
 
-  pl_subtab.set_second_phase()
+  pl_scarf.set_second_phase()
 
-  train_ds = SubTabDataset(X_train, y_train.values)
-  valid_ds = SubTabDataset(X_valid, y_valid.values)
+  train_ds = SCARFDataset(X_train, y_train.values, is_second_phase=True)
+  valid_ds = SCARFDataset(X_valid, y_valid.values, is_second_phase=True)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams))
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted")
 
-  trainer.fit(pl_subtab, datamodule)
+  trainer.fit(pl_scarf, datamodule)
 
   # Evaluation
   from sklearn.metrics import accuracy_score
   import torch
   from torch.nn import functional as F
   from torch.utils.data import DataLoader, SequentialSampler
 
-  test_ds = SubTabDataset(X_test)
-  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4, collate_fn=SubTabCollateFN(data_hparams))
+  test_ds = SCARFDataset(X_test, is_second_phase=True)
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4)
 
-  preds = trainer.predict(pl_subtab, test_dl)
+  preds = trainer.predict(pl_scarf, test_dl)
           
   preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
 
   accuracy = accuracy_score(y_test, preds.argmax(1))
 
   print("Accuracy %.2f" % accuracy)
   ```
 
 </details>
 
-#### To DO
+
+## Benchmark
+
+We provide a simple benchmark using TabularS3L against XGBoost. The train-validation-test ratio is 6:2:2 and we tuned each model over 50 trials using Optuna. The results are the average of the random seeds [0,4]. The best results are bold. 'acc', 'b-acc', and 'mse' mean 'Accuracy', 'Balanced Accuracy', and 'Mean Squared Error', respectively.
+
+Use this benchmark for reference only, as only a small number of random seeds were used.
+
+##### 10% labeled samples 
+
+| Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
+|:---:|:---:|:---:|:---:|
+| XGBoost | 0.7325 | 0.4763 | **5.5739** |
+| DAE | 0.7208 | 0.4885 | 5.6168 | 
+| VIME | 0.7182 | **0.5087** | 5.6637 |
+| SubTab | 0.7312 | 0.4930 | 7.2418 |
+| SCARF | **0.7416** | 0.4710 | 5.8888 | 
+
+--------
+
+##### 100% labeled samples
+
+| Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
+|:---:|:---:|:---:|:---:|
+| XGBoost | 0.7234 | 0.5291 | 4.8377 |
+| DAE | 0.7390 | 0.5500 | 4.5758 |
+| VIME | **0.7688** | 0.5477 | 4.5804 |
+| SubTab | 0.7390 | 0.5432 | 6.3104 |
+| SCARF | 0.7442 | **0.5521** | **4.4443** |
+
+## To DO
 
 - [x] Release nn.Module and Dataset of VIME, SubTab, and SCARF
   - [x] VIME
   - [x] SubTab
   - [x] SCARF
 - [x] Release LightningModules of VIME, SubTab, and SCARF
   - [x] VIME
   - [x] SubTab
   - [x] SCARF
-- [ ] Release Denoising AutoEncoder
-  - [ ] nn.Module
-  - [ ] LightningModule
+- [x] Release Denoising AutoEncoder
+  - [x] nn.Module
+  - [x] LightningModule
 - [ ] Release SwitchTab
   - [ ] nn.Module
   - [ ] LightningModule
-- [ ] Release PTaRL
-  - [ ] Add Backbones
-    - [ ] MLP
-    - [ ] ResNet
-    - [ ] FT-Transformer
-  - [ ] LightningModule
-- [ ] Add example codes
+- [x] Add example codes
 
 ## Contributing
 
 Contributions to this implementation are highly appreciated. Whether it's suggesting improvements, reporting bugs, or proposing new features, feel free to open an issue or submit a pull request.
 
 
 ## Credit  
 ```
 @software{alcoholrithm_2024_10776538,
   author       = {Minwook Kim},
   title        = {TabularS3L},
   month        = mar,
   year         = 2024,
   publisher    = {Zenodo},
-  version      = {v0.20},
+  version      = {v0.21},
   doi          = {10.5281/zenodo.10776538},
   url          = {https://doi.org/10.5281/zenodo.10776538}
 }
 ```
```

### Comparing `ts3l-0.21/README.md` & `ts3l-0.30/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # TabularS3L
 
 [**Overview**](#tabulars3l)
 | [**Installation**](#installation)
 | [**Available Models with Quick Start Guides**](#available-models-with-quick-start)
+| [**Benchmark**](#benchmark)
 | [**To DO**](#to-do)
 | [**Contributing**](#contributing)
 | [**Credit**](#credit)
 
 
 [![pypi](https://img.shields.io/pypi/v/ts3l)](https://pypi.org/project/ts3l/0.20/)
 [![DOI](https://zenodo.org/badge/756740921.svg)](https://zenodo.org/doi/10.5281/zenodo.10776537)
@@ -23,26 +24,121 @@
 
 ## Available Models with Quick Start
 
 TabularS3L employs a two-phase learning approach, where the learning strategies differ between phases. Below is an overview of the models available within TabularS3L, highlighting the learning strategies employed in each phase. The abbreviations 'Self-SL', 'Semi-SL', and 'SL' represent self-supervised learning, semi-supervised learning, and supervised learning, respectively.
 
 | Model | First Phase | Second Phase |
 |:---:|:---:|:---:|
+| **DAE** ([GitHub](https://github.com/ryancheunggit/tabular_dae))| Self-SL | SL |
 | **VIME** ([NeurIPS'20](https://proceedings.neurips.cc/paper/2020/hash/7d97667a3e056acab9aaf653807b4a03-Abstract.html)) | Self-SL | Semi-SL or SL |
 | **SubTab** ([NeurIPS'21](https://proceedings.neurips.cc/paper/2021/hash/9c8661befae6dbcd08304dbf4dcaf0db-Abstract.html)) | Self-SL | SL |
 | **SCARF** ([ICLR'22](https://iclr.cc/virtual/2022/spotlight/6297))| Self-SL | SL |
 
+#### Denoising AutoEncoder (DAE)
+DAE processes input data that has been partially corrupted, producing clean data and predicting which features are corrupted during the self-supervised learning.
+The denoising task enables the model to learn the input distribution and generate latent representations that are robust to corruption. 
+These latent representations can be utilized for a variety of downstream tasks.
+
+<details close>
+  <summary>Quick Start</summary>
+  
+  ```python
+  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
+
+  # Prepare the DAELightning Module
+  from ts3l.pl_modules import DAELightning
+  from ts3l.utils.dae_utils import DAEDataset, DAECollateFN
+  from ts3l.utils import TS3LDataModule
+  from ts3l.utils.dae_utils import DAEConfig
+  from pytorch_lightning import Trainer
+  
+  metric = "accuracy_score"
+  input_dim = X_train.shape[1]
+  hidden_dim = 1024
+  output_dim = 2
+  encoder_depth=4
+  head_depth = 2
+  noise_type = "Swap"
+  noise_ratio = 0.3
+  
+  max_epochs = 20
+  batch_size = 128
+  
+  X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
+  
+  config = DAEConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
+  input_dim=input_dim, hidden_dim=hidden_dim,
+  output_dim=output_dim, encoder_depth=encoder_depth,
+  head_depth = head_depth,
+  noise_type = noise_type,
+  noise_ratio = noise_ratio,
+  num_categoricals=len(category_cols), num_continuous=len(continuous_cols)
+  )
+  
+  pl_dae = DAELightning(config)
+  
+  ### First Phase Learning
+  train_ds = DAEDataset(X = X_train, unlabeled_data = X_unlabeled, continuous_cols = continuous_cols, category_cols = category_cols)
+  valid_ds = DAEDataset(X = X_valid, continuous_cols = continuous_cols, category_cols = category_cols)
+  
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=DAECollateFN(config), valid_collate_fn=DAECollateFN(config))
+  
+  trainer = Trainer(
+                      accelerator = 'cpu',
+                      max_epochs = max_epochs,
+                      num_sanity_val_steps = 2,
+      )
+  
+  trainer.fit(pl_dae, datamodule)
+  
+  ### Second Phase Learning
+  
+  pl_dae.set_second_phase()
+  
+  train_ds = DAEDataset(X = X_train, Y = y_train.values, unlabeled_data=X_unlabeled, continuous_cols=continuous_cols, category_cols=category_cols)
+  valid_ds = DAEDataset(X = X_valid, Y = y_valid.values, continuous_cols=continuous_cols, category_cols=category_cols)
+          
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted")
+  
+  trainer = Trainer(
+                      accelerator = 'cpu',
+                      max_epochs = max_epochs,
+                      num_sanity_val_steps = 2,
+      )
+  
+  trainer.fit(pl_dae, datamodule)
+  
+  # Evaluation
+  from sklearn.metrics import accuracy_score
+  import torch
+  from torch.nn import functional as F
+  from torch.utils.data import DataLoader, SequentialSampler
+  
+  test_ds = DAEDataset(X_test, category_cols=category_cols, continuous_cols=continuous_cols)
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds))
+  
+  preds = trainer.predict(pl_dae, test_dl)
+          
+  preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
+  
+  accuracy = accuracy_score(y_test, preds.argmax(1))
+  
+  print("Accuracy %.2f" % accuracy)
+  ```
+
+</details>
+
 #### VIME: Extending the Success of Self- and Semi-supervised Learning to Tabular Domain
 VIME enhances tabular data learning through a dual approach. In its first phase, it utilize a pretext task of estimating mask vectors from corrupted tabular data, alongside a reconstruction pretext task for self-supervised learning. The second phase leverages consistency regularization on unlabeled data.
 
 <details close>
   <summary>Quick Start</summary>
   
   ```python
-  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, category_cols, and continuous_cols
+  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
 
   # Prepare the VIMELightning Module
   from ts3l.pl_modules import VIMELightning
   from ts3l.utils.vime_utils import VIMEDataset
   from ts3l.utils import TS3LDataModule
   from ts3l.utils.vime_utils import VIMEConfig
   from pytorch_lightning import Trainer
@@ -53,65 +149,60 @@
   output_dim = 2
   alpha1 = 2.0
   alpha2 = 2.0
   beta = 1.0
   K = 3
   p_m = 0.2
 
-  data_hparams = {
-              "K" : K,
-              "p_m" : p_m
-          }
-
   batch_size = 128
 
   X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
 
   config = VIMEConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
   input_dim=input_dim, hidden_dim=hidden_dim,
   output_dim=output_dim, alpha1=alpha1, alpha2=alpha2, 
-  beta=beta, K=K,
+  beta=beta, K=K, p_m = p_m,
   num_categoricals=len(category_cols), num_continuous=len(continuous_cols)
   )
 
   pl_vime = VIMELightning(config)
 
   ### First Phase Learning
-  train_ds = VIMEDataset(X = X_train, unlabeled_data = X_unlabeled, data_hparams=data_hparams, continous_cols = continuous_cols, category_cols = category_cols)
-  valid_ds = VIMEDataset(X = X_valid, data_hparams=data_hparams, continous_cols = continuous_cols, category_cols = category_cols)
+  train_ds = VIMEDataset(X = X_train, unlabeled_data = X_unlabeled, config=config, continuous_cols = continuous_cols, category_cols = category_cols)
+  valid_ds = VIMEDataset(X = X_valid, config=config, continuous_cols = continuous_cols, category_cols = category_cols)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', n_jobs = 4)
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random')
 
   trainer = Trainer(
                       accelerator = 'cpu',
-                      max_epochs = 10,
+                      max_epochs = 20,
                       num_sanity_val_steps = 2,
       )
 
   trainer.fit(pl_vime, datamodule)
 
   ### Second Phase Learning
   from ts3l.utils.vime_utils import VIMESemiSLCollateFN
 
   pl_vime.set_second_phase()
 
-  train_ds = VIMEDataset(X_train, y_train.values, data_hparams, unlabeled_data=X_unlabeled, continous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
-  valid_ds = VIMEDataset(X_valid, y_valid.values, data_hparams, continous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  train_ds = VIMEDataset(X_train, y_train.values, config, unlabeled_data=X_unlabeled, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  valid_ds = VIMEDataset(X_valid, y_valid.values, config, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
           
   datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=VIMESemiSLCollateFN())
 
   trainer.fit(pl_vime, datamodule)
 
   # Evaluation
   from sklearn.metrics import accuracy_score
   import torch
   from torch.nn import functional as F
   from torch.utils.data import DataLoader, SequentialSampler
 
-  test_ds = VIMEDataset(X_test, category_cols=category_cols, continous_cols=continuous_cols, is_second_phase=True)
+  test_ds = VIMEDataset(X_test, category_cols=category_cols, continuous_cols=continuous_cols, is_second_phase=True)
   test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds))
 
   preds = trainer.predict(pl_vime, test_dl)
           
   preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
 
   accuracy = accuracy_score(y_test, preds.argmax(1))
@@ -149,41 +240,32 @@
   n_subsets = 4
   overlap_ratio = 0.75
 
   mask_ratio = 0.1
   noise_type = "Swap"
   noise_level = 0.1
 
-  data_hparams = {
-              "n_subsets" : n_subsets,
-              "overlap_ratio" : overlap_ratio,
-              "mask_ratio" : mask_ratio,
-              "noise_type" : noise_type,
-              "noise_level" : noise_level,
-              "n_column" : input_dim
-          }
-
   batch_size = 128
   max_epochs = 3
 
   X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
 
   config = SubTabConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
   input_dim=input_dim, hidden_dim=hidden_dim,
   output_dim=output_dim, tau=tau, use_cosine_similarity= use_cosine_similarity, use_contrastive=use_contrastive, use_distance=use_distance, 
-  n_subsets=n_subsets, overlap_ratio=overlap_ratio
+  n_subsets=n_subsets, overlap_ratio=overlap_ratio, mask_ratio=mask_ratio, noise_type=noise_type, noise_level=noise_level
   )
 
   pl_subtab = SubTabLightning(config)
 
   ### First Phase Learning
   train_ds = SubTabDataset(X_train, unlabeled_data=X_unlabeled)
   valid_ds = SubTabDataset(X_valid)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams), n_jobs = 4)
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=SubTabCollateFN(config), valid_collate_fn=SubTabCollateFN(config), n_jobs = 4)
 
   trainer = Trainer(
                       accelerator = 'cpu',
                       max_epochs = max_epochs,
                       num_sanity_val_steps = 2,
       )
 
@@ -192,26 +274,26 @@
   ### Second Phase Learning
 
   pl_subtab.set_second_phase()
 
   train_ds = SubTabDataset(X_train, y_train.values)
   valid_ds = SubTabDataset(X_valid, y_valid.values)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams))
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=SubTabCollateFN(config), valid_collate_fn=SubTabCollateFN(config))
 
   trainer.fit(pl_subtab, datamodule)
 
   # Evaluation
   from sklearn.metrics import accuracy_score
   import torch
   from torch.nn import functional as F
   from torch.utils.data import DataLoader, SequentialSampler
 
   test_ds = SubTabDataset(X_test)
-  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4, collate_fn=SubTabCollateFN(data_hparams))
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4, collate_fn=SubTabCollateFN(config))
 
   preds = trainer.predict(pl_subtab, test_dl)
           
   preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
 
   accuracy = accuracy_score(y_test, preds.argmax(1))
 
@@ -225,139 +307,148 @@
 
 <details close>
   <summary>Quick Start</summary>
   
   ```python
   # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
 
-  # Prepare the SubTabLightning Module
-  from ts3l.pl_modules import SubTabLightning
-  from ts3l.utils.subtab_utils import SubTabDataset, SubTabCollateFN
+  # Prepare the SCARFLightning Module
+  from ts3l.pl_modules import SCARFLightning
+  from ts3l.utils.scarf_utils import SCARFDataset
   from ts3l.utils import TS3LDataModule
-  from ts3l.utils.subtab_utils import SubTabConfig
+  from ts3l.utils.scarf_utils import SCARFConfig
   from pytorch_lightning import Trainer
 
   metric = "accuracy_score"
   input_dim = X_train.shape[1]
   hidden_dim = 1024
   output_dim = 2
-  tau = 1.0
-  use_cosine_similarity = True
-  use_contrastive = True
-  use_distance = True
-  n_subsets = 4
-  overlap_ratio = 0.75
+  encoder_depth = 3
+  head_depth = 1
+  dropout_rate = 0.04
 
-  mask_ratio = 0.1
-  noise_type = "Swap"
-  noise_level = 0.1
-
-  data_hparams = {
-              "n_subsets" : n_subsets,
-              "overlap_ratio" : overlap_ratio,
-              "mask_ratio" : mask_ratio,
-              "noise_type" : noise_type,
-              "noise_level" : noise_level,
-              "n_column" : input_dim
-          }
+  corruption_rate = 0.6
 
   batch_size = 128
-  max_epochs = 3
+  max_epochs = 10
 
   X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
 
-  config = SubTabConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
+  config = SCARFConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
   input_dim=input_dim, hidden_dim=hidden_dim,
-  output_dim=output_dim, tau=tau, use_cosine_similarity= use_cosine_similarity, use_contrastive=use_contrastive, use_distance=use_distance, 
-  n_subsets=n_subsets, overlap_ratio=overlap_ratio
+  output_dim=output_dim, encoder_depth=encoder_depth, head_depth=head_depth,
+  dropout_rate=dropout_rate, corruption_rate = corruption_rate
   )
 
-  pl_subtab = SubTabLightning(config)
+  pl_scarf = SCARFLightning(config)
 
   ### First Phase Learning
-  train_ds = SubTabDataset(X_train, unlabeled_data=X_unlabeled)
-  valid_ds = SubTabDataset(X_valid)
+  train_ds = SCARFDataset(X_train, unlabeled_data=X_unlabeled, config = config)
+  valid_ds = SCARFDataset(X_valid, config=config)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams), n_jobs = 4)
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size=batch_size, train_sampler="random")
 
   trainer = Trainer(
                       accelerator = 'cpu',
                       max_epochs = max_epochs,
                       num_sanity_val_steps = 2,
       )
 
-  trainer.fit(pl_subtab, datamodule)
+  trainer.fit(pl_scarf, datamodule)
 
   ### Second Phase Learning
 
-  pl_subtab.set_second_phase()
+  pl_scarf.set_second_phase()
 
-  train_ds = SubTabDataset(X_train, y_train.values)
-  valid_ds = SubTabDataset(X_valid, y_valid.values)
+  train_ds = SCARFDataset(X_train, y_train.values, is_second_phase=True)
+  valid_ds = SCARFDataset(X_valid, y_valid.values, is_second_phase=True)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams))
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted")
 
-  trainer.fit(pl_subtab, datamodule)
+  trainer.fit(pl_scarf, datamodule)
 
   # Evaluation
   from sklearn.metrics import accuracy_score
   import torch
   from torch.nn import functional as F
   from torch.utils.data import DataLoader, SequentialSampler
 
-  test_ds = SubTabDataset(X_test)
-  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4, collate_fn=SubTabCollateFN(data_hparams))
+  test_ds = SCARFDataset(X_test, is_second_phase=True)
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4)
 
-  preds = trainer.predict(pl_subtab, test_dl)
+  preds = trainer.predict(pl_scarf, test_dl)
           
   preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
 
   accuracy = accuracy_score(y_test, preds.argmax(1))
 
   print("Accuracy %.2f" % accuracy)
   ```
 
 </details>
 
-#### To DO
+
+## Benchmark
+
+We provide a simple benchmark using TabularS3L against XGBoost. The train-validation-test ratio is 6:2:2 and we tuned each model over 50 trials using Optuna. The results are the average of the random seeds [0,4]. The best results are bold. 'acc', 'b-acc', and 'mse' mean 'Accuracy', 'Balanced Accuracy', and 'Mean Squared Error', respectively.
+
+Use this benchmark for reference only, as only a small number of random seeds were used.
+
+##### 10% labeled samples 
+
+| Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
+|:---:|:---:|:---:|:---:|
+| XGBoost | 0.7325 | 0.4763 | **5.5739** |
+| DAE | 0.7208 | 0.4885 | 5.6168 | 
+| VIME | 0.7182 | **0.5087** | 5.6637 |
+| SubTab | 0.7312 | 0.4930 | 7.2418 |
+| SCARF | **0.7416** | 0.4710 | 5.8888 | 
+
+--------
+
+##### 100% labeled samples
+
+| Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
+|:---:|:---:|:---:|:---:|
+| XGBoost | 0.7234 | 0.5291 | 4.8377 |
+| DAE | 0.7390 | 0.5500 | 4.5758 |
+| VIME | **0.7688** | 0.5477 | 4.5804 |
+| SubTab | 0.7390 | 0.5432 | 6.3104 |
+| SCARF | 0.7442 | **0.5521** | **4.4443** |
+
+## To DO
 
 - [x] Release nn.Module and Dataset of VIME, SubTab, and SCARF
   - [x] VIME
   - [x] SubTab
   - [x] SCARF
 - [x] Release LightningModules of VIME, SubTab, and SCARF
   - [x] VIME
   - [x] SubTab
   - [x] SCARF
-- [ ] Release Denoising AutoEncoder
-  - [ ] nn.Module
-  - [ ] LightningModule
+- [x] Release Denoising AutoEncoder
+  - [x] nn.Module
+  - [x] LightningModule
 - [ ] Release SwitchTab
   - [ ] nn.Module
   - [ ] LightningModule
-- [ ] Release PTaRL
-  - [ ] Add Backbones
-    - [ ] MLP
-    - [ ] ResNet
-    - [ ] FT-Transformer
-  - [ ] LightningModule
-- [ ] Add example codes
+- [x] Add example codes
 
 ## Contributing
 
 Contributions to this implementation are highly appreciated. Whether it's suggesting improvements, reporting bugs, or proposing new features, feel free to open an issue or submit a pull request.
 
 
 ## Credit  
 ```
 @software{alcoholrithm_2024_10776538,
   author       = {Minwook Kim},
   title        = {TabularS3L},
   month        = mar,
   year         = 2024,
   publisher    = {Zenodo},
-  version      = {v0.20},
+  version      = {v0.21},
   doi          = {10.5281/zenodo.10776538},
   url          = {https://doi.org/10.5281/zenodo.10776538}
 }
 ```
```

### Comparing `ts3l-0.21/setup.py` & `ts3l-0.30/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,34 +13,34 @@
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # requirements
-with pathlib.Path('requirements.txt').open() as requirements_txt:
+with open(path.join(here, 'requirements.txt'), encoding='utf-8') as requirements_txt:
     install_requires = [
         str(requirement)
         for requirement
         in pkg_resources.parse_requirements(requirements_txt)
     ]
 
 setup(
     name='ts3l',
-    version='v0.21',
+    version='v0.30',
     description='A PyTorch Lightning-based library for self- and semi-supervised learning on tabular data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Alcoholrithm/TabularS3L',
     author='Minwook Kim',
     author_email='kmiiiaa@pusan.ac.kr',
 
     # Note that this is a string of words separated by whitespace, not a list.
-    keywords='tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF',
+    keywords='tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF DenoisingAutoEncoder',
     packages=find_packages(),
     # The `include_package_data` parameter in the `setup()` function is used to specify whether to
     # include non-Python files (such as data files, configuration files, etc.) that are part of the
     # package when it is installed.
     include_package_data=False,
     install_requires=install_requires,
     python_requires='>=3.7',
-)
+)
```

### Comparing `ts3l-0.21/ts3l/models/scarf/scarf.py` & `ts3l-0.30/ts3l/models/scarf/scarf.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,31 +2,15 @@
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.distributions.uniform import Uniform
 
 import numpy as np
-
-class MLP(torch.nn.Sequential):
-    """Simple multi-layer perceptron with ReLu activation and optional dropout layer"""
-
-    def __init__(self, input_dim, hidden_dim, n_layers, dropout=0.0):
-        layers = []
-        in_dim = input_dim
-        for _ in range(n_layers - 1):
-            layers.append(torch.nn.Linear(in_dim, hidden_dim))
-            layers.append(nn.BatchNorm1d(hidden_dim)),
-            layers.append(nn.ReLU(inplace=True))
-            layers.append(torch.nn.Dropout(dropout))
-            in_dim = hidden_dim
-
-        layers.append(torch.nn.Linear(in_dim, hidden_dim))
-
-        super().__init__(*layers)
+from ts3l.models.common import MLP
 
 
 class SCARF(nn.Module):
     def __init__(
         self,
         # sampling_candidate: NDArray[np.float_],
         input_dim,
```

### Comparing `ts3l-0.21/ts3l/models/subtab/subtab.py` & `ts3l-0.30/ts3l/models/subtab/subtab.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 from numpy.typing import NDArray
 
 import itertools
 
 from types import SimpleNamespace
-from typing import Dict, Any, Tuple, List
+from typing import Dict, Any, Tuple, List, Union
 
 class ShallowEncoder(nn.Module):
     def __init__(self,
                  feat_dim : int,
                  hidden_dim : int,
                  n_subsets : int,
                  overlap_ratio : float,
@@ -64,15 +64,15 @@
     
     def encode(self, x : torch.Tensor) -> torch.Tensor:
         return self.encoder(x)
     
     def decode(self, x : torch.Tensor) -> torch.Tensor:
         return self.decoder(x)
     
-    def forward(self, x : torch.Tensor) -> torch.Tensor:
+    def forward(self, x : torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         latent = self.encode(x)
         projection = self.projection_net(latent)
         projection = F.normalize(projection, p = 2, dim = 1)
         x_recon = self.decode(latent)
         return latent, projection, x_recon
 
 class SubTab(nn.Module):
@@ -102,30 +102,29 @@
 
     def set_first_phase(self) -> None:
         self.forward = self.__first_phase_step
     
     def set_second_phase(self) -> None:
         self.forward = self.__second_phase_step
 
-    def __first_phase_step(self, x : torch.Tensor) -> torch.Tensor:
+    def __first_phase_step(self, x : torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
 
         latents, projections, x_recons = self.ae(x)
         
         return projections, x_recons, x
     
-    def __arange_subsets(self, latent: torch.FloatTensor) -> torch.FloatTensor:
+    def __arange_subsets(self, latent: torch.Tensor) -> torch.Tensor:
         no, dim = latent.shape
         samples = int(no / self.n_subsets)
-        
         latent = latent.reshape((self.n_subsets, samples, dim))
         return torch.concat([latent[:, i] for i in range(samples)])
     
     def __second_phase_step(self, 
                   x : torch.Tensor,
-                  return_embeddings : bool = False) -> torch.Tensor:
+                  return_embeddings : bool = False) -> Union[Tuple[torch.Tensor, torch.Tensor], torch.Tensor]:
 
         latent = self.ae.encode(x)
         latent = self.__arange_subsets(latent)
         
         latent = latent.reshape(x.shape[0] // self.n_subsets, self.n_subsets, -1).mean(1)
         out = self.head(latent)
```

### Comparing `ts3l-0.21/ts3l/models/vime/vime.py` & `ts3l-0.30/ts3l/models/vime/vime.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.21/ts3l/models/vime/vime_self.py` & `ts3l-0.30/ts3l/models/vime/vime_self.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.21/ts3l/models/vime/vime_semi.py` & `ts3l-0.30/ts3l/models/vime/vime_semi.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.21/ts3l/pl_modules/base_module.py` & `ts3l-0.30/ts3l/pl_modules/base_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,66 +1,65 @@
-from typing import Dict, Any, Type
+from typing import Dict, Any, List
 from ts3l.utils import RegressionMetric, ClassificationMetric
 
 from abc import ABC, abstractmethod
 
 import torch
 from torch import nn
 
 import pytorch_lightning as pl
 
 from dataclasses import asdict
 from ts3l.utils import BaseConfig
-from typing import Type
     
 
     
 class TS3LLightining(ABC, pl.LightningModule):
     """The pytorch lightning module of TabularS3L
     """
-    def __init__(self, config: Type[BaseConfig]) -> None:
+    def __init__(self, config: BaseConfig) -> None:
         """Initialize the pytorch lightining module of TabularS3L
 
         Args:
-            config (Type[BaseConfig]): The configuration of TS3LLightining.
+            config (BaseConfig): The configuration of TS3LLightining.
         """
         super(TS3LLightining, self).__init__()
         
-        config = asdict(config)
+        _config = asdict(config)
         
-        self.random_seed = config["random_seed"]
-        del config["random_seed"]
+        self.random_seed = _config["random_seed"]
+        del _config["random_seed"]
         
         pl.seed_everything(self.random_seed)
         
-        self.optim = getattr(torch.optim, config["optim"])
-        del config["optim"]
-        self.optim_hparams = config["optim_hparams"]
-        del config["optim_hparams"]
-        
-        self.sched = getattr(torch.optim.lr_scheduler, config["scheduler"]) if config["scheduler"] is not None else None
-        del config["scheduler"]
-        self.scheduler_hparams = config["scheduler_hparams"]
-        del config["scheduler_hparams"]
-        
-        self.loss_fn = getattr(torch.nn, config["loss_fn"])(**config["loss_hparams"])
-        del config["loss_fn"]
-        del config["loss_hparams"]
-        
-        self.__configure_metric(config["task"], config["metric"], config["metric_hparams"])
-        del config["task"]
-        del config["metric"]
-        del config["metric_hparams"]
+        self.optim = getattr(torch.optim, _config["optim"])
+        del _config["optim"]
+        self.optim_hparams = _config["optim_hparams"]
+        del _config["optim_hparams"]
+        
+        self.sched = getattr(torch.optim.lr_scheduler, _config["scheduler"]) if _config["scheduler"] is not None else None
+        del _config["scheduler"]
+        self.scheduler_hparams = _config["scheduler_hparams"]
+        del _config["scheduler_hparams"]
+        
+        self.loss_fn = getattr(torch.nn, _config["loss_fn"])(**_config["loss_hparams"])
+        del _config["loss_fn"]
+        del _config["loss_hparams"]
+        
+        self.__configure_metric(_config["task"], _config["metric"], _config["metric_hparams"])
+        del _config["task"]
+        del _config["metric"]
+        del _config["metric_hparams"]
         
-        self._initialize(config)
+        self._initialize(_config)
         
         self.set_first_phase()
 
-        self.first_phase_step_outputs = []
-        self.second_phase_step_outputs = []
+        self.first_phase_step_outputs: List[Dict[str, Any]] = []
+        self.second_phase_step_outputs: List[Dict[str, Any]] = []
         
         self.save_hyperparameters()
     
     @abstractmethod
     def _initialize(self, config: Dict[str, Any]) -> None:
         pass
     
@@ -80,27 +79,27 @@
         self.scheduler = self.sched(self.optimizer, **self.scheduler_hparams)
         return [self.optimizer], [{'scheduler': self.scheduler, 'interval': 'step'} ]
 
     def set_first_phase(self) -> None:
         """Set the module to pretraining
         """
         self.model.set_first_phase()
-        self.training_step = self._first_phase_step
-        self.on_validation_start = self._on_first_phase_validation_start
-        self.validation_step = self._first_phase_step
-        self.on_validation_epoch_end = self._first_phase_validation_epoch_end
+        self.training_step = self._first_phase_step # type: ignore
+        self.on_validation_start = self._on_first_phase_validation_start # type: ignore
+        self.validation_step = self._first_phase_step # type: ignore
+        self.on_validation_epoch_end = self._first_phase_validation_epoch_end # type: ignore
 
     def set_second_phase(self) -> None:
         """Set the module to finetunning
         """
         self.model.set_second_phase()
-        self.training_step = self._second_phase_step
-        self.on_validation_start = self._on_second_phase_validation_start
-        self.validation_step = self._second_phase_step
-        self.on_validation_epoch_end = self._second_phase_validation_epoch_end
+        self.training_step = self._second_phase_step # type: ignore
+        self.on_validation_start = self._on_second_phase_validation_start # type: ignore
+        self.validation_step = self._second_phase_step # type: ignore
+        self.on_validation_epoch_end = self._second_phase_validation_epoch_end # type: ignore
 
     def forward(self,
                 batch:Dict[str, Any]
     ) -> torch.FloatTensor:
         """Do forward pass for given input
 
         Args:
@@ -109,19 +108,19 @@
         Returns:
             torch.FloatTensor: The output of forward pass
         """
         return self.model(batch)
     
 
     @abstractmethod
-    def _get_first_phase_loss(self, batch:Dict[str, Any]):
+    def _get_first_phase_loss(self, batch: Any) -> torch.FloatTensor:
         """Calculate the first phase loss
 
         Args:
-            batch (Dict[str, Any]): The input batch
+            batch (Any): The input batch
 
         Returns:
             torch.FloatTensor: The final loss of first phase step
         """
         pass
     
     def _first_phase_step(self,
@@ -208,16 +207,16 @@
         }
     
     def _on_second_phase_validation_start(self):
         """Log the training loss and the performance of the second phase
         """
         if len(self.second_phase_step_outputs) > 0:
             train_loss = torch.Tensor([out["loss"] for out in self.second_phase_step_outputs]).detach().mean()
-            y = torch.cat([out["y"] for out in self.second_phase_step_outputs]).detach()
-            y_hat = torch.cat([out["y_hat"] for out in self.second_phase_step_outputs]).detach()
+            y = torch.cat([out["y"] for out in self.second_phase_step_outputs if out["y"].numel() != 1]).detach().cpu()
+            y_hat = torch.cat([out["y_hat"] for out in self.second_phase_step_outputs if out["y_hat"].numel() != 1]).detach().cpu()
             
             train_score = self.metric(y_hat, y)
             
             self.log("train_loss", train_loss, prog_bar = True)
             self.log("train_" + self.metric.__name__, train_score, prog_bar = True)
             self.second_phase_step_outputs = []   
             
@@ -225,16 +224,16 @@
     
     def _second_phase_validation_epoch_end(self) -> None:
         """Log the validation loss and the performance of the second phase
         """
         val_loss = torch.Tensor([out["loss"] for out in self.second_phase_step_outputs]).mean()
 
         
-        y = torch.cat([out["y"] for out in self.second_phase_step_outputs])
-        y_hat = torch.cat([out["y_hat"] for out in self.second_phase_step_outputs])
+        y = torch.cat([out["y"].cpu() for out in self.second_phase_step_outputs if out["y"].numel() != 1])
+        y_hat = torch.cat([out["y_hat"].cpu() for out in self.second_phase_step_outputs if out["y_hat"].numel() != 1])
         val_score = self.metric(y_hat, y)
 
         self.log("val_" + self.metric.__name__, val_score, prog_bar = True)
         self.log("val_loss", val_loss, prog_bar = True)
         self.second_phase_step_outputs = []      
         return super().on_validation_epoch_end()
```

### Comparing `ts3l-0.21/ts3l/pl_modules/scarf_lightning.py` & `ts3l-0.30/ts3l/pl_modules/scarf_lightning.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.21/ts3l/pl_modules/subtab_lightning.py` & `ts3l-0.30/ts3l/pl_modules/subtab_lightning.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,54 +39,54 @@
         del config["use_cosine_similarity"]
         del config["shuffle"]
         del config["mask_ratio"]
         del config["noise_type"]
         del config["noise_level"]
         self.model = SubTab(**config)
     
-    def __get_recon_label(self, label: torch.FloatTensor) -> torch.FloatTensor:
+    def __get_recon_label(self, label: torch.Tensor) -> torch.Tensor:
         """Duplicates the input label tensor across the batch dimension to match the number of subsets for reconstruction loss.
 
         Args:
-            label (torch.FloatTensor): The input tensor representing the label to be duplicated.
+            label (torch.Tensor): The input tensor representing the label to be duplicated.
 
         Returns:
-            torch.FloatTensor: A tensor with the input `label` duplicated `self.n_subsets` times along the batch dimension.
+            torch.Tensor: A tensor with the input `label` duplicated `self.n_subsets` times along the batch dimension.
         """
         recon_label = label
         for _ in range(1, self.n_subsets):
             recon_label = torch.concat((recon_label, label), dim = 0)
         return recon_label
     
-    def __arange_subsets(self, projections: torch.FloatTensor) -> torch.FloatTensor:
+    def __arange_subsets(self, projections: torch.Tensor) -> torch.Tensor:
         """
         Rearranges the projections tensor into a sequence of subsets for first phase loss.
         This method takes a tensor of projections and reshapes it into a format where each subset of projections is concatenated along the first dimension. 
         The original tensor, which is assumed to represent a series of projections, is first reshaped into a tensor of shape `(n_subsets, samples, dim)` 
         where `n_subsets` is the number of subsets, `samples` is the batch_size, and `dim` is the embedding dimension. 
         The method then concatenates these subsets along the zeroth dimension to produce a sequence of projections suitable for first phase loss.
 
         Args:
-            projections (torch.FloatTensor): A tensor of shape `(no, dim)` where `no` is the total number of observations and `dim` is the embedding dimension. 
+            projections (torch.Tensor): A tensor of shape `(no, dim)` where `no` is the total number of observations and `dim` is the embedding dimension. 
 
         Returns:
-            torch.FloatTensor: A reshaped tensor where subsets of projections are concatenated along the first dimension. 
+            torch.Tensor: A reshaped tensor where subsets of projections are concatenated along the first dimension. 
                                 The resulting shape is `(no, dim)`, maintaining the original dimensionality but rearranging the order of observations to align with subset divisions.
         """
         no, dim = projections.shape
         samples = int(no / self.n_subsets)
         
         projections = projections.reshape((self.n_subsets, samples, dim))
         return torch.concat([projections[:, i] for i in range(samples)])
 
-    def _get_first_phase_loss(self, batch:Tuple[torch.FloatTensor, Union[torch.FloatTensor, torch.LongTensor]]):
+    def _get_first_phase_loss(self, batch:Tuple[torch.FloatTensor, torch.Tensor, torch.Tensor]) -> torch.FloatTensor:
         """Calculate the first phase loss
 
         Args:
-            batch (Tuple[torch.FloatTensor, Union[torch.FloatTensor, torch.LongTensor]]): The input batch
+            batch (Tuple[torch.FloatTensor, torch.Tensor, torch.Tensor]): The input batch
 
         Returns:
             torch.FloatTensor: The final loss of first phase step
         """
         x, y_recons, y = batch
         projections, x_recons, x = self.model(x)
```

### Comparing `ts3l-0.21/ts3l/pl_modules/vime_lightning.py` & `ts3l-0.30/ts3l/pl_modules/vime_lightning.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,21 +93,20 @@
         if len(unlabeled) > 0:
             u_y_hat = self.model(unlabeled)
             target = u_y_hat[::self.consistency_len]
             target = target.repeat(1, self.K).reshape((-1, u_y_hat.shape[-1]))
             preds = torch.stack([u_y_hat[i, :] for i in range(len(u_y_hat)) if i % self.consistency_len != 0], dim = 0)
             unsupervised_loss += self.consistency_loss(preds, target)
         
-        labeled_x = x[y != self.u_label].squeeze()
+        labeled_x = x[y != self.u_label]
         labeled_y = y[y != self.u_label]
 
         y_hat = self.model(labeled_x).squeeze()
 
         supervised_loss = self.loss_fn(y_hat, labeled_y)
-        
         loss = supervised_loss + self.beta * unsupervised_loss
         
         return loss, labeled_y, y_hat
     
     def predict_step(self, batch, batch_idx: int
         ) -> torch.FloatTensor:
             """The predict step of VIME
```

### Comparing `ts3l-0.21/ts3l/utils/base_config.py` & `ts3l-0.30/ts3l/utils/base_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,84 +1,88 @@
 from dataclasses import dataclass, field
 
-from typing import Dict, Any
+from typing import Dict, Any, Optional
 from torch import optim, nn
 import torchmetrics
 import sklearn
 
 @dataclass
 class BaseConfig:
     """ Configuration class for initializing components of the TabularS3L Lightning Module, including optimizers, 
     learning rate schedulers, and loss functions, along with their respective hyperparameters.
 
     Attributes:
         task (str): Specify whether the problem is regression or classification.
+        input_dim (int): The dimension of the input.
+        output_dim (int): The dimension of output.
+        loss_fn (str): Name of the loss function to be used. Must be an attribute of 'torch.nn'.
         optim (str): Name of the optimizer to be used. Must be an attribute of 'torch.optim'. Default is 'AdamW'.
         optim_hparams (Dict[str, Any]): Hyperparameters for the optimizer. Default is {'lr': 0.0001, 'weight_decay': 0.00005}.
         scheduler (str): Name of the learning rate scheduler to be used. Must be an attribute of 'torch.optim.lr_scheduler' or None. Default is None.
         scheduler_hparams (Dict[str, Any]): Hyperparameters for the scheduler. Default is None, indicating no scheduler is used.
-        loss_fn (str): Name of the loss function to be used. Must be an attribute of 'torch.nn'.
         loss_hparams (Dict[str, Any]): Hyperparameters for the loss function. Default is empty dictionary.
         metric (str): Name of the metric to be used. Must be an attribute of 'torchmetrics.functional' or 'sklearn.metrics'. Default is None.
         metric_hparams (Dict[str, Any]): Hyperparameters for the metric. Default is an empty dictionary.
         random_seed (int): Seed for random number generators to ensure reproducibility. Defaults to 42.
 
     Raises:
         ValueError: If the specified 'optim' is not a valid optimizer in 'torch.optim'.
         ValueError: If the specified 'scheduler' is not None and is not a valid scheduler in 'torch.optim.lr_scheduler'.
-        
-        ValueError: If the 'loss_fn' attribute is None, indicating that a loss function must be specified.
+
         ValueError: If the specified 'loss_fn' is not None and is not a valid loss function in 'torch.nn'.
         
-        ValueError: If the 'metric' attribute is None, indicating that a metric must be specified.
         ValueError: If the specified 'metric' is not a valid metric in 'torchmetrics' or 'sklearn.metrics'.
         
-        ValueError: If the 'task' attribute is None, indicating that a task must be specified.
         ValueError: If the specified 'task' is not a valid task in ['regression', 'classification']'.
         
     """
-    task: str = field(default=None)
+    task: str
+    
+    input_dim: int
+    
+    output_dim: int
+    
+    loss_fn: str
+    
+    loss_hparams: Dict[str, Any] = field(default_factory=dict)
+    
+    metric: Optional[str] = field(default=None)
+    
+    metric_hparams: Dict[str, Any] = field(default_factory=dict)
     
     optim: str = field(default="AdamW")
     
     optim_hparams: Dict[str, Any] = field(
                                             default_factory=lambda: {
                                                     "lr" : 0.0001,
                                                     "weight_decay" : 0.00005
                                             }
                                         )
     
-    scheduler: str = field(default=None)
-    
-    scheduler_hparams: Dict[str, Any] = field(default = None)
-    
-    loss_fn: str = field(default=None)
-    
-    loss_hparams: Dict[str, Any] = field(default_factory=dict)
-    
-    metric: str = field(default=None)
+    scheduler: Optional[str] = field(default=None)
     
-    metric_hparams: Dict[str, Any] = field(default_factory=dict)
+    scheduler_hparams: Optional[Dict[str, Any]] = field(default = None)
     
     random_seed: int = field(default=42)
     
     def __post_init__(self):
-        if self.task is None:
-            raise ValueError("The task of the problem must be specified in the 'task' attribute.")
-        elif (type(self.task) is not str or (self.task != "regression" and self.task != "classification")):
+
+        if (type(self.task) is not str or (self.task != "regression" and self.task != "classification")):
             raise ValueError(f"{self.task} is not a valid task. Choices are: ['regression', 'classification']")
         
         if type(self.optim) is not str or not hasattr(optim, self.optim):
             raise ValueError(f"{self.optim} is not a valid optimizer in torch.optim")
         
         if self.scheduler is not None and (type(self.scheduler) is not str or not hasattr(optim.lr_scheduler, self.scheduler)):
             raise ValueError(f"{self.scheduler} is not a valid scheduler in torch.optim.lr_scheduler")
-        
-        if self.loss_fn is None:
-            raise ValueError("A loss function must be specified in the 'loss_fn' attribute.")
-        elif type(self.loss_fn) is not str or not hasattr(nn, self.loss_fn):
+
+        if type(self.loss_fn) is not str or not hasattr(nn, self.loss_fn):
             raise ValueError(f"{self.loss_fn} is not a valid loss function in torch.nn")
         
         if self.metric is None:
-            raise ValueError("A metric must be specified in the 'metric' attribute.")
+            if self.task == "regression":
+                self.metric = "mean_squared_error"
+            else:
+                self.metric = "accuracy_score"
+                
         elif (type(self.metric) is not str or (not hasattr(torchmetrics.functional, self.metric) and not hasattr(sklearn.metrics, self.metric))):
             raise ValueError(f"{self.metric} is not a valid metric in torchmetrics.functional or sklearn.metrics")
```

### Comparing `ts3l-0.21/ts3l/utils/datamodule.py` & `ts3l-0.30/ts3l/utils/datamodule.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from torch.utils.data import Dataset, DataLoader, SequentialSampler, WeightedRandomSampler, RandomSampler
 
 from pytorch_lightning import LightningDataModule
 
 class TS3LDataModule(LightningDataModule):
     """The pytorch lightning datamodule for TabularS3L
     """
-    def __init__(self, train_ds:Dataset, val_ds:Dataset, batch_size: int, train_sampler: str, train_collate_fn = None, valid_collate_fn = None, n_jobs: int = 32, drop_last: int = False, is_regression:bool = False):
+    def __init__(self, train_ds:Dataset, val_ds:Dataset, batch_size: int, train_sampler: str, train_collate_fn = None, valid_collate_fn = None, n_jobs: int = 32, drop_last: bool = False, is_regression:bool = False):
         """Initialize the datamodule
 
         Args:
             train_ds (Dataset): The training dataset.
             val_ds (Dataset): The validation dataset.
             batch_size (int): The batch size of the dataset.
             train_sampler (str): The training sampler for training dataset. It must be one of ["seq", "weighted", "random"].
@@ -41,31 +41,37 @@
         
         Use a weighted random sampler for the second phase step of the classification task, otherwise use a random sampler.
         
         Args:
             stage (str): Only for compatibility, not used
         """
         if self.train_sampler == "seq":
-            sampler = SequentialSampler(self.train_ds)
+            sampler = SequentialSampler(self.train_ds) # type: ignore
             shuffle = True
         elif self.train_sampler == "weighted":
-            sampler = WeightedRandomSampler(self.train_ds.weights, num_samples = len(self.train_ds))
+            sampler = WeightedRandomSampler(self.train_ds.weights, num_samples = len(self.train_ds)) # type: ignore
             shuffle = False
         elif self.train_sampler == "random":
-            sampler = RandomSampler(self.train_ds, num_samples = len(self.train_ds))
+            sampler = RandomSampler(self.train_ds, num_samples = len(self.train_ds)) # type: ignore
             shuffle = False
 
         self.train_dl = DataLoader(self.train_ds, 
                                     batch_size = self.batch_size, 
                                     shuffle=shuffle, 
                                     sampler = sampler,
                                     num_workers=self.n_jobs,
                                     drop_last=self.drop_last,
                                     collate_fn = self.train_collate_fn)
-        self.val_dl = DataLoader(self.val_ds, batch_size = self.batch_size, shuffle=False, sampler = SequentialSampler(self.val_ds), num_workers=self.n_jobs, drop_last=False, collate_fn=self.valid_collate_fn)
+        self.val_dl = DataLoader(self.val_ds, 
+                                batch_size = self.batch_size, 
+                                shuffle=False, 
+                                sampler = SequentialSampler(self.val_ds), # type: ignore
+                                num_workers=self.n_jobs, 
+                                drop_last=False, 
+                                collate_fn=self.valid_collate_fn)
     
     def train_dataloader(self):
         """Return the training dataloader.
         """
         return self.train_dl
 
     def val_dataloader(self):
```

### Comparing `ts3l-0.21/ts3l/utils/misc.py` & `ts3l-0.30/ts3l/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.21/ts3l/utils/scarf_utils/data_utils.py` & `ts3l-0.30/ts3l/utils/scarf_utils/data_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import Union, Tuple, Dict, Any
+from typing import Union, Tuple, Dict, Any, Optional
 from numpy.typing import NDArray
 
 from torch.utils.data import Dataset
 
 import numpy as np
 import pandas as pd
 import torch
 from torch.utils.data import Dataset
 
 from dataclasses import asdict
 from ts3l.utils.scarf_utils import SCARFConfig
 
 class SCARFDataset(Dataset):
     def __init__(self, X: pd.DataFrame, 
-                        Y: Union[NDArray[np.int_], NDArray[np.float_]] = None,
-                        unlabeled_data: pd.DataFrame = None, 
-                        config: SCARFConfig = None,
-                        is_regression: bool = False,
-                        is_second_phase: bool = False,
+                        Y: Optional[Union[NDArray[np.int_], NDArray[np.float_]]] = None,
+                        unlabeled_data: Optional[pd.DataFrame] = None, 
+                        config: Optional[SCARFConfig] = None,
+                        is_regression: Optional[bool] = False,
+                        is_second_phase: Optional[bool] = False,
                         ) -> None:
         """A dataset class for SCARF that handles labeled and unlabeled data.
 
         This class is designed to manage data for the SCARF, accommodating both labeled and unlabeled datasets
         for self-supervised learning scenarios. It supports regression and classification tasks.
 
         Args:
@@ -34,31 +34,31 @@
             is_regression (bool, optional): Flag indicating whether the task is regression (True) or classification (False).
                 Defaults to False.
             is_second_phase (bool, optional): Flag indicating whether the dataset is for first phase or second phase learning. 
                 Default is False.
         """
         
         if config is not None:
-            self.config = asdict(config)
+            self.config = config
             
         if unlabeled_data is not None:
             X = pd.concat([X, unlabeled_data])
             
         self.data = torch.FloatTensor(X.values)
         
-        self.corruption_rate = self.config["corruption_rate"] if not is_second_phase else 0.0
+        self.corruption_rate = self.config.corruption_rate if not is_second_phase else 0.0
         self.corruption_len = int(X.shape[1] * self.corruption_rate)
+        if not is_second_phase:
+            self.corruption_len = max(1, self.corruption_len)
+            
         self.n_sampling_candidate , self.n_features = X.shape
 
         self.is_regression = is_regression
         
-        if is_regression:
-            self.label_class = torch.FloatTensor
-        else:
-            self.label_class = torch.LongTensor
+        self.label_class = torch.FloatTensor if is_regression else torch.LongTensor
             
         if Y is None:
             self.label = None
         else:
             self.label = self.label_class(Y)
             
             if self.label_class == torch.LongTensor:
@@ -87,16 +87,16 @@
             if self.corruption_len:
                 corruption_mask = torch.zeros((self.n_features), dtype=torch.bool)
                 corruption_idx = torch.randperm(self.n_features)[:self.corruption_len]
 
                 corruption_mask[corruption_idx] = True
                 
                 x_random = torch.randint(0, self.n_sampling_candidate, corruption_mask.shape)
-                x_corrupted = torch.FloatTensor([self.data[:, i][x_random[i]] for i in range(self.n_features)])
-                x_corrupted = torch.where(corruption_mask, x_corrupted, self.data[idx])
+                _x_corrupted = torch.FloatTensor([self.data[:, i][x_random[i]] for i in range(self.n_features)])
+                x_corrupted = torch.where(corruption_mask, _x_corrupted, self.data[idx])
                 return self.data[idx], x_corrupted
             return self.data[idx]
         else:
             return self.data[idx], self.label[idx]
 
     def __len__(self):
         """Returns the total number of items in the dataset.
```

### Comparing `ts3l-0.21/ts3l/utils/scarf_utils/loss.py` & `ts3l-0.30/ts3l/utils/scarf_utils/loss.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.21/ts3l/utils/scarf_utils/scarf_config.py` & `ts3l-0.30/ts3l/utils/scarf_utils/scarf_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,59 +6,48 @@
 @dataclass
 class SCARFConfig(BaseConfig):
     """ Configuration class for initializing components of the SCARFLightning Module, including hyperparameters of SCARF,
     optimizers, learning rate schedulers, and loss functions, along with their respective hyperparameters.
 
     Inherits Attributes:
         task (str): Specify whether the problem is regression or classification.
+        input_dim (int): The dimension of the input.
+        output_dim (int): The dimension of output.
+        loss_fn (str): Name of the loss function to be used. Must be an attribute of 'torch.nn'.
         optim (str): Name of the optimizer to be used. Must be an attribute of 'torch.optim'. Default is 'AdamW'.
         optim_hparams (Dict[str, Any]): Hyperparameters for the optimizer. Default is {'lr': 0.0001, 'weight_decay': 0.00005}.
         scheduler (str): Name of the learning rate scheduler to be used. Must be an attribute of 'torch.optim.lr_scheduler' or None. Default is None.
         scheduler_hparams (Dict[str, Any]): Hyperparameters for the scheduler. Default is None, indicating no scheduler is used.
-        loss_fn (str): Name of the loss function to be used. Must be an attribute of 'torch.nn'.
         loss_hparams (Dict[str, Any]): Hyperparameters for the loss function. Default is empty dictionary.
         metric (str): Name of the metric to be used. Must be an attribute of 'torchmetrics.functional' or 'sklearn.metrics'. Default is None.
         metric_hparams (Dict[str, Any]): Hyperparameters for the metric. Default is an empty dictionary.
         random_seed (int): Seed for random number generators to ensure reproducibility. Defaults to 42.
         
     New Attributes:
-        input_dim (int): The dimension of the input.
         hidden_dim (int): The dimension of hidden layer. Default is 256.
-        output_dim (int): The dimension of output.
         encoder_depth (bool):  The depth of encoder. Default is 4.
         head_depth (bool): The depth of head. Default is 2.
         dropout_rate (bool): A hyperparameter that is to control dropout layer. Default is 0.04.
         tau (float): A hyperparameter that is to scale similarity between views during the first phase.
         corruption_rate (float): The proportion of features to be corrupted, simulating noisy conditions for robustness. 
                 For the second phase dataset, it should be 0. Defaults to 0.0.
 
     Raises:
         ValueError: Inherited from 'BaseConfig' to indicate that a configuration for the task, optimizer, scheduler, loss function, or metric is either invalid or not specified.
         
-        ValueError: Raised if 'input_dim' or 'output_dim' are not specified, indicating these dimensions must be defined.                    
     """
     
-    input_dim: int = field(default=None)
-    
     hidden_dim: int = field(default=256)
     
-    output_dim: int = field(default=None)
-    
     encoder_depth: int = field(default=4)
     
     head_depth: int = field(default=2)
     
     dropout_rate: float = field(default=0.04)
     
     tau: float = field(default=0.1)
     
     corruption_rate: float = field(default=0)
     
     
     def __post_init__(self):
-        super().__post_init__()
-        
-        if self.input_dim is None:
-            raise ValueError("The dimension of input must be specified in the 'input_dim' attribute.")
-        
-        if self.output_dim is None:
-            raise ValueError("The dimension of output must be specified in the 'output_dim' attribute.")
+        super().__post_init__()
```

### Comparing `ts3l-0.21/ts3l/utils/subtab_utils/data_utils.py` & `ts3l-0.30/ts3l/utils/subtab_utils/data_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,110 @@
-from typing import Dict, Any, Tuple, Union
+from typing import Dict, Any, Tuple, Union, Optional
 from numpy.typing import NDArray
 
 import torch
 from torch.utils.data import Dataset
 import numpy as np
 import pandas as pd
 
 from dataclasses import asdict
 from ts3l.utils.subtab_utils import SubTabConfig
 class SubTabDataset(Dataset):
     def __init__(self, X: pd.DataFrame, 
-                        Y: Union[NDArray[np.int_], NDArray[np.float_]] = None,
-                        unlabeled_data: pd.DataFrame = None, 
-                        is_regression: bool = False
+                        Y: Optional[Union[NDArray[np.int_], NDArray[np.float_]]] = None,
+                        unlabeled_data: Optional[pd.DataFrame] = None, 
+                        is_regression: Optional[bool] = False
                         ) -> None:
         """A dataset class for SubTab that handles labeled and unlabeled data.
 
         This class is designed to manage data for the SubTab, accommodating both labeled and unlabeled datasets
         for self-supervised learning scenarios. It supports regression and classification tasks.
 
         Args:
             X (pd.DataFrame): DataFrame containing the features of the labeled data.
-            Y (Union[NDArray[np.int_], NDArray[np.float_]], optional): Numpy array containing the labels for the data. 
+            Y (Optional[Union[NDArray[np.int_], NDArray[np.float_]]]): Numpy array containing the labels for the data. 
                 Use integers for classification labels and floats for regression targets. Defaults to None.
-            unlabeled_data (pd.DataFrame): DataFrame containing the features of the unlabeled data, used for 
+            unlabeled_data (Optional[pd.DataFrame]): DataFrame containing the features of the unlabeled data, used for 
                 self-supervised learning. Defaults to None.
-            is_regression (bool, optional): Flag indicating whether the task is regression (True) or classification (False).
+            is_regression (Optional[bool]): Flag indicating whether the task is regression (True) or classification (False).
                 Defaults to False.
         """
         if unlabeled_data is not None:
             X = pd.concat([X, unlabeled_data])
             
         self.data = torch.FloatTensor(X.values)
         
-        if is_regression:
-            self.label_class = torch.FloatTensor
-        else:
-            self.label_class = torch.LongTensor
+        self.label_class = torch.FloatTensor if is_regression else torch.LongTensor
             
         if Y is None:
             self.label = None
         else:
             self.label = self.label_class(Y)
             
             if not is_regression:
                 class_counts = [sum((self.label == i)) for i in set(self.label.numpy())]
                 num_samples = len(self.label)
 
                 class_weights = [num_samples/class_counts[i] for i in range(len(class_counts))]
                 self.weights = [class_weights[self.label[i]] for i in range(int(num_samples))]
     
-    def __getitem__(self, idx: int) -> Tuple[torch.FloatTensor, Union[torch.FloatTensor, torch.LongTensor]]:
+    def __getitem__(self, idx: int) -> Tuple[torch.Tensor, torch.Tensor]:
         """Retrieves the feature and label tensors for a given index.
 
         Args:
             idx (int): The index of the data point to retrieve.
 
         Returns:
-            Tuple[torch.FloatTensor, Union[torch.FloatTensor, torch.LongTensor]]: The feature tensor and the label 
+            Tuple[torch.Tensor, torch.Tensor]: The feature tensor and the label 
             tensor (if available) for the given index. If labels are not provided, a placeholder is returned.
         """
         if self.label is None:
-            return self.data[idx], [0]
+            return self.data[idx], torch.LongTensor([0])
         return self.data[idx], self.label[idx]
     
     def __len__(self) -> int:
         """Returns the total number of items in the dataset.
 
         Returns:
             int: The size of the dataset.
         """
         return len(self.data)
     
 class SubTabCollateFN(object):
-    def __init__(self, config: SubTabConfig = None) -> None:
+    def __init__(self, config: SubTabConfig) -> None:
         """A collate function for SubTab to generate subsets of features for dataloaders.
 
         This collate function is designed to prepare batches for the SubTab model by generating subsets of features with
         optional noise and masking. It supports configurable shuffling, overlap, and masking of features.
 
         Args:
-            config (Dict[str, Any]): The given hyperparameter set for SubTab.
+            config (SubTabConfig): The given hyperparameter set for SubTab.
         """
         
-        if config is not None:
-            self.config = asdict(config)
+        self.config = config
             
-        self.shuffle = self.config["shuffle"]
+        self.shuffle = self.config.shuffle
         
-        self.n_subsets = self.config["n_subsets"]
-        self.overlap_ratio = self.config["overlap_ratio"]
-        self.mask_ratio = self.config["mask_ratio"]
-        self.noise_type = self.config["noise_type"]
-        self.noise_level = self.config["noise_level"]
+        self.n_subsets = self.config.n_subsets
+        self.overlap_ratio = self.config.overlap_ratio
+        self.mask_ratio = self.config.mask_ratio
+        self.noise_type = self.config.noise_type
+        self.noise_level = self.config.noise_level
         
-        self.input_dim = self.config["input_dim"]
+        self.input_dim = self.config.input_dim
         self.n_column_subset = int(self.input_dim / self.n_subsets)
         # Number of overlapping features between subsets
         self.n_overlap = int(self.overlap_ratio * self.n_column_subset)
         self.column_idx = np.array(range(self.input_dim))
     
-    def __generate_noisy_xbar(self, x : torch.FloatTensor) -> torch.Tensor:
+    def __generate_noisy_xbar(self, x : torch.Tensor) -> torch.Tensor:
         """Generates a noisy version of the input sample `x`.
 
         Args:
-            x (torch.FloatTensor): The original sample.
+            x (torch.Tensor): The original sample.
 
         Returns:
             torch.Tensor: The noisy sample.
         """
         no, dim = x.shape
         
         # Initialize corruption array
@@ -118,68 +114,68 @@
         if self.noise_type == "Swap":
             x_bar = torch.stack([x[np.random.permutation(no), i] for i in range(dim)], dim=1).to(x.device)
         elif self.noise_type == "Gaussian":
             x_bar = x + torch.normal(torch.zeros(x.shape), torch.full(x.shape, self.noise_level)).to(x.device)
 
         return x_bar
     
-    def __generate_x_tilde(self, x: torch.FloatTensor, subset_column_idx: NDArray[np.int32]) -> torch.FloatTensor:
+    def __generate_x_tilde(self, x: torch.Tensor, subset_column_idx: NDArray[np.int32]) -> torch.Tensor:
         """Generates a masked and potentially noisy subset of the input sample `x` based on the provided column indices.
 
         Args:
-            x (torch.FloatTensor): The original sample.
+            x (torch.Tensor): The original sample.
             subset_column_idx (NDArray[np.int32]): Indices of columns to include in the subset.
 
         Returns:
-            torch.FloatTensor: The processed subset of the sample.
+            torch.Tensor: The processed subset of the sample.
         """
         x_bar = x[:, subset_column_idx]
         x_bar_noisy = self.__generate_noisy_xbar(x_bar)
         
         mask = torch.distributions.binomial.Binomial(total_count = 1, probs = self.mask_ratio).sample(x_bar.shape).to(x_bar.device)
         
         x_bar = x_bar * (1 - mask) + x_bar_noisy * mask
         
         return x_bar
     
     def __generate_subset(self,
                         x : torch.Tensor,
-    ) -> torch.FloatTensor:
+    ) -> torch.Tensor:
         """Generates subsets of features from the input sample `x`, applying shuffling, noise, and masking as configured.
 
         Args:
             x (torch.Tensor): The batch of samples.
 
         Returns:
-            torch.FloatTensor: A tensor containing the generated subsets for the batch.
+            torch.Tensor: A tensor containing the generated subsets for the batch.
         """
 
-        permuted_order = np.random.permutation(self.n_subsets) if self.shuffle else range(self.n_subsets)
+        permuted_order = np.random.permutation(self.n_subsets) if self.shuffle else np.arange(self.n_subsets)
 
-        subset_column_indice = [self.column_idx[:self.n_column_subset + self.n_overlap]]
-        subset_column_indice.extend([self.column_idx[range(i * self.n_column_subset - self.n_overlap, (i + 1) * self.n_column_subset)] for i in range(self.n_subsets)])
+        subset_column_indice_list = [self.column_idx[:self.n_column_subset + self.n_overlap]]
+        subset_column_indice_list.extend([self.column_idx[range(i * self.n_column_subset - self.n_overlap, (i + 1) * self.n_column_subset)] for i in range(self.n_subsets)])
         
         
-        subset_column_indice = np.array(subset_column_indice)
+        subset_column_indice = np.array(subset_column_indice_list)
         subset_column_indice = subset_column_indice[permuted_order]
         
         if len(subset_column_indice) == 1:
             subset_column_indice = np.concatenate([subset_column_indice, subset_column_indice])
         
         x_tildes = torch.concat([self.__generate_x_tilde(x, subset_column_indice[i]) for i in range(self.n_subsets)]) # [subset1, subset2, ... ,  subsetN]
 
         return x_tildes
     
-    def __call__(self, batch):
+    def __call__(self, batch: Tuple[torch.Tensor, torch.Tensor]) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """Processes a batch of samples, and generating feature subsets.
 
         Args:
-            batch: A batch of samples.
+            batch (Tuple[torch.Tensor, torch.Tensor]): A batch of samples.
 
         Returns:
-            A tuple containing the processed feature subsets, the original samples, and the labels.
+            Tuple[torch.Tensor, torch.Tensor, torch.Tensor]: A tuple containing the processed feature subsets, the original samples, and the labels.
         """
         y_recons = torch.stack([sample[0] for sample in batch])
         x = self.__generate_subset(y_recons)
         y = torch.tensor([sample[1] for sample in batch])
         
         return x, y_recons, y
```

### Comparing `ts3l-0.21/ts3l/utils/subtab_utils/loss.py` & `ts3l-0.30/ts3l/utils/subtab_utils/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         # Loss calculation for the anchor
         pos_sum = torch.sum(torch.exp(positives))
         neg_sum = torch.sum(torch.exp(negatives))
         # return -torch.log(pos_sum / (pos_sum + neg_sum))
         anchor_loss = -torch.log(pos_sum / (pos_sum + neg_sum))
         return anchor_loss
         
-    def XNegloss(self, projections: torch.FloatTensor) -> torch.FloatTensor:
+    def XNegloss(self, projections: torch.FloatTensor) -> torch.Tensor:
         
         
         # Compute cosine similarity using the provided function
         similarity = self.similarity_fn(projections, projections) / self.temperature
         
         # return torch.stack([self.get_anchor_loss(turn, similarity[turn]) for turn in range(len(similarity))]).mean()
         anchor_losses = [self.get_anchor_loss(turn, similarity[turn]) for turn in range(len(similarity))]
```

### Comparing `ts3l-0.21/ts3l/utils/subtab_utils/subtab_config.py` & `ts3l-0.30/ts3l/utils/subtab_utils/subtab_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass, field
 from ts3l.utils import BaseConfig
 
-from typing import Any, List
+from typing import Any, List, Optional
 
 @dataclass
 class SubTabConfig(BaseConfig):
     """ Configuration class for initializing components of the SubTabLightning Module, including hyperparameters of SubTab,
     optimizers, learning rate schedulers, and loss functions, along with their respective hyperparameters.
 
     Inherits Attributes:
@@ -17,41 +17,35 @@
         loss_fn (str): Name of the loss function to be used. Must be an attribute of `torch.nn`.
         loss_hparams (Dict[str, Any]): Hyperparameters for the loss function. Default is empty dictionary.
         metric (str): Name of the metric to be used. Must be an attribute of `torchmetrics.functional` or 'sklearn.metrics'. Default is None.
         metric_hparams (Dict[str, Any]): Hyperparameters for the metric. Default is an empty dictionary.
         random_seed (int): Seed for random number generators to ensure reproducibility. Defaults to 42.
         
     New Attributes:
-        input_dim (int): The dimension of the input.
         hidden_dim (int): The dimension of hidden layer. Default is 256.
-        output_dim (int): The dimension of output.
         tau (float): A hyperparameter that is to scale similarity between projections during the first phase.
         use_cosine_similarity (bool):  A hyperparameter that is to select whether using cosine similarity or dot similarity when calculating similarity
                                         between projections during the first phase. Default is False.
         use_contrastive (bool): A hyperparameter that is to select using contrastive loss or not during the first phase. Default is True.
         use_distance (bool): A hyperparameter that is to select using distance loss or not during the first phase. Default is True.
         n_subsets (int): The number of subsets to generate different views of the data. Default is 4.
         overlap_ratio (float): A hyperparameter that is to control the extent of overlapping between the subsets. Default is 0.75.
         shuffle (bool): Whether to shuffle the subsets. 
         mask_ratio (float): Ratio of features to be masked as noise.
         noise_type (str): The type of noise to apply.
         noise_level (float): Intensity of Gaussian noise to be applied.
 
     Raises:
         ValueError: Inherited from `BaseConfig` to indicate that a configuration for the task, optimizer, scheduler, loss function, or metric is either invalid or not specified.
-        
-        ValueError: Raised if `input_dim` or `output_dim` are not specified, indicating these dimensions must be defined.                    
+        ValueError: If the specified 'noise_type' is not in ["Swap", "Gaussian", "Zero_Out"].
+        ValueError: If the specified 'noise_level' is not a valid value.
     """
     
-    input_dim: int = field(default=None)
-    
     hidden_dim: int = field(default=256)
     
-    output_dim: int = field(default=None)
-    
     tau: float = field(default=0.1)
     
     use_cosine_similarity: bool = field(default=False)
     
     use_contrastive: bool = field(default=True)
     
     use_distance: bool = field(default=True)
@@ -62,23 +56,17 @@
     
     shuffle: bool = field(default=False)
     
     mask_ratio: float = field(default=0.2)
     
     noise_type: str = field(default="Swap")
     
-    noise_level: float = field(default=None)
+    noise_level: float = field(default=0)
     
     def __post_init__(self):
         super().__post_init__()
         
-        if self.input_dim is None:
-            raise ValueError("The dimension of input must be specified in the 'input_dim' attribute.")
-        
-        if self.output_dim is None:
-            raise ValueError("The dimension of output must be specified in the 'output_dim' attribute.")
-        
         if self.noise_type not in ["Swap", "Gaussian", "Zero_Out"]:
             raise ValueError('The noise type must be one of ["Swap", "Gaussian", "Zero_Out"], but %s.' % self.noise_type)
         
-        if (self.noise_type == "Gaussian") and (self.noise_level == None) or (self.noise_level < 0):
-            raise ValueError("The noise level must be a float that is >= 0 when the noise type is Gaussian.")
+        if (self.noise_type == "Gaussian") and (self.noise_level <= 0):
+            raise ValueError("The noise level must be a float that is > 0 when the noise type is Gaussian.")
```

### Comparing `ts3l-0.21/ts3l/utils/vime_utils/data_utils.py` & `ts3l-0.30/ts3l/utils/vime_utils/data_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 import pandas as pd
-from typing import Dict, Any, List, Union
+from typing import Dict, Any, List, Union, Optional, Tuple
 from numpy.typing import NDArray
 
 import torch
 from torch.utils.data import Dataset
 
 import numpy as np
 from dataclasses import asdict
 from ts3l.utils.vime_utils import VIMEConfig
 
 class VIMEDataset(Dataset):
     def __init__(self,
                 X: pd.DataFrame,
-                Y: Union[NDArray[np.int_], NDArray[np.float_]] = None, 
-                config: VIMEConfig = None, 
-                unlabeled_data: pd.DataFrame = None, 
-                continous_cols: List = None, 
-                category_cols: List = None, 
-                u_label = -1, 
-                is_second_phase: bool = False,
-                is_regression: bool = False, 
+                Y: Optional[Union[NDArray[np.int_], NDArray[np.float_]]] = None, 
+                config: Optional[VIMEConfig] = None, 
+                unlabeled_data: Optional[pd.DataFrame] = None, 
+                continuous_cols: Optional[List] = None, 
+                category_cols: Optional[List] = None, 
+                u_label: Any = -1, 
+                is_second_phase: Optional[bool] = False,
+                is_regression: Optional[bool] = False, 
         ) -> None:
         """A dataset class for VIME that handles labeled and unlabeled data.
 
         This class is designed to manage data for the VIME, accommodating both labeled and unlabeled datasets
         for self- and semi-supervised learning scenarios. It supports regression and classification tasks.
 
         Args:
             X (pd.DataFrame): DataFrame containing the features of the labeled data.
             Y (Union[NDArray[np.int_], NDArray[np.float_]], optional): Numpy array containing the labels for the data. 
                 Use integers for classification labels and floats for regression targets. Defaults to None.
             config (Dict[str, Any]): The given hyperparameter set for VIME.
             unlabeled_data (pd.DataFrame): DataFrame containing the features of the unlabeled data, used for 
                 self-supervised learning. Defaults to None.
-            continous_cols (List, optional): List of continuous columns. Defaults to None.
+            continuous_cols (List, optional): List of continuous columns. Defaults to None.
             category_cols (List, optional): List of categorical columns. Defaults to None.
             u_label (int, optional): The specifier for unlabeled sample. Defaults to -1.
             is_second_phase (bool): The flag that determines whether the dataset is for first phase or second phase learning. Default is False.
             is_regression (bool, optional): Flag indicating whether the task is regression (True) or classification (False).
                 Defaults to False.
         """
         
         self.label = None
         
         if not is_second_phase:
             self.__getitem = self.__first_phase_get_item
             
         else:
             self.__getitem = self.__second_phase_get_item
-            if is_regression:
-                self.label_class = torch.FloatTensor
-            else:
-                self.label_class = torch.LongTensor
+            
+            self.label_class = torch.FloatTensor if is_regression else torch.LongTensor
             
             if Y is not None:
             
                 self.label = self.label_class(Y)
             
                 if unlabeled_data is not None:
                     self.label = torch.concat((self.label, self.label_class([u_label for _ in range(len(unlabeled_data))])), dim=0)
@@ -71,37 +69,37 @@
                     if unlabeled_data is not None:
                         unlabeled_weight = len(X) / len(unlabeled_data)
                         self.weights.extend([unlabeled_weight for _ in range(len(unlabeled_data))])
         
         if unlabeled_data is not None:
             X = pd.concat([X, unlabeled_data])
             
-        self.cont_data = torch.FloatTensor(X[continous_cols].values)
+        self.cont_data = torch.FloatTensor(X[continuous_cols].values)
         self.cat_data = torch.FloatTensor(X[category_cols].values)
         
-        self.continuous_cols = continous_cols
+        self.continuous_cols = continuous_cols
         self.category_cols = category_cols
 
         if config is not None:
-            self.config = asdict(config)
+            self.config = config
         
         self.u_label = u_label
     
-    def __getitem__(self, idx: int) -> Dict[str, torch.tensor]:
+    def __getitem__(self, idx: int) -> Dict[str, Union[torch.Tensor, Tuple[torch.Tensor, ...]]]:
         """Retrieves the feature and label tensors for a given index. The structure of the label 
             varies depending on the learning phase: 
 
             - In the first phase, the label is a tuple containing a mask and the original feature tensor.
             - In the second phase, the label is either a token indicating unlabeled samples or the actual label for labeled samples.
 
         Args:
             idx (int): The index of the data point to retrieve.
 
         Returns:
-            Dict[Any, torch.tensor]: The feature tensor and the label for the given index. 
+            Dict[Any, torch.Tensor]: The feature tensor and the label for the given index. 
             For first phase learning, label is a tuple of mask and original feature tensor.
             For second phase learning, label is a one of a token for unlabeled samples or a label of it.
         """
         return self.__getitem(idx)
     
     def __mask_generator(self, p_m, x):
         """Generate mask vector.
@@ -113,15 +111,15 @@
         Returns:
             - mask: binary mask matrix 
         """
         mask = np.random.binomial(1, p_m, x.shape)
 
         return np.expand_dims(mask, axis=0)
 
-    def __pretext_generator(self, m, x, empirical_dist):  
+    def __pretext_generator(self, m, x, empirical_dist) -> Tuple[torch.LongTensor, torch.FloatTensor]:  
         """Generate corrupted samples.
         
         Args:
             m: mask matrix
             x: feature matrix
             
         Returns:
@@ -144,80 +142,79 @@
         m_new = 1 * (x != x_tilde)
         
         if dim != 1:
             return m_new.squeeze(), x_tilde.squeeze()
         else:
             return m_new.squeeze().reshape(1), x_tilde.squeeze().reshape(1)
     
-    def __generate_x_tildes(self, cat_samples: torch.FloatTensor, cont_samples:torch.FloatTensor) -> torch.FloatTensor:
+    def __generate_x_tildes(self, cat_samples: torch.Tensor, cont_samples:torch.Tensor) -> torch.Tensor:
         """Generate x_tilde for consistency regularization
 
         Args:
-            cat_samples (torch.FloatTensor): The categorical features to generate x_tilde
-            cont_samples (torch.FloatTensor): The continuous features to generate x_tilde
+            cat_samples (torch.Tensor): The categorical features to generate x_tilde
+            cont_samples (torch.Tensor): The continuous features to generate x_tilde
 
         Returns:
-            torch.FloatTensor: x_tilde for consistency regularization
+            torch.Tensor: x_tilde for consistency regularization
         """
-        m_unlab = self.__mask_generator(self.config["p_m"], cat_samples)
+        m_unlab = self.__mask_generator(self.config.p_m, cat_samples)
         dcat_m_label, cat_x_tilde = self.__pretext_generator(m_unlab, cat_samples, self.cat_data)
         
-        m_unlab = self.__mask_generator(self.config["p_m"], cont_samples)
+        m_unlab = self.__mask_generator(self.config.p_m, cont_samples)
         cont_m_label, cont_x_tilde = self.__pretext_generator(m_unlab, cont_samples, self.cont_data)
         x_tilde = torch.concat((cat_x_tilde, cont_x_tilde)).float()
         
         return x_tilde
     
-    def __first_phase_get_item(self, idx: int) -> Dict[str, torch.tensor]:
+    def __first_phase_get_item(self, idx: int) -> Dict[str, Union[torch.Tensor, Tuple[torch.Tensor, ...]]]:
         """Return a input and label pair
 
         Args:
             idx (int): The index of the data to sample
 
         Returns:
-            Dict[str, Any]: A pair of input and label for first phase learning
+            Dict[str, Union[torch.Tensor, Tuple[torch.Tensor, ...]]]: A pair of input and label for first phase learning
         """
         cat_samples = self.cat_data[idx]
-        m_unlab = self.__mask_generator(self.config["p_m"], cat_samples)
+        m_unlab = self.__mask_generator(self.config.p_m, cat_samples)
         cat_m_label, cat_x_tilde = self.__pretext_generator(m_unlab, cat_samples, self.cat_data)
 
         cont_samples = self.cont_data[idx]
-        m_unlab = self.__mask_generator(self.config["p_m"], cont_samples)
+        m_unlab = self.__mask_generator(self.config.p_m, cont_samples)
         cont_m_label, cont_x_tilde = self.__pretext_generator(m_unlab, cont_samples, self.cont_data)
 
         m_label = torch.concat((cat_m_label, cont_m_label)).float()
         x_tilde = torch.concat((cat_x_tilde, cont_x_tilde)).float()
 
         x = torch.concat((cat_samples, cont_samples))
 
         return {
                 "input" : x_tilde,
                 "label" : (m_label, x)
                 }
 
-    def __second_phase_get_item(self, idx) -> Dict[str, torch.tensor]:
+    def __second_phase_get_item(self, idx) -> Dict[str, Union[torch.Tensor, Tuple[torch.Tensor, ...]]]:
         """Return a input and label pair
 
         Args:
             idx (int): The index of the data to sample
 
         Returns:
-            Dict[str, Any]: A pair of input and label for second phase learning
+            Dict[str, Union[torch.Tensor, Tuple[torch.Tensor, ...]]]: A pair of input and label for second phase learning
         """
         cat_samples = self.cat_data[idx]
         cont_samples = self.cont_data[idx]
         x = torch.concat((cat_samples, cont_samples)).squeeze()
         if self.label is not None:
             
             if self.label[idx] == self.u_label:
-                xs = [x]
+                _xs = [x]
+                _xs.extend([self.__generate_x_tildes(cat_samples, cont_samples) for _ in range(self.config.K)])
+                xs = torch.stack(_xs)
                 
-                xs.extend([self.__generate_x_tildes(cat_samples, cont_samples) for _ in range(self.config["K"])])
-
-                xs = torch.stack(xs)
                 return {
                     "input" : xs,
                     "label" : self.label_class([self.u_label for _ in range(len(xs))])
                 }
             else:
                 return {
                     "input" : x.unsqueeze(0),
```

### Comparing `ts3l-0.21/ts3l/utils/vime_utils/vime_config.py` & `ts3l-0.30/ts3l/utils/vime_utils/vime_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from dataclasses import dataclass, field
 from ts3l.utils import BaseConfig
 
-from typing import Any, List
+from typing import Any, List, Optional
 
 @dataclass
 class VIMEConfig(BaseConfig):
     """ Configuration class for initializing components of the VIMELightning Module, including hyperparameters of VIME,
     optimizers, learning rate schedulers, and loss functions, along with their respective hyperparameters.
 
     Inherits Attributes:
         task (str): Specify whether the problem is regression or classification.
-        optim (str): Name of the optimizer to be used. Must be an attribute of `torch.optim`. Default is 'AdamW'.
+        input_dim (int): The dimension of the input.
+        output_dim (int): The dimension of output.
+        loss_fn (str): Name of the loss function to be used. Must be an attribute of 'torch.nn'.
+        optim (str): Name of the optimizer to be used. Must be an attribute of 'torch.optim'. Default is 'AdamW'.
         optim_hparams (Dict[str, Any]): Hyperparameters for the optimizer. Default is {'lr': 0.0001, 'weight_decay': 0.00005}.
-        scheduler (str): Name of the learning rate scheduler to be used. Must be an attribute of `torch.optim.lr_scheduler` or None. Default is None.
+        scheduler (str): Name of the learning rate scheduler to be used. Must be an attribute of 'torch.optim.lr_scheduler' or None. Default is None.
         scheduler_hparams (Dict[str, Any]): Hyperparameters for the scheduler. Default is None, indicating no scheduler is used.
-        loss_fn (str): Name of the loss function to be used. Must be an attribute of `torch.nn`.
         loss_hparams (Dict[str, Any]): Hyperparameters for the loss function. Default is empty dictionary.
-        metric (str): Name of the metric to be used. Must be an attribute of `torchmetrics.functional` or 'sklearn.metrics'. Default is None.
+        metric (str): Name of the metric to be used. Must be an attribute of 'torchmetrics.functional' or 'sklearn.metrics'. Default is None.
         metric_hparams (Dict[str, Any]): Hyperparameters for the metric. Default is an empty dictionary.
         random_seed (int): Seed for random number generators to ensure reproducibility. Defaults to 42.
         
     New Attributes:
-        input_dim (int): The dimension of the input.
         hidden_dim (int): The hidden dimension of predictor. Default is 256.
-        output_dim (int): The output dimension of predictor.
         num_categoricals int: The number of categorical features.
         num_continuous int: The number of continuous features.
         u_label (Any): The special token for unlabeled samples.
         alpha1 (float): A hyperparameter that is to control the trade-off between 
                         the mask estimation and categorical feature estimation loss during first phase. 
                         Default is 2.0.
         alpha2 (float): A hyperparameter that is to control the trade-off between 
@@ -37,28 +37,23 @@
                         the supervised and unsupervised loss during second phase. 
                         Default is 1.0.
         K (int): The number of augmented samples for consistency regularization. Default is 3.
         p_m (float): A hyperparameter that is to control the masking ratio during the first phase learning. Default is 0.3.
 
     Raises:
         ValueError: Inherited from `BaseConfig` to indicate that a configuration for the task, optimizer, scheduler, loss function, or metric is either invalid or not specified.
-
         ValueError: Raised if both `num_categoricals` and `num_continuous` are None, indicating that at least one attribute must be specified.
-        ValueError: Raised if `input_dim` or `output_dim` are not specified, indicating these dimensions must be defined.                    
+        
     """
     
-    input_dim: int = field(default=None)
-    
     hidden_dim: int = field(default=256)
     
-    output_dim: int = field(default=None)
-    
-    num_categoricals: int = field(default=None)
+    num_categoricals: Optional[int] = field(default=None)
     
-    num_continuous: int = field(default=None)
+    num_continuous: Optional[int] = field(default=None)
     
     u_label: Any = field(default=-1)
     
     alpha1: float = field(default=2.0)
     
     alpha2: float = field(default=2.0)
     
@@ -67,18 +62,12 @@
     K: int = field(default=3)
     
     p_m: float = field(default=0.3)
     
     def __post_init__(self):
         super().__post_init__()
         
-        if self.input_dim is None:
-            raise ValueError("The dimension of input must be specified in the 'input_dim' attribute.")
-        
-        if self.output_dim is None:
-            raise ValueError("The dimension of predictor's output must be specified in the 'output_dim' attribute.")
-        
         if self.num_categoricals is None and self.num_continuous is None:
             raise ValueError("At least one attribute (num_categorical or num_continuous) must be specified.")
         else:
             self.num_categoricals = self.num_categoricals if self.num_categoricals is not None else 0
             self.num_continuous = self.num_continuous if self.num_continuous is not None else 0
```

### Comparing `ts3l-0.21/ts3l.egg-info/PKG-INFO` & `ts3l-0.30/ts3l.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ts3l
-Version: 0.21
+Version: 0.30
 Summary: A PyTorch Lightning-based library for self- and semi-supervised learning on tabular data.
 Home-page: https://github.com/Alcoholrithm/TabularS3L
 Author: Minwook Kim
 Author-email: kmiiiaa@pusan.ac.kr
-Keywords: tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF
+Keywords: tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF DenoisingAutoEncoder
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: torch
@@ -17,14 +17,15 @@
 Requires-Dist: torchmetrics
 
 # TabularS3L
 
 [**Overview**](#tabulars3l)
 | [**Installation**](#installation)
 | [**Available Models with Quick Start Guides**](#available-models-with-quick-start)
+| [**Benchmark**](#benchmark)
 | [**To DO**](#to-do)
 | [**Contributing**](#contributing)
 | [**Credit**](#credit)
 
 
 [![pypi](https://img.shields.io/pypi/v/ts3l)](https://pypi.org/project/ts3l/0.20/)
 [![DOI](https://zenodo.org/badge/756740921.svg)](https://zenodo.org/doi/10.5281/zenodo.10776537)
@@ -41,26 +42,121 @@
 
 ## Available Models with Quick Start
 
 TabularS3L employs a two-phase learning approach, where the learning strategies differ between phases. Below is an overview of the models available within TabularS3L, highlighting the learning strategies employed in each phase. The abbreviations 'Self-SL', 'Semi-SL', and 'SL' represent self-supervised learning, semi-supervised learning, and supervised learning, respectively.
 
 | Model | First Phase | Second Phase |
 |:---:|:---:|:---:|
+| **DAE** ([GitHub](https://github.com/ryancheunggit/tabular_dae))| Self-SL | SL |
 | **VIME** ([NeurIPS'20](https://proceedings.neurips.cc/paper/2020/hash/7d97667a3e056acab9aaf653807b4a03-Abstract.html)) | Self-SL | Semi-SL or SL |
 | **SubTab** ([NeurIPS'21](https://proceedings.neurips.cc/paper/2021/hash/9c8661befae6dbcd08304dbf4dcaf0db-Abstract.html)) | Self-SL | SL |
 | **SCARF** ([ICLR'22](https://iclr.cc/virtual/2022/spotlight/6297))| Self-SL | SL |
 
+#### Denoising AutoEncoder (DAE)
+DAE processes input data that has been partially corrupted, producing clean data and predicting which features are corrupted during the self-supervised learning.
+The denoising task enables the model to learn the input distribution and generate latent representations that are robust to corruption. 
+These latent representations can be utilized for a variety of downstream tasks.
+
+<details close>
+  <summary>Quick Start</summary>
+  
+  ```python
+  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
+
+  # Prepare the DAELightning Module
+  from ts3l.pl_modules import DAELightning
+  from ts3l.utils.dae_utils import DAEDataset, DAECollateFN
+  from ts3l.utils import TS3LDataModule
+  from ts3l.utils.dae_utils import DAEConfig
+  from pytorch_lightning import Trainer
+  
+  metric = "accuracy_score"
+  input_dim = X_train.shape[1]
+  hidden_dim = 1024
+  output_dim = 2
+  encoder_depth=4
+  head_depth = 2
+  noise_type = "Swap"
+  noise_ratio = 0.3
+  
+  max_epochs = 20
+  batch_size = 128
+  
+  X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
+  
+  config = DAEConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
+  input_dim=input_dim, hidden_dim=hidden_dim,
+  output_dim=output_dim, encoder_depth=encoder_depth,
+  head_depth = head_depth,
+  noise_type = noise_type,
+  noise_ratio = noise_ratio,
+  num_categoricals=len(category_cols), num_continuous=len(continuous_cols)
+  )
+  
+  pl_dae = DAELightning(config)
+  
+  ### First Phase Learning
+  train_ds = DAEDataset(X = X_train, unlabeled_data = X_unlabeled, continuous_cols = continuous_cols, category_cols = category_cols)
+  valid_ds = DAEDataset(X = X_valid, continuous_cols = continuous_cols, category_cols = category_cols)
+  
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=DAECollateFN(config), valid_collate_fn=DAECollateFN(config))
+  
+  trainer = Trainer(
+                      accelerator = 'cpu',
+                      max_epochs = max_epochs,
+                      num_sanity_val_steps = 2,
+      )
+  
+  trainer.fit(pl_dae, datamodule)
+  
+  ### Second Phase Learning
+  
+  pl_dae.set_second_phase()
+  
+  train_ds = DAEDataset(X = X_train, Y = y_train.values, unlabeled_data=X_unlabeled, continuous_cols=continuous_cols, category_cols=category_cols)
+  valid_ds = DAEDataset(X = X_valid, Y = y_valid.values, continuous_cols=continuous_cols, category_cols=category_cols)
+          
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted")
+  
+  trainer = Trainer(
+                      accelerator = 'cpu',
+                      max_epochs = max_epochs,
+                      num_sanity_val_steps = 2,
+      )
+  
+  trainer.fit(pl_dae, datamodule)
+  
+  # Evaluation
+  from sklearn.metrics import accuracy_score
+  import torch
+  from torch.nn import functional as F
+  from torch.utils.data import DataLoader, SequentialSampler
+  
+  test_ds = DAEDataset(X_test, category_cols=category_cols, continuous_cols=continuous_cols)
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds))
+  
+  preds = trainer.predict(pl_dae, test_dl)
+          
+  preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
+  
+  accuracy = accuracy_score(y_test, preds.argmax(1))
+  
+  print("Accuracy %.2f" % accuracy)
+  ```
+
+</details>
+
 #### VIME: Extending the Success of Self- and Semi-supervised Learning to Tabular Domain
 VIME enhances tabular data learning through a dual approach. In its first phase, it utilize a pretext task of estimating mask vectors from corrupted tabular data, alongside a reconstruction pretext task for self-supervised learning. The second phase leverages consistency regularization on unlabeled data.
 
 <details close>
   <summary>Quick Start</summary>
   
   ```python
-  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, category_cols, and continuous_cols
+  # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
 
   # Prepare the VIMELightning Module
   from ts3l.pl_modules import VIMELightning
   from ts3l.utils.vime_utils import VIMEDataset
   from ts3l.utils import TS3LDataModule
   from ts3l.utils.vime_utils import VIMEConfig
   from pytorch_lightning import Trainer
@@ -71,65 +167,60 @@
   output_dim = 2
   alpha1 = 2.0
   alpha2 = 2.0
   beta = 1.0
   K = 3
   p_m = 0.2
 
-  data_hparams = {
-              "K" : K,
-              "p_m" : p_m
-          }
-
   batch_size = 128
 
   X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
 
   config = VIMEConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
   input_dim=input_dim, hidden_dim=hidden_dim,
   output_dim=output_dim, alpha1=alpha1, alpha2=alpha2, 
-  beta=beta, K=K,
+  beta=beta, K=K, p_m = p_m,
   num_categoricals=len(category_cols), num_continuous=len(continuous_cols)
   )
 
   pl_vime = VIMELightning(config)
 
   ### First Phase Learning
-  train_ds = VIMEDataset(X = X_train, unlabeled_data = X_unlabeled, data_hparams=data_hparams, continous_cols = continuous_cols, category_cols = category_cols)
-  valid_ds = VIMEDataset(X = X_valid, data_hparams=data_hparams, continous_cols = continuous_cols, category_cols = category_cols)
+  train_ds = VIMEDataset(X = X_train, unlabeled_data = X_unlabeled, config=config, continuous_cols = continuous_cols, category_cols = category_cols)
+  valid_ds = VIMEDataset(X = X_valid, config=config, continuous_cols = continuous_cols, category_cols = category_cols)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', n_jobs = 4)
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random')
 
   trainer = Trainer(
                       accelerator = 'cpu',
-                      max_epochs = 10,
+                      max_epochs = 20,
                       num_sanity_val_steps = 2,
       )
 
   trainer.fit(pl_vime, datamodule)
 
   ### Second Phase Learning
   from ts3l.utils.vime_utils import VIMESemiSLCollateFN
 
   pl_vime.set_second_phase()
 
-  train_ds = VIMEDataset(X_train, y_train.values, data_hparams, unlabeled_data=X_unlabeled, continous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
-  valid_ds = VIMEDataset(X_valid, y_valid.values, data_hparams, continous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  train_ds = VIMEDataset(X_train, y_train.values, config, unlabeled_data=X_unlabeled, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
+  valid_ds = VIMEDataset(X_valid, y_valid.values, config, continuous_cols=continuous_cols, category_cols=category_cols, is_second_phase=True)
           
   datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=VIMESemiSLCollateFN())
 
   trainer.fit(pl_vime, datamodule)
 
   # Evaluation
   from sklearn.metrics import accuracy_score
   import torch
   from torch.nn import functional as F
   from torch.utils.data import DataLoader, SequentialSampler
 
-  test_ds = VIMEDataset(X_test, category_cols=category_cols, continous_cols=continuous_cols, is_second_phase=True)
+  test_ds = VIMEDataset(X_test, category_cols=category_cols, continuous_cols=continuous_cols, is_second_phase=True)
   test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds))
 
   preds = trainer.predict(pl_vime, test_dl)
           
   preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
 
   accuracy = accuracy_score(y_test, preds.argmax(1))
@@ -167,41 +258,32 @@
   n_subsets = 4
   overlap_ratio = 0.75
 
   mask_ratio = 0.1
   noise_type = "Swap"
   noise_level = 0.1
 
-  data_hparams = {
-              "n_subsets" : n_subsets,
-              "overlap_ratio" : overlap_ratio,
-              "mask_ratio" : mask_ratio,
-              "noise_type" : noise_type,
-              "noise_level" : noise_level,
-              "n_column" : input_dim
-          }
-
   batch_size = 128
   max_epochs = 3
 
   X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
 
   config = SubTabConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
   input_dim=input_dim, hidden_dim=hidden_dim,
   output_dim=output_dim, tau=tau, use_cosine_similarity= use_cosine_similarity, use_contrastive=use_contrastive, use_distance=use_distance, 
-  n_subsets=n_subsets, overlap_ratio=overlap_ratio
+  n_subsets=n_subsets, overlap_ratio=overlap_ratio, mask_ratio=mask_ratio, noise_type=noise_type, noise_level=noise_level
   )
 
   pl_subtab = SubTabLightning(config)
 
   ### First Phase Learning
   train_ds = SubTabDataset(X_train, unlabeled_data=X_unlabeled)
   valid_ds = SubTabDataset(X_valid)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams), n_jobs = 4)
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=SubTabCollateFN(config), valid_collate_fn=SubTabCollateFN(config), n_jobs = 4)
 
   trainer = Trainer(
                       accelerator = 'cpu',
                       max_epochs = max_epochs,
                       num_sanity_val_steps = 2,
       )
 
@@ -210,26 +292,26 @@
   ### Second Phase Learning
 
   pl_subtab.set_second_phase()
 
   train_ds = SubTabDataset(X_train, y_train.values)
   valid_ds = SubTabDataset(X_valid, y_valid.values)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams))
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=SubTabCollateFN(config), valid_collate_fn=SubTabCollateFN(config))
 
   trainer.fit(pl_subtab, datamodule)
 
   # Evaluation
   from sklearn.metrics import accuracy_score
   import torch
   from torch.nn import functional as F
   from torch.utils.data import DataLoader, SequentialSampler
 
   test_ds = SubTabDataset(X_test)
-  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4, collate_fn=SubTabCollateFN(data_hparams))
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4, collate_fn=SubTabCollateFN(config))
 
   preds = trainer.predict(pl_subtab, test_dl)
           
   preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
 
   accuracy = accuracy_score(y_test, preds.argmax(1))
 
@@ -243,139 +325,148 @@
 
 <details close>
   <summary>Quick Start</summary>
   
   ```python
   # Assume that we have X_train, X_valid, X_test, y_train, y_valid, y_test, categorical_cols, and continuous_cols
 
-  # Prepare the SubTabLightning Module
-  from ts3l.pl_modules import SubTabLightning
-  from ts3l.utils.subtab_utils import SubTabDataset, SubTabCollateFN
+  # Prepare the SCARFLightning Module
+  from ts3l.pl_modules import SCARFLightning
+  from ts3l.utils.scarf_utils import SCARFDataset
   from ts3l.utils import TS3LDataModule
-  from ts3l.utils.subtab_utils import SubTabConfig
+  from ts3l.utils.scarf_utils import SCARFConfig
   from pytorch_lightning import Trainer
 
   metric = "accuracy_score"
   input_dim = X_train.shape[1]
   hidden_dim = 1024
   output_dim = 2
-  tau = 1.0
-  use_cosine_similarity = True
-  use_contrastive = True
-  use_distance = True
-  n_subsets = 4
-  overlap_ratio = 0.75
+  encoder_depth = 3
+  head_depth = 1
+  dropout_rate = 0.04
 
-  mask_ratio = 0.1
-  noise_type = "Swap"
-  noise_level = 0.1
-
-  data_hparams = {
-              "n_subsets" : n_subsets,
-              "overlap_ratio" : overlap_ratio,
-              "mask_ratio" : mask_ratio,
-              "noise_type" : noise_type,
-              "noise_level" : noise_level,
-              "n_column" : input_dim
-          }
+  corruption_rate = 0.6
 
   batch_size = 128
-  max_epochs = 3
+  max_epochs = 10
 
   X_train, X_unlabeled, y_train, _ = train_test_split(X_train, y_train, train_size = 0.1, random_state=0, stratify=y_train)
 
-  config = SubTabConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
+  config = SCARFConfig( task="classification", loss_fn="CrossEntropyLoss", metric=metric, metric_hparams={},
   input_dim=input_dim, hidden_dim=hidden_dim,
-  output_dim=output_dim, tau=tau, use_cosine_similarity= use_cosine_similarity, use_contrastive=use_contrastive, use_distance=use_distance, 
-  n_subsets=n_subsets, overlap_ratio=overlap_ratio
+  output_dim=output_dim, encoder_depth=encoder_depth, head_depth=head_depth,
+  dropout_rate=dropout_rate, corruption_rate = corruption_rate
   )
 
-  pl_subtab = SubTabLightning(config)
+  pl_scarf = SCARFLightning(config)
 
   ### First Phase Learning
-  train_ds = SubTabDataset(X_train, unlabeled_data=X_unlabeled)
-  valid_ds = SubTabDataset(X_valid)
+  train_ds = SCARFDataset(X_train, unlabeled_data=X_unlabeled, config = config)
+  valid_ds = SCARFDataset(X_valid, config=config)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size, train_sampler='random', train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams), n_jobs = 4)
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size=batch_size, train_sampler="random")
 
   trainer = Trainer(
                       accelerator = 'cpu',
                       max_epochs = max_epochs,
                       num_sanity_val_steps = 2,
       )
 
-  trainer.fit(pl_subtab, datamodule)
+  trainer.fit(pl_scarf, datamodule)
 
   ### Second Phase Learning
 
-  pl_subtab.set_second_phase()
+  pl_scarf.set_second_phase()
 
-  train_ds = SubTabDataset(X_train, y_train.values)
-  valid_ds = SubTabDataset(X_valid, y_valid.values)
+  train_ds = SCARFDataset(X_train, y_train.values, is_second_phase=True)
+  valid_ds = SCARFDataset(X_valid, y_valid.values, is_second_phase=True)
 
-  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted", train_collate_fn=SubTabCollateFN(data_hparams), valid_collate_fn=SubTabCollateFN(data_hparams))
+  datamodule = TS3LDataModule(train_ds, valid_ds, batch_size = batch_size, train_sampler="weighted")
 
-  trainer.fit(pl_subtab, datamodule)
+  trainer.fit(pl_scarf, datamodule)
 
   # Evaluation
   from sklearn.metrics import accuracy_score
   import torch
   from torch.nn import functional as F
   from torch.utils.data import DataLoader, SequentialSampler
 
-  test_ds = SubTabDataset(X_test)
-  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4, collate_fn=SubTabCollateFN(data_hparams))
+  test_ds = SCARFDataset(X_test, is_second_phase=True)
+  test_dl = DataLoader(test_ds, batch_size, shuffle=False, sampler = SequentialSampler(test_ds), num_workers=4)
 
-  preds = trainer.predict(pl_subtab, test_dl)
+  preds = trainer.predict(pl_scarf, test_dl)
           
   preds = F.softmax(torch.concat([out.cpu() for out in preds]).squeeze(),dim=1)
 
   accuracy = accuracy_score(y_test, preds.argmax(1))
 
   print("Accuracy %.2f" % accuracy)
   ```
 
 </details>
 
-#### To DO
+
+## Benchmark
+
+We provide a simple benchmark using TabularS3L against XGBoost. The train-validation-test ratio is 6:2:2 and we tuned each model over 50 trials using Optuna. The results are the average of the random seeds [0,4]. The best results are bold. 'acc', 'b-acc', and 'mse' mean 'Accuracy', 'Balanced Accuracy', and 'Mean Squared Error', respectively.
+
+Use this benchmark for reference only, as only a small number of random seeds were used.
+
+##### 10% labeled samples 
+
+| Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
+|:---:|:---:|:---:|:---:|
+| XGBoost | 0.7325 | 0.4763 | **5.5739** |
+| DAE | 0.7208 | 0.4885 | 5.6168 | 
+| VIME | 0.7182 | **0.5087** | 5.6637 |
+| SubTab | 0.7312 | 0.4930 | 7.2418 |
+| SCARF | **0.7416** | 0.4710 | 5.8888 | 
+
+--------
+
+##### 100% labeled samples
+
+| Model | diabetes (acc) | cmc (b-acc) | abalone (mse) |
+|:---:|:---:|:---:|:---:|
+| XGBoost | 0.7234 | 0.5291 | 4.8377 |
+| DAE | 0.7390 | 0.5500 | 4.5758 |
+| VIME | **0.7688** | 0.5477 | 4.5804 |
+| SubTab | 0.7390 | 0.5432 | 6.3104 |
+| SCARF | 0.7442 | **0.5521** | **4.4443** |
+
+## To DO
 
 - [x] Release nn.Module and Dataset of VIME, SubTab, and SCARF
   - [x] VIME
   - [x] SubTab
   - [x] SCARF
 - [x] Release LightningModules of VIME, SubTab, and SCARF
   - [x] VIME
   - [x] SubTab
   - [x] SCARF
-- [ ] Release Denoising AutoEncoder
-  - [ ] nn.Module
-  - [ ] LightningModule
+- [x] Release Denoising AutoEncoder
+  - [x] nn.Module
+  - [x] LightningModule
 - [ ] Release SwitchTab
   - [ ] nn.Module
   - [ ] LightningModule
-- [ ] Release PTaRL
-  - [ ] Add Backbones
-    - [ ] MLP
-    - [ ] ResNet
-    - [ ] FT-Transformer
-  - [ ] LightningModule
-- [ ] Add example codes
+- [x] Add example codes
 
 ## Contributing
 
 Contributions to this implementation are highly appreciated. Whether it's suggesting improvements, reporting bugs, or proposing new features, feel free to open an issue or submit a pull request.
 
 
 ## Credit  
 ```
 @software{alcoholrithm_2024_10776538,
   author       = {Minwook Kim},
   title        = {TabularS3L},
   month        = mar,
   year         = 2024,
   publisher    = {Zenodo},
-  version      = {v0.20},
+  version      = {v0.21},
   doi          = {10.5281/zenodo.10776538},
   url          = {https://doi.org/10.5281/zenodo.10776538}
 }
 ```
```

### Comparing `ts3l-0.21/ts3l.egg-info/SOURCES.txt` & `ts3l-0.30/ts3l.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 LICENSE
 README.md
 setup.py
+test/test_dae.py
 test/test_scarf.py
 test/test_subtab.py
 test/test_vime.py
 ts3l/__init__.py
 ts3l.egg-info/PKG-INFO
 ts3l.egg-info/SOURCES.txt
 ts3l.egg-info/dependency_links.txt
 ts3l.egg-info/requires.txt
 ts3l.egg-info/top_level.txt
 ts3l/models/__init__.py
+ts3l/models/common/__init__.py
+ts3l/models/common/mlp.py
+ts3l/models/dae/__init__.py
+ts3l/models/dae/dae.py
 ts3l/models/scarf/__init__.py
 ts3l/models/scarf/scarf.py
 ts3l/models/subtab/__init__.py
 ts3l/models/subtab/subtab.py
 ts3l/models/vime/__init__.py
 ts3l/models/vime/vime.py
 ts3l/models/vime/vime_self.py
 ts3l/models/vime/vime_semi.py
 ts3l/pl_modules/__init__.py
 ts3l/pl_modules/base_module.py
+ts3l/pl_modules/dae_lightning.py
 ts3l/pl_modules/scarf_lightning.py
 ts3l/pl_modules/subtab_lightning.py
 ts3l/pl_modules/vime_lightning.py
 ts3l/utils/__init__.py
 ts3l/utils/base_config.py
 ts3l/utils/datamodule.py
 ts3l/utils/misc.py
+ts3l/utils/dae_utils/__init__.py
+ts3l/utils/dae_utils/dae_config.py
+ts3l/utils/dae_utils/data_utils.py
 ts3l/utils/scarf_utils/__init__.py
 ts3l/utils/scarf_utils/data_utils.py
 ts3l/utils/scarf_utils/loss.py
 ts3l/utils/scarf_utils/scarf_config.py
 ts3l/utils/subtab_utils/__init__.py
 ts3l/utils/subtab_utils/data_utils.py
 ts3l/utils/subtab_utils/loss.py
```

