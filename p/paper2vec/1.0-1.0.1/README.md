# Comparing `tmp/paper2vec-1.0.tar.gz` & `tmp/paper2vec-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper2vec-1.0.tar", last modified: Sun Apr 21 23:24:26 2024, max compression
+gzip compressed data, was "paper2vec-1.0.1.tar", last modified: Sun Apr 21 23:33:43 2024, max compression
```

## Comparing `paper2vec-1.0.tar` & `paper2vec-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.816762 paper2vec-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 23:24:19.000000 paper2vec-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 23:24:26.816762 paper2vec-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 23:24:19.000000 paper2vec-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.812762 paper2vec-1.0/paper2vec/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.812762 paper2vec-1.0/paper2vec/datadestination/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/datadestination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/datadestination/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.816762 paper2vec-1.0/paper2vec/datasource/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/datasource/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.816762 paper2vec-1.0/paper2vec/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/scripts/qdrant_create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.816762 paper2vec-1.0/paper2vec/vectorizer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/vectorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/vectorizer/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.812762 paper2vec-1.0/paper2vec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 23:24:26.000000 paper2vec-1.0/paper2vec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-21 23:24:26.000000 paper2vec-1.0/paper2vec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 23:24:26.000000 paper2vec-1.0/paper2vec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 23:24:26.000000 paper2vec-1.0/paper2vec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 23:24:26.000000 paper2vec-1.0/paper2vec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 23:24:26.816762 paper2vec-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 23:24:19.000000 paper2vec-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 23:33:37.000000 paper2vec-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-21 23:33:43.139913 paper2vec-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 23:33:37.000000 paper2vec-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/datadestination/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/datadestination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/datadestination/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/datasource/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/datasource/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/retrieverdestination/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/retrieverdestination/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/scripts/qdrant_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec/vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/vectorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 23:33:37.000000 paper2vec-1.0.1/paper2vec/vectorizer/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:33:43.139913 paper2vec-1.0.1/paper2vec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-21 23:33:43.000000 paper2vec-1.0.1/paper2vec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-21 23:33:43.000000 paper2vec-1.0.1/paper2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 23:33:43.000000 paper2vec-1.0.1/paper2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 23:33:43.000000 paper2vec-1.0.1/paper2vec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 23:33:43.000000 paper2vec-1.0.1/paper2vec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 23:33:43.139913 paper2vec-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-21 23:33:37.000000 paper2vec-1.0.1/setup.py
```

### Comparing `paper2vec-1.0/LICENSE` & `paper2vec-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0/paper2vec/abc.py` & `paper2vec-1.0.1/paper2vec/abc.py`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0/paper2vec/config.py` & `paper2vec-1.0.1/paper2vec/config.py`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0/paper2vec/datadestination/qdrant.py` & `paper2vec-1.0.1/paper2vec/datadestination/qdrant.py`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0/paper2vec/datasource/neo4j.py` & `paper2vec-1.0.1/paper2vec/datasource/neo4j.py`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0/paper2vec/vectorizer/openai.py` & `paper2vec-1.0.1/paper2vec/vectorizer/openai.py`

 * *Files identical despite different names*

### Comparing `paper2vec-1.0/setup.py` & `paper2vec-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 package_dir = {
     'paper2vec': 'paper2vec',
+    'paper2vec.retrieverdestination': 'paper2vec/retrieverdestination',
     'paper2vec.datadestination': 'paper2vec/datadestination',
     'paper2vec.datasource': 'paper2vec/datasource',
     'paper2vec.vectorizer': 'paper2vec/vectorizer',
     'paper2vec.scripts': 'paper2vec/scripts',
 }
 
 setup(
     name='paper2vec',
-    version='1.0',
+    version='1.0.1',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/paper2vec',
     description=u'Turn your collected papers into vectors!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

