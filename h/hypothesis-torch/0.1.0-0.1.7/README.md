# Comparing `tmp/hypothesis_torch-0.1.0.tar.gz` & `tmp/hypothesis_torch-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.1.0.tar", last modified: Sun Apr 21 20:31:52 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.1.7.tar", last modified: Sun Apr 21 21:29:44 2024, max compression
```

## Comparing `hypothesis_torch-0.1.0.tar` & `hypothesis_torch-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 andrewsansom   (501) staff       (20)        0 2024-04-21 20:31:52.265514 hypothesis_torch-0.1.0/
--rw-r--r--   0 andrewsansom   (501) staff       (20)     1070 2024-02-19 03:33:04.000000 hypothesis_torch-0.1.0/LICENSE
--rw-r--r--   0 andrewsansom   (501) staff       (20)     8036 2024-04-21 20:31:52.265202 hypothesis_torch-0.1.0/PKG-INFO
--rw-r--r--   0 andrewsansom   (501) staff       (20)     5272 2024-04-21 19:37:34.000000 hypothesis_torch-0.1.0/README.md
-drwxr-xr-x   0 andrewsansom   (501) staff       (20)        0 2024-04-21 20:31:52.263373 hypothesis_torch-0.1.0/hypothesis_torch/
--rw-r--r--   0 andrewsansom   (501) staff       (20)      405 2024-04-21 20:04:36.000000 hypothesis_torch-0.1.0/hypothesis_torch/__init__.py
--rw-r--r--   0 andrewsansom   (501) staff       (20)     1435 2024-04-21 02:42:21.000000 hypothesis_torch-0.1.0/hypothesis_torch/device.py
--rw-r--r--   0 andrewsansom   (501) staff       (20)     2171 2024-04-21 19:17:08.000000 hypothesis_torch-0.1.0/hypothesis_torch/dtype.py
--rw-r--r--   0 andrewsansom   (501) staff       (20)     3707 2024-04-21 18:59:35.000000 hypothesis_torch-0.1.0/hypothesis_torch/huggingface.py
--rw-r--r--   0 andrewsansom   (501) staff       (20)     1892 2024-04-21 18:37:45.000000 hypothesis_torch-0.1.0/hypothesis_torch/inspection_util.py
--rw-r--r--   0 andrewsansom   (501) staff       (20)     9066 2024-04-21 19:35:40.000000 hypothesis_torch-0.1.0/hypothesis_torch/module.py
--rw-r--r--   0 andrewsansom   (501) staff       (20)     2847 2024-04-21 19:10:57.000000 hypothesis_torch-0.1.0/hypothesis_torch/tensor.py
--rw-r--r--   0 andrewsansom   (501) staff       (20)      755 2024-04-21 02:44:44.000000 hypothesis_torch-0.1.0/hypothesis_torch/utils.py
-drwxr-xr-x   0 andrewsansom   (501) staff       (20)        0 2024-04-21 20:31:52.264475 hypothesis_torch-0.1.0/hypothesis_torch.egg-info/
--rw-r--r--   0 andrewsansom   (501) staff       (20)     8036 2024-04-21 20:31:52.000000 hypothesis_torch-0.1.0/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 andrewsansom   (501) staff       (20)      461 2024-04-21 20:31:52.000000 hypothesis_torch-0.1.0/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 andrewsansom   (501) staff       (20)        1 2024-04-21 20:31:52.000000 hypothesis_torch-0.1.0/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 andrewsansom   (501) staff       (20)       78 2024-04-21 20:31:52.000000 hypothesis_torch-0.1.0/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 andrewsansom   (501) staff       (20)       17 2024-04-21 20:31:52.000000 hypothesis_torch-0.1.0/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 andrewsansom   (501) staff       (20)     1897 2024-04-21 20:31:26.000000 hypothesis_torch-0.1.0/pyproject.toml
--rw-r--r--   0 andrewsansom   (501) staff       (20)       38 2024-04-21 20:31:52.265560 hypothesis_torch-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 21:29:44.353732 hypothesis_torch-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-21 21:29:11.000000 hypothesis_torch-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8036 2024-04-21 21:29:44.353732 hypothesis_torch-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5272 2024-04-21 21:29:11.000000 hypothesis_torch-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 21:29:44.349732 hypothesis_torch-0.1.7/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-21 21:29:41.000000 hypothesis_torch-0.1.7/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2024-04-21 21:29:11.000000 hypothesis_torch-0.1.7/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2024-04-21 21:29:11.000000 hypothesis_torch-0.1.7/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2024-04-21 21:29:11.000000 hypothesis_torch-0.1.7/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-04-21 21:29:11.000000 hypothesis_torch-0.1.7/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)     9137 2024-04-21 21:29:11.000000 hypothesis_torch-0.1.7/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-04-21 21:29:11.000000 hypothesis_torch-0.1.7/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-04-21 21:29:11.000000 hypothesis_torch-0.1.7/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 21:29:44.349732 hypothesis_torch-0.1.7/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8036 2024-04-21 21:29:44.000000 hypothesis_torch-0.1.7/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      461 2024-04-21 21:29:44.000000 hypothesis_torch-0.1.7/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 21:29:44.000000 hypothesis_torch-0.1.7/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-21 21:29:44.000000 hypothesis_torch-0.1.7/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-21 21:29:44.000000 hypothesis_torch-0.1.7/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1928 2024-04-21 21:29:11.000000 hypothesis_torch-0.1.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-21 21:29:44.353732 hypothesis_torch-0.1.7/setup.cfg
```

### Comparing `hypothesis_torch-0.1.0/LICENSE` & `hypothesis_torch-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.0/PKG-INFO` & `hypothesis_torch-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.1.0
+Version: 0.1.7
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hypothesis_torch-0.1.0/README.md` & `hypothesis_torch-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.0/hypothesis_torch/device.py` & `hypothesis_torch-0.1.7/hypothesis_torch/device.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.0/hypothesis_torch/dtype.py` & `hypothesis_torch-0.1.7/hypothesis_torch/dtype.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.1.0/hypothesis_torch/huggingface.py` & `hypothesis_torch-0.1.7/hypothesis_torch/huggingface.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,14 +80,15 @@
             instantiated on the meta device. This is useful for testing uses of transformers models that do not require
             a forward pass.
         kwargs: Keyword arguments to pass to the transformer constructor. If a keyword argument is a strategy, it will
             be drawn from.
     """
     if isinstance(cls, st.SearchStrategy):
         cls = draw(cls)
+    assert issubclass(cls, transformers.PreTrainedModel)
     config = draw(build_from_cls_init(cls.config_class, **kwargs))
 
     if isinstance(instantiate_weights, st.SearchStrategy):
         instantiate_weights = draw(instantiate_weights)
 
     if instantiate_weights:
         return cls(config)
```

### Comparing `hypothesis_torch-0.1.0/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.1.7/hypothesis_torch/inspection_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import inspect
 from typing import Callable, TypeVar
 
-import hypothesis.strategies as st
-import transformers
 
 T = TypeVar("T")
 
 
 class ParameterInferAnnotationsFromDefault(inspect.Parameter):
     """A parameter that infers the annotation from the default value if it is not specified.
```

### Comparing `hypothesis_torch-0.1.0/hypothesis_torch/module.py` & `hypothesis_torch-0.1.7/hypothesis_torch/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,19 +204,19 @@
         activations: list[nn.Module] = draw(
             st.lists(activation_layer_strategy, min_size=len(layers), max_size=len(layers))
         )
         return nn.Sequential(*utils.alternate(layers, activations))
 
 
 def convolution_output_shape(
-    input_shape: tuple[int, ...],
-    kernel_size: tuple[int, ...],
-    stride: tuple[int, ...],
-    padding: tuple[int, ...],
-    dilation: tuple[int, ...],
+    input_shape: tuple[int, ...] | torch.Tensor,
+    kernel_size: tuple[int, ...]| torch.Tensor,
+    stride: tuple[int, ...]| torch.Tensor,
+    padding: tuple[int, ...]| torch.Tensor,
+    dilation: tuple[int, ...]| torch.Tensor,
 ) -> tuple[int, ...]:
     """Calculate the output shape of a convolutional layer."""
     input_shape = torch.tensor(input_shape, dtype=torch.uint8)
     kernel_size = torch.tensor(kernel_size, dtype=torch.uint8)
     stride = torch.tensor(stride, dtype=torch.uint8)
     padding = torch.tensor(padding, dtype=torch.uint8)
     dilation = torch.tensor(dilation, dtype=torch.uint8)
```

### Comparing `hypothesis_torch-0.1.0/hypothesis_torch/tensor.py` & `hypothesis_torch-0.1.7/hypothesis_torch/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Any, Mapping
 
 import hypothesis.extra.numpy as numpy_st
 import torch
 from hypothesis import strategies as st
 
-from hypothesis_torch import dtype as dtype_module, device as device_module
+from hypothesis_torch import dtype as dtype_module
 
 
 @st.composite
 def tensor_strategy(
     draw: st.DrawFn,
     dtype: torch.dtype | st.SearchStrategy[torch.dtype],
     shape: int | st.SearchStrategy[int] | tuple[int, ...] | st.SearchStrategy[tuple[int, ...]],
```

### Comparing `hypothesis_torch-0.1.0/hypothesis_torch/utils.py` & `hypothesis_torch-0.1.7/hypothesis_torch/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,48 @@
 from __future__ import annotations
 
 import itertools
 import sys
-from typing import Iterable, TypeVar, Tuple, Generator
+from typing import Iterable, TypeVar, Generator
 
 T = TypeVar("T")
+T_co = TypeVar("T_co", covariant=True)
 
 if sys.version_info < (3, 10):
 
-    def pairwise(iterable: Iterable[T]) -> Iterable[Tuple[T, T]]:
+    def pairwise(iterable: Iterable[T]) -> Iterable[tuple[T, T]]:
+        """Iterate over pairs of consecutive elements in an iterable.
+
+        Note:
+            This is a backport of the `pairwise` function from Python 3.10 (for older versions of Python).
+
+        Args:
+            iterable: The iterable to iterate over.
+
+        Returns:
+            An iterable of pairs of consecutive elements.
+        """
         # pairwise('ABCDEFG') --> AB BC CD DE EF FG
         a, b = itertools.tee(iterable)
         next(b, None)
         return zip(a, b)
 else:
-    from itertools import pairwise
+    pairwise = itertools.pairwise
+
+
+def alternate(iterable1: Iterable[T_co], iterable2: Iterable[T_co]) -> Generator[T_co, None, None]:
+    """Alternate elements from two iterables.
 
+    Args:
+        iterable1: The first iterable.
+        iterable2: The second iterable.
 
-def alternate(iterable1: Iterable[T], iterable2: Iterable[T]) -> Generator[T, None, None]:
-    fillvalue = object()
+    Yields:
+        Elements from the two iterables in alternation.
+    """
+    fill_value = object()
     it1 = iter(iterable1)
     it2 = iter(iterable2)
-    for pair in itertools.zip_longest(it1, it2, fillvalue=fillvalue):
+    for pair in itertools.zip_longest(it1, it2, fillvalue=fill_value):
         for element in pair:
-            if element is not fillvalue:
+            if element is not fill_value:
                 yield element
```

### Comparing `hypothesis_torch-0.1.0/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.1.7/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.1.0
+Version: 0.1.7
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hypothesis_torch-0.1.0/pyproject.toml` & `hypothesis_torch-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 Documentation = "https://github.com/qthequartermasterman/hypothesis-torch"
 Repository = "https://github.com/qthequartermasterman/hypothesis-torch.git"
 Issues = "https://github.com/qthequartermasterman/hypothesis-torch/issues"
 
 [tool.ruff]
 line-length = 120
 
-[tool.semantic-release]
+[tool.semantic_release]
 major_on_zero = false
 version_variables = [
     "hypothesis_torch/__init__.py:__version__",
 ]
-build_command = "python -m build"
+build_command = "python -m pip install build && python -m build"
 
 [tool.setuptools.dynamic]
 version = {attr = "hypothesis_torch.__version__"}
```

