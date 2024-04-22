# Comparing `tmp/rds-core-0.2.4.tar.gz` & `tmp/rds-core-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds-core-0.2.4.tar", last modified: Tue Mar 19 17:01:59 2024, max compression
+gzip compressed data, was "rds-core-0.2.5.tar", last modified: Mon Apr 22 00:12:23 2024, max compression
```

## Comparing `rds-core-0.2.4.tar` & `rds-core-0.2.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.669094 rds-core-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-19 17:01:50.000000 rds-core-0.2.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-19 17:01:59.669094 rds-core-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-19 17:01:50.000000 rds-core-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-19 17:01:50.000000 rds-core-0.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.661094 rds-core-0.2.4/rds/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/contrib/datasus/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/contrib/datasus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/contrib/datasus/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/contrib/datasus/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/contrib/datasus/transformers/fields/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/contrib/datasus/transformers/fields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/core/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/cache/inmemory.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/cache/nocache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/cache/search_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/core/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/helpers/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/core/searchengine/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/searchengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/core/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/core/transformers/fields/
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/transformers/fields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/core/transformers/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/transformers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/core/types/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.665094 rds-core-0.2.4/rds/core/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-19 17:01:50.000000 rds-core-0.2.4/rds/core/validators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:01:59.669094 rds-core-0.2.4/rds_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-19 17:01:59.000000 rds-core-0.2.4/rds_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-19 17:01:59.000000 rds-core-0.2.4/rds_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 17:01:59.000000 rds-core-0.2.4/rds_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-19 17:01:59.000000 rds-core-0.2.4/rds_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-19 17:01:59.000000 rds-core-0.2.4/rds_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-19 17:01:59.669094 rds-core-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-19 17:01:50.000000 rds-core-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 00:12:13.000000 rds-core-0.2.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-22 00:12:23.879859 rds-core-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-22 00:12:13.000000 rds-core-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-22 00:12:13.000000 rds-core-0.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.875859 rds-core-0.2.5/rds/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.875859 rds-core-0.2.5/rds/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/contrib/datasus/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/contrib/datasus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/contrib/datasus/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/contrib/datasus/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/contrib/datasus/transformers/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/contrib/datasus/transformers/fields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/cache/inmemory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/cache/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/cache/search_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/helpers/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/core/searchengine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/searchengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/core/transformers/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/transformers/fields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/core/transformers/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/transformers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/core/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds/core/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-22 00:12:13.000000 rds-core-0.2.5/rds/core/validators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:12:23.879859 rds-core-0.2.5/rds_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-22 00:12:23.000000 rds-core-0.2.5/rds_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-22 00:12:23.000000 rds-core-0.2.5/rds_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 00:12:23.000000 rds-core-0.2.5/rds_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-22 00:12:23.000000 rds-core-0.2.5/rds_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 00:12:23.000000 rds-core-0.2.5/rds_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-22 00:12:23.879859 rds-core-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-22 00:12:13.000000 rds-core-0.2.5/setup.py
```

### Comparing `rds-core-0.2.4/PKG-INFO` & `rds-core-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rds-core
-Version: 0.2.4
+Version: 0.2.5
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: https://github.com/lais-huol/rds-core
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Download-URL: https://github.com/lais-huol/rds-core/tags
 Description: É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
```

### Comparing `rds-core-0.2.4/README.md` & `rds-core-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/pyproject.toml` & `rds-core-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/contrib/datasus/transformers/fields/__init__.py` & `rds-core-0.2.5/rds/contrib/datasus/transformers/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/__init__.py` & `rds-core-0.2.5/rds/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/cache/__init__.py` & `rds-core-0.2.5/rds/core/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/cache/base.py` & `rds-core-0.2.5/rds/core/cache/base.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/cache/inmemory.py` & `rds-core-0.2.5/rds/core/cache/inmemory.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/cache/nocache.py` & `rds-core-0.2.5/rds/core/cache/nocache.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/cache/search_engine.py` & `rds-core-0.2.5/rds/core/cache/search_engine.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/helpers/__init__.py` & `rds-core-0.2.5/rds/core/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/helpers/http_client.py` & `rds-core-0.2.5/rds/core/helpers/http_client.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/searchengine/__init__.py` & `rds-core-0.2.5/rds/core/searchengine/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/transformers/fields/__init__.py` & `rds-core-0.2.5/rds/core/transformers/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/transformers/models/__init__.py` & `rds-core-0.2.5/rds/core/transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds/core/validators/__init__.py` & `rds-core-0.2.5/rds/core/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/rds_core.egg-info/PKG-INFO` & `rds-core-0.2.5/rds_core.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rds-core
-Version: 0.2.4
+Version: 0.2.5
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: https://github.com/lais-huol/rds-core
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Download-URL: https://github.com/lais-huol/rds-core/tags
 Description: É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
```

### Comparing `rds-core-0.2.4/rds_core.egg-info/SOURCES.txt` & `rds-core-0.2.5/rds_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.4/setup.py` & `rds-core-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 with open("requirements.txt", "w") as file1:
     for requirement in requirements:
         file1.write(f"{requirement}\n")
 
 setup(
     name="rds-core",
-    version="0.2.4",
+    version="0.2.5",
     description="Framework para serviços do Rede de Dados em Saúde do LAIS",
     long_description="É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o"
     " desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de"
     " Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias"
     " RDS, a exemplo RDS-RN e RDS-ES.",
     author="Kelson da Costa Medeiros",
     author_email="kelson.medeiros@lais.huol.ufrn.br",
```

