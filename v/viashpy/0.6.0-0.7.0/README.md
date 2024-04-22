# Comparing `tmp/viashpy-0.6.0.tar.gz` & `tmp/viashpy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viashpy-0.6.0.tar", last modified: Mon Jan 22 14:49:34 2024, max compression
+gzip compressed data, was "viashpy-0.7.0.tar", last modified: Mon Apr 22 08:38:51 2024, max compression
```

## Comparing `viashpy-0.6.0.tar` & `viashpy-0.7.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-01-22 14:49:34.606186 viashpy-0.6.0/
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-01-22 14:49:34.606186 viashpy-0.6.0/.github/
--rw-rw-r--   0 di        (1002) di        (1002)      202 2022-12-02 22:58:53.000000 viashpy-0.6.0/.github/dependabot.yml
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-01-22 14:49:34.606186 viashpy-0.6.0/.github/workflows/
--rw-rw-r--   0 di        (1002) di        (1002)     1367 2024-01-22 14:42:51.000000 viashpy-0.6.0/.github/workflows/ci.yml
--rw-rw-r--   0 di        (1002) di        (1002)      623 2024-01-19 08:59:14.000000 viashpy-0.6.0/.gitignore
--rw-rw-r--   0 di        (1002) di        (1002)     4026 2024-01-22 14:43:21.000000 viashpy-0.6.0/CHANGELOG.rst
--rw-rw-r--   0 di        (1002) di        (1002)    32217 2022-12-02 22:58:53.000000 viashpy-0.6.0/LICENSE
--rw-rw-r--   0 di        (1002) di        (1002)      125 2022-12-02 22:58:53.000000 viashpy-0.6.0/MANIFEST.in
--rw-r--r--   0 di        (1002) di        (1002)     2808 2024-01-22 14:49:34.606186 viashpy-0.6.0/PKG-INFO
--rw-rw-r--   0 di        (1002) di        (1002)     1683 2022-12-02 22:58:53.000000 viashpy-0.6.0/README.md
--rw-rw-r--   0 di        (1002) di        (1002)       20 2024-01-22 14:42:51.000000 viashpy-0.6.0/_viash.yaml
--rw-rw-r--   0 di        (1002) di        (1002)      508 2024-01-22 14:42:51.000000 viashpy-0.6.0/pyproject.toml
--rw-rw-r--   0 di        (1002) di        (1002)     1350 2024-01-22 14:49:34.606186 viashpy-0.6.0/setup.cfg
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-01-22 14:49:34.606186 viashpy-0.6.0/tests/
--rw-rw-r--   0 di        (1002) di        (1002)      812 2024-01-22 14:42:51.000000 viashpy-0.6.0/tests/conftest.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-01-22 14:49:34.606186 viashpy-0.6.0/tests/integration/
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-01-22 14:49:34.606186 viashpy-0.6.0/tests/integration/test_run_component/
--rw-rw-r--   0 di        (1002) di        (1002)     1188 2024-01-22 14:42:51.000000 viashpy-0.6.0/tests/integration/test_run_component/dummy_config.vsh.yaml
--rw-rw-r--   0 di        (1002) di        (1002)     3110 2024-01-22 14:42:51.000000 viashpy-0.6.0/tests/integration/test_run_component/test_script.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-01-22 14:49:34.606186 viashpy-0.6.0/tests/unittests/
--rw-rw-r--   0 di        (1002) di        (1002)     4559 2023-10-04 04:21:36.000000 viashpy-0.6.0/tests/unittests/conftest.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-01-22 14:49:34.606186 viashpy-0.6.0/tests/unittests/fixtures/
--rw-rw-r--   0 di        (1002) di        (1002)     3815 2023-10-06 03:56:03.000000 viashpy-0.6.0/tests/unittests/fixtures/test_meta_variables.py
--rw-rw-r--   0 di        (1002) di        (1002)      675 2022-12-05 09:54:14.000000 viashpy-0.6.0/tests/unittests/fixtures/test_other.py
--rw-rw-r--   0 di        (1002) di        (1002)    11495 2024-01-22 14:42:51.000000 viashpy-0.6.0/tests/unittests/fixtures/test_run_component.py
--rw-rw-r--   0 di        (1002) di        (1002)     1059 2023-09-29 10:18:41.000000 viashpy-0.6.0/tests/unittests/test_read_config.py
--rw-rw-r--   0 di        (1002) di        (1002)     4352 2022-12-05 10:10:54.000000 viashpy-0.6.0/tests/unittests/test_utils.py
--rw-rw-r--   0 di        (1002) di        (1002)      832 2024-01-22 14:42:51.000000 viashpy-0.6.0/tox.ini
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-01-22 14:49:34.606186 viashpy-0.6.0/viashpy/
--rw-rw-r--   0 di        (1002) di        (1002)        0 2024-01-18 20:55:07.000000 viashpy-0.6.0/viashpy/__init__.py
--rw-rw-r--   0 di        (1002) di        (1002)      411 2024-01-22 14:49:34.000000 viashpy-0.6.0/viashpy/__version__.py
--rw-rw-r--   0 di        (1002) di        (1002)     2452 2024-01-22 14:42:51.000000 viashpy-0.6.0/viashpy/_run.py
--rw-rw-r--   0 di        (1002) di        (1002)      541 2024-01-18 20:55:07.000000 viashpy-0.6.0/viashpy/config.py
--rw-rw-r--   0 di        (1002) di        (1002)     7429 2024-01-22 14:42:51.000000 viashpy-0.6.0/viashpy/testing.py
--rw-rw-r--   0 di        (1002) di        (1002)     2321 2024-01-22 09:56:18.000000 viashpy-0.6.0/viashpy/utils.py
-drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-01-22 14:49:34.606186 viashpy-0.6.0/viashpy.egg-info/
--rw-r--r--   0 di        (1002) di        (1002)     2808 2024-01-22 14:49:34.000000 viashpy-0.6.0/viashpy.egg-info/PKG-INFO
--rw-rw-r--   0 di        (1002) di        (1002)      805 2024-01-22 14:49:34.000000 viashpy-0.6.0/viashpy.egg-info/SOURCES.txt
--rw-rw-r--   0 di        (1002) di        (1002)        1 2024-01-22 14:49:34.000000 viashpy-0.6.0/viashpy.egg-info/dependency_links.txt
--rw-rw-r--   0 di        (1002) di        (1002)       37 2024-01-22 14:49:34.000000 viashpy-0.6.0/viashpy.egg-info/entry_points.txt
--rw-rw-r--   0 di        (1002) di        (1002)       35 2024-01-22 14:49:34.000000 viashpy-0.6.0/viashpy.egg-info/requires.txt
--rw-rw-r--   0 di        (1002) di        (1002)        8 2024-01-22 14:49:34.000000 viashpy-0.6.0/viashpy.egg-info/top_level.txt
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-04-22 08:38:51.366029 viashpy-0.7.0/
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-04-22 08:38:51.366029 viashpy-0.7.0/.github/
+-rw-rw-r--   0 di        (1002) di        (1002)      202 2022-12-02 22:58:53.000000 viashpy-0.7.0/.github/dependabot.yml
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-04-22 08:38:51.366029 viashpy-0.7.0/.github/workflows/
+-rw-rw-r--   0 di        (1002) di        (1002)     1367 2024-02-14 13:23:38.000000 viashpy-0.7.0/.github/workflows/ci.yml
+-rw-rw-r--   0 di        (1002) di        (1002)      623 2024-01-19 08:59:14.000000 viashpy-0.7.0/.gitignore
+-rw-rw-r--   0 di        (1002) di        (1002)     4896 2024-04-22 08:29:24.000000 viashpy-0.7.0/CHANGELOG.rst
+-rw-rw-r--   0 di        (1002) di        (1002)    32217 2022-12-02 22:58:53.000000 viashpy-0.7.0/LICENSE
+-rw-rw-r--   0 di        (1002) di        (1002)      125 2022-12-02 22:58:53.000000 viashpy-0.7.0/MANIFEST.in
+-rw-r--r--   0 di        (1002) di        (1002)     2808 2024-04-22 08:38:51.366029 viashpy-0.7.0/PKG-INFO
+-rw-rw-r--   0 di        (1002) di        (1002)     1683 2022-12-02 22:58:53.000000 viashpy-0.7.0/README.md
+-rw-rw-r--   0 di        (1002) di        (1002)       20 2024-01-22 14:42:51.000000 viashpy-0.7.0/_viash.yaml
+-rw-rw-r--   0 di        (1002) di        (1002)      508 2024-01-22 14:42:51.000000 viashpy-0.7.0/pyproject.toml
+-rw-rw-r--   0 di        (1002) di        (1002)     1350 2024-04-22 08:38:51.370029 viashpy-0.7.0/setup.cfg
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-04-22 08:38:51.366029 viashpy-0.7.0/tests/
+-rw-rw-r--   0 di        (1002) di        (1002)      812 2024-01-22 14:42:51.000000 viashpy-0.7.0/tests/conftest.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-04-22 08:38:51.366029 viashpy-0.7.0/tests/integration/
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-04-22 08:38:51.366029 viashpy-0.7.0/tests/integration/test_run_component/
+-rw-rw-r--   0 di        (1002) di        (1002)     1188 2024-04-16 09:35:01.000000 viashpy-0.7.0/tests/integration/test_run_component/dummy_config.vsh.yaml
+-rw-rw-r--   0 di        (1002) di        (1002)     3129 2024-04-16 09:35:01.000000 viashpy-0.7.0/tests/integration/test_run_component/test_script.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-04-22 08:38:51.366029 viashpy-0.7.0/tests/unittests/
+-rw-rw-r--   0 di        (1002) di        (1002)     4559 2023-10-04 04:21:36.000000 viashpy-0.7.0/tests/unittests/conftest.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-04-22 08:38:51.366029 viashpy-0.7.0/tests/unittests/fixtures/
+-rw-rw-r--   0 di        (1002) di        (1002)     3815 2023-10-06 03:56:03.000000 viashpy-0.7.0/tests/unittests/fixtures/test_meta_variables.py
+-rw-rw-r--   0 di        (1002) di        (1002)      675 2022-12-05 09:54:14.000000 viashpy-0.7.0/tests/unittests/fixtures/test_other.py
+-rw-rw-r--   0 di        (1002) di        (1002)    18956 2024-04-22 08:28:48.000000 viashpy-0.7.0/tests/unittests/fixtures/test_run_component.py
+-rw-rw-r--   0 di        (1002) di        (1002)     1059 2023-09-29 10:18:41.000000 viashpy-0.7.0/tests/unittests/test_read_config.py
+-rw-rw-r--   0 di        (1002) di        (1002)     4352 2022-12-05 10:10:54.000000 viashpy-0.7.0/tests/unittests/test_utils.py
+-rw-rw-r--   0 di        (1002) di        (1002)      900 2024-04-22 08:28:48.000000 viashpy-0.7.0/tox.ini
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-04-22 08:38:51.366029 viashpy-0.7.0/viashpy/
+-rw-rw-r--   0 di        (1002) di        (1002)        0 2024-01-18 20:55:07.000000 viashpy-0.7.0/viashpy/__init__.py
+-rw-rw-r--   0 di        (1002) di        (1002)      411 2024-04-22 08:38:51.000000 viashpy-0.7.0/viashpy/__version__.py
+-rw-rw-r--   0 di        (1002) di        (1002)     5836 2024-04-22 08:28:48.000000 viashpy-0.7.0/viashpy/_run.py
+-rw-rw-r--   0 di        (1002) di        (1002)      541 2024-01-18 20:55:07.000000 viashpy-0.7.0/viashpy/config.py
+-rw-rw-r--   0 di        (1002) di        (1002)     7859 2024-04-22 08:28:48.000000 viashpy-0.7.0/viashpy/testing.py
+-rw-rw-r--   0 di        (1002) di        (1002)       95 2024-04-22 08:28:48.000000 viashpy-0.7.0/viashpy/types.py
+-rw-rw-r--   0 di        (1002) di        (1002)     2258 2024-04-16 09:35:01.000000 viashpy-0.7.0/viashpy/utils.py
+drwxrwxr-x   0 di        (1002) di        (1002)        0 2024-04-22 08:38:51.366029 viashpy-0.7.0/viashpy.egg-info/
+-rw-r--r--   0 di        (1002) di        (1002)     2808 2024-04-22 08:38:51.000000 viashpy-0.7.0/viashpy.egg-info/PKG-INFO
+-rw-rw-r--   0 di        (1002) di        (1002)      822 2024-04-22 08:38:51.000000 viashpy-0.7.0/viashpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 di        (1002) di        (1002)        1 2024-04-22 08:38:51.000000 viashpy-0.7.0/viashpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 di        (1002) di        (1002)       37 2024-04-22 08:38:51.000000 viashpy-0.7.0/viashpy.egg-info/entry_points.txt
+-rw-rw-r--   0 di        (1002) di        (1002)       35 2024-04-22 08:38:51.000000 viashpy-0.7.0/viashpy.egg-info/requires.txt
+-rw-rw-r--   0 di        (1002) di        (1002)        8 2024-04-22 08:38:51.000000 viashpy-0.7.0/viashpy.egg-info/top_level.txt
```

### Comparing `viashpy-0.6.0/.github/workflows/ci.yml` & `viashpy-0.7.0/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -40,11 +40,11 @@
           PYTHON_ENV="${{ matrix.python-version }}"
           PYTHON_ENV_NO_DOTS=${PYTHON_ENV//.}
           tox run --skip-env '^(?!py'$PYTHON_ENV_NO_DOTS').+'
   integration_tests:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
-    - uses: viash-io/viash-actions/setup@v4
+    - uses: viash-io/viash-actions/setup@v5
     - name: Viash ns test
       run: |
         viash ns test -s tests/integration/ -p docker --memory 1GB
```

### Comparing `viashpy-0.6.0/.gitignore` & `viashpy-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `viashpy-0.6.0/CHANGELOG.rst` & `viashpy-0.7.0/CHANGELOG.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,41 @@
 
 Changelog
 *********
 
-*.*.* (TBD)
+0.8.0 (TBD)
 ===========
 
+0.7.0 (22/04/2023)
+==================
+
+New Functionality
+-----------------
+
+* Added support for viash 0.9.0 (#23).
+
+Breaking Changes
+----------------
+
+* `run_component` now executes `viash run` with `--engine docker` (or `--platform docker`) 
+  when the test is executed inline (and not as a result of using 'viash test') 
+  instead of the first engine that is defined in the config. Another engine can be
+  specified by using the `engine` keyword argument (#22).
+
+Minor Changes
+-------------
+
+* `run_component` now uses `cachedbuild` setup strategy when tests are executed inline
+  with engine `docker`. This makes sure that the docker image is update when it already
+  exists on the system (#22).
+
+* Added debugging information about the calls that are made to `viash`. If you want to enable
+  debugging information, use `--log-cli-level=DEBUG` from `pytest` (#22).
+
+
 0.6.0 (22/01/2024)
 ==================
 
 Breaking Changes
 ----------------
 * The minimum supported version of pytest is now `6.2` (PR #20).
```

### Comparing `viashpy-0.6.0/LICENSE` & `viashpy-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viashpy-0.6.0/PKG-INFO` & `viashpy-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viashpy
-Version: 0.6.0
+Version: 0.7.0
 Summary: A plugin with various tools and utilities to interact with viash using python.
 Author: Dries Schaumont
 Author-email: dries@data-intuitive.com
 Maintainer: Dries Schaumont
 Maintainer-email: dries@data-intuitive.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `viashpy-0.6.0/README.md` & `viashpy-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `viashpy-0.6.0/setup.cfg` & `viashpy-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `viashpy-0.6.0/tests/conftest.py` & `viashpy-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.6.0/tests/integration/test_run_component/dummy_config.vsh.yaml` & `viashpy-0.7.0/tests/integration/test_run_component/dummy_config.vsh.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   test_resources:
     - type: python_script
       path: test_script.py
     - path: /tests/integration/test_run_component/dummy_config.vsh.yaml
 platforms:
   - type: native
   - type: docker
-    image: python:3.10
+    image: python:3.12
     test_setup:
       - type: docker
         copy: ["filiberke /viashpy"]
       - type: python
         packages:
           - /viashpy
           - ruamel.yaml
```

### Comparing `viashpy-0.6.0/tests/integration/test_run_component/test_script.py` & `viashpy-0.7.0/tests/integration/test_run_component/test_script.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         del original_config["functionality"]["test_resources"]
         del original_config["functionality"]["resources"][1]
         result_path = random_config_path()
         yaml_interface.dump(original_config, result_path)
         return result_path
 
     def test_run_component_check_correct_memory_syntax(self, run_component):
-        captured_output = run_component(["--output", "bar.txt"])
+        captured_output = run_component(["--output", "bar.txt"], platform="native")
         with open("bar.txt", "r") as open_output_file:
             contents = open_output_file.read()
             assert contents == "foo!"
         assert (
             captured_output is not None
         ), "Some output from stdout or stderr should have been captured"
         assert (
```

### Comparing `viashpy-0.6.0/tests/unittests/conftest.py` & `viashpy-0.7.0/tests/unittests/conftest.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.6.0/tests/unittests/fixtures/test_meta_variables.py` & `viashpy-0.7.0/tests/unittests/fixtures/test_meta_variables.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.6.0/tests/unittests/fixtures/test_other.py` & `viashpy-0.7.0/tests/unittests/fixtures/test_other.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.6.0/tests/unittests/fixtures/test_run_component.py` & `viashpy-0.7.0/tests/unittests/fixtures/test_run_component.py`

 * *Files 26% similar despite different names*

```diff
@@ -42,14 +42,134 @@
         [
             "*AttributeError: Could not find meta variable in module*",
         ]
     )
     assert result.ret != 0
 
 
+def test_run_viash_returns_unknown_viash_version_format_raises(
+    pytester, makepyfile_and_add_meta, dummy_config
+):
+    makepyfile_and_add_meta(
+        """
+        import subprocess
+        from pathlib import Path
+
+        def test_loading_run_component(mocker, run_component):
+            mocked = mocker.patch('viashpy._run.check_output', return_value=b"UNKNOWNVERSION")
+            run_component(["bar"])
+            mocked.assert_called_once_with([Path("foo"), "bar"],
+                                        stderr=subprocess.STDOUT)
+        """,
+        dummy_config,
+        "foo",
+    )
+    result = pytester.runpytest("-v")
+    result.stdout.fnmatch_lines(
+        [
+            "*Could not parse the version information as output by viash.*",
+        ]
+    )
+    assert result.ret != 0
+
+
+@pytest.mark.parametrize("viash_version", ["(0, 8, 2)", "(0, 9, 0)"])
+def test_run_both_platform_and_engine_raises(
+    pytester, makepyfile_and_add_meta, dummy_config, viash_version
+):
+    makepyfile_and_add_meta(
+        f"""
+        import subprocess
+        from pathlib import Path
+
+        def test_loading_run_component(mocker, run_component):
+            mocked_viash_check = mocker.patch('viashpy._run._get_viash_version', return_value={viash_version})
+            run_component(["bar"], platform="native", engine="native")
+        """,
+        dummy_config,
+        "foo",
+    )
+    result = pytester.runpytest("-v")
+    result.stdout.fnmatch_lines(
+        [
+            "*ValueError: Cannot pass both an 'engine' and a 'plaform'.*",
+        ]
+    )
+    assert result.ret != 0
+
+
+@pytest.mark.parametrize(
+    "viash_version, wrong_platform_or_engine",
+    [((0, 8, 2), "engine"), ((0, 9, 0), "platform")],
+)
+def test_engine_platform_specified_but_wrong_viash_version(
+    pytester,
+    makepyfile_and_add_meta,
+    dummy_config,
+    viash_version,
+    wrong_platform_or_engine,
+):
+    makepyfile_and_add_meta(
+        f"""
+        import subprocess
+        from functools import partial
+        from pathlib import Path
+
+        def test_loading_run_component(mocker, run_component):
+            mocked_viash_check = mocker.patch('viashpy._run._get_viash_version',
+                                              return_value=({','.join(map(str, viash_version))}))
+            run_component(["bar"], {wrong_platform_or_engine}="native")
+        """,
+        dummy_config,
+        "foo",
+    )
+    result = pytester.runpytest("-v")
+    correct_arg = "engine" if wrong_platform_or_engine == "platform" else "platform"
+    result.stdout.fnmatch_lines(
+        [
+            f"*ValueError: Viash version {'.'.join(map(str, viash_version))} requires using "
+            f"'{correct_arg}' instead of '{wrong_platform_or_engine}'.*",
+        ]
+    )
+    assert result.ret != 0
+
+
+def test_could_not_get_viash_version_raises(
+    pytester, makepyfile_and_add_meta, dummy_config
+):
+    makepyfile_and_add_meta(
+        """
+        import subprocess
+        from functools import partial
+        from pathlib import Path
+
+        def test_loading_run_component(mocker, run_component):
+            mocked_viash_check = mocker.patch('viashpy._run.check_output',
+                                              side_effect=subprocess.CalledProcessError(1, "foo"))
+            run_component(["bar"], platform="native")
+        """,
+        dummy_config,
+        "foo",
+    )
+    result = pytester.runpytest("-v")
+    result.stdout.fnmatch_lines(
+        [
+            "*subprocess.CalledProcessError: Command 'foo' returned non-zero exit status 1.*",
+        ]
+    )
+    assert result.ret != 0
+
+
+@pytest.mark.parametrize(
+    "viash_version, platform_or_engine",
+    [
+        ("viash 0.8.2 (c) 2020 Data Intuitive", "platform"),
+        ("viash 0.9.0 (c) 2020 Data Intuitive", "engine"),
+    ],
+)
 @pytest.mark.parametrize(
     "memory_pb, memory_tb, memory_gb, memory_mb, memory_kb, memory_b, expected_bytes, expected_warning",
     [
         (
             None,
             None,
             None,
@@ -131,44 +251,57 @@
     memory_tb,
     memory_gb,
     memory_mb,
     memory_kb,
     memory_b,
     expected_bytes,
     expected_warning,
+    viash_version,
+    platform_or_engine,
 ):
     expected_memory_args = ", "
     memory_specifiers = [
         memory_pb,
         memory_tb,
         memory_gb,
         memory_mb,
         memory_kb,
         memory_b,
     ]
     memory_specifiers = [
         specifier for specifier in memory_specifiers if specifier != "None"
     ]
     if any(memory_specifiers):
-        expected_memory_args = f', "---memory", "{expected_bytes}B", '
-    expected = (
-        '["viash", "run", Path(meta["config"]), "--", "bar"%s]' % expected_memory_args
+        expected_memory_args = f', "--memory", "{expected_bytes}B", '
+    expected_base_command = (
+        f'["viash", "run", Path(meta["config"]), "--{platform_or_engine}", "docker", "-c",'
+        f"\".{platform_or_engine}s[.type == 'docker'].target_tag := 'test'\""
+    )
+    expected_build_call = (
+        f"mocker.call({expected_base_command}, "
+        '"--", "---setup", "cachedbuild"], stderr=subprocess.STDOUT)'
     )
+    expected_run_call = (
+        f'mocker.call({expected_base_command}{expected_memory_args}"--", "bar"], '
+        "stderr=subprocess.STDOUT)"
+    )
+
     makepyfile_and_add_meta(
         f"""
         import subprocess
         from pathlib import Path
 
         def test_loading_run_component(mocker, run_component):
             mocked_check_output = mocker.patch('viashpy._run.check_output',
-                                               return_value=b"Some dummy output")
+                                               side_effect=[b"{viash_version}", None, b"Some dummy output"])
             mocked_path = mocker.patch('viashpy.testing.Path.is_file', return_value=True)
             stdout = run_component(["bar"])
-            mocked_check_output.assert_called_once_with({expected},
-                                                        stderr=subprocess.STDOUT)
+            mocked_check_output.assert_has_calls([mocker.call(['viash', '--version']),
+                                                  {expected_build_call},
+                                                  {expected_run_call}])
             assert stdout == b"Some dummy output"
         """,
         dummy_config,
         "foo",
         memory_pb=memory_pb,
         memory_tb=memory_tb,
         memory_gb=memory_gb,
@@ -177,59 +310,137 @@
         memory_b=memory_b,
     )
     result = pytester.runpytest()
     result.assert_outcomes(passed=1)
     if expected_warning:
         result.stdout.fnmatch_lines(
             [
-                "*Different values were defined in the 'meta' dictionary that limit memory, choosing the one with the smallest unit.*"
+                "*Different values were defined in the 'meta' dictionary that "
+                "limit memory, choosing the one with the smallest unit.*"
             ]
         )
     assert result.ret == 0
 
 
+@pytest.mark.parametrize(
+    "viash_version, platform_or_engine",
+    [((0, 8, 2), "platform"), ((0, 9, 0), "engine")],
+)
+@pytest.mark.parametrize(
+    "expected_build_cmd, expected_run_cmd",
+    [
+        (
+            '["viash", "run", Path(meta["config"]), "--{0}", "docker", "-c", '
+            '".{0}s[.type == \'docker\'].target_tag := \'test\'", "--", "---setup", "cachedbuild"]',
+            '["viash", "run", Path(meta["config"]), "--{0}", "docker", '
+            '"-c", ".{0}s[.type == \'docker\'].target_tag := \'test\'", "--", "bar"]',
+        ),
+    ],
+)
+def test_run_component_set_platform_or_engine(
+    pytester,
+    makepyfile_and_add_meta,
+    dummy_config,
+    expected_build_cmd,
+    expected_run_cmd,
+    viash_version,
+    platform_or_engine,
+):
+    expected_build_cmd_call, excpected_run_cmd_call = "", ""
+    if expected_build_cmd:
+        expected_build_cmd = expected_build_cmd.format(platform_or_engine)
+        expected_build_cmd_call = f"mocker.call({expected_build_cmd}, stderr=-2)"
+    if expected_run_cmd:
+        expected_run_cmd = expected_run_cmd.format(platform_or_engine)
+        excpected_run_cmd_call = f"mocker.call({expected_run_cmd}, stderr=-2)"
+    expected = ", ".join(
+        filter(None, [expected_build_cmd_call, excpected_run_cmd_call])
+    )
+    makepyfile_and_add_meta(
+        f"""
+        import subprocess
+        from pathlib import Path
+
+        def test_loading_run_component(mocker, run_component):
+            mocked_viash_check = mocker.patch('viashpy._run._get_viash_version', return_value={viash_version})
+            mocked_check_output = mocker.patch('viashpy._run.check_output', return_value=b"Some dummy output")
+            mocked_path = mocker.patch('viashpy.testing.Path.is_file', return_value=True)
+            stdout = run_component(["bar"], {platform_or_engine}="docker")
+            mocked_check_output.assert_has_calls([{expected}])
+            assert stdout == b"Some dummy output"
+        """,
+        dummy_config,
+        "foo",
+    )
+    result = pytester.runpytest("-v")
+    result.assert_outcomes(passed=1)
+
+
 @pytest.mark.parametrize("memory, expected_bytes", [(None, None), (6, 6442450944)])
 @pytest.mark.parametrize("cpu", [None, 2])
 @pytest.mark.parametrize(
-    "config_fixture, expected",
+    "config_fixture, expected_build_cmd, expected_run_cmd, expected_prefix",
     [
         (
             "dummy_config",
-            '["viash", "run", Path(meta["config"]), "--", "bar"%s%s]',
+            '["viash", "run", Path(meta["config"]), "--platform", "docker", "-c", '
+            '".platforms[.type == \'docker\'].target_tag := \'test\'", "--", "---setup", "cachedbuild"]',
+            '["viash", "run", Path(meta["config"]), "--platform", "docker", '
+            '"-c", ".platforms[.type == \'docker\'].target_tag := \'test\'"%s%s, "--", "bar"]',
+            "--",
         ),
-        ("dummy_config_with_info", '[Path("foo"), "bar"%s%s]'),
+        ("dummy_config_with_info", "", '[Path("foo"), "bar"%s%s]', "---"),
     ],
 )
 def test_run_component_executes_subprocess(
     request,
     pytester,
     makepyfile_and_add_meta,
     memory,
     expected_bytes,
     cpu,
     config_fixture,
-    expected,
+    expected_build_cmd,
+    expected_run_cmd,
+    expected_prefix,
 ):
     format_string = (
-        f', "---cpus", "{cpu}"' if cpu else "",
-        f', "---memory", "{expected_bytes}B"' if memory else "",
+        f', "{expected_prefix}cpus", "{cpu}"' if cpu else "",
+        f', "{expected_prefix}memory", "{expected_bytes}B"' if memory else "",
+    )
+    expected_run_cmd = expected_run_cmd % format_string
+    (
+        expected_version_cmd,
+        expected_build_cmd_call,
+        excpected_run_cmd_call,
+        mocked_return,
+    ) = [""] * 4
+    if expected_build_cmd:
+        mocked_return += 'b"viash 0.8.2 (c) 2020 Data Intuitive", None, '
+        expected_build_cmd_call = f"mocker.call({expected_build_cmd}, stderr=-2)"
+    if expected_run_cmd:
+        excpected_run_cmd_call = f"mocker.call({expected_run_cmd}, stderr=-2)"
+    expected = ", ".join(
+        filter(
+            None,
+            [expected_version_cmd, expected_build_cmd_call, excpected_run_cmd_call],
+        )
     )
-    expected = expected % format_string
+    mocked_return += 'b"Some dummy output"'
     makepyfile_and_add_meta(
         f"""
         import subprocess
         from pathlib import Path
 
         def test_loading_run_component(mocker, run_component):
             mocked_check_output = mocker.patch('viashpy._run.check_output',
-                                               return_value=b"Some dummy output")
+                                               side_effect=[{mocked_return}])
             mocked_path = mocker.patch('viashpy.testing.Path.is_file', return_value=True)
             stdout = run_component(["bar"])
-            mocked_check_output.assert_called_once_with({expected},
-                                                        stderr=subprocess.STDOUT)
+            mocked_check_output.assert_has_calls([{expected}])
             assert stdout == b"Some dummy output"
         """,
         request.getfixturevalue(config_fixture),
         "foo",
         cpu=cpu,
         memory_gb=memory,
     )
```

### Comparing `viashpy-0.6.0/tests/unittests/test_read_config.py` & `viashpy-0.7.0/tests/unittests/test_read_config.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.6.0/tests/unittests/test_utils.py` & `viashpy-0.7.0/tests/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.6.0/tox.ini` & `viashpy-0.7.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # For more information about tox, see https://tox.readthedocs.io/en/latest/
 [tox]
 envlist = 
     py{39}-pytest{62}
-    py{39,310,311,312}-pytest{70,71,72,73,74}
+    py{39,310,311,312}-pytest{70,71,72,73,74,80,81}
     flake8
 isolated_build = True
 
 [testenv]
 deps = 
     pytest62: pytest>=6.2,<6.3
     pytest70: pytest>=7.0,<7.1
     pytest71: pytest>=7.1,<7.2
     pytest72: pytest>=7.2,<7.3
     pytest73: pytest>=7.3,<7.4
     pytest74: pytest>=7.4,<7.5
+    pytest80: pytest>=8.0,<8.1
+    pytest81: pytest>=8.1,<8.2
     coverage
     pytest-mock
 commands = 
     coverage run -m pytest --pyargs tests/unittests
     coverage report -m
     coverage xml
```

### Comparing `viashpy-0.6.0/viashpy/config.py` & `viashpy-0.7.0/viashpy/config.py`

 * *Files identical despite different names*

### Comparing `viashpy-0.6.0/viashpy/testing.py` & `viashpy-0.7.0/viashpy/testing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
 import pytest
 import logging
 from ._run import run_build_component, viash_run, tobytesconverter
+from .types import Engine, Platform
 from .config import read_viash_config
 from pathlib import Path
 from functools import wraps
 from subprocess import CalledProcessError
 import warnings
 
 logger = logging.getLogger(__name__)
@@ -129,18 +131,23 @@
     that the test is being run as a result from running 'viash test'/
     'viash_test' or the 'source' config as defined by the user.
     From a parsed config, the path to the original config source can be
     retreived from .['info']['config'] keys.
     """
     try:
         # meta_config is a parsed viash config, retreive the location of the source
-        return Path(meta_config["info"]["config"])
+        return Path(meta_config["build_info"]["config"])
     except KeyError:
-        # If .['info']['config'] is not defined, assume that the config is a source config
-        return meta_config_path
+        # viash < 0.9 defines info instead of build_info
+        try:
+            return Path(meta_config["info"]["config"])
+        except KeyError:
+            # If .['info']['config'] or .['build_info']['config'] is not defined,
+            # assume that the config is a source config
+            return meta_config_path
 
 
 @pytest.fixture
 def viash_source_config(viash_source_config_path):
     return read_viash_config(viash_source_config_path)
 
 
@@ -179,21 +186,25 @@
                     raise e.with_traceback(None) from None
 
         return wrapper
 
     if viash_source_config_path.is_file():
 
         @run_and_handle_errors
-        def wrapper(args_as_list):
+        def wrapper(
+            args_as_list, engine: Engine | None = None, platform: Platform | None = None
+        ):
             return viash_run(
                 viash_source_config_path,
                 args_as_list,
                 viash_location=viash_executable,
                 cpus=cpus,
                 memory=memory_bytes,
+                engine=engine,
+                platform=platform,
             )
 
         return wrapper
 
     logger.debug(
         "Could not find the original viash config source. "
         "Assuming test script is run from 'viash test' or 'viash_test'."
```

### Comparing `viashpy-0.6.0/viashpy/utils.py` & `viashpy-0.7.0/viashpy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
 def extract_tar(pathname: Path | str, output_dir: Path | str):
     pathname, output_dir = Path(pathname), Path(output_dir)
 
     if not pathname.is_file():
         raise FileNotFoundError(f"{pathname} does not exist or is not a file.")
 
-    # TODO: is_tarfile supports a path from python >= 3.9
-    if not tarfile.is_tarfile(str(pathname)):
+    if not tarfile.is_tarfile(pathname):
         raise ValueError(f"{pathname} is not a tarfile.")
 
     if not output_dir.is_dir():
         raise FileNotFoundError(
             f"Directory {output_dir} does not exist or is not a directory."
         )
```

### Comparing `viashpy-0.6.0/viashpy.egg-info/PKG-INFO` & `viashpy-0.7.0/viashpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viashpy
-Version: 0.6.0
+Version: 0.7.0
 Summary: A plugin with various tools and utilities to interact with viash using python.
 Author: Dries Schaumont
 Author-email: dries@data-intuitive.com
 Maintainer: Dries Schaumont
 Maintainer-email: dries@data-intuitive.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `viashpy-0.6.0/viashpy.egg-info/SOURCES.txt` & `viashpy-0.7.0/viashpy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 tests/unittests/fixtures/test_other.py
 tests/unittests/fixtures/test_run_component.py
 viashpy/__init__.py
 viashpy/__version__.py
 viashpy/_run.py
 viashpy/config.py
 viashpy/testing.py
+viashpy/types.py
 viashpy/utils.py
 viashpy.egg-info/PKG-INFO
 viashpy.egg-info/SOURCES.txt
 viashpy.egg-info/dependency_links.txt
 viashpy.egg-info/entry_points.txt
 viashpy.egg-info/requires.txt
 viashpy.egg-info/top_level.txt
```

