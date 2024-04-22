# Comparing `tmp/rfb_driver_db-0.0.1.tar.gz` & `tmp/rfb_driver_db-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfb_driver_db-0.0.1.tar", last modified: Thu Mar  7 13:56:09 2024, max compression
+gzip compressed data, was "rfb_driver_db-0.0.2.tar", last modified: Mon Apr 22 07:07:57 2024, max compression
```

## Comparing `rfb_driver_db-0.0.1.tar` & `rfb_driver_db-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:56:09.869784 rfb_driver_db-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43009 2024-03-07 13:56:09.869784 rfb_driver_db-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 13:56:09.869784 rfb_driver_db-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:56:09.865784 rfb_driver_db-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:56:09.869784 rfb_driver_db-0.0.1/src/rfb_driver_db/
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/src/rfb_driver_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-07 13:56:09.000000 rfb_driver_db-0.0.1/src/rfb_driver_db/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/src/rfb_driver_db/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_dao_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_dao_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_dao_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_dao_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-03-07 13:55:32.000000 rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:56:09.869784 rfb_driver_db-0.0.1/src/rfb_driver_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43009 2024-03-07 13:56:09.000000 rfb_driver_db-0.0.1/src/rfb_driver_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-07 13:56:09.000000 rfb_driver_db-0.0.1/src/rfb_driver_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 13:56:09.000000 rfb_driver_db-0.0.1/src/rfb_driver_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-07 13:56:09.000000 rfb_driver_db-0.0.1/src/rfb_driver_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-07 13:56:09.000000 rfb_driver_db-0.0.1/src/rfb_driver_db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:07:57.433493 rfb_driver_db-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43009 2024-04-22 07:07:57.433493 rfb_driver_db-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:07:57.433493 rfb_driver_db-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:07:57.429493 rfb_driver_db-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:07:57.429493 rfb_driver_db-0.0.2/src/rfb_driver_db/
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/src/rfb_driver_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 07:07:57.000000 rfb_driver_db-0.0.2/src/rfb_driver_db/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/src/rfb_driver_db/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_dao_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_dao_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_dao_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_dao_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-22 07:07:30.000000 rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:07:57.433493 rfb_driver_db-0.0.2/src/rfb_driver_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43009 2024-04-22 07:07:57.000000 rfb_driver_db-0.0.2/src/rfb_driver_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-22 07:07:57.000000 rfb_driver_db-0.0.2/src/rfb_driver_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:07:57.000000 rfb_driver_db-0.0.2/src/rfb_driver_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 07:07:57.000000 rfb_driver_db-0.0.2/src/rfb_driver_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 07:07:57.000000 rfb_driver_db-0.0.2/src/rfb_driver_db.egg-info/top_level.txt
```

### Comparing `rfb_driver_db-0.0.1/LICENSE.txt` & `rfb_driver_db-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rfb_driver_db-0.0.1/PKG-INFO` & `rfb_driver_db-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb_driver_db
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple database connector for SQLAlchemy. It is used to 
 Author-email: Javier Sanz <javiersanzmoline@gmail.com>, Raldea <r.aldea.csic+pypi@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `rfb_driver_db-0.0.1/README.md` & `rfb_driver_db-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rfb_driver_db-0.0.1/pyproject.toml` & `rfb_driver_db-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rfb_driver_db-0.0.1/src/rfb_driver_db/__init__.py` & `rfb_driver_db-0.0.2/src/rfb_driver_db/__init__.py`

 * *Files identical despite different names*

### Comparing `rfb_driver_db-0.0.1/src/rfb_driver_db/context.py` & `rfb_driver_db-0.0.2/src/rfb_driver_db/context.py`

 * *Files identical despite different names*

### Comparing `rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_dao_base.py` & `rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_dao_base.py`

 * *Files identical despite different names*

### Comparing `rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_dao_cache.py` & `rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_dao_cache.py`

 * *Files identical despite different names*

### Comparing `rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_dao_master.py` & `rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_dao_master.py`

 * *Files identical despite different names*

### Comparing `rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_dao_utils.py` & `rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_dao_utils.py`

 * *Files identical despite different names*

### Comparing `rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_engine.py` & `rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     err: Error while connecting with DB.
     ConnectionError: Max db connection resets reached. Connection with db may have been lost.
 '''
 #######################        MANDATORY IMPORTS         #######################
 from __future__ import annotations
 #######################         GENERIC IMPORTS          #######################
 from typing import Any
+from datetime import datetime
 
 #######################       THIRD PARTY IMPORTS        #######################
 # SQL Alchemy
 from sqlalchemy import create_engine
 from sqlalchemy.engine.base import Engine
 from sqlalchemy.orm import Session
-
 #######################    SYSTEM ABSTRACTION IMPORTS    #######################
 from rfb_config_tool import sys_conf_read_config_params
 from rfb_logger_tool import Logger, sys_log_logger_get_module_logger
 log: Logger = sys_log_logger_get_module_logger(__name__)
 
 #######################          PROJECT IMPORTS         #######################
 
@@ -52,33 +52,29 @@
         # read connection parameters
         self.config_file = config_file
         section='database'
         if db_type == DrvDbTypeE.CACHE_DB:
             section = 'cache_db'
         if db_type == DrvDbTypeE.MASTER_DB:
             section = 'master_db'
+        self.section = section
         try:
-            params = sys_conf_read_config_params(filename=config_file, section= section)
+            params = sys_conf_read_config_params(filename=config_file, section= self.section)
 
             # create engine
-            if db_type == DrvDbTypeE.CACHE_DB:
-                url = 'mysql+mysqlconnector://'
-            elif db_type == DrvDbTypeE.MASTER_DB:
-                url = 'mysql+mysqlconnector://'
-                section = 'cache_db'
-            else:
-                raise ConnectionError("Data base type or engine not supported")
+            url = 'mysql+mysqlconnector://' + params['user'] + ':'\
+                    + params['password'] + '@' + params['host'] + ':'\
+                    + str(params['port']) + '/' + params['database']
 
-            url += params['user'] + ':' + params['password'] + '@' \
-                    + params['host'] + ':' + str(params['port']) + '/' + params['database']
             log.debug(f"Creating database engine with url: [{url}]")
             self.engine: Engine = create_engine(url=url, echo=False, future=True)
             self.session : Session = Session(bind=self.engine, future=True)
             self.session.begin()
             self.n_resets = 0
+            self.__last_connection = datetime.now()
 
         except Exception as err:
             log.error(msg="Error on DB Session creation. Please check DB " +\
                       f"credentials and params: {params}")
             log.error(msg=err)
             raise err
 
@@ -93,43 +89,54 @@
                 Defaults to False.
 
         Raises:
             err: Throw an exception if any error occurs during commit transaction.
         '''
         try:
             self.session.commit()
+            self.__last_connection = datetime.now()
         except Exception as err:
             log.critical(err)
             log.critical("Error while commiting change to DB. Performing rollback...")
             self.session.rollback()
             if raise_exception:
                 raise err
 
+    def check_connection(self) -> None:
+        '''
+        Check when has been the last connection with the database and reconnect with it
+        '''
+        elapsed_time = datetime.now() - self.__last_connection
+        if elapsed_time.seconds > 30:
+            log.warning((f"Database {self.section} last connection "
+                         "was 30s ago, trying to connect again"))
+            self.__reset_engine()
 
     def close_connection(self) -> None:
         '''
         Close the connection with the database.
         '''
         self.commit_changes()
         self.session.close()
 
 
     def __reset_engine(self) -> None:
         '''
         Create a new engine and initialize it
         '''
         params: dict[str, Any] = sys_conf_read_config_params(#pylint: disable=unsubscriptable-object
-            filename=self.config_file, section='database')
+            filename=self.config_file, section=self.section)
 
         url = 'mysql+mysqlconnector://' + params['user'] + ':'\
             + params['password'] + '@' + params['host'] + ':'\
             + str(params['port']) + '/' + params['database']
         self.engine = create_engine(url, echo=False, future=True)
         self.session = Session(self.engine, future=True)
         self.session.begin()
+        self.__last_connection = datetime.now()
 
 
     def reset(self) -> None:
         '''
         Resets the connection to the database .
 
         Raises:
```

### Comparing `rfb_driver_db-0.0.1/src/rfb_driver_db/drv_db_types.py` & `rfb_driver_db-0.0.2/src/rfb_driver_db/drv_db_types.py`

 * *Files identical despite different names*

### Comparing `rfb_driver_db-0.0.1/src/rfb_driver_db.egg-info/PKG-INFO` & `rfb_driver_db-0.0.2/src/rfb_driver_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfb_driver_db
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple database connector for SQLAlchemy. It is used to 
 Author-email: Javier Sanz <javiersanzmoline@gmail.com>, Raldea <r.aldea.csic+pypi@gmail.com>, Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `rfb_driver_db-0.0.1/src/rfb_driver_db.egg-info/SOURCES.txt` & `rfb_driver_db-0.0.2/src/rfb_driver_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

