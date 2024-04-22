# Comparing `tmp/gitlab_projects_migrate-1.0.0.tar.gz` & `tmp/gitlab_projects_migrate-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_migrate-1.0.0.tar", last modified: Sun Apr 21 16:11:24 2024, max compression
+gzip compressed data, was "gitlab_projects_migrate-1.1.0.tar", last modified: Mon Apr 22 00:53:17 2024, max compression
```

## Comparing `gitlab_projects_migrate-1.0.0.tar` & `gitlab_projects_migrate-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 16:11:24.889294 gitlab_projects_migrate-1.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 16:11:24.882294 gitlab_projects_migrate-1.0.0/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      702 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     6085 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 16:11:24.883294 gitlab_projects_migrate-1.0.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4902 2024-04-21 16:11:24.888294 gitlab_projects_migrate-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3321 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 16:11:24.883294 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 16:11:24.885294 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4356 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 16:11:24.886294 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/features/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     4044 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/features/migration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 16:11:24.886294 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 16:11:24.887294 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/system/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 16:11:24.888294 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4902 2024-04-21 16:11:24.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1094 2024-04-21 16:11:24.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 16:11:24.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2024-04-21 16:11:24.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-21 16:11:24.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-21 16:11:24.000000 gitlab_projects_migrate-1.0.0/gitlab_projects_migrate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 16:11:24.888294 gitlab_projects_migrate-1.0.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-21 16:11:24.889294 gitlab_projects_migrate-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2684 2024-04-21 16:11:17.000000 gitlab_projects_migrate-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.116985 gitlab_projects_migrate-1.1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.109985 gitlab_projects_migrate-1.1.0/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      702 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     6085 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.110985 gitlab_projects_migrate-1.1.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)      469 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-04-22 00:53:17.115985 gitlab_projects_migrate-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.110985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.112985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4603 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.112985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3163 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/features/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5472 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/features/migration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.113985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.114985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/prints/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.114985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.115985 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-22 00:53:17.000000 gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 00:53:17.115985 gitlab_projects_migrate-1.1.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 00:53:17.116985 gitlab_projects_migrate-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2684 2024-04-22 00:53:10.000000 gitlab_projects_migrate-1.1.0/setup.py
```

### Comparing `gitlab_projects_migrate-1.0.0/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_migrate-1.1.0/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.0.0/.chglog/changelog.sh` & `gitlab_projects_migrate-1.1.0/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.0.0/.chglog/config.yml` & `gitlab_projects_migrate-1.1.0/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.0.0/.gitlab-ci.yml` & `gitlab_projects_migrate-1.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.0.0/.style.yapf` & `gitlab_projects_migrate-1.1.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.0.0/.vscode/extensions.json` & `gitlab_projects_migrate-1.1.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.0.0/.vscode/settings.json` & `gitlab_projects_migrate-1.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.0.0/LICENSE` & `gitlab_projects_migrate-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.0.0/PKG-INFO` & `gitlab_projects_migrate-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-migrate
-Version: 1.0.0
+Version: 1.1.0
 Summary: Migrate GitLab projects from a GitLab group to another GitLab's group
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-migrate
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-migrate/blob/main/CHANGELOG.md
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colored>=1.4.2
 Requires-Dist: python-gitlab>=4.4.0
 Requires-Dist: setuptools>=45.1.0
 
 # gitlab-projects-migrate
 
 <!-- markdownlint-disable no-inline-html -->
 
@@ -74,28 +75,29 @@
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 
 ```yaml
-usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--keep-members]
+usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--keep-members] [--overwrite]
                                [--set-avatar FILE] [--update-description]
                                [input_gitlab] [input_group] [output_gitlab] [output_group]
 
 gitlab-projects-migrate: Synchronize projects from a GitLab group to another GitLab group
 
 internal arguments:
   -h, --help            # Show this help message
   --version             # Show the current version
 
 migration arguments:
   -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN environment)
   -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN environment or input_token)
   --keep-members        # Keep input members after importing on output GitLab
+  --overwrite           # Overwrite existing projects on output GitLab
   --set-avatar FILE     # Set imported projects' avatar to a specific image file
   --update-description  # Update project description automatically inside output group
 
 positional arguments:
   input_gitlab          # Input GitLab URL (default: https://gitlab.com)
   input_group           # Input GitLab group
   output_gitlab         # Output GitLab URL (default: https://gitlab.com)
@@ -104,14 +106,15 @@
 
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Dependencies
 
+- [colored](https://pypi.org/project/colored/): Terminal colors and styles
 - [python-gitlab](https://pypi.org/project/python-gitlab/): A python wrapper for the GitLab API
 - [setuptools](https://pypi.org/project/setuptools/): Build and manage Python packages
 
 ---
 
 ## References
```

### Comparing `gitlab_projects_migrate-1.0.0/README.md` & `gitlab_projects_migrate-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -41,28 +41,29 @@
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 
 ```yaml
-usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--keep-members]
+usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--keep-members] [--overwrite]
                                [--set-avatar FILE] [--update-description]
                                [input_gitlab] [input_group] [output_gitlab] [output_group]
 
 gitlab-projects-migrate: Synchronize projects from a GitLab group to another GitLab group
 
 internal arguments:
   -h, --help            # Show this help message
   --version             # Show the current version
 
 migration arguments:
   -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN environment)
   -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN environment or input_token)
   --keep-members        # Keep input members after importing on output GitLab
+  --overwrite           # Overwrite existing projects on output GitLab
   --set-avatar FILE     # Set imported projects' avatar to a specific image file
   --update-description  # Update project description automatically inside output group
 
 positional arguments:
   input_gitlab          # Input GitLab URL (default: https://gitlab.com)
   input_group           # Input GitLab group
   output_gitlab         # Output GitLab URL (default: https://gitlab.com)
@@ -71,14 +72,15 @@
 
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Dependencies
 
+- [colored](https://pypi.org/project/colored/): Terminal colors and styles
 - [python-gitlab](https://pypi.org/project/python-gitlab/): A python wrapper for the GitLab API
 - [setuptools](https://pypi.org/project/setuptools/): Build and manage Python packages
 
 ---
 
 ## References
```

### Comparing `gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/cli/main.py` & `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from os import environ
 from sys import exit as sys_exit
 
 # Components
 from ..features.migration import MigrationFeature
 from ..package.bundle import Bundle
 from ..package.version import Version
+from ..prints.colors import Colors
 from ..system.platform import Platform
 
 # Main
 def main() -> None:
 
     # Variables
     group: _ArgumentGroup
@@ -59,14 +60,20 @@
     group.add_argument(
         '--keep-members',
         dest='keep_members',
         action='store_true',
         help='Keep input members after importing on output GitLab',
     )
     group.add_argument(
+        '--overwrite',
+        dest='overwrite',
+        action='store_true',
+        help='Overwrite existing projects on output GitLab',
+    )
+    group.add_argument(
         '--set-avatar',
         dest='set_avatar',
         action='store',
         metavar='FILE',
         help='Set imported projects\' avatar to a specific image file',
     )
     group.add_argument(
@@ -113,14 +120,17 @@
     if options.help:
         print(' ')
         parser.print_help()
         print(' ')
         Platform.flush()
         sys_exit(0)
 
+    # Prepare colors
+    Colors.prepare()
+
     # Version informations
     if options.version:
         print(
             f'{Bundle.NAME} {Version.get()} from {Version.path()} (python {Version.python()})'
         )
         Platform.flush()
         sys_exit(0)
```

### Comparing `gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/features/gitlab.py` & `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/features/gitlab.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from os.path import join
 from shutil import make_archive, unpack_archive
 from tempfile import TemporaryDirectory
 from time import sleep
 
 # Modules libraries
 from gitlab import Gitlab
+from gitlab.exceptions import GitlabGetError
 from gitlab.v4.objects import Group, Project
 
 # GitLabFeature class
 class GitLabFeature:
 
     # Members
     __gitlab: Gitlab
@@ -26,14 +27,22 @@
     def group(self, criteria: str) -> Group:
         return self.__gitlab.groups.get(criteria)
 
     # Project
     def project(self, criteria: str) -> Project:
         return self.__gitlab.projects.get(criteria)
 
+    # Project delete
+    def project_delete(self, criteria: str) -> None:
+        try:
+            self.project(criteria).delete()
+            sleep(5)
+        except GitlabGetError:
+            pass
+
     # Project export
     def project_export(self, archive: str, criteria: str,
                        keep_members: bool = False) -> None:
 
         # Create project export
         project = self.project(criteria)
         project_export = project.exports.create()
@@ -57,23 +66,30 @@
                 if stem.endswith('.tar.gz'):
                     stem = stem[:-len('.tar.gz')]
                 unpack_archive(archive, temp_directory, 'gztar')
                 remove(join(temp_directory, 'tree', 'project', 'project_members.ndjson'))
                 remove(archive)
                 make_archive(stem, 'gztar', temp_directory)
 
-    # Project import
-    def project_import(self, archive: str, group: str, path: str, name: str) -> Project:
+    # Project import, pylint: disable=too-many-arguments
+    def project_import(
+        self,
+        archive: str,
+        group: str,
+        path: str,
+        name: str,
+        overwrite: bool = False,
+    ) -> Project:
         with open(archive, 'rb') as file:
             project_imported = self.__gitlab.projects.import_project(
                 file,
                 path=path,
                 name=name,
                 namespace=group,
-                overwrite=False,
+                overwrite=overwrite,
             )
 
         # Upload project import
         project_import = self.__gitlab.projects.get(project_imported['id'],
                                                     lazy=True).imports.get()
         while project_import.import_status not in ['finished', 'failed']:
             sleep(1)
```

### Comparing `gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/package/version.py` & `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.0.0/gitlab_projects_migrate/system/platform.py` & `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate/system/platform.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_migrate-1.0.0/gitlab_projects_migrate.egg-info/PKG-INFO` & `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-migrate
-Version: 1.0.0
+Version: 1.1.0
 Summary: Migrate GitLab projects from a GitLab group to another GitLab's group
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-migrate
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-migrate/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-migrate/blob/main/CHANGELOG.md
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colored>=1.4.2
 Requires-Dist: python-gitlab>=4.4.0
 Requires-Dist: setuptools>=45.1.0
 
 # gitlab-projects-migrate
 
 <!-- markdownlint-disable no-inline-html -->
 
@@ -74,28 +75,29 @@
 ---
 
 ## Usage
 
 <!-- prettier-ignore-start -->
 
 ```yaml
-usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--keep-members]
+usage: gitlab-projects-migrate [-h] [--version] [-I INPUT_TOKEN] [-O OUTPUT_TOKEN] [--keep-members] [--overwrite]
                                [--set-avatar FILE] [--update-description]
                                [input_gitlab] [input_group] [output_gitlab] [output_group]
 
 gitlab-projects-migrate: Synchronize projects from a GitLab group to another GitLab group
 
 internal arguments:
   -h, --help            # Show this help message
   --version             # Show the current version
 
 migration arguments:
   -I INPUT_TOKEN        # Input GitLab API token (default: GITLAB_INPUT_TOKEN environment)
   -O OUTPUT_TOKEN       # Output GitLab API token (default: GITLAB_OUTPUT_TOKEN environment or input_token)
   --keep-members        # Keep input members after importing on output GitLab
+  --overwrite           # Overwrite existing projects on output GitLab
   --set-avatar FILE     # Set imported projects' avatar to a specific image file
   --update-description  # Update project description automatically inside output group
 
 positional arguments:
   input_gitlab          # Input GitLab URL (default: https://gitlab.com)
   input_group           # Input GitLab group
   output_gitlab         # Output GitLab URL (default: https://gitlab.com)
@@ -104,14 +106,15 @@
 
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Dependencies
 
+- [colored](https://pypi.org/project/colored/): Terminal colors and styles
 - [python-gitlab](https://pypi.org/project/python-gitlab/): A python wrapper for the GitLab API
 - [setuptools](https://pypi.org/project/setuptools/): Build and manage Python packages
 
 ---
 
 ## References
```

### Comparing `gitlab_projects_migrate-1.0.0/gitlab_projects_migrate.egg-info/SOURCES.txt` & `gitlab_projects_migrate-1.1.0/gitlab_projects_migrate.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,13 +24,15 @@
 gitlab_projects_migrate/cli/main.py
 gitlab_projects_migrate/features/__init__.py
 gitlab_projects_migrate/features/gitlab.py
 gitlab_projects_migrate/features/migration.py
 gitlab_projects_migrate/package/__init__.py
 gitlab_projects_migrate/package/bundle.py
 gitlab_projects_migrate/package/version.py
+gitlab_projects_migrate/prints/__init__.py
+gitlab_projects_migrate/prints/colors.py
 gitlab_projects_migrate/system/__init__.py
 gitlab_projects_migrate/system/platform.py
 requirements/build.txt
 requirements/deploy.txt
 requirements/quality.txt
 requirements/runtime.txt
```

### Comparing `gitlab_projects_migrate-1.0.0/setup.py` & `gitlab_projects_migrate-1.1.0/setup.py`

 * *Files identical despite different names*

