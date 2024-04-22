# Comparing `tmp/dbt-bytehouse-1.3.2.tar.gz` & `tmp/dbt-bytehouse-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-bytehouse-1.3.2.tar", last modified: Thu Feb  9 17:09:26 2023, max compression
+gzip compressed data, was "dbt-bytehouse-1.7.1.tar", last modified: Mon Apr 22 06:29:25 2024, max compression
```

## Comparing `dbt-bytehouse-1.3.2.tar` & `dbt-bytehouse-1.7.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.758738 dbt-bytehouse-1.3.2/
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)    11451 2023-02-09 17:03:39.000000 dbt-bytehouse-1.3.2/LICENSE
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)    20530 2023-02-09 17:09:26.758258 dbt-bytehouse-1.3.2/PKG-INFO
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)    19501 2023-02-09 17:03:39.000000 dbt-bytehouse-1.3.2/README.md
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.700668 dbt-bytehouse-1.3.2/dbt/
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.699877 dbt-bytehouse-1.3.2/dbt/adapters/
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.718071 dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     1229 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/__init__.py
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)      681 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/__version__.py
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     4849 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/column.py
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     5115 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/connections.py
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     2820 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/credentials.py
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     3050 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/dbclient.py
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)    14778 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/impl.py
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)    11172 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/nativeclient.py
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     2289 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/relation.py
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.701329 dbt-bytehouse-1.3.2/dbt/include/
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.719970 dbt-bytehouse-1.3.2/dbt/include/bytehouse/
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)      715 2023-02-09 17:03:35.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/__init__.py
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)       80 2023-02-09 17:03:35.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/dbt_project.yml
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.722956 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.725129 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/adapters/
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     1120 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/adapters/apply_grants.sql
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     1534 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/adapters/relation.sql
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     4956 2023-02-09 17:03:35.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/adapters.sql
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     1686 2023-02-09 17:03:35.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/catalog.sql
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.748808 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     8061 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/incremental.sql
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     2137 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/seed.sql
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     3834 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/snapshot.sql
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     7004 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/table.sql
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     1111 2023-02-09 17:03:34.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/test.sql
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     3315 2023-02-09 17:03:35.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/view.sql
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     1537 2023-02-09 17:03:35.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/persist_docs.sql
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.749932 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/schema_tests/
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     1095 2023-02-09 17:03:35.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/schema_tests/relationships.sql
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.752391 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/utils/
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)      660 2023-02-09 17:03:35.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/utils/datatypes.sql
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     2227 2023-02-09 17:03:35.000000 dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/utils/utils.sql
-drwxr-xr-x   0 rafsanmazumder   (503) staff       (20)        0 2023-02-09 17:09:26.757296 dbt-bytehouse-1.3.2/dbt_bytehouse.egg-info/
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)    20530 2023-02-09 17:09:26.000000 dbt-bytehouse-1.3.2/dbt_bytehouse.egg-info/PKG-INFO
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     1350 2023-02-09 17:09:26.000000 dbt-bytehouse-1.3.2/dbt_bytehouse.egg-info/SOURCES.txt
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)        1 2023-02-09 17:09:26.000000 dbt-bytehouse-1.3.2/dbt_bytehouse.egg-info/dependency_links.txt
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)       49 2023-02-09 17:09:26.000000 dbt-bytehouse-1.3.2/dbt_bytehouse.egg-info/requires.txt
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)        4 2023-02-09 17:09:26.000000 dbt-bytehouse-1.3.2/dbt_bytehouse.egg-info/top_level.txt
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)      367 2023-02-09 17:03:39.000000 dbt-bytehouse-1.3.2/pyproject.toml
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)       38 2023-02-09 17:09:26.758886 dbt-bytehouse-1.3.2/setup.cfg
--rw-r--r--   0 rafsanmazumder   (503) staff       (20)     3203 2023-02-09 17:03:39.000000 dbt-bytehouse-1.3.2/setup.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.554251 dbt-bytehouse-1.7.1/
+-rw-r--r--   0 bytedance   (501) staff       (20)    11451 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/LICENSE
+-rw-r--r--   0 bytedance   (501) staff       (20)    20624 2024-04-22 06:29:25.553814 dbt-bytehouse-1.7.1/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)    19501 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/README.md
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.532251 dbt-bytehouse-1.7.1/dbt/
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.531889 dbt-bytehouse-1.7.1/dbt/adapters/
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.540881 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1229 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      681 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/__version__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4847 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/column.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5147 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/connections.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2819 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/credentials.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3042 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/dbclient.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    14888 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/impl.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    11128 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/nativeclient.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2325 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/relation.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.532492 dbt-bytehouse-1.7.1/dbt/include/
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.542031 dbt-bytehouse-1.7.1/dbt/include/bytehouse/
+-rw-r--r--   0 bytedance   (501) staff       (20)      715 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)       80 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/dbt_project.yml
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.544041 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.545243 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1120 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters/apply_grants.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     1534 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters/relation.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     4956 2024-04-18 02:42:07.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     1686 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/catalog.sql
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.548554 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/
+-rw-r--r--   0 bytedance   (501) staff       (20)     8057 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/incremental.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     2137 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/seed.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     3834 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/snapshot.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     7180 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/table.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     1111 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/test.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     3315 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/view.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     1537 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/persist_docs.sql
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.549250 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/schema_tests/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1095 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/schema_tests/relationships.sql
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.550525 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/utils/
+-rw-r--r--   0 bytedance   (501) staff       (20)      660 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/utils/datatypes.sql
+-rw-r--r--   0 bytedance   (501) staff       (20)     2223 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/utils/utils.sql
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-04-22 06:29:25.553211 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)    20624 2024-04-22 06:29:25.000000 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)     1350 2024-04-22 06:29:25.000000 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2024-04-22 06:29:25.000000 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       49 2024-04-22 06:29:25.000000 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/requires.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        4 2024-04-22 06:29:25.000000 dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)      367 2023-11-27 05:45:50.000000 dbt-bytehouse-1.7.1/pyproject.toml
+-rw-r--r--   0 bytedance   (501) staff       (20)       38 2024-04-22 06:29:25.554302 dbt-bytehouse-1.7.1/setup.cfg
+-rw-r--r--   0 bytedance   (501) staff       (20)     3203 2024-04-22 06:24:19.000000 dbt-bytehouse-1.7.1/setup.py
```

### Comparing `dbt-bytehouse-1.3.2/LICENSE` & `dbt-bytehouse-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/PKG-INFO` & `dbt-bytehouse-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bytehouse
-Version: 1.3.2
+Version: 1.7.1
 Summary: The ByteHouse plugin for dbt (data build tool)
 Home-page: https://github.com/bytehouse-cloud/bytehouse-dbt
 Author: Rafsan Mazumder
 Author-email: rafsan.mazumder@bytedance.com
 License: MIT
 Project-URL: Documentation, https://github.com/bytehouse-cloud/bytehouse-dbt
 Project-URL: Changes, https://github.com/bytehouse-cloud/bytehouse-dbt/blob/main/CHANGELOG.md
@@ -18,14 +18,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dbt-core~=1.7.0
+Requires-Dist: bytehouse-driver
+Requires-Dist: python-dateutil
 
 # Introduction
 `dbt` (Data Building Tool) is an open source tool that enables data analysts and engineers to transform
 data in their warehouses simply by writing select statements. `dbt` performs the T (Transform) of ETL and
 allows companies to write transformations as queries and orchestrate them in a more efficient way. 
 ByteHouse dbt connector is a plugin enabling users to build their data warehouse ecosystem with dbt 
 and ByteHouse. 
@@ -55,15 +58,15 @@
     + [How it works](#how-it-works)
 - [Project Documentation](#project-documentation)
 - [Local Development](#local-development)
 - [Original Author](#original-author)
 - [License](#license)
 # Requirements
 Make sure you have `dbt` & `python` installed on your machine. If not, then you can follow this guide https://docs.getdbt.com/docs/get-started/installation
-- dbt v1.3.0 or greater
+- dbt v1.7.0 or greater
 - python v3.7 or greater
 # Creating ByteHouse Account
 You need to create ByteHouse account in order to use bytehouse-dbt connector. You can simply create a free account with
 the process mentioned in our official website documentation: https://docs.bytehouse.cloud/en/docs/quick-start <br/>
 
 You can also create ByteHouse account through Volcano Engine by ByteDance: 
 https://www.volcengine.com/product/bytehouse-cloud
```

### Comparing `dbt-bytehouse-1.3.2/README.md` & `dbt-bytehouse-1.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     + [How it works](#how-it-works)
 - [Project Documentation](#project-documentation)
 - [Local Development](#local-development)
 - [Original Author](#original-author)
 - [License](#license)
 # Requirements
 Make sure you have `dbt` & `python` installed on your machine. If not, then you can follow this guide https://docs.getdbt.com/docs/get-started/installation
-- dbt v1.3.0 or greater
+- dbt v1.7.0 or greater
 - python v3.7 or greater
 # Creating ByteHouse Account
 You need to create ByteHouse account in order to use bytehouse-dbt connector. You can simply create a free account with
 the process mentioned in our official website documentation: https://docs.bytehouse.cloud/en/docs/quick-start <br/>
 
 You can also create ByteHouse account through Volcano Engine by ByteDance: 
 https://www.volcengine.com/product/bytehouse-cloud
```

#### html2text {}

```diff
@@ -19,15 +19,15 @@
 Models](#materialization-types-of-models) * [View Materializations](#view-
 materializations) * [Table Materializations](#table-materializations) *
 [Incremental Materializations](#incremental-materializations) + [How it works]
 (#how-it-works) - [Project Documentation](#project-documentation) - [Local
 Development](#local-development) - [Original Author](#original-author) -
 [License](#license) # Requirements Make sure you have `dbt` & `python`
 installed on your machine. If not, then you can follow this guide https://
-docs.getdbt.com/docs/get-started/installation - dbt v1.3.0 or greater - python
+docs.getdbt.com/docs/get-started/installation - dbt v1.7.0 or greater - python
 v3.7 or greater # Creating ByteHouse Account You need to create ByteHouse
 account in order to use bytehouse-dbt connector. You can simply create a free
 account with the process mentioned in our official website documentation:
 https://docs.bytehouse.cloud/en/docs/quick-start
 You can also create ByteHouse account through Volcano Engine by ByteDance:
 https://www.volcengine.com/product/bytehouse-cloud # Installation Create a new
 repository where we will instantiate a `Python` virtual environment.
```

### Comparing `dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/__init__.py` & `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/__version__.py` & `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/__version__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,8 +12,8 @@
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 
-version = '1.3.2'
+version = '1.7.1'
```

### Comparing `dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/column.py` & `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/column.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 
 import re
 from dataclasses import dataclass
 from typing import Any, TypeVar
 
 from dbt.adapters.base.column import Column
-from dbt.exceptions import RuntimeException
+from dbt.exceptions import DbtRuntimeError
 
 Self = TypeVar('Self', bound='ByteHouseColumn')
 
 
 @dataclass
 class ByteHouseColumn(Column):
     TYPE_LABELS = {
@@ -110,15 +110,15 @@
         return self.dtype.lower().startswith('decimal')
 
     def is_float(self) -> bool:
         return self.dtype.lower().startswith('float')
 
     def string_size(self) -> int:
         if not self.is_string():
-            raise RuntimeException('Called string_size() on non-string field!')
+            raise DbtRuntimeError('Called string_size() on non-string field!')
 
         if not self.dtype.lower().startswith('fixedstring') or self.char_size is None:
             return 256
         else:
             return int(self.char_size)
 
     @classmethod
```

### Comparing `dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/connections.py` & `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
     @contextmanager
     def exception_handler(self, sql):
         try:
             yield
         except Exception as exp:
             logger.debug('Error running SQL: {}', sql)
-            if isinstance(exp, dbt.exceptions.RuntimeException):
+            if isinstance(exp, dbt.exceptions.DbtRuntimeError):
                 raise
-            raise dbt.exceptions.RuntimeException(exp) from exp
+            raise dbt.exceptions.DbtRuntimeError(str(exp)) from exp
 
     @classmethod
     def open(cls, connection):
         if connection.state == 'open':
             logger.debug('Connection is already open, skipping open.')
             return connection
         credentials = cls.get_credentials(connection.credentials)
@@ -88,15 +88,15 @@
         data = []
         for row in response:
             data.append(dict(zip(column_names, row)))
 
         return dbt.clients.agate_helper.table_from_data_flat(data, column_names)
 
     def execute(
-        self, sql: str, auto_begin: bool = False, fetch: bool = False
+        self, sql: str, auto_begin: bool = False, fetch: bool = False, limit: Optional[int] = None
     ) -> Tuple[str, agate.Table]:
         # Don't try to fetch result of clustered DDL responses, we don't know what to do with them
         if fetch and ddl_re.match(sql):
             fetch = False
 
         sql = self._add_query_comment(sql)
         conn = self.get_thread_connection()
```

### Comparing `dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/credentials.py` & `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     @property
     def unique_field(self):
         return self.host
 
     def __post_init__(self):
         if self.database is not None and self.database != self.schema:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f'    schema: {self.schema} \n'
                 f'    database: {self.database} \n'
                 f'    cluster: {self.cluster} \n'
                 f'On ByteHouse, database must be omitted or have the same value as'
                 f' schema.'
             )
         self.database = None
```

### Comparing `dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/dbclient.py` & `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/dbclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 
 from abc import ABC, abstractmethod
 
 from dbt.events import AdapterLogger
-from dbt.exceptions import FailedToConnectException
+from dbt.exceptions import FailedToConnectError
 
 from dbt.adapters.bytehouse.credentials import ByteHouseCredentials
 
 logger = AdapterLogger('bytehouse')
 
 
 def get_db_client(credentials: ByteHouseCredentials):
@@ -31,15 +31,15 @@
     try:
         import bytehouse_driver  # noqa
 
         from dbt.adapters.bytehouse.nativeclient import BhNativeClient
 
         return BhNativeClient(credentials)
     except ImportError:
-        raise FailedToConnectException(
+        raise FailedToConnectError(
             'Native adapter required but package bytehouse-driver is not installed'
         )
 
 
 class BhRetryableException(Exception):
     pass
```

### Comparing `dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/impl.py` & `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     @classmethod
     def convert_date_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return 'Date'
 
     @classmethod
     def convert_time_type(cls, agate_table: agate.Table, col_idx: int) -> str:
-        raise dbt.exceptions.NotImplementedException(
+        raise dbt.exceptions.NotImplementedError(
             '`convert_time_type` is not implemented for this adapter!'
         )
 
     @available.parse(lambda *a, **k: {})
     def get_bytehouse_cluster_name(self):
         conn = self.connections.get_if_exists()
         if conn.credentials.cluster:
@@ -163,27 +163,24 @@
                 can_exchange=can_exchange,
             )
             relations.append(relation)
 
         return relations
 
     def get_relation(self, database: Optional[str], schema: str, identifier: str):
-        if not self.Relation.include_policy.database:
-            database = None
-
         return super().get_relation(database, schema, identifier)
 
     @available
     def get_ch_database(self, schema: str):
         try:
             results = self.execute_macro('bytehouse__get_database', kwargs={'database': schema})
             if len(results.rows):
                 return ByteHouseDatabase(**results.rows[0])
             return None
-        except dbt.exceptions.RuntimeException:
+        except dbt.exceptions.DbtRuntimeError:
             return None
 
     def parse_bytehouse_columns(
         self, relation: ByteHouseRelation, raw_rows: List[agate.Row]
     ) -> List[ByteHouseColumn]:
         rows = [dict(zip(row._keys, row._values)) for row in raw_rows]
 
@@ -222,15 +219,15 @@
     def _get_one_catalog(
         self,
         information_schema: InformationSchema,
         schemas: Set[str],
         manifest: Manifest,
     ) -> agate.Table:
         if len(schemas) != 1:
-            dbt.exceptions.raise_compiler_error(
+            dbt.exceptions.CompilationError(
                 f'Expected only one schema in bytehouse _get_one_catalog, found ' f'{schemas}'
             )
 
         return super()._get_one_catalog(information_schema, schemas, manifest)
 
     @classmethod
     def _catalog_filter_table(cls, table: agate.Table, manifest: Manifest) -> agate.Table:
@@ -342,29 +339,33 @@
         finally:
             conn.state = 'close'
 
     @available
     def get_model_settings(self, model):
         settings = model['config'].get('settings', dict())
         res = []
-        for key in settings:
-            res.append(f' {key}={settings[key]}')
+        for key, value in settings.items():
+            # Check if the value is a string and quote it; otherwise, use the value as is
+            if isinstance(value, str):
+                res.append(f"{key}='{value}'")
+            else:
+                res.append(f"{key}={value}")
         return '' if len(res) == 0 else 'SETTINGS ' + ', '.join(res) + '\n'
 
 
 @dataclass
 class ByteHouseDatabase:
     name: str
     engine: str
     comment: str
 
 
 def _expect_row_value(key: str, row: agate.Row):
     if key not in row.keys():
-        raise dbt.exceptions.InternalException(
+        raise dbt.exceptions.DbtInternalError(
             f'Got a row without \'{key}\' column, columns: {row.keys()}'
         )
 
     return row[key]
 
 
 def _catalog_filter_schemas(manifest: Manifest) -> Callable[[agate.Row], bool]:
@@ -384,15 +385,15 @@
     v1_parts = v1.split('.')
     v2_parts = v2.split('.')
     for part1, part2 in zip(v1_parts, v2_parts):
         try:
             if int(part1) != int(part2):
                 return 1 if int(part1) > int(part2) else -1
         except ValueError:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 "Version must consist of only numbers separated by '.'"
             )
     # Versions are equal - return False
     return 0
 
 
 COLUMNS_EQUAL_SQL = '''
```

### Comparing `dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/nativeclient.py` & `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/nativeclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
    limitations under the License.
 """
 
 import bytehouse_driver
 from dateutil import parser
 from bytehouse_driver import Client
 from bytehouse_driver.errors import NetworkError, SocketTimeoutError
-from dbt.exceptions import DatabaseException as DBTDatabaseException
+from dbt.exceptions import DbtDatabaseError as DBTDatabaseException
 from dbt.version import __version__ as dbt_version
 
 from dbt.adapters.bytehouse import ByteHouseCredentials
 from dbt.adapters.bytehouse.dbclient import BhClientWrapper, BhRetryableException
 
 
 class BhNativeClient(BhClientWrapper):
@@ -117,16 +117,15 @@
         self._client.execute("DROP DATABASE IF EXISTS system_meta")
         self._client.execute("CREATE DATABASE system_meta")
         self._client.execute("CREATE TABLE system_meta.databases (name String, engine String, comment String) engine = CnchMergeTree("
                              ") order by tuple()")
         databases_result = self._client.execute("SHOW DATABASES")
         databases_holder = []
         for database in databases_result:
-            database_name = database[0]
-            if database_name.startswith("dbt"):
+            if database[0] == self.database:
                 databases_holder.append(database)
         databases_result = databases_holder
         if len(databases_result) > 0:
             self._client.execute("INSERT INTO system_meta.databases VALUES", ((x[0], x[8], x[7]) for x in databases_result))
 
         if "system_meta.tables" not in sql and "system_meta.columns" not in sql:
             return
```

### Comparing `dbt-bytehouse-1.3.2/dbt/adapters/bytehouse/relation.py` & `dbt-bytehouse-1.7.1/dbt/adapters/bytehouse/relation.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Optional
 
 import dbt.exceptions
 from dbt.adapters.base.relation import BaseRelation, Policy
 
 
 @dataclass
@@ -35,37 +35,37 @@
     database: bool = False
     schema: bool = True
     identifier: bool = True
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class ByteHouseRelation(BaseRelation):
-    quote_policy: ByteHouseQuotePolicy = ByteHouseQuotePolicy()
-    include_policy: ByteHouseIncludePolicy = ByteHouseIncludePolicy()
+    quote_policy: Policy = field(default_factory=lambda: ByteHouseQuotePolicy())
+    include_policy: Policy = field(default_factory=lambda: ByteHouseIncludePolicy())
     quote_character: str = ''
     can_exchange: bool = False
 
     def __post_init__(self):
         if self.database != self.schema and self.database:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f'Cannot set database {self.database} in bytehouse!'
             )
 
     def render(self):
         if self.include_policy.database and self.include_policy.schema:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 'Got a bytehouse relation with schema and database set to '
                 'include, but only one can be set'
             )
         return super().render()
 
     def matches(
         self,
         database: Optional[str] = None,
         schema: Optional[str] = None,
         identifier: Optional[str] = None,
     ):
         if schema:
-            raise dbt.exceptions.RuntimeException(
+            raise dbt.exceptions.DbtRuntimeError(
                 f'Passed unexpected schema value {schema} to Relation.matches'
             )
         return self.database == database and self.identifier == identifier
```

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/__init__.py` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/adapters/apply_grants.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/adapters/relation.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/adapters.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/catalog.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/incremental.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/incremental.sql`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,14 @@
       {% set fail_msg %}
           The source and target schemas on this incremental model are out of sync!
           They can be reconciled in several ways:
             - set the `on_schema_change` config to either append_new_columns or sync_all_columns, depending on your situation.
             - Re-run the incremental model with `full_refresh: True` to update the target schema.
             - update the schema manually and re-run the process.
       {% endset %}
-      {% do exceptions.raise_compiler_error(fail_msg) %}
+      {% do exceptions.CompilationError(fail_msg) %}
       {{ return }}
     {% endif %}
 
     {% do sync_column_schemas(on_schema_change, target_relation, schema_changes_dict) %}
 
 {% endmacro %}
```

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/seed.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/snapshot.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/table.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/table.sql`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,15 @@
         {% endcall %}
         {{ bytehouse__insert_into(relation.include(database=False), sql) }}
     {%- endif %}
 {%- endmacro %}
 
 {% macro create_table_or_empty(temporary, relation, sql) -%}
     {%- set sql_header = config.get('sql_header', none) -%}
+    {%- set cnch_unique_key = config.get('cnch_unique_key') -%}
 
     {{ sql_header if sql_header is not none }}
 
     {% if temporary -%}
         create temporary table {{ relation.name }}
         engine Memory
         {{ order_cols(label="order by") }}
@@ -177,14 +178,17 @@
     {%- else %}
         {% call statement('main') %}
            drop table if exists {{ relation.include(database=False) }}
         {% endcall %}
         create table {{ relation.include(database=False) }}
         {{ on_cluster_clause(label="on cluster") }}
         {{ engine_clause(label="engine") }}
+        {% if cnch_unique_key is not none %}
+            UNIQUE KEY ({{ cnch_unique_key }})
+        {% endif %}
         {{ order_cols(label="order by") }}
         {{ primary_key_clause(label="primary key") }}
         {{ partition_cols(label="partition by") }}
         {{ adapter.get_model_settings(model) }}
         {% if not adapter.is_before_version('22.7.1') -%}
             empty
         {%- endif %}
```

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/test.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/materializations/view.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/persist_docs.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/schema_tests/relationships.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/schema_tests/relationships.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/utils/datatypes.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/utils/datatypes.sql`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/dbt/include/bytehouse/macros/utils/utils.sql` & `dbt-bytehouse-1.7.1/dbt/include/bytehouse/macros/utils/utils.sql`

 * *Files 15% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 {% macro bytehouse__replace(field, old_chars, new_chars) %}
    replaceAll({{ field }},'{{ old_chars }}','{{ new_chars }}')
 {% endmacro %}
 
 
 {% macro bytehouse__listagg(measure, delimiter_text, order_by_clause, limit_num) %}
-  {{ exceptions.raise_compiler_error(
+  {{ exceptions.CompilationError(
     'bytehouse does not support the listagg function.  See the groupArray function instead')
     }}
 {% endmacro %}
 
 
 {% macro bytehouse__array_construct(inputs, data_type) -%}
     {% if inputs|length > 0 %}
```

### Comparing `dbt-bytehouse-1.3.2/dbt_bytehouse.egg-info/PKG-INFO` & `dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bytehouse
-Version: 1.3.2
+Version: 1.7.1
 Summary: The ByteHouse plugin for dbt (data build tool)
 Home-page: https://github.com/bytehouse-cloud/bytehouse-dbt
 Author: Rafsan Mazumder
 Author-email: rafsan.mazumder@bytedance.com
 License: MIT
 Project-URL: Documentation, https://github.com/bytehouse-cloud/bytehouse-dbt
 Project-URL: Changes, https://github.com/bytehouse-cloud/bytehouse-dbt/blob/main/CHANGELOG.md
@@ -18,14 +18,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dbt-core~=1.7.0
+Requires-Dist: bytehouse-driver
+Requires-Dist: python-dateutil
 
 # Introduction
 `dbt` (Data Building Tool) is an open source tool that enables data analysts and engineers to transform
 data in their warehouses simply by writing select statements. `dbt` performs the T (Transform) of ETL and
 allows companies to write transformations as queries and orchestrate them in a more efficient way. 
 ByteHouse dbt connector is a plugin enabling users to build their data warehouse ecosystem with dbt 
 and ByteHouse. 
@@ -55,15 +58,15 @@
     + [How it works](#how-it-works)
 - [Project Documentation](#project-documentation)
 - [Local Development](#local-development)
 - [Original Author](#original-author)
 - [License](#license)
 # Requirements
 Make sure you have `dbt` & `python` installed on your machine. If not, then you can follow this guide https://docs.getdbt.com/docs/get-started/installation
-- dbt v1.3.0 or greater
+- dbt v1.7.0 or greater
 - python v3.7 or greater
 # Creating ByteHouse Account
 You need to create ByteHouse account in order to use bytehouse-dbt connector. You can simply create a free account with
 the process mentioned in our official website documentation: https://docs.bytehouse.cloud/en/docs/quick-start <br/>
 
 You can also create ByteHouse account through Volcano Engine by ByteDance: 
 https://www.volcengine.com/product/bytehouse-cloud
```

### Comparing `dbt-bytehouse-1.3.2/dbt_bytehouse.egg-info/SOURCES.txt` & `dbt-bytehouse-1.7.1/dbt_bytehouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-bytehouse-1.3.2/setup.py` & `dbt-bytehouse-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return match.group(1)
 
 
 package_name = 'dbt-bytehouse'
 package_version = _dbt_bytehouse_version()
 description = '''The ByteHouse plugin for dbt (data build tool)'''
 
-dbt_version = '1.3.0'
+dbt_version = '1.7.0'
 dbt_minor = '.'.join(dbt_version.split('.')[0:2])
 
 if not package_version.startswith(dbt_minor):
     raise ValueError(
         f'Invalid setup.py: package_version={package_version} must start with '
         f'dbt_version={dbt_minor}'
     )
```

