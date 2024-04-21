# Comparing `tmp/paper2vec-0.6.tar.gz` & `tmp/paper2vec-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper2vec-0.6.tar", last modified: Sun Apr 21 22:44:25 2024, max compression
+gzip compressed data, was "paper2vec-0.7.tar", last modified: Sun Apr 21 22:51:54 2024, max compression
```

## Comparing `paper2vec-0.6.tar` & `paper2vec-0.7.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 22:44:19.000000 paper2vec-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 22:44:25.933956 paper2vec-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 22:44:19.000000 paper2vec-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.929956 paper2vec-0.6/paper2vec/
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/paper2vec/datadestination/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/datadestination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/datadestination/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/paper2vec/datasource/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/datasource/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/paper2vec/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/scripts/qdrant_create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/paper2vec/vectorizer/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/vectorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 22:44:19.000000 paper2vec-0.6/paper2vec/vectorizer/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:44:25.933956 paper2vec-0.6/paper2vec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 22:44:25.000000 paper2vec-0.6/paper2vec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-21 22:44:25.000000 paper2vec-0.6/paper2vec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:44:25.000000 paper2vec-0.6/paper2vec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 22:44:25.000000 paper2vec-0.6/paper2vec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 22:44:25.000000 paper2vec-0.6/paper2vec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:44:25.933956 paper2vec-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 22:44:19.000000 paper2vec-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 22:51:48.000000 paper2vec-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 22:51:54.858118 paper2vec-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 22:51:48.000000 paper2vec-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec/datadestination/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/datadestination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/datadestination/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec/datasource/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/datasource/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/scripts/qdrant_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec/vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/vectorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 22:51:48.000000 paper2vec-0.7/paper2vec/vectorizer/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:51:54.858118 paper2vec-0.7/paper2vec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-21 22:51:54.000000 paper2vec-0.7/paper2vec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-21 22:51:54.000000 paper2vec-0.7/paper2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:51:54.000000 paper2vec-0.7/paper2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 22:51:54.000000 paper2vec-0.7/paper2vec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 22:51:54.000000 paper2vec-0.7/paper2vec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:51:54.858118 paper2vec-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 22:51:48.000000 paper2vec-0.7/setup.py
```

### Comparing `paper2vec-0.6/LICENSE` & `paper2vec-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paper2vec-0.6/paper2vec/__main__.py` & `paper2vec-0.7/paper2vec/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 import asyncio
 from itertools import product
 from paper2vec.datasource import alias as datasources
 from paper2vec.vectorizer import alias as vectorizers
 from paper2vec.datadestination import alias as datadestinations
 from paper2vec.retrieverdestination import alias as retrieverdestinations
 from paper2vec.abc import run_vectorizer, run_retriever
-from argparse import ArgumentParser
+from argparse import ArgumentParser, _SubParsersAction
 
 
-def func_parser_gen_vectorizer(datasource_constructor, vectorizer_constructor, datadestination_constructor):
-    def func_parser(parser):
-        args = parser.parse_args()
-        datasource = datasource_constructor(args)
-        vectorizer = vectorizer_constructor(args)
-        datadestination = datadestination_constructor(args)
-        asyncio.get_event_loop().run_until_complete(
-            run_vectorizer(datasource, vectorizer, datadestination, batch_size=args.batch_size)
-        )
-    return func_parser
-
+def add_arguments_vectorizer(subparsers: _SubParsersAction):
 
-def func_parser_gen_retriever(datasource_constructor, retriever_constructor):
-    def func_parser(parser):
-        args = parser.parse_args()
-        datasource = datasource_constructor(args)
-        retriever = retriever_constructor(args)
-        asyncio.get_event_loop().run_until_complete(
-            run_retriever(datasource, retriever, batch_size=args.batch_size)
+    def func_parser_gen(datasource_constructor, vectorizer_constructor, datadestination_constructor):
+        def func_parser(parser):
+            args = parser.parse_args()
+            datasource = datasource_constructor(args)
+            vectorizer = vectorizer_constructor(args)
+            datadestination = datadestination_constructor(args)
+            asyncio.get_event_loop().run_until_complete(
+                run_vectorizer(datasource, vectorizer, datadestination, batch_size=args.batch_size)
+            )
+        return func_parser
+
+    for datasource, vectorizer, datadestination in product(datasources.keys(), vectorizers.keys(), datadestinations.keys()):
+        subparser = subparsers.add_parser(
+            f"{datasource}-{vectorizer}-{datadestination}",
+            help=f"{datasource} -text-> {vectorizer} -vector-> {datadestination}"
+        )
+        datasources[datasource].add_arguments(subparser)
+        vectorizers[vectorizer].add_arguments(subparser)
+        datadestinations[datadestination].add_arguments(subparser)
+        subparser.set_defaults(func=func_parser_gen(
+            datasources[datasource],
+            vectorizers[vectorizer],
+            datadestinations[datadestination]
+        ))
+
+
+def add_arguments_retriever(subparsers: _SubParsersAction):
+
+    def func_parser_gen(datasource_constructor, retriever_constructor):
+        def func_parser(parser):
+            args = parser.parse_args()
+            datasource = datasource_constructor(args)
+            retriever = retriever_constructor(args)
+            asyncio.get_event_loop().run_until_complete(
+                run_retriever(datasource, retriever, batch_size=args.batch_size)
+            )
+        return func_parser
+
+    for datasource, retrieverdestination in product(datasources.keys(), retrieverdestinations.keys()):
+        subparser = subparsers.add_parser(
+            f"{datasource}-{retrieverdestination}",
+            help=f"{datasource} -text-> {retrieverdestination}"
         )
-    return func_parser
+        datasources[datasource].add_arguments(subparser)
+        retrieverdestinations[retrieverdestination].add_arguments(subparser)
+        subparser.set_defaults(func=func_parser_gen(
+            datasources[datasource],
+            retrieverdestinations[retrieverdestination]
+        ))
 
 
-parser = ArgumentParser()
-parser.add_argument("--batch-size", type=int, default=64, help=f'Batch size of vectorize.')
-subparsers = parser.add_subparsers(help='sub-command help')
-for datasource, vectorizer, datadestination in product(datasources.keys(), vectorizers.keys(), datadestinations.keys()):
-    subparser = subparsers.add_parser(
-        f"{datasource}-{vectorizer}-{datadestination}",
-        help=f"{datasource} -text-> {vectorizer} -vector-> {datadestination}"
-    )
-    datasources[datasource].add_arguments(subparser)
-    vectorizers[vectorizer].add_arguments(subparser)
-    datadestinations[datadestination].add_arguments(subparser)
-    subparser.set_defaults(func=func_parser_gen_vectorizer(
-        datasources[datasource],
-        vectorizers[vectorizer],
-        datadestinations[datadestination]
-    ))
-for datasource, retrieverdestination in product(datasources.keys(), retrieverdestinations.keys()):
-    subparser = subparsers.add_parser(
-        f"{datasource}-{retrieverdestination}",
-        help=f"{datasource} -text-> {retrieverdestination}"
-    )
-    datasources[datasource].add_arguments(subparser)
-    retrieverdestinations[retrieverdestination].add_arguments(subparser)
-    subparser.set_defaults(func=func_parser_gen_retriever(
-        datasources[datasource],
-        retrieverdestinations[retrieverdestination]
-    ))
-
-
-# --------- Run ---------
-args = parser.parse_args()
-args.func(parser)
+def add_arguments(parser: ArgumentParser):
+    parser.add_argument("--batch-size", type=int, default=64, help=f'Batch size of vectorize.')
+    subparsers = parser.add_subparsers(help='sub-command help')
+    add_arguments_vectorizer(subparsers)
+    add_arguments_retriever(subparsers)
```

### Comparing `paper2vec-0.6/paper2vec/abc.py` & `paper2vec-0.7/paper2vec/abc.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.6/paper2vec/datadestination/qdrant.py` & `paper2vec-0.7/paper2vec/datadestination/qdrant.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.6/paper2vec/datasource/neo4j.py` & `paper2vec-0.7/paper2vec/datasource/neo4j.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.6/paper2vec/vectorizer/openai.py` & `paper2vec-0.7/paper2vec/vectorizer/openai.py`

 * *Files identical despite different names*

### Comparing `paper2vec-0.6/setup.py` & `paper2vec-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'paper2vec.datasource': 'paper2vec/datasource',
     'paper2vec.vectorizer': 'paper2vec/vectorizer',
     'paper2vec.scripts': 'paper2vec/scripts',
 }
 
 setup(
     name='paper2vec',
-    version='0.6',
+    version='0.7',
     author='yindaheng98',
     author_email='yindaheng98@gmail.com',
     url='https://github.com/yindaheng98/paper2vec',
     description=u'Turn your collected papers into vectors!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

