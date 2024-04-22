# Comparing `tmp/SpiderKidSDK-0.0.2.tar.gz` & `tmp/SpiderKidSDK-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpiderKidSDK-0.0.2.tar", last modified: Mon Apr 22 02:30:49 2024, max compression
+gzip compressed data, was "SpiderKidSDK-0.0.3.tar", last modified: Mon Apr 22 02:42:21 2024, max compression
```

## Comparing `SpiderKidSDK-0.0.2.tar` & `SpiderKidSDK-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:30:49.969636 SpiderKidSDK-0.0.2/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      676 2024-04-22 02:30:49.969462 SpiderKidSDK-0.0.2/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      458 2024-04-22 02:17:06.000000 SpiderKidSDK-0.0.2/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:30:49.968474 SpiderKidSDK-0.0.2/SpiderKid/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       57 2024-04-22 02:30:35.000000 SpiderKidSDK-0.0.2/SpiderKid/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      922 2024-04-22 02:07:59.000000 SpiderKidSDK-0.0.2/SpiderKid/spider_kid.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:30:49.969121 SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      676 2024-04-22 02:30:49.000000 SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      254 2024-04-22 02:30:49.000000 SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2024-04-22 02:30:49.000000 SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       10 2024-04-22 02:30:49.000000 SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2024-04-22 02:30:49.969666 SpiderKidSDK-0.0.2/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      428 2024-04-22 02:30:42.000000 SpiderKidSDK-0.0.2/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:42:21.117594 SpiderKidSDK-0.0.3/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      697 2024-04-22 02:42:21.117390 SpiderKidSDK-0.0.3/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      458 2024-04-22 02:17:06.000000 SpiderKidSDK-0.0.3/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:42:21.116786 SpiderKidSDK-0.0.3/SpiderKidSDK.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      697 2024-04-22 02:42:21.000000 SpiderKidSDK-0.0.3/SpiderKidSDK.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      208 2024-04-22 02:42:21.000000 SpiderKidSDK-0.0.3/SpiderKidSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2024-04-22 02:42:21.000000 SpiderKidSDK-0.0.3/SpiderKidSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       10 2024-04-22 02:42:21.000000 SpiderKidSDK-0.0.3/SpiderKidSDK.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2024-04-22 02:42:21.117627 SpiderKidSDK-0.0.3/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      449 2024-04-22 02:42:15.000000 SpiderKidSDK-0.0.3/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:42:21.117118 SpiderKidSDK-0.0.3/spiderkid/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       57 2024-04-22 02:30:35.000000 SpiderKidSDK-0.0.3/spiderkid/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      922 2024-04-22 02:07:59.000000 SpiderKidSDK-0.0.3/spiderkid/spider_kid.py
```

### Comparing `SpiderKidSDK-0.0.2/PKG-INFO` & `SpiderKidSDK-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: SpiderKidSDK
-Version: 0.0.2
-Summary: SpiderKid SDK
+Version: 0.0.3
+Summary: SpiderKid Software Development Kit
 Home-page: https://github.com/Jyonn/SpiderKidSDK
 Author: Jyonn Liu
 Author-email: liu@qijiong.work
 Description-Content-Type: text/markdown
 
 # SpiderKidSDK
```

### Comparing `SpiderKidSDK-0.0.2/SpiderKid/spider_kid.py` & `SpiderKidSDK-0.0.3/spiderkid/spider_kid.py`

 * *Files identical despite different names*

### Comparing `SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/PKG-INFO` & `SpiderKidSDK-0.0.3/SpiderKidSDK.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: SpiderKidSDK
-Version: 0.0.2
-Summary: SpiderKid SDK
+Version: 0.0.3
+Summary: SpiderKid Software Development Kit
 Home-page: https://github.com/Jyonn/SpiderKidSDK
 Author: Jyonn Liu
 Author-email: liu@qijiong.work
 Description-Content-Type: text/markdown
 
 # SpiderKidSDK
```

