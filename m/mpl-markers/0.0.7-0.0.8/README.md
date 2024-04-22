# Comparing `tmp/mpl_markers-0.0.7.tar.gz` & `tmp/mpl_markers-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_markers-0.0.7.tar", last modified: Sat Apr 20 16:13:13 2024, max compression
+gzip compressed data, was "mpl_markers-0.0.8.tar", last modified: Mon Apr 22 01:31:36 2024, max compression
```

## Comparing `mpl_markers-0.0.7.tar` & `mpl_markers-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 16:13:13.116762 mpl_markers-0.0.7/
--rw-rw-rw-   0        0        0     1058 2023-07-19 22:42:52.000000 mpl_markers-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       34 2023-07-19 22:42:52.000000 mpl_markers-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4208 2024-04-20 16:13:13.116762 mpl_markers-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3379 2024-04-20 16:06:21.000000 mpl_markers-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 16:13:13.085512 mpl_markers-0.0.7/mpl_markers/
--rw-rw-rw-   0        0        0       23 2024-01-29 04:35:13.000000 mpl_markers-0.0.7/mpl_markers/__init__.py
--rw-rw-rw-   0        0        0    33814 2024-04-20 15:58:16.000000 mpl_markers-0.0.7/mpl_markers/artists.py
--rw-rw-rw-   0        0        0     3904 2024-04-20 15:29:51.000000 mpl_markers-0.0.7/mpl_markers/interactive.py
--rw-rw-rw-   0        0        0    28047 2024-04-20 15:58:16.000000 mpl_markers-0.0.7/mpl_markers/markers.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:13:13.101138 mpl_markers-0.0.7/mpl_markers/style/
--rw-rw-rw-   0        0        0     1175 2024-04-20 15:04:31.000000 mpl_markers-0.0.7/mpl_markers/style/default.json
--rw-rw-rw-   0        0        0     3735 2024-03-31 04:01:33.000000 mpl_markers-0.0.7/mpl_markers/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:13:13.116762 mpl_markers-0.0.7/mpl_markers.egg-info/
--rw-rw-rw-   0        0        0     4208 2024-04-20 16:13:13.000000 mpl_markers-0.0.7/mpl_markers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2024-04-20 16:13:13.000000 mpl_markers-0.0.7/mpl_markers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 16:13:13.000000 mpl_markers-0.0.7/mpl_markers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-20 16:13:13.000000 mpl_markers-0.0.7/mpl_markers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-20 16:13:13.000000 mpl_markers-0.0.7/mpl_markers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      837 2024-04-20 16:12:39.000000 mpl_markers-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-20 16:13:13.116762 mpl_markers-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0       55 2024-01-29 04:35:13.000000 mpl_markers-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 16:13:13.101138 mpl_markers-0.0.7/tests/
--rw-rw-rw-   0        0        0     8240 2024-04-20 15:37:20.000000 mpl_markers-0.0.7/tests/test_markers.py
+drwxrwxrwx   0        0        0        0 2024-04-22 01:31:36.465136 mpl_markers-0.0.8/
+-rw-rw-rw-   0        0        0     1058 2023-07-19 22:42:52.000000 mpl_markers-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       34 2023-07-19 22:42:52.000000 mpl_markers-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4370 2024-04-22 01:31:36.445989 mpl_markers-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3539 2024-04-22 01:29:31.000000 mpl_markers-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 01:31:36.402298 mpl_markers-0.0.8/mpl_markers/
+-rw-rw-rw-   0        0        0       23 2024-01-29 04:35:13.000000 mpl_markers-0.0.8/mpl_markers/__init__.py
+-rw-rw-rw-   0        0        0    33791 2024-04-22 01:21:46.000000 mpl_markers-0.0.8/mpl_markers/artists.py
+-rw-rw-rw-   0        0        0     4322 2024-04-21 23:13:06.000000 mpl_markers-0.0.8/mpl_markers/interactive.py
+-rw-rw-rw-   0        0        0    28076 2024-04-22 01:17:56.000000 mpl_markers-0.0.8/mpl_markers/markers.py
+drwxrwxrwx   0        0        0        0 2024-04-22 01:31:36.445989 mpl_markers-0.0.8/mpl_markers/style/
+-rw-rw-rw-   0        0        0     1175 2024-04-20 15:04:31.000000 mpl_markers-0.0.8/mpl_markers/style/default.json
+-rw-rw-rw-   0        0        0     3735 2024-03-31 04:01:33.000000 mpl_markers-0.0.8/mpl_markers/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 01:31:36.445989 mpl_markers-0.0.8/mpl_markers.egg-info/
+-rw-rw-rw-   0        0        0     4370 2024-04-22 01:31:36.000000 mpl_markers-0.0.8/mpl_markers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2024-04-22 01:31:36.000000 mpl_markers-0.0.8/mpl_markers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 01:31:36.000000 mpl_markers-0.0.8/mpl_markers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-22 01:31:36.000000 mpl_markers-0.0.8/mpl_markers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-22 01:31:36.000000 mpl_markers-0.0.8/mpl_markers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      837 2024-04-22 01:24:25.000000 mpl_markers-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-22 01:31:36.466138 mpl_markers-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0       55 2024-01-29 04:35:13.000000 mpl_markers-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 01:31:36.445989 mpl_markers-0.0.8/tests/
+-rw-rw-rw-   0        0        0     7852 2024-04-22 01:20:07.000000 mpl_markers-0.0.8/tests/test_markers.py
```

### Comparing `mpl_markers-0.0.7/LICENSE.txt` & `mpl_markers-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpl_markers-0.0.7/PKG-INFO` & `mpl_markers-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl-markers
-Version: 0.0.7
+Version: 0.0.8
 Summary: interactive marker support for matplotlib
 Author-email: Rick Lyon <rlyon14@gmail.com>
 Project-URL: repository, https://github.com/ricklyon/mpl_markers
 Keywords: matplotlib,markers,interactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -46,19 +46,21 @@
 fig, ax = plt.subplots(1,1)
 x1 = np.linspace(-2*np.pi, 2*np.pi, 1000)
 
 ax.plot(x1, np.sin(x1)*np.cos(x1)**2)
 
 mplm.line_marker(x=0)
 ```
-In GUI backends (i.e. Qt5Agg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
+In interactive matplotlib backends (i.e. QtAgg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
 generated in Jupyter Notebooks.
 
 ![example1](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example1.gif)
 
+Additional markers can be added by using Shift+Left Mouse button. The active marker can be removed from the plot by pressing the Delete key.
+
 ### Axis Markers
 Add an axis marker that moves freely on the canvas:
 ```python
 ax.xaxis.set_major_formatter(lambda x, pos: '{:.2f}$\pi$'.format(x/np.pi))
 mplm.axis_marker(x=0, y=-0.2)
 ```
```

### Comparing `mpl_markers-0.0.7/README.md` & `mpl_markers-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,19 +26,21 @@
 fig, ax = plt.subplots(1,1)
 x1 = np.linspace(-2*np.pi, 2*np.pi, 1000)
 
 ax.plot(x1, np.sin(x1)*np.cos(x1)**2)
 
 mplm.line_marker(x=0)
 ```
-In GUI backends (i.e. Qt5Agg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
+In interactive matplotlib backends (i.e. QtAgg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
 generated in Jupyter Notebooks.
 
 ![example1](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example1.gif)
 
+Additional markers can be added by using Shift+Left Mouse button. The active marker can be removed from the plot by pressing the Delete key.
+
 ### Axis Markers
 Add an axis marker that moves freely on the canvas:
 ```python
 ax.xaxis.set_major_formatter(lambda x, pos: '{:.2f}$\pi$'.format(x/np.pi))
 mplm.axis_marker(x=0, y=-0.2)
 ```
```

### Comparing `mpl_markers-0.0.7/mpl_markers/artists.py` & `mpl_markers-0.0.8/mpl_markers/artists.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,25 +301,25 @@
         self._idx = idx
         self._xd = np.real(self._xdata[idx])
         self._yd = np.real(self._ydata[idx])
 
         # pad values in display coordinates (pixels)
         label_xpad = 10 * self.axes.figure.dpi / 100 if not self.yline else 0
 
-        # hide marker if data is not finite or NaN
-        if not np.isfinite(self._yd) or not np.isfinite(self._xd):
+        # get label position in display coordinates. Use the line axes instead of the class axes since
+        # the line may belong to another twinx/y axes and have different scaling.
+        xl, yl = utils.data2display(self.data_line.axes, (self._xd, self._yd))
+
+        # hide marker if data is not finite or is NaN
+        if np.any(~np.isfinite([self._yd, self._xd, xl, yl])):
             self.set_hidden(True)
             return
         else:
             self.set_hidden(False)
 
-        # get label position in display coordinates. Use the line axes instead of the class axes since
-        # the line may belong to another twinx/y axes and have different scaling.
-        xl, yl = utils.data2display(self.data_line.axes, (self._xd, self._yd))
-
         # set label to left side of axes if yline is active
         xl = 0 if self.yline else xl
 
         if self.ylabel:
             # set the x position to the data point location plus a small pad (in display coordinates)
             xd_lbl = self._alias_xdata[idx] if np.any(self._alias_xdata) else self._xd
             txt = utils.yformatter(
@@ -756,15 +756,15 @@
             controls if line markers are placed by the x value ('x'), the y value ('y'), or by both ('xy').
         """
 
         # override the placement mode if lines aren't monotonic
         if not self._monotonic_xdata and x and y:
             mode = "xy"
 
-        use_alias = bool(mode == "x" and not disp and np.any(self._alias_xdata))
+        use_alias = not disp and np.any(self._alias_xdata)
         # save the arguments to update the marker position when the axes bbox changes later
         self._position_args = (x, y, disp, mode)
 
         # set the positions for each of the line labels
         xd_yd = np.zeros((2, len(self.lines)))
         self._xlbl = None
```

### Comparing `mpl_markers-0.0.7/mpl_markers/interactive.py` & `mpl_markers-0.0.8/mpl_markers/interactive.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,20 +78,29 @@
         return
 
     axes._marker_move = False
 
     m = utils.get_event_marker(axes, event)
     active_marker = axes.marker_active
 
+    # create a new marker
     if m is None and (active_marker is None or axes.figure._marker_hold):
-        markers.line_marker(x, y, axes=axes)
+        # attempt to create a pcolormesh marker if there are no lines on the plot,
+        # if the plot doesn't have a colormesh object, this will return None.
+        if not len(axes.lines):
+            markers.mesh_marker(x, y, axes=axes)
+        # if there are lines on the plot, create a line marker
+        else:
+            markers.line_marker(x, y, axes=axes)
         markers.draw_all(axes)
+    # change the active marker
     elif m is not None:
         markers.set_active(axes, m)
         markers.draw_all(axes)
+    # move the active marker
     elif active_marker is not None:
         markers.move_active(x, y, axes=axes, call_handler=True)
         markers.draw_active(axes)
     else:
         return
```

### Comparing `mpl_markers-0.0.7/mpl_markers/markers.py` & `mpl_markers-0.0.8/mpl_markers/markers.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,14 +376,15 @@
     axes = axes._marker_axes
 
     for m in axes.markers:
         m.remove()
 
     # clear marker list and active marker
     axes.markers = []
+    axes._marker_lines = []
     axes.marker_active = None
 
 
 def remove(axes: Axes = None, marker: artists.MarkerArtist = None):
     """
     Removes a marker from the axes. If no marker is provided, removes the active marker.
     """
```

### Comparing `mpl_markers-0.0.7/mpl_markers/style/default.json` & `mpl_markers-0.0.8/mpl_markers/style/default.json`

 * *Files identical despite different names*

### Comparing `mpl_markers-0.0.7/mpl_markers/utils.py` & `mpl_markers-0.0.8/mpl_markers/utils.py`

 * *Files identical despite different names*

### Comparing `mpl_markers-0.0.7/mpl_markers.egg-info/PKG-INFO` & `mpl_markers-0.0.8/mpl_markers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl-markers
-Version: 0.0.7
+Version: 0.0.8
 Summary: interactive marker support for matplotlib
 Author-email: Rick Lyon <rlyon14@gmail.com>
 Project-URL: repository, https://github.com/ricklyon/mpl_markers
 Keywords: matplotlib,markers,interactive
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -46,19 +46,21 @@
 fig, ax = plt.subplots(1,1)
 x1 = np.linspace(-2*np.pi, 2*np.pi, 1000)
 
 ax.plot(x1, np.sin(x1)*np.cos(x1)**2)
 
 mplm.line_marker(x=0)
 ```
-In GUI backends (i.e. Qt5Agg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
+In interactive matplotlib backends (i.e. QtAgg), the marker can be dragged to any location along the data line, or moved incrementally with the left/right arrow keys. Interactive markers are not supported for static inline figures 
 generated in Jupyter Notebooks.
 
 ![example1](https://raw.githubusercontent.com/ricklyon/mpl_markers/main/docs/img/example1.gif)
 
+Additional markers can be added by using Shift+Left Mouse button. The active marker can be removed from the plot by pressing the Delete key.
+
 ### Axis Markers
 Add an axis marker that moves freely on the canvas:
 ```python
 ax.xaxis.set_major_formatter(lambda x, pos: '{:.2f}$\pi$'.format(x/np.pi))
 mplm.axis_marker(x=0, y=-0.2)
 ```
```

### Comparing `mpl_markers-0.0.7/pyproject.toml` & `mpl_markers-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpl-markers"
-version = "0.0.7"
+version = "0.0.8"
 description = "interactive marker support for matplotlib"
 readme = "README.md"
 authors = [{ name = "Rick Lyon", email = "rlyon14@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mpl_markers-0.0.7/tests/test_markers.py` & `mpl_markers-0.0.8/tests/test_markers.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,43 +71,25 @@
 
     # @unittest.skip
     def test_alias(self):
         fig, (ax1) = plt.subplots(1, 1)
         ax1.set_title("test_alias")
         x1_pi = np.linspace(0, 2, 1000)
         x1 = x1_pi * np.pi
-        # x2 = np.linspace(0, np.pi/2, 1000)
 
         d = np.exp(1j * x1)
-        # d[700:750]  = np.nan
-
         ax1.plot(np.real(d), np.imag(d))
 
         # set marker to angle. The xdata for the marker is the real component of d, so to set the angle we need to specify the index
-        angle1 = 3 / 4
-        angle2 = -1 / 4
+        angle1 = 3 / 2
 
         def yfmt(x, y, idx):
-            return "{:.3f}$\pi$".format(y)
-
-        def xfmt(x, y, idx):
             return "{:.3f}$\pi$".format(x)
 
-        mplm.line_marker(
-            x=angle1, yline=True, alias_xdata=x1_pi, yformatter=yfmt, xformatter=xfmt
-        )
-
-        mplm.line_marker(
-            x=angle2,
-            yline=True,
-            alias_xdata=x1_pi,
-            yformatter="{:.3f}$\pi$",
-            xformatter="{:.3f}$\pi$",
-        )
-
+        mplm.line_marker(x=angle1, alias_xdata=x1_pi, yformatter=yfmt, xline=False)
         plt.show()
 
     # @unittest.skip
     def test_marker_properties(self):
         fig, ax = plt.subplots(1, 1)
         ax.set_title("test_marker_properties")
         x2 = np.linspace(-3 * np.pi, 3 * np.pi, 400)
@@ -173,14 +155,15 @@
     def test_polar2(self):
         fig, axes = plt.subplots(1, 1, subplot_kw=dict(polar=True))
 
         theta = np.linspace(-180, 180, 200)
         theta_rad = np.deg2rad(theta)
 
         axes.plot(theta_rad, np.abs(np.sin(theta_rad)))
+        axes.set_ylim([0.5, 1])
 
         m = mplm.line_marker(x=-np.pi / 2)
         plt.show()
 
     # @unittest.skip
     def test_axis_markers(sef):
         fig, ax = plt.subplots(1, 1)
```

