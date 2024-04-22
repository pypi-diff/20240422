# Comparing `tmp/cs.iso14496-20231129.tar.gz` & `tmp/cs.iso14496-20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.iso14496-20231129.tar", last modified: Wed Nov 29 11:03:55 2023, max compression
+gzip compressed data, was "cs.iso14496-20240422.tar", last modified: Mon Apr 22 06:42:27 2024, max compression
```

## Comparing `cs.iso14496-20231129.tar` & `cs.iso14496-20240422.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-11-29 11:03:55.309842 cs.iso14496-20231129/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-11-29 11:03:30.000000 cs.iso14496-20231129/MANIFEST.in
--rw-r--r--   0 cameron    (501) cameron    (502)    16955 2023-11-29 11:03:55.309576 cs.iso14496-20231129/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    27209 2023-11-29 11:03:35.000000 cs.iso14496-20231129/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-11-29 11:03:55.298677 cs.iso14496-20231129/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-11-29 11:03:55.299057 cs.iso14496-20231129/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-11-29 11:03:55.301802 cs.iso14496-20231129/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    85776 2023-11-29 11:03:17.000000 cs.iso14496-20231129/lib/python/cs/iso14496.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-11-29 11:03:55.308528 cs.iso14496-20231129/lib/python/cs.iso14496.egg-info/
--rw-r--r--   0 cameron    (501) cameron    (502)    16955 2023-11-29 11:03:55.000000 cs.iso14496-20231129/lib/python/cs.iso14496.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      310 2023-11-29 11:03:55.000000 cs.iso14496-20231129/lib/python/cs.iso14496.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-11-29 11:03:55.000000 cs.iso14496-20231129/lib/python/cs.iso14496.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      226 2023-11-29 11:03:55.000000 cs.iso14496-20231129/lib/python/cs.iso14496.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-11-29 11:03:55.000000 cs.iso14496-20231129/lib/python/cs.iso14496.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    17008 2023-11-29 11:03:45.000000 cs.iso14496-20231129/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1072 2023-11-29 11:03:55.310875 cs.iso14496-20231129/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-11-29 11:03:35.000000 cs.iso14496-20231129/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 06:42:27.693725 cs.iso14496-20240422/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 06:42:16.000000 cs.iso14496-20240422/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    26312 2024-04-22 06:42:27.693343 cs.iso14496-20240422/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    25531 2024-04-22 06:42:19.000000 cs.iso14496-20240422/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 06:42:27.689393 cs.iso14496-20240422/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 06:42:27.689658 cs.iso14496-20240422/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 06:42:27.690984 cs.iso14496-20240422/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    86848 2024-04-22 06:42:03.000000 cs.iso14496-20240422/lib/python/cs/iso14496.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 06:42:27.692884 cs.iso14496-20240422/lib/python/cs.iso14496.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    26312 2024-04-22 06:42:27.000000 cs.iso14496-20240422/lib/python/cs.iso14496.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      291 2024-04-22 06:42:27.000000 cs.iso14496-20240422/lib/python/cs.iso14496.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 06:42:27.000000 cs.iso14496-20240422/lib/python/cs.iso14496.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      290 2024-04-22 06:42:27.000000 cs.iso14496-20240422/lib/python/cs.iso14496.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 06:42:27.000000 cs.iso14496-20240422/lib/python/cs.iso14496.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    27045 2024-04-22 06:42:25.000000 cs.iso14496-20240422/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 06:42:27.693826 cs.iso14496-20240422/setup.cfg
```

### Comparing `cs.iso14496-20231129/README.md` & `cs.iso14496-20240422/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,58 @@
+Metadata-Version: 2.1
+Name: cs.iso14496
+Version: 20240422
+Summary: Facilities for ISO14496 files - the ISO Base Media File Format, the basis for several things including MP4 and MOV.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python3
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Multimedia :: Video
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
 Facilities for ISO14496 files - the ISO Base Media File Format,
 the basis for several things including MP4 and MOV.
 
-*Latest release 20231129*:
-Small updates and fixes.
+*Latest release 20240422*:
+* Replace dropped UTF16NULField with BinaryUTF16NUL.
+* Comment out unused CO64BoxBody.chunk_offsets, uses dropped (and not replaced) deferred_field.
+* Drop FallbackBoxBody, we'll just use BoxBody when there's no box specific subclass.
+* Replace pick_boxbody_class with BoxBody.for_box_type.
+* Rename boxbody_type_from_klass to boxbody_type_from_class.
+* Drop obsolete KNOWN_BOXBODY_CLASSES.
+* MP4Command.cmd_info: print moov.udta.meta.ilst.cover in SIXEL format on a terminal.
+* Rename parse_deref_path to get_deref_path like other lexical functions.
+* ILSTBoxBody.__getattr__: fix lookup of long names.
 
 ISO make the standard available here:
-* [link](http://standards.iso.org/ittf/PubliclyAvailableStandards/index.html)
-* [link](http://standards.iso.org/ittf/PubliclyAvailableStandards/c068960_ISO_IEC_14496-12_2015.zip)
-
-## Function `add_body_class(klass)`
-
-Register a box body class in KNOWN_BOXBODY_CLASSES.
+* [available standards main page](http://standards.iso.org/ittf/PubliclyAvailableStandards/index.html)
+* [zip file download](http://standards.iso.org/ittf/PubliclyAvailableStandards/c068960_ISO_IEC_14496-12_2015.zip)
 
 ## Function `add_body_subclass(superclass, box_type, section, desc)`
 
-Create and register a new BoxBody class that is simply a subclass of
-another.  Returns the new class.
+Create and register a new `BoxBody` class that is simply a subclass of
+another.
+Return the new class.
 
 ## Function `add_generic_sample_boxbody(box_type, section, desc, struct_format_v0, sample_fields, struct_format_v1=None, has_inferred_entry_count=False)`
 
 Create and add a specific Time to Sample box - section 8.6.1.
 
 ## Function `add_time_to_sample_boxbody(box_type, section, desc)`
 
 Add a Time to Sample box - section 8.6.1.
 
-## Class `Box(cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `Box(cs.binary.SimpleBinary)`
 
 Base class for all boxes - ISO14496 section 4.2.
 
 This has the following fields:
 * `header`: a `BoxHeader`
 * `body`: a `BoxBody` instance, usually a specific subclass
 * `unparsed`: any unconsumed bytes from the `Box` are stored as here
@@ -47,39 +70,39 @@
 but might be the samples if the body is a sample box,
 etc.
 
 *Method `Box.ancestor(self, box_type)`*:
 Return the closest ancestor box of type `box_type`.
 
 *Property `Box.box_type`*:
-The Box header type.
+The `Box` header type.
 
 *Property `Box.box_type_path`*:
 The type path to this Box.
 
 *Property `Box.box_type_s`*:
-The Box header type as a string.
+The `Box` header type as a string.
 
 If the header type bytes decode as ASCII, return that,
 otherwise the header bytes' repr().
 
 *Method `Box.dump(self, **kw)`*:
 Dump this Box.
 
 *Method `Box.gather_metadata(self)`*:
 Walk the `Box` hierarchy looking for metadata.
 Yield `(Box,TagSet)` for each `b'moov'` or `b'trak'` `Box`.
 
 *Method `Box.metatags(self)`*:
 Return a `TagSet` containing metadata for this box.
 
-*Method `Box.parse(bfr)`*:
-Decode a Box from `bfr` and return it.
+*Method `Box.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
+Decode a `Box` from `bfr` and return it.
 
-*Method `Box.parse_field(self, field_name, bfr, binary_cls)`*:
+*Method `Box.parse_field(self, field_name, bfr: cs.buffer.CornuCopyBuffer, binary_cls)`*:
 `parse_field` delegates to the `Box` body `parse_field`.
 
 *Property `Box.parse_length`*:
 The length of the box as consumed from the buffer,
 computed as `self.end_offset-self.offset`.
 
 *Method `Box.reparse_buffer(self)`*:
@@ -105,24 +128,24 @@
 
 *Property `Box.unparsed_bs`*:
 The unparsed data as a single `bytes` instance.
 
 *Property `Box.user_type`*:
 The header user_type.
 
-*Method `Box.walk(self)`*:
+*Method `Box.walk(self) -> Iterable[Tuple[ForwardRef('Box'), List[ForwardRef('Box')]]]`*:
 Walk this `Box` hierarchy.
 
 Yields the starting box and its children as `(self,subboxes)`
 and then yields `(subbox,subsubboxes)` for each child in turn.
 
 As with `os.walk`, the returned `subboxes` list
-may be modified to prune the subsequent walk.
+may be modified in place to prune or reorder the subsequent walk.
 
-## Class `BoxBody(cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `BoxBody(cs.binary.SimpleBinary)`
 
 Abstract basis for all `Box` bodies.
 
 *Method `BoxBody.__getattr__(self, attr)`*:
 The following virtual attributes are defined:
 * *TYPE*`s`:
   "boxes of type *TYPE*",
@@ -146,219 +169,228 @@
   If there are zero matches, return `None`.
   Otherwise return the matching box.
 
 *Method `BoxBody.add_field(self, field_name, value)`*:
 Add a field named `field_name` with the specified `value`
 to the box fields.
 
-*Method `BoxBody.boxbody_type_from_klass()`*:
+*Method `BoxBody.boxbody_type_from_class()`*:
 Compute the Box's 4 byte type field from the class name.
 
-*Method `BoxBody.parse(bfr)`*:
+*Method `BoxBody.for_box_type(box_type: bytes)`*:
+Return the `BoxBody` subclass suitable for the `box_type`.
+
+*Method `BoxBody.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Create a new instance and gather the `Box` body fields from `bfr`.
 
 Subclasses implement a `parse_fields` method to parse additional fields.
 
-*Method `BoxBody.parse_boxes(self, bfr, **kw)`*:
+*Method `BoxBody.parse_boxes(self, bfr: cs.buffer.CornuCopyBuffer, **kw)`*:
 Utility method to parse the remainder of the buffer as a
 sequence of `Box`es.
 
-*Method `BoxBody.parse_field(self, field_name, bfr, binary_cls)`*:
+*Method `BoxBody.parse_field(self, field_name, bfr: cs.buffer.CornuCopyBuffer, binary_cls)`*:
 Parse an instance of `binary_cls` from `bfr`
 and store it as the attribute named `field_name`.
 
 `binary_cls` may also be an `int`, in which case that many
 bytes are read from `bfr`.
 
-*Method `BoxBody.parse_field_value(self, field_name, bfr, binary_cls)`*:
+*Method `BoxBody.parse_field_value(self, field_name, bfr: cs.buffer.CornuCopyBuffer, binary_cls)`*:
 Parse a single value binary, store the value as `field_name`,
 store the instance as the field `field_name+'__Binary'`
 for transcription.
 
 Note that this disassociaes the plain value attribute
 from what gets transcribed.
 
-*Method `BoxBody.parse_fields(self, bfr)`*:
+*Method `BoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse additional fields.
 This base class implementation consumes nothing.
 
 *Method `BoxBody.transcribe(self)`*:
 Transcribe the binary structure.
 
 This default implementation transcribes the fields parsed with the
 `parse_field` method in the order parsed.
 
 *Method `BoxBody.transcribe_fields(self)`*:
 Transcribe the fields parsed with the `parse_field` method in the
 order parsed.
 
-## Class `BoxHeader(cs.binary.BoxHeader, cs.binary._BinaryMultiValue_Base, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `BoxHeader(cs.binary.BoxHeader)`
 
-An ISO14496 Box header packet.
+An ISO14496 `Box` header packet.
 
-*Method `BoxHeader.parse(bfr)`*:
+*Method `BoxHeader.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Decode a box header from `bfr`.
 
-## Class `BTRTBoxBody(BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `BTRTBoxBody(BoxBody)`
 
 BitRateBoxBody - section 8.5.2.2.
 
-*Method `BTRTBoxBody.parse_fields(self, bfr)`*:
+*Method `BTRTBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `bufferSizeDB`, `maxBitrate` and `avgBitrate` fields.
 
-## Class `CO64BoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `CO64BoxBody(FullBoxBody)`
 
 A 'c064' Chunk Offset box - section 8.7.5.
 
-*Property `CO64BoxBody.chunk_offsets`*:
-Boilerplate for the property: test for parsed value, parse
-from raw data if not yet present.
-
-*Method `CO64BoxBody.parse_fields(self, bfr)`*:
+*Method `CO64BoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `entry_count` and `chunk_offsets` fields.
 
 *Method `CO64BoxBody.transcribe(self)`*:
 Transcribe a `CO64BoxBody`.
 
-## Class `ContainerBoxBody(BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `ContainerBoxBody(BoxBody)`
 
 Common subclass of several things with `.boxes`.
 
-## Class `CPRTBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `CPRTBoxBody(FullBoxBody)`
 
 A 'cprt' Copyright box - section 8.10.2.
 
 *Property `CPRTBoxBody.language`*:
 The `language_field` as the 3 character ISO 639-2/T language code.
 
-*Method `CPRTBoxBody.parse_fields(self, bfr)`*:
+*Method `CPRTBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `language` and `notice` fields.
 
-## Class `CSLGBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `CSLGBoxBody(FullBoxBody)`
 
 A 'cslg' Composition to Decode box - section 8.6.1.4.
 
 *`CSLGBoxBody.CSLGParamsLong`*
 
 *`CSLGBoxBody.CSLGParamsQuad`*
 
 *Method `CSLGBoxBody.__getattr__(self, attr)`*:
 Present the `params` attributes at the top level.
 
-*Method `CSLGBoxBody.parse_fields(self, bfr)`*:
+*Method `CSLGBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the compositionToDTSShift`, `leastDecodeToDisplayDelta`,
 `greatestDecodeToDisplayDelta`, `compositionStartTime` and
 `compositionEndTime` fields.
 
-## Function `decode_itunes_date_field(data)`
+## Function `decode_itunes_date_field(data) -> datetime.datetime`
 
 The iTunes 'Date' meta field: a year or an ISO timestamp.
 
 ## Function `deref_box(B, path)`
 
 Dereference a path with respect to this Box.
 
-## Class `DREFBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `DREFBoxBody(FullBoxBody)`
 
 A 'dref' Data Reference box containing Data Entry boxes - section 8.7.2.1.
 
-*Method `DREFBoxBody.parse_fields(self, bfr)`*:
+*Method `DREFBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `entry_count` and `boxes` fields.
 
 ## Function `dump_box(B, indent='', fp=None, crop_length=170, indent_incr=None)`
 
 Recursively dump a Box.
 
-## Class `ELNGBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `ELNGBoxBody(FullBoxBody)`
 
 A ELNGBoxBody is a Extended Language Tag box - ISO14496 section 8.4.6.
 
-*Method `ELNGBoxBody.parse_fields(self, bfr)`*:
+*Method `ELNGBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `extended_language` field.
 
-## Class `ELSTBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `ELSTBoxBody(FullBoxBody)`
 
 An 'elst' Edit List FullBoxBody - section 8.6.6.
 
 *`ELSTBoxBody.V0EditEntry`*
 
 *`ELSTBoxBody.V1EditEntry`*
 
 *Property `ELSTBoxBody.entry_class`*:
 The class representing each entry.
 
 *Property `ELSTBoxBody.entry_count`*:
 The number of entries.
 
-*Method `ELSTBoxBody.parse_fields(self, bfr)`*:
+*Method `ELSTBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse the fields of an `ELSTBoxBody`.
 
 *Method `ELSTBoxBody.transcribe(self)`*:
 Transcribe an `ELSTBoxBody`.
 
-## Class `FallbackBoxBody(BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
-
-A `BoxBody` subclass which parses nothing for unimplemented `Box` types,
-used by `pick_boxbody_class()`.
-
-## Class `FREEBoxBody(BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `FREEBoxBody(BoxBody)`
 
 A 'free' or 'skip' box - ISO14496 section 8.1.2.
 Note the length and discard the data portion.
 
-*Method `FREEBoxBody.parse_fields(self, bfr, end_offset=Ellipsis, **kw)`*:
+*Method `FREEBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer, end_offset=Ellipsis, **kw)`*:
 Gather the `padding` field.
 
-## Class `FTYPBoxBody(BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `FTYPBoxBody(BoxBody)`
 
 An 'ftyp' File Type box - ISO14496 section 4.3.
 Decode the major_brand, minor_version and compatible_brands.
 
 *Property `FTYPBoxBody.compatible_brands`*:
 The compatible brands as a list of 4 byte bytes instances.
 
-*Method `FTYPBoxBody.parse_fields(self, bfr, **kw)`*:
+*Method `FTYPBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer, **kw)`*:
 Gather the `major_brand`, `minor_version` and `brand_bs` fields.
 
-## Class `FullBoxBody(BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `FullBoxBody(BoxBody)`
 
 A common extension of a basic BoxBody, with a version and flags field.
 ISO14496 section 4.2.
 
 *Property `FullBoxBody.flags`*:
 The flags value, computed from the 3 flag bytes.
 
-## Class `HDLRBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Function `get_deref_path(path, offset=0)`
+
+Parse a `path` string from `offset`.
+Return the path components and the offset where the parse stopped.
+
+Path components:
+* _identifier_: an identifier represents a `Box` field or if such a
+  field is not present, a the first subbox of this type
+* `[`_index_`]`: the subbox with index _index_
+
+Examples:
+
+    >>> get_deref_path('.abcd[5]')
+    (['abcd', 5], 8)
+
+## Class `HDLRBoxBody(FullBoxBody)`
 
 A HDLRBoxBody is a Handler Reference box - ISO14496 section 8.4.3.
 
 *Property `HDLRBoxBody.handler_type`*:
 The handler_type as an ASCII string, its usual form.
 
-*Method `HDLRBoxBody.parse_fields(self, bfr)`*:
+*Method `HDLRBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `handler_type_long` and `name` fields.
 
 ## Function `ILSTAofBSchema(attribute_name)`
 
 Attribute name and type for ILST "A of B" schema.
 
-## Class `ILSTBoxBody(ContainerBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `ILSTBoxBody(ContainerBoxBody)`
 
 Apple iTunes Information List, container for iTunes metadata fields.
 
 The basis of the format knowledge here comes from AtomicParsley's
 documentation here:
 
     http://atomicparsley.sourceforge.net/mpeg-4files.html
 
 and additional information from:
 
     https://github.com/sergiomb2/libmp4v2/wiki/iTunesMetadata
 
-*Method `ILSTBoxBody.parse_fields(self, bfr)`*:
+*Method `ILSTBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 pylint: disable=attribute-defined-outside-init,too-many-locals
 pylint: disable=too-many-statements,too-many-branches
 
 ## Function `ILSTISOFormatSchema(attribute_name)`
 
 Attribute name and type for ILST ISO format schema.
 
@@ -368,19 +400,19 @@
 
 ## Function `ILSTTextSchema(attribute_name)`
 
 Attribute name and type for ILST text schema.
 
 ## Function `ILSTUInt32BESchema(attribute_name)`
 
-Attribute name and type for ILST UInt32BE schema.
+Attribute name and type for ILST `UInt32BE` schema.
 
 ## Function `ILSTUInt8Schema(attribute_name)`
 
-Attribute name and type for ILST UInt8BE schema.
+Attribute name and type for ILST `UInt8BE` schema.
 
 ## Class `itunes_media_type(builtins.tuple)`
 
 itunes_media_type(type, stik)
 
 *Property `itunes_media_type.stik`*:
 Alias for field number 1
@@ -401,131 +433,135 @@
 *Property `itunes_store_country_code.itunes_store_code`*:
 Alias for field number 2
 
 ## Function `main(argv=None)`
 
 Command line mode.
 
-## Class `MDATBoxBody(BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `MDATBoxBody(BoxBody)`
 
 A Media Data Box - ISO14496 section 8.1.1.
 
-*Method `MDATBoxBody.parse_fields(self, bfr)`*:
+*Method `MDATBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather all data to the end of the field.
 
 *Method `MDATBoxBody.transcribe(self)`*:
 Transcribe the data.
 Raise an `AssertionError` if we skipped the data during the parse.
 
 *Method `MDATBoxBody.transcribed_length(self)`*:
 Return the transcription length even if we didn't keep the data.
 
-## Class `MDHDBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `MDHDBoxBody(FullBoxBody)`
 
 A MDHDBoxBody is a Media Header box - ISO14496 section 8.4.2.
 
-*Method `MDHDBoxBody.parse_fields(self, bfr)`*:
+*Method `MDHDBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `creation_time`, `modification_time`, `timescale`,
 `duration` and `language_short` fields.
 
-## Class `METABoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `METABoxBody(FullBoxBody)`
 
 A 'meta' Meta BoxBody - section 8.11.1.
 
 *Method `METABoxBody.__getattr__(self, attr)`*:
 Present the `ilst` attributes if present.
 
-*Method `METABoxBody.parse_fields(self, bfr)`*:
-Gather the `theHandler` Box and gather the following Boxes as `boxes`.
+*Method `METABoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
+Gather the `theHandler` `Box` and gather the following Boxes as `boxes`.
 
-## Class `MOOVBoxBody(ContainerBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `MOOVBoxBody(ContainerBoxBody)`
 
 An 'moov' Movie box - ISO14496 section 8.2.1.
 Decode the contained boxes.
 
 ## Class `MP4Command(cs.cmdutils.BaseCommand)`
 
-Command line usage:
+Command line implementation.
+
+Usage summary:
 
-Usage: mp4 subcommand [...]
-  Subcommands:
-    autotag autotag [-n] [-p prefix] [--prefix=prefix] paths...
-      Tag paths based on embedded MP4 metadata.
-      -n  No action.
-      -p prefix, --prefix=prefix
-          Set the prefix of added tags, default: 'mp4'
-    deref ...
-        Dereference a Box specification against ISO14496 files.
-    extract extract [-H] filename boxref output
-      Extract the referenced Box from the specified filename into output.
-      -H  Skip the Box header.
-    help [-l] [subcommand-names...]
-      Print the full help for the named subcommands,
-      or for all subcommands if no names are specified.
-      -l  Long help even if no subcommand-names provided.
-    info info [{-|filename}]...]
-      Print informative report about each source.
-    parse [parse [{-|filename}]...]
-      Parse the named files (or stdin for "-").
-    shell
-      Run a command prompt via cmd.Cmd using this command's subcommands.
-    tags path
-      Report the tags of `path` based on embedded MP4 metadata.
-    test [testnames...]
-      Run self tests.
+    Usage: mp4 subcommand [...]
+      Subcommands:
+        autotag [-n] [-p prefix] [--prefix=prefix] paths...
+          Tag paths based on embedded MP4 metadata.
+          -n  No action.
+          -p prefix, --prefix=prefix
+              Set the prefix of added tags, default: 'mp4'
+        deref boxspec paths...
+          Dereference a Box specification against ISO14496 files.
+        extract [-H] filename boxref output
+          Extract the referenced Box from the specified filename into output.
+          -H  Skip the Box header.
+        help [-l] [subcommand-names...]
+          Print help for subcommands.
+          This outputs the full help for the named subcommands,
+          or the short help for all subcommands if no names are specified.
+          -l  Long help even if no subcommand-names provided.
+        info [{-|filename}]...]
+          Print informative report about each source.
+        parse [{-|filename}...]
+          Parse the named files (or stdin for "-").
+        shell
+          Run a command prompt via cmd.Cmd using this command's subcommands.
+        tags [{-p,--prefix} prefix] path
+          Report the tags of `path` based on embedded MP4 metadata.
+        test [testnames...]
+          Run self tests.
 
-*Method `MP4Command.cmd_autotag(self, argv, fstags)`*:
-Usage: {cmd} autotag [-n] [-p prefix] [--prefix=prefix] paths...
+*Method `MP4Command.cmd_autotag(self, argv, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x108080040>)`*:
+Usage: {cmd} [-n] [-p prefix] [--prefix=prefix] paths...
 Tag paths based on embedded MP4 metadata.
 -n  No action.
 -p prefix, --prefix=prefix
     Set the prefix of added tags, default: 'mp4'
 
 *Method `MP4Command.cmd_deref(self, argv)`*:
+Usage: {cmd} boxspec paths...
 Dereference a Box specification against ISO14496 files.
 
 *Method `MP4Command.cmd_extract(self, argv)`*:
-Usage: {cmd} extract [-H] filename boxref output
+Usage: {cmd} [-H] filename boxref output
 Extract the referenced Box from the specified filename into output.
 -H  Skip the Box header.
 
 *Method `MP4Command.cmd_info(self, argv)`*:
-Usage: {cmd} info [{{-|filename}}]...]
+Usage: {cmd} [{{-|filename}}]...]
 Print informative report about each source.
 
 *Method `MP4Command.cmd_parse(self, argv)`*:
-Usage: {cmd} [parse [{{-|filename}}]...]
+Usage: {cmd} [{{-|filename}}...]
 Parse the named files (or stdin for "-").
 
 *Method `MP4Command.cmd_tags(self, argv)`*:
-Usage: {cmd} path
+Usage: {cmd} [{{-p,--prefix}} prefix] path
 Report the tags of `path` based on embedded MP4 metadata.
 
 *Method `MP4Command.cmd_test(self, argv)`*:
 Usage: {cmd} [testnames...]
 Run self tests.
 
-## Class `MVHDBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `MVHDBoxBody(FullBoxBody)`
 
 An 'mvhd' Movie Header box - ISO14496 section 8.2.2.
 
-## Class `OverBox(cs.binary.BinaryListValues, cs.binary.AbstractBinary, cs.binary.BinaryMixin, HasBoxesMixin)`
+## Class `OverBox(cs.binary.BinaryListValues, HasBoxesMixin)`
 
 A fictitious `Box` encompassing all the Boxes in an input buffer.
 
 *Property `OverBox.boxes`*:
 Alias `.value` as `.boxes`: the `Box`es encompassed by this `OverBox`.
 
 *Method `OverBox.dump(self, **kw)`*:
 Dump this OverBox.
 
 *Property `OverBox.length`*:
 The `OverBox` is as long as the subsidary Boxes.
 
-*Method `OverBox.parse(bfr)`*:
+*Method `OverBox.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Parse the `OverBox`.
 
 *Method `OverBox.walk(self)`*:
 Walk the `Box`es in the `OverBox`.
 
 This does not yield the `OverBox` itself, it isn't really a `Box`.
 
@@ -538,212 +574,203 @@
 * `int`: a OS file descriptor
 * `bytes`: a `bytes` object
 * `file`: if not `int` or `str` the presumption
   is that this is a file-like object
 
 Keyword arguments are as for `OverBox.from_buffer`.
 
-## Function `parse_deref_path(path, offset=0)`
-
-Parse a `path` string from `offset`.
-Return the path components and the offset where the parse stopped.
-
-Path components:
-* _identifier_: an identifier represents a Box field or if such a
-  field is not present, a the first subbox of this type
-* `[`_index_`]`: the subbox with index _index_
-
-Examples:
-
-    >>> parse_deref_path('.abcd[5]')
-    ['abcd', 5]
-
 ## Function `parse_fields(bfr, copy_offsets=None, **kw)`
 
 Parse an ISO14496 stream from the CornuCopyBuffer `bfr`,
 yield top level OverBoxes.
 
 Parameters:
 * `bfr`: a `CornuCopyBuffer` provided the stream data,
   preferably seekable
 * `discard_data`: whether to discard unparsed data, default `False`
-* `copy_offsets`: callable to receive Box offsets
+* `copy_offsets`: callable to receive `Box` offsets
 
 ## Function `parse_tags(path, tag_prefix=None)`
 
 Parse the tags from `path`.
 Yield `(box,tags)` for each subbox with tags.
 
 The optional `tag_prefix` parameter
 may be specified to prefix each tag name with a prefix.
 Other keyword arguments are passed to `parse()`
 (typical example: `discard_data=True`).
 
-## Class `PDINBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `PDINBoxBody(FullBoxBody)`
 
 A 'pdin' Progressive Download Information box - ISO14496 section 8.1.3.
 
 *`PDINBoxBody.PDInfo`*
 
-*Method `PDINBoxBody.parse_fields(self, bfr, **kw)`*:
+*Method `PDINBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer, **kw)`*:
 Gather the normal version information
 and then the `(rate,initial_delay)` pairs of the data section
 as the `pdinfo` field.
 
-## Function `pick_boxbody_class(box_type: bytes)`
-
-Infer a `BoxBody` subclass from the 4-byte bytes `box_type`.
-Returns `FallbackBoxBody` for unimplemented types.
-
 ## Function `report(box, indent='', fp=None, indent_incr=None)`
 
 Report some human friendly information about a box.
 
-## Class `SMHDBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `SMHDBoxBody(FullBoxBody)`
 
 A 'smhd' Sound Media Headerbox - section 12.2.2.
 
-*Method `SMHDBoxBody.parse_fields(self, bfr)`*:
+*Method `SMHDBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `balance` field.
 
-## Class `STCOBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `STCOBoxBody(FullBoxBody)`
 
 A 'stco' Chunk Offset box - section 8.7.5.
 
 *Property `STCOBoxBody.chunk_offsets`*:
 Parse the `UInt32BE` chunk offsets from stashed buffer.
 
-*Method `STCOBoxBody.parse_fields(self, bfr)`*:
+*Method `STCOBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `entry_count` and `chunk_offsets` fields.
 
-## Class `STSCBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `STSCBoxBody(FullBoxBody)`
 
 'stsc' (Sample Table box - section 8.7.4.1.
 
 *`STSCBoxBody.STSCEntry`*
 
 *Property `STSCBoxBody.entries`*:
-Parse the `STSCEntry` list into a list of `int`s.
+A list of `int`s parsed from the `STSCEntry` list.
 
-*Method `STSCBoxBody.parse_fields(self, bfr)`*:
+*Method `STSCBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `entry_count` and `entries` fields.
 
-## Class `STSZBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `STSZBoxBody(FullBoxBody)`
 
 A 'stsz' Sample Size box - section 8.7.3.2.
 
 *Property `STSZBoxBody.entry_sizes`*:
 Parse the `UInt32BE` entry sizes from stashed buffer
 into a list of `int`s.
 
-*Method `STSZBoxBody.parse_fields(self, bfr)`*:
+*Method `STSZBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `sample_size`, `sample_count`, and `entry_sizes` fields.
 
 *Method `STSZBoxBody.transcribe(self)`*:
 Transcribe the `STSZBoxBody`.
 
-## Class `STZ2BoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `STZ2BoxBody(FullBoxBody)`
 
 A 'stz2' Compact Sample Size box - section 8.7.3.3.
 
-*Method `STZ2BoxBody.parse_fields(self, bfr)`*:
+*Method `STZ2BoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `field_size`, `sample_count` and `entry_sizes` fields.
 
 *Method `STZ2BoxBody.transcribe(self)`*:
 transcribe the STZ2BoxBody.
 
-## Class `TimeStamp32(cs.binary.UInt32BE, cs.binary.UInt32BE, builtins.tuple, cs.binary.AbstractBinary, cs.binary.BinaryMixin, TimeStampMixin)`
+## Class `TimeStamp32(cs.binary.UInt32BE, TimeStampMixin)`
 
 The 32 bit form of an ISO14496 timestamp.
 
-## Class `TimeStamp64(cs.binary.UInt64BE, cs.binary.UInt64BE, builtins.tuple, cs.binary.AbstractBinary, cs.binary.BinaryMixin, TimeStampMixin)`
+## Class `TimeStamp64(cs.binary.UInt64BE, TimeStampMixin)`
 
 The 64 bit form of an ISO14496 timestamp.
 
 ## Class `TimeStampMixin`
 
 Methods to assist with ISO14496 timestamps.
 
 *Property `TimeStampMixin.datetime`*:
 This timestamp as an UTC datetime.
 
 *Property `TimeStampMixin.unixtime`*:
 This timestamp as a UNIX time (seconds since 1 January 1970).
 
-## Class `TKHDBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `TKHDBoxBody(FullBoxBody)`
 
 A 'tkhd' Track Header box - ISO14496 section 8.2.2.
 
 *`TKHDBoxBody.TKHDMatrix`*
 
-## Class `TrackGroupTypeBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `TrackGroupTypeBoxBody(FullBoxBody)`
 
 A TrackGroupTypeBoxBody contains a track group id - ISO14496 section 8.3.3.2.
 
-*Method `TrackGroupTypeBoxBody.parse_fields(self, bfr)`*:
+*Method `TrackGroupTypeBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `track_group_id` field.
 
-## Class `TrackReferenceTypeBoxBody(BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `TrackReferenceTypeBoxBody(BoxBody)`
 
 A TrackReferenceTypeBoxBody contains references to other tracks - ISO14496 section 8.3.3.2.
 
-*Method `TrackReferenceTypeBoxBody.parse_fields(self, bfr)`*:
+*Method `TrackReferenceTypeBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `track_ids` field.
 
-## Class `TREFBoxBody(ContainerBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `TREFBoxBody(ContainerBoxBody)`
 
 Track Reference BoxBody, container for trackReferenceTypeBoxes - ISO14496 section 8.3.3.
 
 ## Class `TTSB_Sample(builtins.tuple)`
 
 TTSB_Sample(count, delta)
 
 *Property `TTSB_Sample.count`*:
 Alias for field number 0
 
 *Property `TTSB_Sample.delta`*:
 Alias for field number 1
 
-## Class `URL_BoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `URL_BoxBody(FullBoxBody)`
 
 An 'url ' Data Entry URL BoxBody - section 8.7.2.1.
 
-*Method `URL_BoxBody.parse_fields(self, bfr)`*:
+*Method `URL_BoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `location` field.
 
-## Class `URN_BoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `URN_BoxBody(FullBoxBody)`
 
 An 'urn ' Data Entry URL BoxBody - section 8.7.2.1.
 
-*Method `URN_BoxBody.parse_fields(self, bfr)`*:
+*Method `URN_BoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `name` and `location` fields.
 
-## Class `UTF8or16Field(cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `UTF8or16Field(cs.binary.SimpleBinary)`
 
 An ISO14496 UTF8 or UTF16 encoded string.
 
-*Method `UTF8or16Field.parse(bfr)`*:
+*Method `UTF8or16Field.parse(bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather optional BOM and then UTF8 or UTF16 string.
 
 *Method `UTF8or16Field.transcribe(self)`*:
 Transcribe the field suitably encoded.
 
-## Class `VMHDBoxBody(FullBoxBody, BoxBody, cs.binary.SimpleBinary, types.SimpleNamespace, cs.binary.AbstractBinary, cs.binary.BinaryMixin)`
+## Class `VMHDBoxBody(FullBoxBody)`
 
 A 'vmhd' Video Media Headerbox - section 12.1.2.
 
 *`VMHDBoxBody.OpColor`*
 
-*Method `VMHDBoxBody.parse_fields(self, bfr)`*:
+*Method `VMHDBoxBody.parse_fields(self, bfr: cs.buffer.CornuCopyBuffer)`*:
 Gather the `graphicsmode` and `opcolor` fields.
 
 # Release Log
 
 
 
+*Release 20240422*:
+* Replace dropped UTF16NULField with BinaryUTF16NUL.
+* Comment out unused CO64BoxBody.chunk_offsets, uses dropped (and not replaced) deferred_field.
+* Drop FallbackBoxBody, we'll just use BoxBody when there's no box specific subclass.
+* Replace pick_boxbody_class with BoxBody.for_box_type.
+* Rename boxbody_type_from_klass to boxbody_type_from_class.
+* Drop obsolete KNOWN_BOXBODY_CLASSES.
+* MP4Command.cmd_info: print moov.udta.meta.ilst.cover in SIXEL format on a terminal.
+* Rename parse_deref_path to get_deref_path like other lexical functions.
+* ILSTBoxBody.__getattr__: fix lookup of long names.
+
 *Release 20231129*:
 Small updates and fixes.
 
 *Release 20230212*:
 * Drop cs.context.StackableState in favour of cs.threads.State.
 * MP4Command.cmd_autotag: use @uses_fstags for the fstags parameter.
 
@@ -780,7 +807,8 @@
 
 *Release 20180810*:
 * parse_fd(): use a mmap to access the descriptor if a regular file and not discard_data;
 * this lets us use the mmapped file as backing store for the data, a big win for the media sections.
 
 *Release 20180805*:
 Initial PyPI release.
+
```

### Comparing `cs.iso14496-20231129/lib/python/cs/iso14496.py` & `cs.iso14496-20240422/lib/python/cs/iso14496.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,81 +4,88 @@
 #
 
 '''
 Facilities for ISO14496 files - the ISO Base Media File Format,
 the basis for several things including MP4 and MOV.
 
 ISO make the standard available here:
-* [link](http://standards.iso.org/ittf/PubliclyAvailableStandards/index.html)
-* [link](http://standards.iso.org/ittf/PubliclyAvailableStandards/c068960_ISO_IEC_14496-12_2015.zip)
+* [available standards main page](http://standards.iso.org/ittf/PubliclyAvailableStandards/index.html)
+* [zip file download](http://standards.iso.org/ittf/PubliclyAvailableStandards/c068960_ISO_IEC_14496-12_2015.zip)
 '''
 
-from abc import ABC
 from base64 import b64encode, b64decode
 from collections import namedtuple
 from contextlib import contextmanager
 from datetime import datetime
 from getopt import getopt, GetoptError
 import os
 import sys
+from typing import Iterable, List, Tuple
+
+from icontract import require
+from typeguard import typechecked
 
 from cs.binary import (
     UInt8,
     Int16BE,
-    UTF16NULField,
     Int32BE,
     UInt16BE,
     UInt32BE,
     UInt64BE,
     BinaryUTF8NUL,
     BinaryUTF16NUL,
     SimpleBinary,
     BinaryListValues,
     BinaryMultiStruct,
     BinaryMultiValue,
     BinarySingleValue,
-    deferred_field,
     pt_spec,
 )
 from cs.buffer import CornuCopyBuffer
 from cs.cmdutils import BaseCommand
-from cs.fstags import FSTags, rpaths, uses_fstags
-from cs.lex import get_identifier, get_decimal_value, cropped_repr
+from cs.fs import scandirpaths
+from cs.fstags import FSTags, uses_fstags
+from cs.imageutils import sixel_from_image_bytes
+from cs.lex import get_identifier, get_decimal_value
 from cs.logutils import warning
 from cs.pfx import Pfx, pfx_method, XP
 from cs.py.func import prop
 from cs.tagset import TagSet, Tag
 from cs.threads import locked_property, ThreadState
 from cs.units import transcribe_bytes_geek as geek, transcribe_time
 from cs.upd import print, out  # pylint: disable=redefined-builtin
 
-__version__ = '20231129'
+__version__ = '20240422'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Topic :: Multimedia :: Video",
     ],
     'install_requires': [
         'cs.binary',
         'cs.buffer',
         'cs.cmdutils',
+        'cs.fs',
         'cs.fstags',
+        'cs.imageutils',
         'cs.lex',
         'cs.logutils',
         'cs.pfx',
         'cs.py.func',
         'cs.tagset',
         'cs.threads',
         'cs.units',
         'cs.upd',
+        'icontract',
+        'typeguard',
     ],
 }
 
 PARSE_MODE = ThreadState(copy_boxes=False, discard_data=False)
 
 def main(argv=None):
   ''' Command line mode.
@@ -88,61 +95,61 @@
 class MP4Command(BaseCommand):
 
   GETOPT_SPEC = ''
 
   TAG_PREFIX = 'mp4'
 
   @uses_fstags
-  def cmd_autotag(self, argv, fstags):
-    ''' Usage: {cmd} autotag [-n] [-p prefix] [--prefix=prefix] paths...
+  def cmd_autotag(self, argv, fstags: FSTags):
+    ''' Usage: {cmd} [-n] [-p prefix] [--prefix=prefix] paths...
           Tag paths based on embedded MP4 metadata.
           -n  No action.
           -p prefix, --prefix=prefix
               Set the prefix of added tags, default: 'mp4'
     '''
-    xit = 0
-    no_action = False
-    tag_prefix = self.TAG_PREFIX
-    opts, argv = getopt(argv, 'np:', longopts=['prefix'])
-    for option, value in opts:
-      with Pfx(option):
-        if option == '-n':
-          no_action = True
-        elif option in ('-p', '--prefix'):
-          tag_prefix = value
-        else:
-          raise RuntimeError("unsupported option")
+    options = self.options
+    options.tag_prefix = self.TAG_PREFIX
+    options.popopts(
+        argv,
+        p_=(
+            'tag_prefix',
+            f'prefix to the applied tags, default "{self.TAG_PREFIX}."'
+        ),
+        prefix_=(
+            'tag_prefix',
+            f'prefix to the applied tags, default "{self.TAG_PREFIX}."'
+        ),
+    )
+    doit = options.doit
+    tag_prefix = options.tag_prefix
+    verbose = options.verbose or not options.doit
     if not argv:
       argv = [os.getcwd()]
+    xit = 0
     with fstags:
       for top_path in argv:
-        for _, path in rpaths(top_path):
+        for path in scandirpaths(top_path):
           out(path)
           with Pfx(path):
             tagged_path = fstags[path]
             with PARSE_MODE(discard_data=True):
-              try:
-                for box, tags in parse_tags(path, tag_prefix=tag_prefix):
-                  for tag in tags:
-                    if no_action:
-                      tag_s = str(tag)
-                      if len(tag_s) > 32:
-                        tag_s = tag_s[:29] + '...'
-                      print(path, '+', tag_s)
-                    else:
-                      tagged_path.add(tag)
-              except (TypeError, NameError, AttributeError, AssertionError):
-                raise
-              except Exception as e:
-                warning("%s: %s", type(e).__name__, e)
-                xit = 1
+              for _, tags in parse_tags(path, tag_prefix=tag_prefix):
+                for tag in tags:
+                  if verbose:
+                    tag_s = str(tag)
+                    if len(tag_s) > 64:
+                      tag_s = tag_s[:61] + '...'
+                    print(path, '+', tag_s)
+                  if doit:
+                    tagged_path.add(tag)
     return xit
 
   def cmd_deref(self, argv):
-    ''' Dereference a Box specification against ISO14496 files.
+    ''' Usage: {cmd} boxspec paths...
+          Dereference a Box specification against ISO14496 files.
     '''
     spec = argv.pop(0)
     with Pfx(spec):
       if spec == '-':
         parsee = sys.stdin.fileno()
       else:
         parsee = spec
@@ -150,15 +157,15 @@
       over_box.dump()
       for path in argv:
         with Pfx(path):
           B = deref_box(over_box, path)
           print(path, "offset=%d" % B.offset, B)
 
   def cmd_extract(self, argv):
-    ''' Usage: {cmd} extract [-H] filename boxref output
+    ''' Usage: {cmd} [-H] filename boxref output
           Extract the referenced Box from the specified filename into output.
           -H  Skip the Box header.
     '''
     skip_header = False
     if argv and argv[0] == '-H':
       argv.pop(0)
       skip_header = True
@@ -203,40 +210,55 @@
             if need is not None and need < len(chunk):
               chunk = chunk[need]
             ofp.write(chunk)
             need -= len(chunk)
       os.close(fd)
 
   def cmd_info(self, argv):
-    ''' Usage: {cmd} info [{{-|filename}}]...]
+    ''' Usage: {cmd} [{{-|filename}}]...]
           Print informative report about each source.
     '''
     if not argv:
       argv = ['-']
+    xit = 0
     for spec in argv:
       with Pfx(spec):
         if spec == '-':
           parsee = sys.stdin.fileno()
         else:
           parsee = spec
         with PARSE_MODE(discard_data=True):
           over_box = parse(parsee)
         print(spec + ":")
         for top_box in over_box:
           for box, tags in top_box.gather_metadata():
             if tags:
               print(' ', box.box_type_path, str(len(tags)) + ':')
               for tag in tags:
-                if tag.name == 'moov.udta.meta.ilst.cover':
-                  print('   ', tag.name, cropped_repr(tag.value))
-                else:
-                  print('   ', tag, repr(tag.value))
+                with Pfx(tag.name):
+                  if tag.name == 'moov.udta.meta.ilst.cover':
+                    image_bs = b64decode(tag.value)
+                    if sys.stdout.isatty():
+                      print(f'    {tag.name}:')
+                      with open(sixel_from_image_bytes(image_bs),
+                                'rb') as sixelf:
+                        print(sixelf.read().decode('ascii'))
+                    else:
+                      print(f'    {tag.name}: {image_bs[:32]!r}...')
+                  else:
+                    try:
+                      print('   ', tag)
+                    except TypeError as e:
+                      warning("cannot print: %s", e)
+                      xit = 1
+                      print('   ', tag.name, '=', repr(tag.value))
+    return xit
 
   def cmd_parse(self, argv):
-    ''' Usage: {cmd} [parse [{{-|filename}}]...]
+    ''' Usage: {cmd} [{{-|filename}}...]
           Parse the named files (or stdin for "-").
     '''
     if not argv:
       argv = ['-']
     for spec in argv:
       with Pfx(spec):
         if spec == '-':
@@ -244,15 +266,15 @@
         else:
           parsee = spec
         with PARSE_MODE(discard_data=True):
           over_box = parse(parsee)
         over_box.dump(crop_length=None)
 
   def cmd_tags(self, argv):
-    ''' Usage: {cmd} path
+    ''' Usage: {cmd} [{{-p,--prefix}} prefix] path
           Report the tags of `path` based on embedded MP4 metadata.
     '''
     xit = 0
     fstags = FSTags()
     tag_prefix = self.TAG_PREFIX
     opts, argv = getopt(argv, 'p:', longopts=['prefix'])
     for option, value in opts:
@@ -266,15 +288,15 @@
     path = argv.pop(0)
     if argv:
       raise GetoptError("extra arguments after path: %r" % (argv,))
     with fstags:
       out(path)
       with Pfx(path):
         with PARSE_MODE(discard_data=True):
-          for box, tags in parse_tags(path, tag_prefix=tag_prefix):
+          for _, tags in parse_tags(path, tag_prefix=tag_prefix):
             for tag in tags:
               print(tag)
     return xit
 
   def cmd_test(self, argv):
     ''' Usage: {cmd} [testnames...]
           Run self tests.
@@ -284,27 +306,27 @@
 
 # a convenience chunk of 256 zero bytes, mostly for use by 'free' blocks
 B0_256 = bytes(256)
 
 # an arbitrary maximum read size for fetching the data section
 SIZE_16MB = 1024 * 1024 * 16
 
-def parse_deref_path(path, offset=0):
+def get_deref_path(path, offset=0):
   ''' Parse a `path` string from `offset`.
       Return the path components and the offset where the parse stopped.
 
       Path components:
-      * _identifier_: an identifier represents a Box field or if such a
+      * _identifier_: an identifier represents a `Box` field or if such a
         field is not present, a the first subbox of this type
       * `[`_index_`]`: the subbox with index _index_
 
       Examples:
 
-          >>> parse_deref_path('.abcd[5]')
-          ['abcd', 5]
+          >>> get_deref_path('.abcd[5]')
+          (['abcd', 5], 8)
   '''
   parts = []
   while offset < len(path):
     # .type
     if path.startswith('.', offset):
       name, offset2 = get_identifier(path, offset + 1)
       if name:
@@ -322,15 +344,15 @@
   return parts, offset
 
 def deref_box(B, path):
   ''' Dereference a path with respect to this Box.
   '''
   with Pfx("deref_path(%r)", path):
     if isinstance(path, str):
-      parts, offset = parse_deref_path(path)
+      parts, offset = get_deref_path(path)
       if offset < len(path):
         raise ValueError(
             "parse_path(%r): stopped early at %d:%r" %
             (path, offset, path[offset:])
         )
       return deref_box(B, parts)
     for i, part in enumerate(path):
@@ -378,15 +400,15 @@
 
   BOM_ENCODING = {
       b'\xfe\xff': 'utf_16_le',
       b'\xff\xfe': 'utf_16_be',
   }
 
   @classmethod
-  def parse(cls, bfr):
+  def parse(cls, bfr: CornuCopyBuffer):
     ''' Gather optional BOM and then UTF8 or UTF16 string.
     '''
     self = cls()
     bfr.extend(1)
     if bfr[0] == 0:
       # empty sting, no BOM
       bom = b''
@@ -407,15 +429,15 @@
     return self
 
   def transcribe(self):
     ''' Transcribe the field suitably encoded.
     '''
     if self.bom:
       yield self.bom
-      yield UTF16NULField.transcribe_value(
+      yield BinaryUTF16NUL.transcribe_value(
           self.text, encoding=self.BOM_ENCODING[self.bom]
       )
     else:
       yield BinaryUTF8NUL.transcribe_value(self.text)
 
 class TimeStampMixin:
   ''' Methods to assist with ISO14496 timestamps.
@@ -460,23 +482,23 @@
 
   def __str__(self):
     return str(self.datetime) or str(self.value)
 
 class BoxHeader(BinaryMultiValue('BoxHeader', {
     'box_size': UInt32BE,
 })):
-  ''' An ISO14496 Box header packet.
+  ''' An ISO14496 `Box` header packet.
   '''
 
   # speculative max size that will fit in the UInt32BE box_size
   # with room for bigger sizes in the optional UInt64BE length field
   MAX_BOX_SIZE_32 = 2**32 - 8
 
   @classmethod
-  def parse(cls, bfr):
+  def parse(cls, bfr: CornuCopyBuffer):
     ''' Decode a box header from `bfr`.
     '''
     self = cls()
     # note start of header
     self.offset = bfr.offset
     box_size = UInt32BE.parse_value(bfr)
     box_type = self.box_type = bfr.take(4)
@@ -508,19 +530,58 @@
     yield UInt32BE.transcribe_value(box_size)
     yield self.box_type
     if self.box_size is not Ellipsis and self.box_size > self.MAX_BOX_SIZE_32:
       yield UInt64BE.transcribe_value(self.box_size)
     if self.box_type == b'uuid':
       yield self.user_type
 
-class BoxBody(SimpleBinary, ABC):
+class BoxBody(SimpleBinary):
   ''' Abstract basis for all `Box` bodies.
   '''
 
   FIELD_TYPES = dict(offset=int, post_offset=int)
+  SUBCLASSES_BY_BOXTYPE = {}
+
+  @classmethod
+  def __init_subclass__(cls, bodyclass_name=None, doc=None):
+    if bodyclass_name is not None:
+      cls.__name__ = bodyclass_name
+    if doc is not None:
+      cls.__doc__ = doc
+    # update the mapping of box_type to BoxBody subclass
+    try:
+      # explicit list of box_type byte strings
+      box_types = cls.BOX_TYPES
+    except AttributeError:
+      # infer the box_type from the class name's leading 4 characters
+      try:
+        box_type = cls.boxbody_type_from_class()
+      except ValueError as e:
+        box_types = ()
+      else:
+        box_types = (box_type,)
+    SUBCLASSES_BY_BOXTYPE = BoxBody.SUBCLASSES_BY_BOXTYPE
+    for box_type in box_types:
+      try:
+        existing_box_class = SUBCLASSES_BY_BOXTYPE[box_type]
+      except KeyError:
+        # new box_type as expected
+        SUBCLASSES_BY_BOXTYPE[box_type] = cls
+      else:
+        raise TypeError(
+            f'box_type {box_type!r} already in BoxBody.SUBCLASSES_BY_BOXTYPE as {existing_box_class.__name__}'
+        )
+
+  @staticmethod
+  @require(lambda box_type: len(box_type) == 4)
+  @typechecked
+  def for_box_type(box_type: bytes):
+    ''' Return the `BoxBody` subclass suitable for the `box_type`.
+    '''
+    return BoxBody.SUBCLASSES_BY_BOXTYPE.get(box_type, BoxBody)
 
   def __getattr__(self, attr):
     ''' The following virtual attributes are defined:
         * *TYPE*`s`:
           "boxes of type *TYPE*",
           an uppercased box type name with a training `s`;
           a list of all elements whose `.box_type`
@@ -550,17 +611,18 @@
     if len(attr) == 5 and (attr.endswith('s') or attr.endswith('0')):
       attr4 = attr[:4]
       if attr4.isupper():
         box_type = attr4.lower().encode('ascii')
         try:
           boxes = self.boxes
         except AttributeError:
-          warning("no .boxes")
-          boxes = ()
-        boxes = [box for box in boxes if box.box_type == box_type]
+          warning("%s.%s: no .boxes", self.__class__.__name__, attr)
+          boxes = []
+        else:
+          boxes = [box for box in boxes if box.box_type == box_type]
         if attr.endswith('s'):
           return boxes
         if attr.endswith('0'):
           if len(boxes) == 0:
             return None
           box, = boxes
           return box
@@ -569,42 +631,42 @@
   def __str__(self):
     return super().__str__(getattr(self, '_parsed_field_names', ()))
 
   def __iter__(self):
     yield from ()
 
   @classmethod
-  def parse(cls, bfr):
+  def parse(cls, bfr: CornuCopyBuffer):
     ''' Create a new instance and gather the `Box` body fields from `bfr`.
 
         Subclasses implement a `parse_fields` method to parse additional fields.
     '''
     self = cls()
     self._parsed_field_names = []
     self.parse_fields(bfr)
     return self
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Parse additional fields.
         This base class implementation consumes nothing.
     '''
 
-  def parse_field_value(self, field_name, bfr, binary_cls):
+  def parse_field_value(self, field_name, bfr: CornuCopyBuffer, binary_cls):
     ''' Parse a single value binary, store the value as `field_name`,
         store the instance as the field `field_name+'__Binary'`
         for transcription.
 
         Note that this disassociaes the plain value attribute
         from what gets transcribed.
     '''
     instance = binary_cls.parse(bfr)
     self.add_field('_' + field_name + '__Binary', instance)
     setattr(self, field_name, instance.value)
 
-  def parse_field(self, field_name, bfr, binary_cls):
+  def parse_field(self, field_name, bfr: CornuCopyBuffer, binary_cls):
     ''' Parse an instance of `binary_cls` from `bfr`
         and store it as the attribute named `field_name`.
 
         `binary_cls` may also be an `int`, in which case that many
         bytes are read from `bfr`.
     '''
     if isinstance(binary_cls, int):
@@ -634,31 +696,31 @@
         order parsed.
     '''
     return map(
         lambda field_name: getattr(self, field_name),
         self._parsed_field_names,
     )
 
-  def parse_boxes(self, bfr, **kw):
+  def parse_boxes(self, bfr: CornuCopyBuffer, **kw):
     ''' Utility method to parse the remainder of the buffer as a
         sequence of `Box`es.
     '''
     self.boxes = list(Box.scan(bfr, **kw))
     self._parsed_field_names.append('boxes')
 
   @classmethod
-  def boxbody_type_from_klass(cls):
+  def boxbody_type_from_class(cls):
     ''' Compute the Box's 4 byte type field from the class name.
     '''
     class_name = cls.__name__
     if len(class_name) == 11 and class_name.endswith('BoxBody'):
       class_prefix = class_name[:4]
       if class_prefix.rstrip('_').isupper():
         return class_prefix.replace('_', ' ').lower().encode('ascii')
-    raise AttributeError("no automatic box type for %s" % (cls,))
+    raise ValueError(f'no automatic box type for class named {class_name!r}')
 
 class Box(SimpleBinary):
   ''' Base class for all boxes - ISO14496 section 4.2.
 
       This has the following fields:
       * `header`: a `BoxHeader`
       * `body`: a `BoxBody` instance, usually a specific subclass
@@ -693,59 +755,56 @@
 
   __repr__ = __str__
 
   def __getattr__(self, attr):
     ''' If there is no direct attribute from `SimpleBinary.__getattr__`,
         have a look in the `.header` and `.body`.
     '''
-    if attr in ('header', 'body'):
-      raise AttributeError("%s.%s: not present" % (type(self).__name__, attr))
-    try:
-      value = getattr(self.header, attr)
-    except AttributeError:
-      try:
-        value = getattr(self.body, attr)
-      except AttributeError:
-        raise AttributeError(
-            "%s.%s: not present via %r or the .header or .body fields" % (
-                type(self).__name__, attr,
-                ",".join(map(lambda cls: cls.__name__,
-                             type(self).__mro__))
-            )
-        )
-    return value
+    with Pfx("%s.%s", self.__class__.__name__, attr):
+      if attr not in ('header', 'body'):
+        try:
+          value = getattr(self.header, attr)
+        except AttributeError:
+          try:
+            value = getattr(self.body, attr)
+          except AttributeError as e:
+            raise AttributeError(
+                f'not present via {self.__class__.__mro__} or the .header or .body fields'
+            ) from e
+        return value
+      raise AttributeError("not present")
 
   def __iter__(self):
     ''' Iterating over a `Box` iterates over its body.
         Typically that would be the `.body.boxes`
         but might be the samples if the body is a sample box,
         etc.
     '''
     if self.body is None:
       ##warning("iter(%s): body is None", self)
       return
     yield from iter(self.body)
 
   @classmethod
-  def parse(cls, bfr):
-    ''' Decode a Box from `bfr` and return it.
+  def parse(cls, bfr: CornuCopyBuffer):
+    ''' Decode a `Box` from `bfr` and return it.
     '''
     self = cls()
     self.offset = bfr.offset
     header = self.header = BoxHeader.parse(bfr)
     with Pfx("%s.parse", header.box_type):
       length = header.box_size
       if length is Ellipsis:
         end_offset = Ellipsis
         bfr_tail = bfr
         warning("Box.parse: Box %s has no length", header)
       else:
         end_offset = self.offset + length
         bfr_tail = bfr.bounded(end_offset)
-      body_class = pick_boxbody_class(header.type)
+      body_class = BoxBody.for_box_type(header.type)
       body_offset = bfr_tail.offset
       self.body = body_class.parse(bfr_tail)
       # attach subBoxen to self
       boxes = getattr(self.body, 'boxes', None)
       if boxes:
         for box in boxes:
           box.parent = self
@@ -762,15 +821,15 @@
       self.self_check()
       bfr.report_offset(self.offset)
       copy_boxes = PARSE_MODE.copy_boxes
       if copy_boxes:
         copy_boxes(self)
       return self
 
-  def parse_field(self, field_name, bfr, binary_cls):
+  def parse_field(self, field_name, bfr: CornuCopyBuffer, binary_cls):
     ''' `parse_field` delegates to the `Box` body `parse_field`.
     '''
     return self.body.parse_field(field_name, bfr, binary_cls)
 
   @property
   def parse_length(self):
     ''' The length of the box as consumed from the buffer,
@@ -831,20 +890,19 @@
     with Pfx(self):
       box_type = self.header.type
       try:
         BOX_TYPE = self.BOX_TYPE
       except AttributeError:
         try:
           BOX_TYPES = self.BOX_TYPES
-        except AttributeError:
+        except AttributeError as e:
           if not isinstance(self, Box):
             raise RuntimeError(
-                "no BOX_TYPE or BOX_TYPES to check in class %r" %
-                (type(self),)
-            )
+                f'no BOX_TYPE or BOX_TYPES to check in class {type(self)!r}'
+            ) from e
         else:
           if box_type not in BOX_TYPES:
             warning(
                 "box_type should be in %r but got %r", BOX_TYPES,
                 bytes(box_type)
             )
       else:
@@ -867,21 +925,21 @@
     self.unparsed = []
     bfr = CornuCopyBuffer(unparsed)
     yield bfr
     self.unparsed = list(bfr)
 
   @property
   def box_type(self):
-    ''' The Box header type.
+    ''' The `Box` header type.
     '''
     return self.header.type
 
   @property
   def box_type_s(self):
-    ''' The Box header type as a string.
+    ''' The `Box` header type as a string.
 
         If the header type bytes decode as ASCII, return that,
         otherwise the header bytes' repr().
     '''
     box_type_b = bytes(self.box_type)
     try:
       box_type_name = box_type_b.decode('ascii')
@@ -915,15 +973,15 @@
     return self.header.user_type
 
   # NB: a @property instead of @prop to preserve AttributeError
   @property
   def BOX_TYPE(self):
     ''' The default .BOX_TYPE is inferred from the class name.
     '''
-    return type(self).boxbody_type_from_klass()
+    return type(self).boxbody_type_from_class()
 
   def ancestor(self, box_type):
     ''' Return the closest ancestor box of type `box_type`.
     '''
     if isinstance(box_type, str):
       box_type = box_type.encode('ascii')
     parent = self.parent
@@ -934,22 +992,22 @@
     return parent
 
   def dump(self, **kw):
     ''' Dump this Box.
     '''
     return dump_box(self, **kw)
 
-  def walk(self):
+  def walk(self) -> Iterable[Tuple["Box", List["Box"]]]:
     ''' Walk this `Box` hierarchy.
 
         Yields the starting box and its children as `(self,subboxes)`
         and then yields `(subbox,subsubboxes)` for each child in turn.
 
         As with `os.walk`, the returned `subboxes` list
-        may be modified to prune the subsequent walk.
+        may be modified in place to prune or reorder the subsequent walk.
     '''
     # We don't go list(self) or [].extend(self) because both of those fire
     # the transcription of the box because of list's preallocation heuristics.
     # Instead we make a bare iterator and list() that, specific
     # incantation from Peter Otten.
     subboxes = list(iter(self))
     yield self, subboxes
@@ -981,81 +1039,44 @@
       ##dump_box(self, crop_length=None)
       return tags
 
   def gather_metadata(self):
     ''' Walk the `Box` hierarchy looking for metadata.
         Yield `(Box,TagSet)` for each `b'moov'` or `b'trak'` `Box`.
     '''
-    for box, subboxes in self.walk():
+    for box, _ in self.walk():
       if box.box_type in (b'moov', b'trak'):
         yield box, box.metatags()
 
 # patch us in
 Box.FIELD_TYPES['parent'] = (False, (type(None), Box))
 BoxBody.FIELD_TYPES['parent'] = Box
 
-# mapping of known box subclasses for use by factories
-KNOWN_BOXBODY_CLASSES = {}
-
-class FallbackBoxBody(BoxBody):
-  ''' A `BoxBody` subclass which parses nothing for unimplemented `Box` types,
-      used by `pick_boxbody_class()`.
-  '''
-
-  def __str__(self):
-    return type(self).__name__
-
-def pick_boxbody_class(box_type: bytes):
-  ''' Infer a `BoxBody` subclass from the 4-byte bytes `box_type`.
-      Returns `FallbackBoxBody` for unimplemented types.
-  '''
-  return KNOWN_BOXBODY_CLASSES.get(box_type, FallbackBoxBody)
-
-def add_body_class(klass):
-  ''' Register a box body class in KNOWN_BOXBODY_CLASSES.
-  '''
-  global KNOWN_BOXBODY_CLASSES
-  with Pfx("add_body_class(%s)", klass):
-    try:
-      box_types = klass.BOX_TYPES
-    except AttributeError:
-      box_type = klass.boxbody_type_from_klass()
-      box_types = (box_type,)
-    for box_type in box_types:
-      if box_type in KNOWN_BOXBODY_CLASSES:
-        raise TypeError(
-            "box_type %r already in KNOWN_BOXBODY_CLASSES as %s" %
-            (box_type, KNOWN_BOXBODY_CLASSES[box_type])
-        )
-      KNOWN_BOXBODY_CLASSES[box_type] = klass
-
 def add_body_subclass(superclass, box_type, section, desc):
-  ''' Create and register a new BoxBody class that is simply a subclass of
-      another.  Returns the new class.
+  ''' Create and register a new `BoxBody` class that is simply a subclass of
+      another.
+      Return the new class.
   '''
   if isinstance(box_type, bytes):
     box_type = box_type.decode('ascii')
-  classname = box_type.upper() + 'BoxBody'
+  classname = f'{box_type.upper()}BoxBody'
   box_type = box_type.encode('ascii')
 
-  class SubClass(superclass):
-    ''' A distinct subclass simply subclassing the parent.
-    '''
+  class _SubClass(
+      superclass,
+      bodyclass_name=classname,
+      doc=f'An {box_type!r} {desc} box - ISO14496 section {section}.',
+  ):
 
     def transcribe(self):
       ''' A stub transcribe method distinct from the parent.
       '''
       yield from super().transcribe()
 
-  SubClass.__name__ = classname
-  SubClass.__doc__ = (
-      "Box type %r %s box - ISO14496 section %s." % (box_type, desc, section)
-  )
-  add_body_class(SubClass)
-  return SubClass
+  return _SubClass
 
 class HasBoxesMixin:
 
   def __iter__(self):
     return iter(self.boxes)
 
   def __getattr__(self, attr):
@@ -1080,15 +1101,15 @@
   def boxes(self):
     ''' Alias `.value` as `.boxes`: the `Box`es encompassed by this `OverBox`.
     '''
     return self.values
 
   # TODO: this seems to parse a single `Box`: can we drop `OverBox`?
   @classmethod
-  def parse(cls, bfr):
+  def parse(cls, bfr: CornuCopyBuffer):
     ''' Parse the `OverBox`.
     '''
     offset = bfr.offset
     self = super().parse(bfr, pt=Box)
     self.offset = offset
     self.end_offset = bfr.offset
     return self
@@ -1121,15 +1142,15 @@
       BoxBody.FIELD_TYPES,
       _version__Binary=UInt8,
       _flags0__Binary=UInt8,
       _flags1__Binary=UInt8,
       _flags2__Binary=UInt8,
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     super().parse_fields(bfr)
     self.parse_field_value('version', bfr, UInt8)
     self.parse_field_value('flags0', bfr, UInt8)
     self.parse_field_value('flags1', bfr, UInt8)
     self.parse_field_value('flags2', bfr, UInt8)
 
   @property
@@ -1140,15 +1161,15 @@
 
 class MDATBoxBody(BoxBody):
   ''' A Media Data Box - ISO14496 section 8.1.1.
   '''
 
   FIELD_TYPES = dict(BoxBody.FIELD_TYPES, data=(True, (type(None), list)))
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather all data to the end of the field.
     '''
     super().parse_fields(bfr)
     offset0 = bfr.offset
     if PARSE_MODE.discard_data:
       self.data = None
       bfr.skipto(bfr.end_offset)
@@ -1164,29 +1185,27 @@
   def transcribe(self):
     ''' Transcribe the data.
         Raise an `AssertionError` if we skipped the data during the parse.
     '''
     assert self.data is not None
     return self.data
 
-add_body_class(MDATBoxBody)
-
 class FREEBoxBody(BoxBody):
   ''' A 'free' or 'skip' box - ISO14496 section 8.1.2.
       Note the length and discard the data portion.
   '''
 
   FIELD_TYPES = dict(
       BoxBody.FIELD_TYPES,
       free_size=int,
   )
 
   BOX_TYPES = (b'free', b'skip')
 
-  def parse_fields(self, bfr, end_offset=Ellipsis, **kw):
+  def parse_fields(self, bfr: CornuCopyBuffer, end_offset=Ellipsis, **kw):
     ''' Gather the `padding` field.
     '''
     super().parse_fields(bfr, **kw)
     self.free_size = bfr.end_offset - bfr.offset
     bfr.skipto(bfr.end_offset)
 
   def transcribe(self):
@@ -1194,29 +1213,27 @@
     n256 = len(B0_256)
     while free_size >= n256:
       yield B0_256
       free_size -= n256
     if free_size > 0:
       yield bytes(free_size)
 
-add_body_class(FREEBoxBody)
-
 class FTYPBoxBody(BoxBody):
   ''' An 'ftyp' File Type box - ISO14496 section 4.3.
       Decode the major_brand, minor_version and compatible_brands.
   '''
 
   FIELD_TYPES = dict(
       BoxBody.FIELD_TYPES,
       major_brand=bytes,
       minor_version=int,
       brands_bs=bytes,
   )
 
-  def parse_fields(self, bfr, **kw):
+  def parse_fields(self, bfr: CornuCopyBuffer, **kw):
     ''' Gather the `major_brand`, `minor_version` and `brand_bs` fields.
     '''
     super().parse_fields(bfr, **kw)
     self.major_brand = bfr.take(4)
     self.minor_version = UInt32BE.parse_value(bfr)
     self.brands_bs = b''.join(bfr)
 
@@ -1231,59 +1248,53 @@
     ''' The compatible brands as a list of 4 byte bytes instances.
     '''
     return [
         self.brands_bs[offset:offset + 4]
         for offset in range(0, len(self.brands_bs), 4)
     ]
 
-add_body_class(FTYPBoxBody)
-
 class PDINBoxBody(FullBoxBody):
   ''' A 'pdin' Progressive Download Information box - ISO14496 section 8.1.3.
   '''
 
   FIELD_TYPES = dict(
       FullBoxBody.FIELD_TYPES,
       pdinfo=list,
   )
 
   # field names for the tuples in a PDINBoxBody
   PDInfo = BinaryMultiStruct('PDInfo', '>LL', 'rate initial_delay')
 
-  def parse_fields(self, bfr, **kw):
+  def parse_fields(self, bfr: CornuCopyBuffer, **kw):
     ''' Gather the normal version information
         and then the `(rate,initial_delay)` pairs of the data section
         as the `pdinfo` field.
     '''
     super().parse_fields(bfr, **kw)
     self.add_field('pdinfo', list(PDINBoxBody.PDInfo.scan(bfr)))
 
-add_body_class(PDINBoxBody)
-
 class ContainerBoxBody(BoxBody):
   ''' Common subclass of several things with `.boxes`.
   '''
 
   FIELD_TYPES = dict(BoxBody.FIELD_TYPES, boxes=list)
 
   @pfx_method
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     super().parse_fields(bfr)
     self.parse_boxes(bfr)
 
   def __iter__(self):
     return iter(self.boxes)
 
 class MOOVBoxBody(ContainerBoxBody):
   ''' An 'moov' Movie box - ISO14496 section 8.2.1.
       Decode the contained boxes.
   '''
 
-add_body_class(MOOVBoxBody)
-
 class MVHDBoxBody(FullBoxBody):
   ''' An 'mvhd' Movie Header box - ISO14496 section 8.2.2.
   '''
 
   FIELD_TYPES = dict(
       FullBoxBody.FIELD_TYPES,
       creation_time=(True, (TimeStamp32, TimeStamp64)),
@@ -1294,15 +1305,15 @@
       volume_short=Int16BE,
       reserved1=bytes,
       matrix=Matrix9Long,
       predefined1=bytes,
       next_track_id=UInt32BE,
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     super().parse_fields(bfr)
     # obtain box data after version and flags decode
     if self.version == 0:
       self.parse_field('creation_time', bfr, TimeStamp32)
       self.parse_field('modification_time', bfr, TimeStamp32)
       self.parse_field('timescale', bfr, UInt32BE)
       self.parse_field('duration', bfr, UInt32BE)
@@ -1344,16 +1355,14 @@
   @prop
   def volume(self):
     ''' Volume field converted to float: 1.0 represents full volume.
     '''
     volume_short = self.volume_short
     return (volume_short >> 8) + (volume_short & 0xff) / 256.0
 
-add_body_class(MVHDBoxBody)
-
 add_body_subclass(ContainerBoxBody, 'trak', '8.3.1', 'Track')
 
 class TKHDBoxBody(FullBoxBody):
   ''' A 'tkhd' Track Header box - ISO14496 section 8.2.2.
   '''
 
   TKHDMatrix = BinaryMultiStruct(
@@ -1374,15 +1383,15 @@
       volume=Int16BE,
       reserved4=UInt16BE,
       matrix=TKHDMatrix,
       width=UInt32BE,
       height=UInt32BE,
   )
 
-  def parse_fields(self, bfr, **kw):
+  def parse_fields(self, bfr: CornuCopyBuffer, **kw):
     super().parse_fields(bfr, **kw)
     # obtain box data after version and flags decode
     if self.version == 0:
       self.parse_field('creation_time', bfr, TimeStamp32)
       self.parse_field('modification_time', bfr, TimeStamp32)
       self.parse_field('track_id', bfr, UInt32BE)
       self.parse_field('reserved1', bfr, UInt32BE)
@@ -1448,24 +1457,20 @@
 
   @prop
   def timescale(self):
     ''' The `timescale` comes from the movie header box (8.3.2.3).
     '''
     return self.ancestor('mvhd').timescale
 
-add_body_class(TKHDBoxBody)
-
 ##add_body_subclass(ContainerBoxBody, 'tref', '8.3.3', 'track Reference')
 
 class TREFBoxBody(ContainerBoxBody):
   ''' Track Reference BoxBody, container for trackReferenceTypeBoxes - ISO14496 section 8.3.3.
   '''
 
-add_body_class(TREFBoxBody)
-
 class TrackReferenceTypeBoxBody(BoxBody):
   ''' A TrackReferenceTypeBoxBody contains references to other tracks - ISO14496 section 8.3.3.2.
   '''
   FIELD_TYPES = dict(BoxBody.FIELD_TYPES, track_ids=list)
 
   BOX_TYPES = (
       b'hint',
@@ -1475,31 +1480,30 @@
       b'hind',
       b'vdep',
       b'vplx',
       b'subt',
       b'forc',
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `track_ids` field.
     '''
     super().parse_fields(bfr)
     self.add_field('track_ids', list(UInt32BE.scan(bfr)))
 
-add_body_class(TrackReferenceTypeBoxBody)
 add_body_subclass(ContainerBoxBody, 'trgr', '8.3.4', 'Track Group')
 
 class TrackGroupTypeBoxBody(FullBoxBody):
   ''' A TrackGroupTypeBoxBody contains a track group id - ISO14496 section 8.3.3.2.
   '''
 
   def __init__(self, box_type, box_data):
     FullBoxBody.__init__(self, box_type, box_data)
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `track_group_id` field.
     '''
     super().parse_fields(bfr)
     self.parse_field('track_group_id', bfr, UInt32BE)
 
 add_body_subclass(
     TrackGroupTypeBoxBody, 'msrc', '8.3.4.3',
@@ -1517,15 +1521,15 @@
       modification_time=(True, (TimeStamp32, TimeStamp64)),
       timescale=UInt32BE,
       duration=(True, (UInt32BE, UInt64BE)),
       language_short=UInt16BE,
       pre_defined=UInt16BE,
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `creation_time`, `modification_time`, `timescale`,
         `duration` and `language_short` fields.
     '''
     super().parse_fields(bfr)
     # obtain box data after version and flags decode
     if self.version == 0:
       self.parse_field('creation_time', bfr, TimeStamp32)
@@ -1561,31 +1565,29 @@
             x + 0x60 for x in (
                 (language_short >> 10) & 0x1f, (language_short >> 5) & 0x1f,
                 language_short & 0x1f
             )
         ]
     ).decode('ascii')
 
-add_body_class(MDHDBoxBody)
-
 class HDLRBoxBody(FullBoxBody):
   ''' A HDLRBoxBody is a Handler Reference box - ISO14496 section 8.4.3.
   '''
 
   FIELD_TYPES = dict(
       FullBoxBody.FIELD_TYPES,
       pre_defined=UInt32BE,
       handler_type_long=UInt32BE,
       reserved1=UInt32BE,
       reserved2=UInt32BE,
       reserved3=UInt32BE,
       name=BinaryUTF8NUL,
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `handler_type_long` and `name` fields.
     '''
     super().parse_fields(bfr)
     # NB: handler_type is supposed to be an unsigned long, but in
     # practice seems to be 4 ASCII bytes, so we present it as a string
     # for readability
     self.parse_field('pre_defined', bfr, UInt32BE)
@@ -1606,39 +1608,37 @@
 
   @property
   def handler_type(self):
     ''' The handler_type as an ASCII string, its usual form.
     '''
     return bytes(self.handler_type_long).decode('ascii')
 
-add_body_class(HDLRBoxBody)
 add_body_subclass(ContainerBoxBody, b'minf', '8.4.4', 'Media Information')
 add_body_subclass(FullBoxBody, 'nmhd', '8.4.5.2', 'Null Media Header')
 
 class ELNGBoxBody(FullBoxBody):
   ''' A ELNGBoxBody is a Extended Language Tag box - ISO14496 section 8.4.6.
   '''
 
   FIELD_TYPES = dict(
       FullBoxBody.FIELD_TYPES,
       extended_language=BinaryUTF8NUL,
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `extended_language` field.
     '''
     super().parse_fields(bfr)
     # extended language based on RFC4646
     self.parse_field('extended_language', bfr, BinaryUTF8NUL)
 
   def transcribe(self):
     yield super().transcribe()
     yield self.extended_language
 
-add_body_class(ELNGBoxBody)
 add_body_subclass(ContainerBoxBody, b'stbl', '8.5.1', 'Sample Table')
 
 class _SampleTableContainerBoxBody(FullBoxBody):
   ''' An intermediate FullBoxBody subclass which contains more boxes.
   '''
 
   FIELD_TYPES = dict(
@@ -1646,15 +1646,15 @@
       entry_count=UInt32BE,
       boxes=list,
   )
 
   def __iter__(self):
     return iter(self.boxes)
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `entry_count` and `boxes`.
     '''
     super().parse_fields(bfr)
     # obtain box data after version and flags decode
     self.entry_count = UInt32BE.parse(bfr)
     self.parse_boxes(bfr, count=int(self.entry_count.value))
 
@@ -1667,34 +1667,33 @@
     _SampleTableContainerBoxBody, b'stsd', '8.5.2', 'Sample Description'
 )
 
 class _SampleEntry(BoxBody):
   ''' Superclass of Sample Entry boxes.
   '''
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `data_reference_inde` field.
     '''
     super().parse_fields(bfr)
     self.add_field('reserved', bfr.take(6))
     self.parse_field('data_reference_index', bfr, UInt16BE)
 
 class BTRTBoxBody(BoxBody):
   ''' BitRateBoxBody - section 8.5.2.2.
   '''
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `bufferSizeDB`, `maxBitrate` and `avgBitrate` fields.
     '''
     super().parse_fields(bfr)
     self.parse_field('bufferSizeDB', bfr, UInt32BE)
     self.parse_field('maxBitrate', bfr, UInt32BE)
     self.parse_field('avgBitRate', bfr, UInt32BE)
 
-add_body_class(BTRTBoxBody)
 add_body_subclass(
     _SampleTableContainerBoxBody, b'stdp', '8.5.3', 'Degradation Priority'
 )
 
 TTSB_Sample = namedtuple('TTSB_Sample', 'count delta')
 
 # pylint: disable=too-many-arguments
@@ -1716,27 +1715,30 @@
   sample_type_v0 = BinaryMultiStruct(
       sample_class_name + 'V0', struct_format_v0, sample_fields
   )
   sample_type_v1 = BinaryMultiStruct(
       sample_class_name + 'V1', struct_format_v1, sample_fields
   )
 
-  class SpecificSampleBoxBody(FullBoxBody):
-    ''' Time to Sample box - section 8.6.1.
-    '''
+  class _SpecificSampleBoxBody(
+      FullBoxBody,
+      bodyclass_name=class_name,
+      doc=f'`Box` type {box_type!r} {desc} box - ISO14496 section {section}.',
+  ):
+
     FIELD_TYPES = dict(
         FullBoxBody.FIELD_TYPES,
         entry_count=(False, UInt32BE),
         has_inferred_entry_count=bool,
         sample_type=(True, type),
         samples_count=int,
         samples_bs=bytes,
     )
 
-    def parse_fields(self, bfr):
+    def parse_fields(self, bfr: CornuCopyBuffer):
       super().parse_fields(bfr)
       if self.version == 0:
         sample_type = self.sample_type = sample_type_v0
       elif self.version == 1:
         sample_type = self.sample_type = sample_type_v1
       else:
         warning(
@@ -1768,36 +1770,31 @@
       except AttributeError:
         yield self.samples_bs
       else:
         yield from map(self.sample_type.transcribe_value, samples)
 
     @locked_property
     @pfx_method
-    def samples(self, bfr):
+    def samples(self, bfr: CornuCopyBuffer):
       ''' The `sample_data` decoded.
       '''
       bfr = CornuCopyBuffer.from_bytes(self.sample_bs)
       sample_type = self.sample_type
       decoded = []
       for _ in range(self.samples_count):
         decoded.append(sample_type.parse_value(bfr))
       assert bfr.at_eof()
       return decoded
 
-  SpecificSampleBoxBody.__name__ = class_name
-  SpecificSampleBoxBody.__doc__ = (
-      "Box type %r %s box - ISO14496 section %s." % (box_type, desc, section)
-  )
   # we define these here because the names collide with the closure
-  SpecificSampleBoxBody.struct_format_v0 = struct_format_v0
-  SpecificSampleBoxBody.sample_type_v0 = sample_type_v0
-  SpecificSampleBoxBody.struct_format_v1 = struct_format_v1
-  SpecificSampleBoxBody.sample_type_v1 = sample_type_v1
-  add_body_class(SpecificSampleBoxBody)
-  return SpecificSampleBoxBody
+  _SpecificSampleBoxBody.struct_format_v0 = struct_format_v0
+  _SpecificSampleBoxBody.sample_type_v0 = sample_type_v0
+  _SpecificSampleBoxBody.struct_format_v1 = struct_format_v1
+  _SpecificSampleBoxBody.sample_type_v1 = sample_type_v1
+  return _SpecificSampleBoxBody
 
 def add_time_to_sample_boxbody(box_type, section, desc):
   ''' Add a Time to Sample box - section 8.6.1.
   '''
   return add_generic_sample_boxbody(
       box_type,
       section,
@@ -1826,15 +1823,15 @@
   CSLGParamsLong = BinaryMultiStruct(
       'CSLGParamsLong', '>lllll', CSLG_PARAM_NAMES
   )
   CSLGParamsQuad = BinaryMultiStruct(
       'CSLGParamsLong', '>qqqqq', CSLG_PARAM_NAMES
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the compositionToDTSShift`, `leastDecodeToDisplayDelta`,
         `greatestDecodeToDisplayDelta`, `compositionStartTime` and
         `compositionEndTime` fields.
     '''
     super().parse_fields(bfr)
     if self.version == 0:
       param_type = self.CSLGParamsLong
@@ -1849,16 +1846,14 @@
     ''' Present the `params` attributes at the top level.
     '''
     try:
       return getattr(self.params, attr)
     except AttributeError:
       return super().__getattr__(attr)
 
-add_body_class(CSLGBoxBody)
-
 add_generic_sample_boxbody(b'stss', '8.6.2', 'Sync Sample', '>L', 'number')
 
 add_generic_sample_boxbody(
     b'stsh', '8.6.3', 'Shadow Sync Table', '>LL',
     'shadowed_sample_number sync_sample_number'
 )
 
@@ -1894,15 +1889,15 @@
 
   @property
   def entry_count(self):
     ''' The number of entries.
     '''
     return len(self.entries)
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Parse the fields of an `ELSTBoxBody`.
     '''
     super().parse_fields(bfr)
     assert self.version in (0, 1)
     entry_count = UInt32BE.parse_value(bfr)
     self.entries = list(self.entry_class.scan(bfr, count=entry_count))
 
@@ -1917,52 +1912,48 @@
 
 class URL_BoxBody(FullBoxBody):
   ''' An 'url ' Data Entry URL BoxBody - section 8.7.2.1.
   '''
 
   FIELD_TYPES = dict(FullBoxBody.FIELD_TYPES, location=BinaryUTF8NUL)
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `location` field.
     '''
     super().parse_fields(bfr)
     self.parse_field('location', bfr, BinaryUTF8NUL)
 
-add_body_class(URL_BoxBody)
-
 class URN_BoxBody(FullBoxBody):
   ''' An 'urn ' Data Entry URL BoxBody - section 8.7.2.1.
   '''
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `name` and `location` fields.
     '''
     super().parse_fields(bfr)
     self.parse_field('name', bfr, BinaryUTF8NUL)
     self.parse_field('location', bfr, BinaryUTF8NUL)
 
   def transcribe(self):
     yield super().transcribe()
     yield self.name
     yield self.location
 
-add_body_class(URN_BoxBody)
-
 class STSZBoxBody(FullBoxBody):
   ''' A 'stsz' Sample Size box - section 8.7.3.2.
   '''
 
   FIELD_TYPES = dict(
       FullBoxBody.FIELD_TYPES,
       sample_size=UInt32BE,
       sample_count=UInt32BE,
       entry_sizes_bs=(False, (bytes,)),
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `sample_size`, `sample_count`, and `entry_sizes` fields.
     '''
     super().parse_fields(bfr)
     self.sample_size = UInt32BE.parse(bfr)
     sample_size = self.sample_size.value
     self.sample_count = UInt32BE.parse(bfr)
     sample_count = self.sample_count.value
@@ -1994,21 +1985,19 @@
     XP("parse %d bytes from .entry_sizes_bs", len(self.entry_sizes_bs))
     bfr = CornuCopyBuffer.from_bytes(self.entry_sizes_bs)
     entry_sizes = []
     for _ in range(self.sample_count.value):
       entry_sizes.append(UInt32BE.parse_value(bfr))
     return entry_sizes
 
-add_body_class(STSZBoxBody)
-
 class STZ2BoxBody(FullBoxBody):
   ''' A 'stz2' Compact Sample Size box - section 8.7.3.3.
   '''
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `field_size`, `sample_count` and `entry_sizes` fields.
     '''
     super().parse_fields(bfr)
     self.reserved = bfr.take(3)
     self.field_size = UInt8.parse_value(bfr)
     self.sample_count = UInt32BE.parse_value(bfr)
     # TODO: defer the parse of entry_sizes
@@ -2077,15 +2066,15 @@
   )
 
   STSCEntry = BinaryMultiStruct(
       'STSCEntry', '>LLL',
       'first_chunk samples_per_chunk sample_description_index'
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `entry_count` and `entries` fields.
     '''
     super().parse_fields(bfr)
     self.entry_count = UInt32BE.parse_value(bfr)
     self.entries_bs = bfr.take(self.entry_count * STSCBoxBody.STSCEntry.length)
 
   def transcribe(self):
@@ -2096,37 +2085,35 @@
     except AttributeError:
       yield self.entries_bs
     else:
       yield from map(STSCBoxBody.STSCEntry.transcribe_value, entries)
 
   @locked_property
   @pfx_method
-  def entries(self, bfr):
-    ''' Parse the `STSCEntry` list into a list of `int`s.
+  def entries(self, bfr: CornuCopyBuffer):
+    ''' A list of `int`s parsed from the `STSCEntry` list.
     '''
     bfr = CornuCopyBuffer.from_bytes(self.entries_bs)
     entries = []
     for _ in range(self.entry_count):
       entries.append(STSCBoxBody.STSCEntry.parse_value(bfr))
     return entries
 
-add_body_class(STSCBoxBody)
-
 class STCOBoxBody(FullBoxBody):
   ''' A 'stco' Chunk Offset box - section 8.7.5.
   '''
 
   FIELD_TYPES = dict(
       FullBoxBody.FIELD_TYPES,
       entry_count=int,
       chunk_offsets_bs=bytes,
       ##chunk_offsets=ListField,
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `entry_count` and `chunk_offsets` fields.
     '''
     super().parse_fields(bfr)
     self.entry_count = UInt32BE.parse_value(bfr)
     self.chunk_offsets_bs = bfr.take(self.entry_count * UInt32BE.length)
 
   def transcribe(self):
@@ -2137,37 +2124,35 @@
     except AttributeError:
       yield self.chunk_offsets_bs
     else:
       yield from map(UInt32BE.transcribe_value, chunk_offsets)
 
   @locked_property
   @pfx_method
-  def chunk_offsets(self, bfr):
+  def chunk_offsets(self, bfr: CornuCopyBuffer):
     ''' Parse the `UInt32BE` chunk offsets from stashed buffer.
     '''
     XP("decode .chunk_offsets_bs")
     bfr = CornuCopyBuffer.from_bytes(self.chunk_offsets_bs)
     chunk_offsets = []
     for _ in range(self.entry_count):
       chunk_offsets.append(UInt32BE.parse_value(bfr))
     return chunk_offsets
 
-add_body_class(STCOBoxBody)
-
 class CO64BoxBody(FullBoxBody):
   ''' A 'c064' Chunk Offset box - section 8.7.5.
   '''
 
   FIELD_TYPES = dict(
       FullBoxBody.FIELD_TYPES,
       entry_count=int,
       chunk_offsets_bs=bytes,
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `entry_count` and `chunk_offsets` fields.
     '''
     super().parse_fields(bfr)
     self.entry_count = UInt32BE.parse_value(bfr)
     self.chunk_offsets_bs = bfr.take(self.entry_count * UInt64BE.length)
 
   def transcribe(self):
@@ -2178,51 +2163,47 @@
     try:
       chunk_offsets = self._chunk_offsets
     except AttributeError:
       yield self.chunk_offsets_bs
     else:
       yield from map(UInt64BE.transcribe_value, chunk_offsets)
 
-  @deferred_field
-  def chunk_offsets(self, bfr):
-    ''' Computed on demand list of chunk offsets.
-    '''
-    offsets = []
-    for _ in range(self.entry_count):
-      offsets.append(UInt64BE.from_buffer(bfr))
-    return offsets
-
-add_body_class(CO64BoxBody)
+  ##@deferred_field
+  ##def chunk_offsets(self,bfr:CornuCopyBuffer):
+  ##  ''' Computed on demand list of chunk offsets.
+  ##  '''
+  ##  offsets = []
+  ##  for _ in range(self.entry_count):
+  ##    offsets.append(UInt64BE.from_buffer(bfr))
+  ##  return offsets
 
 class DREFBoxBody(FullBoxBody):
   ''' A 'dref' Data Reference box containing Data Entry boxes - section 8.7.2.1.
   '''
 
   FIELD_TYPES = dict(
       FullBoxBody.FIELD_TYPES,
       entry_count=UInt32BE,
       boxes=list,
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `entry_count` and `boxes` fields.
     '''
     super().parse_fields(bfr)
     self.parse_field('entry_count', bfr, UInt32BE)
     self.parse_boxes(bfr, count=int(self.entry_count.value))
 
-add_body_class(DREFBoxBody)
-
 add_body_subclass(ContainerBoxBody, b'udta', '8.10.1', 'User Data')
 
 class CPRTBoxBody(FullBoxBody):
   ''' A 'cprt' Copyright box - section 8.10.2.
   '''
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `language` and `notice` fields.
     '''
     super().parse_fields(bfr)
     self.parse_field('language_packed', bfr, UInt16BE)
     self.parse_field('notice', bfr, UTF8or16Field)
 
   @property
@@ -2255,74 +2236,72 @@
       theHandler=Box,
       boxes=list,
   )
 
   def __iter__(self):
     return iter(self.boxes)
 
-  def parse_fields(self, bfr):
-    ''' Gather the `theHandler` Box and gather the following Boxes as `boxes`.
+  def parse_fields(self, bfr: CornuCopyBuffer):
+    ''' Gather the `theHandler` `Box` and gather the following Boxes as `boxes`.
     '''
     super().parse_fields(bfr)
     self.parse_field('theHandler', bfr, Box)
     ## we don't have a .parent yet - does this break the handler path?
     ## self.theHandler.parent = self.parent
     self.parse_boxes(bfr)
 
   @pfx_method
   def __getattr__(self, attr):
     ''' Present the `ilst` attributes if present.
     '''
-    with Pfx("%r", attr):
-      if attr == 'boxes':
-        raise AttributeError("NO BOXES")
+    if attr != 'boxes':
       try:
+        # direct attribute access
         return super().__getattr__(attr)
       except AttributeError as e:
+        # otherwise dereference through the .ilst subbox if present
         ilst = super().__getattr__('ILST0')
-        if ilst is None:
-          raise AttributeError(attr) from e
-        value = getattr(ilst, attr, None)
-        if value is None:
-          raise AttributeError("no ILST.%s" % (attr,)) from e
-        return value
-
-add_body_class(METABoxBody)
+        if ilst is not None:
+          value = getattr(ilst, attr, None)
+          if value is not None:
+            return value
+    raise AttributeError(f'{self.__class__.__name__}.{attr}')
 
 # class to glom all the bytes
 _ILSTRawSchema = pt_spec(
-    (lambda bfr: bfr.take(...), lambda bs: bs), name='ILSTRawSchema'
+    (lambda bfr: bfr.take(...), lambda bs: bs),
+    name='ILSTRawSchema',
 )
 
 def ILSTRawSchema(attribute_name):
   ''' Attribute name and type for ILST raw schema.
   '''
   return attribute_name, _ILSTRawSchema
 
 # class to decode bytes as UTF-8
 _ILSTTextSchema = pt_spec(
     (
         lambda bfr: bfr.take(...).decode('utf-8'),
         lambda txt: txt.encode('utf-8'),
     ),
-    name='ILSTTextSchema'
+    name='ILSTTextSchema',
 )
 
 def ILSTTextSchema(attribute_name):
   ''' Attribute name and type for ILST text schema.
   '''
   return attribute_name, _ILSTTextSchema
 
 def ILSTUInt32BESchema(attribute_name):
-  ''' Attribute name and type for ILST UInt32BE schema.
+  ''' Attribute name and type for ILST `UInt32BE` schema.
   '''
   return attribute_name, UInt32BE
 
 def ILSTUInt8Schema(attribute_name):
-  ''' Attribute name and type for ILST UInt8BE schema.
+  ''' Attribute name and type for ILST `UInt8BE` schema.
   '''
   return attribute_name, UInt8
 
 # class to decode n/total as a pair of UInt32BE values
 _ILSTAofBSchema = BinaryMultiValue(
     'ILSTAofBSchema', dict(n=UInt32BE, total=UInt32BE)
 )
@@ -2344,15 +2323,15 @@
 def ILSTISOFormatSchema(attribute_name):
   ''' Attribute name and type for ILST ISO format schema.
   '''
   return attribute_name, _ILSTISOFormatSchema
 
 itunes_media_type = namedtuple('itunes_media_type', 'type stik')
 
-def decode_itunes_date_field(data):
+def decode_itunes_date_field(data) -> datetime:
   ''' The iTunes 'Date' meta field: a year or an ISO timestamp.
   '''
   try:
     value = datetime.fromisoformat(data)
   except ValueError:
     value = datetime(int(data), 1, 1)
   return value
@@ -2402,14 +2381,15 @@
 
   FIELD_TYPES = dict(
       ContainerBoxBody.FIELD_TYPES,
       tags=TagSet,
   )
   FIELD_TRANSCRIBERS = dict(tags=lambda _: None,)
 
+  # the schema names are available as attributes
   SUBBOX_SCHEMA = {
       b'\xa9alb': ILSTTextSchema('album_title'),
       b'\xa9art': ILSTTextSchema('artist'),
       b'\xa9ART': ILSTTextSchema('album_artist'),
       b'\xa9cmt': ILSTTextSchema('comment'),
       b'\xa9cpy': ILSTTextSchema('copyright'),
       b'\xa9day': ILSTTextSchema('year'),
@@ -2516,15 +2496,15 @@
           'TotalAudioJumps': int,
           'TotalVideoJumps': int,
       }
   }
 
   # pylint: disable=attribute-defined-outside-init,too-many-locals
   # pylint: disable=too-many-statements,too-many-branches
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     super().parse_fields(bfr)
     self.tags = TagSet()
     for subbox in self.boxes:
       subbox_type = bytes(subbox.box_type)
       with Pfx("subbox %r", subbox_type):
         with subbox.reparse_buffer() as subbfr:
           subbox.parse_boxes(subbfr)
@@ -2548,15 +2528,15 @@
                 data_box.parse_field_value('text', databfr, _ILSTUTF8Text)
               value = data_box.text
               subsubbox_schema = self.SUBSUBBOX_SCHEMA.get(mean_box.text, {})
               decoder = subsubbox_schema.get(name_box.text)
               if decoder is not None:
                 value = decoder(value)
               # annotate the subbox and the ilst
-              attribute_name = '.'.join((mean_box.text, name_box.text))
+              attribute_name = f'{mean_box.text}.{name_box.text}'
               setattr(subbox, attribute_name, value)
               self.tags.add(attribute_name, value)
         else:
           # single data box
           if not inner_boxes:
             warning("no inner boxes, expected 1 data box")
           else:
@@ -2593,73 +2573,74 @@
                           attribute_name,
                           b64encode(tag_value).decode('ascii')
                       )
                     else:
                       self.tags.add(attribute_name, tag_value)
 
   def __getattr__(self, attr):
+    # see if this is a schema long name
     for schema_code, schema in self.SUBBOX_SCHEMA.items():
       if schema.attribute_name == attr:
         subbox_attr = schema_code.decode('iso8859-1').upper()
-        subbox = getattr(self, subbox_attr)
-        return None
+        with Pfx(
+            "%s.%s: schema:%r: self.%s",
+            self.__class__.__name__,
+            attr,
+            schema_code,
+            subbox_attr,
+        ):
+          return getattr(self, subbox_attr)
     return super().__getattr__(attr)
 
-add_body_class(ILSTBoxBody)
-
 class VMHDBoxBody(FullBoxBody):
   ''' A 'vmhd' Video Media Headerbox - section 12.1.2.
   '''
 
   OpColor = BinaryMultiStruct('OpColor', '>HHH', 'red green blue')
 
   FIELD_TYPES = dict(
       FullBoxBody.FIELD_TYPES,
       graphicsmode=UInt16BE,
       opcolor=OpColor,
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `graphicsmode` and `opcolor` fields.
     '''
     super().parse_fields(bfr)
     self.parse_field('graphicsmode', bfr, UInt16BE)
     self.parse_field('opcolor', bfr, VMHDBoxBody.OpColor)
 
   def transcribe(self):
     yield super().transcribe()
     yield self.graphicsmode
     yield self.opcolor
 
-add_body_class(VMHDBoxBody)
-
 class SMHDBoxBody(FullBoxBody):
   ''' A 'smhd' Sound Media Headerbox - section 12.2.2.
   '''
 
   FIELD_TYPES = dict(
       FullBoxBody.FIELD_TYPES,
       balance=Int16BE,
       reserved=UInt16BE,
   )
 
-  def parse_fields(self, bfr):
+  def parse_fields(self, bfr: CornuCopyBuffer):
     ''' Gather the `balance` field.
     '''
     super().parse_fields(bfr)
     self.parse_field('balance', bfr, Int16BE)
     self.parse_field('reserved', bfr, UInt16BE)
 
   def transcribe(self):
     yield super().transcribe()
     yield self.balance
     yield self.reserved
 
-add_body_class(SMHDBoxBody)
-
 def parse_tags(path, tag_prefix=None):
   ''' Parse the tags from `path`.
       Yield `(box,tags)` for each subbox with tags.
 
       The optional `tag_prefix` parameter
       may be specified to prefix each tag name with a prefix.
       Other keyword arguments are passed to `parse()`
@@ -2709,15 +2690,15 @@
   ''' Parse an ISO14496 stream from the CornuCopyBuffer `bfr`,
       yield top level OverBoxes.
 
       Parameters:
       * `bfr`: a `CornuCopyBuffer` provided the stream data,
         preferably seekable
       * `discard_data`: whether to discard unparsed data, default `False`
-      * `copy_offsets`: callable to receive Box offsets
+      * `copy_offsets`: callable to receive `Box` offsets
   '''
   if copy_offsets is not None:
     bfr.copy_offsets = copy_offsets
   yield from OverBox.scan(bfr, **kw)
 
 # pylint: disable=too-many-branches
 def dump_box(B, indent='', fp=None, crop_length=170, indent_incr=None):
```

