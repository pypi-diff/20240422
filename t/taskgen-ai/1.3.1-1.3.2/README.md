# Comparing `tmp/taskgen_ai-1.3.1.tar.gz` & `tmp/taskgen_ai-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskgen_ai-1.3.1.tar", last modified: Tue Apr 16 15:44:22 2024, max compression
+gzip compressed data, was "taskgen_ai-1.3.2.tar", last modified: Mon Apr 22 03:28:31 2024, max compression
```

## Comparing `taskgen_ai-1.3.1.tar` & `taskgen_ai-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-16 15:44:22.560490 taskgen_ai-1.3.1/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-1.3.1/LICENSE
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21085 2024-04-16 15:44:22.560018 taskgen_ai-1.3.1/PKG-INFO
--rw-rw-r--   0 tanchongmin   (501) staff       (20)    20503 2024-04-16 15:00:00.000000 taskgen_ai-1.3.1/README.md
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      649 2024-04-16 15:43:59.000000 taskgen_ai-1.3.1/pyproject.toml
--rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-04-16 15:44:22.560575 taskgen_ai-1.3.1/setup.cfg
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      180 2024-04-16 15:00:11.000000 taskgen_ai-1.3.1/setup.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-16 15:44:22.556525 taskgen_ai-1.3.1/taskgen/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      170 2024-03-14 09:43:26.000000 taskgen_ai-1.3.1/taskgen/__init__.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    33533 2024-04-05 09:43:06.000000 taskgen_ai-1.3.1/taskgen/agent.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    36446 2024-04-05 09:43:08.000000 taskgen_ai-1.3.1/taskgen/base.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-16 15:44:22.559506 taskgen_ai-1.3.1/taskgen_ai.egg-info/
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21085 2024-04-16 15:44:22.000000 taskgen_ai-1.3.1/taskgen_ai.egg-info/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-04-16 15:44:22.000000 taskgen_ai-1.3.1/taskgen_ai.egg-info/SOURCES.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-04-16 15:44:22.000000 taskgen_ai-1.3.1/taskgen_ai.egg-info/dependency_links.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       14 2024-04-16 15:44:22.000000 taskgen_ai-1.3.1/taskgen_ai.egg-info/requires.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-04-16 15:44:22.000000 taskgen_ai-1.3.1/taskgen_ai.egg-info/top_level.txt
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:28:31.022642 taskgen_ai-1.3.2/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-1.3.2/LICENSE
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21112 2024-04-22 03:28:31.021906 taskgen_ai-1.3.2/PKG-INFO
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)    20503 2024-04-22 02:38:29.000000 taskgen_ai-1.3.2/README.md
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      664 2024-04-22 02:38:21.000000 taskgen_ai-1.3.2/pyproject.toml
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-04-22 03:28:31.022803 taskgen_ai-1.3.2/setup.cfg
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      202 2024-04-22 02:38:59.000000 taskgen_ai-1.3.2/setup.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:28:31.017894 taskgen_ai-1.3.2/taskgen/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      170 2024-03-14 09:43:26.000000 taskgen_ai-1.3.2/taskgen/__init__.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    33533 2024-04-22 02:45:45.000000 taskgen_ai-1.3.2/taskgen/agent.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    36879 2024-04-22 03:04:08.000000 taskgen_ai-1.3.2/taskgen/base.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-22 03:28:31.021254 taskgen_ai-1.3.2/taskgen_ai.egg-info/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21112 2024-04-22 03:28:31.000000 taskgen_ai-1.3.2/taskgen_ai.egg-info/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-04-22 03:28:31.000000 taskgen_ai-1.3.2/taskgen_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-04-22 03:28:31.000000 taskgen_ai-1.3.2/taskgen_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       26 2024-04-22 03:28:31.000000 taskgen_ai-1.3.2/taskgen_ai.egg-info/requires.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-04-22 03:28:31.000000 taskgen_ai-1.3.2/taskgen_ai.egg-info/top_level.txt
```

### Comparing `taskgen_ai-1.3.1/LICENSE` & `taskgen_ai-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taskgen_ai-1.3.1/PKG-INFO` & `taskgen_ai-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
+Requires-Dist: dill>=0.3.7
 
-# TaskGen v1.3.1
+# TaskGen v1.3.2
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete!
```

### Comparing `taskgen_ai-1.3.1/README.md` & `taskgen_ai-1.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TaskGen v1.3.1
+# TaskGen v1.3.2
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete!
```

### Comparing `taskgen_ai-1.3.1/pyproject.toml` & `taskgen_ai-1.3.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taskgen-ai"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="John Tan Chong Min", email="tanchongmin@gmail.com" },
 ]
 description = "A Task-based agentic framework building on StrictJSON outputs by LLM agents"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["openai>=1.3.6"]
+dependencies = ["openai>=1.3.6", "dill>=0.3.7"]
 
 [project.urls]
 Homepage = "https://github.com/simbianai/taskgen"
 Issues = "https://github.com/simbianai/taskgen/issues"
```

### Comparing `taskgen_ai-1.3.1/taskgen/agent.py` & `taskgen_ai-1.3.2/taskgen/agent.py`

 * *Files identical despite different names*

### Comparing `taskgen_ai-1.3.1/taskgen/base.py` & `taskgen_ai-1.3.2/taskgen/base.py`

 * *Files 2% similar despite different names*

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
@@ -503,15 +507,18 @@
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
```

### Comparing `taskgen_ai-1.3.1/taskgen_ai.egg-info/PKG-INFO` & `taskgen_ai-1.3.2/taskgen_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.3.6
+Requires-Dist: dill>=0.3.7
 
-# TaskGen v1.3.1
+# TaskGen v1.3.2
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
 - Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
 - Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete!
```

