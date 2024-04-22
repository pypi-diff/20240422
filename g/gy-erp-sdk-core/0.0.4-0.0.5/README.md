# Comparing `tmp/gy-erp-sdk-core-0.0.4.tar.gz` & `tmp/gy-erp-sdk-core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gy-erp-sdk-core-0.0.4.tar", last modified: Mon Apr 22 02:38:47 2024, max compression
+gzip compressed data, was "gy-erp-sdk-core-0.0.5.tar", last modified: Mon Apr 22 02:57:24 2024, max compression
```

## Comparing `gy-erp-sdk-core-0.0.4.tar` & `gy-erp-sdk-core-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:38:47.403409 gy-erp-sdk-core-0.0.4/
--rw-r--r--   0 zty        (501) staff       (20)      889 2024-04-22 02:38:47.403113 gy-erp-sdk-core-0.0.4/PKG-INFO
--rw-r--r--   0 zty        (501) staff       (20)      490 2024-04-19 09:51:51.000000 gy-erp-sdk-core-0.0.4/README.md
-drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:38:47.396516 gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/
--rw-r--r--   0 zty        (501) staff       (20)      889 2024-04-22 02:38:47.000000 gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/PKG-INFO
--rw-r--r--   0 zty        (501) staff       (20)      394 2024-04-22 02:38:47.000000 gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 zty        (501) staff       (20)        1 2024-04-22 02:38:47.000000 gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 zty        (501) staff       (20)       13 2024-04-22 02:38:47.000000 gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/top_level.txt
-drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:38:47.396856 gy-erp-sdk-core-0.0.4/gyerpsdkcore/
--rw-r--r--   0 zty        (501) staff       (20)      107 2024-04-22 02:34:37.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/__init__.py
-drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:38:47.400642 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/
--rw-r--r--   0 zty        (501) staff       (20)       80 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/__init__.py
--rw-r--r--   0 zty        (501) staff       (20)      663 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/base.py
--rw-r--r--   0 zty        (501) staff       (20)      171 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/item.py
--rw-r--r--   0 zty        (501) staff       (20)      333 2024-04-19 09:51:26.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/new_stock.py
--rw-r--r--   0 zty        (501) staff       (20)      464 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/trade.py
-drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:38:47.402501 gy-erp-sdk-core-0.0.4/gyerpsdkcore/client/
--rw-r--r--   0 zty        (501) staff       (20)      343 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/client/__init__.py
--rw-r--r--   0 zty        (501) staff       (20)     1908 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/gyerpsdkcore/client/base.py
--rw-r--r--   0 zty        (501) staff       (20)       38 2024-04-22 02:38:47.403533 gy-erp-sdk-core-0.0.4/setup.cfg
--rw-r--r--   0 zty        (501) staff       (20)      820 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.4/setup.py
+drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:57:24.792266 gy-erp-sdk-core-0.0.5/
+-rw-r--r--   0 zty        (501) staff       (20)      889 2024-04-22 02:57:24.791748 gy-erp-sdk-core-0.0.5/PKG-INFO
+-rw-r--r--   0 zty        (501) staff       (20)      490 2024-04-19 09:51:51.000000 gy-erp-sdk-core-0.0.5/README.md
+drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:57:24.782770 gy-erp-sdk-core-0.0.5/gy_erp_sdk_core.egg-info/
+-rw-r--r--   0 zty        (501) staff       (20)      889 2024-04-22 02:57:24.000000 gy-erp-sdk-core-0.0.5/gy_erp_sdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 zty        (501) staff       (20)      394 2024-04-22 02:57:24.000000 gy-erp-sdk-core-0.0.5/gy_erp_sdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 zty        (501) staff       (20)        1 2024-04-22 02:57:24.000000 gy-erp-sdk-core-0.0.5/gy_erp_sdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 zty        (501) staff       (20)       13 2024-04-22 02:57:24.000000 gy-erp-sdk-core-0.0.5/gy_erp_sdk_core.egg-info/top_level.txt
+drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:57:24.783187 gy-erp-sdk-core-0.0.5/gyerpsdkcore/
+-rw-r--r--   0 zty        (501) staff       (20)      107 2024-04-22 02:57:22.000000 gy-erp-sdk-core-0.0.5/gyerpsdkcore/__init__.py
+drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:57:24.786753 gy-erp-sdk-core-0.0.5/gyerpsdkcore/api/
+-rw-r--r--   0 zty        (501) staff       (20)      128 2024-04-22 02:56:44.000000 gy-erp-sdk-core-0.0.5/gyerpsdkcore/api/__init__.py
+-rw-r--r--   0 zty        (501) staff       (20)      663 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.5/gyerpsdkcore/api/base.py
+-rw-r--r--   0 zty        (501) staff       (20)      171 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.5/gyerpsdkcore/api/item.py
+-rw-r--r--   0 zty        (501) staff       (20)      333 2024-04-19 09:51:26.000000 gy-erp-sdk-core-0.0.5/gyerpsdkcore/api/new_stock.py
+-rw-r--r--   0 zty        (501) staff       (20)      464 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.5/gyerpsdkcore/api/trade.py
+drwxr-xr-x   0 zty        (501) staff       (20)        0 2024-04-22 02:57:24.789278 gy-erp-sdk-core-0.0.5/gyerpsdkcore/client/
+-rw-r--r--   0 zty        (501) staff       (20)      374 2024-04-22 02:56:44.000000 gy-erp-sdk-core-0.0.5/gyerpsdkcore/client/__init__.py
+-rw-r--r--   0 zty        (501) staff       (20)     1908 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.5/gyerpsdkcore/client/base.py
+-rw-r--r--   0 zty        (501) staff       (20)       38 2024-04-22 02:57:24.792473 gy-erp-sdk-core-0.0.5/setup.cfg
+-rw-r--r--   0 zty        (501) staff       (20)      820 2024-04-19 09:29:34.000000 gy-erp-sdk-core-0.0.5/setup.py
```

### Comparing `gy-erp-sdk-core-0.0.4/PKG-INFO` & `gy-erp-sdk-core-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gy-erp-sdk-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: gy erp api Python sdk.
 Home-page: https://github.com/stevenQiang
 Author: Steven
 Author-email: qianggao7@gmail.com
 License: cc
 Description: # gy-erp-sdk-core
```

### Comparing `gy-erp-sdk-core-0.0.4/gy_erp_sdk_core.egg-info/PKG-INFO` & `gy-erp-sdk-core-0.0.5/gy_erp_sdk_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gy-erp-sdk-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: gy erp api Python sdk.
 Home-page: https://github.com/stevenQiang
 Author: Steven
 Author-email: qianggao7@gmail.com
 License: cc
 Description: # gy-erp-sdk-core
```

### Comparing `gy-erp-sdk-core-0.0.4/gyerpsdkcore/api/base.py` & `gy-erp-sdk-core-0.0.5/gyerpsdkcore/api/base.py`

 * *Files identical despite different names*

### Comparing `gy-erp-sdk-core-0.0.4/gyerpsdkcore/client/base.py` & `gy-erp-sdk-core-0.0.5/gyerpsdkcore/client/base.py`

 * *Files identical despite different names*

### Comparing `gy-erp-sdk-core-0.0.4/setup.py` & `gy-erp-sdk-core-0.0.5/setup.py`

 * *Files identical despite different names*

