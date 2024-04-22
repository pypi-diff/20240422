# Comparing `tmp/happyscript-0.0.1.tar.gz` & `tmp/happyscript-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happyscript-0.0.1.tar", last modified: Mon Apr 22 02:21:02 2024, max compression
+gzip compressed data, was "happyscript-0.0.2.tar", last modified: Mon Apr 22 02:42:45 2024, max compression
```

## Comparing `happyscript-0.0.1.tar` & `happyscript-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 02:21:02.478159 happyscript-0.0.1/
--rw-rw-rw-   0        0        0      193 2024-04-22 02:21:02.478159 happyscript-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       26 2024-04-22 02:04:12.000000 happyscript-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 02:21:02.462836 happyscript-0.0.1/happyscript/
--rw-rw-rw-   0        0        0   211595 2024-04-22 01:55:54.000000 happyscript-0.0.1/happyscript/happyscript.py
-drwxrwxrwx   0        0        0        0 2024-04-22 02:21:02.478159 happyscript-0.0.1/happyscript.egg-info/
--rw-rw-rw-   0        0        0      193 2024-04-22 02:21:02.000000 happyscript-0.0.1/happyscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2024-04-22 02:21:02.000000 happyscript-0.0.1/happyscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 02:21:02.000000 happyscript-0.0.1/happyscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-22 02:21:02.000000 happyscript-0.0.1/happyscript.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      274 2024-04-22 02:17:13.000000 happyscript-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 02:21:02.478159 happyscript-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-22 02:42:45.553816 happyscript-0.0.2/
+-rw-rw-rw-   0        0        0      193 2024-04-22 02:42:45.553816 happyscript-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2024-04-22 02:04:12.000000 happyscript-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 02:42:45.539808 happyscript-0.0.2/happyscript/
+-rw-rw-rw-   0        0        0   211595 2024-04-22 01:55:54.000000 happyscript-0.0.2/happyscript/happyscript.py
+drwxrwxrwx   0        0        0        0 2024-04-22 02:42:45.553816 happyscript-0.0.2/happyscript.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-04-22 02:42:45.000000 happyscript-0.0.2/happyscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2024-04-22 02:42:45.000000 happyscript-0.0.2/happyscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 02:42:45.000000 happyscript-0.0.2/happyscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-22 02:42:45.000000 happyscript-0.0.2/happyscript.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      274 2024-04-22 02:42:29.000000 happyscript-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-22 02:42:45.553816 happyscript-0.0.2/setup.cfg
```

### Comparing `happyscript-0.0.1/happyscript/happyscript.py` & `happyscript-0.0.2/happyscript/happyscript.py`

 * *Files identical despite different names*

