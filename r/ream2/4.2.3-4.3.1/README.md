# Comparing `tmp/ream2-4.2.3.tar.gz` & `tmp/ream2-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ream2-4.2.3.tar", max compression
+gzip compressed data, was "ream2-4.3.1.tar", max compression
```

## Comparing `ream2-4.2.3.tar` & `ream2-4.3.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1064 2024-03-01 19:31:57.840964 ream2-4.2.3/LICENSE
--rw-r--r--   0        0        0     5267 2024-03-01 19:31:57.840964 ream2-4.2.3/README.md
--rw-r--r--   0        0        0      800 2024-03-01 19:31:57.840964 ream2-4.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-01 19:31:57.840964 ream2-4.2.3/ream/__init__.py
--rw-r--r--   0        0        0    16604 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/actor_graph.py
--rw-r--r--   0        0        0     2369 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/actor_state.py
--rw-r--r--   0        0        0     2040 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/actor_version.py
--rw-r--r--   0        0        0        0 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/actors/__init__.py
--rw-r--r--   0        0        0     6238 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/actors/base.py
--rw-r--r--   0        0        0     1683 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/actors/dsid.py
--rw-r--r--   0        0        0     1340 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/actors/enum.py
--rw-r--r--   0        0        0      363 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/actors/interface.py
--rw-r--r--   0        0        0    44945 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/cache_helper.py
--rw-r--r--   0        0        0     3393 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/cli_helper.py
--rw-r--r--   0        0        0     1197 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/data_model_helper/__init__.py
--rw-r--r--   0        0        0     3481 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/data_model_helper/_batch_file_manager.py
--rw-r--r--   0        0        0     2294 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/data_model_helper/_container.py
--rw-r--r--   0        0        0      582 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/data_model_helper/_index.py
--rw-r--r--   0        0        0    34039 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/data_model_helper/_numpy_model.py
--rw-r--r--   0        0        0     7533 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/data_model_helper/_polars_model.py
--rw-r--r--   0        0        0     1409 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/data_model_helper/_raw_model.py
--rw-r--r--   0        0        0    15796 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/dataset_helper.py
--rw-r--r--   0        0        0    13815 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/fs.py
--rw-r--r--   0        0        0     8713 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/helper.py
--rw-r--r--   0        0        0     7193 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/params_helper.py
--rw-r--r--   0        0        0     1169 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/prelude.py
--rw-r--r--   0        0        0        0 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/py.typed
--rw-r--r--   0        0        0     4114 2024-03-01 19:31:57.844964 ream2-4.2.3/ream/workspace.py
--rw-r--r--   0        0        0     6386 1970-01-01 00:00:00.000000 ream2-4.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-21 22:34:58.559390 ream2-4.3.1/LICENSE
+-rw-r--r--   0        0        0     5267 2024-04-21 22:34:58.559390 ream2-4.3.1/README.md
+-rw-r--r--   0        0        0      820 2024-04-21 22:34:58.559390 ream2-4.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-21 22:34:58.559390 ream2-4.3.1/ream/__init__.py
+-rw-r--r--   0        0        0    16604 2024-04-21 22:34:58.559390 ream2-4.3.1/ream/actor_graph.py
+-rw-r--r--   0        0        0     2369 2024-04-21 22:34:58.559390 ream2-4.3.1/ream/actor_state.py
+-rw-r--r--   0        0        0     2040 2024-04-21 22:34:58.559390 ream2-4.3.1/ream/actor_version.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:34:58.559390 ream2-4.3.1/ream/actors/__init__.py
+-rw-r--r--   0        0        0     6238 2024-04-21 22:34:58.559390 ream2-4.3.1/ream/actors/base.py
+-rw-r--r--   0        0        0     1683 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/actors/dsid.py
+-rw-r--r--   0        0        0     1340 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/actors/enum.py
+-rw-r--r--   0        0        0      363 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/actors/interface.py
+-rw-r--r--   0        0        0    46618 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/cache_helper.py
+-rw-r--r--   0        0        0     3393 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/cli_helper.py
+-rw-r--r--   0        0        0     1433 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/data_model_helper/__init__.py
+-rw-r--r--   0        0        0     3481 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/data_model_helper/_batch_file_manager.py
+-rw-r--r--   0        0        0     2294 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/data_model_helper/_container.py
+-rw-r--r--   0        0        0      582 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/data_model_helper/_index.py
+-rw-r--r--   0        0        0    38154 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/data_model_helper/_numpy_model.py
+-rw-r--r--   0        0        0      946 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/data_model_helper/_pandas_model.py
+-rw-r--r--   0        0        0     7533 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/data_model_helper/_polars_model.py
+-rw-r--r--   0        0        0     1409 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/data_model_helper/_raw_model.py
+-rw-r--r--   0        0        0    15796 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/dataset_helper.py
+-rw-r--r--   0        0        0    15333 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/fs.py
+-rw-r--r--   0        0        0     8774 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/helper.py
+-rw-r--r--   0        0        0     7193 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/params_helper.py
+-rw-r--r--   0        0        0     1169 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/prelude.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/py.typed
+-rw-r--r--   0        0        0     4114 2024-04-21 22:34:58.563390 ream2-4.3.1/ream/workspace.py
+-rw-r--r--   0        0        0     6427 1970-01-01 00:00:00.000000 ream2-4.3.1/PKG-INFO
```

### Comparing `ream2-4.2.3/LICENSE` & `ream2-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/README.md` & `ream2-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/actor_graph.py` & `ream2-4.3.1/ream/actor_graph.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/actor_state.py` & `ream2-4.3.1/ream/actor_state.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/actor_version.py` & `ream2-4.3.1/ream/actor_version.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/actors/base.py` & `ream2-4.3.1/ream/actors/base.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/actors/dsid.py` & `ream2-4.3.1/ream/actors/dsid.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/actors/enum.py` & `ream2-4.3.1/ream/actors/enum.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/cache_helper.py` & `ream2-4.3.1/ream/cache_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from __future__ import annotations
 
 import bz2
+import csv
 import gzip
 import pickle
 import weakref
 from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from contextlib import contextmanager
 from dataclasses import fields
 from functools import lru_cache, partial, wraps
 from inspect import Parameter, signature
+from io import StringIO
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Generic,
     Iterable,
     Literal,
     Optional,
     Protocol,
     Sequence,
     Type,
     TypeVar,
     Union,
+    cast,
     get_args,
     get_origin,
     get_type_hints,
 )
 
 import orjson
+import serde.csv
 from hugedict.misc import Chain2, identity
 from hugedict.sqlite import SqliteDict, SqliteDictFieldType
 from loguru import logger
 from ream.data_model_helper import DataSerdeMixin
 from ream.fs import FS
 from ream.helper import Compression, ContextContainer, orjson_dumps
 from serde.helper import DEFAULT_ORJSON_OPTS, JsonSerde, _orjson_default, orjson_dumps
@@ -79,23 +83,27 @@
         compression: Optional[Compression] = None,
         mem_persist: Optional[Union[MemBackend, bool]] = None,
         log_serde_time: bool = False,
         cls: Optional[Type[JsonSerde]] = None,
         indent: Literal[0, 2] = 0,
     ):
         backend = SqliteBackend(
-            ser=partial(
-                FileBackendFactory.json_ser,
-                orjson_opts=DEFAULT_ORJSON_OPTS | orjson.OPT_INDENT_2,
-            )
-            if indent == 2
-            else FileBackendFactory.json_ser,
-            deser=FileBackendFactory.json_deser
-            if cls is None
-            else partial(FileBackendFactory.json_deser_cls, cls),
+            ser=(
+                partial(
+                    FileBackendFactory.json_ser,
+                    orjson_opts=DEFAULT_ORJSON_OPTS | orjson.OPT_INDENT_2,
+                )
+                if indent == 2
+                else FileBackendFactory.json_ser
+            ),
+            deser=(
+                FileBackendFactory.json_deser
+                if cls is None
+                else partial(FileBackendFactory.json_deser_cls, cls)
+            ),
             compression=compression,
         )
         return wrap_backend(backend, mem_persist, log_serde_time)
 
 
 class ClsSerdeBackendFactory:
     """A cache that uses the save/load methods of a class as deser/ser functions."""
@@ -213,26 +221,45 @@
             filename=filename,
             fileext="pkl",
             compression=compression,
         )
         return wrap_backend(backend, mem_persist, log_serde_time)
 
     @staticmethod
+    def csv(
+        filename: Optional[Union[str, Callable[..., str]]] = None,
+        delimiter: str = ",",
+        compression: Optional[Compression] = None,
+        mem_persist: Optional[Union[MemBackend, bool]] = None,
+        log_serde_time: bool = False,
+    ):
+        backend = FileBackend(
+            ser=FileBackendFactory.csv_ser,
+            deser=FileBackendFactory.csv_deser,
+            filename=filename,
+            fileext="csv",
+            compression=compression,
+        )
+        return wrap_backend(backend, mem_persist, log_serde_time)
+
+    @staticmethod
     def jl(
         filename: Optional[Union[str, Callable[..., str]]] = None,
         compression: Optional[Compression] = None,
         mem_persist: Optional[Union[MemBackend, bool]] = None,
         cls: Optional[Type[JsonSerde]] = None,
         log_serde_time: bool = False,
     ):
         backend = FileBackend(
             ser=FileBackendFactory.jl_ser,
-            deser=FileBackendFactory.jl_deser
-            if cls is None
-            else partial(FileBackendFactory.jl_deser_cls, cls),
+            deser=(
+                FileBackendFactory.jl_deser
+                if cls is None
+                else partial(FileBackendFactory.jl_deser_cls, cls)
+            ),
             filename=filename,
             fileext="jl",
             compression=compression,
         )
         return wrap_backend(backend, mem_persist, log_serde_time)
 
     @staticmethod
@@ -241,23 +268,27 @@
         compression: Optional[Compression] = None,
         mem_persist: Optional[Union[MemBackend, bool]] = None,
         cls: Optional[Type[JsonSerde]] = None,
         log_serde_time: bool = False,
         indent: Literal[0, 2] = 0,
     ):
         backend = FileBackend(
-            ser=partial(
-                FileBackendFactory.json_ser,
-                orjson_opts=DEFAULT_ORJSON_OPTS | orjson.OPT_INDENT_2,
-            )
-            if indent == 2
-            else FileBackendFactory.json_ser,
-            deser=FileBackendFactory.json_deser
-            if cls is None
-            else partial(FileBackendFactory.json_deser_cls, cls),
+            ser=(
+                partial(
+                    FileBackendFactory.json_ser,
+                    orjson_opts=DEFAULT_ORJSON_OPTS | orjson.OPT_INDENT_2,
+                )
+                if indent == 2
+                else FileBackendFactory.json_ser
+            ),
+            deser=(
+                FileBackendFactory.json_deser
+                if cls is None
+                else partial(FileBackendFactory.json_deser_cls, cls)
+            ),
             filename=filename,
             fileext="json",
             compression=compression,
         )
         return wrap_backend(backend, mem_persist, log_serde_time)
 
     @staticmethod
@@ -284,14 +315,43 @@
         return orjson.loads(data)
 
     @staticmethod
     def json_deser_cls(clz: Type[JsonSerde], data: bytes):
         return clz.from_dict(orjson.loads(data))
 
     @staticmethod
+    def csv_ser(
+        obj: list[dict[str, str]] | list[list[str]],
+        delimiter: str = ",",
+    ):
+        if len(obj) == 0:
+            return b""
+
+        f = StringIO()
+        writer = csv.writer(
+            f, delimiter=delimiter, quoting=csv.QUOTE_MINIMAL, lineterminator="\n"
+        )
+
+        if isinstance(obj[0], dict):
+            keys = list(obj[0].keys())
+            writer.writerow(keys)
+            for row in cast(list[dict[str, str]], obj):
+                writer.writerow((row[key] for key in keys))
+        else:
+            for row in obj:
+                writer.writerow(row)
+        return f.getvalue().encode()
+
+    @staticmethod
+    def csv_deser(data: bytes, delimiter: str = ","):
+        f = StringIO(data.decode())
+        reader = csv.reader(f, delimiter=delimiter)
+        return list(reader)
+
+    @staticmethod
     def jl_ser(
         objs: Sequence[dict] | Sequence[tuple] | Sequence[list] | Sequence[JsonSerde],
         orjson_opts: int | None = DEFAULT_ORJSON_OPTS,
         orjson_default: Callable[[Any], Any] | None = None,
     ):
         out = []
         if len(objs) > 0 and hasattr(objs[0], "to_dict"):
@@ -772,24 +832,21 @@
             raise RuntimeError("Backend can only be postinited once")
 
     @contextmanager
     def context(self, obj: HasWorkingFsTrait, *args, **kwargs):
         yield None
 
     @abstractmethod
-    def has_key(self, key: bytes) -> bool:
-        ...
+    def has_key(self, key: bytes) -> bool: ...
 
     @abstractmethod
-    def get(self, key: bytes) -> Value:
-        ...
+    def get(self, key: bytes) -> Value: ...
 
     @abstractmethod
-    def set(self, key: bytes, value: Value) -> None:
-        ...
+    def set(self, key: bytes, value: Value) -> None: ...
 
 
 class MemBackend(Backend):
     """A backend that caches in memory.
 
     Note that due to the design of the `Cache.cache` function, this backend is shared
     across instances of the same class because the backend instance is tied to the
@@ -1126,16 +1183,15 @@
         ):
             self.backend.set(key, value)
 
 
 class HasWorkingFsTrait(Protocol):
     logger: Logger
 
-    def get_working_fs(self) -> FS:
-        ...
+    def get_working_fs(self) -> FS: ...
 
 
 class Cacheable:
     """A class that implement HasWorkingFSTrait so it can be used with @Cache.file decorator.
 
     Args:
         workdir: directory to store cached files.
@@ -1206,20 +1262,18 @@
 def assign_dataclass_field_names(cls: type[T]):
     """Set back the fields of the dataclass to be the same as the name of the fields so they can use T.<field> as the field name"""
     for field in fields(cls):
         setattr(cls, field.name, field.name)
 
 
 class SerdeProtocol(Protocol):
-    def ser(self) -> bytes:
-        ...
+    def ser(self) -> bytes: ...
 
     @classmethod
-    def deser(cls, data: bytes) -> Self:
-        ...
+    def deser(cls, data: bytes) -> Self: ...
 
 
 def unwrap_cache_decorators(cls: type, methods: list[str] | None = None):
     """Decorator to disable caching decorator by unwrap all methods of a class."""
     for method in methods or dir(cls):
         fn = getattr(cls, method)
         iswrapped = hasattr(fn, "__wrapped__")
```

### Comparing `ream2-4.2.3/ream/cli_helper.py` & `ream2-4.3.1/ream/cli_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/data_model_helper/__init__.py` & `ream2-4.3.1/ream/data_model_helper/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from ream.data_model_helper._container import DataContainer, DataSerdeMixin
 from ream.data_model_helper._index import Index, OffsetIndex
 from ream.data_model_helper._numpy_model import (
     ContiguousIndexChecker,
     DictNumpyArray,
+    EncodedSingleMasked2DNumpyArray,
+    EncodedSingleNumpyArray,
     NumpyDataModel,
     NumpyDataModelContainer,
     NumpyDataModelHelper,
     NumpyDataModelMetadata,
     Single2DNumpyArray,
     SingleLevelIndexedNumpyArray,
     SingleNumpyArray,
     deser_dict_array,
     ser_dict_array,
 )
+from ream.data_model_helper._pandas_model import SinglePandasDataFrame
 from ream.data_model_helper._polars_model import (
     PolarDataModel,
     PolarDataModelMetadata,
     SingleLevelIndexedPLDataFrame,
     SinglePolarDataFrame,
 )
 from ream.data_model_helper._raw_model import DictList
@@ -29,14 +32,17 @@
     "NumpyDataModel",
     "NumpyDataModelContainer",
     "NumpyDataModelHelper",
     "NumpyDataModelMetadata",
     "ContiguousIndexChecker",
     "Single2DNumpyArray",
     "SingleNumpyArray",
+    "EncodedSingleNumpyArray",
+    "EncodedSingleMasked2DNumpyArray",
+    "SinglePandasDataFrame",
     "DictNumpyArray",
     "SingleLevelIndexedNumpyArray",
     "PolarDataModel",
     "PolarDataModelMetadata",
     "SingleLevelIndexedPLDataFrame",
     "SinglePolarDataFrame",
     "DictList",
```

### Comparing `ream2-4.2.3/ream/data_model_helper/_batch_file_manager.py` & `ream2-4.3.1/ream/data_model_helper/_batch_file_manager.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/data_model_helper/_container.py` & `ream2-4.3.1/ream/data_model_helper/_container.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/data_model_helper/_index.py` & `ream2-4.3.1/ream/data_model_helper/_index.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/data_model_helper/_numpy_model.py` & `ream2-4.3.1/ream/data_model_helper/_numpy_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import pickle
 import struct
 from copy import deepcopy
-from dataclasses import dataclass, fields, is_dataclass
+from dataclasses import dataclass, field, fields, is_dataclass
+from functools import partial
 from pathlib import Path
 from typing import (
+    Any,
     Callable,
     List,
     Literal,
+    Mapping,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
     get_origin,
@@ -23,15 +26,15 @@
 import orjson
 import pyarrow as pa
 import pyarrow.parquet as pq
 import serde.json
 from nptyping import NDArray, Shape
 from nptyping.ndarray import NDArrayMeta  # type: ignore
 from nptyping.shape_expression import get_dimensions  # type: ignore
-from nptyping.typing_ import Number
+from nptyping.typing_ import Bool, Int32, Number
 from ream.data_model_helper._batch_file_manager import BatchFileManager, VirtualDir
 from ream.data_model_helper._container import DataSerdeMixin
 from ream.data_model_helper._index import Index, OffsetIndex
 from ream.helper import (
     Compression,
     get_classpath,
     has_dict_with_nonstr_keys,
@@ -131,15 +134,15 @@
                                 useorjson = False
                     elif ann_origin is not type(None):
                         raise ValueError(
                             f"Value of attribute {name} is not numpy array or index or NoneType"
                         )
 
             if useorjson:
-                default_serdict = orjson.dumps
+                default_serdict = partial(orjson.dumps, option=orjson.OPT_NON_STR_KEYS)
                 default_deserdict = orjson.loads
             else:
                 default_serdict = pickle.dumps
                 default_deserdict = pickle.loads
 
             cls._metadata = NumpyDataModelMetadata(
                 cls=cls,
@@ -219,15 +222,15 @@
         kind: Literal["stable", "quicksort"] = "stable",
     ):
         """Sort the elements between [i, j).
         Note: This operator mutates the array
         """
         metadata: NumpyDataModelMetadata = self._metadata  # type: ignore
         sortedvalue = getattr(self, sortby)
-        sortedindex = np.argsort(sortedvalue, kind=kind)
+        sortedindex = np.argsort(sortedvalue[i:j], kind=kind)
         if sortorder == "desc":
             sortedindex = sortedindex[::-1]
 
         for field in metadata.array_props:
             value = getattr(self, field)
             value[i:j] = value[i:j][sortedindex]
 
@@ -787,56 +790,152 @@
 
         return index
 
 
 class SingleNumpyArray(NumpyDataModel):
     __slots__ = ["value"]
 
-    value: NDArray[Shape["*"], Number]
+    value: NDArray[Shape["*"], Any]
 
-    def __init__(self, value: NDArray[Shape["*"], Number]):
+    def __init__(self, value: NDArray[Shape["*"], Any]):
         self.value = value
 
+    def __getitem__(self, idx: int | slice):
+        if not isinstance(idx, int):
+            return self.__class__(self.value[idx])
+        return self.value[idx]
+
+
+class EncodedSingleNumpyArray(NumpyDataModel):
+    __slots__ = ["decoder", "value"]
+
+    decoder: list[str]
+    value: NDArray[Shape["*"], Int32]
+
+    def __init__(self, decoder: list[str], value: NDArray[Shape["*"], Int32]):
+        self.decoder = decoder
+        self.value = value
+
+    def __getitem__(self, idx: int | slice):
+        if not isinstance(idx, int):
+            return self.__class__(self.decoder, self.value[idx])
+        return self.value[idx]
+
+    @staticmethod
+    def from_array(arr, encoder: Optional[dict[str, int]] = None):
+        encoder = encoder or {}
+        new_arr = []
+        for val in arr:
+            if val not in encoder:
+                encoder[val] = len(encoder)
+            new_arr.append(encoder[val])
+
+        return EncodedSingleNumpyArray(get_decoder(encoder), np.array(new_arr))
+
+    @staticmethod
+    def from_lst_arrays(arr, encoder: Optional[dict[str, int]] = None):
+        encoder = encoder or {}
+        new_arr = np.empty((len(arr),), dtype=np.object_)
+        for i, lst in enumerate(arr):
+            new_lst = []
+            for val in lst:
+                if val not in encoder:
+                    encoder[val] = len(encoder)
+                new_lst.append(encoder[val])
+            new_arr[i] = np.array(new_lst)
+
+        return EncodedSingleNumpyArray(get_decoder(encoder), new_arr)
+
+    @staticmethod
+    def from_known_size_integer_encoder(int_encoder: KnownSizeIntegerEncoder):
+        return EncodedSingleNumpyArray(int_encoder.get_decoder(), int_encoder.values)
+
+    def to_list(self):
+        return [self.decoder[val] for val in self.value]
+
 
 class Single2DNumpyArray(NumpyDataModel):
     __slots__ = ["value"]
 
-    value: NDArray[Shape["*,*"], Number]
+    value: NDArray[Shape["*,*"], Any]
 
-    def __init__(self, value: NDArray[Shape["*,*"], Number]):
+    def __init__(self, value: NDArray[Shape["*,*"], Any]):
         self.value = value
 
+    def __getitem__(self, idx: int | slice):
+        if not isinstance(idx, int):
+            return self.__class__(self.value[idx])
+        return self.value[idx]
+
 
 @dataclass
 class SingleLevelIndexedNumpyArray(NumpyDataModel):
     __slots__ = ["index", "value"]
 
     index: dict[str, tuple[int, int]]
-    value: NDArray[Shape["*,*"], Number]
+    value: NDArray[Shape["*"], Any]
 
     def __init__(
-        self, index: dict[str, tuple[int, int]], value: NDArray[Shape["*,*"], Number]
+        self, index: dict[str, tuple[int, int]], value: NDArray[Shape["*"], Any]
     ):
         self.index = index
         self.value = value
 
-    def get_array(self, key: str) -> NDArray[Shape["*"], Number]:
+    def get_array(self, key: str) -> NDArray[Shape["*"], Any]:
         start, end = self.index[key]
         return self.value[start:end]
 
 
+class EncodedSingleMasked2DNumpyArray(NumpyDataModel):
+    __slots__ = ["decoder", "value", "mask"]
+
+    decoder: list[str]
+    value: NDArray[Shape["*,*"], Int32]
+    mask: NDArray[Shape["*,*"], Bool]
+
+    def __init__(
+        self,
+        decoder: list[str],
+        value: NDArray[Shape["*,*"], Int32],
+        mask: NDArray[Shape["*,*"], Bool],
+    ):
+        self.decoder = decoder
+        self.value = value
+        self.mask = mask
+
+    def __getitem__(self, idx: int | slice):
+        if not isinstance(idx, int):
+            return self.__class__(self.decoder, self.value[idx], self.mask[idx])
+        return self.value[idx], self.mask[idx]
+
+    @staticmethod
+    def from_list_arrays(arr, encoder: Optional[dict[str, int]] = None):
+        encoder = encoder or {}
+        ncols = max(len(x) for x in arr)
+        new_arr = np.zeros((len(arr), ncols), dtype=np.int32)
+        mask = np.ones(new_arr.shape, dtype=np.bool_)
+        for i, lst in enumerate(arr):
+            for j, val in enumerate(lst):
+                if val not in encoder:
+                    encoder[val] = len(encoder)
+                new_arr[i, j] = encoder[val]
+            mask[i, len(lst) :] = False
+
+        return EncodedSingleMasked2DNumpyArray(get_decoder(encoder), new_arr, mask)
+
+
 class DictNumpyArray(NumpyDataModel):
     __slots__ = ["value"]
 
-    value: dict[str, NDArray[Shape["*"], Number]]
+    value: dict[str, NDArray[Shape["*"], Any]]
 
-    def __init__(self, value: dict[str, NDArray[Shape["*"], Number]]):
+    def __init__(self, value: dict[str, NDArray[Shape["*"], Any]]):
         self.value = value
 
-    def __getitem__(self, item: str) -> NDArray[Shape["*"], Number]:
+    def __getitem__(self, item: str) -> NDArray[Shape["*"], Any]:
         return self.value[item]
 
     def save(
         self,
         loc: Path,
         compression: Optional[Compression] = None,
         compression_level: Optional[int] = None,
@@ -857,31 +956,33 @@
         for name in columns:
             kwargs[name] = tbl.column(name).to_numpy()
         return cls(kwargs)
 
 
 SingleLevelIndexedNumpyArray.init()
 SingleNumpyArray.init()
+EncodedSingleNumpyArray.init()
+EncodedSingleMasked2DNumpyArray.init()
 Single2DNumpyArray.init()
 DictNumpyArray.init()
 
 
 def ser_dict_array(
-    odict: dict[str, NumpyDataModel],
+    odict: Mapping[str, DataSerdeMixin],
     loc: Path,
-    compression: Optional[Compression],
+    compression: Optional[Compression] = None,
 ):
     classes = {}
     for key, value in odict.items():
         value.save(loc / key, compression)
         classes[key] = get_classpath(value.__class__)
     serde.json.ser(classes, loc / "metadata.json")
 
 
-def deser_dict_array(loc: Path, compression: Optional[Compression]):
+def deser_dict_array(loc: Path, compression: Optional[Compression] = None):
     classes = serde.json.deser(loc / "metadata.json")
     objects = {}
     for key, cls in classes.items():
         objects[key] = import_attr(cls).load(loc / key, compression)
     return objects
 
 
@@ -900,7 +1001,34 @@
         "lz4": "LZ4",
         "zstd": "ZSTD",
     }
     if compression in map:
         return map[compression]
 
     raise Exception(f"Not supported compression: {compression}")
+
+
+V = TypeVar("V")
+
+
+class KnownSizeIntegerEncoder:
+    def __init__(self, encoder: dict[str | tuple[str, ...], int], size: int):
+        self.encoder = encoder
+        self.values = np.zeros(size, dtype=np.int32)
+
+    def __setitem__(self, idx: int | slice, val: str | tuple[str, ...]):
+        if val not in self.encoder:
+            self.encoder[val] = len(self.encoder)
+        self.values[idx] = self.encoder[val]
+
+    def get_decoder(self) -> list:
+        return get_decoder(self.encoder)
+
+
+def get_decoder(encoder: dict[V, int]) -> list[V]:
+    counter = 0
+    output = []
+    for key, val in encoder.items():
+        assert val == counter, (val, counter)
+        counter += 1
+        output.append(key)
+    return output
```

### Comparing `ream2-4.2.3/ream/data_model_helper/_polars_model.py` & `ream2-4.3.1/ream/data_model_helper/_polars_model.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/data_model_helper/_raw_model.py` & `ream2-4.3.1/ream/data_model_helper/_raw_model.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/dataset_helper.py` & `ream2-4.3.1/ream/dataset_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/fs.py` & `ream2-4.3.1/ream/fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import os
 import pickle
 import shutil
 import sqlite3
 from contextlib import contextmanager
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Generator, Optional, Union
+from random import choice, choices
+from typing import Generator, Literal, Optional, Union
 from zipfile import ZipFile
 
 import orjson
 import serde.pickle
 from filelock import FileLock
 from loguru import logger
 from ream.helper import orjson_dumps
@@ -117,15 +118,15 @@
         """Export the following FS"""
         with ZipFile(outfile, "w") as f:
             f.writestr("fs.db", self.export_db())
             f.writestr("_METADATA", metadata)
 
             for file in self.root.iterdir():
                 if file.is_dir():
-                    f.mkdir(str(file.relative_to(self.root)))
+                    # f.mkdir(str(file.relative_to(self.root)))
                     os_walk_it = os.walk(str(file))
                     os_walk_root = next(os_walk_it)[0]  # skip the root
                     assert Path(os_walk_root) == file
                     for dirpath, dirnames, filenames in os.walk(str(file)):
                         dirpath = Path(dirpath)
                         rel_dirpath = dirpath.relative_to(self.root)
                         f.mkdir(str(rel_dirpath))
@@ -155,16 +156,20 @@
                 if (
                     file.filename == "_METADATA"
                     or file.filename == "_LOCK"
                     or file.filename == "fs.db"
                 ):
                     continue
 
-                with zf.open(file, mode="r") as f:
-                    (self.root / fpath).write_bytes(f.read())
+                if file.is_dir():
+                    (self.root / fpath).mkdir(exist_ok=True, parents=True)
+                else:
+                    (self.root / fpath).parent.mkdir(exist_ok=True, parents=True)
+                    with zf.open(file, mode="r") as f:
+                        (self.root / fpath).write_bytes(f.read())
 
             self.import_db(zf.read("fs.db"))
 
     def export_db(self):
         return pickle.dumps(
             self.db.execute("SELECT path, diskpath, success, key FROM files").fetchall()
         )
@@ -343,14 +348,26 @@
                         pdiskpath.parent
                         / (
                             pdiskpath.name[: len(pdiskpath.name) - len(ext)]
                             + f"_{last_id + 1:03d}"
                             + ext
                         )
                     )
+
+                # if _realdiskpath does not exist -- meaning the file was deleted, but the entry is still in the database
+                # we are going to have UNIQUE constraint violation, so we need to remove it first
+                record = self.fs.db.execute(
+                    "SELECT rowid FROM files WHERE diskpath = ? LIMIT 1",
+                    (self._realdiskpath,),
+                ).fetchone()
+                if record is not None:
+                    self.fs.db.execute(
+                        "DELETE FROM files WHERE rowid = ?", (record[0],)
+                    )
+
                 cur = self.fs.db.execute(
                     "INSERT INTO files VALUES (?, ?, ?, ?)",
                     (
                         self.relpath,
                         self._realdiskpath,
                         ItemStatus.NotSuccess,
                         self.ser_key,
@@ -385,8 +402,33 @@
                     if f.is_dir():
                         shutil.rmtree(f)
                     else:
                         f.unlink()
             return self.fs.root / self._realdiskpath
 
         raise Exception("Unreachable!")
-        raise Exception("Unreachable!")
+
+
+if __name__ == "__main__":
+    import click
+
+    @click.command()
+    @click.option("-i", "--input", required=True, help="FS's root directory")
+    @click.option(
+        "-o",
+        "--output",
+        required=True,
+        help="Output file if it's an export command, Input file if it's an import command.",
+    )
+    @click.option(
+        "-c", "--command", required=True, help="Command to run: import/export"
+    )
+    def cli(input: str, output: str, command: Literal["import", "export"]):
+        fs = FS(Path(input))
+
+        if command == "import":
+            fs.import_fs(Path(output))
+
+        if command == "export":
+            fs.export_fs(Path(output), b"From v100/000")
+
+    cli()
```

### Comparing `ream2-4.2.3/ream/helper.py` & `ream2-4.3.1/ream/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from __future__ import annotations
+
 import atexit
 import cProfile
 import functools
 import importlib
 import sys
 import threading
 from contextlib import contextmanager
 from pathlib import Path
 from typing import (
+    Callable,
     Literal,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
@@ -22,15 +25,15 @@
 from loguru import logger
 from serde.helper import AVAILABLE_COMPRESSIONS
 
 TYPE_ALIASES = {"typing.List": "list", "typing.Dict": "dict", "typing.Set": "set"}
 Compression = Literal["snappy", "gzip", "lz4", "zstd", "bz2"]
 
 
-def get_classpath(type: Type) -> str:
+def get_classpath(type: Type | Callable) -> str:
     if type.__module__ == "builtins":
         return type.__qualname__
 
     if hasattr(type, "__qualname__"):
         return type.__module__ + "." + type.__qualname__
 
     # typically a class from the typing module
```

### Comparing `ream2-4.2.3/ream/params_helper.py` & `ream2-4.3.1/ream/params_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/prelude.py` & `ream2-4.3.1/ream/prelude.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/ream/workspace.py` & `ream2-4.3.1/ream/workspace.py`

 * *Files identical despite different names*

### Comparing `ream2-4.2.3/PKG-INFO` & `ream2-4.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: ream2
-Version: 4.2.3
+Version: 4.3.1
 Summary: An actor architecture for research software
 Home-page: https://github.com/binh-vu/ream
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: filelock (>=3.8.0,<4.0.0)
 Requires-Dist: graph-wrapper (>=1.6.0,<2.0.0)
-Requires-Dist: hugedict (>=2.9.2,<3.0.0)
+Requires-Dist: hugedict (>=2.12.10,<3.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: nptyping (>=2.5.0,<3.0.0)
 Requires-Dist: orjson (>=3.9.0,<4.0.0)
+Requires-Dist: pandas (>=2.1.3,<3.0.0)
 Requires-Dist: polars (>=0.18.0)
 Requires-Dist: pyarrow (>=13.0.0,<14.0.0)
 Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
 Requires-Dist: serde2 (>=1.6.0,<2.0.0)
 Requires-Dist: t2-yada (>=1.2.0,<2.0.0)
 Requires-Dist: timer4 (>=1.0.4,<2.0.0)
 Project-URL: Repository, https://github.com/binh-vu/ream
```

