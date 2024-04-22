# Comparing `tmp/python-nvd3-0.8.0.tar.gz` & `tmp/python-nvd3-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-nvd3-0.8.0.tar", last modified: Thu Aug 15 11:05:22 2013, max compression
+gzip compressed data, was "dist/python-nvd3-0.9.0.tar", last modified: Mon Sep 30 09:40:52 2013, max compression
```

## Comparing `python-nvd3-0.8.0.tar` & `python-nvd3-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/python_nvd3.egg-info/
--rw-rw-r--   0 areski    (1000) areski    (1000)       10 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/python_nvd3.egg-info/requires.txt
--rw-rw-r--   0 areski    (1000) areski    (1000)        1 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/python_nvd3.egg-info/namespace_packages.txt
--rw-rw-r--   0 areski    (1000) areski    (1000)      899 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/python_nvd3.egg-info/SOURCES.txt
--rw-rw-r--   0 areski    (1000) areski    (1000)        1 2013-04-27 18:48:10.000000 python-nvd3-0.8.0/python_nvd3.egg-info/not-zip-safe
--rw-rw-r--   0 areski    (1000) areski    (1000)       37 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/python_nvd3.egg-info/entry_points.txt
--rw-rw-r--   0 areski    (1000) areski    (1000)        1 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/python_nvd3.egg-info/dependency_links.txt
--rw-rw-r--   0 areski    (1000) areski    (1000)        5 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/python_nvd3.egg-info/top_level.txt
--rw-rw-r--   0 areski    (1000) areski    (1000)     5134 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/python_nvd3.egg-info/PKG-INFO
--rw-r--r--   0 areski    (1000) areski    (1000)     1136 2013-04-08 11:09:58.000000 python-nvd3-0.8.0/MIT-LICENSE.txt
--rw-rw-r--   0 areski    (1000) areski    (1000)     3283 2013-06-05 15:05:36.000000 python-nvd3-0.8.0/README.rst
--rw-rw-r--   0 areski    (1000) areski    (1000)       89 2013-04-16 14:39:51.000000 python-nvd3-0.8.0/MANIFEST.in
--rw-rw-r--   0 areski    (1000) areski    (1000)       59 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/setup.cfg
-drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/nvd3/
--rw-rw-r--   0 areski    (1000) areski    (1000)    17233 2013-08-15 11:03:11.000000 python-nvd3-0.8.0/nvd3/NVD3Chart.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     3333 2013-07-09 12:20:11.000000 python-nvd3-0.8.0/nvd3/multiBarChart.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     2667 2013-04-27 18:40:30.000000 python-nvd3-0.8.0/nvd3/discreteBarChart.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     3329 2013-04-27 18:41:01.000000 python-nvd3-0.8.0/nvd3/multiBarHorizontalChart.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     2943 2013-07-09 12:20:04.000000 python-nvd3-0.8.0/nvd3/multiBarChart.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     4681 2013-07-09 12:20:11.000000 python-nvd3-0.8.0/nvd3/linePlusBarChart.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     3827 2013-07-09 12:20:07.000000 python-nvd3-0.8.0/nvd3/cumulativeLineChart.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     4241 2013-07-09 12:20:11.000000 python-nvd3-0.8.0/nvd3/cumulativeLineChart.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     4114 2013-07-10 14:17:49.000000 python-nvd3-0.8.0/nvd3/lineChart.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     4006 2013-07-09 12:20:11.000000 python-nvd3-0.8.0/nvd3/stackedAreaChart.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     3111 2013-06-12 11:42:05.000000 python-nvd3-0.8.0/nvd3/discreteBarChart.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     1278 2013-08-15 11:04:42.000000 python-nvd3-0.8.0/nvd3/__init__.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     3607 2013-07-09 12:20:02.000000 python-nvd3-0.8.0/nvd3/stackedAreaChart.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     3729 2013-07-09 12:20:05.000000 python-nvd3-0.8.0/nvd3/lineWithFocusChart.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     4463 2013-05-31 16:37:35.000000 python-nvd3-0.8.0/nvd3/scatterChart.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     4388 2013-07-11 15:42:20.000000 python-nvd3-0.8.0/nvd3/lineChart.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)    15210 2013-08-15 10:57:10.000000 python-nvd3-0.8.0/nvd3/NVD3Chart.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     4959 2013-06-12 11:42:05.000000 python-nvd3-0.8.0/nvd3/scatterChart.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     2876 2013-07-09 21:45:41.000000 python-nvd3-0.8.0/nvd3/__init__.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     3795 2013-06-12 11:42:05.000000 python-nvd3-0.8.0/nvd3/multiBarHorizontalChart.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     4043 2013-07-09 12:20:11.000000 python-nvd3-0.8.0/nvd3/lineWithFocusChart.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     4283 2013-07-09 12:20:09.000000 python-nvd3-0.8.0/nvd3/linePlusBarChart.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     4279 2013-05-30 12:31:54.000000 python-nvd3-0.8.0/nvd3/pieChart.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     4383 2013-06-12 11:42:05.000000 python-nvd3-0.8.0/nvd3/pieChart.pyc
--rw-rw-r--   0 areski    (1000) areski    (1000)     5286 2013-05-30 16:23:06.000000 python-nvd3-0.8.0/setup.py
--rw-rw-r--   0 areski    (1000) areski    (1000)     5134 2013-08-15 11:05:22.000000 python-nvd3-0.8.0/PKG-INFO
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2013-09-30 09:40:52.000000 python-nvd3-0.9.0/
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2013-09-30 09:40:52.000000 python-nvd3-0.9.0/python_nvd3.egg-info/
+-rw-rw-r--   0 areski    (1000) areski    (1000)       10 2013-09-30 09:40:51.000000 python-nvd3-0.9.0/python_nvd3.egg-info/requires.txt
+-rw-rw-r--   0 areski    (1000) areski    (1000)        1 2013-09-30 09:40:51.000000 python-nvd3-0.9.0/python_nvd3.egg-info/namespace_packages.txt
+-rw-rw-r--   0 areski    (1000) areski    (1000)      899 2013-09-30 09:40:52.000000 python-nvd3-0.9.0/python_nvd3.egg-info/SOURCES.txt
+-rw-rw-r--   0 areski    (1000) areski    (1000)        1 2013-04-27 18:48:10.000000 python-nvd3-0.9.0/python_nvd3.egg-info/not-zip-safe
+-rw-rw-r--   0 areski    (1000) areski    (1000)       37 2013-09-30 09:40:51.000000 python-nvd3-0.9.0/python_nvd3.egg-info/entry_points.txt
+-rw-rw-r--   0 areski    (1000) areski    (1000)        1 2013-09-30 09:40:51.000000 python-nvd3-0.9.0/python_nvd3.egg-info/dependency_links.txt
+-rw-rw-r--   0 areski    (1000) areski    (1000)        5 2013-09-30 09:40:51.000000 python-nvd3-0.9.0/python_nvd3.egg-info/top_level.txt
+-rw-rw-r--   0 areski    (1000) areski    (1000)     5719 2013-09-30 09:40:51.000000 python-nvd3-0.9.0/python_nvd3.egg-info/PKG-INFO
+-rw-r--r--   0 areski    (1000) areski    (1000)     1136 2013-04-08 11:09:58.000000 python-nvd3-0.9.0/MIT-LICENSE.txt
+-rw-rw-r--   0 areski    (1000) areski    (1000)     3732 2013-09-30 09:39:20.000000 python-nvd3-0.9.0/README.rst
+-rw-rw-r--   0 areski    (1000) areski    (1000)       89 2013-04-16 14:39:51.000000 python-nvd3-0.9.0/MANIFEST.in
+-rw-rw-r--   0 areski    (1000) areski    (1000)       59 2013-09-30 09:40:52.000000 python-nvd3-0.9.0/setup.cfg
+drwxrwxr-x   0 areski    (1000) areski    (1000)        0 2013-09-30 09:40:52.000000 python-nvd3-0.9.0/nvd3/
+-rw-rw-r--   0 areski    (1000) areski    (1000)    17414 2013-09-30 09:32:04.000000 python-nvd3-0.9.0/nvd3/NVD3Chart.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     3333 2013-07-09 12:20:11.000000 python-nvd3-0.9.0/nvd3/multiBarChart.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     2667 2013-04-27 18:40:30.000000 python-nvd3-0.9.0/nvd3/discreteBarChart.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     3329 2013-04-27 18:41:01.000000 python-nvd3-0.9.0/nvd3/multiBarHorizontalChart.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     2943 2013-07-09 12:20:04.000000 python-nvd3-0.9.0/nvd3/multiBarChart.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     4681 2013-07-09 12:20:11.000000 python-nvd3-0.9.0/nvd3/linePlusBarChart.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     3827 2013-07-09 12:20:07.000000 python-nvd3-0.9.0/nvd3/cumulativeLineChart.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     4241 2013-07-09 12:20:11.000000 python-nvd3-0.9.0/nvd3/cumulativeLineChart.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     4114 2013-07-10 14:17:49.000000 python-nvd3-0.9.0/nvd3/lineChart.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     4006 2013-07-09 12:20:11.000000 python-nvd3-0.9.0/nvd3/stackedAreaChart.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     3111 2013-06-12 11:42:05.000000 python-nvd3-0.9.0/nvd3/discreteBarChart.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     1278 2013-09-30 09:39:39.000000 python-nvd3-0.9.0/nvd3/__init__.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     3607 2013-07-09 12:20:02.000000 python-nvd3-0.9.0/nvd3/stackedAreaChart.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     3729 2013-07-09 12:20:05.000000 python-nvd3-0.9.0/nvd3/lineWithFocusChart.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     4463 2013-05-31 16:37:35.000000 python-nvd3-0.9.0/nvd3/scatterChart.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     4388 2013-07-11 15:42:20.000000 python-nvd3-0.9.0/nvd3/lineChart.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)    15258 2013-09-30 09:15:14.000000 python-nvd3-0.9.0/nvd3/NVD3Chart.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     4959 2013-06-12 11:42:05.000000 python-nvd3-0.9.0/nvd3/scatterChart.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     2876 2013-08-15 11:09:13.000000 python-nvd3-0.9.0/nvd3/__init__.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     3795 2013-06-12 11:42:05.000000 python-nvd3-0.9.0/nvd3/multiBarHorizontalChart.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     4043 2013-07-09 12:20:11.000000 python-nvd3-0.9.0/nvd3/lineWithFocusChart.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     4283 2013-07-09 12:20:09.000000 python-nvd3-0.9.0/nvd3/linePlusBarChart.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     4279 2013-05-30 12:31:54.000000 python-nvd3-0.9.0/nvd3/pieChart.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     4383 2013-06-12 11:42:05.000000 python-nvd3-0.9.0/nvd3/pieChart.pyc
+-rw-rw-r--   0 areski    (1000) areski    (1000)     5286 2013-05-30 16:23:06.000000 python-nvd3-0.9.0/setup.py
+-rw-rw-r--   0 areski    (1000) areski    (1000)     5719 2013-09-30 09:40:52.000000 python-nvd3-0.9.0/PKG-INFO
```

### Comparing `python-nvd3-0.8.0/python_nvd3.egg-info/SOURCES.txt` & `python-nvd3-0.9.0/python_nvd3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/python_nvd3.egg-info/PKG-INFO` & `python-nvd3-0.9.0/python_nvd3.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-nvd3
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python NVD3
 Home-page: http://github.com/areski/python-nvd3
 Author: Belaid Arezqui
 Author-email: areski@gmail.com
 License: MIT license
 Description: Python Wrapper for NVD3 - It's time for beautiful charts
         ========================================================
@@ -32,14 +32,31 @@
         Install, upgrade and uninstall python-nvd3 with these commands::
         
             $ pip install python-nvd3
             $ pip install --upgrade python-nvd3
             $ pip uninstall python-nvd3
         
         
+        Dependecies
+        -----------
+        
+        You will "bower" installed in order to install D3 and NvD3, see bower website for futher info : http://bower.io/
+        
+        Bower depends on Node and npm. It's installed globally using npm::
+        
+            npm install -g bower
+        
+        Then in your directory where you will use python-nvd3, just type the following::
+        
+            $ bower install d3
+            $ bower install nvd3
+        
+        This will create a directory "bower_components" where d3 & nvd3 will be installed.
+        
+        
         Usage
         -----
         
         After installation use python-nvd3 as follows ::
         
             from nvd3 import pieChart
```

### Comparing `python-nvd3-0.8.0/MIT-LICENSE.txt` & `python-nvd3-0.9.0/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/README.rst` & `python-nvd3-0.9.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -24,14 +24,31 @@
 Install, upgrade and uninstall python-nvd3 with these commands::
 
     $ pip install python-nvd3
     $ pip install --upgrade python-nvd3
     $ pip uninstall python-nvd3
 
 
+Dependecies
+-----------
+
+You will "bower" installed in order to install D3 and NvD3, see bower website for futher info : http://bower.io/
+
+Bower depends on Node and npm. It's installed globally using npm::
+
+    npm install -g bower
+
+Then in your directory where you will use python-nvd3, just type the following::
+
+    $ bower install d3
+    $ bower install nvd3
+
+This will create a directory "bower_components" where d3 & nvd3 will be installed.
+
+
 Usage
 -----
 
 After installation use python-nvd3 as follows ::
 
     from nvd3 import pieChart
```

### Comparing `python-nvd3-0.8.0/nvd3/NVD3Chart.py` & `python-nvd3-0.9.0/nvd3/NVD3Chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,21 +130,28 @@
 
         if 'resize' in kwargs and kwargs["resize"]:
             self.resize = True
 
         self.show_legend = kwargs.get("show_legend", True)
         self.show_labels = kwargs.get("show_labels", True)
 
+        #CDN http://cdnjs.com/libraries/nvd3/ needs to make sure it's up to date
         self.header_css = [
             '<link media="all" href="%s" type="text/css" rel="stylesheet" />\n' % h for h in
-            ('http://nvd3.org/src/nv.d3.css',)
+            (
+                './bower_components/nvd3/src/nv.d3.css',
+            )
         ]
+
         self.header_js = [
             '<script src="%s" type="text/javascript"></script>\n' % h for h in
-            ('http://nvd3.org/lib/d3.v2.js', 'http://nvd3.org/nv.d3.js')
+            (
+                './bower_components/d3/d3.min.js',
+                './bower_components/nvd3/nv.d3.min.js'
+            )
         ]
 
     def add_serie(self, y, x, name=None, extra={}, **kwargs):
         """
         add serie - Series are list of data that will be plotted
         y {1, 2, 3, 4, 5} / x {1, 2, 3, 4, 5}
```

### Comparing `python-nvd3-0.8.0/nvd3/multiBarChart.pyc` & `python-nvd3-0.9.0/nvd3/multiBarChart.pyc`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/discreteBarChart.py` & `python-nvd3-0.9.0/nvd3/discreteBarChart.py`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/multiBarHorizontalChart.py` & `python-nvd3-0.9.0/nvd3/multiBarHorizontalChart.py`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/multiBarChart.py` & `python-nvd3-0.9.0/nvd3/multiBarChart.py`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/linePlusBarChart.pyc` & `python-nvd3-0.9.0/nvd3/linePlusBarChart.pyc`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/cumulativeLineChart.py` & `python-nvd3-0.9.0/nvd3/cumulativeLineChart.py`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/cumulativeLineChart.pyc` & `python-nvd3-0.9.0/nvd3/cumulativeLineChart.pyc`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/lineChart.py` & `python-nvd3-0.9.0/nvd3/lineChart.py`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/stackedAreaChart.pyc` & `python-nvd3-0.9.0/nvd3/stackedAreaChart.pyc`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/discreteBarChart.pyc` & `python-nvd3-0.9.0/nvd3/discreteBarChart.pyc`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/__init__.py` & `python-nvd3-0.9.0/nvd3/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Python-nvd3 is a Python wrapper for NVD3 graph library.
 NVD3 is an attempt to build re-usable charts and chart components
 for d3.js without taking away the power that d3.js gives you.
 
 Project location : https://github.com/areski/python-nvd3
 """
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 
 from .lineChart import lineChart
 from .pieChart import pieChart
 from .lineWithFocusChart import lineWithFocusChart
 from .stackedAreaChart import stackedAreaChart
 from .multiBarHorizontalChart import multiBarHorizontalChart
```

### Comparing `python-nvd3-0.8.0/nvd3/stackedAreaChart.py` & `python-nvd3-0.9.0/nvd3/stackedAreaChart.py`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/lineWithFocusChart.py` & `python-nvd3-0.9.0/nvd3/lineWithFocusChart.py`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/scatterChart.py` & `python-nvd3-0.9.0/nvd3/scatterChart.py`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/lineChart.pyc` & `python-nvd3-0.9.0/nvd3/lineChart.pyc`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/NVD3Chart.pyc` & `python-nvd3-0.9.0/nvd3/NVD3Chart.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a bfb3 0c52 6300 0000 0000 0000  .......Rc.......
+00000000: 03f3 0d0a 1f41 4952 6300 0000 0000 0000  .....AIRc.......
 00000010: 0003 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000020: 005a 0000 6401 0064 0200 6c01 006d 0200  .Z..d..d..l..m..
 00000030: 5a02 0001 6401 0064 0300 6c03 006d 0400  Z...d..d..l..m..
 00000040: 5a04 0001 6401 0064 0400 6c05 005a 0500  Z...d..d..l..Z..
 00000050: 6405 005a 0600 6406 0065 0600 165a 0700  d..Z..d..e...Z..
 00000060: 6407 0064 0800 8401 005a 0800 6409 0066  d..d.....Z..d..f
 00000070: 0000 640a 0084 0000 8300 0059 5a09 0064  ..d........YZ..d
@@ -191,761 +191,764 @@
 00000be0: 0a20 2020 2020 2020 2043 6f6e 7374 7275  .        Constru
 00000bf0: 6374 6f72 0a20 2020 2020 2020 2073 0800  ctor.        s..
 00000c00: 0000 2564 2025 6220 2559 6901 0000 0073  ..%d %b %Yi....s
 00000c10: 0700 0000 6368 6172 7425 6474 0700 0000  ....chart%dt....
 00000c20: 7374 6163 6b65 6474 0600 0000 7265 7369  stackedt....resi
 00000c30: 7a65 740b 0000 0073 686f 775f 6c65 6765  zet....show_lege
 00000c40: 6e64 740b 0000 0073 686f 775f 6c61 6265  ndt....show_labe
-00000c50: 6c73 731d 0000 0068 7474 703a 2f2f 6e76  lss....http://nv
-00000c60: 6433 2e6f 7267 2f73 7263 2f6e 762e 6433  d3.org/src/nv.d3
-00000c70: 2e63 7373 7340 0000 003c 6c69 6e6b 206d  .csss@...<link m
-00000c80: 6564 6961 3d22 616c 6c22 2068 7265 663d  edia="all" href=
-00000c90: 2225 7322 2074 7970 653d 2274 6578 742f  "%s" type="text/
-00000ca0: 6373 7322 2072 656c 3d22 7374 796c 6573  css" rel="styles
-00000cb0: 6865 6574 2220 2f3e 0a73 1c00 0000 6874  heet" />.s....ht
-00000cc0: 7470 3a2f 2f6e 7664 332e 6f72 672f 6c69  tp://nvd3.org/li
-00000cd0: 622f 6433 2e76 322e 6a73 7318 0000 0068  b/d3.v2.jss....h
-00000ce0: 7474 703a 2f2f 6e76 6433 2e6f 7267 2f6e  ttp://nvd3.org/n
-00000cf0: 762e 6433 2e6a 7373 3200 0000 3c73 6372  v.d3.jss2...<scr
-00000d00: 6970 7420 7372 633d 2225 7322 2074 7970  ipt src="%s" typ
-00000d10: 653d 2274 6578 742f 6a61 7661 7363 7269  e="text/javascri
-00000d20: 7074 223e 3c2f 7363 7269 7074 3e0a 4e28  pt"></script>.N(
-00000d30: 0100 0000 731d 0000 0068 7474 703a 2f2f  ....s....http://
-00000d40: 6e76 6433 2e6f 7267 2f73 7263 2f6e 762e  nvd3.org/src/nv.
-00000d50: 6433 2e63 7373 2802 0000 0073 1c00 0000  d3.css(....s....
-00000d60: 6874 7470 3a2f 2f6e 7664 332e 6f72 672f  http://nvd3.org/
-00000d70: 6c69 622f 6433 2e76 322e 6a73 7318 0000  lib/d3.v2.jss...
-00000d80: 0068 7474 703a 2f2f 6e76 6433 2e6f 7267  .http://nvd3.org
-00000d90: 2f6e 762e 6433 2e6a 7328 1500 0000 7409  /nv.d3.js(....t.
-00000da0: 0000 005f 5f63 6c61 7373 5f5f 7408 0000  ...__class__t...
-00000db0: 005f 5f6e 616d 655f 5f74 0500 0000 6d6f  .__name__t....mo
-00000dc0: 6465 6c74 0600 0000 7365 7269 6573 7408  delt....seriest.
-00000dd0: 0000 0061 7869 736c 6973 7452 0100 0000  ...axislistR....
-00000de0: 7412 0000 0074 656d 706c 6174 655f 7061  t....template_pa
-00000df0: 6765 5f6e 7664 3374 1500 0000 7465 6d70  ge_nvd3t....temp
-00000e00: 6c61 7465 5f63 6f6e 7465 6e74 5f6e 7664  late_content_nvd
-00000e10: 3374 1700 0000 6368 6172 7474 6f6f 6c74  3t....charttoolt
-00000e20: 6970 5f64 6174 6566 6f72 6d61 7474 0500  ip_dateformatt..
-00000e30: 0000 636f 756e 7474 0400 0000 6e61 6d65  ..countt....name
-00000e40: 740f 0000 006a 7175 6572 795f 6f6e 5f72  t....jquery_on_r
-00000e50: 6561 6479 740e 0000 0063 6f6c 6f72 5f63  eadyt....color_c
-00000e60: 6174 6567 6f72 7974 0400 0000 5472 7565  ategoryt....True
-00000e70: 5208 0000 0052 0900 0000 7403 0000 0067  R....R....t....g
-00000e80: 6574 520a 0000 0052 0b00 0000 740a 0000  etR....R....t...
-00000e90: 0068 6561 6465 725f 6373 7374 0900 0000  .header_csst....
-00000ea0: 6865 6164 6572 5f6a 7328 0600 0000 7404  header_js(....t.
-00000eb0: 0000 0073 656c 6652 1500 0000 5217 0000  ...selfR....R...
-00000ec0: 0052 1600 0000 7406 0000 006b 7761 7267  .R....t....kwarg
-00000ed0: 7374 0100 0000 6828 0000 0000 2800 0000  st....h(....(...
-00000ee0: 0073 4d00 0000 2f68 6f6d 652f 6172 6573  .sM.../home/ares
-00000ef0: 6b69 2f70 7562 6c69 635f 6874 6d6c 2f64  ki/public_html/d
-00000f00: 6a61 6e67 6f2f 4d79 5072 6f6a 6563 7473  jango/MyProjects
-00000f10: 2f6e 7664 332f 7079 7468 6f6e 2d6e 7664  /nvd3/python-nvd
-00000f20: 332f 6e76 6433 2f4e 5644 3343 6861 7274  3/nvd3/NVD3Chart
-00000f30: 2e70 7974 0800 0000 5f5f 696e 6974 5f5f  .pyt....__init__
-00000f40: 6700 0000 732e 0000 0000 060f 0309 0109  g...s...........
-00000f50: 010f 010f 0109 0206 010f 0110 0109 0209  ................
-00000f60: 0206 010c 0216 010c 0216 010c 0215 0115  ................
-00000f70: 0303 011d 0303 0163 0500 0000 0d00 0000  .......c........
-00000f80: 0e00 0000 4b00 0000 7387 0400 007c 0300  ....K...s....|..
-00000f90: 7320 0064 0100 7400 007c 0000 6a01 0083  s .d..t..|..j...
-00000fa0: 0100 6402 0017 167d 0300 6e00 0064 0300  ..d....}..n..d..
-00000fb0: 7c05 006b 0600 7338 0064 0400 7c05 006b  |..k..s8.d..|..k
-00000fc0: 0600 72eb 0064 0400 7c05 006b 0600 725b  ..r..d..|..k..r[
-00000fd0: 007c 0500 6404 0019 725b 007c 0500 6404  .|..d...r[.|..d.
-00000fe0: 0019 7d06 006e 0600 6402 007d 0600 6403  ..}..n..d..}..d.
-00000ff0: 007c 0500 6b06 0072 8400 7c05 0064 0300  .|..k..r..|..d..
-00001000: 1972 8400 7c05 0064 0300 197d 0700 6e06  .r..|..d...}..n.
-00001010: 0064 0500 7d07 0067 0000 7402 007c 0100  .d..}..g..t..|..
-00001020: 8301 0044 5d4b 005c 0200 7d08 007d 0100  ...D]K.\..}..}..
-00001030: 6904 007c 0200 7c08 0019 6406 0036 7c01  i..|..|...d..6|.
-00001040: 0064 0700 367c 0700 6403 0036 7403 007c  .d..6|..d..6t..|
-00001050: 0600 7404 0083 0200 72d8 007c 0600 7c08  ..t.....r..|..|.
-00001060: 0019 6e03 007c 0600 6404 0036 5e02 0071  ..n..|..d..6^..q
-00001070: 9700 7d09 006e 3700 6700 0074 0200 7c01  ..}..n7.g..t..|.
-00001080: 0083 0100 445d 2400 5c02 007d 0800 7d01  ....D]$.\..}..}.
-00001090: 0069 0200 7c02 007c 0800 1964 0600 367c  .i..|..|...d..6|
-000010a0: 0100 6407 0036 5e02 0071 f800 7d09 0069  ..d..6^..q..}..i
-000010b0: 0200 7c09 0064 0800 367c 0300 6409 0036  ..|..d..6|..d..6
-000010c0: 7d0a 0064 0a00 7c05 006b 0600 725d 017c  }..d..|..k..r].|
-000010d0: 0500 640a 0019 725d 017c 0500 640a 0019  ..d...r].|..d...
-000010e0: 7c0a 0064 0a00 3c6e 0000 7c00 006a 0500  |..d..<n..|..j..
-000010f0: 640b 006b 0200 7295 0164 0c00 7c04 006b  d..k..r..d..|..k
-00001100: 0600 7295 017c 0400 640c 0019 7295 017c  ..r..|..d...r..|
-00001110: 0400 640c 0019 7c00 005f 0600 7195 016e  ..d...|.._..q..n
-00001120: 0000 640d 007c 0500 6b06 0072 bc01 7c05  ..d..|..k..r..|.
-00001130: 0064 0d00 1972 bc01 7c05 0064 0d00 197c  .d...r..|..d...|
-00001140: 0a00 640e 003c 6e0a 0064 0f00 7c0a 0064  ..d..<n..d..|..d
-00001150: 0e00 3c64 1000 7c05 006b 0600 72e9 017c  ..<d..|..k..r..|
-00001160: 0500 6410 0019 72e9 0164 1100 7c0a 0064  ..d...r..d..|..d
-00001170: 1000 3c6e 0000 6412 007c 0500 6b06 0072  ..<n..d..|..k..r
-00001180: 0c02 7c05 0064 1200 1972 0c02 6411 007c  ..|..d...r..d..|
-00001190: 0a00 6412 003c 6e00 0064 1300 7c05 006b  ..d..<n..d..|..k
-000011a0: 0600 7233 027c 0500 6413 0019 7233 027c  ..r3.|..d...r3.|
-000011b0: 0500 6413 0019 7c0a 0064 1300 3c6e 0000  ..d...|..d..<n..
-000011c0: 7c04 006a 0700 6414 0083 0100 7252 027c  |..j..d.....rR.|
-000011d0: 0400 6414 0019 7c00 005f 0800 6e00 007c  ..d...|.._..n..|
-000011e0: 0400 6a07 0064 1500 8301 0072 7304 7409  ..j..d.....rs.t.
-000011f0: 007c 0000 5f0a 007c 0000 6a05 0064 0b00  .|.._..|..j..d..
-00001200: 6b03 0072 e303 7c04 0064 1500 1964 1600  k..r..|..d...d..
-00001210: 197d 0b00 7c04 0064 1500 1964 1700 197d  .}..|..d...d...}
-00001220: 0c00 7c0b 0072 af02 6418 0074 0b00 7c0b  ..|..r..d..t..|.
-00001230: 0083 0100 1764 1900 176e 0300 641a 007d  .....d...n..d..}
-00001240: 0b00 7c0c 0072 cf02 641b 0074 0b00 7c0c  ..|..r..d..t..|.
-00001250: 0083 0100 1764 1800 176e 0300 641a 007d  .....d...n..d..}
-00001260: 0c00 7c00 006a 0500 641c 006b 0200 7234  ..|..j..d..k..r4
-00001270: 037c 0000 046a 0c00 740d 0064 1d00 8301  .|...j..t..d....
-00001280: 0064 1e00 177c 0300 1764 1f00 1774 0d00  .d...|...d...t..
-00001290: 6420 0083 0100 1764 2100 177c 0b00 1764  d .....d!..|...d
-000012a0: 2200 177c 0c00 1764 2300 1774 0d00 641d  "..|...d#..t..d.
-000012b0: 0083 0100 1764 2400 1737 025f 0c00 71e3  .....d$..7._..q.
-000012c0: 037c 0000 6a05 0064 2500 6b02 0072 9303  .|..j..d%.k..r..
-000012d0: 7c00 0004 6a0c 0074 0d00 641d 0083 0100  |...j..t..d.....
-000012e0: 6426 0017 7c03 0017 6427 0017 740d 0064  d&..|...d'..t..d
-000012f0: 2000 8301 0017 6421 0017 7c0b 0017 6428   .....d!..|...d(
-00001300: 0017 7c0c 0017 6423 0017 740d 0064 1d00  ..|...d#..t..d..
-00001310: 8301 0017 6424 0017 3702 5f0c 0071 e303  ....d$..7._..q..
-00001320: 7c00 0004 6a0c 0074 0d00 641d 0083 0100  |...j..t..d.....
-00001330: 6426 0017 7c03 0017 6427 0017 740d 0064  d&..|...d'..t..d
-00001340: 2000 8301 0017 6421 0017 7c0b 0017 6422   .....d!..|...d"
-00001350: 0017 7c0c 0017 6423 0017 740d 0064 1d00  ..|...d#..t..d..
-00001360: 8301 0017 6424 0017 3702 5f0c 006e 0000  ....d$..7._..n..
-00001370: 7c00 006a 0500 640b 006b 0200 7273 047c  |..j..d..k..rs.|
-00001380: 0400 6415 0019 6416 0019 7d0b 007c 0400  ..d...d...}..|..
-00001390: 6415 0019 6417 0019 7d0c 007c 0b00 7228  d...d...}..|..r(
-000013a0: 0464 1800 740b 007c 0b00 8301 0017 6419  .d..t..|......d.
-000013b0: 0017 6e03 0064 1a00 7d0b 007c 0c00 7248  ..n..d..}..|..rH
-000013c0: 0464 1b00 740b 007c 0c00 8301 0017 6418  .d..t..|......d.
-000013d0: 0017 6e03 0064 1a00 7d0c 007c 0000 046a  ..n..d..}..|...j
-000013e0: 0c00 6421 007c 0b00 1764 2900 177c 0c00  ..d!.|...d)..|..
-000013f0: 1764 2300 1737 025f 0c00 7173 046e 0000  .d#..7._..qs.n..
-00001400: 7c00 006a 0100 6a0e 007c 0a00 8301 0001  |..j..j..|......
-00001410: 642a 0053 282b 0000 0073 c600 0000 0a20  d*.S(+...s..... 
-00001420: 2020 2020 2020 2061 6464 2073 6572 6965         add serie
-00001430: 202d 2053 6572 6965 7320 6172 6520 6c69   - Series are li
-00001440: 7374 206f 6620 6461 7461 2074 6861 7420  st of data that 
-00001450: 7769 6c6c 2062 6520 706c 6f74 7465 640a  will be plotted.
-00001460: 2020 2020 2020 2020 7920 7b31 2c20 322c          y {1, 2,
-00001470: 2033 2c20 342c 2035 7d20 2f20 7820 7b31   3, 4, 5} / x {1
-00001480: 2c20 322c 2033 2c20 342c 2035 7d0a 0a20  , 2, 3, 4, 5}.. 
-00001490: 2020 2020 2020 2054 4f44 4f3a 2041 6464         TODO: Add
-000014a0: 2064 6f63 2066 6f72 2073 7570 706f 7274   doc for support
-000014b0: 6564 2070 6172 616d 6574 6572 732c 2069  ed parameters, i
-000014c0: 6520 785f 6178 6973 5f64 6174 652c 2073  e x_axis_date, s
-000014d0: 6861 7065 2c20 7369 7a65 0a0a 2020 2020  hape, size..    
-000014e0: 2020 2020 7308 0000 0053 6572 6965 2025      s....Serie %
-000014f0: 6469 0100 0000 7405 0000 0073 6861 7065  di....t....shape
-00001500: 7404 0000 0073 697a 6574 0600 0000 6369  t....sizet....ci
-00001510: 7263 6c65 7401 0000 0078 7401 0000 0079  rclet....xt....y
-00001520: 7406 0000 0076 616c 7565 7374 0300 0000  t....valuest....
-00001530: 6b65 7974 0400 0000 7479 7065 7408 0000  keyt....typet...
-00001540: 0070 6965 4368 6172 7474 0a00 0000 636f  .pieChartt....co
-00001550: 6c6f 725f 6c69 7374 7405 0000 0079 6178  lor_listt....yax
-00001560: 6973 7405 0000 0079 4178 6973 7401 0000  ist....yAxist...
-00001570: 0031 7403 0000 0062 6172 7404 0000 0074  .1t....bart....t
-00001580: 7275 6574 0800 0000 6469 7361 626c 6564  ruet....disabled
-00001590: 7405 0000 0063 6f6c 6f72 740b 0000 0064  t....colort....d
-000015a0: 6174 655f 666f 726d 6174 7407 0000 0074  ate_formatt....t
-000015b0: 6f6f 6c74 6970 7407 0000 0079 5f73 7461  ooltipt....y_sta
-000015c0: 7274 7405 0000 0079 5f65 6e64 7401 0000  rtt....y_endt...
-000015d0: 0027 7304 0000 0027 202b 2052 0600 0000  .'s....' + R....
-000015e0: 7304 0000 0020 2b20 2774 1000 0000 6c69  s.... + 't....li
-000015f0: 6e65 506c 7573 4261 7243 6861 7274 6903  nePlusBarCharti.
-00001600: 0000 0073 1000 0000 6966 286b 6579 2e69  ...s....if(key.i
-00001610: 6e64 6578 4f66 2827 730b 0000 0027 2920  ndexOf('s....') 
-00001620: 3e20 2d31 2029 7b0a 6904 0000 0073 0800  > -1 ){.i....s..
-00001630: 0000 7661 7220 7920 3d20 7317 0000 0020  ..var y = s.... 
-00001640: 5374 7269 6e67 2867 7261 7068 2e70 6f69  String(graph.poi
-00001650: 6e74 2e79 2920 7302 0000 003b 0a73 0200  nt.y) s....;.s..
-00001660: 0000 7d0a 7413 0000 0063 756d 756c 6174  ..}.t....cumulat
-00001670: 6976 654c 696e 6543 6861 7274 730b 0000  iveLineCharts...
-00001680: 0069 6628 6b65 7920 3d3d 2027 7304 0000  .if(key == 's...
-00001690: 0027 297b 0a73 0b00 0000 2053 7472 696e  .'){.s.... Strin
-000016a0: 6728 6529 2073 1300 0000 2053 7472 696e  g(e) s.... Strin
-000016b0: 6728 652e 706f 696e 742e 7929 204e 280f  g(e.point.y) N(.
-000016c0: 0000 0074 0300 0000 6c65 6e52 0f00 0000  ...t....lenR....
-000016d0: 7409 0000 0065 6e75 6d65 7261 7465 740a  t....enumeratet.
-000016e0: 0000 0069 7369 6e73 7461 6e63 6574 0400  ...isinstancet..
-000016f0: 0000 6c69 7374 520e 0000 0052 2900 0000  ..listR....R)...
-00001700: 5219 0000 0052 1300 0000 5218 0000 0074  R....R....R....t
-00001710: 1300 0000 6375 7374 6f6d 5f74 6f6f 6c74  ....custom_toolt
-00001720: 6970 5f66 6c61 6774 0300 0000 7374 7274  ip_flagt....strt
-00001730: 1800 0000 746f 6f6c 7469 705f 636f 6e64  ....tooltip_cond
-00001740: 6974 696f 6e5f 7374 7269 6e67 5204 0000  ition_stringR...
-00001750: 0074 0600 0000 6170 7065 6e64 280d 0000  .t....append(...
-00001760: 0052 1c00 0000 5224 0000 0052 2300 0000  .R....R$...R#...
-00001770: 5215 0000 0074 0500 0000 6578 7472 6152  R....t....extraR
-00001780: 1d00 0000 7405 0000 0063 7369 7a65 7406  ....t....csizet.
-00001790: 0000 0063 7368 6170 6574 0100 0000 6974  ...cshapet....it
-000017a0: 0500 0000 7365 7269 6574 0d00 0000 6461  ....seriet....da
-000017b0: 7461 5f6b 6579 7661 6c75 6574 0600 0000  ta_keyvaluet....
-000017c0: 5f73 7461 7274 7404 0000 005f 656e 6428  _startt...._end(
-000017d0: 0000 0000 2800 0000 0073 4d00 0000 2f68  ....(....sM.../h
-000017e0: 6f6d 652f 6172 6573 6b69 2f70 7562 6c69  ome/areski/publi
-000017f0: 635f 6874 6d6c 2f64 6a61 6e67 6f2f 4d79  c_html/django/My
-00001800: 5072 6f6a 6563 7473 2f6e 7664 332f 7079  Projects/nvd3/py
-00001810: 7468 6f6e 2d6e 7664 332f 6e76 6433 2f4e  thon-nvd3/nvd3/N
-00001820: 5644 3343 6861 7274 2e70 7974 0900 0000  VD3Chart.pyt....
-00001830: 6164 645f 7365 7269 6592 0000 0073 6800  add_serie....sh.
-00001840: 0000 0008 0601 1a03 1801 1601 0d02 0601  ................
-00001850: 1601 0d02 0601 0305 5e02 3702 1404 1601  ........^.7.....
-00001860: 1102 0f01 1601 1304 1601 1102 0a02 1601  ................
-00001870: 0d02 1601 0d02 1601 1102 0f01 1002 0f01  ................
-00001880: 0902 0f01 0e01 0e01 2001 2002 0f01 0702  ........ . .....
-00001890: 4901 0f01 0702 4902 0702 4902 0f01 0e01  I.....I...I.....
-000018a0: 0e01 2001 2001 0701 1e02 6302 0000 0002  .. . .....c.....
-000018b0: 0000 0002 0000 0043 0000 0073 1300 0000  .......C...s....
-000018c0: 7400 007c 0100 8301 007c 0000 5f01 0064  t..|.....|.._..d
-000018d0: 0100 5328 0200 0000 7310 0000 0053 6574  ..S(....s....Set
-000018e0: 2047 7261 7068 2068 6569 6768 744e 2802   Graph heightN(.
-000018f0: 0000 0052 3d00 0000 7406 0000 0068 6569  ...R=...t....hei
-00001900: 6768 7428 0200 0000 521c 0000 0052 4900  ght(....R....RI.
-00001910: 0000 2800 0000 0028 0000 0000 734d 0000  ..(....(....sM..
-00001920: 002f 686f 6d65 2f61 7265 736b 692f 7075  ./home/areski/pu
-00001930: 626c 6963 5f68 746d 6c2f 646a 616e 676f  blic_html/django
-00001940: 2f4d 7950 726f 6a65 6374 732f 6e76 6433  /MyProjects/nvd3
-00001950: 2f70 7974 686f 6e2d 6e76 6433 2f6e 7664  /python-nvd3/nvd
-00001960: 332f 4e56 4433 4368 6172 742e 7079 7410  3/NVD3Chart.pyt.
-00001970: 0000 0073 6574 5f67 7261 7068 5f68 6569  ...set_graph_hei
-00001980: 6768 74ee 0000 0073 0200 0000 0002 6302  ght....s......c.
-00001990: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
-000019a0: 1300 0000 7400 007c 0100 8301 007c 0000  ....t..|.....|..
-000019b0: 5f01 0064 0100 5328 0200 0000 730f 0000  _..d..S(....s...
-000019c0: 0053 6574 2047 7261 7068 2077 6964 7468  .Set Graph width
-000019d0: 4e28 0200 0000 523d 0000 0074 0500 0000  N(....R=...t....
-000019e0: 7769 6474 6828 0200 0000 521c 0000 0052  width(....R....R
-000019f0: 4b00 0000 2800 0000 0028 0000 0000 734d  K...(....(....sM
-00001a00: 0000 002f 686f 6d65 2f61 7265 736b 692f  .../home/areski/
-00001a10: 7075 626c 6963 5f68 746d 6c2f 646a 616e  public_html/djan
-00001a20: 676f 2f4d 7950 726f 6a65 6374 732f 6e76  go/MyProjects/nv
-00001a30: 6433 2f70 7974 686f 6e2d 6e76 6433 2f6e  d3/python-nvd3/n
-00001a40: 7664 332f 4e56 4433 4368 6172 742e 7079  vd3/NVD3Chart.py
-00001a50: 740f 0000 0073 6574 5f67 7261 7068 5f77  t....set_graph_w
-00001a60: 6964 7468 f200 0000 7302 0000 0000 0263  idth....s......c
-00001a70: 0200 0000 0200 0000 0200 0000 4300 0000  ............C...
-00001a80: 730d 0000 007c 0100 7c00 005f 0000 6401  s....|..|.._..d.
-00001a90: 0053 2802 0000 0073 1300 0000 5365 7420  .S(....s....Set 
-00001aa0: 636f 6e74 6169 6e65 7268 6561 6465 724e  containerheaderN
-00001ab0: 2801 0000 0074 0f00 0000 636f 6e74 6169  (....t....contai
-00001ac0: 6e65 7268 6561 6465 7228 0200 0000 521c  nerheader(....R.
-00001ad0: 0000 0052 4d00 0000 2800 0000 0028 0000  ...RM...(....(..
-00001ae0: 0000 734d 0000 002f 686f 6d65 2f61 7265  ..sM.../home/are
-00001af0: 736b 692f 7075 626c 6963 5f68 746d 6c2f  ski/public_html/
-00001b00: 646a 616e 676f 2f4d 7950 726f 6a65 6374  django/MyProject
-00001b10: 732f 6e76 6433 2f70 7974 686f 6e2d 6e76  s/nvd3/python-nv
-00001b20: 6433 2f6e 7664 332f 4e56 4433 4368 6172  d3/nvd3/NVD3Char
-00001b30: 742e 7079 7413 0000 0073 6574 5f63 6f6e  t.pyt....set_con
-00001b40: 7461 696e 6572 6865 6164 6572 f600 0000  tainerheader....
-00001b50: 7302 0000 0000 0263 0200 0000 0200 0000  s......c........
-00001b60: 0200 0000 4300 0000 730d 0000 007c 0100  ....C...s....|..
-00001b70: 7c00 005f 0000 6401 0053 2802 0000 0073  |.._..d..S(....s
-00001b80: 0d00 0000 5365 7420 6461 7465 2066 616c  ....Set date fal
-00001b90: 674e 2801 0000 0074 0900 0000 6461 7465  gN(....t....date
-00001ba0: 5f66 6c61 6728 0200 0000 521c 0000 0052  _flag(....R....R
-00001bb0: 4f00 0000 2800 0000 0028 0000 0000 734d  O...(....(....sM
-00001bc0: 0000 002f 686f 6d65 2f61 7265 736b 692f  .../home/areski/
-00001bd0: 7075 626c 6963 5f68 746d 6c2f 646a 616e  public_html/djan
-00001be0: 676f 2f4d 7950 726f 6a65 6374 732f 6e76  go/MyProjects/nv
-00001bf0: 6433 2f70 7974 686f 6e2d 6e76 6433 2f6e  d3/python-nvd3/n
-00001c00: 7664 332f 4e56 4433 4368 6172 742e 7079  vd3/NVD3Chart.py
-00001c10: 740d 0000 0073 6574 5f64 6174 655f 666c  t....set_date_fl
-00001c20: 6167 fa00 0000 7302 0000 0000 0263 0200  ag....s......c..
-00001c30: 0000 0200 0000 0200 0000 4300 0000 730d  ..........C...s.
-00001c40: 0000 007c 0100 7c00 005f 0000 6401 0053  ...|..|.._..d..S
-00001c50: 2802 0000 0073 2300 0000 5365 7420 6375  (....s#...Set cu
-00001c60: 7374 6f6d 5f74 6f6f 6c74 6970 5f66 6c61  stom_tooltip_fla
-00001c70: 6720 2620 6461 7465 5f66 6c61 674e 2801  g & date_flagN(.
-00001c80: 0000 0052 3c00 0000 2802 0000 0052 1c00  ...R<...(....R..
-00001c90: 0000 523c 0000 0028 0000 0000 2800 0000  ..R<...(....(...
-00001ca0: 0073 4d00 0000 2f68 6f6d 652f 6172 6573  .sM.../home/ares
-00001cb0: 6b69 2f70 7562 6c69 635f 6874 6d6c 2f64  ki/public_html/d
-00001cc0: 6a61 6e67 6f2f 4d79 5072 6f6a 6563 7473  jango/MyProjects
-00001cd0: 2f6e 7664 332f 7079 7468 6f6e 2d6e 7664  /nvd3/python-nvd
-00001ce0: 332f 6e76 6433 2f4e 5644 3343 6861 7274  3/nvd3/NVD3Chart
-00001cf0: 2e70 7974 1700 0000 7365 745f 6375 7374  .pyt....set_cust
-00001d00: 6f6d 5f74 6f6f 6c74 6970 5f66 6c61 67fe  om_tooltip_flag.
-00001d10: 0000 0073 0200 0000 0002 6301 0000 0001  ...s......c.....
-00001d20: 0000 0001 0000 0043 0000 0073 1100 0000  .......C...s....
-00001d30: 7c00 006a 0000 8300 0001 7c00 006a 0100  |..j......|..j..
-00001d40: 5328 0100 0000 7312 0000 0072 6574 7572  S(....s....retur
-00001d50: 6e20 6874 6d6c 636f 6e74 656e 7428 0200  n htmlcontent(..
-00001d60: 0000 7409 0000 0062 7569 6c64 6874 6d6c  ..t....buildhtml
-00001d70: 740b 0000 0068 746d 6c63 6f6e 7465 6e74  t....htmlcontent
-00001d80: 2801 0000 0052 1c00 0000 2800 0000 0028  (....R....(....(
-00001d90: 0000 0000 734d 0000 002f 686f 6d65 2f61  ....sM.../home/a
-00001da0: 7265 736b 692f 7075 626c 6963 5f68 746d  reski/public_htm
-00001db0: 6c2f 646a 616e 676f 2f4d 7950 726f 6a65  l/django/MyProje
-00001dc0: 6374 732f 6e76 6433 2f70 7974 686f 6e2d  cts/nvd3/python-
-00001dd0: 6e76 6433 2f6e 7664 332f 4e56 4433 4368  nvd3/nvd3/NVD3Ch
-00001de0: 6172 742e 7079 7407 0000 005f 5f73 7472  art.pyt....__str
-00001df0: 5f5f 0201 0000 7304 0000 0000 020a 0163  __....s........c
-00001e00: 0100 0000 0100 0000 0500 0000 4300 0000  ............C...
-00001e10: 733c 0000 007c 0000 6a00 0083 0000 017c  s<...|..j......|
-00001e20: 0000 6a01 0083 0000 017c 0000 6a02 006a  ..j......|..j..j
-00001e30: 0300 6401 007c 0000 6a04 0064 0200 7c00  ..d..|..j..d..|.
-00001e40: 006a 0500 8300 027c 0000 5f06 0064 0300  .j.....|.._..d..
-00001e50: 5328 0400 0000 73d1 0000 0042 7569 6c64  S(....s....Build
-00001e60: 2048 544d 4c20 636f 6e74 656e 7420 6f6e   HTML content on
-00001e70: 6c79 2c20 6e6f 2068 6561 6465 7220 6f72  ly, no header or
-00001e80: 2062 6f64 7920 7461 6773 2e20 546f 2062   body tags. To b
-00001e90: 6520 7573 6566 756c 2074 6869 730a 2020  e useful this.  
-00001ea0: 2020 2020 2020 7769 6c6c 2075 7375 616c        will usual
-00001eb0: 6c79 2072 6571 7569 7265 2074 6865 2061  ly require the a
-00001ec0: 7474 7269 6275 7465 2060 6a75 7165 7279  ttribute `juqery
-00001ed0: 5f6f 6e5f 7265 6164 7960 2074 6f20 6265  _on_ready` to be
-00001ee0: 2073 6574 2077 6869 6368 0a20 2020 2020   set which.     
-00001ef0: 2020 2077 696c 6c20 7772 6170 2074 6865     will wrap the
-00001f00: 206a 7320 696e 2024 2866 756e 6374 696f   js in $(functio
-00001f10: 6e28 297b 3c72 6567 756c 6172 5f6a 733e  n(){<regular_js>
-00001f20: 7d3b 290a 2020 2020 2020 2020 7409 0000  };).        t...
-00001f30: 0063 6f6e 7461 696e 6572 7407 0000 006a  .containert....j
-00001f40: 7363 6861 7274 4e28 0700 0000 740e 0000  schartN(....t...
-00001f50: 0062 7569 6c64 636f 6e74 6169 6e65 7274  .buildcontainert
-00001f60: 0c00 0000 6275 696c 646a 7363 6861 7274  ....buildjschart
-00001f70: 5212 0000 0074 0a00 0000 7375 6273 7469  R....t....substi
-00001f80: 7475 7465 5255 0000 0052 5600 0000 5253  tuteRU...RV...RS
-00001f90: 0000 0028 0100 0000 521c 0000 0028 0000  ...(....R....(..
-00001fa0: 0000 2800 0000 0073 4d00 0000 2f68 6f6d  ..(....sM.../hom
-00001fb0: 652f 6172 6573 6b69 2f70 7562 6c69 635f  e/areski/public_
-00001fc0: 6874 6d6c 2f64 6a61 6e67 6f2f 4d79 5072  html/django/MyPr
-00001fd0: 6f6a 6563 7473 2f6e 7664 332f 7079 7468  ojects/nvd3/pyth
-00001fe0: 6f6e 2d6e 7664 332f 6e76 6433 2f4e 5644  on-nvd3/nvd3/NVD
-00001ff0: 3343 6861 7274 2e70 7974 0c00 0000 6275  3Chart.pyt....bu
-00002000: 696c 6463 6f6e 7465 6e74 0701 0000 7308  ildcontent....s.
-00002010: 0000 0000 050a 010a 0115 0163 0100 0000  ...........c....
-00002020: 0100 0000 0700 0000 4300 0000 734f 0000  ........C...sO..
-00002030: 007c 0000 6a00 0083 0000 017c 0000 6a01  .|..j......|..j.
-00002040: 0083 0000 017c 0000 6a02 0083 0000 017c  .....|..j......|
-00002050: 0000 6a03 006a 0400 6401 007c 0000 6a05  ..j..j..d..|..j.
-00002060: 0064 0200 7c00 006a 0600 6403 007c 0000  .d..|..j..d..|..
-00002070: 6a07 0083 0003 7c00 005f 0800 6404 0053  j.....|.._..d..S
-00002080: 2805 0000 0073 7e00 0000 4275 696c 6420  (....s~...Build 
-00002090: 7468 6520 4854 4d4c 2070 6167 650a 2020  the HTML page.  
-000020a0: 2020 2020 2020 4372 6561 7465 2074 6865        Create the
-000020b0: 2068 746d 6c68 6561 6465 7220 7769 7468   htmlheader with
-000020c0: 2063 7373 202f 206a 730a 2020 2020 2020   css / js.      
-000020d0: 2020 4372 6561 7465 2068 746d 6c20 7061    Create html pa
-000020e0: 6765 0a20 2020 2020 2020 2041 6464 204a  ge.        Add J
-000020f0: 7320 636f 6465 2066 6f72 206e 7664 330a  s code for nvd3.
-00002100: 2020 2020 2020 2020 7406 0000 0068 6561          t....hea
-00002110: 6465 7252 5500 0000 5256 0000 004e 2809  derRU...RV...N(.
-00002120: 0000 0074 0f00 0000 6275 696c 6468 746d  ...t....buildhtm
-00002130: 6c68 6561 6465 7252 5700 0000 5258 0000  lheaderRW...RX..
-00002140: 0052 1100 0000 5259 0000 0074 0a00 0000  .R....RY...t....
-00002150: 6874 6d6c 6865 6164 6572 5255 0000 0052  htmlheaderRU...R
-00002160: 5600 0000 5253 0000 0028 0100 0000 521c  V...RS...(....R.
-00002170: 0000 0028 0000 0000 2800 0000 0073 4d00  ...(....(....sM.
-00002180: 0000 2f68 6f6d 652f 6172 6573 6b69 2f70  ../home/areski/p
-00002190: 7562 6c69 635f 6874 6d6c 2f64 6a61 6e67  ublic_html/djang
-000021a0: 6f2f 4d79 5072 6f6a 6563 7473 2f6e 7664  o/MyProjects/nvd
-000021b0: 332f 7079 7468 6f6e 2d6e 7664 332f 6e76  3/python-nvd3/nv
-000021c0: 6433 2f4e 5644 3343 6861 7274 2e70 7952  d3/NVD3Chart.pyR
-000021d0: 5200 0000 1101 0000 7308 0000 0000 060a  R.......s.......
-000021e0: 010a 010a 0263 0100 0000 0300 0000 0400  .....c..........
-000021f0: 0000 4300 0000 7353 0000 0064 0100 7c00  ..C...sS...d..|.
-00002200: 005f 0000 7820 007c 0000 6a01 0044 5d15  ._..x .|..j..D].
-00002210: 007d 0100 7c00 0004 6a00 007c 0100 3702  .}..|...j..|..7.
-00002220: 5f00 0071 1300 5778 2000 7c00 006a 0200  _..q..Wx .|..j..
-00002230: 445d 1500 7d02 007c 0000 046a 0000 7c02  D]..}..|...j..|.
-00002240: 0037 025f 0000 7136 0057 6402 0053 2803  .7._..q6.Wd..S(.
-00002250: 0000 0073 1c00 0000 6765 6e65 7261 7465  ...s....generate
-00002260: 2048 544d 4c20 6865 6164 6572 2063 6f6e   HTML header con
-00002270: 7465 6e74 5206 0000 004e 2803 0000 0052  tentR....N(....R
-00002280: 5d00 0000 521a 0000 0052 1b00 0000 2803  ]...R....R....(.
-00002290: 0000 0052 1c00 0000 7403 0000 0063 7373  ...R....t....css
-000022a0: 7402 0000 006a 7328 0000 0000 2800 0000  t....js(....(...
-000022b0: 0073 4d00 0000 2f68 6f6d 652f 6172 6573  .sM.../home/ares
-000022c0: 6b69 2f70 7562 6c69 635f 6874 6d6c 2f64  ki/public_html/d
-000022d0: 6a61 6e67 6f2f 4d79 5072 6f6a 6563 7473  jango/MyProjects
-000022e0: 2f6e 7664 332f 7079 7468 6f6e 2d6e 7664  /nvd3/python-nvd
-000022f0: 332f 6e76 6433 2f4e 5644 3343 6861 7274  3/nvd3/NVD3Chart
-00002300: 2e70 7952 5c00 0000 1d01 0000 730a 0000  .pyR\.......s...
-00002310: 0000 0209 0110 0113 0110 0163 0100 0000  ...........c....
-00002320: 0100 0000 0500 0000 4300 0000 73e7 0000  ........C...s...
-00002330: 007c 0000 6a00 007c 0000 5f01 007c 0000  .|..j..|.._..|..
-00002340: 6a02 0072 5a00 7c00 006a 0200 6401 0019  j..rZ.|..j..d...
-00002350: 6402 006b 0300 7241 007c 0000 046a 0300  d..k..rA.|...j..
-00002360: 6403 007c 0000 6a02 0016 3702 5f03 0071  d..|..j...7._..q
-00002370: 5a00 7c00 0004 6a03 0064 0400 7c00 006a  Z.|...j..d..|..j
-00002380: 0200 1637 025f 0300 6e00 007c 0000 6a04  ...7._..n..|..j.
-00002390: 0072 a800 7c00 006a 0400 6401 0019 6402  .r..|..j..d...d.
-000023a0: 006b 0300 728f 007c 0000 046a 0300 6405  .k..r..|...j..d.
-000023b0: 007c 0000 6a04 0016 3702 5f03 0071 a800  .|..j...7._..q..
-000023c0: 7c00 0004 6a03 0064 0600 7c00 006a 0400  |...j..d..|..j..
-000023d0: 1637 025f 0300 6e00 007c 0000 6a03 0072  .7._..n..|..j..r
-000023e0: c400 6407 007c 0000 6a03 0016 7c00 005f  ..d..|..j...|.._
-000023f0: 0300 6e00 007c 0000 046a 0100 6408 007c  ..n..|...j..d..|
-00002400: 0000 6a05 007c 0000 6a03 0066 0200 1637  ..j..|..j..f...7
-00002410: 025f 0100 6409 0053 280a 0000 0073 1100  ._..d..S(....s..
-00002420: 0000 6765 6e65 7261 7465 2048 544d 4c20  ..generate HTML 
-00002430: 6469 7669 ffff ffff 7401 0000 0025 730b  divi....t....%s.
-00002440: 0000 0077 6964 7468 3a25 7370 783b 7309  ...width:%spx;s.
-00002450: 0000 0077 6964 7468 3a25 733b 730c 0000  ...width:%s;s...
-00002460: 0068 6569 6768 743a 2573 7078 3b73 0a00  .height:%spx;s..
-00002470: 0000 6865 6967 6874 3a25 733b 730a 0000  ..height:%s;s...
-00002480: 0073 7479 6c65 3d22 2573 2273 2200 0000  .style="%s"s"...
-00002490: 3c64 6976 2069 643d 2225 7322 3e3c 7376  <div id="%s"><sv
-000024a0: 6720 2573 3e3c 2f73 7667 3e3c 2f64 6976  g %s></svg></div
-000024b0: 3e0a 4e28 0600 0000 524d 0000 0052 5500  >.N(....RM...RU.
-000024c0: 0000 524b 0000 0074 0500 0000 7374 796c  ..RK...t....styl
-000024d0: 6552 4900 0000 5215 0000 0028 0100 0000  eRI...R....(....
-000024e0: 521c 0000 0028 0000 0000 2800 0000 0073  R....(....(....s
-000024f0: 4d00 0000 2f68 6f6d 652f 6172 6573 6b69  M.../home/areski
-00002500: 2f70 7562 6c69 635f 6874 6d6c 2f64 6a61  /public_html/dja
-00002510: 6e67 6f2f 4d79 5072 6f6a 6563 7473 2f6e  ngo/MyProjects/n
-00002520: 7664 332f 7079 7468 6f6e 2d6e 7664 332f  vd3/python-nvd3/
-00002530: 6e76 6433 2f4e 5644 3343 6861 7274 2e70  nvd3/NVD3Chart.p
-00002540: 7952 5700 0000 2501 0000 7318 0000 0000  yRW...%...s.....
-00002550: 020c 0209 0113 0119 0219 0109 0113 0119  ................
-00002560: 0219 0109 0113 0263 0100 0000 0100 0000  .......c........
-00002570: 0300 0000 4300 0000 7351 0100 007c 0000  ....C...sQ...|..
-00002580: 6a00 0072 4d01 7c00 006a 0100 73e3 007c  j..rM.|..j..s..|
-00002590: 0000 6a02 0064 0100 6b02 0072 8000 7403  ..j..d..k..r..t.
-000025a0: 0064 0200 8301 0064 0300 1774 0300 6404  .d.....d...t..d.
-000025b0: 0083 0100 1764 0500 1774 0300 6404 0083  .....d...t..d...
-000025c0: 0100 177c 0000 6a04 0017 7403 0064 0400  ...|..j...t..d..
-000025d0: 8301 0017 6406 0017 7403 0064 0400 8301  ....d...t..d....
-000025e0: 0017 6407 0017 7403 0064 0200 8301 0017  ..d...t..d......
-000025f0: 6408 0017 7c00 005f 0500 714a 0174 0300  d...|.._..qJ.t..
-00002600: 6402 0083 0100 6403 0017 7403 0064 0400  d.....d...t..d..
-00002610: 8301 0017 6409 0017 7403 0064 0400 8301  ....d...t..d....
-00002620: 0017 640a 0017 7c00 006a 0400 1774 0300  ..d...|..j...t..
-00002630: 6404 0083 0100 1764 0b00 1774 0300 6404  d......d...t..d.
-00002640: 0083 0100 1764 0700 1774 0300 6402 0083  .....d...t..d...
-00002650: 0100 1764 0800 177c 0000 5f05 0071 4d01  ...d...|.._..qM.
-00002660: 7403 0064 0200 8301 0064 0300 1774 0300  t..d.....d...t..
-00002670: 6404 0083 0100 1764 0c00 7c00 006a 0600  d......d..|..j..
-00002680: 1617 7403 0064 0400 8301 0017 640a 0017  ..t..d......d...
-00002690: 7c00 006a 0400 1774 0300 6404 0083 0100  |..j...t..d.....
-000026a0: 1764 0d00 1774 0300 6404 0083 0100 1764  .d...t..d......d
-000026b0: 0700 1774 0300 6402 0083 0100 1764 0800  ...t..d......d..
-000026c0: 177c 0000 5f05 006e 0000 640e 0053 280f  .|.._..n..d..S(.
-000026d0: 0000 0073 2500 0000 6765 6e65 7261 7465  ...s%...generate
-000026e0: 2063 7573 746f 6d20 746f 6f6c 7469 7020   custom tooltip 
-000026f0: 666f 7220 7468 6520 6368 6172 7452 2800  for the chartR(.
-00002700: 0000 6902 0000 0073 3200 0000 6368 6172  ..i....s2...char
-00002710: 742e 746f 6f6c 7469 7043 6f6e 7465 6e74  t.tooltipContent
-00002720: 2866 756e 6374 696f 6e28 6b65 792c 2079  (function(key, y
-00002730: 2c20 652c 2067 7261 7068 2920 7b0a 6903  , e, graph) {.i.
-00002740: 0000 0073 1500 0000 7661 7220 7820 3d20  ...s....var x = 
-00002750: 5374 7269 6e67 286b 6579 293b 0a73 3300  String(key);.s3.
-00002760: 0000 746f 6f6c 7469 705f 7374 7220 3d20  ..tooltip_str = 
-00002770: 273c 6365 6e74 6572 3e3c 623e 272b 782b  '<center><b>'+x+
-00002780: 273c 2f62 3e3c 2f63 656e 7465 723e 2720  '</b></center>' 
-00002790: 2b20 793b 0a73 1400 0000 7265 7475 726e  + y;.s....return
-000027a0: 2074 6f6f 6c74 6970 5f73 7472 3b0a 7304   tooltip_str;.s.
-000027b0: 0000 007d 293b 0a73 1f00 0000 7661 7220  ...});.s....var 
-000027c0: 7820 3d20 5374 7269 6e67 2867 7261 7068  x = String(graph
-000027d0: 2e70 6f69 6e74 2e78 293b 0a73 1f00 0000  .point.x);.s....
-000027e0: 7661 7220 7920 3d20 5374 7269 6e67 2867  var y = String(g
-000027f0: 7261 7068 2e70 6f69 6e74 2e79 293b 0a73  raph.point.y);.s
-00002800: 4200 0000 746f 6f6c 7469 705f 7374 7220  B...tooltip_str 
-00002810: 3d20 273c 6365 6e74 6572 3e3c 623e 272b  = '<center><b>'+
-00002820: 6b65 792b 273c 2f62 3e3c 2f63 656e 7465  key+'</b></cente
-00002830: 723e 2720 2b20 7920 2b20 2720 6174 2027  r>' + y + ' at '
-00002840: 202b 2078 3b0a 7341 0000 0076 6172 2078   + x;.sA...var x
-00002850: 203d 2064 332e 7469 6d65 2e66 6f72 6d61   = d3.time.forma
-00002860: 7428 2725 7327 2928 6e65 7720 4461 7465  t('%s')(new Date
-00002870: 2870 6172 7365 496e 7428 6772 6170 682e  (parseInt(graph.
-00002880: 706f 696e 742e 7829 2929 3b0a 7342 0000  point.x)));.sB..
-00002890: 0074 6f6f 6c74 6970 5f73 7472 203d 2027  .tooltip_str = '
-000028a0: 3c63 656e 7465 723e 3c62 3e27 2b6b 6579  <center><b>'+key
-000028b0: 2b27 3c2f 623e 3c2f 6365 6e74 6572 3e27  +'</b></center>'
-000028c0: 202b 2079 202b 2027 206f 6e20 2720 2b20   + y + ' on ' + 
-000028d0: 783b 0a4e 2807 0000 0052 3c00 0000 524f  x;.N(....R<...RO
-000028e0: 0000 0052 0e00 0000 5204 0000 0052 3e00  ...R....R....R>.
-000028f0: 0000 740c 0000 0063 6861 7274 746f 6f6c  ..t....charttool
-00002900: 7469 7052 1300 0000 2801 0000 0052 1c00  tipR....(....R..
-00002910: 0000 2800 0000 0028 0000 0000 734d 0000  ..(....(....sM..
-00002920: 002f 686f 6d65 2f61 7265 736b 692f 7075  ./home/areski/pu
-00002930: 626c 6963 5f68 746d 6c2f 646a 616e 676f  blic_html/django
-00002940: 2f4d 7950 726f 6a65 6374 732f 6e76 6433  /MyProjects/nvd3
-00002950: 2f70 7974 686f 6e2d 6e76 6433 2f6e 7664  /python-nvd3/nvd
-00002960: 332f 4e56 4433 4368 6172 742e 7079 7414  3/NVD3Chart.pyt.
-00002970: 0000 0062 7569 6c64 5f63 7573 746f 6d5f  ...build_custom_
-00002980: 746f 6f6c 7469 7038 0100 0073 0c00 0000  tooltip8...s....
-00002990: 0002 0901 0901 0f06 5f08 6309 6301 0000  ........_.c.c...
-000029a0: 0007 0000 0009 0000 0043 0000 0073 d403  .........C...s..
-000029b0: 0000 6401 007c 0000 5f00 007c 0000 6a01  ..d..|.._..|..j.
-000029c0: 0072 2400 7c00 0004 6a00 0064 0200 3702  .r$.|...j..d..7.
-000029d0: 5f00 006e 0000 7c00 0004 6a00 0074 0200  _..n..|...j..t..
-000029e0: 8300 0037 025f 0000 7c00 006a 0300 7251  ...7._..|..j..rQ
-000029f0: 007c 0000 046a 0000 6403 0037 025f 0000  .|...j..d..7._..
-00002a00: 6e00 007c 0000 046a 0000 6404 0037 025f  n..|...j..d..7._
-00002a10: 0000 7c00 0004 6a00 0074 0200 6405 0083  ..|...j..t..d...
-00002a20: 0100 6406 007c 0000 6a04 0016 1737 025f  ..d..|..j....7._
-00002a30: 0000 7c00 006a 0400 6407 006b 0300 72c8  ..|..j..d..k..r.
-00002a40: 007c 0000 6a05 000c 72c8 007c 0000 6a06  .|..j...r..|..j.
-00002a50: 0072 c800 7c00 0004 6a00 0074 0200 6405  .r..|...j..t..d.
-00002a60: 0083 0100 6408 007c 0000 6a06 0016 1737  ....d..|..j....7
-00002a70: 025f 0000 71c8 006e 0000 7c00 006a 0700  ._..q..n..|..j..
-00002a80: 72ed 007c 0000 046a 0000 7402 0064 0500  r..|...j..t..d..
-00002a90: 8301 0064 0900 1737 025f 0000 6e00 007c  ...d...7._..n..|
-00002aa0: 0000 6a04 0064 0700 6b03 0072 8801 7889  ..j..d..k..r..x.
-00002ab0: 0074 0800 7c00 006a 0900 6a0a 0083 0000  .t..|..j..j.....
-00002ac0: 8301 0044 5d6f 005c 0200 7d01 007d 0200  ...D]o.\..}..}..
-00002ad0: 7c00 0004 6a00 0074 0200 6405 0083 0100  |...j..t..d.....
-00002ae0: 640a 007c 0100 1617 3702 5f00 0078 4300  d..|....7._..xC.
-00002af0: 7408 007c 0200 6a0a 0083 0000 8301 0044  t..|..j........D
-00002b00: 5d2f 005c 0200 7d03 007d 0400 7c00 0004  ]/.\..}..}..|...
-00002b10: 6a00 0074 0200 640b 0083 0100 640c 007c  j..t..d.....d..|
-00002b20: 0300 7c04 0066 0200 1617 3702 5f00 0071  ..|..f....7._..q
-00002b30: 4e01 5771 1201 576e 0000 7c00 006a 0b00  N.Wq..Wn..|..j..
-00002b40: 72aa 017c 0000 046a 0c00 640d 007c 0000  r..|...j..d..|..
-00002b50: 6a0b 0016 3702 5f0c 006e 0000 7c00 006a  j...7._..n..|..j
-00002b60: 0d00 72cc 017c 0000 046a 0c00 640e 007c  ..r..|...j..d..|
-00002b70: 0000 6a0d 0016 3702 5f0c 006e 0000 640f  ..j...7._..n..d.
-00002b80: 007c 0000 6a0e 0016 7d05 007c 0000 6a04  .|..j...}..|..j.
-00002b90: 0064 0700 6b02 0072 f801 6410 007c 0000  .d..k..r..d..|..
-00002ba0: 6a0e 0016 7d05 006e 0000 7c00 006a 0f00  j...}..n..|..j..
-00002bb0: 6401 006b 0200 7213 0264 1100 7c00 005f  d..k..r..d..|.._
-00002bc0: 0f00 6e00 007c 0000 6a10 0083 0000 017c  ..n..|..j......|
-00002bd0: 0000 046a 0000 7c00 006a 1100 3702 5f00  ...j..|..j..7._.
-00002be0: 007c 0000 6a04 0064 1200 6b03 0072 7f02  .|..j..d..k..r..
-00002bf0: 7c00 006a 1200 7263 027c 0000 046a 0000  |..j..rc.|...j..
-00002c00: 7402 0064 0500 8301 0064 1300 1737 025f  t..d.....d...7._
-00002c10: 0000 717f 027c 0000 046a 0000 7402 0064  ..q..|...j..t..d
-00002c20: 0500 8301 0064 1400 1737 025f 0000 6e00  .....d...7._..n.
-00002c30: 007c 0000 6a04 0064 0700 6b02 0072 cf02  .|..j..d..k..r..
-00002c40: 7c00 006a 1300 72b3 027c 0000 046a 0000  |..j..r..|...j..
-00002c50: 7402 0064 0500 8301 0064 1500 1737 025f  t..d.....d...7._
-00002c60: 0000 71cf 027c 0000 046a 0000 7402 0064  ..q..|...j..t..d
-00002c70: 0500 8301 0064 1600 1737 025f 0000 6e00  .....d...7._..n.
-00002c80: 007c 0000 046a 0000 7402 0064 0500 8301  .|...j..t..d....
-00002c90: 0064 1700 7c00 006a 0e00 1617 7402 0064  .d..|..j....t..d
-00002ca0: 0b00 8301 0017 6418 007c 0500 1617 7402  ......d..|....t.
-00002cb0: 0064 0b00 8301 0017 6419 0017 7402 0064  .d......d...t..d
-00002cc0: 0b00 8301 0017 7c00 006a 0c00 1774 0200  ......|..j...t..
-00002cd0: 640b 0083 0100 1764 1a00 1737 025f 0000  d......d...7._..
-00002ce0: 7c00 006a 1400 7253 037c 0000 046a 0000  |..j..rS.|...j..
-00002cf0: 7402 0064 1b00 8301 0064 1c00 1737 025f  t..d.....d...7._
-00002d00: 0000 6e00 007c 0000 046a 0000 7402 0064  ..n..|...j..t..d
-00002d10: 1b00 8301 0064 1d00 1737 025f 0000 7c00  .....d...7._..|.
-00002d20: 006a 0300 7287 037c 0000 046a 0000 641e  .j..r..|...j..d.
-00002d30: 0037 025f 0000 6e00 0074 1500 6a16 007c  .7._..n..t..j..|
-00002d40: 0000 6a17 0083 0100 7d06 007c 0000 046a  ..j.....}..|...j
-00002d50: 0000 641f 007c 0000 6a0e 007c 0600 6602  ..d..|..j..|..f.
-00002d60: 0016 3702 5f00 007c 0000 6a01 0072 d003  ..7._..|..j..r..
-00002d70: 7c00 0004 6a00 0064 2000 3702 5f00 006e  |...j..d .7._..n
-00002d80: 0000 6421 0053 2822 0000 0073 2600 0000  ..d!.S("...s&...
-00002d90: 6765 6e65 7261 7465 206a 6176 6173 6372  generate javascr
-00002da0: 6970 7420 636f 6465 2066 6f72 2074 6865  ipt code for the
-00002db0: 2063 6861 7274 5206 0000 0073 2100 0000   chartR....s!...
-00002dc0: 0a3c 7363 7269 7074 2074 7970 653d 2274  .<script type="t
-00002dd0: 6578 742f 6a61 7661 7363 7269 7074 223e  ext/javascript">
-00002de0: 0a73 0d00 0000 2428 6675 6e63 7469 6f6e  .s....$(function
-00002df0: 2829 7b73 1900 0000 6e76 2e61 6464 4772  (){s....nv.addGr
-00002e00: 6170 6828 6675 6e63 7469 6f6e 2829 207b  aph(function() {
-00002e10: 0a69 0200 0000 731c 0000 0076 6172 2063  .i....s....var c
-00002e20: 6861 7274 203d 206e 762e 6d6f 6465 6c73  hart = nv.models
-00002e30: 2e25 7328 293b 0a52 2800 0000 7324 0000  .%s();.R(...s$..
-00002e40: 0063 6861 7274 2e63 6f6c 6f72 2864 332e  .chart.color(d3.
-00002e50: 7363 616c 652e 2573 2829 2e72 616e 6765  scale.%s().range
-00002e60: 2829 293b 0a73 1400 0000 6368 6172 742e  ());.s....chart.
-00002e70: 7374 6163 6b65 6428 7472 7565 293b 7309  stacked(true);s.
-00002e80: 0000 0063 6861 7274 2e25 730a 6903 0000  ...chart.%s.i...
-00002e90: 0073 0900 0000 2e25 7328 2573 293b 0a73  .s.....%s(%s);.s
-00002ea0: 1300 0000 2e61 7474 7228 2777 6964 7468  .....attr('width
-00002eb0: 272c 2025 7329 0a73 1400 0000 2e61 7474  ', %s).s.....att
-00002ec0: 7228 2768 6569 6768 7427 2c20 2573 290a  r('height', %s).
-00002ed0: 7307 0000 0064 6174 615f 2573 7313 0000  s....data_%ss...
-00002ee0: 005b 6461 7461 5f25 735b 305d 2e76 616c  .[data_%s[0].val
-00002ef0: 7565 735d 731f 0000 0076 6172 2079 203d  ues]s....var y =
-00002f00: 2053 7472 696e 6728 6772 6170 682e 706f   String(graph.po
-00002f10: 696e 742e 7929 3b0a 7410 0000 0064 6973  int.y);.t....dis
-00002f20: 6372 6574 6542 6172 4368 6172 7473 1800  creteBarCharts..
-00002f30: 0000 6368 6172 742e 7368 6f77 4c65 6765  ..chart.showLege
-00002f40: 6e64 2874 7275 6529 3b0a 7319 0000 0063  nd(true);.s....c
-00002f50: 6861 7274 2e73 686f 774c 6567 656e 6428  hart.showLegend(
-00002f60: 6661 6c73 6529 3b0a 7318 0000 0063 6861  false);.s....cha
-00002f70: 7274 2e73 686f 774c 6162 656c 7328 7472  rt.showLabels(tr
-00002f80: 7565 293b 0a73 1900 0000 6368 6172 742e  ue);.s....chart.
-00002f90: 7368 6f77 4c61 6265 6c73 2866 616c 7365  showLabels(false
-00002fa0: 293b 0a73 1500 0000 6433 2e73 656c 6563  );.s....d3.selec
-00002fb0: 7428 2723 2573 2073 7667 2729 0a73 0b00  t('#%s svg').s..
-00002fc0: 0000 2e64 6174 756d 2825 7329 0a73 1c00  ...datum(%s).s..
-00002fd0: 0000 2e74 7261 6e73 6974 696f 6e28 292e  ...transition().
-00002fe0: 6475 7261 7469 6f6e 2835 3030 290a 730f  duration(500).s.
-00002ff0: 0000 002e 6361 6c6c 2863 6861 7274 293b  ....call(chart);
-00003000: 0a0a 6901 0000 0073 2500 0000 6e76 2e75  ..i....s%...nv.u
-00003010: 7469 6c73 2e77 696e 646f 7752 6573 697a  tils.windowResiz
-00003020: 6528 6368 6172 742e 7570 6461 7465 293b  e(chart.update);
-00003030: 0a73 1100 0000 7265 7475 726e 2063 6861  .s....return cha
-00003040: 7274 3b0a 7d29 3b73 0400 0000 0a7d 293b  rt;.});s.....});
-00003050: 730c 0000 0064 6174 615f 2573 3d25 733b  s....data_%s=%s;
-00003060: 0a73 0900 0000 3c2f 7363 7269 7074 3e4e  .s....</script>N
-00003070: 2818 0000 0052 5600 0000 740d 0000 0074  (....RV...t....t
-00003080: 6167 5f73 6372 6970 745f 6a73 5204 0000  ag_script_jsR...
-00003090: 0052 1600 0000 520e 0000 0052 2900 0000  .R....R....R)...
-000030a0: 5217 0000 0052 0800 0000 523b 0000 0052  R....R....R;...R
-000030b0: 1000 0000 7405 0000 0069 7465 6d73 524b  ....t....itemsRK
-000030c0: 0000 0074 0f00 0000 6433 5f73 656c 6563  ...t....d3_selec
-000030d0: 745f 6578 7472 6152 4900 0000 5215 0000  t_extraRI...R...
-000030e0: 0052 3e00 0000 5263 0000 0052 6200 0000  .R>...Rc...Rb...
-000030f0: 520a 0000 0052 0b00 0000 5209 0000 0074  R....R....R....t
-00003100: 0400 0000 6a73 6f6e 7405 0000 0064 756d  ....jsont....dum
-00003110: 7073 520f 0000 0028 0700 0000 521c 0000  psR....(....R...
-00003120: 0074 0900 0000 6178 6973 5f6e 616d 6574  .t....axis_namet
-00003130: 0100 0000 6174 0400 0000 6174 7472 7405  ....at....attrt.
-00003140: 0000 0076 616c 7565 7405 0000 0064 6174  ...valuet....dat
-00003150: 756d 7409 0000 0073 6572 6965 735f 6a73  umt....series_js
-00003160: 2800 0000 0028 0000 0000 734d 0000 002f  (....(....sM.../
-00003170: 686f 6d65 2f61 7265 736b 692f 7075 626c  home/areski/publ
-00003180: 6963 5f68 746d 6c2f 646a 616e 676f 2f4d  ic_html/django/M
-00003190: 7950 726f 6a65 6374 732f 6e76 6433 2f70  yProjects/nvd3/p
-000031a0: 7974 686f 6e2d 6e76 6433 2f6e 7664 332f  ython-nvd3/nvd3/
-000031b0: 4e56 4433 4368 6172 742e 7079 5258 0000  NVD3Chart.pyRX..
-000031c0: 0055 0100 0073 6000 0000 0003 0901 0901  .U...s`.........
-000031d0: 1202 1202 0901 1202 0f02 2002 1901 0901  .......... .....
-000031e0: 2602 0901 1c07 0f01 2201 1d01 1f01 2e02  &.......".......
-000031f0: 0901 1901 0901 1902 0d01 0f01 1004 0f01  ................
-00003200: 0c02 0a01 1202 0f01 0901 1c02 1c03 0f01  ................
-00003210: 0901 1c02 1c03 0704 5802 0901 1c01 1902  ........X.......
-00003220: 0901 1203 1201 1c01 0901 6305 0000 0006  ..........c.....
-00003230: 0000 0003 0000 0043 0000 0073 9900 0000  .......C...s....
-00003240: 6900 007d 0500 7c03 0072 3600 7c03 0064  i..}..|..r6.|..d
-00003250: 0100 6b02 0072 2500 6402 007c 0500 6403  ..k..r%.d..|..d.
-00003260: 003c 7136 0064 0400 7c03 0016 7c05 0064  .<q6.d..|...|..d
-00003270: 0300 3c6e 0000 7c02 0072 4900 7c02 007c  ..<n..|..rI.|..|
-00003280: 0500 6405 003c 6e00 007c 0400 7288 007c  ..d..<n..|..r..|
-00003290: 0300 7c00 005f 0000 6406 007c 0000 6a00  ..|.._..d..|..j.
-000032a0: 0016 7c05 0064 0300 3c7c 0100 6407 0019  ..|..d..<|..d...
-000032b0: 6408 006b 0200 7288 0074 0100 7c00 005f  d..k..r..t..|.._
-000032c0: 0200 7188 006e 0000 7c05 007c 0000 6a03  ..q..n..|..|..j.
-000032d0: 007c 0100 3c64 0900 5328 0a00 0000 731f  .|..<d..S(....s.
-000032e0: 0000 000a 2020 2020 2020 2020 4372 6561  ....        Crea
-000032f0: 7465 2058 2d61 7869 730a 2020 2020 2020  te X-axis.      
-00003300: 2020 7405 0000 0041 4d5f 504d 732e 0000    t....AM_PMs...
-00003310: 0066 756e 6374 696f 6e28 6429 207b 2072  .function(d) { r
-00003320: 6574 7572 6e20 6765 745f 616d 5f70 6d28  eturn get_am_pm(
-00003330: 7061 7273 6549 6e74 2864 2929 3b20 7d74  parseInt(d)); }t
-00003340: 0a00 0000 7469 636b 466f 726d 6174 7310  ....tickFormats.
-00003350: 0000 0064 332e 666f 726d 6174 2827 2c25  ...d3.format(',%
-00003360: 7327 2974 0900 0000 6178 6973 4c61 6265  s')t....axisLabe
-00003370: 6c73 4300 0000 6675 6e63 7469 6f6e 2864  lsC...function(d
-00003380: 2920 7b20 7265 7475 726e 2064 332e 7469  ) { return d3.ti
-00003390: 6d65 2e66 6f72 6d61 7428 2725 7327 2928  me.format('%s')(
-000033a0: 6e65 7720 4461 7465 2870 6172 7365 496e  new Date(parseIn
-000033b0: 7428 6429 2929 207d 0a69 0000 0000 5223  t(d))) }.i....R#
-000033c0: 0000 004e 2804 0000 0074 0a00 0000 6461  ...N(....t....da
-000033d0: 7465 666f 726d 6174 5218 0000 0074 0b00  teformatR....t..
-000033e0: 0000 785f 6178 6973 5f64 6174 6552 1000  ..x_axis_dateR..
-000033f0: 0000 2806 0000 0052 1c00 0000 5215 0000  ..(....R....R...
-00003400: 0074 0500 0000 6c61 6265 6c74 0600 0000  .t....labelt....
-00003410: 666f 726d 6174 7404 0000 0064 6174 6574  formatt....datet
-00003420: 0400 0000 6178 6973 2800 0000 0028 0000  ....axis(....(..
-00003430: 0000 734d 0000 002f 686f 6d65 2f61 7265  ..sM.../home/are
-00003440: 736b 692f 7075 626c 6963 5f68 746d 6c2f  ski/public_html/
-00003450: 646a 616e 676f 2f4d 7950 726f 6a65 6374  django/MyProject
-00003460: 732f 6e76 6433 2f70 7974 686f 6e2d 6e76  s/nvd3/python-nv
-00003470: 6433 2f6e 7664 332f 4e56 4433 4368 6172  d3/nvd3/NVD3Char
-00003480: 742e 7079 740d 0000 0063 7265 6174 655f  t.pyt....create_
-00003490: 785f 6178 6973 a901 0000 731a 0000 0000  x_axis....s.....
-000034a0: 0406 0106 010c 010d 0211 0206 010d 0306  ................
-000034b0: 0109 0111 0210 010f 0363 0500 0000 0600  .........c......
-000034c0: 0000 0400 0000 4300 0000 735a 0000 0069  ......C...sZ...i
-000034d0: 0000 7d05 007c 0400 721f 007c 0300 721f  ..}..|..r..|..r.
-000034e0: 007c 0300 7c05 0064 0100 3c6e 1700 7c03  .|..|..d..<n..|.
-000034f0: 0072 3600 6402 007c 0300 167c 0500 6401  .r6.d..|...|..d.
-00003500: 003c 6e00 007c 0200 7249 007c 0200 7c05  .<n..|..rI.|..|.
-00003510: 0064 0300 3c6e 0000 7c05 007c 0000 6a00  .d..<n..|..|..j.
-00003520: 007c 0100 3c64 0400 5328 0500 0000 731f  .|..<d..S(....s.
-00003530: 0000 000a 2020 2020 2020 2020 4372 6561  ....        Crea
-00003540: 7465 2059 2d61 7869 730a 2020 2020 2020  te Y-axis.      
-00003550: 2020 5271 0000 0073 1000 0000 6433 2e66    Rq...s....d3.f
-00003560: 6f72 6d61 7428 272c 2573 2729 5272 0000  ormat(',%s')Rr..
-00003570: 004e 2801 0000 0052 1000 0000 2806 0000  .N(....R....(...
-00003580: 0052 1c00 0000 5215 0000 0052 7500 0000  .R....R....Ru...
-00003590: 5276 0000 0074 0d00 0000 6375 7374 6f6d  Rv...t....custom
-000035a0: 5f66 6f72 6d61 7452 7800 0000 2800 0000  _formatRx...(...
-000035b0: 0028 0000 0000 734d 0000 002f 686f 6d65  .(....sM.../home
-000035c0: 2f61 7265 736b 692f 7075 626c 6963 5f68  /areski/public_h
-000035d0: 746d 6c2f 646a 616e 676f 2f4d 7950 726f  tml/django/MyPro
-000035e0: 6a65 6374 732f 6e76 6433 2f70 7974 686f  jects/nvd3/pytho
-000035f0: 6e2d 6e76 6433 2f6e 7664 332f 4e56 4433  n-nvd3/nvd3/NVD3
-00003600: 4368 6172 742e 7079 740d 0000 0063 7265  Chart.pyt....cre
-00003610: 6174 655f 795f 6178 6973 c201 0000 7310  ate_y_axis....s.
-00003620: 0000 0000 0406 020c 010d 0206 0111 0206  ................
-00003630: 010d 034e 2833 0000 0052 0d00 0000 740a  ...N(3...R....t.
-00003640: 0000 005f 5f6d 6f64 756c 655f 5f74 0700  ...__module__t..
-00003650: 0000 5f5f 646f 635f 5f52 1400 0000 5273  ..__doc__R....Rs
-00003660: 0000 0052 0f00 0000 5210 0000 0052 6100  ...R....R....Ra.
-00003670: 0000 5253 0000 0052 5d00 0000 7404 0000  ..RS...R]...t...
-00003680: 004e 6f6e 6552 4900 0000 524b 0000 0052  .NoneRI...RK...R
-00003690: 0e00 0000 5267 0000 0074 0500 0000 4661  ....Rg...t....Fa
-000036a0: 6c73 6552 7400 0000 5209 0000 0052 0800  lseRt...R....R..
-000036b0: 0000 5211 0000 0052 5500 0000 524d 0000  ..R....RU...RM..
-000036c0: 0052 5600 0000 523c 0000 0052 4f00 0000  .RV...R<...RO...
-000036d0: 5262 0000 0052 3e00 0000 5217 0000 0052  Rb...R>...R....R
-000036e0: 2900 0000 5218 0000 0052 6500 0000 5213  )...R....Re...R.
-000036f0: 0000 0074 0d00 0000 785f 6178 6973 5f66  ...t....x_axis_f
-00003700: 6f72 6d61 7452 0a00 0000 520b 0000 0052  ormatR....R....R
-00003710: 1f00 0000 5248 0000 0052 4a00 0000 524c  ....RH...RJ...RL
-00003720: 0000 0052 4e00 0000 5250 0000 0052 5100  ...RN...RP...RQ.
-00003730: 0000 5254 0000 0052 5a00 0000 5252 0000  ..RT...RZ...RR..
-00003740: 0052 5c00 0000 5257 0000 0052 6300 0000  .R\...RW...Rc...
-00003750: 5258 0000 0052 7900 0000 527b 0000 0028  RX...Ry...R{...(
-00003760: 0000 0000 2800 0000 0028 0000 0000 734d  ....(....(....sM
-00003770: 0000 002f 686f 6d65 2f61 7265 736b 692f  .../home/areski/
-00003780: 7075 626c 6963 5f68 746d 6c2f 646a 616e  public_html/djan
-00003790: 676f 2f4d 7950 726f 6a65 6374 732f 6e76  go/MyProjects/nv
-000037a0: 6433 2f70 7974 686f 6e2d 6e76 6433 2f6e  d3/python-nvd3/n
-000037b0: 7664 332f 4e56 4433 4368 6172 742e 7079  vd3/NVD3Chart.py
-000037c0: 5205 0000 0028 0000 0073 5c00 0000 0620  R....(...s\.... 
-000037d0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-000037e0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-000037f0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
-00003800: 0601 0601 0601 0601 0601 0602 122b 0f5c  .............+.\
-00003810: 0904 0904 0904 0c04 0904 0905 090a 090c  ................
-00003820: 0908 0913 091d 0954 1219 6300 0000 0004  .......T..c.....
-00003830: 0000 000b 0000 0043 0000 0073 5900 0000  .......C...sY...
-00003840: 6401 007d 0000 7400 0064 0200 7c00 0064  d..}..t..d..|..d
-00003850: 0300 6404 0083 0002 7d01 007c 0100 6a01  ..d.....}..|..j.
-00003860: 0064 0500 6406 0064 0700 6408 0064 0900  .d..d..d..d..d..
-00003870: 640a 0064 0b00 7402 0064 0c00 640d 0083  d..d..t..d..d...
-00003880: 0204 017c 0100 6a03 0083 0000 5c02 007d  ...|..j.....\..}
-00003890: 0200 7d03 0064 0e00 5328 0f00 0000 732c  ..}..d..S(....s,
-000038a0: 0000 000a 2020 2020 5061 7273 6520 6f70  ....    Parse op
-000038b0: 7469 6f6e 7320 616e 6420 7072 6f63 6573  tions and proces
-000038c0: 7320 636f 6d6d 616e 6473 0a20 2020 2073  s commands.    s
-000038d0: 1800 0000 7573 6167 653a 206e 7664 332e  ....usage: nvd3.
-000038e0: 7079 205b 6f70 7469 6f6e 735d 7405 0000  py [options]t...
-000038f0: 0075 7361 6765 7407 0000 0076 6572 7369  .usaget....versi
-00003900: 6f6e 732c 0000 0070 7974 686f 6e2d 6e76  ons,...python-nv
-00003910: 6433 2030 2e32 2e32 202d 2050 7974 686f  d3 0.2.2 - Pytho
-00003920: 6e20 7772 6170 7065 7220 666f 7220 6e76  n wrapper for nv
-00003930: 6433 2073 0200 0000 2d71 7307 0000 002d  d3 s....-qs....-
-00003940: 2d71 7569 6574 7406 0000 0061 6374 696f  -quiett....actio
-00003950: 6e74 0b00 0000 7374 6f72 655f 6661 6c73  nt....store_fals
-00003960: 6574 0400 0000 6465 7374 7407 0000 0076  et....destt....v
-00003970: 6572 626f 7365 7407 0000 0064 6566 6175  erboset....defau
-00003980: 6c74 7404 0000 0068 656c 7073 1e00 0000  ltt....helps....
-00003990: 646f 6e27 7420 7072 696e 7420 6d65 7373  don't print mess
-000039a0: 6167 6573 2074 6f20 7374 646f 7574 4e28  ages to stdoutN(
-000039b0: 0400 0000 5200 0000 0074 0a00 0000 6164  ....R....t....ad
-000039c0: 645f 6f70 7469 6f6e 5218 0000 0074 0a00  d_optionR....t..
-000039d0: 0000 7061 7273 655f 6172 6773 2804 0000  ..parse_args(...
-000039e0: 0052 8100 0000 7406 0000 0070 6172 7365  .R....t....parse
-000039f0: 7274 0700 0000 6f70 7469 6f6e 7374 0400  rt....optionst..
-00003a00: 0000 6172 6773 2800 0000 0028 0000 0000  ..args(....(....
-00003a10: 734d 0000 002f 686f 6d65 2f61 7265 736b  sM.../home/aresk
-00003a20: 692f 7075 626c 6963 5f68 746d 6c2f 646a  i/public_html/dj
-00003a30: 616e 676f 2f4d 7950 726f 6a65 6374 732f  ango/MyProjects/
-00003a40: 6e76 6433 2f70 7974 686f 6e2d 6e76 6433  nvd3/python-nvd3
-00003a50: 2f6e 7664 332f 4e56 4433 4368 6172 742e  /nvd3/NVD3Chart.
-00003a60: 7079 7405 0000 005f 6d61 696e d501 0000  pyt...._main....
-00003a70: 730c 0000 0000 0506 0115 010f 0112 0107  s...............
-00003a80: 0274 0800 0000 5f5f 6d61 696e 5f5f 280c  .t....__main__(.
-00003a90: 0000 0052 7d00 0000 7408 0000 006f 7074  ...R}...t....opt
-00003aa0: 7061 7273 6552 0000 0000 7406 0000 0073  parseR....t....s
-00003ab0: 7472 696e 6752 0100 0000 5268 0000 0052  tringR....Rh...R
-00003ac0: 1200 0000 5211 0000 0052 0400 0000 5205  ....R....R....R.
-00003ad0: 0000 0052 8e00 0000 520d 0000 0028 0000  ...R....R....(..
-00003ae0: 0000 2800 0000 0028 0000 0000 734d 0000  ..(....(....sM..
-00003af0: 002f 686f 6d65 2f61 7265 736b 692f 7075  ./home/areski/pu
-00003b00: 626c 6963 5f68 746d 6c2f 646a 616e 676f  blic_html/django
-00003b10: 2f4d 7950 726f 6a65 6374 732f 6e76 6433  /MyProjects/nvd3
-00003b20: 2f70 7974 686f 6e2d 6e76 6433 2f6e 7664  /python-nvd3/nvd
-00003b30: 332f 4e56 4433 4368 6172 742e 7079 7408  3/NVD3Chart.pyt.
-00003b40: 0000 003c 6d6f 6475 6c65 3e0a 0000 0073  ...<module>....s
-00003b50: 1600 0000 0602 1001 1001 0c05 060b 0a03  ................
-00003b60: 0c07 13ff 00ae 090e 0c01                 ..........
+00000c50: 6c73 7325 0000 002e 2f62 6f77 6572 5f63  lss%..../bower_c
+00000c60: 6f6d 706f 6e65 6e74 732f 6e76 6433 2f73  omponents/nvd3/s
+00000c70: 7263 2f6e 762e 6433 2e63 7373 7340 0000  rc/nv.d3.csss@..
+00000c80: 003c 6c69 6e6b 206d 6564 6961 3d22 616c  .<link media="al
+00000c90: 6c22 2068 7265 663d 2225 7322 2074 7970  l" href="%s" typ
+00000ca0: 653d 2274 6578 742f 6373 7322 2072 656c  e="text/css" rel
+00000cb0: 3d22 7374 796c 6573 6865 6574 2220 2f3e  ="stylesheet" />
+00000cc0: 0a73 1f00 0000 2e2f 626f 7765 725f 636f  .s...../bower_co
+00000cd0: 6d70 6f6e 656e 7473 2f64 332f 6433 2e6d  mponents/d3/d3.m
+00000ce0: 696e 2e6a 7373 2400 0000 2e2f 626f 7765  in.jss$..../bowe
+00000cf0: 725f 636f 6d70 6f6e 656e 7473 2f6e 7664  r_components/nvd
+00000d00: 332f 6e76 2e64 332e 6d69 6e2e 6a73 7332  3/nv.d3.min.jss2
+00000d10: 0000 003c 7363 7269 7074 2073 7263 3d22  ...<script src="
+00000d20: 2573 2220 7479 7065 3d22 7465 7874 2f6a  %s" type="text/j
+00000d30: 6176 6173 6372 6970 7422 3e3c 2f73 6372  avascript"></scr
+00000d40: 6970 743e 0a4e 2801 0000 0073 2500 0000  ipt>.N(....s%...
+00000d50: 2e2f 626f 7765 725f 636f 6d70 6f6e 656e  ./bower_componen
+00000d60: 7473 2f6e 7664 332f 7372 632f 6e76 2e64  ts/nvd3/src/nv.d
+00000d70: 332e 6373 7328 0200 0000 731f 0000 002e  3.css(....s.....
+00000d80: 2f62 6f77 6572 5f63 6f6d 706f 6e65 6e74  /bower_component
+00000d90: 732f 6433 2f64 332e 6d69 6e2e 6a73 7324  s/d3/d3.min.jss$
+00000da0: 0000 002e 2f62 6f77 6572 5f63 6f6d 706f  ..../bower_compo
+00000db0: 6e65 6e74 732f 6e76 6433 2f6e 762e 6433  nents/nvd3/nv.d3
+00000dc0: 2e6d 696e 2e6a 7328 1500 0000 7409 0000  .min.js(....t...
+00000dd0: 005f 5f63 6c61 7373 5f5f 7408 0000 005f  .__class__t...._
+00000de0: 5f6e 616d 655f 5f74 0500 0000 6d6f 6465  _name__t....mode
+00000df0: 6c74 0600 0000 7365 7269 6573 7408 0000  lt....seriest...
+00000e00: 0061 7869 736c 6973 7452 0100 0000 7412  .axislistR....t.
+00000e10: 0000 0074 656d 706c 6174 655f 7061 6765  ...template_page
+00000e20: 5f6e 7664 3374 1500 0000 7465 6d70 6c61  _nvd3t....templa
+00000e30: 7465 5f63 6f6e 7465 6e74 5f6e 7664 3374  te_content_nvd3t
+00000e40: 1700 0000 6368 6172 7474 6f6f 6c74 6970  ....charttooltip
+00000e50: 5f64 6174 6566 6f72 6d61 7474 0500 0000  _dateformatt....
+00000e60: 636f 756e 7474 0400 0000 6e61 6d65 740f  countt....namet.
+00000e70: 0000 006a 7175 6572 795f 6f6e 5f72 6561  ...jquery_on_rea
+00000e80: 6479 740e 0000 0063 6f6c 6f72 5f63 6174  dyt....color_cat
+00000e90: 6567 6f72 7974 0400 0000 5472 7565 5208  egoryt....TrueR.
+00000ea0: 0000 0052 0900 0000 7403 0000 0067 6574  ...R....t....get
+00000eb0: 520a 0000 0052 0b00 0000 740a 0000 0068  R....R....t....h
+00000ec0: 6561 6465 725f 6373 7374 0900 0000 6865  eader_csst....he
+00000ed0: 6164 6572 5f6a 7328 0600 0000 7404 0000  ader_js(....t...
+00000ee0: 0073 656c 6652 1500 0000 5217 0000 0052  .selfR....R....R
+00000ef0: 1600 0000 7406 0000 006b 7761 7267 7374  ....t....kwargst
+00000f00: 0100 0000 6828 0000 0000 2800 0000 0073  ....h(....(....s
+00000f10: 4d00 0000 2f68 6f6d 652f 6172 6573 6b69  M.../home/areski
+00000f20: 2f70 7562 6c69 635f 6874 6d6c 2f64 6a61  /public_html/dja
+00000f30: 6e67 6f2f 4d79 5072 6f6a 6563 7473 2f6e  ngo/MyProjects/n
+00000f40: 7664 332f 7079 7468 6f6e 2d6e 7664 332f  vd3/python-nvd3/
+00000f50: 6e76 6433 2f4e 5644 3343 6861 7274 2e70  nvd3/NVD3Chart.p
+00000f60: 7974 0800 0000 5f5f 696e 6974 5f5f 6700  yt....__init__g.
+00000f70: 0000 7330 0000 0000 060f 0309 0109 010f  ..s0............
+00000f80: 010f 0109 0206 010f 0110 0109 0209 0206  ................
+00000f90: 010c 0216 010c 0216 010c 0215 0115 0403  ................
+00000fa0: 021d 0503 0200 0163 0500 0000 0d00 0000  .......c........
+00000fb0: 0e00 0000 4b00 0000 7387 0400 007c 0300  ....K...s....|..
+00000fc0: 7320 0064 0100 7400 007c 0000 6a01 0083  s .d..t..|..j...
+00000fd0: 0100 6402 0017 167d 0300 6e00 0064 0300  ..d....}..n..d..
+00000fe0: 7c05 006b 0600 7338 0064 0400 7c05 006b  |..k..s8.d..|..k
+00000ff0: 0600 72eb 0064 0400 7c05 006b 0600 725b  ..r..d..|..k..r[
+00001000: 007c 0500 6404 0019 725b 007c 0500 6404  .|..d...r[.|..d.
+00001010: 0019 7d06 006e 0600 6402 007d 0600 6403  ..}..n..d..}..d.
+00001020: 007c 0500 6b06 0072 8400 7c05 0064 0300  .|..k..r..|..d..
+00001030: 1972 8400 7c05 0064 0300 197d 0700 6e06  .r..|..d...}..n.
+00001040: 0064 0500 7d07 0067 0000 7402 007c 0100  .d..}..g..t..|..
+00001050: 8301 0044 5d4b 005c 0200 7d08 007d 0100  ...D]K.\..}..}..
+00001060: 6904 007c 0200 7c08 0019 6406 0036 7c01  i..|..|...d..6|.
+00001070: 0064 0700 367c 0700 6403 0036 7403 007c  .d..6|..d..6t..|
+00001080: 0600 7404 0083 0200 72d8 007c 0600 7c08  ..t.....r..|..|.
+00001090: 0019 6e03 007c 0600 6404 0036 5e02 0071  ..n..|..d..6^..q
+000010a0: 9700 7d09 006e 3700 6700 0074 0200 7c01  ..}..n7.g..t..|.
+000010b0: 0083 0100 445d 2400 5c02 007d 0800 7d01  ....D]$.\..}..}.
+000010c0: 0069 0200 7c02 007c 0800 1964 0600 367c  .i..|..|...d..6|
+000010d0: 0100 6407 0036 5e02 0071 f800 7d09 0069  ..d..6^..q..}..i
+000010e0: 0200 7c09 0064 0800 367c 0300 6409 0036  ..|..d..6|..d..6
+000010f0: 7d0a 0064 0a00 7c05 006b 0600 725d 017c  }..d..|..k..r].|
+00001100: 0500 640a 0019 725d 017c 0500 640a 0019  ..d...r].|..d...
+00001110: 7c0a 0064 0a00 3c6e 0000 7c00 006a 0500  |..d..<n..|..j..
+00001120: 640b 006b 0200 7295 0164 0c00 7c04 006b  d..k..r..d..|..k
+00001130: 0600 7295 017c 0400 640c 0019 7295 017c  ..r..|..d...r..|
+00001140: 0400 640c 0019 7c00 005f 0600 7195 016e  ..d...|.._..q..n
+00001150: 0000 640d 007c 0500 6b06 0072 bc01 7c05  ..d..|..k..r..|.
+00001160: 0064 0d00 1972 bc01 7c05 0064 0d00 197c  .d...r..|..d...|
+00001170: 0a00 640e 003c 6e0a 0064 0f00 7c0a 0064  ..d..<n..d..|..d
+00001180: 0e00 3c64 1000 7c05 006b 0600 72e9 017c  ..<d..|..k..r..|
+00001190: 0500 6410 0019 72e9 0164 1100 7c0a 0064  ..d...r..d..|..d
+000011a0: 1000 3c6e 0000 6412 007c 0500 6b06 0072  ..<n..d..|..k..r
+000011b0: 0c02 7c05 0064 1200 1972 0c02 6411 007c  ..|..d...r..d..|
+000011c0: 0a00 6412 003c 6e00 0064 1300 7c05 006b  ..d..<n..d..|..k
+000011d0: 0600 7233 027c 0500 6413 0019 7233 027c  ..r3.|..d...r3.|
+000011e0: 0500 6413 0019 7c0a 0064 1300 3c6e 0000  ..d...|..d..<n..
+000011f0: 7c04 006a 0700 6414 0083 0100 7252 027c  |..j..d.....rR.|
+00001200: 0400 6414 0019 7c00 005f 0800 6e00 007c  ..d...|.._..n..|
+00001210: 0400 6a07 0064 1500 8301 0072 7304 7409  ..j..d.....rs.t.
+00001220: 007c 0000 5f0a 007c 0000 6a05 0064 0b00  .|.._..|..j..d..
+00001230: 6b03 0072 e303 7c04 0064 1500 1964 1600  k..r..|..d...d..
+00001240: 197d 0b00 7c04 0064 1500 1964 1700 197d  .}..|..d...d...}
+00001250: 0c00 7c0b 0072 af02 6418 0074 0b00 7c0b  ..|..r..d..t..|.
+00001260: 0083 0100 1764 1900 176e 0300 641a 007d  .....d...n..d..}
+00001270: 0b00 7c0c 0072 cf02 641b 0074 0b00 7c0c  ..|..r..d..t..|.
+00001280: 0083 0100 1764 1800 176e 0300 641a 007d  .....d...n..d..}
+00001290: 0c00 7c00 006a 0500 641c 006b 0200 7234  ..|..j..d..k..r4
+000012a0: 037c 0000 046a 0c00 740d 0064 1d00 8301  .|...j..t..d....
+000012b0: 0064 1e00 177c 0300 1764 1f00 1774 0d00  .d...|...d...t..
+000012c0: 6420 0083 0100 1764 2100 177c 0b00 1764  d .....d!..|...d
+000012d0: 2200 177c 0c00 1764 2300 1774 0d00 641d  "..|...d#..t..d.
+000012e0: 0083 0100 1764 2400 1737 025f 0c00 71e3  .....d$..7._..q.
+000012f0: 037c 0000 6a05 0064 2500 6b02 0072 9303  .|..j..d%.k..r..
+00001300: 7c00 0004 6a0c 0074 0d00 641d 0083 0100  |...j..t..d.....
+00001310: 6426 0017 7c03 0017 6427 0017 740d 0064  d&..|...d'..t..d
+00001320: 2000 8301 0017 6421 0017 7c0b 0017 6428   .....d!..|...d(
+00001330: 0017 7c0c 0017 6423 0017 740d 0064 1d00  ..|...d#..t..d..
+00001340: 8301 0017 6424 0017 3702 5f0c 0071 e303  ....d$..7._..q..
+00001350: 7c00 0004 6a0c 0074 0d00 641d 0083 0100  |...j..t..d.....
+00001360: 6426 0017 7c03 0017 6427 0017 740d 0064  d&..|...d'..t..d
+00001370: 2000 8301 0017 6421 0017 7c0b 0017 6422   .....d!..|...d"
+00001380: 0017 7c0c 0017 6423 0017 740d 0064 1d00  ..|...d#..t..d..
+00001390: 8301 0017 6424 0017 3702 5f0c 006e 0000  ....d$..7._..n..
+000013a0: 7c00 006a 0500 640b 006b 0200 7273 047c  |..j..d..k..rs.|
+000013b0: 0400 6415 0019 6416 0019 7d0b 007c 0400  ..d...d...}..|..
+000013c0: 6415 0019 6417 0019 7d0c 007c 0b00 7228  d...d...}..|..r(
+000013d0: 0464 1800 740b 007c 0b00 8301 0017 6419  .d..t..|......d.
+000013e0: 0017 6e03 0064 1a00 7d0b 007c 0c00 7248  ..n..d..}..|..rH
+000013f0: 0464 1b00 740b 007c 0c00 8301 0017 6418  .d..t..|......d.
+00001400: 0017 6e03 0064 1a00 7d0c 007c 0000 046a  ..n..d..}..|...j
+00001410: 0c00 6421 007c 0b00 1764 2900 177c 0c00  ..d!.|...d)..|..
+00001420: 1764 2300 1737 025f 0c00 7173 046e 0000  .d#..7._..qs.n..
+00001430: 7c00 006a 0100 6a0e 007c 0a00 8301 0001  |..j..j..|......
+00001440: 642a 0053 282b 0000 0073 c600 0000 0a20  d*.S(+...s..... 
+00001450: 2020 2020 2020 2061 6464 2073 6572 6965         add serie
+00001460: 202d 2053 6572 6965 7320 6172 6520 6c69   - Series are li
+00001470: 7374 206f 6620 6461 7461 2074 6861 7420  st of data that 
+00001480: 7769 6c6c 2062 6520 706c 6f74 7465 640a  will be plotted.
+00001490: 2020 2020 2020 2020 7920 7b31 2c20 322c          y {1, 2,
+000014a0: 2033 2c20 342c 2035 7d20 2f20 7820 7b31   3, 4, 5} / x {1
+000014b0: 2c20 322c 2033 2c20 342c 2035 7d0a 0a20  , 2, 3, 4, 5}.. 
+000014c0: 2020 2020 2020 2054 4f44 4f3a 2041 6464         TODO: Add
+000014d0: 2064 6f63 2066 6f72 2073 7570 706f 7274   doc for support
+000014e0: 6564 2070 6172 616d 6574 6572 732c 2069  ed parameters, i
+000014f0: 6520 785f 6178 6973 5f64 6174 652c 2073  e x_axis_date, s
+00001500: 6861 7065 2c20 7369 7a65 0a0a 2020 2020  hape, size..    
+00001510: 2020 2020 7308 0000 0053 6572 6965 2025      s....Serie %
+00001520: 6469 0100 0000 7405 0000 0073 6861 7065  di....t....shape
+00001530: 7404 0000 0073 697a 6574 0600 0000 6369  t....sizet....ci
+00001540: 7263 6c65 7401 0000 0078 7401 0000 0079  rclet....xt....y
+00001550: 7406 0000 0076 616c 7565 7374 0300 0000  t....valuest....
+00001560: 6b65 7974 0400 0000 7479 7065 7408 0000  keyt....typet...
+00001570: 0070 6965 4368 6172 7474 0a00 0000 636f  .pieChartt....co
+00001580: 6c6f 725f 6c69 7374 7405 0000 0079 6178  lor_listt....yax
+00001590: 6973 7405 0000 0079 4178 6973 7401 0000  ist....yAxist...
+000015a0: 0031 7403 0000 0062 6172 7404 0000 0074  .1t....bart....t
+000015b0: 7275 6574 0800 0000 6469 7361 626c 6564  ruet....disabled
+000015c0: 7405 0000 0063 6f6c 6f72 740b 0000 0064  t....colort....d
+000015d0: 6174 655f 666f 726d 6174 7407 0000 0074  ate_formatt....t
+000015e0: 6f6f 6c74 6970 7407 0000 0079 5f73 7461  ooltipt....y_sta
+000015f0: 7274 7405 0000 0079 5f65 6e64 7401 0000  rtt....y_endt...
+00001600: 0027 7304 0000 0027 202b 2052 0600 0000  .'s....' + R....
+00001610: 7304 0000 0020 2b20 2774 1000 0000 6c69  s.... + 't....li
+00001620: 6e65 506c 7573 4261 7243 6861 7274 6903  nePlusBarCharti.
+00001630: 0000 0073 1000 0000 6966 286b 6579 2e69  ...s....if(key.i
+00001640: 6e64 6578 4f66 2827 730b 0000 0027 2920  ndexOf('s....') 
+00001650: 3e20 2d31 2029 7b0a 6904 0000 0073 0800  > -1 ){.i....s..
+00001660: 0000 7661 7220 7920 3d20 7317 0000 0020  ..var y = s.... 
+00001670: 5374 7269 6e67 2867 7261 7068 2e70 6f69  String(graph.poi
+00001680: 6e74 2e79 2920 7302 0000 003b 0a73 0200  nt.y) s....;.s..
+00001690: 0000 7d0a 7413 0000 0063 756d 756c 6174  ..}.t....cumulat
+000016a0: 6976 654c 696e 6543 6861 7274 730b 0000  iveLineCharts...
+000016b0: 0069 6628 6b65 7920 3d3d 2027 7304 0000  .if(key == 's...
+000016c0: 0027 297b 0a73 0b00 0000 2053 7472 696e  .'){.s.... Strin
+000016d0: 6728 6529 2073 1300 0000 2053 7472 696e  g(e) s.... Strin
+000016e0: 6728 652e 706f 696e 742e 7929 204e 280f  g(e.point.y) N(.
+000016f0: 0000 0074 0300 0000 6c65 6e52 0f00 0000  ...t....lenR....
+00001700: 7409 0000 0065 6e75 6d65 7261 7465 740a  t....enumeratet.
+00001710: 0000 0069 7369 6e73 7461 6e63 6574 0400  ...isinstancet..
+00001720: 0000 6c69 7374 520e 0000 0052 2900 0000  ..listR....R)...
+00001730: 5219 0000 0052 1300 0000 5218 0000 0074  R....R....R....t
+00001740: 1300 0000 6375 7374 6f6d 5f74 6f6f 6c74  ....custom_toolt
+00001750: 6970 5f66 6c61 6774 0300 0000 7374 7274  ip_flagt....strt
+00001760: 1800 0000 746f 6f6c 7469 705f 636f 6e64  ....tooltip_cond
+00001770: 6974 696f 6e5f 7374 7269 6e67 5204 0000  ition_stringR...
+00001780: 0074 0600 0000 6170 7065 6e64 280d 0000  .t....append(...
+00001790: 0052 1c00 0000 5224 0000 0052 2300 0000  .R....R$...R#...
+000017a0: 5215 0000 0074 0500 0000 6578 7472 6152  R....t....extraR
+000017b0: 1d00 0000 7405 0000 0063 7369 7a65 7406  ....t....csizet.
+000017c0: 0000 0063 7368 6170 6574 0100 0000 6974  ...cshapet....it
+000017d0: 0500 0000 7365 7269 6574 0d00 0000 6461  ....seriet....da
+000017e0: 7461 5f6b 6579 7661 6c75 6574 0600 0000  ta_keyvaluet....
+000017f0: 5f73 7461 7274 7404 0000 005f 656e 6428  _startt...._end(
+00001800: 0000 0000 2800 0000 0073 4d00 0000 2f68  ....(....sM.../h
+00001810: 6f6d 652f 6172 6573 6b69 2f70 7562 6c69  ome/areski/publi
+00001820: 635f 6874 6d6c 2f64 6a61 6e67 6f2f 4d79  c_html/django/My
+00001830: 5072 6f6a 6563 7473 2f6e 7664 332f 7079  Projects/nvd3/py
+00001840: 7468 6f6e 2d6e 7664 332f 6e76 6433 2f4e  thon-nvd3/nvd3/N
+00001850: 5644 3343 6861 7274 2e70 7974 0900 0000  VD3Chart.pyt....
+00001860: 6164 645f 7365 7269 6599 0000 0073 6800  add_serie....sh.
+00001870: 0000 0008 0601 1a03 1801 1601 0d02 0601  ................
+00001880: 1601 0d02 0601 0305 5e02 3702 1404 1601  ........^.7.....
+00001890: 1102 0f01 1601 1304 1601 1102 0a02 1601  ................
+000018a0: 0d02 1601 0d02 1601 1102 0f01 1002 0f01  ................
+000018b0: 0902 0f01 0e01 0e01 2001 2002 0f01 0702  ........ . .....
+000018c0: 4901 0f01 0702 4902 0702 4902 0f01 0e01  I.....I...I.....
+000018d0: 0e01 2001 2001 0701 1e02 6302 0000 0002  .. . .....c.....
+000018e0: 0000 0002 0000 0043 0000 0073 1300 0000  .......C...s....
+000018f0: 7400 007c 0100 8301 007c 0000 5f01 0064  t..|.....|.._..d
+00001900: 0100 5328 0200 0000 7310 0000 0053 6574  ..S(....s....Set
+00001910: 2047 7261 7068 2068 6569 6768 744e 2802   Graph heightN(.
+00001920: 0000 0052 3d00 0000 7406 0000 0068 6569  ...R=...t....hei
+00001930: 6768 7428 0200 0000 521c 0000 0052 4900  ght(....R....RI.
+00001940: 0000 2800 0000 0028 0000 0000 734d 0000  ..(....(....sM..
+00001950: 002f 686f 6d65 2f61 7265 736b 692f 7075  ./home/areski/pu
+00001960: 626c 6963 5f68 746d 6c2f 646a 616e 676f  blic_html/django
+00001970: 2f4d 7950 726f 6a65 6374 732f 6e76 6433  /MyProjects/nvd3
+00001980: 2f70 7974 686f 6e2d 6e76 6433 2f6e 7664  /python-nvd3/nvd
+00001990: 332f 4e56 4433 4368 6172 742e 7079 7410  3/NVD3Chart.pyt.
+000019a0: 0000 0073 6574 5f67 7261 7068 5f68 6569  ...set_graph_hei
+000019b0: 6768 74f5 0000 0073 0200 0000 0002 6302  ght....s......c.
+000019c0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+000019d0: 1300 0000 7400 007c 0100 8301 007c 0000  ....t..|.....|..
+000019e0: 5f01 0064 0100 5328 0200 0000 730f 0000  _..d..S(....s...
+000019f0: 0053 6574 2047 7261 7068 2077 6964 7468  .Set Graph width
+00001a00: 4e28 0200 0000 523d 0000 0074 0500 0000  N(....R=...t....
+00001a10: 7769 6474 6828 0200 0000 521c 0000 0052  width(....R....R
+00001a20: 4b00 0000 2800 0000 0028 0000 0000 734d  K...(....(....sM
+00001a30: 0000 002f 686f 6d65 2f61 7265 736b 692f  .../home/areski/
+00001a40: 7075 626c 6963 5f68 746d 6c2f 646a 616e  public_html/djan
+00001a50: 676f 2f4d 7950 726f 6a65 6374 732f 6e76  go/MyProjects/nv
+00001a60: 6433 2f70 7974 686f 6e2d 6e76 6433 2f6e  d3/python-nvd3/n
+00001a70: 7664 332f 4e56 4433 4368 6172 742e 7079  vd3/NVD3Chart.py
+00001a80: 740f 0000 0073 6574 5f67 7261 7068 5f77  t....set_graph_w
+00001a90: 6964 7468 f900 0000 7302 0000 0000 0263  idth....s......c
+00001aa0: 0200 0000 0200 0000 0200 0000 4300 0000  ............C...
+00001ab0: 730d 0000 007c 0100 7c00 005f 0000 6401  s....|..|.._..d.
+00001ac0: 0053 2802 0000 0073 1300 0000 5365 7420  .S(....s....Set 
+00001ad0: 636f 6e74 6169 6e65 7268 6561 6465 724e  containerheaderN
+00001ae0: 2801 0000 0074 0f00 0000 636f 6e74 6169  (....t....contai
+00001af0: 6e65 7268 6561 6465 7228 0200 0000 521c  nerheader(....R.
+00001b00: 0000 0052 4d00 0000 2800 0000 0028 0000  ...RM...(....(..
+00001b10: 0000 734d 0000 002f 686f 6d65 2f61 7265  ..sM.../home/are
+00001b20: 736b 692f 7075 626c 6963 5f68 746d 6c2f  ski/public_html/
+00001b30: 646a 616e 676f 2f4d 7950 726f 6a65 6374  django/MyProject
+00001b40: 732f 6e76 6433 2f70 7974 686f 6e2d 6e76  s/nvd3/python-nv
+00001b50: 6433 2f6e 7664 332f 4e56 4433 4368 6172  d3/nvd3/NVD3Char
+00001b60: 742e 7079 7413 0000 0073 6574 5f63 6f6e  t.pyt....set_con
+00001b70: 7461 696e 6572 6865 6164 6572 fd00 0000  tainerheader....
+00001b80: 7302 0000 0000 0263 0200 0000 0200 0000  s......c........
+00001b90: 0200 0000 4300 0000 730d 0000 007c 0100  ....C...s....|..
+00001ba0: 7c00 005f 0000 6401 0053 2802 0000 0073  |.._..d..S(....s
+00001bb0: 0d00 0000 5365 7420 6461 7465 2066 616c  ....Set date fal
+00001bc0: 674e 2801 0000 0074 0900 0000 6461 7465  gN(....t....date
+00001bd0: 5f66 6c61 6728 0200 0000 521c 0000 0052  _flag(....R....R
+00001be0: 4f00 0000 2800 0000 0028 0000 0000 734d  O...(....(....sM
+00001bf0: 0000 002f 686f 6d65 2f61 7265 736b 692f  .../home/areski/
+00001c00: 7075 626c 6963 5f68 746d 6c2f 646a 616e  public_html/djan
+00001c10: 676f 2f4d 7950 726f 6a65 6374 732f 6e76  go/MyProjects/nv
+00001c20: 6433 2f70 7974 686f 6e2d 6e76 6433 2f6e  d3/python-nvd3/n
+00001c30: 7664 332f 4e56 4433 4368 6172 742e 7079  vd3/NVD3Chart.py
+00001c40: 740d 0000 0073 6574 5f64 6174 655f 666c  t....set_date_fl
+00001c50: 6167 0101 0000 7302 0000 0000 0263 0200  ag....s......c..
+00001c60: 0000 0200 0000 0200 0000 4300 0000 730d  ..........C...s.
+00001c70: 0000 007c 0100 7c00 005f 0000 6401 0053  ...|..|.._..d..S
+00001c80: 2802 0000 0073 2300 0000 5365 7420 6375  (....s#...Set cu
+00001c90: 7374 6f6d 5f74 6f6f 6c74 6970 5f66 6c61  stom_tooltip_fla
+00001ca0: 6720 2620 6461 7465 5f66 6c61 674e 2801  g & date_flagN(.
+00001cb0: 0000 0052 3c00 0000 2802 0000 0052 1c00  ...R<...(....R..
+00001cc0: 0000 523c 0000 0028 0000 0000 2800 0000  ..R<...(....(...
+00001cd0: 0073 4d00 0000 2f68 6f6d 652f 6172 6573  .sM.../home/ares
+00001ce0: 6b69 2f70 7562 6c69 635f 6874 6d6c 2f64  ki/public_html/d
+00001cf0: 6a61 6e67 6f2f 4d79 5072 6f6a 6563 7473  jango/MyProjects
+00001d00: 2f6e 7664 332f 7079 7468 6f6e 2d6e 7664  /nvd3/python-nvd
+00001d10: 332f 6e76 6433 2f4e 5644 3343 6861 7274  3/nvd3/NVD3Chart
+00001d20: 2e70 7974 1700 0000 7365 745f 6375 7374  .pyt....set_cust
+00001d30: 6f6d 5f74 6f6f 6c74 6970 5f66 6c61 6705  om_tooltip_flag.
+00001d40: 0100 0073 0200 0000 0002 6301 0000 0001  ...s......c.....
+00001d50: 0000 0001 0000 0043 0000 0073 1100 0000  .......C...s....
+00001d60: 7c00 006a 0000 8300 0001 7c00 006a 0100  |..j......|..j..
+00001d70: 5328 0100 0000 7312 0000 0072 6574 7572  S(....s....retur
+00001d80: 6e20 6874 6d6c 636f 6e74 656e 7428 0200  n htmlcontent(..
+00001d90: 0000 7409 0000 0062 7569 6c64 6874 6d6c  ..t....buildhtml
+00001da0: 740b 0000 0068 746d 6c63 6f6e 7465 6e74  t....htmlcontent
+00001db0: 2801 0000 0052 1c00 0000 2800 0000 0028  (....R....(....(
+00001dc0: 0000 0000 734d 0000 002f 686f 6d65 2f61  ....sM.../home/a
+00001dd0: 7265 736b 692f 7075 626c 6963 5f68 746d  reski/public_htm
+00001de0: 6c2f 646a 616e 676f 2f4d 7950 726f 6a65  l/django/MyProje
+00001df0: 6374 732f 6e76 6433 2f70 7974 686f 6e2d  cts/nvd3/python-
+00001e00: 6e76 6433 2f6e 7664 332f 4e56 4433 4368  nvd3/nvd3/NVD3Ch
+00001e10: 6172 742e 7079 7407 0000 005f 5f73 7472  art.pyt....__str
+00001e20: 5f5f 0901 0000 7304 0000 0000 020a 0163  __....s........c
+00001e30: 0100 0000 0100 0000 0500 0000 4300 0000  ............C...
+00001e40: 733c 0000 007c 0000 6a00 0083 0000 017c  s<...|..j......|
+00001e50: 0000 6a01 0083 0000 017c 0000 6a02 006a  ..j......|..j..j
+00001e60: 0300 6401 007c 0000 6a04 0064 0200 7c00  ..d..|..j..d..|.
+00001e70: 006a 0500 8300 027c 0000 5f06 0064 0300  .j.....|.._..d..
+00001e80: 5328 0400 0000 73d1 0000 0042 7569 6c64  S(....s....Build
+00001e90: 2048 544d 4c20 636f 6e74 656e 7420 6f6e   HTML content on
+00001ea0: 6c79 2c20 6e6f 2068 6561 6465 7220 6f72  ly, no header or
+00001eb0: 2062 6f64 7920 7461 6773 2e20 546f 2062   body tags. To b
+00001ec0: 6520 7573 6566 756c 2074 6869 730a 2020  e useful this.  
+00001ed0: 2020 2020 2020 7769 6c6c 2075 7375 616c        will usual
+00001ee0: 6c79 2072 6571 7569 7265 2074 6865 2061  ly require the a
+00001ef0: 7474 7269 6275 7465 2060 6a75 7165 7279  ttribute `juqery
+00001f00: 5f6f 6e5f 7265 6164 7960 2074 6f20 6265  _on_ready` to be
+00001f10: 2073 6574 2077 6869 6368 0a20 2020 2020   set which.     
+00001f20: 2020 2077 696c 6c20 7772 6170 2074 6865     will wrap the
+00001f30: 206a 7320 696e 2024 2866 756e 6374 696f   js in $(functio
+00001f40: 6e28 297b 3c72 6567 756c 6172 5f6a 733e  n(){<regular_js>
+00001f50: 7d3b 290a 2020 2020 2020 2020 7409 0000  };).        t...
+00001f60: 0063 6f6e 7461 696e 6572 7407 0000 006a  .containert....j
+00001f70: 7363 6861 7274 4e28 0700 0000 740e 0000  schartN(....t...
+00001f80: 0062 7569 6c64 636f 6e74 6169 6e65 7274  .buildcontainert
+00001f90: 0c00 0000 6275 696c 646a 7363 6861 7274  ....buildjschart
+00001fa0: 5212 0000 0074 0a00 0000 7375 6273 7469  R....t....substi
+00001fb0: 7475 7465 5255 0000 0052 5600 0000 5253  tuteRU...RV...RS
+00001fc0: 0000 0028 0100 0000 521c 0000 0028 0000  ...(....R....(..
+00001fd0: 0000 2800 0000 0073 4d00 0000 2f68 6f6d  ..(....sM.../hom
+00001fe0: 652f 6172 6573 6b69 2f70 7562 6c69 635f  e/areski/public_
+00001ff0: 6874 6d6c 2f64 6a61 6e67 6f2f 4d79 5072  html/django/MyPr
+00002000: 6f6a 6563 7473 2f6e 7664 332f 7079 7468  ojects/nvd3/pyth
+00002010: 6f6e 2d6e 7664 332f 6e76 6433 2f4e 5644  on-nvd3/nvd3/NVD
+00002020: 3343 6861 7274 2e70 7974 0c00 0000 6275  3Chart.pyt....bu
+00002030: 696c 6463 6f6e 7465 6e74 0e01 0000 7308  ildcontent....s.
+00002040: 0000 0000 050a 010a 0115 0163 0100 0000  ...........c....
+00002050: 0100 0000 0700 0000 4300 0000 734f 0000  ........C...sO..
+00002060: 007c 0000 6a00 0083 0000 017c 0000 6a01  .|..j......|..j.
+00002070: 0083 0000 017c 0000 6a02 0083 0000 017c  .....|..j......|
+00002080: 0000 6a03 006a 0400 6401 007c 0000 6a05  ..j..j..d..|..j.
+00002090: 0064 0200 7c00 006a 0600 6403 007c 0000  .d..|..j..d..|..
+000020a0: 6a07 0083 0003 7c00 005f 0800 6404 0053  j.....|.._..d..S
+000020b0: 2805 0000 0073 7e00 0000 4275 696c 6420  (....s~...Build 
+000020c0: 7468 6520 4854 4d4c 2070 6167 650a 2020  the HTML page.  
+000020d0: 2020 2020 2020 4372 6561 7465 2074 6865        Create the
+000020e0: 2068 746d 6c68 6561 6465 7220 7769 7468   htmlheader with
+000020f0: 2063 7373 202f 206a 730a 2020 2020 2020   css / js.      
+00002100: 2020 4372 6561 7465 2068 746d 6c20 7061    Create html pa
+00002110: 6765 0a20 2020 2020 2020 2041 6464 204a  ge.        Add J
+00002120: 7320 636f 6465 2066 6f72 206e 7664 330a  s code for nvd3.
+00002130: 2020 2020 2020 2020 7406 0000 0068 6561          t....hea
+00002140: 6465 7252 5500 0000 5256 0000 004e 2809  derRU...RV...N(.
+00002150: 0000 0074 0f00 0000 6275 696c 6468 746d  ...t....buildhtm
+00002160: 6c68 6561 6465 7252 5700 0000 5258 0000  lheaderRW...RX..
+00002170: 0052 1100 0000 5259 0000 0074 0a00 0000  .R....RY...t....
+00002180: 6874 6d6c 6865 6164 6572 5255 0000 0052  htmlheaderRU...R
+00002190: 5600 0000 5253 0000 0028 0100 0000 521c  V...RS...(....R.
+000021a0: 0000 0028 0000 0000 2800 0000 0073 4d00  ...(....(....sM.
+000021b0: 0000 2f68 6f6d 652f 6172 6573 6b69 2f70  ../home/areski/p
+000021c0: 7562 6c69 635f 6874 6d6c 2f64 6a61 6e67  ublic_html/djang
+000021d0: 6f2f 4d79 5072 6f6a 6563 7473 2f6e 7664  o/MyProjects/nvd
+000021e0: 332f 7079 7468 6f6e 2d6e 7664 332f 6e76  3/python-nvd3/nv
+000021f0: 6433 2f4e 5644 3343 6861 7274 2e70 7952  d3/NVD3Chart.pyR
+00002200: 5200 0000 1801 0000 7308 0000 0000 060a  R.......s.......
+00002210: 010a 010a 0263 0100 0000 0300 0000 0400  .....c..........
+00002220: 0000 4300 0000 7353 0000 0064 0100 7c00  ..C...sS...d..|.
+00002230: 005f 0000 7820 007c 0000 6a01 0044 5d15  ._..x .|..j..D].
+00002240: 007d 0100 7c00 0004 6a00 007c 0100 3702  .}..|...j..|..7.
+00002250: 5f00 0071 1300 5778 2000 7c00 006a 0200  _..q..Wx .|..j..
+00002260: 445d 1500 7d02 007c 0000 046a 0000 7c02  D]..}..|...j..|.
+00002270: 0037 025f 0000 7136 0057 6402 0053 2803  .7._..q6.Wd..S(.
+00002280: 0000 0073 1c00 0000 6765 6e65 7261 7465  ...s....generate
+00002290: 2048 544d 4c20 6865 6164 6572 2063 6f6e   HTML header con
+000022a0: 7465 6e74 5206 0000 004e 2803 0000 0052  tentR....N(....R
+000022b0: 5d00 0000 521a 0000 0052 1b00 0000 2803  ]...R....R....(.
+000022c0: 0000 0052 1c00 0000 7403 0000 0063 7373  ...R....t....css
+000022d0: 7402 0000 006a 7328 0000 0000 2800 0000  t....js(....(...
+000022e0: 0073 4d00 0000 2f68 6f6d 652f 6172 6573  .sM.../home/ares
+000022f0: 6b69 2f70 7562 6c69 635f 6874 6d6c 2f64  ki/public_html/d
+00002300: 6a61 6e67 6f2f 4d79 5072 6f6a 6563 7473  jango/MyProjects
+00002310: 2f6e 7664 332f 7079 7468 6f6e 2d6e 7664  /nvd3/python-nvd
+00002320: 332f 6e76 6433 2f4e 5644 3343 6861 7274  3/nvd3/NVD3Chart
+00002330: 2e70 7952 5c00 0000 2401 0000 730a 0000  .pyR\...$...s...
+00002340: 0000 0209 0110 0113 0110 0163 0100 0000  ...........c....
+00002350: 0100 0000 0500 0000 4300 0000 73e7 0000  ........C...s...
+00002360: 007c 0000 6a00 007c 0000 5f01 007c 0000  .|..j..|.._..|..
+00002370: 6a02 0072 5a00 7c00 006a 0200 6401 0019  j..rZ.|..j..d...
+00002380: 6402 006b 0300 7241 007c 0000 046a 0300  d..k..rA.|...j..
+00002390: 6403 007c 0000 6a02 0016 3702 5f03 0071  d..|..j...7._..q
+000023a0: 5a00 7c00 0004 6a03 0064 0400 7c00 006a  Z.|...j..d..|..j
+000023b0: 0200 1637 025f 0300 6e00 007c 0000 6a04  ...7._..n..|..j.
+000023c0: 0072 a800 7c00 006a 0400 6401 0019 6402  .r..|..j..d...d.
+000023d0: 006b 0300 728f 007c 0000 046a 0300 6405  .k..r..|...j..d.
+000023e0: 007c 0000 6a04 0016 3702 5f03 0071 a800  .|..j...7._..q..
+000023f0: 7c00 0004 6a03 0064 0600 7c00 006a 0400  |...j..d..|..j..
+00002400: 1637 025f 0300 6e00 007c 0000 6a03 0072  .7._..n..|..j..r
+00002410: c400 6407 007c 0000 6a03 0016 7c00 005f  ..d..|..j...|.._
+00002420: 0300 6e00 007c 0000 046a 0100 6408 007c  ..n..|...j..d..|
+00002430: 0000 6a05 007c 0000 6a03 0066 0200 1637  ..j..|..j..f...7
+00002440: 025f 0100 6409 0053 280a 0000 0073 1100  ._..d..S(....s..
+00002450: 0000 6765 6e65 7261 7465 2048 544d 4c20  ..generate HTML 
+00002460: 6469 7669 ffff ffff 7401 0000 0025 730b  divi....t....%s.
+00002470: 0000 0077 6964 7468 3a25 7370 783b 7309  ...width:%spx;s.
+00002480: 0000 0077 6964 7468 3a25 733b 730c 0000  ...width:%s;s...
+00002490: 0068 6569 6768 743a 2573 7078 3b73 0a00  .height:%spx;s..
+000024a0: 0000 6865 6967 6874 3a25 733b 730a 0000  ..height:%s;s...
+000024b0: 0073 7479 6c65 3d22 2573 2273 2200 0000  .style="%s"s"...
+000024c0: 3c64 6976 2069 643d 2225 7322 3e3c 7376  <div id="%s"><sv
+000024d0: 6720 2573 3e3c 2f73 7667 3e3c 2f64 6976  g %s></svg></div
+000024e0: 3e0a 4e28 0600 0000 524d 0000 0052 5500  >.N(....RM...RU.
+000024f0: 0000 524b 0000 0074 0500 0000 7374 796c  ..RK...t....styl
+00002500: 6552 4900 0000 5215 0000 0028 0100 0000  eRI...R....(....
+00002510: 521c 0000 0028 0000 0000 2800 0000 0073  R....(....(....s
+00002520: 4d00 0000 2f68 6f6d 652f 6172 6573 6b69  M.../home/areski
+00002530: 2f70 7562 6c69 635f 6874 6d6c 2f64 6a61  /public_html/dja
+00002540: 6e67 6f2f 4d79 5072 6f6a 6563 7473 2f6e  ngo/MyProjects/n
+00002550: 7664 332f 7079 7468 6f6e 2d6e 7664 332f  vd3/python-nvd3/
+00002560: 6e76 6433 2f4e 5644 3343 6861 7274 2e70  nvd3/NVD3Chart.p
+00002570: 7952 5700 0000 2c01 0000 7318 0000 0000  yRW...,...s.....
+00002580: 020c 0209 0113 0119 0219 0109 0113 0119  ................
+00002590: 0219 0109 0113 0263 0100 0000 0100 0000  .......c........
+000025a0: 0300 0000 4300 0000 7351 0100 007c 0000  ....C...sQ...|..
+000025b0: 6a00 0072 4d01 7c00 006a 0100 73e3 007c  j..rM.|..j..s..|
+000025c0: 0000 6a02 0064 0100 6b02 0072 8000 7403  ..j..d..k..r..t.
+000025d0: 0064 0200 8301 0064 0300 1774 0300 6404  .d.....d...t..d.
+000025e0: 0083 0100 1764 0500 1774 0300 6404 0083  .....d...t..d...
+000025f0: 0100 177c 0000 6a04 0017 7403 0064 0400  ...|..j...t..d..
+00002600: 8301 0017 6406 0017 7403 0064 0400 8301  ....d...t..d....
+00002610: 0017 6407 0017 7403 0064 0200 8301 0017  ..d...t..d......
+00002620: 6408 0017 7c00 005f 0500 714a 0174 0300  d...|.._..qJ.t..
+00002630: 6402 0083 0100 6403 0017 7403 0064 0400  d.....d...t..d..
+00002640: 8301 0017 6409 0017 7403 0064 0400 8301  ....d...t..d....
+00002650: 0017 640a 0017 7c00 006a 0400 1774 0300  ..d...|..j...t..
+00002660: 6404 0083 0100 1764 0b00 1774 0300 6404  d......d...t..d.
+00002670: 0083 0100 1764 0700 1774 0300 6402 0083  .....d...t..d...
+00002680: 0100 1764 0800 177c 0000 5f05 0071 4d01  ...d...|.._..qM.
+00002690: 7403 0064 0200 8301 0064 0300 1774 0300  t..d.....d...t..
+000026a0: 6404 0083 0100 1764 0c00 7c00 006a 0600  d......d..|..j..
+000026b0: 1617 7403 0064 0400 8301 0017 640a 0017  ..t..d......d...
+000026c0: 7c00 006a 0400 1774 0300 6404 0083 0100  |..j...t..d.....
+000026d0: 1764 0d00 1774 0300 6404 0083 0100 1764  .d...t..d......d
+000026e0: 0700 1774 0300 6402 0083 0100 1764 0800  ...t..d......d..
+000026f0: 177c 0000 5f05 006e 0000 640e 0053 280f  .|.._..n..d..S(.
+00002700: 0000 0073 2500 0000 6765 6e65 7261 7465  ...s%...generate
+00002710: 2063 7573 746f 6d20 746f 6f6c 7469 7020   custom tooltip 
+00002720: 666f 7220 7468 6520 6368 6172 7452 2800  for the chartR(.
+00002730: 0000 6902 0000 0073 3200 0000 6368 6172  ..i....s2...char
+00002740: 742e 746f 6f6c 7469 7043 6f6e 7465 6e74  t.tooltipContent
+00002750: 2866 756e 6374 696f 6e28 6b65 792c 2079  (function(key, y
+00002760: 2c20 652c 2067 7261 7068 2920 7b0a 6903  , e, graph) {.i.
+00002770: 0000 0073 1500 0000 7661 7220 7820 3d20  ...s....var x = 
+00002780: 5374 7269 6e67 286b 6579 293b 0a73 3300  String(key);.s3.
+00002790: 0000 746f 6f6c 7469 705f 7374 7220 3d20  ..tooltip_str = 
+000027a0: 273c 6365 6e74 6572 3e3c 623e 272b 782b  '<center><b>'+x+
+000027b0: 273c 2f62 3e3c 2f63 656e 7465 723e 2720  '</b></center>' 
+000027c0: 2b20 793b 0a73 1400 0000 7265 7475 726e  + y;.s....return
+000027d0: 2074 6f6f 6c74 6970 5f73 7472 3b0a 7304   tooltip_str;.s.
+000027e0: 0000 007d 293b 0a73 1f00 0000 7661 7220  ...});.s....var 
+000027f0: 7820 3d20 5374 7269 6e67 2867 7261 7068  x = String(graph
+00002800: 2e70 6f69 6e74 2e78 293b 0a73 1f00 0000  .point.x);.s....
+00002810: 7661 7220 7920 3d20 5374 7269 6e67 2867  var y = String(g
+00002820: 7261 7068 2e70 6f69 6e74 2e79 293b 0a73  raph.point.y);.s
+00002830: 4200 0000 746f 6f6c 7469 705f 7374 7220  B...tooltip_str 
+00002840: 3d20 273c 6365 6e74 6572 3e3c 623e 272b  = '<center><b>'+
+00002850: 6b65 792b 273c 2f62 3e3c 2f63 656e 7465  key+'</b></cente
+00002860: 723e 2720 2b20 7920 2b20 2720 6174 2027  r>' + y + ' at '
+00002870: 202b 2078 3b0a 7341 0000 0076 6172 2078   + x;.sA...var x
+00002880: 203d 2064 332e 7469 6d65 2e66 6f72 6d61   = d3.time.forma
+00002890: 7428 2725 7327 2928 6e65 7720 4461 7465  t('%s')(new Date
+000028a0: 2870 6172 7365 496e 7428 6772 6170 682e  (parseInt(graph.
+000028b0: 706f 696e 742e 7829 2929 3b0a 7342 0000  point.x)));.sB..
+000028c0: 0074 6f6f 6c74 6970 5f73 7472 203d 2027  .tooltip_str = '
+000028d0: 3c63 656e 7465 723e 3c62 3e27 2b6b 6579  <center><b>'+key
+000028e0: 2b27 3c2f 623e 3c2f 6365 6e74 6572 3e27  +'</b></center>'
+000028f0: 202b 2079 202b 2027 206f 6e20 2720 2b20   + y + ' on ' + 
+00002900: 783b 0a4e 2807 0000 0052 3c00 0000 524f  x;.N(....R<...RO
+00002910: 0000 0052 0e00 0000 5204 0000 0052 3e00  ...R....R....R>.
+00002920: 0000 740c 0000 0063 6861 7274 746f 6f6c  ..t....charttool
+00002930: 7469 7052 1300 0000 2801 0000 0052 1c00  tipR....(....R..
+00002940: 0000 2800 0000 0028 0000 0000 734d 0000  ..(....(....sM..
+00002950: 002f 686f 6d65 2f61 7265 736b 692f 7075  ./home/areski/pu
+00002960: 626c 6963 5f68 746d 6c2f 646a 616e 676f  blic_html/django
+00002970: 2f4d 7950 726f 6a65 6374 732f 6e76 6433  /MyProjects/nvd3
+00002980: 2f70 7974 686f 6e2d 6e76 6433 2f6e 7664  /python-nvd3/nvd
+00002990: 332f 4e56 4433 4368 6172 742e 7079 7414  3/NVD3Chart.pyt.
+000029a0: 0000 0062 7569 6c64 5f63 7573 746f 6d5f  ...build_custom_
+000029b0: 746f 6f6c 7469 703f 0100 0073 0c00 0000  tooltip?...s....
+000029c0: 0002 0901 0901 0f06 5f08 6309 6301 0000  ........_.c.c...
+000029d0: 0007 0000 0009 0000 0043 0000 0073 d403  .........C...s..
+000029e0: 0000 6401 007c 0000 5f00 007c 0000 6a01  ..d..|.._..|..j.
+000029f0: 0072 2400 7c00 0004 6a00 0064 0200 3702  .r$.|...j..d..7.
+00002a00: 5f00 006e 0000 7c00 0004 6a00 0074 0200  _..n..|...j..t..
+00002a10: 8300 0037 025f 0000 7c00 006a 0300 7251  ...7._..|..j..rQ
+00002a20: 007c 0000 046a 0000 6403 0037 025f 0000  .|...j..d..7._..
+00002a30: 6e00 007c 0000 046a 0000 6404 0037 025f  n..|...j..d..7._
+00002a40: 0000 7c00 0004 6a00 0074 0200 6405 0083  ..|...j..t..d...
+00002a50: 0100 6406 007c 0000 6a04 0016 1737 025f  ..d..|..j....7._
+00002a60: 0000 7c00 006a 0400 6407 006b 0300 72c8  ..|..j..d..k..r.
+00002a70: 007c 0000 6a05 000c 72c8 007c 0000 6a06  .|..j...r..|..j.
+00002a80: 0072 c800 7c00 0004 6a00 0074 0200 6405  .r..|...j..t..d.
+00002a90: 0083 0100 6408 007c 0000 6a06 0016 1737  ....d..|..j....7
+00002aa0: 025f 0000 71c8 006e 0000 7c00 006a 0700  ._..q..n..|..j..
+00002ab0: 72ed 007c 0000 046a 0000 7402 0064 0500  r..|...j..t..d..
+00002ac0: 8301 0064 0900 1737 025f 0000 6e00 007c  ...d...7._..n..|
+00002ad0: 0000 6a04 0064 0700 6b03 0072 8801 7889  ..j..d..k..r..x.
+00002ae0: 0074 0800 7c00 006a 0900 6a0a 0083 0000  .t..|..j..j.....
+00002af0: 8301 0044 5d6f 005c 0200 7d01 007d 0200  ...D]o.\..}..}..
+00002b00: 7c00 0004 6a00 0074 0200 6405 0083 0100  |...j..t..d.....
+00002b10: 640a 007c 0100 1617 3702 5f00 0078 4300  d..|....7._..xC.
+00002b20: 7408 007c 0200 6a0a 0083 0000 8301 0044  t..|..j........D
+00002b30: 5d2f 005c 0200 7d03 007d 0400 7c00 0004  ]/.\..}..}..|...
+00002b40: 6a00 0074 0200 640b 0083 0100 640c 007c  j..t..d.....d..|
+00002b50: 0300 7c04 0066 0200 1617 3702 5f00 0071  ..|..f....7._..q
+00002b60: 4e01 5771 1201 576e 0000 7c00 006a 0b00  N.Wq..Wn..|..j..
+00002b70: 72aa 017c 0000 046a 0c00 640d 007c 0000  r..|...j..d..|..
+00002b80: 6a0b 0016 3702 5f0c 006e 0000 7c00 006a  j...7._..n..|..j
+00002b90: 0d00 72cc 017c 0000 046a 0c00 640e 007c  ..r..|...j..d..|
+00002ba0: 0000 6a0d 0016 3702 5f0c 006e 0000 640f  ..j...7._..n..d.
+00002bb0: 007c 0000 6a0e 0016 7d05 007c 0000 6a04  .|..j...}..|..j.
+00002bc0: 0064 0700 6b02 0072 f801 6410 007c 0000  .d..k..r..d..|..
+00002bd0: 6a0e 0016 7d05 006e 0000 7c00 006a 0f00  j...}..n..|..j..
+00002be0: 6401 006b 0200 7213 0264 1100 7c00 005f  d..k..r..d..|.._
+00002bf0: 0f00 6e00 007c 0000 6a10 0083 0000 017c  ..n..|..j......|
+00002c00: 0000 046a 0000 7c00 006a 1100 3702 5f00  ...j..|..j..7._.
+00002c10: 007c 0000 6a04 0064 1200 6b03 0072 7f02  .|..j..d..k..r..
+00002c20: 7c00 006a 1200 7263 027c 0000 046a 0000  |..j..rc.|...j..
+00002c30: 7402 0064 0500 8301 0064 1300 1737 025f  t..d.....d...7._
+00002c40: 0000 717f 027c 0000 046a 0000 7402 0064  ..q..|...j..t..d
+00002c50: 0500 8301 0064 1400 1737 025f 0000 6e00  .....d...7._..n.
+00002c60: 007c 0000 6a04 0064 0700 6b02 0072 cf02  .|..j..d..k..r..
+00002c70: 7c00 006a 1300 72b3 027c 0000 046a 0000  |..j..r..|...j..
+00002c80: 7402 0064 0500 8301 0064 1500 1737 025f  t..d.....d...7._
+00002c90: 0000 71cf 027c 0000 046a 0000 7402 0064  ..q..|...j..t..d
+00002ca0: 0500 8301 0064 1600 1737 025f 0000 6e00  .....d...7._..n.
+00002cb0: 007c 0000 046a 0000 7402 0064 0500 8301  .|...j..t..d....
+00002cc0: 0064 1700 7c00 006a 0e00 1617 7402 0064  .d..|..j....t..d
+00002cd0: 0b00 8301 0017 6418 007c 0500 1617 7402  ......d..|....t.
+00002ce0: 0064 0b00 8301 0017 6419 0017 7402 0064  .d......d...t..d
+00002cf0: 0b00 8301 0017 7c00 006a 0c00 1774 0200  ......|..j...t..
+00002d00: 640b 0083 0100 1764 1a00 1737 025f 0000  d......d...7._..
+00002d10: 7c00 006a 1400 7253 037c 0000 046a 0000  |..j..rS.|...j..
+00002d20: 7402 0064 1b00 8301 0064 1c00 1737 025f  t..d.....d...7._
+00002d30: 0000 6e00 007c 0000 046a 0000 7402 0064  ..n..|...j..t..d
+00002d40: 1b00 8301 0064 1d00 1737 025f 0000 7c00  .....d...7._..|.
+00002d50: 006a 0300 7287 037c 0000 046a 0000 641e  .j..r..|...j..d.
+00002d60: 0037 025f 0000 6e00 0074 1500 6a16 007c  .7._..n..t..j..|
+00002d70: 0000 6a17 0083 0100 7d06 007c 0000 046a  ..j.....}..|...j
+00002d80: 0000 641f 007c 0000 6a0e 007c 0600 6602  ..d..|..j..|..f.
+00002d90: 0016 3702 5f00 007c 0000 6a01 0072 d003  ..7._..|..j..r..
+00002da0: 7c00 0004 6a00 0064 2000 3702 5f00 006e  |...j..d .7._..n
+00002db0: 0000 6421 0053 2822 0000 0073 2600 0000  ..d!.S("...s&...
+00002dc0: 6765 6e65 7261 7465 206a 6176 6173 6372  generate javascr
+00002dd0: 6970 7420 636f 6465 2066 6f72 2074 6865  ipt code for the
+00002de0: 2063 6861 7274 5206 0000 0073 2100 0000   chartR....s!...
+00002df0: 0a3c 7363 7269 7074 2074 7970 653d 2274  .<script type="t
+00002e00: 6578 742f 6a61 7661 7363 7269 7074 223e  ext/javascript">
+00002e10: 0a73 0d00 0000 2428 6675 6e63 7469 6f6e  .s....$(function
+00002e20: 2829 7b73 1900 0000 6e76 2e61 6464 4772  (){s....nv.addGr
+00002e30: 6170 6828 6675 6e63 7469 6f6e 2829 207b  aph(function() {
+00002e40: 0a69 0200 0000 731c 0000 0076 6172 2063  .i....s....var c
+00002e50: 6861 7274 203d 206e 762e 6d6f 6465 6c73  hart = nv.models
+00002e60: 2e25 7328 293b 0a52 2800 0000 7324 0000  .%s();.R(...s$..
+00002e70: 0063 6861 7274 2e63 6f6c 6f72 2864 332e  .chart.color(d3.
+00002e80: 7363 616c 652e 2573 2829 2e72 616e 6765  scale.%s().range
+00002e90: 2829 293b 0a73 1400 0000 6368 6172 742e  ());.s....chart.
+00002ea0: 7374 6163 6b65 6428 7472 7565 293b 7309  stacked(true);s.
+00002eb0: 0000 0063 6861 7274 2e25 730a 6903 0000  ...chart.%s.i...
+00002ec0: 0073 0900 0000 2e25 7328 2573 293b 0a73  .s.....%s(%s);.s
+00002ed0: 1300 0000 2e61 7474 7228 2777 6964 7468  .....attr('width
+00002ee0: 272c 2025 7329 0a73 1400 0000 2e61 7474  ', %s).s.....att
+00002ef0: 7228 2768 6569 6768 7427 2c20 2573 290a  r('height', %s).
+00002f00: 7307 0000 0064 6174 615f 2573 7313 0000  s....data_%ss...
+00002f10: 005b 6461 7461 5f25 735b 305d 2e76 616c  .[data_%s[0].val
+00002f20: 7565 735d 731f 0000 0076 6172 2079 203d  ues]s....var y =
+00002f30: 2053 7472 696e 6728 6772 6170 682e 706f   String(graph.po
+00002f40: 696e 742e 7929 3b0a 7410 0000 0064 6973  int.y);.t....dis
+00002f50: 6372 6574 6542 6172 4368 6172 7473 1800  creteBarCharts..
+00002f60: 0000 6368 6172 742e 7368 6f77 4c65 6765  ..chart.showLege
+00002f70: 6e64 2874 7275 6529 3b0a 7319 0000 0063  nd(true);.s....c
+00002f80: 6861 7274 2e73 686f 774c 6567 656e 6428  hart.showLegend(
+00002f90: 6661 6c73 6529 3b0a 7318 0000 0063 6861  false);.s....cha
+00002fa0: 7274 2e73 686f 774c 6162 656c 7328 7472  rt.showLabels(tr
+00002fb0: 7565 293b 0a73 1900 0000 6368 6172 742e  ue);.s....chart.
+00002fc0: 7368 6f77 4c61 6265 6c73 2866 616c 7365  showLabels(false
+00002fd0: 293b 0a73 1500 0000 6433 2e73 656c 6563  );.s....d3.selec
+00002fe0: 7428 2723 2573 2073 7667 2729 0a73 0b00  t('#%s svg').s..
+00002ff0: 0000 2e64 6174 756d 2825 7329 0a73 1c00  ...datum(%s).s..
+00003000: 0000 2e74 7261 6e73 6974 696f 6e28 292e  ...transition().
+00003010: 6475 7261 7469 6f6e 2835 3030 290a 730f  duration(500).s.
+00003020: 0000 002e 6361 6c6c 2863 6861 7274 293b  ....call(chart);
+00003030: 0a0a 6901 0000 0073 2500 0000 6e76 2e75  ..i....s%...nv.u
+00003040: 7469 6c73 2e77 696e 646f 7752 6573 697a  tils.windowResiz
+00003050: 6528 6368 6172 742e 7570 6461 7465 293b  e(chart.update);
+00003060: 0a73 1100 0000 7265 7475 726e 2063 6861  .s....return cha
+00003070: 7274 3b0a 7d29 3b73 0400 0000 0a7d 293b  rt;.});s.....});
+00003080: 730c 0000 0064 6174 615f 2573 3d25 733b  s....data_%s=%s;
+00003090: 0a73 0900 0000 3c2f 7363 7269 7074 3e4e  .s....</script>N
+000030a0: 2818 0000 0052 5600 0000 740d 0000 0074  (....RV...t....t
+000030b0: 6167 5f73 6372 6970 745f 6a73 5204 0000  ag_script_jsR...
+000030c0: 0052 1600 0000 520e 0000 0052 2900 0000  .R....R....R)...
+000030d0: 5217 0000 0052 0800 0000 523b 0000 0052  R....R....R;...R
+000030e0: 1000 0000 7405 0000 0069 7465 6d73 524b  ....t....itemsRK
+000030f0: 0000 0074 0f00 0000 6433 5f73 656c 6563  ...t....d3_selec
+00003100: 745f 6578 7472 6152 4900 0000 5215 0000  t_extraRI...R...
+00003110: 0052 3e00 0000 5263 0000 0052 6200 0000  .R>...Rc...Rb...
+00003120: 520a 0000 0052 0b00 0000 5209 0000 0074  R....R....R....t
+00003130: 0400 0000 6a73 6f6e 7405 0000 0064 756d  ....jsont....dum
+00003140: 7073 520f 0000 0028 0700 0000 521c 0000  psR....(....R...
+00003150: 0074 0900 0000 6178 6973 5f6e 616d 6574  .t....axis_namet
+00003160: 0100 0000 6174 0400 0000 6174 7472 7405  ....at....attrt.
+00003170: 0000 0076 616c 7565 7405 0000 0064 6174  ...valuet....dat
+00003180: 756d 7409 0000 0073 6572 6965 735f 6a73  umt....series_js
+00003190: 2800 0000 0028 0000 0000 734d 0000 002f  (....(....sM.../
+000031a0: 686f 6d65 2f61 7265 736b 692f 7075 626c  home/areski/publ
+000031b0: 6963 5f68 746d 6c2f 646a 616e 676f 2f4d  ic_html/django/M
+000031c0: 7950 726f 6a65 6374 732f 6e76 6433 2f70  yProjects/nvd3/p
+000031d0: 7974 686f 6e2d 6e76 6433 2f6e 7664 332f  ython-nvd3/nvd3/
+000031e0: 4e56 4433 4368 6172 742e 7079 5258 0000  NVD3Chart.pyRX..
+000031f0: 005c 0100 0073 6000 0000 0003 0901 0901  .\...s`.........
+00003200: 1202 1202 0901 1202 0f02 2002 1901 0901  .......... .....
+00003210: 2602 0901 1c07 0f01 2201 1d01 1f01 2e02  &.......".......
+00003220: 0901 1901 0901 1902 0d01 0f01 1004 0f01  ................
+00003230: 0c02 0a01 1202 0f01 0901 1c02 1c03 0f01  ................
+00003240: 0901 1c02 1c03 0704 5802 0901 1c01 1902  ........X.......
+00003250: 0901 1203 1201 1c01 0901 6305 0000 0006  ..........c.....
+00003260: 0000 0003 0000 0043 0000 0073 9900 0000  .......C...s....
+00003270: 6900 007d 0500 7c03 0072 3600 7c03 0064  i..}..|..r6.|..d
+00003280: 0100 6b02 0072 2500 6402 007c 0500 6403  ..k..r%.d..|..d.
+00003290: 003c 7136 0064 0400 7c03 0016 7c05 0064  .<q6.d..|...|..d
+000032a0: 0300 3c6e 0000 7c02 0072 4900 7c02 007c  ..<n..|..rI.|..|
+000032b0: 0500 6405 003c 6e00 007c 0400 7288 007c  ..d..<n..|..r..|
+000032c0: 0300 7c00 005f 0000 6406 007c 0000 6a00  ..|.._..d..|..j.
+000032d0: 0016 7c05 0064 0300 3c7c 0100 6407 0019  ..|..d..<|..d...
+000032e0: 6408 006b 0200 7288 0074 0100 7c00 005f  d..k..r..t..|.._
+000032f0: 0200 7188 006e 0000 7c05 007c 0000 6a03  ..q..n..|..|..j.
+00003300: 007c 0100 3c64 0900 5328 0a00 0000 731f  .|..<d..S(....s.
+00003310: 0000 000a 2020 2020 2020 2020 4372 6561  ....        Crea
+00003320: 7465 2058 2d61 7869 730a 2020 2020 2020  te X-axis.      
+00003330: 2020 7405 0000 0041 4d5f 504d 732e 0000    t....AM_PMs...
+00003340: 0066 756e 6374 696f 6e28 6429 207b 2072  .function(d) { r
+00003350: 6574 7572 6e20 6765 745f 616d 5f70 6d28  eturn get_am_pm(
+00003360: 7061 7273 6549 6e74 2864 2929 3b20 7d74  parseInt(d)); }t
+00003370: 0a00 0000 7469 636b 466f 726d 6174 7310  ....tickFormats.
+00003380: 0000 0064 332e 666f 726d 6174 2827 2c25  ...d3.format(',%
+00003390: 7327 2974 0900 0000 6178 6973 4c61 6265  s')t....axisLabe
+000033a0: 6c73 4300 0000 6675 6e63 7469 6f6e 2864  lsC...function(d
+000033b0: 2920 7b20 7265 7475 726e 2064 332e 7469  ) { return d3.ti
+000033c0: 6d65 2e66 6f72 6d61 7428 2725 7327 2928  me.format('%s')(
+000033d0: 6e65 7720 4461 7465 2870 6172 7365 496e  new Date(parseIn
+000033e0: 7428 6429 2929 207d 0a69 0000 0000 5223  t(d))) }.i....R#
+000033f0: 0000 004e 2804 0000 0074 0a00 0000 6461  ...N(....t....da
+00003400: 7465 666f 726d 6174 5218 0000 0074 0b00  teformatR....t..
+00003410: 0000 785f 6178 6973 5f64 6174 6552 1000  ..x_axis_dateR..
+00003420: 0000 2806 0000 0052 1c00 0000 5215 0000  ..(....R....R...
+00003430: 0074 0500 0000 6c61 6265 6c74 0600 0000  .t....labelt....
+00003440: 666f 726d 6174 7404 0000 0064 6174 6574  formatt....datet
+00003450: 0400 0000 6178 6973 2800 0000 0028 0000  ....axis(....(..
+00003460: 0000 734d 0000 002f 686f 6d65 2f61 7265  ..sM.../home/are
+00003470: 736b 692f 7075 626c 6963 5f68 746d 6c2f  ski/public_html/
+00003480: 646a 616e 676f 2f4d 7950 726f 6a65 6374  django/MyProject
+00003490: 732f 6e76 6433 2f70 7974 686f 6e2d 6e76  s/nvd3/python-nv
+000034a0: 6433 2f6e 7664 332f 4e56 4433 4368 6172  d3/nvd3/NVD3Char
+000034b0: 742e 7079 740d 0000 0063 7265 6174 655f  t.pyt....create_
+000034c0: 785f 6178 6973 b001 0000 731a 0000 0000  x_axis....s.....
+000034d0: 0406 0106 010c 010d 0211 0206 010d 0306  ................
+000034e0: 0109 0111 0210 010f 0363 0500 0000 0600  .........c......
+000034f0: 0000 0400 0000 4300 0000 735a 0000 0069  ......C...sZ...i
+00003500: 0000 7d05 007c 0400 721f 007c 0300 721f  ..}..|..r..|..r.
+00003510: 007c 0300 7c05 0064 0100 3c6e 1700 7c03  .|..|..d..<n..|.
+00003520: 0072 3600 6402 007c 0300 167c 0500 6401  .r6.d..|...|..d.
+00003530: 003c 6e00 007c 0200 7249 007c 0200 7c05  .<n..|..rI.|..|.
+00003540: 0064 0300 3c6e 0000 7c05 007c 0000 6a00  .d..<n..|..|..j.
+00003550: 007c 0100 3c64 0400 5328 0500 0000 731f  .|..<d..S(....s.
+00003560: 0000 000a 2020 2020 2020 2020 4372 6561  ....        Crea
+00003570: 7465 2059 2d61 7869 730a 2020 2020 2020  te Y-axis.      
+00003580: 2020 5271 0000 0073 1000 0000 6433 2e66    Rq...s....d3.f
+00003590: 6f72 6d61 7428 272c 2573 2729 5272 0000  ormat(',%s')Rr..
+000035a0: 004e 2801 0000 0052 1000 0000 2806 0000  .N(....R....(...
+000035b0: 0052 1c00 0000 5215 0000 0052 7500 0000  .R....R....Ru...
+000035c0: 5276 0000 0074 0d00 0000 6375 7374 6f6d  Rv...t....custom
+000035d0: 5f66 6f72 6d61 7452 7800 0000 2800 0000  _formatRx...(...
+000035e0: 0028 0000 0000 734d 0000 002f 686f 6d65  .(....sM.../home
+000035f0: 2f61 7265 736b 692f 7075 626c 6963 5f68  /areski/public_h
+00003600: 746d 6c2f 646a 616e 676f 2f4d 7950 726f  tml/django/MyPro
+00003610: 6a65 6374 732f 6e76 6433 2f70 7974 686f  jects/nvd3/pytho
+00003620: 6e2d 6e76 6433 2f6e 7664 332f 4e56 4433  n-nvd3/nvd3/NVD3
+00003630: 4368 6172 742e 7079 740d 0000 0063 7265  Chart.pyt....cre
+00003640: 6174 655f 795f 6178 6973 c901 0000 7310  ate_y_axis....s.
+00003650: 0000 0000 0406 020c 010d 0206 0111 0206  ................
+00003660: 010d 034e 2833 0000 0052 0d00 0000 740a  ...N(3...R....t.
+00003670: 0000 005f 5f6d 6f64 756c 655f 5f74 0700  ...__module__t..
+00003680: 0000 5f5f 646f 635f 5f52 1400 0000 5273  ..__doc__R....Rs
+00003690: 0000 0052 0f00 0000 5210 0000 0052 6100  ...R....R....Ra.
+000036a0: 0000 5253 0000 0052 5d00 0000 7404 0000  ..RS...R]...t...
+000036b0: 004e 6f6e 6552 4900 0000 524b 0000 0052  .NoneRI...RK...R
+000036c0: 0e00 0000 5267 0000 0074 0500 0000 4661  ....Rg...t....Fa
+000036d0: 6c73 6552 7400 0000 5209 0000 0052 0800  lseRt...R....R..
+000036e0: 0000 5211 0000 0052 5500 0000 524d 0000  ..R....RU...RM..
+000036f0: 0052 5600 0000 523c 0000 0052 4f00 0000  .RV...R<...RO...
+00003700: 5262 0000 0052 3e00 0000 5217 0000 0052  Rb...R>...R....R
+00003710: 2900 0000 5218 0000 0052 6500 0000 5213  )...R....Re...R.
+00003720: 0000 0074 0d00 0000 785f 6178 6973 5f66  ...t....x_axis_f
+00003730: 6f72 6d61 7452 0a00 0000 520b 0000 0052  ormatR....R....R
+00003740: 1f00 0000 5248 0000 0052 4a00 0000 524c  ....RH...RJ...RL
+00003750: 0000 0052 4e00 0000 5250 0000 0052 5100  ...RN...RP...RQ.
+00003760: 0000 5254 0000 0052 5a00 0000 5252 0000  ..RT...RZ...RR..
+00003770: 0052 5c00 0000 5257 0000 0052 6300 0000  .R\...RW...Rc...
+00003780: 5258 0000 0052 7900 0000 527b 0000 0028  RX...Ry...R{...(
+00003790: 0000 0000 2800 0000 0028 0000 0000 734d  ....(....(....sM
+000037a0: 0000 002f 686f 6d65 2f61 7265 736b 692f  .../home/areski/
+000037b0: 7075 626c 6963 5f68 746d 6c2f 646a 616e  public_html/djan
+000037c0: 676f 2f4d 7950 726f 6a65 6374 732f 6e76  go/MyProjects/nv
+000037d0: 6433 2f70 7974 686f 6e2d 6e76 6433 2f6e  d3/python-nvd3/n
+000037e0: 7664 332f 4e56 4433 4368 6172 742e 7079  vd3/NVD3Chart.py
+000037f0: 5205 0000 0028 0000 0073 5c00 0000 0620  R....(...s\.... 
+00003800: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+00003810: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+00003820: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+00003830: 0601 0601 0601 0601 0601 0602 1232 0f5c  .............2.\
+00003840: 0904 0904 0904 0c04 0904 0905 090a 090c  ................
+00003850: 0908 0913 091d 0954 1219 6300 0000 0004  .......T..c.....
+00003860: 0000 000b 0000 0043 0000 0073 5900 0000  .......C...sY...
+00003870: 6401 007d 0000 7400 0064 0200 7c00 0064  d..}..t..d..|..d
+00003880: 0300 6404 0083 0002 7d01 007c 0100 6a01  ..d.....}..|..j.
+00003890: 0064 0500 6406 0064 0700 6408 0064 0900  .d..d..d..d..d..
+000038a0: 640a 0064 0b00 7402 0064 0c00 640d 0083  d..d..t..d..d...
+000038b0: 0204 017c 0100 6a03 0083 0000 5c02 007d  ...|..j.....\..}
+000038c0: 0200 7d03 0064 0e00 5328 0f00 0000 732c  ..}..d..S(....s,
+000038d0: 0000 000a 2020 2020 5061 7273 6520 6f70  ....    Parse op
+000038e0: 7469 6f6e 7320 616e 6420 7072 6f63 6573  tions and proces
+000038f0: 7320 636f 6d6d 616e 6473 0a20 2020 2073  s commands.    s
+00003900: 1800 0000 7573 6167 653a 206e 7664 332e  ....usage: nvd3.
+00003910: 7079 205b 6f70 7469 6f6e 735d 7405 0000  py [options]t...
+00003920: 0075 7361 6765 7407 0000 0076 6572 7369  .usaget....versi
+00003930: 6f6e 732c 0000 0070 7974 686f 6e2d 6e76  ons,...python-nv
+00003940: 6433 2030 2e32 2e32 202d 2050 7974 686f  d3 0.2.2 - Pytho
+00003950: 6e20 7772 6170 7065 7220 666f 7220 6e76  n wrapper for nv
+00003960: 6433 2073 0200 0000 2d71 7307 0000 002d  d3 s....-qs....-
+00003970: 2d71 7569 6574 7406 0000 0061 6374 696f  -quiett....actio
+00003980: 6e74 0b00 0000 7374 6f72 655f 6661 6c73  nt....store_fals
+00003990: 6574 0400 0000 6465 7374 7407 0000 0076  et....destt....v
+000039a0: 6572 626f 7365 7407 0000 0064 6566 6175  erboset....defau
+000039b0: 6c74 7404 0000 0068 656c 7073 1e00 0000  ltt....helps....
+000039c0: 646f 6e27 7420 7072 696e 7420 6d65 7373  don't print mess
+000039d0: 6167 6573 2074 6f20 7374 646f 7574 4e28  ages to stdoutN(
+000039e0: 0400 0000 5200 0000 0074 0a00 0000 6164  ....R....t....ad
+000039f0: 645f 6f70 7469 6f6e 5218 0000 0074 0a00  d_optionR....t..
+00003a00: 0000 7061 7273 655f 6172 6773 2804 0000  ..parse_args(...
+00003a10: 0052 8100 0000 7406 0000 0070 6172 7365  .R....t....parse
+00003a20: 7274 0700 0000 6f70 7469 6f6e 7374 0400  rt....optionst..
+00003a30: 0000 6172 6773 2800 0000 0028 0000 0000  ..args(....(....
+00003a40: 734d 0000 002f 686f 6d65 2f61 7265 736b  sM.../home/aresk
+00003a50: 692f 7075 626c 6963 5f68 746d 6c2f 646a  i/public_html/dj
+00003a60: 616e 676f 2f4d 7950 726f 6a65 6374 732f  ango/MyProjects/
+00003a70: 6e76 6433 2f70 7974 686f 6e2d 6e76 6433  nvd3/python-nvd3
+00003a80: 2f6e 7664 332f 4e56 4433 4368 6172 742e  /nvd3/NVD3Chart.
+00003a90: 7079 7405 0000 005f 6d61 696e dc01 0000  pyt...._main....
+00003aa0: 730c 0000 0000 0506 0115 010f 0112 0107  s...............
+00003ab0: 0274 0800 0000 5f5f 6d61 696e 5f5f 280c  .t....__main__(.
+00003ac0: 0000 0052 7d00 0000 7408 0000 006f 7074  ...R}...t....opt
+00003ad0: 7061 7273 6552 0000 0000 7406 0000 0073  parseR....t....s
+00003ae0: 7472 696e 6752 0100 0000 5268 0000 0052  tringR....Rh...R
+00003af0: 1200 0000 5211 0000 0052 0400 0000 5205  ....R....R....R.
+00003b00: 0000 0052 8e00 0000 520d 0000 0028 0000  ...R....R....(..
+00003b10: 0000 2800 0000 0028 0000 0000 734d 0000  ..(....(....sM..
+00003b20: 002f 686f 6d65 2f61 7265 736b 692f 7075  ./home/areski/pu
+00003b30: 626c 6963 5f68 746d 6c2f 646a 616e 676f  blic_html/django
+00003b40: 2f4d 7950 726f 6a65 6374 732f 6e76 6433  /MyProjects/nvd3
+00003b50: 2f70 7974 686f 6e2d 6e76 6433 2f6e 7664  /python-nvd3/nvd
+00003b60: 332f 4e56 4433 4368 6172 742e 7079 7408  3/NVD3Chart.pyt.
+00003b70: 0000 003c 6d6f 6475 6c65 3e0a 0000 0073  ...<module>....s
+00003b80: 1600 0000 0602 1001 1001 0c05 060b 0a03  ................
+00003b90: 0c07 13ff 00b5 090e 0c01                 ..........
```

### Comparing `python-nvd3-0.8.0/nvd3/scatterChart.pyc` & `python-nvd3-0.9.0/nvd3/scatterChart.pyc`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/__init__.pyc` & `python-nvd3-0.9.0/nvd3/__init__.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 4710 dc51 6300 0000 0000 0000  ....G..Qc.......
+00000000: 03f3 0d0a cab5 0c52 6300 0000 0000 0000  .......Rc.......
 00000010: 0003 0000 0040 0000 0073 8c01 0000 6400  .....@...s....d.
 00000020: 005a 0000 6401 005a 0100 6402 0064 0300  .Z..d..Z..d..d..
 00000030: 6c02 006d 0200 5a02 0001 6402 0064 0400  l..m..Z...d..d..
 00000040: 6c03 006d 0300 5a03 0001 6402 0064 0500  l..m..Z...d..d..
 00000050: 6c04 006d 0400 5a04 0001 6402 0064 0600  l..m..Z...d..d..
 00000060: 6c05 006d 0500 5a05 0001 6402 0064 0700  l..m..Z...d..d..
 00000070: 6c06 006d 0600 5a06 0001 6402 0064 0800  l..m..Z...d..d..
@@ -36,15 +36,15 @@
 00000230: 6f72 2064 332e 6a73 2077 6974 686f 7574  or d3.js without
 00000240: 2074 616b 696e 6720 6177 6179 2074 6865   taking away the
 00000250: 2070 6f77 6572 2074 6861 7420 6433 2e6a   power that d3.j
 00000260: 7320 6769 7665 7320 796f 752e 0a0a 5072  s gives you...Pr
 00000270: 6f6a 6563 7420 6c6f 6361 7469 6f6e 203a  oject location :
 00000280: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000290: 636f 6d2f 6172 6573 6b69 2f70 7974 686f  com/areski/pytho
-000002a0: 6e2d 6e76 6433 0a73 0500 0000 302e 372e  n-nvd3.s....0.7.
+000002a0: 6e2d 6e76 6433 0a73 0500 0000 302e 382e  n-nvd3.s....0.8.
 000002b0: 3069 0100 0000 2801 0000 0074 0900 0000  0i....(....t....
 000002c0: 6c69 6e65 4368 6172 7428 0100 0000 7408  lineChart(....t.
 000002d0: 0000 0070 6965 4368 6172 7428 0100 0000  ...pieChart(....
 000002e0: 7412 0000 006c 696e 6557 6974 6846 6f63  t....lineWithFoc
 000002f0: 7573 4368 6172 7428 0100 0000 7410 0000  usChart(....t...
 00000300: 0073 7461 636b 6564 4172 6561 4368 6172  .stackedAreaChar
 00000310: 7428 0100 0000 7417 0000 006d 756c 7469  t(....t....multi
```

### Comparing `python-nvd3-0.8.0/nvd3/multiBarHorizontalChart.pyc` & `python-nvd3-0.9.0/nvd3/multiBarHorizontalChart.pyc`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/lineWithFocusChart.pyc` & `python-nvd3-0.9.0/nvd3/lineWithFocusChart.pyc`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/linePlusBarChart.py` & `python-nvd3-0.9.0/nvd3/linePlusBarChart.py`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/pieChart.py` & `python-nvd3-0.9.0/nvd3/pieChart.py`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/nvd3/pieChart.pyc` & `python-nvd3-0.9.0/nvd3/pieChart.pyc`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/setup.py` & `python-nvd3-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-nvd3-0.8.0/PKG-INFO` & `python-nvd3-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-nvd3
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python NVD3
 Home-page: http://github.com/areski/python-nvd3
 Author: Belaid Arezqui
 Author-email: areski@gmail.com
 License: MIT license
 Description: Python Wrapper for NVD3 - It's time for beautiful charts
         ========================================================
@@ -32,14 +32,31 @@
         Install, upgrade and uninstall python-nvd3 with these commands::
         
             $ pip install python-nvd3
             $ pip install --upgrade python-nvd3
             $ pip uninstall python-nvd3
         
         
+        Dependecies
+        -----------
+        
+        You will "bower" installed in order to install D3 and NvD3, see bower website for futher info : http://bower.io/
+        
+        Bower depends on Node and npm. It's installed globally using npm::
+        
+            npm install -g bower
+        
+        Then in your directory where you will use python-nvd3, just type the following::
+        
+            $ bower install d3
+            $ bower install nvd3
+        
+        This will create a directory "bower_components" where d3 & nvd3 will be installed.
+        
+        
         Usage
         -----
         
         After installation use python-nvd3 as follows ::
         
             from nvd3 import pieChart
```

