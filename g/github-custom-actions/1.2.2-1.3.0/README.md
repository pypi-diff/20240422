# Comparing `tmp/github_custom_actions-1.2.2.tar.gz` & `tmp/github_custom_actions-1.3.0.tar.gz`

## Comparing `github_custom_actions-1.2.2.tar` & `github_custom_actions-1.3.0.tar`

### file list

```diff
@@ -1,54 +1,58 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/.coveragerc
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/.mypy.ini
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/.pylintrc
--rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/activate.sh
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/invoke.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/pytest.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/requirements.dev.in
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/requirements.dev.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/requirements.in
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/requirements.txt
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/tasks.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/.github/workflows/pip_publish.yml
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/.github/workflows/static.yml
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/docs/mkdocs.yml
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/docs/src/en/github_env_vars.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/docs/src/en/index.md
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/docs/src/en/quick_start.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/docs/src/en/reference.md
--rw-r--r--   0        0        0   302032 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/docs/src/en/images/var_ide_hover_docstring.jpg
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/docs/src/ru/github_env_vars.md
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/docs/src/ru/index.md
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/docs/src/ru/quick_start.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/scripts/__init__.py
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/scripts/build.sh
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/scripts/docs-render-config.sh
--rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/scripts/docstrings.sh
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/scripts/include_pyproject_requirements.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/scripts/upload.sh
--rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/scripts/verup.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/src/github_custom_actions/__about__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/src/github_custom_actions/__init__.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/src/github_custom_actions/action_base.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/src/github_custom_actions/attr_dict_vars.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/src/github_custom_actions/env_attr_dict_vars.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/src/github_custom_actions/file_attr_dict_vars.py
--rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/src/github_custom_actions/github_vars.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/src/github_custom_actions/inputs_outputs.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/tests/conftest.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/tests/test_action_base.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/tests/test_env_attr_dict_vars.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/tests/test_file_attr_dict_vars.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/tests/test_github_custom_actions.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/tests/test_github_vars.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/tests/test_inputs_outputs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/LICENSE.txt
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/README.md
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 github_custom_actions-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.coveragerc
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.mypy.ini
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.pylintrc
+-rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/activate.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/invoke.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/pytest.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/requirements.dev.in
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/requirements.dev.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/requirements.in
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/requirements.txt
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tasks.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.github/workflows/pip_publish.yml
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.github/workflows/static.yml
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/mkdocs.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/includes/input_output_typed.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/includes/install_pipx_macos.sh
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/includes/quick_start.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/github_env_vars.md
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/index.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/inputs.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/installation.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/reference.md
+-rw-r--r--   0        0        0    52770 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/en/images/var_ide_hover_docstring.jpg
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/ru/github_env_vars.md
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/ru/index.md
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/docs/src/ru/installation.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/__init__.py
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/build.sh
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/docs-render-config.sh
+-rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/docstrings.sh
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/include_pyproject_requirements.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/upload.sh
+-rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/scripts/verup.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/__about__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/__init__.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/action_base.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/attr_dict_vars.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/env_attr_dict_vars.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/file_attr_dict_vars.py
+-rw-r--r--   0        0        0    10652 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/github_vars.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/src/github_custom_actions/inputs_outputs.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_action_base.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_env_attr_dict_vars.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_file_attr_dict_vars.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_github_custom_actions.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_github_vars.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/tests/test_inputs_outputs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/README.md
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 github_custom_actions-1.3.0/PKG-INFO
```

### Comparing `github_custom_actions-1.2.2/.pre-commit-config.yaml` & `github_custom_actions-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/activate.sh` & `github_custom_actions-1.3.0/activate.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/requirements.dev.txt` & `github_custom_actions-1.3.0/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/tasks.py` & `github_custom_actions-1.3.0/tasks.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/.github/workflows/ci.yml` & `github_custom_actions-1.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/.github/workflows/docs.yml` & `github_custom_actions-1.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/.github/workflows/pip_publish.yml` & `github_custom_actions-1.3.0/.github/workflows/pip_publish.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/.github/workflows/static.yml` & `github_custom_actions-1.3.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/docs/mkdocs.yml` & `github_custom_actions-1.3.0/docs/mkdocs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 # Repository
 repo_name: github_custom_actions
 repo_url: https://github.com/andgineer/github-custom-actions
 edit_uri: edit/master/docs
 docs_dir: 'src/LANGUAGE'
 site_dir: '../site/SITE_PREFIX'
 
+nav:
+  - index.md
+  - installation.md
+  - inputs.md
+  - github_env_vars.md
+
 plugins:
   - awesome-pages
   - search:
       lang: LANGUAGE
   - mkdocstrings:
       handlers:
         python:
@@ -46,15 +52,15 @@
   - abbr
   - attr_list
   - pymdownx.details
   - pymdownx.superfences
   - pymdownx.tabbed:
       alternate_style: true
   - pymdownx.snippets:
-      base_path: 'docs'
+      base_path: 'docs/includes'
 
 theme:
   name: material
   features:
     - toc.integrate
     - navigation.tracking
     - content.code.copy
```

### Comparing `github_custom_actions-1.2.2/docs/src/en/index.md` & `github_custom_actions-1.3.0/docs/src/en/installation.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-# Installation
-
-Python package for creating [custom GitHub Actions](https://docs.github.com/en/actions/creating-actions/about-custom-actions). 
-
-Supports Python 3.7 and higher for very only self-hosted action runners.
-
-- [Example of usage](https://github.com/andgineer/allure-report)
-
-## Installation
-
 ## Installing pipx
 [`pipx`](https://pypa.github.io/pipx/) creates isolated environments to avoid conflicts with existing system packages.
 
 === "MacOS"
     In the terminal, execute:
     ```bash
-    brew install pipx
-    pipx ensurepath
+    --8<-- "install_pipx_macos.sh"
     ```
 
 === "Linux"
     First, ensure Python is installed.
 
     Enter in the terminal:
```

### Comparing `github_custom_actions-1.2.2/docs/src/ru/index.md` & `github_custom_actions-1.3.0/docs/src/ru/installation.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-# github-custom-actions
-
-Библиотека упрощающая создание
-[custom GitHub Actions](https://docs.github.com/en/actions/creating-actions/about-custom-actions).
-
-Поддерживает Python 3.7 и выше для древних self-hosted action runners.
-
-- [Пример использования](https://github.com/andgineer/allure-report)
-
 ## Установка
 
 ## Установка pipx
 [`pipx`](https://pypa.github.io/pipx/) создает изолированные среды, чтобы избежать конфликтов с 
 существующими системными пакетами.
 
 === "MacOS"
```

### Comparing `github_custom_actions-1.2.2/scripts/include_pyproject_requirements.py` & `github_custom_actions-1.3.0/scripts/include_pyproject_requirements.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/scripts/verup.sh` & `github_custom_actions-1.3.0/scripts/verup.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/src/github_custom_actions/action_base.py` & `github_custom_actions-1.3.0/src/github_custom_actions/action_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import traceback
-from typing import Any, Optional
+from pathlib import Path
+from typing import Any, get_type_hints
 
-from jinja2 import Template
+from jinja2 import Template, Environment, FileSystemLoader
 
 from github_custom_actions.inputs_outputs import ActionOutputs, ActionInputs
 from github_custom_actions.github_vars import GithubVars
 
 
 class FileTextProperty:
     """Property descriptor read / write from a file."""
@@ -36,23 +37,29 @@
 
 class ActionBase:
     """Base class for GitHub Actions.
 
     Implement main() method in the subclass.
     """
 
-    def __init__(
-        self, inputs: Optional[ActionInputs] = None, outputs: Optional[ActionOutputs] = None
-    ) -> None:
-        # (!) AttrDictVars() works as dict so empty one is False.
-        # This is why we cannot use usual shorthand "or" here
-        self.inputs = inputs if inputs is not None else ActionInputs()
-        self.outputs = outputs if outputs is not None else ActionOutputs()
+    inputs: ActionInputs
+    outputs: ActionOutputs
+    vars: GithubVars
+
+    def __init__(self) -> None:
+        # Initialize inputs, outputs according to the type than could be set in subclass.
+        types = get_type_hints(self.__class__)
+        self.inputs = types["inputs"]()
+        self.outputs = types["outputs"]()
         self.vars = GithubVars()
 
+        base_dir = Path(__file__).resolve().parent
+        templates_dir = base_dir / "templates"
+        self.environment = Environment(loader=FileSystemLoader(str(templates_dir)))
+
     summary = FileTextProperty("github_step_summary")
 
     def main(self) -> None:
         """Main method."""
         raise NotImplementedError
 
     def run(self) -> None:
```

### Comparing `github_custom_actions-1.2.2/src/github_custom_actions/attr_dict_vars.py` & `github_custom_actions-1.3.0/src/github_custom_actions/attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/src/github_custom_actions/env_attr_dict_vars.py` & `github_custom_actions-1.3.0/src/github_custom_actions/env_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/src/github_custom_actions/file_attr_dict_vars.py` & `github_custom_actions-1.3.0/src/github_custom_actions/file_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/src/github_custom_actions/github_vars.py` & `github_custom_actions-1.3.0/src/github_custom_actions/github_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/src/github_custom_actions/inputs_outputs.py` & `github_custom_actions-1.3.0/src/github_custom_actions/inputs_outputs.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/tests/conftest.py` & `github_custom_actions-1.3.0/tests/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,10 +34,15 @@
     another_input: str
 
 
 class Outputs(ActionOutputs):
     my_output: str
 
 
+class Action(ActionBase):
+    inputs: Inputs
+    outputs: Outputs
+
+
 @pytest.fixture(scope="function")
 def action(inputs, outputs):
-    return ActionBase(inputs=Inputs(), outputs=Outputs())
+    return Action()
```

### Comparing `github_custom_actions-1.2.2/tests/test_env_attr_dict_vars.py` & `github_custom_actions-1.3.0/tests/test_env_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/tests/test_file_attr_dict_vars.py` & `github_custom_actions-1.3.0/tests/test_file_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/tests/test_github_vars.py` & `github_custom_actions-1.3.0/tests/test_github_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/tests/test_inputs_outputs.py` & `github_custom_actions-1.3.0/tests/test_inputs_outputs.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/LICENSE.txt` & `github_custom_actions-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/README.md` & `github_custom_actions-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,41 +3,22 @@
 # github-custom-actions
 
 Python package for creating [custom GitHub Actions](https://docs.github.com/en/actions/creating-actions/about-custom-actions). 
 
 #### Example of usage
 
 ```python
-from github_custom_actions import ActionBase, ActionInputs, ActionOutputs
-
-class MyInputs(ActionInputs):
-    my_input: str
-    """My input description"""
-    
-    my_path: Path
-    """My path description"""
-    
-    
-class MyOutputs(ActionOutputs):
-    runner_os: str
-    """Runner OS description"""
-
+from github_custom_actions import ActionBase
     
 class MyAction(ActionBase):
-    def __init__(self):
-        super().__init__(inputs=MyInputs(), outputs=MyOutputs())
-        if self.inputs.my_path is None:
-            raise ValueError("my_path is required")
-
     def main(self):
-        self.inputs.my_path.mkdir(exist_ok=True)
-        self.outputs.runner_os = self.vars.runner_os
+        self.outputs["runner-os"] = self.vars.runner_os
         self.summary.text += (
             self.render(
-                "### {{ inputs.my_input }}.\n"
+                "### {{ inputs['my-input'] }}.\n"
                 "Have a nice day!"
             )
         )
 
 if __name__ == "__main__":
     MyAction().run()
 ```
```

### Comparing `github_custom_actions-1.2.2/pyproject.toml` & `github_custom_actions-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-1.2.2/PKG-INFO` & `github_custom_actions-1.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: github-custom-actions
-Version: 1.2.2
+Version: 1.3.0
 Summary: Python package for creating custom GitHub Actions.
 Project-URL: Homepage, https://andgineer.github.io/github-custom-actions/
 Project-URL: Documentation, https://andgineer.github.io/github-custom-actions/
 Author-email: Andrey Sorokin <andrey@sorokin.engineer>
 License: Copyright (c) 2024 Andrey Sorokin <andrey@sorokin.engineer>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -39,41 +39,22 @@
 # github-custom-actions
 
 Python package for creating [custom GitHub Actions](https://docs.github.com/en/actions/creating-actions/about-custom-actions). 
 
 #### Example of usage
 
 ```python
-from github_custom_actions import ActionBase, ActionInputs, ActionOutputs
-
-class MyInputs(ActionInputs):
-    my_input: str
-    """My input description"""
-    
-    my_path: Path
-    """My path description"""
-    
-    
-class MyOutputs(ActionOutputs):
-    runner_os: str
-    """Runner OS description"""
-
+from github_custom_actions import ActionBase
     
 class MyAction(ActionBase):
-    def __init__(self):
-        super().__init__(inputs=MyInputs(), outputs=MyOutputs())
-        if self.inputs.my_path is None:
-            raise ValueError("my_path is required")
-
     def main(self):
-        self.inputs.my_path.mkdir(exist_ok=True)
-        self.outputs.runner_os = self.vars.runner_os
+        self.outputs["runner-os"] = self.vars.runner_os
         self.summary.text += (
             self.render(
-                "### {{ inputs.my_input }}.\n"
+                "### {{ inputs['my-input'] }}.\n"
                 "Have a nice day!"
             )
         )
 
 if __name__ == "__main__":
     MyAction().run()
 ```
```

