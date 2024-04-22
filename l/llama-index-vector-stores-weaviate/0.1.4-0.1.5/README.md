# Comparing `tmp/llama_index_vector_stores_weaviate-0.1.4.tar.gz` & `tmp/llama_index_vector_stores_weaviate-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_weaviate-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_weaviate-0.1.5.tar", max compression
```

## Comparing `llama_index_vector_stores_weaviate-0.1.4.tar` & `llama_index_vector_stores_weaviate-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       49 2024-03-07 18:51:43.808124 llama_index_vector_stores_weaviate-0.1.4/README.md
--rw-r--r--   0        0        0      107 2024-03-07 18:51:43.808124 llama_index_vector_stores_weaviate-0.1.4/llama_index/vector_stores/weaviate/__init__.py
--rw-r--r--   0        0        0    11106 2024-03-07 18:51:43.808124 llama_index_vector_stores_weaviate-0.1.4/llama_index/vector_stores/weaviate/base.py
--rw-r--r--   0        0        0     4890 2024-03-07 18:51:43.808124 llama_index_vector_stores_weaviate-0.1.4/llama_index/vector_stores/weaviate/utils.py
--rw-r--r--   0        0        0     1495 2024-03-07 18:51:43.808124 llama_index_vector_stores_weaviate-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 llama_index_vector_stores_weaviate-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-04-22 02:36:02.224598 llama_index_vector_stores_weaviate-0.1.5/README.md
+-rw-r--r--   0        0        0      107 2024-04-22 02:36:02.224598 llama_index_vector_stores_weaviate-0.1.5/llama_index/vector_stores/weaviate/__init__.py
+-rw-r--r--   0        0        0    12383 2024-04-22 02:36:02.224598 llama_index_vector_stores_weaviate-0.1.5/llama_index/vector_stores/weaviate/base.py
+-rw-r--r--   0        0        0     4890 2024-04-22 02:36:02.224598 llama_index_vector_stores_weaviate-0.1.5/llama_index/vector_stores/weaviate/utils.py
+-rw-r--r--   0        0        0     1495 2024-04-22 02:36:02.224598 llama_index_vector_stores_weaviate-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 llama_index_vector_stores_weaviate-0.1.5/PKG-INFO
```

### Comparing `llama_index_vector_stores_weaviate-0.1.4/llama_index/vector_stores/weaviate/base.py` & `llama_index_vector_stores_weaviate-0.1.5/llama_index/vector_stores/weaviate/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     parse_get_response,
     to_node,
 )
 
 import weaviate  # noqa
 from weaviate import AuthApiKey, Client
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 def _transform_weaviate_filter_condition(condition: str) -> str:
     """Translate standard metadata filter op to Chroma specific spec."""
     if condition == "and":
         return "And"
     elif condition == "or":
@@ -104,14 +104,33 @@
     k most similar nodes.
 
     Args:
         weaviate_client (weaviate.Client): WeaviateClient
             instance from `weaviate-client` package
         index_name (Optional[str]): name for Weaviate classes
 
+    Examples:
+        `pip install llama-index-vector-stores-weaviate`
+
+        ```python
+        import weaviate
+
+        resource_owner_config = weaviate.AuthClientPassword(
+            username="<username>",
+            password="<password>",
+        )
+        client = weaviate.Client(
+            "https://llama-test-ezjahb4m.weaviate.network",
+            auth_client_secret=resource_owner_config,
+        )
+
+        vector_store = WeaviateVectorStore(
+            weaviate_client=client, index_name="LlamaIndex"
+        )
+        ```
     """
 
     stores_text: bool = True
 
     index_name: str
     url: Optional[str]
     text_key: str
@@ -141,15 +160,15 @@
                 url=url, auth_client_secret=auth_config, **client_kwargs
             )
         else:
             self._client = cast(Client, weaviate_client)
 
         # validate class prefix starts with a capital letter
         if class_prefix is not None:
-            logger.warning("class_prefix is deprecated, please use index_name")
+            _logger.warning("class_prefix is deprecated, please use index_name")
             # legacy, kept for backward compatibility
             index_name = f"{class_prefix}_Node"
 
         index_name = index_name or f"LlamaIndex_{uuid4().hex}"
         if not index_name[0].isupper():
             raise ValueError(
                 "Index name must start with a capital letter, e.g. 'LlamaIndex'"
@@ -253,14 +272,32 @@
 
         query_result = query.do()
         parsed_result = parse_get_response(query_result)
         entries = parsed_result[self.index_name]
         for entry in entries:
             self._client.data_object.delete(entry["_additional"]["id"], self.index_name)
 
+    def delete_index(self) -> None:
+        """Delete the index associated with the client.
+
+        Raises:
+        - Exception: If the deletion fails, for some reason.
+        """
+        if not class_schema_exists(self._client, self.index_name):
+            _logger.warning(
+                f"Index '{self.index_name}' does not exist. No action taken."
+            )
+            return
+        try:
+            self._client.schema.delete_class(self.index_name)
+            _logger.info(f"Successfully deleted index '{self.index_name}'.")
+        except Exception as e:
+            _logger.error(f"Failed to delete index '{self.index_name}': {e}")
+            raise Exception(f"Failed to delete index '{self.index_name}': {e}")
+
     def query(self, query: VectorStoreQuery, **kwargs: Any) -> VectorStoreQueryResult:
         """Query index for top k most similar nodes."""
         all_properties = get_all_properties(self._client, self.index_name)
 
         # build query
         query_builder = self._client.query.get(self.index_name, all_properties)
 
@@ -288,23 +325,23 @@
         query_builder = query_builder.with_additional(
             ["id", "vector", "distance", "score"]
         )
 
         vector = query.query_embedding
         similarity_key = "distance"
         if query.mode == VectorStoreQueryMode.DEFAULT:
-            logger.debug("Using vector search")
+            _logger.debug("Using vector search")
             if vector is not None:
                 query_builder = query_builder.with_near_vector(
                     {
                         "vector": vector,
                     }
                 )
         elif query.mode == VectorStoreQueryMode.HYBRID:
-            logger.debug(f"Using hybrid search with alpha {query.alpha}")
+            _logger.debug(f"Using hybrid search with alpha {query.alpha}")
             similarity_key = "score"
             if vector is not None and query.query_str:
                 query_builder = query_builder.with_hybrid(
                     query=query.query_str,
                     alpha=query.alpha,
                     vector=vector,
                 )
@@ -312,15 +349,15 @@
         if query.filters is not None:
             filter = _to_weaviate_filter(query.filters)
             query_builder = query_builder.with_where(filter)
         elif "filter" in kwargs and kwargs["filter"] is not None:
             query_builder = query_builder.with_where(kwargs["filter"])
 
         query_builder = query_builder.with_limit(query.similarity_top_k)
-        logger.debug(f"Using limit of {query.similarity_top_k}")
+        _logger.debug(f"Using limit of {query.similarity_top_k}")
 
         # execute query
         query_result = query_builder.do()
 
         # parse results
         parsed_result = parse_get_response(query_result)
         entries = parsed_result[self.index_name]
```

### Comparing `llama_index_vector_stores_weaviate-0.1.4/llama_index/vector_stores/weaviate/utils.py` & `llama_index_vector_stores_weaviate-0.1.5/llama_index/vector_stores/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_weaviate-0.1.4/pyproject.toml` & `llama_index_vector_stores_weaviate-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores weaviate integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-weaviate"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 weaviate-client = "^3.26.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_weaviate-0.1.4/PKG-INFO` & `llama_index_vector_stores_weaviate-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-weaviate
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index vector_stores weaviate integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

