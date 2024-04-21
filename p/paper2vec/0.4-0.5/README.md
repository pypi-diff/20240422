# Comparing `tmp/paper2vec-0.4.tar.gz` & `tmp/paper2vec-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper2vec-0.4.tar", last modified: Sat Apr 20 22:06:55 2024, max compression
+gzip compressed data, was "paper2vec-0.5.tar", last modified: Sun Apr 21 20:38:40 2024, max compression
```

## Comparing `paper2vec-0.4.tar` & `paper2vec-0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:06:55.512439 paper2vec-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-20 22:06:47.000000 paper2vec-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-20 22:06:55.512439 paper2vec-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 22:06:47.000000 paper2vec-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:06:55.512439 paper2vec-0.4/paper2vec/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-20 22:06:47.000000 paper2vec-0.4/paper2vec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-20 22:06:47.000000 paper2vec-0.4/paper2vec/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:06:55.512439 paper2vec-0.4/paper2vec/datadestination/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-20 22:06:47.000000 paper2vec-0.4/paper2vec/datadestination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-20 22:06:47.000000 paper2vec-0.4/paper2vec/datadestination/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:06:55.512439 paper2vec-0.4/paper2vec/datasource/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-20 22:06:47.000000 paper2vec-0.4/paper2vec/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-20 22:06:47.000000 paper2vec-0.4/paper2vec/datasource/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:06:55.512439 paper2vec-0.4/paper2vec/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-20 22:06:47.000000 paper2vec-0.4/paper2vec/scripts/qdrant_create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:06:55.512439 paper2vec-0.4/paper2vec/vectorizer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-20 22:06:47.000000 paper2vec-0.4/paper2vec/vectorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-20 22:06:47.000000 paper2vec-0.4/paper2vec/vectorizer/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:06:55.512439 paper2vec-0.4/paper2vec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-20 22:06:55.000000 paper2vec-0.4/paper2vec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-20 22:06:55.000000 paper2vec-0.4/paper2vec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 22:06:55.000000 paper2vec-0.4/paper2vec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-20 22:06:55.000000 paper2vec-0.4/paper2vec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 22:06:55.000000 paper2vec-0.4/paper2vec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 22:06:55.512439 paper2vec-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-20 22:06:47.000000 paper2vec-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 20:38:30.000000 paper2vec-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 20:38:40.575598 paper2vec-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 20:38:30.000000 paper2vec-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec/datadestination/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/datadestination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/datadestination/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec/datasource/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/datasource/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/scripts/qdrant_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec/vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/vectorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 20:38:30.000000 paper2vec-0.5/paper2vec/vectorizer/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:38:40.575598 paper2vec-0.5/paper2vec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 20:38:40.000000 paper2vec-0.5/paper2vec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-21 20:38:40.000000 paper2vec-0.5/paper2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 20:38:40.000000 paper2vec-0.5/paper2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 20:38:40.000000 paper2vec-0.5/paper2vec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 20:38:40.000000 paper2vec-0.5/paper2vec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 20:38:40.575598 paper2vec-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 20:38:30.000000 paper2vec-0.5/setup.py
```

### Comparing `paper2vec-0.4/LICENSE` & `paper2vec-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `paper2vec-0.4/paper2vec/__main__.py` & `paper2vec-0.5/paper2vec/__main__.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.4/paper2vec/abc.py` & `paper2vec-0.5/paper2vec/abc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 import abc
-from typing import List, Dict, AsyncGenerator
+from typing import List, Dict, AsyncGenerator, NamedTuple
 from argparse import ArgumentParser
 
 
 class Config(metaclass=abc.ABCMeta):
     @staticmethod
     @abc.abstractmethod
     def add_arguments(parser: ArgumentParser) -> None:
         pass
 
 
-class Content:
-    def __init__(self, id: str, text: str, payload: Dict):
-        self.id: str = id
-        self.text: str = text
-        self.payload: Dict = payload
+class Content(NamedTuple):
+    id: str
+    text: str
+    metadata: Dict
 
 
 class DataSource(Config):
     @abc.abstractmethod
     async def get_contents(self) -> AsyncGenerator[Content, None]:
         yield
 
 
 class Vectorizer(Config):
     @abc.abstractmethod
     async def vectorize(self, *contents: str) -> List[List[float]]:
         pass
 
 
-class Point:
-    def __init__(self, id: str, vector: List[float], payload: Dict):
-        self.id: str = id
-        self.vector: List[float] = vector
-        self.payload: Dict = payload
+class Point(NamedTuple):
+    id: str = id
+    vector: List[float]
+    metadata: Dict
 
 
 class DataDestination(Config):
     @abc.abstractmethod
     async def write_vectors(self, *vectors: Point) -> None:
         pass
 
 
+class RetrieverDestination(Config):
+    @abc.abstractmethod
+    async def upsert(self, *contents: Content) -> None:
+        pass
+
+
 async def run(datasource: DataSource, vectorizer: Vectorizer, datadestination: DataDestination, batch_size: int):
     batch: List[Content] = []
     async for content in datasource.get_contents():
         batch.append(content)
         if len(batch) >= batch_size:
             vectors = await vectorizer.vectorize(*[c.text for c in batch])
             points = [
-                Point(id=content.id, vector=vector, payload=content.payload) for vector, content in zip(vectors, batch)
+                Point(id=content.id, vector=vector, metadata=content.metadata) for vector, content in zip(vectors, batch)
             ]
             await datadestination.write_vectors(*points)
             batch = []
     if len(batch) > 0:
         vectors = await vectorizer.vectorize(*[c.text for c in batch])
         points = [
-            Point(id=content.id, vector=vector, payload=content.payload) for vector, content in zip(vectors, batch)
+            Point(id=content.id, vector=vector, metadata=content.metadata) for vector, content in zip(vectors, batch)
         ]
         await datadestination.write_vectors(*points)
```

### Comparing `paper2vec-0.4/paper2vec/datadestination/qdrant.py` & `paper2vec-0.5/paper2vec/datadestination/qdrant.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     async def write_vectors(self, *vectors: Point):
         operation_info = await self.client.upsert(
             collection_name=self.collection_name,
             wait=True,
             points=[
                 PointStruct(
                     id=str(uuid.UUID(hashlib.md5(point.id.encode("UTF-8")).hexdigest())),
-                    vector=point.vector, payload=point.payload
+                    vector=point.vector, payload=point.metadata
                 ) for point in vectors
             ]
         )
         print(operation_info)
 
     async def create_collection(self, size: int):
         await self.client.create_collection(
```

### Comparing `paper2vec-0.4/paper2vec/datasource/neo4j.py` & `paper2vec-0.5/paper2vec/datasource/neo4j.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 async def get_papers(tx, query):
     papers = []
     for record in await (await tx.run(query)).values():
         if "title" not in record[0]:
             papers.append(None)
             continue
         paper = "Title: " + record[0]["title"]
-        payload = {"title": record[0]["title"], "title_hash": record[0]["title_hash"]}
+        metadata = {"title": record[0]["title"], "title_hash": record[0]["title_hash"]}
         if "abstract" in record[0]:
             paper += " Abstract: " + record[0]["abstract"]
-        content = Content(id=record[0]["title_hash"], text=paper, payload=payload)
+        content = Content(id=record[0]["title_hash"], text=paper, metadata=metadata)
         papers.append(content)
     return papers
 
 
 async def get_total(tx, query):
     records = await (await tx.run(query)).values()
     return records[0][0]
```

### Comparing `paper2vec-0.4/paper2vec/vectorizer/openai.py` & `paper2vec-0.5/paper2vec/vectorizer/openai.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.4/setup.py` & `paper2vec-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'paper2vec.datasource': 'paper2vec/datasource',
     'paper2vec.vectorizer': 'paper2vec/vectorizer',
     'paper2vec.scripts': 'paper2vec/scripts',
 }
 
 setup(
     name='paper2vec',
-    version='0.4',
+    version='0.5',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/paper2vec',
     description=u'Turn your collected papers into vectors!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

