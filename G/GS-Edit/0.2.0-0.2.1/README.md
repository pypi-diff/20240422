# Comparing `tmp/gs_edit-0.2.0.tar.gz` & `tmp/gs_edit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs_edit-0.2.0.tar", last modified: Mon Apr 22 02:19:50 2024, max compression
+gzip compressed data, was "gs_edit-0.2.1.tar", last modified: Mon Apr 22 03:02:10 2024, max compression
```

## Comparing `gs_edit-0.2.0.tar` & `gs_edit-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 02:19:50.070000 gs_edit-0.2.0/
--rw-rw-rw-   0        0        0     1066 2024-02-12 21:48:00.000000 gs_edit-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1742 2024-04-22 02:19:52.000000 gs_edit-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-04 04:14:34.000000 gs_edit-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 02:19:52.000000 gs_edit-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      681 2024-04-22 02:19:30.000000 gs_edit-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 02:19:50.070000 gs_edit-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 02:19:50.080000 gs_edit-0.2.0/src/GS_Edit.egg-info/
--rw-rw-rw-   0        0        0     1742 2024-04-22 02:19:52.000000 gs_edit-0.2.0/src/GS_Edit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      734 2024-04-22 02:19:52.000000 gs_edit-0.2.0/src/GS_Edit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 02:19:52.000000 gs_edit-0.2.0/src/GS_Edit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-22 02:19:52.000000 gs_edit-0.2.0/src/GS_Edit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-22 02:19:52.000000 gs_edit-0.2.0/src/GS_Edit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-22 02:19:52.000000 gs_edit-0.2.0/src/GS_Edit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-22 02:19:50.080000 gs_edit-0.2.0/src/gsedit/
--rw-rw-rw-   0        0        0        0 2024-04-22 02:06:00.000000 gs_edit-0.2.0/src/gsedit/__init__.py
--rw-rw-rw-   0        0        0      375 2024-04-22 02:00:36.000000 gs_edit-0.2.0/src/gsedit/cli.py
--rw-rw-rw-   0        0        0      958 2024-03-26 00:10:36.000000 gs_edit-0.2.0/src/gsedit/code_completer.py
--rw-rw-rw-   0        0        0     8120 2024-04-22 02:07:52.000000 gs_edit-0.2.0/src/gsedit/css_editor.py
--rw-rw-rw-   0        0        0     8706 2024-04-19 04:12:50.000000 gs_edit-0.2.0/src/gsedit/file_explorer.py
--rw-rw-rw-   0        0        0     4266 2024-04-22 02:07:52.000000 gs_edit-0.2.0/src/gsedit/grep.py
--rw-rw-rw-   0        0        0     3374 2024-03-21 05:28:34.000000 gs_edit-0.2.0/src/gsedit/grepgine.py
--rw-rw-rw-   0        0        0     1477 2024-03-21 05:28:34.000000 gs_edit-0.2.0/src/gsedit/gsconfig.py
--rw-rw-rw-   0        0        0     4085 2024-04-22 02:07:52.000000 gs_edit-0.2.0/src/gsedit/integrated_terminal.py
--rw-rw-rw-   0        0        0    19210 2024-04-19 04:12:50.000000 gs_edit-0.2.0/src/gsedit/language_lexer.py
--rw-rw-rw-   0        0        0     2846 2024-04-22 02:07:52.000000 gs_edit-0.2.0/src/gsedit/main.py
--rw-rw-rw-   0        0        0     1787 2024-04-22 02:07:52.000000 gs_edit-0.2.0/src/gsedit/main_body.py
--rw-rw-rw-   0        0        0    14261 2024-04-22 02:07:52.000000 gs_edit-0.2.0/src/gsedit/menu_bar.py
--rw-rw-rw-   0        0        0      784 2024-04-22 02:07:52.000000 gs_edit-0.2.0/src/gsedit/popup.py
--rw-rw-rw-   0        0        0    11554 2024-03-26 00:10:42.000000 gs_edit-0.2.0/src/gsedit/res_src.py
--rw-rw-rw-   0        0        0     3073 2024-04-22 02:07:52.000000 gs_edit-0.2.0/src/gsedit/sidebar.py
--rw-rw-rw-   0        0        0      541 2024-04-22 02:07:52.000000 gs_edit-0.2.0/src/gsedit/status_bar.py
--rw-rw-rw-   0        0        0     1230 2024-04-22 02:07:52.000000 gs_edit-0.2.0/src/gsedit/tab_bar.py
--rw-rw-rw-   0        0        0     6917 2024-04-01 00:33:10.000000 gs_edit-0.2.0/src/gsedit/text_editor.py
--rw-rw-rw-   0        0        0     2340 2024-04-22 02:07:52.000000 gs_edit-0.2.0/src/gsedit/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-22 02:19:50.090000 gs_edit-0.2.0/src/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 02:04:38.000000 gs_edit-0.2.0/src/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:02:10.420000 gs_edit-0.2.1/
+-rw-rw-rw-   0        0        0     1066 2024-02-12 21:48:00.000000 gs_edit-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1742 2024-04-22 03:02:12.000000 gs_edit-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-04 04:14:34.000000 gs_edit-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 03:02:12.000000 gs_edit-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      681 2024-04-22 03:01:50.000000 gs_edit-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:02:10.420000 gs_edit-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 03:02:10.430000 gs_edit-0.2.1/src/GS_Edit.egg-info/
+-rw-rw-rw-   0        0        0     1742 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      734 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-22 03:02:12.000000 gs_edit-0.2.1/src/GS_Edit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 03:02:10.430000 gs_edit-0.2.1/src/gsedit/
+-rw-rw-rw-   0        0        0        0 2024-04-22 02:06:00.000000 gs_edit-0.2.1/src/gsedit/__init__.py
+-rw-rw-rw-   0        0        0      382 2024-04-22 02:45:16.000000 gs_edit-0.2.1/src/gsedit/cli.py
+-rw-rw-rw-   0        0        0      958 2024-03-26 00:10:36.000000 gs_edit-0.2.1/src/gsedit/code_completer.py
+-rw-rw-rw-   0        0        0     8520 2024-04-22 03:00:52.000000 gs_edit-0.2.1/src/gsedit/css_editor.py
+-rw-rw-rw-   0        0        0     8720 2024-04-22 02:33:12.000000 gs_edit-0.2.1/src/gsedit/file_explorer.py
+-rw-rw-rw-   0        0        0     4445 2024-04-22 02:47:20.000000 gs_edit-0.2.1/src/gsedit/grep.py
+-rw-rw-rw-   0        0        0     3381 2024-04-22 02:35:40.000000 gs_edit-0.2.1/src/gsedit/grepgine.py
+-rw-rw-rw-   0        0        0     1477 2024-03-21 05:28:34.000000 gs_edit-0.2.1/src/gsedit/gsconfig.py
+-rw-rw-rw-   0        0        0     4388 2024-04-22 02:51:32.000000 gs_edit-0.2.1/src/gsedit/integrated_terminal.py
+-rw-rw-rw-   0        0        0    19217 2024-04-22 02:35:24.000000 gs_edit-0.2.1/src/gsedit/language_lexer.py
+-rw-rw-rw-   0        0        0     3017 2024-04-22 02:43:30.000000 gs_edit-0.2.1/src/gsedit/main.py
+-rw-rw-rw-   0        0        0     1955 2024-04-22 02:47:40.000000 gs_edit-0.2.1/src/gsedit/main_body.py
+-rw-rw-rw-   0        0        0    14413 2024-04-22 02:47:58.000000 gs_edit-0.2.1/src/gsedit/menu_bar.py
+-rw-rw-rw-   0        0        0      882 2024-04-22 02:53:56.000000 gs_edit-0.2.1/src/gsedit/popup.py
+-rw-rw-rw-   0        0        0    11554 2024-03-26 00:10:42.000000 gs_edit-0.2.1/src/gsedit/res_src.py
+-rw-rw-rw-   0        0        0     3237 2024-04-22 02:49:22.000000 gs_edit-0.2.1/src/gsedit/sidebar.py
+-rw-rw-rw-   0        0        0      700 2024-04-22 02:45:14.000000 gs_edit-0.2.1/src/gsedit/status_bar.py
+-rw-rw-rw-   0        0        0     1599 2024-04-22 02:58:22.000000 gs_edit-0.2.1/src/gsedit/tab_bar.py
+-rw-rw-rw-   0        0        0     6945 2024-04-22 02:50:02.000000 gs_edit-0.2.1/src/gsedit/text_editor.py
+-rw-rw-rw-   0        0        0     2524 2024-04-22 02:50:20.000000 gs_edit-0.2.1/src/gsedit/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:02:10.430000 gs_edit-0.2.1/src/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 02:04:38.000000 gs_edit-0.2.1/src/tests/__init__.py
```

### Comparing `gs_edit-0.2.0/LICENSE` & `gs_edit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.0/PKG-INFO` & `gs_edit-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GS-Edit
-Version: 0.2.0
+Version: 0.2.1
 Summary: The Best Code Editor - GS
 Home-page: https://github.com/james-kaddissi/yourproject
 Author: James Kaddissi
 Author-email: jameskaddissi@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gs_edit-0.2.0/README.md` & `gs_edit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.0/setup.py` & `gs_edit-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='GS-Edit', 
-    version='0.2.0',
+    version='0.2.1',
     description='The Best Code Editor - GS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',  
     author='James Kaddissi',
     author_email='jameskaddissi@gmail.com',
     url='https://github.com/james-kaddissi/yourproject',
     packages=find_packages(where='src'),
```

### Comparing `gs_edit-0.2.0/src/GS_Edit.egg-info/PKG-INFO` & `gs_edit-0.2.1/src/GS_Edit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GS-Edit
-Version: 0.2.0
+Version: 0.2.1
 Summary: The Best Code Editor - GS
 Home-page: https://github.com/james-kaddissi/yourproject
 Author: James Kaddissi
 Author-email: jameskaddissi@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gs_edit-0.2.0/src/GS_Edit.egg-info/SOURCES.txt` & `gs_edit-0.2.1/src/GS_Edit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.0/src/gsedit/code_completer.py` & `gs_edit-0.2.1/src/gsedit/code_completer.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.0/src/gsedit/css_editor.py` & `gs_edit-0.2.1/src/gsedit/css_editor.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,28 +46,39 @@
 
         self.statusBar()
         self.load_file_list()
         self.refresh_style()
         self.splitter.setSizes([300, 500])
 
     def refresh_style(self):
-        with open("./src/gsedit/css/cssEditor.qss", "r") as f:
-            self.setStyleSheet(f.read())
+        base_path = os.path.dirname(__file__)
+        style_sheet_path = os.path.join(base_path, 'css', 'cssEditor.qss')
+        with open(style_sheet_path, "r") as style_file:
+            self.setStyleSheet(style_file.read())
 
     def load_file_list(self):
-        path = './src/gsedit/css'
-        for file_name in os.listdir(path):
+        base_path = os.path.dirname(__file__) 
+        css_path = os.path.join(base_path, 'css')  
+
+        if not os.path.exists(css_path):
+            self.statusBar().showMessage('CSS directory not found: {}'.format(css_path))
+            return
+
+        for file_name in os.listdir(css_path):
             if file_name.endswith('.qss'):
                 self.file_browser.addItem(file_name)
 
     def load_css_properties(self, current, previous):
         if not current:
             return
-        self.current_file = f"./src/gsedit/css/{current.text()}"  
-        self.refresh_css_editor(self.current_file)
+
+        base_path = os.path.dirname(__file__)
+        css_path = os.path.join(base_path, 'css', current.text())
+        
+        self.refresh_css_editor(css_path)
 
     def refresh_css_editor(self, file_path):
         while self.property_layout.count():
             child = self.property_layout.takeAt(0)
             if child.widget():
                 child.widget().deleteLater()
         self.property_layout.addWidget(QLabel(f"Editing: {file_path}"))
```

### Comparing `gs_edit-0.2.0/src/gsedit/file_explorer.py` & `gs_edit-0.2.1/src/gsedit/file_explorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from PyQt5.Qsci import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
 
 from pathlib import Path
 import subprocess, sys, shutil, os
 
-from text_editor import TextEditor
-from popup import PopupMessage
+from gsedit.text_editor import TextEditor
+from gsedit.popup import PopupMessage
 
 class FileExplorer(QTreeView):
     def __init__(self, tab, add_tab, window):
         super(FileExplorer, self).__init__(None)
 
         self.tab = tab
         self.add_tab = add_tab
```

### Comparing `gs_edit-0.2.0/src/gsedit/grep.py` & `gs_edit-0.2.1/src/gsedit/grep.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from PyQt5.QtWidgets import *
 from PyQt5 import *
 from PyQt5.Qsci import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
 
 from pathlib import Path
-from text_editor import TextEditor
-import gsconfig
+from gsedit.text_editor import TextEditor
+import gsedit.gsconfig
+
+import os
 
 class GrepLayout(QVBoxLayout):
     def __init__(self) -> None:
         super(GrepLayout, self).__init__()
         self.initialize_layout()
 
     def initialize_layout(self):
@@ -37,15 +39,18 @@
         self.initialize_toggler()
         self.refresh_style()
     
     def initialize_toggler(self):
         self.setFont(self.window.window_font)
 
     def refresh_style(self):
-        self.setStyleSheet(open("./src/gsedit/css/grep.qss", "r").read())
+        base_path = os.path.dirname(__file__) 
+        style_sheet_path = os.path.join(base_path, 'css', 'grep.qss')
+        with open(style_sheet_path, "r") as style_file:
+            self.setStyleSheet(style_file.read())
 
 class GrepResult(QListWidget):
     def __init__(self, window) -> None:
         super(GrepResult, self).__init__()
         self.window = window
         self.initialize_results()
```

### Comparing `gs_edit-0.2.0/src/gsedit/grepgine.py` & `gs_edit-0.2.1/src/gsedit/grepgine.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from PyQt5.QtWidgets import *
 from PyQt5 import *
 from PyQt5.Qsci import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
 
-import gsconfig
+import gsedit.gsconfig
 
 class GrepListItem(QListWidgetItem):
     def __init__(self, name, path, ln,  endln, lntxt):
         self.name = name
         self.path = path
         self.ln = ln
         self.endln = endln
```

### Comparing `gs_edit-0.2.0/src/gsedit/gsconfig.py` & `gs_edit-0.2.1/src/gsedit/gsconfig.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.0/src/gsedit/integrated_terminal.py` & `gs_edit-0.2.1/src/gsedit/integrated_terminal.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,18 @@
         self.process.readyReadStandardError.connect(self.error_output_triggered)
         self.process.start("cmd.exe" if os.name == 'nt' else "/bin/bash")
         self.is_command_executing = False
         self.command_start_position = self.textCursor().position()
         self.clicked = pyqtSignal()
 
     def refresh_style(self):
-        self.setStyleSheet(open("./src/gsedit/css/integratedTerminal.qss", "r").read())
+        base_path = os.path.dirname(__file__)
+        style_sheet_path = os.path.join(base_path, 'css', 'integratedTerminal.qss')
+        with open(style_sheet_path, "r") as style_file:
+            self.setStyleSheet(style_file.read())
 
     def keyPressEvent(self, event):
         cursor = self.textCursor()
         if event.key() in (Qt.Key_Return, Qt.Key_Enter) and not self.is_command_executing:
             self.executeCommand()
         elif event.key() == Qt.Key_Backspace:
             if cursor.position() > self.command_start_position:
@@ -81,15 +84,18 @@
         self.tab_widget = QTabWidget()
         self.layout.addWidget(self.tab_widget)
         self.add_new_terminal_tab()
         self.refresh_style()
 
 
     def refresh_style(self):
-        self.setStyleSheet(open("./src/gsedit/css/integratedTerminal.qss", "r").read())
+        base_path = os.path.dirname(__file__) 
+        style_sheet_path = os.path.join(base_path, 'css', 'integratedTerminal.qss')
+        with open(style_sheet_path, "r") as style_file:
+            self.setStyleSheet(style_file.read())
 
     def add_new_terminal_tab(self):
         splitter = QSplitter(Qt.Horizontal)
         terminal = IntegratedTerminalTextEdit()
         splitter.addWidget(terminal)
         self.tab_widget.addTab(splitter, "Terminal")
```

### Comparing `gs_edit-0.2.0/src/gsedit/language_lexer.py` & `gs_edit-0.2.1/src/gsedit/language_lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import json
 
 from PyQt5.Qsci import *
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 from PyQt5.QtWidgets import *
 
-import gsconfig
+import gsedit.gsconfig
 
 
 class GSLexer(QsciLexerCustom):
     def __init__(self, language, editor, path=None, base_config=None):
         super(GSLexer, self).__init__(editor)
         self.editor = editor
         self.language = language
```

### Comparing `gs_edit-0.2.0/src/gsedit/main.py` & `gs_edit-0.2.1/src/gsedit/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 # PyQt imports (migration to PyQt6 should be a simple task for a future date)
 from PyQt5.QtWidgets import *
 from PyQt5 import *
 from PyQt5.Qsci import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
 # Class imports
-from status_bar import StatusBar
-from menu_bar import MenuBar
-from tab_bar import TabBar
-from main_body import MainBodyFrame
-from sidebar import Sidebar
+from gsedit.status_bar import StatusBar
+from gsedit.menu_bar import MenuBar
+from gsedit.tab_bar import TabBar
+from gsedit.main_body import MainBodyFrame
+from gsedit.sidebar import Sidebar
 from gsedit.tools import FileExplorerFrame, GrepFrame
-from css_editor import CSSEditor
+from gsedit.css_editor import CSSEditor
 # Other function imports
-import gsconfig
+import gsedit.gsconfig
 
 class MainWindow(QMainWindow):
     def __init__(self):
         # CONFIG
         super(QMainWindow, self).__init__()
         self.app_title = "GS-Edit"
         self.app_icon = QIcon("./src/gsedit/images/icon.png")
@@ -34,16 +34,18 @@
         self.current_tool = "folder"
         self.css_editor = CSSEditor(self)
 
     def initialize_window(self):
         # window configuration
         self.setWindowTitle(self.app_title)
         self.resize(1400, 1000)
-        # initialize styles
-        self.setStyleSheet(open("./src/gsedit/css/style.qss", "r").read())
+        base_path = os.path.dirname(__file__)
+        style_sheet_path = os.path.join(base_path, 'css', 'style.qss')
+        with open(style_sheet_path, "r") as style_file:
+            self.setStyleSheet(style_file.read())
         self.window_font = QFont("Fixedsys")
         self.window_font.setPointSize(12)
         self.setFont(self.window_font)
         self.configure_statusbar()
         self.configure_body()
         self.configure_menu()
         self.show()
```

### Comparing `gs_edit-0.2.0/src/gsedit/main_body.py` & `gs_edit-0.2.1/src/gsedit/main_body.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from PyQt5.QtWidgets import *
 from PyQt5 import *
 from PyQt5.Qsci import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
 
-from integrated_terminal import IntegratedTerminal
-
+from gsedit.integrated_terminal import IntegratedTerminal
 
+import os
 
 class MainBodyFrame(QFrame):
     def __init__(self, window) -> None:
         super(MainBodyFrame, self).__init__()
         self.refresh_style()
         self.window = window
         self.initialize_frame()
         self.set_layout()
 
     def refresh_style(self):
-        self.setStyleSheet(open("./src/gsedit/css/mainBody.qss", "r").read())
+        base_path = os.path.dirname(__file__) 
+        style_sheet_path = os.path.join(base_path, 'css', 'mainBody.qss')
+        with open(style_sheet_path, "r") as style_file:
+            self.setStyleSheet(style_file.read())
 
     def initialize_frame(self):
         self.setFrameShape(QFrame.NoFrame)
         self.setFrameShadow(QFrame.Plain)
         self.setLineWidth(0)
         self.setMidLineWidth(0)
         self.setContentsMargins(0, 0, 0, 0,)
```

### Comparing `gs_edit-0.2.0/src/gsedit/menu_bar.py` & `gs_edit-0.2.1/src/gsedit/menu_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,18 @@
         self.initialize_main_menu_bar()
         self.refresh_style()
         self.window = main_window
         self.status_bar = status_bar
         self.file_explorer = file_explorer
 
     def refresh_style(self):
-        self.setStyleSheet(open("./src/gsedit/css/menuBar.qss", "r").read())
+        base_path = os.path.dirname(__file__) 
+        style_sheet_path = os.path.join(base_path, 'css', 'menuBar.qss')
+        with open(style_sheet_path, "r") as style_file:
+            self.setStyleSheet(style_file.read())
 
     def initialize_main_menu_bar(self):
 
         self.initialize_file_menu()
         self.initialize_edit_menu()
         self.initialize_selection_menu()
         self.initialize_run_menu()
```

### Comparing `gs_edit-0.2.0/src/gsedit/popup.py` & `gs_edit-0.2.1/src/gsedit/popup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from PyQt5 import *
 from PyQt5.QtWidgets import *
 from PyQt5.Qsci import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
 
+import os
+
 class PopupMessage(QMessageBox):
     def __init__(self, title, text) -> None:
         super(PopupMessage, self).__init__()
         self.title = title
         self.text = text
         self.initialize_popup()
 
     def initialize_popup(self):
         self.setFont(self.font())
         self.font().setPointSize(16)
         self.setWindowTitle(self.title)
         self.setText(self.text)
+        image_path = os.path.join(os.path.dirname(__file__), 'images', 'close.svg')
         self.setWindowIcon(QIcon("./src/gsedit/images/close.svg"))
         self.setStandardButtons(QMessageBox.Yes | QMessageBox.No)
         self.setDefaultButton(QMessageBox.No)
         self.setIcon(QMessageBox.Warning)
 
         return self.exec_()
```

### Comparing `gs_edit-0.2.0/src/gsedit/res_src.py` & `gs_edit-0.2.1/src/gsedit/res_src.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.0/src/gsedit/sidebar.py` & `gs_edit-0.2.1/src/gsedit/sidebar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from PyQt5.QtWidgets import *
 from PyQt5 import *
 from PyQt5.Qsci import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
 
+import os
 
 class Sidebar(QFrame):
     def __init__(self, window) -> None:
         super(Sidebar, self).__init__()
         self.window = window
         self.initialize_sidebar()
         self.refresh_style()
     
     def initialize_sidebar(self):
         self.setFrameShape(QFrame.StyledPanel)
         self.setFrameShadow(QFrame.Plain)
         self.setLayout(SidebarLayout(self.window))
 
     def refresh_style(self):
-        self.setStyleSheet(open("./src/gsedit/css/sidebar.qss", "r").read()) #collin smith
+        base_path = os.path.dirname(__file__)  
+        style_sheet_path = os.path.join(base_path, 'css', 'sidebar.qss')
+        with open(style_sheet_path, "r") as style_file:
+            self.setStyleSheet(style_file.read()) #collin smith
 
 class SidebarLayout(QVBoxLayout):
     def __init__(self, window) -> None:
         super(SidebarLayout, self).__init__()
         self.window = window
         self.initialize_layout()
         self.initialize_icons()
```

### Comparing `gs_edit-0.2.0/src/gsedit/status_bar.py` & `gs_edit-0.2.1/src/gsedit/status_bar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from PyQt5.QtWidgets import *
 from PyQt5 import *
 from PyQt5.Qsci import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
 
 import sys
+import os
 
 class StatusBar(QStatusBar):
     def __init__(self) -> None:
         super(StatusBar, self).__init__()
         self.refresh_style()
         self.set_timed_message("GS-Edit started successfully!", 3000)
 
     def refresh_style(self):
-        self.setStyleSheet(open("./src/gsedit/css/statusBar.qss", "r").read())
+        base_path = os.path.dirname(__file__) 
+        style_sheet_path = os.path.join(base_path, 'css', 'statusBar.qss')
+        with open(style_sheet_path, "r") as style_file:
+            self.setStyleSheet(style_file.read())
 
     def set_timed_message(self, message, time):
         self.showMessage(message, time)
```

### Comparing `gs_edit-0.2.0/src/gsedit/tab_bar.py` & `gs_edit-0.2.1/src/gsedit/tab_bar.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,26 +2,36 @@
 from PyQt5 import *
 from PyQt5.Qsci import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
 from PyQt5.QtWidgets import *
 
 import os
-from popup import PopupMessage
+from gsedit.popup import PopupMessage
 
 class TabBar(QTabWidget):
     def __init__(self, main_window, status_bar) -> None:
         super(TabBar, self).__init__()
         self.window = main_window
         self.bar = status_bar
         self.refresh_style()
         self.initialize_tabs()
     
     def refresh_style(self):
-        self.setStyleSheet(open("./src/gsedit/css/tabBar.qss", "r").read())
+        base_path = os.path.dirname(__file__)
+        style_sheet_path = os.path.join(base_path, 'css', 'tabBar.qss')
+
+        with open(style_sheet_path, "r") as style_file:
+            style_content = style_file.read()
+
+        icon_path = os.path.join(base_path, 'images', 'close.svg').replace('\\', '/')
+        style_content = style_content.replace('url_placeholder', icon_path)
+
+        self.setStyleSheet(style_content)
+
 
     def initialize_tabs(self):
         self.setUsesScrollButtons(True)
         self.setContentsMargins(0, 0, 0, 0)
         self.setTabsClosable(True)
         self.setMovable(True)
         self.setDocumentMode(True)
```

### Comparing `gs_edit-0.2.0/src/gsedit/text_editor.py` & `gs_edit-0.2.1/src/gsedit/text_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
 from typing import *
 
 import pkgutil
 import keyword
 
-import gsconfig
+import gsedit.gsconfig
 
 from pathlib import Path
 
-from language_lexer import PythonLexer, CLexer, JSONLexer, RustLexer, CppLexer
-from code_completer import Completer
+from gsedit.language_lexer import PythonLexer, CLexer, JSONLexer, RustLexer, CppLexer
+from gsedit.code_completer import Completer
 
 
 if TYPE_CHECKING:
-    from main import MainWindow # prevents circular imports
+    from gsedit.main import MainWindow # prevents circular imports
 
 class TextEditor(QsciScintilla):
     def __init__(self, window, parent = None, path = None, pyf=None, cf=None, jsonf=None, rustf=None, cppf=None):
         super(TextEditor, self).__init__(parent)
         self.window = window
         self.path = path
         self.abs_path = self.path.absolute()
```

### Comparing `gs_edit-0.2.0/src/gsedit/tools.py` & `gs_edit-0.2.1/src/gsedit/tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from PyQt5.QtWidgets import *
 from PyQt5 import *
 from PyQt5.Qsci import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
+import os
 
-from file_explorer import FileExplorer, FileExplorerLayout
-from grep import GrepLayout, Searchbar, GrepToggle, GrepResult
-from grepgine import Grepgine
+from gsedit.file_explorer import FileExplorer, FileExplorerLayout
+from gsedit.grep import GrepLayout, Searchbar, GrepToggle, GrepResult
+from gsedit.grepgine import Grepgine
 
 class GeneralToolFrame(QFrame):
     def __init__(self) -> None:
         super(GeneralToolFrame, self).__init__()
         self.initialize_frame(200, 400)
         self.refresh_style()
     
@@ -18,15 +19,18 @@
         self.setMaximumWidth(maximum)
         self.setMinimumWidth(minimum)
         self.setFrameShape(QFrame.NoFrame)
         self.setFrameShadow(QFrame.Plain)
         self.setContentsMargins(0, 0, 0, 0)
 
     def refresh_style(self):
-        self.setStyleSheet(open("./src/gsedit/css/tools.qss", "r").read())
+        base_path = os.path.dirname(__file__) 
+        style_sheet_path = os.path.join(base_path, 'css', 'tools.qss')
+        with open(style_sheet_path, "r") as style_file:
+            self.setStyleSheet(style_file.read())
 
 class FileExplorerFrame(GeneralToolFrame):
     def __init__(self, window) -> None:
         super(FileExplorerFrame, self).__init__()
         self.window = window
         self.file_explorer_layout = FileExplorerLayout()
         self.file_explorer = FileExplorer(tab=self.window.tab, add_tab=self.window.grep_frame.grep_view.add_tab, window=self.window)
```

