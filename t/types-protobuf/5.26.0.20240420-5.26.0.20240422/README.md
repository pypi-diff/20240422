# Comparing `tmp/types-protobuf-5.26.0.20240420.tar.gz` & `tmp/types-protobuf-5.26.0.20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-protobuf-5.26.0.20240420.tar", last modified: Sat Apr 20 02:14:57 2024, max compression
+gzip compressed data, was "types-protobuf-5.26.0.20240422.tar", last modified: Mon Apr 22 02:18:58 2024, max compression
```

## Comparing `types-protobuf-5.26.0.20240420.tar` & `types-protobuf-5.26.0.20240422.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:57.876143 types-protobuf-5.26.0.20240420/
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-20 02:14:57.000000 types-protobuf-5.26.0.20240420/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 02:14:57.000000 types-protobuf-5.26.0.20240420/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-20 02:14:57.876143 types-protobuf-5.26.0.20240420/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:57.868143 types-protobuf-5.26.0.20240420/google-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-20 02:14:57.000000 types-protobuf-5.26.0.20240420/google-stubs/METADATA.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:57.872143 types-protobuf-5.26.0.20240420/google-stubs/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/any_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/api_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:57.872143 types-protobuf-5.26.0.20240420/google-stubs/protobuf/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/compiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14146 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/compiler/plugin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/descriptor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   105621 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/descriptor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/descriptor_pool.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/duration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/field_mask_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:57.876143 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/api_implementation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/builder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/enum_type_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/extension_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/message_listener.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/python_message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/type_checkers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/well_known_types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/wire_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/json_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/message_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 02:14:57.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/reflection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/source_context_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/symbol_database.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/text_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/timestamp_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/type_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:57.876143 types-protobuf-5.26.0.20240420/google-stubs/protobuf/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-20 02:14:41.000000 types-protobuf-5.26.0.20240420/google-stubs/protobuf/wrappers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 02:14:57.876143 types-protobuf-5.26.0.20240420/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-20 02:14:57.000000 types-protobuf-5.26.0.20240420/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:14:57.876143 types-protobuf-5.26.0.20240420/types_protobuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-20 02:14:57.000000 types-protobuf-5.26.0.20240420/types_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-20 02:14:57.000000 types-protobuf-5.26.0.20240420/types_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:14:57.000000 types-protobuf-5.26.0.20240420/types_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 02:14:57.000000 types-protobuf-5.26.0.20240420/types_protobuf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:58.500899 types-protobuf-5.26.0.20240422/
+-rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-04-22 02:18:57.000000 types-protobuf-5.26.0.20240422/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 02:18:57.000000 types-protobuf-5.26.0.20240422/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-22 02:18:58.500899 types-protobuf-5.26.0.20240422/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:58.492899 types-protobuf-5.26.0.20240422/google-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-22 02:18:57.000000 types-protobuf-5.26.0.20240422/google-stubs/METADATA.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:58.496899 types-protobuf-5.26.0.20240422/google-stubs/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/any_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/api_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:58.496899 types-protobuf-5.26.0.20240422/google-stubs/protobuf/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/compiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14146 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/compiler/plugin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/descriptor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   105621 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/descriptor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/descriptor_pool.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/duration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/field_mask_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:58.500899 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/api_implementation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/builder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/enum_type_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/extension_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/message_listener.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/python_message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/type_checkers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/well_known_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/wire_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/json_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/message_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 02:18:57.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/reflection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/source_context_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/symbol_database.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/text_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/timestamp_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/type_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:58.500899 types-protobuf-5.26.0.20240422/google-stubs/protobuf/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-22 02:18:48.000000 types-protobuf-5.26.0.20240422/google-stubs/protobuf/wrappers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 02:18:58.500899 types-protobuf-5.26.0.20240422/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-22 02:18:57.000000 types-protobuf-5.26.0.20240422/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:18:58.500899 types-protobuf-5.26.0.20240422/types_protobuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-22 02:18:58.000000 types-protobuf-5.26.0.20240422/types_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-22 02:18:58.000000 types-protobuf-5.26.0.20240422/types_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 02:18:58.000000 types-protobuf-5.26.0.20240422/types_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 02:18:58.000000 types-protobuf-5.26.0.20240422/types_protobuf.egg-info/top_level.txt
```

### Comparing `types-protobuf-5.26.0.20240420/CHANGELOG.md` & `types-protobuf-5.26.0.20240422/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 5.26.0.20240422 (2024-04-22)
+
+Simplify protoc install in protobuf generation scripts (#11785)
+
 ## 5.26.0.20240420 (2024-04-20)
 
 Bump protobuf to 5.26.* (#11784)
 
 Also update generate_proto_stubs script
 
 ## 4.25.0.20240417 (2024-04-17)
```

### Comparing `types-protobuf-5.26.0.20240420/PKG-INFO` & `types-protobuf-5.26.0.20240422/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 5.26.0.20240420
+Version: 5.26.0.20240422
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,17 +27,17 @@
 
 This version of `types-protobuf` aims to provide accurate annotations
 for `protobuf==5.26.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/protobuf. All fixes for
 types and metadata should be contributed there.
 
-Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on [protobuf v26.1](https://github.com/protocolbuffers/protobuf/releases/tag/v26.1) (python protobuf==5.26.1)
+Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on [protobuf v26.1](https://github.com/protocolbuffers/protobuf/releases/tag/v26.1) (python protobuf==5.26.1)
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+This package was generated from typeshed commit `1017c525f84b5e78a75ad909c6a4ef2b5c0610e6` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/any_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/any_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/api_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/compiler/plugin_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/compiler/plugin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/descriptor.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/descriptor.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/descriptor_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/descriptor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/descriptor_pool.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/descriptor_pool.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/duration_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/duration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/empty_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/field_mask_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/field_mask_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/containers.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/decoder.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/encoder.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/enum_type_wrapper.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/enum_type_wrapper.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/extension_dict.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/extension_dict.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/well_known_types.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/well_known_types.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/internal/wire_format.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/internal/wire_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/json_format.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/json_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/message.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/message.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/message_factory.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/message_factory.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/service.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/service.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/source_context_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/source_context_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/struct_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/struct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/symbol_database.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/symbol_database.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/text_format.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/text_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/timestamp_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/timestamp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/type_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/google-stubs/protobuf/wrappers_pb2.pyi` & `types-protobuf-5.26.0.20240422/google-stubs/protobuf/wrappers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-5.26.0.20240420/setup.py` & `types-protobuf-5.26.0.20240422/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 
 This version of `types-protobuf` aims to provide accurate annotations
 for `protobuf==5.26.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/protobuf. All fixes for
 types and metadata should be contributed there.
 
-Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on [protobuf v26.1](https://github.com/protocolbuffers/protobuf/releases/tag/v26.1) (python protobuf==5.26.1)
+Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on [protobuf v26.1](https://github.com/protocolbuffers/protobuf/releases/tag/v26.1) (python protobuf==5.26.1)
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+This package was generated from typeshed commit `1017c525f84b5e78a75ad909c6a4ef2b5c0610e6` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="5.26.0.20240420",
+      version="5.26.0.20240422",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md",
```

### Comparing `types-protobuf-5.26.0.20240420/types_protobuf.egg-info/PKG-INFO` & `types-protobuf-5.26.0.20240422/types_protobuf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 5.26.0.20240420
+Version: 5.26.0.20240422
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,17 +27,17 @@
 
 This version of `types-protobuf` aims to provide accurate annotations
 for `protobuf==5.26.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/protobuf. All fixes for
 types and metadata should be contributed there.
 
-Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on [protobuf v26.1](https://github.com/protocolbuffers/protobuf/releases/tag/v26.1) (python protobuf==5.26.1)
+Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on [protobuf v26.1](https://github.com/protocolbuffers/protobuf/releases/tag/v26.1) (python protobuf==5.26.1)
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+This package was generated from typeshed commit `1017c525f84b5e78a75ad909c6a4ef2b5c0610e6` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-protobuf-5.26.0.20240420/types_protobuf.egg-info/SOURCES.txt` & `types-protobuf-5.26.0.20240422/types_protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

