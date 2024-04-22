# Comparing `tmp/SpiderKidSDK-0.0.1.tar.gz` & `tmp/SpiderKidSDK-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpiderKidSDK-0.0.1.tar", last modified: Mon Apr 22 02:17:51 2024, max compression
+gzip compressed data, was "SpiderKidSDK-0.0.2.tar", last modified: Mon Apr 22 02:30:49 2024, max compression
```

## Comparing `SpiderKidSDK-0.0.1.tar` & `SpiderKidSDK-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:17:51.087141 SpiderKidSDK-0.0.1/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      676 2024-04-22 02:17:51.086977 SpiderKidSDK-0.0.1/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      458 2024-04-22 02:17:06.000000 SpiderKidSDK-0.0.1/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:17:51.086217 SpiderKidSDK-0.0.1/SpiderKid/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       57 2024-04-22 02:08:02.000000 SpiderKidSDK-0.0.1/SpiderKid/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      922 2024-04-22 02:07:59.000000 SpiderKidSDK-0.0.1/SpiderKid/spider_kid.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:17:51.086806 SpiderKidSDK-0.0.1/SpiderKidSDK.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      676 2024-04-22 02:17:51.000000 SpiderKidSDK-0.0.1/SpiderKidSDK.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      208 2024-04-22 02:17:51.000000 SpiderKidSDK-0.0.1/SpiderKidSDK.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2024-04-22 02:17:51.000000 SpiderKidSDK-0.0.1/SpiderKidSDK.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       10 2024-04-22 02:17:51.000000 SpiderKidSDK-0.0.1/SpiderKidSDK.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2024-04-22 02:17:51.087170 SpiderKidSDK-0.0.1/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      428 2024-04-22 02:10:17.000000 SpiderKidSDK-0.0.1/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:30:49.969636 SpiderKidSDK-0.0.2/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      676 2024-04-22 02:30:49.969462 SpiderKidSDK-0.0.2/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      458 2024-04-22 02:17:06.000000 SpiderKidSDK-0.0.2/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:30:49.968474 SpiderKidSDK-0.0.2/SpiderKid/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       57 2024-04-22 02:30:35.000000 SpiderKidSDK-0.0.2/SpiderKid/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      922 2024-04-22 02:07:59.000000 SpiderKidSDK-0.0.2/SpiderKid/spider_kid.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2024-04-22 02:30:49.969121 SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      676 2024-04-22 02:30:49.000000 SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      254 2024-04-22 02:30:49.000000 SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2024-04-22 02:30:49.000000 SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       10 2024-04-22 02:30:49.000000 SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2024-04-22 02:30:49.969666 SpiderKidSDK-0.0.2/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      428 2024-04-22 02:30:42.000000 SpiderKidSDK-0.0.2/setup.py
```

### Comparing `SpiderKidSDK-0.0.1/PKG-INFO` & `SpiderKidSDK-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpiderKidSDK
-Version: 0.0.1
+Version: 0.0.2
 Summary: SpiderKid SDK
 Home-page: https://github.com/Jyonn/SpiderKidSDK
 Author: Jyonn Liu
 Author-email: liu@qijiong.work
 Description-Content-Type: text/markdown
 
 # SpiderKidSDK
```

### Comparing `SpiderKidSDK-0.0.1/SpiderKid/spider_kid.py` & `SpiderKidSDK-0.0.2/SpiderKid/spider_kid.py`

 * *Files identical despite different names*

### Comparing `SpiderKidSDK-0.0.1/SpiderKidSDK.egg-info/PKG-INFO` & `SpiderKidSDK-0.0.2/SpiderKidSDK.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpiderKidSDK
-Version: 0.0.1
+Version: 0.0.2
 Summary: SpiderKid SDK
 Home-page: https://github.com/Jyonn/SpiderKidSDK
 Author: Jyonn Liu
 Author-email: liu@qijiong.work
 Description-Content-Type: text/markdown
 
 # SpiderKidSDK
```

