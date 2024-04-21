# Comparing `tmp/paper2vec-1.0.1.tar.gz` & `tmp/paper2vec-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper2vec-1.0.1.tar", last modified: Sun Apr 21 23:33:43 2024, max compression
+gzip compressed data, was "paper2vec-1.0.2.tar", last modified: Sun Apr 21 23:41:44 2024, max compression
```

## Comparing `paper2vec-1.0.1.tar` & `paper2vec-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 23:33:37.000000 paper2vec-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-21 23:33:43.139913 paper2vec-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 23:33:37.000000 paper2vec-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/datadestination/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/datadestination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/datadestination/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/datasource/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/datasource/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/retrieverdestination/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/retrieverdestination/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/scripts/qdrant_create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/vectorizer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/vectorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/vectorizer/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-21 23:33:43.000000 paper2vec-1.0.1/paper2vec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-21 23:33:43.000000 paper2vec-1.0.1/paper2vec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 23:33:43.000000 paper2vec-1.0.1/paper2vec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 23:33:43.000000 paper2vec-1.0.1/paper2vec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 23:33:43.000000 paper2vec-1.0.1/paper2vec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 23:33:43.139913 paper2vec-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-21 23:33:37.000000 paper2vec-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.508509 paper2vec-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 23:41:36.000000 paper2vec-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-21 23:41:44.508509 paper2vec-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 23:41:36.000000 paper2vec-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.500509 paper2vec-1.0.2/paper2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.500509 paper2vec-1.0.2/paper2vec/datadestination/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/datadestination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/datadestination/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.500509 paper2vec-1.0.2/paper2vec/datasource/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/datasource/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.500509 paper2vec-1.0.2/paper2vec/retrieverdestination/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.500509 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.504509 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.504509 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.504509 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/api/default/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/api/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/api/default/delete_delete_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/api/default/query_main_query_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/api/default/upsert_file_upsert_file_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/api/default/upsert_upsert_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.508509 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/body_upsert_file_upsert_file_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/delete_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/document_chunk_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/document_chunk_with_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/document_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/document_metadata_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/query_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/upsert_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/upsert_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/fast_api_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/retrieverdestination/openai/retrieval_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.508509 paper2vec-1.0.2/paper2vec/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/scripts/qdrant_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.508509 paper2vec-1.0.2/paper2vec/vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/vectorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 23:41:36.000000 paper2vec-1.0.2/paper2vec/vectorizer/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:41:44.500509 paper2vec-1.0.2/paper2vec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-21 23:41:44.000000 paper2vec-1.0.2/paper2vec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-21 23:41:44.000000 paper2vec-1.0.2/paper2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 23:41:44.000000 paper2vec-1.0.2/paper2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 23:41:44.000000 paper2vec-1.0.2/paper2vec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 23:41:44.000000 paper2vec-1.0.2/paper2vec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 23:41:44.508509 paper2vec-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-21 23:41:36.000000 paper2vec-1.0.2/setup.py
```

### Comparing `paper2vec-1.0.1/LICENSE` & `paper2vec-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0.1/paper2vec/abc.py` & `paper2vec-1.0.2/paper2vec/abc.py`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0.1/paper2vec/config.py` & `paper2vec-1.0.2/paper2vec/config.py`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0.1/paper2vec/datadestination/qdrant.py` & `paper2vec-1.0.2/paper2vec/datadestination/qdrant.py`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0.1/paper2vec/datasource/neo4j.py` & `paper2vec-1.0.2/paper2vec/datasource/neo4j.py`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0.1/paper2vec/vectorizer/openai.py` & `paper2vec-1.0.2/paper2vec/vectorizer/openai.py`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0.1/setup.py` & `paper2vec-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,23 +5,28 @@
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 package_dir = {
     'paper2vec': 'paper2vec',
     'paper2vec.retrieverdestination': 'paper2vec/retrieverdestination',
+    'paper2vec.retrieverdestination.openai': 'paper2vec/retrieverdestination/openai',
+    'paper2vec.retrieverdestination.openai.fast_api_client': 'paper2vec/retrieverdestination/openai/fast_api_client',
+    'paper2vec.retrieverdestination.openai.fast_api_client.models': 'paper2vec/retrieverdestination/openai/fast_api_client/models',
+    'paper2vec.retrieverdestination.openai.fast_api_client.api': 'paper2vec/retrieverdestination/openai/fast_api_client/api',
+    'paper2vec.retrieverdestination.openai.fast_api_client.api.default': 'paper2vec/retrieverdestination/openai/fast_api_client/api/default',
     'paper2vec.datadestination': 'paper2vec/datadestination',
     'paper2vec.datasource': 'paper2vec/datasource',
     'paper2vec.vectorizer': 'paper2vec/vectorizer',
     'paper2vec.scripts': 'paper2vec/scripts',
 }
 
 setup(
     name='paper2vec',
-    version='1.0.1',
+    version='1.0.2',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/paper2vec',
     description=u'Turn your collected papers into vectors!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

