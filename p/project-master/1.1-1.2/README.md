# Comparing `tmp/project_master-1.1.tar.gz` & `tmp/project_master-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_master-1.1.tar", last modified: Mon Apr 22 09:25:42 2024, max compression
+gzip compressed data, was "project_master-1.2.tar", last modified: Mon Apr 22 09:27:55 2024, max compression
```

## Comparing `project_master-1.1.tar` & `project_master-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 09:25:42.519457 project_master-1.1/
--rw-rw-rw-   0        0        0     1515 2024-04-22 09:11:27.000000 project_master-1.1/LICENSE
--rw-rw-rw-   0        0        0     3141 2024-04-22 09:25:42.518427 project_master-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2332 2024-04-22 09:20:46.000000 project_master-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 09:25:42.501976 project_master-1.1/project_master/
--rw-rw-rw-   0        0        0       23 2024-04-22 09:11:27.000000 project_master-1.1/project_master/__init__.py
--rw-rw-rw-   0        0        0     2028 2024-04-22 09:20:46.000000 project_master-1.1/project_master/core.py
--rw-rw-rw-   0        0        0     2499 2024-04-22 09:11:27.000000 project_master-1.1/project_master/file_content.py
--rw-rw-rw-   0        0        0     1102 2024-04-22 09:23:42.000000 project_master-1.1/project_master/main.py
-drwxrwxrwx   0        0        0        0 2024-04-22 09:25:42.517421 project_master-1.1/project_master.egg-info/
--rw-rw-rw-   0        0        0     3141 2024-04-22 09:25:42.000000 project_master-1.1/project_master.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-04-22 09:25:42.000000 project_master-1.1/project_master.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 09:25:42.000000 project_master-1.1/project_master.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-22 09:25:42.000000 project_master-1.1/project_master.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 09:25:42.519457 project_master-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1078 2024-04-22 09:25:32.000000 project_master-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:27:55.422785 project_master-1.2/
+-rw-rw-rw-   0        0        0     1515 2024-04-22 09:11:27.000000 project_master-1.2/LICENSE
+-rw-rw-rw-   0        0        0     3141 2024-04-22 09:27:55.421786 project_master-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2332 2024-04-22 09:20:46.000000 project_master-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 09:27:55.409785 project_master-1.2/project_master/
+-rw-rw-rw-   0        0        0       23 2024-04-22 09:11:27.000000 project_master-1.2/project_master/__init__.py
+-rw-rw-rw-   0        0        0     2014 2024-04-22 09:27:51.000000 project_master-1.2/project_master/core.py
+-rw-rw-rw-   0        0        0     2499 2024-04-22 09:11:27.000000 project_master-1.2/project_master/file_content.py
+-rw-rw-rw-   0        0        0     1104 2024-04-22 09:27:51.000000 project_master-1.2/project_master/main.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:27:55.420786 project_master-1.2/project_master.egg-info/
+-rw-rw-rw-   0        0        0     3141 2024-04-22 09:27:55.000000 project_master-1.2/project_master.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-04-22 09:27:55.000000 project_master-1.2/project_master.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 09:27:55.000000 project_master-1.2/project_master.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-22 09:27:55.000000 project_master-1.2/project_master.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 09:27:55.422785 project_master-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1078 2024-04-22 09:27:51.000000 project_master-1.2/setup.py
```

### Comparing `project_master-1.1/LICENSE` & `project_master-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `project_master-1.1/PKG-INFO` & `project_master-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project_master
-Version: 1.1
+Version: 1.2
 Summary: This Python script generates a standardized project structure for your Python projects. It creates the necessary folders and files based on your specifications.
 Home-page: https://github.com/Armen-Jean-Andreasian
 Author: Armen-Jean Andreasian
 Author-email: armen_andreasian@proton.me
 License: BSD
 Keywords: project,directory,python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `project_master-1.1/README.md` & `project_master-1.2/README.md`

 * *Files identical despite different names*

### Comparing `project_master-1.1/project_master/core.py` & `project_master-1.2/project_master/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-from project_master.file_content import get_readme_content, get_gitignore_content, get_licence_content
 from datetime import datetime
+from .file_content import get_readme_content, get_gitignore_content, get_licence_content
 
 
 class ProjectStructureGenerator:
     folders = ['dev', 'src', 'tests', 'utils']
     files = ['requirements.txt', 'README.md', 'LICENSE', '.gitignore']
 
     _folders_pro = ['docs', 'data', 'config', 'logs']
```

### Comparing `project_master-1.1/project_master/file_content.py` & `project_master-1.2/project_master/file_content.py`

 * *Files identical despite different names*

### Comparing `project_master-1.1/project_master/main.py` & `project_master-1.2/project_master/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src import ProjectStructureGenerator
+from .core import ProjectStructureGenerator
 
 
 class Cat:
     @staticmethod
     def build_structure(project_name: str, developer_name: str, pro_mode=False):
         """
         Builds project structure.
```

### Comparing `project_master-1.1/project_master.egg-info/PKG-INFO` & `project_master-1.2/project_master.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-master
-Version: 1.1
+Version: 1.2
 Summary: This Python script generates a standardized project structure for your Python projects. It creates the necessary folders and files based on your specifications.
 Home-page: https://github.com/Armen-Jean-Andreasian
 Author: Armen-Jean Andreasian
 Author-email: armen_andreasian@proton.me
 License: BSD
 Keywords: project,directory,python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `project_master-1.1/setup.py` & `project_master-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='project_master',
     packages=['project_master'],
-    version='1.1',
+    version='1.2',
     license='BSD',
 
     description='This Python script generates a standardized project structure for your Python projects. It creates the necessary folders and files based on your specifications.',
 
     author='Armen-Jean Andreasian',
     author_email='armen_andreasian@proton.me',
```

