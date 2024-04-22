# Comparing `tmp/strictjson-4.0.0.tar.gz` & `tmp/strictjson-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strictjson-4.0.0.tar", last modified: Mon Mar  4 02:43:23 2024, max compression
+gzip compressed data, was "strictjson-4.0.1.tar", last modified: Mon Apr 22 03:29:13 2024, max compression
```

## Comparing `strictjson-4.0.0.tar` & `strictjson-4.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-03-04 02:43:23.916635 strictjson-4.0.0/
--rw-r--r--   0 tanchongmin   (501) staff       (20)     1073 2024-01-05 08:31:13.000000 strictjson-4.0.0/LICENSE
--rw-r--r--   0 tanchongmin   (501) staff       (20)    15759 2024-03-04 02:43:23.915169 strictjson-4.0.0/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)    15150 2024-03-04 02:42:12.000000 strictjson-4.0.0/README.md
--rw-r--r--   0 tanchongmin   (501) staff       (20)      675 2024-03-04 02:39:44.000000 strictjson-4.0.0/pyproject.toml
--rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-03-04 02:43:23.916735 strictjson-4.0.0/setup.cfg
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-03-04 02:43:23.911022 strictjson-4.0.0/strictjson/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      171 2024-02-26 00:45:10.000000 strictjson-4.0.0/strictjson/__init__.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    31146 2024-03-03 15:33:26.000000 strictjson-4.0.0/strictjson/agent.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    35982 2024-03-03 13:10:12.000000 strictjson-4.0.0/strictjson/base.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-03-04 02:43:23.914416 strictjson-4.0.0/strictjson.egg-info/
--rw-r--r--   0 tanchongmin   (501) staff       (20)    15759 2024-03-04 02:43:23.000000 strictjson-4.0.0/strictjson.egg-info/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-03-04 02:43:23.000000 strictjson-4.0.0/strictjson.egg-info/SOURCES.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-03-04 02:43:23.000000 strictjson-4.0.0/strictjson.egg-info/dependency_links.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       14 2024-03-04 02:43:23.000000 strictjson-4.0.0/strictjson.egg-info/requires.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       11 2024-03-04 02:43:23.000000 strictjson-4.0.0/strictjson.egg-info/top_level.txt
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:29:13.524657 strictjson-4.0.1/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)     1073 2024-01-05 08:31:13.000000 strictjson-4.0.1/LICENSE
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    15786 2024-04-22 03:29:13.523885 strictjson-4.0.1/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    15150 2024-04-22 02:39:25.000000 strictjson-4.0.1/README.md
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      690 2024-04-22 02:37:17.000000 strictjson-4.0.1/pyproject.toml
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-04-22 03:29:13.524781 strictjson-4.0.1/setup.cfg
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:29:13.520788 strictjson-4.0.1/strictjson/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      171 2024-02-26 00:45:10.000000 strictjson-4.0.1/strictjson/__init__.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    33533 2024-04-22 02:45:45.000000 strictjson-4.0.1/strictjson/agent.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    36879 2024-04-22 03:03:40.000000 strictjson-4.0.1/strictjson/base.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:29:13.523335 strictjson-4.0.1/strictjson.egg-info/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    15786 2024-04-22 03:29:13.000000 strictjson-4.0.1/strictjson.egg-info/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-04-22 03:29:13.000000 strictjson-4.0.1/strictjson.egg-info/SOURCES.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-04-22 03:29:13.000000 strictjson-4.0.1/strictjson.egg-info/dependency_links.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       26 2024-04-22 03:29:13.000000 strictjson-4.0.1/strictjson.egg-info/requires.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       11 2024-04-22 03:29:13.000000 strictjson-4.0.1/strictjson.egg-info/top_level.txt
```

### Comparing `strictjson-4.0.0/LICENSE` & `strictjson-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strictjson-4.0.0/PKG-INFO` & `strictjson-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: strictjson
-Version: 4.0.0
+Version: 4.0.1
 Summary: A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/tanchongmin/strictjson
 Project-URL: Issues, https://github.com/tanchongmin/strictjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.3.6
+Requires-Dist: openai>=1.3.6
+Requires-Dist: dill>=0.3.7
 
-# Strict JSON v4.0.0
+# Strict JSON v4.0.1
 [UPDATE]: For Agentic Framework, do check out TaskGen (the official Agentic Framework building on StrictJSON). This will make the StrictJSON repo neater and this github will focus on using StrictJSON for LLM Output Parsing
 - https://github.com/simbianai/taskgen
 
 ### A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve
 - Works for JSON outputs with multiple ' or " or { or } or \ or unmatched braces/brackets that may break a json.loads()
 
 ### Base Functionalities (see Tutorial.ipynb)
```

### Comparing `strictjson-4.0.0/README.md` & `strictjson-4.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Strict JSON v4.0.0
+# Strict JSON v4.0.1
 [UPDATE]: For Agentic Framework, do check out TaskGen (the official Agentic Framework building on StrictJSON). This will make the StrictJSON repo neater and this github will focus on using StrictJSON for LLM Output Parsing
 - https://github.com/simbianai/taskgen
 
 ### A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve
 - Works for JSON outputs with multiple ' or " or { or } or \ or unmatched braces/brackets that may break a json.loads()
 
 ### Base Functionalities (see Tutorial.ipynb)
```

### Comparing `strictjson-4.0.0/pyproject.toml` & `strictjson-4.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "strictjson"
-version = "4.0.0"
+version = "4.0.1"
 authors = [
   { name="John Tan Chong Min", email="tanchongmin@gmail.com" },
 ]
 description = "A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["openai==1.3.6"]
+dependencies = ["openai>=1.3.6", "dill>=0.3.7"]
 
 [project.urls]
 Homepage = "https://github.com/tanchongmin/strictjson"
 Issues = "https://github.com/tanchongmin/strictjson/issues"
```

### Comparing `strictjson-4.0.0/strictjson/agent.py` & `strictjson-4.0.1/strictjson/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import heapq
 import openai
 from openai import OpenAI
 import numpy as np
 import copy
+import dill as pickle
 from .base import *
 
 ### Helper Functions
 def top_k_index(lst, k):
     ''' Given a list lst, find the top k indices corresponding to the top k values '''
     indexed_lst = list(enumerate(lst))
     top_k_values_with_indices = heapq.nlargest(k, indexed_lst, key=lambda x: x[1])
@@ -31,14 +32,17 @@
         self.database = database
             
     def __call__(self, query, key) -> float:
         ''' Takes in a query and a key and outputs a similarity score 
         Inputs:
         query: Str. The query you want to evaluate
         key: Str. The key you want to evaluate'''
+        # ensure they are both str
+        query = str(query)
+        key = str(key)
      
         # defaults to OpenAI if ranking_fn is not provided
         if self.ranking_fn is None:
             client = OpenAI()
             if query in self.database:
                 query_embedding = self.database[query]
             else:
@@ -63,23 +67,25 @@
     - Inputs:
         - `memory`: List. Default: Empty List. The list containing the memory items
         - `top_k`: Int. Default: 3. The number of memory list items to retrieve
         - `mapper`: Function. Maps the memory item to another form for comparison by ranker or LLM. Default: `lambda x: x`
             - Example mapping: `lambda x: x.fn_description` (If x is a Class and the string you want to compare for similarity is the fn_description attribute of that class)
         - `approach`: str. Either `retrieve_by_ranker` or `retrieve_by_llm` to retrieve memory items
             - Ranker is faster and cheaper as it compares via embeddings, but are inferior to LLM-based methods for contextual information
+        - `llm`: Function. The llm to use for `strict_json` llm retriever
         - `ranker`: `Ranker`. The Ranker which defines a similarity score between a query and a key. Default: OpenAI `text-embedding-3-small` model. 
             - Can be replaced with a function which returns similarity score from 0 to 1 when given a query and key
      '''
-    def __init__(self, memory: list = [], top_k: int = 3, mapper = lambda x: x, approach = 'retrieve_by_ranker', ranker = Ranker()):
+    def __init__(self, memory: list = [], top_k: int = 3, mapper = lambda x: x, approach = 'retrieve_by_ranker', llm = None, ranker = Ranker()):
         self.memory = memory
         self.top_k = top_k
         self.mapper = mapper
         self.approach = approach
         self.ranker = ranker
+        self.llm = llm
         
     def retrieve(self, task: str) -> list:
         ''' Performs retrieval of top_k similar memories according to approach stated '''
         if self.approach == 'retrieve_by_ranker':
             return self.retrieve_by_ranker(task)
         else:
             return self.retrieve_by_llm(task)
@@ -91,15 +97,16 @@
         top_k_indices = top_k_index(memory_score, self.top_k)
         return [self.memory[index] for index in top_k_indices]
     
     def retrieve_by_llm(self, task: str) -> list:
         ''' Performs retrieval via LLMs 
         Returns the key list as well as the value list '''
         res = strict_json(f'You are to output the top {self.top_k} most similar list items in Memory that meet this description: {task}\nMemory: {[f"{i}. {self.mapper(mem)}" for i, mem in enumerate(self.memory)]}', '', 
-              output_format = {f"top_{self.top_k}_list": f"Indices of top {self.top_k} most similar list items in Memory, type: list[int]"})
+              output_format = {f"top_{self.top_k}_list": f"Indices of top {self.top_k} most similar list items in Memory, type: list[int]"},
+              llm = self.llm)
         top_k_indices = res[f'top_{self.top_k}_list']
         return [self.memory[index] for index in top_k_indices]
     
     def append(self, new_memory):
         ''' Adds a new_memory'''
         self.memory.append(new_memory)
         
@@ -123,17 +130,19 @@
     
 class Agent:
     def __init__(self, agent_name: str = 'Helpful Assistant',
                  agent_description: str = 'A generalist agent meant to help solve problems',
                  max_subtasks: int = 5,
                  memory_bank = {'Function': Memory(top_k = 5, mapper = lambda x: x.fn_name + ': ' + x.fn_description, approach = 'retrieve_by_ranker')},
                  shared_variables = dict(),
+                 get_global_context = None,
                  default_to_llm = True,
                  verbose: bool = True,
                  debug: bool = False,
+                 llm = None,
                  **kwargs):
         ''' 
         Creates an LLM-based agent using description and outputs JSON based on output_format. 
         Agent does not answer in normal free-flow conversation, but outputs only concise task-based answers
         Design Philosophy:
         - Give only enough context needed to solve problem
         - Modularise components for greater accuracy of each component
@@ -144,51 +153,85 @@
         - max_subtasks: Int. The maximum number of subtasks the agent can have
         - memory_bank: class Dict[Memory]. Stores multiple types of memory for use by the agent. Customise the Memory config within the Memory class.
             - Key: `Function` (Already Implemented Natively) - Does RAG over Task -> Function mapping
             - Can add in more keys that would fit your use case. Retrieves similar items to task / overall plan (if able) for additional context in `get_next_subtasks()` and `use_llm()` function
             - For RAG over Documents, it is best done in a function of the Agent to retrieve more information when needed (so that we do not overload the Agent with information)
         - shared_variables. Dict. Default: empty dict. Stores the variables to be shared amongst inner functions and agents. 
             If not empty, will pass this dictionary by reference down to the inner agents and functions
+        - get_global_context. Function. Takes in self (agent variable) and returns the additional prompt (str) to be appended to `get_next_subtask` and `use_llm`. Allows for persistent agent states to be added to the prompt
         - default_to_llm. Bool. Default: True. Whether to default to use_llm function if there is no match to other functions. If False, use_llm will not be given to Agent
         - verbose: Bool. Default: True. Whether to print out intermediate thought processes of the Agent
         - debug: Bool. Default: False. Whether to debug StrictJSON messages
+        - llm: Function. The llm parameter that gets passed into Function/strict_json
         
         Inputs (optional):
         - **kwargs: Dict. Additional arguments you would like to pass on to the strict_json function
         
         '''
         self.agent_name = agent_name
         self.agent_description = agent_description
         self.max_subtasks = max_subtasks
         self.verbose = verbose
         self.memory_bank = memory_bank
         self.shared_variables = shared_variables
         self.default_to_llm = default_to_llm
-        
+        self.get_global_context = get_global_context
+
         self.debug = debug
-        
+        self.llm = llm
+
         # reset agent's state
         self.reset()
-        
+
         self.kwargs = kwargs
-        
+
         # start with default of only llm as the function
         self.function_map = {}
         # stores all existing function descriptions - prevent duplicate assignment of functions
         self.fn_description_list = []
         # adds the use llm function
         if self.default_to_llm:
             self.assign_functions([Function(fn_name = 'use_llm', 
                                         fn_description = f'Used only when no other function can do the task', 
+                                        is_compulsory = True,
                                         output_format = {"Output": "Output of LLM"})])
         # adds the end task function
         self.assign_functions([Function(fn_name = 'end_task',
                                        fn_description = 'Use only when task is completed',
+                                       is_compulsory = True,
                                        output_format = {})])
         
+    def save_agent(self, filename: str):
+        ''' Saves the entire agent to filename for reuse next time '''
+        
+        if not isinstance(filename, str):
+            if filename[-4:] != '.pkl':
+                raise Exception('Filename is not ending with .pkl')
+            return
+            
+        # Open a file in write-binary mode
+        with open(filename, 'wb') as file:
+            # Use pickle.dump() to save the dictionary to the file
+            pickle.dump(self, file)
+
+        print(f"Agent saved to {filename}")
+    
+    def load_agent(self, filename: str):
+        ''' Loads the entire agent from filename '''
+        
+        if not isinstance(filename, str):
+            if filename[-4:] != '.pkl':
+                raise Exception('Filename is not ending with .pkl')
+            return
+        
+        with open(filename, 'rb') as file:
+            self = pickle.load(file)
+            print(f"Agent loaded from {filename}")
+            return self
+        
     ## Generic Functions ##
     def reset(self):
         ''' Resets agent state, including resetting subtasks_completed '''
         self.assign_task('No task assigned')
         self.subtasks_completed = {}
         
     def assign_task(self, task: str, overall_task: str = ''):
@@ -208,30 +251,38 @@
         If you want to provide the agent with the context of functions available to it, set provide_function_list to True (default: False)
         If task is given, then we will use it to do RAG over functions'''
         
         # if we have a task to focus on, we can filter the functions (other than use_llm and end_task) by that task
         filtered_fn_list = None
         if task != '':
             filtered_fn_list = self.memory_bank['Function'].retrieve(task)
-            # add back use_llm and end_task if present in function_map
-            if 'use_llm' in self.function_map:
-                filtered_fn_list.append(self.function_map['use_llm'])
-            if 'end_task' in self.function_map:
-                filtered_fn_list.append(self.function_map['end_task'])
+            # add back compulsory functions (default: use_llm, end_task) if present in function_map
+            for name, function in self.function_map.items():
+                if function.is_compulsory:
+                    filtered_fn_list.append(function)
+                
+        # add in additional context to the prompt
+        global_context = ''
+        if self.get_global_context is not None:
+            global_context = 'Additional Context:' + self.get_global_context(self) + '\n'
         
         system_prompt = f"You are an agent named {self.agent_name} with the following description: ```{self.agent_description}```\n"
         if provide_function_list:
             system_prompt += f"You have the following Equipped Functions available:\n```{self.list_functions(filtered_fn_list)}```\n"
+        system_prompt += global_context
         system_prompt += query
         
+        
         res = strict_json(system_prompt = system_prompt,
         user_prompt = '',
         output_format = output_format, 
         verbose = self.debug,
+        llm = self.llm,
         **self.kwargs)
+
         return res
     
     def status(self):
         ''' Prints prettily the update of the agent's status. 
         If you would want to reference any agent-specific variable, just do so directly without calling this function '''
         print('Agent Name:', self.agent_name)
         print('Agent Description:', self.agent_description)
@@ -268,16 +319,16 @@
 
             # add in the function into the function_map
             self.function_map[stored_fn_name] = function
             
             # add function's description into fn_description_list
             self.fn_description_list.append(function.fn_description)
                                     
-            # add function to memory bank if is not the default functions
-            if stored_fn_name not in ['use_llm', 'end_task']:
+            # add function to memory bank for RAG over functions later on if is not a compulsory functions
+            if not function.is_compulsory:
                 self.memory_bank['Function'].append(function)
             
         return self
         
     def remove_function(self, function_name: str):
         ''' Removes a function from the agent '''
         if function_name in self.function_map:
@@ -290,15 +341,15 @@
             # remove function from function map
             del self.function_map[function_name]
         
     def list_functions(self, fn_list = None) -> list:
         ''' Returns the list of functions available to the agent. If fn_list is given, restrict the functions to only those in the list '''
         if fn_list is not None and len(fn_list) < len(self.function_map):
             if self.verbose:
-                print('Filtered Function Names:', ', '.join([name for name, function in self.function_map.items() if function.fn_name not in ['use_llm', 'end_task'] and function in fn_list]))
+                print('Filtered Function Names:', ', '.join([name for name, function in self.function_map.items() if function in fn_list]))
             return [f'Name: {name}\n' + str(function) for name, function in self.function_map.items() if function in fn_list]
         else:
             return [f'Name: {name}\n' + str(function) for name, function in self.function_map.items()]                       
     
     def print_functions(self):
         ''' Prints out the list of functions available to the agent '''
         functions = self.list_functions()
@@ -307,15 +358,15 @@
     def select_function(self, task: str = ''):
         ''' Based on the task (without any context), output the next function name and input parameters '''
         _, function_name, function_params = self.get_next_subtask(task = task)
             
         return function_name, function_params
     
     def use_agent(self, agent_name: str, agent_task: str):
-        ''' Uses an inner agent to do a task for the meta agent. Task outcomes goes directly to subtasks_completed of meta agent '''
+        ''' Uses an inner agent to do a task for the meta agent. Task outcome goes directly to subtasks_completed of meta agent '''
         self.use_function(agent_name, {"instruction": agent_task}, agent_task)
         
     def use_function(self, function_name: str, function_params: dict, subtask: str = '', stateful: bool = True):
         ''' Uses the function. stateful means we store the outcome of the function '''
         if function_name == "use_llm":
             if self.verbose: 
                 print(f'Getting LLM to perform the following task: {function_params["instruction"]}')
@@ -360,15 +411,14 @@
             if res == '':
                 res = {'Status': 'Completed'}
             
             self.add_subtask_result(subtask, res)
 
         return res
    
-        
     def get_next_subtask(self, task = ''):
         ''' Based on what the task is and the subtasks completed, we get the next subtask, function and input parameters'''
         
         if task == '':
                 background_info = f"Assigned Task:```{self.task}```\nAssigned Plan: ```{self.overall_plan}```\nPast Subtasks Completed: ```{self.subtasks_completed}```\n"
         else:
             background_info = f"Assigned Task:```{task}```\n"
@@ -385,19 +435,23 @@
             if name == 'Function': continue
             # Do not need to add to context if the memory item is empty
             if self.memory_bank[name].isempty(): continue
             else:
                 rag_info += f'Related {name}: ```{self.memory_bank[name].retrieve(task)}```\n'
                 
         # First select the Equipped Function
-        res = self.query(query = f'''{background_info}{rag_info}First create an Overall Plan modified from Assigned Plan with an array of steps to do Assigned Task from beginning to end, including uncompleted steps. Then, reflect on Past Subtasks Completed (note not all past subtasks are relevant to Assigned Task) to see what steps in Overall Plan are already completed. Then, generate Overall Plan Completed that outputs True for array elements of Overall Plan that are complete and False otherwsie. Then, generate the Next Step to fulfil the Assigned Task that can be performed by a single Equipped Function. If Assigned Task is completed, output end_task for Equipped Function''',
+        res = self.query(query = f'''{background_info}{rag_info}First create an Overall Plan modified from Assigned Plan with an array of steps to do Assigned Task from beginning to end, including uncompleted steps. Then, reflect on Past Subtasks Completed (note not all past subtasks are relevant to Assigned Task) to see what steps in Overall Plan are already completed. Then, generate Overall Plan Completed that outputs True for array elements of Overall Plan that are complete and False otherwise. Then, generate the Next Step to fulfil the Assigned Task that can be performed by a single Equipped Function. If Assigned Task is completed, output end_task for Equipped Function''',
                          output_format = {"Thoughts": "How to do Assigned Task", "Overall Plan": "Array of steps to complete Assigned Task from beginning to end, type: list", "Reflection": "What has been done and what is still left to do", "Overall Plan Completed": "Whether array elements in Overall Plan are already completed, type: List[bool]", "Next Step": "First non-completed element in Overall Plan", "Equipped Function": f"Name of Equipped Function to use for Next Step, type: Enum{list(self.function_map.keys())}", "Instruction": "Instruction for the Equipped Function if any"},
-                          provide_function_list = True,
+                         provide_function_list = True,
                          task = task)
-
+        
+        # end task if equipped function is incorrect
+        if res["Equipped Function"] not in self.function_map:
+            res["Equipped Function"] = "end_task"
+                
         # If equipped function is use_llm, or end_task, we don't need to do another query
         cur_function = self.function_map[res["Equipped Function"]]
         if res["Equipped Function"] == 'use_llm':
             res['Equipped Function Input'] = {'instruction': res['Next Step']}
         elif res['Equipped Function'] == 'end_task':
             res['Equipped Function Input'] = {}
         # Otherwise, if it is only the instruction, no type check needed, so just take the instruction
@@ -414,20 +468,23 @@
             for match in matches:
                 if ':' in match:
                     first_part, second_part = match.split(':', 1)
                     input_format[first_part] = f'A suitable value, type: {second_part}'
                 else:
                     input_format[match] = 'A suitable value'
                     
+            # if there is no input, then do not need LLM to extract out function's input
+            if input_format == {}:
+                res["Equipped Function Input"] = {}
                     
-            res2 = self.query(query = f'''{background_info}{rag_info}Current Subtask: {res["Next Step"]}\nEquipped Function Name: {res["Equipped Function"]}\nEquipped Function Details: {str(cur_function)}\nOutput suitable values for the input parameters of the Equipped Function to fulfil Current Subtask''',
-                         output_format = input_format,
-                         provide_function_list = False)
-            
-            res["Equipped Function Input"] = res2
+            else:    
+                res2 = self.query(query = f'''{background_info}{rag_info}Current Subtask: {res["Next Step"]}\nEquipped Function Name: {res["Equipped Function"]}\nEquipped Function Details: {str(cur_function)}\nOutput suitable values for the input parameters of the Equipped Function to fulfil Current Subtask''',
+                             output_format = input_format,
+                             provide_function_list = False)
+                res["Equipped Function Input"] = res2
 
         ## End Task Overrides
         # if the next step is already done before, then end the task. Unless it is in OS mode, then allow it
         if res["Next Step"] in self.subtasks_completed and self.default_to_llm is True:
             res["Equipped Function"] = "end_task"
 
         # if whole plan is completed, end task
@@ -485,16 +542,16 @@
         if stateful:
             self.add_subtask_result(my_query, res)
         
         return res
 
     def run(self, task: str = '', overall_task: str = '', num_subtasks: int = 0) -> list:
         ''' Attempts to do the task using LLM and available functions
-        Loops through and performs either a function call or LLM call up to max_steps number of times
-        If overall_task is filled, then we store it to pass to the inner agents for more context'''
+        Loops through and performs either a function call or LLM call up to num_subtasks number of times
+        If overall_task is filled, then we store it to pass to the inner agents for more context '''
             
         # Assign the task
         if task != '':
             self.task_completed = False
             # If meta agent's task is here as well, assign it too
             if overall_task != '':
                 self.assign_task(task, overall_task)
```

### Comparing `strictjson-4.0.0/strictjson/base.py` & `strictjson-4.0.1/strictjson/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -416,25 +416,26 @@
                 if param.default == inspect.Parameter.empty:
                     raise Exception(f'Input variable "{param_name}" not in docstring of "{my_function.__name__}"')
     
     return my_fn_description, param_list
 
 ### Main Functions ###
                 
-def strict_json(system_prompt: str, user_prompt: str, output_format: dict, custom_checks: dict = dict(), check_data = None, delimiter: str = '###', num_tries: int = 3, openai_json_mode: bool = False, **kwargs):
+def strict_json(system_prompt: str, user_prompt: str, output_format: dict, return_as_json = False, custom_checks: dict = dict(), check_data = None, delimiter: str = '###', num_tries: int = 3, openai_json_mode: bool = False, **kwargs):
     ''' Ensures that OpenAI will always adhere to the desired output JSON format defined in output_format. 
     Uses rule-based iterative feedback to ask GPT to self-correct.
     Keeps trying up to num_tries it it does not. Returns empty JSON if unable to after num_tries iterations.
     
     Inputs (compulsory):
     - system_prompt: String. Write in whatever you want GPT to become. e.g. "You are a \<purpose in life\>"
     - user_prompt: String. The user input. Later, when we use it as a function, this is the function input
     - output_format: Dict. JSON format with the key as the output key, and the value as the output description
     
     Inputs (optional):
+    - return_as_json: Bool. Default: False. Whether to return the output as a json. If False, returns as Python dict. If True, returns as json string
     - custom_checks: Dict. Key is output key, value is function which does checking of content for output field
     - check_data: Any data type. The additional data for custom_checks to use if required
     - delimiter: String (Default: '###'). This is the delimiter to surround the keys. With delimiter ###, key becomes ###key###
     - num_tries: Integer (default: 3). The number of tries to iteratively prompt GPT to generate correct json format
     - openai_json_mode: Boolean (default: False). Whether or not to use OpenAI JSON Mode
     - **kwargs: Dict. Additional arguments for LLM chat
     
@@ -453,31 +454,34 @@
         
         output_format_prompt = "\nOutput in the following json string format: " + str(output_format) + "\nBe concise."
             
         my_system_prompt = str(system_prompt) + output_format_prompt
         my_user_prompt = str(user_prompt) 
             
         res = chat(my_system_prompt, my_user_prompt, response_format = {"type": "json_object"}, **kwargs)
-            
-        try:
-            loaded_json = json.loads(res)
-        except Exception as e:
-            loaded_json = {}
-        return loaded_json
+        
+        if return_as_json:
+            return res
+        else:
+            try:
+                loaded_json = json.loads(res)
+            except Exception as e:
+                loaded_json = {}
+            return loaded_json
         
     # Otherwise, implement JSON parsing using Strict JSON
     else:
         # start off with no error message
         error_msg = ''
 
         # wrap the values with angle brackets and wrap keys with delimiter to encourage LLM to modify it
         new_output_format = wrap_with_angle_brackets(output_format, delimiter, 1)
         
         output_format_prompt = f'''\nOutput in the following json string format: {new_output_format}
-Update text enclosed in <>. Be concise. Output only the json string without any explanation.'''
+Update text enclosed in <>. Be concise. Output only the json string without any explanation. You must output valid json with all keys present.'''
 
         for i in range(num_tries):
             my_system_prompt = str(system_prompt) + output_format_prompt + error_msg
             my_user_prompt = str(user_prompt) 
 
             # Use OpenAI to get a response
             res = chat(my_system_prompt, my_user_prompt, **kwargs)
@@ -503,30 +507,35 @@
                             requirement, requirement_met, action_needed = check(end_dict[key], check_data)
                             print(f'Running check for "{requirement}" on output field of "{key}"')
                             if not requirement_met:
                                 print(f'Requirement not met. Action needed: "{action_needed}"\n\n')
                                 raise Exception(f'Output field of "{key}" does not meet requirement "{requirement}". Action needed: "{action_needed}"')
                             else:
                                 print('Requirement met\n\n')
-                return end_dict
+                if return_as_json:
+                    return json.dumps(end_dict, ensure_ascii=False)
+                else:
+                    return end_dict
 
             except Exception as e:
                 error_msg = f"\n\nPrevious json: {res}\njson error: {str(e)}\nFix the error."                
                 print("An exception occurred:", str(e))
                 print("Current invalid json format:", res)
 
         return {}
 
 class Function:
     def __init__(self,
                  fn_description: str = '', 
                  output_format: dict = {},
                  examples = None,
                  external_fn = None,
+                 is_compulsory = False,
                  fn_name = None,
+                 llm = None,
                  **kwargs):
         ''' 
         Creates an LLM-based function or wraps an external function using fn_description and outputs JSON based on output_format. 
         (Optional) Can define the function based on examples (list of Dict containing input and output variables for each example)
         (Optional) If you would like greater specificity in your function's input, you can describe the variable after the : in the input variable name, e.g. `<var1: an integer from 10 to 30`. Here, `var1` is the input variable and `an integer from 10 to 30` is the description.
         
         Inputs (primary):
@@ -534,15 +543,17 @@
 Can also be done automatically by providing docstring with input variable names in external_fn
         - output_format: Dict. Dictionary containing output variables names and description for each variable.
            
         Inputs (optional):
         - examples: Dict or List[Dict]. Examples in Dictionary form with the input and output variables (list if more than one)
         - external_fn: Python Function. If defined, instead of using LLM to process the function, we will run the external function. 
             If there are multiple outputs of this function, we will map it to the keys of `output_format` in a one-to-one fashion
+        - is_compulsory: Bool. Default: False. This is whether to always use the Function when doing planning in Agents
         - fn_name: String. If provided, this will be the name of the function. Otherwise, if `external_fn` is provided, it will be the name of `external_fn`. Otherwise, we will use LLM to generate a function name from the `fn_description`
+        - llm: Function. The llm parameter to pass into strict_json
         - **kwargs: Dict. Additional arguments you would like to pass on to the strict_json function
         
         ## Example
         fn_description = 'Output the sum of <num1> and <num2>'
         output_format = {'output': 'sum of two numbers'}
         examples = [{'num1': 5, 'num2': 6, 'output': 11}, {'num1': 2, 'num2': 4, 'output': 6}]
         '''
@@ -568,15 +579,17 @@
         # if there is no external function docstring provided, raise an error
         elif self.fn_description == '':
             raise Exception('Input variable "fn_description" (or docstring for External Functions) not provided')
 
         self.output_format = output_format
         self.examples = examples
         self.external_fn = external_fn
+        self.is_compulsory = is_compulsory
         self.fn_name = fn_name
+        self.llm = llm
         self.kwargs = kwargs
         
         self.variable_names = []
         self.shared_variable_names = []
         # use regex to extract variables from function description
         matches = re.findall(r'<(.*?)>', self.fn_description)
             
@@ -601,15 +614,17 @@
             # if external function has a name, use it
             if self.external_fn is not None and hasattr(self.external_fn, '__name__') and self.external_fn.__name__ != '<lambda>':
                 self.fn_name = self.external_fn.__name__
             # otherwise, generate name out
             else:
                 res = strict_json(system_prompt = "Output a function name to summarise the usage of this function.",
                                   user_prompt = str(self.fn_description),
-                                  output_format = {"Thoughts": "What function does", "Name": "Function name with _ separating words that summarises what function does"})
+                                  output_format = {"Thoughts": "What function does", "Name": "Function name with _ separating words that summarises what function does"},
+                                 llm = self.llm,
+                                 **self.kwargs)
                 self.fn_name = res['Name']
                 
         # change instance's name to function's name
         self.__name__ = self.fn_name
 
         # Append examples to description
         if self.examples is not None:
@@ -654,14 +669,15 @@
                 function_kwargs['var'+str(num+1)] = arg
                 
         # If strict_json function, do the function. 
         if self.external_fn is None:
             res = strict_json(system_prompt = self.fn_description,
                             user_prompt = function_kwargs,
                             output_format = self.output_format,
+                            llm = self.llm,
                             **self.kwargs, **strict_json_kwargs)
             
         # Else run the external function
         else:
             res = {}
             # if external function uses shared_variables, pass it in
             argspec = inspect.getfullargspec(self.external_fn)
```

### Comparing `strictjson-4.0.0/strictjson.egg-info/PKG-INFO` & `strictjson-4.0.1/strictjson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: strictjson
-Version: 4.0.0
+Version: 4.0.1
 Summary: A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/tanchongmin/strictjson
 Project-URL: Issues, https://github.com/tanchongmin/strictjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.3.6
+Requires-Dist: openai>=1.3.6
+Requires-Dist: dill>=0.3.7
 
-# Strict JSON v4.0.0
+# Strict JSON v4.0.1
 [UPDATE]: For Agentic Framework, do check out TaskGen (the official Agentic Framework building on StrictJSON). This will make the StrictJSON repo neater and this github will focus on using StrictJSON for LLM Output Parsing
 - https://github.com/simbianai/taskgen
 
 ### A Strict JSON Framework for LLM Outputs, that fixes problems that json.loads() cannot solve
 - Works for JSON outputs with multiple ' or " or { or } or \ or unmatched braces/brackets that may break a json.loads()
 
 ### Base Functionalities (see Tutorial.ipynb)
```

