# Comparing `tmp/sekoia_automation_sdk-1.8.2.tar.gz` & `tmp/sekoia_automation_sdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sekoia_automation_sdk-1.8.2.tar", max compression
+gzip compressed data, was "sekoia_automation_sdk-1.9.0.tar", max compression
```

## Comparing `sekoia_automation_sdk-1.8.2.tar` & `sekoia_automation_sdk-1.9.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0     1066 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/LICENSE
--rw-r--r--   0        0        0     8422 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/README.md
--rw-r--r--   0        0        0     3335 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/__init__.py
--rw-r--r--   0        0        0    11254 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/action.py
--rw-r--r--   0        0        0       73 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/__init__.py
--rw-r--r--   0        0        0     4629 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/connector.py
--rw-r--r--   0        0        0      136 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/__init__.py
--rw-r--r--   0        0        0      169 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/aws/__init__.py
--rw-r--r--   0        0        0     3255 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/aws/client.py
--rw-r--r--   0        0        0      215 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/files/__init__.py
--rw-r--r--   0        0        0      678 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/files/csv.py
--rw-r--r--   0        0        0      240 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/files/utils.py
--rw-r--r--   0        0        0      219 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/http/__init__.py
--rw-r--r--   0        0        0     2658 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/http/http_client.py
--rw-r--r--   0        0        0     3920 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/http/token_refresher.py
--rw-r--r--   0        0        0      686 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/http/utils.py
--rw-r--r--   0        0        0     5547 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/cli.py
--rw-r--r--   0        0        0      737 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/config.py
--rw-r--r--   0        0        0     9366 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/connector/__init__.py
--rw-r--r--   0        0        0     2313 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/connector/workers.py
--rw-r--r--   0        0        0      426 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/constants.py
--rw-r--r--   0        0        0      869 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/exceptions.py
--rw-r--r--   0        0        0       67 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/loguru/__init__.py
--rw-r--r--   0        0        0     2449 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/loguru/config.py
--rw-r--r--   0        0        0     1101 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/loguru/formatters.py
--rw-r--r--   0        0        0     1120 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/loguru/handlers.py
--rw-r--r--   0        0        0      399 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/metrics/__init__.py
--rw-r--r--   0        0        0      383 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/metrics/base.py
--rw-r--r--   0        0        0     1185 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/metrics/prometheus.py
--rw-r--r--   0        0        0    17526 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/module.py
--rw-r--r--   0        0        0        0 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/__init__.py
--rw-r--r--   0        0        0     6605 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/documentation/generate.py
--rw-r--r--   0        0        0     2669 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/documentation/templates/module.md
--rw-r--r--   0        0        0     8919 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/files_generator.py
--rw-r--r--   0        0        0      144 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/new_module/template/cookiecutter.json
--rw-r--r--   0        0        0       23 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/new_module/template/hooks/post_gen_project.sh
--rw-r--r--   0        0        0      301 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
--rw-r--r--   0        0        0      255 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
--rw-r--r--   0        0        0      417 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
--rw-r--r--   0        0        0      596 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
--rw-r--r--   0        0        0      358 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
--rw-r--r--   0        0        0      368 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
--rw-r--r--   0        0        0      140 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
--rw-r--r--   0        0        0    10011 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/openapi.py
--rwxr-xr-x   0        0        0    14717 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/sync_library.py
--rw-r--r--   0        0        0     2089 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/update_sdk_version.py
--rw-r--r--   0        0        0     7063 2023-11-28 10:42:05.443903 sekoia_automation_sdk-1.8.2/sekoia_automation/storage.py
--rw-r--r--   0        0        0    16659 2023-11-28 10:42:05.447903 sekoia_automation_sdk-1.8.2/sekoia_automation/trigger.py
--rw-r--r--   0        0        0     1294 2023-11-28 10:42:05.447903 sekoia_automation_sdk-1.8.2/sekoia_automation/utils.py
--rw-r--r--   0        0        0    10387 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-12-01 14:00:12.192987 sekoia_automation_sdk-1.9.0/LICENSE
+-rw-r--r--   0        0        0     8422 2023-12-01 14:00:12.192987 sekoia_automation_sdk-1.9.0/README.md
+-rw-r--r--   0        0        0     3335 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/__init__.py
+-rw-r--r--   0        0        0    11254 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/action.py
+-rw-r--r--   0        0        0       73 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/__init__.py
+-rw-r--r--   0        0        0     4628 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/connector.py
+-rw-r--r--   0        0        0      136 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/__init__.py
+-rw-r--r--   0        0        0      169 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/aws/__init__.py
+-rw-r--r--   0        0        0     3255 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/aws/client.py
+-rw-r--r--   0        0        0      215 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/files/__init__.py
+-rw-r--r--   0        0        0      678 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/files/csv.py
+-rw-r--r--   0        0        0      240 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/files/utils.py
+-rw-r--r--   0        0        0      219 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/http/__init__.py
+-rw-r--r--   0        0        0     2658 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/http/http_client.py
+-rw-r--r--   0        0        0     3920 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/http/token_refresher.py
+-rw-r--r--   0        0        0      686 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/http/utils.py
+-rw-r--r--   0        0        0     5547 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/cli.py
+-rw-r--r--   0        0        0      737 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/config.py
+-rw-r--r--   0        0        0     9366 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/connector/__init__.py
+-rw-r--r--   0        0        0     2313 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/connector/workers.py
+-rw-r--r--   0        0        0      426 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/constants.py
+-rw-r--r--   0        0        0      869 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/exceptions.py
+-rw-r--r--   0        0        0       67 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/loguru/__init__.py
+-rw-r--r--   0        0        0     2449 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/loguru/config.py
+-rw-r--r--   0        0        0     1101 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/loguru/formatters.py
+-rw-r--r--   0        0        0     1120 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/loguru/handlers.py
+-rw-r--r--   0        0        0      399 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/metrics/__init__.py
+-rw-r--r--   0        0        0      383 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/metrics/base.py
+-rw-r--r--   0        0        0     1185 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/metrics/prometheus.py
+-rw-r--r--   0        0        0    17526 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/module.py
+-rw-r--r--   0        0        0        0 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/__init__.py
+-rw-r--r--   0        0        0     6605 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/documentation/generate.py
+-rw-r--r--   0        0        0     2669 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/documentation/templates/module.md
+-rw-r--r--   0        0        0     8919 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/files_generator.py
+-rw-r--r--   0        0        0      144 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/new_module/template/cookiecutter.json
+-rw-r--r--   0        0        0       23 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/new_module/template/hooks/post_gen_project.sh
+-rw-r--r--   0        0        0      301 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
+-rw-r--r--   0        0        0      255 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
+-rw-r--r--   0        0        0      417 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
+-rw-r--r--   0        0        0      596 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
+-rw-r--r--   0        0        0      358 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
+-rw-r--r--   0        0        0      368 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
+-rw-r--r--   0        0        0      140 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
+-rw-r--r--   0        0        0    10011 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/openapi.py
+-rwxr-xr-x   0        0        0    14717 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/sync_library.py
+-rw-r--r--   0        0        0     2089 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/update_sdk_version.py
+-rw-r--r--   0        0        0     7063 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/storage.py
+-rw-r--r--   0        0        0      770 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/timer.py
+-rw-r--r--   0        0        0    16872 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/trigger.py
+-rw-r--r--   0        0        0     1294 2023-12-01 14:00:12.196987 sekoia_automation_sdk-1.9.0/sekoia_automation/utils.py
+-rw-r--r--   0        0        0    10387 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.9.0/PKG-INFO
```

### Comparing `sekoia_automation_sdk-1.8.2/LICENSE` & `sekoia_automation_sdk-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/README.md` & `sekoia_automation_sdk-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/pyproject.toml` & `sekoia_automation_sdk-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sekoia-automation-sdk"
 
-version = "1.8.2"
+version = "1.9.0"
 description = "SDK to create Sekoia.io playbook modules"
 license = "MIT"
 readme = "README.md"
 authors = ["Sekoia.io"]
 packages = [
     { include = "sekoia_automation" },
 ]
```

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/action.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/action.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/aio/connector.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/aio/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         Args:
             events: list[str]
 
         Returns:
             list[str]:
         """
         self._last_events_time = datetime.utcnow()
-        batch_api = urljoin(self.configuration.intake_server, "/batch")
+        batch_api = urljoin(self.configuration.intake_server, "batch")
 
         self.log(f"Push {len(events)} events to intakes")
 
         result_ids = []
 
         chunks = self._chunk_events(events)
```

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/aws/client.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/aws/client.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/files/csv.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/files/csv.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/http/http_client.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/http/http_client.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/http/token_refresher.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/http/token_refresher.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/aio/helpers/http/utils.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/aio/helpers/http/utils.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/cli.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/cli.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/config.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/config.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/connector/__init__.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/connector/workers.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/connector/workers.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/exceptions.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/exceptions.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/loguru/config.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/loguru/config.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/loguru/formatters.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/loguru/formatters.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/loguru/handlers.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/loguru/handlers.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/metrics/prometheus.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/module.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/module.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/documentation/generate.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/documentation/generate.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/documentation/templates/module.md` & `sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/documentation/templates/module.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/files_generator.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/files_generator.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml` & `sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/openapi.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/openapi.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/sync_library.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/sync_library.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/scripts/update_sdk_version.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/scripts/update_sdk_version.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/storage.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/storage.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/trigger.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/trigger.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     InvalidDirectoryError,
     ModuleConfigurationError,
     SendEventError,
     TriggerConfigurationError,
 )
 from sekoia_automation.metrics import PrometheusExporterThread, make_exporter
 from sekoia_automation.module import Module, ModuleItem
+from sekoia_automation.timer import RepeatedTimer
 from sekoia_automation.utils import (
     capture_retry_error,
     get_annotation_for,
     get_as_model,
     validate_with_model,
 )
 
@@ -41,15 +42,15 @@
     # the trigger is considered in error.
     # 0 means that the trigger is never considered in error
     seconds_without_events = 0
     LIVENESS_PORT_FILE_NAME = "liveness_port"
     METRICS_PORT_FILE_NAME = "metrics_port"
 
     LOGS_MAX_BATCH_SIZE = 50
-    LOGS_MAX_DELTA = timedelta(seconds=5)
+    LOGS_MAX_DELTA = 5  # seconds
 
     # Time to wait for stop event to be received
     _STOP_EVENT_WAIT = 120
 
     def __init__(self, module: Module | None = None, data_path: Path | None = None):
         super().__init__(module, data_path)
         self._configuration: dict | BaseModel | None = None
@@ -57,15 +58,16 @@
         self._last_events_time = datetime.utcnow()
         self._startup_time = datetime.utcnow()
         sentry_sdk.set_tag("item_type", "trigger")
         self._secrets: dict[str, Any] = {}
         self._stop_event = Event()
         self._critical_log_sent = False
         self._logs: list[dict] = []
-        self._first_log_time: datetime | None = None
+
+        self._logs_timer = RepeatedTimer(self.LOGS_MAX_DELTA, self._send_logs_to_api)
 
         # Register signal to terminate thread
         signal.signal(signal.SIGINT, self.stop)
         signal.signal(signal.SIGTERM, self.stop)
 
         self._liveness_server = None
         self._exporter = None
@@ -100,14 +102,15 @@
         return secrets
 
     def stop(self, *args, **kwargs) -> None:  # noqa: ARG002
         """
         Engage the trigger exit
         """
         self._stop_event.set()
+        self._logs_timer.stop()
 
     @property
     def running(self) -> bool:
         """
         Return if the trigger is still active or not
         """
         return not self._stop_event.is_set()
@@ -164,14 +167,15 @@
             self._stop_event.wait(self._STOP_EVENT_WAIT)
 
     def execute(self) -> None:
         self._ensure_data_path_set()
         # Always restart the trigger, except if the error seems to be unrecoverable
         self._secrets = self._get_secrets_from_server()
         self.module.set_secrets(self._secrets)
+        self._logs_timer.start()
         try:
             while not self._stop_event.is_set():
                 try:
                     self._execute_once()
                 except Exception:  # pragma: no cover
                     # Exception are handled in `_execute_once` but in case
                     # an error occurred while handling an error we catch everything
@@ -303,21 +307,17 @@
         self._logs.append(
             {
                 "date": datetime.utcnow().isoformat(),
                 "level": level,
                 "message": message,
             }
         )
-        if self._first_log_time is None:
-            self._first_log_time = datetime.utcnow()
-
         if (
             level in ["error", "critical"]  # Don't wait for error or critical logs
             or len(self._logs) >= self.LOGS_MAX_BATCH_SIZE  # batch is full
-            or datetime.utcnow() - self._first_log_time >= self.LOGS_MAX_DELTA
         ):
             self._send_logs_to_api()
 
         if level == "critical":
             self._critical_log_sent = True
 
     @retry(
@@ -325,21 +325,27 @@
         wait=wait_exponential(max=10),
         stop=stop_after_attempt(10),
         retry_error_callback=capture_retry_error,
     )
     def _send_logs_to_api(self):
         if not self._logs:
             return
-        data = {"logs": self._logs}
-        response = requests.request(
-            "POST", self.logs_url, json=data, headers=self._headers, timeout=30
-        )
-        response.raise_for_status()
+        # Clear self._logs, so we won't lose logs that are added while sending
+        logs = self._logs
         self._logs = []
-        self._first_log_time = None
+        try:
+            data = {"logs": logs}
+            response = requests.request(
+                "POST", self.logs_url, json=data, headers=self._headers, timeout=30
+            )
+            response.raise_for_status()
+        except Exception:
+            # If the request failed, we add the logs back to the list
+            self._logs.extend(logs)
+            raise
 
     @abstractmethod
     def run(self) -> None:
         """
         Method that each trigger should implement to contain its logic.
 
         Should usually be an infinite loop, calling send_event when relevant.
```

### Comparing `sekoia_automation_sdk-1.8.2/sekoia_automation/utils.py` & `sekoia_automation_sdk-1.9.0/sekoia_automation/utils.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.8.2/PKG-INFO` & `sekoia_automation_sdk-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekoia-automation-sdk
-Version: 1.8.2
+Version: 1.9.0
 Summary: SDK to create Sekoia.io playbook modules
 Home-page: https://sekoia.io/
 License: MIT
 Keywords: SDK,Sekoia.io,automation,playbook
 Author: Sekoia.io
 Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Developers
```

