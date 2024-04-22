# Comparing `tmp/nanopb-0.4.9.dev1464.tar.gz` & `tmp/nanopb-0.4.9.dev1465.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanopb-0.4.9.dev1464.tar", max compression
+gzip compressed data, was "nanopb-0.4.9.dev1465.tar", max compression
```

## Comparing `nanopb-0.4.9.dev1464.tar` & `nanopb-0.4.9.dev1465.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     4461 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/README.md
--rw-r--r--   0        0        0        0 2024-03-04 02:10:06.362625 nanopb-0.4.9.dev1464/nanopb/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 02:10:06.362625 nanopb-0.4.9.dev1464/nanopb/generator/__init__.py
--rwxr-xr-x   0        0        0      235 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/nanopb_generator
--rw-r--r--   0        0        0      206 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/nanopb_generator.bat
--rwxr-xr-x   0        0        0   112055 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/nanopb_generator.py
--rwxr-xr-x   0        0        0      460 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/nanopb_generator.py2
--rw-r--r--   0        0        0     5839 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/platformio_generator.py
--rw-r--r--   0        0        0      126 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/proto/Makefile
--rw-r--r--   0        0        0     4851 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/proto/__init__.py
--rw-r--r--   0        0        0     3431 2024-03-04 02:10:06.386625 nanopb-0.4.9.dev1464/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2662 2024-03-04 02:10:06.462625 nanopb-0.4.9.dev1464/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc
--rw-r--r--   0        0        0     2790 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/proto/_utils.py
--rw-r--r--   0        0        0    36277 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/proto/google/protobuf/descriptor.proto
--rw-r--r--   0        0        0     7139 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/proto/nanopb.proto
--rw-r--r--   0        0        0     4443 2024-03-04 02:10:06.470625 nanopb-0.4.9.dev1464/nanopb/generator/proto/nanopb_pb2.py
--rwxr-xr-x   0        0        0     1577 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/protoc
--rwxr-xr-x   0        0        0      374 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/protoc-gen-nanopb
--rwxr-xr-x   0        0        0      554 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/protoc-gen-nanopb-py2
--rw-r--r--   0        0        0      449 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/protoc-gen-nanopb.bat
--rw-r--r--   0        0        0      302 2024-03-02 12:07:14.000000 nanopb-0.4.9.dev1464/nanopb/generator/protoc.bat
--rw-r--r--   0        0        0     1065 2024-03-04 02:10:06.486625 nanopb-0.4.9.dev1464/pyproject.toml
--rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 nanopb-0.4.9.dev1464/PKG-INFO
+-rw-r--r--   0        0        0     4461 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 02:09:19.262771 nanopb-0.4.9.dev1465/nanopb/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 02:09:19.262771 nanopb-0.4.9.dev1465/nanopb/generator/__init__.py
+-rwxr-xr-x   0        0        0      235 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/nanopb_generator
+-rw-r--r--   0        0        0      206 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/nanopb_generator.bat
+-rwxr-xr-x   0        0        0   112055 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/nanopb_generator.py
+-rwxr-xr-x   0        0        0      460 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/nanopb_generator.py2
+-rw-r--r--   0        0        0     5839 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/platformio_generator.py
+-rw-r--r--   0        0        0      126 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/proto/Makefile
+-rw-r--r--   0        0        0     4851 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/proto/__init__.py
+-rw-r--r--   0        0        0     3431 2024-04-22 02:09:19.278771 nanopb-0.4.9.dev1465/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2662 2024-04-22 02:09:19.354771 nanopb-0.4.9.dev1465/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2790 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/proto/_utils.py
+-rw-r--r--   0        0        0    36277 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/proto/google/protobuf/descriptor.proto
+-rw-r--r--   0        0        0     7139 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/proto/nanopb.proto
+-rw-r--r--   0        0        0     4443 2024-04-22 02:09:19.362772 nanopb-0.4.9.dev1465/nanopb/generator/proto/nanopb_pb2.py
+-rwxr-xr-x   0        0        0     1577 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/protoc
+-rwxr-xr-x   0        0        0      374 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/protoc-gen-nanopb
+-rwxr-xr-x   0        0        0      554 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/protoc-gen-nanopb-py2
+-rw-r--r--   0        0        0      449 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/protoc-gen-nanopb.bat
+-rw-r--r--   0        0        0      302 2024-04-19 15:52:04.000000 nanopb-0.4.9.dev1465/nanopb/generator/protoc.bat
+-rw-r--r--   0        0        0     1065 2024-04-22 02:09:19.382772 nanopb-0.4.9.dev1465/pyproject.toml
+-rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 nanopb-0.4.9.dev1465/PKG-INFO
```

### Comparing `nanopb-0.4.9.dev1464/README.md` & `nanopb-0.4.9.dev1465/README.md`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1464/nanopb/generator/nanopb_generator.py` & `nanopb-0.4.9.dev1465/nanopb/generator/nanopb_generator.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1464/nanopb/generator/platformio_generator.py` & `nanopb-0.4.9.dev1465/nanopb/generator/platformio_generator.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1464/nanopb/generator/proto/__init__.py` & `nanopb-0.4.9.dev1465/nanopb/generator/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1464/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc` & `nanopb-0.4.9.dev1465/nanopb/generator/proto/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Mar  2 12:07:14 2024 UTC, .py size: 4851 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 7216 e365 f312 0000  U.......r..e....
+00000000: 550d 0d0a 0000 0000 2493 2266 f312 0000  U.......$."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a03 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6403 6c06 5a06 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 5a07 6401 6403 6c08 5a08 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6403 6c09 5a09 6404 6405 6c0a 6d0b 5a0b  d.l.Z.d.d.l.m.Z.
```

### Comparing `nanopb-0.4.9.dev1464/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc` & `nanopb-0.4.9.dev1465/nanopb/generator/proto/__pycache__/_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Mar  2 12:07:14 2024 UTC, .py size: 2790 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 7216 e365 e60a 0000  U.......r..e....
+00000000: 550d 0d0a 0000 0000 2493 2266 e60a 0000  U.......$."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6402 6403 8400 5a04 6404  d.l.Z.d.d...Z.d.
 00000050: 6405 8400 5a05 6406 6407 8400 5a06 6408  d...Z.d.d...Z.d.
 00000060: 6409 8400 5a07 6508 640a 6b02 7246 6507  d...Z.e.d.k.rFe.
 00000070: 8300 0100 6401 5300 290b e900 0000 004e  ....d.S.)......N
```

### Comparing `nanopb-0.4.9.dev1464/nanopb/generator/proto/_utils.py` & `nanopb-0.4.9.dev1465/nanopb/generator/proto/_utils.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1464/nanopb/generator/proto/google/protobuf/descriptor.proto` & `nanopb-0.4.9.dev1465/nanopb/generator/proto/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1464/nanopb/generator/proto/nanopb.proto` & `nanopb-0.4.9.dev1465/nanopb/generator/proto/nanopb.proto`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1464/nanopb/generator/proto/nanopb_pb2.py` & `nanopb-0.4.9.dev1465/nanopb/generator/proto/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1464/nanopb/generator/protoc` & `nanopb-0.4.9.dev1465/nanopb/generator/protoc`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1464/nanopb/generator/protoc-gen-nanopb-py2` & `nanopb-0.4.9.dev1465/nanopb/generator/protoc-gen-nanopb-py2`

 * *Files identical despite different names*

### Comparing `nanopb-0.4.9.dev1464/pyproject.toml` & `nanopb-0.4.9.dev1465/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nanopb"
-version = "0.4.9-dev1464"
+version = "0.4.9-dev1465"
 description = "Nanopb is a small code-size Protocol Buffers implementation in ansi C. It is especially suitable for use in microcontrollers, but fits any memory restricted system."
 authors = ["Petteri Aimonen <jpa@npb.mail.kapsi.fi>"]
 license = "Zlib"
 repository = "https://github.com/nanopb/nanopb/"
 readme = "README.md"
 homepage = "https://jpa.kapsi.fi/nanopb/"
 documentation = "https://jpa.kapsi.fi/nanopb/docs/index.html"
```

### Comparing `nanopb-0.4.9.dev1464/PKG-INFO` & `nanopb-0.4.9.dev1465/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanopb
-Version: 0.4.9.dev1464
+Version: 0.4.9.dev1465
 Summary: Nanopb is a small code-size Protocol Buffers implementation in ansi C. It is especially suitable for use in microcontrollers, but fits any memory restricted system.
 Home-page: https://jpa.kapsi.fi/nanopb/
 License: Zlib
 Keywords: protobuf,protoc
 Author: Petteri Aimonen
 Author-email: jpa@npb.mail.kapsi.fi
 Requires-Python: >=2.7
```

