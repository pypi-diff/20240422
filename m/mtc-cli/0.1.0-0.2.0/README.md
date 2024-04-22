# Comparing `tmp/mtc-cli-0.1.0.tar.gz` & `tmp/mtc_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtc-cli-0.1.0.tar", last modified: Thu Nov 30 23:05:23 2023, max compression
+gzip compressed data, was "mtc_cli-0.2.0.tar", last modified: Mon Apr 22 08:49:56 2024, max compression
```

## Comparing `mtc-cli-0.1.0.tar` & `mtc_cli-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-11-30 23:05:23.616567 mtc-cli-0.1.0/
--rw-r--r--   0 alec       (501) staff       (20)    34913 2021-05-27 22:14:13.000000 mtc-cli-0.1.0/LICENSE.md
--rw-r--r--   0 alec       (501) staff       (20)       13 2021-05-27 22:14:13.000000 mtc-cli-0.1.0/MANIFEST.in
--rw-r--r--   0 alec       (501) staff       (20)     1921 2023-11-30 23:05:23.616387 mtc-cli-0.1.0/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)     1255 2023-11-29 04:55:39.000000 mtc-cli-0.1.0/README.md
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-11-30 23:05:23.615120 mtc-cli-0.1.0/mtc/
--rw-r--r--   0 alec       (501) staff       (20)        0 2021-05-27 22:14:13.000000 mtc-cli-0.1.0/mtc/__init__.py
--rw-r--r--   0 alec       (501) staff       (20)    11060 2023-11-29 04:56:08.000000 mtc-cli-0.1.0/mtc/__main__.py
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-11-30 23:05:23.616213 mtc-cli-0.1.0/mtc_cli.egg-info/
--rw-r--r--   0 alec       (501) staff       (20)     1921 2023-11-30 23:05:23.000000 mtc-cli-0.1.0/mtc_cli.egg-info/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)      276 2023-11-30 23:05:23.000000 mtc-cli-0.1.0/mtc_cli.egg-info/SOURCES.txt
--rw-r--r--   0 alec       (501) staff       (20)        1 2023-11-30 23:05:23.000000 mtc-cli-0.1.0/mtc_cli.egg-info/dependency_links.txt
--rw-r--r--   0 alec       (501) staff       (20)       43 2023-11-30 23:05:23.000000 mtc-cli-0.1.0/mtc_cli.egg-info/entry_points.txt
--rw-r--r--   0 alec       (501) staff       (20)       11 2023-11-30 23:05:23.000000 mtc-cli-0.1.0/mtc_cli.egg-info/requires.txt
--rw-r--r--   0 alec       (501) staff       (20)        4 2023-11-30 23:05:23.000000 mtc-cli-0.1.0/mtc_cli.egg-info/top_level.txt
--rw-r--r--   0 alec       (501) staff       (20)      103 2021-05-27 22:14:13.000000 mtc-cli-0.1.0/pyproject.toml
--rw-r--r--   0 alec       (501) staff       (20)       38 2023-11-30 23:05:23.616607 mtc-cli-0.1.0/setup.cfg
--rw-r--r--   0 alec       (501) staff       (20)     1062 2023-11-30 23:03:36.000000 mtc-cli-0.1.0/setup.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-04-22 08:49:56.078184 mtc_cli-0.2.0/
+-rw-r--r--   0 alec       (501) staff       (20)    34913 2023-07-14 22:15:14.000000 mtc_cli-0.2.0/LICENSE.md
+-rw-r--r--   0 alec       (501) staff       (20)       13 2023-07-14 22:15:14.000000 mtc_cli-0.2.0/MANIFEST.in
+-rw-r--r--   0 alec       (501) staff       (20)     2026 2024-04-22 08:49:56.077993 mtc_cli-0.2.0/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)     1343 2024-04-21 01:48:56.000000 mtc_cli-0.2.0/README.md
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-04-22 08:49:56.076993 mtc_cli-0.2.0/mtc_cli/
+-rw-r--r--   0 alec       (501) staff       (20)        0 2023-07-14 22:15:14.000000 mtc_cli-0.2.0/mtc_cli/__init__.py
+-rw-r--r--   0 alec       (501) staff       (20)     2862 2024-04-18 00:42:00.000000 mtc_cli-0.2.0/mtc_cli/__main__.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-04-22 08:49:56.077778 mtc_cli-0.2.0/mtc_cli.egg-info/
+-rw-r--r--   0 alec       (501) staff       (20)     2026 2024-04-22 08:49:56.000000 mtc_cli-0.2.0/mtc_cli.egg-info/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)      284 2024-04-22 08:49:56.000000 mtc_cli-0.2.0/mtc_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 alec       (501) staff       (20)        1 2024-04-22 08:49:56.000000 mtc_cli-0.2.0/mtc_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 alec       (501) staff       (20)       51 2024-04-22 08:49:56.000000 mtc_cli-0.2.0/mtc_cli.egg-info/entry_points.txt
+-rw-r--r--   0 alec       (501) staff       (20)       11 2024-04-22 08:49:56.000000 mtc_cli-0.2.0/mtc_cli.egg-info/requires.txt
+-rw-r--r--   0 alec       (501) staff       (20)        8 2024-04-22 08:49:56.000000 mtc_cli-0.2.0/mtc_cli.egg-info/top_level.txt
+-rw-r--r--   0 alec       (501) staff       (20)      103 2023-07-14 22:15:14.000000 mtc_cli-0.2.0/pyproject.toml
+-rw-r--r--   0 alec       (501) staff       (20)       38 2024-04-22 08:49:56.078228 mtc_cli-0.2.0/setup.cfg
+-rw-r--r--   0 alec       (501) staff       (20)     1079 2024-04-22 04:32:57.000000 mtc_cli-0.2.0/setup.py
```

### Comparing `mtc-cli-0.1.0/LICENSE.md` & `mtc_cli-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mtc-cli-0.1.0/PKG-INFO` & `mtc_cli-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: mtc-cli
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple CLI tool for moving enwp files to Commons
 Home-page: https://github.com/fastily/mtc-cli
 Author: Fastily
 Author-email: fastily@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/fastily/mtc-cli/issues
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: fastilybot
+Requires-Dist: pwiki
+Requires-Dist: rich
 
 # mtc-cli
-[![Python 3.9+](https://upload.wikimedia.org/wikipedia/commons/4/4f/Blue_Python_3.9%2B_Shield_Badge.svg)](https://www.python.org)
+[![Python 3.12+](https://upload.wikimedia.org/wikipedia/commons/5/50/Blue_Python_3.12%2B_Shield_Badge.svg)](https://www.python.org)
 [![MediaWiki 1.35+](https://upload.wikimedia.org/wikipedia/commons/b/b3/Blue_MediaWiki_1.35%2B_Shield_Badge.svg)](https://www.mediawiki.org/wiki/MediaWiki)
 [![License: GPL v3](https://upload.wikimedia.org/wikipedia/commons/8/86/GPL_v3_Blue_Badge.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)
 
 mtc-cli is a command line tool that helps simplify and automate file imports from Wikipedia to Commons.
 
 This is the rewritten, spiritual successor to the original [MTC!](https://github.com/fastily/mtc) tool.
 
 ### Install
 ```bash
 pip install mtc-cli
 ```
 
 ### Usage
 ```
-usage: __main__.py [-h] [-u username] [-f] [-d] [-t] [titles ...]
+usage: __main__.py [-h] [-u username] [-f] [-d] [-a api_endpoint] [titles ...]
 
 mtc CLI
 
 positional arguments:
-  titles       Files, usernames, templates, or categories
+  titles           Files, usernames, templates, or categories
 
 options:
-  -h, --help   show this help message and exit
-  -u username  the username to use
-  -f           Force (ignore filter) file transfer(s)
-  -d           Activate dry run/debug mode (does not transfer files)
-  -t           Add a Now Commons tag to the enwp file
+  -h, --help       show this help message and exit
+  -u username      the username to use
+  -f               Force (ignore filter) file transfer(s)
+  -d               Activate dry run/debug mode (does not transfer files)
+  -a api_endpoint  The default desc generation API endpoint to use. Defaults to public toolforge instance.
 ```
 
 👉 Password is set via env variable `<USERNAME>_PW`, such that `<USERNAME>` is the username of the bot in all caps.
```

### Comparing `mtc-cli-0.1.0/README.md` & `mtc_cli-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # mtc-cli
-[![Python 3.9+](https://upload.wikimedia.org/wikipedia/commons/4/4f/Blue_Python_3.9%2B_Shield_Badge.svg)](https://www.python.org)
+[![Python 3.12+](https://upload.wikimedia.org/wikipedia/commons/5/50/Blue_Python_3.12%2B_Shield_Badge.svg)](https://www.python.org)
 [![MediaWiki 1.35+](https://upload.wikimedia.org/wikipedia/commons/b/b3/Blue_MediaWiki_1.35%2B_Shield_Badge.svg)](https://www.mediawiki.org/wiki/MediaWiki)
 [![License: GPL v3](https://upload.wikimedia.org/wikipedia/commons/8/86/GPL_v3_Blue_Badge.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)
 
 mtc-cli is a command line tool that helps simplify and automate file imports from Wikipedia to Commons.
 
 This is the rewritten, spiritual successor to the original [MTC!](https://github.com/fastily/mtc) tool.
 
 ### Install
 ```bash
 pip install mtc-cli
 ```
 
 ### Usage
 ```
-usage: __main__.py [-h] [-u username] [-f] [-d] [-t] [titles ...]
+usage: __main__.py [-h] [-u username] [-f] [-d] [-a api_endpoint] [titles ...]
 
 mtc CLI
 
 positional arguments:
-  titles       Files, usernames, templates, or categories
+  titles           Files, usernames, templates, or categories
 
 options:
-  -h, --help   show this help message and exit
-  -u username  the username to use
-  -f           Force (ignore filter) file transfer(s)
-  -d           Activate dry run/debug mode (does not transfer files)
-  -t           Add a Now Commons tag to the enwp file
+  -h, --help       show this help message and exit
+  -u username      the username to use
+  -f               Force (ignore filter) file transfer(s)
+  -d               Activate dry run/debug mode (does not transfer files)
+  -a api_endpoint  The default desc generation API endpoint to use. Defaults to public toolforge instance.
 ```
 
 👉 Password is set via env variable `<USERNAME>_PW`, such that `<USERNAME>` is the username of the bot in all caps.
```

### Comparing `mtc-cli-0.1.0/mtc_cli.egg-info/PKG-INFO` & `mtc_cli-0.2.0/mtc_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: mtc-cli
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple CLI tool for moving enwp files to Commons
 Home-page: https://github.com/fastily/mtc-cli
 Author: Fastily
 Author-email: fastily@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/fastily/mtc-cli/issues
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: fastilybot
+Requires-Dist: pwiki
+Requires-Dist: rich
 
 # mtc-cli
-[![Python 3.9+](https://upload.wikimedia.org/wikipedia/commons/4/4f/Blue_Python_3.9%2B_Shield_Badge.svg)](https://www.python.org)
+[![Python 3.12+](https://upload.wikimedia.org/wikipedia/commons/5/50/Blue_Python_3.12%2B_Shield_Badge.svg)](https://www.python.org)
 [![MediaWiki 1.35+](https://upload.wikimedia.org/wikipedia/commons/b/b3/Blue_MediaWiki_1.35%2B_Shield_Badge.svg)](https://www.mediawiki.org/wiki/MediaWiki)
 [![License: GPL v3](https://upload.wikimedia.org/wikipedia/commons/8/86/GPL_v3_Blue_Badge.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)
 
 mtc-cli is a command line tool that helps simplify and automate file imports from Wikipedia to Commons.
 
 This is the rewritten, spiritual successor to the original [MTC!](https://github.com/fastily/mtc) tool.
 
 ### Install
 ```bash
 pip install mtc-cli
 ```
 
 ### Usage
 ```
-usage: __main__.py [-h] [-u username] [-f] [-d] [-t] [titles ...]
+usage: __main__.py [-h] [-u username] [-f] [-d] [-a api_endpoint] [titles ...]
 
 mtc CLI
 
 positional arguments:
-  titles       Files, usernames, templates, or categories
+  titles           Files, usernames, templates, or categories
 
 options:
-  -h, --help   show this help message and exit
-  -u username  the username to use
-  -f           Force (ignore filter) file transfer(s)
-  -d           Activate dry run/debug mode (does not transfer files)
-  -t           Add a Now Commons tag to the enwp file
+  -h, --help       show this help message and exit
+  -u username      the username to use
+  -f               Force (ignore filter) file transfer(s)
+  -d               Activate dry run/debug mode (does not transfer files)
+  -a api_endpoint  The default desc generation API endpoint to use. Defaults to public toolforge instance.
 ```
 
 👉 Password is set via env variable `<USERNAME>_PW`, such that `<USERNAME>` is the username of the bot in all caps.
```

