# Comparing `tmp/connectome_interpreter-1.4.1.tar.gz` & `tmp/connectome_interpreter-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.4.1.tar", last modified: Sat Apr 20 15:30:10 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.5.0.tar", last modified: Sun Apr 21 22:28:32 2024, max compression
```

## Comparing `connectome_interpreter-1.4.1.tar` & `connectome_interpreter-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:30:10.279308 connectome_interpreter-1.4.1/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.4.1/LICENSE
--rw-rw-rw-   0        0        0      938 2024-04-20 15:30:10.277968 connectome_interpreter-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:30:10.256308 connectome_interpreter-1.4.1/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.4.1/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    33223 2024-04-15 08:20:09.000000 connectome_interpreter-1.4.1/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    18727 2024-04-18 22:37:14.000000 connectome_interpreter-1.4.1/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16261 2024-04-14 17:16:24.000000 connectome_interpreter-1.4.1/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    30999 2024-04-20 15:28:13.000000 connectome_interpreter-1.4.1/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:30:10.275864 connectome_interpreter-1.4.1/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0      938 2024-04-20 15:30:09.000000 connectome_interpreter-1.4.1/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2024-04-20 15:30:10.000000 connectome_interpreter-1.4.1/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:30:09.000000 connectome_interpreter-1.4.1/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-04-20 15:30:09.000000 connectome_interpreter-1.4.1/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-04-20 15:30:09.000000 connectome_interpreter-1.4.1/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 15:30:10.279308 connectome_interpreter-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1557 2024-04-20 15:28:44.000000 connectome_interpreter-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:30:10.276863 connectome_interpreter-1.4.1/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.4.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.4.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:28:32.483544 connectome_interpreter-1.5.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0      938 2024-04-21 22:28:32.483544 connectome_interpreter-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 22:28:32.438568 connectome_interpreter-1.5.0/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.5.0/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    33223 2024-04-15 08:20:09.000000 connectome_interpreter-1.5.0/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    17800 2024-04-21 21:48:11.000000 connectome_interpreter-1.5.0/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16261 2024-04-14 17:16:24.000000 connectome_interpreter-1.5.0/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    31484 2024-04-20 23:13:30.000000 connectome_interpreter-1.5.0/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:28:32.469242 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0      938 2024-04-21 22:28:32.000000 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-04-21 22:28:32.000000 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 22:28:32.000000 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-04-21 22:28:32.000000 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-21 22:28:32.000000 connectome_interpreter-1.5.0/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-21 22:28:32.484539 connectome_interpreter-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1557 2024-04-20 17:52:45.000000 connectome_interpreter-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:28:32.481552 connectome_interpreter-1.5.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.5.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.5.0/tests/test_compress_paths.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.5.0/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.4.1/LICENSE` & `connectome_interpreter-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.4.1/PKG-INFO` & `connectome_interpreter-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome_interpreter
-Version: 1.4.1
+Version: 1.5.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
```

### Comparing `connectome_interpreter-1.4.1/README.md` & `connectome_interpreter-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.4.1/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.5.0/connectome_interpreter/activation_maximisation.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.4.1/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.5.0/connectome_interpreter/compress_paths.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import torch
 from tqdm import tqdm
 import pandas as pd
 import plotly.express as px
 from scipy.sparse import issparse
 
-from .utils import dynamic_representation, torch_sparse_where, to_nparray
+from .utils import dynamic_representation, torch_sparse_where, to_nparray, tensor_to_csc
 
 
 def compress_paths(inprop, step_number, threshold=0, output_threshold=1e-4):
     """
     Performs iterative multiplication of a sparse matrix `inprop` for a specified number of steps, 
     applying thresholding to filter out values below a certain `threshold` to optimize memory usage 
     and computation speed. The function is optimized to run on GPU if available. 
@@ -26,22 +26,20 @@
         step_number (int): The number of iterations to perform the matrix multiplication.
         threshold (float, optional): The threshold value to apply after each multiplication. 
                                      Values below this threshold are set to zero. Defaults to 0.
         output_threshold (float, optional): The threshold value to apply to the final output, 
                                             used to reduce memory footprint. Defaults to 1e-4.
 
     Returns:
-        list: A list of `torch.Tensor` objects, each representing the sparse matrix after each 
-              iteration of compression, with each tensor being processed to save memory.
+        list: A list of scipy.sparse.csc_matrix objects, each representing connectivity from all neurons to all neurons n steps away. 
 
     Note:
         This function requires PyTorch and is designed to automatically utilize CUDA-enabled GPU devices 
         if available to accelerate computations. The input matrix `inprop` is converted to a dense tensor 
-        before processing. Intermediate results are stored in a list of tensors, where each tensor is 
-        converted to a sparse format after thresholding to save memory.
+        before processing. 
 
     Example:
         >>> from scipy.sparse import csr_matrix
         >>> import numpy as np
         >>> inprop = csr_matrix(np.array([[0.1, 0.2], [0.3, 0.4]]))
         >>> step_number = 2
         >>> compressed_paths = compress_paths(inprop, step_number, threshold=0.1, output_threshold=0.01)
@@ -52,65 +50,52 @@
 
     inprop_tensor = torch.tensor(inprop.toarray(), device=device)
 
     for i in tqdm(range(step_number)):
         if i == 0:
             out_tensor = inprop_tensor
         else:
-            out_tensor = torch.matmul(steps_fast[-1], inprop_tensor)
+            out_tensor = torch.matmul(out_tensor, inprop_tensor)
 
-            # Downgrade the previous one to save memory
-            steps_fast[-1] = torch.where(steps_fast[-1] >= output_threshold,
-                                         steps_fast[-1], torch.tensor(0.0, device=device))
-            steps_fast[-1] = steps_fast[-1].to_sparse()
+            # # Downgrade the previous one to save memory
+            # steps_fast[-1] = torch.where(steps_fast[-1] >= output_threshold,
+            #                              steps_fast[-1], torch.tensor(0.0, device=device))
+            # steps_fast[-1] = steps_fast[-1].to_sparse()
 
-        # Thresholding
+        # Thresholding during matmul
         if threshold != 0:
             out_tensor = torch.where(
                 out_tensor >= threshold, out_tensor, torch.tensor(0.0, device=device))
 
-        steps_fast.append(out_tensor)
-
-    # Downgrade the last one to save memory
-    steps_fast[-1] = torch.where(steps_fast[-1] >= output_threshold,
-                                 steps_fast[-1], torch.tensor(0.0, device=device))
-    steps_fast[-1] = steps_fast[-1].to_sparse()
+        # Thresholding for output
+        out_csc = torch.where(out_tensor >= output_threshold,
+                              out_tensor, torch.tensor(0.0, device=device))
+        out_csc = tensor_to_csc(out_csc.to('cpu'))
+        steps_fast.append(out_csc)
 
+    torch.cuda.empty_cache()
     return steps_fast
 
 
 def compress_paths_signed(inprop, idx_to_sign, target_layer_number, threshold=0, output_threshold=1e-4):
     """
-    Calculates the cumulative excitatory and inhibitory influences across specified layers of a neural network, using PyTorch for GPU acceleration. This function processes a connectivity matrix (where presynaptic neurons are represented by rows and postsynaptic neurons by columns) to distinguish and compute the cumulative influence of excitatory and inhibitory neurons at each layer.
+    Calculates the excitatory and inhibitory influences across specified layers of a neural network, using PyTorch for GPU acceleration. This function processes a connectivity matrix (where presynaptic neurons are represented by rows and postsynaptic neurons by columns) to distinguish and compute the influence of excitatory and inhibitory neurons at each layer.
 
     Args:
-        inprop (torch.Tensor or scipy.sparse.csc_matrix): The initial connectivity matrix representing direct connections between adjacent layers. If a scipy sparse matrix is provided, it is converted to a dense PyTorch tensor.
+        inprop (scipy.sparse.csc_matrix): The initial connectivity matrix representing direct connections between adjacent layers. 
         idx_to_sign (dict): A dictionary mapping neuron indices to their types (1 for excitatory, -1 for inhibitory), used to differentiate between excitatory and inhibitory influences.
-        target_layer_number (int): The number of layers through which to calculate cumulative influences, starting from the second layer (with the first layer's influence being defined by `inprop`).
-        threshold (float, optional): A value to threshold the influences; influences below this value are set to zero. Defaults to 0.
+        target_layer_number (int): The number of layers through which to calculate influences, starting from the second layer (with the first layer's influence, the direct connectivity, being defined by `inprop`).
+        threshold (float, optional): A value to threshold the influences; influences below this value are set to zero, and not passed on in future layers. Defaults to 0.
         output_threshold (float, optional): A threshold for the final output to reduce memory usage, with values below this threshold set to zero. Defaults to 1e-4.
 
     Returns:
-        Tuple[List[torch.Tensor], List[torch.Tensor]]: Two lists of tensors representing the cumulative excitatory and inhibitory influences, respectively, up to the specified target layer. Each tensor is stored on the GPU and can be moved to the CPU or converted to numpy arrays as needed.
-
-    Example:
-        >>> import torch
-        >>> n_neurons = 4  # Example size, replace with your actual size
-        >>> inprop = torch.tensor([[0, 0.7, 0.2, 0.1],
-                                [0.5, 0, 0.3, 0.5],
-                                [0.4, 0.2, 0, 0.4],
-                                [0.1, 0.1, 0.5, 0]], dtype=torch.float32)
-        >>> idx_to_sign = {0: 1, 1: 1, 2: -1, 3: -1}  # Mapping of indices to sign (1 for excitatory, -1 for inhibitory)
-        >>> target_layer_number = 3
-        >>> lne_gpu, lni_gpu = compress_paths_signed(inprop, idx_to_sign, target_layer_number)
-        >>> print("Cumulative excitatory influence (GPU):\\n", lne_gpu[0].cpu().numpy())
-        >>> print("Cumulative inhibitory influence (GPU):\\n", lni_gpu[0].cpu().numpy())
+        Tuple[List[scipy.sparse.csc_matrix], List[scipy.sparse.csc_matrix]]: Two lists of sparse matrices representing the excitatory and inhibitory influences, respectively, up to the specified target layer. 
 
     Note:
-        This function requires PyTorch with GPU support. Ensure your environment supports CUDA and that PyTorch is correctly installed.
+        This function is ideal with GPU support. Ensure your environment supports CUDA and that PyTorch is correctly installed.
     """
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     inprop_tensor = torch.tensor(
         inprop.toarray(), device=device, dtype=torch.float32)
 
     # Create masks for excitatory and inhibitory neurons
@@ -138,37 +123,44 @@
             lni_new = torch.matmul(
                 lne, steps_inhibitory[0]) + torch.matmul(lni, steps_excitatory[0])
 
             # Apply thresholding
             if threshold > 0:
                 lne_new = torch_sparse_where(lne_new, threshold)
                 lni_new = torch_sparse_where(lni_new, threshold)
-                # lne_new = torch.where(lne_new >= threshold, lne_new, torch.tensor(0.0, device=device))
-                # lni_new = torch.where(lni_new >= threshold, lni_new, torch.tensor(0.0, device=device))
 
             # Dynamic representation based on density
             lne = dynamic_representation(lne_new)
             lni = dynamic_representation(lni_new)
             torch.cuda.empty_cache()
 
-        steps_excitatory.append(lne)
-        steps_inhibitory.append(lni)
+        # steps_excitatory.append(lne)
+        # steps_inhibitory.append(lni)
 
-        # Downgrade previous matrices to save memory
-        if steps_excitatory:
-            steps_excitatory[-1] = torch_sparse_where(
-                steps_excitatory[-1], output_threshold).to_sparse()
-            steps_inhibitory[-1] = torch_sparse_where(
-                steps_inhibitory[-1], output_threshold).to_sparse()
-
-    # Downgrade the last one to save memory
-    steps_excitatory[-1] = torch_sparse_where(
-        steps_excitatory[-1], output_threshold).to_sparse()
-    steps_inhibitory[-1] = torch_sparse_where(
-        steps_inhibitory[-1], output_threshold).to_sparse()
+        # Thresholding for output
+        stepe_csc = torch_sparse_where(lne, output_threshold)
+        stepe_csc = tensor_to_csc(stepe_csc.to('cpu'))
+        steps_excitatory.append(stepe_csc)
+
+        stepi_csc = torch_sparse_where(lni, output_threshold)
+        stepi_csc = tensor_to_csc(stepi_csc.to('cpu'))
+        steps_inhibitory.append(stepi_csc)
+
+    #     # Downgrade previous matrices to save memory
+    #     if steps_excitatory:
+    #         steps_excitatory[-1] = torch_sparse_where(
+    #             steps_excitatory[-1], output_threshold).to_sparse()
+    #         steps_inhibitory[-1] = torch_sparse_where(
+    #             steps_inhibitory[-1], output_threshold).to_sparse()
+
+    # # Downgrade the last one to save memory
+    # steps_excitatory[-1] = torch_sparse_where(
+    #     steps_excitatory[-1], output_threshold).to_sparse()
+    # steps_inhibitory[-1] = torch_sparse_where(
+    #     steps_inhibitory[-1], output_threshold).to_sparse()
     torch.cuda.empty_cache()
 
     return steps_excitatory, steps_inhibitory
 
 
 def add_first_n_matrices(matrices, n):
     """
```

### Comparing `connectome_interpreter-1.4.1/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.5.0/connectome_interpreter/path_finding.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.4.1/connectome_interpreter/utils.py` & `connectome_interpreter-1.5.0/connectome_interpreter/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,27 @@
 from tqdm import tqdm
 import networkx as nx
 
 
 def dynamic_representation(tensor, density_threshold=0.2):
     """Convert tensor to sparse if density is below threshold, otherwise to dense."""
     nonzero_elements = torch.nonzero(tensor).size(0)
-    total_elements = tensor.numel()
-    density = nonzero_elements / total_elements
 
-    if density < density_threshold:
-        return tensor.to_sparse()
+    # to_sparse() doesn't support operations on tensors with more than INT_MAX (2,147,483,647) elements
+    if nonzero_elements < 2147483647:
+        total_elements = tensor.numel()
+        density = nonzero_elements / total_elements
+
+        if density < density_threshold:
+            return tensor.to_sparse()
+        else:
+            return tensor.to_dense()
     else:
-        return tensor.to_dense()
+        print("Tensor is too large to convert to sparse. Returning dense tensor.")
+        return tensor
 
 
 def torch_sparse_where(x, threshold):
     """
     Apply a threshold to a tensor, setting values below the threshold to zero. This function allows the tensor to be sparse. torch.where() does not.
 
     Args:
@@ -54,33 +60,34 @@
     return result
 
 
 def tensor_to_csc(tensor):
     """Turn torch.Tensor into scipy Compressed Sparse Column matrix.
 
     Args:
-      tensor (torch.Tensor): A sparse tensor.
+      tensor (torch.Tensor): A (sparse) tensor.
 
     Returns:
       scipy.sparse.csc_matrix: A Scipy sparse Compressed Sparse Column matrix.
     """
-    tensor = tensor.to('cpu').coalesce()
-    # Extract indices and values
-    indices = tensor.indices().numpy()
-    values = tensor.values().numpy()
-    # Calculate the shape of the original tensor
-    shape = tensor.shape
-
-    # Create a SciPy COO matrix
-    coo = coo_matrix((values, (indices[0], indices[1])), shape=shape)
-
-    # Convert COO matrix to CSC matrix
-    csc = coo.tocsc()
+    if tensor.is_sparse:
+        tensor = tensor.coalesce()
+        indices = tensor.indices().numpy()
+        values = tensor.values().numpy()
+        shape = tensor.shape
+        coo = coo_matrix((values, (indices[0], indices[1])), shape=shape)
+    else:
+        # Convert dense tensor to COO directly, necessary if the tensor is not sparse
+        indices = torch.nonzero(tensor).t()
+        values = tensor[indices[0], indices[1]]
+        shape = tensor.shape
+        coo = coo_matrix(
+            (values.numpy(), (indices[0].numpy(), indices[1].numpy())), shape=shape)
 
-    return csc
+    return coo.tocsc()
 
 
 def coo_tensor_to_el(coo_tensor):
     """
     Convert a PyTorch sparse COO tensor to a DataFrame representing an edge list.
 
     This function checks if the input tensor is sparse. If not, it converts it to a sparse COO tensor.
```

### Comparing `connectome_interpreter-1.4.1/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.5.0/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome-interpreter
-Version: 1.4.1
+Version: 1.5.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
 Keywords: connectomics,neural network,mechanistic interpretability
```

### Comparing `connectome_interpreter-1.4.1/setup.py` & `connectome_interpreter-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.4.1',
+    version='1.5.0',
     packages=find_packages(),
     install_requires=[
         # List your package dependencies here
         'numpy',
         'pandas',
         'scipy',
         'torch',
```

### Comparing `connectome_interpreter-1.4.1/tests/test_utils.py` & `connectome_interpreter-1.5.0/tests/test_utils.py`

 * *Files identical despite different names*

