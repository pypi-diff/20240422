# Comparing `tmp/llama_index_vector_stores_databricks-0.1.1.tar.gz` & `tmp/llama_index_vector_stores_databricks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_databricks-0.1.1.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_databricks-0.1.2.tar", max compression
```

## Comparing `llama_index_vector_stores_databricks-0.1.1.tar` & `llama_index_vector_stores_databricks-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       65 2024-03-14 22:46:27.147382 llama_index_vector_stores_databricks-0.1.1/README.md
--rw-r--r--   0        0        0       17 2024-03-14 22:46:27.147382 llama_index_vector_stores_databricks-0.1.1/llama_index/vector_stores/databricks/BUILD
--rw-r--r--   0        0        0      124 2024-03-14 22:46:27.147382 llama_index_vector_stores_databricks-0.1.1/llama_index/vector_stores/databricks/__init__.py
--rw-r--r--   0        0        0    14270 2024-03-14 22:46:27.147382 llama_index_vector_stores_databricks-0.1.1/llama_index/vector_stores/databricks/base.py
--rw-r--r--   0        0        0     1554 2024-03-14 22:46:27.147382 llama_index_vector_stores_databricks-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 llama_index_vector_stores_databricks-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       65 2024-04-22 02:04:56.207354 llama_index_vector_stores_databricks-0.1.2/README.md
+-rw-r--r--   0        0        0       17 2024-04-22 02:04:56.207354 llama_index_vector_stores_databricks-0.1.2/llama_index/vector_stores/databricks/BUILD
+-rw-r--r--   0        0        0      124 2024-04-22 02:04:56.207354 llama_index_vector_stores_databricks-0.1.2/llama_index/vector_stores/databricks/__init__.py
+-rw-r--r--   0        0        0    14323 2024-04-22 02:04:56.207354 llama_index_vector_stores_databricks-0.1.2/llama_index/vector_stores/databricks/base.py
+-rw-r--r--   0        0        0     1554 2024-04-22 02:04:56.207354 llama_index_vector_stores_databricks-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 llama_index_vector_stores_databricks-0.1.2/PKG-INFO
```

### Comparing `llama_index_vector_stores_databricks-0.1.1/llama_index/vector_stores/databricks/base.py` & `llama_index_vector_stores_databricks-0.1.2/llama_index/vector_stores/databricks/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,16 @@
         for node in nodes:
             node_id = node.node_id
             metadata = node_to_metadata_dict(node, remove_text=True, flat_metadata=True)
 
             metadata_columns = self.columns or []
 
             # explicitly record doc_id as metadata (for delete)
-            metadata_columns.append("doc_id")
+            if "doc_id" not in metadata_columns:
+                metadata_columns.append("doc_id")
 
             entry = {
                 self._primary_key: node_id,
                 self.text_column: node.get_content(),
                 self._embedding_vector_column_name(): node.get_embedding(),
                 **{
                     col: metadata.get(col)
```

### Comparing `llama_index_vector_stores_databricks-0.1.1/pyproject.toml` & `llama_index_vector_stores_databricks-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [tool.poetry]
 authors = ["Alberto Da Costa <alberto@bamelevate.com>", "Nickhil Nabar <nickhil@bamelevate.com"]
 description = "llama-index vector_stores databricks vector search integration"
 license = "MIT"
 name = "llama-index-vector-stores-databricks"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 llama-index-core = "^0.10.1"
 databricks-vectorsearch = "^0.21"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_databricks-0.1.1/PKG-INFO` & `llama_index_vector_stores_databricks-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-databricks
-Version: 0.1.1
+Version: 0.1.2
 Summary: llama-index vector_stores databricks vector search integration
 License: MIT
 Author: Alberto Da Costa
 Author-email: alberto@bamelevate.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

