# Comparing `tmp/magictk-0.0.2.46.tar.gz` & `tmp/magictk-0.0.2.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.46.tar", last modified: Sun Apr 21 10:06:33 2024, max compression
+gzip compressed data, was "magictk-0.0.2.47.tar", last modified: Sun Apr 21 14:23:31 2024, max compression
```

## Comparing `magictk-0.0.2.46.tar` & `magictk-0.0.2.47.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 10:06:33.911550 magictk-0.0.2.46/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-21 10:06:33.000000 magictk-0.0.2.46/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-21 10:06:33.911550 magictk-0.0.2.46/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-21 10:06:33.000000 magictk-0.0.2.46/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 10:06:33.907550 magictk-0.0.2.46/magictk/
--rw-r--r--   0 root         (0) root         (0)      400 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3253 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    13450 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11146 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12040 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/mtk.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5893 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0)    22329 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     8925 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/scrollbar.py
--rw-r--r--   0 root         (0) root         (0)     6077 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10213 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 10:06:33.907550 magictk-0.0.2.46/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      592 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-21 10:06:33.000000 magictk-0.0.2.46/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-21 10:06:33.911550 magictk-0.0.2.46/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-21 10:06:33.000000 magictk-0.0.2.46/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 14:23:31.601804 magictk-0.0.2.47/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-21 14:23:31.000000 magictk-0.0.2.47/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-21 14:23:31.601804 magictk-0.0.2.47/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-21 14:23:31.000000 magictk-0.0.2.47/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 14:23:31.597803 magictk-0.0.2.47/magictk/
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3253 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11146 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12040 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5893 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0)    22329 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     7112 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/scrollbar.py
+-rw-r--r--   0 root         (0) root         (0)     6077 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 14:23:31.601804 magictk-0.0.2.47/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      592 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-21 14:23:31.000000 magictk-0.0.2.47/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-21 14:23:31.601804 magictk-0.0.2.47/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-21 14:23:31.000000 magictk-0.0.2.47/setup.py
```

### Comparing `magictk-0.0.2.46/PKG-INFO` & `magictk-0.0.2.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.46
+Version: 0.0.2.47
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.46/README.md` & `magictk-0.0.2.47/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/_window_ctl.py` & `magictk-0.0.2.47/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/_window_size.py` & `magictk-0.0.2.47/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/basicwindow.py` & `magictk-0.0.2.47/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/button.py` & `magictk-0.0.2.47/magictk/button.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/checkbox.py` & `magictk-0.0.2.47/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/color_tmpl.py` & `magictk-0.0.2.47/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/entry.py` & `magictk-0.0.2.47/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/fontconfig.py` & `magictk-0.0.2.47/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/icon.ico` & `magictk-0.0.2.47/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/photoload.py` & `magictk-0.0.2.47/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/progressbar.py` & `magictk-0.0.2.47/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/res.pickle` & `magictk-0.0.2.47/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/scrollbar.py` & `magictk-0.0.2.47/magictk/scrollbar.py`

 * *Files 26% similar despite different names*

```diff
@@ -55,17 +55,18 @@
                 self.__fill_obj[rid+"_pos"].append([px, py])
                 self.__fill_obj[rid+"_pos2"].append([y_n, x_n])
 
                 x_n += 1
             y_n += 1
 
     def __init__(self, master=None, root_anim=None, w=None, h=8, colors="primary", color_list: dict = None, allh=100,
-                 maxh=50):
+                 maxh=50, callback=lambda obj, val: None):
         self._r_allh = allh
         self._r_maxh = maxh
+        self.callback = callback
         self.w = 8
         self.h = h
         self.__master = master
         self.colors = colors
         if (color_list is not None):
             self.color = color_list
         if (root_anim == None):
@@ -121,15 +122,15 @@
                         self.color["background"], self.color["border_base"], int((1-self.border_info[self.__fill_obj["bottomside_pos2"][i][0]][self.__fill_obj["bottomside_pos2"][i][1]]/255)*1000)/1000))
             self.update_pos()
 
         def mouse_move(event: tkinter.Event):
             delta_y = event.y-self.scroll_y
             self.scroll_y = min(self.h-self.bar_len,
                                 max(0, self.scroll_y+delta_y-self.move_start))
-            print(self.get())
+            self.callback(self, self.get())
             self.update_pos()
 
         def mouse_release(event: tkinter.Event):
             for i in range(len(self.__fill_obj["upside"])):
                 self.canvas.itemconfig(
                     self.__fill_obj["upside"][i], fill=color_tmpl.mix_color(
                         self.color["background"], self.color["border_light"], int((1-self.border_info[self.__fill_obj["upside_pos2"][i][0]][self.__fill_obj["upside_pos2"][i][1]]/255)*1000)/1000))
@@ -148,60 +149,12 @@
         self.__draw_corner(0, 0, 0, self.scroll_y,
                            self.color["border_light"], "upside", bgcolor=self.color["background"])
         self.__fill_obj["fgbar"] = [
             self.canvas.create_rectangle(1, 4+self.scroll_y, self.w-1, self.scroll_y+self.bar_len-4+1, width=0, fill=self.color["border_light"])]
         self.__draw_corner(0, 1, 0, self.scroll_y+self.bar_len-4+1,
                            self.color["border_light"], "bottomside", bgcolor=self.color["background"])
 
-    def __update_pixel(self):
-        self.__move_progress_pixel = max(4, int((self.w-6)*self.progress))
-
-    def add_progress(self, n):
-        self.progress = max(min(self.progress+n, 1.0), 0.0)
-        self.__update_pixel()
-
-    def set_progress(self, n):
-        self.progress = max(min(n, 1.0), 0.0)
-        self.__update_pixel()
-
-    def bind_anim(self):
-        def anim_magictk():
-            if (int(self.__progress_pixel) < int(self.__move_progress_pixel)):
-                if (self.__move_progress_pixel-self.__progress_pixel > 8):
-                    self.__progress_pixel += 8
-                else:
-                    add_n = int(
-                        (self.__progress_pixel-self.__move_progress_pixel)/2)
-                    if (add_n <= 2):
-                        self.__progress_pixel = self.__move_progress_pixel
-                    else:
-                        self.__progress_pixel += add_n
-                self.__update_prog()
-            elif (int(self.__progress_pixel) > int(self.__move_progress_pixel)):
-                if (self.__progress_pixel-self.__move_progress_pixel > 8):
-                    self.__progress_pixel -= 8
-                else:
-                    add_n = int(
-                        (self.__progress_pixel-self.__move_progress_pixel)/2)
-                    if (add_n <= 2):
-                        self.__progress_pixel = self.__move_progress_pixel
-                    else:
-                        self.__progress_pixel -= add_n
-                self.__update_prog()
-
-        def anim_normal(*args):
-            self.__root.after(anim_normal, 16)
-
-        try:
-            self.__root.anim == 0
-        except:
-            self.__root.after(anim_normal, 16)
-        else:
-            if (anim_magictk not in self.__root.anim):
-                self.__root.anim.append(anim_magictk)
-                self.__anim_obj_id = self.__root.anim[-1]
-
     def get(self):
         if (self.scroll_y+self.bar_len >= self.h):
             return self._r_allh
         else:
             return int(min(self.scroll_y*self.y_size, self._r_allh))
```

### Comparing `magictk-0.0.2.46/magictk/select.py` & `magictk-0.0.2.47/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/submenu.py` & `magictk-0.0.2.47/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/window.py` & `magictk-0.0.2.47/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk/workspace.py` & `magictk-0.0.2.47/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/magictk.egg-info/PKG-INFO` & `magictk-0.0.2.47/magictk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.46
+Version: 0.0.2.47
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.46/magictk.egg-info/SOURCES.txt` & `magictk-0.0.2.47/magictk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.46/setup.py` & `magictk-0.0.2.47/setup.py`

 * *Files identical despite different names*

