# Comparing `tmp/asgineer-0.8.1.tar.gz` & `tmp/asgineer-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgineer-0.8.1.tar", last modified: Wed Sep  8 13:36:21 2021, max compression
+gzip compressed data, was "asgineer-0.8.2.tar", last modified: Mon Apr 22 08:07:44 2024, max compression
```

## Comparing `asgineer-0.8.1.tar` & `asgineer-0.8.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2021-09-08 13:36:21.673752 asgineer-0.8.1/
--rw-rw-rw-   0        0        0      975 2021-09-08 13:36:21.673752 asgineer-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     2251 2021-09-08 13:33:47.000000 asgineer-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2021-09-08 13:36:21.642478 asgineer-0.8.1/asgineer/
--rw-rw-rw-   0        0        0      460 2021-09-08 13:35:42.000000 asgineer-0.8.1/asgineer/__init__.py
--rw-rw-rw-   0        0        0     9516 2021-09-08 13:33:47.000000 asgineer-0.8.1/asgineer/_app.py
--rw-rw-rw-   0        0        0      920 2021-09-08 13:33:47.000000 asgineer-0.8.1/asgineer/_compat.py
--rw-rw-rw-   0        0        0    16749 2021-09-08 13:33:47.000000 asgineer-0.8.1/asgineer/_request.py
--rw-rw-rw-   0        0        0     2969 2021-09-08 13:33:47.000000 asgineer-0.8.1/asgineer/_run.py
--rw-rw-rw-   0        0        0    20231 2021-09-08 13:33:47.000000 asgineer-0.8.1/asgineer/testutils.py
--rw-rw-rw-   0        0        0     5725 2021-09-08 13:33:47.000000 asgineer-0.8.1/asgineer/utils.py
-drwxrwxrwx   0        0        0        0 2021-09-08 13:36:21.673752 asgineer-0.8.1/asgineer.egg-info/
--rw-rw-rw-   0        0        0      975 2021-09-08 13:36:21.000000 asgineer-0.8.1/asgineer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2021-09-08 13:36:21.000000 asgineer-0.8.1/asgineer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-08 13:36:21.000000 asgineer-0.8.1/asgineer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-09-08 13:36:21.000000 asgineer-0.8.1/asgineer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2020-08-18 22:21:14.000000 asgineer-0.8.1/asgineer.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2021-09-08 13:36:21.673752 asgineer-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     2354 2021-09-08 13:34:10.000000 asgineer-0.8.1/setup.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-04-22 08:07:44.266609 asgineer-0.8.2/
+-rw-r--r--   0 almar      (501) staff       (20)     1321 2022-03-07 22:03:46.000000 asgineer-0.8.2/LICENSE
+-rw-r--r--   0 almar      (501) staff       (20)      789 2024-04-22 08:07:44.266487 asgineer-0.8.2/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     2251 2022-03-07 22:03:46.000000 asgineer-0.8.2/README.md
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-04-22 08:07:44.265372 asgineer-0.8.2/asgineer/
+-rw-r--r--   0 almar      (501) staff       (20)      460 2024-04-22 08:06:38.000000 asgineer-0.8.2/asgineer/__init__.py
+-rw-r--r--   0 almar      (501) staff       (20)    10163 2024-04-22 07:21:37.000000 asgineer-0.8.2/asgineer/_app.py
+-rw-r--r--   0 almar      (501) staff       (20)      920 2022-03-07 22:03:46.000000 asgineer-0.8.2/asgineer/_compat.py
+-rw-r--r--   0 almar      (501) staff       (20)    16745 2022-03-09 10:00:12.000000 asgineer-0.8.2/asgineer/_request.py
+-rw-r--r--   0 almar      (501) staff       (20)     2969 2022-03-07 22:03:46.000000 asgineer-0.8.2/asgineer/_run.py
+-rw-r--r--   0 almar      (501) staff       (20)    20231 2022-03-07 22:03:46.000000 asgineer-0.8.2/asgineer/testutils.py
+-rw-r--r--   0 almar      (501) staff       (20)     5971 2024-04-22 07:21:37.000000 asgineer-0.8.2/asgineer/utils.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2024-04-22 08:07:44.266308 asgineer-0.8.2/asgineer.egg-info/
+-rw-r--r--   0 almar      (501) staff       (20)      789 2024-04-22 08:07:44.000000 asgineer-0.8.2/asgineer.egg-info/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)      317 2024-04-22 08:07:44.000000 asgineer-0.8.2/asgineer.egg-info/SOURCES.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2024-04-22 08:07:44.000000 asgineer-0.8.2/asgineer.egg-info/dependency_links.txt
+-rw-r--r--   0 almar      (501) staff       (20)        9 2024-04-22 08:07:44.000000 asgineer-0.8.2/asgineer.egg-info/top_level.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2022-03-07 22:15:58.000000 asgineer-0.8.2/asgineer.egg-info/zip-safe
+-rw-r--r--   0 almar      (501) staff       (20)       38 2024-04-22 08:07:44.266647 asgineer-0.8.2/setup.cfg
+-rw-r--r--   0 almar      (501) staff       (20)     2205 2024-04-22 08:06:21.000000 asgineer-0.8.2/setup.py
```

### Comparing `asgineer-0.8.1/PKG-INFO` & `asgineer-0.8.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 1.2
-Name: asgineer
-Version: 0.8.1
-Summary: A really thin ASGI web framework
-Home-page: https://github.com/almarklein/asgineer
-Author: Almar Klein
-Author-email: almar.klein@gmail.com
-License: (new) BSD
-Download-URL: https://pypi.org/project/asgineer/
-Description: 
-        Asgineer - A really thin ASGI web framework
-        
-Keywords: ASGI web framework
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Provides: asgineer
-Requires-Python: >=3.6
+Metadata-Version: 2.1
+Name: asgineer
+Version: 0.8.2
+Summary: A really thin ASGI web framework
+Home-page: https://github.com/almarklein/asgineer
+Download-URL: https://pypi.org/project/asgineer/
+Author: Almar Klein
+Author-email: almar.klein@gmail.com
+License: (new) BSD
+Keywords: ASGI web framework
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Provides: asgineer
+Requires-Python: >=3.7
+License-File: LICENSE
+
+
+Asgineer - A really thin ASGI web framework
```

### Comparing `asgineer-0.8.1/README.md` & `asgineer-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `asgineer-0.8.1/asgineer/_app.py` & `asgineer-0.8.2/asgineer/_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,20 +136,33 @@
 
     try:
 
         # Call request handler to get the result
         where = "request handler"
         result = await handler(request)
 
+        def _response_has_body(
+            request, response_status, response_headers, response_body
+        ):
+            # https://www.rfc-editor.org/rfc/rfc7230#section-3.3
+            if request.method == "HEAD":
+                return False
+            if (100 <= response_status <= 199) or response_status in [204, 304]:
+                return False
+            return True
+
         if request._app_state == _request.CONNECTING:
             # Process the handler output
             where = "processing handler output"
             status, headers, body = normalize_response(result)
             # Make sure that there is a content type
-            if "content-type" not in headers:
+            if (
+                _response_has_body(request, status, headers, body)
+                and "content-type" not in headers
+            ):
                 headers["content-type"] = guess_content_type_from_body(body)
             # Convert the body
             if isinstance(body, bytes):
                 pass
             elif isinstance(body, str):
                 body = body.encode()
             elif isinstance(body, dict):
@@ -171,15 +184,19 @@
                     raise ValueError("Body cannot be a coroutine, forgot await?")
                 else:
                     raise ValueError(f"Body cannot be {type(body)}.")
             # Send response. Note that per the spec, if we do not specify
             # the content-length, the server sets Transfer-Encoding to chunked.
             if isinstance(body, bytes):
                 where = "sending response"
-                headers.setdefault("content-length", str(len(body)))
+                if (
+                    _response_has_body(request, status, headers, body)
+                    and "content-length" not in headers
+                ):
+                    headers["content-length"] = str(len(body))
                 await request.accept(status, headers)
                 await request.send(body, more=False)
             else:
                 where = "sending chunked response"
                 accepted = False
                 async for chunk in body:
                     if not isinstance(chunk, (bytes, str)):
```

### Comparing `asgineer-0.8.1/asgineer/_compat.py` & `asgineer-0.8.2/asgineer/_compat.py`

 * *Files identical despite different names*

### Comparing `asgineer-0.8.1/asgineer/_request.py` & `asgineer-0.8.2/asgineer/_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         # Iterate
         while True:
             chunk = await self._receive_chunk()
             yield chunk
             if self._client_state != CONNECTED:  # i.e. DONE or DISCONNECTED
                 break
 
-    async def get_body(self, limit=10 * 2 ** 20):
+    async def get_body(self, limit=10 * 2**20):
         """Async function to get the bytes of the body.
         If the end of the stream is not reached before the byte limit
         is reached (default 10MiB), raises an ``IOError``.
         """
         if self._body is None:
             nbytes = 0
             chunks = []
@@ -280,15 +280,15 @@
                 if nbytes > limit:
                     chunks.clear()
                     raise IOError("Request body too large.")
                 chunks.append(chunk)
             self._body = b"".join(chunks)
         return self._body
 
-    async def get_json(self, limit=10 * 2 ** 20):
+    async def get_json(self, limit=10 * 2**20):
         """Async function to get the body as a dict.
         If the end of the stream is not reached before the byte limit
         is reached (default 10MiB), raises an ``IOError``.
         """
         body = await self.get_body(limit)
         return json.loads(body.decode())
```

### Comparing `asgineer-0.8.1/asgineer/_run.py` & `asgineer-0.8.2/asgineer/_run.py`

 * *Files identical despite different names*

### Comparing `asgineer-0.8.1/asgineer/testutils.py` & `asgineer-0.8.2/asgineer/testutils.py`

 * *Files identical despite different names*

### Comparing `asgineer-0.8.1/asgineer/utils.py` & `asgineer-0.8.2/asgineer/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,79 +75,86 @@
     """
 
     if not isinstance(assets, dict):
         raise TypeError("make_asset_handler() expects a dict of assets")
     if not (isinstance(max_age, int) and max_age >= 0):  # pragma: no cover
         raise TypeError("make_asset_handler() max_age must be a positive int")
 
-    # Copy the dict, store hashes, prepare zipped data
-    assets = dict((key.lower(), val) for (key, val) in assets.items())
-    hashes = {}
+    # Store etags, prepare unzipped/zipped bodies, store ctypes
+    etags = {}
+    unzipped = {}
     zipped = {}
     ctypes = {}
-    for key, val in assets.items():
+    for path, body in assets.items():
+        # Get lowercase path
+        lpath = path.lower()
         # Get binary body
-        if isinstance(val, bytes):
-            bbody = val
-        elif isinstance(val, str):
-            bbody = val.encode()
+        if isinstance(body, bytes):
+            bbody = body
+        elif isinstance(body, str):
+            bbody = body.encode()
         else:
-            raise ValueError("Asset bodies must be str or bytes.")
-        # Store hash
-        hashes[key] = hashlib.sha256(bbody).hexdigest()
-        # Store zipped version if it makes sense
+            raise ValueError("Asset bodies must be bytes or str.")
+        # Store etag
+        etags[lpath] = hashlib.sha256(bbody).hexdigest()
+        # Store unzipped body
+        unzipped[lpath] = bbody
+        # Store zipped body if it makes sense
         if len(bbody) >= min_compress_size:
-            if not key.endswith(VIDEO_EXTENSIONS):
+            if not lpath.endswith(VIDEO_EXTENSIONS):
                 bbody_zipped = gzip.compress(bbody)
                 if len(bbody_zipped) < 0.90 * len(bbody):
-                    zipped[key] = bbody_zipped
-        # Store mimetype
-        ctype, enc = mimetypes.guess_type(key)
+                    zipped[lpath] = bbody_zipped
+        # Store ctype
+        ctype, _ = mimetypes.guess_type(lpath)
         if ctype:
-            ctypes[key] = ctype
+            ctypes[lpath] = ctype
         else:
-            ctypes[key] = guess_content_type_from_body(val)
+            ctypes[lpath] = guess_content_type_from_body(body)
 
     async def asset_handler(request, path=None):
         if request.method not in ("GET", "HEAD"):
             return 405, {}, "Method not allowed"
+
         if path is None:
             path = request.path.lstrip("/")
         path = path.lower()
 
-        # Exit early on 404
-        if path not in assets:
-            return 404, {}, "404 not found"
-
-        content_etag = hashes.get(path, None)
-        request_etag = request.headers.get("if-none-match", None)
-        headers = {
-            "etag": content_etag,
-            "cache-control": f"public, must-revalidate, max-age={max_age:d}",
-        }
+        if path not in unzipped:
+            return 404, {}, "File not found"
 
-        # If client already has the exact asset, send confirmation now
-        if request_etag and request_etag == content_etag:
-            return 304, headers, b""
+        assert path in etags
+        assert path in ctypes
 
-        # Set content type
-        if path in ctypes:
-            headers["content-type"] = ctypes[path]
+        status = 200
+        body = unzipped[path]
+        headers = {}
+        headers["cache-control"] = f"public, must-revalidate, max-age={max_age:d}"
+        headers["content-length"] = str(len(body))
+        headers["content-type"] = ctypes[path]
+        headers["etag"] = f'"{etags[path]}"'
 
         # Get body, zip if we should and can
-        if path in zipped and "gzip" in request.headers.get("accept-encoding", ""):
-            headers["content-encoding"] = "gzip"
+        if "gzip" in request.headers.get("accept-encoding", "") and path in zipped:
             body = zipped[path]
-        else:
-            body = assets[path]
+            headers["content-encoding"] = "gzip"
+            headers["content-length"] = str(len(body))
+
+        # If client already has the exact asset, send confirmation now
+        if request.headers.get("if-none-match") == headers["etag"]:
+            status = 304
+            body = b""
+            # https://www.rfc-editor.org/rfc/rfc7232#section-4.1
+            headers.pop("content-encoding", None)
+            headers.pop("content-length", None)
+            headers.pop("content-type", None)
 
         # The response to a head request should not include a body
         if request.method == "HEAD":
-            headers["content-length"] = str(len(body))
             body = b""
 
         # Note that we always return bytes, not a stream-response. The
         # assets used with this utility are assumed to be small-ish,
         # since they are in-memory.
-        return 200, headers, body
+        return status, headers, body
 
     return asset_handler
```

### Comparing `asgineer-0.8.1/asgineer.egg-info/PKG-INFO` & `asgineer-0.8.2/asgineer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 1.2
-Name: asgineer
-Version: 0.8.1
-Summary: A really thin ASGI web framework
-Home-page: https://github.com/almarklein/asgineer
-Author: Almar Klein
-Author-email: almar.klein@gmail.com
-License: (new) BSD
-Download-URL: https://pypi.org/project/asgineer/
-Description: 
-        Asgineer - A really thin ASGI web framework
-        
-Keywords: ASGI web framework
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Provides: asgineer
-Requires-Python: >=3.6
+Metadata-Version: 2.1
+Name: asgineer
+Version: 0.8.2
+Summary: A really thin ASGI web framework
+Home-page: https://github.com/almarklein/asgineer
+Download-URL: https://pypi.org/project/asgineer/
+Author: Almar Klein
+Author-email: almar.klein@gmail.com
+License: (new) BSD
+Keywords: ASGI web framework
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Provides: asgineer
+Requires-Python: >=3.7
+License-File: LICENSE
+
+
+Asgineer - A really thin ASGI web framework
```

### Comparing `asgineer-0.8.1/setup.py` & `asgineer-0.8.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,26 +59,23 @@
     url="https://github.com/almarklein/asgineer",
     download_url="https://pypi.org/project/asgineer/",
     keywords="ASGI web framework",
     description=description,
     long_description=doc,
     platforms="any",
     provides=[name],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=[],
     packages=["asgineer"],
     # entry_points={'console_scripts': ['asgi = asgi:cli'], },
     zip_safe=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP",
         "License :: OSI Approved :: BSD License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3",
     ],
 )
```

