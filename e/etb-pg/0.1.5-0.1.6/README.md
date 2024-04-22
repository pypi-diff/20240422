# Comparing `tmp/etb-pg-0.1.5.tar.gz` & `tmp/etb-pg-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etb-pg-0.1.5.tar", max compression
+gzip compressed data, was "etb-pg-0.1.6.tar", max compression
```

## Comparing `etb-pg-0.1.5.tar` & `etb-pg-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2981 2024-02-19 15:34:00.506722 etb-pg-0.1.5/README.md
--rw-r--r--   0        0        0     3637 2024-02-24 02:43:33.278995 etb-pg-0.1.5/etb_pg/PG.py
--rw-r--r--   0        0        0      101 2024-02-24 02:43:54.635087 etb-pg-0.1.5/etb_pg/__init__.py
--rw-r--r--   0        0        0      509 2024-02-24 02:43:18.050930 etb-pg-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3744 2024-02-24 02:44:30.041607 etb-pg-0.1.5/setup.py
--rw-r--r--   0        0        0     3584 2024-02-24 02:44:30.041784 etb-pg-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2981 2024-02-19 15:34:00.506722 etb-pg-0.1.6/README.md
+-rw-r--r--   0        0        0     3775 2024-04-22 00:52:01.867971 etb-pg-0.1.6/etb_pg/PG.py
+-rw-r--r--   0        0        0      101 2024-04-22 00:52:19.687977 etb-pg-0.1.6/etb_pg/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-22 00:52:25.639979 etb-pg-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3744 2024-04-22 00:52:43.715079 etb-pg-0.1.6/setup.py
+-rw-r--r--   0        0        0     3584 2024-04-22 00:52:43.715269 etb-pg-0.1.6/PKG-INFO
```

### Comparing `etb-pg-0.1.5/README.md` & `etb-pg-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `etb-pg-0.1.5/etb_pg/PG.py` & `etb-pg-0.1.6/etb_pg/PG.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from typing import Any, Callable
 import psycopg
 
 
 class PGDB:
     '''class for interacting with Postgres Databases\n
     conn_dict: dict = {
-    \t "user" : "",
-    \t "password" : "",
-    \t "host" : "",
-    \t "port" : "",
-    \t "dbname" : ""
+        "user" : "",
+        "password" : "",
+        "host" : "",
+        "port" : "",
+        "dbname" : ""
     }
     read_only (optional, default=True): Set the connection to be read only\n
     sql_dir (optional): Specify the absolute path of the directory where queries are stored\n
     README at https://github.com/HFxLhT8JqeU5BnUG/etb-pg'''
 
     DEFAULT_SCHEMA: str = "public"
 
@@ -52,31 +52,34 @@
 
 
     def execute_str_query(self, query: str):
         '''Execute a raw string query'''
         return self._execute_query(query)
 
 
-    def _execute_query(self, query: str) -> list[dict[str, Any]]:
+    def _execute_query(self, query: str) -> list[dict[str, Any]] | None:
         '''Internal use, called by class methods that accept various input formats'''
 
         with self.__connection__.cursor() as curs:
 
             curs.execute(query)
-            self.__connection__.commit()
+            if not curs.description:
+                self.__connection__.commit()
+                return
+
+            else:
+                result = curs.fetchall()
+                cols = curs.description
+
+                rows = [
+                    { cols[i].name : row[i] for i in range(len(row)) }
+                    for row in result
+                    ]
 
-            result = curs.fetchall()
-            cols = curs.description
-
-        rows = [
-            { cols[i].name : row[i] for i in range(len(row)) }
-              for row in result
-              ]
-
-        return rows
+                return rows
 
 
     def str_to_query(self, fun: Callable[..., str]):
         '''Decorator for function that returns a string\n
         Will treat the string returned by decorated function as a query and return the result'''
 
         def wrapper(*args, **kwargs):
```

### Comparing `etb-pg-0.1.5/setup.py` & `etb-pg-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['psycopg-binary>=3.1.18,<4.0.0', 'psycopg>=3.1.18,<4.0.0']
 
 setup_kwargs = {
     'name': 'etb-pg',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Interface for PostgreSQL databases',
     'long_description': '# PG Library\n\nA small class for interacting with Postgres databases. Developed for the CS 495 TV Manager project.\n\n## Initialize\n\nPass a dictionary with connection credentials when instantiating the PGDB object.\n```\nconn_dict: dict = {\n    "user" : "",        # default $USER\n    "password" : "",    # default None\n    "host" : "",        # default localhost\n    "port" : "",        # default 5432\n    "dbname" : ""       # default $USER\n}\n```\nAll of the connection params are optional, and default to the regular Postgres defaults (commented above).\n\nOptional args are read_only connection (default True) and an SQL directory where the object will check for queries stored as as readable files (default None).\n\n\n## Usage\n\nYou can execute a query from a file, from a raw string, from a decorated function, or run a very simple select query. As with the actual Postgres database, schema is always an optional argument, and always defaults to "public" if not provided. Results of a query are always returned as a list of dictionaries, in which the column name maps to the value.\n\nexecute_file_query(): If no SQL directory is passed when the object is created, then it will assume you\'re passing with an absolute file path. If there is no file extension included in the method call, then it will assume it\'s looking for a .sql file. If you did pass an SQL directory at instantiation, and you\'re using .sql file extensions, you can just pass the name of the file as a string without path or extension. For example, if you initialized the PGDB object with sql_dir = \'/home/app/SQL\', you can execute the query in \'/home/app/SQL/my_query.sql\' with execute_file_query(\'my_query\').\n\nexecute_str_query(): Execute a raw string query.\n\nstr_to_query(): Use this to decorate a function that returns a string. Could be useful for mildly dynamic queries. For example (assuming you have already created a PGDB object called "pg_interface"):\n\n```\n@pg_interface.str_to_query\ndef foo(cols: list[str], identifier: str) -> str:\n    columns = \', st.\'.join(cols)\n\n    query = f"""select st.{columns}\n            from schema.table_name st\n            where st.id = \'{identifier}\'"""\n    \n    return query\n```\n\nUsing the decorator, foo() will return the result of the query.\n\nget_columns(): Not a query function. Will return a list of {column_name : python_type} for the specified schema/table.\n\nget_rows(): Will return the results of a query that selects the specified columns from the specified schema/table.\n\n\nThere are no methods for doing joins or window functions- I want to keep any logic that\'s even remotely complex in a version controlled .sql file, or let the user wrap the logic in a decorated function. There\'s also nothing for creates/updates/deletes or anything like that- I want to leave the real ELT to another application or library or framework better suited for it. You can use the get_rows() method for very simple, unqualified selects from a table (or, preferably, a view or function).',
     'author': 'Tate Button',
     'author_email': 'yg3bpwn0or679hau8fxi@duck.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/HFxLhT8JqeU5BnUG/etb-pg',
```

### Comparing `etb-pg-0.1.5/PKG-INFO` & `etb-pg-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etb-pg
-Version: 0.1.5
+Version: 0.1.6
 Summary: Interface for PostgreSQL databases
 Home-page: https://github.com/HFxLhT8JqeU5BnUG/etb-pg
 License: MIT
 Author: Tate Button
 Author-email: yg3bpwn0or679hau8fxi@duck.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

