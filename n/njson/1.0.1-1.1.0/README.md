# Comparing `tmp/njson-1.0.1.tar.gz` & `tmp/njson-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "njson-1.0.1.tar", max compression
+gzip compressed data, was "njson-1.1.0.tar", max compression
```

## Comparing `njson-1.0.1.tar` & `njson-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2024-04-19 00:48:35.815407 njson-1.0.1/LICENSE
--rw-r--r--   0        0        0     3742 2024-04-19 00:48:35.815407 njson-1.0.1/README.md
--rw-r--r--   0        0        0      162 2024-04-19 00:48:35.815407 njson-1.0.1/njson/__init__.py
--rw-r--r--   0        0        0    20044 2024-04-19 00:48:35.816407 njson-1.0.1/njson/njson.py
--rw-r--r--   0        0        0      568 2024-04-19 00:48:35.816407 njson-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4654 1970-01-01 00:00:00.000000 njson-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-04-22 04:52:19.621926 njson-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3742 2024-04-22 04:52:19.622926 njson-1.1.0/README.md
+-rw-r--r--   0        0        0      162 2024-04-22 04:52:19.622926 njson-1.1.0/njson/__init__.py
+-rw-r--r--   0        0        0    29137 2024-04-22 04:52:19.622926 njson-1.1.0/njson/njson.py
+-rw-r--r--   0        0        0      568 2024-04-22 04:52:19.622926 njson-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4654 1970-01-01 00:00:00.000000 njson-1.1.0/PKG-INFO
```

### Comparing `njson-1.0.1/LICENSE` & `njson-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `njson-1.0.1/README.md` & `njson-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `njson-1.0.1/njson/njson.py` & `njson-1.1.0/njson/njson.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,168 +1,212 @@
-from typing import Iterable, Union, Hashable, Any, Type
+from typing import Iterable, Union, Hashable, Any, Type, Callable, Mapping
 from types import GeneratorType
 from itertools import zip_longest, dropwhile
 from collections import deque, abc
 from pathlib import Path
 import json, io
 
 # -----------------------------------------------------------------------------
 # Unitily functions to parse data before creating NestedJson class object
 
 def read_json(path):
-    """Return NestedJson, loaded from file-like object containing
-    a JSON document."""
+    '''Return `NestedJson` loaded from file-like object containing
+    a JSON document.'''
     p = Path(path)
     if p.exists() and not p.is_dir():
         with io.open(p, 'r') as f:
             data = json.load(f)
         return NestedJson(data)
     else:
         raise FileNotFoundError(f'File {p} was not found or is a directory.')
 
 def read_json_str(data: str):
-    """Return NestedJson, loaded from json string."""
+    '''Return `NestedJson`, loaded from json string.'''
     return NestedJson(json.loads(data))
 
 def from_flat_dict(data):
-    """Return NestedJson with data parsed as flat-dict.
+    '''Return `NestedJson` with data parsed as flat-dict.
     Flat-dict data is dictionary with tuple keys, such as
     `{('a', 'b'): 1, ('c',): 2}`.
-    """
+    '''
     return NestedJson(NestedJson._nest_flat_dict(data))
 
 def from_nested_flat_dict(data):
-    """Return NestedJson with data parsed as nested flat-dict.
+    '''Return `NestedJson` with data parsed as nested flat-dict.
     Nested flat-dict data is dictionary with nested flat-dict data.
     Flat-dict data is dictionary with tuple keys.
-    """
+    '''
     return NestedJson(NestedJson._nested_nest_flat_dict(data))
 
 def from_series(data):
-    """Return NestedJson with data parsed as data-series.
+    '''Return `NestedJson` with data parsed as data-series.
     Data-series data is dictionary with uniform length tuple keys,
     such as `{('a', 'b'): 1, ('c', ''): 2}`.
-    """
+    '''
     return NestedJson(NestedJson._nest_series(data))
 
 def from_nested_series(data):
-    """Return NestedJson with data parsed as nested data-series."""
+    '''Return `NestedJson` with data parsed as nested data-series.'''
     return NestedJson(NestedJson._nested_nest_series(data))
 
 # -----------------------------------------------------------------------------
-# ParsedNestedJson class
+# NestedJsonKeysView class
+class NestedJsonKeysView(abc.KeysView):
+    def __init__(self, mapping):
+        self._mapping = mapping._keys
+
+# -----------------------------------------------------------------------------
+# NestedJsonKeysView class
+class NestedJsonValuesView(abc.ValuesView):
+    def __init__(self, mapping):
+        self._mapping = mapping._values
+
+    def __repr__(self):
+        return f'{self.__class__.__name__}({self._mapping})'
+
+    def __iter__(self):
+        yield from self._mapping
+
+    def __contains__(self, value):
+        return value in self._mapping
+
+# -----------------------------------------------------------------------------
+# NestedJsonKeysView class
+class NestedJsonItemsView(abc.ItemsView):
+    def __init__(self, mapping):
+        self._parent_mapping = mapping
+        self._mapping = self._parent_mapping._mapping
+
+    def __repr__(self):
+        return f'{self.__class__.__name__}({list(self._mapping)})'
+
+    def __iter__(self):
+        yield from self._mapping
+
+    def __contains__(self, item):
+        key, value = item
+        try:
+            v = self._parent_mapping._get(*key)
+        except KeyError:
+            return False
+        else:
+            return v is value or v == value
+
+# -----------------------------------------------------------------------------
+# _ParsedNestedJson class
 class _ParsedNestedJson:
-    """Provide grouped attributes for NestedJson with lazy parsing of data.
+    '''Provide grouped attributes for `NestedJson` with lazy parsing of data.
 
     Attributes:
-        fd (NestedJson): NestedJson with data parsed as flat-dict.
-        ds (NestedJson): NestedJson with data parsed as data-series.
-        nfd (NestedJson): NestedJson with data parsed as nested flat-dict.
-        nds (NestedJson): NestedJson with data parsed as nested data-series.
-    """
+        fd (NestedJson): `NestedJson` with data parsed as flat-dict.
+        ds (NestedJson): `NestedJson` with data parsed as data-series.
+        nfd (NestedJson): `NestedJson` with data parsed as nested flat-dict.
+        nds (NestedJson): `NestedJson` with data parsed as nested data-series.
+    '''
     def __init__(self, parent):
         self.parent = parent
 
     @property
     def fd(self):
+        '''Return `NestedJson` with data parsed as flat-dict.'''
         return self.parent._as_parsed_flat_dict
 
     @property
     def ds(self):
+        '''Return `NestedJson` with data parsed as data-series.'''
         return self.parent._as_parsed_data_series
 
     @property
     def nfd(self):
+        '''Return `NestedJson` with data parsed as nested flat-dict.'''
         return self.parent._as_parsed_nested_flat_dict
 
     @property
     def nds(self):
+        '''Return `NestedJson` with data parsed as nested data-series.'''
         return self.parent._as_parsed_nested_data_series
 
 # -----------------------------------------------------------------------------
 # NestedJson class
 
 class NestedJson(abc.Mapping):
-    """Provide fast JSON-like data transformation to and from nested
+    '''Provide fast JSON-like data transformation to and from nested
     parent-child and flat label-value data items, such as Pandas `Series` with
     MultiIndex index.
 
     Args:
         data (list,dict): json-like nested data
 
     Attributes:
-        data (dict,list): Return data.
+        data (dict,list): Return input data.
         str (str): Return data as json str.
-        flat_dict (dict): Return a flat dict where keys are tuples with parent
+        nitems (int): Return number of nested items in `NestedJson`.
+        nlevels (int): Return maximum number of nesting levels in `NestedJson`.
+        flat_dict (dict): Return a flat-dict where keys are tuples with parent
             keys from the nested json-like data.
-        data_series (dict): Return a flat dict. If the iterables are of 
-            uneven length, missing values are filled-in with '' at the start of
-            key tuples.
-        data_series_bfill (dict): Return a flat dict. If the iterables are of 
-            uneven length, missing values are filled-in with '' at the end of
-            key tuples.
-        values (list): Return values of the nested json-like data.
-        keys (list): Return keys of the nested json-like data.
-        keys_fillna_end (list): Return keys of the nested json-like data. If the
-            iterables are of uneven length, missing values are filled-in with ''
+        data_series (dict): Return a flat-dict. If the iterables are of 
+            uneven length, missing values are filled-in with empty string `''`
             at the end of key tuples.
-        keys_fillna_start (list): Return keys of the nested json-like data. If
-            the iterables are of uneven length, missing values are filled-in
-            with '' at the start of key tuples.
-        parsed.nfd (NestedJson): NestedJson with data parsed as nested flat-dict.
-            Provides convenient access above listed NestedJson attributes after
-            parsing source data. For example, `.parsed.nfd.data` will return 
-            flat-dict source data transformed to nested json-like data.
-        parsed.nds (NestedJson): NestedJson with data parsed as nested data-series.
-        parsed.fd (NestedJson): NestedJson with data parsed as flat-dict.
-        parsed.ds (NestedJson): NestedJson with data parsed as data-series.
+        data_series_bfill (dict): Return a flat-dict. If the iterables are of 
+            uneven length, missing values are filled-in with empty string `''`
+            at the start of key tuples.
+        parsed (_ParsedNestedJson): Parse input data and return `NestedJson`.
+            Specifically:
+            parsed.nfd (NestedJson): Return `NestedJson` with input data parsed
+                as nested flat-dict.
+            parsed.nds (NestedJson): Return `NestedJson` with input data parsed
+                as nested data-series.
+            parsed.fd (NestedJson): Return `NestedJson` with input data parsed
+                as flat-dict (skip parsing sub-elements).
+            parsed.ds (NestedJson): Return `NestedJson` with input data parsed
+                as data-series (skip parsing sub-elements).
 
     Example usage:
         ## Flatten and unflatten nested json-like or flat-dict-like data.
         ```python
         >>> import njson as nj
         >>> d = {'a': 1, 'b': [{}}, {'d': 2}]}
         >>> njd = nj.NestedJson(d)
         >>> print(njd.data) # source data
         >>> print(njd.flat_dict) # data as flat-dict with parent key tuples
-        >>> print(njd.data_series) # data as flat-dict with parent key tuples
-        >>> print(njd.data_series_bfill) # ... even length key tuples aligned "rigth"
+        >>> print(njd.data_series) # with event length parent key tuples
+        >>> print(njd.data_series_bfill) # even length key tuples aligned rigth
         >>> print(njd.get('b')) # get data
         >>> print(njd.get('b', 0)) # get nested data
         >>> print(njd.get('b', 1)) # get data at any nesting level
-        >>> njd.parsed.nfd.str # json str of origianl data parsed as nested flat-dict
+        >>> njd.parsed.nfd.str # json str of `.data` parsed as nested flat-dict
         {'a': 1, 'b': [{}, {'d': 2}]}
         {('a',): 1, ('b', 0): {}, ('b', 1, 'd'): 2}
         {('a', '', ''): 1, ('b', 0, ''): {}, ('b', 1, 'd'): 2}
         {('', '', 'a'): 1, ('', 'b', 0): {}, ('b', 1, 'd'): 2}
         [{}, {'d': 2}]
         {}
         {'d': 2}
         '{"a": 1, "b": [{}, {"d": 2}]}'
         ```
 
         **Note**
-        * All flat-dict keys are tuples representing parent keys of json-like data.
-        * The flat-dict labels keys for nested lists are integer values.
-        * Empty dict,  list, tuple, set values are not flattened, as they have no values
-          or parent keys.
-        * The `.data_series` flat-dict with even length key tuples has similar data
-          structure to pandas `MultiIndex` `Series`. Key tuple length normalization 
-          prepares data for efficient creation of Pandas `Series` objects from deeply
-          nested JSON object data.
+        * Flat-dict keys are parent key tuples of nested json-like data values.
+        * List value parent key labels in flat-dict are integer values.
+        * Empty dict, list, tuple, set values are not "flattened", as they have
+          no nested values or parent keys for nested values.
+        * The `.data_series` - a flat-dict with even length key tuples - has 
+          similar data structure to pandas `Series` with `MultiIndex`. As such, 
+          key tuple length normalization prepares data for efficient creation
+          of Pandas `Series` objects from deeply nested JSON object data.
 
         ## Transforming Pandas `Series`, `DataFrame` to and from JSON-like data
         ```python
         >>> import pandas as pd
         >>> import njson as nj
         >>> d = {'a': 1, 'b': [{}, {'d': 2}]}
         >>> njd = nj.NestedJson(d)
-        >>> ds = njd.to_data_series(pd.Series)
-        >>> print(ds)
-        >>> print(ds.unstack(level = [0]))
+        >>> ds = njd.to_data_series(into = pd.Series)
+        >>> print(ds) # pandas Series from NestedJson
+        >>> print(ds.unstack(level = [0])) # to DataFrame from Series
         >>> print(ds.to_dict(into = NestedJson).parsed.nds.data)
         <class 'pandas.core.series.Series'>
         a           1
         b  0       {}
            1  d     2
         dtype: object
                     d
@@ -173,75 +217,204 @@
         b  0       {}
            1  d     2
         dtype: object
         {'a': 1, 'b': [{}, {'d': 2}]}
         ```
 
         **Note**
-        * Pass pandas Series `pd.Series` to NestedJson 
-          `NestedJson.to_data_series(into = NestedJson)` to directly 
-          derive Pandas `Series` data. Then access `.parsed.nds.data`
-          attribute to return nested JSON-like data.
-        * Pass `NestedJson` to pandas `Series.to_dict(into = NestedJson)` to directly 
-          derive `NestedJson` from Pandas `Series` data.
-        * Stacking and unstacking Pandas `Series` with `.unstack()` and `.stack()`
-          allows to tranform the nested JSON-like data to and from convenient 
-          tabular-like Pandas `DataFrame` data structure. Note that (un)stacking
-          by default sorts the level(s) in the resulting index/columns and therefore can
-          alter the order of elements.
-
-    """
+        * Pass pandas `Series` to `NestedJson`'s `.to_data_series` method to
+          directly derive Pandas `Series` data. Then access `.parsed.nds.data`
+          attribute to derive nested JSON-like data.
+        * Pass `NestedJson` to pandas `Series.to_dict(into = NestedJson)` to
+          directly derive `NestedJson` from Pandas `Series` data.
+        * Stacking and unstacking Pandas `Series` with `.unstack()` and
+          `.stack()` allows to tranform the nested JSON-like data to and from
+          convenient tabular-like Pandas `DataFrame` data structure. Note that
+          (un)stacking by default sorts the level(s) in the resulting index or
+          columns and therefore can alter the order of elements.
+    '''
 
     _FILLVALUE = ''
 
     def __init__(
         self,
         data: Union[dict, list] = None,
     ) -> None:
-        self.__data = data
-        if type(self.__data) is GeneratorType:
-            self.data = dict(self.__data)
+        if type(data) is GeneratorType:
+            self.data = dict(data)
+        elif type(data) is NestedJson:
+            self.data = data.data
         else:
-            self.data = self.__data
+            self.data = data
 
     def __getitem__(self, key) -> dict:
-        """Implement evaluation of self[key]."""
-        return self.get(key)
+        '''Implement evaluation of self[key].'''
+        if key == (slice(None, None, None),):
+            return self.data
+        elif type(key) is tuple:
+            return self._get(*key)
+        elif type(key) is slice:
+            if key == slice(None, None, None):
+                return self.data
+            return NestedJson._get_slice(self.data, key)
+        else:
+            return self._get(key)
+
+    def __contains__(self, key) -> bool:
+        '''Return boolean indicating if key is in `NestedJson`.'''
+        try:
+            if type(key) is tuple:
+                self._get(*key)
+            else:
+                self._get(key)
+        except:
+            return False
+        else:
+            return True
+
+    def __eq__(self, other: object) -> bool:
+        '''Return `NestedJson` equal to other.'''
+        if isinstance(other, (dict, list)):
+            return self.data == other
+        elif not isinstance(other, self.__class__):
+            raise TypeError
+        return self.data == other.data
+
+    def __ne__(self, other: object) -> bool:
+        '''Return `NestedJson` not Equal to other.'''
+        return not self.__eq__(other)
+
+    def __setitem__(self, key, value) -> None:
+        '''Update nested `NestedJson` value.'''
+        if type(key) is tuple:
+            print(key)
+            if key[1:]:
+                pks, ck = key[:-1], key[-1]
+                if pks not in self:
+                    raise IndexError("Key out of bounds.")
+                else:
+                    parent_data = self._get(*pks)
+                    parent_data[ck] = value
+            else:
+                if key[0] not in self:
+                    raise IndexError("Key out of bounds.")
+                else:
+                    self.data[key[0]] = value
+        else:
+            if key not in self:
+                raise IndexError("Key out of bounds.")
+            else:
+                self.data[key] = value
 
     def __len__(self) -> int:
-        """Return the number of items in NestedJson."""
-        return len(self.keys)
+        '''Return the number of nested values in NestedJson.'''
+        return NestedJson._count_nested_values(self.data)
 
     def __str__(self) -> str:
-        """Return the string value of the instance."""
+        '''Return the string value of the instance.'''
         return str(self.flat_dict)
 
     def __repr__(self) -> str:
-        """Return the string representation of the instance."""
+        '''Return the string representation of the instance.'''
         return '<{} {}>"'.format(
             self.__class__.__name__,
-            str(self)
+            self.flat_dict
         )
 
     def __reduce__(self) -> Union[list, set, tuple, dict]:
-        """Return state information for pickling."""
+        '''Return state information for pickling.'''
         return type(self), (self.data)
 
     def __iter__(self) -> iter:
-        """Iterate over dictionary key tuples."""
-        return iter(self.flat_dict)
+        '''Iterate over dictionary key tuples.'''
+        yield from self._mapping
+
+    @staticmethod
+    def _nlevels(data):
+        if type(data) is dict and data:
+            return 1 + max([
+                NestedJson._nlevels(item) for item in data.values()
+                if (
+                    type(item) is dict or
+                    type(item) is list or
+                    type(item) is tuple or
+                    type(item) is set
+                ) and item
+            ] or [0])
+        if (
+            type(data) is list or
+            type(data) is tuple or
+            type(data) is set
+        ) and data:
+            return 1 + max([
+                NestedJson._nlevels(item) for item in data
+                if (
+                    type(item) is dict or
+                    type(item) is list or
+                    type(item) is tuple or
+                    type(item) is set
+                ) and item
+            ] or [0])
+        return 0
+
+    @staticmethod
+    def _count_nested_values(data) -> list:
+        if not (
+            type(data) is dict or
+            type(data) is list or
+            type(data) is tuple or
+            type(data) is set
+        ):
+            return 1
+        elif len(data) == 0:
+            return 0
+        else:
+            length = 0
+            for value in (data.values() if type(data) is dict else data):
+                if (
+                    type(value) is dict or
+                    type(value) is list or
+                    type(value) is tuple or
+                    type(value) is set
+                ) and data:
+                    length += NestedJson._count_nested_values(value)
+                else:
+                    length += 1
+        return length
+
+    @staticmethod
+    def _nested_get(data: Union[list,dict], *keys: Hashable) -> Any:
+        '''Get sub-element from nested json-like data.'''
+        for k in keys:
+            data = data[k]
+        return data
+
+    def _get(self, *keys: Hashable) -> Any:
+        '''Get sub-element from `NestedJson` data.'''
+        return NestedJson._nested_get(self.data, *keys)
+
+    @staticmethod
+    def _get_slice(data: Union[list,dict], s: slice) -> Union[dict,list]:
+        '''Get slice from list or dict data.'''
+        if type(data) is list:
+            return data[s]
+        elif type(data) is dict:
+            return {
+                k: data[k]
+                for k in list(data.keys())[s]
+            }
 
     @staticmethod
     def _not_fillvalue(d):
-        """Check if an object is data_series fillvalue."""
+        '''Check if an object is data_series fillvalue.'''
         return d is not NestedJson._FILLVALUE
 
     @staticmethod
     def _is_fillvalue(d):
-        """Check if an object is data_series fillvalue."""
+        '''Check if an object is data_series fillvalue.'''
         return d is NestedJson._FILLVALUE
 
     @staticmethod
     def _drop_fillvalue(data):
         orig_type = type(data)
         return orig_type(filter(NestedJson._not_fillvalue, data))
 
@@ -249,72 +422,86 @@
     def _drop_fillvalue_start(data):
         orig_type = type(data)
         return orig_type(dropwhile(NestedJson._is_fillvalue,iter(data)))
 
     @staticmethod
     def _drop_fillvalue_end(data):
         orig_type = type(data)
-        return orig_type(dropwhile(NestedJson._is_fillvalue,reversed(data)))[::-1]
+        return orig_type(
+            dropwhile(NestedJson._is_fillvalue,reversed(data))
+            )[::-1]
+
 
     @staticmethod
     def _has_listlike_keys(data: dict) -> bool:
-        """Check if a dict is list-like."""
-        if data is dict():
-            return False
-        for i,k in enumerate(data.keys()):
+        '''Check if dict has json-list-like keys.'''
+        for i,k in enumerate(data):
             if i != k:
                 return False
-        return True
+        return bool(data)
 
     @staticmethod
     def _has_nested_list_dict(data: dict) -> bool:
-        """Check if dict has list or dict values."""
-        for k,v in data.items():
+        '''Check if dict has list or dict values.'''
+        for v in data.values():
             if type(v) is list or type(v) is dict:
                 return True
         return False
 
     @staticmethod
     def _listlikedict_to_list(data: dict) -> Union[list,dict]:
-        if type(data) is dict and NestedJson._has_listlike_keys(data):
+        if NestedJson._has_listlike_keys(data):
             return list(data.values())
         else:
             return data
 
     @staticmethod
-    def _nested_listlikedict_to_list(data: Union[list,dict,Any]) -> Union[list,dict,Any]:
-        if data in [{}, []]:
-            return data
-        elif type(data) is dict:
+    def _nested_listlikedict_to_list(
+        data: Union[list,dict,Any]
+    ) -> Union[list,dict,Any]:
+        if type(data) is dict and data:
             if NestedJson._has_listlike_keys(data):
-                return [NestedJson._nested_listlikedict_to_list(val) for val in data.values()]
+                return [
+                    NestedJson._nested_listlikedict_to_list(val)
+                    for val in data.values()
+                ]
             else:
                 if NestedJson._has_nested_list_dict(data):
-                    return {key: NestedJson._nested_listlikedict_to_list(val) for key,val in data.items()}
+                    return {
+                        key: NestedJson._nested_listlikedict_to_list(val)
+                        for key,val in data.items()
+                    }
                 else:
                     return NestedJson._listlikedict_to_list(data)
-        elif type(data) is list:
-            return [NestedJson._nested_listlikedict_to_list(val) for val in data]
+        elif type(data) is list and data:
+            return [
+                NestedJson._nested_listlikedict_to_list(val)
+                for val in data
+            ]
         else:
             return data
 
     @staticmethod
     def _align_start(keys: tuple) -> tuple:
-        """Return keys with key items aligned at the start and fill values moved to end."""
+        '''Return keys with key items aligned at the start and fill values
+        moved to end.
+        '''
         if keys[0] is NestedJson._FILLVALUE:
             d = deque(keys)
             while d[0] is NestedJson._FILLVALUE:
                 d.rotate(-1)
             return tuple(d)
         else:
             return keys
 
     @staticmethod
     def _align_end(keys: tuple) -> tuple:
-        """Return keys with key items aligned at the end and fill values moved to start."""
+        '''Return keys with key items aligned at the end and fill values moved
+        to start.
+        '''
         if keys[-1] is NestedJson._FILLVALUE:
             d = deque(keys)
             while d[-1] is NestedJson._FILLVALUE:
                 d.rotate(1)
             return tuple(d)
         else:
             return keys
@@ -324,26 +511,26 @@
         if not (
             type(data) is dict or
             type(data) is list or
             type(data) is tuple or
             type(data) is set
         ):
             return data
-        elif len(data) == 0:
+        elif not data:
             return data
         else:
             result = []
             for value in (data.values() if type(data) is dict else data):
                 if (
                     type(value) is dict or
                     type(value) is list or
                     type(value) is tuple or
                     type(value) is set
                 ):
-                    if len(value) == 0:
+                    if not value:
                         result.append(value)
                     else:
                         result += NestedJson._nested_get_values(value)
                 else:
                     result.append(value)
             return result
 
@@ -408,27 +595,30 @@
                 d[key[-1]] = value
             else:
                 d = result
                 d[key] = value
         return NestedJson._nested_listlikedict_to_list(result)
 
     @staticmethod
-    def _nested_nest_flat_dict(data: Union[list,dict,Any]) -> Union[list,dict,Any]:
-        if data in [{}, []]:
-            return data
-        elif type(data) is dict:
+    def _nested_nest_flat_dict(
+        data: Union[list,dict,Any]
+    ) -> Union[list,dict,Any]:
+        if type(data) is dict and data:
             if NestedJson._has_nested_list_dict(data):
                 return NestedJson._listlikedict_to_list(
                     NestedJson._nest_flat_dict(
-                        {key: NestedJson._nested_nest_flat_dict(val) for key,val in data.items()}
+                        {
+                            key: NestedJson._nested_nest_flat_dict(val)
+                            for key,val in data.items()
+                        }
                     )
                 )
             else:
                 return NestedJson._nest_flat_dict(data)
-        elif type(data) is list:
+        elif type(data) is list and data:
             return [NestedJson._nested_nest_flat_dict(val) for val in data]
         else:
             return data
 
     @staticmethod
     def _nest_data_series(data: dict) -> Union[dict,list]:
         result = dict()
@@ -443,64 +633,73 @@
                 d[key[-1]] = value
             else:
                 d = result
                 d[key] = value
         return NestedJson._nested_listlikedict_to_list(result)
 
     @staticmethod
-    def _nested_nest_data_series(data: Union[list,dict,Any]) -> Union[list,dict,Any]:
-        if data in [{}, []]:
-            return data
-        elif type(data) is dict:
+    def _nested_nest_data_series(
+        data: Union[list,dict,Any]
+    ) -> Union[list,dict,Any]:
+        if type(data) is dict and data:
             if NestedJson._has_nested_list_dict(data):
                 return NestedJson._listlikedict_to_list(
                     NestedJson._nest_data_series(
-                        {key: NestedJson._nested_nest_data_series(val) for key,val in data.items()}
+                        {
+                            key: NestedJson._nested_nest_data_series(val)
+                            for key,val in data.items()
+                        }
                     )
                 )
             else:
                 return NestedJson._nest_data_series(data)
-        elif type(data) is list:
+        elif type(data) is list and data:
             return [NestedJson._nested_nest_data_series(val) for val in data]
         else:
             return data
 
     @property
-    def keys(self):
+    def _keys(self):
         return NestedJson._nested_get_keys(self.data)
 
     @property
-    def keys_fillna_end(self):
-        return list(map(
-            tuple,
-            zip(*zip_longest(*self.keys, fillvalue = self._FILLVALUE))
-        ))
+    def _values(self):
+        return NestedJson._nested_get_values(self.data)
 
     @property
-    def keys_fillna_start(self):
-        return list(map(
-            tuple,
-            map(reversed,zip(*zip_longest(*map(reversed, self.keys), fillvalue = self._FILLVALUE)))
-        ))
+    def _mapping(self):
+        return zip(self._keys, self._values)
 
     @property
-    def values(self):
-        return NestedJson._nested_get_values(self.data)
+    def _mapping_keys_fillna_end(self):
+        return map(
+            tuple,
+            zip(*zip_longest(
+                *self._keys,
+                fillvalue = self._FILLVALUE
+            ))
+        )
 
     @property
-    def flat_dict(self):
-        return dict(zip(self.keys, self.values))
+    def _mapping_keys_fillna_start(self):
+        return map(
+            tuple,
+            map(reversed,zip(*zip_longest(
+                *map(reversed, self._keys),
+                fillvalue = self._FILLVALUE
+            )))
+        )
 
     @property
-    def data_series(self) -> dict:
-        return dict(zip(self.keys_fillna_end, self.values))
+    def _mapping_data_series(self) -> dict:
+        return zip(self._mapping_keys_fillna_end, self._values)
 
     @property
-    def data_series_bfill(self) -> dict:
-        return dict(zip(self.keys_fillna_start, self.values))
+    def _mapping_data_series_bfill(self) -> dict:
+        return zip(self._mapping_keys_fillna_start, self._values)
 
     @property
     def _as_parsed_flat_dict(self):
         return self.__class__(self._nest_flat_dict(self.data))
 
     @property
     def _as_parsed_nested_flat_dict(self):
@@ -512,54 +711,136 @@
 
     @property
     def _as_parsed_nested_data_series(self):
         return self.__class__(self._nested_nest_data_series(self.data))
 
     @property
     def str(self):
+        '''Return data as json str.'''
         return json.dumps(self.data)
 
     @property
-    def parsed(self):
+    def nitems(self):
+        '''Return number of nested items in `NestedJson`.'''
+        return len(self)
+
+    @property
+    def nlevels(self):
+        '''Return maximum number of nesting levels in `NestedJson`.'''
+        return NestedJson._nlevels(self.data)
+
+    @property
+    def flat_dict(self):
+        '''Return a flat-dict where keys are tuples with parent keys from the
+        `NestedJson` input data.
+        '''
+        return dict(self._mapping)
+
+    @property
+    def data_series(self) -> dict:
+        '''Return a flat-dict. If the iterables are of uneven length, missing
+        values are filled-in with empty string `''` at the end of key tuples.
+        '''
+        return dict(self._mapping_data_series)
+
+    @property
+    def data_series_bfill(self) -> dict:
+        '''Return a flat-dict. If the iterables are of uneven length, missing
+        values are filled-in with empty string `''` at the start of key tuples.
+        '''
+        return dict(self._mapping_data_series_bfill)
+
+    @property
+    def parsed(self) -> _ParsedNestedJson:
+        '''Parse input data and return `NestedJson`. Specifically:
+        parsed.nfd (NestedJson): Return `NestedJson` with input data parsed
+            as nested flat-dict.
+        parsed.nds (NestedJson): Return `NestedJson` with input data parsed
+            as nested data-series.
+        parsed.fd (NestedJson): Return `NestedJson` with input data parsed
+            as flat-dict.
+        parsed.ds (NestedJson): Return `NestedJson` with input data parsed
+            as data-series.
+        '''
         return _ParsedNestedJson(self)
 
-    def get(self, *keys: Hashable) -> Any:
-        '''Get sub-element value.'''
-        data = self.data
-        for k in keys: data = data[k]
-        return data
+    def get(self, *key: Hashable, default=None) -> Any:
+        '''Get any nested element or return value of keyword agrument `default`
+        if key is not found.'''
+        try:
+            return self._get(*key)
+        except KeyError:
+            return default
+
+    def keys(self) -> NestedJsonKeysView:
+        '''View NestedJson's keys.'''
+        return NestedJsonKeysView(self)
+
+    def values(self) -> NestedJsonValuesView:
+        '''View NestedJson's values.'''
+        return NestedJsonValuesView(self)
+
+    def items(self) -> NestedJsonItemsView:
+        '''View NestedJson's items.'''
+        return NestedJsonItemsView(self)
+
+    def slice(self, *key: Hashable) -> Any:
+        '''Get any nested element as `NestedJson` if nested element is dict or
+        list, otherwise return the nested value.
+        '''
+        sub_element = self._get(*key)
+        if (
+            type(sub_element) is dict or
+            type(sub_element) is list
+        ):
+            return self.__class__(sub_element)
+        else:
+            return sub_element
 
-    def to_data_series(self, into: Type[Iterable] = dict, bfill = False) -> Iterable:
-        """
-        Return an iterable object (default dictionary) of nested json-like data 
-        with padded label key tuples.
-
-        into (Type[Iterable]): default dict
-            Iterable type to convert to the returned iterable object, such as,
-            list, tuple, pandas `Series`.
-        bfill (bool): default False
-            Fill nested key tuples backward (default) or forward.
-
-        Returns
-        -------
-        Data converted into specified Iterable Type object.
-        """
-        print(str(into))
+    def to_data_series(
+        self,
+        into: Callable[[dict], Any] = None,
+        bfill = False,
+        ) -> Iterable:
+        '''
+        Call `into` function with `NestedJson` data-series passed as argument.
+
+        Arguments:
+            into (Callable[[dict], Any]): Call function with `NestedJson`
+                data-series dictionary passed as argument. For example, pandas
+                `Series`.
+            bfill (bool): default False
+                Fill nested key tuples backward (default) or forward.
+
+        Returns:
+            Data converted into specified Iterable Type object.
+        '''
         data_series = self.data_series_bfill if bfill else self.data_series
-        if into in [dict]:
+        if into is dict:
             return data_series
-        elif into in [set()] or (
-            isinstance(into, Type) and
-            str(into) == "<class 'pandas.core.series.Series'>"
-        ):
-            return into(data_series)
-        elif into in [set()] or (
-            isinstance(into, Type) and
-            str(into) == "<class 'pandas.core.frame.DataFrame'>"
+        elif getattr(into, '__module__', False) == 'pandas.core.frame' and (
+            hasattr(into, 'from_dict')
         ):
+            # Add pandas DataFrame column name `0` wrapper dictionary, as pandas
+            # DataFrame enumerates index names, when only data is provided.
             return into.from_dict({0: data_series})
         else:
-            return into(data_series.items())
+            return into(data_series)
 
-    def pipe_data(self, fn: Type) -> Any:
-        '''Apply function to data.'''
-        return fn(self.data)
+    def pipe_data(self, fn: Callable[[Mapping], Any]) -> Any:
+        '''Pass `NestedJson`'s `.data` as argument to `fn`.'''
+        return fn(self.data)
+
+    def pipe_flat_dict(self, fn: Callable[[dict], Any]) -> Any:
+        '''Pass `NestedJson`'s `.flat_dict` as argument to `fn`.'''
+        return fn(self.flat_dict)
+
+    def pipe_data_series(
+        self, fn: Callable[[dict], Any] = dict,
+        bfill = False
+    ) -> Iterable:
+        '''Pass `NestedJson`'s `.data_series` as argument to `fn`.'''
+        return fn(self.data_series)
+
+    def pipe_mapping(self, fn: Callable[[Mapping], Any]) -> Any:
+        '''Pass `NestedJson`'s iterable as argument to `fn`.'''
+        return fn(self._mapping)
```

### Comparing `njson-1.0.1/pyproject.toml` & `njson-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "njson"
-version = "1.0.1"
+version = "1.1.0"
 description = "Provide fast JSON-like data transformation to and from nested parent-child and flat label-value data items, such as Pandas `Series` with MultiIndex index."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/martins-bruvelis/njson"
 documentation = "https://gitlab.com/martins-bruvelis/njson/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `njson-1.0.1/PKG-INFO` & `njson-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: njson
-Version: 1.0.1
+Version: 1.1.0
 Summary: Provide fast JSON-like data transformation to and from nested parent-child and flat label-value data items, such as Pandas `Series` with MultiIndex index.
 Home-page: https://gitlab.com/martins-bruvelis/njson
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

