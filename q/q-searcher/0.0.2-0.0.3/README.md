# Comparing `tmp/q_searcher-0.0.2.tar.gz` & `tmp/q_searcher-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q_searcher-0.0.2.tar", max compression
+gzip compressed data, was "q_searcher-0.0.3.tar", max compression
```

## Comparing `q_searcher-0.0.2.tar` & `q_searcher-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1093 2023-11-24 16:54:00.910269 q_searcher-0.0.2/LICENSE
--rw-r--r--   0        0        0      706 2024-02-29 03:10:50.589504 q_searcher-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1333 2024-02-29 03:23:43.643452 q_searcher-0.0.2/README.md
--rw-r--r--   0        0        0       66 2024-02-29 03:34:18.482036 q_searcher-0.0.2/src/q_searcher/__init__.py
--rw-r--r--   0        0        0       66 2024-02-29 03:35:42.311363 q_searcher-0.0.2/src/q_searcher/const.py
--rw-r--r--   0        0        0     1159 2024-03-28 05:16:13.729613 q_searcher-0.0.2/src/q_searcher/init.py
--rw-r--r--   0        0        0     1529 2024-02-29 03:37:01.501897 q_searcher-0.0.2/src/q_searcher/search.py
--rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 q_searcher-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2024-04-22 03:13:22.905520 q_searcher-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0     1333 2024-04-22 03:13:22.905520 q_searcher-0.0.3/README.md
+-rwxr-xr-x   0        0        0      678 2024-04-22 03:14:15.665519 q_searcher-0.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0       63 2024-04-22 03:13:22.905520 q_searcher-0.0.3/src/q_searcher/__init__.py
+-rwxr-xr-x   0        0        0       64 2024-04-22 03:13:22.905520 q_searcher-0.0.3/src/q_searcher/const.py
+-rwxr-xr-x   0        0        0     1196 2024-04-22 03:13:22.905520 q_searcher-0.0.3/src/q_searcher/init.py
+-rwxr-xr-x   0        0        0     1468 2024-04-22 03:13:22.905520 q_searcher-0.0.3/src/q_searcher/search.py
+-rw-r--r--   0        0        0     1937 2024-04-22 03:14:17.558139 q_searcher-0.0.3/setup.py
+-rw-r--r--   0        0        0     1915 2024-04-22 03:14:17.558375 q_searcher-0.0.3/PKG-INFO
```

### Comparing `q_searcher-0.0.2/LICENSE` & `q_searcher-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `q_searcher-0.0.2/README.md` & `q_searcher-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `q_searcher-0.0.2/PKG-INFO` & `q_searcher-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
-Name: q_searcher
-Version: 0.0.2
+Name: q-searcher
+Version: 0.0.3
 Summary: 
 Author: UioSun
 Author-email: uiosun@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Project-URL: Homepage, https://github.com/freedom-island/q_searcher
 Project-URL: Issues, https://github.com/freedom-island/q_searcher/issues
 Project-URL: Website, https://www.uiosun.com/libs/q_searcher
 Description-Content-Type: text/markdown
 
 # 量化的时序函数包
```

