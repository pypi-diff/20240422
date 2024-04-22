# Comparing `tmp/klein_queue-2.4.4.tar.gz` & `tmp/klein_queue-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/klein_queue-2.4.4.tar", last modified: Tue Jul 18 13:45:34 2023, max compression
+gzip compressed data, was "klein_queue-2.4.5.tar", last modified: Mon Apr 22 08:43:15 2024, max compression
```

## Comparing `klein_queue-2.4.4.tar` & `klein_queue-2.4.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:45:34.000000 klein_queue-2.4.4/
--rw-rw-rw-   0 root         (0) root         (0)     9136 2023-07-18 13:45:06.000000 klein_queue-2.4.4/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-18 13:45:06.000000 klein_queue-2.4.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2558 2023-07-18 13:45:34.000000 klein_queue-2.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2228 2023-07-18 13:45:06.000000 klein_queue-2.4.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 13:45:34.000000 klein_queue-2.4.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1637 2023-07-18 13:45:06.000000 klein_queue-2.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue/
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2406 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/api.py
--rw-rw-rw-   0 root         (0) root         (0)    11730 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/connect.py
--rw-rw-rw-   0 root         (0) root         (0)    12614 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)     4596 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7847 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/publisher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2558 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      558 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:43:15.140802 klein_queue-2.4.5/
+-rw-rw-rw-   0 root         (0) root         (0)     9136 2024-04-22 08:43:06.000000 klein_queue-2.4.5/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-22 08:43:06.000000 klein_queue-2.4.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4358 2024-04-22 08:43:15.140802 klein_queue-2.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3933 2024-04-22 08:43:06.000000 klein_queue-2.4.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 08:43:15.140802 klein_queue-2.4.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2024-04-22 08:43:06.000000 klein_queue-2.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:43:15.136219 klein_queue-2.4.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:43:15.137136 klein_queue-2.4.5/src/klein_queue/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:43:15.138969 klein_queue-2.4.5/src/klein_queue/rabbitmq/
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2406 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    11730 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/connect.py
+-rw-rw-rw-   0 root         (0) root         (0)    12614 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7847 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/klein_queue/rabbitmq/publisher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:43:15.138969 klein_queue-2.4.5/src/klein_queue.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4358 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      558 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 08:43:15.000000 klein_queue-2.4.5/src/klein_queue.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-22 08:43:06.000000 klein_queue-2.4.5/src/version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `klein_queue-2.4.4/LICENSE.txt` & `klein_queue-2.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.4/setup.py` & `klein_queue-2.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.4/src/klein_queue/errors.py` & `klein_queue-2.4.5/src/klein_queue/errors.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.4/src/klein_queue/rabbitmq/api.py` & `klein_queue-2.4.5/src/klein_queue/rabbitmq/api.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.4/src/klein_queue/rabbitmq/connect.py` & `klein_queue-2.4.5/src/klein_queue/rabbitmq/connect.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.4/src/klein_queue/rabbitmq/consumer.py` & `klein_queue-2.4.5/src/klein_queue/rabbitmq/consumer.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.4/src/klein_queue/rabbitmq/exceptions.py` & `klein_queue-2.4.5/src/klein_queue/rabbitmq/exceptions.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.4/src/klein_queue/rabbitmq/publisher.py` & `klein_queue-2.4.5/src/klein_queue/rabbitmq/publisher.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.4/src/klein_queue.egg-info/SOURCES.txt` & `klein_queue-2.4.5/src/klein_queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

