# Comparing `tmp/basic-bar-0.3.tar.gz` & `tmp/basic_bar-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic-bar-0.3.tar", last modified: Fri Jun  2 08:22:34 2023, max compression
+gzip compressed data, was "basic_bar-0.4.tar", last modified: Sun Apr 21 22:16:42 2024, max compression
```

## Comparing `basic-bar-0.3.tar` & `basic_bar-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:22:34.501681 basic-bar-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-02 08:22:12.000000 basic-bar-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-02 08:22:34.501681 basic-bar-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-02 08:22:12.000000 basic-bar-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:22:34.497681 basic-bar-0.3/basic_bar/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 08:22:12.000000 basic-bar-0.3/basic_bar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-02 08:22:12.000000 basic-bar-0.3/basic_bar/basic_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:22:34.497681 basic-bar-0.3/basic_bar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-02 08:22:34.000000 basic-bar-0.3/basic_bar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-02 08:22:34.000000 basic-bar-0.3/basic_bar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:22:34.000000 basic-bar-0.3/basic_bar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 08:22:34.000000 basic-bar-0.3/basic_bar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:22:34.501681 basic-bar-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-02 08:22:12.000000 basic-bar-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:16:42.553331 basic_bar-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-21 22:16:38.000000 basic_bar-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-21 22:16:42.553331 basic_bar-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-21 22:16:38.000000 basic_bar-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:16:42.553331 basic_bar-0.4/basic_bar/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-21 22:16:38.000000 basic_bar-0.4/basic_bar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-21 22:16:38.000000 basic_bar-0.4/basic_bar/basic_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:16:42.553331 basic_bar-0.4/basic_bar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-21 22:16:42.000000 basic_bar-0.4/basic_bar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-21 22:16:42.000000 basic_bar-0.4/basic_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:16:42.000000 basic_bar-0.4/basic_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 22:16:42.000000 basic_bar-0.4/basic_bar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:16:42.553331 basic_bar-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-21 22:16:38.000000 basic_bar-0.4/setup.py
```

### Comparing `basic-bar-0.3/LICENSE` & `basic_bar-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `basic-bar-0.3/PKG-INFO` & `basic_bar-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basic-bar
-Version: 0.3
+Version: 0.4
 Summary: A simple and efficient progress bar
 Home-page: https://github.com/splch/py-basic-bar
 Author: Spencer Churchill
 Author-email: spence@duck.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `basic-bar-0.3/basic_bar/basic_bar.py` & `basic_bar-0.4/basic_bar/basic_bar.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import time, sys
 
-def bar(iterable, length=33):
+
+def progress(iterable, length=33):
     total, start = len(iterable), time.monotonic()
     for count, it in enumerate(iterable, 1):
         yield it
-        elapsed_time, remaining_time = time.monotonic() - start, (time.monotonic() - start) / count * (total - count)
-        percent, filled_len = count / total, int(length * (count / total))
-        sys.stdout.write(f'\r▕{"█" * filled_len}{" " * (length - filled_len)}▏ {percent*100:.2f}% {remaining_time:.2f}s'), sys.stdout.flush()
+        if count % max(1, total // 10000) == 0 or count == total:
+            percent = count / total
+            sys.stdout.write(
+                f'\r▕{"█" * int(length * percent) + " " * (length - int(length * percent))}▏ '
+                f"{percent * 100:.2f}% "
+                f"{(time.monotonic() - start) / count * (total - count):.2f}s"
+            ), sys.stdout.flush()
     sys.stdout.write(f'\r▕{"█" * length}▏ 100.00% {time.monotonic() - start:.2f}s\n')
```

### Comparing `basic-bar-0.3/basic_bar.egg-info/PKG-INFO` & `basic_bar-0.4/basic_bar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basic-bar
-Version: 0.3
+Version: 0.4
 Summary: A simple and efficient progress bar
 Home-page: https://github.com/splch/py-basic-bar
 Author: Spencer Churchill
 Author-email: spence@duck.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `basic-bar-0.3/setup.py` & `basic_bar-0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name="basic-bar",
-    version="0.3",
+    version="0.4",
     description="A simple and efficient progress bar",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Spencer Churchill",
     author_email="spence@duck.com",
     url="https://github.com/splch/py-basic-bar",
     packages=find_packages(),
```

