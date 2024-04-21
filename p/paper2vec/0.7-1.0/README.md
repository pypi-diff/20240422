# Comparing `tmp/paper2vec-0.7.tar.gz` & `tmp/paper2vec-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper2vec-0.7.tar", last modified: Sun Apr 21 22:51:54 2024, max compression
+gzip compressed data, was "paper2vec-1.0.tar", last modified: Sun Apr 21 23:24:26 2024, max compression
```

## Comparing `paper2vec-0.7.tar` & `paper2vec-1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 22:51:48.000000 paper2vec-0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 22:51:54.858118 paper2vec-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 22:51:48.000000 paper2vec-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec/datadestination/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/datadestination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/datadestination/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec/datasource/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/datasource/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/scripts/qdrant_create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec/vectorizer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/vectorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/vectorizer/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 22:51:54.000000 paper2vec-0.7/paper2vec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-21 22:51:54.000000 paper2vec-0.7/paper2vec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:51:54.000000 paper2vec-0.7/paper2vec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 22:51:54.000000 paper2vec-0.7/paper2vec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 22:51:54.000000 paper2vec-0.7/paper2vec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:51:54.858118 paper2vec-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 22:51:48.000000 paper2vec-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.816762 paper2vec-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 23:24:19.000000 paper2vec-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 23:24:26.816762 paper2vec-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 23:24:19.000000 paper2vec-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.812762 paper2vec-1.0/paper2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.812762 paper2vec-1.0/paper2vec/datadestination/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/datadestination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/datadestination/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.816762 paper2vec-1.0/paper2vec/datasource/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/datasource/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.816762 paper2vec-1.0/paper2vec/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/scripts/qdrant_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.816762 paper2vec-1.0/paper2vec/vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/vectorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 23:24:19.000000 paper2vec-1.0/paper2vec/vectorizer/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:24:26.812762 paper2vec-1.0/paper2vec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 23:24:26.000000 paper2vec-1.0/paper2vec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-21 23:24:26.000000 paper2vec-1.0/paper2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 23:24:26.000000 paper2vec-1.0/paper2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 23:24:26.000000 paper2vec-1.0/paper2vec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 23:24:26.000000 paper2vec-1.0/paper2vec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 23:24:26.816762 paper2vec-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 23:24:19.000000 paper2vec-1.0/setup.py
```

### Comparing `paper2vec-0.7/LICENSE` & `paper2vec-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper2vec-0.7/paper2vec/abc.py` & `paper2vec-1.0/paper2vec/abc.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.7/paper2vec/config.py` & `paper2vec-1.0/paper2vec/config.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.7/paper2vec/datadestination/qdrant.py` & `paper2vec-1.0/paper2vec/datadestination/qdrant.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.7/paper2vec/datasource/neo4j.py` & `paper2vec-1.0/paper2vec/datasource/neo4j.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,22 +2,31 @@
 from paper2vec.abc import DataSource, Content
 from argparse import ArgumentParser
 
 
 async def get_papers(tx, query):
     papers = []
     for record in await (await tx.run(query)).values():
-        if "title" not in record[0]:
+        paper = record[0]
+        if "title" not in paper:
             papers.append(None)
             continue
-        paper = "Title: " + record[0]["title"]
-        metadata = {"title": record[0]["title"], "title_hash": record[0]["title_hash"]}
-        if "abstract" in record[0]:
-            paper += " Abstract: " + record[0]["abstract"]
-        content = Content(id=record[0]["title_hash"], text=paper, metadata=metadata)
+        metadata = {"source": "file", "source_id": paper["title_hash"]}
+        if "doi" in paper:
+            metadata["url"] = f"https://doi.org/" + paper["doi"]
+        elif "paperId" in paper:
+            metadata["url"] = f"https://www.semanticscholar.org/paper/" + paper["paperId"]
+        if "date" in paper:
+            metadata["created_at"] = paper["date"]
+        elif "year" in paper:
+            metadata["created_at"] = paper["year"]
+        text = "Title: " + paper["title"]
+        if "abstract" in paper:
+            text += "\n Abstract: " + paper["abstract"]
+        content = Content(id=paper["title_hash"] + "-title-abstract", text=text, metadata=metadata)
         papers.append(content)
     return papers
 
 
 async def get_total(tx, query):
     records = await (await tx.run(query)).values()
     return records[0][0]
```

### Comparing `paper2vec-0.7/paper2vec/vectorizer/openai.py` & `paper2vec-1.0/paper2vec/vectorizer/openai.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.7/setup.py` & `paper2vec-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'paper2vec.datasource': 'paper2vec/datasource',
     'paper2vec.vectorizer': 'paper2vec/vectorizer',
     'paper2vec.scripts': 'paper2vec/scripts',
 }
 
 setup(
     name='paper2vec',
-    version='0.7',
+    version='1.0',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/paper2vec',
     description=u'Turn your collected papers into vectors!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

