# Comparing `tmp/bk-audit-1.2.0b1.tar.gz` & `tmp/bk_audit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk-audit-1.2.0b1.tar", last modified: Thu Feb  1 02:11:31 2024, max compression
+gzip compressed data, was "bk_audit-1.2.1.tar", last modified: Mon Apr 22 03:54:48 2024, max compression
```

## Comparing `bk-audit-1.2.0b1.tar` & `bk_audit-1.2.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:11:31.430786 bk-audit-1.2.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-02-01 02:11:31.426786 bk-audit-1.2.0b1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:11:31.422786 bk-audit-1.2.0b1/bk_audit/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:11:31.422786 bk-audit-1.2.0b1/bk_audit/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/constants/contrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/constants/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/constants/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:11:31.422786 bk-audit-1.2.0b1/bk_audit/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:11:31.422786 bk-audit-1.2.0b1/bk_audit/contrib/bk_audit/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/bk_audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/bk_audit/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/bk_audit/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/bk_audit/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:11:31.422786 bk-audit-1.2.0b1/bk_audit/contrib/django/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/django/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/django/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/django/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:11:31.426786 bk-audit-1.2.0b1/bk_audit/contrib/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/opentelemetry/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/opentelemetry/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/opentelemetry/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/contrib/opentelemetry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:11:31.426786 bk-audit-1.2.0b1/bk_audit/log/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/log/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/log/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/log/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/log/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/log/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:11:31.426786 bk-audit-1.2.0b1/bk_audit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/bk_audit/utils/time_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:11:31.426786 bk-audit-1.2.0b1/bk_audit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-02-01 02:11:31.000000 bk-audit-1.2.0b1/bk_audit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-01 02:11:31.000000 bk-audit-1.2.0b1/bk_audit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 02:11:31.000000 bk-audit-1.2.0b1/bk_audit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-01 02:11:31.000000 bk-audit-1.2.0b1/bk_audit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-01 02:11:31.000000 bk-audit-1.2.0b1/bk_audit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 02:11:31.430786 bk-audit-1.2.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 02:11:31.426786 bk-audit-1.2.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/tests/test_ot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-01 02:11:21.000000 bk-audit-1.2.0b1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.852488 bk_audit-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 03:54:35.000000 bk_audit-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-22 03:54:48.852488 bk_audit-1.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.844488 bk_audit-1.2.1/bk_audit/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.848488 bk_audit-1.2.1/bk_audit/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/constants/contrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/constants/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/constants/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.848488 bk_audit-1.2.1/bk_audit/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.848488 bk_audit-1.2.1/bk_audit/contrib/bk_audit/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/bk_audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/bk_audit/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/bk_audit/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/bk_audit/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.848488 bk_audit-1.2.1/bk_audit/contrib/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/django/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/django/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/django/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.848488 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.852488 bk_audit-1.2.1/bk_audit/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.852488 bk_audit-1.2.1/bk_audit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/utils/time_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.852488 bk_audit-1.2.1/bk_audit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-22 03:54:48.000000 bk_audit-1.2.1/bk_audit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-22 03:54:48.000000 bk_audit-1.2.1/bk_audit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 03:54:48.000000 bk_audit-1.2.1/bk_audit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 03:54:48.000000 bk_audit-1.2.1/bk_audit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 03:54:48.000000 bk_audit-1.2.1/bk_audit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-22 03:54:35.000000 bk_audit-1.2.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 03:54:48.852488 bk_audit-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-22 03:54:35.000000 bk_audit-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.852488 bk_audit-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-22 03:54:35.000000 bk_audit-1.2.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-22 03:54:35.000000 bk_audit-1.2.1/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-22 03:54:35.000000 bk_audit-1.2.1/tests/test_ot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-22 03:54:35.000000 bk_audit-1.2.1/tests/test_utils.py
```

### Comparing `bk-audit-1.2.0b1/PKG-INFO` & `bk_audit-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bk-audit
-Version: 1.2.0b1
+Version: 1.2.1
 Summary: Bk Audit SDK
 Home-page: https://bk.tencent.com
 Author: blueking
 Author-email: blueking@tencent.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -23,15 +23,15 @@
 Requires-Dist: opentelemetry-exporter-otlp<1.13.0,>=1.7.1; extra == "opentelemetry"
 Provides-Extra: bk-resource
 Requires-Dist: bk_resource>=0.4.0; extra == "bk-resource"
 
 ![logo.png](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/assests/logo.png)
 
 [![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/LICENSE.txt)
-[![Release Version](https://img.shields.io/badge/release-1.2.0-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
+[![Release Version](https://img.shields.io/badge/release-1.2.1-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/pulls)
 [![codecov](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk/branch/master/graph/badge.svg?token=CUG20ZMOVQ)](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk)
 [![Test](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml/badge.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml)
 
 [(English Documents Available)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/readme_en.md)
 
 ## Overview
```

### Comparing `bk-audit-1.2.0b1/bk_audit/__init__.py` & `bk_audit-1.2.1/bk_audit/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/client.py` & `bk_audit-1.2.1/bk_audit/client.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/constants/__init__.py` & `bk_audit-1.2.1/bk_audit/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/constants/contrib.py` & `bk_audit-1.2.1/bk_audit/constants/contrib.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/constants/log.py` & `bk_audit-1.2.1/bk_audit/constants/log.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/constants/utils.py` & `bk_audit-1.2.1/bk_audit/constants/utils.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/__init__.py` & `bk_audit-1.2.1/bk_audit/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/bk_audit/__init__.py` & `bk_audit-1.2.1/bk_audit/contrib/bk_audit/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/bk_audit/apps.py` & `bk_audit-1.2.1/bk_audit/contrib/bk_audit/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 """
 
 import os
 
 from django.apps import AppConfig
 from django.utils.translation import gettext_lazy
 
-from bk_audit.contrib.bk_audit.settings import bk_audit_settings
-
 
 class AuditConfig(AppConfig):
     name = "bk_audit.contrib.bk_audit"
     verbose_name = gettext_lazy("BK Audit")
 
     def ready(self):
+        from bk_audit.contrib.bk_audit.settings import bk_audit_settings
+
         if not bk_audit_settings.ot_endpoint and not os.getenv("BKAPP_OTEL_LOG_ENDPOINT"):
             return
 
         from bk_audit.contrib.bk_audit.client import bk_audit_client
         from bk_audit.contrib.opentelemetry.setup import setup
 
         setup(
```

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/bk_audit/client.py` & `bk_audit-1.2.1/bk_audit/contrib/bk_audit/client.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/bk_audit/settings.py` & `bk_audit-1.2.1/bk_audit/contrib/bk_audit/settings.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/django/__init__.py` & `bk_audit-1.2.1/bk_audit/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/django/formatters.py` & `bk_audit-1.2.1/bk_audit/contrib/django/formatters.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/django/loggers.py` & `bk_audit-1.2.1/bk_audit/contrib/django/loggers.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/django/resources.py` & `bk_audit-1.2.1/bk_audit/contrib/django/resources.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/opentelemetry/__init__.py` & `bk_audit-1.2.1/bk_audit/contrib/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/opentelemetry/exporters.py` & `bk_audit-1.2.1/bk_audit/contrib/opentelemetry/exporters.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/opentelemetry/processor.py` & `bk_audit-1.2.1/bk_audit/contrib/opentelemetry/processor.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/opentelemetry/setup.py` & `bk_audit-1.2.1/bk_audit/contrib/opentelemetry/setup.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/contrib/opentelemetry/utils.py` & `bk_audit-1.2.1/bk_audit/contrib/opentelemetry/utils.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/log/__init__.py` & `bk_audit-1.2.1/bk_audit/log/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/log/base.py` & `bk_audit-1.2.1/bk_audit/log/base.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/log/exporters.py` & `bk_audit-1.2.1/bk_audit/log/exporters.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/log/formatters.py` & `bk_audit-1.2.1/bk_audit/log/formatters.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/log/models.py` & `bk_audit-1.2.1/bk_audit/log/models.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/log/queue.py` & `bk_audit-1.2.1/bk_audit/log/queue.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/utils/__init__.py` & `bk_audit-1.2.1/bk_audit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/utils/decorators.py` & `bk_audit-1.2.1/bk_audit/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit/utils/time_tool.py` & `bk_audit-1.2.1/bk_audit/utils/time_tool.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/bk_audit.egg-info/PKG-INFO` & `bk_audit-1.2.1/bk_audit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bk-audit
-Version: 1.2.0b1
+Version: 1.2.1
 Summary: Bk Audit SDK
 Home-page: https://bk.tencent.com
 Author: blueking
 Author-email: blueking@tencent.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -23,15 +23,15 @@
 Requires-Dist: opentelemetry-exporter-otlp<1.13.0,>=1.7.1; extra == "opentelemetry"
 Provides-Extra: bk-resource
 Requires-Dist: bk_resource>=0.4.0; extra == "bk-resource"
 
 ![logo.png](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/assests/logo.png)
 
 [![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/LICENSE.txt)
-[![Release Version](https://img.shields.io/badge/release-1.2.0-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
+[![Release Version](https://img.shields.io/badge/release-1.2.1-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/pulls)
 [![codecov](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk/branch/master/graph/badge.svg?token=CUG20ZMOVQ)](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk)
 [![Test](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml/badge.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml)
 
 [(English Documents Available)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/readme_en.md)
 
 ## Overview
```

### Comparing `bk-audit-1.2.0b1/bk_audit.egg-info/SOURCES.txt` & `bk_audit-1.2.1/bk_audit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/readme.md` & `bk_audit-1.2.1/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ![logo.png](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/assests/logo.png)
 
 [![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/LICENSE.txt)
-[![Release Version](https://img.shields.io/badge/release-1.2.0-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
+[![Release Version](https://img.shields.io/badge/release-1.2.1-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/pulls)
 [![codecov](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk/branch/master/graph/badge.svg?token=CUG20ZMOVQ)](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk)
 [![Test](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml/badge.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml)
 
 [(English Documents Available)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/readme_en.md)
 
 ## Overview
```

### Comparing `bk-audit-1.2.0b1/setup.py` & `bk_audit-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 current_directory = os.path.abspath(os.path.dirname(__file__))
 readme_path = os.path.join(current_directory, "readme.md")
 with open(readme_path) as f:
     readme = f.read()
 
 setup(
     name="bk-audit",
-    version="1.2.0-beta.1",
+    version="1.2.1",
     author="blueking",
     url="https://bk.tencent.com",
     author_email="blueking@tencent.com",
     description="Bk Audit SDK",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=[
```

### Comparing `bk-audit-1.2.0b1/tests/test_client.py` & `bk_audit-1.2.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/tests/test_django.py` & `bk_audit-1.2.1/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/tests/test_ot.py` & `bk_audit-1.2.1/tests/test_ot.py`

 * *Files identical despite different names*

### Comparing `bk-audit-1.2.0b1/tests/test_utils.py` & `bk_audit-1.2.1/tests/test_utils.py`

 * *Files identical despite different names*

