# Comparing `tmp/pgsqlx-2.1.3.tar.gz` & `tmp/pgsqlx-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-2.1.3.tar", last modified: Fri Mar 29 02:31:31 2024, max compression
+gzip compressed data, was "dist\pgsqlx-2.1.4.tar", last modified: Mon Apr 22 03:34:32 2024, max compression
```

## Comparing `pgsqlx-2.1.3.tar` & `pgsqlx-2.1.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 02:31:31.000000 pgsqlx-2.1.3/
-drwxrwxrwx   0        0        0        0 2024-03-29 02:31:31.000000 pgsqlx-2.1.3/pgsqlx/
--rw-rw-rw-   0        0        0      156 2024-03-27 03:58:42.000000 pgsqlx-2.1.3/pgsqlx/constant.py
--rw-rw-rw-   0        0        0     1578 2024-03-27 03:47:00.000000 pgsqlx-2.1.3/pgsqlx/db.py
--rw-rw-rw-   0        0        0     1248 2024-03-27 03:48:25.000000 pgsqlx-2.1.3/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-2.1.3/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0     2282 2024-03-27 03:54:51.000000 pgsqlx-2.1.3/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     3308 2024-03-27 03:36:59.000000 pgsqlx-2.1.3/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     1392 2024-03-27 03:31:45.000000 pgsqlx-2.1.3/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 02:31:31.000000 pgsqlx-2.1.3/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2024-03-29 02:31:30.000000 pgsqlx-2.1.3/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-29 02:31:30.000000 pgsqlx-2.1.3/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5846 2024-03-29 02:31:30.000000 pgsqlx-2.1.3/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-03-29 02:31:30.000000 pgsqlx-2.1.3/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      319 2024-03-29 02:31:30.000000 pgsqlx-2.1.3/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2024-03-29 02:31:30.000000 pgsqlx-2.1.3/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5846 2024-03-29 02:31:31.000000 pgsqlx-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5169 2024-03-29 02:30:59.000000 pgsqlx-2.1.3/README.rst
--rw-rw-rw-   0        0        0       42 2024-03-29 02:31:31.000000 pgsqlx-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1370 2024-03-29 02:31:22.000000 pgsqlx-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/
+drwxrwxrwx   0        0        0        0 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx/
+-rw-rw-rw-   0        0        0       47 2024-04-22 01:34:52.000000 pgsqlx-2.1.4/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0     1253 2024-04-22 01:30:19.000000 pgsqlx-2.1.4/pgsqlx/db.py
+-rw-rw-rw-   0        0        0     1246 2024-04-22 01:31:03.000000 pgsqlx-2.1.4/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-2.1.4/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     3302 2024-04-22 01:29:23.000000 pgsqlx-2.1.4/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     1348 2024-04-22 01:26:50.000000 pgsqlx-2.1.4/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5812 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      305 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5812 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5136 2024-04-22 01:22:30.000000 pgsqlx-2.1.4/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1312 2024-04-22 01:12:18.000000 pgsqlx-2.1.4/setup.py
```

### Comparing `pgsqlx-2.1.3/pgsqlx/db.py` & `pgsqlx-2.1.4/pgsqlx/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,14 @@
 from . import Dialect
 from .log_support import save_log, save_key_seq_log
 
 # Don't remove. Import for not repetitive implementation
 from sqlbatis.db import insert, save, save_select_key, execute, batch_insert, batch_execute, get, query, query_one, select, select_one, save_sql, \
     save_sql_select_key, do_execute, do_get, do_query, do_query_one, do_select, do_select_one, do_select_page, do_query_page, select_page, query_page,\
-    do_save_sql, do_save_sql_select_key, drop, truncate, sql, table, page
-
-
-# def save(table_name: str, **kwargs):
-#     """
-#     Insert data into table, return primary key.
-#     :param table_name: table
-#     :param kwargs:
-#     :return: Primary key
-#     """
-#     save_log(table_name, **kwargs)
-#     return save_key_seq(Dialect.get_select_key(table_name=table_name), table_name, **kwargs)
+    do_save_sql, do_save_sql_select_key, drop_table, drop_table, sql, table, page
 
 
 def save_key_seq(key_seq: str, table_name: str, **kwargs):
     """
     Insert data into table, return primary key.
     :param key_seq: primary key sequnece
     :param table_name: table
```

### Comparing `pgsqlx-2.1.3/pgsqlx/dbx.py` & `pgsqlx-2.1.4/pgsqlx/dbx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from . import Dialect, db
-from sqlbatis import sql_holder as holder
+from mysqlx import sql_holder as holder
 from .log_support import sql_id_log, sql_id_key_seq_log
 from sqlbatis.dbx import save_select_key, batch_execute, execute, get, query, query_one, select, select_one, select_page, query_page, sql, page
 
 
 def save(sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
```

### Comparing `pgsqlx-2.1.3/pgsqlx/log_support.py` & `pgsqlx-2.1.4/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-2.1.3/pgsqlx/sql_mapper.py` & `pgsqlx-2.1.4/pgsqlx/sql_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sqlexec
 import functools
 from .log_support import logger
-from sqlbatis.support import SqlAction
-from sqlbatis.sql_support import simple_sql, get_named_sql_args
-from sqlbatis.sql_holder import get_sql_model, do_get_sql
+from mysqlx.support import SqlAction
+from mysqlx.sql_support import simple_sql, get_named_sql_args
+from mysqlx.sql_holder import get_sql_model, do_get_sql
 from sqlbatis.sql_mapper import get_exec_func, before, get_select_func
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
 def mapper(namespace: str = None, sql_id: str = None, batch=False, return_key=False, key_seq=None):
     def _decorator(func):
```

### Comparing `pgsqlx-2.1.3/pgsqlx/__init__.py` & `pgsqlx-2.1.4/pgsqlx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,14 @@
     with_connection,
     with_transaction,
     get_connection,
     close,
     Driver,
     sql,
     mapper,
-    init_snowflake,
-    get_snowflake_id,
     init_db as _init_db
 )
 
 from .sql_mapper import sql, mapper
 from sqlexec import Dialect, Engine
 
 def init_db(*args, **kwargs):
```

### Comparing `pgsqlx-2.1.3/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-2.1.4/pgsqlx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 2.1.3
+Version: 2.1.4
 Summary: A thread safe sql executor for PostgreSQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -43,15 +43,14 @@
        </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-    from pgsqlx.orm import Model
     from typing import List, Tuple, Mapping
     from pgsqlx import mapper, sql, db, dbx, init_db
 
     @mapper(namespace='person')
     def select_all(): List
 
     @mapper(namespace='person')
```

### Comparing `pgsqlx-2.1.3/PKG-INFO` & `pgsqlx-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 2.1.3
+Version: 2.1.4
 Summary: A thread safe sql executor for PostgreSQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -43,15 +43,14 @@
        </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-    from pgsqlx.orm import Model
     from typing import List, Tuple, Mapping
     from pgsqlx import mapper, sql, db, dbx, init_db
 
     @mapper(namespace='person')
     def select_all(): List
 
     @mapper(namespace='person')
```

### Comparing `pgsqlx-2.1.3/README.rst` & `pgsqlx-2.1.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
        </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-    from pgsqlx.orm import Model
     from typing import List, Tuple, Mapping
     from pgsqlx import mapper, sql, db, dbx, init_db
 
     @mapper(namespace='person')
     def select_all(): List
 
     @mapper(namespace='person')
```

### Comparing `pgsqlx-2.1.3/setup.py` & `pgsqlx-2.1.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,19 +14,17 @@
 setup(
     name='pgsqlx',
     packages=['pgsqlx'],
     description="A thread safe sql executor for PostgreSQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        # 'Jinja2>=2.7.0',
-        # 'psycopg2>=2.7.4',
-        'sqlx-batis>=2.1.2',
+        'sqlx-batis>=2.1.4',
     ],
-    version='2.1.3',
+    version='2.1.4',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

