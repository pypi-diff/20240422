# Comparing `tmp/common-tools-ai-bnq-0.0.5.tar.gz` & `tmp/common-tools-ai-bnq-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-tools-ai-bnq-0.0.5.tar", last modified: Fri Apr 19 09:47:25 2024, max compression
+gzip compressed data, was "common-tools-ai-bnq-0.0.6.tar", last modified: Mon Apr 22 07:58:41 2024, max compression
```

## Comparing `common-tools-ai-bnq-0.0.5.tar` & `common-tools-ai-bnq-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 09:47:25.536304 common-tools-ai-bnq-0.0.5/
--rw-rw-rw-   0        0        0      288 2024-04-19 09:47:25.535684 common-tools-ai-bnq-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-03-27 09:01:03.000000 common-tools-ai-bnq-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 09:47:25.515611 common-tools-ai-bnq-0.0.5/bnq_py_core/
--rw-rw-rw-   0        0        0      122 2024-03-27 09:34:31.000000 common-tools-ai-bnq-0.0.5/bnq_py_core/__init__.py
--rw-rw-rw-   0        0        0     4574 2024-04-19 09:14:08.000000 common-tools-ai-bnq-0.0.5/bnq_py_core/logger_record.py
--rw-rw-rw-   0        0        0     3955 2024-04-19 09:44:48.000000 common-tools-ai-bnq-0.0.5/bnq_py_core/nacos_connect.py
--rw-rw-rw-   0        0        0     2074 2024-04-19 07:39:44.000000 common-tools-ai-bnq-0.0.5/bnq_py_core/read_conf_from_ini.py
--rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.0.5/bnq_py_core/singleton.py
-drwxrwxrwx   0        0        0        0 2024-04-19 09:47:25.531606 common-tools-ai-bnq-0.0.5/common_tools_ai_bnq.egg-info/
--rw-rw-rw-   0        0        0      288 2024-04-19 09:47:25.000000 common-tools-ai-bnq-0.0.5/common_tools_ai_bnq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-04-19 09:47:25.000000 common-tools-ai-bnq-0.0.5/common_tools_ai_bnq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 09:47:25.000000 common-tools-ai-bnq-0.0.5/common_tools_ai_bnq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-19 09:47:25.000000 common-tools-ai-bnq-0.0.5/common_tools_ai_bnq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-19 09:47:25.000000 common-tools-ai-bnq-0.0.5/common_tools_ai_bnq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 09:47:25.536304 common-tools-ai-bnq-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      590 2024-04-19 09:47:18.000000 common-tools-ai-bnq-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 09:47:25.534691 common-tools-ai-bnq-0.0.5/test/
--rw-rw-rw-   0        0        0      122 2024-04-10 03:16:38.000000 common-tools-ai-bnq-0.0.5/test/__init__.py
--rw-rw-rw-   0        0        0    27286 2024-04-10 03:37:31.000000 common-tools-ai-bnq-0.0.5/test/test_batch_triton.py
--rw-rw-rw-   0        0        0     3464 2024-04-10 07:43:55.000000 common-tools-ai-bnq-0.0.5/test/test_decorator.py
--rw-rw-rw-   0        0        0      897 2024-04-16 08:13:06.000000 common-tools-ai-bnq-0.0.5/test/test_pymysql.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:58:41.007823 common-tools-ai-bnq-0.0.6/
+-rw-rw-rw-   0        0        0      288 2024-04-22 07:58:41.006823 common-tools-ai-bnq-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-03-27 09:01:03.000000 common-tools-ai-bnq-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 07:58:40.989713 common-tools-ai-bnq-0.0.6/bnq_py_core/
+-rw-rw-rw-   0        0        0      122 2024-03-27 09:34:31.000000 common-tools-ai-bnq-0.0.6/bnq_py_core/__init__.py
+-rw-rw-rw-   0        0        0     4574 2024-04-19 09:14:08.000000 common-tools-ai-bnq-0.0.6/bnq_py_core/logger_record.py
+-rw-rw-rw-   0        0        0     3561 2024-04-22 07:58:02.000000 common-tools-ai-bnq-0.0.6/bnq_py_core/nacos_connect.py
+-rw-rw-rw-   0        0        0     2074 2024-04-19 07:39:44.000000 common-tools-ai-bnq-0.0.6/bnq_py_core/read_conf_from_ini.py
+-rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.0.6/bnq_py_core/singleton.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:58:41.000713 common-tools-ai-bnq-0.0.6/common_tools_ai_bnq.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-04-22 07:58:40.000000 common-tools-ai-bnq-0.0.6/common_tools_ai_bnq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2024-04-22 07:58:40.000000 common-tools-ai-bnq-0.0.6/common_tools_ai_bnq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 07:58:40.000000 common-tools-ai-bnq-0.0.6/common_tools_ai_bnq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-22 07:58:40.000000 common-tools-ai-bnq-0.0.6/common_tools_ai_bnq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-22 07:58:40.000000 common-tools-ai-bnq-0.0.6/common_tools_ai_bnq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 07:58:41.007823 common-tools-ai-bnq-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      590 2024-04-22 07:58:37.000000 common-tools-ai-bnq-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:58:41.005825 common-tools-ai-bnq-0.0.6/test/
+-rw-rw-rw-   0        0        0      122 2024-04-10 03:16:38.000000 common-tools-ai-bnq-0.0.6/test/__init__.py
+-rw-rw-rw-   0        0        0      221 2024-04-22 02:30:57.000000 common-tools-ai-bnq-0.0.6/test/gen_key.py
+-rw-rw-rw-   0        0        0    27286 2024-04-10 03:37:31.000000 common-tools-ai-bnq-0.0.6/test/test_batch_triton.py
+-rw-rw-rw-   0        0        0     3464 2024-04-10 07:43:55.000000 common-tools-ai-bnq-0.0.6/test/test_decorator.py
+-rw-rw-rw-   0        0        0      520 2024-04-22 07:28:44.000000 common-tools-ai-bnq-0.0.6/test/test_global.py
+-rw-rw-rw-   0        0        0      897 2024-04-16 08:13:06.000000 common-tools-ai-bnq-0.0.6/test/test_pymysql.py
```

### Comparing `common-tools-ai-bnq-0.0.5/bnq_py_core/logger_record.py` & `common-tools-ai-bnq-0.0.6/bnq_py_core/logger_record.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.5/bnq_py_core/nacos_connect.py` & `common-tools-ai-bnq-0.0.6/bnq_py_core/nacos_connect.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,14 +121,9 @@
 
 if __name__ == "__main__":
     test_data = {'group': {'t-dev': ['project_name_1', 'project_name_2']},
                  'username': 'nacos',
                  'password': 'nacos',
                  'server_addresses': '127.0.0.1:8080',
                  'namespace': 't-dev'}
-    test_data = {'group': {'DEFAULT_GROUP': ['test_data']}, 'username': 'nacos',
-                 'password': 'nacos', 'server_addresses': '10.188.12.3:8848', 'namespace': 'AI-dev'}
-
-    # test_data = {'group': {'AI-dev': ['spaceDesign', 'services_health_check']}, 'username': 'nacos',
-    #              'password': 'nacos', 'server_addresses': '10.188.12.3:8848', 'namespace': 'AI-dev'}
     conf_test = NacConnect(**test_data)
     print(conf_test())
```

### Comparing `common-tools-ai-bnq-0.0.5/bnq_py_core/read_conf_from_ini.py` & `common-tools-ai-bnq-0.0.6/bnq_py_core/read_conf_from_ini.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.5/bnq_py_core/singleton.py` & `common-tools-ai-bnq-0.0.6/bnq_py_core/singleton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.5/setup.py` & `common-tools-ai-bnq-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Author:Zhang HongTao
 # @File:setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='common-tools-ai-bnq',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
     install_requires=[
         # 依赖项列表
         'structlog==23.1.0',
         'concurrent-log-handler==0.9.22',
         'nacos-sdk-python==0.1.12',
         'PyYAML==6.0.1',
```

### Comparing `common-tools-ai-bnq-0.0.5/test/test_batch_triton.py` & `common-tools-ai-bnq-0.0.6/test/test_batch_triton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.5/test/test_decorator.py` & `common-tools-ai-bnq-0.0.6/test/test_decorator.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.5/test/test_pymysql.py` & `common-tools-ai-bnq-0.0.6/test/test_pymysql.py`

 * *Files identical despite different names*

