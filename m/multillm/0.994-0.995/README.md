# Comparing `tmp/multillm-0.994.tar.gz` & `tmp/multillm-0.995.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multillm-0.994.tar", last modified: Sun Apr 21 20:00:28 2024, max compression
+gzip compressed data, was "multillm-0.995.tar", last modified: Sun Apr 21 21:59:50 2024, max compression
```

## Comparing `multillm-0.994.tar` & `multillm-0.995.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 20:00:28.538675 multillm-0.994/
--rw-r--r--   0 sandeep    (502) staff       (20)     1090 2024-04-19 07:14:31.000000 multillm-0.994/LICENSE
--rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-21 20:00:28.537978 multillm-0.994/PKG-INFO
--rw-r--r--   0 sandeep    (502) staff       (20)    23438 2024-04-19 07:14:31.000000 multillm-0.994/README.md
--rw-r--r--   0 sandeep    (502) staff       (20)      154 2024-04-19 07:14:31.000000 multillm-0.994/README.txt
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 20:00:28.524150 multillm-0.994/multillm/
--rw-r--r--   0 sandeep    (502) staff       (20)     2646 2024-04-19 07:14:31.000000 multillm-0.994/multillm/Action.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3335 2024-04-19 07:14:31.000000 multillm-0.994/multillm/BaseLLM.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3459 2024-04-19 07:14:31.000000 multillm-0.994/multillm/DynamicClass.py
--rw-r--r--   0 sandeep    (502) staff       (20)     9433 2024-04-19 07:14:31.000000 multillm-0.994/multillm/MultiLLM.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3105 2024-04-19 07:14:31.000000 multillm-0.994/multillm/Prompt.py
--rw-r--r--   0 sandeep    (502) staff       (20)     2167 2024-04-19 07:14:31.000000 multillm-0.994/multillm/Rank.py
--rw-r--r--   0 sandeep    (502) staff       (20)     1209 2024-04-19 07:14:31.000000 multillm-0.994/multillm/Redis.py
--rw-r--r--   0 sandeep    (502) staff       (20)       26 2024-04-19 07:14:31.000000 multillm-0.994/multillm/__init__.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5551 2024-04-19 07:14:31.000000 multillm-0.994/multillm/example.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3491 2024-04-19 07:14:31.000000 multillm-0.994/multillm/example_rank_callback.py
--rw-r--r--   0 sandeep    (502) staff       (20)    12433 2024-04-19 07:14:31.000000 multillm-0.994/multillm/example_rank_callback3_scaled.py
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 20:00:28.536566 multillm-0.994/multillm/models/
--rw-r--r--   0 sandeep    (502) staff       (20)     4022 2024-04-19 07:14:31.000000 multillm-0.994/multillm/models/Codegen.py
--rw-r--r--   0 sandeep    (502) staff       (20)     3780 2024-04-19 07:14:31.000000 multillm-0.994/multillm/models/Dolly.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4065 2024-04-19 07:14:31.000000 multillm-0.994/multillm/models/GPT.py
--rw-r--r--   0 sandeep    (502) staff       (20)     2519 2024-04-19 07:14:31.000000 multillm-0.994/multillm/models/GPTJ.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5326 2024-04-19 07:14:31.000000 multillm-0.994/multillm/models/LLAMA2.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5348 2024-04-21 19:58:55.000000 multillm-0.994/multillm/models/LLAMA3.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4298 2024-04-19 07:14:31.000000 multillm-0.994/multillm/models/Mistral.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4474 2024-04-19 07:14:31.000000 multillm-0.994/multillm/models/Zephyr.py
--rw-r--r--   0 sandeep    (502) staff       (20)     6399 2024-04-19 07:14:31.000000 multillm-0.994/multillm/models/bard.py
--rw-r--r--   0 sandeep    (502) staff       (20)     5513 2024-04-19 07:14:31.000000 multillm-0.994/multillm/models/claude.py
--rw-r--r--   0 sandeep    (502) staff       (20)     4026 2024-04-19 07:14:31.000000 multillm-0.994/multillm/models/gemini.py
--rw-r--r--   0 sandeep    (502) staff       (20)    12554 2024-04-19 07:14:31.000000 multillm-0.994/multillm/rank_callback.py
-drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 20:00:28.537243 multillm-0.994/multillm.egg-info/
--rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-21 20:00:28.000000 multillm-0.994/multillm.egg-info/PKG-INFO
--rw-r--r--   0 sandeep    (502) staff       (20)      768 2024-04-21 20:00:28.000000 multillm-0.994/multillm.egg-info/SOURCES.txt
--rw-r--r--   0 sandeep    (502) staff       (20)        1 2024-04-21 20:00:28.000000 multillm-0.994/multillm.egg-info/dependency_links.txt
--rw-r--r--   0 sandeep    (502) staff       (20)       51 2024-04-21 20:00:28.000000 multillm-0.994/multillm.egg-info/entry_points.txt
--rw-r--r--   0 sandeep    (502) staff       (20)        9 2024-04-21 20:00:28.000000 multillm-0.994/multillm.egg-info/top_level.txt
--rw-r--r--   0 sandeep    (502) staff       (20)      946 2024-04-21 19:59:05.000000 multillm-0.994/pyproject.toml
--rw-r--r--   0 sandeep    (502) staff       (20)       38 2024-04-21 20:00:28.538791 multillm-0.994/setup.cfg
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 21:59:50.805134 multillm-0.995/
+-rw-r--r--   0 sandeep    (502) staff       (20)     1090 2024-04-19 07:14:31.000000 multillm-0.995/LICENSE
+-rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-21 21:59:50.804151 multillm-0.995/PKG-INFO
+-rw-r--r--   0 sandeep    (502) staff       (20)    23438 2024-04-19 07:14:31.000000 multillm-0.995/README.md
+-rw-r--r--   0 sandeep    (502) staff       (20)      154 2024-04-19 07:14:31.000000 multillm-0.995/README.txt
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 21:59:50.781892 multillm-0.995/multillm/
+-rw-r--r--   0 sandeep    (502) staff       (20)     2646 2024-04-19 07:14:31.000000 multillm-0.995/multillm/Action.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3335 2024-04-19 07:14:31.000000 multillm-0.995/multillm/BaseLLM.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3459 2024-04-19 07:14:31.000000 multillm-0.995/multillm/DynamicClass.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     9433 2024-04-19 07:14:31.000000 multillm-0.995/multillm/MultiLLM.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3105 2024-04-19 07:14:31.000000 multillm-0.995/multillm/Prompt.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     2167 2024-04-19 07:14:31.000000 multillm-0.995/multillm/Rank.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     1209 2024-04-19 07:14:31.000000 multillm-0.995/multillm/Redis.py
+-rw-r--r--   0 sandeep    (502) staff       (20)       26 2024-04-19 07:14:31.000000 multillm-0.995/multillm/__init__.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5551 2024-04-19 07:14:31.000000 multillm-0.995/multillm/example.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3491 2024-04-19 07:14:31.000000 multillm-0.995/multillm/example_rank_callback.py
+-rw-r--r--   0 sandeep    (502) staff       (20)    12433 2024-04-19 07:14:31.000000 multillm-0.995/multillm/example_rank_callback3_scaled.py
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 21:59:50.802718 multillm-0.995/multillm/models/
+-rw-r--r--   0 sandeep    (502) staff       (20)     4022 2024-04-19 07:14:31.000000 multillm-0.995/multillm/models/Codegen.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     3780 2024-04-19 07:14:31.000000 multillm-0.995/multillm/models/Dolly.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4065 2024-04-19 07:14:31.000000 multillm-0.995/multillm/models/GPT.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     2519 2024-04-19 07:14:31.000000 multillm-0.995/multillm/models/GPTJ.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5326 2024-04-19 07:14:31.000000 multillm-0.995/multillm/models/LLAMA2.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5348 2024-04-21 21:58:31.000000 multillm-0.995/multillm/models/LLAMA3.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4298 2024-04-19 07:14:31.000000 multillm-0.995/multillm/models/Mistral.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4474 2024-04-19 07:14:31.000000 multillm-0.995/multillm/models/Zephyr.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     6399 2024-04-19 07:14:31.000000 multillm-0.995/multillm/models/bard.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     5513 2024-04-19 07:14:31.000000 multillm-0.995/multillm/models/claude.py
+-rw-r--r--   0 sandeep    (502) staff       (20)     4026 2024-04-19 07:14:31.000000 multillm-0.995/multillm/models/gemini.py
+-rw-r--r--   0 sandeep    (502) staff       (20)    12554 2024-04-19 07:14:31.000000 multillm-0.995/multillm/rank_callback.py
+drwxr-xr-x   0 sandeep    (502) staff       (20)        0 2024-04-21 21:59:50.803524 multillm-0.995/multillm.egg-info/
+-rw-r--r--   0 sandeep    (502) staff       (20)    23984 2024-04-21 21:59:50.000000 multillm-0.995/multillm.egg-info/PKG-INFO
+-rw-r--r--   0 sandeep    (502) staff       (20)      768 2024-04-21 21:59:50.000000 multillm-0.995/multillm.egg-info/SOURCES.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)        1 2024-04-21 21:59:50.000000 multillm-0.995/multillm.egg-info/dependency_links.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)       51 2024-04-21 21:59:50.000000 multillm-0.995/multillm.egg-info/entry_points.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)        9 2024-04-21 21:59:50.000000 multillm-0.995/multillm.egg-info/top_level.txt
+-rw-r--r--   0 sandeep    (502) staff       (20)      946 2024-04-21 21:58:42.000000 multillm-0.995/pyproject.toml
+-rw-r--r--   0 sandeep    (502) staff       (20)       38 2024-04-21 21:59:50.805274 multillm-0.995/setup.cfg
```

### Comparing `multillm-0.994/LICENSE` & `multillm-0.995/LICENSE`

 * *Files identical despite different names*

### Comparing `multillm-0.994/PKG-INFO` & `multillm-0.995/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multillm
-Version: 0.994
+Version: 0.995
 Summary: VerifAI MultiLLM: A module to invoke multiple LLMs concurrently and rank their results
 Author-email: VerifAI Inc <hello@verifai.ai>
 Project-URL: Homepage, https://github.com/verifai/multiLLM
 Project-URL: Bug Tracker, https://github.com/verifai/multiLLM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multillm-0.994/README.md` & `multillm-0.995/README.md`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/Action.py` & `multillm-0.995/multillm/Action.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/BaseLLM.py` & `multillm-0.995/multillm/BaseLLM.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/DynamicClass.py` & `multillm-0.995/multillm/DynamicClass.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/MultiLLM.py` & `multillm-0.995/multillm/MultiLLM.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/Prompt.py` & `multillm-0.995/multillm/Prompt.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/Rank.py` & `multillm-0.995/multillm/Rank.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/Redis.py` & `multillm-0.995/multillm/Redis.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/example.py` & `multillm-0.995/multillm/example.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/example_rank_callback.py` & `multillm-0.995/multillm/example_rank_callback.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/example_rank_callback3_scaled.py` & `multillm-0.995/multillm/example_rank_callback3_scaled.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/models/Codegen.py` & `multillm-0.995/multillm/models/Codegen.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/models/Dolly.py` & `multillm-0.995/multillm/models/Dolly.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/models/GPT.py` & `multillm-0.995/multillm/models/GPT.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/models/GPTJ.py` & `multillm-0.995/multillm/models/GPTJ.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/models/LLAMA2.py` & `multillm-0.995/multillm/models/LLAMA2.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/models/LLAMA3.py` & `multillm-0.995/multillm/models/LLAMA3.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def get_response(self, prompt: Prompt, taskid=None, convid = None):
         
         
         """Predict using a Large Language Model."""
         project_id = "llama2"
         location = "us-central1"
         #url = "http://34.221.191.141/llama2/predict"
-        url = "http://34.216.129.113/llama3-vllm"
+        url = "http://18.237.205.198/llama3-vllm"
 
         
         """ Get credentials file set in the config, and set appropriate variables for your model """
 
         try:
             """ Call API """
 
@@ -100,15 +100,15 @@
             #values = {'question':  prmpt}
 
             """ vllm server
         http://54.190.15.83/llama2-vllm     -H "Content-Type: application/json"
            -d '{ "model": "meta-llama/Meta-Llama-3-8B-Instruct-chat-hf", "prompt": "write verilog code for a 4 port 16 entry FIFO controllers", "max_tokens":4096}'
 
             """
-            values = {'prompt':  prmpt, "model" : "meta-llama/Meta-Llama-3-8B-Instruct", "max_tokens":4000}
+            values = {'prompt':  prmpt, "model" : "meta-llama/Meta-Llama-3-8B-Instruct", "max_tokens":3900}
       
             resp = requests.post(url, data=json.dumps(values),headers=headers)
             #print("LLAMA2 Response: {0}" .format(resp.text))
             data = resp.json()
 
             """ GPT Style Response from vLLM server
               {"id":"cmpl-8282910626ff42518fb0e17f01c412f7",
```

### Comparing `multillm-0.994/multillm/models/Mistral.py` & `multillm-0.995/multillm/models/Mistral.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/models/Zephyr.py` & `multillm-0.995/multillm/models/Zephyr.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/models/bard.py` & `multillm-0.995/multillm/models/bard.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/models/claude.py` & `multillm-0.995/multillm/models/claude.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/models/gemini.py` & `multillm-0.995/multillm/models/gemini.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm/rank_callback.py` & `multillm-0.995/multillm/rank_callback.py`

 * *Files identical despite different names*

### Comparing `multillm-0.994/multillm.egg-info/PKG-INFO` & `multillm-0.995/multillm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multillm
-Version: 0.994
+Version: 0.995
 Summary: VerifAI MultiLLM: A module to invoke multiple LLMs concurrently and rank their results
 Author-email: VerifAI Inc <hello@verifai.ai>
 Project-URL: Homepage, https://github.com/verifai/multiLLM
 Project-URL: Bug Tracker, https://github.com/verifai/multiLLM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multillm-0.994/multillm.egg-info/SOURCES.txt` & `multillm-0.995/multillm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multillm-0.994/pyproject.toml` & `multillm-0.995/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "multillm"
-version = "0.994"
+version = "0.995"
 authors = [
   { name="VerifAI Inc", email="hello@verifai.ai" },
 ]
 
 description = "VerifAI MultiLLM: A module to invoke multiple LLMs concurrently and rank their results"
 readme = "README.md"
 requires-python = ">=3.8"
```

