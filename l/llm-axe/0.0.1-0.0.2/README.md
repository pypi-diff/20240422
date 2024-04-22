# Comparing `tmp/llm_axe-0.0.1.tar.gz` & `tmp/llm_axe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_axe-0.0.1.tar", last modified: Mon Apr 22 01:07:13 2024, max compression
+gzip compressed data, was "llm_axe-0.0.2.tar", last modified: Mon Apr 22 04:29:33 2024, max compression
```

## Comparing `llm_axe-0.0.1.tar` & `llm_axe-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 01:07:13.129779 llm_axe-0.0.1/
--rw-rw-rw-   0        0        0      740 2024-04-22 01:07:13.129279 llm_axe-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 01:07:13.124279 llm_axe-0.0.1/llm_axe/
--rw-rw-rw-   0        0        0      328 2024-04-22 00:14:20.000000 llm_axe-0.0.1/llm_axe/__init__.py
--rw-rw-rw-   0        0        0     9236 2024-04-21 23:58:38.000000 llm_axe-0.0.1/llm_axe/agents.py
--rw-rw-rw-   0        0        0     3883 2024-04-22 00:03:24.000000 llm_axe-0.0.1/llm_axe/core.py
--rw-rw-rw-   0        0        0      576 2024-04-20 19:13:17.000000 llm_axe-0.0.1/llm_axe/models.py
-drwxrwxrwx   0        0        0        0 2024-04-22 01:07:13.128279 llm_axe-0.0.1/llm_axe.egg-info/
--rw-rw-rw-   0        0        0      740 2024-04-22 01:07:13.000000 llm_axe-0.0.1/llm_axe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-22 01:07:13.000000 llm_axe-0.0.1/llm_axe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 01:07:13.000000 llm_axe-0.0.1/llm_axe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 01:07:13.000000 llm_axe-0.0.1/llm_axe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 01:07:13.129779 llm_axe-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1155 2024-04-22 01:06:51.000000 llm_axe-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 04:29:33.094571 llm_axe-0.0.2/
+-rw-rw-rw-   0        0        0      728 2024-04-22 04:29:33.093573 llm_axe-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-22 04:29:33.087070 llm_axe-0.0.2/llm_axe/
+-rw-rw-rw-   0        0        0      328 2024-04-22 04:26:56.000000 llm_axe-0.0.2/llm_axe/__init__.py
+-rw-rw-rw-   0        0        0    12307 2024-04-22 04:25:13.000000 llm_axe-0.0.2/llm_axe/agents.py
+-rw-rw-rw-   0        0        0     4206 2024-04-22 03:42:57.000000 llm_axe-0.0.2/llm_axe/core.py
+-rw-rw-rw-   0        0        0      576 2024-04-20 19:13:17.000000 llm_axe-0.0.2/llm_axe/models.py
+drwxrwxrwx   0        0        0        0 2024-04-22 04:29:33.092573 llm_axe-0.0.2/llm_axe.egg-info/
+-rw-rw-rw-   0        0        0      728 2024-04-22 04:29:32.000000 llm_axe-0.0.2/llm_axe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-22 04:29:32.000000 llm_axe-0.0.2/llm_axe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 04:29:32.000000 llm_axe-0.0.2/llm_axe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-22 04:29:32.000000 llm_axe-0.0.2/llm_axe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 04:29:33.094571 llm_axe-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1143 2024-04-22 04:28:43.000000 llm_axe-0.0.2/setup.py
```

### Comparing `llm_axe-0.0.1/PKG-INFO` & `llm_axe-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: llm_axe
-Version: 0.0.1
+Version: 0.0.2
 Summary: A toolkit for quicky implementing complex interactions for local LLMs
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 
-A toolkit for quicky implementing complex interactions for local LLMs. Includes features such as function callers, online agents, pre-made generic agents, and more.
+llm_axe allows you to quickly implement complex interactions for local LLMs, such as function callers, online agents, pre-made generic agents, and more.
```

### Comparing `llm_axe-0.0.1/llm_axe/agents.py` & `llm_axe-0.0.2/llm_axe/agents.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,72 @@
 import warnings
-from llm_axe.core import AgentType, safe_read_json, generate_schema, get_yaml_prompt, internet_search, read_website
+import os
+from llm_axe.core import AgentType, safe_read_json, generate_schema, get_yaml_prompt, internet_search, read_website, read_pdf
+
+
+class PdfReader():
+    """
+    A PdfReader agent is used to answer questions based on information from given PDF files.
+    """
+
+    def __init__(self, llm:object=None, pdf_files:list=None, additional_system_instructions:str="", custom_system_prompt:str=None):
+        """
+        Initializes a new PdfReader.
+        Args:
+            llm (object): An object that implements the ask() method.
+            pdf_files (list): A list of PDF files to read. Each file should be a string representing the path to the PDF file.
+            additional_system_instructions (str, optional): Additional instructions to include in the system prompt.
+            custom_system_prompt (str, optional): Custom system prompt. Defaults to None.
+        """
+        self.llm = llm
+        self.pdf_files = pdf_files
+        self.additional_instructions = additional_system_instructions
+        self.system_prompt = get_yaml_prompt("system_prompts.yaml", "DocumentReader")
+        self.custom_system_prompt = custom_system_prompt
+
+
+    def ask(self, question:str, pdf_files:list=None):
+        """
+        Ask a question based on the given PDF files.
+        """
+        if self.llm is None:
+            raise ValueError("No LLM object provided.")
+        
+        prompts = self.get_prompt(question, pdf_files)
+        return self.llm.ask(prompts)
+    
+    def get_prompt(self, question, pdf_files:list=None):
+        """
+        Generates the prompt for the LLM.
+        args:
+            question (str): The question to ask.
+            pdf_files (list): A list of PDF files to read. Each file should be a string representing the path to the PDF file. 
+        """
+        pdf_text = ""
+        for pdf_file in pdf_files:
+            pdf_text += f"Contents of document {os.path.basename(pdf_file)} :\n"
+            pdf_text += read_pdf(pdf_file) + "\n\n"
+        
+        if self.custom_system_prompt is None:
+            self.system_prompt = get_yaml_prompt("system_prompts.yaml", "DocumentReader")
+        else:
+            self.system_prompt = self.custom_system_prompt
+
+        self.system_prompt = {"role":"system", 
+                          "content": self.system_prompt.format(documents=pdf_text, additional_instructions=self.additional_instructions)}
+        
+        user_prompt = {"role":"user", "content": question}
+        prompts = [self.system_prompt, user_prompt]
+
+        return prompts
+    
 
 class FunctionCaller():
     """
-    A FunctionCaller object is used to call functions using an LLM.
+    A FunctionCaller agent is used to call functions using an LLM.
     By default, premade system prompts are used, however you can provide your own if you have issues with the default.
     For best results, your function name and parameters must be given meaningful names, 
     have type annotations doc string descriptions.
     """
 
     def __init__(self, llm:object=None, functions:list=None, additional_system_instructions:str="", custom_system_prompt:str=None):            
         """
@@ -103,26 +162,32 @@
                     - content (str): The content of the user prompt.
         """
         user_prompt = {"role":"user", "content": question}
         prompts = [self.system_prompt, user_prompt]
         return prompts
 
 
-
 class OnlineAgent:
     """
     An agent that has internet access. 
     It will use the internet to try and best answer the user prompt
     """
 
-    def __init__(self, llm:object, additional_system_instructions:str=""):
+    def __init__(self, llm:object, additional_system_instructions:str="", custom_searcher:callable=None):
+        """
+        Args:
+            llm (object): An LLM object. Must have an ask method.
+            additional_system_instructions (str, optional): Instructions in addition to the system prompt. Defaults to "".
+            custom_searcher (function, optional): A custom online searcher function. The searcher function must take a query and return a list of string URLS
+        """
         self.llm = llm
         self.system_prompt = get_yaml_prompt("system_prompts.yaml", "OnlineSearcher")
         self.system_prompt = {"role":"system", 
                               "content": self.system_prompt.format(additional_instructions=additional_system_instructions)}
+        self.search_function = custom_searcher if custom_searcher else internet_search
 
     def search(self, prompt):
         """
         Searches the internet and answers the prompt based on the search results.
 
         Parameters:
             prompt (str): The prompt or question to answer.
@@ -130,21 +195,20 @@
         Returns:
             str: The response that answers the prompt.
         """
 
         # Will first get a good search query
         # The query will be used to find relevant URLS
         # The llm will pick the best URL and read it to answer the prompt
-        
+    
         query = self.get_search_query(prompt)
         if query is None:
             return None
-        print(query)
 
-        search_results = internet_search(query)
+        search_results = self.search_function(query)
         search_results = " ".join(search_results) #list to a string
         url_picker_prompt = get_yaml_prompt("system_prompts.yaml", "UrlPicker")
         url_picker_prompt = {"role":"system", "content": url_picker_prompt.format(question=prompt, urls=search_results)}
         resp = self.llm.ask([url_picker_prompt])
         resp_json = safe_read_json(resp)
         
         # Check if the response is a valid url
@@ -159,15 +223,18 @@
         user_prompt = f'''
                     Please read the following information:
                     
                     Information about Website {url}: 
                     {website_text}
 
                     Answer the following question based on the above information: 
-                    {prompt}'''
+                    {prompt}
+
+                    Start your answer with "Based on information from the internet, "
+                    '''
         
         final_responder = Agent(llm=self.llm, agent_type=AgentType.GENERIC_RESPONDER)
         return final_responder.ask(user_prompt)
 
     def get_search_query(self, question):
         user_prompt = {"role":"user", "content": question}
         prompts = [self.system_prompt, user_prompt]
```

### Comparing `llm_axe-0.0.1/llm_axe/core.py` & `llm_axe-0.0.2/llm_axe/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,39 @@
 import warnings
 import yaml
 import docstring_parser
 from enum import Enum
 from googlesearch import search
 import requests
 from bs4 import BeautifulSoup
+from pypdf import PdfReader
 
 class AgentType(Enum):
     """
     Enum for agent types
     See documentation for explanation of Agents
     """
     PLANNER = "Planner"
     SUMMARIZER = "Summarizer"
     GENERIC_RESPONDER = "GenericResponder"
 
+
+def read_pdf(file):
+    """
+    Reads a pdf file and returns the complete text content.
+    Args:
+        file (str): The path to the pdf file.
+    """
+    reader = PdfReader(file)
+    text = ""
+    for page in reader.pages:
+        text += page.extract_text()
+    return text
+
+
 def get_yaml_prompt(yaml_file_name:str, prompt_name:str):
     """
     Reads a prompt from a yaml file.
     See system_prompts.yaml for a list of prompts.
     Args:
         yaml_file_name (str): The name of the yaml file to load.
         prompt_name (str): The name of the prompt to load.
```

### Comparing `llm_axe-0.0.1/llm_axe/models.py` & `llm_axe-0.0.2/llm_axe/models.py`

 * *Files identical despite different names*

### Comparing `llm_axe-0.0.1/llm_axe.egg-info/PKG-INFO` & `llm_axe-0.0.2/llm_axe.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: llm-axe
-Version: 0.0.1
+Version: 0.0.2
 Summary: A toolkit for quicky implementing complex interactions for local LLMs
 Author: Emir Sahin
 Author-email: emirsah122@gmail.com
 License: MIT
 Keywords: python,llm axe,llm toolkit,local llm,local llm internet,function caller llm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 
-A toolkit for quicky implementing complex interactions for local LLMs. Includes features such as function callers, online agents, pre-made generic agents, and more.
+llm_axe allows you to quickly implement complex interactions for local LLMs, such as function callers, online agents, pre-made generic agents, and more.
```

### Comparing `llm_axe-0.0.1/setup.py` & `llm_axe-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'A toolkit for quicky implementing complex interactions for local LLMs'
-LONG_DESCRIPTION = 'A toolkit for quicky implementing complex interactions for local LLMs. Includes features such as function callers, online agents, pre-made generic agents, and more.'
+LONG_DESCRIPTION = 'llm_axe allows you to quickly implement complex interactions for local LLMs, such as function callers, online agents, pre-made generic agents, and more.'
 
 # Setting up
 setup(
         name="llm_axe", 
         version=VERSION,
         author="Emir Sahin",
         author_email="emirsah122@gmail.com",
```

