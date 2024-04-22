# Comparing `tmp/eenhoorntje_llm_lib-0.6.tar.gz` & `tmp/eenhoorntje_llm_lib-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eenhoorntje_llm_lib-0.6.tar", last modified: Sat Apr 20 02:23:08 2024, max compression
+gzip compressed data, was "eenhoorntje_llm_lib-0.7.tar", last modified: Mon Apr 22 03:00:24 2024, max compression
```

## Comparing `eenhoorntje_llm_lib-0.6.tar` & `eenhoorntje_llm_lib-0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 02:23:08.772265 eenhoorntje_llm_lib-0.6/
--rw-rw-rw-   0        0        0      284 2024-04-20 02:23:08.771268 eenhoorntje_llm_lib-0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-20 02:23:05.000000 eenhoorntje_llm_lib-0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 02:23:08.761294 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/
--rw-rw-rw-   0        0        0        0 2024-04-18 09:27:19.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/__init__.py
--rw-rw-rw-   0        0        0     1634 2024-04-20 01:20:42.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/deepl.py
--rw-rw-rw-   0        0        0     2437 2024-04-20 01:57:53.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/gemini.py
--rw-rw-rw-   0        0        0    11811 2024-04-20 02:11:12.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/language_codes.py
--rw-rw-rw-   0        0        0     1441 2024-04-20 01:57:53.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/llm.py
--rw-rw-rw-   0        0        0     1988 2024-04-18 09:36:38.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/llm_cache.py
--rw-rw-rw-   0        0        0      882 2024-04-20 02:21:34.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/translate.py
--rw-rw-rw-   0        0        0     1558 2024-04-20 02:21:34.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/translate_llm.py
--rw-rw-rw-   0        0        0      937 2024-04-18 12:13:56.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 02:23:08.771268 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib.egg-info/
--rw-rw-rw-   0        0        0      284 2024-04-20 02:23:08.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-04-20 02:23:08.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 02:23:08.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-20 02:23:08.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-20 02:23:08.000000 eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 02:23:08.772265 eenhoorntje_llm_lib-0.6/setup.cfg
--rw-rw-rw-   0        0        0      523 2024-04-20 02:23:05.000000 eenhoorntje_llm_lib-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:00:24.894962 eenhoorntje_llm_lib-0.7/
+-rw-rw-rw-   0        0        0      284 2024-04-22 03:00:24.894962 eenhoorntje_llm_lib-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-20 02:23:05.000000 eenhoorntje_llm_lib-0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 03:00:24.879035 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:27:19.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/__init__.py
+-rw-rw-rw-   0        0        0     1634 2024-04-20 01:20:42.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/deepl.py
+-rw-rw-rw-   0        0        0     2437 2024-04-20 01:57:53.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/gemini.py
+-rw-rw-rw-   0        0        0    11811 2024-04-20 02:11:12.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/language_codes.py
+-rw-rw-rw-   0        0        0     1457 2024-04-22 02:59:55.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/llm.py
+-rw-rw-rw-   0        0        0     1988 2024-04-18 09:36:38.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/llm_cache.py
+-rw-rw-rw-   0        0        0      882 2024-04-20 02:21:34.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/translate.py
+-rw-rw-rw-   0        0        0     1558 2024-04-20 02:21:34.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/translate_llm.py
+-rw-rw-rw-   0        0        0      937 2024-04-18 12:13:56.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:00:24.893965 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib.egg-info/
+-rw-rw-rw-   0        0        0      284 2024-04-22 03:00:24.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-04-22 03:00:24.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 03:00:24.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-22 03:00:24.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-22 03:00:24.000000 eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 03:00:24.894962 eenhoorntje_llm_lib-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      523 2024-04-22 03:00:20.000000 eenhoorntje_llm_lib-0.7/setup.py
```

### Comparing `eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/deepl.py` & `eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/deepl.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/gemini.py` & `eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/gemini.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/language_codes.py` & `eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/language_codes.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/llm.py` & `eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/llm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from openai import OpenAI
 import json
 import eenhoorntje_llm_lib.llm_cache
+import eenhoorntje_llm_lib.utils
 import time
 
 
 def clear_cache():
     eenhoorntje_llm_lib.llm_cache.cache.clear()
 
 
 def call_llm(messages, model="anthropic/claude-3-haiku", temperature=0.0, max_tokens=500):
-    api_key = json.load(open("keys.json", "r", encoding="utf-8"))["OPEN_ROUTER_API_KEY"]
+    api_key = eenhoorntje_llm_lib.utils.get_key("OPEN_ROUTER_API_KEY")
     client = OpenAI(
         base_url="https://openrouter.ai/api/v1",
         api_key=api_key,
     )
 
     cache_key = None
     if temperature == 0.0:
```

### Comparing `eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/llm_cache.py` & `eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/llm_cache.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/translate.py` & `eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/translate.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/translate_llm.py` & `eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/translate_llm.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib/utils.py` & `eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib/utils.py`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.6/eenhoorntje_llm_lib.egg-info/SOURCES.txt` & `eenhoorntje_llm_lib-0.7/eenhoorntje_llm_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eenhoorntje_llm_lib-0.6/setup.py` & `eenhoorntje_llm_lib-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='eenhoorntje_llm_lib',
-    version='0.6',
+    version='0.7',
     description='A lib for cached LLM calling and translation',
     author='Dmitrii Lukianov',
     author_email='unicornporated@gmil.com',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["openai", "google-generativeai"],
```

