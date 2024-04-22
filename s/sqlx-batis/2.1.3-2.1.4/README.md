# Comparing `tmp/sqlx-batis-2.1.3.tar.gz` & `tmp/sqlx-batis-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-2.1.3.tar", last modified: Fri Mar 29 02:33:57 2024, max compression
+gzip compressed data, was "dist\sqlx-batis-2.1.4.tar", last modified: Mon Apr 22 02:10:47 2024, max compression
```

## Comparing `sqlx-batis-2.1.3.tar` & `sqlx-batis-2.1.4.tar`

### file list

```diff
@@ -1,27 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 02:33:57.000000 sqlx-batis-2.1.3/
--rw-rw-rw-   0        0        0     6114 2024-03-29 02:33:57.000000 sqlx-batis-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5423 2024-03-29 02:33:52.000000 sqlx-batis-2.1.3/README.rst
--rw-rw-rw-   0        0        0       42 2024-03-29 02:33:57.000000 sqlx-batis-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1352 2024-03-29 02:33:52.000000 sqlx-batis-2.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-29 02:33:57.000000 sqlx-batis-2.1.3/sqlbatis/
--rw-rw-rw-   0        0        0      892 2024-03-26 02:58:34.000000 sqlx-batis-2.1.3/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     5873 2024-03-26 05:34:40.000000 sqlx-batis-2.1.3/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6529 2024-03-27 02:19:48.000000 sqlx-batis-2.1.3/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     3731 2023-08-01 15:34:15.000000 sqlx-batis-2.1.3/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    35767 2024-03-27 03:21:39.000000 sqlx-batis-2.1.3/sqlbatis/orm.py
--rw-rw-rw-   0        0        0    12439 2024-03-27 01:08:33.000000 sqlx-batis-2.1.3/sqlbatis/orm_support.py
--rw-rw-rw-   0        0        0     2672 2023-08-04 01:49:10.000000 sqlx-batis-2.1.3/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7278 2023-08-04 01:47:15.000000 sqlx-batis-2.1.3/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0      963 2024-03-26 06:12:24.000000 sqlx-batis-2.1.3/sqlbatis/sql_id_exec.py
--rw-rw-rw-   0        0        0     5274 2024-03-26 06:21:11.000000 sqlx-batis-2.1.3/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0      295 2024-03-26 05:59:56.000000 sqlx-batis-2.1.3/sqlbatis/sql_page_exec.py
--rw-rw-rw-   0        0        0     1676 2024-03-26 14:41:52.000000 sqlx-batis-2.1.3/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      340 2024-03-26 05:16:39.000000 sqlx-batis-2.1.3/sqlbatis/support.py
--rw-rw-rw-   0        0        0     1527 2024-03-28 03:25:48.000000 sqlx-batis-2.1.3/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 02:33:57.000000 sqlx-batis-2.1.3/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2024-03-29 02:33:57.000000 sqlx-batis-2.1.3/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-27 04:09:07.000000 sqlx-batis-2.1.3/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     6114 2024-03-29 02:33:57.000000 sqlx-batis-2.1.3/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2024-03-29 02:33:57.000000 sqlx-batis-2.1.3/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      520 2024-03-29 02:33:57.000000 sqlx-batis-2.1.3/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2024-03-29 02:33:57.000000 sqlx-batis-2.1.3/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 02:10:47.000000 sqlx-batis-2.1.4/
+-rw-rw-rw-   0        0        0     5310 2024-04-22 02:10:47.000000 sqlx-batis-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4642 2024-04-22 01:22:49.000000 sqlx-batis-2.1.4/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-22 02:10:47.000000 sqlx-batis-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1323 2024-04-22 00:31:42.000000 sqlx-batis-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 02:10:47.000000 sqlx-batis-2.1.4/sqlbatis/
+-rw-rw-rw-   0        0        0     1271 2024-04-22 00:57:23.000000 sqlx-batis-2.1.4/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     1140 2024-04-22 01:00:42.000000 sqlx-batis-2.1.4/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0      726 2024-04-22 01:02:01.000000 sqlx-batis-2.1.4/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0      679 2024-04-22 01:07:22.000000 sqlx-batis-2.1.4/sqlbatis/sql_id_exec.py
+-rw-rw-rw-   0        0        0     4076 2024-04-22 01:03:46.000000 sqlx-batis-2.1.4/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0      295 2024-03-26 05:59:56.000000 sqlx-batis-2.1.4/sqlbatis/sql_page_exec.py
+-rw-rw-rw-   0        0        0      217 2024-04-22 00:39:30.000000 sqlx-batis-2.1.4/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 02:10:47.000000 sqlx-batis-2.1.4/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-22 02:10:47.000000 sqlx-batis-2.1.4/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 01:24:52.000000 sqlx-batis-2.1.4/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5310 2024-04-22 02:10:47.000000 sqlx-batis-2.1.4/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-04-22 02:10:47.000000 sqlx-batis-2.1.4/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      370 2024-04-22 02:10:47.000000 sqlx-batis-2.1.4/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2024-04-22 02:10:47.000000 sqlx-batis-2.1.4/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-2.1.3/PKG-INFO` & `sqlx-batis-2.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 2.1.3
+Version: 2.1.4
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -43,15 +43,14 @@
        </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-    from sqlbatis.orm import Model
     from typing import List, Tuple, Mapping
     from sqlbatis import mapper, sql, dbx, init_db
 
     @mapper(namespace='person')
     def select_all(): List
 
     @mapper(namespace='person')
@@ -133,36 +132,14 @@
         # result:
         # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
         persons = db.select('select id, name, age from person where name = ?', 'zhangsan')
         # result:
         # [(3, 'zhangsan', 15)]
 
-        # you can use orm to operate a single table
-        class Person(Model):
-            __pk__ = 'id'
-            __table__ = 'person'
-
-            def __init__(self, id: int = None, name: str = None, age: int = None):
-                self.id = id
-                self.name = name
-                self.age = age
-
-
-        effected_rowcount = Person.insert(name='tianqi', age=77)
-
-        persons = Person.query(name='tianqi')
-        # select id, name, age from person where name = :name
-        # result:
-        # {'id': 7, 'name': 'tianqi', 'age': 77}
-
-        persons = Person.query(name__eq='zhangsan')
-        # select id, name, age from person where name = :name
-        # result:
-        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
 Transaction
 '''''''''''
 
 .. code:: python
 
         from sqlbatis import with_transaction, transaction
```

### Comparing `sqlx-batis-2.1.3/README.rst` & `sqlx-batis-2.1.4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,14 @@
        </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-    from sqlbatis.orm import Model
     from typing import List, Tuple, Mapping
     from sqlbatis import mapper, sql, dbx, init_db
 
     @mapper(namespace='person')
     def select_all(): List
 
     @mapper(namespace='person')
@@ -120,36 +119,14 @@
         # result:
         # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
         persons = db.select('select id, name, age from person where name = ?', 'zhangsan')
         # result:
         # [(3, 'zhangsan', 15)]
 
-        # you can use orm to operate a single table
-        class Person(Model):
-            __pk__ = 'id'
-            __table__ = 'person'
-
-            def __init__(self, id: int = None, name: str = None, age: int = None):
-                self.id = id
-                self.name = name
-                self.age = age
-
-
-        effected_rowcount = Person.insert(name='tianqi', age=77)
-
-        persons = Person.query(name='tianqi')
-        # select id, name, age from person where name = :name
-        # result:
-        # {'id': 7, 'name': 'tianqi', 'age': 77}
-
-        persons = Person.query(name__eq='zhangsan')
-        # select id, name, age from person where name = :name
-        # result:
-        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
 Transaction
 '''''''''''
 
 .. code:: python
 
         from sqlbatis import with_transaction, transaction
```

### Comparing `sqlx-batis-2.1.3/setup.py` & `sqlx-batis-2.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 setup(
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'Jinja2>=2.7.0',
-        'sqlx-exec>=2.3.3',
+        'mysqlx>=2.1.4',
     ],
-    version='2.1.3',
+    version='2.1.4',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-2.1.3/sqlbatis/sql_id_exec.py` & `sqlx-batis-2.1.4/sqlbatis/sql_id_exec.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 from . import dbx
-from sqlexec.sql_exec import SqlExec as _SqlExec
+from mysqlx.sql_id_exec import SqlExec as _SqlExec
 from sqlexec.page_exec import PageExec
 
 
 class SqlExec(_SqlExec):
 
-    def save(self, *args, **kwargs):
-        """
-        Insert data into table, return primary key.
-
-        :param select_key: sql for select primary key
-        :param args:
-        :return: Primary key
-        """
-        return self.exec.save(self.sql, *args, **kwargs)
-
     def save_select_key(self, select_key: str, *args, **kwargs):
         """
         Insert data into table, return primary key.
 
         :param select_key: sql for select primary key
         :param args:
         :return: Primary key
```

### Comparing `sqlx-batis-2.1.3/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-2.1.4/sqlx_batis.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 2.1.3
+Version: 2.1.4
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -43,15 +43,14 @@
        </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-    from sqlbatis.orm import Model
     from typing import List, Tuple, Mapping
     from sqlbatis import mapper, sql, dbx, init_db
 
     @mapper(namespace='person')
     def select_all(): List
 
     @mapper(namespace='person')
@@ -133,36 +132,14 @@
         # result:
         # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
         persons = db.select('select id, name, age from person where name = ?', 'zhangsan')
         # result:
         # [(3, 'zhangsan', 15)]
 
-        # you can use orm to operate a single table
-        class Person(Model):
-            __pk__ = 'id'
-            __table__ = 'person'
-
-            def __init__(self, id: int = None, name: str = None, age: int = None):
-                self.id = id
-                self.name = name
-                self.age = age
-
-
-        effected_rowcount = Person.insert(name='tianqi', age=77)
-
-        persons = Person.query(name='tianqi')
-        # select id, name, age from person where name = :name
-        # result:
-        # {'id': 7, 'name': 'tianqi', 'age': 77}
-
-        persons = Person.query(name__eq='zhangsan')
-        # select id, name, age from person where name = :name
-        # result:
-        # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
 
 Transaction
 '''''''''''
 
 .. code:: python
 
         from sqlbatis import with_transaction, transaction
```

