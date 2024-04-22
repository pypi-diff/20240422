# Comparing `tmp/embedding-techx-1.0.tar.gz` & `tmp/embedding-techx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedding-techx-1.0.tar", last modified: Mon Apr 22 08:19:45 2024, max compression
+gzip compressed data, was "embedding-techx-1.0.1.tar", last modified: Mon Apr 22 08:49:37 2024, max compression
```

## Comparing `embedding-techx-1.0.tar` & `embedding-techx-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 08:19:45.195481 embedding-techx-1.0/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      303 2024-04-22 08:19:45.194856 embedding-techx-1.0/PKG-INFO
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 08:19:45.191953 embedding-techx-1.0/embedding-techx/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      857 2024-04-22 07:58:22.000000 embedding-techx-1.0/embedding-techx/__init__.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     3126 2024-04-22 07:24:49.000000 embedding-techx-1.0/embedding-techx/dataframe.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     2427 2024-04-22 07:58:11.000000 embedding-techx-1.0/embedding-techx/domain_emb.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     7471 2024-04-22 07:58:05.000000 embedding-techx-1.0/embedding-techx/embedding.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     8299 2024-04-22 07:55:58.000000 embedding-techx-1.0/embedding-techx/evaluate.py
--rw-r--r--   0 ninananakorn   (501) staff       (20)     1658 2024-04-22 07:54:40.000000 embedding-techx-1.0/embedding-techx/search.py
-drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 08:19:45.194437 embedding-techx-1.0/embedding_techx.egg-info/
--rw-r--r--   0 ninananakorn   (501) staff       (20)      303 2024-04-22 08:19:45.000000 embedding-techx-1.0/embedding_techx.egg-info/PKG-INFO
--rw-r--r--   0 ninananakorn   (501) staff       (20)      372 2024-04-22 08:19:45.000000 embedding-techx-1.0/embedding_techx.egg-info/SOURCES.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-04-22 08:19:45.000000 embedding-techx-1.0/embedding_techx.egg-info/dependency_links.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       96 2024-04-22 08:19:45.000000 embedding-techx-1.0/embedding_techx.egg-info/requires.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       16 2024-04-22 08:19:45.000000 embedding-techx-1.0/embedding_techx.egg-info/top_level.txt
--rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-04-22 08:19:45.195546 embedding-techx-1.0/setup.cfg
--rw-r--r--   0 ninananakorn   (501) staff       (20)      408 2024-04-22 08:09:19.000000 embedding-techx-1.0/setup.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 08:49:37.709020 embedding-techx-1.0.1/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      260 2024-04-22 08:49:37.708428 embedding-techx-1.0.1/PKG-INFO
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 08:49:37.702138 embedding-techx-1.0.1/embedding-techx/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      857 2024-04-22 07:58:22.000000 embedding-techx-1.0.1/embedding-techx/__init__.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     3126 2024-04-22 08:47:08.000000 embedding-techx-1.0.1/embedding-techx/dataframe.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     2427 2024-04-22 08:47:06.000000 embedding-techx-1.0.1/embedding-techx/domain_emb.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     7471 2024-04-22 08:47:06.000000 embedding-techx-1.0.1/embedding-techx/embedding.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     8299 2024-04-22 08:47:07.000000 embedding-techx-1.0.1/embedding-techx/evaluate.py
+-rw-r--r--   0 ninananakorn   (501) staff       (20)     1658 2024-04-22 08:47:07.000000 embedding-techx-1.0.1/embedding-techx/search.py
+drwxr-xr-x   0 ninananakorn   (501) staff       (20)        0 2024-04-22 08:49:37.708018 embedding-techx-1.0.1/embedding_techx.egg-info/
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      260 2024-04-22 08:49:37.000000 embedding-techx-1.0.1/embedding_techx.egg-info/PKG-INFO
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      372 2024-04-22 08:49:37.000000 embedding-techx-1.0.1/embedding_techx.egg-info/SOURCES.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)        1 2024-04-22 08:49:37.000000 embedding-techx-1.0.1/embedding_techx.egg-info/dependency_links.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       81 2024-04-22 08:49:37.000000 embedding-techx-1.0.1/embedding_techx.egg-info/requires.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       16 2024-04-22 08:49:37.000000 embedding-techx-1.0.1/embedding_techx.egg-info/top_level.txt
+-rw-r--r--   0 ninananakorn   (501) staff       (20)       38 2024-04-22 08:49:37.709147 embedding-techx-1.0.1/setup.cfg
+-rw-r--r--   0 ninananakorn   (501) staff       (20)      373 2024-04-22 08:49:30.000000 embedding-techx-1.0.1/setup.py
```

### Comparing `embedding-techx-1.0/embedding-techx/__init__.py` & `embedding-techx-1.0.1/embedding-techx/__init__.py`

 * *Files identical despite different names*

### Comparing `embedding-techx-1.0/embedding-techx/dataframe.py` & `embedding-techx-1.0.1/embedding-techx/dataframe.py`

 * *Files identical despite different names*

### Comparing `embedding-techx-1.0/embedding-techx/domain_emb.py` & `embedding-techx-1.0.1/embedding-techx/domain_emb.py`

 * *Files identical despite different names*

### Comparing `embedding-techx-1.0/embedding-techx/embedding.py` & `embedding-techx-1.0.1/embedding-techx/embedding.py`

 * *Files identical despite different names*

### Comparing `embedding-techx-1.0/embedding-techx/evaluate.py` & `embedding-techx-1.0.1/embedding-techx/evaluate.py`

 * *Files identical despite different names*

### Comparing `embedding-techx-1.0/embedding-techx/search.py` & `embedding-techx-1.0.1/embedding-techx/search.py`

 * *Files identical despite different names*

