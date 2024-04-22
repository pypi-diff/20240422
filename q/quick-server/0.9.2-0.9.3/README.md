# Comparing `tmp/quick_server-0.9.2.tar.gz` & `tmp/quick_server-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_server-0.9.2.tar", last modified: Wed Mar 27 23:48:06 2024, max compression
+gzip compressed data, was "quick_server-0.9.3.tar", last modified: Mon Apr 22 01:55:30 2024, max compression
```

## Comparing `quick_server-0.9.2.tar` & `quick_server-0.9.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 23:48:06.786306 quick_server-0.9.2/
--rw-r--r--   0 krause     (501) staff       (20)    11357 2024-03-08 04:22:16.000000 quick_server-0.9.2/LICENSE
--rw-r--r--   0 krause     (501) staff       (20)      183 2023-08-16 14:09:57.000000 quick_server-0.9.2/MANIFEST.in
--rw-r--r--   0 krause     (501) staff       (20)    27554 2024-03-27 23:48:06.786080 quick_server-0.9.2/PKG-INFO
--rw-r--r--   0 krause     (501) staff       (20)    13896 2023-08-16 14:12:32.000000 quick_server-0.9.2/README.rst
--rw-r--r--   0 krause     (501) staff       (20)     3878 2024-03-27 23:47:52.000000 quick_server-0.9.2/pyproject.toml
--rw-r--r--   0 krause     (501) staff       (20)       38 2024-03-27 23:48:06.786347 quick_server-0.9.2/setup.cfg
--rw-r--r--   0 krause     (501) staff       (20)     1788 2024-03-08 04:22:16.000000 quick_server-0.9.2/setup.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 23:48:06.779173 quick_server-0.9.2/src/
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 23:48:06.784944 quick_server-0.9.2/src/quick_server/
--rw-r--r--   0 krause     (501) staff       (20)     3520 2024-03-08 04:22:16.000000 quick_server-0.9.2/src/quick_server/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     2006 2024-03-08 04:22:16.000000 quick_server-0.9.2/src/quick_server/__main__.py
--rw-r--r--   0 krause     (501) staff       (20)       78 2023-08-16 14:09:57.000000 quick_server-0.9.2/src/quick_server/favicon.ico
--rw-r--r--   0 krause     (501) staff       (20)        0 2023-08-16 14:09:57.000000 quick_server-0.9.2/src/quick_server/py.typed
--rw-r--r--   0 krause     (501) staff       (20)   148798 2024-03-27 23:47:52.000000 quick_server-0.9.2/src/quick_server/quick_server.py
--rw-r--r--   0 krause     (501) staff       (20)     9306 2024-03-08 04:22:16.000000 quick_server-0.9.2/src/quick_server/worker.js
--rw-r--r--   0 krause     (501) staff       (20)     9398 2024-03-08 04:22:16.000000 quick_server-0.9.2/src/quick_server/worker.legacy.js
--rw-r--r--   0 krause     (501) staff       (20)     3846 2024-03-08 04:22:16.000000 quick_server-0.9.2/src/quick_server/worker_request.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 23:48:06.785814 quick_server-0.9.2/src/quick_server.egg-info/
--rw-r--r--   0 krause     (501) staff       (20)    27554 2024-03-27 23:48:06.000000 quick_server-0.9.2/src/quick_server.egg-info/PKG-INFO
--rw-r--r--   0 krause     (501) staff       (20)      456 2024-03-27 23:48:06.000000 quick_server-0.9.2/src/quick_server.egg-info/SOURCES.txt
--rw-r--r--   0 krause     (501) staff       (20)        1 2024-03-27 23:48:06.000000 quick_server-0.9.2/src/quick_server.egg-info/dependency_links.txt
--rw-r--r--   0 krause     (501) staff       (20)       13 2024-03-27 23:48:06.000000 quick_server-0.9.2/src/quick_server.egg-info/top_level.txt
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 01:55:30.759650 quick_server-0.9.3/
+-rw-r--r--   0 krause     (501) staff       (20)    11357 2024-03-08 04:22:16.000000 quick_server-0.9.3/LICENSE
+-rw-r--r--   0 krause     (501) staff       (20)      183 2023-08-16 14:09:57.000000 quick_server-0.9.3/MANIFEST.in
+-rw-r--r--   0 krause     (501) staff       (20)    27554 2024-04-22 01:55:30.759421 quick_server-0.9.3/PKG-INFO
+-rw-r--r--   0 krause     (501) staff       (20)    13896 2023-08-16 14:12:32.000000 quick_server-0.9.3/README.rst
+-rw-r--r--   0 krause     (501) staff       (20)     3878 2024-04-22 01:53:35.000000 quick_server-0.9.3/pyproject.toml
+-rw-r--r--   0 krause     (501) staff       (20)       38 2024-04-22 01:55:30.759687 quick_server-0.9.3/setup.cfg
+-rw-r--r--   0 krause     (501) staff       (20)     1788 2024-03-08 04:22:16.000000 quick_server-0.9.3/setup.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 01:55:30.755005 quick_server-0.9.3/src/
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 01:55:30.758430 quick_server-0.9.3/src/quick_server/
+-rw-r--r--   0 krause     (501) staff       (20)     3520 2024-03-08 04:22:16.000000 quick_server-0.9.3/src/quick_server/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     2006 2024-03-08 04:22:16.000000 quick_server-0.9.3/src/quick_server/__main__.py
+-rw-r--r--   0 krause     (501) staff       (20)       78 2023-08-16 14:09:57.000000 quick_server-0.9.3/src/quick_server/favicon.ico
+-rw-r--r--   0 krause     (501) staff       (20)        0 2023-08-16 14:09:57.000000 quick_server-0.9.3/src/quick_server/py.typed
+-rw-r--r--   0 krause     (501) staff       (20)   149248 2024-04-22 01:53:35.000000 quick_server-0.9.3/src/quick_server/quick_server.py
+-rw-r--r--   0 krause     (501) staff       (20)     9306 2024-03-08 04:22:16.000000 quick_server-0.9.3/src/quick_server/worker.js
+-rw-r--r--   0 krause     (501) staff       (20)     9398 2024-03-08 04:22:16.000000 quick_server-0.9.3/src/quick_server/worker.legacy.js
+-rw-r--r--   0 krause     (501) staff       (20)     3846 2024-03-08 04:22:16.000000 quick_server-0.9.3/src/quick_server/worker_request.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 01:55:30.759175 quick_server-0.9.3/src/quick_server.egg-info/
+-rw-r--r--   0 krause     (501) staff       (20)    27554 2024-04-22 01:55:30.000000 quick_server-0.9.3/src/quick_server.egg-info/PKG-INFO
+-rw-r--r--   0 krause     (501) staff       (20)      456 2024-04-22 01:55:30.000000 quick_server-0.9.3/src/quick_server.egg-info/SOURCES.txt
+-rw-r--r--   0 krause     (501) staff       (20)        1 2024-04-22 01:55:30.000000 quick_server-0.9.3/src/quick_server.egg-info/dependency_links.txt
+-rw-r--r--   0 krause     (501) staff       (20)       13 2024-04-22 01:55:30.000000 quick_server-0.9.3/src/quick_server.egg-info/top_level.txt
```

### Comparing `quick_server-0.9.2/LICENSE` & `quick_server-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.2/PKG-INFO` & `quick_server-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick_server
-Version: 0.9.2
+Version: 0.9.3
 Summary: QuickServer is a quick to use and easy to set up server implementation.
 Author-email: Josua Krause <josua.krause@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `quick_server-0.9.2/README.rst` & `quick_server-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.2/pyproject.toml` & `quick_server-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
     name = "quick_server"
     description = "QuickServer is a quick to use and easy to set up server implementation."
     readme = "README.rst"
-    version = "0.9.2"
+    version = "0.9.3"
     authors = [
         {name = "Josua Krause", email = "josua.krause@gmail.com"},
     ]
     keywords = [
         "server",
         "REST",
         "file",
```

### Comparing `quick_server-0.9.2/setup.py` & `quick_server-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.2/src/quick_server/__init__.py` & `quick_server-0.9.3/src/quick_server/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.2/src/quick_server/__main__.py` & `quick_server-0.9.3/src/quick_server/__main__.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.2/src/quick_server/quick_server.py` & `quick_server-0.9.3/src/quick_server/quick_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
         return res
     res = getattr(fun, "__name__", None)
     if res is not None:
         return res
     return f"{res}"
 
 
-__version__ = version(__package__)
+__version__ = version(cast(str, __package__))
 
 
 def _getheader_fallback(obj: Any, key: str) -> Any:
     return obj.get(key)
 
 
 def _getheader_p2(obj: Any, key: str) -> Any:
@@ -1167,30 +1167,40 @@
                     mpath = os.path.join(mpath, word)
                 # make path absolute and check if it exists
                 mpath = os.path.abspath(mpath)
                 if os.path.exists(mpath):
                     break
             # if pass is still None here the file cannot be found
             if mpath is None:
+
+                def forward(url_path: str, *, remove_last: bool) -> None:
+                    for (name, pxy) in self.server._folder_proxys:
+                        if not url_path.startswith(name):
+                            continue
+                        start_adj = 0 if remove_last else 1
+                        remain = url_path[len(name) - start_adj:]
+                        proxy = urlparse.urlparse(pxy)
+                        reala = urlparse.urlparse(init_path)
+                        pxya = urlparse.urlunparse((
+                            proxy[0],  # scheme
+                            proxy[1],  # netloc
+                            f"{proxy[2]}{remain}",  # path
+                            reala[3],  # params
+                            reala[4],  # query
+                            reala[5],  # fragment
+                        ))
+                        self.send_to_proxy(pxya)
+
                 # try proxies
-                for (name, pxy) in self.server._folder_proxys:
-                    if not orig_path.startswith(name):
-                        continue
-                    remain = orig_path[len(name) - 1:]
-                    proxy = urlparse.urlparse(pxy)
-                    reala = urlparse.urlparse(init_path)
-                    pxya = urlparse.urlunparse((
-                        proxy[0],  # scheme
-                        proxy[1],  # netloc
-                        f"{proxy[2]}{remain}",  # path
-                        reala[3],  # params
-                        reala[4],  # query
-                        reala[5],  # fragment
-                    ))
-                    self.send_to_proxy(pxya)  # raises PreventDefaultResponse
+                # raises PreventDefaultResponse if successful
+                forward(orig_path, remove_last=False)
+                if len(orig_path) and orig_path[-1] != "/":
+                    forward(f"{orig_path}/", remove_last=True)
+
+                # out of luck
                 if orig_path not in self.common_invalid_paths:
                     msg(f"no matching folder alias: {orig_path}")
                 raise PreventDefaultResponse(404, "File not found")
             path: str = mpath
             if os.path.isdir(path):
                 if not is_folder:
                     needs_redirect = True
```

### Comparing `quick_server-0.9.2/src/quick_server/worker.js` & `quick_server-0.9.3/src/quick_server/worker.js`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.2/src/quick_server/worker.legacy.js` & `quick_server-0.9.3/src/quick_server/worker.legacy.js`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.2/src/quick_server/worker_request.py` & `quick_server-0.9.3/src/quick_server/worker_request.py`

 * *Files identical despite different names*

### Comparing `quick_server-0.9.2/src/quick_server.egg-info/PKG-INFO` & `quick_server-0.9.3/src/quick_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick_server
-Version: 0.9.2
+Version: 0.9.3
 Summary: QuickServer is a quick to use and easy to set up server implementation.
 Author-email: Josua Krause <josua.krause@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

