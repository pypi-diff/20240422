# Comparing `tmp/mysqlx-2.1.3.tar.gz` & `tmp/mysqlx-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-2.1.3.tar", last modified: Fri Mar 29 02:35:32 2024, max compression
+gzip compressed data, was "dist\mysqlx-2.1.4.tar", last modified: Mon Apr 22 01:17:31 2024, max compression
```

## Comparing `mysqlx-2.1.3.tar` & `mysqlx-2.1.4.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 02:35:32.000000 mysqlx-2.1.3/
-drwxrwxrwx   0        0        0        0 2024-03-29 02:35:32.000000 mysqlx-2.1.3/mysqlx/
--rw-rw-rw-   0        0        0      380 2024-03-27 03:46:06.000000 mysqlx-2.1.3/mysqlx/db.py
--rw-rw-rw-   0        0        0      136 2024-03-27 02:54:52.000000 mysqlx-2.1.3/mysqlx/dbx.py
--rw-rw-rw-   0        0        0      592 2023-07-28 02:20:31.000000 mysqlx-2.1.3/mysqlx/log_support.py
--rw-rw-rw-   0        0        0     6065 2023-09-03 06:51:18.000000 mysqlx-2.1.3/mysqlx/orm.py
--rw-rw-rw-   0        0        0     1423 2024-03-27 01:58:09.000000 mysqlx-2.1.3/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 02:35:32.000000 mysqlx-2.1.3/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2024-03-29 02:35:31.000000 mysqlx-2.1.3/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-29 02:35:31.000000 mysqlx-2.1.3/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5722 2024-03-29 02:35:31.000000 mysqlx-2.1.3/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-03-29 02:35:31.000000 mysqlx-2.1.3/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      279 2024-03-29 02:35:31.000000 mysqlx-2.1.3/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2024-03-29 02:35:31.000000 mysqlx-2.1.3/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5722 2024-03-29 02:35:32.000000 mysqlx-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5057 2024-03-29 02:34:39.000000 mysqlx-2.1.3/README.rst
--rw-rw-rw-   0        0        0       42 2024-03-29 02:35:32.000000 mysqlx-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1375 2024-03-29 02:35:20.000000 mysqlx-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 01:17:31.000000 mysqlx-2.1.4/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-2.1.4/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx/
+-rw-rw-rw-   0        0        0      163 2024-04-21 14:49:14.000000 mysqlx-2.1.4/mysqlx/constant.py
+-rw-rw-rw-   0        0        0     5069 2024-04-21 15:19:48.000000 mysqlx-2.1.4/mysqlx/db.py
+-rw-rw-rw-   0        0        0     5898 2024-04-21 15:53:48.000000 mysqlx-2.1.4/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     7187 2024-03-27 02:51:39.000000 mysqlx-2.1.4/mysqlx/generator.py
+-rw-rw-rw-   0        0        0     1802 2023-07-24 02:58:28.000000 mysqlx-2.1.4/mysqlx/generator.tpl
+-rw-rw-rw-   0        0        0      871 2024-04-21 15:19:48.000000 mysqlx-2.1.4/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0     7278 2023-08-04 01:47:15.000000 mysqlx-2.1.4/mysqlx/sql_holder.py
+-rw-rw-rw-   0        0        0      626 2024-04-22 01:06:31.000000 mysqlx-2.1.4/mysqlx/sql_id_exec.py
+-rw-rw-rw-   0        0        0     4880 2024-04-21 15:26:32.000000 mysqlx-2.1.4/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0      295 2024-03-26 05:59:56.000000 mysqlx-2.1.4/mysqlx/sql_page_exec.py
+-rw-rw-rw-   0        0        0     1676 2024-04-21 15:19:48.000000 mysqlx-2.1.4/mysqlx/sql_support.py
+-rw-rw-rw-   0        0        0      340 2024-03-26 05:16:39.000000 mysqlx-2.1.4/mysqlx/support.py
+-rw-rw-rw-   0        0        0     1588 2024-04-21 15:35:44.000000 mysqlx-2.1.4/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 00:27:57.000000 mysqlx-2.1.4/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4984 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      461 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4984 2024-04-22 01:17:31.000000 mysqlx-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4319 2024-04-22 00:20:10.000000 mysqlx-2.1.4/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-22 01:17:31.000000 mysqlx-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1327 2024-04-22 00:30:05.000000 mysqlx-2.1.4/setup.py
```

### Comparing `mysqlx-2.1.3/mysqlx/__init__.py` & `mysqlx-2.1.4/mysqlx/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from sqlbatis import (
+from sqlexec import (
     connection,
     transaction,
     with_connection,
     with_transaction,
     get_connection,
     close,
     Driver,
-    sql,
-    mapper,
-    init_snowflake,
-    get_snowflake_id,
-    init_db as _init_db
+    Dialect,
+    Engine,
+    init as _init
 )
-from sqlexec import Dialect, Engine
 
+from .sql_mapper import sql, mapper
 
 def init_db(*args, **kwargs):
     """
     Compliant with the Python DB API 2.0 (PEP-249).
 
     from mysqlx import init_db
     init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
@@ -32,10 +30,15 @@
     :param pool_size=0: int, default 0, size of connection pool
     :param show_sql=False: bool,  if True, print sql
     :param debug=False: bool, if True, print debug context
     :param trans_placeholder=True: bool, if True, sql placeholder '?' --> '%s'
 
     Other parameters of connection pool refer to DBUtils: https://webwareforpython.github.io/DBUtils/main.html#pooleddb-pooled-db
     """
+    from .constant import MAPPER_PATH
+    from .sql_holder import load_mapper
 
-    Dialect.init(Engine.MYSQL)
-    _init_db(*args, **kwargs)
+    # Dialect.init(Engine.MYSQL)
+    mapper_path = kwargs.pop(MAPPER_PATH) if MAPPER_PATH in kwargs else None
+    _init(*args, **kwargs)
+    if mapper_path:
+        load_mapper(mapper_path)
```

### Comparing `mysqlx-2.1.3/mysqlx.egg-info/PKG-INFO` & `mysqlx-2.1.4/mysqlx.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 2.1.3
+Version: 2.1.4
 Summary: A thread safe sql executor for MySQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 Mapper file
 '''''''''''
 
 Create a mapper file in 'mapper' folder, you can named
 'user_mapper.xml', like follow:
 
@@ -126,37 +127,14 @@
         # result:
         # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
         users = db.sql('select id, name, age from user name = :name').query(name='zhangsan')
         # result:
         # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-        # you can use orm to operate a single table
-        class User(Model):
-            __key__ = 'id'
-            __table__ = 'user'
-
-            def __init__(self, id: int = None, name: str = None, age: int = None):
-                self.id = id
-                self.name = name
-                self.age = age
-
-
-        effected_rowcount = User.insert(name='tianqi', age=77)
-
-        users = User.query(name='tianqi')
-        # select id, name, age from user where name = :name
-        # result:
-        # {'id': 7, 'name': 'tianqi', 'age': 77}
-
-        users = User.query(name__eq='zhangsan')
-        # select id, name, age from user where name = :name
-        # result:
-        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
 Transaction
 '''''''''''
 
 .. code:: python
 
        from mysqlx import with_transaction, transaction
 
@@ -167,15 +145,15 @@
 
 
        def test_transaction2():
            with transaction():
                insert_func(....)
                update_func(....)
 
-You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
+You can generate model class with mysqlx-generator: https://pypi.org/project/sqlx-orm
 
 If you want to operate PostgreSQL database, may be you need PgSqlx: https://pypi.org/project/pgsqlx
 
 If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
 
 If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
```

### Comparing `mysqlx-2.1.3/PKG-INFO` & `mysqlx-2.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 2.1.3
+Version: 2.1.4
 Summary: A thread safe sql executor for MySQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 Mapper file
 '''''''''''
 
 Create a mapper file in 'mapper' folder, you can named
 'user_mapper.xml', like follow:
 
@@ -126,37 +127,14 @@
         # result:
         # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
         users = db.sql('select id, name, age from user name = :name').query(name='zhangsan')
         # result:
         # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-        # you can use orm to operate a single table
-        class User(Model):
-            __key__ = 'id'
-            __table__ = 'user'
-
-            def __init__(self, id: int = None, name: str = None, age: int = None):
-                self.id = id
-                self.name = name
-                self.age = age
-
-
-        effected_rowcount = User.insert(name='tianqi', age=77)
-
-        users = User.query(name='tianqi')
-        # select id, name, age from user where name = :name
-        # result:
-        # {'id': 7, 'name': 'tianqi', 'age': 77}
-
-        users = User.query(name__eq='zhangsan')
-        # select id, name, age from user where name = :name
-        # result:
-        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
 Transaction
 '''''''''''
 
 .. code:: python
 
        from mysqlx import with_transaction, transaction
 
@@ -167,15 +145,15 @@
 
 
        def test_transaction2():
            with transaction():
                insert_func(....)
                update_func(....)
 
-You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
+You can generate model class with mysqlx-generator: https://pypi.org/project/sqlx-orm
 
 If you want to operate PostgreSQL database, may be you need PgSqlx: https://pypi.org/project/pgsqlx
 
 If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
 
 If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
```

### Comparing `mysqlx-2.1.3/README.rst` & `mysqlx-2.1.4/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -113,37 +113,14 @@
         # result:
         # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
         users = db.sql('select id, name, age from user name = :name').query(name='zhangsan')
         # result:
         # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
-        # you can use orm to operate a single table
-        class User(Model):
-            __key__ = 'id'
-            __table__ = 'user'
-
-            def __init__(self, id: int = None, name: str = None, age: int = None):
-                self.id = id
-                self.name = name
-                self.age = age
-
-
-        effected_rowcount = User.insert(name='tianqi', age=77)
-
-        users = User.query(name='tianqi')
-        # select id, name, age from user where name = :name
-        # result:
-        # {'id': 7, 'name': 'tianqi', 'age': 77}
-
-        users = User.query(name__eq='zhangsan')
-        # select id, name, age from user where name = :name
-        # result:
-        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
 Transaction
 '''''''''''
 
 .. code:: python
 
        from mysqlx import with_transaction, transaction
 
@@ -154,14 +131,14 @@
 
 
        def test_transaction2():
            with transaction():
                insert_func(....)
                update_func(....)
 
-You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
+You can generate model class with mysqlx-generator: https://pypi.org/project/sqlx-orm
 
 If you want to operate PostgreSQL database, may be you need PgSqlx: https://pypi.org/project/pgsqlx
 
 If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
 
 If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
```

### Comparing `mysqlx-2.1.3/setup.py` & `mysqlx-2.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 setup(
     name='mysqlx',
     packages=['mysqlx'],
     description="A thread safe sql executor for MySQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        # 'Jinja2>=2.7.0',
-        'sqlx-batis>=2.1.2',
-        # 'mysql-connector-python>=8.0.13',
+        'Jinja2>=2.7.0',
+        'sqlx-exec>=2.3.6',
     ],
-    version='2.1.3',
+    version='2.1.4',
     url='https://gitee.com/summry/mysqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

