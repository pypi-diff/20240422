# Comparing `tmp/onediffx-1.0.0.dev202404200125.tar.gz` & `tmp/onediffx-1.0.0.dev202404210128.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediffx-1.0.0.dev202404200125.tar", last modified: Sat Apr 20 01:25:37 2024, max compression
+gzip compressed data, was "onediffx-1.0.0.dev202404210128.tar", last modified: Sun Apr 21 01:28:56 2024, max compression
```

## Comparing `onediffx-1.0.0.dev202404200125.tar` & `onediffx-1.0.0.dev202404210128.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.036902 onediffx-1.0.0.dev202404200125/
--rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-04-20 01:25:37.036902 onediffx-1.0.0.dev202404200125/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21461 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.028902 onediffx-1.0.0.dev202404200125/onediffx/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.028902 onediffx-1.0.0.dev202404200125/onediffx/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/compilers/diffusion_pipeline_compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.032902 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.032902 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/fast_unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_2d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_3d_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_video_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.032902 onediffx-1.0.0.dev202404200125/onediffx/lora/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/state_dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/text_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/lora/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.032902 onediffx-1.0.0.dev202404200125/onediffx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/onediffx/utils/patch_image_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.036902 onediffx-1.0.0.dev202404200125/onediffx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-04-20 01:25:37.000000 onediffx-1.0.0.dev202404200125/onediffx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-20 01:25:37.000000 onediffx-1.0.0.dev202404200125/onediffx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:25:37.000000 onediffx-1.0.0.dev202404200125/onediffx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-20 01:25:37.000000 onediffx-1.0.0.dev202404200125/onediffx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:25:37.000000 onediffx-1.0.0.dev202404200125/onediffx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:25:37.036902 onediffx-1.0.0.dev202404200125/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:25:37.032902 onediffx-1.0.0.dev202404200125/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-20 01:25:15.000000 onediffx-1.0.0.dev202404200125/tests/test_lora.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:56.809258 onediffx-1.0.0.dev202404210128/
+-rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-04-21 01:28:56.809258 onediffx-1.0.0.dev202404210128/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21242 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:56.801258 onediffx-1.0.0.dev202404210128/onediffx/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:56.801258 onediffx-1.0.0.dev202404210128/onediffx/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/compilers/diffusion_pipeline_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:56.805258 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:56.805258 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24987 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/fast_unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25684 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/unet_2d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25800 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/unet_3d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/unet_spatio_temporal_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79951 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/pipeline_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91202 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/pipeline_stable_diffusion_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/deep_cache/pipeline_stable_video_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:56.805258 onediffx-1.0.0.dev202404210128/onediffx/lora/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/lora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/lora/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/lora/state_dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/lora/text_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/lora/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13887 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/lora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:56.805258 onediffx-1.0.0.dev202404210128/onediffx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/onediffx/utils/patch_image_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:56.809258 onediffx-1.0.0.dev202404210128/onediffx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-04-21 01:28:56.000000 onediffx-1.0.0.dev202404210128/onediffx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-21 01:28:56.000000 onediffx-1.0.0.dev202404210128/onediffx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 01:28:56.000000 onediffx-1.0.0.dev202404210128/onediffx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-21 01:28:56.000000 onediffx-1.0.0.dev202404210128/onediffx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 01:28:56.000000 onediffx-1.0.0.dev202404210128/onediffx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 01:28:56.809258 onediffx-1.0.0.dev202404210128/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 01:28:56.805258 onediffx-1.0.0.dev202404210128/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-21 01:28:34.000000 onediffx-1.0.0.dev202404210128/tests/test_lora.py
```

### Comparing `onediffx-1.0.0.dev202404200125/PKG-INFO` & `onediffx-1.0.0.dev202404210128/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediffx
-Version: 1.0.0.dev202404200125
+Version: 1.0.0.dev202404210128
 Summary: onediff extensions for diffusers
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -303,22 +303,32 @@
 
 Set the LoRA layers of `adapter_name` for the unet and text-encoder(s) with related `adapter_weights`.
 
 - pipeline (`LoraLoaderMixin`): The pipeline that will set adapters.
 - adapter_names(`str` or `List[str]`): The adapter name(s) of LoRA(s) to be set for the pipeline, must appear in the `adapter_name` parameter of the `load_and_fuse_lora` function, otherwise it will be ignored.
 - adapter_weights(`float` or `List[float]`, optional): The weight(s) of adapter(s), if is None, it will be set to 1.0.
 
-#### `onediffx.lora.delete_adapters``
+#### `onediffx.lora.delete_adapters`
 
 `onediffx.lora.delete_adapters(pipeline: LoraLoaderMixin, adapter_names: Union[List[str], str])`
 
 Deletes the LoRA layers of `adapter_name` for the unet and text-encoder(s).
 
 - adapter_names (`str` or `List[str]`): The names of the adapter to delete. Can be a single string or a list of strings
 
+#### `onediffx.lora.update_graph_with_constant_folding_info`
+
+`onediffx.lora.update_graph_with_constant_folding_info(module: torch.nn.Module, info: Dict[str, flow.Tensor] = None)`
+
+Update the weights of graph after loading LoRA. (If OneDiff has enabled constant folding optimization during compilation, some parameters in the static graph may not be updated correctly after loading lora. Invoke this function manually to update the weights of the static graph correctly.)
+
+Check [text_to_image_sdxl_lora.py](./examples/text_to_image_sdxl_lora.py) for more details.
+
+> **Note**: If you are using onediffx instead of diffusers and PEFT to load LoRA, there is no need to call this function, as onediffx will handle all the necessary work.
+
 ### Example
 
 ```python
 import torch
 from diffusers import DiffusionPipeline
 from onediffx import compile_pipe
 from onediffx.lora import load_and_fuse_lora, set_and_fuse_adapters, delete_adapters
@@ -437,24 +447,14 @@
 | [1, 2, 3, 4]    | 2.02 s                         | 0.73 s                 |
 | [1, 2, 3, 4, 5] | 1.00 s                         | 0.80 s                 |
 
 ### Note
 
 1. OneDiff extensions for LoRA is currently only supported for limited PEFT APIs, and only supports diffusers of at least version 0.21.0.
 
-2. If your LoRA model only contains the weights of the Linear module, you can directly use OneDiffX without any modifications. But if your LoRA model includes the weights of the Conv module (such as LyCORIS), you need to disable constant folding optimization by above methods (which may cause a performance drop of around 4.4%), otherwise the weights of the Conv module may not be loaded into the model.
-    - Set the env var `ONEFLOW_MLIR_ENABLE_INFERENCE_OPTIMIZATION` to 0
-    - Set compiler_config.mlir_enable_inference_optimization to 0 before invoking `oneflow_compile` as the code below
-        ```
-        from onediffx import compiler_config
-        compiler_config.mlir_enable_inference_optimization = 0
-        ...
-        pipe.unet = oneflow_compile(pipe.unet)
-        ...
-        ```
 ### Optimization
 - When not using the PEFT backend, diffusers will replace the module corresponding to LoRA with the LoRACompatible module, incurring additional parameter initialization time overhead. In OneDiffX, the LoRA parameters are directly fused into the model, bypassing the step of replacing the module, thereby reducing the time overhead.
 
 - When using the PEFT backend, PEFT will also replace the module corresponding to LoRA with the corresponding BaseTunerLayer. Similar to diffusers, this increases the time overhead. OneDiffX also bypasses this step by directly operating on the original model.
 
 - While traversing the submodules of the model, we observed that the `getattr` time overhead of OneDiff's `DeployableModule` is high. Because the parameters of DeployableModule share the same address as the PyTorch module it wraps, we choose to traverse `DeployableModule._torch_module`, greatly improving traversal efficiency.
 
@@ -477,15 +477,15 @@
 # After loading the new state dict into the `compiled_unet._torch_module`, the weights of the compiled_unet are updated too
 new_base.unet = compiled_unet
 # This step doesn't need additional time to compile the UNet again because
 # new_base.unet is already compiled
 new_base(prompt)
 ```
 
-> Note: Please make sure that your PyTorch version is **at least 2.1.0**, and set the environment variable `ONEFLOW_MLIR_ENABLE_INFERENCE_OPTIMIZATION` to **0**. And the feature is not supported for quantized model.
+> Note: The feature is not supported for quantized model.
 
 
 ## Quantization
 
 **Note**: Quantization feature is only supported by **OneDiff Enterprise**.
 
 OneDiff Enterprise offers a quantization method that reduces memory usage, increases speed, and maintains quality without any loss.
```

### Comparing `onediffx-1.0.0.dev202404200125/README.md` & `onediffx-1.0.0.dev202404210128/onediffx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: onediffx
+Version: 1.0.0.dev202404210128
+Summary: onediff extensions for diffusers
+Home-page: https://github.com/siliconflow/onediff
+Author: OneDiff contributors
+Author-email: caishenghang@oneflow.org
+License: Apache
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+Requires-Dist: transformers>=4.27.1
+Requires-Dist: diffusers<=0.27.0,>=0.19.3
+Requires-Dist: accelerate
+Requires-Dist: torch
+Requires-Dist: onefx
+Requires-Dist: omegaconf
+
 # OneDiffX (for HF diffusers)
 
 OneDiffX is a OneDiff Extension for HF diffusers. It provides some acceleration utilities, such as DeepCache.
 
 - [Install and Setup](#install-and-setup)
 - [Compile, save and load pipeline](#compile-save-and-load-pipeline)
 - Acceleration for state-of-the-art Models
@@ -275,22 +303,32 @@
 
 Set the LoRA layers of `adapter_name` for the unet and text-encoder(s) with related `adapter_weights`.
 
 - pipeline (`LoraLoaderMixin`): The pipeline that will set adapters.
 - adapter_names(`str` or `List[str]`): The adapter name(s) of LoRA(s) to be set for the pipeline, must appear in the `adapter_name` parameter of the `load_and_fuse_lora` function, otherwise it will be ignored.
 - adapter_weights(`float` or `List[float]`, optional): The weight(s) of adapter(s), if is None, it will be set to 1.0.
 
-#### `onediffx.lora.delete_adapters``
+#### `onediffx.lora.delete_adapters`
 
 `onediffx.lora.delete_adapters(pipeline: LoraLoaderMixin, adapter_names: Union[List[str], str])`
 
 Deletes the LoRA layers of `adapter_name` for the unet and text-encoder(s).
 
 - adapter_names (`str` or `List[str]`): The names of the adapter to delete. Can be a single string or a list of strings
 
+#### `onediffx.lora.update_graph_with_constant_folding_info`
+
+`onediffx.lora.update_graph_with_constant_folding_info(module: torch.nn.Module, info: Dict[str, flow.Tensor] = None)`
+
+Update the weights of graph after loading LoRA. (If OneDiff has enabled constant folding optimization during compilation, some parameters in the static graph may not be updated correctly after loading lora. Invoke this function manually to update the weights of the static graph correctly.)
+
+Check [text_to_image_sdxl_lora.py](./examples/text_to_image_sdxl_lora.py) for more details.
+
+> **Note**: If you are using onediffx instead of diffusers and PEFT to load LoRA, there is no need to call this function, as onediffx will handle all the necessary work.
+
 ### Example
 
 ```python
 import torch
 from diffusers import DiffusionPipeline
 from onediffx import compile_pipe
 from onediffx.lora import load_and_fuse_lora, set_and_fuse_adapters, delete_adapters
@@ -409,24 +447,14 @@
 | [1, 2, 3, 4]    | 2.02 s                         | 0.73 s                 |
 | [1, 2, 3, 4, 5] | 1.00 s                         | 0.80 s                 |
 
 ### Note
 
 1. OneDiff extensions for LoRA is currently only supported for limited PEFT APIs, and only supports diffusers of at least version 0.21.0.
 
-2. If your LoRA model only contains the weights of the Linear module, you can directly use OneDiffX without any modifications. But if your LoRA model includes the weights of the Conv module (such as LyCORIS), you need to disable constant folding optimization by above methods (which may cause a performance drop of around 4.4%), otherwise the weights of the Conv module may not be loaded into the model.
-    - Set the env var `ONEFLOW_MLIR_ENABLE_INFERENCE_OPTIMIZATION` to 0
-    - Set compiler_config.mlir_enable_inference_optimization to 0 before invoking `oneflow_compile` as the code below
-        ```
-        from onediffx import compiler_config
-        compiler_config.mlir_enable_inference_optimization = 0
-        ...
-        pipe.unet = oneflow_compile(pipe.unet)
-        ...
-        ```
 ### Optimization
 - When not using the PEFT backend, diffusers will replace the module corresponding to LoRA with the LoRACompatible module, incurring additional parameter initialization time overhead. In OneDiffX, the LoRA parameters are directly fused into the model, bypassing the step of replacing the module, thereby reducing the time overhead.
 
 - When using the PEFT backend, PEFT will also replace the module corresponding to LoRA with the corresponding BaseTunerLayer. Similar to diffusers, this increases the time overhead. OneDiffX also bypasses this step by directly operating on the original model.
 
 - While traversing the submodules of the model, we observed that the `getattr` time overhead of OneDiff's `DeployableModule` is high. Because the parameters of DeployableModule share the same address as the PyTorch module it wraps, we choose to traverse `DeployableModule._torch_module`, greatly improving traversal efficiency.
 
@@ -449,15 +477,15 @@
 # After loading the new state dict into the `compiled_unet._torch_module`, the weights of the compiled_unet are updated too
 new_base.unet = compiled_unet
 # This step doesn't need additional time to compile the UNet again because
 # new_base.unet is already compiled
 new_base(prompt)
 ```
 
-> Note: Please make sure that your PyTorch version is **at least 2.1.0**, and set the environment variable `ONEFLOW_MLIR_ENABLE_INFERENCE_OPTIMIZATION` to **0**. And the feature is not supported for quantized model.
+> Note: The feature is not supported for quantized model.
 
 
 ## Quantization
 
 **Note**: Quantization feature is only supported by **OneDiff Enterprise**.
 
 OneDiff Enterprise offers a quantization method that reduces memory usage, increases speed, and maintains quality without any loss.
```

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/compilers/diffusion_pipeline_compiler.py` & `onediffx-1.0.0.dev202404210128/onediffx/compilers/diffusion_pipeline_compiler.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/__init__.py` & `onediffx-1.0.0.dev202404210128/onediffx/deep_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/fast_unet_2d_condition.py` & `onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/fast_unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py` & `onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/fast_unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/pipeline_utils.py` & `onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_2d_blocks.py` & `onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/unet_2d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_2d_condition.py` & `onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/unet_2d_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_3d_blocks.py` & `onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/unet_3d_blocks.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/models/unet_spatio_temporal_condition.py` & `onediffx-1.0.0.dev202404210128/onediffx/deep_cache/models/unet_spatio_temporal_condition.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_diffusion.py` & `onediffx-1.0.0.dev202404210128/onediffx/deep_cache/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_diffusion_xl.py` & `onediffx-1.0.0.dev202404210128/onediffx/deep_cache/pipeline_stable_diffusion_xl.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/deep_cache/pipeline_stable_video_diffusion.py` & `onediffx-1.0.0.dev202404210128/onediffx/deep_cache/pipeline_stable_video_diffusion.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/lora/lora.py` & `onediffx-1.0.0.dev202404210128/onediffx/lora/lora.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/lora/state_dict_utils.py` & `onediffx-1.0.0.dev202404210128/onediffx/lora/state_dict_utils.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/lora/text_encoder.py` & `onediffx-1.0.0.dev202404210128/onediffx/lora/text_encoder.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/lora/unet.py` & `onediffx-1.0.0.dev202404210128/onediffx/lora/unet.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/lora/utils.py` & `onediffx-1.0.0.dev202404210128/onediffx/lora/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     from diffusers.utils.import_utils import is_peft_available
 
     if is_peft_available():
         import peft
 else:
     is_peft_available = lambda: False
 
+from onediff.infer_compiler.utils.param_utils import update_graph_related_tensor
+
 if version.parse(diffusers.__version__) <= version.parse("0.20.0"):
     from diffusers.loaders import PatchedLoraProjection
 else:
     from diffusers.models.lora import PatchedLoraProjection
 from onediff.infer_compiler.oneflow.dual_module import DualModule
 
 if version.parse(diffusers.__version__) <= version.parse("0.20.0"):
@@ -132,14 +134,15 @@
                 self, w_up, w_down, weight / self.scaling[adapter]
             )
         self.active_adapter_names[adapter] = weight
 
     if delta_weight is not None:
         fused_weight = self.weight.data.float() + delta_weight
         self.weight.data.copy_(fused_weight.to(device=device, dtype=dtype))
+        update_graph_related_tensor(self)
 
 
 def _delete_adapter(self, adapter_names):
     if not isinstance(self, (torch.nn.Linear, torch.nn.Conv2d, PatchedLoraProjection)):
         raise TypeError(
             f"[OneDiffX _delete_adapter] Expect type Linear or Conv2d, got {type(self)}"
         )
@@ -220,14 +223,15 @@
     self.adapter_names.add(adapter_name)
     self.active_adapter_names[adapter_name] = 1.0
 
     if fuse:
         lora_weight = get_delta_weight(self, w_up, w_down, 1.0)
         fused_weight = self.weight.data.float() + lora_weight
         self.weight.data.copy_(fused_weight.to(device=device, dtype=dtype))
+        update_graph_related_tensor(self)
 
 
 def _unfuse_lora(
     self: Union[torch.nn.Linear, PatchedLoraProjection, torch.nn.Conv2d],
     adapter_names: Union[str, List[str]] = None,
 ):
     assert isinstance(self, (torch.nn.Linear, PatchedLoraProjection, torch.nn.Conv2d))
@@ -259,14 +263,15 @@
             delta_weight += get_delta_weight(self, w_up, w_down, weight).to(
                 dtype=dtype, device=device
             )
         self.active_adapter_names.pop(name)
 
     if delta_weight is not None:
         self.weight.data -= delta_weight
+        update_graph_related_tensor(self)
 
 
 # the code is referenced from https://github.com/huggingface/diffusers/blob/ce9825b56bd8a6849e68b9590022e935400659e6/src/diffusers/loaders/lora_conversion_utils.py#L24
 @classmethod
 def _maybe_map_sgm_blocks_to_diffusers(
     cls, state_dict, unet_config, delimiter="_", block_slice_pos=5
 ):
```

### Comparing `onediffx-1.0.0.dev202404200125/onediffx/utils/patch_image_processor.py` & `onediffx-1.0.0.dev202404210128/onediffx/utils/patch_image_processor.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/onediffx.egg-info/PKG-INFO` & `onediffx-1.0.0.dev202404210128/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: onediffx
-Version: 1.0.0.dev202404200125
-Summary: onediff extensions for diffusers
-Home-page: https://github.com/siliconflow/onediff
-Author: OneDiff contributors
-Author-email: caishenghang@oneflow.org
-License: Apache
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Requires-Dist: transformers>=4.27.1
-Requires-Dist: diffusers<=0.27.0,>=0.19.3
-Requires-Dist: accelerate
-Requires-Dist: torch
-Requires-Dist: onefx
-Requires-Dist: omegaconf
-
 # OneDiffX (for HF diffusers)
 
 OneDiffX is a OneDiff Extension for HF diffusers. It provides some acceleration utilities, such as DeepCache.
 
 - [Install and Setup](#install-and-setup)
 - [Compile, save and load pipeline](#compile-save-and-load-pipeline)
 - Acceleration for state-of-the-art Models
@@ -303,22 +275,32 @@
 
 Set the LoRA layers of `adapter_name` for the unet and text-encoder(s) with related `adapter_weights`.
 
 - pipeline (`LoraLoaderMixin`): The pipeline that will set adapters.
 - adapter_names(`str` or `List[str]`): The adapter name(s) of LoRA(s) to be set for the pipeline, must appear in the `adapter_name` parameter of the `load_and_fuse_lora` function, otherwise it will be ignored.
 - adapter_weights(`float` or `List[float]`, optional): The weight(s) of adapter(s), if is None, it will be set to 1.0.
 
-#### `onediffx.lora.delete_adapters``
+#### `onediffx.lora.delete_adapters`
 
 `onediffx.lora.delete_adapters(pipeline: LoraLoaderMixin, adapter_names: Union[List[str], str])`
 
 Deletes the LoRA layers of `adapter_name` for the unet and text-encoder(s).
 
 - adapter_names (`str` or `List[str]`): The names of the adapter to delete. Can be a single string or a list of strings
 
+#### `onediffx.lora.update_graph_with_constant_folding_info`
+
+`onediffx.lora.update_graph_with_constant_folding_info(module: torch.nn.Module, info: Dict[str, flow.Tensor] = None)`
+
+Update the weights of graph after loading LoRA. (If OneDiff has enabled constant folding optimization during compilation, some parameters in the static graph may not be updated correctly after loading lora. Invoke this function manually to update the weights of the static graph correctly.)
+
+Check [text_to_image_sdxl_lora.py](./examples/text_to_image_sdxl_lora.py) for more details.
+
+> **Note**: If you are using onediffx instead of diffusers and PEFT to load LoRA, there is no need to call this function, as onediffx will handle all the necessary work.
+
 ### Example
 
 ```python
 import torch
 from diffusers import DiffusionPipeline
 from onediffx import compile_pipe
 from onediffx.lora import load_and_fuse_lora, set_and_fuse_adapters, delete_adapters
@@ -437,24 +419,14 @@
 | [1, 2, 3, 4]    | 2.02 s                         | 0.73 s                 |
 | [1, 2, 3, 4, 5] | 1.00 s                         | 0.80 s                 |
 
 ### Note
 
 1. OneDiff extensions for LoRA is currently only supported for limited PEFT APIs, and only supports diffusers of at least version 0.21.0.
 
-2. If your LoRA model only contains the weights of the Linear module, you can directly use OneDiffX without any modifications. But if your LoRA model includes the weights of the Conv module (such as LyCORIS), you need to disable constant folding optimization by above methods (which may cause a performance drop of around 4.4%), otherwise the weights of the Conv module may not be loaded into the model.
-    - Set the env var `ONEFLOW_MLIR_ENABLE_INFERENCE_OPTIMIZATION` to 0
-    - Set compiler_config.mlir_enable_inference_optimization to 0 before invoking `oneflow_compile` as the code below
-        ```
-        from onediffx import compiler_config
-        compiler_config.mlir_enable_inference_optimization = 0
-        ...
-        pipe.unet = oneflow_compile(pipe.unet)
-        ...
-        ```
 ### Optimization
 - When not using the PEFT backend, diffusers will replace the module corresponding to LoRA with the LoRACompatible module, incurring additional parameter initialization time overhead. In OneDiffX, the LoRA parameters are directly fused into the model, bypassing the step of replacing the module, thereby reducing the time overhead.
 
 - When using the PEFT backend, PEFT will also replace the module corresponding to LoRA with the corresponding BaseTunerLayer. Similar to diffusers, this increases the time overhead. OneDiffX also bypasses this step by directly operating on the original model.
 
 - While traversing the submodules of the model, we observed that the `getattr` time overhead of OneDiff's `DeployableModule` is high. Because the parameters of DeployableModule share the same address as the PyTorch module it wraps, we choose to traverse `DeployableModule._torch_module`, greatly improving traversal efficiency.
 
@@ -477,15 +449,15 @@
 # After loading the new state dict into the `compiled_unet._torch_module`, the weights of the compiled_unet are updated too
 new_base.unet = compiled_unet
 # This step doesn't need additional time to compile the UNet again because
 # new_base.unet is already compiled
 new_base(prompt)
 ```
 
-> Note: Please make sure that your PyTorch version is **at least 2.1.0**, and set the environment variable `ONEFLOW_MLIR_ENABLE_INFERENCE_OPTIMIZATION` to **0**. And the feature is not supported for quantized model.
+> Note: The feature is not supported for quantized model.
 
 
 ## Quantization
 
 **Note**: Quantization feature is only supported by **OneDiff Enterprise**.
 
 OneDiff Enterprise offers a quantization method that reduces memory usage, increases speed, and maintains quality without any loss.
```

### Comparing `onediffx-1.0.0.dev202404200125/onediffx.egg-info/SOURCES.txt` & `onediffx-1.0.0.dev202404210128/onediffx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/setup.py` & `onediffx-1.0.0.dev202404210128/setup.py`

 * *Files identical despite different names*

### Comparing `onediffx-1.0.0.dev202404200125/tests/test_lora.py` & `onediffx-1.0.0.dev202404210128/tests/test_lora.py`

 * *Files identical despite different names*

