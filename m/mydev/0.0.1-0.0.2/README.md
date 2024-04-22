# Comparing `tmp/mydev-0.0.1.tar.gz` & `tmp/mydev-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mydev-0.0.1.tar", last modified: Sun Apr 21 03:03:45 2024, max compression
+gzip compressed data, was "mydev-0.0.2.tar", last modified: Mon Apr 22 02:48:56 2024, max compression
```

## Comparing `mydev-0.0.1.tar` & `mydev-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0       37 2024-04-01 05:59:54.867140 mydev-0.0.1/README.md
--rw-r--r--   0        0        0      638 2024-04-21 03:03:45.046593 mydev-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-01 05:58:23.447148 mydev-0.0.1/src/mydev/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 06:10:47.357080 mydev-0.0.1/src/mydev/agent/__init__.py
--rw-r--r--   0        0        0      195 2024-04-04 05:21:26.779115 mydev-0.0.1/src/mydev/agent/main.py
--rw-r--r--   0        0        0     1549 2024-04-13 22:21:46.190471 mydev-0.0.1/src/mydev/agent/models.py
--rw-r--r--   0        0        0        0 2024-04-01 06:14:15.067062 mydev-0.0.1/src/mydev/cli/__init__.py
--rw-r--r--   0        0        0     5274 2024-04-14 02:45:56.652870 mydev-0.0.1/src/mydev/cli/agent.py
--rw-r--r--   0        0        0     2561 2024-04-04 04:59:15.409367 mydev-0.0.1/src/mydev/cli/db.py
--rw-r--r--   0        0        0      225 2024-04-20 23:21:19.227374 mydev-0.0.1/src/mydev/cli/infra.py
--rw-r--r--   0        0        0     1316 2024-04-20 23:21:19.237374 mydev-0.0.1/src/mydev/cli/main.py
--rw-r--r--   0        0        0     1706 2024-04-04 02:56:40.240744 mydev-0.0.1/src/mydev/cli/pm.py
--rw-r--r--   0        0        0      649 2024-04-04 05:00:16.079357 mydev-0.0.1/src/mydev/config.py
--rw-r--r--   0        0        0       57 2024-04-01 08:28:53.516319 mydev-0.0.1/src/mydev/console.py
--rw-r--r--   0        0        0     1037 2024-04-20 23:15:08.677463 mydev-0.0.1/src/mydev/db.py
--rw-r--r--   0        0        0        0 2024-04-20 23:20:20.427388 mydev-0.0.1/src/mydev/infra/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 23:21:56.647370 mydev-0.0.1/src/mydev/infra/shell.py
--rw-r--r--   0        0        0        0 2024-04-04 05:27:40.109048 mydev-0.0.1/src/mydev/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 10:21:43.805702 mydev-0.0.1/src/mydev/pm/__init__.py
--rw-r--r--   0        0        0     4225 2024-04-04 03:37:20.590287 mydev-0.0.1/src/mydev/pm/manager.py
--rw-r--r--   0        0        0      409 2024-04-04 00:04:05.392684 mydev-0.0.1/src/mydev/pm/models.py
--rw-r--r--   0        0        0        0 2024-04-01 10:23:20.505693 mydev-0.0.1/src/mydev/utils/__init__.py
--rw-r--r--   0        0        0      465 2024-04-04 04:15:32.419857 mydev-0.0.1/src/mydev/utils/constants.py
--rw-r--r--   0        0        0      259 2024-04-04 02:47:27.670851 mydev-0.0.1/src/mydev/utils/monitoring.py
--rw-r--r--   0        0        0      231 2024-04-01 10:37:03.965616 mydev-0.0.1/src/mydev/utils/secrets.py
--rw-r--r--   0        0        0    11479 2024-04-14 02:30:57.983237 mydev-0.0.1/src/mydev/utils/ssh.py
--rw-r--r--   0        0        0        0 2024-04-01 05:58:23.447148 mydev-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3367 2024-04-04 01:30:54.611708 mydev-0.0.1/tests/test_pm.py
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 mydev-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-04-01 05:59:54.867140 mydev-0.0.2/README.md
+-rw-r--r--   0        0        0      638 2024-04-22 02:48:56.526811 mydev-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-01 05:58:23.447148 mydev-0.0.2/src/mydev/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 06:10:47.357080 mydev-0.0.2/src/mydev/agent/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-21 03:38:50.149541 mydev-0.0.2/src/mydev/agent/main.py
+-rw-r--r--   0        0        0     1549 2024-04-13 22:21:46.190471 mydev-0.0.2/src/mydev/agent/models.py
+-rw-r--r--   0        0        0     1893 2024-04-21 03:45:59.962847 mydev-0.0.2/src/mydev/assets/install.sh
+-rw-r--r--   0        0        0        0 2024-04-01 06:14:15.067062 mydev-0.0.2/src/mydev/cli/__init__.py
+-rw-r--r--   0        0        0     5274 2024-04-14 02:45:56.652870 mydev-0.0.2/src/mydev/cli/agent.py
+-rw-r--r--   0        0        0     2561 2024-04-04 04:59:15.409367 mydev-0.0.2/src/mydev/cli/db.py
+-rw-r--r--   0        0        0      225 2024-04-20 23:21:19.227374 mydev-0.0.2/src/mydev/cli/infra.py
+-rw-r--r--   0        0        0     1316 2024-04-20 23:21:19.237374 mydev-0.0.2/src/mydev/cli/main.py
+-rw-r--r--   0        0        0     1706 2024-04-04 02:56:40.240744 mydev-0.0.2/src/mydev/cli/pm.py
+-rw-r--r--   0        0        0      649 2024-04-04 05:00:16.079357 mydev-0.0.2/src/mydev/config.py
+-rw-r--r--   0        0        0       57 2024-04-01 08:28:53.516319 mydev-0.0.2/src/mydev/console.py
+-rw-r--r--   0        0        0     1037 2024-04-20 23:15:08.677463 mydev-0.0.2/src/mydev/db.py
+-rw-r--r--   0        0        0        0 2024-04-20 23:20:20.427388 mydev-0.0.2/src/mydev/infra/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 23:21:56.647370 mydev-0.0.2/src/mydev/infra/shell.py
+-rw-r--r--   0        0        0        0 2024-04-04 05:27:40.109048 mydev-0.0.2/src/mydev/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 10:21:43.805702 mydev-0.0.2/src/mydev/pm/__init__.py
+-rw-r--r--   0        0        0     4225 2024-04-04 03:37:20.590287 mydev-0.0.2/src/mydev/pm/manager.py
+-rw-r--r--   0        0        0      409 2024-04-04 00:04:05.392684 mydev-0.0.2/src/mydev/pm/models.py
+-rw-r--r--   0        0        0        0 2024-04-01 10:23:20.505693 mydev-0.0.2/src/mydev/utils/__init__.py
+-rw-r--r--   0        0        0      523 2024-04-21 03:32:50.912624 mydev-0.0.2/src/mydev/utils/constants.py
+-rw-r--r--   0        0        0      259 2024-04-04 02:47:27.670851 mydev-0.0.2/src/mydev/utils/monitoring.py
+-rw-r--r--   0        0        0      231 2024-04-01 10:37:03.965616 mydev-0.0.2/src/mydev/utils/secrets.py
+-rw-r--r--   0        0        0    11479 2024-04-14 02:30:57.983237 mydev-0.0.2/src/mydev/utils/ssh.py
+-rw-r--r--   0        0        0        0 2024-04-01 05:58:23.447148 mydev-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3367 2024-04-04 01:30:54.611708 mydev-0.0.2/tests/test_pm.py
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 mydev-0.0.2/PKG-INFO
```

### Comparing `mydev-0.0.1/pyproject.toml` & `mydev-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mydev"
-version = "0.0.1"
+version = "0.0.2"
 description = "Personal dev tools"
 authors = [
     { name = "Jianglong Ye", email = "jianglong.yeh@gmail.com" },
 ]
 dependencies = [
     "fastapi>=0.110.0",
     "typer>=0.12.0",
```

### Comparing `mydev-0.0.1/src/mydev/agent/models.py` & `mydev-0.0.2/src/mydev/agent/models.py`

 * *Files identical despite different names*

### Comparing `mydev-0.0.1/src/mydev/cli/agent.py` & `mydev-0.0.2/src/mydev/cli/agent.py`

 * *Files identical despite different names*

### Comparing `mydev-0.0.1/src/mydev/cli/db.py` & `mydev-0.0.2/src/mydev/cli/db.py`

 * *Files identical despite different names*

### Comparing `mydev-0.0.1/src/mydev/cli/main.py` & `mydev-0.0.2/src/mydev/cli/main.py`

 * *Files identical despite different names*

### Comparing `mydev-0.0.1/src/mydev/cli/pm.py` & `mydev-0.0.2/src/mydev/cli/pm.py`

 * *Files identical despite different names*

### Comparing `mydev-0.0.1/src/mydev/config.py` & `mydev-0.0.2/src/mydev/config.py`

 * *Files identical despite different names*

### Comparing `mydev-0.0.1/src/mydev/db.py` & `mydev-0.0.2/src/mydev/db.py`

 * *Files identical despite different names*

### Comparing `mydev-0.0.1/src/mydev/pm/manager.py` & `mydev-0.0.2/src/mydev/pm/manager.py`

 * *Files identical despite different names*

### Comparing `mydev-0.0.1/src/mydev/utils/ssh.py` & `mydev-0.0.2/src/mydev/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `mydev-0.0.1/tests/test_pm.py` & `mydev-0.0.2/tests/test_pm.py`

 * *Files identical despite different names*

### Comparing `mydev-0.0.1/PKG-INFO` & `mydev-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mydev
-Version: 0.0.1
+Version: 0.0.2
 Summary: Personal dev tools
 Author-Email: Jianglong Ye <jianglong.yeh@gmail.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: fastapi>=0.110.0
 Requires-Dist: typer>=0.12.0
 Requires-Dist: uvicorn>=0.29.0
```

