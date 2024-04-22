# Comparing `tmp/jarguments-0.0.1.tar.gz` & `tmp/jarguments-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarguments-0.0.1.tar", last modified: Wed Jan 24 23:13:34 2024, max compression
+gzip compressed data, was "jarguments-0.1.0.tar", last modified: Mon Apr 22 05:09:58 2024, max compression
```

## Comparing `jarguments-0.0.1.tar` & `jarguments-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:13:34.970670 jarguments-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-24 23:13:24.000000 jarguments-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-01-24 23:13:34.970670 jarguments-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-01-24 23:13:24.000000 jarguments-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:13:34.966670 jarguments-0.0.1/jarguments/
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-01-24 23:13:24.000000 jarguments-0.0.1/jarguments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:13:34.970670 jarguments-0.0.1/jarguments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-01-24 23:13:34.000000 jarguments-0.0.1/jarguments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-24 23:13:34.000000 jarguments-0.0.1/jarguments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 23:13:34.000000 jarguments-0.0.1/jarguments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-24 23:13:34.000000 jarguments-0.0.1/jarguments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 23:13:34.000000 jarguments-0.0.1/jarguments.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 23:13:34.970670 jarguments-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-24 23:13:24.000000 jarguments-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:09:58.966656 jarguments-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 05:09:53.000000 jarguments-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-22 05:09:58.966656 jarguments-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-22 05:09:53.000000 jarguments-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:09:58.962656 jarguments-0.1.0/jarguments/
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-22 05:09:53.000000 jarguments-0.1.0/jarguments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 05:09:58.966656 jarguments-0.1.0/jarguments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-22 05:09:58.000000 jarguments-0.1.0/jarguments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-22 05:09:58.000000 jarguments-0.1.0/jarguments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:09:58.000000 jarguments-0.1.0/jarguments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 05:09:58.000000 jarguments-0.1.0/jarguments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 05:09:58.000000 jarguments-0.1.0/jarguments.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 05:09:58.966656 jarguments-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-22 05:09:53.000000 jarguments-0.1.0/setup.py
```

### Comparing `jarguments-0.0.1/LICENSE` & `jarguments-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jarguments-0.0.1/PKG-INFO` & `jarguments-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,13 @@
-Metadata-Version: 2.1
-Name: jarguments
-Version: 0.0.1
-Summary: Providing a straightforward way to create command-line arguments.
-Home-page: https://github.com/silvncr/jarguments
-Author: silvncr
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- omit from toc -->
 # jarguments
 
 simplifying args jargon
 
+![[license](LICENSE)](https://img.shields.io/github/license/silvncr/jarguments)
 ![[publish status](https://github.com/silvncr/jarguments/actions/workflows/python-publish.yml)](https://img.shields.io/github/actions/workflow/status/silvncr/jarguments/python-publish.yml)
 ![[latest release](https://github.com/silvncr/jarguments/releases/latest)](https://img.shields.io/github/v/release/silvncr/jarguments)
 
 ## Summary
 
 Providing a straightforward way to create command-line arguments.
 
@@ -35,68 +21,69 @@
 - [Usage](#usage)
   - [Library](#library)
   - [Command-line](#command-line)
 
 ## Installation
 
 ```sh
-git clone https://github.com/silvncr/jarguments.git
-cd jarguments
-python setup.py install
+pip install jarguments
 ```
 
 ## Usage
 
 ### Library
 
 There are three steps to using the jarguments library:
 
 1. Import the jarguments library.
 
     ```py
-    from jarguments import *
+    import jarguments as j
     ```
 
 2. Provide your arguments with jarguments' classes.
 
     ```py
-    args = JParser(
-      JBool('show_text', help='determines whether "text" is shown'),
-      JStr('text'),
+    args = j.JParser(
+      j.JBool('show-text', help='determines whether "text" is shown'),
+      j.JInt('number', default=1),
+      j.JArgument('text', type=str, multiple=True),
     )
     ```
 
-3. Use your outputs; they are parsed automatically.
+3. Use the outputs; they're parsed automatically!
 
     ```py
     if args.show_text:
-      print(args.text)
+      for _ in range(args.number):
+        print(args.text)
     ```
 
 ### Command-line
 
 - Now you can run your script with arguments:
 
     ```sh
-    $ python script.py --show_text --text "hello world"
-    hello world
+    $ python example.py --show-text --text "hello" "world"
+    ["hello", "world"]
     ```
 
 - Arguments without a default value are required. If you don't provide them, the script will raise an error:
 
     ```sh
-    $ python script.py --show_text
+    $ python example.py --show-text
     error: the following arguments are required: --text
     ```
 
 - If you want to see help messages, run your script with the `-h` or `--help` flag:
 
     ```sh
-    $ python script.py -h
-    usage: script.py [-h] [--show_text] --text TEXT
+    $ python example.py -h
+    usage: example.py [-h] [--show-text [SHOW_TEXT]] [--number NUMBER] --text [TEXT ...]
 
     options:
-      -h, --help            show this help message and exit   
-      --show_text [SHOW_TEXT]
+      -h, --help            show this help message and exit
+      --show-text [SHOW_TEXT]
                             determines whether "text" is shown
-      --text TEXT
+      --number NUMBER
+      --text [TEXT ...]
     ```
```

### Comparing `jarguments-0.0.1/jarguments.egg-info/PKG-INFO` & `jarguments-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarguments
-Version: 0.0.1
+Version: 0.1.0
 Summary: Providing a straightforward way to create command-line arguments.
 Home-page: https://github.com/silvncr/jarguments
 Author: silvncr
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
@@ -14,14 +14,15 @@
 License-File: LICENSE
 
 <!-- omit from toc -->
 # jarguments
 
 simplifying args jargon
 
+![[license](LICENSE)](https://img.shields.io/github/license/silvncr/jarguments)
 ![[publish status](https://github.com/silvncr/jarguments/actions/workflows/python-publish.yml)](https://img.shields.io/github/actions/workflow/status/silvncr/jarguments/python-publish.yml)
 ![[latest release](https://github.com/silvncr/jarguments/releases/latest)](https://img.shields.io/github/v/release/silvncr/jarguments)
 
 ## Summary
 
 Providing a straightforward way to create command-line arguments.
 
@@ -35,68 +36,69 @@
 - [Usage](#usage)
   - [Library](#library)
   - [Command-line](#command-line)
 
 ## Installation
 
 ```sh
-git clone https://github.com/silvncr/jarguments.git
-cd jarguments
-python setup.py install
+pip install jarguments
 ```
 
 ## Usage
 
 ### Library
 
 There are three steps to using the jarguments library:
 
 1. Import the jarguments library.
 
     ```py
-    from jarguments import *
+    import jarguments as j
     ```
 
 2. Provide your arguments with jarguments' classes.
 
     ```py
-    args = JParser(
-      JBool('show_text', help='determines whether "text" is shown'),
-      JStr('text'),
+    args = j.JParser(
+      j.JBool('show-text', help='determines whether "text" is shown'),
+      j.JInt('number', default=1),
+      j.JArgument('text', type=str, multiple=True),
     )
     ```
 
-3. Use your outputs; they are parsed automatically.
+3. Use the outputs; they're parsed automatically!
 
     ```py
     if args.show_text:
-      print(args.text)
+      for _ in range(args.number):
+        print(args.text)
     ```
 
 ### Command-line
 
 - Now you can run your script with arguments:
 
     ```sh
-    $ python script.py --show_text --text "hello world"
-    hello world
+    $ python example.py --show-text --text "hello" "world"
+    ["hello", "world"]
     ```
 
 - Arguments without a default value are required. If you don't provide them, the script will raise an error:
 
     ```sh
-    $ python script.py --show_text
+    $ python example.py --show-text
     error: the following arguments are required: --text
     ```
 
 - If you want to see help messages, run your script with the `-h` or `--help` flag:
 
     ```sh
-    $ python script.py -h
-    usage: script.py [-h] [--show_text] --text TEXT
+    $ python example.py -h
+    usage: example.py [-h] [--show-text [SHOW_TEXT]] [--number NUMBER] --text [TEXT ...]
 
     options:
-      -h, --help            show this help message and exit   
-      --show_text [SHOW_TEXT]
+      -h, --help            show this help message and exit
+      --show-text [SHOW_TEXT]
                             determines whether "text" is shown
-      --text TEXT
+      --number NUMBER
+      --text [TEXT ...]
     ```
```

### Comparing `jarguments-0.0.1/setup.py` & `jarguments-0.1.0/setup.py`

 * *Files identical despite different names*

