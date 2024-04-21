# Comparing `tmp/payconpy-2.0.0.tar.gz` & `tmp/payconpy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payconpy-2.0.0.tar", last modified: Sun Apr 21 22:04:58 2024, max compression
+gzip compressed data, was "payconpy-2.0.1.tar", last modified: Sun Apr 21 22:16:04 2024, max compression
```

## Comparing `payconpy-2.0.0.tar` & `payconpy-2.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:58.042830 payconpy-2.0.0/
--rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.0.0/LICENSE
--rw-rw-rw-   0        0        0      899 2024-04-21 22:04:58.035576 payconpy-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      456 2024-04-21 22:04:31.000000 payconpy-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.641655 payconpy-2.0.0/payconpy/
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.735283 payconpy-2.0.0/payconpy/femails/
--rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.0.0/payconpy/femails/__init__.py
--rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.0.0/payconpy/femails/femails.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.754712 payconpy-2.0.0/payconpy/fexceptions/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.768258 payconpy-2.0.0/payconpy/fpdf/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.786341 payconpy-2.0.0/payconpy/fpdf/focr/
--rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.0.0/payconpy/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0    11098 2024-03-28 19:02:26.000000 payconpy-2.0.0/payconpy/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.809365 payconpy-2.0.0/payconpy/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.0.0/payconpy/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.831306 payconpy-2.0.0/payconpy/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.0.0/payconpy/fpysimplegui/fpysimplegui.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.850868 payconpy-2.0.0/payconpy/fpython/
--rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fpython/__init__.py
--rw-rw-rw-   0        0        0    57479 2024-04-21 19:22:58.000000 payconpy-2.0.0/payconpy/fpython/fpython.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.875823 payconpy-2.0.0/payconpy/fregex/
--rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fregex/__init__.py
--rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.0.0/payconpy/fregex/fregex.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.895578 payconpy-2.0.0/payconpy/fselenium/
--rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fselenium/__init__.py
--rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.0.0/payconpy/fselenium/fselenium.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.914248 payconpy-2.0.0/payconpy/odoo/
--rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.0.0/payconpy/odoo/__init__.py
--rw-rw-rw-   0        0        0    11710 2024-04-21 21:00:14.000000 payconpy-2.0.0/payconpy/odoo/odoo_xmlrpc.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.938284 payconpy-2.0.0/payconpy/openai/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.0.0/payconpy/openai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.954964 payconpy-2.0.0/payconpy/openai/apis/
--rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.0.0/payconpy/openai/apis/__init__.py
--rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.0.0/payconpy/openai/apis/apis.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.986395 payconpy-2.0.0/payconpy/openai/assistants/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.0.0/payconpy/openai/assistants/__init__.py
--rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.0.0/payconpy/openai/assistants/assistants.py
--rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.0.0/payconpy/openai/get_cost.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:58.018143 payconpy-2.0.0/payconpy/utils/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.0.0/payconpy/utils/__init__.py
--rw-rw-rw-   0        0        0   136255 2024-04-21 22:03:25.000000 payconpy-2.0.0/payconpy/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.713002 payconpy-2.0.0/payconpy.egg-info/
--rw-rw-rw-   0        0        0      899 2024-04-21 22:04:57.000000 payconpy-2.0.0/payconpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2024-04-21 22:04:57.000000 payconpy-2.0.0/payconpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 22:04:57.000000 payconpy-2.0.0/payconpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      202 2024-04-21 22:04:57.000000 payconpy-2.0.0/payconpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      261 2024-04-21 22:04:57.000000 payconpy-2.0.0/payconpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 22:04:58.043710 payconpy-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2049 2024-04-21 22:04:07.000000 payconpy-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:04.149412 payconpy-2.0.1/
+-rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0      899 2024-04-21 22:16:04.144242 payconpy-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-04-21 22:04:31.000000 payconpy-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.598138 payconpy-2.0.1/payconpy/
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.746459 payconpy-2.0.1/payconpy/femails/
+-rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.0.1/payconpy/femails/__init__.py
+-rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.0.1/payconpy/femails/femails.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.786045 payconpy-2.0.1/payconpy/fexceptions/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.0.1/payconpy/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.0.1/payconpy/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.802402 payconpy-2.0.1/payconpy/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.0.1/payconpy/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.822501 payconpy-2.0.1/payconpy/fpdf/focr/
+-rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.0.1/payconpy/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0    11098 2024-03-28 19:02:26.000000 payconpy-2.0.1/payconpy/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.845426 payconpy-2.0.1/payconpy/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.0.1/payconpy/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.0.1/payconpy/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.866389 payconpy-2.0.1/payconpy/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.0.1/payconpy/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.0.1/payconpy/fpysimplegui/fpysimplegui.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.888349 payconpy-2.0.1/payconpy/fpython/
+-rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.0.1/payconpy/fpython/__init__.py
+-rw-rw-rw-   0        0        0    57479 2024-04-21 19:22:58.000000 payconpy-2.0.1/payconpy/fpython/fpython.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.909661 payconpy-2.0.1/payconpy/fregex/
+-rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.0.1/payconpy/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.0.1/payconpy/fregex/fregex.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.934349 payconpy-2.0.1/payconpy/fselenium/
+-rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.0.1/payconpy/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.0.1/payconpy/fselenium/fselenium.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.953410 payconpy-2.0.1/payconpy/odoo/
+-rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.0.1/payconpy/odoo/__init__.py
+-rw-rw-rw-   0        0        0    11710 2024-04-21 21:00:14.000000 payconpy-2.0.1/payconpy/odoo/odoo_xmlrpc.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.978861 payconpy-2.0.1/payconpy/openai/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.0.1/payconpy/openai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:04.000253 payconpy-2.0.1/payconpy/openai/apis/
+-rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.0.1/payconpy/openai/apis/__init__.py
+-rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.0.1/payconpy/openai/apis/apis.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:04.028900 payconpy-2.0.1/payconpy/openai/assistants/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.0.1/payconpy/openai/assistants/__init__.py
+-rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.0.1/payconpy/openai/assistants/assistants.py
+-rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.0.1/payconpy/openai/get_cost.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:04.119681 payconpy-2.0.1/payconpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.0.1/payconpy/utils/__init__.py
+-rw-rw-rw-   0        0        0   136287 2024-04-21 22:15:49.000000 payconpy-2.0.1/payconpy/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:16:03.690184 payconpy-2.0.1/payconpy.egg-info/
+-rw-rw-rw-   0        0        0      899 2024-04-21 22:16:03.000000 payconpy-2.0.1/payconpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2024-04-21 22:16:03.000000 payconpy-2.0.1/payconpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 22:16:03.000000 payconpy-2.0.1/payconpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      202 2024-04-21 22:16:03.000000 payconpy-2.0.1/payconpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      261 2024-04-21 22:16:03.000000 payconpy-2.0.1/payconpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 22:16:04.150411 payconpy-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2049 2024-04-21 22:15:55.000000 payconpy-2.0.1/setup.py
```

### Comparing `payconpy-2.0.0/LICENSE` & `payconpy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/PKG-INFO` & `payconpy-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-2.0.0/payconpy/femails/femails.py` & `payconpy-2.0.1/payconpy/femails/femails.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/fexceptions/exceptions.py` & `payconpy-2.0.1/payconpy/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/fpdf/focr/orc.py` & `payconpy-2.0.1/payconpy/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/fpdf/pdfutils/pdfutils.py` & `payconpy-2.0.1/payconpy/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/fpysimplegui/fpysimplegui.py` & `payconpy-2.0.1/payconpy/fpysimplegui/fpysimplegui.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/fpython/fpython.py` & `payconpy-2.0.1/payconpy/fpython/fpython.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/fregex/fregex.py` & `payconpy-2.0.1/payconpy/fregex/fregex.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/fselenium/fselenium.py` & `payconpy-2.0.1/payconpy/fselenium/fselenium.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/odoo/odoo_xmlrpc.py` & `payconpy-2.0.1/payconpy/odoo/odoo_xmlrpc.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/openai/apis/apis.py` & `payconpy-2.0.1/payconpy/openai/apis/apis.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/openai/assistants/assistants.py` & `payconpy-2.0.1/payconpy/openai/assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/openai/get_cost.py` & `payconpy-2.0.1/payconpy/openai/get_cost.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/payconpy/utils/utils.py` & `payconpy-2.0.1/payconpy/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,14 +302,16 @@
 Para alcançar ambos os gostos, também deixei um código para usar uma planilha Excel, como se fosse um banco de dados.
 '''
 from payconpy.fpython.functions_for_py import *
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import Column, String, Integer
+import pandas as pd
+import os
 
 engine = create_engine('sqlite:///database.db', pool_size=15, max_overflow=20)
 Base = declarative_base()
 Session = sessionmaker(bind=engine)
 
 
 class TABLE(Base):
```

### Comparing `payconpy-2.0.0/payconpy.egg-info/PKG-INFO` & `payconpy-2.0.1/payconpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-2.0.0/payconpy.egg-info/SOURCES.txt` & `payconpy-2.0.1/payconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payconpy-2.0.0/setup.py` & `payconpy-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '2.0.0'
+version = '2.0.1'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='payconpy',
         version=version,
         url='https://github.com/githubpaycon/payconpy',
```

