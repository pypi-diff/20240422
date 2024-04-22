# Comparing `tmp/pywinstyles-1.7.tar.gz` & `tmp/pywinstyles-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywinstyles-1.7.tar", last modified: Sun Feb 18 14:33:08 2024, max compression
+gzip compressed data, was "pywinstyles-1.8.tar", last modified: Mon Apr 22 06:17:20 2024, max compression
```

## Comparing `pywinstyles-1.7.tar` & `pywinstyles-1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-02-18 14:33:08.182702 pywinstyles-1.7/
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 pywinstyles-1.7/LICENSE
--rw-rw-rw-   0        0        0     3946 2024-02-18 14:33:08.182702 pywinstyles-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3278 2024-02-18 14:32:05.000000 pywinstyles-1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-02-18 14:33:08.174695 pywinstyles-1.7/pywinstyles/
--rw-rw-rw-   0        0        0      512 2024-02-18 14:02:09.000000 pywinstyles-1.7/pywinstyles/__init__.py
--rw-rw-rw-   0        0        0    13039 2024-02-18 14:16:26.000000 pywinstyles-1.7/pywinstyles/py_win_style.py
-drwxrwxrwx   0        0        0        0 2024-02-18 14:33:08.182702 pywinstyles-1.7/pywinstyles.egg-info/
--rw-rw-rw-   0        0        0     3946 2024-02-18 14:33:08.000000 pywinstyles-1.7/pywinstyles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2024-02-18 14:33:08.000000 pywinstyles-1.7/pywinstyles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-18 14:33:08.000000 pywinstyles-1.7/pywinstyles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-02-18 14:33:08.000000 pywinstyles-1.7/pywinstyles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      602 2024-02-18 14:33:08.192708 pywinstyles-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1109 2024-02-18 14:32:14.000000 pywinstyles-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:17:20.365515 pywinstyles-1.8/
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 pywinstyles-1.8/LICENSE
+-rw-rw-rw-   0        0        0     4080 2024-04-22 06:17:20.365515 pywinstyles-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3410 2024-04-22 06:16:57.000000 pywinstyles-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 06:17:20.349891 pywinstyles-1.8/pywinstyles/
+-rw-rw-rw-   0        0        0      547 2024-04-22 06:07:44.000000 pywinstyles-1.8/pywinstyles/__init__.py
+-rw-rw-rw-   0        0        0    15817 2024-04-22 06:12:01.000000 pywinstyles-1.8/pywinstyles/py_win_style.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:17:20.365515 pywinstyles-1.8/pywinstyles.egg-info/
+-rw-rw-rw-   0        0        0     4080 2024-04-22 06:17:20.000000 pywinstyles-1.8/pywinstyles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2024-04-22 06:17:20.000000 pywinstyles-1.8/pywinstyles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 06:17:20.000000 pywinstyles-1.8/pywinstyles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-22 06:17:20.000000 pywinstyles-1.8/pywinstyles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      602 2024-04-22 06:17:20.381140 pywinstyles-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1109 2024-04-22 06:15:34.000000 pywinstyles-1.8/setup.py
```

### Comparing `pywinstyles-1.7/LICENSE` & `pywinstyles-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pywinstyles-1.7/PKG-INFO` & `pywinstyles-1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinstyles
-Version: 1.7
+Version: 1.8
 Summary:  Customize window styles in windows 11
 Home-page: https://github.com/Akascape/py-window-styles
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: window-styles,pywinstyles,pywindowstyles,customtkinter,tkinter,python-window-themes,gui,python-gui,pyqt,title-bar,title-bar-color,windows-themes,wxpython,windows11
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -78,19 +78,23 @@
 ### Get Windows Accent Color
 ```python
 default_color = pywinstyles.get_accent_color() # returns hex color string
 ```
 
 ### Set opacity of individual widgets
 ```python
-pywinstyes.set_opacity(widget_id, value=0.5)
+pywinstyles.set_opacity(widget_id, value=0.5)
 ```
 
 ### Make a color transparent inside widget
 ```python
-pywinstyes.set_opacity(widget_id, color="white")
+pywinstyles.set_opacity(widget_id, color="white")
+```
+### Add file DND feature to widgets
+```python
+def drop_func(file):
+  print(file) 
+pywinstyles.apply_dnd(widget_id, frop_func)
 ```
-
 **Hope this package can help in UI development with python**
 
 **Author: Akash Bora**
-
```

### Comparing `pywinstyles-1.7/README.md` & `pywinstyles-1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,19 +63,23 @@
 ### Get Windows Accent Color
 ```python
 default_color = pywinstyles.get_accent_color() # returns hex color string
 ```
 
 ### Set opacity of individual widgets
 ```python
-pywinstyes.set_opacity(widget_id, value=0.5)
+pywinstyles.set_opacity(widget_id, value=0.5)
 ```
 
 ### Make a color transparent inside widget
 ```python
-pywinstyes.set_opacity(widget_id, color="white")
+pywinstyles.set_opacity(widget_id, color="white")
+```
+### Add file DND feature to widgets
+```python
+def drop_func(file):
+  print(file) 
+pywinstyles.apply_dnd(widget_id, frop_func)
 ```
-
 **Hope this package can help in UI development with python**
 
-**Author: Akash Bora**
-
+**Author: Akash Bora**
```

### Comparing `pywinstyles-1.7/pywinstyles/__init__.py` & `pywinstyles-1.8/pywinstyles/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Custom window styles for windows 11
 Author: Akash Bora
 License: MIT
 Homepage: https://github.com/Akascape/py-window-styles
 """
 
-__version__ = '1.7'
+__version__ = '1.8'
 
 from .py_win_style import apply_style
 from .py_win_style import change_header_color
 from .py_win_style import change_border_color
 from .py_win_style import change_title_color
 from .py_win_style import get_accent_color
 from .py_win_style import set_opacity
 from .py_win_style import ChangeDWMAttrib
 from .py_win_style import ChangeDWMAccent
-
+from .py_win_style import apply_dnd
```

### Comparing `pywinstyles-1.7/pywinstyles/py_win_style.py` & `pywinstyles-1.8/pywinstyles/py_win_style.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 Py-Win-Styles
 Author: Akash Bora
-Version: 1.7
+Version: 1.8
 """
 
-from typing import Any
+from __future__ import annotations
+from typing import Any, Union, Callable
 
 try:
     import winreg
     from ctypes import (POINTER, Structure, byref, c_int, pointer, sizeof,
-                        windll)
+                        windll, c_buffer, WINFUNCTYPE, c_uint64)
     from ctypes.wintypes import DWORD, ULONG
+    import platform
+
 except ImportError:
     raise ImportError("pywinstyles import errror: No windows environment detected!")
 
 
 class ACCENT_POLICY(Structure):
     _fields_ = [
         ("AccentState", DWORD),
@@ -93,15 +96,15 @@
             ChangeDWMAccent(self.HWND, 6, 0)
             ChangeDWMAccent(self.HWND, 4, 0)
             ChangeDWMAccent(self.HWND, 11, 0)
             ChangeDWMAttrib(self.HWND, 19, c_int(0))
             ChangeDWMAttrib(self.HWND, 20, c_int(0))
             ChangeDWMAccent(self.HWND, 30, 0)
             ChangeDWMAccent(self.HWND, 19, 0)
-
+            DisableFrameIntoClientArea(self.HWND)
 
 class change_header_color():
     """change the titlebar background color"""
 
     def __init__(self, window: Any, color: str) -> None:
 
         self.HWND = detect(window)
@@ -158,20 +161,81 @@
         wnd_exstyle = windll.user32.GetWindowLongA(self.widget_id, -20)
         new_exstyle = wnd_exstyle | 0x00080000
         windll.user32.SetWindowLongA(self.widget_id, -20, new_exstyle)
         windll.user32.SetLayeredWindowAttributes(
             self.widget_id, self.color, self.opacity, 3
         )
 
+class apply_dnd():
+    """apply file drag and drop in a widget"""
+    
+    def __init__(self, widget: int, func: Callable, char_limit: int=260) -> None:
 
+        try:
+            # check for tkinter widgets exclusively
+            hwnd = widget.winfo_id()
+        except:
+            hwnd = widget
+        if not isinstance(hwnd, int):
+            raise ValueError("widget ID should be passed, not the widget name.")
+        
+        if platform.architecture()[0] == "32bit":
+            GetWindowLong = windll.user32.GetWindowLongW
+            SetWindowLong = windll.user32.SetWindowLongW
+            typ = DWORD
+
+        if platform.architecture()[0] == "64bit":
+            GetWindowLong = windll.user32.GetWindowLongPtrA
+            SetWindowLong = windll.user32.SetWindowLongPtrA
+            typ = c_uint64
+
+        prototype = WINFUNCTYPE(typ, typ, typ, typ, typ)
+        WM_DROP_FILES = 0x233
+        GWL_WND_PROC = -4
+        create_buffer = c_buffer
+        func_DragQueryFile = (windll.shell32.DragQueryFile)
+
+        def py_drop_func(hwnd, msg, wp, lp):
+            global files
+            if msg == WM_DROP_FILES:
+                count = func_DragQueryFile(typ(wp), -1, None, None)
+                file_buffer = create_buffer(char_limit)
+                files = []
+                for i in range(count):
+                    func_DragQueryFile(typ(wp), i, file_buffer, sizeof(file_buffer))
+                    drop_name = file_buffer.value.decode("utf-8")
+                    files.append(drop_name)
+                func(files)
+                windll.shell32.DragFinish(typ(wp))
+
+            return windll.user32.CallWindowProcW(
+                *map(typ, (globals()[old], hwnd, msg, wp, lp))
+            )
+
+        """ Allow upto 10 widgets only to have dnd feature in one window, reduces system uses"""
+        limit_num = 10
+        for i in range(limit_num):
+            if i + 1 == limit_num:
+                raise OverflowError("DND limit reached for this session!")
+            owp = f"old_wnd_proc_{i}"
+            if owp not in globals():
+                old, new = owp, f"new_wnd_proc_{i}"
+                break
+
+        globals()[old] = None
+        globals()[new] = prototype(py_drop_func)
+
+        windll.shell32.DragAcceptFiles(hwnd, True)
+        globals()[old] = GetWindowLong(hwnd, GWL_WND_PROC)
+        SetWindowLong(hwnd, GWL_WND_PROC, globals()[new])
+        
 def ChangeDWMAttrib(hWnd: int, attrib: int, color) -> None:
     windll.dwmapi.DwmSetWindowAttribute(hWnd, attrib, byref(color), sizeof(c_int))
 
-
-def ChangeDWMAccent(hWnd: int, attrib: int, state: int, color: str | None = None) -> None:
+def ChangeDWMAccent(hWnd: int, attrib: int, state: int, color: Union[str, None] = None) -> None:
     accentPolicy = ACCENT_POLICY()
 
     winCompAttrData = WINDOW_COMPOSITION_ATTRIBUTES()
     winCompAttrData.Attribute = attrib
     winCompAttrData.SizeOfData = sizeof(accentPolicy)
     winCompAttrData.Data = pointer(accentPolicy)
 
@@ -181,14 +245,18 @@
 
     windll.user32.SetWindowCompositionAttribute(hWnd, pointer(winCompAttrData))
 
 
 def ExtendFrameIntoClientArea(HWND: int) -> None:
     margins = MARGINS(-1, -1, -1, -1)
     windll.dwmapi.DwmExtendFrameIntoClientArea(HWND, byref(margins))
+    
+def DisableFrameIntoClientArea(HWND: int) -> None:
+    margins = MARGINS(0, 0, 0, 0)
+    windll.dwmapi.DwmExtendFrameIntoClientArea(HWND, byref(margins))
 
 
 def get_accent_color() -> str:
     """returns current accent color of windows
     code provided by Zane (Zingzy) https://github.com/Zingzy
     """
     key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, r"Software\Microsoft\Windows\DWM")
```

### Comparing `pywinstyles-1.7/pywinstyles.egg-info/PKG-INFO` & `pywinstyles-1.8/pywinstyles.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinstyles
-Version: 1.7
+Version: 1.8
 Summary:  Customize window styles in windows 11
 Home-page: https://github.com/Akascape/py-window-styles
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: window-styles,pywinstyles,pywindowstyles,customtkinter,tkinter,python-window-themes,gui,python-gui,pyqt,title-bar,title-bar-color,windows-themes,wxpython,windows11
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -78,19 +78,23 @@
 ### Get Windows Accent Color
 ```python
 default_color = pywinstyles.get_accent_color() # returns hex color string
 ```
 
 ### Set opacity of individual widgets
 ```python
-pywinstyes.set_opacity(widget_id, value=0.5)
+pywinstyles.set_opacity(widget_id, value=0.5)
 ```
 
 ### Make a color transparent inside widget
 ```python
-pywinstyes.set_opacity(widget_id, color="white")
+pywinstyles.set_opacity(widget_id, color="white")
+```
+### Add file DND feature to widgets
+```python
+def drop_func(file):
+  print(file) 
+pywinstyles.apply_dnd(widget_id, frop_func)
 ```
-
 **Hope this package can help in UI development with python**
 
 **Author: Akash Bora**
-
```

### Comparing `pywinstyles-1.7/setup.cfg` & `pywinstyles-1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7977 696e 7374 796c 6573 0d0a   = pywinstyles..
-00000020: 7665 7273 696f 6e20 3d20 312e 370d 0a64  version = 1.7..d
+00000020: 7665 7273 696f 6e20 3d20 312e 380d 0a64  version = 1.8..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2043 7573  escription = Cus
 00000040: 746f 6d69 7a65 2077 696e 646f 7720 7374  tomize window st
 00000050: 796c 6573 2069 6e20 7769 6e64 6f77 7320  yles in windows 
 00000060: 3131 0d0a 6c6f 6e67 5f64 6573 6372 6970  11..long_descrip
 00000070: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000080: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000090: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `pywinstyles-1.7/setup.py` & `pywinstyles-1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'pywinstyles',
-    version = '1.7',
+    version = '1.8',
     description = " Customize window styles in windows 11",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/py-window-styles",
```

