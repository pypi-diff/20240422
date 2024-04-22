# Comparing `tmp/sislv4utils-0.0.5.tar.gz` & `tmp/sislv4utils-0.0.6.tar.gz`

## Comparing `sislv4utils-0.0.5.tar` & `sislv4utils-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/src/sislv4utils/__init__.py
--rw-r--r--   0        0        0     9310 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/src/sislv4utils/config.py
--rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/src/sislv4utils/elastic.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/src/sislv4utils/message.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/src/sislv4utils/mqtt.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/src/sislv4utils/objectstore.py
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/src/sislv4utils/service.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/LICENSE
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/README.md
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 sislv4utils-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/src/sislv4utils/__init__.py
+-rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/src/sislv4utils/config.py
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/src/sislv4utils/elastic.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/src/sislv4utils/message.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/src/sislv4utils/mqtt.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/src/sislv4utils/objectstore.py
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/src/sislv4utils/service.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/README.md
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 sislv4utils-0.0.6/PKG-INFO
```

### Comparing `sislv4utils-0.0.5/src/sislv4utils/config.py` & `sislv4utils-0.0.6/src/sislv4utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 import logging
 import configparser
 from os.path import join as make_path
 import etcd3
 from enum import Enum
 
 class Provider(Enum):
-        ETCD = 0,
-        FILE = 1
+        AUTO = 0
+        ETCD = 1,
+        FILE = 2,
 
 class Config(object):
     # region members
 
     _logformat = '%(asctime)s : %(levelname)s - %(filename)s (line: %(lineno)d) %(funcName)s() -> %(message)s'
     _rundir_ = 'run'
     _tmpdir_ = 'tmp'
     _etcd_host = os.getenv('ETCD_HOST', '')
     _etcd_port = int(os.getenv('ETCD_PORT', 2379))
     _etcd_root = os.getenv('ETCD_ROOT', '/')
-    _provider = Provider.ETCD
+    _provider = Provider.AUTO
 
     WAR_OPTIONVAL = 'Unable to parse value for option [{0}::{1}].'
     ERR_PARSEFAIL = 'Error parsing config file.'
 
     # endregion
 
     # region properties
@@ -116,15 +117,16 @@
         if not self._mqtt: raise NotImplementedError
         return self._mqtt['value']
 
     # endregion
     
     # region methods
 
-    def __init__(self, provider: Provider = Provider.ETCD):
+    def __init__(self, provider: Provider = Provider.AUTO):
+        if provider == Provider.AUTO: provider = Provider.FILE if not Config._etcd_host else Provider.ETCD
         Config._provider = provider
 
         # base path; all other folders will be relative to this path
         self._moddir = os.path.dirname(
             sys.modules[self.__class__.__module__].__file__)
 
         # the run folder; if not available make one
```

### Comparing `sislv4utils-0.0.5/src/sislv4utils/elastic.py` & `sislv4utils-0.0.6/src/sislv4utils/elastic.py`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.5/src/sislv4utils/message.py` & `sislv4utils-0.0.6/src/sislv4utils/message.py`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.5/src/sislv4utils/mqtt.py` & `sislv4utils-0.0.6/src/sislv4utils/mqtt.py`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.5/src/sislv4utils/objectstore.py` & `sislv4utils-0.0.6/src/sislv4utils/objectstore.py`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.5/src/sislv4utils/service.py` & `sislv4utils-0.0.6/src/sislv4utils/service.py`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.5/.gitignore` & `sislv4utils-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.5/LICENSE` & `sislv4utils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sislv4utils-0.0.5/pyproject.toml` & `sislv4utils-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sislv4utils"
-version = "0.0.5"
+version = "0.0.6"
 
 authors = [
   { name="Bibhas Das", email="bibhas.das@somnetics.in" },
 ]
 
 description = "Seamless v4 utilities"
```

### Comparing `sislv4utils-0.0.5/PKG-INFO` & `sislv4utils-0.0.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.3
-Name: sislv4utils
-Version: 0.0.5
-Summary: Seamless v4 utilities
-Author-email: Bibhas Das <bibhas.das@somnetics.in>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Requires-Dist: elasticsearch>=8.13.0
-Requires-Dist: etcd3>=0.12.0
-Requires-Dist: falcon>=3.1.3
-Requires-Dist: minio>=7.2.5
-Requires-Dist: paho-mqtt>=2.0.0
-Requires-Dist: pika>=1.3.2
-Requires-Dist: protobuf==3.20.3
-Requires-Dist: requests>=2.25.1
-Description-Content-Type: text/markdown
-
 ## Seamless V4 Utilities
 (code-url: https://github.com/sislv4/sislv4utils)
 
 Companion utility library for Seamless v4 architecture
 
 **Install**
 ```
@@ -31,14 +11,19 @@
 **Uninstall**
 ```
 pip3 uninstall sislv4utils
 ```
 
 ## Version History
 
+**v0.0.6**
++ A new enum value Provider.AUTO has been introduced in Config
+    - Setting provider to Auto will check if ETCD_HOST have been defined as environment variable in runtime
+    - if Yes, then all config._provider will be set to ETCD; else it will be set to FILE
+
 **v0.0.5**
 + MessageQueue constructor now accepts Config object instead of host, port etc
 + MqttcClient constructor now accepts Config object instead of host, port etc
 + ObjectStore constructor now accepts Config object instead of host, port etc
 + Service class and its derived classes have been modified accordingly
 
 **v0.0.4**
```

