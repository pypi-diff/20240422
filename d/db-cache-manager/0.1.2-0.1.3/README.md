# Comparing `tmp/db_cache_manager-0.1.2.tar.gz` & `tmp/db_cache_manager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_cache_manager-0.1.2.tar", last modified: Thu Apr 18 10:42:15 2024, max compression
+gzip compressed data, was "db_cache_manager-0.1.3.tar", last modified: Mon Apr 22 07:38:18 2024, max compression
```

## Comparing `db_cache_manager-0.1.2.tar` & `db_cache_manager-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:42:15.176619 db_cache_manager-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/src/db_cache_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/src/db_cache_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32586 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/src/db_cache_manager/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-18 10:42:15.000000 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-18 10:42:15.000000 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:42:15.000000 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 10:42:15.000000 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 10:42:15.000000 db_cache_manager-0.1.2/src/db_cache_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:42:15.180619 db_cache_manager-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-18 10:42:10.000000 db_cache_manager-0.1.2/tests/test_cache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:38:18.988830 db_cache_manager-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 07:38:14.000000 db_cache_manager-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-22 07:38:18.988830 db_cache_manager-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-04-22 07:38:14.000000 db_cache_manager-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-22 07:38:14.000000 db_cache_manager-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:38:18.988830 db_cache_manager-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:38:18.984830 db_cache_manager-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:38:18.988830 db_cache_manager-0.1.3/src/db_cache_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:38:14.000000 db_cache_manager-0.1.3/src/db_cache_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32859 2024-04-22 07:38:14.000000 db_cache_manager-0.1.3/src/db_cache_manager/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:38:18.988830 db_cache_manager-0.1.3/src/db_cache_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-22 07:38:18.000000 db_cache_manager-0.1.3/src/db_cache_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-22 07:38:18.000000 db_cache_manager-0.1.3/src/db_cache_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:38:18.000000 db_cache_manager-0.1.3/src/db_cache_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-22 07:38:18.000000 db_cache_manager-0.1.3/src/db_cache_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 07:38:18.000000 db_cache_manager-0.1.3/src/db_cache_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:38:18.988830 db_cache_manager-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-22 07:38:14.000000 db_cache_manager-0.1.3/tests/test_cache_manager.py
```

### Comparing `db_cache_manager-0.1.2/LICENSE` & `db_cache_manager-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `db_cache_manager-0.1.2/PKG-INFO` & `db_cache_manager-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db_cache_manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: Custom database connector and cache manager with default support for fingerprinting and fingerprint lookups, DAG-like chains of identical rows, and cache tables that reference each other.
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>, Aitor Pérez <aitor.perez@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/db-cache-manager
 Project-URL: Bug Tracker, https://github.com/epflgraph/db-cache-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `db_cache_manager-0.1.2/README.md` & `db_cache_manager-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `db_cache_manager-0.1.2/pyproject.toml` & `db_cache_manager-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "db_cache_manager"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" },
   { name="Aitor Pérez", email="aitor.perez@epfl.ch" }
 ]
 description = "Custom database connector and cache manager with default support for fingerprinting and fingerprint lookups, DAG-like chains of identical rows, and cache tables that reference each other."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `db_cache_manager-0.1.2/src/db_cache_manager/db.py` & `db_cache_manager-0.1.3/src/db_cache_manager/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,27 +427,29 @@
             results = [{column_list[i]: result[i] for i in range(len(column_list))} for result in results]
         else:
             results = None
         return results
 
     def _get_all_details(self, table_name, cols, start=0, limit=-1, exclude_token=None, allow_nulls=True,
                          earliest_date=None, latest_date=None, equality_conditions=None, has_date_col=False,
-                         sort_by_date_col=True, use_date_modified_col=False):
+                         sort_by_date_col=True, sort_by_id_token=True, use_date_modified_col=False):
         """
         Internal method. Gets the details of all rows in a table, with some conditions.
         Args:
             table_name: Table name
             cols: Columns to retrieve
             start: The offset parameter of the LIMIT clause
             limit: the limit parameter of the LIMIT clause
             exclude_token: List of tokens to exclude
             allow_nulls: Whether to allow null values or to exclude rows where any of the required columns is null
             earliest_date: The earliest date to include
             equality_conditions: Equality conditions
-            has_date_col: Whether the table has a date_added column, which would be used to sort the results.
+            has_date_col: Whether the table has a date_added column be used to sort the results.
+            sort_by_date_col: Whether to use the date col (if existing) to sort
+            sort_by_id_token: Whether to use the id token col to sort, overridden by sort_by_date_col
             use_date_modified_col: Whether to use the date_modified or the date_added column for comparisons
                 with `earliest_date` or `latest_date`.
         Returns:
             Dictionary mapping each id_token to a dictionary of column name : values.
         """
         all_values = list()
         column_list = ['id_token'] + cols
@@ -481,15 +483,15 @@
             query += add_where_or_and(query)
             eq_condition_str, eq_condition_values = add_equality_conditions(equality_conditions)
             query += eq_condition_str
             all_values.extend(eq_condition_values)
         # ORDER BY comes before LIMIT but after WHERE
         if has_date_col and sort_by_date_col:
             query += "\nORDER BY date_added"
-        else:
+        elif sort_by_id_token:
             query += "\nORDER BY id_token"
         if limit != -1:
             query += f"""
             LIMIT {start},{limit}
             """
         results = self.db.execute_query(query, values=tuple(all_values))
         if len(results) > 0:
@@ -748,15 +750,16 @@
 
     def get_all_closest_matches(self):
         """
         Retrieves all the rows in the closest match table
         Returns:
             All rows in most similar token table
         """
-        results = self._get_all_details(self.most_similar_table, ['most_similar_token'], has_date_col=False)
+        results = self._get_all_details(self.most_similar_table, ['most_similar_token'],
+                                        has_date_col=False, sort_by_id_token=False)
         if results is not None:
             return {x: results[x]['most_similar_token'] for x in results
                     if results[x]['most_similar_token'] is not None}
         return None
 
 
 class ExampleDBCachingManager(DBCachingManagerBase):
```

### Comparing `db_cache_manager-0.1.2/src/db_cache_manager.egg-info/PKG-INFO` & `db_cache_manager-0.1.3/src/db_cache_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db_cache_manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: Custom database connector and cache manager with default support for fingerprinting and fingerprint lookups, DAG-like chains of identical rows, and cache tables that reference each other.
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>, Aitor Pérez <aitor.perez@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/db-cache-manager
 Project-URL: Bug Tracker, https://github.com/epflgraph/db-cache-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `db_cache_manager-0.1.2/tests/test_cache_manager.py` & `db_cache_manager-0.1.3/tests/test_cache_manager.py`

 * *Files identical despite different names*

