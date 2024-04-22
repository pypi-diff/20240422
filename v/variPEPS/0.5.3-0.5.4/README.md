# Comparing `tmp/varipeps-0.5.3.tar.gz` & `tmp/varipeps-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varipeps-0.5.3.tar", max compression
+gzip compressed data, was "varipeps-0.5.4.tar", max compression
```

## Comparing `varipeps-0.5.3.tar` & `varipeps-0.5.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35103 2024-03-27 09:15:12.924445 varipeps-0.5.3/LICENSE
--rw-r--r--   0        0        0     1048 2024-03-27 09:15:12.924445 varipeps-0.5.3/README.md
--rw-r--r--   0        0        0     1037 2024-03-27 09:15:12.936445 varipeps-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      680 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/__init__.py
--rw-r--r--   0        0        0      741 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/__version__.py
--rw-r--r--   0        0        0    11223 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/config.py
--rw-r--r--   0        0        0      100 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/contractions/__init__.py
--rw-r--r--   0        0        0     5553 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/contractions/apply.py
--rw-r--r--   0        0        0    33811 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/contractions/definitions.py
--rw-r--r--   0        0        0      214 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/ctmrg/__init__.py
--rw-r--r--   0        0        0    24093 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/ctmrg/absorption.py
--rw-r--r--   0        0        0    24758 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/ctmrg/projectors.py
--rw-r--r--   0        0        0    22359 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/ctmrg/routine.py
--rw-r--r--   0        0        0      260 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/expectation/__init__.py
--rw-r--r--   0        0        0     1956 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/expectation/model.py
--rw-r--r--   0        0        0     5609 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/expectation/one_site.py
--rw-r--r--   0        0        0     3348 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/expectation/spiral_helpers.py
--rw-r--r--   0        0        0    17657 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/expectation/three_sites.py
--rw-r--r--   0        0        0    19770 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/expectation/two_sites.py
--rw-r--r--   0        0        0     1178 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/global_state.py
--rw-r--r--   0        0        0      191 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/mapping/__init__.py
--rw-r--r--   0        0        0    40413 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/mapping/florett_pentagon.py
--rw-r--r--   0        0        0    22846 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/mapping/honeycomb.py
--rw-r--r--   0        0        0    39677 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/mapping/kagome.py
--rw-r--r--   0        0        0    46746 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/mapping/maple_leaf.py
--rw-r--r--   0        0        0     1288 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/mapping/model.py
--rw-r--r--   0        0        0    59284 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/mapping/square_kagome.py
--rw-r--r--   0        0        0    19181 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/mapping/triangular.py
--rw-r--r--   0        0        0      152 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/optimization/__init__.py
--rw-r--r--   0        0        0     6434 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/optimization/basinhopping.py
--rw-r--r--   0        0        0    10290 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/optimization/inner_function.py
--rw-r--r--   0        0        0    23104 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/optimization/line_search.py
--rw-r--r--   0        0        0    23194 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/optimization/optimizer.py
--rw-r--r--   0        0        0      113 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/peps/__init__.py
--rw-r--r--   0        0        0    35787 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/peps/tensor.py
--rw-r--r--   0        0        0    41065 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/peps/unitcell.py
--rw-r--r--   0        0        0     1086 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/typing.py
--rw-r--r--   0        0        0      119 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/utils/__init__.py
--rw-r--r--   0        0        0     1285 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/utils/debug_print.py
--rw-r--r--   0        0        0      739 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/utils/func_cache.py
--rw-r--r--   0        0        0     2438 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/utils/periodic_indices.py
--rw-r--r--   0        0        0     1657 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/utils/projector_dict.py
--rw-r--r--   0        0        0     5398 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/utils/random.py
--rw-r--r--   0        0        0     3396 2024-03-27 09:15:12.940445 varipeps-0.5.3/varipeps/utils/svd.py
--rw-r--r--   0        0        0     1953 1970-01-01 00:00:00.000000 varipeps-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    35103 2024-04-22 09:32:46.130676 varipeps-0.5.4/LICENSE
+-rw-r--r--   0        0        0     3116 2024-04-22 09:32:46.130676 varipeps-0.5.4/README.md
+-rw-r--r--   0        0        0     1157 2024-04-22 09:32:46.142676 varipeps-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      680 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/__init__.py
+-rw-r--r--   0        0        0      741 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/__version__.py
+-rw-r--r--   0        0        0    11223 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/config.py
+-rw-r--r--   0        0        0      100 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/contractions/__init__.py
+-rw-r--r--   0        0        0     5553 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/contractions/apply.py
+-rw-r--r--   0        0        0    33811 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/contractions/definitions.py
+-rw-r--r--   0        0        0      214 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/ctmrg/__init__.py
+-rw-r--r--   0        0        0    24093 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/ctmrg/absorption.py
+-rw-r--r--   0        0        0    24758 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/ctmrg/projectors.py
+-rw-r--r--   0        0        0    22359 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/ctmrg/routine.py
+-rw-r--r--   0        0        0      260 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/__init__.py
+-rw-r--r--   0        0        0     1956 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/model.py
+-rw-r--r--   0        0        0     5609 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/one_site.py
+-rw-r--r--   0        0        0     3352 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/spiral_helpers.py
+-rw-r--r--   0        0        0    17657 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/three_sites.py
+-rw-r--r--   0        0        0    19770 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/two_sites.py
+-rw-r--r--   0        0        0     1184 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/global_state.py
+-rw-r--r--   0        0        0      191 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/__init__.py
+-rw-r--r--   0        0        0    44983 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/florett_pentagon.py
+-rw-r--r--   0        0        0    22817 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/honeycomb.py
+-rw-r--r--   0        0        0    39648 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/kagome.py
+-rw-r--r--   0        0        0    46761 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/maple_leaf.py
+-rw-r--r--   0        0        0     1288 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/model.py
+-rw-r--r--   0        0        0    59271 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/square_kagome.py
+-rw-r--r--   0        0        0    19197 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/triangular.py
+-rw-r--r--   0        0        0      152 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/optimization/__init__.py
+-rw-r--r--   0        0        0     6434 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/optimization/basinhopping.py
+-rw-r--r--   0        0        0    10290 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/optimization/inner_function.py
+-rw-r--r--   0        0        0    23104 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/optimization/line_search.py
+-rw-r--r--   0        0        0    24773 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/optimization/optimizer.py
+-rw-r--r--   0        0        0      113 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/peps/__init__.py
+-rw-r--r--   0        0        0    35787 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/peps/tensor.py
+-rw-r--r--   0        0        0    41065 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/peps/unitcell.py
+-rw-r--r--   0        0        0     1086 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/typing.py
+-rw-r--r--   0        0        0      119 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/__init__.py
+-rw-r--r--   0        0        0     1285 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/debug_print.py
+-rw-r--r--   0        0        0      739 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/func_cache.py
+-rw-r--r--   0        0        0     2438 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/periodic_indices.py
+-rw-r--r--   0        0        0     1657 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/projector_dict.py
+-rw-r--r--   0        0        0     5398 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/random.py
+-rw-r--r--   0        0        0     3396 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/svd.py
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 varipeps-0.5.4/PKG-INFO
```

### Comparing `varipeps-0.5.3/LICENSE` & `varipeps-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/pyproject.toml` & `varipeps-0.5.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "variPEPS"
-version = "0.5.3"
+version = "0.5.4"
 description = "Versatile tensor network library for variational ground state simulations in two spatial dimensions"
 authors = ["Jan Naumann <j.naumann@fu-berlin.de>", "Philipp Schmoll <philipp.schmoll@fu-berlin.de>", "Frederik Wilde", "Finn Krein"]
-license = "GPL-3.0 or later"
+license = "GPL-3.0-or-later"
 readme = "README.md"
+repository = "https://github.com/variPEPS/variPEPS_Python"
+documentation = "https://varipeps.readthedocs.io/en/stable/"
 packages = [{include = "varipeps"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 numpy = ">=1.21.2"
 scipy = ">=1.7.1"
 jax = {extras = ["cpu"], version = ">=0.3.16"}
```

### Comparing `varipeps-0.5.3/varipeps/__init__.py` & `varipeps-0.5.4/varipeps/__init__.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/__version__.py` & `varipeps-0.5.4/varipeps/__version__.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/config.py` & `varipeps-0.5.4/varipeps/config.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/contractions/apply.py` & `varipeps-0.5.4/varipeps/contractions/apply.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/contractions/definitions.py` & `varipeps-0.5.4/varipeps/contractions/definitions.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/ctmrg/absorption.py` & `varipeps-0.5.4/varipeps/ctmrg/absorption.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/ctmrg/projectors.py` & `varipeps-0.5.4/varipeps/ctmrg/projectors.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/ctmrg/routine.py` & `varipeps-0.5.4/varipeps/ctmrg/routine.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/expectation/model.py` & `varipeps-0.5.4/varipeps/expectation/model.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/expectation/one_site.py` & `varipeps-0.5.4/varipeps/expectation/one_site.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/expectation/spiral_helpers.py` & `varipeps-0.5.4/varipeps/expectation/spiral_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         Vector for the spatial difference.
       q (:term:`sequence` of :obj:`jax.numpy.ndarray`):
         Sequence with the relevant wavevector for the different indices of
         the gate.
       unitary_operator_D (:obj:`jax.numpy.ndarray`):
         Array with the eigenvalues of the operator from which the unitary
         is generated.
-      unitary_operator_D (:obj:`jax.numpy.ndarray`):
+      unitary_operator_sigma (:obj:`jax.numpy.ndarray`):
         Array with the eigenvectors of the operator from which the unitary
         is generated.
       phys_d (:obj:`int`):
         Physical dimension of the indices of the gate.
       number_sites (:obj:`int`):
         Number of sites the gate is applied to.
       apply_to_index (:term:`sequence` of :obj:`int`):
```

### Comparing `varipeps-0.5.3/varipeps/expectation/three_sites.py` & `varipeps-0.5.4/varipeps/expectation/three_sites.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/expectation/two_sites.py` & `varipeps-0.5.4/varipeps/expectation/two_sites.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/global_state.py` & `varipeps-0.5.4/varipeps/global_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from jax.tree_util import register_pytree_node_class
 
 from typing import TypeVar, Tuple, Any, Type, Optional
 
 from .config import Projector_Method
 
-T_VariPEPS_Global_State = TypeVar("T_VariPEPS_Global_State", bound="VariPEPS_Global_State")
+T_VariPEPS_Global_State = TypeVar(
+    "T_VariPEPS_Global_State", bound="VariPEPS_Global_State"
+)
 
 
 @dataclass
 @register_pytree_node_class
 class VariPEPS_Global_State:
     """
     Class to track internal global state. Values of the instance of this
```

### Comparing `varipeps-0.5.3/varipeps/mapping/florett_pentagon.py` & `varipeps-0.5.4/varipeps/mapping/florett_pentagon.py`

 * *Files 4% similar despite different names*

```diff
@@ -594,45 +594,45 @@
         blue_36 = jnp.kron(blue_e, Id_other_sites)
         blue_36 = blue_36.reshape(d, d, d, d, d, d, d, d, d, d, d, d, d, d, d, d, d, d)
         blue_36 = blue_36.transpose(
             2, 3, 0, 4, 5, 1, 6, 7, 8, 11, 12, 9, 13, 14, 10, 15, 16, 17
         )
         blue_36 = blue_36.reshape(d**9, d**9)
 
-        green_12 = jnp.kron(g_e, Id_other_sites)
-        green_12 = green_12.reshape(
+        green_base = jnp.kron(g_e, Id_other_sites)
+        green_base = green_base.reshape(
             d, d, d, d, d, d, d, d, d, d, d, d, d, d, d, d, d, d
         )
 
-        green_24 = green_12.transpose(
+        green_24 = green_base.transpose(
             2, 0, 3, 1, 4, 5, 6, 7, 8, 11, 9, 12, 10, 13, 14, 15, 16, 17
         )
         green_24 = green_24.reshape(d**9, d**9)
 
-        green_45 = green_12.transpose(
+        green_45 = green_base.transpose(
             2, 3, 4, 0, 1, 5, 6, 7, 8, 11, 12, 13, 9, 10, 14, 15, 16, 17
         )
         green_45 = green_45.reshape(d**9, d**9)
 
-        green_46 = green_12.transpose(
+        green_46 = green_base.transpose(
             2, 3, 4, 0, 5, 1, 6, 7, 8, 11, 12, 13, 9, 14, 10, 15, 16, 17
         )
         green_46 = green_46.reshape(d**9, d**9)
 
-        green_37 = green_12.transpose(
+        green_37 = green_base.transpose(
             2, 3, 0, 4, 5, 6, 1, 7, 8, 11, 12, 9, 13, 14, 15, 10, 16, 17
         )
         green_37 = green_37.reshape(d**9, d**9)
 
-        green_78 = green_12.transpose(
+        green_78 = green_base.transpose(
             2, 3, 4, 5, 6, 7, 0, 1, 8, 11, 12, 13, 14, 15, 16, 9, 10, 17
         )
         green_78 = green_78.reshape(d**9, d**9)
 
-        green_79 = green_12.transpose(
+        green_79 = green_base.transpose(
             2, 3, 4, 5, 6, 7, 0, 8, 1, 11, 12, 13, 14, 15, 16, 9, 17, 10
         )
         green_79 = green_79.reshape(d**9, d**9)
 
         result[i] = (
             black_12
             + black_13
@@ -865,15 +865,17 @@
             if all(jnp.allclose(g, jnp.real(g)) for g in self.green_gates)
             and all(jnp.allclose(g, jnp.real(g)) for g in self.blue_gates)
             and all(jnp.allclose(g, jnp.real(g)) for g in self.black_gates)
             else jnp.complex128
         )
 
         if self.is_spiral_peps:
-            raise NotImplementedError
+            self._spiral_D, self._spiral_sigma = jnp.linalg.eigh(
+                self.spiral_unitary_operator
+            )
 
     def __call__(
         self,
         peps_tensors: Sequence[jnp.ndarray],
         unitcell: PEPS_Unit_Cell,
         spiral_vectors: Optional[Union[jnp.ndarray, Sequence[jnp.ndarray]]] = None,
         *,
@@ -887,24 +889,154 @@
 
         if return_single_gate_results:
             single_gates_result = [dict()] * len(self.black_gates)
 
             working_onsite_gates = tuple(
                 o for e in self._onsite_single_gates for o in e
             )
-            working_h_single_gates = tuple(
-                h for e in self._right_single_gates for h in e
+
+        if self.is_spiral_peps:
+            if isinstance(spiral_vectors, jnp.ndarray):
+                spiral_vectors = (
+                    spiral_vectors,
+                    spiral_vectors,
+                    spiral_vectors,
+                )
+            if len(spiral_vectors) == 1:
+                spiral_vectors = (
+                    spiral_vectors[0],
+                    spiral_vectors[0],
+                    None,
+                    None,
+                    None,
+                    None,
+                    None,
+                    None,
+                    spiral_vectors[0],
+                )
+            if len(spiral_vectors) == 4:
+                spiral_vectors = (
+                    spiral_vectors[0],
+                    spiral_vectors[1],
+                    None,
+                    None,
+                    None,
+                    None,
+                    None,
+                    None,
+                    spiral_vectors[2],
+                )
+            if len(spiral_vectors) != 9:
+                raise ValueError("Length mismatch for spiral vectors!")
+
+            working_h_gates = tuple(
+                apply_unitary(
+                    h,
+                    jnp.array((0, 1)),
+                    spiral_vectors[0:9:8],
+                    self._spiral_D,
+                    self._spiral_sigma,
+                    self.real_d,
+                    3,
+                    (1, 2),
+                    varipeps_config.spiral_wavevector_type,
+                )
+                for h in self._right_tuple
             )
-            working_v_single_gates = tuple(
-                v for e in self._down_single_gates for v in e
+            working_v_gates = tuple(
+                apply_unitary(
+                    v,
+                    jnp.array((1, 0)),
+                    spiral_vectors[:2],
+                    self._spiral_D,
+                    self._spiral_sigma,
+                    self.real_d,
+                    4,
+                    (2, 3),
+                    varipeps_config.spiral_wavevector_type,
+                )
+                for v in self._down_tuple
             )
-            working_d_single_gates = tuple(
-                d for e in self._diagonal_single_gates for d in e
+            working_d_gates = tuple(
+                apply_unitary(
+                    d,
+                    jnp.array((1, 1)),
+                    spiral_vectors[:1],
+                    self._spiral_D,
+                    self._spiral_sigma,
+                    self.real_d,
+                    3,
+                    (2,),
+                    varipeps_config.spiral_wavevector_type,
+                )
+                for d in self._diagonal_tuple
             )
 
+            if return_single_gate_results:
+                working_h_single_gates = tuple(
+                    apply_unitary(
+                        h,
+                        jnp.array((0, 1)),
+                        spiral_vectors[0:9:8],
+                        self._spiral_D,
+                        self._spiral_sigma,
+                        self.real_d,
+                        3,
+                        (1, 2),
+                        varipeps_config.spiral_wavevector_type,
+                    )
+                    for e in self._right_single_gates
+                    for h in e
+                )
+                working_v_single_gates = tuple(
+                    apply_unitary(
+                        v,
+                        jnp.array((1, 0)),
+                        spiral_vectors[:2],
+                        self._spiral_D,
+                        self._spiral_sigma,
+                        self.real_d,
+                        4,
+                        (2, 3),
+                        varipeps_config.spiral_wavevector_type,
+                    )
+                    for e in self._down_single_gates
+                    for v in e
+                )
+                working_d_single_gates = tuple(
+                    apply_unitary(
+                        d,
+                        jnp.array((1, 1)),
+                        spiral_vectors[:1],
+                        self._spiral_D,
+                        self._spiral_sigma,
+                        self.real_d,
+                        3,
+                        (2,),
+                        varipeps_config.spiral_wavevector_type,
+                    )
+                    for e in self._diagonal_single_gates
+                    for d in e
+                )
+        else:
+            working_h_gates = self._right_tuple
+            working_v_gates = self._down_tuple
+            working_d_gates = self._diagonal_tuple
+
+            if return_single_gate_results:
+                working_h_single_gates = tuple(
+                    h for e in self._right_single_gates for h in e
+                )
+                working_v_single_gates = tuple(
+                    v for e in self._down_single_gates for v in e
+                )
+                working_d_single_gates = tuple(
+                    d for e in self._diagonal_single_gates for d in e
+                )
+
         for x, iter_rows in unitcell.iter_all_rows(only_unique=only_unique):
             for y, view in iter_rows:
                 # On site term
                 if len(self.black_gates) > 0:
                     onsite_tensor = peps_tensors[view.get_indices((0, 0))[0][0]]
                     onsite_tensor_obj = view[0, 0][0][0]
 
@@ -933,22 +1065,22 @@
                         horizontal_tensors, horizontal_tensor_objs, ((5,), (1, 9))
                     )
 
                     if return_single_gate_results:
                         step_result_horizontal = _two_site_workhorse(
                             density_matrix_left,
                             density_matrix_right,
-                            self._right_tuple + working_h_single_gates,
+                            working_h_gates + working_h_single_gates,
                             self._result_type is jnp.float64,
                         )
                     else:
                         step_result_horizontal = _two_site_workhorse(
                             density_matrix_left,
                             density_matrix_right,
-                            self._right_tuple,
+                            working_h_gates,
                             self._result_type is jnp.float64,
                         )
 
                     vertical_tensors_i = view.get_indices((slice(0, 2, None), 0))
                     vertical_tensors = [
                         peps_tensors[i] for j in vertical_tensors_i for i in j
                     ]
@@ -960,22 +1092,22 @@
                         vertical_tensors, vertical_tensor_objs, ((8, 9), (1, 2))
                     )
 
                     if return_single_gate_results:
                         step_result_vertical = _two_site_workhorse(
                             density_matrix_top,
                             density_matrix_bottom,
-                            self._down_tuple + working_v_single_gates,
+                            working_v_gates + working_v_single_gates,
                             self._result_type is jnp.float64,
                         )
                     else:
                         step_result_vertical = _two_site_workhorse(
                             density_matrix_top,
                             density_matrix_bottom,
-                            self._down_tuple,
+                            working_v_gates,
                             self._result_type is jnp.float64,
                         )
 
                     diagonal_tensors_i = view.get_indices(
                         (slice(0, 2, None), slice(0, 2, None))
                     )
                     diagonal_tensors = [
@@ -1007,24 +1139,24 @@
 
                     if return_single_gate_results:
                         step_result_diagonal = _two_site_diagonal_workhorse(
                             density_matrix_top_left,
                             density_matrix_bottom_right,
                             traced_density_matrix_top_right,
                             traced_density_matrix_bottom_left,
-                            self._diagonal_tuple + working_d_single_gates,
+                            working_d_gates + working_d_single_gates,
                             self._result_type is jnp.float64,
                         )
                     else:
                         step_result_diagonal = _two_site_diagonal_workhorse(
                             density_matrix_top_left,
                             density_matrix_bottom_right,
                             traced_density_matrix_top_right,
                             traced_density_matrix_bottom_left,
-                            self._diagonal_tuple,
+                            working_d_gates,
                             self._result_type is jnp.float64,
                         )
 
                     for sr_i, (sr_o, sr_h, sr_v, sr_d) in enumerate(
                         jax.util.safe_zip(
                             step_result_onsite[: len(self.black_gates)],
                             step_result_horizontal[: len(self.black_gates)],
```

### Comparing `varipeps-0.5.3/varipeps/mapping/honeycomb.py` & `varipeps-0.5.4/varipeps/mapping/honeycomb.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,13 +618,11 @@
         auxiliary_data: Optional[Dict[str, Any]] = None,
     ) -> None:
         if counter is not None:
             cls.save_to_file(
                 f"{str(filename)}.{counter}",
                 tensors,
                 unitcell,
-                auxiliary_data=auxiliary_data
+                auxiliary_data=auxiliary_data,
             )
         else:
-            cls.save_to_file(
-                filename, tensors, unitcell, auxiliary_data=auxiliary_data
-            )
+            cls.save_to_file(filename, tensors, unitcell, auxiliary_data=auxiliary_data)
```

### Comparing `varipeps-0.5.3/varipeps/mapping/kagome.py` & `varipeps-0.5.4/varipeps/mapping/kagome.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,20 +623,18 @@
         auxiliary_data: Optional[Dict[str, Any]] = None,
     ) -> None:
         if counter is not None:
             cls.save_to_file(
                 f"{str(filename)}.{counter}",
                 tensors,
                 unitcell,
-                auxiliary_data=auxiliary_data
+                auxiliary_data=auxiliary_data,
             )
         else:
-            cls.save_to_file(
-                filename, tensors, unitcell, auxiliary_data=auxiliary_data
-            )
+            cls.save_to_file(filename, tensors, unitcell, auxiliary_data=auxiliary_data)
 
 
 class iPESS3_9Sites_Three_PEPS_Site:
     """
     Map a 9-sites Kagome iPESS3 unit cell to PEPS structure using a PEPS
     unitcell consisting of three unique sites.
     """
```

### Comparing `varipeps-0.5.3/varipeps/mapping/maple_leaf.py` & `varipeps-0.5.4/varipeps/mapping/maple_leaf.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,26 @@
 from varipeps.utils.random import PEPS_Random_Number_Generator
 
 from varipeps.mapping.square_kagome import (
     square_kagome_density_matrix_horizontal,
     square_kagome_density_matrix_vertical,
 )
 
-from typing import Sequence, Union, List, Callable, TypeVar, Optional, Tuple, Type, Dict, Any
+from typing import (
+    Sequence,
+    Union,
+    List,
+    Callable,
+    TypeVar,
+    Optional,
+    Tuple,
+    Type,
+    Dict,
+    Any,
+)
 
 T_Maple_Leaf_Map_PESS_To_PEPS = TypeVar(
     "T_Maple_Leaf_Map_PESS_To_PEPS", bound="Maple_Leaf_Map_PESS_To_PEPS"
 )
 
 
 def maple_leaf_density_matrix_diagonal(
@@ -1280,10 +1291,8 @@
             cls.save_to_file(
                 f"{str(filename)}.{counter}",
                 tensors,
                 unitcell,
                 auxiliary_data=auxiliary_data,
             )
         else:
-            cls.save_to_file(
-                filename, tensors, unitcell, auxiliary_data=auxiliary_data
-            )
+            cls.save_to_file(filename, tensors, unitcell, auxiliary_data=auxiliary_data)
```

### Comparing `varipeps-0.5.3/varipeps/mapping/model.py` & `varipeps-0.5.4/varipeps/mapping/model.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/mapping/square_kagome.py` & `varipeps-0.5.4/varipeps/mapping/square_kagome.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,26 @@
 from varipeps.expectation.one_site import calc_one_site_multi_gates
 from varipeps.expectation.two_sites import _two_site_workhorse
 from varipeps.expectation.spiral_helpers import apply_unitary
 from varipeps.typing import Tensor
 from varipeps.mapping import Map_To_PEPS_Model
 from varipeps.utils.random import PEPS_Random_Number_Generator
 
-from typing import Sequence, Union, List, Callable, TypeVar, Optional, Tuple, Type, Dict, Any
+from typing import (
+    Sequence,
+    Union,
+    List,
+    Callable,
+    TypeVar,
+    Optional,
+    Tuple,
+    Type,
+    Dict,
+    Any,
+)
 
 T_Square_Kagome_Map_PESS_To_PEPS = TypeVar(
     "T_Square_Kagome_Map_PESS_To_PEPS", bound="Square_Kagome_Map_PESS_To_PEPS"
 )
 T_Square_Kagome_Map_4_1_1_To_PEPS = TypeVar(
     "T_Square_Kagome_Map_4_1_1_To_PEPS", bound="Square_Kagome_Map_4_1_1_To_PEPS"
 )
@@ -1231,20 +1242,18 @@
         auxiliary_data: Optional[Dict[str, Any]] = None,
     ) -> None:
         if counter is not None:
             cls.save_to_file(
                 f"{str(filename)}.{counter}",
                 tensors,
                 unitcell,
-                auxiliary_data=auxiliary_data
+                auxiliary_data=auxiliary_data,
             )
         else:
-            cls.save_to_file(
-                filename, tensors, unitcell, auxiliary_data=auxiliary_data
-            )
+            cls.save_to_file(filename, tensors, unitcell, auxiliary_data=auxiliary_data)
 
 
 @jit
 def _map_4_1_1(input_tensors):
     (t1, t6, square_tensor) = input_tensors
 
     result = jnp.tensordot(t1, square_tensor, ((2,), (1,)))
@@ -1607,13 +1616,11 @@
         auxiliary_data: Optional[Dict[str, Any]] = None,
     ) -> None:
         if counter is not None:
             cls.save_to_file(
                 f"{str(filename)}.{counter}",
                 tensors,
                 unitcell,
-                auxiliary_data=auxiliary_data
+                auxiliary_data=auxiliary_data,
             )
         else:
-            cls.save_to_file(
-                filename, tensors, unitcell, auxiliary_data=auxiliary_data
-            )
+            cls.save_to_file(filename, tensors, unitcell, auxiliary_data=auxiliary_data)
```

### Comparing `varipeps-0.5.3/varipeps/mapping/triangular.py` & `varipeps-0.5.4/varipeps/mapping/triangular.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,26 @@
     calc_two_sites_horizontal_multiple_gates,
     calc_two_sites_diagonal_top_left_bottom_right_multiple_gates,
 )
 from varipeps.typing import Tensor
 from varipeps.utils.random import PEPS_Random_Number_Generator
 from varipeps.mapping import Map_To_PEPS_Model
 
-from typing import Sequence, Union, List, Callable, TypeVar, Optional, Tuple, Type, Dict, Any
+from typing import (
+    Sequence,
+    Union,
+    List,
+    Callable,
+    TypeVar,
+    Optional,
+    Tuple,
+    Type,
+    Dict,
+    Any,
+)
 
 T_Triangular_Map_PESS_To_PEPS = TypeVar(
     "T_Triangular_Map_PESS_To_PEPS", bound="Triangular_Map_PESS_To_PEPS"
 )
 
 
 @dataclass
@@ -503,13 +514,11 @@
         auxiliary_data: Optional[Dict[str, Any]] = None,
     ) -> None:
         if counter is not None:
             cls.save_to_file(
                 f"{str(filename)}.{counter}",
                 tensors,
                 unitcell,
-                auxiliary_data=auxiliary_data
+                auxiliary_data=auxiliary_data,
             )
         else:
-            cls.save_to_file(
-                filename, tensors, unitcell, auxiliary_data=auxiliary_data
-            )
+            cls.save_to_file(filename, tensors, unitcell, auxiliary_data=auxiliary_data)
```

### Comparing `varipeps-0.5.3/varipeps/optimization/basinhopping.py` & `varipeps-0.5.4/varipeps/optimization/basinhopping.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/optimization/inner_function.py` & `varipeps-0.5.4/varipeps/optimization/inner_function.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/optimization/line_search.py` & `varipeps-0.5.4/varipeps/optimization/line_search.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/optimization/optimizer.py` & `varipeps-0.5.4/varipeps/optimization/optimizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -273,14 +273,15 @@
     working_value = None
 
     max_trunc_error = jnp.nan
 
     best_value = jnp.inf
     best_tensors = None
     best_unitcell = None
+    best_run = None
 
     random_noise_retries = 0
 
     signal_reset_descent_dir = False
 
     spiral_indices = None
     if (
@@ -303,15 +304,18 @@
         l_bfgs_grad_cache = deque(maxlen=varipeps_config.optimizer_l_bfgs_maxlen + 1)
 
     count = 0
     linesearch_step: Union[float, jnp.ndarray] = (
         varipeps_config.line_search_initial_step_size
     )
     working_value: Union[float, jnp.ndarray]
-    max_trunc_error_list = []
+    max_trunc_error_list = {random_noise_retries: []}
+    step_energies = {random_noise_retries: []}
+    step_chi = {random_noise_retries: []}
+    step_conv = {random_noise_retries: []}
 
     if (
         varipeps_config.optimizer_preconverge_with_half_projectors
         and not varipeps_global_state.basinhopping_disable_half_projector
     ):
         varipeps_global_state.ctmrg_projector_method = Projector_Method.HALF
     else:
@@ -413,14 +417,15 @@
             signal_reset_descent_dir = False
 
             if _scalar_descent_grad(descent_dir, working_gradient) > 0:
                 tqdm.write("Found bad descent dir. Reset to negative gradient!")
                 descent_dir = [-elem for elem in working_gradient]
 
             conv = jnp.linalg.norm(ravel_pytree(working_gradient)[0])
+            step_conv[random_noise_retries].append(conv)
 
             try:
                 (
                     working_tensors,
                     working_unitcell,
                     working_value,
                     linesearch_step,
@@ -456,14 +461,15 @@
                             "Convergence is not sufficient. Retry with some random noise on best result."
                         )
 
                         if working_value < best_value:
                             best_value = working_value
                             best_tensors = working_tensors
                             best_unitcell = working_unitcell
+                            best_run = random_noise_retries
 
                         if isinstance(input_tensors, PEPS_Unit_Cell) or (
                             isinstance(input_tensors, collections.abc.Sequence)
                             and isinstance(input_tensors[0], PEPS_Unit_Cell)
                         ):
                             working_tensors = (
                                 cast(
@@ -493,35 +499,46 @@
                             working_unitcell = None
 
                         descent_dir = None
                         working_gradient = None
                         signal_reset_descent_dir = True
                         count = -1
                         random_noise_retries += 1
+
+                        step_energies[random_noise_retries] = []
+                        step_chi[random_noise_retries] = []
+                        step_conv[random_noise_retries] = []
+                        max_trunc_error_list[random_noise_retries] = []
+
                         pbar.reset()
                         pbar.refresh()
                     else:
                         conv = 0
-
-            max_trunc_error_list.append(max_trunc_error)
+            else:
+                max_trunc_error_list[random_noise_retries].append(max_trunc_error)
+                step_energies[random_noise_retries].append(working_value)
+                step_chi[random_noise_retries].append(
+                    working_unitcell.get_unique_tensors()[0].chi
+                )
 
             if conv < varipeps_config.optimizer_convergence_eps:
                 working_value, (
                     working_unitcell,
                     max_trunc_error,
                 ) = calc_ctmrg_expectation(
                     working_tensors,
                     working_unitcell,
                     expectation_func,
                     convert_to_unitcell_func,
                     additional_input,
                     enforce_elementwise_convergence=varipeps_config.ad_use_custom_vjp,
                 )
                 varipeps_global_state.ctmrg_projector_method = None
-                max_trunc_error_list[-1] = max_trunc_error
+                max_trunc_error_list[random_noise_retries][-1] = max_trunc_error
+                step_energies[random_noise_retries][-1] = working_value
                 break
 
             if (
                 varipeps_config.optimizer_preconverge_with_half_projectors
                 and not varipeps_global_state.basinhopping_disable_half_projector
                 and conv
                 < varipeps_config.optimizer_preconverge_with_half_projectors_eps
@@ -557,15 +574,24 @@
                     "Max. trunc. err.": f"{max_trunc_error:0.8g}",
                 }
             )
             pbar.refresh()
 
             if count % varipeps_config.optimizer_autosave_step_count == 0:
                 auxiliary_data = {
-                    "max_trunc_error_list": max_trunc_error_list,
+                    "max_trunc_error_list": tuple(
+                        max_trunc_error_list[k]
+                        for k in sorted(max_trunc_error_list.keys())
+                    ),
+                    "step_energies": tuple(
+                        step_energies[k] for k in sorted(step_energies.keys())
+                    ),
+                    "step_chi": tuple(step_chi[k] for k in sorted(step_chi.keys())),
+                    "step_conv": tuple(step_conv[k] for k in sorted(step_conv.keys())),
+                    "best_run": best_run if best_run is not None else 0,
                 }
 
                 if spiral_indices is not None:
                     for spiral_i in spiral_indices:
                         auxiliary_data[f"spiral_vector_{spiral_i:d}"] = working_tensors[
                             spiral_i
                         ]
@@ -585,18 +611,23 @@
                     auxiliary_data=auxiliary_data,
                 )
 
     if working_value < best_value:
         best_value = working_value
         best_tensors = working_tensors
         best_unitcell = working_unitcell
+        best_run = random_noise_retries
 
     print(f"Best energy result found: {best_value}")
 
     return OptimizeResult(
         success=True,
         x=best_tensors,
         fun=best_value,
         unitcell=best_unitcell,
         nit=count,
         max_trunc_error_list=max_trunc_error_list,
+        step_energies=step_energies,
+        step_chi=step_chi,
+        step_conv=step_conv,
+        best_run=best_run,
     )
```

### Comparing `varipeps-0.5.3/varipeps/peps/tensor.py` & `varipeps-0.5.4/varipeps/peps/tensor.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/peps/unitcell.py` & `varipeps-0.5.4/varipeps/peps/unitcell.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/typing.py` & `varipeps-0.5.4/varipeps/typing.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/utils/debug_print.py` & `varipeps-0.5.4/varipeps/utils/debug_print.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/utils/func_cache.py` & `varipeps-0.5.4/varipeps/utils/func_cache.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/utils/periodic_indices.py` & `varipeps-0.5.4/varipeps/utils/periodic_indices.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/utils/projector_dict.py` & `varipeps-0.5.4/varipeps/utils/projector_dict.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/utils/random.py` & `varipeps-0.5.4/varipeps/utils/random.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.3/varipeps/utils/svd.py` & `varipeps-0.5.4/varipeps/utils/svd.py`

 * *Files identical despite different names*

