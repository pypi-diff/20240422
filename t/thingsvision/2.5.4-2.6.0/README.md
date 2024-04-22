# Comparing `tmp/thingsvision-2.5.4.tar.gz` & `tmp/thingsvision-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsvision-2.5.4.tar", last modified: Tue Apr 16 08:06:45 2024, max compression
+gzip compressed data, was "thingsvision-2.6.0.tar", last modified: Mon Apr 22 08:56:41 2024, max compression
```

## Comparing `thingsvision-2.5.4.tar` & `thingsvision-2.6.0.tar`

### file list

```diff
@@ -1,98 +1,101 @@
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.896856 thingsvision-2.5.4/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.5.4/LICENSE
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16350 2024-04-16 08:06:45.896520 thingsvision-2.5.4/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15747 2024-04-09 09:52:31.000000 thingsvision-2.5.4/README.md
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-04-16 08:06:45.896971 thingsvision-2.5.4/setup.cfg
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1747 2023-04-30 10:17:04.000000 thingsvision-2.5.4/setup.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.881827 thingsvision-2.5.4/tests/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.5.4/tests/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.882452 thingsvision-2.5.4/tests/extractor/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.4/tests/extractor/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.883501 thingsvision-2.5.4/tests/extractor/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.4/tests/extractor/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2024-04-06 10:03:37.000000 thingsvision-2.5.4/tests/extractor/extraction/test_custom_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.5.4/tests/extractor/extraction/test_model_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-06 10:03:24.000000 thingsvision-2.5.4/tests/extractor/extraction/test_pretrained_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-06 10:04:01.000000 thingsvision-2.5.4/tests/extractor/extraction/test_torch_vs_tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-01 11:29:46.000000 thingsvision-2.5.4/tests/extractor/test_load_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.5.4/tests/extractor/test_transformations.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11484 2024-04-08 11:02:58.000000 thingsvision-2.5.4/tests/helper.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.5.4/tests/test_features.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.5.4/tests/test_rest.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.884148 thingsvision-2.5.4/thingsvision/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.5.4/thingsvision/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-04-16 08:06:05.000000 thingsvision-2.5.4/thingsvision/_version.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.885660 thingsvision-2.5.4/thingsvision/core/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.5.4/thingsvision/core/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.886042 thingsvision-2.5.4/thingsvision/core/cka/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/core/cka/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/core/cka/base.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.887430 thingsvision-2.5.4/thingsvision/core/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-01 11:36:55.000000 thingsvision-2.5.4/thingsvision/core/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10749 2024-04-04 09:43:21.000000 thingsvision-2.5.4/thingsvision/core/extraction/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    17334 2024-04-08 11:02:58.000000 thingsvision-2.5.4/thingsvision/core/extraction/extractors.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8452 2024-04-04 09:43:21.000000 thingsvision-2.5.4/thingsvision/core/extraction/helpers.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.5.4/thingsvision/core/extraction/tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8530 2024-04-08 11:02:58.000000 thingsvision-2.5.4/thingsvision/core/extraction/torch.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.888128 thingsvision-2.5.4/thingsvision/core/rsa/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/core/rsa/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.5.4/thingsvision/core/rsa/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.5.4/thingsvision/core/rsa/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.890391 thingsvision-2.5.4/thingsvision/custom_models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.5.4/thingsvision/custom_models/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.5.4/thingsvision/custom_models/alexnet_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.5.4/thingsvision/custom_models/alexnet_salobjsub.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.891612 thingsvision-2.5.4/thingsvision/custom_models/cornet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/custom_models/cornet/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_r.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_rt.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_s.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_z.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.5.4/thingsvision/custom_models/custom.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.892058 thingsvision-2.5.4/thingsvision/custom_models/dreamsim/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.5.4/thingsvision/custom_models/dreamsim/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.5.4/thingsvision/custom_models/dreamsim/dreamsim.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.892474 thingsvision-2.5.4/thingsvision/custom_models/harmonization/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.5.4/thingsvision/custom_models/harmonization/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.5.4/thingsvision/custom_models/harmonization/harmonization.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.5.4/thingsvision/custom_models/inception_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.5.4/thingsvision/custom_models/official_clip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.5.4/thingsvision/custom_models/openclip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.5.4/thingsvision/custom_models/resnet50_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.5.4/thingsvision/custom_models/vgg16_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.5.4/thingsvision/custom_models/vgg16bn_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5992 2024-04-16 08:05:49.000000 thingsvision-2.5.4/thingsvision/thingsvision.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.892692 thingsvision-2.5.4/thingsvision/utils/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.5.4/thingsvision/utils/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.893068 thingsvision-2.5.4/thingsvision/utils/alignment/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.5.4/thingsvision/utils/alignment/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.5.4/thingsvision/utils/alignment/transforms.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.893280 thingsvision-2.5.4/thingsvision/utils/checkpointing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.5.4/thingsvision/utils/checkpointing/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.894135 thingsvision-2.5.4/thingsvision/utils/data/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.5.4/thingsvision/utils/data/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.5.4/thingsvision/utils/data/data_loader.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.5.4/thingsvision/utils/data/dataset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.5.4/thingsvision/utils/data/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.894352 thingsvision-2.5.4/thingsvision/utils/imagenet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/utils/imagenet/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.894565 thingsvision-2.5.4/thingsvision/utils/models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.5.4/thingsvision/utils/models/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.895148 thingsvision-2.5.4/thingsvision/utils/models/dino/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2024-04-05 17:27:52.000000 thingsvision-2.5.4/thingsvision/utils/models/dino/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.5.4/thingsvision/utils/models/dino/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.5.4/thingsvision/utils/models/dino/vision_transformer.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.895779 thingsvision-2.5.4/thingsvision/utils/models/mae/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      116 2024-04-08 11:02:58.000000 thingsvision-2.5.4/thingsvision/utils/models/mae/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2157 2024-04-08 11:02:58.000000 thingsvision-2.5.4/thingsvision/utils/models/mae/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2108 2024-04-08 11:02:58.000000 thingsvision-2.5.4/thingsvision/utils/models/mae/vit_mae.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.896203 thingsvision-2.5.4/thingsvision/utils/storing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.5.4/thingsvision/utils/storing/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.5.4/thingsvision/utils/storing/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-16 08:06:45.885451 thingsvision-2.5.4/thingsvision.egg-info/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16350 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2773 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/SOURCES.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/dependency_links.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/entry_points.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      332 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/requires.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-04-16 08:06:45.000000 thingsvision-2.5.4/thingsvision.egg-info/top_level.txt
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.588134 thingsvision-2.6.0/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.6.0/LICENSE
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16338 2024-04-22 08:56:41.587827 thingsvision-2.6.0/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15735 2024-04-22 08:56:16.000000 thingsvision-2.6.0/README.md
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-04-22 08:56:41.588221 thingsvision-2.6.0/setup.cfg
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1698 2024-04-22 08:56:16.000000 thingsvision-2.6.0/setup.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.554206 thingsvision-2.6.0/tests/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.6.0/tests/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.555307 thingsvision-2.6.0/tests/extractor/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.0/tests/extractor/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.557856 thingsvision-2.6.0/tests/extractor/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.0/tests/extractor/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2024-04-06 10:03:37.000000 thingsvision-2.6.0/tests/extractor/extraction/test_custom_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.6.0/tests/extractor/extraction/test_model_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-06 10:03:24.000000 thingsvision-2.6.0/tests/extractor/extraction/test_pretrained_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-06 10:04:01.000000 thingsvision-2.6.0/tests/extractor/extraction/test_torch_vs_tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-01 11:29:46.000000 thingsvision-2.6.0/tests/extractor/test_load_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.6.0/tests/extractor/test_transformations.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10966 2024-04-22 08:56:16.000000 thingsvision-2.6.0/tests/helper.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2024-04-22 08:56:16.000000 thingsvision-2.6.0/tests/test_features.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4368 2024-04-22 08:56:16.000000 thingsvision-2.6.0/tests/test_rest.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.559116 thingsvision-2.6.0/thingsvision/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.6.0/thingsvision/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-04-22 08:56:16.000000 thingsvision-2.6.0/thingsvision/_version.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.561208 thingsvision-2.6.0/thingsvision/core/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.6.0/thingsvision/core/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.562329 thingsvision-2.6.0/thingsvision/core/cka/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       29 2024-04-22 08:56:16.000000 thingsvision-2.6.0/thingsvision/core/cka/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2269 2024-04-22 08:56:16.000000 thingsvision-2.6.0/thingsvision/core/cka/cka_base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3567 2024-04-22 08:56:16.000000 thingsvision-2.6.0/thingsvision/core/cka/cka_numpy.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5433 2024-04-22 08:56:16.000000 thingsvision-2.6.0/thingsvision/core/cka/cka_torch.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      818 2024-04-22 08:56:16.000000 thingsvision-2.6.0/thingsvision/core/cka/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.565529 thingsvision-2.6.0/thingsvision/core/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-01 11:36:55.000000 thingsvision-2.6.0/thingsvision/core/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10749 2024-04-04 09:43:21.000000 thingsvision-2.6.0/thingsvision/core/extraction/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    17334 2024-04-08 11:02:58.000000 thingsvision-2.6.0/thingsvision/core/extraction/extractors.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8452 2024-04-04 09:43:21.000000 thingsvision-2.6.0/thingsvision/core/extraction/helpers.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.6.0/thingsvision/core/extraction/tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8530 2024-04-19 11:52:36.000000 thingsvision-2.6.0/thingsvision/core/extraction/torch.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.566480 thingsvision-2.6.0/thingsvision/core/rsa/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.6.0/thingsvision/core/rsa/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.6.0/thingsvision/core/rsa/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.6.0/thingsvision/core/rsa/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.572325 thingsvision-2.6.0/thingsvision/custom_models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.6.0/thingsvision/custom_models/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.6.0/thingsvision/custom_models/alexnet_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.6.0/thingsvision/custom_models/alexnet_salobjsub.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.574684 thingsvision-2.6.0/thingsvision/custom_models/cornet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.6.0/thingsvision/custom_models/cornet/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.6.0/thingsvision/custom_models/cornet/cornet_r.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.6.0/thingsvision/custom_models/cornet/cornet_rt.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.6.0/thingsvision/custom_models/cornet/cornet_s.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.6.0/thingsvision/custom_models/cornet/cornet_z.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.6.0/thingsvision/custom_models/custom.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.575792 thingsvision-2.6.0/thingsvision/custom_models/dreamsim/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.6.0/thingsvision/custom_models/dreamsim/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.6.0/thingsvision/custom_models/dreamsim/dreamsim.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.577535 thingsvision-2.6.0/thingsvision/custom_models/harmonization/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.6.0/thingsvision/custom_models/harmonization/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.6.0/thingsvision/custom_models/harmonization/harmonization.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.6.0/thingsvision/custom_models/inception_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.6.0/thingsvision/custom_models/official_clip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.6.0/thingsvision/custom_models/openclip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.6.0/thingsvision/custom_models/resnet50_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.6.0/thingsvision/custom_models/vgg16_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.6.0/thingsvision/custom_models/vgg16bn_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5992 2024-04-16 08:05:49.000000 thingsvision-2.6.0/thingsvision/thingsvision.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.578456 thingsvision-2.6.0/thingsvision/utils/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.6.0/thingsvision/utils/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.579347 thingsvision-2.6.0/thingsvision/utils/alignment/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.6.0/thingsvision/utils/alignment/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.6.0/thingsvision/utils/alignment/transforms.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.580068 thingsvision-2.6.0/thingsvision/utils/checkpointing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.6.0/thingsvision/utils/checkpointing/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.582309 thingsvision-2.6.0/thingsvision/utils/data/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.6.0/thingsvision/utils/data/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.6.0/thingsvision/utils/data/data_loader.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.6.0/thingsvision/utils/data/dataset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.6.0/thingsvision/utils/data/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.582969 thingsvision-2.6.0/thingsvision/utils/imagenet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.6.0/thingsvision/utils/imagenet/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.583397 thingsvision-2.6.0/thingsvision/utils/models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.6.0/thingsvision/utils/models/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.584916 thingsvision-2.6.0/thingsvision/utils/models/dino/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2024-04-05 17:27:52.000000 thingsvision-2.6.0/thingsvision/utils/models/dino/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.6.0/thingsvision/utils/models/dino/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.6.0/thingsvision/utils/models/dino/vision_transformer.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.586526 thingsvision-2.6.0/thingsvision/utils/models/mae/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      116 2024-04-08 11:02:58.000000 thingsvision-2.6.0/thingsvision/utils/models/mae/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2157 2024-04-08 11:02:58.000000 thingsvision-2.6.0/thingsvision/utils/models/mae/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2108 2024-04-08 11:02:58.000000 thingsvision-2.6.0/thingsvision/utils/models/mae/vit_mae.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.587445 thingsvision-2.6.0/thingsvision/utils/storing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.6.0/thingsvision/utils/storing/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2024-04-20 11:40:10.000000 thingsvision-2.6.0/thingsvision/utils/storing/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-22 08:56:41.560961 thingsvision-2.6.0/thingsvision.egg-info/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16338 2024-04-22 08:56:41.000000 thingsvision-2.6.0/thingsvision.egg-info/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2880 2024-04-22 08:56:41.000000 thingsvision-2.6.0/thingsvision.egg-info/SOURCES.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-04-22 08:56:41.000000 thingsvision-2.6.0/thingsvision.egg-info/dependency_links.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-04-22 08:56:41.000000 thingsvision-2.6.0/thingsvision.egg-info/entry_points.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      325 2024-04-22 08:56:41.000000 thingsvision-2.6.0/thingsvision.egg-info/requires.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-04-22 08:56:41.000000 thingsvision-2.6.0/thingsvision.egg-info/top_level.txt
```

### Comparing `thingsvision-2.5.4/LICENSE` & `thingsvision-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/PKG-INFO` & `thingsvision-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.5.4
+Version: 2.6.0
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -29,15 +29,15 @@
     <a href="https://pypi.org/project/thingsvision/" rel="nofollow">
         <img src="https://img.shields.io/pypi/v/thingsvision" alt="PyPI" />
     </a>
     <a href="https://pepy.tech/project/thingsvision">
         <img src="https://img.shields.io/pypi/dm/thingsvision" alt="downloads">
     </a>
     <a href="https://www.python.org/" rel="nofollow">
-        <img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg" alt="Python version" />
+        <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10-blue.svg" alt="Python version" />
     </a>
     <a href="https://github.com/ViCCo-Group/thingsvision/blob/master/LICENSE" rel="nofollow">
         <img src="https://img.shields.io/pypi/l/thingsvision" alt="License" />
     </a>
     <a href="https://github.com/psf/black" rel="nofollow">
         <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
     </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.5.4 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.6.0 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `thingsvision-2.5.4/README.md` & `thingsvision-2.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     <a href="https://pypi.org/project/thingsvision/" rel="nofollow">
         <img src="https://img.shields.io/pypi/v/thingsvision" alt="PyPI" />
     </a>
     <a href="https://pepy.tech/project/thingsvision">
         <img src="https://img.shields.io/pypi/dm/thingsvision" alt="downloads">
     </a>
     <a href="https://www.python.org/" rel="nofollow">
-        <img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg" alt="Python version" />
+        <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10-blue.svg" alt="Python version" />
     </a>
     <a href="https://github.com/ViCCo-Group/thingsvision/blob/master/LICENSE" rel="nofollow">
         <img src="https://img.shields.io/pypi/l/thingsvision" alt="License" />
     </a>
     <a href="https://github.com/psf/black" rel="nofollow">
         <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
     </a>
```

### Comparing `thingsvision-2.5.4/setup.py` & `thingsvision-2.6.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 
 # activate __version__ variable
 exec(open("thingsvision/_version.py").read())
 
 requirements = [
     "ftfy",
     "h5py",
-    # "keras-cv-attention-models>=1.3.5",
     "matplotlib",
     "numba",
     "numpy",
-    "open_clip_torch==2.0.*",
+    "open_clip_torch==2.24.*",
     "pandas",
     "regex",
     "scikit-image",
     "scikit-learn",
     "scipy",
     "tensorflow==2.9.* ; sys_platform != 'darwin' or platform_machine != 'arm64'",
     "tensorflow-macos==2.9.* ; sys_platform == 'darwin' and platform_machine == 'arm64'",
-    "timm==0.6.*",
-    "torch==1.13.*",
-    "torchvision==0.14.*",
+    "timm",
+    "torch>=2.0.0",
+    "torchvision==0.15.2",
     "torchtyping",
     "tqdm",
     "CLIP",
     # 'CLIP @ git+ssh://git@github.com/openai/CLIP@v1.0#egg=CLIP' # TODO: see issue #111
 ]
 
 setuptools.setup(
```

### Comparing `thingsvision-2.5.4/tests/extractor/extraction/test_custom_model.py` & `thingsvision-2.6.0/tests/extractor/extraction/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/tests/extractor/extraction/test_model_extractor.py` & `thingsvision-2.6.0/tests/extractor/extraction/test_model_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/tests/extractor/extraction/test_pretrained_model.py` & `thingsvision-2.6.0/tests/extractor/extraction/test_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/tests/extractor/extraction/test_torch_vs_tensorflow.py` & `thingsvision-2.6.0/tests/extractor/extraction/test_torch_vs_tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/tests/extractor/test_load_extractor.py` & `thingsvision-2.6.0/tests/extractor/test_load_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/tests/extractor/test_transformations.py` & `thingsvision-2.6.0/tests/extractor/test_transformations.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/tests/helper.py` & `thingsvision-2.6.0/tests/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import numpy as np
 import skimage
 import tensorflow as tf
 import torch
 import torch.nn as nn
 from tensorflow.keras.layers import Dense
 from tensorflow.keras.models import Sequential
-
 from thingsvision import get_extractor
 from thingsvision.utils.data import DataLoader, ImageDataset
 
 DATA_PATH = "./data"
 TEST_PATH = "./test_images"
 OUT_PATH = "./test"
 
@@ -115,32 +114,20 @@
     },
     "jigsaw-rn50": {
         "model_name": "jigsaw-rn50",
         "modules": ["avgpool"],
         "pretrained": True,
         "source": "ssl",
     },
-    "rotnet-rn50": {
-        "model_name": "rotnet-rn50",
-        "modules": ["avgpool"],
-        "pretrained": True,
-        "source": "ssl",
-    },
     "swav-rn50": {
         "model_name": "swav-rn50",
         "modules": ["avgpool"],
         "pretrained": True,
         "source": "ssl",
     },
-    "pirl-rn50": {
-        "model_name": "pirl-rn50",
-        "modules": ["avgpool"],
-        "pretrained": True,
-        "source": "ssl",
-    },
     "barlowtwins-rn50": {
         "model_name": "barlowtwins-rn50",
         "modules": ["avgpool"],
         "pretrained": True,
         "source": "ssl",
     },
     "dino-vit-tiny-p8": {
@@ -203,21 +190,14 @@
     "DreamSim_mlp_clip_vitb32": {
         "model_name": "DreamSim",
         "modules": ["model.mlp"],
         "pretrained": True,
         "source": "custom",
         "kwargs": {"variant": "clip_vitb32"},
     },
-    "DreamSim_mlp_open_clip_vitb32": {
-        "model_name": "DreamSim",
-        "modules": ["model.mlp"],
-        "pretrained": True,
-        "source": "custom",
-        "kwargs": {"variant": "open_clip_vitb32"},
-    },
     "DreamSim_mlp_dino_vitb16": {
         "model_name": "DreamSim",
         "modules": ["model.mlp"],
         "pretrained": True,
         "source": "custom",
         "kwargs": {"variant": "dino_vitb16"},
     },
```

### Comparing `thingsvision-2.5.4/tests/test_features.py` & `thingsvision-2.6.0/tests/test_features.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 import unittest
-import torch
 
 import numpy as np
+import torch
 from thingsvision.core.extraction import center_features, normalize_features
 from thingsvision.utils.storing import save_features, split_features
 
 import tests.helper as helper
 
 
 class FeaturesTestCase(unittest.TestCase):
```

### Comparing `thingsvision-2.5.4/tests/test_rest.py` & `thingsvision-2.6.0/tests/test_rest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 import unittest
 
 import numpy as np
+import torch
+from thingsvision.core.cka import get_cka
 from thingsvision.core.rsa import compute_rdm, correlate_rdms, plot_rdm
-from thingsvision.core.cka import CKA
 from thingsvision.utils.storing import save_features
 
 import tests.helper as helper
 
+
 class RSATestCase(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         helper.create_test_images()
         model_name = "vgg16"
         extractor, _, batches = helper.create_extractor_and_dataloader(
             model_name, pretrained=False, source="torchvision"
@@ -44,15 +46,14 @@
 
         for rdm_i, rdm_j in zip(rdms[:-1], rdms[1:]):
             corr = correlate_rdms(rdm_i, rdm_j)
             self.assertTrue(isinstance(corr, float))
             self.assertTrue(corr > float(-1) and corr < float(1))
 
 
-
 class CKATestCase(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         helper.create_test_images()
 
     def test_cka(self):
@@ -71,19 +72,36 @@
         )
         module_name = helper.MODEL_AND_MODULE_NAMES[model_name_j]["modules"][1]
         features_j = extractor.extract_features(
             batches=batches, module_name=module_name, flatten_acts=False
         )
         self.assertEqual(features_i.shape, features_j.shape)
         m = features_i.shape[0]
-        for kernel in ['linear', 'rbf']:
-            cka = CKA(m=m, kernel=kernel, sigma=0.5 if kernel == 'rbf' else None)
-            rho = cka.compare(features_i, features_j)
-            self.assertTrue(isinstance(rho, float))
-            self.assertTrue(rho > float(-1) and rho < float(1))
+        for backend in ["numpy", "torch"]:
+            if backend == "torch":
+                device = "cpu"
+                features_i = torch.from_numpy(features_i)
+                features_j = torch.from_numpy(features_j)
+            else:
+                device = None
+            for kernel in ["linear", "rbf"]:
+                sigma = 0.5 if kernel == "rbf" else None
+                for debiased in [True, False]:
+                    cka = get_cka(
+                        backend=backend,
+                        m=m,
+                        unbiased=debiased,
+                        kernel=kernel,
+                        sigma=sigma,
+                        device=device,
+                    )
+                    rho = cka.compare(features_i, features_j)
+                    if backend == "torch":
+                        rho = rho.item()
+                    self.assertTrue(rho > float(-1) and rho < float(1))
 
 
 class FileNamesTestCase(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         helper.create_test_images()
```

### Comparing `thingsvision-2.5.4/thingsvision/core/extraction/base.py` & `thingsvision-2.6.0/thingsvision/core/extraction/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/core/extraction/extractors.py` & `thingsvision-2.6.0/thingsvision/core/extraction/extractors.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/core/extraction/helpers.py` & `thingsvision-2.6.0/thingsvision/core/extraction/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/core/extraction/tensorflow.py` & `thingsvision-2.6.0/thingsvision/core/extraction/tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/core/extraction/torch.py` & `thingsvision-2.6.0/thingsvision/core/extraction/torch.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/core/rsa/helpers.py` & `thingsvision-2.6.0/thingsvision/core/rsa/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/alexnet_ecoset.py` & `thingsvision-2.6.0/thingsvision/custom_models/alexnet_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/alexnet_salobjsub.py` & `thingsvision-2.6.0/thingsvision/custom_models/alexnet_salobjsub.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/cornet/__init__.py` & `thingsvision-2.6.0/thingsvision/custom_models/cornet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_r.py` & `thingsvision-2.6.0/thingsvision/custom_models/cornet/cornet_r.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_rt.py` & `thingsvision-2.6.0/thingsvision/custom_models/cornet/cornet_rt.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_s.py` & `thingsvision-2.6.0/thingsvision/custom_models/cornet/cornet_s.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/cornet/cornet_z.py` & `thingsvision-2.6.0/thingsvision/custom_models/cornet/cornet_z.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/dreamsim/dreamsim.py` & `thingsvision-2.6.0/thingsvision/custom_models/dreamsim/dreamsim.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/harmonization/harmonization.py` & `thingsvision-2.6.0/thingsvision/custom_models/harmonization/harmonization.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/inception_ecoset.py` & `thingsvision-2.6.0/thingsvision/custom_models/inception_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/openclip.py` & `thingsvision-2.6.0/thingsvision/custom_models/openclip.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/resnet50_ecoset.py` & `thingsvision-2.6.0/thingsvision/custom_models/resnet50_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/vgg16_ecoset.py` & `thingsvision-2.6.0/thingsvision/custom_models/vgg16_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/custom_models/vgg16bn_ecoset.py` & `thingsvision-2.6.0/thingsvision/custom_models/vgg16bn_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/thingsvision.py` & `thingsvision-2.6.0/thingsvision/thingsvision.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/alignment/transforms.py` & `thingsvision-2.6.0/thingsvision/utils/alignment/transforms.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/checkpointing/__init__.py` & `thingsvision-2.6.0/thingsvision/utils/checkpointing/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/data/__init__.py` & `thingsvision-2.6.0/thingsvision/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/data/data_loader.py` & `thingsvision-2.6.0/thingsvision/utils/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/data/dataset.py` & `thingsvision-2.6.0/thingsvision/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/data/helpers.py` & `thingsvision-2.6.0/thingsvision/utils/data/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/imagenet/__init__.py` & `thingsvision-2.6.0/thingsvision/utils/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/models/dino/utils.py` & `thingsvision-2.6.0/thingsvision/utils/models/dino/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/models/dino/vision_transformer.py` & `thingsvision-2.6.0/thingsvision/utils/models/dino/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/models/mae/utils.py` & `thingsvision-2.6.0/thingsvision/utils/models/mae/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/models/mae/vit_mae.py` & `thingsvision-2.6.0/thingsvision/utils/models/mae/vit_mae.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision/utils/storing/helpers.py` & `thingsvision-2.6.0/thingsvision/utils/storing/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.4/thingsvision.egg-info/PKG-INFO` & `thingsvision-2.6.0/thingsvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.5.4
+Version: 2.6.0
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -29,15 +29,15 @@
     <a href="https://pypi.org/project/thingsvision/" rel="nofollow">
         <img src="https://img.shields.io/pypi/v/thingsvision" alt="PyPI" />
     </a>
     <a href="https://pepy.tech/project/thingsvision">
         <img src="https://img.shields.io/pypi/dm/thingsvision" alt="downloads">
     </a>
     <a href="https://www.python.org/" rel="nofollow">
-        <img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue.svg" alt="Python version" />
+        <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10-blue.svg" alt="Python version" />
     </a>
     <a href="https://github.com/ViCCo-Group/thingsvision/blob/master/LICENSE" rel="nofollow">
         <img src="https://img.shields.io/pypi/l/thingsvision" alt="License" />
     </a>
     <a href="https://github.com/psf/black" rel="nofollow">
         <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
     </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.5.4 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.6.0 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `thingsvision-2.5.4/thingsvision.egg-info/SOURCES.txt` & `thingsvision-2.6.0/thingsvision.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 thingsvision.egg-info/SOURCES.txt
 thingsvision.egg-info/dependency_links.txt
 thingsvision.egg-info/entry_points.txt
 thingsvision.egg-info/requires.txt
 thingsvision.egg-info/top_level.txt
 thingsvision/core/__init__.py
 thingsvision/core/cka/__init__.py
-thingsvision/core/cka/base.py
+thingsvision/core/cka/cka_base.py
+thingsvision/core/cka/cka_numpy.py
+thingsvision/core/cka/cka_torch.py
+thingsvision/core/cka/helpers.py
 thingsvision/core/extraction/__init__.py
 thingsvision/core/extraction/base.py
 thingsvision/core/extraction/extractors.py
 thingsvision/core/extraction/helpers.py
 thingsvision/core/extraction/tensorflow.py
 thingsvision/core/extraction/torch.py
 thingsvision/core/rsa/__init__.py
```

