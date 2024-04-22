# Comparing `tmp/cognite-synthetic-tags-0.3.3.tar.gz` & `tmp/cognite_synthetic_tags-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite-synthetic-tags-0.3.3.tar", last modified: Fri Feb 25 14:45:51 2022, max compression
+gzip compressed data, was "cognite_synthetic_tags-0.5.0.tar", max compression
```

## Comparing `cognite-synthetic-tags-0.3.3.tar` & `cognite_synthetic_tags-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,8 @@
-drwxr-xr-x   0 fran       (501) staff       (20)        0 2022-02-25 14:45:51.320027 cognite-synthetic-tags-0.3.3/
--rw-r--r--   0 fran       (501) staff       (20)    29554 2022-02-25 14:45:51.319811 cognite-synthetic-tags-0.3.3/PKG-INFO
--rw-r--r--   0 fran       (501) staff       (20)    23080 2021-12-10 13:54:32.000000 cognite-synthetic-tags-0.3.3/README.md
-drwxr-xr-x   0 fran       (501) staff       (20)        0 2022-02-25 14:45:51.318218 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/
--rw-r--r--   0 fran       (501) staff       (20)      154 2021-12-10 13:54:32.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/__init__.py
--rw-r--r--   0 fran       (501) staff       (20)     1537 2021-12-10 13:54:32.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/_operations.py
--rw-r--r--   0 fran       (501) staff       (20)     2160 2021-12-16 10:03:03.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/data_stores.py
--rw-r--r--   0 fran       (501) staff       (20)     5427 2021-12-17 08:29:19.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/tag.py
--rw-r--r--   0 fran       (501) staff       (20)    12187 2022-01-09 20:06:24.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/tag_resolver.py
--rw-r--r--   0 fran       (501) staff       (20)     1046 2021-12-10 13:54:32.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/types.py
-drwxr-xr-x   0 fran       (501) staff       (20)        0 2022-02-25 14:45:51.319296 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags.egg-info/
--rw-r--r--   0 fran       (501) staff       (20)    29554 2022-02-25 14:45:51.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags.egg-info/PKG-INFO
--rw-r--r--   0 fran       (501) staff       (20)      515 2022-02-25 14:45:51.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags.egg-info/SOURCES.txt
--rw-r--r--   0 fran       (501) staff       (20)        1 2022-02-25 14:45:51.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags.egg-info/dependency_links.txt
--rw-r--r--   0 fran       (501) staff       (20)       21 2022-02-25 14:45:51.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags.egg-info/requires.txt
--rw-r--r--   0 fran       (501) staff       (20)       23 2022-02-25 14:45:51.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags.egg-info/top_level.txt
--rw-r--r--   0 fran       (501) staff       (20)        1 2021-07-27 12:24:06.000000 cognite-synthetic-tags-0.3.3/cognite_synthetic_tags.egg-info/zip-safe
--rw-r--r--   0 fran       (501) staff       (20)     1025 2022-02-25 14:38:37.000000 cognite-synthetic-tags-0.3.3/pyproject.toml
--rw-r--r--   0 fran       (501) staff       (20)       38 2022-02-25 14:45:51.320085 cognite-synthetic-tags-0.3.3/setup.cfg
--rw-r--r--   0 fran       (501) staff       (20)     1733 2022-02-25 14:45:10.000000 cognite-synthetic-tags-0.3.3/setup.py
+-rw-r--r--   0        0        0      154 2024-04-22 00:48:55.939343 cognite_synthetic_tags-0.5.0/cognite_synthetic_tags/__init__.py
+-rw-r--r--   0        0        0     1818 2024-04-22 00:48:55.939343 cognite_synthetic_tags-0.5.0/cognite_synthetic_tags/_operations.py
+-rw-r--r--   0        0        0     2568 2024-04-22 00:48:55.939343 cognite_synthetic_tags-0.5.0/cognite_synthetic_tags/data_stores.py
+-rw-r--r--   0        0        0     5535 2024-04-22 00:48:55.939343 cognite_synthetic_tags-0.5.0/cognite_synthetic_tags/tag.py
+-rw-r--r--   0        0        0    12204 2024-04-22 00:48:55.939343 cognite_synthetic_tags-0.5.0/cognite_synthetic_tags/tag_resolver.py
+-rw-r--r--   0        0        0     1046 2024-04-22 00:48:55.939343 cognite_synthetic_tags-0.5.0/cognite_synthetic_tags/types.py
+-rw-r--r--   0        0        0     1083 2024-04-22 00:48:55.943343 cognite_synthetic_tags-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 cognite_synthetic_tags-0.5.0/PKG-INFO
```

### Comparing `cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/_operations.py` & `cognite_synthetic_tags-0.5.0/cognite_synthetic_tags/_operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 from __future__ import annotations
 
 import operator
 from typing import Callable, Dict
 
+import numpy as np
+
+
+def _div_by_0_guard(div_operator):
+    """
+    Guard against this warning when b is zero:
+        'pandas invalid value encountered in double_scalars'
+    """
+    return lambda a, b: np.nan if b == 0 else div_operator(a, b)
+
+
 # https://docs.python.org/3/library/operator.html
 DEFAULT_OPERATIONS: Dict[str, Callable] = {
     "+": operator.add,
     "-": operator.sub,
     "*": operator.mul,
-    "/": operator.truediv,
-    "//": operator.floordiv,
+    "/": _div_by_0_guard(operator.truediv),
+    "//": _div_by_0_guard(operator.floordiv),
     "%": operator.mod,
     "**": operator.pow,
     "&": lambda a, b: operator.and_(bool(a), bool(b)),
     "|": lambda a, b: operator.or_(bool(a), bool(b)),
     "^": lambda a, b: operator.xor(bool(a), bool(b)),
     "not": lambda a: operator.not_(bool(a)),  # ~
     "bool": lambda a: bool(a),  # no bitwise operator, only Tag.bool()
```

### Comparing `cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/data_stores.py` & `cognite_synthetic_tags-0.5.0/cognite_synthetic_tags/data_stores.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 import abc
 from typing import Callable, List
 
 import numpy as np
 import pandas as pd
+from cognite.client.data_classes import DatapointsList
 
 __all__ = [
     "CDFStore",
 ]
 
 
 class Store(abc.ABC):
     def __init__(self, retrieve_func, *args, **kwargs):
         self.retrieve_func = retrieve_func
         self.retrieve_args = args
         self.retrieve_kwargs = kwargs
-        self._process_funcs: List[Callable[[pd.DataFrame], pd.DataFrame]] = []
+        self._preprocess_funcs: List[Callable[[pd.DataFrame], pd.DataFrame]] = (
+            []
+        )
+        self._process_funcs: List[
+            Callable[[DatapointsList], DatapointsList]
+        ] = []
 
     def __call__(self, external_ids):
         res = self._fetch(external_ids)
+        for preprocess_func in self._preprocess_funcs:
+            res = preprocess_func(res)
         df = self._process(res, external_ids)
         for process_func in self._process_funcs:
             df = process_func(df)
         return {col: df[col] for col in df.columns}
 
     @abc.abstractmethod
-    def _fetch(self, external_ids):
-        ...
+    def _fetch(self, external_ids): ...  # pragma: no cover
 
     @abc.abstractmethod
-    def _process(self, raw, external_ids):
-        ...
+    def _process(self, raw, external_ids): ...  # pragma: no cover
+
+    def preprocess(self, func):
+        self._preprocess_funcs.append(func)
+        return self
 
     def process(self, func):
         self._process_funcs.append(func)
         return self
 
 
 class CDFStore(Store):
@@ -56,15 +66,15 @@
         if len(aggregates) > 1:
             raise ValueError(
                 f"CDFStore supports up to 1 item in `aggregates` list,"
                 f" got: {aggregates}"
             )
         aggregate = aggregates[0] if aggregates else None
         columns = (
-            tags
+            list(tags)
             if aggregate is None
             else [f"{tag}|{aggregate}" for tag in tags]
         )
 
         # Add any missing columns:
         df.loc[:, [c for c in columns if c not in df.columns]] = self.fill_with
```

### Comparing `cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/tag.py` & `cognite_synthetic_tags-0.5.0/cognite_synthetic_tags/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,16 +136,20 @@
 
         For example:
           specs = {"status": Tag("A") or Tag("B")}
         Here the value of specs["status"] will always be Tag("A"). This happens
         be there is a chance to resolve the specs (i.e. the short-circuiting
         happens on the line of code in the example).
         """
-        if os.environ.get("COGNITE_SYNTHETIC_TAGS_ALLOW_BOOL", False):
-            logger.warning(UnsupportedOperationError.MESSAGE.format(tag=self))
+        handling = os.environ.get("COGNITE_SYNTHETIC_TAGS_ALLOW_BOOL", False)
+        if handling:
+            if handling != "silent":
+                logger.warning(
+                    UnsupportedOperationError.MESSAGE.format(tag=self),
+                )
             return True
         else:
             raise UnsupportedOperationError(self)
 
     def bool(self) -> Tag:
         return self.calc("bool")
```

### Comparing `cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/tag_resolver.py` & `cognite_synthetic_tags-0.5.0/cognite_synthetic_tags/tag_resolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,23 +96,35 @@
         #    `TagResolver` instance).
         for store_key, store_tags in real_tags.items():
             known_tags = store_tags & set(self.context.keys())
             real_tags[store_key] -= known_tags
 
         # fetch all the data from CDF:
         for store_key, store_tags in real_tags.items():
-
             if not store_tags:
                 continue
 
+            # remove store suffix before calling the data store:
+            if store_key != self._default_store_key:
+                store_tags = {
+                    tag.replace(f"__{store_key}", "") for tag in store_tags
+                }
+
             # actually finally call the data store:
             #   (data stores are functions form `data_stores` module, see there
             #   for details)
             values = self.data_stores[store_key](store_tags)
 
+            # add store suffix back:
+            if store_key != self._default_store_key:
+                values = {
+                    f"{key}__{store_key}": value
+                    for key, value in values.items()
+                }
+
             # add the values to context:
             #   (to be used later in `self._resolve_formula`)
             self.context.update(values)
 
         # add literals back:
         self.context.update(literals)
 
@@ -202,15 +214,15 @@
             if tag.name in self._recursive_tags[-1]:
                 raise ValueError(
                     f"Cyclic definition of tags with:"
                     f" {tag.name} in {tag.formula}"
                 )
             self._recursive_tags[-1].add(tag.name)
             item = self._specs[tag.name]
-            tag.formula = getattr(item, "formula", item)
+            tag.formula = getattr(item, "formula", item)  # type: ignore
         return tag
 
     def _resolve_formula(self, formula: TagFormulaT) -> TagValueT:
         """
         Take a formula and return a value.
         Uses `self.context` dict to fetch individual values (leaves in the
         tree of math operations in the formula).
@@ -226,40 +238,33 @@
                 # literal, for example when adding an integer to a `Tag`
                 operands.append(cast(TagValueT, item))
             elif subformula is None:
                 # no formula, just a tag name - must be present in context
                 operands.append(self.context[item.name])
             else:
                 # got some formula, recursion!
-                operands.append(self._resolve_formula(subformula))
+                operands.append(
+                    self._resolve_formula(subformula),  # type: ignore
+                )
 
         # find which operation should be applied:
         operation: OperationT
         if callable(operator_):
             operation = operator_
         else:
             assert (
                 operator_ in self.operations
             ), f"Unknown operator: {operator_}"
             operation = self.operations[operator_]
 
         # apply the operator to the operands:
         uniform_operands = self._make_series(operands)
-        # ...do it manually so that we support all possible operations
-        # ...(this is slower, but supports things like string manipulation)
-        # ... TODO consider making a FastTagResolver ?
-        values_series: List[pd.Series] = uniform_operands
-        result = pd.Series(
-            (
-                operation(*[series[i] for series in values_series])
-                for i in values_series[0].index
-            ),
-            index=values_series[0].index,
+        result = pd.concat(uniform_operands, axis=1).apply(
+            lambda row: operation(*row), axis=1
         )
-
         return result
 
     @staticmethod
     def _extract_literals_from_specs(
         specs: TagSpecsT,
     ) -> Tuple[TagSpecsT, TagResolverContextT]:
         """
@@ -287,24 +292,24 @@
         """
         series: List[pd.Series] = [
             val for val in data if isinstance(val, pd.Series)
         ]
         if not series:
             series = [pd.Series(index=pd.DatetimeIndex([datetime.utcnow()]))]
 
-        # check that all series have the same indexes:
-        #   (all are returned from the same CDF API call, so they should)
-        index = series[0].index
-        assert all(
-            single_series.index.identical(index) for single_series in series[1:]
-        ), "Series need to have the same index."
+        df = pd.concat([*series], axis=1)
+        index = df.index
         # convert any non-series items to series:
         #   (repeat the item for every index)
         all_series: List[pd.Series] = [
-            val if isinstance(val, pd.Series) else pd.Series(val, index=index)
+            (
+                val
+                if isinstance(val, pd.Series)
+                else pd.Series(val, index=index, dtype=float)
+            )
             for val in data
         ]
 
         return all_series
 
     @staticmethod
     def _make_series_in_dict(data: TagResolverContextT) -> TagResolverContextT:
```

### Comparing `cognite-synthetic-tags-0.3.3/cognite_synthetic_tags/types.py` & `cognite_synthetic_tags-0.5.0/cognite_synthetic_tags/types.py`

 * *Files identical despite different names*

### Comparing `cognite-synthetic-tags-0.3.3/pyproject.toml` & `cognite_synthetic_tags-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite_synthetic_tags"
-version = "0.3.3"
+version = "0.5.0"
 description = "Framework for working easily with tags, synthetic and regular, from Cognite Data Fusion (CDF) API."
 authors = ["Fran Hrzenjak <fran.hrzenjak@cognite.com>"]
 license = "Apache License 2.0"
 
 [tool.black]
 line-length = 80
 
@@ -18,25 +18,28 @@
 ensure_newline_before_comments=true
 
 [tool.coverage.run]
 branch=true
 source=["cognite_synthetic_tags"]
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pandas = "^1.3.3"
-cognite-sdk-core = "^2.42.0"
-
-[tool.poetry.dev-dependencies]
-mypy = "^0.910"
-pre-commit = "^2.13.0"
-pytest = "^6.2.4"
-pytest-mock = "^3.6.1"
-coverage = {extras = ["toml"], version = "^5.5"}
+python = ">=3.9,<4"
+cognite-sdk = {version = ">7,<8", extras = ["pandas"]}
+
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.8.0"
+pre-commit = "^3.6.2"
+pytest = "^8.0.2"
+pytest-mock = "^3.12.0"
+coverage = {version = "^7.4.3", extras = ["toml"]}
+python-dotenv = "^1.0.1"
+pytest-regressions = "^2.5.0"
+arrow = "^1.3.0"
+pytest-cov = "^5.0.0"
 
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
-    "setuptools>30,<50.0",  # https://github.com/pypa/setuptools/issues/2353
+    "setuptools>60.0",
     "wheel",
 ]
 build-backend = "poetry.core.masonry.api"
```

