# Comparing `tmp/server_templates-0.2.6.tar.gz` & `tmp/server_templates-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "server_templates-0.2.6.tar", last modified: Fri Mar 29 11:41:02 2024, max compression
+gzip compressed data, was "server_templates-0.2.7.tar", last modified: Mon Apr 22 08:40:26 2024, max compression
```

## Comparing `server_templates-0.2.6.tar` & `server_templates-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 11:41:02.420133 server_templates-0.2.6/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 server_templates-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     1896 2024-03-29 11:41:02.419633 server_templates-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2024-03-29 11:37:45.000000 server_templates-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 11:41:02.389753 server_templates-0.2.6/server_templates/
--rw-rw-rw-   0        0        0      149 2024-02-15 07:01:39.000000 server_templates-0.2.6/server_templates/__init__.py
--rw-rw-rw-   0        0        0     7623 2024-03-05 15:09:35.000000 server_templates-0.2.6/server_templates/client_requests.py
-drwxrwxrwx   0        0        0        0 2024-03-29 11:41:02.410268 server_templates-0.2.6/server_templates/server_aiohttp/
--rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.2.6/server_templates/server_aiohttp/__init__.py
--rw-rw-rw-   0        0        0    10652 2024-03-29 11:33:06.000000 server_templates-0.2.6/server_templates/server_aiohttp/main.py
-drwxrwxrwx   0        0        0        0 2024-03-29 11:41:02.415722 server_templates-0.2.6/server_templates/server_fastapi/
--rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.2.6/server_templates/server_fastapi/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-03-29 09:04:18.000000 server_templates-0.2.6/server_templates/server_fastapi/main.py
-drwxrwxrwx   0        0        0        0 2024-03-29 11:41:02.418664 server_templates-0.2.6/server_templates.egg-info/
--rw-rw-rw-   0        0        0     1896 2024-03-29 11:41:02.000000 server_templates-0.2.6/server_templates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-03-29 11:41:02.000000 server_templates-0.2.6/server_templates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 11:41:02.000000 server_templates-0.2.6/server_templates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-29 11:41:02.000000 server_templates-0.2.6/server_templates.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 11:41:02.423647 server_templates-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     2092 2024-01-30 06:52:17.000000 server_templates-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:26.954530 server_templates-0.2.7/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 server_templates-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     1970 2024-04-22 08:40:26.954530 server_templates-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2024-04-22 08:38:53.000000 server_templates-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:26.942181 server_templates-0.2.7/server_templates/
+-rw-rw-rw-   0        0        0      196 2024-04-17 12:25:31.000000 server_templates-0.2.7/server_templates/__init__.py
+-rw-rw-rw-   0        0        0     7623 2024-03-05 15:09:35.000000 server_templates-0.2.7/server_templates/client_requests.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:26.948878 server_templates-0.2.7/server_templates/server_aiohttp/
+-rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.2.7/server_templates/server_aiohttp/__init__.py
+-rw-rw-rw-   0        0        0    10652 2024-03-29 11:33:06.000000 server_templates-0.2.7/server_templates/server_aiohttp/main.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:26.951962 server_templates-0.2.7/server_templates/server_fastapi/
+-rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.2.7/server_templates/server_fastapi/__init__.py
+-rw-rw-rw-   0        0        0    21044 2024-04-22 07:59:40.000000 server_templates-0.2.7/server_templates/server_fastapi/main.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:26.953501 server_templates-0.2.7/server_templates.egg-info/
+-rw-rw-rw-   0        0        0     1970 2024-04-22 08:40:26.000000 server_templates-0.2.7/server_templates.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-04-22 08:40:26.000000 server_templates-0.2.7/server_templates.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 08:40:26.000000 server_templates-0.2.7/server_templates.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-22 08:40:26.000000 server_templates-0.2.7/server_templates.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 08:40:26.956531 server_templates-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     2092 2024-01-30 06:52:17.000000 server_templates-0.2.7/setup.py
```

### Comparing `server_templates-0.2.6/LICENSE` & `server_templates-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `server_templates-0.2.6/PKG-INFO` & `server_templates-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: server_templates
-Version: 0.2.6
+Version: 0.2.7
 Summary: templates for servers
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/server_templates
-Keywords: api,api server,http server
+Keywords: api,api server,http server,aiohttp,FastApi
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# server_templates (v0.2.6)
+# server_templates (v0.2.7)
 
 ## DESCRIPTION_SHORT
 templates for servers
 
 ## DESCRIPTION_LONG
 designed for keep all servers templates in one place
 
 
 ## Features
-1. server_aiohttp  
+1. server:  
+	- aiohttp (try not to use, as old)  
+	- FastApi (preferred)  
 2. client_requests item+stack  
 
 
 ********************************************************************************
 ## License
 See the [LICENSE](LICENSE) file for license rights and limitations (MIT).
```

### Comparing `server_templates-0.2.6/README.md` & `server_templates-0.2.7/server_templates.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,42 @@
-# server_templates (v0.2.6)
+Metadata-Version: 2.1
+Name: server_templates
+Version: 0.2.7
+Summary: templates for servers
+Home-page: https://github.com/centroid457/
+Author: Andrei Starichenko
+Author-email: centroid@mail.ru
+Project-URL: Source, https://github.com/centroid457/server_templates
+Keywords: api,api server,http server,aiohttp,FastApi
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Typing :: Typed
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# server_templates (v0.2.7)
 
 ## DESCRIPTION_SHORT
 templates for servers
 
 ## DESCRIPTION_LONG
 designed for keep all servers templates in one place
 
 
 ## Features
-1. server_aiohttp  
+1. server:  
+	- aiohttp (try not to use, as old)  
+	- FastApi (preferred)  
 2. client_requests item+stack  
 
 
 ********************************************************************************
 ## License
 See the [LICENSE](LICENSE) file for license rights and limitations (MIT).
```

### Comparing `server_templates-0.2.6/server_templates/client_requests.py` & `server_templates-0.2.7/server_templates/client_requests.py`

 * *Files identical despite different names*

### Comparing `server_templates-0.2.6/server_templates/server_aiohttp/main.py` & `server_templates-0.2.7/server_templates/server_aiohttp/main.py`

 * *Files identical despite different names*

### Comparing `server_templates-0.2.6/setup.py` & `server_templates-0.2.7/setup.py`

 * *Files identical despite different names*

