# Comparing `tmp/localdatamanager-0.0.6.tar.gz` & `tmp/localdatamanager-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localdatamanager-0.0.6.tar", last modified: Sun Apr 21 21:32:45 2024, max compression
+gzip compressed data, was "localdatamanager-0.1.0.tar", last modified: Mon Apr 22 02:28:49 2024, max compression
```

## Comparing `localdatamanager-0.0.6.tar` & `localdatamanager-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:32:45.687640 localdatamanager-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 21:32:41.000000 localdatamanager-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-21 21:32:45.687640 localdatamanager-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-21 21:32:41.000000 localdatamanager-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-21 21:32:41.000000 localdatamanager-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 21:32:45.687640 localdatamanager-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:32:45.683640 localdatamanager-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:32:45.683640 localdatamanager-0.0.6/src/LocalDataManager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 21:32:41.000000 localdatamanager-0.0.6/src/LocalDataManager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-04-21 21:32:41.000000 localdatamanager-0.0.6/src/LocalDataManager/file_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:32:45.687640 localdatamanager-0.0.6/src/LocalDataManager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-21 21:32:45.000000 localdatamanager-0.0.6/src/LocalDataManager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-21 21:32:45.000000 localdatamanager-0.0.6/src/LocalDataManager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 21:32:45.000000 localdatamanager-0.0.6/src/LocalDataManager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 21:32:45.000000 localdatamanager-0.0.6/src/LocalDataManager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 21:32:45.000000 localdatamanager-0.0.6/src/LocalDataManager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:32:45.687640 localdatamanager-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-21 21:32:41.000000 localdatamanager-0.0.6/test/test_file_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.555317 localdatamanager-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.555317 localdatamanager-0.1.0/src/LocalDataManager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/src/LocalDataManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/src/LocalDataManager/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/src/LocalDataManager/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/src/LocalDataManager/db/db_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/src/LocalDataManager/file_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/src/LocalDataManager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-22 02:28:49.000000 localdatamanager-0.1.0/src/LocalDataManager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-22 02:28:49.000000 localdatamanager-0.1.0/src/LocalDataManager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 02:28:49.000000 localdatamanager-0.1.0/src/LocalDataManager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 02:28:49.000000 localdatamanager-0.1.0/src/LocalDataManager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 02:28:49.000000 localdatamanager-0.1.0/src/LocalDataManager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:28:49.559317 localdatamanager-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-22 02:28:43.000000 localdatamanager-0.1.0/test/test_file_management.py
```

### Comparing `localdatamanager-0.0.6/LICENSE` & `localdatamanager-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `localdatamanager-0.0.6/PKG-INFO` & `localdatamanager-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: LocalDataManager
-Version: 0.0.6
+Version: 0.1.0
 Summary: A package for facilitating local file management
 Author-email: Blaine Perry <blainecperry@gmail.com>
 Project-URL: Homepage, https://github.com/bcperry/LocalDataManager
 Project-URL: Issues, https://github.com/bcperry/LocalDataManager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
+Requires-Dist: sqlalchemy
 
 
 
 -----------------
 
 # ``LocalDataManager``: Python-based Data Management and Indexing
```

### Comparing `localdatamanager-0.0.6/README.md` & `localdatamanager-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `localdatamanager-0.0.6/pyproject.toml` & `localdatamanager-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LocalDataManager"
-version = "0.0.6"
+version = "0.1.0"
 authors = [
   { name="Blaine Perry", email="blainecperry@gmail.com" },
 ]
 description = "A package for facilitating local file management"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "pandas"
+  "pandas",
+  "sqlalchemy"
 ]
 [project.urls]
 Homepage = "https://github.com/bcperry/LocalDataManager"
 Issues = "https://github.com/bcperry/LocalDataManager/issues"
```

### Comparing `localdatamanager-0.0.6/src/LocalDataManager/file_manager.py` & `localdatamanager-0.1.0/src/LocalDataManager/file_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import sqlite3
 import hashlib
 import logging
 import pandas as pd
 from io import BytesIO
 from sqlite3 import Error
 
+# ORM for databasing 
+from .db.db_classes import Base, File
+from sqlalchemy import create_engine, select
+from sqlalchemy.pool import NullPool
+from sqlalchemy.orm import Session
+
+
 from typing import Union, Literal
 
 
 class FileManager: 
     """
     A class to represent a the File Manager.
     ...
@@ -33,15 +40,15 @@
     :check_names:
     :get_managed_files_df:
     :save_file:
     :save_dataframe:
 
     """
 
-    def __init__(self, base_path: os.PathLike = None, db_file:str = 'filemanager.db', data_arch:Union[Literal['medallion'], Literal['levels']] = 'medallion'):
+    def __init__(self, base_path: os.PathLike = None, db_file:str = 'filemanager.db', data_arch:Union[Literal['medallion'], Literal['levels']] = 'medallion', verbose = False):
         """
         Constructs all the necessary attributes for the file manager object.
 
         Parameters
         ----------
         :base_path: the path to the data management system
         :db_file: the name of the sqlite database used to manage the files
@@ -60,46 +67,18 @@
         if self.data_arch == 'medallion':
             self.data_levels = ['bronze', 'silver', 'gold']
         elif self.data_arch =='levels':
             self.data_levels = ['level_1', 'level_2', 'level_3']
 
         try:
             self.create_management_folders()
-            connection = sqlite3.connect(os.path.join(self.base_path, db_file))
-            self.connection = connection
-            self.create_management_table()
-        except Error as e:
-            logging.info(e)
- 
-    def close_connection(self):
-        self.connection.close()
-
-    def create_management_table(self, SQL:str=None):
-        """ create a file management table in the SQLite database
-        :param SQL: SQL command to create the table
-        :param connection: a database connection
-
-        :return: Boolean
-        """
-        if SQL is None:
-            SQL = """ CREATE TABLE IF NOT EXISTS files (
-                                                name text NOT NULL,
-                                                hash text PRIMARY KEY,
-                                                location text NOT NULL
-                                            ); """
-
-
-        try:
-            c = self.connection.cursor()
-            c.execute(SQL)
+            self.engine = create_engine(f"sqlite:///{os.path.join(base_path,db_file)}", echo=verbose, poolclass=NullPool)
+            Base.metadata.create_all(self.engine)
         except Error as e:
             logging.info(e)
-            return False
-
-        return True
 
     def create_management_folders(self):
         """ create the folders required to manage the files
         :param path: string filepath in which to create the management structure
         :param data_arch: [medallion, levels] data scheme for which to create
 
         :return: Boolean
@@ -121,20 +100,22 @@
 
     def insert_file_into_files(self, name: str, hash: str, location: os.PathLike):
         """
         Create a new file into the files table
         :param file:
         :return: file id
         """
-        sql = ''' INSERT INTO files(name,hash,location)
-                VALUES(?,?,?) '''
-        cur = self.connection.cursor()
-        cur.execute(sql, (name, hash, location))
-        self.connection.commit()
-        return cur.lastrowid
+        with Session(self.engine) as session:
+            file = File(name=name,
+                        hash=hash,
+                        location=location
+                        )
+            session.add(file)
+            session.commit()
+        return f"{name} Managed"
 
     def hash_file(self, file: BytesIO):
         """
         Provides hashing functionality.
 
         Parameters:
             file:
@@ -174,22 +155,18 @@
         Parameters:
             None
 
         Returns:
             List of all hashes 
 
         """
-        # Creating cursor object using connection object
-        cursor = self.connection.cursor()
-            
-        # executing our sql query
-        cursor.execute("""SELECT hash FROM files;""")
-            
-        # create a list of all hashes
-        hashlist = [i[0] for i in cursor.fetchall()]
+        
+        with Session(self.engine) as session:
+            stmt = select(File.hash)
+            hashlist = list(session.scalars(stmt))
 
         return hashlist
 
     def check_hashes(self, hash: str):
         """
         Provides functionality to check if a file has been hashed previously.
 
@@ -215,22 +192,17 @@
         Parameters:
             None:
 
         Returns:
             list of all managed filenames 
 
         """
-        # Creating cursor object using connection object
-        cursor = self.connection.cursor()
-            
-        # executing our sql query
-        cursor.execute("""SELECT name FROM files;""")
-            
-        # create a list of all hashes
-        namelist = [i[0] for i in cursor.fetchall()]
+        with Session(self.engine) as session:
+            stmt = select(File.name)
+            namelist = list(session.scalars(stmt))
 
         return namelist
 
     def check_names(self, filename: str):
         """
         Provides functionality to check if a file with the same name exists.
 
@@ -256,23 +228,22 @@
         Parameters:
             None
 
         Returns:
             dataframe of all managed file information 
 
         """
-        # Creating cursor object using connection object
-        cursor = self.connection.cursor()
-            
-        # executing our sql query
-        cursor.execute("""SELECT * FROM files;""")
-            
-        # create a list of all hashes
-        files = cursor.fetchall()
-        df = pd.DataFrame(files, columns=['filename', 'hash', 'location'])
+        df = pd.read_sql_table('files', self.engine)
+        # # df = pd.read_sql_table('table_name', 'postgres:///db_name')  
+        # with Session(self.engine) as session:
+        #     stmt = select(File)
+        #     files = list(session.scalars(stmt))
+        # # Convert ORM query result to a DataFrame
+        # df = pd.DataFrame([item.to_dict() for item in files])
+        # # df = pd.DataFrame(files, columns=['filename', 'hash', 'location'])
 
         return df
 
     def save_file(self, file: BytesIO, data_level: str):
         """
         Provides functionality to save documents per the data management
         system.
@@ -321,15 +292,15 @@
                     data = file.read(self.BUF_SIZE)
                     if not data:
                         break
                     f.write(data)
 
             # with the file saved, add it to the database
             self.insert_file_into_files(name=filename, hash=hash, location=path)
-            return True
+            return f"{filename} managed"
         except Exception as err:
             logging.error(err)
             return err
 
     def save_dataframe(self, dataframe: pd.DataFrame, name: str, data_level: str):
         """
         Provides functionality to convert dataframes to csvs for storage in the data management
```

### Comparing `localdatamanager-0.0.6/src/LocalDataManager.egg-info/PKG-INFO` & `localdatamanager-0.1.0/src/LocalDataManager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: LocalDataManager
-Version: 0.0.6
+Version: 0.1.0
 Summary: A package for facilitating local file management
 Author-email: Blaine Perry <blainecperry@gmail.com>
 Project-URL: Homepage, https://github.com/bcperry/LocalDataManager
 Project-URL: Issues, https://github.com/bcperry/LocalDataManager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
+Requires-Dist: sqlalchemy
 
 
 
 -----------------
 
 # ``LocalDataManager``: Python-based Data Management and Indexing
```

### Comparing `localdatamanager-0.0.6/test/test_file_management.py` & `localdatamanager-0.1.0/test/test_file_management.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import shutil
 
 class TestFileManager(unittest.TestCase):
     '''For testing the File class'''
 
     @classmethod
     def tearDownClass(self) -> None:
-        self.manager.connection.close()
         shutil.rmtree('data')
 
     @classmethod
     def setUpClass(self):
 
         # create the required folder
         if not os.path.exists('data'):
@@ -22,45 +21,39 @@
             except:
                 print(f'Failed to create data directory')
                 pass
         
         # stand up the file manager
         from src.LocalDataManager.file_manager import FileManager
         self.manager = FileManager(base_path= 'data', db_file='testFile.db')
-        self.manager.create_management_table()
         self.manager.insert_file_into_files('name', 'hash', 'location')
 
 
     def test_import(self):
         """ Test that the Data Management module can be imported. """
         import src.LocalDataManager
 
-    def test_create_management_table(self):
-        """ Test the database connection. """
-        table = self.manager.create_management_table()
-        self.manager.create_management_table()
-        self.assertTrue(table)
 
     def test_create_management_folders(self):
         """ Test the creation of the Folder structure"""
         manager = self.manager.create_management_folders()
         self.assertTrue(manager)
 
     def test_hash_file(self):
         """ Test the file hashing"""
 
         # Reading a file 
         file = open(r'test/testfile.txt', mode='rb')
         # print(file.read())
         hash = self.manager.hash_file(file)
-        self.assertEquals(hash , '9f86d081884c7d659a2feaa0c55ad015a3bf4f1b2b0b822cd15d6c15b0f00a08')
+        self.assertEqual(hash , '9f86d081884c7d659a2feaa0c55ad015a3bf4f1b2b0b822cd15d6c15b0f00a08')
 
     def test_insert_file_into_files(self):
         result = self.manager.insert_file_into_files('name.txt', 'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855', 'location')
-        self.assertGreaterEqual(result, 0)
+        self.assertEqual(result, "name.txt Managed")
 
     def test_check_hashes(self):
         self.assertTrue(self.manager.check_hashes('hash'))
         self.assertFalse(self.manager.check_hashes('not_here'))
 
     def test_check_names(self):
         self.assertTrue(self.manager.check_names('name'))
```

