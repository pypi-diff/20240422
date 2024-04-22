# Comparing `tmp/pg_logidater-0.3.2.tar.gz` & `tmp/pg_logidater-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_logidater-0.3.2.tar", max compression
+gzip compressed data, was "pg_logidater-0.3.3.tar", max compression
```

## Comparing `pg_logidater-0.3.2.tar` & `pg_logidater-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.3.2/LICENSE
--rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.3.2/README.md
--rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.3.2/pg_logidater/__init__.py
--rw-r--r--   0        0        0    10163 2024-04-10 18:12:32.925105 pg_logidater-0.3.2/pg_logidater/cli.py
--rw-r--r--   0        0        0     1326 2024-04-10 07:00:49.766735 pg_logidater-0.3.2/pg_logidater/exceptions.py
--rw-r--r--   0        0        0     2220 2024-04-10 18:12:39.811524 pg_logidater-0.3.2/pg_logidater/master.py
--rw-r--r--   0        0        0     1553 2024-04-10 18:12:44.616579 pg_logidater-0.3.2/pg_logidater/replica.py
--rw-r--r--   0        0        0     2813 2024-04-10 07:23:02.468326 pg_logidater-0.3.2/pg_logidater/sqlqueries.py
--rw-r--r--   0        0        0     5570 2024-04-11 19:15:49.271005 pg_logidater-0.3.2/pg_logidater/tartget.py
--rw-r--r--   0        0        0     8987 2024-04-11 19:26:26.238111 pg_logidater-0.3.2/pg_logidater/utils.py
--rw-r--r--   0        0        0      871 2024-04-12 06:27:17.544337 pg_logidater-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pg_logidater-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.3.3/LICENSE
+-rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.3.3/pg_logidater/__init__.py
+-rw-r--r--   0        0        0    10189 2024-04-22 08:21:48.069551 pg_logidater-0.3.3/pg_logidater/cli.py
+-rw-r--r--   0        0        0     1326 2024-04-10 07:00:49.766735 pg_logidater-0.3.3/pg_logidater/exceptions.py
+-rw-r--r--   0        0        0     2220 2024-04-10 18:12:39.811524 pg_logidater-0.3.3/pg_logidater/master.py
+-rw-r--r--   0        0        0     1553 2024-04-10 18:12:44.616579 pg_logidater-0.3.3/pg_logidater/replica.py
+-rw-r--r--   0        0        0     2813 2024-04-10 07:23:02.468326 pg_logidater-0.3.3/pg_logidater/sqlqueries.py
+-rw-r--r--   0        0        0     5570 2024-04-11 19:15:49.271005 pg_logidater-0.3.3/pg_logidater/tartget.py
+-rw-r--r--   0        0        0     8961 2024-04-22 08:23:02.845772 pg_logidater-0.3.3/pg_logidater/utils.py
+-rw-r--r--   0        0        0      871 2024-04-22 08:17:18.486553 pg_logidater-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pg_logidater-0.3.3/PKG-INFO
```

### Comparing `pg_logidater-0.3.2/LICENSE` & `pg_logidater-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.2/README.md` & `pg_logidater-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.2/pg_logidater/cli.py` & `pg_logidater-0.3.3/pg_logidater/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
 
 
 @cli()
 def drop_setup(args) -> None:
     _logger.info("Cleaning target server")
     try:
         target_sql = SqlConn("/tmp", user="postgres", db=args["database"])
-        target_sql.drop_subscriber()
+        target_sql.drop_subscriber(sub_name=args["repl_name"])
         target_sql = SqlConn("/tmp", user="postgres", db="postgres")
         target_sql.drop_database(args["database"])
     except OperationalError as err:
         _logger.warning(err)
     _logger.info("Cleaning up master")
     master_sql = SqlConn(args["master_host"], user=args["psql_user"], db=args["database"])
     master_sql.drop_publication(args["repl_name"])
```

### Comparing `pg_logidater-0.3.2/pg_logidater/exceptions.py` & `pg_logidater-0.3.3/pg_logidater/exceptions.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.2/pg_logidater/master.py` & `pg_logidater-0.3.3/pg_logidater/master.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.2/pg_logidater/replica.py` & `pg_logidater-0.3.3/pg_logidater/replica.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.2/pg_logidater/sqlqueries.py` & `pg_logidater-0.3.3/pg_logidater/sqlqueries.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.2/pg_logidater/tartget.py` & `pg_logidater-0.3.3/pg_logidater/tartget.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.2/pg_logidater/utils.py` & `pg_logidater-0.3.3/pg_logidater/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,18 +97,17 @@
             _logger.warning(f"Publication {pub_name} - doesn't exist")
             self.sql_conn.rollback()
 
     def create_subscriber(self, name, host, database, repl_slot) -> str:
         self.query(sql.SQL_CREATE_SUBSCRIPTION.format(name=name, master=host, db=database, pub_name=name, repl_slot=repl_slot))
         return self.query(sql.SQL_SELECT_SUB_NAME.format(name=name), fetchone=True)[0]
 
-    def drop_subscriber(self, drop_slot: bool = False) -> None:
+    def drop_subscriber(self, sub_name: str, drop_slot: bool = False) -> None:
         self.sql_conn.autocommit = True
         try:
-            sub_name = self.get_db_sub()
             if sub_name:
                 self.disable_subscription(sub_name)
                 if not drop_slot:
                     self.set_slot_name(sub_name, "NONE")
                 self.query(sql.SQL_DROP_SUBSCRIPTION.format(name=sub_name))
         except psycopg2.errors.UndefinedObject:
             _logger.warning(f"Subscription {sub_name} doesn't exist!")
```

### Comparing `pg_logidater-0.3.2/pyproject.toml` & `pg_logidater-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pg-logidater"
 readme = "README.md"
 authors = ["Arunas Grigalionis <arunas.grigalionis@gmail.com>"]
 description = "Postgresql logical replication setup utility"
-version = "0.3.1"
+version = "0.3.3"
 license = "GPL-3.0-only"
 homepage = "https://github.com/niekosau"
 repository = "https://github.com/niekosau/pg-logidater"
 keywords = ["postgres"]
 
 [tool.poetry.scripts]
 pg-logidater = 'pg_logidater.cli:main'
```

### Comparing `pg_logidater-0.3.2/PKG-INFO` & `pg_logidater-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-logidater
-Version: 0.3.2
+Version: 0.3.3
 Summary: Postgresql logical replication setup utility
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Keywords: postgres
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
```

