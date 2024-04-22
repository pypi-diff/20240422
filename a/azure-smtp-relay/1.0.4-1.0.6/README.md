# Comparing `tmp/azure_smtp_relay-1.0.4.tar.gz` & `tmp/azure_smtp_relay-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_smtp_relay-1.0.4.tar", last modified: Wed Dec 20 06:27:00 2023, max compression
+gzip compressed data, was "azure_smtp_relay-1.0.6.tar", last modified: Mon Apr 22 02:00:49 2024, max compression
```

## Comparing `azure_smtp_relay-1.0.4.tar` & `azure_smtp_relay-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-12-20 06:27:00.167434 azure_smtp_relay-1.0.4/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1069 2023-11-14 05:26:03.000000 azure_smtp_relay-1.0.4/LICENSE
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    14493 2023-12-20 06:27:00.163433 azure_smtp_relay-1.0.4/PKG-INFO
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    13317 2023-12-19 05:11:39.000000 azure_smtp_relay-1.0.4/README.md
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1228 2023-12-19 05:28:24.000000 azure_smtp_relay-1.0.4/pyproject.toml
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       38 2023-12-20 06:27:00.167434 azure_smtp_relay-1.0.4/setup.cfg
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-12-20 06:27:00.159433 azure_smtp_relay-1.0.4/src/
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-12-20 06:27:00.163433 azure_smtp_relay-1.0.4/src/azure_smtp_relay/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4944 2023-12-19 05:28:24.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay/__init__.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    10603 2023-12-19 05:10:57.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay/__main__.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     7349 2023-11-13 06:27:30.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay/address_list.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     5160 2023-11-27 05:19:28.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay/config.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    13989 2023-11-27 05:18:42.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay/handler.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    20807 2023-12-20 03:04:21.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay/relay.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    15326 2023-12-18 02:19:15.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay/toml_config_mgr.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-12-20 06:27:00.163433 azure_smtp_relay-1.0.4/src/azure_smtp_relay.egg-info/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    14493 2023-12-20 06:27:00.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay.egg-info/PKG-INFO
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      487 2023-12-20 06:27:00.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay.egg-info/SOURCES.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        1 2023-12-20 06:27:00.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay.egg-info/dependency_links.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      186 2023-12-20 06:27:00.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay.egg-info/requires.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       17 2023-12-20 06:27:00.000000 azure_smtp_relay-1.0.4/src/azure_smtp_relay.egg-info/top_level.txt
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2024-04-22 02:00:49.608496 azure_smtp_relay-1.0.6/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1069 2023-11-14 05:26:03.000000 azure_smtp_relay-1.0.6/LICENSE
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    14493 2024-04-22 02:00:49.608496 azure_smtp_relay-1.0.6/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    13317 2023-12-19 05:11:39.000000 azure_smtp_relay-1.0.6/README.md
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1228 2024-04-22 01:52:43.000000 azure_smtp_relay-1.0.6/pyproject.toml
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       38 2024-04-22 02:00:49.608496 azure_smtp_relay-1.0.6/setup.cfg
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2024-04-22 02:00:49.604496 azure_smtp_relay-1.0.6/src/
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2024-04-22 02:00:49.608496 azure_smtp_relay-1.0.6/src/azure_smtp_relay/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4944 2024-04-22 01:52:43.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay/__init__.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    10603 2023-12-19 05:10:57.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay/__main__.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     7349 2023-11-13 06:27:30.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay/address_list.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     5160 2023-11-27 05:19:28.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay/config.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    13989 2023-11-27 05:18:42.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay/handler.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    20807 2023-12-20 03:04:21.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay/relay.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    15294 2023-12-27 03:30:39.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay/toml_config_mgr.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2024-04-22 02:00:49.608496 azure_smtp_relay-1.0.6/src/azure_smtp_relay.egg-info/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    14493 2024-04-22 02:00:49.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay.egg-info/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      487 2024-04-22 02:00:49.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay.egg-info/SOURCES.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        1 2024-04-22 02:00:49.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay.egg-info/dependency_links.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      186 2024-04-22 02:00:49.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay.egg-info/requires.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       17 2024-04-22 02:00:49.000000 azure_smtp_relay-1.0.6/src/azure_smtp_relay.egg-info/top_level.txt
```

### Comparing `azure_smtp_relay-1.0.4/LICENSE` & `azure_smtp_relay-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `azure_smtp_relay-1.0.4/PKG-INFO` & `azure_smtp_relay-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure_smtp_relay
-Version: 1.0.4
+Version: 1.0.6
 Summary: Python SMTP service using aiosmtpd that relays through Azure Email Communication Service
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: homepage, https://www.learningtopi.com/python-modules-applications/azure_smtp_relay/
 Project-URL: bug tracker, https://github.com/LearningToPi/azure_smtp_relay/issues
 Project-URL: source code, https://github.com/LearningToPi/azure_smtp_relay
 Keywords: queue,thread,async
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `azure_smtp_relay-1.0.4/README.md` & `azure_smtp_relay-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `azure_smtp_relay-1.0.4/pyproject.toml` & `azure_smtp_relay-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "azure_smtp_relay"
-version = "1.0.4"
+version = "1.0.6"
 description = "Python SMTP service using aiosmtpd that relays through Azure Email Communication Service"
 authors = [{name = "Thomas Dunteman", email= "git@learningtopi.com"}]
 keywords = ["queue", "thread", "async"]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
 	"License :: OSI Approved :: MIT License",
```

### Comparing `azure_smtp_relay-1.0.4/src/azure_smtp_relay/__init__.py` & `azure_smtp_relay-1.0.6/src/azure_smtp_relay/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,8 +90,8 @@
 
 """
 
 from azure.identity import ClientSecretCredential
 from azure.core.credentials import AzureKeyCredential
 from .relay import AzureSmtpRelay
 
-VERSION = (1, 0, 4)    # updated 2023-12-18 22:28:24.700365 from : (1, 0, 3)
+VERSION = (1, 0, 6)    # updated 2024-04-21 18:52:43.027265 from : (1, 0, 5)
```

### Comparing `azure_smtp_relay-1.0.4/src/azure_smtp_relay/__main__.py` & `azure_smtp_relay-1.0.6/src/azure_smtp_relay/__main__.py`

 * *Files identical despite different names*

### Comparing `azure_smtp_relay-1.0.4/src/azure_smtp_relay/address_list.py` & `azure_smtp_relay-1.0.6/src/azure_smtp_relay/address_list.py`

 * *Files identical despite different names*

### Comparing `azure_smtp_relay-1.0.4/src/azure_smtp_relay/config.py` & `azure_smtp_relay-1.0.6/src/azure_smtp_relay/config.py`

 * *Files identical despite different names*

### Comparing `azure_smtp_relay-1.0.4/src/azure_smtp_relay/handler.py` & `azure_smtp_relay-1.0.6/src/azure_smtp_relay/handler.py`

 * *Files identical despite different names*

### Comparing `azure_smtp_relay-1.0.4/src/azure_smtp_relay/relay.py` & `azure_smtp_relay-1.0.6/src/azure_smtp_relay/relay.py`

 * *Files identical despite different names*

### Comparing `azure_smtp_relay-1.0.4/src/azure_smtp_relay/toml_config_mgr.py` & `azure_smtp_relay-1.0.6/src/azure_smtp_relay/toml_config_mgr.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         """
         String representation of the IP object.
 
         Returns:
             str: String representation of the IP object.
         """
         return str(self.ip)
-    
+
 class network:
     """
     Represents an IP network.
 
     Attributes:
         network (ipcalc.Network): Network object.
 
@@ -106,15 +106,15 @@
         """
         String representation of the Network object.
 
         Returns:
             str: String representation of the Network object.
         """
         return str(self.network)
-    
+
 class email:
     """
     Represents an email address.
 
     Attributes:
         email (str): Email address.
 
@@ -143,15 +143,15 @@
         """
         String representation of the Email object.
 
         Returns:
             str: String representation of the Email object.
         """
         return self.email
-    
+
 class domain:
     """
     Represents a domain.
 
     Attributes:
         domain (str): Domain name.
 
@@ -208,15 +208,15 @@
 
         Returns:
             None
         """
         if not validators.url(url_string):
             raise ValueError(f"URL '{url_string}' is not valid.")
         self.url = url_string
-        
+
     def __str__(self):
         """
         String representation of the URL object.
 
         Returns:
             str: String representation of the URL object.
         """
@@ -354,24 +354,24 @@
         for section in self._config:
             for key, settings in self._config[section].items():
                 if settings.get('required', False) and (settings.get('value', None) is None and settings.get('default') is None):
                     if section not in missing_params:
                         missing_params[section] = {}
                     missing_params[section] = self._config[section][key]
         return missing_params
-    
+
     def sections(self) -> list:
         """
         Return a list of the config sections.
 
         Returns:
             list: List of section names.
         """
         return list(self._config.keys())
-    
+
     def section_keys(self, section:str) -> list:
         """
         Return a list of keys in a specific section.
 
         Args:
             section (str): The section name.
 
@@ -397,15 +397,15 @@
                 } for section in self._config.keys()
             }
             if section is None:
                 return config
             else:
                 return config[section]
         raise ValueError(f"Required configuration has not been provided. Missing values: {self.required_parameters_missing}")
-    
+
     def update_argparser(self, parser=None) -> argparse.ArgumentParser:
         """
         Update or create an ArgumentParser with configuration parameters.
 
         Args:
             parser (argparse.ArgumentParser, optional): The ArgumentParser object to update. Defaults to None.
```

### Comparing `azure_smtp_relay-1.0.4/src/azure_smtp_relay.egg-info/PKG-INFO` & `azure_smtp_relay-1.0.6/src/azure_smtp_relay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: azure-smtp-relay
-Version: 1.0.4
+Name: azure_smtp_relay
+Version: 1.0.6
 Summary: Python SMTP service using aiosmtpd that relays through Azure Email Communication Service
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: homepage, https://www.learningtopi.com/python-modules-applications/azure_smtp_relay/
 Project-URL: bug tracker, https://github.com/LearningToPi/azure_smtp_relay/issues
 Project-URL: source code, https://github.com/LearningToPi/azure_smtp_relay
 Keywords: queue,thread,async
 Classifier: License :: OSI Approved :: MIT License
```

