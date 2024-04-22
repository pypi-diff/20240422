# Comparing `tmp/spiderwebai-py-0.1.2.tar.gz` & `tmp/spiderwebai-py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiderwebai-py-0.1.2.tar", last modified: Sun Apr 21 20:05:22 2024, max compression
+gzip compressed data, was "spiderwebai-py-0.1.3.tar", last modified: Sun Apr 21 20:32:46 2024, max compression
```

## Comparing `spiderwebai-py-0.1.2.tar` & `spiderwebai-py-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-21 20:05:22.232313 spiderwebai-py-0.1.2/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spiderwebai-py-0.1.2/LICENSE
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     3581 2024-04-21 20:05:22.232169 spiderwebai-py-0.1.2/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     2835 2024-04-18 18:14:45.000000 spiderwebai-py-0.1.2/README.md
--rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-21 20:05:22.232356 spiderwebai-py-0.1.2/setup.cfg
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     1065 2024-04-21 20:02:14.000000 spiderwebai-py-0.1.2/setup.py
-drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-21 20:05:22.231979 spiderwebai-py-0.1.2/spiderwebai_py.egg-info/
--rw-r--r--   0 jeffreymendez   (501) staff       (20)     3581 2024-04-21 20:05:22.000000 spiderwebai-py-0.1.2/spiderwebai_py.egg-info/PKG-INFO
--rw-r--r--   0 jeffreymendez   (501) staff       (20)      215 2024-04-21 20:05:22.000000 spiderwebai-py-0.1.2/spiderwebai_py.egg-info/SOURCES.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-21 20:05:22.000000 spiderwebai-py-0.1.2/spiderwebai_py.egg-info/dependency_links.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-21 20:05:22.000000 spiderwebai-py-0.1.2/spiderwebai_py.egg-info/requires.txt
--rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-21 20:05:22.000000 spiderwebai-py-0.1.2/spiderwebai_py.egg-info/top_level.txt
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-21 20:32:46.529589 spiderwebai-py-0.1.3/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       10 2024-04-18 16:30:24.000000 spiderwebai-py-0.1.3/LICENSE
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     3581 2024-04-21 20:32:46.529445 spiderwebai-py-0.1.3/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     2835 2024-04-18 18:14:45.000000 spiderwebai-py-0.1.3/README.md
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       38 2024-04-21 20:32:46.529654 spiderwebai-py-0.1.3/setup.cfg
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     1065 2024-04-21 20:32:07.000000 spiderwebai-py-0.1.3/setup.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-21 20:32:46.528586 spiderwebai-py-0.1.3/spiderwebai/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       39 2024-04-18 16:23:20.000000 spiderwebai-py-0.1.3/spiderwebai/__init__.py
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     5501 2024-04-21 20:02:06.000000 spiderwebai-py-0.1.3/spiderwebai/spiderwebai.py
+drwxr-xr-x   0 jeffreymendez   (501) staff       (20)        0 2024-04-21 20:32:46.529269 spiderwebai-py-0.1.3/spiderwebai_py.egg-info/
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)     3581 2024-04-21 20:32:46.000000 spiderwebai-py-0.1.3/spiderwebai_py.egg-info/PKG-INFO
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)      266 2024-04-21 20:32:46.000000 spiderwebai-py-0.1.3/spiderwebai_py.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        1 2024-04-21 20:32:46.000000 spiderwebai-py-0.1.3/spiderwebai_py.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)        9 2024-04-21 20:32:46.000000 spiderwebai-py-0.1.3/spiderwebai_py.egg-info/requires.txt
+-rw-r--r--   0 jeffreymendez   (501) staff       (20)       12 2024-04-21 20:32:46.000000 spiderwebai-py-0.1.3/spiderwebai_py.egg-info/top_level.txt
```

### Comparing `spiderwebai-py-0.1.2/PKG-INFO` & `spiderwebai-py-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiderwebai-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python SDK for SpiderWebAI API
 Home-page: https://github.com/spider-rs/spiderwebai-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `spiderwebai-py-0.1.2/README.md` & `spiderwebai-py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `spiderwebai-py-0.1.2/setup.py` & `spiderwebai-py-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read_file(fname):
     return open(os.path.join(os.path.dirname(__file__), fname), encoding="utf-8").read()
 
 
 setup(
     name="spiderwebai-py",
-    version="0.1.2",
+    version="0.1.3",
     url="https://github.com/spider-rs/spiderwebai-clients/tree/main/python",
     author="Spider",
     author_email="jeff@a11ywatch.com",
     description="Python SDK for SpiderWebAI API",
     packages=find_packages(),
     install_requires=[
         "requests",
```

### Comparing `spiderwebai-py-0.1.2/spiderwebai_py.egg-info/PKG-INFO` & `spiderwebai-py-0.1.3/spiderwebai_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiderwebai-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python SDK for SpiderWebAI API
 Home-page: https://github.com/spider-rs/spiderwebai-clients/tree/main/python
 Author: Spider
 Author-email: jeff@a11ywatch.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

