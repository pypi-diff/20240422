# Comparing `tmp/cs.binary-20240316.tar.gz` & `tmp/cs.binary-20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.binary-20240316.tar", last modified: Sat Mar 16 06:57:14 2024, max compression
+gzip compressed data, was "cs.binary-20240422.tar", last modified: Mon Apr 22 06:30:55 2024, max compression
```

## Comparing `cs.binary-20240316.tar` & `cs.binary-20240422.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:57:14.044664 cs.binary-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 06:56:51.000000 cs.binary-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    19673 2024-03-16 06:57:14.044291 cs.binary-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    33594 2024-03-16 06:56:58.000000 cs.binary-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:57:14.038879 cs.binary-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:57:14.039175 cs.binary-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:57:14.041719 cs.binary-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    51436 2024-03-16 06:56:41.000000 cs.binary-20240316/lib/python/cs/binary.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:57:14.043757 cs.binary-20240316/lib/python/cs.binary.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    19673 2024-03-16 06:57:13.000000 cs.binary-20240316/lib/python/cs.binary.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-03-16 06:57:14.000000 cs.binary-20240316/lib/python/cs.binary.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 06:57:13.000000 cs.binary-20240316/lib/python/cs.binary.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      111 2024-03-16 06:57:13.000000 cs.binary-20240316/lib/python/cs.binary.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 06:57:13.000000 cs.binary-20240316/lib/python/cs.binary.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    20164 2024-03-16 06:57:12.000000 cs.binary-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:57:14.044764 cs.binary-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 06:30:55.321897 cs.binary-20240422/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 06:30:31.000000 cs.binary-20240422/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    34159 2024-04-22 06:30:55.321605 cs.binary-20240422/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    33150 2024-04-22 06:30:39.000000 cs.binary-20240422/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 06:30:55.317232 cs.binary-20240422/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 06:30:55.317489 cs.binary-20240422/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 06:30:55.318899 cs.binary-20240422/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    51423 2024-04-22 06:30:17.000000 cs.binary-20240422/lib/python/cs/binary.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 06:30:55.321175 cs.binary-20240422/lib/python/cs.binary.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    34159 2024-04-22 06:30:54.000000 cs.binary-20240422/lib/python/cs.binary.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-04-22 06:30:55.000000 cs.binary-20240422/lib/python/cs.binary.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 06:30:54.000000 cs.binary-20240422/lib/python/cs.binary.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      111 2024-04-22 06:30:55.000000 cs.binary-20240422/lib/python/cs.binary.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 06:30:55.000000 cs.binary-20240422/lib/python/cs.binary.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    34651 2024-04-22 06:30:53.000000 cs.binary-20240422/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 06:30:55.321981 cs.binary-20240422/setup.cfg
```

### Comparing `cs.binary-20240316/README.md` & `cs.binary-20240422/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,34 @@
+Metadata-Version: 2.1
+Name: cs.binary
+Version: 20240422
+Summary: Facilities associated with binary data parsing and transcription. The classes in this module support easy parsing of binary data structures, returning instances with the binary data decoded into attributes and capable of transcribing themselves in binary form (trivially via `bytes(instance)` and also otherwise).
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python3
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
 Facilities associated with binary data parsing and transcription.
 The classes in this module support easy parsing of binary data
 structures,
 returning instances with the binary data decoded into attributes
 and capable of transcribing themselves in binary form
 (trivially via `bytes(instance)` and also otherwise).
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240422*:
+New _BinaryMultiValue_Base.for_json() method returning a dict containing the fields.
 
 Note: this module requires Python 3.6+ because various default
 behaviours rely on `dict`s preserving their insert order.
 
 See `cs.iso14496` for an ISO 14496 (eg MPEG4) parser
 built using this module.
 
@@ -86,24 +104,24 @@
   the components of the structure,
   including substranscriptions which themselves
   adhere to this protocol - they may be `None`, `bytes`-like objects,
   ASCII compatible strings or iterables.
   This supports directly returning or yielding the result of a field's
   `.transcribe` method.
 
-## Class `BinaryByteses(AbstractBinary, BinaryMixin)`
+## Class `BinaryByteses(AbstractBinary)`
 
 A list of `bytes` parsed directly from the native iteration of the buffer.
 
 ## Function `BinaryFixedBytes(class_name, length: int)`
 
 Factory for an `AbstractBinary` subclass matching `length` bytes of data.
 The bytes are saved as the attribute `.data`.
 
-## Class `BinaryListValues(AbstractBinary, BinaryMixin)`
+## Class `BinaryListValues(AbstractBinary)`
 
 A list of values with a common parse specification,
 such as sample or Boxes in an ISO14496 Box structure.
 
 *Method `BinaryListValues.parse(bfr, count=None, *, end_offset=None, min_count=None, max_count=None, pt)`*:
 Read values from `bfr`.
 Return a `BinaryListValue` containing the values.
@@ -391,15 +409,15 @@
     <_struct.Struct object at ...>
     >>> field = UInt16BE.from_bytes(bytes((2,3)))
     >>> field
     UInt16BE(value=515)
     >>> field.value
     515
 
-## Class `BinarySingleValue(AbstractBinary, BinaryMixin)`
+## Class `BinarySingleValue(AbstractBinary)`
 
 A representation of a single value as the attribute `.value`.
 
 Subclasses must implement:
 * `parse` or `parse_value`
 * `transcribe` or `transcribe_value`
 
@@ -426,15 +444,15 @@
 Subclasses must implement this method or `transcribe_value`.
 
 *Method `BinarySingleValue.transcribe_value(value)`*:
 Transcribe `value` as bytes based on this class.
 
 Subclasses must implement this method or `transcribe`.
 
-## Class `BinaryUTF16NUL(BinarySingleValue, AbstractBinary, BinaryMixin)`
+## Class `BinaryUTF16NUL(BinarySingleValue)`
 
 A NUL terminated UTF-16 string.
 
 *Method `BinaryUTF16NUL.__init__(self, value, *, encoding)`*:
 pylint: disable=super-init-not-called
 
 *Method `BinaryUTF16NUL.parse(bfr, *, encoding)`*:
@@ -447,25 +465,25 @@
 
 *Method `BinaryUTF16NUL.transcribe(self)`*:
 Transcribe `self.value` in UTF-16 with a terminating NUL.
 
 *Method `BinaryUTF16NUL.transcribe_value(value, encoding='utf-16')`*:
 Transcribe `value` in UTF-16 with a terminating NUL.
 
-## Class `BinaryUTF8NUL(BinarySingleValue, AbstractBinary, BinaryMixin)`
+## Class `BinaryUTF8NUL(BinarySingleValue)`
 
 A NUL terminated UTF-8 string.
 
 *Method `BinaryUTF8NUL.parse_value(bfr)`*:
 Read a NUL terminated UTF-8 string from `bfr`, return field.
 
 *Method `BinaryUTF8NUL.transcribe_value(s)`*:
 Transcribe the `value` in UTF-8 with a terminating NUL.
 
-## Class `BSData(BinarySingleValue, AbstractBinary, BinaryMixin)`
+## Class `BSData(BinarySingleValue)`
 
 A run length encoded data chunk, with the length encoded as a `BSUInt`.
 
 *Property `BSData.data`*:
 An alias for the `.value` attribute.
 
 *Property `BSData.data_offset`*:
@@ -477,35 +495,35 @@
 
 *Method `BSData.parse_value(bfr)`*:
 Parse the data from `bfr`.
 
 *Method `BSData.transcribe_value(data)`*:
 Transcribe the payload length and then the payload.
 
-## Class `BSSFloat(BinarySingleValue, AbstractBinary, BinaryMixin)`
+## Class `BSSFloat(BinarySingleValue)`
 
 A float transcribed as a BSString of str(float).
 
 *Method `BSSFloat.parse_value(bfr)`*:
 Parse a BSSFloat from a buffer and return the float.
 
 *Method `BSSFloat.transcribe_value(f)`*:
 Transcribe a float.
 
-## Class `BSString(BinarySingleValue, AbstractBinary, BinaryMixin)`
+## Class `BSString(BinarySingleValue)`
 
 A run length encoded string, with the length encoded as a BSUInt.
 
 *Method `BSString.parse_value(bfr, encoding='utf-8', errors='strict')`*:
 Parse a run length encoded string from `bfr`.
 
 *Method `BSString.transcribe_value(value: str, encoding='utf-8')`*:
 Transcribe a string.
 
-## Class `BSUInt(BinarySingleValue, AbstractBinary, BinaryMixin)`
+## Class `BSUInt(BinarySingleValue)`
 
 A binary serialised unsigned `int`.
 
 This uses a big endian byte encoding where continuation octets
 have their high bit set. The bits contributing to the value
 are in the low order 7 bits.
 
@@ -563,15 +581,15 @@
         yield self.theHandler
         yield self.boxes
 
 The binary classes `flatten` the result of the `.transcribe`
 method to obtain `bytes` insteances for the object's bnary
 transcription.
 
-## Class `Float64BE(Float64BE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `Float64BE(Float64BE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'>d'` and presents the attributes ('value',).
 
 *Method `Float64BE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -580,15 +598,15 @@
 
 *Method `Float64BE.transcribe(self)`*:
 Transcribe via `struct.pack`.
 
 *Method `Float64BE.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
-## Class `Float64LE(Float64LE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `Float64LE(Float64LE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'<d'` and presents the attributes ('value',).
 
 *Method `Float64LE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -597,15 +615,15 @@
 
 *Method `Float64LE.transcribe(self)`*:
 Transcribe via `struct.pack`.
 
 *Method `Float64LE.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
-## Class `Int16BE(Int16BE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `Int16BE(Int16BE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'>h'` and presents the attributes ('value',).
 
 *Method `Int16BE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -614,15 +632,15 @@
 
 *Method `Int16BE.transcribe(self)`*:
 Transcribe via `struct.pack`.
 
 *Method `Int16BE.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
-## Class `Int16LE(Int16LE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `Int16LE(Int16LE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'<h'` and presents the attributes ('value',).
 
 *Method `Int16LE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -631,15 +649,15 @@
 
 *Method `Int16LE.transcribe(self)`*:
 Transcribe via `struct.pack`.
 
 *Method `Int16LE.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
-## Class `Int32BE(Int32BE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `Int32BE(Int32BE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'>l'` and presents the attributes ('value',).
 
 *Method `Int32BE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -648,15 +666,15 @@
 
 *Method `Int32BE.transcribe(self)`*:
 Transcribe via `struct.pack`.
 
 *Method `Int32BE.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
-## Class `Int32LE(Int32LE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `Int32LE(Int32LE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'<l'` and presents the attributes ('value',).
 
 *Method `Int32LE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -696,15 +714,15 @@
 
 Otherwise, if `pt` is an `int`
 define `f_parse_value` to obtain exactly that many bytes from a buffer
 and `f_transcribe_value` to return those bytes directly.
 
 Otherwise presume `pt` is a 2-tuple of `(f_parse_value,f_transcribe_value)`.
 
-## Class `SimpleBinary(types.SimpleNamespace, AbstractBinary, BinaryMixin)`
+## Class `SimpleBinary(types.SimpleNamespace, AbstractBinary)`
 
 Abstract binary class based on a `SimpleNamespace`,
 thus providing a nice `__str__` and a keyword based `__init__`.
 Implementors must still define `.parse` and `.transcribe`.
 
 To constrain the arguments passed to `__init__`,
 define an `__init__` which accepts specific keyword arguments
@@ -712,15 +730,15 @@
 
     def __init__(self, *, field1=None, field2):
         """ Accept only `field1` (optional)
             and `field2` (mandatory).
         """
         super().__init__(field1=field1, field2=field2)
 
-## Class `UInt16BE(UInt16BE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `UInt16BE(UInt16BE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'>H'` and presents the attributes ('value',).
 
 *Method `UInt16BE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -729,15 +747,15 @@
 
 *Method `UInt16BE.transcribe(self)`*:
 Transcribe via `struct.pack`.
 
 *Method `UInt16BE.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
-## Class `UInt16LE(UInt16LE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `UInt16LE(UInt16LE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'<H'` and presents the attributes ('value',).
 
 *Method `UInt16LE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -746,15 +764,15 @@
 
 *Method `UInt16LE.transcribe(self)`*:
 Transcribe via `struct.pack`.
 
 *Method `UInt16LE.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
-## Class `UInt32BE(UInt32BE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `UInt32BE(UInt32BE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'>L'` and presents the attributes ('value',).
 
 *Method `UInt32BE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -763,15 +781,15 @@
 
 *Method `UInt32BE.transcribe(self)`*:
 Transcribe via `struct.pack`.
 
 *Method `UInt32BE.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
-## Class `UInt32LE(UInt32LE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `UInt32LE(UInt32LE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'<L'` and presents the attributes ('value',).
 
 *Method `UInt32LE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -780,15 +798,15 @@
 
 *Method `UInt32LE.transcribe(self)`*:
 Transcribe via `struct.pack`.
 
 *Method `UInt32LE.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
-## Class `UInt64BE(UInt64BE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `UInt64BE(UInt64BE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'>Q'` and presents the attributes ('value',).
 
 *Method `UInt64BE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -797,15 +815,15 @@
 
 *Method `UInt64BE.transcribe(self)`*:
 Transcribe via `struct.pack`.
 
 *Method `UInt64BE.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
-## Class `UInt64LE(UInt64LE, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `UInt64LE(UInt64LE, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'<Q'` and presents the attributes ('value',).
 
 *Method `UInt64LE.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -814,15 +832,15 @@
 
 *Method `UInt64LE.transcribe(self)`*:
 Transcribe via `struct.pack`.
 
 *Method `UInt64LE.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
-## Class `UInt8(UInt8, builtins.tuple, AbstractBinary, BinaryMixin)`
+## Class `UInt8(UInt8, AbstractBinary)`
 
 An `AbstractBinary` `namedtuple` which parses and transcribes
 the struct format `'B'` and presents the attributes ('value',).
 
 *Method `UInt8.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse from `bfr` via `struct.unpack`.
 
@@ -835,14 +853,17 @@
 *Method `UInt8.transcribe_value(value)`*:
 Transcribe a value back into bytes.
 
 # Release Log
 
 
 
+*Release 20240422*:
+New _BinaryMultiValue_Base.for_json() method returning a dict containing the fields.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
 BREAKING CHANGE: drop the long deprecated PacketField related classes.
 
 *Release 20231129*:
@@ -938,7 +959,8 @@
 * BytesField: implement value_s and from_buffer.
 * multi_struct_field: implement __len__ for generated class.
 * flatten: treat memoryviews like bytes.
 * Assorted docstrings and fixes.
 
 *Release 20180801*:
 Initial PyPI release.
+
```

### Comparing `cs.binary-20240316/lib/python/cs/binary.py` & `cs.binary-20240422/lib/python/cs/binary.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 from cs.buffer import CornuCopyBuffer
 from cs.deco import OBSOLETE, promote, strable
 from cs.gimmicks import warning, debug
 from cs.lex import cropped, cropped_repr, typed_str
 from cs.pfx import Pfx, pfx, pfx_method, pfx_call
 from cs.seq import Seq
 
-__version__ = '20240316'
+__version__ = '20240422'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Programming Language :: Python :: 3",
@@ -348,57 +348,54 @@
         This is to accomodate nonconformant streams
         without raising exceptions.
         Callers wanting to validate `max_count` may want to probe `bfr.at_eof()`
         after return.
         Callers not wanting a warning over `min_count` should not specify it,
         and instead check the number of instances returned themselves.
     '''
-    with Pfx("%s.scan", cls.__name__):
-      if count is None:
-        if min_count is None:
-          min_count = 0
-        else:
-          if min_count < 0:
-            raise ValueError(
-                "min_count must be >=0 if specified, got: %r" % (min_count,)
-            )
-        if max_count is not None:
-          if max_count < 0:
-            raise ValueError(
-                "max_count must be >=0 if specified, got: %r" % (max_count,)
-            )
-          if max_count < min_count:
-            raise ValueError(
-                "max_count must be >= min_count, got: min_count=%r, max_count=%rr"
-                % (min_count, max_count)
-            )
+    if count is None:
+      if min_count is None:
+        min_count = 0
       else:
-        if min_count is not None or max_count is not None:
+        if min_count < 0:
           raise ValueError(
-              "scan_with_offsets: may not combine count with either min_count or max_count"
+              "min_count must be >=0 if specified, got: %r" % (min_count,)
           )
-        if count < 0:
+      if max_count is not None:
+        if max_count < 0:
           raise ValueError(
-              "count must be >=0 if specified, got: %r" % (count,)
+              "max_count must be >=0 if specified, got: %r" % (max_count,)
           )
-        min_count = max_count = count
-      scanned = 0
-      while (max_count is None or scanned < max_count) and not bfr.at_eof():
-        pre_offset = bfr.offset
-        obj = cls.parse(bfr)
-        if with_offsets:
-          yield pre_offset, obj, bfr.offset
-        else:
-          yield obj
-        scanned += 1
-      if min_count is not None and scanned < min_count:
-        warning(
-            "fewer than min_count=%s instances scanned, only %d found",
-            min_count, scanned
+        if max_count < min_count:
+          raise ValueError(
+              "max_count must be >= min_count, got: min_count=%r, max_count=%rr"
+              % (min_count, max_count)
+          )
+    else:
+      if min_count is not None or max_count is not None:
+        raise ValueError(
+            "scan_with_offsets: may not combine count with either min_count or max_count"
         )
+      if count < 0:
+        raise ValueError("count must be >=0 if specified, got: %r" % (count,))
+      min_count = max_count = count
+    scanned = 0
+    while (max_count is None or scanned < max_count) and not bfr.at_eof():
+      pre_offset = bfr.offset
+      obj = cls.parse(bfr)
+      if with_offsets:
+        yield pre_offset, obj, bfr.offset
+      else:
+        yield obj
+      scanned += 1
+    if min_count is not None and scanned < min_count:
+      warning(
+          "fewer than min_count=%s instances scanned, only %d found",
+          min_count, scanned
+      )
 
   @classmethod
   @OBSOLETE(suggestion="BinaryMixin.scan")
   def scan_with_offsets(cls, bfr, count=None, min_count=None, max_count=None):
     ''' Wrapper for `scan()` which yields `(pre_offset,instance,post_offset)`
         indicating the start and end offsets of the yielded instances.
         All parameters are as for `scan()`.
@@ -1237,16 +1234,23 @@
             ),
             max_length=crop_length,
             roffset=0
         )
     )
 
   __str__ = _s
+
   ##__repr__ = _s
 
+  def for_json(self):
+    return {
+        field_name: getattr(self, field_name)
+        for field_name in self.FIELD_ORDER
+    }
+
   @classmethod
   def parse(cls, bfr):
     ''' Default parse: parse each predefined field from the buffer in order
         and set the associated attributes.
 
         Subclasses might override this if they have a flexible structure
         where not all fields necessarily appear.
```

