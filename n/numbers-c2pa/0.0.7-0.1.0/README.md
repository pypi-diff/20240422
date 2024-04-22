# Comparing `tmp/numbers-c2pa-0.0.7.tar.gz` & `tmp/numbers_c2pa-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/numbers-c2pa/numbers-c2pa/dist/.tmp-l6vx6c5z/numbers-c2pa-0.0.7.tar", last modified: Tue May 16 08:05:50 2023, max compression
+gzip compressed data, was "numbers_c2pa-0.1.0.tar", last modified: Mon Apr 22 09:09:13 2024, max compression
```

## Comparing `numbers-c2pa-0.0.7.tar` & `numbers_c2pa-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/src/numbers_c2pa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/src/numbers_c2pa/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/src/numbers_c2pa/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/src/numbers_c2pa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:05:49.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:09:13.601177 numbers_c2pa-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-22 09:09:07.000000 numbers_c2pa-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-22 09:09:13.601177 numbers_c2pa-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-22 09:09:07.000000 numbers_c2pa-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 09:09:07.000000 numbers_c2pa-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-22 09:09:13.601177 numbers_c2pa-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 09:09:07.000000 numbers_c2pa-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:09:13.597177 numbers_c2pa-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:09:13.597177 numbers_c2pa-0.1.0/src/numbers_c2pa/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-22 09:09:07.000000 numbers_c2pa-0.1.0/src/numbers_c2pa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-04-22 09:09:07.000000 numbers_c2pa-0.1.0/src/numbers_c2pa/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 09:09:07.000000 numbers_c2pa-0.1.0/src/numbers_c2pa/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-22 09:09:07.000000 numbers_c2pa-0.1.0/src/numbers_c2pa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:09:13.601177 numbers_c2pa-0.1.0/src/numbers_c2pa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-22 09:09:13.000000 numbers_c2pa-0.1.0/src/numbers_c2pa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-22 09:09:13.000000 numbers_c2pa-0.1.0/src/numbers_c2pa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:09:13.000000 numbers_c2pa-0.1.0/src/numbers_c2pa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 09:09:13.000000 numbers_c2pa-0.1.0/src/numbers_c2pa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 09:09:13.000000 numbers_c2pa-0.1.0/src/numbers_c2pa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:09:13.000000 numbers_c2pa-0.1.0/src/numbers_c2pa.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:09:13.601177 numbers_c2pa-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-22 09:09:07.000000 numbers_c2pa-0.1.0/tests/test_core.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `numbers-c2pa-0.0.7/LICENSE` & `numbers_c2pa-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.7/PKG-INFO` & `numbers_c2pa-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: numbers-c2pa
-Version: 0.0.7
+Version: 0.1.0
 Summary: Numbers C2PA tool
 Home-page: https://github.com/numbersprotocol/numbers-c2pa
 Author: Numbers Co., Inc
 Author-email: dev@numbersprotocol.io
 Keywords: authenticity
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cryptography
+Requires-Dist: requests
 Provides-Extra: tests
+Requires-Dist: tox; extra == "tests"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx; extra == "docs"
 
 # numbers-c2pa
 
 
 ## Setup
 
 Install Rust
```

### Comparing `numbers-c2pa-0.0.7/README.md` & `numbers_c2pa-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.7/setup.cfg` & `numbers_c2pa-0.1.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [metadata]
 name = numbers-c2pa
-version = 0.0.7
+version = 0.1.0
 author = Numbers Co., Inc
 author_email = dev@numbersprotocol.io
 description = Numbers C2PA tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = authenticity
 url = https://github.com/numbersprotocol/numbers-c2pa
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 package_dir = 
 	=src
 zip_safe = True
-python_requires = >=3.6
+python_requires = >=3.7
 packages = find:
 install_requires = 
 	cryptography
+	requests
 
 [options.packages.find]
 where = src
 exclude = docs tests
 
 [options.extras_require]
 tests = 
@@ -53,23 +53,24 @@
 	line-too-long,
 	missing-module-docstring,
 	missing-class-docstring,
 	missing-function-docstring,
 	too-few-public-methods,
 	too-many-public-methods,
 	too-many-arguments,
+	unspecified-encoding,
 
 [flake8]
 max-line-length = 120
 max-complexity = 10
 exclude = .git,__pycache__,__init__.py,.mypy_cache,.pytest_cache,venv,.venv
 
 [tox:tox]
-envlist = 
-	py36, py37, py38, py39, py310, flake8, pylint, bandit
+env_list = 
+	py38, py39, py310, flake8, pylint, bandit, test, report
 
 [testenv]
 deps = 
 	coverage
 	pytest
 	pytest-mock
 	pytest-httpx
```

### Comparing `numbers-c2pa-0.0.7/src/numbers_c2pa/__init__.py` & `numbers_c2pa-0.1.0/src/numbers_c2pa/__init__.py`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.7/src/numbers_c2pa/core.py` & `numbers_c2pa-0.1.0/src/numbers_c2pa/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 import mimetypes
 import os
-import subprocess
+import subprocess  # nosec
 from datetime import datetime
-from tempfile import NamedTemporaryFile, TemporaryDirectory
+from tempfile import TemporaryDirectory
 from typing import Any, Dict, List, Optional
 
+import requests
+
 from .exceptions import NoClaimFound, UnknownError
 
 
 def _mimetype_to_ext(asset_mime_type: str):
     ext = mimetypes.guess_extension(asset_mime_type)
     if not ext:
         raise ValueError(f'Could not find a file extension for MIME type: {asset_mime_type}')
@@ -25,40 +27,43 @@
     sign_cert: Optional[str] = None,
 ):
     env_vars = os.environ.copy()
     if private_key:
         env_vars['C2PA_PRIVATE_KEY'] = private_key
     if sign_cert:
         env_vars['C2PA_SIGN_CERT'] = sign_cert
-    command = f'c2patool "{file_path}" -m "{manifest_path}" -o "{output_path}"'
+    command = f"c2patool '{file_path}' -m '{manifest_path}' -o '{output_path}'"
+
     if force_overwrite:
         command += ' -f'
     try:
         subprocess.run(
             command,
             shell=True,
             env=env_vars,
             check=True,
             stderr=subprocess.PIPE,
-        )
+        )  # nosec
     except subprocess.CalledProcessError as e:
-        raise UnknownError(e.stderr)
+        raise UnknownError(e.stderr) from e
 
 
 def create_c2pa_manifest(
     nid: str,
     creator_public_key: str,
     asset_hash: str,
     date_created: datetime,
     location_created: str,
     date_captured: Optional[datetime],
     alg: str = 'es256',
     ta_url: str = 'http://timestamp.digicert.com',
     vendor: str = 'numbersprotocol',
     claim_generator: str = 'Numbers_Protocol',
+    digital_source_type: Optional[str] = None,
+    generated_by: Optional[str] = None,
 ):
     captureTimestamp = date_captured.timestamp() if date_captured else None
     manifest = {
         'alg': alg,
         'ta_url': ta_url,
         'vendor': vendor,
         'claim_generator': claim_generator,
@@ -77,24 +82,42 @@
                     ],
                     'dateCreated': date_created.strftime('%Y-%m-%dT%H:%M:%SZ'),
                     'locationCreated': location_created,
                     'identifier': nid,
                 }
             },
             {
+                'label': 'c2pa.actions',
+                'data': {
+                    'actions': [
+                        {
+                            'action': 'c2pa.opened',
+                        }
+                    ],
+                }
+            },
+            {
                 'label': 'numbers.integrity.json',
                 'data': {
                     'nid': nid,
                     'publicKey': creator_public_key,
                     'mediaHash': asset_hash,
                     'captureTimestamp': captureTimestamp,
                 }
             }
         ]
     }
+    if digital_source_type:
+        manifest['assertions'][1]['data']['actions'][0].update({
+            'digitalSourceType': f'http://cv.iptc.org/newscodes/digitalsourcetype/{digital_source_type}',
+        })
+    if generated_by:
+        manifest['assertions'][1]['data']['actions'][0].update({
+            'softwareAgent': f'{generated_by}'
+        })
     return manifest
 
 
 def create_custom_c2pa_manifest(
     alg: str = 'es256',
     ta_url: str = 'http://timestamp.digicert.com',
     vendor: str = 'numbersprotocol',
@@ -185,24 +208,41 @@
 def inject_file(
     asset_file: str,
     c2pa_output_file: str,
     manifest: Dict[str, Any],
     private_key: Optional[str] = None,
     sign_cert: Optional[str] = None,
     force_overwrite: bool = True,
+    thumbnail_url: Optional[str] = None,
 ):
     """Perform C2PA injection given an existing asset file.
     """
-    with NamedTemporaryFile(prefix='manifest_', mode='w') as manifest_temp_file:
-        json.dump(manifest, manifest_temp_file)
-        manifest_temp_file.flush()
+    with TemporaryDirectory() as temp_dir:
+        if thumbnail_url:
+            thumbnail_file_path = os.path.join(temp_dir, 'thumbnail.jpg')
+            response = requests.get(thumbnail_url, stream=True, timeout=120)
+            response.raise_for_status()
+            with open(thumbnail_file_path, 'wb') as thumbnail_file:
+                for chunk in response.iter_content(chunk_size=8192):
+                    thumbnail_file.write(chunk)
+                thumbnail_file.flush()
+            manifest['thumbnail'] = {
+                'format': 'image/jpeg',
+                'identifier': thumbnail_file_path,
+            }
+
+        # Save the manifest to a temporary file
+        manifest_file_path = os.path.join(temp_dir, 'manifest.json')
+        with open(manifest_file_path, 'w',) as manifest_file:
+            json.dump(manifest, manifest_file)
+            manifest_file.flush()
 
         c2patool_inject(
             asset_file,
-            manifest_temp_file.name,
+            manifest_file.name,
             c2pa_output_file,
             force_overwrite=force_overwrite,
             private_key=private_key,
             sign_cert=sign_cert,
         )
 
 
@@ -210,29 +250,29 @@
     file_ext = _mimetype_to_ext(asset_mime_type)
     with TemporaryDirectory(prefix='temp_dir') as temp_dir:
         asset_c2pa_file = os.path.join(temp_dir, f'asset-c2pa.{file_ext}')
         with open(asset_c2pa_file, 'wb') as f:
             f.write(asset_c2pa_bytes)
 
         command = ['c2patool', asset_c2pa_file]
-        process = subprocess.run(command, text=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=False)
+        process = subprocess.run(
+            command, text=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=False
+        )  # nosec
         if process.returncode != 0:
             if 'No claim found' in process.stderr:
                 raise NoClaimFound
-            else:
-                raise UnknownError(process.stderr)
+            raise UnknownError(process.stderr)
 
         json_output = json.loads(process.stdout)
         return json_output
 
 
 def read_c2pa_file(c2pa_file: str):
     command = ['c2patool', c2pa_file]
-    process = subprocess.run(command, text=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=False)
+    process = subprocess.run(command, text=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=False)  # nosec
     if process.returncode != 0:
         if 'No claim found' in process.stderr:
             raise NoClaimFound
-        else:
-            raise UnknownError(process.stderr)
+        raise UnknownError(process.stderr)
 
     json_output = json.loads(process.stdout)
     return json_output
```

### Comparing `numbers-c2pa-0.0.7/src/numbers_c2pa/utils.py` & `numbers_c2pa-0.1.0/src/numbers_c2pa/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         .subject_name(subject)
         .issuer_name(subject)
         .public_key(private_key.public_key())
         .serial_number(x509.random_serial_number())
         .not_valid_before(datetime.datetime.utcnow())
         .not_valid_after(datetime.datetime.utcnow() + datetime.timedelta(days=365))
         .add_extension(
-            x509.SubjectAlternativeName([x509.DNSName(u"my-organization.com")]),
+            x509.SubjectAlternativeName([x509.DNSName('my-organization.com')]),
             critical=False,
         )
         .add_extension(
             x509.BasicConstraints(ca=False, path_length=None), critical=True,
         )
         .sign(private_key, hashes.SHA256())
     )
```

### Comparing `numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/PKG-INFO` & `numbers_c2pa-0.1.0/src/numbers_c2pa.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: numbers-c2pa
-Version: 0.0.7
+Version: 0.1.0
 Summary: Numbers C2PA tool
 Home-page: https://github.com/numbersprotocol/numbers-c2pa
 Author: Numbers Co., Inc
 Author-email: dev@numbersprotocol.io
 Keywords: authenticity
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cryptography
+Requires-Dist: requests
 Provides-Extra: tests
+Requires-Dist: tox; extra == "tests"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx; extra == "docs"
 
 # numbers-c2pa
 
 
 ## Setup
 
 Install Rust
```

