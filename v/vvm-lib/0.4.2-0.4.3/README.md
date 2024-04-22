# Comparing `tmp/vvm_lib-0.4.2.tar.gz` & `tmp/vvm_lib-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvm_lib-0.4.2.tar", last modified: Mon Apr 22 08:57:19 2024, max compression
+gzip compressed data, was "vvm_lib-0.4.3.tar", last modified: Mon Apr 22 09:26:28 2024, max compression
```

## Comparing `vvm_lib-0.4.2.tar` & `vvm_lib-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 08:57:19.110454 vvm_lib-0.4.2/
--rw-rw-rw-   0        0        0      454 2024-04-22 08:57:19.110454 vvm_lib-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-20 07:29:21.000000 vvm_lib-0.4.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 08:57:19.115376 vvm_lib-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      747 2024-04-22 08:49:53.000000 vvm_lib-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:57:19.086567 vvm_lib-0.4.2/vvm_lib/
-drwxrwxrwx   0        0        0        0 2024-04-22 08:57:19.108453 vvm_lib-0.4.2/vvm_lib/DB/
--rw-rw-rw-   0        0        0       17 2024-04-22 08:37:11.000000 vvm_lib-0.4.2/vvm_lib/DB/__init__.py
--rw-rw-rw-   0        0        0     5821 2024-04-22 08:49:07.000000 vvm_lib-0.4.2/vvm_lib/DB/db.py
--rw-rw-rw-   0        0        0      229 2024-04-20 07:29:21.000000 vvm_lib-0.4.2/vvm_lib/__init__.py
--rw-rw-rw-   0        0        0     2747 2024-04-20 07:29:21.000000 vvm_lib-0.4.2/vvm_lib/google_book.py
--rw-rw-rw-   0        0        0     3545 2024-04-20 07:29:21.000000 vvm_lib-0.4.2/vvm_lib/greenplum.py
--rw-rw-rw-   0        0        0      654 2024-04-20 07:29:21.000000 vvm_lib-0.4.2/vvm_lib/mssql.py
--rw-rw-rw-   0        0        0      855 2024-04-20 07:29:21.000000 vvm_lib-0.4.2/vvm_lib/vault.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:57:19.109453 vvm_lib-0.4.2/vvm_lib.egg-info/
--rw-rw-rw-   0        0        0      454 2024-04-22 08:57:19.000000 vvm_lib-0.4.2/vvm_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-04-22 08:57:19.000000 vvm_lib-0.4.2/vvm_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 08:57:19.000000 vvm_lib-0.4.2/vvm_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 08:57:19.000000 vvm_lib-0.4.2/vvm_lib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       94 2024-04-22 08:57:19.000000 vvm_lib-0.4.2/vvm_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 08:57:19.000000 vvm_lib-0.4.2/vvm_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 09:26:28.263125 vvm_lib-0.4.3/
+-rw-rw-rw-   0        0        0      454 2024-04-22 09:26:28.262126 vvm_lib-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-20 07:29:21.000000 vvm_lib-0.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 09:26:28.268124 vvm_lib-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      747 2024-04-22 09:26:05.000000 vvm_lib-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:26:28.230192 vvm_lib-0.4.3/vvm_lib/
+drwxrwxrwx   0        0        0        0 2024-04-22 09:26:28.259125 vvm_lib-0.4.3/vvm_lib/DB/
+-rw-rw-rw-   0        0        0       17 2024-04-22 08:37:11.000000 vvm_lib-0.4.3/vvm_lib/DB/__init__.py
+-rw-rw-rw-   0        0        0     5821 2024-04-22 08:49:07.000000 vvm_lib-0.4.3/vvm_lib/DB/db.py
+-rw-rw-rw-   0        0        0      229 2024-04-20 07:29:21.000000 vvm_lib-0.4.3/vvm_lib/__init__.py
+-rw-rw-rw-   0        0        0     2747 2024-04-20 07:29:21.000000 vvm_lib-0.4.3/vvm_lib/google_book.py
+-rw-rw-rw-   0        0        0     3545 2024-04-20 07:29:21.000000 vvm_lib-0.4.3/vvm_lib/greenplum.py
+-rw-rw-rw-   0        0        0      654 2024-04-20 07:29:21.000000 vvm_lib-0.4.3/vvm_lib/mssql.py
+-rw-rw-rw-   0        0        0      855 2024-04-20 07:29:21.000000 vvm_lib-0.4.3/vvm_lib/vault.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:26:28.261123 vvm_lib-0.4.3/vvm_lib.egg-info/
+-rw-rw-rw-   0        0        0      454 2024-04-22 09:26:28.000000 vvm_lib-0.4.3/vvm_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2024-04-22 09:26:28.000000 vvm_lib-0.4.3/vvm_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 09:26:28.000000 vvm_lib-0.4.3/vvm_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 08:57:19.000000 vvm_lib-0.4.3/vvm_lib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       94 2024-04-22 09:26:28.000000 vvm_lib-0.4.3/vvm_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-22 09:26:28.000000 vvm_lib-0.4.3/vvm_lib.egg-info/top_level.txt
```

### Comparing `vvm_lib-0.4.2/setup.py` & `vvm_lib-0.4.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 
 setup(name='vvm_lib',
-      version='0.4.2',
+      version='0.4.3',
       description='my frequently used functions',
       packages=[
           'vvm_lib',
-          "vvm_lib.DB",
+          "vvm_lib.db",
           ],
       package_dir={
         "vvm_lib": "vvm_lib",
-        "vvm_lib.DB": "vvm_lib/DB",
+        "vvm_lib.DB": "vvm_lib/db",
     },
       author_email='v.vazhinskiy@yandex.ru',
       author="vvazhinskiy",
       url="https://github.com/VazhikVM/vvm_lib",
       zip_safe=False,
       install_requires=[
           "pandas",
```

### Comparing `vvm_lib-0.4.2/vvm_lib/DB/db.py` & `vvm_lib-0.4.3/vvm_lib/DB/db.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-0.4.2/vvm_lib/google_book.py` & `vvm_lib-0.4.3/vvm_lib/google_book.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-0.4.2/vvm_lib/greenplum.py` & `vvm_lib-0.4.3/vvm_lib/greenplum.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-0.4.2/vvm_lib/mssql.py` & `vvm_lib-0.4.3/vvm_lib/mssql.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-0.4.2/vvm_lib/vault.py` & `vvm_lib-0.4.3/vvm_lib/vault.py`

 * *Files identical despite different names*

