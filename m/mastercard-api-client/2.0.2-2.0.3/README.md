# Comparing `tmp/mastercard_api_client-2.0.2.tar.gz` & `tmp/mastercard_api_client-2.0.3.tar.gz`

## Comparing `mastercard_api_client-2.0.2.tar` & `mastercard_api_client-2.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/_version.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/__init__.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/baseobject.py
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/config.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/constants.py
--rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/controller.py
--rw-r--r--   0        0        0     8777 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/exceptions.py
--rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/model.py
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/util.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/security/__init__.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/security/authentication.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/security/oauth.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/security/util.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/.gitignore
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/README.md
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/_version.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/core/__init__.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/core/baseobject.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/core/config.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/core/constants.py
+-rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/core/controller.py
+-rw-r--r--   0        0        0     8777 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/core/exceptions.py
+-rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/core/model.py
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/core/util.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/security/__init__.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/security/authentication.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/security/oauth.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/mastercardapicore/security/util.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/.gitignore
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/README.md
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.3/PKG-INFO
```

### Comparing `mastercard_api_client-2.0.2/.github/workflows/publish.yaml` & `mastercard_api_client-2.0.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/mastercardapicore/core/baseobject.py` & `mastercard_api_client-2.0.3/mastercardapicore/core/baseobject.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/mastercardapicore/core/config.py` & `mastercard_api_client-2.0.3/mastercardapicore/core/config.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/mastercardapicore/core/constants.py` & `mastercard_api_client-2.0.3/mastercardapicore/core/constants.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/mastercardapicore/core/controller.py` & `mastercard_api_client-2.0.3/mastercardapicore/core/controller.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/mastercardapicore/core/exceptions.py` & `mastercard_api_client-2.0.3/mastercardapicore/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/mastercardapicore/core/model.py` & `mastercard_api_client-2.0.3/mastercardapicore/core/model.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/mastercardapicore/core/util.py` & `mastercard_api_client-2.0.3/mastercardapicore/core/util.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/mastercardapicore/security/authentication.py` & `mastercard_api_client-2.0.3/mastercardapicore/security/authentication.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/mastercardapicore/security/oauth.py` & `mastercard_api_client-2.0.3/mastercardapicore/security/oauth.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/mastercardapicore/security/util.py` & `mastercard_api_client-2.0.3/mastercardapicore/security/util.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/.gitignore` & `mastercard_api_client-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/pyproject.toml` & `mastercard_api_client-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.2/PKG-INFO` & `mastercard_api_client-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mastercard-api-client
-Version: 2.0.2
+Version: 2.0.3
 Summary: MasterCard API Python Core SDK, fork of the mastercard-api-core library.
 Author-email: Twisto Platform <platform@twisto.cz>
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

