# Comparing `tmp/baysalt_christmas-1.1.3.tar.gz` & `tmp/baysalt_christmas-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-1.1.3.tar", last modified: Fri Jan  5 03:42:13 2024, max compression
+gzip compressed data, was "baysalt_christmas-1.1.4.tar", last modified: Mon Apr 22 09:13:02 2024, max compression
```

## Comparing `baysalt_christmas-1.1.3.tar` & `baysalt_christmas-1.1.4.tar`

### file list

```diff
@@ -1,45 +1,41 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-01-05 03:42:13.517974 baysalt_christmas-1.1.3/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-12-25 02:54:05.000000 baysalt_christmas-1.1.3/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-1.1.3/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4093 2024-01-05 03:42:13.517826 baysalt_christmas-1.1.3/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-1.1.3/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-01-05 03:42:13.514259 baysalt_christmas-1.1.3/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4093 2024-01-05 03:42:13.000000 baysalt_christmas-1.1.3/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      964 2024-01-05 03:42:13.000000 baysalt_christmas-1.1.3/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2024-01-05 03:42:13.000000 baysalt_christmas-1.1.3/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2024-01-05 03:42:13.000000 baysalt_christmas-1.1.3/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2024-01-05 03:42:13.000000 baysalt_christmas-1.1.3/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-01-05 03:42:13.515465 baysalt_christmas-1.1.3/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    22673 2023-09-24 17:35:32.000000 baysalt_christmas-1.1.3/christmas/Blogging.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-01-05 03:42:13.515783 baysalt_christmas-1.1.3/christmas/Pyshell/
--rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-1.1.3/christmas/Pyshell/RS_File.py
--rw-r--r--   0 christmas   (501) staff       (20)      232 2023-09-18 07:37:39.000000 baysalt_christmas-1.1.3/christmas/Pyshell/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     3787 2023-12-24 15:59:53.000000 baysalt_christmas-1.1.3/christmas/S_DateTime.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-01-05 03:42:13.516045 baysalt_christmas-1.1.3/christmas/SameAsMATLAB/
--rw-r--r--   0 christmas   (501) staff       (20)     1286 2023-11-27 09:14:09.000000 baysalt_christmas-1.1.3/christmas/SameAsMATLAB/CoorTrans.py
--rw-r--r--   0 christmas   (501) staff       (20)      236 2023-11-27 08:58:33.000000 baysalt_christmas-1.1.3/christmas/SameAsMATLAB/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-01-05 03:42:13.516290 baysalt_christmas-1.1.3/christmas/Standard/
--rw-r--r--   0 christmas   (501) staff       (20)      234 2023-09-18 07:38:49.000000 baysalt_christmas-1.1.3/christmas/Standard/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     5903 2023-10-08 09:19:02.000000 baysalt_christmas-1.1.3/christmas/Standard/xr_attrs.py
--rw-r--r--   0 christmas   (501) staff       (20)      479 2023-11-27 08:58:33.000000 baysalt_christmas-1.1.3/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     6246 2023-12-18 03:26:45.000000 baysalt_christmas-1.1.3/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1812 2023-09-24 17:45:18.000000 baysalt_christmas-1.1.3/christmas/cprintfs.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-01-05 03:42:13.516997 baysalt_christmas-1.1.3/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-1.1.3/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-1.1.3/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-1.1.3/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-01-05 03:42:13.517274 baysalt_christmas-1.1.3/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      245 2023-11-03 16:47:28.000000 baysalt_christmas-1.1.3/christmas/mncPy/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 christmas   (501) staff       (20)      278 2023-09-24 17:39:02.000000 baysalt_christmas-1.1.3/christmas/mncPy/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-1.1.3/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-1.1.3/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)    10216 2023-09-24 17:47:39.000000 baysalt_christmas-1.1.3/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3683 2023-09-24 17:48:11.000000 baysalt_christmas-1.1.3/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     2673 2024-01-05 03:20:35.000000 baysalt_christmas-1.1.3/christmas/server_info.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-01-05 03:42:13.517646 baysalt_christmas-1.1.3/christmas/tools/
--rw-r--r--   0 christmas   (501) staff       (20)      916 2023-09-24 17:50:48.000000 baysalt_christmas-1.1.3/christmas/tools/P_params.py
--rw-r--r--   0 christmas   (501) staff       (20)      264 2023-07-20 11:57:28.000000 baysalt_christmas-1.1.3/christmas/tools/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4052 2023-10-08 16:11:23.000000 baysalt_christmas-1.1.3/christmas/tools/download_check.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-1.1.3/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2024-01-05 03:42:13.518021 baysalt_christmas-1.1.3/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      794 2024-01-05 03:22:31.000000 baysalt_christmas-1.1.3/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:13:02.019477 baysalt_christmas-1.1.4/
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2024-04-16 09:59:40.000000 baysalt_christmas-1.1.4/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4183 2024-04-22 09:13:02.019240 baysalt_christmas-1.1.4/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-1.1.4/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:13:02.018895 baysalt_christmas-1.1.4/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4183 2024-04-22 09:13:01.000000 baysalt_christmas-1.1.4/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      848 2024-04-22 09:13:01.000000 baysalt_christmas-1.1.4/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2024-04-22 09:13:01.000000 baysalt_christmas-1.1.4/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2024-04-22 09:13:01.000000 baysalt_christmas-1.1.4/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2024-04-22 09:13:01.000000 baysalt_christmas-1.1.4/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:13:02.015534 baysalt_christmas-1.1.4/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    22673 2023-09-24 17:35:32.000000 baysalt_christmas-1.1.4/christmas/Blogging.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:13:02.015869 baysalt_christmas-1.1.4/christmas/Pyshell/
+-rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-1.1.4/christmas/Pyshell/RS_File.py
+-rw-r--r--   0 christmas   (501) staff       (20)      232 2023-09-18 07:37:39.000000 baysalt_christmas-1.1.4/christmas/Pyshell/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3787 2023-12-24 15:59:53.000000 baysalt_christmas-1.1.4/christmas/S_DateTime.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:13:02.016163 baysalt_christmas-1.1.4/christmas/SameAsMATLAB/
+-rw-r--r--   0 christmas   (501) staff       (20)     1270 2024-03-15 18:59:22.000000 baysalt_christmas-1.1.4/christmas/SameAsMATLAB/CoorTrans.py
+-rw-r--r--   0 christmas   (501) staff       (20)      236 2023-11-27 08:58:33.000000 baysalt_christmas-1.1.4/christmas/SameAsMATLAB/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:13:02.016453 baysalt_christmas-1.1.4/christmas/Standard/
+-rw-r--r--   0 christmas   (501) staff       (20)      234 2023-09-18 07:38:49.000000 baysalt_christmas-1.1.4/christmas/Standard/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     5903 2023-10-08 09:19:02.000000 baysalt_christmas-1.1.4/christmas/Standard/xr_attrs.py
+-rw-r--r--   0 christmas   (501) staff       (20)      479 2023-11-27 08:58:33.000000 baysalt_christmas-1.1.4/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     6288 2024-03-15 19:00:40.000000 baysalt_christmas-1.1.4/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1812 2023-09-24 17:45:18.000000 baysalt_christmas-1.1.4/christmas/cprintfs.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:13:02.018090 baysalt_christmas-1.1.4/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-1.1.4/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-1.1.4/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-1.1.4/christmas/mncPy/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-1.1.4/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-1.1.4/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)    10216 2023-09-24 17:47:39.000000 baysalt_christmas-1.1.4/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4861 2024-04-22 09:12:36.000000 baysalt_christmas-1.1.4/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     2651 2024-03-15 19:01:03.000000 baysalt_christmas-1.1.4/christmas/server_info.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:13:02.018703 baysalt_christmas-1.1.4/christmas/tools/
+-rw-r--r--   0 christmas   (501) staff       (20)      916 2023-09-24 17:50:48.000000 baysalt_christmas-1.1.4/christmas/tools/P_params.py
+-rw-r--r--   0 christmas   (501) staff       (20)      264 2023-07-20 11:57:28.000000 baysalt_christmas-1.1.4/christmas/tools/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4052 2023-10-08 16:11:23.000000 baysalt_christmas-1.1.4/christmas/tools/download_check.py
+-rw-r--r--   0 christmas   (501) staff       (20)      749 2024-03-21 07:10:04.000000 baysalt_christmas-1.1.4/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2024-04-22 09:13:02.019530 baysalt_christmas-1.1.4/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      794 2024-04-22 09:13:01.000000 baysalt_christmas-1.1.4/setup.py
```

### Comparing `baysalt_christmas-1.1.3/PKG-INFO` & `baysalt_christmas-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 1.1.3
+Version: 1.1.4
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: netCDF4
+Requires-Dist: xarray
+Requires-Dist: colorlog
 
 # This Package is a collection of Christmas related packages.
 ## Authors : Christmas
 ## Maintainer : Christmas
 
 To install this package, run:
```

### Comparing `baysalt_christmas-1.1.3/README.md` & `baysalt_christmas-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-1.1.4/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
-Name: baysalt-christmas
-Version: 1.1.3
+Name: baysalt_christmas
+Version: 1.1.4
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: netCDF4
+Requires-Dist: xarray
+Requires-Dist: colorlog
 
 # This Package is a collection of Christmas related packages.
 ## Authors : Christmas
 ## Maintainer : Christmas
 
 To install this package, run:
```

### Comparing `baysalt_christmas-1.1.3/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-1.1.4/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.DS_Store
 MANIFEST.in
 README.md
 run_twine.py
 setup.py
 baysalt_christmas.egg-info/PKG-INFO
 baysalt_christmas.egg-info/SOURCES.txt
 baysalt_christmas.egg-info/dependency_links.txt
@@ -23,12 +22,10 @@
 christmas/Standard/__init__.py
 christmas/Standard/xr_attrs.py
 christmas/mncPy/.gitignore
 christmas/mncPy/LICENSE
 christmas/mncPy/__init__.py
 christmas/mncPy/common.py
 christmas/mncPy/compress.py
-christmas/mncPy/__pycache__/__init__.cpython-310.pyc
-christmas/mncPy/__pycache__/__init__.cpython-311.pyc
 christmas/tools/P_params.py
 christmas/tools/__init__.py
 christmas/tools/download_check.py
```

### Comparing `baysalt_christmas-1.1.3/christmas/Blogging.py` & `baysalt_christmas-1.1.4/christmas/Blogging.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/christmas/Pyshell/RS_File.py` & `baysalt_christmas-1.1.4/christmas/Pyshell/RS_File.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/christmas/S_DateTime.py` & `baysalt_christmas-1.1.4/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/christmas/SameAsMATLAB/CoorTrans.py` & `baysalt_christmas-1.1.4/christmas/SameAsMATLAB/CoorTrans.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,22 @@
 
     \\>>>dms2degree(utf8(2°20'35.09"W))
     -2.34330555556F
 
     """
     
     dms_str = re.sub(r'\s', '', dms_str)
-    
+
     if re.search('[NSEWnsew]', dms_str) is None:
         sign = -1 if re.search('[swSW]', dms_str) else 1
     else:
         sign = 1
-    
+
     numbers = [*filter(len, re.split(r'\D+', dms_str, maxsplit=4))]
-    
+
     degree = numbers[0]
     minute = numbers[1] if len(numbers) >= 2 else '0'
     second = numbers[2] if len(numbers) >= 3 else '0'
     frac_seconds = numbers[3] if len(numbers) >= 4 else '0'
-    
-    second += "." + frac_seconds
+
+    second += f".{frac_seconds}"
     return sign * (int(degree) + float(minute) / 60 + float(second) / 3600)
```

### Comparing `baysalt_christmas-1.1.3/christmas/Standard/xr_attrs.py` & `baysalt_christmas-1.1.4/christmas/Standard/xr_attrs.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/christmas/commonCode.py` & `baysalt_christmas-1.1.4/christmas/commonCode.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,19 +112,20 @@
         os.makedirs(path)
 
 
 def makedirs(*path, exist_ok=False):
     """
     创建文件夹
     :param path: 文件夹路径
+    :param exist_ok: 是否忽略错误
     :return:
     """
     for p in path:
         if not os.path.exists(p):
-            os.makedirs(p,exist_ok=exist_ok)
+            os.makedirs(p, exist_ok=exist_ok)
 
 
 def rmfiles(*path):
     """
     删除文件
     :param path: 文件路径
     :return:
@@ -140,15 +141,15 @@
     :param path: 文件夹路径
     :param ignore_errors: 是否忽略错误
     :param onerror: 错误处理
     :return:
     """
     for p in path:
         if os.path.exists(p):
-            shutil.rmtree(p,ignore_errors=ignore_errors, onerror=onerror)
+            shutil.rmtree(p, ignore_errors=ignore_errors, onerror=onerror)
 
 
 def rmdirs(*path):
     """
     删除文件夹
     :param path: 文件夹路径
     :return:
```

### Comparing `baysalt_christmas-1.1.3/christmas/cprintfs.py` & `baysalt_christmas-1.1.4/christmas/cprintfs.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/christmas/mncPy/.gitignore` & `baysalt_christmas-1.1.4/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/christmas/mncPy/LICENSE` & `baysalt_christmas-1.1.4/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/christmas/mncPy/common.py` & `baysalt_christmas-1.1.4/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/christmas/mncPy/compress.py` & `baysalt_christmas-1.1.4/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/christmas/processBar.py` & `baysalt_christmas-1.1.4/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/christmas/server_info.py` & `baysalt_christmas-1.1.4/christmas/server_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,15 @@
 
 
 def get_server_ip_local():
     """
     获取服务器内网ip
     :return: 服务器内网ip
     """
-    host_ip = socket.gethostbyname(socket.gethostname())
-    return host_ip
+    return socket.gethostbyname(socket.gethostname())
 
 
 def get_server_ip_public():
     """
     获取服务器公网ip
     :return: 服务器公网ip
     """
```

### Comparing `baysalt_christmas-1.1.3/christmas/tools/P_params.py` & `baysalt_christmas-1.1.4/christmas/tools/P_params.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/christmas/tools/download_check.py` & `baysalt_christmas-1.1.4/christmas/tools/download_check.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.3/setup.py` & `baysalt_christmas-1.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="1.1.3",
+    version="1.1.4",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

