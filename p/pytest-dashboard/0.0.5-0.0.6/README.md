# Comparing `tmp/pytest_dashboard-0.0.5.tar.gz` & `tmp/pytest_dashboard-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_dashboard-0.0.5.tar", max compression
+gzip compressed data, was "pytest_dashboard-0.0.6.tar", max compression
```

## Comparing `pytest_dashboard-0.0.5.tar` & `pytest_dashboard-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1495 2024-04-18 13:00:54.063779 pytest_dashboard-0.0.5/LICENSE
--rw-r--r--   0        0        0      643 2024-04-18 13:00:54.063779 pytest_dashboard-0.0.5/README.md
--rw-r--r--   0        0        0      776 2024-04-18 13:01:22.043916 pytest_dashboard-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-18 13:01:22.043916 pytest_dashboard-0.0.5/pytest_dashboard/__init__.py
--rw-r--r--   0        0        0     2997 2024-04-18 13:00:54.063779 pytest_dashboard-0.0.5/pytest_dashboard/_tolly_progresses.py
--rw-r--r--   0        0        0     2184 2024-04-18 13:00:54.063779 pytest_dashboard-0.0.5/pytest_dashboard/conftest.py
--rw-r--r--   0        0        0      136 2024-04-18 13:00:54.063779 pytest_dashboard-0.0.5/pytest_dashboard/tolly.py
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 pytest_dashboard-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1495 2024-04-22 06:56:40.263174 pytest_dashboard-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1248 2024-04-22 06:56:40.263174 pytest_dashboard-0.0.6/README.md
+-rw-r--r--   0        0        0      776 2024-04-22 06:56:56.895243 pytest_dashboard-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-22 06:56:56.895243 pytest_dashboard-0.0.6/pytest_dashboard/__init__.py
+-rw-r--r--   0        0        0     3434 2024-04-22 06:56:40.267174 pytest_dashboard-0.0.6/pytest_dashboard/_tolly_progresses.py
+-rw-r--r--   0        0        0     2184 2024-04-22 06:56:40.267174 pytest_dashboard-0.0.6/pytest_dashboard/conftest.py
+-rw-r--r--   0        0        0      136 2024-04-22 06:56:40.267174 pytest_dashboard-0.0.6/pytest_dashboard/tolly.py
+-rw-r--r--   0        0        0     2101 1970-01-01 00:00:00.000000 pytest_dashboard-0.0.6/PKG-INFO
```

### Comparing `pytest_dashboard-0.0.5/LICENSE` & `pytest_dashboard-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_dashboard-0.0.5/pyproject.toml` & `pytest_dashboard-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-dashboard"
-version = "0.0.5"  # ignored by versioning plugin
+version = "0.0.6"  # ignored by versioning plugin
 description = ""
 authors = ["kazuma.naito <kazuma.naito@murata.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/pyfemtet/pytest-dashboard"
 
 [tool.poetry.dependencies]
```

### Comparing `pytest_dashboard-0.0.5/pytest_dashboard/_tolly_progresses.py` & `pytest_dashboard-0.0.6/pytest_dashboard/_tolly_progresses.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 )
 
 UPDATE_INTERVAL = 1
 
 should_stop = False
 
 
-def _progress_passed(data):
+def _progress_passed(data) -> bool:
     # if empty, return False
     if data is None:
         return False
 
     # if all(results), return True
     passed_list = []
     for result in data['results']:
@@ -39,40 +39,52 @@
             passed = passed * (call == 'passed')
         if teardown is not None:
             passed = passed * (teardown == 'passed')
         passed_list.append(passed)
     return all(passed_list)
 
 
-def _progress_state(data):
+def _progress_state(data) -> str:
     # if empty, not started
     if data is None:
         return 'not started'
 
-    # if len(items) > len(results), in progress
-    if len(data['items']) > len(data['results']):
-        return 'in progress'
-
-    # if len(items) == len(results), finished
-    if len(data['items']) == len(data['results']):
+    # if len(items) == len(results) and data['results'][-1] has the key 'teardown', finished
+    if (
+            len(data['items']) == len(data['results'])
+            and 'teardown' in data['results'][-1].keys()
+    ):
         return 'finished'
 
-    return 'undefined'
+    # else, ongoing
+    return 'ongoing'
 
 
 def merge_progress_files(progresses_dir, entire_progress_path):
-    # glob all .yaml and check their state and passed
+    # glob all -progress.yaml and check their state and passed
     merged_data = {}
-    for path in glob(os.path.join(progresses_dir, '*progress.yaml')):
+    state_list = []
+    passed_list = []
+    for path in glob(os.path.join(progresses_dir, '*-progress.yaml')):
         with open(path, 'r') as f:
             data = yaml.safe_load(f)
+            # add each progress
             name = os.path.basename(path)[:-14]  # -progress.yaml is 14 chars
             state = _progress_state(data)
             passed = _progress_passed(data)
             merged_data[name] = dict(state=state, passed=passed)
+            # add to entire list
+            state_list.append(state)
+            passed_list.append(passed)
+
+    # add entire progress
+    name = 'entire'
+    state = 'finished' if all([s=='finished' for s in state_list]) else 'ongoing'
+    passed = all(passed_list)
+    merged_data[name] = dict(state=state, passed=passed)
 
     # save merged entire-progress.yaml
     with open(entire_progress_path, 'w') as f:
         yaml.dump(merged_data, f)
 
 
 def _update_forever(progresses_dir, entire_progress_path):
```

### Comparing `pytest_dashboard-0.0.5/pytest_dashboard/conftest.py` & `pytest_dashboard-0.0.6/pytest_dashboard/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_dashboard-0.0.5/PKG-INFO` & `pytest_dashboard-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dashboard
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Home-page: https://github.com/pyfemtet/pytest-dashboard
 License: BSD-3-Clause
 Author: kazuma.naito
 Author-email: kazuma.naito@murata.com
 Requires-Python: >=3.9.3,<3.13
 Classifier: License :: OSI Approved :: BSD License
@@ -23,16 +23,31 @@
 
 # pytest-dashboard
 
 ## usage
 `python -m pytest`
 by this command, you get `[datetime]-progress.yaml` file on working directory as realtime pytest progress report.
 
-`python -m pytest --progress-path=[path/to/progress.yaml]`
-by this command, you get `path/to/progress.yaml` file.
+`python -m pytest --progress-path=[path/to/some-progress.yaml]`
+by this command, you get `path/to/some-progress.yaml` file.
+
+`python -m pytest-dashboard.tolly PROGRESSES_DIR --entire_progress_path=[path/to/entire-progress.yaml]`
+by this command, you get started to monitor changes of
+the progress files (ends with `-progress.yaml`)
+inside `PROGRESS_DIR` and save the state summary
+to `path/to/entire-progress.yaml`.
+
+So it is recommended to set `--progress-path` option of pytest
+ending with `-progress.yaml`.
+For example, `2024-04-22-progress.yaml`,
+
+> **Note**
+> if your `entire_progress_path` is ends with `-progress.yaml`,
+> you cannot save the entire progress file to
+> the same directory with each progress file.
 
 `python -m pytest_dashboard.tolly --progress-dir=[dir/contains/progress.yaml_files]`
 by this command, you monitor -progress.yaml files
 inside `dir/contains/progress.yaml_files`
 and continurous update to tolly them
 to `--entire-progress-path` (optional, default to `entire-progress.yaml`) file.
```

