# Comparing `tmp/qtlink-1.2.6.tar.gz` & `tmp/qtlink-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.2.6.tar", last modified: Thu Apr 18 14:04:35 2024, max compression
+gzip compressed data, was "qtlink-1.2.7.tar", last modified: Mon Apr 22 07:08:56 2024, max compression
```

## Comparing `qtlink-1.2.6.tar` & `qtlink-1.2.7.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.513302 qtlink-1.2.6/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.6/LICENSE
--rw-rw-rw-   0        0        0      466 2024-04-18 14:04:35.512575 qtlink-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.424073 qtlink-1.2.6/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.6/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.466017 qtlink-1.2.6/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.6/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1996 2024-04-17 13:33:05.000000 qtlink-1.2.6/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0     1719 2024-04-17 13:30:53.000000 qtlink-1.2.6/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     2060 2024-04-17 13:09:04.000000 qtlink-1.2.6/qtlink/dialog/dialog_table_check.py
--rw-rw-rw-   0        0        0     2096 2024-04-17 13:09:04.000000 qtlink-1.2.6/qtlink/dialog/dialog_table_display.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.466017 qtlink-1.2.6/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.6/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.6/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.486765 qtlink-1.2.6/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.6/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.6/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.6/qtlink/table/table_controller_multiple_check.py
--rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.6/qtlink/table/table_controller_single_check.py
--rw-rw-rw-   0        0        0     5182 2024-04-18 14:03:24.000000 qtlink-1.2.6/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.500551 qtlink-1.2.6/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.6/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     2094 2024-04-17 09:07:46.000000 qtlink-1.2.6/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.6/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.511439 qtlink-1.2.6/qtlink.egg-info/
--rw-rw-rw-   0        0        0      466 2024-04-18 14:04:35.000000 qtlink-1.2.6/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2024-04-18 14:04:35.000000 qtlink-1.2.6/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 14:04:35.000000 qtlink-1.2.6/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 14:04:35.000000 qtlink-1.2.6/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 14:04:35.000000 qtlink-1.2.6/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 14:04:35.513302 qtlink-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      637 2024-04-18 14:04:15.000000 qtlink-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:08:56.966606 qtlink-1.2.7/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0      466 2024-04-22 07:08:56.965787 qtlink-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 07:08:56.803052 qtlink-1.2.7/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.7/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:08:56.877587 qtlink-1.2.7/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.7/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1445 2024-04-22 07:06:38.000000 qtlink-1.2.7/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     2060 2024-04-17 13:09:04.000000 qtlink-1.2.7/qtlink/dialog/dialog_table_check.py
+-rw-rw-rw-   0        0        0     2096 2024-04-17 13:09:04.000000 qtlink-1.2.7/qtlink/dialog/dialog_table_display.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:08:56.893622 qtlink-1.2.7/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.7/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.7/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:08:56.925057 qtlink-1.2.7/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.7/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.7/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.7/qtlink/table/table_controller_multiple_check.py
+-rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.7/qtlink/table/table_controller_single_check.py
+-rw-rw-rw-   0        0        0     5182 2024-04-18 14:03:24.000000 qtlink-1.2.7/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:08:56.957127 qtlink-1.2.7/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.7/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2094 2024-04-17 09:07:46.000000 qtlink-1.2.7/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.7/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:08:56.964057 qtlink-1.2.7/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      466 2024-04-22 07:08:56.000000 qtlink-1.2.7/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      639 2024-04-22 07:08:56.000000 qtlink-1.2.7/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 07:08:56.000000 qtlink-1.2.7/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-22 07:08:56.000000 qtlink-1.2.7/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-22 07:08:56.000000 qtlink-1.2.7/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 07:08:56.966606 qtlink-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      637 2024-04-22 07:08:19.000000 qtlink-1.2.7/setup.py
```

### Comparing `qtlink-1.2.6/LICENSE` & `qtlink-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.6/qtlink/dialog/dialog_table_check.py` & `qtlink-1.2.7/qtlink/dialog/dialog_table_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.6/qtlink/dialog/dialog_table_display.py` & `qtlink-1.2.7/qtlink/dialog/dialog_table_display.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.6/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.2.7/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.6/qtlink/table/table_controller.py` & `qtlink-1.2.7/qtlink/table/table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.6/qtlink/table/table_controller_multiple_check.py` & `qtlink-1.2.7/qtlink/table/table_controller_multiple_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.6/qtlink/table/table_controller_single_check.py` & `qtlink-1.2.7/qtlink/table/table_controller_single_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.6/qtlink/util.py` & `qtlink-1.2.7/qtlink/util.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.6/qtlink/widgets/drop_widget.py` & `qtlink-1.2.7/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.6/qtlink/widgets/list_widget.py` & `qtlink-1.2.7/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.6/qtlink.egg-info/SOURCES.txt` & `qtlink-1.2.7/qtlink.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 qtlink/util.py
 qtlink.egg-info/PKG-INFO
 qtlink.egg-info/SOURCES.txt
 qtlink.egg-info/dependency_links.txt
 qtlink.egg-info/requires.txt
 qtlink.egg-info/top_level.txt
 qtlink/dialog/__init__.py
-qtlink/dialog/dialog_choice.py
 qtlink/dialog/dialog_info.py
 qtlink/dialog/dialog_table_check.py
 qtlink/dialog/dialog_table_display.py
 qtlink/mpl_canvas/__init__.py
 qtlink/mpl_canvas/mpl_canvas.py
 qtlink/table/__init__.py
 qtlink/table/table_controller.py
```

### Comparing `qtlink-1.2.6/setup.py` & `qtlink-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.2.6",
+    version="1.2.7",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6'],
```

