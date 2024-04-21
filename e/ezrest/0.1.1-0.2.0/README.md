# Comparing `tmp/ezrest-0.1.1.tar.gz` & `tmp/ezrest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezrest-0.1.1.tar", last modified: Sat Apr 20 14:12:47 2024, max compression
+gzip compressed data, was "ezrest-0.2.0.tar", last modified: Sun Apr 21 22:00:20 2024, max compression
```

## Comparing `ezrest-0.1.1.tar` & `ezrest-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-20 14:12:47.989097 ezrest-0.1.1/
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1071 2024-04-08 18:35:44.000000 ezrest-0.1.1/LICENSE
--rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4147 2024-04-20 14:12:47.989097 ezrest-0.1.1/PKG-INFO
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-20 14:12:47.985097 ezrest-0.1.1/docs/
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1738 2024-04-18 20:20:47.000000 ezrest-0.1.1/docs/README.md
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-20 14:12:47.985097 ezrest-0.1.1/ezrest/
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       22 2024-04-20 13:35:49.000000 ezrest-0.1.1/ezrest/__init__.py
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     9776 2024-04-20 14:02:21.000000 ezrest-0.1.1/ezrest/requests.py
-drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-20 14:12:47.985097 ezrest-0.1.1/ezrest.egg-info/
--rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4147 2024-04-20 14:12:47.000000 ezrest-0.1.1/ezrest.egg-info/PKG-INFO
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)      224 2024-04-20 14:12:47.000000 ezrest-0.1.1/ezrest.egg-info/SOURCES.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        1 2024-04-20 14:12:47.000000 ezrest-0.1.1/ezrest.egg-info/dependency_links.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       68 2024-04-20 14:12:47.000000 ezrest-0.1.1/ezrest.egg-info/requires.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        7 2024-04-20 14:12:47.000000 ezrest-0.1.1/ezrest.egg-info/top_level.txt
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1592 2024-04-20 14:01:52.000000 ezrest-0.1.1/pyproject.toml
--rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       38 2024-04-20 14:12:47.989097 ezrest-0.1.1/setup.cfg
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-21 22:00:20.858135 ezrest-0.2.0/
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1071 2024-04-08 18:35:44.000000 ezrest-0.2.0/LICENSE
+-rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4147 2024-04-21 22:00:20.858135 ezrest-0.2.0/PKG-INFO
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-21 22:00:20.854135 ezrest-0.2.0/docs/
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1738 2024-04-21 21:39:54.000000 ezrest-0.2.0/docs/README.md
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-21 22:00:20.854135 ezrest-0.2.0/ezrest/
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       22 2024-04-21 21:39:57.000000 ezrest-0.2.0/ezrest/__init__.py
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     5360 2024-04-21 18:13:33.000000 ezrest-0.2.0/ezrest/objects.py
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     9774 2024-04-21 17:03:21.000000 ezrest-0.2.0/ezrest/requests.py
+drwxrwxr-x   0 mrf0x     (1000) mrf0x     (1000)        0 2024-04-21 22:00:20.858135 ezrest-0.2.0/ezrest.egg-info/
+-rw-r--r--   0 mrf0x     (1000) mrf0x     (1000)     4147 2024-04-21 22:00:20.000000 ezrest-0.2.0/ezrest.egg-info/PKG-INFO
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)      242 2024-04-21 22:00:20.000000 ezrest-0.2.0/ezrest.egg-info/SOURCES.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        1 2024-04-21 22:00:20.000000 ezrest-0.2.0/ezrest.egg-info/dependency_links.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       68 2024-04-21 22:00:20.000000 ezrest-0.2.0/ezrest.egg-info/requires.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)        7 2024-04-21 22:00:20.000000 ezrest-0.2.0/ezrest.egg-info/top_level.txt
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)     1592 2024-04-20 19:15:51.000000 ezrest-0.2.0/pyproject.toml
+-rw-rw-r--   0 mrf0x     (1000) mrf0x     (1000)       38 2024-04-21 22:00:20.858135 ezrest-0.2.0/setup.cfg
```

### Comparing `ezrest-0.1.1/LICENSE` & `ezrest-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezrest-0.1.1/PKG-INFO` & `ezrest-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezrest
-Version: 0.1.1
+Version: 0.2.0
 Summary: Modular Python framework for implementing REST API clients
 Author: Jacek Lewański
 License: MIT License
         
         Copyright (c) 2024 Jacek Lewański
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,15 +66,15 @@
 ## Installation
 
 **Requirements:** Python 3.8+
 
 ```bash
 pip install ezrest
 # Or by providing specific version:
-pip install ezrest==0.1.0
+pip install ezrest==0.2.0
 ```
 
 ## Usage <!-- {docsify-ignore} -->
 
 Please refer to the [documentation pages](https://nullJaX.github.io/ezrest/#/modules) on how to use this module.
 
 ## Contributing
```

### Comparing `ezrest-0.1.1/docs/README.md` & `ezrest-0.2.0/docs/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ## Installation
 
 **Requirements:** Python 3.8+
 
 ```bash
 pip install ezrest
 # Or by providing specific version:
-pip install ezrest==0.1.0
+pip install ezrest==0.2.0
 ```
 
 ## Usage <!-- {docsify-ignore} -->
 
 Please refer to the [documentation pages](https://nullJaX.github.io/ezrest/#/modules) on how to use this module.
 
 ## Contributing
```

### Comparing `ezrest-0.1.1/ezrest/requests.py` & `ezrest-0.2.0/ezrest/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def delete(self, url: str, *args, **kwargs) -> _ResponseType:
         """Performs HTTP DELETE request"""
         raise NotImplementedError()
 
     def list(self, url: str, *args, **kwargs) -> Iterator[_ResponseType]:
         """
-        Returns items/resources one-by-one for endpoints returning collections
+        Yields items/resources one-by-one for endpoints returning collections
         and/or paginated responses.
 
         Example:
 
         def list(self, url: str, *args, **kwargs) -> Iterator[ResponseType]:
             next_url: str = url
             while next_url:
@@ -108,15 +108,15 @@
 
     async def delete(self, url: str, *args, **kwargs) -> _ResponseType:
         """Performs HTTP DELETE request"""
         raise NotImplementedError()
 
     async def list(self, url: str, *args, **kwargs) -> AsyncIterator[_ResponseType]:
         """
-        Returns items/resources one-by-one for endpoints returning collections
+        Yields items/resources one-by-one for endpoints returning collections
         and/or paginated responses.
 
         Example:
 
         async def list(self, url: str, *args, **kwargs) -> AsyncIterator[ResponseType]:
             next_url: str = url
             while next_url:
```

### Comparing `ezrest-0.1.1/ezrest.egg-info/PKG-INFO` & `ezrest-0.2.0/ezrest.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezrest
-Version: 0.1.1
+Version: 0.2.0
 Summary: Modular Python framework for implementing REST API clients
 Author: Jacek Lewański
 License: MIT License
         
         Copyright (c) 2024 Jacek Lewański
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,15 +66,15 @@
 ## Installation
 
 **Requirements:** Python 3.8+
 
 ```bash
 pip install ezrest
 # Or by providing specific version:
-pip install ezrest==0.1.0
+pip install ezrest==0.2.0
 ```
 
 ## Usage <!-- {docsify-ignore} -->
 
 Please refer to the [documentation pages](https://nullJaX.github.io/ezrest/#/modules) on how to use this module.
 
 ## Contributing
```

### Comparing `ezrest-0.1.1/pyproject.toml` & `ezrest-0.2.0/pyproject.toml`

 * *Files identical despite different names*

