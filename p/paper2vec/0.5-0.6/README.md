# Comparing `tmp/paper2vec-0.5.tar.gz` & `tmp/paper2vec-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper2vec-0.5.tar", last modified: Sun Apr 21 20:38:40 2024, max compression
+gzip compressed data, was "paper2vec-0.6.tar", last modified: Sun Apr 21 22:44:25 2024, max compression
```

## Comparing `paper2vec-0.5.tar` & `paper2vec-0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 20:38:30.000000 paper2vec-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 20:38:40.575598 paper2vec-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 20:38:30.000000 paper2vec-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec/datadestination/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/datadestination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/datadestination/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec/datasource/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/datasource/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/scripts/qdrant_create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec/vectorizer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/vectorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/vectorizer/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 20:38:40.000000 paper2vec-0.5/paper2vec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-21 20:38:40.000000 paper2vec-0.5/paper2vec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 20:38:40.000000 paper2vec-0.5/paper2vec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 20:38:40.000000 paper2vec-0.5/paper2vec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 20:38:40.000000 paper2vec-0.5/paper2vec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 20:38:40.575598 paper2vec-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 20:38:30.000000 paper2vec-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 22:44:19.000000 paper2vec-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 22:44:25.933956 paper2vec-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 22:44:19.000000 paper2vec-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.929956 paper2vec-0.6/paper2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/paper2vec/datadestination/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/datadestination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/datadestination/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/paper2vec/datasource/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/datasource/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/paper2vec/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/scripts/qdrant_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/paper2vec/vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/vectorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/vectorizer/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/paper2vec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 22:44:25.000000 paper2vec-0.6/paper2vec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-21 22:44:25.000000 paper2vec-0.6/paper2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:44:25.000000 paper2vec-0.6/paper2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 22:44:25.000000 paper2vec-0.6/paper2vec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 22:44:25.000000 paper2vec-0.6/paper2vec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:44:25.933956 paper2vec-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 22:44:19.000000 paper2vec-0.6/setup.py
```

### Comparing `paper2vec-0.5/LICENSE` & `paper2vec-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `paper2vec-0.5/paper2vec/abc.py` & `paper2vec-0.6/paper2vec/abc.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 class Vectorizer(Config):
     @abc.abstractmethod
     async def vectorize(self, *contents: str) -> List[List[float]]:
         pass
 
 
 class Point(NamedTuple):
-    id: str = id
+    id: str
     vector: List[float]
     metadata: Dict
 
 
 class DataDestination(Config):
     @abc.abstractmethod
     async def write_vectors(self, *vectors: Point) -> None:
@@ -42,15 +42,15 @@
 
 class RetrieverDestination(Config):
     @abc.abstractmethod
     async def upsert(self, *contents: Content) -> None:
         pass
 
 
-async def run(datasource: DataSource, vectorizer: Vectorizer, datadestination: DataDestination, batch_size: int):
+async def run_vectorizer(datasource: DataSource, vectorizer: Vectorizer, datadestination: DataDestination, batch_size: int):
     batch: List[Content] = []
     async for content in datasource.get_contents():
         batch.append(content)
         if len(batch) >= batch_size:
             vectors = await vectorizer.vectorize(*[c.text for c in batch])
             points = [
                 Point(id=content.id, vector=vector, metadata=content.metadata) for vector, content in zip(vectors, batch)
@@ -59,7 +59,18 @@
             batch = []
     if len(batch) > 0:
         vectors = await vectorizer.vectorize(*[c.text for c in batch])
         points = [
             Point(id=content.id, vector=vector, metadata=content.metadata) for vector, content in zip(vectors, batch)
         ]
         await datadestination.write_vectors(*points)
+
+
+async def run_retriever(datasource: DataSource, retriever: RetrieverDestination, batch_size: int):
+    batch: List[Content] = []
+    async for content in datasource.get_contents():
+        batch.append(content)
+        if len(batch) >= batch_size:
+            await retriever.upsert(*batch)
+            batch = []
+    if len(batch) > 0:
+        await retriever.upsert(*batch)
```

### Comparing `paper2vec-0.5/paper2vec/datadestination/qdrant.py` & `paper2vec-0.6/paper2vec/datadestination/qdrant.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.5/paper2vec/datasource/neo4j.py` & `paper2vec-0.6/paper2vec/datasource/neo4j.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.5/paper2vec/vectorizer/openai.py` & `paper2vec-0.6/paper2vec/vectorizer/openai.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.5/setup.py` & `paper2vec-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'paper2vec.datasource': 'paper2vec/datasource',
     'paper2vec.vectorizer': 'paper2vec/vectorizer',
     'paper2vec.scripts': 'paper2vec/scripts',
 }
 
 setup(
     name='paper2vec',
-    version='0.5',
+    version='0.6',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/paper2vec',
     description=u'Turn your collected papers into vectors!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

