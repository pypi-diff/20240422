# Comparing `tmp/pyimg4-0.8.3.tar.gz` & `tmp/pyimg4-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimg4-0.8.3.tar", max compression
+gzip compressed data, was "pyimg4-0.8.4.tar", max compression
```

## Comparing `pyimg4-0.8.3.tar` & `pyimg4-0.8.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2024-04-05 19:38:56.486452 pyimg4-0.8.3/LICENSE
--rw-r--r--   0        0        0     1861 2024-04-05 19:38:56.486452 pyimg4-0.8.3/README.md
--rw-r--r--   0        0        0      183 2024-04-05 19:38:56.486452 pyimg4-0.8.3/pyimg4/__init__.py
--rw-r--r--   0        0        0    28418 2024-04-05 19:38:56.486452 pyimg4-0.8.3/pyimg4/__main__.py
--rw-r--r--   0        0        0     1273 2024-04-05 19:38:56.486452 pyimg4-0.8.3/pyimg4/errors.py
--rw-r--r--   0        0        0    45680 2024-04-05 19:38:56.490452 pyimg4-0.8.3/pyimg4/parser.py
--rw-r--r--   0        0        0      313 2024-04-05 19:38:56.490452 pyimg4-0.8.3/pyimg4/types.py
--rw-r--r--   0        0        0     1377 2024-04-05 19:38:56.490452 pyimg4-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     3241 1970-01-01 00:00:00.000000 pyimg4-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-22 00:52:09.828696 pyimg4-0.8.4/LICENSE
+-rw-r--r--   0        0        0     1812 2024-04-22 00:52:09.828696 pyimg4-0.8.4/README.md
+-rw-r--r--   0        0        0      183 2024-04-22 00:52:09.828696 pyimg4-0.8.4/pyimg4/__init__.py
+-rw-r--r--   0        0        0    28418 2024-04-22 00:52:09.828696 pyimg4-0.8.4/pyimg4/__main__.py
+-rw-r--r--   0        0        0     1273 2024-04-22 00:52:09.828696 pyimg4-0.8.4/pyimg4/errors.py
+-rw-r--r--   0        0        0    44770 2024-04-22 00:52:09.828696 pyimg4-0.8.4/pyimg4/parser.py
+-rw-r--r--   0        0        0      313 2024-04-22 00:52:09.828696 pyimg4-0.8.4/pyimg4/types.py
+-rw-r--r--   0        0        0     1206 2024-04-22 00:52:09.828696 pyimg4-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 pyimg4-0.8.4/PKG-INFO
```

### Comparing `pyimg4-0.8.3/LICENSE` & `pyimg4-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimg4-0.8.3/README.md` & `pyimg4-0.8.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -51,9 +51,8 @@
     - If you would like to use the compression features of PyIMG4, install the optional libraries:
       - ```python3 -m pip install pyimg4[compression]```
 - Local installation:
     - `./install.sh`
     - Requires [Poetry](https://python-poetry.org)
 
 ## Support
-
-For any questions/issues you have, [open an issue](https://github.com/m1stadev/PyIMG4/issues) or join my [Discord](https://m1sta.xyz/discord).
+For any questions/issues you have, [open an issue](https://github.com/m1stadev/PyIMG4/issues).
```

#### html2text {}

```diff
@@ -8,9 +8,8 @@
 im4p Image4 payload commands. im4r Image4 restore info commands. img4 Image4
 commands. ``` ## Requirements - Python 3.8 or higher ## Installation - Install
 from [PyPI](https://pypi.org/project/pyimg4/): - ```python3 -m pip install
 pyimg4``` - If you would like to use the compression features of PyIMG4,
 install the optional libraries: - ```python3 -m pip install pyimg4
 [compression]``` - Local installation: - `./install.sh` - Requires [Poetry]
 (https://python-poetry.org) ## Support For any questions/issues you have, [open
-an issue](https://github.com/m1stadev/PyIMG4/issues) or join my [Discord]
-(https://m1sta.xyz/discord).
+an issue](https://github.com/m1stadev/PyIMG4/issues).
```

### Comparing `pyimg4-0.8.3/pyimg4/__main__.py` & `pyimg4-0.8.4/pyimg4/__main__.py`

 * *Files identical despite different names*

### Comparing `pyimg4-0.8.3/pyimg4/errors.py` & `pyimg4-0.8.4/pyimg4/errors.py`

 * *Files identical despite different names*

### Comparing `pyimg4-0.8.3/pyimg4/parser.py` & `pyimg4-0.8.4/pyimg4/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,41 @@
 from sys import platform
 from typing import Any, List, Optional, Tuple, Union
 from zlib import adler32
 
 import asn1
+import lzss
 from Crypto.Cipher import AES
 
 from .errors import CompressionError, UnexpectedDataError, UnexpectedTagError
 from .types import Compression, KeybagType, Payload
 
-try:
-    import lzss
-
-    _have_lzss = True
-except ImportError:
-    _have_lzss = False
-
-_have_lzfse = False
 if platform == 'Darwin':
-    try:
-        import apple_compress
-
-        def _lzfse_decompress(data: bytes, decmp_size: Optional[int] = None) -> bytes:
-            return apple_compress.decompress(
-                data,
-                algorithm=apple_compress.Algorithm.LZFSE_IBOOT,
-                decmp_size=decmp_size,
-            )
-
-        def _lzfse_compress(data: bytes) -> bytes:
-            return apple_compress.compress(
-                data, algorithm=apple_compress.Algorithm.LZFSE_IBOOT
-            )
+    import apple_compress
 
-        _have_lzfse = True
-    except ImportError:
-        pass
+    def _lzfse_compress(data: bytes) -> bytes:
+        return apple_compress.compress(
+            data, algorithm=apple_compress.Algorithm.LZFSE_IBOOT
+        )
 
-if _have_lzfse is False:
-    try:
-        import liblzfse
+    def _lzfse_decompress(data: bytes, decmp_size: Optional[int] = None) -> bytes:
+        return apple_compress.decompress(
+            data,
+            algorithm=apple_compress.Algorithm.LZFSE_IBOOT,
+            decmp_size=decmp_size,
+        )
 
-        def _lzfse_decompress(data: bytes, _: Optional[int] = None) -> bytes:
-            return liblzfse.decompress(data)
+else:
+    import lzfse
 
-        def _lzfse_compress(data: bytes) -> bytes:
-            return liblzfse.compress(data)
+    def _lzfse_compress(data: bytes) -> bytes:
+        return lzfse.compress(data)
 
-        _have_lzfse = True
-    except ImportError:
-        pass
+    def _lzfse_decompress(data: bytes, _: Optional[int] = None) -> bytes:
+        return lzfse.decompress(data)
 
 
 class _PyIMG4:
     def __init__(self, data: Optional[bytes] = None) -> None:
         self._data = data
 
         self._decoder = asn1.Decoder()
@@ -1175,63 +1158,55 @@
         if self.compression != Compression.NONE:
             repr_ += f', compression={self.compression.name}'
 
         return f'{repr_})'
 
     def _create_complzss_header(self, comp_size: int) -> bytes:
         header = bytearray(b'complzss')
-        header += adler32(self._data).to_bytes(4, 'big')
+        header += adler32(self.data).to_bytes(4, 'big')
         header += self.size.to_bytes(4, 'big')
         header += comp_size.to_bytes(4, 'big')
         header += int(1).to_bytes(4, 'big')
         header += bytearray(0x180 - len(header))
 
         return bytes(header)
 
     def _decompress_data(
         self, data: bytes, compression: Compression, size: Optional[int] = None
     ) -> bytes:
         if compression == Compression.LZSS:
-            if not _have_lzss:
-                raise RuntimeError('pylzss not installed, cannot use LZSS compression')
-
             return lzss.decompress(data)
 
         elif self.compression == Compression.LZFSE:
-            if not _have_lzfse:
-                raise RuntimeError(
-                    'apple-compress/pyliblzfse not installed, cannot use LZFSE compression'
-                )
-
-            return _lzfse_decompress(self._data, size)
+            return _lzfse_decompress(self.data, size)
 
     def _detect_compression(self, size: int, data: bytes) -> None:
         if self.encrypted and size > 0:
             self._compression = Compression.LZFSE_ENCRYPTED
 
         elif data.startswith(b'complzss'):
             self._compression = Compression.LZSS
 
-        elif data.startswith(b'bvx2') and b'bvx$' in self._data:
+        elif data.startswith(b'bvx2') and b'bvx$' in self.data:
             self._compression = Compression.LZFSE
 
         else:
             self._compression = Compression.NONE
 
     def _parse_complzss_header(self) -> None:
-        self.size = int(self._data[0xC:0x10].hex(), 16)
-        cmp_len = int(self._data[0x10:0x14].hex(), 16)
+        self.size = int(self.data[0xC:0x10].hex(), 16)
+        cmp_len = int(self.data[0x10:0x14].hex(), 16)
 
         if (
-            cmp_len < len(self._data) - 0x180
+            cmp_len < len(self.data) - 0x180
         ):  # iOS 9+ A7-A9 kernelcache, so KPP is appended to the LZSS-compressed data
-            extra_len = len(self._data) - cmp_len - 0x180
-            self.extra = self._data[-extra_len:]
+            extra_len = len(self.data) - cmp_len - 0x180
+            self.extra = self.data[-extra_len:]
 
-            self._data = self._data[:-extra_len]
+            self._data = self.data[:-extra_len]
 
     @property
     def compression(self) -> Compression:
         return self._compression
 
     @property
     def data(self) -> bytes:
@@ -1268,15 +1243,15 @@
         if size < 0:
             raise ValueError('Size cannot be less than 0.')
 
         if 0 < size < len(self.data):
             raise ValueError('Size cannot be less than the length of the payload data.')
 
         if self.encrypted is True:
-            self._detect_compression(size, self._data)
+            self._detect_compression(size, self.data)
 
         self._size = size
 
     def add_keybag(self, keybag: Keybag) -> None:
         if not isinstance(keybag, Keybag):
             raise UnexpectedDataError('Keybag', keybag)
 
@@ -1320,54 +1295,43 @@
 
         if self.encrypted is True:
             raise CompressionError('Cannot compress encrypted payload.')
 
         elif self.compression in (Compression.LZSS, Compression.LZFSE):
             raise CompressionError(f'Payload is already {compression.name}-compressed.')
 
-        self.size = len(self._data)
+        self.size = len(self.data)
         if compression == Compression.LZSS:
-            if not _have_lzss:
-                raise RuntimeError('pylzss not installed, cannot use LZSS compression')
-
-            comp_data = lzss.compress(self._data)
+            comp_data = lzss.compress(self.data)
             self._data = self._create_complzss_header(len(comp_data)) + comp_data
 
         elif compression == Compression.LZFSE:
-            if not _have_lzfse:
-                raise RuntimeError(
-                    'apple-compress/pyliblzfse not installed, cannot use LZFSE compression'
-                )
-
-            comp_data = _lzfse_compress(self._data)
+            comp_data = _lzfse_compress(self.data)
             if not (comp_data.startswith(b'bvx2') and b'bvx$' in comp_data):
                 raise CompressionError('Failed to LZFSE-compress payload.')
 
             self._data = comp_data
 
-        self._detect_compression(self.size, self._data)
-
-        if self.extra is not None:
-            self._data += self.extra
+        self._detect_compression(self.size, self.data)
 
     def decompress(self) -> None:
         if self.compression == Compression.NONE:
             raise CompressionError('Payload is not compressed.')
 
         elif self.compression == Compression.LZFSE_ENCRYPTED:
             raise CompressionError('Cannot decompress encrypted payload.')
 
-        self._data = self._decompress_data(self._data, self.compression, self.size)
+        self._data = self._decompress_data(self.data, self.compression, self.size)
         self._compression = Compression.NONE
-        self._detect_compression(self.size, self._data)
+        self._detect_compression(self.size, self.data)
 
     def decrypt(self, kbag: Keybag) -> None:
-        self._data = AES.new(kbag.key, AES.MODE_CBC, kbag.iv).decrypt(self._data)
+        self._data = AES.new(kbag.key, AES.MODE_CBC, kbag.iv).decrypt(self.data)
         self._keybags = []
-        self._detect_compression(self.size, self._data)
+        self._detect_compression(self.size, self.data)
 
         if self.compression == Compression.LZSS:
             self._parse_complzss_header()
         elif self.compression == Compression.LZFSE:
             self.size = len(self._decompress_data(self.data, self.compression))
 
     def output(self) -> Payload:
@@ -1396,8 +1360,13 @@
                             asn1.Numbers.OctetString,
                             asn1.Types.Primitive,
                             asn1.Classes.Universal,
                         )
 
             kbag_data = self._encoder.output()
 
-        return Payload(self._data, kbag_data)
+        if self.extra is not None:
+            data = self.data + self.extra
+        else:
+            data = self.data
+
+        return Payload(data, kbag_data)
```

### Comparing `pyimg4-0.8.3/pyproject.toml` & `pyimg4-0.8.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyimg4"
-version = "0.8.3"
+version = "0.8.4"
 description = "A Python library/CLI tool for parsing Apple's Image4 format."
 authors = ["m1stadev <adamhamdi31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/m1stadev/PyIMG4"
 keywords = ["ios", "jailbreak", "iboot", "img4", "image4"]
 classifiers = [
@@ -20,20 +20,17 @@
 pyimg4 = "pyimg4.__main__:cli"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 asn1 = "^2.7.0"
 click = "^8.1.7"
 pycryptodome = "^3.18.0"
-pyliblzfse = {version = "^0.4.1", optional = true}
-pylzss = {version = "^0.3.4", optional = true}
-apple-compress = {version = "^0.2.3", optional = true}
-
-[tool.poetry.extras]
-compression = ["apple-compress", "pyliblzfse", "pylzss"]
+lzfse = "^0.4.2"
+apple-compress = "^0.2.3"
+pylzss = "^0.3.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
 remotezip = "^0.12.1"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

### Comparing `pyimg4-0.8.3/PKG-INFO` & `pyimg4-0.8.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimg4
-Version: 0.8.3
+Version: 0.8.4
 Summary: A Python library/CLI tool for parsing Apple's Image4 format.
 Home-page: https://github.com/m1stadev/PyIMG4
 License: MIT
 Keywords: ios,jailbreak,iboot,img4,image4
 Author: m1stadev
 Author-email: adamhamdi31@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -16,21 +16,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
-Provides-Extra: compression
-Requires-Dist: apple-compress (>=0.2.3,<0.3.0) ; extra == "compression"
+Requires-Dist: apple-compress (>=0.2.3,<0.3.0)
 Requires-Dist: asn1 (>=2.7.0,<3.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: lzfse (>=0.4.2,<0.5.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
-Requires-Dist: pyliblzfse (>=0.4.1,<0.5.0) ; extra == "compression"
-Requires-Dist: pylzss (>=0.3.4,<0.4.0) ; extra == "compression"
+Requires-Dist: pylzss (>=0.3.7,<0.4.0)
 Project-URL: Bug Tracker, https://github.com/m1stadev/PyIMG4/issues
 Project-URL: Repository, https://github.com/m1stadev/PyIMG4
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src=".github/assets/icon.png" alt="https://github.com/m1stadev/PyIMG4" width=256px> 
 </p>
@@ -84,10 +83,9 @@
     - If you would like to use the compression features of PyIMG4, install the optional libraries:
       - ```python3 -m pip install pyimg4[compression]```
 - Local installation:
     - `./install.sh`
     - Requires [Poetry](https://python-poetry.org)
 
 ## Support
-
-For any questions/issues you have, [open an issue](https://github.com/m1stadev/PyIMG4/issues) or join my [Discord](https://m1sta.xyz/discord).
+For any questions/issues you have, [open an issue](https://github.com/m1stadev/PyIMG4/issues).
```

#### html2text {}

```diff
@@ -1,35 +1,32 @@
-Metadata-Version: 2.1 Name: pyimg4 Version: 0.8.3 Summary: A Python library/CLI
+Metadata-Version: 2.1 Name: pyimg4 Version: 0.8.4 Summary: A Python library/CLI
 tool for parsing Apple's Image4 format. Home-page: https://github.com/m1stadev/
 PyIMG4 License: MIT Keywords: ios,jailbreak,iboot,img4,image4 Author: m1stadev
 Author-email: adamhamdi31@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Utilities Provides-Extra: compression Requires-Dist: apple-compress
-(>=0.2.3,<0.3.0) ; extra == "compression" Requires-Dist: asn1 (>=2.7.0,<3.0.0)
-Requires-Dist: click (>=8.1.7,<9.0.0) Requires-Dist: pycryptodome
-(>=3.18.0,<4.0.0) Requires-Dist: pyliblzfse (>=0.4.1,<0.5.0) ; extra ==
-"compression" Requires-Dist: pylzss (>=0.3.4,<0.4.0) ; extra == "compression"
-Project-URL: Bug Tracker, https://github.com/m1stadev/PyIMG4/issues Project-
-URL: Repository, https://github.com/m1stadev/PyIMG4 Description-Content-Type:
-text/markdown
+Topic :: Utilities Requires-Dist: apple-compress (>=0.2.3,<0.3.0) Requires-
+Dist: asn1 (>=2.7.0,<3.0.0) Requires-Dist: click (>=8.1.7,<9.0.0) Requires-
+Dist: lzfse (>=0.4.2,<0.5.0) Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
+Requires-Dist: pylzss (>=0.3.7,<0.4.0) Project-URL: Bug Tracker, https://
+github.com/m1stadev/PyIMG4/issues Project-URL: Repository, https://github.com/
+m1stadev/PyIMG4 Description-Content-Type: text/markdown
                      [https://github.com/m1stadev/PyIMG4]
                              ************ PPyyIIMMGG44 ************
 
          A Python library/CLI tool for parsing Apple's _I_m_a_g_e_4_ _f_o_r_m_a_t.
 ## Usage ``` Usage: pyimg4 [OPTIONS] COMMAND [ARGS]... A Python CLI tool for
 parsing Apple's Image4 format. Options: --version Show the version and exit. -
 h, --help Show this message and exit. Commands: im4m Image4 manifest commands.
 im4p Image4 payload commands. im4r Image4 restore info commands. img4 Image4
 commands. ``` ## Requirements - Python 3.8 or higher ## Installation - Install
 from [PyPI](https://pypi.org/project/pyimg4/): - ```python3 -m pip install
 pyimg4``` - If you would like to use the compression features of PyIMG4,
 install the optional libraries: - ```python3 -m pip install pyimg4
 [compression]``` - Local installation: - `./install.sh` - Requires [Poetry]
 (https://python-poetry.org) ## Support For any questions/issues you have, [open
-an issue](https://github.com/m1stadev/PyIMG4/issues) or join my [Discord]
-(https://m1sta.xyz/discord).
+an issue](https://github.com/m1stadev/PyIMG4/issues).
```

