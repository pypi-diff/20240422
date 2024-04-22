# Comparing `tmp/monit-agd-1.1.tar.gz` & `tmp/monit-agd-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monit-agd-1.1.tar", last modified: Mon Apr 22 01:28:05 2024, max compression
+gzip compressed data, was "monit-agd-1.1.1.tar", last modified: Mon Apr 22 01:31:58 2024, max compression
```

## Comparing `monit-agd-1.1.tar` & `monit-agd-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:28:05.191732 monit-agd-1.1/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.1/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1633 2024-04-22 01:28:05.191732 monit-agd-1.1/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      998 2024-04-22 01:18:02.000000 monit-agd-1.1/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:28:05.188399 monit-agd-1.1/monit_agd.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1633 2024-04-22 01:28:05.000000 monit-agd-1.1/monit_agd.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      190 2024-04-22 01:28:05.000000 monit-agd-1.1/monit_agd.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-22 01:28:05.000000 monit-agd-1.1/monit_agd.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-22 01:28:05.000000 monit-agd-1.1/monit_agd.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-22 01:28:05.000000 monit-agd-1.1/monit_agd.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-22 01:28:05.191732 monit-agd-1.1/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-04-22 01:27:53.000000 monit-agd-1.1/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:31:58.056604 monit-agd-1.1.1/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 monit-agd-1.1.1/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1591 2024-04-22 01:31:58.056604 monit-agd-1.1.1/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      954 2024-04-22 01:31:52.000000 monit-agd-1.1.1/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:31:58.056604 monit-agd-1.1.1/monit_agd.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1591 2024-04-22 01:31:57.000000 monit-agd-1.1.1/monit_agd.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      190 2024-04-22 01:31:58.000000 monit-agd-1.1.1/monit_agd.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-22 01:31:57.000000 monit-agd-1.1.1/monit_agd.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-04-22 01:31:57.000000 monit-agd-1.1.1/monit_agd.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-04-22 01:31:57.000000 monit-agd-1.1.1/monit_agd.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-04-22 01:31:58.056604 monit-agd-1.1.1/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      867 2024-04-22 01:31:28.000000 monit-agd-1.1.1/setup.py
```

### Comparing `monit-agd-1.1/LICENSE` & `monit-agd-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `monit-agd-1.1/PKG-INFO` & `monit-agd-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.1
+Version: 1.1.1
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Requires-Dist: psutil
 Requires-Dist: python-dotenv
 
 ### Monit
 
 **Instalação:**
 ```bash
-pip install git+https://github.com/Agencia-de-Dados-bsb/monit.git
+pip install monit-agd
 ```
 **Exemplo arquivo `.env`:**
 ```bash
 # Project info
 PROJECT=sample_project
 COMPANY=acme
 LOCATION=ec2
```

### Comparing `monit-agd-1.1/README.md` & `monit-agd-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### Monit
 
 **Instalação:**
 ```bash
-pip install git+https://github.com/Agencia-de-Dados-bsb/monit.git
+pip install monit-agd
 ```
 **Exemplo arquivo `.env`:**
 ```bash
 # Project info
 PROJECT=sample_project
 COMPANY=acme
 LOCATION=ec2
```

### Comparing `monit-agd-1.1/monit_agd.egg-info/PKG-INFO` & `monit-agd-1.1.1/monit_agd.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monit-agd
-Version: 1.1
+Version: 1.1.1
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Requires-Dist: psutil
 Requires-Dist: python-dotenv
 
 ### Monit
 
 **Instalação:**
 ```bash
-pip install git+https://github.com/Agencia-de-Dados-bsb/monit.git
+pip install monit-agd
 ```
 **Exemplo arquivo `.env`:**
 ```bash
 # Project info
 PROJECT=sample_project
 COMPANY=acme
 LOCATION=ec2
```

### Comparing `monit-agd-1.1/setup.py` & `monit-agd-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='monit-agd',
-    version='1.1',
+    version='1.1.1',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

