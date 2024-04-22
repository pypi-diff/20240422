# Comparing `tmp/text_lloom-0.7.tar.gz` & `tmp/text_lloom-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_lloom-0.7.tar", max compression
+gzip compressed data, was "text_lloom-0.7.1.tar", max compression
```

## Comparing `text_lloom-0.7.tar` & `text_lloom-0.7.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.7/README.md
--rw-r--r--   0        0        0      570 2024-04-18 14:07:03.067251 text_lloom-0.7/pyproject.toml
--rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.7/src/text_lloom/__init__.py
--rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.7/src/text_lloom/concept.py
--rw-r--r--   0        0        0    57603 2024-04-18 04:35:08.254531 text_lloom-0.7/src/text_lloom/concept_induction.py
--rw-r--r--   0        0        0    12290 2024-03-08 09:30:26.443347 text_lloom-0.7/src/text_lloom/llm.py
--rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.7/src/text_lloom/prompts.py
--rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.7/src/text_lloom/static/index.css
--rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.7/src/text_lloom/static/index.js
--rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.7/src/text_lloom/static/index_select.css
--rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.7/src/text_lloom/static/index_select.js
--rw-r--r--   0        0        0    29258 2024-04-18 14:05:54.296440 text_lloom-0.7/src/text_lloom/workbench.py
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 text_lloom-0.7/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.7.1/README.md
+-rw-r--r--   0        0        0      546 2024-04-22 09:07:17.168243 text_lloom-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.7.1/src/text_lloom/__init__.py
+-rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.7.1/src/text_lloom/concept.py
+-rw-r--r--   0        0        0    57605 2024-04-22 08:37:58.216130 text_lloom-0.7.1/src/text_lloom/concept_induction.py
+-rw-r--r--   0        0        0     8078 2024-04-22 08:18:42.690605 text_lloom-0.7.1/src/text_lloom/llm.py
+-rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.7.1/src/text_lloom/prompts.py
+-rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.7.1/src/text_lloom/static/index.css
+-rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.7.1/src/text_lloom/static/index.js
+-rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.7.1/src/text_lloom/static/index_select.css
+-rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.7.1/src/text_lloom/static/index_select.js
+-rw-r--r--   0        0        0    29130 2024-04-22 07:18:08.926897 text_lloom-0.7.1/src/text_lloom/workbench.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 text_lloom-0.7.1/PKG-INFO
```

### Comparing `text_lloom-0.7/src/text_lloom/__init__.py` & `text_lloom-0.7.1/src/text_lloom/__init__.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7/src/text_lloom/concept.py` & `text_lloom-0.7.1/src/text_lloom/concept.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7/src/text_lloom/concept_induction.py` & `text_lloom-0.7.1/src/text_lloom/concept_induction.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,27 @@
 import textwrap
 from itertools import chain
 import pickle
 import ipywidgets as widgets
 import re
 
 # Clustering
-from bertopic import BERTopic
-from bertopic.backend import OpenAIBackend
 from hdbscan import HDBSCAN
+import umap
 
 # Local imports
 if __package__ is None or __package__ == '':
     # uses current directory visibility
-    from llm import multi_query_gpt_wrapper, calc_cost_by_tokens
+    from llm import multi_query_gpt_wrapper, calc_cost_by_tokens, get_embeddings
     from prompts import *
     from concept import Concept
     from __init__ import MatrixWidget, ConceptSelectWidget
 else:
     # uses current package visibility
-    from .llm import multi_query_gpt_wrapper, calc_cost_by_tokens
+    from .llm import multi_query_gpt_wrapper, calc_cost_by_tokens, get_embeddings
     from .prompts import *
     from .concept import Concept
     from .__init__ import MatrixWidget, ConceptSelectWidget
 
 # CONSTANTS ================================
 NAN_SCORE = 0  # Numerical score to use in place of NaN values for matrix viz
 OUTLIER_CRITERIA = "Did the example not match any of the above concepts?"
@@ -70,30 +69,34 @@
 
 def pretty_print_dict_list(d_list):
     # Print all dictionaries in a list of dictionaries
     return "\n\t" + "\n\t".join([pretty_print_dict(d) for d in d_list])
 
 def cluster_helper(in_df, doc_col, doc_id_col, min_cluster_size, cluster_id_col, embed_model_name):
     # OpenAI embeddings with HDBSCAN clustering
-    embedding_model = OpenAIBackend(embed_model_name)
+    id_vals = in_df[doc_id_col].tolist()
+    text_vals = in_df[doc_col].tolist()
 
-    hdbscan_model = HDBSCAN(
+    embeddings = get_embeddings(embed_model_name, text_vals)
+    umap_model = umap.UMAP(
+        n_neighbors=15,
+        n_components=5,
+        min_dist=0.0,
+        metric='cosine',
+    )
+    umap_embeddings = umap_model.fit_transform(embeddings)
+    hdb = HDBSCAN(
         min_cluster_size=min_cluster_size, 
         metric='euclidean', 
         cluster_selection_method='leaf', 
         prediction_data=True
     )
-    topic_model = BERTopic(
-        embedding_model=embedding_model, 
-        hdbscan_model=hdbscan_model
-    )
+    res = hdb.fit(umap_embeddings)
+    clusters = res.labels_
 
-    id_vals = in_df[doc_id_col].tolist()
-    text_vals = in_df[doc_col].tolist()
-    clusters, probs = topic_model.fit_transform(text_vals)
     rows = list(zip(id_vals, text_vals, clusters)) # id_col, text_col, cluster_id_col
     cluster_df = pd.DataFrame(rows, columns=[doc_id_col, doc_col, cluster_id_col])
     cluster_df = cluster_df.sort_values(by=[cluster_id_col])
     
     return cluster_df
 
 def save_progress(sess, df, step_name, start, res, model_name, debug=False):
@@ -120,16 +123,16 @@
         sess.time[k] = elapsed
 
 def calc_cost(results, model_name, step_name, sess, debug=False):
     # Calculate cost with API results and model name
     if results is None:
         return
     # Cost estimation
-    in_tokens = np.sum([res.llm_output["token_usage"]["prompt_tokens"] for res in results])
-    out_tokens = np.sum([res.llm_output["token_usage"]["completion_tokens"] for res in results])
+    in_tokens = np.sum([res.usage.prompt_tokens for res in results])
+    out_tokens = np.sum([res.usage.completion_tokens for res in results])
     in_token_cost, out_token_cost = calc_cost_by_tokens(model_name, in_tokens, out_tokens)
     total_cost = in_token_cost + out_token_cost
     if debug:
         print(f"\nTotal: {total_cost} | In: {in_token_cost} | Out: {out_token_cost}")
     if sess is not None:
         # Save to session if provided
         sess.tokens["in_tokens"].append(in_tokens)
@@ -1175,15 +1178,15 @@
     df_bullets[doc_id_col] = df_bullets[doc_id_col].astype(str)
     df_bullets = df_bullets.groupby(doc_id_col).agg(lambda x: list(x)).reset_index()
 
     # Rationale df
     rationale_col = "score rationale"
     highlight_col = "highlight"
     rationale_df = score_df[[doc_id_col, "concept_name", "rationale", highlight_col]]
-    rationale_df.rename(columns={"rationale": rationale_col}, inplace=True)
+    rationale_df = rationale_df.rename(columns={"rationale": rationale_col})
     rationale_df[doc_id_col] = rationale_df[doc_id_col].astype(str)
 
     # Prep data for each group
     for group_name, group_filtering in groupings.items():
         filter_x = group_filtering["x"]
         filter_func = group_filtering["fn"]
         filter_args = group_filtering["args"]
```

### Comparing `text_lloom-0.7/src/text_lloom/prompts.py` & `text_lloom-0.7.1/src/text_lloom/prompts.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7/src/text_lloom/static/index.css` & `text_lloom-0.7.1/src/text_lloom/static/index.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7/src/text_lloom/static/index.js` & `text_lloom-0.7.1/src/text_lloom/static/index.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7/src/text_lloom/static/index_select.css` & `text_lloom-0.7.1/src/text_lloom/static/index_select.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7/src/text_lloom/static/index_select.js` & `text_lloom-0.7.1/src/text_lloom/static/index_select.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.7/src/text_lloom/workbench.py` & `text_lloom-0.7.1/src/text_lloom/workbench.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # Concept induction session functions
 # =================================================
 
 # Imports
 import time
 import pandas as pd
-import ipywidgets as widgets
 import random
 from nltk.tokenize import sent_tokenize
 import os
-import openai
 from yaspin import yaspin
 import base64
 import requests
 
 
 # Local imports
 if __package__ is None or __package__ == '':
@@ -64,19 +62,17 @@
         self.time = {}  # Stores time required for each step
         self.cost = {}  # Stores cost incurred by each step
         self.tokens = {
             "in_tokens": [],
             "out_tokens": [],
         }
 
-        # Set up API key
+        # Check for API key
         if "OPENAI_API_KEY" not in os.environ:
             raise Exception("API key not found. Please set the OPENAI_API_KEY environment variable by running: `os.environ['OPENAI_API_KEY'] = 'your_key'`")
-        else:
-            openai.api_key = os.environ["OPENAI_API_KEY"]
     
     # Preprocesses input dataframe
     def preprocess_df(self, df):
         # Handle missing ID column
         if self.doc_id_col is None:
             print("No `id_col` provided. Created an ID column named 'id'.")
             df = df.copy()
@@ -141,15 +137,15 @@
     def print_step_name(self, step_name):
         # Print step name (with blue highlighting)
         format_step_name = f"{self.highlight_txt(step_name, color='blue')}"
         print(f"\n\n{format_step_name}")
 
     def spinner_wrapper(self):
         # Wrapper for loading spinner
-        return yaspin(text="Loading", color="yellow")
+        return yaspin(text="Loading")
 
     # Estimate cost of generation for the given params
     def estimate_gen_cost(self, params=None, verbose=False):
         if params is None:
             params = self.auto_suggest_parameters()
             print(f"No parameters provided, so using auto-suggested parameters: {params}")
         # Conservative estimates based on empirical data
```

### Comparing `text_lloom-0.7/PKG-INFO` & `text_lloom-0.7.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: text_lloom
-Version: 0.7
+Version: 0.7.1
 Summary: Concept Induction to analyze unstructured text
 Author: Michelle Lam
 Author-email: mlam4@cs.stanford.edu
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anywidget (>=0.9.7,<0.10.0)
-Requires-Dist: bertopic (>=0.16.0,<0.17.0)
-Requires-Dist: google-generativeai (>=0.3.2,<0.4.0)
 Requires-Dist: hdbscan (>=0.8.33,<0.9.0)
 Requires-Dist: ipywidgets (>=8.1.2,<9.0.0)
 Requires-Dist: jupyterlab_widgets (>=3.0.10,<4.0.0)
 Requires-Dist: langchain (==0.0.271)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
-Requires-Dist: openai (==0.28)
+Requires-Dist: openai (>=1.23.1,<2.0.0)
 Requires-Dist: pathos (>=0.3.2,<0.4.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
+Requires-Dist: umap-learn (>=0.5.5,<0.6.0)
 Requires-Dist: yaspin (>=3.0.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 Directory for the LLooM python package
```

