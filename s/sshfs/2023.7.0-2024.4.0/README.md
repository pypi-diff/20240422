# Comparing `tmp/sshfs-2023.7.0.tar.gz` & `tmp/sshfs-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshfs-2023.7.0.tar", last modified: Fri Jul 14 22:12:56 2023, max compression
+gzip compressed data, was "sshfs-2024.4.0.tar", last modified: Sun Apr 21 22:31:30 2024, max compression
```

## Comparing `sshfs-2023.7.0.tar` & `sshfs-2024.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.590614 sshfs-2023.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.582614 sshfs-2023.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.586614 sshfs-2023.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 22:12:45.000000 sshfs-2023.7.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-14 22:12:45.000000 sshfs-2023.7.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-14 22:12:45.000000 sshfs-2023.7.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-14 22:12:45.000000 sshfs-2023.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-14 22:12:45.000000 sshfs-2023.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-14 22:12:45.000000 sshfs-2023.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-14 22:12:56.590614 sshfs-2023.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-14 22:12:45.000000 sshfs-2023.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-14 22:12:45.000000 sshfs-2023.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 22:12:45.000000 sshfs-2023.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-14 22:12:56.590614 sshfs-2023.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 22:12:45.000000 sshfs-2023.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.586614 sshfs-2023.7.0/sshfs/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.586614 sshfs-2023.7.0/sshfs/pools/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/pools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/pools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/pools/hard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/pools/soft.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.586614 sshfs-2023.7.0/sshfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.590614 sshfs-2023.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.590614 sshfs-2023.7.0/tests/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-14 22:12:45.000000 sshfs-2023.7.0/tests/static/user.key
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-14 22:12:45.000000 sshfs-2023.7.0/tests/static/user.key.pub
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-14 22:12:45.000000 sshfs-2023.7.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-14 22:12:45.000000 sshfs-2023.7.0/tests/test_sftp_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-07-14 22:12:45.000000 sshfs-2023.7.0/tests/test_sshfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:31:30.874693 sshfs-2024.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:31:30.866693 sshfs-2024.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:31:30.866693 sshfs-2024.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-21 22:31:26.000000 sshfs-2024.4.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-21 22:31:26.000000 sshfs-2024.4.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-21 22:31:26.000000 sshfs-2024.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-21 22:31:26.000000 sshfs-2024.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-21 22:31:26.000000 sshfs-2024.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-04-21 22:31:26.000000 sshfs-2024.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-21 22:31:30.874693 sshfs-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-21 22:31:26.000000 sshfs-2024.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-21 22:31:26.000000 sshfs-2024.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-21 22:31:26.000000 sshfs-2024.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-21 22:31:30.874693 sshfs-2024.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:31:26.000000 sshfs-2024.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:31:30.870693 sshfs-2024.4.0/sshfs/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-21 22:31:26.000000 sshfs-2024.4.0/sshfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-21 22:31:26.000000 sshfs-2024.4.0/sshfs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-21 22:31:26.000000 sshfs-2024.4.0/sshfs/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:31:30.870693 sshfs-2024.4.0/sshfs/pools/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-21 22:31:26.000000 sshfs-2024.4.0/sshfs/pools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-21 22:31:26.000000 sshfs-2024.4.0/sshfs/pools/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-21 22:31:26.000000 sshfs-2024.4.0/sshfs/pools/hard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-21 22:31:26.000000 sshfs-2024.4.0/sshfs/pools/soft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-04-21 22:31:26.000000 sshfs-2024.4.0/sshfs/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-21 22:31:26.000000 sshfs-2024.4.0/sshfs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:31:30.870693 sshfs-2024.4.0/sshfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-21 22:31:30.000000 sshfs-2024.4.0/sshfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-21 22:31:30.000000 sshfs-2024.4.0/sshfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:31:30.000000 sshfs-2024.4.0/sshfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-21 22:31:30.000000 sshfs-2024.4.0/sshfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-21 22:31:30.000000 sshfs-2024.4.0/sshfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 22:31:30.000000 sshfs-2024.4.0/sshfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:31:30.870693 sshfs-2024.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:31:30.870693 sshfs-2024.4.0/tests/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-21 22:31:26.000000 sshfs-2024.4.0/tests/static/user.key
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-21 22:31:26.000000 sshfs-2024.4.0/tests/static/user.key.pub
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-21 22:31:26.000000 sshfs-2024.4.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-21 22:31:26.000000 sshfs-2024.4.0/tests/test_sftp_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-21 22:31:26.000000 sshfs-2024.4.0/tests/test_sshfs.py
```

### Comparing `sshfs-2023.7.0/.github/workflows/publish.yml` & `sshfs-2024.4.0/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jobs:
   pulish:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@master
 
-    - uses: actions/setup-python@v1
+    - uses: actions/setup-python@v4
       with:
         python-version: '3.8'
 
     - name: Install pypa/build
       run: python -m pip install build
 
     - name: Build the package
```

### Comparing `sshfs-2023.7.0/.github/workflows/test.yml` & `sshfs-2024.4.0/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,17 +18,17 @@
       fail-fast: true
 
       matrix:
         os: [ubuntu-latest, macos-latest]
         pyv: ["3.7", "3.8", "3.9", "3.10", "3.11.0-rc - 3.11"]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
 
-    - uses: actions/setup-python@v2
+    - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.pyv }}
 
     - name: Install dependencies
       run: |
         python -m pip install -r requirements-dev.txt
         python -m pip install -e .
```

### Comparing `sshfs-2023.7.0/.gitignore` & `sshfs-2024.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/.pre-commit-config.yaml` & `sshfs-2024.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/LICENSE` & `sshfs-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/PKG-INFO` & `sshfs-2024.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: sshfs
-Version: 2023.7.0
+Version: 2024.4.0
 Summary: SSH Filesystem -- Async SSH/SFTP backend for fsspec
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: fsspec>=2021.8.1
+Requires-Dist: asyncssh<3,>=2.11.0
 Provides-Extra: bcrypt
+Requires-Dist: asyncssh[bcrypt]; extra == "bcrypt"
 Provides-Extra: fido2
+Requires-Dist: asyncssh[fido2]; extra == "fido2"
 Provides-Extra: gssapi
+Requires-Dist: asyncssh[gssapi]; extra == "gssapi"
 Provides-Extra: libnacl
+Requires-Dist: asyncssh[libnacl]; extra == "libnacl"
 Provides-Extra: pkcs11
+Requires-Dist: asyncssh[python-pkcs11]; extra == "pkcs11"
 Provides-Extra: pyopenssl
+Requires-Dist: asyncssh[pyOpenSSL]; extra == "pyopenssl"
 Provides-Extra: pywin32
-License-File: LICENSE
+Requires-Dist: asyncssh[pywin32]; extra == "pywin32"
 
 # sshfs
 
 sshfs is an implementation of [fsspec](https://github.com/intake/filesystem_spec/) for
 the SFTP protocol using [asyncssh](https://github.com/ronf/asyncssh).
 
 ## Features
```

### Comparing `sshfs-2023.7.0/README.md` & `sshfs-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/setup.cfg` & `sshfs-2024.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,12 +26,13 @@
 pkcs11 = asyncssh[python-pkcs11]
 pyopenssl = asyncssh[pyOpenSSL]
 pywin32 = asyncssh[pywin32]
 
 [options.entry_points]
 fsspec.specs = 
 	ssh = sshfs.spec:SSHFileSystem
+	sftp = sshfs.spec:SSHFileSystem
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sshfs-2023.7.0/sshfs/config.py` & `sshfs-2024.4.0/sshfs/config.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/sshfs/file.py` & `sshfs-2024.4.0/sshfs/file.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/sshfs/pools/base.py` & `sshfs-2024.4.0/sshfs/pools/base.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/sshfs/pools/hard.py` & `sshfs-2024.4.0/sshfs/pools/hard.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/sshfs/pools/soft.py` & `sshfs-2024.4.0/sshfs/pools/soft.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/sshfs/spec.py` & `sshfs-2024.4.0/sshfs/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,7 +312,14 @@
         async with self._client_lock:
             return await self.client.run(*args, **kwargs)
 
     execute = sync_wrapper(_execute)
 
     def _open(self, path, *args, **kwargs):
         return SSHFile(self, path, *args, **kwargs)
+
+    @wrap_exceptions
+    async def _cat_file(self, path, **kwargs):
+        """Asynchronously fetch the contents of a file"""
+        async with self._pool.get() as channel:
+            async with channel.open(path, "rb") as f:
+                return await f.read()
```

### Comparing `sshfs-2023.7.0/sshfs/utils.py` & `sshfs-2024.4.0/sshfs/utils.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/sshfs.egg-info/PKG-INFO` & `sshfs-2024.4.0/sshfs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: sshfs
-Version: 2023.7.0
+Version: 2024.4.0
 Summary: SSH Filesystem -- Async SSH/SFTP backend for fsspec
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: fsspec>=2021.8.1
+Requires-Dist: asyncssh<3,>=2.11.0
 Provides-Extra: bcrypt
+Requires-Dist: asyncssh[bcrypt]; extra == "bcrypt"
 Provides-Extra: fido2
+Requires-Dist: asyncssh[fido2]; extra == "fido2"
 Provides-Extra: gssapi
+Requires-Dist: asyncssh[gssapi]; extra == "gssapi"
 Provides-Extra: libnacl
+Requires-Dist: asyncssh[libnacl]; extra == "libnacl"
 Provides-Extra: pkcs11
+Requires-Dist: asyncssh[python-pkcs11]; extra == "pkcs11"
 Provides-Extra: pyopenssl
+Requires-Dist: asyncssh[pyOpenSSL]; extra == "pyopenssl"
 Provides-Extra: pywin32
-License-File: LICENSE
+Requires-Dist: asyncssh[pywin32]; extra == "pywin32"
 
 # sshfs
 
 sshfs is an implementation of [fsspec](https://github.com/intake/filesystem_spec/) for
 the SFTP protocol using [asyncssh](https://github.com/ronf/asyncssh).
 
 ## Features
```

### Comparing `sshfs-2023.7.0/sshfs.egg-info/SOURCES.txt` & `sshfs-2024.4.0/sshfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/tests/static/user.key` & `sshfs-2024.4.0/tests/static/user.key`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/tests/static/user.key.pub` & `sshfs-2024.4.0/tests/static/user.key.pub`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/tests/test_config.py` & `sshfs-2024.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/tests/test_sftp_pools.py` & `sshfs-2024.4.0/tests/test_sftp_pools.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.7.0/tests/test_sshfs.py` & `sshfs-2024.4.0/tests/test_sshfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import hashlib
 import posixpath
 import secrets
 import tempfile
 import warnings
 from concurrent import futures
-from datetime import datetime, timedelta
 from pathlib import Path
 
 import fsspec
+import pkg_resources
 import pytest
 from asyncssh.sftp import SFTPFailure
 
 from sshfs import SSHFileSystem
 
 _STATIC = (Path(__file__).parent / "static").resolve()
 USERS = {"user": _STATIC / "user.key"}
@@ -69,36 +69,38 @@
 
 def strip_keys(info):
     for key in ["name", "time", "mtime", "atime"]:
         info.pop(key, None)
 
 
 def test_fsspec_registration(ssh_server):
-    fs = fsspec.filesystem(
-        "ssh",
-        host=ssh_server.host,
-        port=ssh_server.port,
-        username="user",
-        client_keys=[USERS["user"]],
-    )
-    assert isinstance(fs, SSHFileSystem)
+    for ep in pkg_resources.iter_entry_points(group="fsspec.specs"):
+        fs = fsspec.filesystem(
+            ep.name,
+            host=ssh_server.host,
+            port=ssh_server.port,
+            username="user",
+            client_keys=[USERS["user"]],
+        )
+        assert isinstance(fs, SSHFileSystem)
 
 
 def test_fsspec_url_parsing(ssh_server, remote_dir, user="user"):
-    url = f"ssh://{user}@{ssh_server.host}:{ssh_server.port}/{remote_dir}/file"
-    with fsspec.open(url, "w", client_keys=[USERS[user]]) as file:
-        # Check the underlying file system.
-        file_fs = file.buffer.fs
-        assert isinstance(file_fs, SSHFileSystem)
-        assert file_fs.storage_options == {
-            "host": ssh_server.host,
-            "port": ssh_server.port,
-            "username": user,
-            "client_keys": [USERS[user]],
-        }
+    for ep in pkg_resources.iter_entry_points(group="fsspec.specs"):
+        url = f"{ep.name}://{user}@{ssh_server.host}:{ssh_server.port}/{remote_dir}/file"
+        with fsspec.open(url, "w", client_keys=[USERS[user]]) as file:
+            # Check the underlying file system.
+            file_fs = file.buffer.fs
+            assert isinstance(file_fs, SSHFileSystem)
+            assert file_fs.storage_options == {
+                "host": ssh_server.host,
+                "port": ssh_server.port,
+                "username": user,
+                "client_keys": [USERS[user]],
+            }
 
 
 def test_info(fs, remote_dir):
     fs.touch(remote_dir + "/a.txt")
     details = fs.info(remote_dir + "/a.txt")
     assert details["type"] == "file"
     assert details["name"] == remote_dir + "/a.txt"
@@ -331,7 +333,25 @@
                 remote_dir + "/cp_data",
                 remote_dir + f"/cp_data_{index}_{secrets.token_hex(16)}",
             )
             for index in range(16)
         ]
         for future in futures.as_completed(cp_futures):
             future.result()
+
+
+def test_cat_file_sync(fs, remote_dir):
+    # Define the content to write to the test file
+    test_content = b"Test content for cat_file"
+    test_file_path = remote_dir + "/test_file.txt"
+
+    # Write content to the file synchronously
+    with open(test_file_path, "wb") as f:
+        f.write(test_content)
+
+    # Use the cat_file method to read the content back synchronously
+    read_content = fs.cat_file(test_file_path)
+
+    # Verify the content read is the same as the content written
+    assert (
+        read_content == test_content
+    ), "The content read from the file does not match the content written."
```

