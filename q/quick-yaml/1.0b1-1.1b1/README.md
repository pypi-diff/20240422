# Comparing `tmp/quick_yaml-1.0b1.tar.gz` & `tmp/quick_yaml-1.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_yaml-1.0b1.tar", last modified: Mon Apr 15 04:43:27 2024, max compression
+gzip compressed data, was "quick_yaml-1.1b1.tar", last modified: Mon Apr 22 05:28:04 2024, max compression
```

## Comparing `quick_yaml-1.0b1.tar` & `quick_yaml-1.1b1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-15 04:43:27.581939 quick_yaml-1.0b1/
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     7652 2024-04-02 03:58:22.000000 quick_yaml-1.0b1/LICENSE
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       34 2024-04-12 08:36:58.000000 quick_yaml-1.0b1/MANIFEST.in
--rw-r--r--   0 sivarajan  (1000) sivarajan  (1000)    13706 2024-04-15 04:43:27.577939 quick_yaml-1.0b1/PKG-INFO
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    12899 2024-04-15 04:30:32.000000 quick_yaml-1.0b1/README.md
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      879 2024-04-15 04:28:11.000000 quick_yaml-1.0b1/pyproject.toml
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       38 2024-04-15 04:43:27.581939 quick_yaml-1.0b1/setup.cfg
-drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-15 04:43:27.577939 quick_yaml-1.0b1/src/
-drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-15 04:43:27.577939 quick_yaml-1.0b1/src/quick_yaml/
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      435 2024-04-12 09:08:35.000000 quick_yaml-1.0b1/src/quick_yaml/Btree.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    12591 2024-04-15 03:49:34.000000 quick_yaml-1.0b1/src/quick_yaml/DatabaseDaemon.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      291 2024-04-15 03:52:01.000000 quick_yaml-1.0b1/src/quick_yaml/__init__.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    20532 2024-04-12 04:50:03.000000 quick_yaml-1.0b1/src/quick_yaml/data_structures.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    20636 2024-04-15 03:21:51.000000 quick_yaml-1.0b1/src/quick_yaml/manager.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     4722 2024-04-12 04:46:47.000000 quick_yaml-1.0b1/src/quick_yaml/mkdocs.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     3905 2024-04-15 03:31:51.000000 quick_yaml-1.0b1/src/quick_yaml/mock_generator.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    10389 2024-04-12 09:07:33.000000 quick_yaml-1.0b1/src/quick_yaml/parser.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      923 2024-04-15 04:28:11.000000 quick_yaml-1.0b1/src/quick_yaml/setup.py
-drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-15 04:43:27.577939 quick_yaml-1.0b1/src/quick_yaml.egg-info/
--rw-r--r--   0 sivarajan  (1000) sivarajan  (1000)    13706 2024-04-15 04:43:27.000000 quick_yaml-1.0b1/src/quick_yaml.egg-info/PKG-INFO
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      629 2024-04-15 04:43:27.000000 quick_yaml-1.0b1/src/quick_yaml.egg-info/SOURCES.txt
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)        1 2024-04-15 04:43:27.000000 quick_yaml-1.0b1/src/quick_yaml.egg-info/dependency_links.txt
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       62 2024-04-15 04:43:27.000000 quick_yaml-1.0b1/src/quick_yaml.egg-info/requires.txt
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       11 2024-04-15 04:43:27.000000 quick_yaml-1.0b1/src/quick_yaml.egg-info/top_level.txt
-drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-15 04:43:27.577939 quick_yaml-1.0b1/test/
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1835 2024-04-15 03:31:51.000000 quick_yaml-1.0b1/test/test_breeze_query.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1243 2024-04-15 03:31:51.000000 quick_yaml-1.0b1/test/test_byaml.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2532 2024-04-15 03:31:51.000000 quick_yaml-1.0b1/test/test_dbd.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1441 2024-04-15 03:31:51.000000 quick_yaml-1.0b1/test/test_find.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2004 2024-04-15 03:31:51.000000 quick_yaml-1.0b1/test/test_query.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2849 2024-04-15 03:31:51.000000 quick_yaml-1.0b1/test/test_transation.py
--rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2518 2024-04-15 03:31:51.000000 quick_yaml-1.0b1/test/testdb_simple.py
+drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     7652 2024-04-02 03:58:22.000000 quick_yaml-1.1b1/LICENSE
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       34 2024-04-12 08:36:58.000000 quick_yaml-1.1b1/MANIFEST.in
+-rw-r--r--   0 sivarajan  (1000) sivarajan  (1000)    13707 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/PKG-INFO
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    12900 2024-04-17 06:06:52.000000 quick_yaml-1.1b1/README.md
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      879 2024-04-22 05:27:53.000000 quick_yaml-1.1b1/pyproject.toml
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       38 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/setup.cfg
+drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-22 05:28:04.753146 quick_yaml-1.1b1/src/
+drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/src/quick_yaml/
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      435 2024-04-12 09:08:35.000000 quick_yaml-1.1b1/src/quick_yaml/Btree.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     8829 2024-04-22 03:40:11.000000 quick_yaml-1.1b1/src/quick_yaml/DatabaseDaemon.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      291 2024-04-18 10:08:18.000000 quick_yaml-1.1b1/src/quick_yaml/__init__.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    22883 2024-04-22 04:20:07.000000 quick_yaml-1.1b1/src/quick_yaml/data_structures.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    35547 2024-04-22 04:18:15.000000 quick_yaml-1.1b1/src/quick_yaml/manager.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     4722 2024-04-12 04:46:47.000000 quick_yaml-1.1b1/src/quick_yaml/mkdocs.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     3905 2024-04-18 10:08:18.000000 quick_yaml-1.1b1/src/quick_yaml/mock_generator.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)    10389 2024-04-18 10:08:18.000000 quick_yaml-1.1b1/src/quick_yaml/parser.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      923 2024-04-15 04:28:11.000000 quick_yaml-1.1b1/src/quick_yaml/setup.py
+drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/src/quick_yaml.egg-info/
+-rw-r--r--   0 sivarajan  (1000) sivarajan  (1000)    13707 2024-04-22 05:28:04.000000 quick_yaml-1.1b1/src/quick_yaml.egg-info/PKG-INFO
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)      653 2024-04-22 05:28:04.000000 quick_yaml-1.1b1/src/quick_yaml.egg-info/SOURCES.txt
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)        1 2024-04-22 05:28:04.000000 quick_yaml-1.1b1/src/quick_yaml.egg-info/dependency_links.txt
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       62 2024-04-22 05:28:04.000000 quick_yaml-1.1b1/src/quick_yaml.egg-info/requires.txt
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)       11 2024-04-22 05:28:04.000000 quick_yaml-1.1b1/src/quick_yaml.egg-info/top_level.txt
+drwxrwxr-x   0 sivarajan  (1000) sivarajan  (1000)        0 2024-04-22 05:28:04.757146 quick_yaml-1.1b1/test/
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1835 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/test_breeze_query.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1243 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/test_byaml.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1931 2024-04-22 03:40:11.000000 quick_yaml-1.1b1/test/test_concurrent.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2532 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/test_dbd.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     1441 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/test_find.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2004 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/test_query.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2869 2024-04-22 03:41:00.000000 quick_yaml-1.1b1/test/test_transation.py
+-rw-rw-r--   0 sivarajan  (1000) sivarajan  (1000)     2518 2024-04-15 03:31:51.000000 quick_yaml-1.1b1/test/testdb_simple.py
```

### Comparing `quick_yaml-1.0b1/LICENSE` & `quick_yaml-1.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.0b1/PKG-INFO` & `quick_yaml-1.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick_yaml
-Version: 1.0b1
+Version: 1.1b1
 Summary: A simple Database Management System for users who want self-contained DBMS that uses YAML File format to store values.
 Author-email: Sivarajan R <sivarajan931@gmail.com>
 Project-URL: Homepage, https://gitlab.com/eazy-home-admin/BreezeDB/
 Project-URL: Issues, https://gitlab.com/eazy-home-admin/BreezeDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -38,15 +38,15 @@
 # Installation steps
 
 To install the package for python, use pip package manager.
 ```bash
  pip install quick_yaml
  ```
 # Basic Usage
-This section will be expanded later in [https://gitlab.com/eazy-home-admin/BreezeDB/-/wikis/home](Wiki)
+This section will be expanded later in [https://gitlab.com/eazy-home-admin/QuickYAML/-/wikis/home](Wiki)
 ```python
 from quick_yaml.manager import QYAMLDB
 db = QYAMLDB('f.ezdb','f.key',encrypted=True) # Encrpytion by default is optional
 db.create_table('sample', unique_columns=['name'] ) # Indexes to be bought in future.
 data = {'name': 'Test Item', 'value': 42}
 db.insert_new_data('sample', data) # Insert a data 
 ```
```

### Comparing `quick_yaml-1.0b1/README.md` & `quick_yaml-1.1b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Installation steps
 
 To install the package for python, use pip package manager.
 ```bash
  pip install quick_yaml
  ```
 # Basic Usage
-This section will be expanded later in [https://gitlab.com/eazy-home-admin/BreezeDB/-/wikis/home](Wiki)
+This section will be expanded later in [https://gitlab.com/eazy-home-admin/QuickYAML/-/wikis/home](Wiki)
 ```python
 from quick_yaml.manager import QYAMLDB
 db = QYAMLDB('f.ezdb','f.key',encrypted=True) # Encrpytion by default is optional
 db.create_table('sample', unique_columns=['name'] ) # Indexes to be bought in future.
 data = {'name': 'Test Item', 'value': 42}
 db.insert_new_data('sample', data) # Insert a data 
 ```
```

### Comparing `quick_yaml-1.0b1/pyproject.toml` & `quick_yaml-1.1b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "quick_yaml"
-version = "1.0b1"
+version = "1.1b1"
 authors = [
   { name="Sivarajan R", email="sivarajan931@gmail.com" },
 ]
 description = "A simple Database Management System for users who want self-contained DBMS that uses YAML File format to store values."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `quick_yaml-1.0b1/src/quick_yaml/data_structures.py` & `quick_yaml-1.1b1/src/quick_yaml/data_structures.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import logging
+import threading
+
 import jmespath
 import numpy as np
 import pandas as pd
 import yaml
 import base64
 from cryptography.fernet import Fernet
 
@@ -492,15 +495,15 @@
            Returns:
                The encryption key. None if the encryption key cannot be loaded.
         """
         try:
             with open(self.key_file, 'rb') as file:
                 return file.read()
         except FileNotFoundError:
-            return None # Returning None to allow for key generation if not found
+            return None  # Returning None to allow for key generation if not found
 
     def encode_to_binary_yaml(self, data):
         """
            Encodes the given data into binary YAML format, optionally encrypting it, and writes it to the file path.
 
            Parameters:
                data (NestedDict or dict): The data to encode and save.
@@ -567,7 +570,67 @@
             encrypted (bool): Whether to encrypt the binary YAML data. Defaults to False.
         Returns:
             A string of path of the generated binary YAML file and the key file (if encrypted)
             """
         b = BYAML(f'{filename}.ezdb', encrypted, f'{filename}.key')
         b.encode_to_binary_yaml(data)
         return f'{filename}.ezdb', f'{filename}.key'
+
+
+class RecordLock:
+    def __init__(self):
+        self.writer_lock = threading.Semaphore(1)
+        self.mutex = threading.Lock()
+        self.readers = 0
+
+
+class RecordLockManager:
+    def __init__(self, logger=None):
+        self.records = {}
+        self.mutex = threading.Lock()
+        if logger is None:
+            logger = logging.getLogger("RecordLockManager")
+            handler = logging.StreamHandler()
+            formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+            handler.setFormatter(formatter)
+            logger.addHandler(handler)
+            logger.setLevel(logging.DEBUG)
+        self.logger = logger
+
+    def make_record_lock(self, record_id):
+        with self.mutex:
+            if record_id not in self.records:
+                self.records[record_id] = RecordLock()
+                self.logger.debug(f"Record lock created for ID: {record_id}")
+
+    def acquire_writer_lock(self, record_id):
+        with self.mutex:
+            if record_id not in self.records:
+                self.make_record_lock(record_id)
+            self.logger.debug(f"Writer waiting to acquire lock for record {record_id}")
+        self.records[record_id].writer_lock.acquire()
+        self.logger.debug(f"Writer acquired lock for record {record_id}")
+
+    def release_writer_lock(self, record_id):
+        self.records[record_id].writer_lock.release()
+        self.logger.debug(f"Writer released lock for record {record_id}")
+
+    def acquire_reader_lock(self, record_id):
+        with self.mutex:
+            if record_id not in self.records:
+                self.make_record_lock(record_id)
+            record = self.records[record_id]
+            record.mutex.acquire()
+
+        record.readers += 1
+        if record.readers == 1:
+            record.writer_lock.acquire()
+        record.mutex.release()
+        self.logger.debug(f"Reader acquired lock for record {record_id}, total readers: {record.readers}")
+
+    def release_reader_lock(self, record_id):
+        with self.records[record_id].mutex:
+            record = self.records[record_id]
+            record.readers -= 1
+            self.logger.debug(f"Reader released lock for record {record_id}, remaining readers: {record.readers}")
+            if record.readers == 0:
+                record.writer_lock.release()
```

### Comparing `quick_yaml-1.0b1/src/quick_yaml/manager.py` & `quick_yaml-1.1b1/src/quick_yaml/manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,29 @@
+import logging
+import time
+from threading import Semaphore, Lock
+
 import jmespath
 
 from .data_structures import BYAML, NestedDict
 from .parser import QueryProcessor
 import pandas as pd
 import copy
 
 
 class MetaData:
+    """
+    A class for storing table metadata
+
+    Attributes:
+        - version (float): The version of the metadata.
+        - unique_columns (list): A list of unique columns for the table.
+        - indexes (list): A list of indexes for the table.
+    """
+
     def __init__(self):
         """
         Initialize the object with an empty dictionary for storing tables.
         """
         self.tables = {}  # A dictionary to hold table-specific metadata
 
     def add_table(self, table_name, unique_columns=None, indexes=None):
@@ -41,54 +54,98 @@
 
     def get_indexes(self, table_name):
         """Returns the indexes for the given table."""
         return self.tables[table_name]['indexes']
 
 
 class QYAMLDB:
+    # TODO: Implement Logs for each command.
     """
-    quick_yaml class represents a simple in-memory database system.
+    A simple and easy-to-use database manager without thread safety
+
+    Attributes:
+        - path (str) : path of database
+        - key_file (str): path of key file
+        - encrypted (bool): flag indicating if encryption is enabled
+        - byaml (BYAML): BYAML instance
+        - log_file (str): path of log file
+        - enable_logging (bool): flag indicating if logging is enabled
+        - log_level (int): level of logging
+        - silent (bool): flag indicating if logging is silent
 
     Methods:
         - __init__: Initialize the database.
         - add_table: Add a table to the database.
         - insert_data: Insert data into a specified table.
-        - query_data: Query data from a specified table.
+        - execute_query: Query data from a specified table.
         - delete_data: Delete data from a specified table.
     """
-    def __init__(self, path, key_file='key.file', encrypted=False,byaml=None):
+
+    def __init__(self, path, key_file='key.file', encrypted=False, byaml=None, log_file='qyaml.log',
+                 enable_logging=True,
+                 log_level=logging.DEBUG, silent=False):
         """
           Initializes the quick_yaml instance.
           Parameters:
               path (str): The file path for the database.
               key_file (str): The file path for the encryption key. Defaults to 'key.file'.
               encrypted (bool): Flag indicating whether encryption is enabled. Defaults to False.
               byaml (BYAML): An existing BYAML instance. If not provided, a new BYAML instance is created.
           Raises:
               ValueError: If the file format is invalid.
           Returns:
               None
           """
+
         if not path.endswith('.ezdb'):
             raise ValueError('Invalid file format. Must use ".ezdb" extension.')
         self.path = path
         self.key_file = key_file
         self.encrypted = encrypted
-        self.transaction_mode = False
+        self.logger_enabled = enable_logging
         self._backup_table = None
         self.byaml = byaml or BYAML(self.path, encryption_enabled=self.encrypted, key_file=self.key_file)
-        self.tables: dict = {}  # Use a dict to manage multiple tables, each with its data and metadata
+        self.tables: dict = {}  # Use a dict to manage multiple tables, each with its data and metadata4
+        # Logging Operations
+        if enable_logging:
+            self._setup_logger(log_file, log_level, not silent)
+        else:
+            self._logger = None
+
+    def _setup_logger(self, log_file, log_level, print_to_console):
+        self._logger = logging.getLogger('QYAMLDB')
+        self._logger.setLevel(log_level)
+        fh = logging.FileHandler(log_file)
+        fh.setLevel(log_level)
+        formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+        fh.setFormatter(formatter)
+        self._logger.addHandler(fh)
+        if print_to_console:
+            ch = logging.StreamHandler()
+            ch.setLevel(log_level)
+            ch.setFormatter(formatter)
+            self._logger.addHandler(ch)
+
+    def _log(self, message, level='debug'):
+        if self.logger_enabled:
+            getattr(self._logger, level)(message)
 
     def save_db(self):
         """Saves the current state of the database to a file."""
 
         to_save = {table_name: {'metadata': table_info['metadata'].to_dict(),
                                 'data': table_info['data'].to_dict()} for table_name, table_info in
                    self.tables.items()}
-        self.byaml.encode_to_binary_yaml(to_save)
+        self._log(f"Saving database to {self.path}", 'info')
+
+        try:
+            self.byaml.encode_to_binary_yaml(to_save)
+            self._log(f"Saved database to {self.path}", 'info')
+        except Exception as e:
+            self._log(f"Failed to save database: {e}", 'error')
 
     def create_table(self, table_name, unique_columns=None, indexes=None):
         """
         Creates a new table in the database.
 
         Parameters:
             table_name (str): The name of the table to create.
@@ -96,22 +153,24 @@
             indexes (list, optional): List of column names to index. Defaults to None.
         Returns:
             str: "done." if the table is created successfully.
         Raises:
             ValueError: If the table already exists.
         """
         if table_name in self.tables:
+            self._log(f"Table '{table_name}' already exists.", 'error')
             raise ValueError(f"Table '{table_name}' already exists.")
         metadata = MetaData()
         metadata.add_table(table_name, unique_columns, indexes)  # MetaData is adjusted to handle this
         self.tables[table_name] = {
             'metadata': metadata,
             'data': NestedDict()
         }
         self.save_db()
+        self._log(f"Created table '{table_name}'.", 'info')
         return "done."
 
     def load_db(self):
         """
         Load the database by decoding the contents from binary YAML and populating the tables dictionary with metadata
          and data.
 
@@ -179,15 +238,16 @@
         Returns:
             str: A message indicating the insertion operation is done.
         """
         try:
             for i in list_of_values:
                 if type(i) is dict or isinstance(i, NestedDict):
                     self.insert_new_data(table_name, i)
-                    return 'done'
+
+
         except Exception:
             print("Error inserting values")
 
     def get_data_by_id(self, table_name, entry_id):
         """
         A function that retrieves data by ID from a specific table.
 
@@ -210,15 +270,15 @@
             entry_id (str): ID of the entry
             updated_data (NestedDict/Dict): Data to be updated.
         """
         if table_name not in self.tables or entry_id not in self.tables[table_name]['data'].get_dict():
             raise ValueError("Table or entry does not exist.")
         print(
             f"DEBUG Table {self.tables[table_name]['data'][entry_id]} type{type(self.tables[table_name]['data'][entry_id])}")
-        if entry_id not in self.tables[table_name]['data']:
+        if entry_id not in self.tables[table_name]['data'].keys():
             return KeyError("Entry does not exist.")
         self.tables[table_name]['data'][entry_id].update(updated_data)
         self.save_db()
         return 'done'
 
     def update_many(self, table_name, condition, update_data, flags=None):
         """ Updates data based on given condition
@@ -308,15 +368,15 @@
         matching_ids = qp.results
         # for each matching records, delete the record
         for entry_id in matching_ids:
             del self.tables[table_name]['data'][entry_id]
         self.save_db()
         return "done"
 
-    def find_jmes(self, table_name, query):
+    def find_jmes(self, table_name, query: str):
         """
         Finds data in the specified table based on a query.
         This uses Jmespath query to find the data in the dictionary
         Parameters:
             table_name (str): The name of the table to search in.
             query (dict): The query to filter the data.
         Returns:
@@ -345,14 +405,15 @@
            """
         # check if table exists
         if table_name not in self.tables:
             raise ValueError(f"Table '{table_name}' does not exist.")
         data = self.tables[table_name]['data'].to_dict()
         executor = QueryProcessor(data)
         executor.process_query(query)
+
         return executor.results
 
     def find(self, table_name, query):
         """
            Finds and filters data in the specified table based on a query.
            Parameters:
                table_name (str): The name of the table to search in.
@@ -387,14 +448,15 @@
         Returns:
             pandas.DataFrame: The converted DataFrame.
 
         Raises:
             ValueError: If the table does not exist in the database.
         """
         if table_name not in self.tables:
+            self._log(f"Executed method to_pandas. Table '{table_name}' does not exist.", 'error')
             raise ValueError(f"Table '{table_name}' does not exist.")
 
         # Extract data from the specified table
         data = self.tables[table_name]['data'].to_dict()
 
         # Flatten the data and convert it into a format suitable for DataFrame creation
         flattened_data = []
@@ -405,68 +467,85 @@
                     entry_data_flat[key] = ', '.join(map(str, value))  # Convert lists to comma-separated strings
                 else:
                     entry_data_flat[key] = value
             flattened_data.append(entry_data_flat)
 
         # Create and return the DataFrame
         df = pd.DataFrame(flattened_data)
+        self._log(f'Result {df}')
         return df
 
-    def begin_transaction(self, data, break_on_invalid_command=True):
+    def begin_transaction(self, data):
         """
         Emulates a transaction processing system.
 
         Parameters:
             data (dict): Dictionary data to be processed
-            break_on_invalid_command (bool): Flag that is used to indicate whether to break on invalid translations.
+
+        Raises:
+            ValueError: If the error strategy is not one of the valid values.
 
         Returns:
             dict: A dictionary containing the status, error message, and transaction details.
         """
 
         # Create a backup copy of the tables
         self._backup_table = copy.deepcopy(self.tables)
 
         # Initialize transaction report
         transaction_report = {
             'successful_operations': 0,
             'failed_operation': 0,
-            'list_of_failed_operations': []
+            'list_of_failed_operations_id': []
         }
 
         # Get the transactional data and error strategy from input data
         transactional_data = data.get('$operations', [])
         error_strategy = data.get('$error_strategy', 'rollback')
+        on_invalid_command = data.get('$on_invalid_command', 'rollback')
 
         # Ensure error_strategy is valid
         if error_strategy not in ('rollback', 'continue', 'break'):
             error_strategy = 'rollback'
 
         for i in transactional_data:
+            transaction_id = i.get('$transaction_id', None)
             try:
+
                 status = self.execute_command(i)
-                if status == 'Invalid command' and break_on_invalid_command:
-                    break
+                if status == 'Invalid command':
+                    if on_invalid_command == 'rollback':
+                        self.tables = self._backup_table
+                        transaction_report['failed_operation'] += len(transactional_data) - transaction_report[
+                            'successful_operations']
+                        return {'status': 'Failure', 'error_message': 'Invalid command', 'details': transaction_report}
+                    elif on_invalid_command == 'break':
+                        transaction_report['failed_operation'] += len(transactional_data) - transaction_report[
+                            'successful_operations']
+                        return {'status': 'Failure', 'error_message': 'Invalid command', 'details': transaction_report}
+                    elif on_invalid_command == 'continue':
+                        transaction_report['list_of_failed_operations_id'].append(transaction_id)
+                        continue
                 transaction_report['successful_operations'] += 1
             except Exception as e:
                 if error_strategy == 'rollback':
                     self.tables = self._backup_table
                     transaction_report['failed_operation'] += len(transactional_data) - transaction_report[
                         'successful_operations']
                     return {'status': 'Failure', 'error_message': str(e), 'details': transaction_report}
                 elif error_strategy == 'break':
                     transaction_report['failed_operation'] += len(transactional_data) - transaction_report[
                         'successful_operations']
                     return {'status': 'Failure', 'error_message': str(e), 'details': transaction_report}
                 elif error_strategy == 'continue':
-                    transaction_report['list_of_failed_operations'].append(i)
+                    transaction_report['list_of_failed_operations_id'].append(transaction_id)
                     continue
 
         # Determine final status based on failed operations
-        stat = "Success" if len(transaction_report['list_of_failed_operations']) == 0 else "Finished with errors"
+        stat = "Success" if len(transaction_report['list_of_failed_operations_id']) == 0 else "Finished with errors"
         return {'status': stat, 'error_message': None, 'details': transaction_report}
 
     def execute_command(self, i):
         """
         Execute a command based on the given input type.
         Parameters:
             i (dict): The input command to be executed.
@@ -493,7 +572,388 @@
         elif i['type'] == '$delete_many' or '$del_many':
             return self.delete_many(i['$table_name'], i['$condition'])
         elif i['type'] == '$create_table':
 
             return self.create_table(i['$table_name'], i['$unique_columns'], None)
         elif i['type'] == '$query':
             return self.execute_query(i['$table_name'], i['$query_data'])
+
+
+class QYAMLDBCoarse(QYAMLDB):
+    """
+   QYAMLDBCoarse is a subclass designed to handle locks in a coarse-grained manner. This is ideal for environments
+    where simplicity and preventing race conditions are prioritized over operation throughput.
+
+    Inherits from:
+        QYAMLDB: The base class for database operations.
+
+
+    Attributes:
+        - _mutex (threading.Semaphore): A semaphore used to synchronize access to the database.
+        - _writers_lock (threading.Semaphore): A semaphore used to synchronize access to the writers.
+        - _readers (int): The number of _readers currently accessing the database.
+
+    """
+
+    # include all the arguments from base class
+    def __init__(self, path, key_file='key.file', encrypted=False, byaml=None, log_file='qyaml.log',
+                 enable_logging=True,
+                 log_level=logging.DEBUG, silent=False):
+        super().__init__(path, key_file, encrypted, byaml, log_file, enable_logging, log_level, silent)
+
+        self._mutex = Semaphore(1)
+        self._writers_lock = Semaphore(1)
+        self._readers = 0
+        self._writers_waiting = False
+        self._data_lock = Lock()
+        self.logger_enabled = enable_logging
+
+    def _start_write(self, agent='Writer'):
+        """
+        Function to acquire the writer lock.
+        """
+        self._log(f'{agent} Waiting to acquire writer lock. With {self._readers} _readers', 'debug')
+        self._mutex.acquire()
+        self._writers_waiting = True
+
+        self._mutex.release()
+
+        self._log(f'{agent} Acquired writer lock. With {self._readers} _readers', 'debug')
+        self._writers_lock.acquire()
+
+    def _end_write(self, agent='Writer'):
+        """
+        Function to release the writer lock.
+        """
+        self._log(f'Releasing writer lock. With {self._readers} _readers', 'debug')
+        self._writers_lock.release()
+
+        self._mutex.acquire()
+        self._writers_waiting = False
+        self._mutex.release()
+
+        self._log(f'Released writer lock.With {self._readers} _readers', 'debug')
+
+    def _start_read(self):
+        """
+        Function to acquire the reader lock.
+        """
+        self._log('Waiting to acquire reader lock', 'debug')
+        self._mutex.acquire() # Acquire mutex lock to synchronize readers attaining lock
+        while self._writers_waiting:
+            # Release all the readers until writers are finished.
+            self._log(f'Lock Released due to waiting of writers. No of _readers {self._readers}')
+            self._mutex.release() # Release mutex in favor of writers
+            time.sleep(0.1)  # Sleep to prevent busy waiting
+            self._mutex.acquire() # Again Try to aqquire locks.
+
+
+        self._log('Acquired reader lock', 'debug')
+        self._readers += 1
+
+        if self._readers == 1:
+            self._log('Waiting for writers lock by _readers', 'debug')
+            self._writers_lock.acquire()
+            self._log('Writers Lock acquired by _readers.', 'debug')
+        self._mutex.release()
+        self._log(f'No of _readers {self._readers}', 'debug')
+
+    def _end_read(self):
+        """Function to release reader lock."""
+        self._log('Releasing reader lock', 'debug')
+        self._mutex.acquire()
+
+        self._readers -= 1
+        self._log(f'Released reader lock. No of Readers {self._readers}', 'debug')
+        if self._readers == 0:
+            self._writers_lock.release()
+        self._mutex.release()
+
+    def create_table(self, table_name, unique_columns=None, indexes=None):
+        """
+        Thread-safe version of create_table.
+        Parameters:
+            table_name (str): The name of the table to create.
+            unique_columns (list, optional): List of column names that should be unique. Defaults to None.
+            indexes (list, optional): List of column names to index. Defaults to None.
+
+        Returns:
+            str: "done." if the table is created successfully.
+
+        Raises:
+            Exception: If the table already exists.
+        """
+        self._start_write()
+        result = None
+        try:
+            result = super().create_table(table_name, unique_columns, indexes)
+        except Exception as e:
+            result = e
+        finally:
+            self._end_write()  # Ensure that lock is released despite exceptions
+        if isinstance(result, Exception):
+            raise result
+
+        return result
+
+    def insert_new_data(self, table_name, data):
+        """
+        Thread-safe version of insert_data.
+        Parameters:
+            table_name (str): The name of the table to insert into.
+            data (dict): The data to insert.
+
+        Returns:
+            str: "done." if the data is inserted successfully.
+
+        Raises:
+            Exception: If the table is not found.
+        """
+        self._start_write()
+        result = None
+        try:
+            result = super().insert_new_data(table_name, data)
+        except Exception as e:
+            result = e
+        finally:
+            self._end_write()
+
+        if isinstance(result, Exception):
+            raise result
+        return result
+
+    def insert_many(self, table_name, data):
+        """
+        Thread-safe version of insert_many.
+        Beware of this function is not ACID compliant. Use begin_translation if you need ACID compliance.
+        Parameters:
+            table_name (str): The name of the table to insert into.
+            data (list): The data to insert.
+
+        Returns:
+            str: "done." if the data is inserted successfully.
+
+        Raises:
+            ValueError: When the data is not found or it viloates unique constraint.
+        """
+        self._start_write()
+        try:
+            result = super().insert_many(table_name, data)
+        except Exception as e:
+            result = e
+        finally:
+            self._end_write()
+
+        if isinstance(result, Exception):
+            raise result
+
+        return result
+
+    def update_entry(self, table_name, entry_id, updated_data):
+        """
+        Thread-safe version of update_entry.
+
+        Parameters:
+            table_name (str): The name of the table to update.
+            entry_id (str): The ID of the entry to update.
+            updated_data (dict): The data to update.
+
+        Returns:
+            str: "done." if the update is successful.
+
+        Raises:
+            ValueError: If the table or entry does not exist.
+        """
+        self._start_write()
+        results = None
+        try:
+            results = super().update_entry(table_name, entry_id, updated_data)
+        except Exception as e:
+            results = e
+        finally:
+            self._end_write()
+
+        if isinstance(results, Exception):
+            raise results
+
+        return results
+
+    def update_many(self, table_name, condition, updated_data, flags=None):
+        """
+        Thread-safe version of update_many.
+        Beware of this function is not ACID compliant. Use begin_translation if you need ACID compliance.
+
+        Parameters:
+            table_name (str): The name of the table to update.
+            condition (dict): The condition to match on.
+            updated_data (dict): The data to update.
+            flags (dict, optional): The flags to use. Defaults to None.
+
+        Returns:
+            str: "done." if the update is successful.
+
+        Raises:
+            ValueError: If the table or entry does not exist.
+        """
+        self._start_write()
+        result = None
+        try:
+            result = super().update_many(table_name, condition, updated_data, flags)
+        except Exception as e:
+            result = e
+        finally:
+            self._end_write()
+
+        if isinstance(result, Exception):
+            raise result
+
+        return result
+
+    def delete_entry(self, table_name, entry_id):
+        """
+        Thread-safe version of delete_entry.
+
+        Parameters:
+            table_name (str): The name of the table to delete from.
+            entry_id (str): The unique identifier of the entry to be deleted.
+
+        Returns:
+            str: "done." if the deletion is successful.
+
+        Raises:
+            ValueError: If the table or entry does not exist.
+        """
+        self._start_write()
+        result = super().delete_entry(table_name, entry_id)
+        self._end_write()
+        return result
+
+    def delete_many(self, table_name, query):
+        """
+        Thread-safe version of delete_many
+        Parameters:
+            table_name (str): The name of the table to delete from.
+            query (dict): The query to filter the records to be deleted.
+
+        Returns:
+            str: "done." if the data is deleted successfully.
+
+        Raises:
+            Exception: If the table is not found.
+
+        """
+        self._start_write()
+        try:
+            result = super().delete_many(table_name, query)
+        except Exception as e:
+            result = e
+        finally:
+            self._end_write()
+
+        if isinstance(result, Exception):
+            raise result
+
+        return result
+
+    def find_jmes(self, table_name, query: str):
+        """
+        Thread-safe version of find_jmes.
+        """
+        self._start_read()
+        try:
+            result = super().find_jmes(table_name, query)
+        except Exception as e:
+            result = e
+        finally:
+            self._end_read()
+
+        if isinstance(result, Exception):
+            raise result
+
+        return result
+
+    def find_all(self, table_name):
+        """
+        Thread-safe version of find_all.
+        """
+        self._start_read()
+        result = None
+        try:
+            result = super().find_all(table_name)
+        except Exception as e:
+            result = e
+        finally:
+            self._end_read()
+
+        if isinstance(result, Exception):
+            raise result
+        return result
+
+    def execute_query(self, table_name, query_data):
+        """
+        Thread-safe version of execute_query.
+        """
+        self._start_read()
+        result = None
+        try:
+            result = super().execute_query(table_name, query_data)
+        except Exception as e:
+            result = e
+        finally:
+            self._end_read()
+
+        if isinstance(result, Exception):
+            raise result
+
+        return result
+
+    def get_data_by_id(self, table_name, entry_id):
+        """
+
+        A function that retrieves data by ID from a specific table. (Threadsafe)
+
+        Parameters:
+            table_name (str): The name of the table to retrieve data from.
+            entry_id (int): The ID of the entry to retrieve.
+
+        Returns:
+            contents: The data associated with the provided entry ID in the specified table.
+        """
+
+        self._start_read()
+        result = None
+        try:
+            result = super().get_data_by_id(table_name, entry_id)
+        except Exception as e:
+            result = e
+        finally:
+            self._end_read()
+
+        if isinstance(result, Exception):
+            raise result
+
+        return result
+
+    def to_pandas(self, table_name):
+        """
+        Thread-safe version of to_pandas.
+        """
+        self._start_read()
+        result = None
+        try:
+            result = super().to_pandas(table_name)
+        except Exception as e:
+            result = e
+        finally:
+            self._end_read()
+
+        if isinstance(result, Exception):
+            raise result
+
+        return result
+
+
+class QYAMLDBFine(QYAMLDB):
+    """
+    A subclass of QYAMLDB that implements fine-grained locking. It implements read/write lock in record level.
+    """
+    pass
```

### Comparing `quick_yaml-1.0b1/src/quick_yaml/mkdocs.py` & `quick_yaml-1.1b1/src/quick_yaml/mkdocs.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.0b1/src/quick_yaml/mock_generator.py` & `quick_yaml-1.1b1/src/quick_yaml/mock_generator.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.0b1/src/quick_yaml/parser.py` & `quick_yaml-1.1b1/src/quick_yaml/parser.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.0b1/src/quick_yaml/setup.py` & `quick_yaml-1.1b1/src/quick_yaml/setup.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.0b1/src/quick_yaml.egg-info/PKG-INFO` & `quick_yaml-1.1b1/src/quick_yaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick_yaml
-Version: 1.0b1
+Version: 1.1b1
 Summary: A simple Database Management System for users who want self-contained DBMS that uses YAML File format to store values.
 Author-email: Sivarajan R <sivarajan931@gmail.com>
 Project-URL: Homepage, https://gitlab.com/eazy-home-admin/BreezeDB/
 Project-URL: Issues, https://gitlab.com/eazy-home-admin/BreezeDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -38,15 +38,15 @@
 # Installation steps
 
 To install the package for python, use pip package manager.
 ```bash
  pip install quick_yaml
  ```
 # Basic Usage
-This section will be expanded later in [https://gitlab.com/eazy-home-admin/BreezeDB/-/wikis/home](Wiki)
+This section will be expanded later in [https://gitlab.com/eazy-home-admin/QuickYAML/-/wikis/home](Wiki)
 ```python
 from quick_yaml.manager import QYAMLDB
 db = QYAMLDB('f.ezdb','f.key',encrypted=True) # Encrpytion by default is optional
 db.create_table('sample', unique_columns=['name'] ) # Indexes to be bought in future.
 data = {'name': 'Test Item', 'value': 42}
 db.insert_new_data('sample', data) # Insert a data 
 ```
```

### Comparing `quick_yaml-1.0b1/src/quick_yaml.egg-info/SOURCES.txt` & `quick_yaml-1.1b1/src/quick_yaml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,12 +14,13 @@
 src/quick_yaml.egg-info/PKG-INFO
 src/quick_yaml.egg-info/SOURCES.txt
 src/quick_yaml.egg-info/dependency_links.txt
 src/quick_yaml.egg-info/requires.txt
 src/quick_yaml.egg-info/top_level.txt
 test/test_breeze_query.py
 test/test_byaml.py
+test/test_concurrent.py
 test/test_dbd.py
 test/test_find.py
 test/test_query.py
 test/test_transation.py
 test/testdb_simple.py
```

### Comparing `quick_yaml-1.0b1/test/test_breeze_query.py` & `quick_yaml-1.1b1/test/test_breeze_query.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.0b1/test/test_byaml.py` & `quick_yaml-1.1b1/test/test_byaml.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.0b1/test/test_dbd.py` & `quick_yaml-1.1b1/test/test_dbd.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.0b1/test/test_find.py` & `quick_yaml-1.1b1/test/test_find.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.0b1/test/test_query.py` & `quick_yaml-1.1b1/test/test_query.py`

 * *Files identical despite different names*

### Comparing `quick_yaml-1.0b1/test/test_transation.py` & `quick_yaml-1.1b1/test/test_transation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import unittest
-from src.quick_yaml.manager import  QYAMLDB
+from src.quick_yaml.manager import QYAMLDB, QYAMLDBCoarse
 import os
 import tempfile
 
 
 class TestEazyDB(unittest.TestCase):
     def setUp(self):
         # Create a temporary file to serve as the database
         self.db_file = tempfile.NamedTemporaryFile(delete=False)
         self.db_path = self.db_file.name + '.ezdb'  # Ensuring the file has the correct extension
         # Initialize the database with the temporary file path
-        self.db = QYAMLDB(self.db_path, encrypted=False)
+        self.db = QYAMLDBCoarse(self.db_path, encrypted=False)
 
     def tearDown(self):
         # Close and remove the temporary database file
         os.unlink(self.db_path)
 
     def test_create_table(self):
         """Test creating a table works correctly."""
```

### Comparing `quick_yaml-1.0b1/test/testdb_simple.py` & `quick_yaml-1.1b1/test/testdb_simple.py`

 * *Files identical despite different names*

