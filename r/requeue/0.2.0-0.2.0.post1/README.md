# Comparing `tmp/requeue-0.2.0.tar.gz` & `tmp/requeue-0.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requeue-0.2.0.tar", max compression
+gzip compressed data, was "requeue-0.2.0.post1.tar", max compression
```

## Comparing `requeue-0.2.0.tar` & `requeue-0.2.0.post1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2024-03-10 22:34:57.217631 requeue-0.2.0/LICENSE
--rw-r--r--   0        0        0     1320 2024-03-12 04:25:45.986781 requeue-0.2.0/README.md
--rw-r--r--   0        0        0      391 2024-03-16 20:07:51.440884 requeue-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2714 2024-03-16 19:58:57.882205 requeue-0.2.0/requeue/__init__.py
--rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 requeue-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-10 22:34:57.217631 requeue-0.2.0.post1/LICENSE
+-rw-r--r--   0        0        0     1318 2024-04-22 03:53:47.024295 requeue-0.2.0.post1/README.md
+-rw-r--r--   0        0        0      397 2024-04-22 03:59:50.554434 requeue-0.2.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     2714 2024-03-16 19:58:57.882205 requeue-0.2.0.post1/requeue/__init__.py
+-rw-r--r--   0        0        0     1927 1970-01-01 00:00:00.000000 requeue-0.2.0.post1/PKG-INFO
```

### Comparing `requeue-0.2.0/LICENSE` & `requeue-0.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `requeue-0.2.0/README.md` & `requeue-0.2.0.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Where the messages come in and are processed;
 
 ```python
 async def run_callbacks(message):
     # If the message completes a request, since it is forwarded,
     # it should not continue to be handled by the callbacks.
     if await queue.complete(message):
-        continue
+        return
 
     # If no request was completed, the message can be processed as usual.
     for callback in client.callbacks:
         await callback(message)
 ```
 
 Inside a callback, to request and await an incoming message, you use `wait_for`.
```

### Comparing `requeue-0.2.0/requeue/__init__.py` & `requeue-0.2.0.post1/requeue/__init__.py`

 * *Files identical despite different names*

### Comparing `requeue-0.2.0/PKG-INFO` & `requeue-0.2.0.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requeue
-Version: 0.2.0
+Version: 0.2.0.post1
 Summary: An asynchronous queue for requesting data
 Home-page: https://gitlab.com/deepadmax/requeue
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maxi@millian.se
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -30,15 +30,15 @@
 Where the messages come in and are processed;
 
 ```python
 async def run_callbacks(message):
     # If the message completes a request, since it is forwarded,
     # it should not continue to be handled by the callbacks.
     if await queue.complete(message):
-        continue
+        return
 
     # If no request was completed, the message can be processed as usual.
     for callback in client.callbacks:
         await callback(message)
 ```
 
 Inside a callback, to request and await an incoming message, you use `wait_for`.
```

