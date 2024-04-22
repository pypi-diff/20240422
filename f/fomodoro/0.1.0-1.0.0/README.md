# Comparing `tmp/fomodoro-0.1.0.tar.gz` & `tmp/fomodoro-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fomodoro-0.1.0.tar", last modified: Mon Apr 22 00:27:40 2024, max compression
+gzip compressed data, was "fomodoro-1.0.0.tar", last modified: Sun Apr 21 22:25:40 2024, max compression
```

## Comparing `fomodoro-0.1.0.tar` & `fomodoro-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 00:27:40.893209 fomodoro-0.1.0/
--rw-rw-rw-   0        0        0       61 2024-04-21 22:49:04.000000 fomodoro-0.1.0/.gitignore
--rw-rw-rw-   0        0        0       23 2024-04-21 05:46:17.000000 fomodoro-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      395 2024-04-22 00:27:40.893209 fomodoro-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       97 2024-04-21 21:06:56.000000 fomodoro-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 00:27:40.681656 fomodoro-0.1.0/fomodoro/
--rw-rw-rw-   0        0        0        0 2024-04-20 22:04:56.000000 fomodoro-0.1.0/fomodoro/__init__.py
--rw-rw-rw-   0        0        0      118 2024-04-21 20:47:01.000000 fomodoro-0.1.0/fomodoro/info.json
--rw-rw-rw-   0        0        0     3973 2024-04-21 20:44:50.000000 fomodoro-0.1.0/fomodoro/main.py
--rw-rw-rw-   0        0        0      463 2024-04-21 05:32:56.000000 fomodoro-0.1.0/fomodoro/stopwatch.py
--rw-rw-rw-   0        0        0      431 2024-04-21 04:04:10.000000 fomodoro-0.1.0/fomodoro/timer.py
--rw-rw-rw-   0        0        0      367 2024-04-21 20:40:56.000000 fomodoro-0.1.0/fomodoro/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 00:27:40.877590 fomodoro-0.1.0/fomodoro.egg-info/
--rw-rw-rw-   0        0        0      395 2024-04-22 00:27:39.000000 fomodoro-0.1.0/fomodoro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-04-22 00:27:39.000000 fomodoro-0.1.0/fomodoro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 00:27:39.000000 fomodoro-0.1.0/fomodoro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-22 00:27:39.000000 fomodoro-0.1.0/fomodoro.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-22 00:27:39.000000 fomodoro-0.1.0/fomodoro.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-22 00:27:39.000000 fomodoro-0.1.0/fomodoro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2024-04-22 00:22:24.000000 fomodoro-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      116 2024-04-20 22:04:56.000000 fomodoro-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 00:27:40.908829 fomodoro-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 22:25:40.008867 fomodoro-1.0.0/
+-rw-rw-rw-   0        0        0       51 2024-04-21 05:49:02.000000 fomodoro-1.0.0/.gitignore
+-rw-rw-rw-   0        0        0       23 2024-04-21 05:46:17.000000 fomodoro-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      357 2024-04-21 22:25:39.993275 fomodoro-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       97 2024-04-21 21:06:56.000000 fomodoro-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 22:25:39.344635 fomodoro-1.0.0/fomodoro/
+-rw-rw-rw-   0        0        0        0 2024-04-20 22:04:56.000000 fomodoro-1.0.0/fomodoro/__init__.py
+-rw-rw-rw-   0        0        0      118 2024-04-21 20:47:01.000000 fomodoro-1.0.0/fomodoro/info.json
+-rw-rw-rw-   0        0        0     3973 2024-04-21 20:44:50.000000 fomodoro-1.0.0/fomodoro/main.py
+-rw-rw-rw-   0        0        0      463 2024-04-21 05:32:56.000000 fomodoro-1.0.0/fomodoro/stopwatch.py
+-rw-rw-rw-   0        0        0      431 2024-04-21 04:04:10.000000 fomodoro-1.0.0/fomodoro/timer.py
+-rw-rw-rw-   0        0        0      367 2024-04-21 20:40:56.000000 fomodoro-1.0.0/fomodoro/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:25:39.977847 fomodoro-1.0.0/fomodoro.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-04-21 22:25:34.000000 fomodoro-1.0.0/fomodoro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-04-21 22:25:35.000000 fomodoro-1.0.0/fomodoro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 22:25:34.000000 fomodoro-1.0.0/fomodoro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-21 22:25:34.000000 fomodoro-1.0.0/fomodoro.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-04-21 22:25:34.000000 fomodoro-1.0.0/fomodoro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      497 2024-04-21 21:08:55.000000 fomodoro-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      116 2024-04-20 22:04:56.000000 fomodoro-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 22:25:40.008867 fomodoro-1.0.0/setup.cfg
```

### Comparing `fomodoro-0.1.0/fomodoro/main.py` & `fomodoro-1.0.0/fomodoro/main.py`

 * *Files identical despite different names*

