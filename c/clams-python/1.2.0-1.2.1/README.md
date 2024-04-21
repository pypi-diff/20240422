# Comparing `tmp/clams-python-1.2.0.tar.gz` & `tmp/clams_python-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-1.2.0.tar", last modified: Thu Apr 11 14:18:10 2024, max compression
+gzip compressed data, was "clams_python-1.2.1.tar", last modified: Sun Apr 21 22:13:16 2024, max compression
```

## Comparing `clams-python-1.2.0.tar` & `clams_python-1.2.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.853357 clams-python-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-11 14:17:48.000000 clams-python-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 14:17:48.000000 clams-python-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-11 14:18:10.853357 clams-python-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-11 14:17:48.000000 clams-python-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 14:17:49.000000 clams-python-1.2.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.845357 clams-python-1.2.0/clams/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.845357 clams-python-1.2.0/clams/app/
--rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.845357 clams-python-1.2.0/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (127)    21677 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.845357 clams-python-1.2.0/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/.dockerignore.template
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/Containerfile.template
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/LICENSE.template
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/README.md.template
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/app.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/metadata.py.template
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/app/requirements.txt.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/develop/templates/gha/
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/gha/for-clams-team.md.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/develop/templates/gha/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/gha/workflows/issue-assign.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/gha/workflows/issue-close.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/develop/templates/gha/workflows/publish.yml.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/mmif_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/mmif_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/mmif_utils/rewind.py
--rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/mmif_utils/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 14:17:48.000000 clams-python-1.2.0/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.849357 clams-python-1.2.0/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.853357 clams-python-1.2.0/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 14:18:10.000000 clams-python-1.2.0/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 14:17:49.000000 clams-python-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:18:10.853357 clams-python-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-11 14:17:49.000000 clams-python-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:18:10.853357 clams-python-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    23502 2024-04-11 14:17:49.000000 clams-python-1.2.0/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-11 14:17:49.000000 clams-python-1.2.0/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.213550 clams_python-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-21 22:12:50.000000 clams_python-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-21 22:12:50.000000 clams_python-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-21 22:13:16.213550 clams_python-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-21 22:12:50.000000 clams_python-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 22:12:50.000000 clams_python-1.2.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.205550 clams_python-1.2.1/clams/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.205550 clams_python-1.2.1/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    19005 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.205550 clams_python-1.2.1/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    21677 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.205550 clams_python-1.2.1/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.205550 clams_python-1.2.1/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/.dockerignore.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/Containerfile.template
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/LICENSE.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/metadata.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/app/requirements.txt.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/gha/for-clams-team.md.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/gha/workflows/issue-assign.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/gha/workflows/issue-close.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/develop/templates/gha/workflows/publish.yml.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/mmif_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/mmif_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/mmif_utils/rewind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/mmif_utils/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-21 22:12:50.000000 clams_python-1.2.1/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 22:13:16.000000 clams_python-1.2.1/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-21 22:12:50.000000 clams_python-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:13:16.213550 clams_python-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-21 22:12:50.000000 clams_python-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:13:16.209550 clams_python-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23502 2024-04-21 22:12:50.000000 clams_python-1.2.1/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-21 22:12:50.000000 clams_python-1.2.1/tests/test_clamscli.py
```

### Comparing `clams-python-1.2.0/LICENSE` & `clams_python-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/PKG-INFO` & `clams_python-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.2.0
+Version: 1.2.1
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.2.0/README.md` & `clams_python-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/__init__.py` & `clams_python-1.2.1/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/app/__init__.py` & `clams_python-1.2.1/clams/app/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,17 @@
         if not isinstance(mmif, Mmif):
             mmif = Mmif(mmif)
         issued_warnings = []
         for key in runtime_params:
             if key not in self.annotate_param_spec:
                 issued_warnings.append(UserWarning(f'An undefined parameter "{key}" (value: "{runtime_params[key]}") is passed'))
         # this will do casting + refinement altogether
+        self.logger.debug(f"User parameters: {runtime_params}")
         refined = self._refine_params(**runtime_params)
+        self.logger.debug(f"Refined parameters: {refined}")
         pretty = refined.get('pretty', False)
         with warnings.catch_warnings(record=True) as ws:
             annotated = self._annotate(mmif, **refined)
             if ws:
                 issued_warnings.extend(ws)
         if issued_warnings:
             warnings_view = annotated.new_view()
@@ -198,28 +200,29 @@
         passed to this method. This means all parameters for "common" configuration that
         are consumed in :meth:`~clams.app.ClamsApp.annotate` should not be recorded in the
         view metadata.
         :param view: a view to sign
         :param runtime_conf: runtime configuration of the app as k-v pairs
         """
         view.metadata.app = self.metadata.identifier
+        params_map = {p.name: p for p in self.metadata.parameters}
         if self._RAW_PARAMS_KEY in runtime_conf:
             for k, v in runtime_conf.items():
                 if k == self._RAW_PARAMS_KEY:
                     for orik, oriv in v.items():
-                        if orik in self.metadata.parameters and self.metadata.parameters[orik].multivalued:
+                        if orik in params_map and params_map[orik].multivalued:
                             view.metadata.add_parameter(orik, str(oriv))
                         else:
                             view.metadata.add_parameter(orik, oriv[0])
                 else:
                     view.metadata.add_app_configuration(k, v)
         else:
             # meaning the parameters directly from flask or argparser and values are in lists
             for k, v in runtime_conf.items():
-                if k in self.metadata.parameters and self.metadata.parameters[k].multivalued:
+                if k in params_map and params_map[k].multivalued:
                     view.metadata.add_parameter(k, str(v))
                 else:
                     view.metadata.add_parameter(k, v[0])
         
     def set_error_view(self, mmif: Union[str, dict, Mmif], **runtime_conf: List[str]) -> Mmif:
         """
         A method to record an error instead of annotation results in the view
```

### Comparing `clams-python-1.2.0/clams/appmetadata/__init__.py` & `clams_python-1.2.1/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/develop/__init__.py` & `clams_python-1.2.1/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/develop/templates/app/.gitignore.template` & `clams_python-1.2.1/clams/develop/templates/app/.gitignore.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/develop/templates/app/Containerfile.template` & `clams_python-1.2.1/clams/develop/templates/app/Containerfile.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/develop/templates/app/README.md.template` & `clams_python-1.2.1/clams/develop/templates/app/README.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/develop/templates/app/app.py.template` & `clams_python-1.2.1/clams/develop/templates/app/app.py.template`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 - provide a way to run the code as a RESTful Flask service 
 
 
 """
 
 import argparse
 import logging
-from typing import Union
 
 # Imports needed for Clams and MMIF.
 # Non-NLP Clams applications will require AnnotationTypes
 
 from clams import ClamsApp, Restifier
 from mmif import Mmif, View, Annotation, Document, AnnotationTypes, DocumentTypes
 
@@ -32,15 +31,15 @@
 
     def _appmetadata(self):
         # see https://sdk.clams.ai/autodoc/clams.app.html#clams.app.ClamsApp._load_appmetadata
         # Also check out ``metadata.py`` in this directory. 
         # When using the ``metadata.py`` leave this do-nothing "pass" method here. 
         pass
 
-    def _annotate(self, mmif: Union[str, dict, Mmif], **parameters) -> Mmif:
+    def _annotate(self, mmif: Mmif, **parameters) -> Mmif:
         # see https://sdk.clams.ai/autodoc/clams.app.html#clams.app.ClamsApp._annotate
         raise NotImplementedError
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--port", action="store", default="5000", help="set port to listen")
```

### Comparing `clams-python-1.2.0/clams/develop/templates/app/metadata.py.template` & `clams_python-1.2.1/clams/develop/templates/app/metadata.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/develop/templates/gha/for-clams-team.md.template` & `clams_python-1.2.1/clams/develop/templates/gha/for-clams-team.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/develop/templates/gha/workflows/publish.yml.template` & `clams_python-1.2.1/clams/develop/templates/gha/workflows/publish.yml.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/mmif_utils/rewind.py` & `clams_python-1.2.1/clams/mmif_utils/rewind.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/mmif_utils/source.py` & `clams_python-1.2.1/clams/mmif_utils/source.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams/restify/__init__.py` & `clams_python-1.2.1/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/clams_python.egg-info/PKG-INFO` & `clams_python-1.2.1/clams_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.2.0
+Version: 1.2.1
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.2.0/clams_python.egg-info/SOURCES.txt` & `clams_python-1.2.1/clams_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/setup.py` & `clams_python-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/tests/test_clamsapp.py` & `clams_python-1.2.1/tests/test_clamsapp.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.2.0/tests/test_clamscli.py` & `clams_python-1.2.1/tests/test_clamscli.py`

 * *Files identical despite different names*

