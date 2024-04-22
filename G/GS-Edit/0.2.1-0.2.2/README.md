# Comparing `tmp/gs_edit-0.2.1.tar.gz` & `tmp/gs_edit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs_edit-0.2.1.tar", last modified: Mon Apr 22 03:02:10 2024, max compression
+gzip compressed data, was "gs_edit-0.2.2.tar", last modified: Mon Apr 22 03:32:35 2024, max compression
```

## Comparing `gs_edit-0.2.1.tar` & `gs_edit-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 03:02:10.420000 gs_edit-0.2.1/
--rw-rw-rw-   0        0        0     1066 2024-02-12 21:48:00.000000 gs_edit-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1742 2024-04-22 03:02:12.000000 gs_edit-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-04 04:14:34.000000 gs_edit-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 03:02:12.000000 gs_edit-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      681 2024-04-22 03:01:50.000000 gs_edit-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:02:10.420000 gs_edit-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 03:02:10.430000 gs_edit-0.2.1/src/GS_Edit.egg-info/
--rw-rw-rw-   0        0        0     1742 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      734 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-22 03:02:10.430000 gs_edit-0.2.1/src/gsedit/
--rw-rw-rw-   0        0        0        0 2024-04-22 02:06:00.000000 gs_edit-0.2.1/src/gsedit/__init__.py
--rw-rw-rw-   0        0        0      382 2024-04-22 02:45:16.000000 gs_edit-0.2.1/src/gsedit/cli.py
--rw-rw-rw-   0        0        0      958 2024-03-26 00:10:36.000000 gs_edit-0.2.1/src/gsedit/code_completer.py
--rw-rw-rw-   0        0        0     8520 2024-04-22 03:00:52.000000 gs_edit-0.2.1/src/gsedit/css_editor.py
--rw-rw-rw-   0        0        0     8720 2024-04-22 02:33:12.000000 gs_edit-0.2.1/src/gsedit/file_explorer.py
--rw-rw-rw-   0        0        0     4445 2024-04-22 02:47:20.000000 gs_edit-0.2.1/src/gsedit/grep.py
--rw-rw-rw-   0        0        0     3381 2024-04-22 02:35:40.000000 gs_edit-0.2.1/src/gsedit/grepgine.py
--rw-rw-rw-   0        0        0     1477 2024-03-21 05:28:34.000000 gs_edit-0.2.1/src/gsedit/gsconfig.py
--rw-rw-rw-   0        0        0     4388 2024-04-22 02:51:32.000000 gs_edit-0.2.1/src/gsedit/integrated_terminal.py
--rw-rw-rw-   0        0        0    19217 2024-04-22 02:35:24.000000 gs_edit-0.2.1/src/gsedit/language_lexer.py
--rw-rw-rw-   0        0        0     3017 2024-04-22 02:43:30.000000 gs_edit-0.2.1/src/gsedit/main.py
--rw-rw-rw-   0        0        0     1955 2024-04-22 02:47:40.000000 gs_edit-0.2.1/src/gsedit/main_body.py
--rw-rw-rw-   0        0        0    14413 2024-04-22 02:47:58.000000 gs_edit-0.2.1/src/gsedit/menu_bar.py
--rw-rw-rw-   0        0        0      882 2024-04-22 02:53:56.000000 gs_edit-0.2.1/src/gsedit/popup.py
--rw-rw-rw-   0        0        0    11554 2024-03-26 00:10:42.000000 gs_edit-0.2.1/src/gsedit/res_src.py
--rw-rw-rw-   0        0        0     3237 2024-04-22 02:49:22.000000 gs_edit-0.2.1/src/gsedit/sidebar.py
--rw-rw-rw-   0        0        0      700 2024-04-22 02:45:14.000000 gs_edit-0.2.1/src/gsedit/status_bar.py
--rw-rw-rw-   0        0        0     1599 2024-04-22 02:58:22.000000 gs_edit-0.2.1/src/gsedit/tab_bar.py
--rw-rw-rw-   0        0        0     6945 2024-04-22 02:50:02.000000 gs_edit-0.2.1/src/gsedit/text_editor.py
--rw-rw-rw-   0        0        0     2524 2024-04-22 02:50:20.000000 gs_edit-0.2.1/src/gsedit/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:02:10.430000 gs_edit-0.2.1/src/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 02:04:38.000000 gs_edit-0.2.1/src/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:32:35.480000 gs_edit-0.2.2/
+-rw-rw-rw-   0        0        0     1066 2024-02-12 21:48:00.000000 gs_edit-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     1738 2024-04-22 03:32:36.000000 gs_edit-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-04 04:14:34.000000 gs_edit-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 03:32:36.000000 gs_edit-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      850 2024-04-22 03:24:42.000000 gs_edit-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:32:35.480000 gs_edit-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 03:32:35.490000 gs_edit-0.2.2/src/GS_Edit.egg-info/
+-rw-rw-rw-   0        0        0     1738 2024-04-22 03:32:36.000000 gs_edit-0.2.2/src/GS_Edit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      845 2024-04-22 03:32:36.000000 gs_edit-0.2.2/src/GS_Edit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 03:32:36.000000 gs_edit-0.2.2/src/GS_Edit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-22 03:32:36.000000 gs_edit-0.2.2/src/GS_Edit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-22 03:32:36.000000 gs_edit-0.2.2/src/GS_Edit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-22 03:32:36.000000 gs_edit-0.2.2/src/GS_Edit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 03:32:35.490000 gs_edit-0.2.2/src/gsedit/
+-rw-rw-rw-   0        0        0        0 2024-04-22 02:06:00.000000 gs_edit-0.2.2/src/gsedit/__init__.py
+-rw-rw-rw-   0        0        0      382 2024-04-22 02:45:16.000000 gs_edit-0.2.2/src/gsedit/cli.py
+-rw-rw-rw-   0        0        0      958 2024-03-26 00:10:36.000000 gs_edit-0.2.2/src/gsedit/code_completer.py
+-rw-rw-rw-   0        0        0     8520 2024-04-22 03:00:52.000000 gs_edit-0.2.2/src/gsedit/css_editor.py
+-rw-rw-rw-   0        0        0     8720 2024-04-22 02:33:12.000000 gs_edit-0.2.2/src/gsedit/file_explorer.py
+-rw-rw-rw-   0        0        0     4445 2024-04-22 02:47:20.000000 gs_edit-0.2.2/src/gsedit/grep.py
+-rw-rw-rw-   0        0        0     3381 2024-04-22 02:35:40.000000 gs_edit-0.2.2/src/gsedit/grepgine.py
+-rw-rw-rw-   0        0        0     1477 2024-03-21 05:28:34.000000 gs_edit-0.2.2/src/gsedit/gsconfig.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:32:35.500000 gs_edit-0.2.2/src/gsedit/images/
+-rw-rw-rw-   0        0        0     1240 2024-02-22 23:10:24.000000 gs_edit-0.2.2/src/gsedit/images/close.svg
+-rw-rw-rw-   0        0        0     1087 2024-02-22 19:27:58.000000 gs_edit-0.2.2/src/gsedit/images/folder.svg
+-rw-rw-rw-   0        0        0     1918 2024-02-29 06:36:00.000000 gs_edit-0.2.2/src/gsedit/images/grep.svg
+-rw-rw-rw-   0        0        0  2514652 2024-03-24 21:36:04.000000 gs_edit-0.2.2/src/gsedit/images/icon.png
+-rw-rw-rw-   0        0        0     4388 2024-04-22 02:51:32.000000 gs_edit-0.2.2/src/gsedit/integrated_terminal.py
+-rw-rw-rw-   0        0        0    19217 2024-04-22 02:35:24.000000 gs_edit-0.2.2/src/gsedit/language_lexer.py
+-rw-rw-rw-   0        0        0     3017 2024-04-22 02:43:30.000000 gs_edit-0.2.2/src/gsedit/main.py
+-rw-rw-rw-   0        0        0     1955 2024-04-22 02:47:40.000000 gs_edit-0.2.2/src/gsedit/main_body.py
+-rw-rw-rw-   0        0        0    14413 2024-04-22 02:47:58.000000 gs_edit-0.2.2/src/gsedit/menu_bar.py
+-rw-rw-rw-   0        0        0      882 2024-04-22 02:53:56.000000 gs_edit-0.2.2/src/gsedit/popup.py
+-rw-rw-rw-   0        0        0    11554 2024-03-26 00:10:42.000000 gs_edit-0.2.2/src/gsedit/res_src.py
+-rw-rw-rw-   0        0        0     3237 2024-04-22 02:49:22.000000 gs_edit-0.2.2/src/gsedit/sidebar.py
+-rw-rw-rw-   0        0        0      700 2024-04-22 02:45:14.000000 gs_edit-0.2.2/src/gsedit/status_bar.py
+-rw-rw-rw-   0        0        0     1599 2024-04-22 02:58:22.000000 gs_edit-0.2.2/src/gsedit/tab_bar.py
+-rw-rw-rw-   0        0        0     6945 2024-04-22 02:50:02.000000 gs_edit-0.2.2/src/gsedit/text_editor.py
+-rw-rw-rw-   0        0        0     2524 2024-04-22 02:50:20.000000 gs_edit-0.2.2/src/gsedit/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:32:35.500000 gs_edit-0.2.2/src/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 02:04:38.000000 gs_edit-0.2.2/src/tests/__init__.py
```

### Comparing `gs_edit-0.2.1/LICENSE` & `gs_edit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/PKG-INFO` & `gs_edit-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: GS-Edit
-Version: 0.2.1
+Version: 0.2.2
 Summary: The Best Code Editor - GS
-Home-page: https://github.com/james-kaddissi/yourproject
+Home-page: https://github.com/james-kaddissi/gs_edit
 Author: James Kaddissi
 Author-email: jameskaddissi@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyQt5
 Requires-Dist: QScintilla
```

### Comparing `gs_edit-0.2.1/README.md` & `gs_edit-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/GS_Edit.egg-info/PKG-INFO` & `gs_edit-0.2.2/src/GS_Edit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: GS-Edit
-Version: 0.2.1
+Version: 0.2.2
 Summary: The Best Code Editor - GS
-Home-page: https://github.com/james-kaddissi/yourproject
+Home-page: https://github.com/james-kaddissi/gs_edit
 Author: James Kaddissi
 Author-email: jameskaddissi@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyQt5
 Requires-Dist: QScintilla
```

### Comparing `gs_edit-0.2.1/src/GS_Edit.egg-info/SOURCES.txt` & `gs_edit-0.2.2/src/GS_Edit.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,8 +23,12 @@
 src/gsedit/popup.py
 src/gsedit/res_src.py
 src/gsedit/sidebar.py
 src/gsedit/status_bar.py
 src/gsedit/tab_bar.py
 src/gsedit/text_editor.py
 src/gsedit/tools.py
+src/gsedit/images/close.svg
+src/gsedit/images/folder.svg
+src/gsedit/images/grep.svg
+src/gsedit/images/icon.png
 src/tests/__init__.py
```

### Comparing `gs_edit-0.2.1/src/gsedit/code_completer.py` & `gs_edit-0.2.2/src/gsedit/code_completer.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/css_editor.py` & `gs_edit-0.2.2/src/gsedit/css_editor.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/file_explorer.py` & `gs_edit-0.2.2/src/gsedit/file_explorer.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/grep.py` & `gs_edit-0.2.2/src/gsedit/grep.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/grepgine.py` & `gs_edit-0.2.2/src/gsedit/grepgine.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/gsconfig.py` & `gs_edit-0.2.2/src/gsedit/gsconfig.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/integrated_terminal.py` & `gs_edit-0.2.2/src/gsedit/integrated_terminal.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/language_lexer.py` & `gs_edit-0.2.2/src/gsedit/language_lexer.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/main.py` & `gs_edit-0.2.2/src/gsedit/main.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/main_body.py` & `gs_edit-0.2.2/src/gsedit/main_body.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/menu_bar.py` & `gs_edit-0.2.2/src/gsedit/menu_bar.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/popup.py` & `gs_edit-0.2.2/src/gsedit/popup.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/res_src.py` & `gs_edit-0.2.2/src/gsedit/res_src.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/sidebar.py` & `gs_edit-0.2.2/src/gsedit/sidebar.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/status_bar.py` & `gs_edit-0.2.2/src/gsedit/status_bar.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/tab_bar.py` & `gs_edit-0.2.2/src/gsedit/tab_bar.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/text_editor.py` & `gs_edit-0.2.2/src/gsedit/text_editor.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.1/src/gsedit/tools.py` & `gs_edit-0.2.2/src/gsedit/tools.py`

 * *Files identical despite different names*

