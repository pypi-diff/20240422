# Comparing `tmp/flgo-0.2.8.tar.gz` & `tmp/flgo-0.2.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flgo-0.2.8.tar", last modified: Thu Apr 18 09:37:41 2024, max compression
+gzip compressed data, was "flgo-0.2.8a0.tar", last modified: Mon Apr 22 02:43:14 2024, max compression
```

## Comparing `flgo-0.2.8.tar` & `flgo-0.2.8a0.tar`

### file list

```diff
@@ -1,553 +1,553 @@
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1091 2023-03-21 13:46:37.000000 flgo-0.2.8/LICENSE
--rw-r--r--   0 wz        (1001) wz        (1001)      716 2024-04-18 09:37:41.237956 flgo-0.2.8/PKG-INFO
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-21 13:46:37.000000 flgo-0.2.8/README.md
--rw-rw-r--   0 wz        (1001) wz        (1001)      764 2024-04-18 09:36:48.000000 flgo-0.2.8/pyproject.toml
--rw-rw-r--   0 wz        (1001) wz        (1001)       38 2024-04-18 09:37:41.237956 flgo-0.2.8/setup.cfg
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.205956 flgo-0.2.8/src/
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.213956 flgo-0.2.8/src/flgo/
--rw-rw-r--   0 wz        (1001) wz        (1001)      915 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.213956 flgo-0.2.8/src/flgo/algorithm/
--rw-rw-r--   0 wz        (1001) wz        (1001)     3753 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/TiFL.py
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3358 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/afl.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4015 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/asyncbase.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6959 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/clustered_sampling.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11333 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/decentralized.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2056 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/ditto.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1264 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/fedasync.py
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/fedavg.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      711 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/fedavgm.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    40012 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/fedbase.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1702 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/fedbuff.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2856 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/feddyn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2258 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/fedfa.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3381 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/fedfv.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7205 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/fedmf.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2920 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/fedmgda.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2110 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/fednova.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1444 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/fedprox.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     8853 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/hierarchical.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1800 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/mifa.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1501 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/powerofchoice.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/qfedavg.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    32732 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/realbase.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3421 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/scaffold.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9202 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/sesorec.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3013 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/standalone.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    17504 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/algorithm/vflbase.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.213956 flgo-0.2.8/src/flgo/benchmark/
--rw-rw-r--   0 wz        (1001) wz        (1001)     2390 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.213956 flgo-0.2.8/src/flgo/benchmark/adult_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      239 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/adult_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      700 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/adult_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.213956 flgo-0.2.8/src/flgo/benchmark/adult_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/adult_classification/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      466 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/adult_classification/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.213956 flgo-0.2.8/src/flgo/benchmark/agnews_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/agnews_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2003 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/agnews_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3955 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/agnews_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.213956 flgo-0.2.8/src/flgo/benchmark/agnews_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/agnews_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.213956 flgo-0.2.8/src/flgo/benchmark/bankmarketing_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/bankmarketing_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      725 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/bankmarketing_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/bankmarketing_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/bankmarketing_classification/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      430 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/bankmarketing_classification/model/lr.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    24978 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/base.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/ciao_recommendation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/ciao_recommendation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      821 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/ciao_recommendation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/ciao_recommendation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      848 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/ciao_recommendation/model/mf.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/cifar100_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1734 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cifar100_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1288 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cifar100_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cifar100_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      510 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cifar100_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/cifar100_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      991 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cifar100_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cifar100_classification/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5388 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cifar100_classification/model/resnet18.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2262 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cifar100_classification/model/resnet18_gn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/cifar10_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1888 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cifar10_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1223 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cifar10_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cifar10_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      520 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cifar10_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/cifar10_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      824 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cifar10_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1502 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cifar10_classification/model/cnn_data_aug.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cifar10_classification/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      741 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cifar10_classification/model/mlp.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2261 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cifar10_classification/model/resnet18_gn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/citeseer_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/citeseer_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1733 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/citeseer_link_prediction/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/citeseer_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/citeseer_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/citeseer_link_prediction/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/citeseer_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/citeseer_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      771 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/citeseer_node_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      807 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/citeseer_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/citeseer_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/citeseer_node_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/coco_detection/
--rw-rw-r--   0 wz        (1001) wz        (1001)      265 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/coco_detection/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6847 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/coco_detection/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/coco_detection/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     9240 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/coco_detection/model/FasterRCNN.py
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/coco_detection/model/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/coco_segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/coco_segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     8013 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/coco_segmentation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/coco_segmentation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/coco_segmentation/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      521 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/coco_segmentation/model/fcn_resnet50.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1459 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/coco_segmentation/model/unet.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/cora_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cora_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1717 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cora_link_prediction/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cora_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/cora_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      853 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cora_link_prediction/model/GCN.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cora_link_prediction/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/cora_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cora_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      805 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cora_node_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      807 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/cora_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/cora_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      727 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cora_node_classification/model/GCN.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      730 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4070 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cora_node_classification/model/GraphSage.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/cora_node_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/crop_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      241 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/crop_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      842 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/crop_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/crop_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1243 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/crop_classification/model/cnn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/distributed_quadratic_programming/
--rw-rw-r--   0 wz        (1001) wz        (1001)       93 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/distributed_quadratic_programming/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2298 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/distributed_quadratic_programming/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/distributed_quadratic_programming/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      569 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/distributed_quadratic_programming/model/vec.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/electricdevices_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      252 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/electricdevices_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      864 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/electricdevices_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.217956 flgo-0.2.8/src/flgo/benchmark/electricdevices_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1243 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/electricdevices_classification/model/cnn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/electricity_forecasting/
--rw-rw-r--   0 wz        (1001) wz        (1001)      245 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/electricity_forecasting/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      697 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/electricity_forecasting/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/electricity_forecasting/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      916 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/electricity_forecasting/model/GRU.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/emnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      357 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/emnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1199 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/emnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/emnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      875 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/emnist_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      709 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/emnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/enzymes_graph_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/enzymes_graph_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1873 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/enzymes_graph_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/enzymes_graph_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/enzymes_graph_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/enzymes_graph_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/epinions_recommendation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/epinions_recommendation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      833 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/epinions_recommendation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/epinions_recommendation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      848 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/epinions_recommendation/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      938 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/epinions_recommendation/model/mf.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/exchange_rate_forecasting/
--rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/exchange_rate_forecasting/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2884 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/exchange_rate_forecasting/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/exchange_rate_forecasting/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      914 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/exchange_rate_forecasting/model/GRU.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/fashion_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/fashion_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/fashion_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      487 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/fashion_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/fashion_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      578 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/fashion_classification/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/fcube_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       78 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/fcube_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1912 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/fcube_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/fcube_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/fcube_classification/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      553 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/fcube_classification/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/femnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      358 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/femnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/femnist_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5327 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/femnist_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/femnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/femnist_classification/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      875 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/femnist_classification/model/cnn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/heart_disease_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/heart_disease_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      723 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/heart_disease_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/heart_disease_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/heart_disease_classification/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      465 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/heart_disease_classification/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/imdb_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/imdb_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1993 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/imdb_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3907 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/imdb_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/imdb_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/imdb_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/leaf_reddit/
--rw-rw-r--   0 wz        (1001) wz        (1001)       87 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/leaf_reddit/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    10132 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/leaf_reddit/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/leaf_reddit/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      980 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/leaf_sent140/
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/leaf_sent140/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11379 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/leaf_sent140/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/leaf_sent140/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/local_movielens_recommendation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      211 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/local_movielens_recommendation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      839 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/local_movielens_recommendation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/local_movielens_recommendation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1748 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/local_movielens_recommendation/model/mf.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/mnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1850 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/mnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      463 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/mnist_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      660 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/mnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/mnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      899 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/mnist_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      703 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/mnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/movielens_recommendation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/movielens_recommendation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      835 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/movielens_recommendation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/movielens_recommendation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/movielens_recommendation/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      787 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/movielens_recommendation/model/mf.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/multi30k_translation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/multi30k_translation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6631 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/multi30k_translation/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6514 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/multi30k_translation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.221956 flgo-0.2.8/src/flgo/benchmark/multi30k_translation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/multi30k_translation/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/mutag_graph_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/mutag_graph_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1564 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/mutag_graph_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/mutag_graph_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/mutag_graph_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/mutag_graph_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/nifECG_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      243 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/nifECG_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      886 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/nifECG_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/nifECG_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1246 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/nifECG_classification/model/cnn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/oxfordiiitpet_segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/oxfordiiitpet_segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1006 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/oxfordiiitpet_segmentation/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      797 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/oxfordiiitpet_segmentation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/oxfordiiitpet_segmentation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/oxfordiiitpet_segmentation/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    34092 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/benchmark/partition.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/penntreebank_modeling/
--rw-rw-r--   0 wz        (1001) wz        (1001)      275 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/penntreebank_modeling/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3387 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/penntreebank_modeling/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/penntreebank_modeling/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/penntreebank_modeling/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/penntreebank_modeling/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/pubmed_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/pubmed_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1726 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/pubmed_link_prediction/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/pubmed_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/pubmed_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/pubmed_link_prediction/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/pubmed_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/pubmed_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      820 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/pubmed_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/pubmed_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      726 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/pubmed_node_classification/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/sbdataset_segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      277 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/sbdataset_segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6604 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/sbdataset_segmentation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/sbdataset_segmentation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/sbdataset_segmentation/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      521 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/sbdataset_segmentation/model/fcn_resnet50.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1459 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/sbdataset_segmentation/model/unet.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/shakespeare_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      262 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/shakespeare_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    15413 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/shakespeare_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/shakespeare_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     2169 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/social_splitted_ciao/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_ciao/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9479 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_ciao/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/social_splitted_ciao/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_ciao/model/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/social_splitted_ciaodvd/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_ciaodvd/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9210 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_ciaodvd/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/social_splitted_douban/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_douban/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     8344 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_douban/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/social_splitted_epinions/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_epinions/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9394 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_epinions/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/social_splitted_epinions/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_epinions/model/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/social_splitted_filmtrust/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_filmtrust/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9247 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/social_splitted_filmtrust/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/sst2_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/sst2_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1987 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/sst2_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3955 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/sst2_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/sst2_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/sst2_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/stl10_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      500 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/stl10_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1302 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/stl10_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/stl10_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      517 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/stl10_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/stl10_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      857 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/stl10_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1536 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/stl10_classification/model/cnn_data_aug.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/stl10_classification/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2261 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/stl10_classification/model/resnet18_gn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3391 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/stl10_classification/model/resnet34_gn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/svhn_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      355 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/svhn_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/svhn_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      444 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/svhn_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.225956 flgo-0.2.8/src/flgo/benchmark/svhn_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      895 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/svhn_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      897 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/svhn_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/synthetic_regression/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1079 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/synthetic_regression/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3901 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/synthetic_regression/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/synthetic_regression/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      555 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/synthetic_regression/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1687 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)    21425 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/dec_temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      341 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/dec_temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/dec_temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1035 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/dec_temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/dec_temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/dec_temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/hier_temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      260 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/hier_temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/hier_temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      847 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/hier_temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/hier_temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/hier_temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/
--rw-rw-r--   0 wz        (1001) wz        (1001)     8935 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6637 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/coco_eval.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9179 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/coco_utils.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2636 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/presets.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      794 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/temp/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    23912 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/transforms.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    16307 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)    21601 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/pointnet2_utils.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/pointnet_utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      811 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)    25417 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet2_utils.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet_utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      813 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)    24155 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet2_utils.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet_utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      347 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4059 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.229956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)    16044 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3939 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/coco_utils.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1314 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/presets.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      797 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2797 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/transforms.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    10798 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/general/
--rw-rw-r--   0 wz        (1001) wz        (1001)      279 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/general/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      625 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/general/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4009 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/general/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/general/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      465 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/general/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/graph_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     9023 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/graph_classification/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/graph_classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/graph_classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/graph_classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/graph_classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)    12697 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      524 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5455 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      682 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)    17008 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/node_classification/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/node_classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/node_classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/node_classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5558 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/node_classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     7121 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/classification/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      338 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3907 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/language_modeling/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/language_modeling/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      275 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/translation/
--rw-rw-r--   0 wz        (1001) wz        (1001)     2774 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/translation/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/translation/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/translation/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/translation/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6514 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/translation/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/translation/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/translation/temp/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    25125 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/partition.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/rec/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/rec/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     8776 2024-04-18 09:37:24.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/rec/datasets.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/rec/rating_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)    11647 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/rec/rating_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      425 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/rec/utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/series/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     9882 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1600 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/datasets.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4639 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/
--rw-rw-r--   0 wz        (1001) wz        (1001)    13427 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4531 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/datasets.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      185 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7994 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:26.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/tabular/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/tabular/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.233956 flgo-0.2.8/src/flgo/benchmark/toolkits/tabular/classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     9992 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/tabular/classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11416 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/tabular/classification/datasets.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7488 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/toolkits/visualization.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/src/flgo/benchmark/vertical_mnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      260 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/vertical_mnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7230 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/vertical_mnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/src/flgo/benchmark/vertical_mnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1162 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/src/flgo/benchmark/voc_detection/
--rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/voc_detection/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2159 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/voc_detection/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      794 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/voc_detection/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/src/flgo/benchmark/voc_detection/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/voc_detection/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/src/flgo/benchmark/wikitext2_modeling/
--rw-rw-r--   0 wz        (1001) wz        (1001)      273 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/wikitext2_modeling/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3375 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/wikitext2_modeling/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/benchmark/wikitext2_modeling/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/src/flgo/benchmark/wikitext2_modeling/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-18 09:37:25.000000 flgo-0.2.8/src/flgo/benchmark/wikitext2_modeling/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/src/flgo/experiment/
--rw-rw-r--   0 wz        (1001) wz        (1001)       62 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/experiment/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    27628 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/experiment/analyzer.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6651 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/experiment/device_scheduler.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/src/flgo/experiment/logger/
--rw-rw-r--   0 wz        (1001) wz        (1001)    90223 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    36834 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1857 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/dec_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2262 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/full_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      343 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/gval_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    59619 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/handlers.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      469 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/hier_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      323 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/parallel_hlogger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1522 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/pfl_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      415 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/pool.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1598 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/simple_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      386 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/test_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      951 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/tune_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1040 2024-04-18 09:37:23.000000 flgo-0.2.8/src/flgo/experiment/logger/vertical_logger.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/src/flgo/simulator/
--rw-rw-r--   0 wz        (1001) wz        (1001)     5181 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/simulator/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    25114 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/simulator/base.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    17046 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/simulator/default_simulator.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1030 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/simulator/my_simulator.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    17600 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/simulator/phone_simulator.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/src/flgo/utils/
--rw-rw-r--   0 wz        (1001) wz        (1001)     3173 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/utils/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    78301 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/utils/fflow.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    28264 2024-04-18 09:37:22.000000 flgo-0.2.8/src/flgo/utils/fmodule.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/src/flgo.egg-info/
--rw-r--r--   0 wz        (1001) wz        (1001)      716 2024-04-18 09:37:41.000000 flgo-0.2.8/src/flgo.egg-info/PKG-INFO
--rw-rw-r--   0 wz        (1001) wz        (1001)    20511 2024-04-18 09:37:41.000000 flgo-0.2.8/src/flgo.egg-info/SOURCES.txt
--rw-rw-r--   0 wz        (1001) wz        (1001)        1 2024-04-18 09:37:41.000000 flgo-0.2.8/src/flgo.egg-info/dependency_links.txt
--rw-rw-r--   0 wz        (1001) wz        (1001)       81 2024-04-18 09:37:41.000000 flgo-0.2.8/src/flgo.egg-info/requires.txt
--rw-rw-r--   0 wz        (1001) wz        (1001)        5 2024-04-18 09:37:41.000000 flgo-0.2.8/src/flgo.egg-info/top_level.txt
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-18 09:37:41.237956 flgo-0.2.8/tests/
--rw-rw-r--   0 wz        (1001) wz        (1001)      947 2023-03-21 13:46:37.000000 flgo-0.2.8/tests/test.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.713194 flgo-0.2.8a0/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1091 2023-03-21 13:46:37.000000 flgo-0.2.8a0/LICENSE
+-rw-r--r--   0 wz        (1001) wz        (1001)      718 2024-04-22 02:43:14.713194 flgo-0.2.8a0/PKG-INFO
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-21 13:46:37.000000 flgo-0.2.8a0/README.md
+-rw-rw-r--   0 wz        (1001) wz        (1001)      765 2024-04-22 02:43:00.000000 flgo-0.2.8a0/pyproject.toml
+-rw-rw-r--   0 wz        (1001) wz        (1001)       38 2024-04-22 02:43:14.713194 flgo-0.2.8a0/setup.cfg
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.677194 flgo-0.2.8a0/src/
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.685194 flgo-0.2.8a0/src/flgo/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      916 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/algorithm/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3753 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/TiFL.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3358 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/afl.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4015 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/asyncbase.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6959 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/clustered_sampling.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11333 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/decentralized.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2056 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/ditto.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1264 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/fedasync.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)       86 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/fedavg.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      711 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/fedavgm.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    40012 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/fedbase.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1702 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/fedbuff.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2856 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/feddyn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2258 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/fedfa.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3381 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/fedfv.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7205 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/fedmf.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2920 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/fedmgda.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2110 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/fednova.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1444 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/fedprox.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8853 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/hierarchical.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1800 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/mifa.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1501 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/powerofchoice.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/qfedavg.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    32732 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/realbase.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3421 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/scaffold.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9202 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/sesorec.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3013 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/standalone.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    17504 2024-04-22 02:42:04.000000 flgo-0.2.8a0/src/flgo/algorithm/vflbase.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2390 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/adult_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      239 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/adult_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      700 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/adult_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/adult_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/adult_classification/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      466 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/adult_classification/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/agnews_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/agnews_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2003 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/agnews_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3955 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/agnews_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/agnews_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/agnews_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/bankmarketing_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/bankmarketing_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      725 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/bankmarketing_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/bankmarketing_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/bankmarketing_classification/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      430 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/bankmarketing_classification/model/lr.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    24978 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/base.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/ciao_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/ciao_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      821 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/ciao_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/ciao_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      848 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/ciao_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1734 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1288 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      510 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      991 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5388 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/model/resnet18.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2262 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/model/resnet18_gn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1888 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1223 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      520 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      824 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1502 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/model/cnn_data_aug.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      741 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/model/mlp.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2261 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/model/resnet18_gn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/citeseer_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/citeseer_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1733 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/citeseer_link_prediction/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/citeseer_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/citeseer_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/citeseer_link_prediction/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/citeseer_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/citeseer_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      771 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/citeseer_node_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      807 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/citeseer_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/citeseer_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/citeseer_node_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/coco_detection/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      265 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/coco_detection/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6847 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/coco_detection/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/coco_detection/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9240 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/coco_detection/model/FasterRCNN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/coco_detection/model/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.689194 flgo-0.2.8a0/src/flgo/benchmark/coco_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/coco_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8013 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/coco_segmentation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/coco_segmentation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/coco_segmentation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      521 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/coco_segmentation/model/fcn_resnet50.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1459 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/coco_segmentation/model/unet.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/cora_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1717 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_link_prediction/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/cora_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      853 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_link_prediction/model/GCN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_link_prediction/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      805 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      807 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      727 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/model/GCN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      730 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4070 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/model/GraphSage.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/crop_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      241 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/crop_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      842 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/crop_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/crop_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1243 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/crop_classification/model/cnn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/distributed_quadratic_programming/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       93 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/distributed_quadratic_programming/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2298 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/distributed_quadratic_programming/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/distributed_quadratic_programming/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      569 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/distributed_quadratic_programming/model/vec.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/electricdevices_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      252 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/electricdevices_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      864 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/electricdevices_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/electricdevices_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1243 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/electricdevices_classification/model/cnn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/electricity_forecasting/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      245 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/electricity_forecasting/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      697 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/electricity_forecasting/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/electricity_forecasting/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      916 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/electricity_forecasting/model/GRU.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/emnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      357 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/emnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1199 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/emnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/emnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      875 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/emnist_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      709 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/emnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/enzymes_graph_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/enzymes_graph_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1873 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/enzymes_graph_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/enzymes_graph_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/enzymes_graph_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/enzymes_graph_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/epinions_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/epinions_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      833 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/epinions_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/epinions_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      848 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/epinions_recommendation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      938 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/epinions_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/exchange_rate_forecasting/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/exchange_rate_forecasting/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2884 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/exchange_rate_forecasting/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/exchange_rate_forecasting/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      914 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/exchange_rate_forecasting/model/GRU.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/fashion_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/fashion_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/fashion_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      487 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/fashion_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/fashion_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      578 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/fashion_classification/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/fcube_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       78 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/fcube_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1912 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/fcube_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/fcube_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/fcube_classification/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      553 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/fcube_classification/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/femnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      358 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/femnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/femnist_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5327 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/femnist_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/femnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/femnist_classification/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      875 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/femnist_classification/model/cnn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/heart_disease_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/heart_disease_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      723 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/heart_disease_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/heart_disease_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/heart_disease_classification/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      465 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/heart_disease_classification/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.693194 flgo-0.2.8a0/src/flgo/benchmark/imdb_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/imdb_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1993 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/imdb_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3907 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/imdb_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/imdb_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/imdb_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/leaf_reddit/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       87 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/leaf_reddit/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    10132 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/leaf_reddit/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/leaf_reddit/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      980 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/leaf_sent140/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       86 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/leaf_sent140/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11379 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/leaf_sent140/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/leaf_sent140/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/local_movielens_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      211 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/local_movielens_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      839 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/local_movielens_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/local_movielens_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1748 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/local_movielens_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/mnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1850 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/mnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      463 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/mnist_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      660 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/mnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/mnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      899 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/mnist_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      703 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/mnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/movielens_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/movielens_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      835 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/movielens_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/movielens_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/movielens_recommendation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      787 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/movielens_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/multi30k_translation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/multi30k_translation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6631 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/multi30k_translation/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6514 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/multi30k_translation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/multi30k_translation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/multi30k_translation/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/mutag_graph_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/mutag_graph_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1564 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/mutag_graph_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/mutag_graph_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/mutag_graph_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/mutag_graph_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/nifECG_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      243 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/nifECG_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      886 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/nifECG_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/nifECG_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1246 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/nifECG_classification/model/cnn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/oxfordiiitpet_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/oxfordiiitpet_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1006 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/oxfordiiitpet_segmentation/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      797 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/oxfordiiitpet_segmentation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/oxfordiiitpet_segmentation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/oxfordiiitpet_segmentation/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    34092 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/benchmark/partition.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/penntreebank_modeling/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      275 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/penntreebank_modeling/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3387 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/penntreebank_modeling/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/penntreebank_modeling/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/penntreebank_modeling/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/penntreebank_modeling/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/pubmed_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/pubmed_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1726 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/pubmed_link_prediction/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/pubmed_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/pubmed_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/pubmed_link_prediction/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/pubmed_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/pubmed_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      820 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/pubmed_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/pubmed_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      726 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/pubmed_node_classification/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/sbdataset_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      277 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/sbdataset_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6604 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/sbdataset_segmentation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/sbdataset_segmentation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/sbdataset_segmentation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      521 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/sbdataset_segmentation/model/fcn_resnet50.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1459 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/sbdataset_segmentation/model/unet.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/shakespeare_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      262 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/shakespeare_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    15413 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/shakespeare_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/shakespeare_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2169 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_ciao/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_ciao/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9479 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_ciao/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_ciao/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_ciao/model/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_ciaodvd/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_ciaodvd/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9210 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_ciaodvd/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.697194 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_douban/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_douban/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8344 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_douban/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_epinions/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_epinions/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9394 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_epinions/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_epinions/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_epinions/model/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_filmtrust/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_filmtrust/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9247 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/social_splitted_filmtrust/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/sst2_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/sst2_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1987 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/sst2_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3955 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/sst2_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/sst2_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/sst2_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      500 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1302 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      517 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      857 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1536 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/model/cnn_data_aug.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2261 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/model/resnet18_gn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3391 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/model/resnet34_gn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/svhn_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      355 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/svhn_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/svhn_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      444 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/svhn_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/svhn_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      895 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/svhn_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      897 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/svhn_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/synthetic_regression/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1079 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/synthetic_regression/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3901 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/synthetic_regression/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/synthetic_regression/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      555 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/synthetic_regression/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1687 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    21425 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/dec_temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      341 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/dec_temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/dec_temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1035 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/dec_temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/dec_temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/dec_temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/hier_temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      260 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/hier_temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/hier_temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      847 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/hier_temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/hier_temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/hier_temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8935 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6637 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/coco_eval.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9179 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/coco_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2636 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/presets.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      794 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/temp/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    23912 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/transforms.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    16307 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    21601 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/pointnet2_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/pointnet_utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.701194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      811 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    25417 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet2_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet_utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      813 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    24155 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet2_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet_utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      347 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4059 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    16044 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3939 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/coco_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1314 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/presets.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      797 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2797 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/transforms.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    10798 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/general/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      279 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/general/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      625 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/general/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4009 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/general/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/general/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      465 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/general/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/graph_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9023 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/graph_classification/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/graph_classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/graph_classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/graph_classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/graph_classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    12697 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      524 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5455 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      682 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    17008 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/node_classification/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/node_classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/node_classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/node_classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5558 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/node_classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7121 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/classification/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      338 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3907 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/language_modeling/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/language_modeling/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      275 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/translation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2774 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/translation/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.705194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/translation/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/translation/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/translation/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6514 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/translation/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/translation/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/translation/temp/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    25125 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/partition.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/rec/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/rec/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8776 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/rec/datasets.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/rec/rating_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11647 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/rec/rating_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      425 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/rec/utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9882 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1600 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/datasets.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4639 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    13427 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4531 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/datasets.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      185 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7994 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:08.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/tabular/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/tabular/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/toolkits/tabular/classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9992 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/tabular/classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11416 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/tabular/classification/datasets.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7488 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/toolkits/visualization.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/vertical_mnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      260 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/vertical_mnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7230 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/vertical_mnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/vertical_mnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1162 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/voc_detection/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/voc_detection/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2159 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/voc_detection/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      794 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/voc_detection/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/voc_detection/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/voc_detection/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/wikitext2_modeling/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      273 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/wikitext2_modeling/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3375 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/wikitext2_modeling/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/benchmark/wikitext2_modeling/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/benchmark/wikitext2_modeling/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-22 02:42:07.000000 flgo-0.2.8a0/src/flgo/benchmark/wikitext2_modeling/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/experiment/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       62 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/experiment/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    27628 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/experiment/analyzer.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6651 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/experiment/device_scheduler.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/experiment/logger/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    90223 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    36834 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1857 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/dec_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2262 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/full_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      343 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/gval_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    59619 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/handlers.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      469 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/hier_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      323 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/parallel_hlogger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1522 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/pfl_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      415 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/pool.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1598 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/simple_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      386 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/test_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      951 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/tune_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1040 2024-04-22 02:42:06.000000 flgo-0.2.8a0/src/flgo/experiment/logger/vertical_logger.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/simulator/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7000 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/simulator/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    25114 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/simulator/base.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    17046 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/simulator/default_simulator.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1030 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/simulator/my_simulator.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    17600 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/simulator/phone_simulator.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.709194 flgo-0.2.8a0/src/flgo/utils/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3173 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/utils/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    78301 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/utils/fflow.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    28264 2024-04-22 02:42:05.000000 flgo-0.2.8a0/src/flgo/utils/fmodule.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.713194 flgo-0.2.8a0/src/flgo.egg-info/
+-rw-r--r--   0 wz        (1001) wz        (1001)      718 2024-04-22 02:43:14.000000 flgo-0.2.8a0/src/flgo.egg-info/PKG-INFO
+-rw-rw-r--   0 wz        (1001) wz        (1001)    20511 2024-04-22 02:43:14.000000 flgo-0.2.8a0/src/flgo.egg-info/SOURCES.txt
+-rw-rw-r--   0 wz        (1001) wz        (1001)        1 2024-04-22 02:43:14.000000 flgo-0.2.8a0/src/flgo.egg-info/dependency_links.txt
+-rw-rw-r--   0 wz        (1001) wz        (1001)       81 2024-04-22 02:43:14.000000 flgo-0.2.8a0/src/flgo.egg-info/requires.txt
+-rw-rw-r--   0 wz        (1001) wz        (1001)        5 2024-04-22 02:43:14.000000 flgo-0.2.8a0/src/flgo.egg-info/top_level.txt
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-22 02:43:14.713194 flgo-0.2.8a0/tests/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      947 2023-03-21 13:46:37.000000 flgo-0.2.8a0/tests/test.py
```

### Comparing `flgo-0.2.8/LICENSE` & `flgo-0.2.8a0/LICENSE`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/PKG-INFO` & `flgo-0.2.8a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flgo
-Version: 0.2.8
+Version: 0.2.8a0
 Summary: A Research-oriented FL Platform. 
 Author-email: Zheng Wang <zwang@stu.xmu.edu.cn>
 Project-URL: Homepage, https://flgo-xmu.github.io
 Project-URL: Bug Tracker, https://github.com/WwZzz/easyFL/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flgo-0.2.8/pyproject.toml` & `flgo-0.2.8a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "setuptools" 
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "flgo"
-version = "0.2.8"
+version = "0.2.8a"
 authors = [
   { name="Zheng Wang", email="zwang@stu.xmu.edu.cn" },
 ]
 dependencies = [
     "tqdm",
     "torch",
     "torchvision",
```

### Comparing `flgo-0.2.8/src/flgo/__init__.py` & `flgo-0.2.8a0/src/flgo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .utils.fflow import init, gen_task, gen_task_by_, gen_benchmark_from_file, zip_task, pull_task_from_, gen_real_task, gen_decentralized_benchmark, gen_hierarchical_benchmark, gen_empty_task, convert_model,tune, run_in_parallel, module2fmodule, multi_init_and_run, set_data_root,download_resource, list_resource, option_helper
 from .benchmark import data_root
 communicator = None
 _data_root = data_root
 _name = None
-__version__ = "v0.2.8"
+__version__ = "v0.2.8a"
 class VirtualCommunicator:
     """
     Communicator that simulates the communication phase between any two objects
     """
     def __init__(self, objects):
         self.objects_map = {obj.id:obj for obj in objects}
         self.objects = objects
```

### Comparing `flgo-0.2.8/src/flgo/algorithm/TiFL.py` & `flgo-0.2.8a0/src/flgo/algorithm/TiFL.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/afl.py` & `flgo-0.2.8a0/src/flgo/algorithm/afl.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/asyncbase.py` & `flgo-0.2.8a0/src/flgo/algorithm/asyncbase.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/clustered_sampling.py` & `flgo-0.2.8a0/src/flgo/algorithm/clustered_sampling.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/decentralized.py` & `flgo-0.2.8a0/src/flgo/algorithm/decentralized.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/ditto.py` & `flgo-0.2.8a0/src/flgo/algorithm/ditto.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/fedasync.py` & `flgo-0.2.8a0/src/flgo/algorithm/fedasync.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/fedavgm.py` & `flgo-0.2.8a0/src/flgo/algorithm/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/fedbase.py` & `flgo-0.2.8a0/src/flgo/algorithm/fedbase.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/fedbuff.py` & `flgo-0.2.8a0/src/flgo/algorithm/fedbuff.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/feddyn.py` & `flgo-0.2.8a0/src/flgo/algorithm/feddyn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/fedfa.py` & `flgo-0.2.8a0/src/flgo/algorithm/fedfa.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/fedfv.py` & `flgo-0.2.8a0/src/flgo/algorithm/fedfv.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/fedmf.py` & `flgo-0.2.8a0/src/flgo/algorithm/fedmf.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/fedmgda.py` & `flgo-0.2.8a0/src/flgo/algorithm/fedmgda.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/fednova.py` & `flgo-0.2.8a0/src/flgo/algorithm/fednova.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/fedprox.py` & `flgo-0.2.8a0/src/flgo/algorithm/fedprox.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/hierarchical.py` & `flgo-0.2.8a0/src/flgo/algorithm/hierarchical.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/mifa.py` & `flgo-0.2.8a0/src/flgo/algorithm/mifa.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/powerofchoice.py` & `flgo-0.2.8a0/src/flgo/algorithm/powerofchoice.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/qfedavg.py` & `flgo-0.2.8a0/src/flgo/algorithm/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/realbase.py` & `flgo-0.2.8a0/src/flgo/algorithm/realbase.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/scaffold.py` & `flgo-0.2.8a0/src/flgo/algorithm/scaffold.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/sesorec.py` & `flgo-0.2.8a0/src/flgo/algorithm/sesorec.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/standalone.py` & `flgo-0.2.8a0/src/flgo/algorithm/standalone.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/algorithm/vflbase.py` & `flgo-0.2.8a0/src/flgo/algorithm/vflbase.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/adult_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/adult_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/agnews_classification/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/agnews_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/agnews_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/agnews_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/bankmarketing_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/bankmarketing_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/base.py` & `flgo-0.2.8a0/src/flgo/benchmark/base.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/ciao_recommendation/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/ciao_recommendation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/ciao_recommendation/model/mf.py` & `flgo-0.2.8a0/src/flgo/benchmark/ciao_recommendation/model/mf.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar100_classification/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar100_classification/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar100_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar100_classification/model/cnn.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar100_classification/model/resnet18.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/model/resnet18.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar100_classification/model/resnet18_gn.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar100_classification/model/resnet18_gn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar10_classification/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar10_classification/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar10_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar10_classification/dataset.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar10_classification/model/cnn.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar10_classification/model/cnn_data_aug.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/model/cnn_data_aug.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar10_classification/model/mlp.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cifar10_classification/model/resnet18_gn.py` & `flgo-0.2.8a0/src/flgo/benchmark/cifar10_classification/model/resnet18_gn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/citeseer_link_prediction/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/citeseer_link_prediction/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/citeseer_link_prediction/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/citeseer_link_prediction/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/citeseer_link_prediction/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/citeseer_link_prediction/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/citeseer_node_classification/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/citeseer_node_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/citeseer_node_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/citeseer_node_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/coco_detection/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/coco_detection/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/coco_detection/model/FasterRCNN.py` & `flgo-0.2.8a0/src/flgo/benchmark/coco_detection/model/FasterRCNN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/coco_segmentation/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/coco_segmentation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/coco_segmentation/model/fcn_resnet50.py` & `flgo-0.2.8a0/src/flgo/benchmark/coco_segmentation/model/fcn_resnet50.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/coco_segmentation/model/unet.py` & `flgo-0.2.8a0/src/flgo/benchmark/coco_segmentation/model/unet.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cora_link_prediction/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/cora_link_prediction/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cora_link_prediction/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/cora_link_prediction/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cora_link_prediction/model/GCN.py` & `flgo-0.2.8a0/src/flgo/benchmark/cora_link_prediction/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cora_link_prediction/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/cora_link_prediction/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cora_node_classification/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cora_node_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cora_node_classification/model/GCN.py` & `flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py` & `flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/cora_node_classification/model/GraphSage.py` & `flgo-0.2.8a0/src/flgo/benchmark/cora_node_classification/model/GraphSage.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/crop_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/crop_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/crop_classification/model/cnn.py` & `flgo-0.2.8a0/src/flgo/benchmark/crop_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/distributed_quadratic_programming/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/distributed_quadratic_programming/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/distributed_quadratic_programming/model/vec.py` & `flgo-0.2.8a0/src/flgo/benchmark/distributed_quadratic_programming/model/vec.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/electricdevices_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/electricdevices_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/electricdevices_classification/model/cnn.py` & `flgo-0.2.8a0/src/flgo/benchmark/electricdevices_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/electricity_forecasting/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/electricity_forecasting/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/electricity_forecasting/model/GRU.py` & `flgo-0.2.8a0/src/flgo/benchmark/electricity_forecasting/model/GRU.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/emnist_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/emnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/emnist_classification/model/cnn.py` & `flgo-0.2.8a0/src/flgo/benchmark/emnist_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/emnist_classification/model/mlp.py` & `flgo-0.2.8a0/src/flgo/benchmark/emnist_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/enzymes_graph_classification/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/enzymes_graph_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/enzymes_graph_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/enzymes_graph_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/epinions_recommendation/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/epinions_recommendation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/epinions_recommendation/model/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/epinions_recommendation/model/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/epinions_recommendation/model/mf.py` & `flgo-0.2.8a0/src/flgo/benchmark/epinions_recommendation/model/mf.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/exchange_rate_forecasting/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/exchange_rate_forecasting/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/exchange_rate_forecasting/model/GRU.py` & `flgo-0.2.8a0/src/flgo/benchmark/exchange_rate_forecasting/model/GRU.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/fashion_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/fashion_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/fashion_classification/model/lr.py` & `flgo-0.2.8a0/src/flgo/benchmark/fashion_classification/model/lr.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/fcube_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/fcube_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/fcube_classification/model/lr.py` & `flgo-0.2.8a0/src/flgo/benchmark/fcube_classification/model/lr.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/femnist_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/femnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/femnist_classification/dataset.py` & `flgo-0.2.8a0/src/flgo/benchmark/femnist_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/femnist_classification/model/cnn.py` & `flgo-0.2.8a0/src/flgo/benchmark/femnist_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/heart_disease_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/heart_disease_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/imdb_classification/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/imdb_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/imdb_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/imdb_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/leaf_reddit/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/leaf_reddit/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py` & `flgo-0.2.8a0/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/leaf_sent140/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/leaf_sent140/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py` & `flgo-0.2.8a0/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/local_movielens_recommendation/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/local_movielens_recommendation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/local_movielens_recommendation/model/mf.py` & `flgo-0.2.8a0/src/flgo/benchmark/local_movielens_recommendation/model/mf.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/mnist_classification/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/mnist_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/mnist_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/mnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/mnist_classification/model/cnn.py` & `flgo-0.2.8a0/src/flgo/benchmark/mnist_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/mnist_classification/model/mlp.py` & `flgo-0.2.8a0/src/flgo/benchmark/mnist_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/movielens_recommendation/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/movielens_recommendation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/movielens_recommendation/model/mf.py` & `flgo-0.2.8a0/src/flgo/benchmark/movielens_recommendation/model/mf.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/multi30k_translation/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/multi30k_translation/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/multi30k_translation/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/multi30k_translation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/mutag_graph_classification/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/mutag_graph_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/mutag_graph_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/mutag_graph_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/nifECG_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/nifECG_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/nifECG_classification/model/cnn.py` & `flgo-0.2.8a0/src/flgo/benchmark/nifECG_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/oxfordiiitpet_segmentation/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/oxfordiiitpet_segmentation/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/oxfordiiitpet_segmentation/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/oxfordiiitpet_segmentation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/partition.py` & `flgo-0.2.8a0/src/flgo/benchmark/partition.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/penntreebank_modeling/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/penntreebank_modeling/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/penntreebank_modeling/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/penntreebank_modeling/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/pubmed_link_prediction/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/pubmed_link_prediction/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/pubmed_link_prediction/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/pubmed_link_prediction/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/pubmed_link_prediction/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/pubmed_link_prediction/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/pubmed_node_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/pubmed_node_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/pubmed_node_classification/model/GCN.py` & `flgo-0.2.8a0/src/flgo/benchmark/pubmed_node_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/sbdataset_segmentation/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/sbdataset_segmentation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/sbdataset_segmentation/model/fcn_resnet50.py` & `flgo-0.2.8a0/src/flgo/benchmark/sbdataset_segmentation/model/fcn_resnet50.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/sbdataset_segmentation/model/unet.py` & `flgo-0.2.8a0/src/flgo/benchmark/sbdataset_segmentation/model/unet.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/shakespeare_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/shakespeare_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py` & `flgo-0.2.8a0/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/social_splitted_ciao/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/social_splitted_ciao/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/social_splitted_ciaodvd/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/social_splitted_ciaodvd/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/social_splitted_douban/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/social_splitted_douban/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/social_splitted_epinions/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/social_splitted_epinions/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/social_splitted_filmtrust/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/social_splitted_filmtrust/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/sst2_classification/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/sst2_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/sst2_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/sst2_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/stl10_classification/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/stl10_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/stl10_classification/dataset.py` & `flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/stl10_classification/model/cnn.py` & `flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/stl10_classification/model/cnn_data_aug.py` & `flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/model/cnn_data_aug.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/stl10_classification/model/resnet18_gn.py` & `flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/model/resnet18_gn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/stl10_classification/model/resnet34_gn.py` & `flgo-0.2.8a0/src/flgo/benchmark/stl10_classification/model/resnet34_gn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/svhn_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/svhn_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/svhn_classification/model/cnn.py` & `flgo-0.2.8a0/src/flgo/benchmark/svhn_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/svhn_classification/model/mlp.py` & `flgo-0.2.8a0/src/flgo/benchmark/svhn_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/synthetic_regression/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/synthetic_regression/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/synthetic_regression/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/synthetic_regression/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/synthetic_regression/model/lr.py` & `flgo-0.2.8a0/src/flgo/benchmark/synthetic_regression/model/lr.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/dec_temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/dec_temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/hier_temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/hier_temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/classification/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/coco_eval.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/coco_eval.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/coco_utils.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/coco_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/presets.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/presets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/transforms.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/transforms.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/detection/utils.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/detection/utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/pointnet2_utils.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/pointnet2_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/pointnet_utils.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/pointnet_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet2_utils.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet2_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet_utils.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet2_utils.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet2_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet_utils.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/coco_utils.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/coco_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/presets.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/presets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/transforms.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/transforms.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/cv/segmentation/utils.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/cv/segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/general/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/general/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/general/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/general/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/graph/graph_classification/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/graph_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/graph/graph_classification/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/graph_classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/temp/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/temp/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/graph/node_classification/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/node_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/graph/node_classification/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/node_classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/classification/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/classification/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/classification/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/translation/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/translation/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/translation/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/nlp/translation/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/nlp/translation/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/partition.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/partition.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/rec/datasets.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/rec/datasets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/rec/rating_prediction/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/rec/rating_prediction/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/datasets.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/datasets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/series/classification/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/datasets.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/datasets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/temp/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/series/forecasting/temp/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/series/forecasting/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/tabular/classification/__init__.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/tabular/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/tabular/classification/datasets.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/tabular/classification/datasets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/toolkits/visualization.py` & `flgo-0.2.8a0/src/flgo/benchmark/toolkits/visualization.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/vertical_mnist_classification/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/vertical_mnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py` & `flgo-0.2.8a0/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/voc_detection/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/voc_detection/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/voc_detection/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/voc_detection/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/voc_detection/model/default_model.py` & `flgo-0.2.8a0/src/flgo/benchmark/voc_detection/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/wikitext2_modeling/config.py` & `flgo-0.2.8a0/src/flgo/benchmark/wikitext2_modeling/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/benchmark/wikitext2_modeling/core.py` & `flgo-0.2.8a0/src/flgo/benchmark/wikitext2_modeling/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/experiment/analyzer.py` & `flgo-0.2.8a0/src/flgo/experiment/analyzer.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/experiment/device_scheduler.py` & `flgo-0.2.8a0/src/flgo/experiment/device_scheduler.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/experiment/logger/__init__.py` & `flgo-0.2.8a0/src/flgo/experiment/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/experiment/logger/config.py` & `flgo-0.2.8a0/src/flgo/experiment/logger/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/experiment/logger/dec_logger.py` & `flgo-0.2.8a0/src/flgo/experiment/logger/dec_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/experiment/logger/full_logger.py` & `flgo-0.2.8a0/src/flgo/experiment/logger/full_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/experiment/logger/handlers.py` & `flgo-0.2.8a0/src/flgo/experiment/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/experiment/logger/pfl_logger.py` & `flgo-0.2.8a0/src/flgo/experiment/logger/pfl_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/experiment/logger/simple_logger.py` & `flgo-0.2.8a0/src/flgo/experiment/logger/simple_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/experiment/logger/tune_logger.py` & `flgo-0.2.8a0/src/flgo/experiment/logger/tune_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/experiment/logger/vertical_logger.py` & `flgo-0.2.8a0/src/flgo/experiment/logger/vertical_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/simulator/base.py` & `flgo-0.2.8a0/src/flgo/simulator/base.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/simulator/default_simulator.py` & `flgo-0.2.8a0/src/flgo/simulator/default_simulator.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/simulator/my_simulator.py` & `flgo-0.2.8a0/src/flgo/simulator/my_simulator.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/simulator/phone_simulator.py` & `flgo-0.2.8a0/src/flgo/simulator/phone_simulator.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/utils/__init__.py` & `flgo-0.2.8a0/src/flgo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/utils/fflow.py` & `flgo-0.2.8a0/src/flgo/utils/fflow.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo/utils/fmodule.py` & `flgo-0.2.8a0/src/flgo/utils/fmodule.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/src/flgo.egg-info/PKG-INFO` & `flgo-0.2.8a0/src/flgo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flgo
-Version: 0.2.8
+Version: 0.2.8a0
 Summary: A Research-oriented FL Platform. 
 Author-email: Zheng Wang <zwang@stu.xmu.edu.cn>
 Project-URL: Homepage, https://flgo-xmu.github.io
 Project-URL: Bug Tracker, https://github.com/WwZzz/easyFL/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flgo-0.2.8/src/flgo.egg-info/SOURCES.txt` & `flgo-0.2.8a0/src/flgo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flgo-0.2.8/tests/test.py` & `flgo-0.2.8a0/tests/test.py`

 * *Files identical despite different names*

