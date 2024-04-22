# Comparing `tmp/llama_index_packs_code_hierarchy-0.1.4.tar.gz` & `tmp/llama_index_packs_code_hierarchy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_code_hierarchy-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_packs_code_hierarchy-0.1.5.tar", max compression
```

## Comparing `llama_index_packs_code_hierarchy-0.1.4.tar` & `llama_index_packs_code_hierarchy-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4966 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/README.md
--rw-r--r--   0        0        0       17 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/BUILD
--rw-r--r--   0        0        0      371 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/__init__.py
--rw-r--r--   0        0        0     1473 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/base.py
--rw-r--r--   0        0        0    33737 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/code_hierarchy.py
--rw-r--r--   0        0        0     6099 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/query_engine.py
--rw-r--r--   0        0        0     1438 2024-04-19 17:35:42.346231 llama_index_packs_code_hierarchy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 llama_index_packs_code_hierarchy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4966 2024-04-22 02:40:21.696867 llama_index_packs_code_hierarchy-0.1.5/README.md
+-rw-r--r--   0        0        0       17 2024-04-22 02:40:21.700867 llama_index_packs_code_hierarchy-0.1.5/llama_index/packs/code_hierarchy/BUILD
+-rw-r--r--   0        0        0      371 2024-04-22 02:40:21.700867 llama_index_packs_code_hierarchy-0.1.5/llama_index/packs/code_hierarchy/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-22 02:40:21.700867 llama_index_packs_code_hierarchy-0.1.5/llama_index/packs/code_hierarchy/base.py
+-rw-r--r--   0        0        0    33737 2024-04-22 02:40:21.700867 llama_index_packs_code_hierarchy-0.1.5/llama_index/packs/code_hierarchy/code_hierarchy.py
+-rw-r--r--   0        0        0     6163 2024-04-22 02:40:21.700867 llama_index_packs_code_hierarchy-0.1.5/llama_index/packs/code_hierarchy/query_engine.py
+-rw-r--r--   0        0        0     1438 2024-04-22 02:40:21.700867 llama_index_packs_code_hierarchy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 llama_index_packs_code_hierarchy-0.1.5/PKG-INFO
```

### Comparing `llama_index_packs_code_hierarchy-0.1.4/README.md` & `llama_index_packs_code_hierarchy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/base.py` & `llama_index_packs_code_hierarchy-0.1.5/llama_index/packs/code_hierarchy/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/code_hierarchy.py` & `llama_index_packs_code_hierarchy-0.1.5/llama_index/packs/code_hierarchy/code_hierarchy.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_code_hierarchy-0.1.4/llama_index/packs/code_hierarchy/query_engine.py` & `llama_index_packs_code_hierarchy-0.1.5/llama_index/packs/code_hierarchy/query_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,18 @@
                             return parent
             return None
 
         if query in self.node_dict:
             return self.node_dict[query][1]
 
         kvs = get_all_dict_recursive(self.repo_map[0])
+        if query not in kvs:
+            return None
         parent_query = query
-        while parent_query not in kvs:
+        while parent_query not in self.node_dict:
             parent_query = get_parent_dict_recursive(self.repo_map[0], parent_query)
             if parent_query is None:
                 return "None"
 
         # After finding the parent_query, ensure it's in self.node_dict before accessing
         if parent_query in self.node_dict:
             return self.node_dict[parent_query][1]
```

### Comparing `llama_index_packs_code_hierarchy-0.1.4/pyproject.toml` & `llama_index_packs_code_hierarchy-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Ryan Peach <rgpeach10@gmail.com>"]
 description = "A node parser which can create a hierarchy of all code scopes in a directory."
 keywords = ["c", "code", "cpp", "hierarchy", "html", "javascript", "python", "repo", "typescript"]
 license = "MIT"
 maintainers = ["ryanpeach"]
 name = "llama-index-packs-code-hierarchy"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 llama-index-core = "^0.10.1"
 tree-sitter-languages = "^1.8.0"
 tree-sitter = "^0.20.2"
 llama-index-agent-openai = ">=0.1.5"
```

### Comparing `llama_index_packs_code_hierarchy-0.1.4/PKG-INFO` & `llama_index_packs_code_hierarchy-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-code-hierarchy
-Version: 0.1.4
+Version: 0.1.5
 Summary: A node parser which can create a hierarchy of all code scopes in a directory.
 License: MIT
 Keywords: c,code,cpp,hierarchy,html,javascript,python,repo,typescript
 Author: Ryan Peach
 Author-email: rgpeach10@gmail.com
 Maintainer: ryanpeach
 Requires-Python: >=3.8.1,<3.12
```

