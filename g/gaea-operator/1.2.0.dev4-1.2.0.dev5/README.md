# Comparing `tmp/gaea_operator-1.2.0.dev4-py3-none-any.whl.zip` & `tmp/gaea_operator-1.2.0.dev5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 147240 bytes, number of entries: 113
+Zip file size: 150300 bytes, number of entries: 113
 -rw-r--r--  2.0 unx      131 b- defN 24-Apr-19 06:41 gaea_operator/__init__.py
 -rw-r--r--  2.0 unx      131 b- defN 24-Apr-19 06:41 gaea_operator/components/__init__.py
 -rw-r--r--  2.0 unx      131 b- defN 24-Apr-19 06:41 gaea_operator/components/eval/__init__.py
 -rw-r--r--  2.0 unx     4169 b- defN 24-Apr-19 06:41 gaea_operator/components/eval/ocrnet.py
 -rw-r--r--  2.0 unx     4268 b- defN 24-Apr-19 06:41 gaea_operator/components/eval/ppyoloe_plus.py
 -rw-r--r--  2.0 unx     4153 b- defN 24-Apr-19 06:41 gaea_operator/components/eval/resnet.py
 -rw-r--r--  2.0 unx     3102 b- defN 24-Apr-19 06:41 gaea_operator/components/inference/__init__.py
@@ -34,19 +34,21 @@
 -rw-r--r--  2.0 unx     4058 b- defN 24-Apr-19 06:41 gaea_operator/config/ppyoloe_plus/ppyoloeplus_config.py
 -rw-r--r--  2.0 unx      130 b- defN 24-Apr-19 06:41 gaea_operator/config/ppyoloe_plus/template/__init__.py
 -rw-r--r--  2.0 unx    12621 b- defN 24-Apr-19 06:41 gaea_operator/config/ppyoloe_plus/template/modify_train_parameter.py
 -rw-r--r--  2.0 unx     4583 b- defN 24-Apr-19 06:41 gaea_operator/config/ppyoloe_plus/template/parameter.yaml
 -rw-r--r--  2.0 unx     4666 b- defN 24-Apr-19 06:41 gaea_operator/config/ppyoloe_plus/template/parameter_c.yaml
 -rw-r--r--  2.0 unx      130 b- defN 24-Apr-19 06:41 gaea_operator/config/resnet/__init__.py
 -rw-r--r--  2.0 unx     4283 b- defN 24-Apr-19 06:41 gaea_operator/config/resnet/resnet_config.py
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-19 06:41 gaea_operator/config/resnet/template/__init__.py
+-rw-r--r--  2.0 unx    11498 b- defN 24-Apr-19 06:41 gaea_operator/config/resnet/template/modify_train_parameter.py
 -rw-r--r--  2.0 unx     2315 b- defN 24-Apr-19 06:41 gaea_operator/config/resnet/template/parameter.yaml
 -rw-r--r--  2.0 unx      370 b- defN 24-Apr-19 06:41 gaea_operator/dataset/__init__.py
 -rw-r--r--  2.0 unx     4259 b- defN 24-Apr-19 06:41 gaea_operator/dataset/cityscape_dataset.py
--rw-r--r--  2.0 unx     6515 b- defN 24-Apr-19 06:41 gaea_operator/dataset/coco_dataset.py
--rw-r--r--  2.0 unx     7389 b- defN 24-Apr-19 06:41 gaea_operator/dataset/dataset.py
+-rw-r--r--  2.0 unx     6508 b- defN 24-Apr-19 07:02 gaea_operator/dataset/coco_dataset.py
+-rw-r--r--  2.0 unx     7314 b- defN 24-Apr-21 12:43 gaea_operator/dataset/dataset.py
 -rw-r--r--  2.0 unx     4297 b- defN 24-Apr-19 06:41 gaea_operator/dataset/imagenet_dataset.py
 -rw-r--r--  2.0 unx      584 b- defN 24-Apr-19 06:41 gaea_operator/metric/__init__.py
 -rw-r--r--  2.0 unx     5740 b- defN 24-Apr-19 06:41 gaea_operator/metric/metric.py
 -rw-r--r--  2.0 unx      433 b- defN 24-Apr-19 06:41 gaea_operator/metric/analysis/__init__.py
 -rw-r--r--  2.0 unx    18968 b- defN 24-Apr-19 06:41 gaea_operator/metric/analysis/eval_metric_analysis.py
 -rw-r--r--  2.0 unx     7907 b- defN 24-Apr-19 06:41 gaea_operator/metric/analysis/inference_metric_analysis.py
 -rw-r--r--  2.0 unx    11706 b- defN 24-Apr-19 06:41 gaea_operator/metric/analysis/label_statistics_metric_analysis.py
@@ -71,45 +73,43 @@
 -rw-r--r--  2.0 unx     4874 b- defN 24-Apr-19 06:41 gaea_operator/metric/types/metric.py
 -rw-r--r--  2.0 unx     2362 b- defN 24-Apr-19 06:41 gaea_operator/metric/types/object_detection_metric.py
 -rw-r--r--  2.0 unx     1244 b- defN 24-Apr-19 06:41 gaea_operator/metric/types/semantic_segmentation_metric.py
 -rw-r--r--  2.0 unx      214 b- defN 24-Apr-19 06:41 gaea_operator/model/__init__.py
 -rw-r--r--  2.0 unx     1436 b- defN 24-Apr-19 06:41 gaea_operator/model/model.py
 -rw-r--r--  2.0 unx      131 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/__init__.py
 -rw-r--r--  2.0 unx      131 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/ocrnet_pipeline/__init__.py
--rw-r--r--  2.0 unx    12000 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/ocrnet_pipeline/ocrnet_pipeline.py
+-rw-r--r--  2.0 unx    12009 b- defN 24-Apr-19 14:15 gaea_operator/pipelines/ocrnet_pipeline/ocrnet_pipeline.py
 -rw-r--r--  2.0 unx     1051 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/ocrnet_pipeline/train_parameter.yaml
 -rw-r--r--  2.0 unx     1119 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/ocrnet_pipeline/transform_parameter.yaml
 -rw-r--r--  2.0 unx      131 b- defN 24-Apr-18 03:50 gaea_operator/pipelines/ppyoloe_plus_pipeline/__init__.py
--rw-r--r--  2.0 unx    12387 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/ppyoloe_plus_pipeline/ppyoloe_plus_pipeline.py
+-rw-r--r--  2.0 unx    12396 b- defN 24-Apr-19 14:15 gaea_operator/pipelines/ppyoloe_plus_pipeline/ppyoloe_plus_pipeline.py
 -rw-r--r--  2.0 unx     1326 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/ppyoloe_plus_pipeline/train_parameter.yaml
 -rw-r--r--  2.0 unx     1815 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/ppyoloe_plus_pipeline/transform_parameter.yaml
 -rw-r--r--  2.0 unx      131 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/resnet_pipeline/__init__.py
--rw-r--r--  2.0 unx    12178 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/resnet_pipeline/resnet_pipeline.py
+-rw-r--r--  2.0 unx    12187 b- defN 24-Apr-19 14:15 gaea_operator/pipelines/resnet_pipeline/resnet_pipeline.py
 -rw-r--r--  2.0 unx     1271 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/resnet_pipeline/train_parameter.yaml
 -rw-r--r--  2.0 unx     1121 b- defN 24-Apr-19 06:41 gaea_operator/pipelines/resnet_pipeline/transform_parameter.yaml
 -rw-r--r--  2.0 unx      181 b- defN 24-Apr-19 06:41 gaea_operator/trainer/__init__.py
 -rw-r--r--  2.0 unx     5406 b- defN 24-Apr-19 06:41 gaea_operator/trainer/trainer.py
 -rw-r--r--  2.0 unx      187 b- defN 24-Apr-19 06:41 gaea_operator/transform/__init__.py
 -rw-r--r--  2.0 unx     3307 b- defN 24-Apr-19 06:41 gaea_operator/transform/cvt_copy_model.py
 -rw-r--r--  2.0 unx      776 b- defN 24-Apr-19 06:41 gaea_operator/transform/transform.py
--rw-r--r--  2.0 unx     1910 b- defN 24-Apr-19 06:41 gaea_operator/utils/__init__.py
--rw-r--r--  2.0 unx     5554 b- defN 24-Apr-19 06:41 gaea_operator/utils/accelerator.py
+-rw-r--r--  2.0 unx     1788 b- defN 24-Apr-19 13:52 gaea_operator/utils/__init__.py
+-rw-r--r--  2.0 unx     5557 b- defN 24-Apr-19 14:15 gaea_operator/utils/accelerator.py
 -rw-r--r--  2.0 unx     2887 b- defN 24-Apr-19 06:41 gaea_operator/utils/compress.py
 -rw-r--r--  2.0 unx      426 b- defN 24-Apr-19 06:41 gaea_operator/utils/consts.py
 -rw-r--r--  2.0 unx     1948 b- defN 24-Apr-19 06:41 gaea_operator/utils/file.py
 -rw-r--r--  2.0 unx     1533 b- defN 24-Apr-19 06:41 gaea_operator/utils/import_module.py
 -rw-r--r--  2.0 unx     6613 b- defN 24-Apr-19 06:41 gaea_operator/utils/model_template.py
--rw-r--r--  2.0 unx      563 b- defN 24-Apr-19 06:41 gaea_operator/utils/polygon.py
 -rw-r--r--  2.0 unx     1680 b- defN 24-Apr-19 06:41 gaea_operator/utils/registry.py
--rw-r--r--  2.0 unx      613 b- defN 24-Apr-19 06:41 gaea_operator/utils/rle.py
 -rw-r--r--  2.0 unx     1000 b- defN 24-Apr-19 06:41 gaea_operator/utils/tensor.py
 -rw-r--r--  2.0 unx      301 b- defN 24-Apr-19 06:41 gaea_operator/utils/time.py
--rw-r--r--  2.0 unx     4864 b- defN 24-Apr-19 06:41 gaea_operator-1.2.0.dev4.data/data/yaml/object_detection.yaml
--rw-r--r--  2.0 unx     4583 b- defN 24-Apr-19 06:41 gaea_operator-1.2.0.dev4.data/data/yaml/parameter.yaml
--rw-r--r--  2.0 unx     4666 b- defN 24-Apr-19 06:41 gaea_operator-1.2.0.dev4.data/data/yaml/parameter_c.yaml
--rw-r--r--  2.0 unx     1051 b- defN 24-Apr-19 06:41 gaea_operator-1.2.0.dev4.data/data/yaml/train_parameter.yaml
--rw-r--r--  2.0 unx     1119 b- defN 24-Apr-19 06:41 gaea_operator-1.2.0.dev4.data/data/yaml/transform_parameter.yaml
--rw-r--r--  2.0 unx     2173 b- defN 24-Apr-19 06:55 gaea_operator-1.2.0.dev4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 06:55 gaea_operator-1.2.0.dev4.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Apr-19 06:55 gaea_operator-1.2.0.dev4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    11528 b- defN 24-Apr-19 06:55 gaea_operator-1.2.0.dev4.dist-info/RECORD
-113 files, 471402 bytes uncompressed, 128304 bytes compressed:  72.8%
+-rw-r--r--  2.0 unx     4864 b- defN 24-Apr-19 06:41 gaea_operator-1.2.0.dev5.data/data/yaml/object_detection.yaml
+-rw-r--r--  2.0 unx     4583 b- defN 24-Apr-19 06:41 gaea_operator-1.2.0.dev5.data/data/yaml/parameter.yaml
+-rw-r--r--  2.0 unx     4666 b- defN 24-Apr-19 06:41 gaea_operator-1.2.0.dev5.data/data/yaml/parameter_c.yaml
+-rw-r--r--  2.0 unx     1051 b- defN 24-Apr-19 06:41 gaea_operator-1.2.0.dev5.data/data/yaml/train_parameter.yaml
+-rw-r--r--  2.0 unx     1119 b- defN 24-Apr-19 06:41 gaea_operator-1.2.0.dev5.data/data/yaml/transform_parameter.yaml
+-rw-r--r--  2.0 unx     2173 b- defN 24-Apr-22 02:55 gaea_operator-1.2.0.dev5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 02:55 gaea_operator-1.2.0.dev5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-22 02:55 gaea_operator-1.2.0.dev5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    11584 b- defN 24-Apr-22 02:55 gaea_operator-1.2.0.dev5.dist-info/RECORD
+113 files, 481736 bytes uncompressed, 131256 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -111,14 +111,20 @@
 
 Filename: gaea_operator/config/resnet/__init__.py
 Comment: 
 
 Filename: gaea_operator/config/resnet/resnet_config.py
 Comment: 
 
+Filename: gaea_operator/config/resnet/template/__init__.py
+Comment: 
+
+Filename: gaea_operator/config/resnet/template/modify_train_parameter.py
+Comment: 
+
 Filename: gaea_operator/config/resnet/template/parameter.yaml
 Comment: 
 
 Filename: gaea_operator/dataset/__init__.py
 Comment: 
 
 Filename: gaea_operator/dataset/cityscape_dataset.py
@@ -291,50 +297,44 @@
 
 Filename: gaea_operator/utils/import_module.py
 Comment: 
 
 Filename: gaea_operator/utils/model_template.py
 Comment: 
 
-Filename: gaea_operator/utils/polygon.py
-Comment: 
-
 Filename: gaea_operator/utils/registry.py
 Comment: 
 
-Filename: gaea_operator/utils/rle.py
-Comment: 
-
 Filename: gaea_operator/utils/tensor.py
 Comment: 
 
 Filename: gaea_operator/utils/time.py
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev4.data/data/yaml/object_detection.yaml
+Filename: gaea_operator-1.2.0.dev5.data/data/yaml/object_detection.yaml
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev4.data/data/yaml/parameter.yaml
+Filename: gaea_operator-1.2.0.dev5.data/data/yaml/parameter.yaml
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev4.data/data/yaml/parameter_c.yaml
+Filename: gaea_operator-1.2.0.dev5.data/data/yaml/parameter_c.yaml
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev4.data/data/yaml/train_parameter.yaml
+Filename: gaea_operator-1.2.0.dev5.data/data/yaml/train_parameter.yaml
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev4.data/data/yaml/transform_parameter.yaml
+Filename: gaea_operator-1.2.0.dev5.data/data/yaml/transform_parameter.yaml
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev4.dist-info/METADATA
+Filename: gaea_operator-1.2.0.dev5.dist-info/METADATA
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev4.dist-info/WHEEL
+Filename: gaea_operator-1.2.0.dev5.dist-info/WHEEL
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev4.dist-info/top_level.txt
+Filename: gaea_operator-1.2.0.dev5.dist-info/top_level.txt
 Comment: 
 
-Filename: gaea_operator-1.2.0.dev4.dist-info/RECORD
+Filename: gaea_operator-1.2.0.dev5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gaea_operator/dataset/coco_dataset.py

```diff
@@ -29,38 +29,38 @@
         self.image_prefix_path = "images"
 
     @classmethod
     def coco_annotation_from_vistudio_v1(cls, annotations: List[Dict]):
         """
         Convert the annotation from Vistudio v1 to Coco format.
         """
-        ann_id = 1
+        anno_id = 1
         new_annotations = []
         for item in annotations:
             im_id = item["image_id"]
             if item.get("annotations") is None:
-                anno = {"id": ann_id, "image_id": im_id}
+                anno = {"id": anno_id, "image_id": im_id}
                 new_annotations.append(anno)
                 continue
             for anno in item["annotations"]:
                 anno["image_id"] = im_id
                 anno['ignore'] = anno['ignore'] if 'ignore' in anno else 0
                 anno['iscrowd'] = "iscrowd" in anno and anno["iscrowd"]
                 for idx in range(len(anno["labels"])):
-                    anno_copy = copy.deepcopy(anno)
-                    anno_copy["id"] = ann_id
-                    if isinstance(anno_copy["labels"][idx]["id"], str):
-                        anno_copy["labels"][idx]["id"] = int(anno_copy["labels"][idx]["id"])
-                    if math.isnan(anno_copy["labels"][idx]["id"]):
+                    new_anno = copy.deepcopy(anno)
+                    new_anno["id"] = anno_id
+                    if isinstance(new_anno["labels"][idx]["id"], str):
+                        new_anno["labels"][idx]["id"] = int(new_anno["labels"][idx]["id"])
+                    if math.isnan(new_anno["labels"][idx]["id"]):
                         continue
-                    anno_copy['category_id'] = anno_copy["labels"][idx]["id"]
-                    anno_copy['score'] = anno["labels"][idx].get("confidence", 1)
-                    anno_copy['confidence'] = anno["labels"][idx].get("confidence", 1)
-                    new_annotations.append(anno_copy)
-                    ann_id += 1
+                    new_anno['category_id'] = new_anno["labels"][idx]["id"]
+                    new_anno['score'] = anno["labels"][idx].get("confidence", 1)
+                    new_anno['confidence'] = anno["labels"][idx].get("confidence", 1)
+                    new_annotations.append(new_anno)
+                    anno_id += 1
 
         return new_annotations
 
     def _get_annotation(self, paths: List, base_uri: str, usage: Union[str, Tuple], work_dir: str) -> List:
         annotation_file_list = []
         for idx, path in enumerate(paths):
             path = os.path.join(work_dir, path)
```

## gaea_operator/dataset/dataset.py

```diff
@@ -5,21 +5,22 @@
 # @Author  : yanxiaodong
 # @File    : dataset_concat.py
 """
 import json
 import os
 from abc import ABCMeta, abstractmethod
 from typing import Any, List, Union, Tuple, Dict
+import pycocotools.mask as mask_utils
 import math
 import numpy as np
 
 import bcelogger
 from windmillclient.client.windmill_client import WindmillClient
 
-from gaea_operator.utils import find_upper_level_folder, write_file, rle_to_mask, polygon_to_mask
+from gaea_operator.utils import find_upper_level_folder, write_file
 
 
 class Dataset(metaclass=ABCMeta):
     """
     A dataset for data processing.
     """
     decompress_output_uri = "/root/dataset"
@@ -124,23 +125,22 @@
                         anno["labels"][idx]["id"] = int(anno["labels"][idx]["id"])
                     if math.isnan(anno["labels"][idx]["id"]):
                         continue
                     # 如果标注标签id不在label,则跳过（修改了标签但是标注没有同步修改）
                     if anno["labels"][idx]["id"] not in label_id2index:
                         continue
                     if "rle" in anno and len(anno["rle"]) > 0:
-                        rle = anno["rle"]
-                        mask = rle_to_mask(rle, pixel_index=label_id2index[anno["labels"][idx]["id"]])
-                        index = mask == label_id2index[anno["labels"][idx]["id"]]
-                        label_raw[index] = mask[index]
+                        rle = mask_utils.frPyObjects(anno["rle"], height, width)
+                        mask = mask_utils.decode(rle).T
                     else:
                         polygon = anno["segmentation"]
-                        polygon_to_mask(polygon=polygon,
-                                        mask=label_raw,
-                                        pixel_index=label_id2index[anno["labels"][idx]["id"]])
+                        rle = mask_utils.frPyObjects([polygon], height, width)
+                        mask = mask_utils.decode(mask_utils.merge(rle))
+                    index = mask == 1
+                    label_raw[index] = label_id2index[anno["labels"][idx]["id"]]
 
             new_annotations.append(new_anno)
 
         return new_annotations
 
     @abstractmethod
     def _get_annotation(self, paths: List, base_uri: List, usage: str, work_dir: str) -> List:
```

## gaea_operator/pipelines/ocrnet_pipeline/ocrnet_pipeline.py

```diff
@@ -79,15 +79,15 @@
                  "MODEL_NAME": "{{model_name}}",
                  "MODEL_DISPLAY_NAME": "{{model_display_name}}",
                  "ADVANCED_PARAMETERS": "{{advanced_parameters}}",
                  "PF_EXTRA_WORK_DIR": extra_fs_mount_path}
     train_env.update(base_env)
     train_params.update(base_params)
     train = ContainerStep(name="train",
-                          docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0.7",
+                          docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0-dev1",
                           parameters=train_params,
                           env=train_env,
                           extra_fs=[ExtraFS(name=extra_fs_name, mount_path=extra_fs_mount_path)],
                           outputs={"output_model_uri": Artifact(), "output_uri": Artifact()},
                           command=f'package_path=$(python3 -c "import site; print(site.getsitepackages()[0])") && '
                                   f'python3 -m gaea_operator.components.train.ocrnet '
                                   f'--output-model-uri={{{{output_model_uri}}}} '
@@ -99,15 +99,15 @@
                                   f'--save_dir={{{{output_model_uri}}}}')
 
     eval_params = {"dataset_name": eval_dataset_name}
     eval_env = {"DATASET_NAME": "{{dataset_name}}"}
     eval_env.update(base_env)
     eval_params.update(base_params)
     eval = ContainerStep(name="eval",
-                         docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0.7",
+                         docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0-dev1",
                          parameters=eval_params,
                          env=eval_env,
                          inputs={"input_model_uri": train.outputs["output_model_uri"]},
                          outputs={"output_uri": Artifact(), "output_dataset_uri": Artifact()},
                          command=f'package_path=$(python3 -c "import site; print(site.getsitepackages()[0])") && '
                                  f'python3 -m gaea_operator.components.eval.ocrnet '
                                  f'--input-model-uri={{{{input_model_uri}}}} '
@@ -136,15 +136,15 @@
     transform_env = {"TRANSFORM_MODEL_NAME": "{{transform_model_name}}",
                      "TRANSFORM_MODEL_DISPLAY_NAME": "{{transform_model_display_name}}",
                      "ACCELERATOR": "{{accelerator}}",
                      "ADVANCED_PARAMETERS": "{{advanced_parameters1}}"}
     transform_env.update(base_env)
     transform_params.update(base_params)
     transform = ContainerStep(name="transform",
-                              docker_env="iregistry.baidu-int.com/windmill-public/transform:v1.2.0.7",
+                              docker_env="iregistry.baidu-int.com/windmill-public/transform:v1.2.0-dev1",
                               env=transform_env,
                               parameters=transform_params,
                               inputs={"input_model_uri": train.outputs["output_model_uri"]},
                               outputs={"output_model_uri": Artifact(), "output_uri": Artifact()},
                               command=f'python3 -m gaea_operator.components.transform.ocrnet '
                                       f'--input-model-uri={{{{input_model_uri}}}} '
                                       f'--output-uri={{{{output_uri}}}} '
```

## gaea_operator/pipelines/ppyoloe_plus_pipeline/ppyoloe_plus_pipeline.py

```diff
@@ -87,15 +87,15 @@
                  "MODEL_NAME": "{{model_name}}",
                  "MODEL_DISPLAY_NAME": "{{model_display_name}}",
                  "ADVANCED_PARAMETERS": "{{advanced_parameters}}",
                  "PF_EXTRA_WORK_DIR": extra_fs_mount_path}
     train_env.update(base_env)
     train_params.update(base_params)
     train = ContainerStep(name="train",
-                          docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0.7",
+                          docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0-dev1",
                           parameters=train_params,
                           env=train_env,
                           extra_fs=[ExtraFS(name=extra_fs_name, mount_path=extra_fs_mount_path)],
                           outputs={"output_model_uri": Artifact(), "output_uri": Artifact()},
                           command=f'package_path=$(python3 -c "import site; print(site.getsitepackages()[0])") && '
                                   f'python3 -m gaea_operator.components.train.ppyoloe_plus '
                                   f'--output-model-uri={{{{output_model_uri}}}} '
@@ -109,15 +109,15 @@
                    "advanced_parameters": '{"conf_threshold":"0.5",'
                                           '"iou_threshold":"0.5"}'}
     eval_env = {"DATASET_NAME": "{{dataset_name}}",
                 "ADVANCED_PARAMETERS": "{{advanced_parameters}}"}
     eval_env.update(base_env)
     eval_params.update(base_params)
     eval = ContainerStep(name="eval",
-                         docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0.7",
+                         docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0-dev1",
                          parameters=eval_params,
                          env=eval_env,
                          inputs={"input_model_uri": train.outputs["output_model_uri"]},
                          outputs={"output_uri": Artifact(), "output_dataset_uri": Artifact()},
                          command=f'package_path=$(python3 -c "import site; print(site.getsitepackages()[0])") && '
                                  f'python3 -m gaea_operator.components.eval.ppyoloe_plus '
                                  f'--input-model-uri={{{{input_model_uri}}}} '
@@ -142,15 +142,15 @@
     transform_env = {"TRANSFORM_MODEL_NAME": "{{transform_model_name}}",
                      "TRANSFORM_MODEL_DISPLAY_NAME": "{{transform_model_display_name}}",
                      "ACCELERATOR": "{{accelerator}}",
                      "ADVANCED_PARAMETERS": "{{advanced_parameters}}"}
     transform_env.update(base_env)
     transform_params.update(base_params)
     transform = ContainerStep(name="transform",
-                              docker_env="iregistry.baidu-int.com/windmill-public/transform:v1.2.0.7",
+                              docker_env="iregistry.baidu-int.com/windmill-public/transform:v1.2.0-dev1",
                               env=transform_env,
                               parameters=transform_params,
                               inputs={"input_model_uri": train.outputs["output_model_uri"]},
                               outputs={"output_model_uri": Artifact(), "output_uri": Artifact()},
                               command=f'python3 -m gaea_operator.components.transform.ppyoloe_plus '
                                       f'--input-model-uri={{{{input_model_uri}}}} '
                                       f'--output-uri={{{{output_uri}}}} '
```

## gaea_operator/pipelines/resnet_pipeline/resnet_pipeline.py

```diff
@@ -89,15 +89,15 @@
                  "MODEL_NAME": "{{model_name}}",
                  "MODEL_DISPLAY_NAME": "{{model_display_name}}",
                  "ADVANCED_PARAMETERS": "{{advanced_parameters}}",
                  "PF_EXTRA_WORK_DIR": extra_fs_mount_path}
     train_env.update(base_env)
     train_params.update(base_params)
     train = ContainerStep(name="train",
-                          docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0.7",
+                          docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0-dev1",
                           parameters=train_params,
                           env=train_env,
                           extra_fs=[ExtraFS(name=extra_fs_name, mount_path=extra_fs_mount_path)],
                           outputs={"output_model_uri": Artifact(), "output_uri": Artifact()},
                           command=f'package_path=$(python3 -c "import site; print(site.getsitepackages()[0])") && '
                                   f'python3 -m gaea_operator.components.train.resnet '
                                   f'--output-model-uri={{{{output_model_uri}}}} '
@@ -108,15 +108,15 @@
                                   f'-o Global.output_dir={{{{output_model_uri}}}}')
 
     eval_params = {"dataset_name": eval_dataset_name}
     eval_env = {"DATASET_NAME": "{{dataset_name}}"}
     eval_env.update(base_env)
     eval_params.update(base_params)
     eval = ContainerStep(name="eval",
-                         docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0.7",
+                         docker_env="iregistry.baidu-int.com/windmill-public/train/paddlepaddle:v1.2.0-dev1",
                          parameters=eval_params,
                          env=eval_env,
                          inputs={"input_model_uri": train.outputs["output_model_uri"]},
                          outputs={"output_uri": Artifact(), "output_dataset_uri": Artifact()},
                          command=f'package_path=$(python3 -c "import site; print(site.getsitepackages()[0])") && '
                                  f'python3 -m gaea_operator.components.eval.resnet '
                                  f'--input-model-uri={{{{input_model_uri}}}} '
@@ -140,15 +140,15 @@
     transform_env = {"TRANSFORM_MODEL_NAME": "{{transform_model_name}}",
                      "TRANSFORM_MODEL_DISPLAY_NAME": "{{transform_model_display_name}}",
                      "ACCELERATOR": "{{accelerator}}",
                      "ADVANCED_PARAMETERS": "{{advanced_parameters}}"}
     transform_env.update(base_env)
     transform_params.update(base_params)
     transform = ContainerStep(name="transform",
-                              docker_env="iregistry.baidu-int.com/windmill-public/transform:v1.2.0.7",
+                              docker_env="iregistry.baidu-int.com/windmill-public/transform:v1.2.0-dev1",
                               env=transform_env,
                               parameters=transform_params,
                               inputs={"input_model_uri": train.outputs["output_model_uri"]},
                               outputs={"output_model_uri": Artifact(), "output_uri": Artifact()},
                               command=f'python3 -m gaea_operator.components.transform.resnet '
                                       f'--input-model-uri={{{{input_model_uri}}}} '
                                       f'--output-uri={{{{output_uri}}}} '
```

## gaea_operator/utils/__init__.py

```diff
@@ -20,16 +20,14 @@
 from .compress import get_filepaths_in_archive
 from .time import format_time
 from .accelerator import get_accelerator, Accelerator
 from .model_template import get_model_template, ModelTemplate
 from .registry import METRIC
 from .import_module import paddle, torch, Tensor, PTensor, TTensor
 from .tensor import list2ndarray, numpy_round2list, paddle_round2list, torch_round2list, list_round
-from .rle import rle_to_mask
-from .polygon import polygon_to_mask
 
 __all__ = ["find_upper_level_folder",
            "get_filepaths_in_archive",
            "write_file",
            "read_file",
            "write_yaml_file",
            "format_time",
@@ -51,10 +49,8 @@
            "Tensor",
            "PTensor",
            "TTensor",
            "list2ndarray",
            "numpy_round2list",
            "paddle_round2list",
            "torch_round2list",
-           "list_round",
-           "rle_to_mask",
-           "polygon_to_mask"]
+           "list_round"]
```

## gaea_operator/utils/accelerator.py

```diff
@@ -69,15 +69,15 @@
 class NvidiaAccelerator(Accelerator):
     """
     Nvidia Accelerator
     """
 
     def __init__(self, name: str = "T4"):
         super().__init__(name=name)
-        self.image = "iregistry.baidu-int.com/windmill-public/inference/nvidia:v1.2.0.7"
+        self.image = "iregistry.baidu-int.com/windmill-public/inference/nvidia:v1.2.0-dev1"
         self.args = {"backend-config": "tensorrt,plugins=/opt/tritonserver/lib/libmmdeploy_tensorrt_ops.so"}
         self.env = \
             {
                 "LD_LIBRARY_PATH":
                     "/usr/local/cuda/compat/lib:/usr/local/nvidia/lib:/usr/local/nvidia/lib64:/opt/tritonserver/lib",
                 "PATH": "/opt/tritonserver/bin:/usr/local/mpi/bin:/usr/local/nvidia/bin:/usr/local/cuda/bin:"
                         "/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/ucx/bin"
```

## Comparing `gaea_operator-1.2.0.dev4.data/data/yaml/object_detection.yaml` & `gaea_operator-1.2.0.dev5.data/data/yaml/object_detection.yaml`

 * *Files identical despite different names*

## Comparing `gaea_operator-1.2.0.dev4.data/data/yaml/parameter.yaml` & `gaea_operator-1.2.0.dev5.data/data/yaml/parameter.yaml`

 * *Files identical despite different names*

## Comparing `gaea_operator-1.2.0.dev4.data/data/yaml/parameter_c.yaml` & `gaea_operator-1.2.0.dev5.data/data/yaml/parameter_c.yaml`

 * *Files identical despite different names*

## Comparing `gaea_operator-1.2.0.dev4.data/data/yaml/train_parameter.yaml` & `gaea_operator-1.2.0.dev5.data/data/yaml/train_parameter.yaml`

 * *Files identical despite different names*

## Comparing `gaea_operator-1.2.0.dev4.data/data/yaml/transform_parameter.yaml` & `gaea_operator-1.2.0.dev5.data/data/yaml/transform_parameter.yaml`

 * *Files identical despite different names*

## Comparing `gaea_operator-1.2.0.dev4.dist-info/METADATA` & `gaea_operator-1.2.0.dev5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaea-operator
-Version: 1.2.0.dev4
+Version: 1.2.0.dev5
 Summary: A common operator library to help with training neural networks.
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/mlops/gaea-operator/tree/master
 Author: liuyawen03
 Author-email: liuyawen03@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `gaea_operator-1.2.0.dev4.dist-info/RECORD` & `gaea_operator-1.2.0.dev5.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,21 @@
 gaea_operator/config/ppyoloe_plus/ppyoloeplus_config.py,sha256=t1jN8ti8hpMM-l1U2Ukl8AS8xZsyKQh2pE5wNE1ew2U,4058
 gaea_operator/config/ppyoloe_plus/template/__init__.py,sha256=lX4deGvIgAQ1fTcskBUDqRfnOlOabgQjZXGwOJCVCkU,130
 gaea_operator/config/ppyoloe_plus/template/modify_train_parameter.py,sha256=BePbG16yrxAJiwctUbc0s1VtKDDThsDtylndcIO8WPk,12621
 gaea_operator/config/ppyoloe_plus/template/parameter.yaml,sha256=cliceLv-V-sYmwEzbXyylbXR4MElQZQ9yrAmg6CIohM,4583
 gaea_operator/config/ppyoloe_plus/template/parameter_c.yaml,sha256=KVxZIotf24fk_SAI1v-CHNMC2ouG_lpMY0l_CtSXoRM,4666
 gaea_operator/config/resnet/__init__.py,sha256=qIyiMMEuckOcc1g1DuA94Pa6HIwl9HHRcHbWtVeHPXc,130
 gaea_operator/config/resnet/resnet_config.py,sha256=oJcrEEsIOe8waeijGNit9B215bNULXYw_xO9AIn6k9U,4283
+gaea_operator/config/resnet/template/__init__.py,sha256=qIyiMMEuckOcc1g1DuA94Pa6HIwl9HHRcHbWtVeHPXc,130
+gaea_operator/config/resnet/template/modify_train_parameter.py,sha256=TbSV1IvnYIDS2m1uixHbJst4rA4BzzynbprqaLcSrwA,11498
 gaea_operator/config/resnet/template/parameter.yaml,sha256=c1lyNOcU63Ekb1gW86ZiHfwIOnrGJhLqOiyXEsLq9yU,2315
 gaea_operator/dataset/__init__.py,sha256=bV9qDmmiN73ZFRAUfOAAuUGv3C38Dejhv7gE0Y9Dx5k,370
 gaea_operator/dataset/cityscape_dataset.py,sha256=nxAllGXO40Fpqvm0RpQoS9whStodLp0ZpXTBhgjFXoM,4259
-gaea_operator/dataset/coco_dataset.py,sha256=pmumPof-fmUTAEGRjZGJpGkiIAoN9F9PjvU_Zcl1KCM,6515
-gaea_operator/dataset/dataset.py,sha256=GMpH1DzPRh4SAZMlTEpKEBLc3kyuzf9kCdjbXMyRtDU,7389
+gaea_operator/dataset/coco_dataset.py,sha256=YQMRb6Oe9yH75x3EpIV9wx8NiabDx0spPIHB8Ox8O28,6508
+gaea_operator/dataset/dataset.py,sha256=FEnDgbyS3bzx_XxLYnoEb-TXL3QB3NMNfbeByBhUmRA,7314
 gaea_operator/dataset/imagenet_dataset.py,sha256=TAfVBn6RtfdOpXP_2wr2hL4SRTwLAdCSKPV0Nm4kswY,4297
 gaea_operator/metric/__init__.py,sha256=fk0G_Cw3od-yzlYq5l48xDslTmqLFddrWoXOi3xqI48,584
 gaea_operator/metric/metric.py,sha256=p6KtrpC0muO0BPAdxePf3-17K5yRI6P5f9YhfncYhIo,5740
 gaea_operator/metric/analysis/__init__.py,sha256=kEv9_MuQOFC83fCprxY19T7omFNXa9dAuxstXlsEsX8,433
 gaea_operator/metric/analysis/eval_metric_analysis.py,sha256=LI84GVQICAdeliKo2JGNmAcp4caK3aObNR72lyMqQkc,18968
 gaea_operator/metric/analysis/inference_metric_analysis.py,sha256=oxXltL3ySZHvT0Ay1LjSo0sgxJb0emjE-gq7ClaJxHI,7907
 gaea_operator/metric/analysis/label_statistics_metric_analysis.py,sha256=93j10RML9xkGAu2fDQokIzl-0DYprLiVtnhdiThYRmQ,11706
@@ -70,44 +72,42 @@
 gaea_operator/metric/types/metric.py,sha256=H1KHU_Kf3yxXd4pvrxY2d75tBNkQ0vEQ526A6tg3AnI,4874
 gaea_operator/metric/types/object_detection_metric.py,sha256=fS5aJZ8lHxRAcs69bfgVlvRijsbAAjuWSg2ZtuVtKA0,2362
 gaea_operator/metric/types/semantic_segmentation_metric.py,sha256=RVOUp2x8QGKwf3EepvBR-yaLvEj0OF6uM0aC0Ah-ASQ,1244
 gaea_operator/model/__init__.py,sha256=EssP2HXBMWO-4iXPbWjscBrXxSojJBOOHV3p-ioV6tA,214
 gaea_operator/model/model.py,sha256=pNswhABsGB5HHeExA4fOHH4ob2uRPqs97sCzRGPQwIo,1436
 gaea_operator/pipelines/__init__.py,sha256=L2s64dKZZVsGx5vKew7wn61rdsT_y7GkzPJaxCs1rmw,131
 gaea_operator/pipelines/ocrnet_pipeline/__init__.py,sha256=L2s64dKZZVsGx5vKew7wn61rdsT_y7GkzPJaxCs1rmw,131
-gaea_operator/pipelines/ocrnet_pipeline/ocrnet_pipeline.py,sha256=LsTmBSXLXmSXx-5nLXL979rYC_e8SGHUkSmBO-qL5nE,12000
+gaea_operator/pipelines/ocrnet_pipeline/ocrnet_pipeline.py,sha256=7g8pjtZ0sKPgA3NY3jG36RFFVNZGPB1w3PNxnEgu-jk,12009
 gaea_operator/pipelines/ocrnet_pipeline/train_parameter.yaml,sha256=-9TJKBJuH8fA-Ftb-zarkuixRYCaDRd7pog6SilDrWk,1051
 gaea_operator/pipelines/ocrnet_pipeline/transform_parameter.yaml,sha256=TdQFxYG4tE0TnasDO_4nfJji1pCbMxRu9j0WtkOrYp8,1119
 gaea_operator/pipelines/ppyoloe_plus_pipeline/__init__.py,sha256=L2s64dKZZVsGx5vKew7wn61rdsT_y7GkzPJaxCs1rmw,131
-gaea_operator/pipelines/ppyoloe_plus_pipeline/ppyoloe_plus_pipeline.py,sha256=DiHdioKyMYUjha0LMvhjfSLqN7wHAxIuAMo2Nceh_2M,12387
+gaea_operator/pipelines/ppyoloe_plus_pipeline/ppyoloe_plus_pipeline.py,sha256=7FPepBD1tGz-941-vbphbaEdwSgg410o03Nma1GPrbc,12396
 gaea_operator/pipelines/ppyoloe_plus_pipeline/train_parameter.yaml,sha256=uDAljU4wltJi_TcK19ZF7eFVjck_Clju82c6yjOpmS8,1326
 gaea_operator/pipelines/ppyoloe_plus_pipeline/transform_parameter.yaml,sha256=j1am43Egq5r5ZPAq8SwQtXGexoGKDoieI07uUE0KJ4s,1815
 gaea_operator/pipelines/resnet_pipeline/__init__.py,sha256=L2s64dKZZVsGx5vKew7wn61rdsT_y7GkzPJaxCs1rmw,131
-gaea_operator/pipelines/resnet_pipeline/resnet_pipeline.py,sha256=hiieMptTPUdVQmcBP4onPx1ddbM01DaH1bsPRDcpItk,12178
+gaea_operator/pipelines/resnet_pipeline/resnet_pipeline.py,sha256=CFLBY_PY1LKVzWnPwq-Un-L-D1rYwmRGpkkF-nNLurw,12187
 gaea_operator/pipelines/resnet_pipeline/train_parameter.yaml,sha256=kVRkIx_DvDle-02D3YoWpVhJ8rkbXOiuBWSCF-YDCfY,1271
 gaea_operator/pipelines/resnet_pipeline/transform_parameter.yaml,sha256=luJ-ZjerE13jXu4e7igHrrtR8_k8UYSCTxiyQbS7VhE,1121
 gaea_operator/trainer/__init__.py,sha256=Kpisv4LZyJQy6vEce-8g3HS8bo8y6rwk8K3pEaF0na0,181
 gaea_operator/trainer/trainer.py,sha256=s0P1HZejcAtksmcIKuoUdHbK8oxGeEGNnpYfQW4fxr0,5406
 gaea_operator/transform/__init__.py,sha256=1NtMabt2_F9fVeLuAM7g3i0yIac_4RP0lHMZzdyDDcY,187
 gaea_operator/transform/cvt_copy_model.py,sha256=jSWWgt2RT9ULPLNyOxypmpNuQ1kWH0gw2XNe6OLE7Sw,3307
 gaea_operator/transform/transform.py,sha256=kDZ4m4QUPbuDYSwT6lKFH7T0GEADNL3f6T-L4IUjG0g,776
-gaea_operator/utils/__init__.py,sha256=SCy0RDbwujrgF1qJv0roKQUSEIti4hhqSh4azbJsgPE,1910
-gaea_operator/utils/accelerator.py,sha256=ZQjb-HwQFcKA36bW25lc_WkUx5A2UZYDGY8c3EOEHMs,5554
+gaea_operator/utils/__init__.py,sha256=DmxN4SMbqaCs_ZHTJBF9eMitaXKLIi1Qm6TKHT_NY0Q,1788
+gaea_operator/utils/accelerator.py,sha256=pSxy9v9IS1xWQ_utJWQ4ljX80-rrRxnHoSBFmDZLAuY,5557
 gaea_operator/utils/compress.py,sha256=rnM_Wv_UrP9LB30xeu6f5Zch3QFH-pHGcReC8PTYjZk,2887
 gaea_operator/utils/consts.py,sha256=0TsyISenFn_x8eRNIH1fdXPLw8zSac-IAfiCxKbhySw,426
 gaea_operator/utils/file.py,sha256=9g9fFq8aw4t0I8D3wkN9Bao3tfaN3X3itZmO4LF6MsU,1948
 gaea_operator/utils/import_module.py,sha256=W1mKFqBClRsYm9MNqParN-03PUFIwgMJJAgSAvD9m38,1533
 gaea_operator/utils/model_template.py,sha256=n9vvjumL9wtqTHmyvLsdZdewyH1sksqGY6APmnIGG7Y,6613
-gaea_operator/utils/polygon.py,sha256=-0_vOQhcs6Q7p70I5Y2DoDhtvxlKIxOiJf6mGx897C8,563
 gaea_operator/utils/registry.py,sha256=QchfsCrwhk3i8gmtS16PAF4029TcdOdEeWUdo1ruAps,1680
-gaea_operator/utils/rle.py,sha256=siXHQ5FCOsR_Mwj1O6v9OgFm_dD18QZsEOl4N-nDJvU,613
 gaea_operator/utils/tensor.py,sha256=BLnnyKz79hOqZy-L7IeA4ffDX5DoWP9NvLzStdI6C8w,1000
 gaea_operator/utils/time.py,sha256=xNKc-rzCCwhh-hNlNO05J_TA6rCMKMepuZ3qzvcScLs,301
-gaea_operator-1.2.0.dev4.data/data/yaml/object_detection.yaml,sha256=2V6AJBVa1nAE9FAosyz4z4Qv0ebw1IumYoRPUWo3Ebg,4864
-gaea_operator-1.2.0.dev4.data/data/yaml/parameter.yaml,sha256=cliceLv-V-sYmwEzbXyylbXR4MElQZQ9yrAmg6CIohM,4583
-gaea_operator-1.2.0.dev4.data/data/yaml/parameter_c.yaml,sha256=KVxZIotf24fk_SAI1v-CHNMC2ouG_lpMY0l_CtSXoRM,4666
-gaea_operator-1.2.0.dev4.data/data/yaml/train_parameter.yaml,sha256=-9TJKBJuH8fA-Ftb-zarkuixRYCaDRd7pog6SilDrWk,1051
-gaea_operator-1.2.0.dev4.data/data/yaml/transform_parameter.yaml,sha256=TdQFxYG4tE0TnasDO_4nfJji1pCbMxRu9j0WtkOrYp8,1119
-gaea_operator-1.2.0.dev4.dist-info/METADATA,sha256=SUoP6BOlo-oCb2aqLatz3S0K2jDqHXnxd4_rwvrP0g4,2173
-gaea_operator-1.2.0.dev4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-gaea_operator-1.2.0.dev4.dist-info/top_level.txt,sha256=1-ONMzqexKnQ2qOurelrROodwfO1B8jTzpzbERvNycY,14
-gaea_operator-1.2.0.dev4.dist-info/RECORD,,
+gaea_operator-1.2.0.dev5.data/data/yaml/object_detection.yaml,sha256=2V6AJBVa1nAE9FAosyz4z4Qv0ebw1IumYoRPUWo3Ebg,4864
+gaea_operator-1.2.0.dev5.data/data/yaml/parameter.yaml,sha256=cliceLv-V-sYmwEzbXyylbXR4MElQZQ9yrAmg6CIohM,4583
+gaea_operator-1.2.0.dev5.data/data/yaml/parameter_c.yaml,sha256=KVxZIotf24fk_SAI1v-CHNMC2ouG_lpMY0l_CtSXoRM,4666
+gaea_operator-1.2.0.dev5.data/data/yaml/train_parameter.yaml,sha256=-9TJKBJuH8fA-Ftb-zarkuixRYCaDRd7pog6SilDrWk,1051
+gaea_operator-1.2.0.dev5.data/data/yaml/transform_parameter.yaml,sha256=TdQFxYG4tE0TnasDO_4nfJji1pCbMxRu9j0WtkOrYp8,1119
+gaea_operator-1.2.0.dev5.dist-info/METADATA,sha256=y9W1V0nEC3Nd9tng-VuE2Ka2vVJOMtAvOaRaZoj4QSE,2173
+gaea_operator-1.2.0.dev5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+gaea_operator-1.2.0.dev5.dist-info/top_level.txt,sha256=1-ONMzqexKnQ2qOurelrROodwfO1B8jTzpzbERvNycY,14
+gaea_operator-1.2.0.dev5.dist-info/RECORD,,
```

