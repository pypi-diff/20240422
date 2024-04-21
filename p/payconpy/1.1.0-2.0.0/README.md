# Comparing `tmp/payconpy-1.1.0.tar.gz` & `tmp/payconpy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payconpy-1.1.0.tar", last modified: Mon Apr  1 13:53:37 2024, max compression
+gzip compressed data, was "payconpy-2.0.0.tar", last modified: Sun Apr 21 22:04:58 2024, max compression
```

## Comparing `payconpy-1.1.0.tar` & `payconpy-2.0.0.tar`

### file list

```diff
@@ -1,48 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.181572 payconpy-1.1.0/
--rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      889 2024-04-01 13:53:37.178408 payconpy-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-03-28 18:37:05.000000 payconpy-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:36.999882 payconpy-1.1.0/payconpy/
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.055515 payconpy-1.1.0/payconpy/femails/
--rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-1.1.0/payconpy/femails/__init__.py
--rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-1.1.0/payconpy/femails/femails.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.067155 payconpy-1.1.0/payconpy/fexceptions/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.072311 payconpy-1.1.0/payconpy/fpdf/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.082553 payconpy-1.1.0/payconpy/fpdf/focr/
--rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-1.1.0/payconpy/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0    11098 2024-03-28 19:02:26.000000 payconpy-1.1.0/payconpy/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.093170 payconpy-1.1.0/payconpy/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3310 2024-03-28 18:06:39.000000 payconpy-1.1.0/payconpy/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.103078 payconpy-1.1.0/payconpy/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-1.1.0/payconpy/fpysimplegui/fpysimplegui.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.114686 payconpy-1.1.0/payconpy/fpython/
--rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fpython/__init__.py
--rw-rw-rw-   0        0        0    56234 2024-03-28 17:58:09.000000 payconpy-1.1.0/payconpy/fpython/fpython.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.126410 payconpy-1.1.0/payconpy/fregex/
--rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fregex/__init__.py
--rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-1.1.0/payconpy/fregex/fregex.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.137122 payconpy-1.1.0/payconpy/fselenium/
--rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-1.1.0/payconpy/fselenium/__init__.py
--rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-1.1.0/payconpy/fselenium/fselenium.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.148860 payconpy-1.1.0/payconpy/openai/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-1.1.0/payconpy/openai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.156086 payconpy-1.1.0/payconpy/openai/assistants/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-1.1.0/payconpy/openai/assistants/__init__.py
--rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-1.1.0/payconpy/openai/assistants/assistants.py
--rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-1.1.0/payconpy/openai/get_cost.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.168823 payconpy-1.1.0/payconpy/utils/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-1.1.0/payconpy/utils/__init__.py
--rw-rw-rw-   0        0        0   133129 2024-03-28 18:54:30.000000 payconpy-1.1.0/payconpy/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:53:37.045467 payconpy-1.1.0/payconpy.egg-info/
--rw-rw-rw-   0        0        0      889 2024-04-01 13:53:36.000000 payconpy-1.1.0/payconpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      896 2024-04-01 13:53:36.000000 payconpy-1.1.0/payconpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 13:53:36.000000 payconpy-1.1.0/payconpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      202 2024-04-01 13:53:36.000000 payconpy-1.1.0/payconpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      226 2024-04-01 13:53:36.000000 payconpy-1.1.0/payconpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 13:53:37.182099 payconpy-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1945 2024-04-01 13:53:27.000000 payconpy-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:58.042830 payconpy-2.0.0/
+-rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      899 2024-04-21 22:04:58.035576 payconpy-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-04-21 22:04:31.000000 payconpy-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.641655 payconpy-2.0.0/payconpy/
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.735283 payconpy-2.0.0/payconpy/femails/
+-rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.0.0/payconpy/femails/__init__.py
+-rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.0.0/payconpy/femails/femails.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.754712 payconpy-2.0.0/payconpy/fexceptions/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.768258 payconpy-2.0.0/payconpy/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.786341 payconpy-2.0.0/payconpy/fpdf/focr/
+-rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.0.0/payconpy/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0    11098 2024-03-28 19:02:26.000000 payconpy-2.0.0/payconpy/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.809365 payconpy-2.0.0/payconpy/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.0.0/payconpy/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.831306 payconpy-2.0.0/payconpy/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.0.0/payconpy/fpysimplegui/fpysimplegui.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.850868 payconpy-2.0.0/payconpy/fpython/
+-rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fpython/__init__.py
+-rw-rw-rw-   0        0        0    57479 2024-04-21 19:22:58.000000 payconpy-2.0.0/payconpy/fpython/fpython.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.875823 payconpy-2.0.0/payconpy/fregex/
+-rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.0.0/payconpy/fregex/fregex.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.895578 payconpy-2.0.0/payconpy/fselenium/
+-rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.0.0/payconpy/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.0.0/payconpy/fselenium/fselenium.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.914248 payconpy-2.0.0/payconpy/odoo/
+-rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.0.0/payconpy/odoo/__init__.py
+-rw-rw-rw-   0        0        0    11710 2024-04-21 21:00:14.000000 payconpy-2.0.0/payconpy/odoo/odoo_xmlrpc.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.938284 payconpy-2.0.0/payconpy/openai/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.0.0/payconpy/openai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.954964 payconpy-2.0.0/payconpy/openai/apis/
+-rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.0.0/payconpy/openai/apis/__init__.py
+-rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.0.0/payconpy/openai/apis/apis.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.986395 payconpy-2.0.0/payconpy/openai/assistants/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.0.0/payconpy/openai/assistants/__init__.py
+-rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.0.0/payconpy/openai/assistants/assistants.py
+-rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.0.0/payconpy/openai/get_cost.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:58.018143 payconpy-2.0.0/payconpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.0.0/payconpy/utils/__init__.py
+-rw-rw-rw-   0        0        0   136255 2024-04-21 22:03:25.000000 payconpy-2.0.0/payconpy/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:04:57.713002 payconpy-2.0.0/payconpy.egg-info/
+-rw-rw-rw-   0        0        0      899 2024-04-21 22:04:57.000000 payconpy-2.0.0/payconpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2024-04-21 22:04:57.000000 payconpy-2.0.0/payconpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 22:04:57.000000 payconpy-2.0.0/payconpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      202 2024-04-21 22:04:57.000000 payconpy-2.0.0/payconpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      261 2024-04-21 22:04:57.000000 payconpy-2.0.0/payconpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 22:04:58.043710 payconpy-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2049 2024-04-21 22:04:07.000000 payconpy-2.0.0/setup.py
```

### Comparing `payconpy-1.1.0/LICENSE` & `payconpy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `payconpy-1.1.0/PKG-INFO` & `payconpy-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 1.1.0
+Version: 2.0.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
@@ -16,15 +16,16 @@
 ## pip install payconpy | NECESSARIO PYTHON 3.10
 
 Aqui voce achara funcoes produzidas para ter maior agilidade nos desenvolvimentos nas tecnologias abaixo:
 
 * Selenium
 * Tesseract
 * Python
+* OpenAI
 
 ## Instalacao
 
 pip install payconpy em seu ambiente virtual e pronto!
 
 Powered By: [Paycon Automações](https://github.com/Paycon-Automacoes)
 
-# Current Version -> 1.0.0
+# Current Version -> 2.0.0
```

### Comparing `payconpy-1.1.0/payconpy/femails/femails.py` & `payconpy-2.0.0/payconpy/femails/femails.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.1.0/payconpy/fexceptions/exceptions.py` & `payconpy-2.0.0/payconpy/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.1.0/payconpy/fpdf/focr/orc.py` & `payconpy-2.0.0/payconpy/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.1.0/payconpy/fpysimplegui/fpysimplegui.py` & `payconpy-2.0.0/payconpy/fpysimplegui/fpysimplegui.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.1.0/payconpy/fpython/fpython.py` & `payconpy-2.0.0/payconpy/fpython/fpython.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,89 @@
 """
 ## Várias funções para ajudar no desenvolvimento de qualquer aplicação em Python
 
 ### Nesse módulo você achará desde funções simples, até funções complexas que levariam um bom tempo para desenvolve-las.
 """
 
 ################################## IMPORTS #############################################
+import os, sys, shutil, platform, re, logging,\
+    unicodedata, gc, requests, time, json,\
+        threading, base64, random, uuid
 from configparser import RawConfigParser
 from datetime import datetime, date, timedelta
 from fnmatch import fnmatch
 from time import sleep
-import os, sys, shutil, platform, re, logging, unicodedata, gc, requests, time, json, threading
 import subprocess as sp
 import zipfile
 from rich import print
 from numpy import unicode_
 ################################## IMPORTS #############################################
 
-def remover_acentos(text:str, encoding:str='utf-8'):
+def generate_uuid() -> str:
+    """Generate uuid
+
+    Returns:
+        str: uuid
+    """
+    return str(uuid.uuid4())
+
+def file_to_base64(file) -> str:
+    """Convert any file to base64
+
+    Args:
+        file (str): File to convert (path)
+
+    Returns:
+        str: file represented in base64
+    """
+    with open(os.path.abspath(file), "rb") as arquivo:
+        base64_ = base64.b64encode(arquivo.read())
+        return base64_.decode("utf-8")
+
+def base64_to_file(base64_string:str, output_file:str) -> None:
+    """Convert any base64 to file
+
+    Args:
+        base64_string (str): base64 represented in string
+        base64_string (str): File to convert (path)
+
+    Returns:
+        None: None
+    """
+    with open(output_file, "wb") as f:
+        image_data = base64.b64decode(base64_string)
+        f.write(image_data)
+
+def random_sleep(min, max) -> None:
+    """Run a random sleep when searching for requests to avoid IP blocks
+
+    Args:
+        min (int|float): Min value to sleep
+        max (int|float): Max value to sleep
+    """
+    sleep(random.uniform(min, max))
+
+def remover_acentos(text:str, encoding:str='utf-8') -> str:
 	try:
 		text = unicode_(text, encoding=encoding)
 	except Exception:
 		pass
 	text = unicodedata.normalize('NFD', text).encode('ascii', 'ignore').decode("utf-8")
 	return str(text)
 
-def getsizefile(path_file:str, return_convet_bytes: bool=False):
+def getsizefile(path_file:str, return_convet_bytes: bool=False) -> int|str:
     """
-    Função retorna o valor da função os.path.getsize()
+    getsizefile in bytes, KB, MB, GB, TB, PB
     
     Args:
-        path_file (str): O caminho do arquivo relativo
-        return_convet_bytes (str): Converte o valor de bits para  B = Byte K = Kilo M = Mega G = Giga T = Tera P = Peta
-        
+        path_file (str): Relative path of the file
+        return_convet_bytes (str): convert the value of bits -> B = Byte K = Kilo M = Mega G = Giga T = Tera P = Peta
+    
+    Returns:
+        int|str: Value of the function os.path.getsize()
     """
     FILE_PATH_ABSOLUTE = os.path.getsize(os.path.abspath(path_file))
     if return_convet_bytes:
         return convert_bytes(FILE_PATH_ABSOLUTE)
     return FILE_PATH_ABSOLUTE
 
 def executa_garbage_collector(generation :int=False) -> int:
@@ -60,28 +108,28 @@
     """
     if generation:
         return gc.collect(generation)
     else:
         return gc.collect()
 
 
-def verifica_se_esta_conectado_na_vpn(ping_host :str):
+def verifica_se_esta_conectado_na_vpn(ping_host :str) -> None:
     PING_HOST = ping_host
     """O método verificará por ping se está conectado no ip da VPN"""
 
     faz_log('Verificando se VPN está ativa pelo IP enviado no config.ini')
     
     output = sp.getoutput(f'ping {PING_HOST} -n 1')  # -n 1 limita a saída
     if ('Esgotado o tempo' in output) or ('time out' in output):
         faz_log('VPN NÃO CONECTADA!', 'w')
     else:
         faz_log("VPN conectada com sucesso!")
 
 
-def transforma_lista_em_string(lista :list):
+def transforma_lista_em_string(lista :list) -> str:
     try:
         return ', '.join(lista)
     except TypeError:
         lista = [str(i) for i in lista]
         return ', '.join(lista)
```

### Comparing `payconpy-1.1.0/payconpy/fregex/fregex.py` & `payconpy-2.0.0/payconpy/fregex/fregex.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.1.0/payconpy/fselenium/fselenium.py` & `payconpy-2.0.0/payconpy/fselenium/fselenium.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.1.0/payconpy/openai/assistants/assistants.py` & `payconpy-2.0.0/payconpy/openai/assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.1.0/payconpy/openai/get_cost.py` & `payconpy-2.0.0/payconpy/openai/get_cost.py`

 * *Files identical despite different names*

### Comparing `payconpy-1.1.0/payconpy/utils/utils.py` & `payconpy-2.0.0/payconpy/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,32 +110,22 @@
             except:
                 pass
             linha += 1
         else:
             print('Foi encontrado a coluna...')
             return df
 
-def cria_diretorios_para_novo_projeto_python(with_draft=False, create_base_dir:bool=True, packages:str='payconpy'):
-    """# ATENÇÃO, UTILIZAR SOMENTE UMA VEZ NO MOMENTO DA CRIAÇÃO DO NOVO PROJETO!
+def cria_diretorios_para_novo_projeto_python(create_base_dir:bool=True, packages:str='payconpy'):
+    """
+    # ATENÇÃO, UTILIZAR SOMENTE UMA VEZ NO MOMENTO DA CRIAÇÃO DO NOVO PROJETO!
+    
+    ## A 
     
     create_base_dir: cria o diretorio para o user colocar a base
     packages: instala pacotes necessários
-    
-    o resultado esperado no arquivo app.py é:
-    
->>> from src.base.base import *
->>> class RobotClass(Bot):
->>>     def __init__(self) -> None:
->>>         self.configs = read_json(CONFIG_PATH)
->>>         self.HEADLESS = self.configs['BOT']['HEADLESS']
->>>         self.DOWNLOAD_FILES = False
->>>         super().__init__(self.HEADLESS, self.DOWNLOAD_FILES)
->>> 
->>>     def run(self):
->>>         self.DRIVER.get("https://google.com.br")  # aqui já está usando selenium dando get
     """
     faz_log('Criando pasta e arquivo de logs com esse log...')
     # cria diretório src
     cria_dir_no_dir_de_trabalho_atual('src')
     APP_PATH = arquivo_com_caminho_absoluto(['src', 'app'], 'app.py')
     BASE_PATH = arquivo_com_caminho_absoluto(['src', 'base'], 'base.py')
     DATABASE_PATH = arquivo_com_caminho_absoluto(['src', 'database'], 'database.py')
@@ -146,53 +136,53 @@
     # cria subdiretorios do src
 
         # CRIA ARQUIVO PYTHON EM SRC\\APP
     with open(APP_PATH, 'w', encoding='utf-8') as f:
         f.write("""from src.base.base import *
 class RobotClass(Bot):
     def __init__(self) -> None:
-        self.configs = read_json(CONFIG_PATH)
-        self.HEADLESS = self.configs['BOT']['HEADLESS']
-        self.DOWNLOAD_FILES = False
-        super().__init__(self.HEADLESS, self.DOWNLOAD_FILES)
+        self.configs = read_json(CONFIG_PATH)  # get configs from bin/config.json
+        self.HEADLESS = self.configs['BOT']['HEADLESS'] # default is False
+        self.DOWNLOAD_FILES = False  # Not add chromeoption (--kiosk-printing) for download files
+        super().__init__(self.HEADLESS, self.DOWNLOAD_FILES, rotate_user_agent=False)  # inherit from Bot class
 
     def run(self):
-        self.DRIVER.get("https://google.com.br")  # aqui já está usando selenium dando get
+        self.DRIVER.get("https://google.com.br")  # here, use selenium for get
+        
     """)
 
 
     # CRIA ARQUIVO PYTHON EM base
     with open(BASE_PATH, 'w', encoding='utf-8') as f:
         f.write("""from selenium.webdriver import Chrome
 from selenium import webdriver
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.common.exceptions import *
 from webdriver_manager.chrome import ChromeDriverManager
-from payconpy.fpython.functions_for_py import *
-from payconpy.fselenium.functions_selenium import *
-from payconpy.fwinotify.fwinotify import *
-from payconpy.fregex.functions_re import *
+from payconpy.fpython.fpython import *
+from payconpy.fselenium.fselenium import *
+from payconpy.fregex.fregex import *
 import pandas as pd
 import json
 import os
 
 # -- GLOBAL -- #
 URL_SUPORTE = f'https://api.whatsapp.com/send?phone=5511985640273'
 CONFIG_PATH = arquivo_com_caminho_absoluto('bin', 'config.json')
 BASE = os.path.abspath('base')
 DOWNLOAD_DIR =  cria_dir_no_dir_de_trabalho_atual(dir='downloads', print_value=False, criar_diretorio=True)
 limpa_diretorio(DOWNLOAD_DIR)
 # -- GLOBAL -- #
 
 class Bot:    
-    def __init__(self, headless, download_files) -> None:
+    def __init__(self, headless, download_files, rotate_user_agent=False) -> None:
         # --- CHROME OPTIONS --- #
         self._options = ChromeOptions()
         
         if download_files:
             # --- PATH BASE DIR --- #
             self._SETTINGS_SAVE_AS_PDF = {
                         "recentDestinations": [
@@ -203,89 +193,119 @@
                             }
                         ],
                         "selectedDestinationId": "Save as PDF",
                         "version": 2,
                     }
 
 
-            self._PROFILE = {'printing.print_preview_sticky_settings.appState': json.dumps(self._SETTINGS_SAVE_AS_PDF),
-                    "savefile.default_directory":  f"{DOWNLOAD_DIR}",
-                    "download.default_directory":  f"{DOWNLOAD_DIR}",
-                    "download.prompt_for_download": False,
-                    "download.directory_upgrade": True,
-                    # "profile.managed_default_content_settings.images": 2,
-                    "safebrowsing.enabled": True}
+            self._PROFILE = {
+                        'printing.print_preview_sticky_settings.appState': json.dumps(self._SETTINGS_SAVE_AS_PDF),
+                        "savefile.default_directory":  f"{DOWNLOAD_DIR}",
+                        "download.default_directory":  f"{DOWNLOAD_DIR}",
+                        "download.prompt_for_download": False,
+                        "download.directory_upgrade": True,
+                        # "profile.managed_default_content_settings.images": 2,
+                        "safebrowsing.enabled": True
+                    }
                 
             self._options.add_experimental_option('prefs', self._PROFILE)
+            self._options.add_argument('--kiosk-printing')  # activate for download files
         
         if headless == True:
             self._options.add_argument('--headless')
+            self._options.add_argument('--disable-gpu')
+            self._options.add_argument("--no-sandbox")
             
         self._options.add_experimental_option("excludeSwitches", ["enable-logging", "enable-automation"])
         self._options.add_experimental_option('useAutomationExtension', False)
-        self.user_agent = cria_user_agent()
-        self._options.add_argument(f"--user-agent={self.user_agent}")
+        if rotate_user_agent:
+            self.user_agent = cria_user_agent()
+            self._options.add_argument(f"--user-agent={self.user_agent}")
         self._options.add_argument("--disable-web-security")
         self._options.add_argument("--allow-running-insecure-content")
         self._options.add_argument("--disable-extensions")
         self._options.add_argument("--start-maximized")
-        self._options.add_argument("--no-sandbox")
         self._options.add_argument("--disable-setuid-sandbox")
         self._options.add_argument("--disable-infobars")
         self._options.add_argument("--disable-webgl")
         self._options.add_argument("--disable-popup-blocking")
-        self._options.add_argument('--disable-gpu')
         self._options.add_argument('--disable-software-rasterizer')
         self._options.add_argument('--no-proxy-server')
         self._options.add_argument("--proxy-server='direct://'")
         self._options.add_argument('--proxy-bypass-list=*')
         self._options.add_argument('--disable-dev-shm-usage')
         self._options.add_argument('--block-new-web-contents')
-        self._options.add_argument('--incognito')
         self._options.add_argument('-–disable-notifications')
         self._options.add_argument("--window-size=1920,1080")
-        self._options.add_argument('--kiosk-printing')
 
         
         self.__service = Service(ChromeDriverManager().install())
         
         # create DRIVER
         self.DRIVER = Chrome(service=self.__service, options=self._options)
         
         def enable_download_in_headless_chrome(driver, download_dir):
             '''
-            Esse código adiciona suporte ao navegador Chrome sem interface gráfica (headless) no Selenium WebDriver para permitir o download automático de arquivos em um diretório especificado.
-
-            Mais especificamente, o código adiciona um comando ausente "send_command" ao executor de comando do driver e, em seguida, executa um comando "Page.setDownloadBehavior" para permitir o download automático de arquivos no diretório especificado.
-
-            O primeiro passo é necessário porque o suporte para o comando "send_command" não está incluído no Selenium WebDriver por padrão. O segundo passo usa o comando "Page.setDownloadBehavior" do Chrome DevTools Protocol para permitir o download automático de arquivos em um diretório especificado.
-
-            Em resumo, o código adiciona suporte para o download automático de arquivos em um diretório especificado no Chrome sem interface gráfica usando o Selenium WebDriver.
+            This code adds headless Chrome browser support to Selenium WebDriver to allow automatic downloading of files to a specified directory.
+            More specifically, the code adds a missing "send_command" command to the driver's command executor and then executes a "Page.setDownloadBehavior" command to allow automatic downloading of files to the specified directory.
+            The first step is necessary because support for the "send_command" command is not included in Selenium WebDriver by default. The second step uses the Chrome DevTools Protocol "Page.setDownloadBehavior" command to allow automatic downloading of files to a specified directory.
+            In short, the code adds support for automatically downloading files to a specified directory in GUI-less Chrome using Selenium WebDriver.
             '''
             driver.command_executor._commands["send_command"] = ("POST", '/session/$sessionId/chromium/send_command')
 
             params = {'cmd': 'Page.setDownloadBehavior', 'params': {'behavior': 'allow', 'downloadPath': download_dir}}
             command_result = driver.execute("send_command", params)
         enable_download_in_headless_chrome(self.DRIVER, DOWNLOAD_DIR)
         
         
-        self.WDW3 = WebDriverWait(self.DRIVER, timeout=3)
-        self.WDW5 = WebDriverWait(self.DRIVER, timeout=5)
-        self.WDW7 = WebDriverWait(self.DRIVER, timeout=7)
+        self.WDW2 = WebDriverWait(self.DRIVER, timeout=2)
+        self.WDW4 = WebDriverWait(self.DRIVER, timeout=4)
+        self.WDW6 = WebDriverWait(self.DRIVER, timeout=6)
+        self.WDW8 = WebDriverWait(self.DRIVER, timeout=8)
         self.WDW10 = WebDriverWait(self.DRIVER, timeout=10)
+        self.WDW20 = WebDriverWait(self.DRIVER, timeout=20)
+        self.WDW25 = WebDriverWait(self.DRIVER, timeout=25)
         self.WDW30 = WebDriverWait(self.DRIVER, timeout=30)
-        self.WDW = self.WDW7
+        self.WDW35 = WebDriverWait(self.DRIVER, timeout=35)
+        self.WDW40 = WebDriverWait(self.DRIVER, timeout=40)
+        self.WDW45 = WebDriverWait(self.DRIVER, timeout=45)
+        self.WDW = self.WDW6
 
         self.DRIVER.maximize_window()
         return self.DRIVER
 """)
     
     # CRIA ARQUIVO PYTHON EM database
     with open(DATABASE_PATH, 'w', encoding='utf-8') as f:
-        f.write("""from payconpy.fpython.functions_for_py import *
+        f.write("""
+'''
+SE ESTIVER COM DÚVIDAS EM QUAL UTILIZAR, LEIA COM ATENÇÃO:
+Benefícos ao utilizar o banco de dados ao invés de uma planilha Excel
+    1. Assegura dados consistentes com regras de validação e restrições do banco.
+    2. Lida com grandes volumes de dados sem problemas de desempenho.
+    3. Suporte a transações garante segurança e consistência com múltiplos usuários executando consultas na tabela.
+    4. Consultas SQL complexas para filtragem e agregação de dados.
+    5. Facilidade para modificar esquemas e adicionar novos campos.
+    6. Integração com APIs, aplicações web e serviços.
+    7. Bancos de dados mantêm registros para auditoria e rastreamento.
+    8. Permite automatização de processos e operações em grande escala.
+
+Meleficios de usar:
+    1. Configurar e gerenciar ORMs é mais complexo que planilhas Excel.
+    2. Uso de ORMs pode exigir habilidades em SQL e programação.
+    3. Bancos de dados necessitam de recursos adicionais para operação.
+    4. Planilhas são melhores para visualizar dados de forma amigável.
+    5. Excel é mais eficiente para tarefas simples ou análises rápidas.
+    6. Planilhas permitem colaboração em tempo real com maior facilidade.
+    7. Depurar erros em ORMs pode ser mais desafiador que em planilhas.
+    8. Bancos de dados requerem atualizações frequentes e manutenção contínua.
+
+Para alcançar ambos os gostos, também deixei um código para usar uma planilha Excel, como se fosse um banco de dados.
+'''
+from payconpy.fpython.functions_for_py import *
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import Column, String, Integer
 
 engine = create_engine('sqlite:///database.db', pool_size=15, max_overflow=20)
 Base = declarative_base()
@@ -338,30 +358,66 @@
         return self.session.query(TABLE).filter_by(id=id).first()
     
 
     def get_column_status(self):
         # Retorna o registro de status com o ID fornecido da tabela. Se nenhum registro for encontrado, retorna None.
         return self.session.query(TABLE.status).all()
     
-    
+class ExcelDBManager:
+    def __init__(self, excel_file):
+        self.excel_file = excel_file
+        # Cria uma planilha se ela não existir
+        if not os.path.exists(self.excel_file):
+            df = pd.DataFrame(columns=['id', 'status', 'nome'])
+            df.to_excel(self.excel_file, index=False)
+
+    def create_item(self, status, name):
+        # Lê a planilha, encontra o próximo ID e adiciona o item
+        df = pd.read_excel(self.excel_file)
+        next_id = df['id'].max() + 1 if not df['id'].empty else 1
+        new_item = {'id': next_id, 'status': status, 'nome': name}
+        df = df.append(new_item, ignore_index=True)
+        df.to_excel(self.excel_file, index=False)
+
+    def get_item(self, item_id):
+        # Retorna o item com o ID especificado
+        df = pd.read_excel(self.excel_file)
+        item = df[df['id'] == item_id]
+        return item if not item.empty else None
+
+    def delete_item(self, item_id):
+        # Exclui o item com o ID especificado
+        df = pd.read_excel(self.excel_file)
+        df = df[df['id'] != item_id]
+        df.to_excel(self.excel_file, index=False)
+
+    def delete_all(self):
+        # Exclui todos os itens
+        df = pd.DataFrame(columns=['id', 'status', 'nome'])
+        df.to_excel(self.excel_file, index=False)
+
+    def get_column_status(self):
+        # Retorna todos os status
+        df = pd.read_excel(self.excel_file)
+        return df['status'].tolist()
 
 """)
     
     # CRIA ARQUIVO PYTHON EM exceptions
     with open(EXCEPTIONS_PATH, 'w', encoding='utf-8') as f:
         f.write("""from payconpy.fexceptions.exceptions import *
 """)
     
     # cria arquivo json
     with open(CONFIG_PATH, 'w', encoding='utf-8') as fjson:
         fjson.write("""{
     "BOT": {
         "USER": "USER",
         "PASSWORD": "PASSWORD",
-        "HEADLESS": true
+        "HEADLESS": false
         }
 }""")
         
     # cria arquivo utils
     with open(UTILS_PATH, 'w', encoding='utf-8') as fjson:
         fjson.write("""""")
 
@@ -387,15 +443,16 @@
     if create_base_dir:
         cria_dir_no_dir_de_trabalho_atual('base')
 
     print('Criando Ambiente Virtual')
     os.system('python -m venv venv')
     print('Criado!')
     print('Baixando pacotes')
-    os.system(f'.\\venv\Scripts\\pip.exe install {packages}')
+    os.system(f'.\\venv\\Scripts\\pip.exe install {packages}')
+    faz_log('LEMBRE-SE DE ATIVAR O AMBIENTE VIRTUAL CRIADO PARA NÃO USAR BIBLIOTECAS GLOBAIS PARA QUE O EXECUTÁVEL VENHA A FICAR PESADO POSTERIORMENTE', color='yellow')
 
 
 def download_file_from_github(url, save_path):
     """
     Baixa um arquivo do GitHub garantindo que o stream seja tratado corretamente,
     o que é crucial para arquivos grandes.
```

### Comparing `payconpy-1.1.0/payconpy.egg-info/PKG-INFO` & `payconpy-2.0.0/payconpy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 1.1.0
+Version: 2.0.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
@@ -16,15 +16,16 @@
 ## pip install payconpy | NECESSARIO PYTHON 3.10
 
 Aqui voce achara funcoes produzidas para ter maior agilidade nos desenvolvimentos nas tecnologias abaixo:
 
 * Selenium
 * Tesseract
 * Python
+* OpenAI
 
 ## Instalacao
 
 pip install payconpy em seu ambiente virtual e pronto!
 
 Powered By: [Paycon Automações](https://github.com/Paycon-Automacoes)
 
-# Current Version -> 1.0.0
+# Current Version -> 2.0.0
```

### Comparing `payconpy-1.1.0/payconpy.egg-info/SOURCES.txt` & `payconpy-2.0.0/payconpy.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,13 +19,17 @@
 payconpy/fpysimplegui/fpysimplegui.py
 payconpy/fpython/__init__.py
 payconpy/fpython/fpython.py
 payconpy/fregex/__init__.py
 payconpy/fregex/fregex.py
 payconpy/fselenium/__init__.py
 payconpy/fselenium/fselenium.py
+payconpy/odoo/__init__.py
+payconpy/odoo/odoo_xmlrpc.py
 payconpy/openai/__init__.py
 payconpy/openai/get_cost.py
+payconpy/openai/apis/__init__.py
+payconpy/openai/apis/apis.py
 payconpy/openai/assistants/__init__.py
 payconpy/openai/assistants/assistants.py
 payconpy/utils/__init__.py
 payconpy/utils/utils.py
```

### Comparing `payconpy-1.1.0/setup.py` & `payconpy-2.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '1.1.0'
+version = '2.0.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='payconpy',
         version=version,
         url='https://github.com/githubpaycon/payconpy',
@@ -26,14 +26,16 @@
             os.path.join('payconpy', 'fpysimplegui'),
             os.path.join('payconpy', 'fpython'),
             os.path.join('payconpy', 'fregex'),
             os.path.join('payconpy', 'fselenium'),
             os.path.join('payconpy', 'utils'),
             os.path.join('payconpy', 'openai'),
             os.path.join('payconpy', 'openai', 'assistants'),
+            os.path.join('payconpy', 'openai', 'apis'),
+            os.path.join('payconpy', 'odoo'),
         ],
         
         install_requires= [
             'selenium',
             'bs4',
             'requests',
             'html5lib',
```

