# Comparing `tmp/report_creator-1.0.7.tar.gz` & `tmp/report_creator-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report_creator-1.0.7.tar", last modified: Sun Apr 21 23:57:03 2024, max compression
+gzip compressed data, was "report_creator-1.0.8.tar", last modified: Mon Apr 22 00:01:39 2024, max compression
```

## Comparing `report_creator-1.0.7.tar` & `report_creator-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-21 23:57:03.469687 report_creator-1.0.7/
--rw-r--r--   0 drace      (501) staff       (20)     1066 2024-04-20 05:46:16.000000 report_creator-1.0.7/LICENSE
--rw-r--r--   0 drace      (501) staff       (20)       69 2024-04-19 02:06:16.000000 report_creator-1.0.7/MANIFEST.in
--rw-r--r--   0 drace      (501) staff       (20)     4124 2024-04-21 23:57:03.469635 report_creator-1.0.7/PKG-INFO
--rw-r--r--   0 drace      (501) staff       (20)     3300 2024-04-20 05:46:16.000000 report_creator-1.0.7/README.md
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-21 23:57:03.468551 report_creator-1.0.7/report_creator/
--rw-r--r--   0 drace      (501) staff       (20)      478 2024-04-19 02:06:16.000000 report_creator-1.0.7/report_creator/__init__.py
--rw-r--r--   0 drace      (501) staff       (20)      174 2024-04-21 23:56:35.000000 report_creator-1.0.7/report_creator/__meta__.py
--rw-r--r--   0 drace      (501) staff       (20)    45428 2024-04-19 02:06:16.000000 report_creator-1.0.7/report_creator/report_creator.py
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-21 23:57:03.469147 report_creator-1.0.7/report_creator/templates/
--rw-r--r--   0 drace      (501) staff       (20)    10528 2024-04-19 02:06:16.000000 report_creator-1.0.7/report_creator/templates/default.html
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-21 23:57:03.469458 report_creator-1.0.7/report_creator.egg-info/
--rw-r--r--   0 drace      (501) staff       (20)     4124 2024-04-21 23:57:03.000000 report_creator-1.0.7/report_creator.egg-info/PKG-INFO
--rw-r--r--   0 drace      (501) staff       (20)      325 2024-04-21 23:57:03.000000 report_creator-1.0.7/report_creator.egg-info/SOURCES.txt
--rw-r--r--   0 drace      (501) staff       (20)        1 2024-04-21 23:57:03.000000 report_creator-1.0.7/report_creator.egg-info/dependency_links.txt
--rw-r--r--   0 drace      (501) staff       (20)       15 2024-04-21 23:57:03.000000 report_creator-1.0.7/report_creator.egg-info/top_level.txt
--rw-r--r--   0 drace      (501) staff       (20)     1079 2024-04-21 23:57:03.469910 report_creator-1.0.7/setup.cfg
--rw-r--r--   0 drace      (501) staff       (20)     1701 2024-04-21 23:57:00.000000 report_creator-1.0.7/setup.py
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:01:39.161110 report_creator-1.0.8/
+-rw-r--r--   0 drace      (501) staff       (20)     1066 2024-04-20 05:46:16.000000 report_creator-1.0.8/LICENSE
+-rw-r--r--   0 drace      (501) staff       (20)       69 2024-04-19 02:06:16.000000 report_creator-1.0.8/MANIFEST.in
+-rw-r--r--   0 drace      (501) staff       (20)     4406 2024-04-22 00:01:39.161050 report_creator-1.0.8/PKG-INFO
+-rw-r--r--   0 drace      (501) staff       (20)     3300 2024-04-20 05:46:16.000000 report_creator-1.0.8/README.md
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:01:39.159828 report_creator-1.0.8/report_creator/
+-rw-r--r--   0 drace      (501) staff       (20)      478 2024-04-19 02:06:16.000000 report_creator-1.0.8/report_creator/__init__.py
+-rw-r--r--   0 drace      (501) staff       (20)      174 2024-04-22 00:01:33.000000 report_creator-1.0.8/report_creator/__meta__.py
+-rw-r--r--   0 drace      (501) staff       (20)    45428 2024-04-19 02:06:16.000000 report_creator-1.0.8/report_creator/report_creator.py
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:01:39.160540 report_creator-1.0.8/report_creator/templates/
+-rw-r--r--   0 drace      (501) staff       (20)    10528 2024-04-19 02:06:16.000000 report_creator-1.0.8/report_creator/templates/default.html
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-22 00:01:39.160850 report_creator-1.0.8/report_creator.egg-info/
+-rw-r--r--   0 drace      (501) staff       (20)     4406 2024-04-22 00:01:39.000000 report_creator-1.0.8/report_creator.egg-info/PKG-INFO
+-rw-r--r--   0 drace      (501) staff       (20)      362 2024-04-22 00:01:39.000000 report_creator-1.0.8/report_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 drace      (501) staff       (20)        1 2024-04-22 00:01:39.000000 report_creator-1.0.8/report_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 drace      (501) staff       (20)      102 2024-04-22 00:01:39.000000 report_creator-1.0.8/report_creator.egg-info/requires.txt
+-rw-r--r--   0 drace      (501) staff       (20)       15 2024-04-22 00:01:39.000000 report_creator-1.0.8/report_creator.egg-info/top_level.txt
+-rw-r--r--   0 drace      (501) staff       (20)     1079 2024-04-22 00:01:39.161353 report_creator-1.0.8/setup.cfg
+-rw-r--r--   0 drace      (501) staff       (20)     2113 2024-04-22 00:01:13.000000 report_creator-1.0.8/setup.py
```

### Comparing `report_creator-1.0.7/LICENSE` & `report_creator-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.7/PKG-INFO` & `report_creator-1.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report_creator
-Version: 1.0.7
+Version: 1.0.8
 Summary: Produce self-contained HTML reports from Python
 Home-page: https://github.com/darenr/report_creator
 Author: Daren Race
 Author-email: daren.race@gmail.com
 License: MIT
 Keywords: python,html,reports,report,creator,generator,markdown,yaml,plot,chart,table
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pip
+Requires-Dist: pandas
+Requires-Dist: pyarrow
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: mistune
+Requires-Dist: pyyaml
+Requires-Dist: plotly-express
+Requires-Dist: Jinja2
+Requires-Dist: humanize
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
 
 # Report Creator
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge)](https://www.apache.org/licenses/LICENSE-2.0)
 [![PyPI Version](https://img.shields.io/pypi/v/report_creator.svg?style=for-the-badge&color=blue)](https://pypi.org/project/report_creator)
 [![Python Versions](https://img.shields.io/pypi/pyversions/report_creator.svg?logo=python&logoColor=white&style=for-the-badge)](https://pypi.org/project/report_creator)
```

### Comparing `report_creator-1.0.7/README.md` & `report_creator-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.7/report_creator/report_creator.py` & `report_creator-1.0.8/report_creator/report_creator.py`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.7/report_creator/templates/default.html` & `report_creator-1.0.8/report_creator/templates/default.html`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.7/report_creator.egg-info/PKG-INFO` & `report_creator-1.0.8/report_creator.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report_creator
-Version: 1.0.7
+Version: 1.0.8
 Summary: Produce self-contained HTML reports from Python
 Home-page: https://github.com/darenr/report_creator
 Author: Daren Race
 Author-email: daren.race@gmail.com
 License: MIT
 Keywords: python,html,reports,report,creator,generator,markdown,yaml,plot,chart,table
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pip
+Requires-Dist: pandas
+Requires-Dist: pyarrow
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: mistune
+Requires-Dist: pyyaml
+Requires-Dist: plotly-express
+Requires-Dist: Jinja2
+Requires-Dist: humanize
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
 
 # Report Creator
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge)](https://www.apache.org/licenses/LICENSE-2.0)
 [![PyPI Version](https://img.shields.io/pypi/v/report_creator.svg?style=for-the-badge&color=blue)](https://pypi.org/project/report_creator)
 [![Python Versions](https://img.shields.io/pypi/pyversions/report_creator.svg?logo=python&logoColor=white&style=for-the-badge)](https://pypi.org/project/report_creator)
```

### Comparing `report_creator-1.0.7/setup.cfg` & `report_creator-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.7/setup.py` & `report_creator-1.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 """Build and installation script for report_creator."""
 
 # standard libs
 import re
+from pathlib import Path
+from typing import List
 
 from setuptools import find_packages, setup
 
 # get long description from README.rst
 with open("README.md") as readme:
     long_description = readme.read()
 
 
+# include necessary deopendencies
+def get_install_requires() -> List[str]:
+    """Returns requirements.txt parsed to a list"""
+    fname = Path(__file__).parent / "requirements.txt"
+    targets = []
+    if fname.exists():
+        with open(fname) as f:
+            targets = f.read().splitlines()
+    return targets
+
+
 # get package metadata by parsing __meta__ module
 with open("report_creator/__meta__.py") as source:
     content = source.read().strip()
     metadata = {
         key: re.search(key + r'\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
         for key in [
             "__version__",
@@ -35,14 +48,15 @@
     keywords="python, html, reports, report, creator, generator, markdown, yaml, plot, chart, table",
     url="https://github.com/darenr/report_creator",
     packages=find_packages(),
     include_package_data=True,
     package_data={"report_creator": ["templates/*"]},
     long_description=long_description,
     long_description_content_type="text/markdown",
+    install_requires=get_install_requires(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

