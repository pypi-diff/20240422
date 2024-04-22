# Comparing `tmp/keras_nightly-3.3.0.dev2024042003.tar.gz` & `tmp/keras_nightly-3.3.0.dev2024042103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.3.0.dev2024042003.tar", last modified: Sat Apr 20 03:21:22 2024, max compression
+gzip compressed data, was "keras_nightly-3.3.0.dev2024042103.tar", last modified: Sun Apr 21 03:22:18 2024, max compression
```

## Comparing `keras_nightly-3.3.0.dev2024042003.tar` & `keras_nightly-3.3.0.dev2024042103.tar`

### file list

```diff
@@ -1,921 +1,921 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.711296 keras_nightly-3.3.0.dev2024042003/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-20 03:21:22.711296 keras_nightly-3.3.0.dev2024042003/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.583294 keras_nightly-3.3.0.dev2024042003/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.587295 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/activation_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/attention_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/base_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/conv_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/core_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/merge_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/normalization_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/pooling_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/regularization_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/reshaping_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/rnn_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.587295 keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/bert_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/image_classification_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.587295 keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.587295 keras_nightly-3.3.0.dev2024042003/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.587295 keras_nightly-3.3.0.dev2024042003/keras/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    30862 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/activations/activations_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.615295 keras_nightly-3.3.0.dev2024042003/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/applications_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/imagenet_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.619295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.619295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/backend_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/compute_output_spec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/dtypes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/global_state_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/keras_tensor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/name_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/stateless_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/variables_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.623295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/distribution_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    30577 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.627295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    27893 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.627295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/distribute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/name_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26461 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    77115 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/optimizer_distribute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/saved_model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.631295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24031 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    47135 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.631295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/backup_and_restore_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/csv_logger_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/early_stopping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/lambda_callback_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/learning_rate_scheduler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/model_checkpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/reduce_lr_on_plateau_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/remote_monitor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/swap_ema_weights_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    27236 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/tensorboard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/terminate_on_nan_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/constraints/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/constraints/constraints_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/distribution/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/distribution/distribution_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/dtype_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/dtype_policy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/export/export_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/export/export_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.643295 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/constant_initializers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/random_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/random_initializers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.643295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.643295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/activation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/elu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/leaky_relu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/prelu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/relu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/softmax_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.647295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/additive_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/grouped_query_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/multi_head_attention_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.651295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    32424 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27575 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv_transpose_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.651295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24999 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    26286 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/dense_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    41791 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    30544 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/einsum_dense_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    15413 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/identity_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/input_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/lambda_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/masking_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    63788 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/layer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.655295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/merging_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.655295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/batch_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/group_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/layer_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/spectral_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/unit_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/unit_normalization_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.659295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.667295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/audio_preprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/category_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/center_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/discretization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/feature_space_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashed_crossing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/index_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/integer_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_brightness_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_contrast_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_flip_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_rotation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_translation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_zoom_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/rescaling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/resizing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/string_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/text_vectorization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.667295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/activity_regularization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/alpha_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_noise_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/spatial_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/spatial_dropout_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.671296 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/flatten_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/permute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/repeat_vector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/reshape_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding3d_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.675295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/bidirectional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/dropout_rnn_cell_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/gru_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/lstm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/rnn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/simple_rnn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/stacked_rnn_cells_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/time_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/time_distributed_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.679295 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.679295 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.679295 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/json_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/legacy_h5_format_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.679295 keras_nightly-3.3.0.dev2024042003/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/losses/loss_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/losses/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/losses/losses_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.683296 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/accuracy_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    63267 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/confusion_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/f_score_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/hinge_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/iou_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metric_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/probabilistic_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/reduction_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/regression_metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.687296 keras_nightly-3.3.0.dev2024042003/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/cloning_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/functional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    24695 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/sequential_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/variable_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/variable_mapping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.691295 keras_nightly-3.3.0.dev2024042003/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    31327 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/core_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/function_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    37256 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    31485 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    19959 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/linalg_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    47868 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/math_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    62113 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    81862 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/nn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   193387 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)   283774 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/numpy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/symbolic_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/symbolic_arguments_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.695296 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adadelta_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adafactor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adagrad_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamax_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    40410 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/ftrl_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/lion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/loss_scale_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/nadam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer_sparse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/rmsprop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.695296 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15392 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/learning_rate_schedule_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/sgd_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.695296 keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/quantizers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.695296 keras_nightly-3.3.0.dev2024042003/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/random/random_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/random/seed_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/random/seed_generator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.699296 keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/regularizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/regularizers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.699296 keras_nightly-3.3.0.dev2024042003/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/object_registration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_api_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    33448 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/serialization_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/serialization_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.699296 keras_nightly-3.3.0.dev2024042003/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.699296 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/compile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/compile_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.703296 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_data_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/generator_data_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/epoch_iterator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    51439 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.703296 keras_nightly-3.3.0.dev2024042003/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/tree/tree_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/tree/tree_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.711296 keras_nightly-3.3.0.dev2024042003/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/audio_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/code_stats_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/dtype_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28322 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/file_utils_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20039 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/io_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23050 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/jax_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/naming_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/numerical_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/python_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/rng_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/sequence_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/summary_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/text_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/timeseries_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/torch_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/tracking_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-20 03:21:20.000000 keras_nightly-3.3.0.dev2024042003/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.711296 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-20 03:21:22.000000 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-04-20 03:21:22.000000 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:21:22.000000 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 03:21:22.000000 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 03:21:22.000000 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-20 03:21:22.715296 keras_nightly-3.3.0.dev2024042003/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-20 03:21:20.000000 keras_nightly-3.3.0.dev2024042003/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.069030 keras_nightly-3.3.0.dev2024042103/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-21 03:22:18.069030 keras_nightly-3.3.0.dev2024042103/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.929031 keras_nightly-3.3.0.dev2024042103/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.929031 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/activation_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/attention_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/base_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/conv_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/core_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/merge_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/normalization_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/pooling_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/regularization_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/reshaping_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/rnn_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/benchmarks/model_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/model_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/model_benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/model_benchmark/bert_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/model_benchmark/image_classification_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/benchmarks/torch_ctl_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/torch_ctl_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/torch_ctl_benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.933031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.937031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.941031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.945031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.949031 keras_nightly-3.3.0.dev2024042103/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.953031 keras_nightly-3.3.0.dev2024042103/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.957031 keras_nightly-3.3.0.dev2024042103/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.957031 keras_nightly-3.3.0.dev2024042103/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.957031 keras_nightly-3.3.0.dev2024042103/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.957031 keras_nightly-3.3.0.dev2024042103/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.957031 keras_nightly-3.3.0.dev2024042103/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30862 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/activations/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.961031 keras_nightly-3.3.0.dev2024042103/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/applications_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/imagenet_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.961031 keras_nightly-3.3.0.dev2024042103/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.965031 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/backend_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/compute_output_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/dtypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/global_state_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/keras_tensor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/name_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/stateless_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/variables_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.969031 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/distribution_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26120 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30709 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.969031 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18006 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28024 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.973031 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/distribute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/name_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26595 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77416 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/optimizer_distribute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/saved_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.977031 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47357 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.977031 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.985031 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/backup_and_restore_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/callback_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/csv_logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/early_stopping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/lambda_callback_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/learning_rate_scheduler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/model_checkpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/reduce_lr_on_plateau_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/remote_monitor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/swap_ema_weights_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27236 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/tensorboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/terminate_on_nan_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.985031 keras_nightly-3.3.0.dev2024042103/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/constraints/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/constraints/constraints_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.985031 keras_nightly-3.3.0.dev2024042103/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.985031 keras_nightly-3.3.0.dev2024042103/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/distribution/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/distribution/distribution_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.989031 keras_nightly-3.3.0.dev2024042103/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/dtype_policies/dtype_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/dtype_policies/dtype_policy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.989031 keras_nightly-3.3.0.dev2024042103/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/export/export_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/export/export_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.989031 keras_nightly-3.3.0.dev2024042103/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/initializers/constant_initializers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/initializers/random_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/initializers/random_initializers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.989031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.993031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/activation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/elu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/leaky_relu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/prelu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/relu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/softmax_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.993031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/additive_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/grouped_query_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/multi_head_attention_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:17.997031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32424 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27575 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv_transpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/depthwise_conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/separable_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/separable_conv_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.001031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24999 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26286 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41835 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31411 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/einsum_dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15413 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/identity_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/input_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/lambda_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/masking_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63788 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/layer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.005031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/merging_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.005031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/batch_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/group_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/layer_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/spectral_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/unit_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/unit_normalization_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.009031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/average_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_average_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_max_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/max_pooling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.017031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/audio_preprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/category_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/center_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/discretization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/feature_space_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/hashed_crossing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/hashing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/index_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/integer_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_brightness_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_contrast_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_flip_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_rotation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_translation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_zoom_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/rescaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/resizing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/string_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/text_vectorization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.021031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/activity_regularization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/alpha_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/gaussian_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/gaussian_noise_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/spatial_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/spatial_dropout_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.025031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/flatten_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/permute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/repeat_vector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/reshape_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding3d_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.029031 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/bidirectional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/dropout_rnn_cell_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/gru_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/lstm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/rnn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/simple_rnn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/stacked_rnn_cells_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/time_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/time_distributed_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.033031 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.033031 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.033031 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/json_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/legacy_h5_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.037031 keras_nightly-3.3.0.dev2024042103/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/losses/loss_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/losses/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/losses/losses_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.041031 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/accuracy_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63267 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/confusion_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/f_score_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/hinge_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/iou_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/metric_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/probabilistic_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/reduction_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/metrics/regression_metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.041031 keras_nightly-3.3.0.dev2024042103/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/models/cloning_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/models/functional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24695 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/models/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/models/sequential_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/models/variable_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/models/variable_mapping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.045030 keras_nightly-3.3.0.dev2024042103/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31327 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/function_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37256 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31485 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19959 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/linalg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47868 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/math_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64046 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83662 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/nn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   194898 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   284656 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/numpy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/operation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/operation_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/symbolic_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/ops/symbolic_arguments_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.053031 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adadelta_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adafactor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adagrad_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adamax_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adamw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40410 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/ftrl_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/lion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/loss_scale_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/nadam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/optimizer_sparse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/rmsprop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.053031 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15392 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/schedules/learning_rate_schedule_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/sgd_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.053031 keras_nightly-3.3.0.dev2024042103/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/quantizers/quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/quantizers/quantizers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.053031 keras_nightly-3.3.0.dev2024042103/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/random/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/random/seed_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/random/seed_generator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.053031 keras_nightly-3.3.0.dev2024042103/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/regularizers/regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/regularizers/regularizers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.053031 keras_nightly-3.3.0.dev2024042103/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/saving/object_registration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/saving/saving_api_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33448 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/saving/saving_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/saving/serialization_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/saving/serialization_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.057031 keras_nightly-3.3.0.dev2024042103/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/testing/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/testing/test_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.057031 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/compile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/compile_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.061030 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/array_data_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/generator_data_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/epoch_iterator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51439 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/trainers/trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.061030 keras_nightly-3.3.0.dev2024042103/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/tree/tree_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/tree/tree_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.069030 keras_nightly-3.3.0.dev2024042103/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/audio_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/code_stats_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/dtype_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28322 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/file_utils_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20039 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/image_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/io_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23050 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/jax_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/naming_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/numerical_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/python_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/rng_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/sequence_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/summary_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/text_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/timeseries_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/torch_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/keras/src/utils/tracking_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-21 03:22:14.000000 keras_nightly-3.3.0.dev2024042103/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:22:18.069030 keras_nightly-3.3.0.dev2024042103/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-21 03:22:17.000000 keras_nightly-3.3.0.dev2024042103/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-04-21 03:22:17.000000 keras_nightly-3.3.0.dev2024042103/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 03:22:17.000000 keras_nightly-3.3.0.dev2024042103/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-21 03:22:17.000000 keras_nightly-3.3.0.dev2024042103/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 03:22:17.000000 keras_nightly-3.3.0.dev2024042103/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-21 03:20:53.000000 keras_nightly-3.3.0.dev2024042103/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 03:22:18.069030 keras_nightly-3.3.0.dev2024042103/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-21 03:22:14.000000 keras_nightly-3.3.0.dev2024042103/setup.py
```

### Comparing `keras_nightly-3.3.0.dev2024042003/LICENSE` & `keras_nightly-3.3.0.dev2024042103/LICENSE`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/PKG-INFO` & `keras_nightly-3.3.0.dev2024042103/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.0.dev2024042003
+Version: 3.3.0.dev2024042103
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.0.dev2024042003/README.md` & `keras_nightly-3.3.0.dev2024042103/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/activation_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/activation_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/attention_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/attention_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/base_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/base_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/conv_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/conv_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/core_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/core_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/merge_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/merge_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/normalization_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/normalization_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/pooling_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/pooling_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/regularization_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/regularization_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/reshaping_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/reshaping_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/rnn_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/layer_benchmark/rnn_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/benchmark_utils.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/model_benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/bert_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/model_benchmark/bert_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/image_classification_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/model_benchmark/image_classification_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/benchmark_utils.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/torch_ctl_benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py` & `keras_nightly-3.3.0.dev2024042103/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from keras.src.ops.math import top_k
 from keras.src.ops.nn import average_pool
 from keras.src.ops.nn import batch_normalization
 from keras.src.ops.nn import binary_crossentropy
 from keras.src.ops.nn import categorical_crossentropy
 from keras.src.ops.nn import conv
 from keras.src.ops.nn import conv_transpose
+from keras.src.ops.nn import ctc_decode
 from keras.src.ops.nn import ctc_loss
 from keras.src.ops.nn import depthwise_conv
 from keras.src.ops.nn import elu
 from keras.src.ops.nn import gelu
 from keras.src.ops.nn import hard_sigmoid
 from keras.src.ops.nn import hard_silu
 from keras.src.ops.nn import hard_silu as hard_swish
@@ -215,11 +216,12 @@
 from keras.src.ops.numpy import transpose
 from keras.src.ops.numpy import tri
 from keras.src.ops.numpy import tril
 from keras.src.ops.numpy import triu
 from keras.src.ops.numpy import true_divide
 from keras.src.ops.numpy import var
 from keras.src.ops.numpy import vdot
+from keras.src.ops.numpy import vectorize
 from keras.src.ops.numpy import vstack
 from keras.src.ops.numpy import where
 from keras.src.ops.numpy import zeros
 from keras.src.ops.numpy import zeros_like
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/nn/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from keras.src.ops.nn import average_pool
 from keras.src.ops.nn import batch_normalization
 from keras.src.ops.nn import binary_crossentropy
 from keras.src.ops.nn import categorical_crossentropy
 from keras.src.ops.nn import conv
 from keras.src.ops.nn import conv_transpose
+from keras.src.ops.nn import ctc_decode
 from keras.src.ops.nn import ctc_loss
 from keras.src.ops.nn import depthwise_conv
 from keras.src.ops.nn import elu
 from keras.src.ops.nn import gelu
 from keras.src.ops.nn import hard_sigmoid
 from keras.src.ops.nn import hard_silu
 from keras.src.ops.nn import hard_silu as hard_swish
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,11 +137,12 @@
 from keras.src.ops.numpy import transpose
 from keras.src.ops.numpy import tri
 from keras.src.ops.numpy import tril
 from keras.src.ops.numpy import triu
 from keras.src.ops.numpy import true_divide
 from keras.src.ops.numpy import var
 from keras.src.ops.numpy import vdot
+from keras.src.ops.numpy import vectorize
 from keras.src.ops.numpy import vstack
 from keras.src.ops.numpy import where
 from keras.src.ops.numpy import zeros
 from keras.src.ops.numpy import zeros_like
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/activations/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/applications/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/applications/convnext/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/backend/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/config/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/layers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/losses/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/mixed_precision/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/ops/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/ops/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from keras.src.ops.math import top_k
 from keras.src.ops.nn import average_pool
 from keras.src.ops.nn import batch_normalization
 from keras.src.ops.nn import binary_crossentropy
 from keras.src.ops.nn import categorical_crossentropy
 from keras.src.ops.nn import conv
 from keras.src.ops.nn import conv_transpose
+from keras.src.ops.nn import ctc_decode
 from keras.src.ops.nn import ctc_loss
 from keras.src.ops.nn import depthwise_conv
 from keras.src.ops.nn import elu
 from keras.src.ops.nn import gelu
 from keras.src.ops.nn import hard_sigmoid
 from keras.src.ops.nn import hard_silu
 from keras.src.ops.nn import hard_silu as hard_swish
@@ -215,11 +216,12 @@
 from keras.src.ops.numpy import transpose
 from keras.src.ops.numpy import tri
 from keras.src.ops.numpy import tril
 from keras.src.ops.numpy import triu
 from keras.src.ops.numpy import true_divide
 from keras.src.ops.numpy import var
 from keras.src.ops.numpy import vdot
+from keras.src.ops.numpy import vectorize
 from keras.src.ops.numpy import vstack
 from keras.src.ops.numpy import where
 from keras.src.ops.numpy import zeros
 from keras.src.ops.numpy import zeros_like
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/ops/linalg/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/ops/nn/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/ops/nn/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from keras.src.ops.nn import average_pool
 from keras.src.ops.nn import batch_normalization
 from keras.src.ops.nn import binary_crossentropy
 from keras.src.ops.nn import categorical_crossentropy
 from keras.src.ops.nn import conv
 from keras.src.ops.nn import conv_transpose
+from keras.src.ops.nn import ctc_decode
 from keras.src.ops.nn import ctc_loss
 from keras.src.ops.nn import depthwise_conv
 from keras.src.ops.nn import elu
 from keras.src.ops.nn import gelu
 from keras.src.ops.nn import hard_sigmoid
 from keras.src.ops.nn import hard_silu
 from keras.src.ops.nn import hard_silu as hard_swish
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/ops/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/ops/numpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,11 +137,12 @@
 from keras.src.ops.numpy import transpose
 from keras.src.ops.numpy import tri
 from keras.src.ops.numpy import tril
 from keras.src.ops.numpy import triu
 from keras.src.ops.numpy import true_divide
 from keras.src.ops.numpy import var
 from keras.src.ops.numpy import vdot
+from keras.src.ops.numpy import vectorize
 from keras.src.ops.numpy import vstack
 from keras.src.ops.numpy import where
 from keras.src.ops.numpy import zeros
 from keras.src.ops.numpy import zeros_like
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/legacy/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/random/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/saving/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/tree/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/api/utils/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/activations/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/activations/activations.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/activations/activations_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/activations/activations_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/api_export.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/applications_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/applications_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/convnext.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/densenet.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/efficientnet.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/imagenet_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/imagenet_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/inception_v3.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/nasnet.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/resnet.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/resnet_v2.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/vgg16.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/vgg19.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/applications/xception.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/backend_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/backend_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/compute_output_spec_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/compute_output_spec_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/dtypes.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/dtypes_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/dtypes_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/global_state.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/keras_tensor_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/keras_tensor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/name_scope.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/name_scope_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/name_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/stateless_scope_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/stateless_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/variables.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/variables_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/common/variables_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/config.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/exports.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/core.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/distribution_lib_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/distribution_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/image.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/linalg.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/math.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/nn.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/nn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,102 +1,134 @@
 import jax
-import jax.experimental.sparse as jax_sparse
-import jax.numpy as jnp
 import numpy as np
 from jax import lax
-from jax import nn as jnn
+from jax import numpy as jnp
 
 from keras.src.backend import standardize_data_format
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common.backend_utils import (
     compute_conv_transpose_padding_args_for_jax,
 )
 from keras.src.backend.config import epsilon
-from keras.src.backend.jax.core import cast
-from keras.src.backend.jax.core import convert_to_tensor
+from keras.src.backend.numpy.core import cast
+from keras.src.backend.numpy.core import convert_to_tensor
+from keras.src.backend.numpy.core import is_tensor
+from keras.src.utils.module_utils import scipy
 
 
 def relu(x):
     x = convert_to_tensor(x)
-    return jnn.relu(x)
+    return np.maximum(x, np.array(0.0, x.dtype))
 
 
 def relu6(x):
     x = convert_to_tensor(x)
-    return jnn.relu6(x)
+    # np.clip incorrectly promote bfloat16 to float32, so we replace it with
+    # np.minimum and np.maximum here
+    return np.minimum(
+        np.maximum(x, np.array(0.0, x.dtype)), np.array(6.0, x.dtype)
+    )
 
 
 def sigmoid(x):
     x = convert_to_tensor(x)
-    return jnn.sigmoid(x)
+    return np.array(1.0, x.dtype) / (np.array(1.0, x.dtype) + np.exp(-x))
 
 
 def tanh(x):
-    x = convert_to_tensor(x)
-    return jnn.tanh(x)
+    return np.tanh(x)
 
 
 def softplus(x):
     x = convert_to_tensor(x)
-    return jnn.softplus(x)
+    return np.logaddexp(x, np.array(0.0, x.dtype))
 
 
 def softsign(x):
     x = convert_to_tensor(x)
-    return jnn.soft_sign(x)
+    return x / (np.array(1.0, x.dtype) + np.abs(x))
 
 
 def silu(x):
     x = convert_to_tensor(x)
-    return jnn.silu(x)
+    return x * sigmoid(x)
 
 
 def log_sigmoid(x):
     x = convert_to_tensor(x)
-    return jnn.log_sigmoid(x)
+    return -softplus(-x)
 
 
 def leaky_relu(x, negative_slope=0.2):
     x = convert_to_tensor(x)
-    return jnn.leaky_relu(x, negative_slope=negative_slope)
+    return np.maximum(x, np.array(negative_slope, x.dtype) * x)
 
 
 def hard_sigmoid(x):
-    x = convert_to_tensor(x)
-    return jnn.hard_sigmoid(x)
+    # python numbers will be promoted to float64 by np, so it's necessary to
+    # first convert the python numbers to np scalars
+    x = x / np.array(6.0, x.dtype) + np.array(0.5, x.dtype)
+    return np.where(
+        x <= 0.0,
+        np.array(0.0, x.dtype),
+        np.where(x >= 1.0, np.array(1.0, x.dtype), x),
+    )
 
 
 def hard_silu(x):
-    x = convert_to_tensor(x)
-    return jnn.hard_silu(x)
+    return x * hard_sigmoid(x)
 
 
 def elu(x, alpha=1.0):
     x = convert_to_tensor(x)
-    return jnn.elu(x, alpha=alpha)
+    return np.where(
+        x >= np.array(0.0, x.dtype), x, np.array(alpha, x.dtype) * np.expm1(x)
+    )
 
 
-def selu(x):
+def selu(
+    x,
+    alpha=1.6732632423543772848170429916717,
+    scale=1.0507009873554804934193349852946,
+):
     x = convert_to_tensor(x)
-    return jnn.selu(x)
+    return np.array(scale, x.dtype) * elu(x, alpha)
 
 
 def gelu(x, approximate=True):
     x = convert_to_tensor(x)
-    return jnn.gelu(x, approximate)
+    # followed by JAX's implementation
+    if approximate:
+        sqrt_2_over_pi = np.sqrt(2 / np.pi).astype(x.dtype)
+        cdf = np.array(0.5, x.dtype) * (
+            np.array(1.0, x.dtype)
+            + np.tanh(
+                sqrt_2_over_pi
+                * (x + np.array(0.044715, x.dtype) * (x**3).astype(x.dtype))
+            )
+        )
+        return x * cdf
+    else:
+        sqrt_2 = np.sqrt(2).astype(x.dtype)
+        return (
+            x
+            * (scipy.special.erf(x / sqrt_2) + 1).astype(x.dtype)
+            / np.array(2, x.dtype)
+        )
 
 
-def softmax(x, axis=-1):
-    x = convert_to_tensor(x)
-    return jnn.softmax(x, axis=axis)
+def softmax(x, axis=None):
+    exp_x = np.exp(x - np.max(x, axis=axis, keepdims=True))
+    return exp_x / np.sum(exp_x, axis=axis, keepdims=True)
 
 
-def log_softmax(x, axis=-1):
-    x = convert_to_tensor(x)
-    return jnn.log_softmax(x, axis=axis)
+def log_softmax(x, axis=None):
+    max_x = np.max(x, axis=axis, keepdims=True)
+    logsumexp = np.log(np.exp(x - max_x).sum(axis=axis, keepdims=True))
+    return x - max_x - logsumexp
 
 
 def _convert_to_spatial_operand(
     x,
     num_spatial_dims,
     data_format="channels_last",
     include_batch_and_channels=True,
@@ -136,21 +168,23 @@
         The output of the reduction for each window slice.
     """
     if padding not in ("same", "valid"):
         raise ValueError(
             f"Invalid padding '{padding}', must be 'same' or 'valid'."
         )
     padding = padding.upper()
-    return lax.reduce_window(
-        inputs,
-        initial_value,
-        reduce_fn,
-        pool_size,
-        strides,
-        padding,
+    return np.array(
+        lax.reduce_window(
+            inputs,
+            initial_value,
+            reduce_fn,
+            pool_size,
+            strides,
+            padding,
+        )
     )
 
 
 def max_pool(
     inputs,
     pool_size,
     strides=None,
@@ -269,22 +303,24 @@
     if channels % kernel_in_channels > 0:
         raise ValueError(
             "The number of input channels must be evenly divisible by "
             f"kernel's in_channels. Received input channels {channels} and "
             f"kernel in_channels {kernel_in_channels}. "
         )
     feature_group_count = channels // kernel_in_channels
-    return jax.lax.conv_general_dilated(
-        convert_to_tensor(inputs),
-        convert_to_tensor(kernel),
-        strides,
-        padding,
-        rhs_dilation=dilation_rate,
-        dimension_numbers=dimension_numbers,
-        feature_group_count=feature_group_count,
+    return np.array(
+        jax.lax.conv_general_dilated(
+            inputs,
+            kernel if is_tensor(kernel) else kernel.numpy(),
+            strides,
+            padding,
+            rhs_dilation=dilation_rate,
+            dimension_numbers=dimension_numbers,
+            feature_group_count=feature_group_count,
+        )
     )
 
 
 def depthwise_conv(
     inputs,
     kernel,
     strides=1,
@@ -311,25 +347,27 @@
         data_format,
         include_batch_and_channels=False,
     )
     feature_group_count = (
         inputs.shape[-1] if data_format == "channels_last" else inputs.shape[1]
     )
     kernel = jnp.reshape(
-        kernel,
+        kernel if is_tensor(kernel) else kernel.numpy(),
         kernel.shape[:-2] + (1, feature_group_count * kernel.shape[-1]),
     )
-    return jax.lax.conv_general_dilated(
-        inputs,
-        kernel,
-        strides,
-        padding,
-        rhs_dilation=dilation_rate,
-        dimension_numbers=dimension_numbers,
-        feature_group_count=feature_group_count,
+    return np.array(
+        jax.lax.conv_general_dilated(
+            inputs,
+            kernel,
+            strides,
+            padding,
+            rhs_dilation=dilation_rate,
+            dimension_numbers=dimension_numbers,
+            feature_group_count=feature_group_count,
+        )
     )
 
 
 def separable_conv(
     inputs,
     depthwise_kernel,
     pointwise_kernel,
@@ -390,79 +428,72 @@
     dilation_rate = _convert_to_spatial_operand(
         dilation_rate,
         num_spatial_dims,
         data_format,
         include_batch_and_channels=False,
     )
 
-    return jax.lax.conv_transpose(
-        inputs,
-        kernel,
-        strides,
-        padding=padding_values,
-        rhs_dilation=dilation_rate,
-        dimension_numbers=dimension_numbers,
-        transpose_kernel=True,
+    return np.array(
+        jax.lax.conv_transpose(
+            inputs,
+            kernel if is_tensor(kernel) else kernel.numpy(),
+            strides,
+            padding=padding_values,
+            rhs_dilation=dilation_rate,
+            dimension_numbers=dimension_numbers,
+            transpose_kernel=True,
+        )
     )
 
 
 def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
-    x = convert_to_tensor(x)
     if sparse:
-        if axis < 0:
-            axis = axis + len(x.shape) + 1
-        if dtype is None:
-            dtype = "float32"
-        # We deal with negative inputs by having zeros in the output although
-        # it's useless. It makes shapes static.
-        values = jnp.greater_equal(jnp.ravel(x), 0).astype(dtype)
-        values_count = values.shape[0]
-        indices = [jnp.arange(dim) for dim in x.shape]
-        indices = jnp.meshgrid(*indices, indexing="ij")
-        indices.insert(axis, jnp.maximum(x, 0))  # Deal with negative indices
-        indices = [a.reshape(values_count, 1).astype("int32") for a in indices]
-        indices = jnp.concatenate(indices, axis=1)
-        shape = list(x.shape)
-        shape.insert(axis, num_classes)
-        shape = tuple(shape)
-        return jax_sparse.BCOO(
-            (values, indices),
-            shape=shape,
-            indices_sorted=True,
-            unique_indices=True,
-        )
-    return jnn.one_hot(x, num_classes, axis=axis, dtype=dtype)
+        raise ValueError("Unsupported value `sparse=True` with numpy backend")
+    x = convert_to_tensor(x)
+    input_shape = x.shape
+
+    # Shrink the last dimension if the shape is (..., 1).
+    if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
+        input_shape = tuple(input_shape[:-1])
+
+    x = x.reshape(-1)
+    if not num_classes:
+        num_classes = np.max(x) + 1
+
+    batch_size = x.shape[0]
+    categorical = np.zeros((batch_size, num_classes), dtype=dtype)
+    valid_indices = x >= 0
+    categorical[np.arange(batch_size)[valid_indices], x[valid_indices]] = 1
+
+    # First, reshape the array with the extra dimension at the end
+    output_shape = input_shape + (num_classes,)
+    categorical = np.reshape(categorical, output_shape)
+
+    # Then, move this new dimension to the right place (according to axis)
+    if axis != -1:
+        categorical = np.moveaxis(categorical, -1, axis)
+
+    return categorical
 
 
 def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
+    if sparse:
+        raise ValueError("Unsupported value `sparse=True` with numpy backend")
     x = convert_to_tensor(x)
     reduction_axis = 1 if len(x.shape) > 1 else 0
-    if sparse:
-        result = one_hot(
-            x, num_classes, axis=axis, dtype="int32", sparse=sparse
-        )
-        # JAX's BCOO does not support max reduction, use sum and compare with 0.
-        result = jax_sparse.bcoo_reduce_sum(result, axes=(reduction_axis,))
-        result = jax_sparse.bcoo_sum_duplicates(result)
-        values = jnp.greater_equal(result.data, 0).astype(dtype)
-        return jax_sparse.BCOO(
-            (values, result.indices),
-            shape=result.shape,
-            indices_sorted=True,
-            unique_indices=True,
-        )
-    return jnp.max(
+    outputs = np.max(
         one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
         axis=reduction_axis,
     )
+    return outputs
 
 
 def categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = jnp.array(target)
-    output = jnp.array(output)
+    target = np.array(target)
+    output = np.array(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
@@ -470,192 +501,131 @@
         raise ValueError(
             "Arguments `target` and `output` must be at least rank 1. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
-        log_prob = jax.nn.log_softmax(output, axis=axis)
+        log_prob = log_softmax(output, axis=axis)
     else:
-        output = output / jnp.sum(output, axis, keepdims=True)
-        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = jnp.log(output)
-    return -jnp.sum(target * log_prob, axis=axis)
+        output = output / np.sum(output, axis, keepdims=True)
+        output = np.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = np.log(output)
+    return -np.sum(target * log_prob, axis=axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = jnp.array(target, dtype="int32")
-    output = jnp.array(output)
+    target = np.array(target, dtype="int32")
+    output = np.array(output)
     if len(target.shape) == len(output.shape) and target.shape[-1] == 1:
-        target = jnp.squeeze(target, axis=-1)
+        target = np.squeeze(target, axis=-1)
 
     if len(output.shape) < 1:
         raise ValueError(
             "Argument `output` must be at least rank 1. "
             "Received: "
             f"output.shape={output.shape}"
         )
     if target.shape != output.shape[:-1]:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape "
             "up until the last dimension: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
     if from_logits:
-        log_prob = jax.nn.log_softmax(output, axis=axis)
+        log_prob = log_softmax(output, axis=axis)
     else:
-        output = output / jnp.sum(output, axis, keepdims=True)
-        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = jnp.log(output)
-    target = jnn.one_hot(target, output.shape[axis], axis=axis)
-    return -jnp.sum(target * log_prob, axis=axis)
+        output = output / np.sum(output, axis, keepdims=True)
+        output = np.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = np.log(output)
+    target = one_hot(target, output.shape[axis], axis=axis)
+    return -np.sum(target * log_prob, axis=axis)
 
 
 def binary_crossentropy(target, output, from_logits=False):
-    target = jnp.array(target)
-    output = jnp.array(output)
+    target = np.array(target)
+    output = np.array(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
-        log_logits = jax.nn.log_sigmoid(output)
-        log_neg_logits = jax.nn.log_sigmoid(-output)
-        return -1.0 * target * log_logits - (1.0 - target) * log_neg_logits
-
-    output = jnp.clip(output, epsilon(), 1.0 - epsilon())
-    bce = target * jnp.log(output)
-    bce += (1.0 - target) * jnp.log(1.0 - output)
+        output = sigmoid(output)
+
+    output = np.clip(output, epsilon(), 1.0 - epsilon())
+    bce = target * np.log(output)
+    bce += (1.0 - target) * np.log(1.0 - output)
     return -bce
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     if synchronized:
         raise NotImplementedError(
-            "Argument synchronized=True is not supported with JAX."
+            "Argument synchronized=True is not supported with NumPy."
         )
+    axes = tuple(axes) if isinstance(axes, list) else axes
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
     ori_dtype = standardize_dtype(x.dtype)
-    if ori_dtype in ("float16", "bfloat16"):
+    if ori_dtype == "float16":
         need_cast = True
         x = cast(x, "float32")
 
-    mean = jnp.mean(x, axes, keepdims=True)
-    variance = jnp.var(x, axis=axes, keepdims=True)
+    mean = np.mean(x, axes, keepdims=True)
+
+    # The variance is computed using $Var = E[|x|^2] - |E[x]|^2$, It is faster
+    # but less numerically stable.
+    variance = np.mean(np.square(x), axis=axes, keepdims=True) - np.square(mean)
 
     if not keepdims:
-        mean = jnp.squeeze(mean, axes)
-        variance = jnp.squeeze(variance, axes)
+        mean = np.squeeze(mean, axes)
+        variance = np.squeeze(variance, axes)
     if need_cast:
         # avoid overflow and underflow when casting from float16 to float32
-        mean = jnp.clip(
-            mean, jnp.finfo(jnp.float16).min, jnp.finfo(jnp.float16).max
-        )
-        variance = jnp.clip(
-            variance, jnp.finfo(jnp.float16).min, jnp.finfo(jnp.float16).max
+        mean = np.clip(mean, np.finfo(np.float16).min, np.finfo(np.float16).max)
+        variance = np.clip(
+            variance, np.finfo(np.float16).min, np.finfo(np.float16).max
         )
         mean = cast(mean, ori_dtype)
         variance = cast(variance, ori_dtype)
     return mean, variance
 
 
 def batch_normalization(
     x, mean, variance, axis, offset=None, scale=None, epsilon=1e-3
 ):
     shape = [1] * len(x.shape)
     shape[axis] = mean.shape[0]
-    mean = jnp.reshape(mean, shape)
-    variance = jnp.reshape(variance, shape)
+    mean = np.reshape(mean, shape)
+    variance = np.reshape(variance, shape)
 
-    inv = jax.lax.rsqrt(variance + epsilon)
+    inv = 1.0 / np.sqrt(variance + epsilon)
     if scale is not None:
-        scale = jnp.reshape(scale, shape)
+        scale = np.reshape(scale, shape)
         inv = inv * scale
 
     res = -mean * inv
     if offset is not None:
-        offset = jnp.reshape(offset, shape)
+        offset = np.reshape(offset, shape)
         res = res + offset
 
-    return jnp.add(x * inv, res)
+    return x * inv + res
 
 
-def ctc_loss(
-    target,
-    output,
-    target_length,
-    output_length,
-    mask_index=0,
+def ctc_decode(
+    inputs,
+    sequence_length,
+    strategy,
+    beam_width=100,
+    top_paths=1,
+    merge_repeated=True,
+    mask_index=None,
 ):
-    batch_size, _, _ = output.shape
-    batch_size, max_target_length = target.shape
-
-    output = output.transpose((1, 0, 2))
-    target = target.transpose((1, 0)).astype("int32")
-
-    logits = jnn.log_softmax(output)
-    mgrid_t, mgrid_b = jnp.meshgrid(
-        jnp.arange(max_target_length), jnp.arange(batch_size)
+    raise NotImplementedError(
+        "NumPy backend does not yet support CTC decoding."
     )
-    logprobs_emit = logits[mgrid_t, mgrid_b, target[:, :, None]]
-    logprobs_mask = logits[:, :, mask_index]
-
-    logit_paddings = jnp.array(
-        jnp.arange(max_target_length) < output_length[:, None],
-        dtype=jnp.float32,
-    )
-
-    repeat = jnp.array(target[1:] == target[:-1])
-    repeat = jnp.pad(repeat, ((0, 1), (0, 0))).transpose((1, 0))
-
-    _logepsilon = -100000.0
-
-    def _iterate(prev, x):
-        prev_mask, prev_emit = prev
-        logprob_mask, logprob_emit, pad = x
-
-        prev_mask_orig = prev_mask
-        prev_mask = prev_mask.at[:, 1:].set(
-            jnp.logaddexp(prev_mask[:, 1:], prev_emit + _logepsilon * repeat),
-        )
-        emit = jnp.logaddexp(
-            prev_mask[:, :-1] + logprob_emit, prev_emit + logprob_emit
-        )
-
-        mask = prev_mask + logprob_mask[:, None]
-        mask = mask.at[:, 1:].set(
-            jnp.logaddexp(
-                mask[:, 1:],
-                prev_emit + logprob_mask[:, None] + _logepsilon * (1 - repeat),
-            )
-        )
-
-        pad = pad[:, None]
-        emit = emit * pad + prev_emit * (1 - pad)
-        mask = mask * pad + prev_mask_orig * (1 - pad)
-
-        return (mask, emit), (mask, emit)
-
-    mask_init = jnp.full((batch_size, max_target_length + 1), _logepsilon)
-    mask_init = mask_init.at[:, 0].set(0.0)
-    emit_init = jnp.full((batch_size, max_target_length), _logepsilon)
-
-    _, (alphas_mask, alphas_emit) = lax.scan(
-        _iterate,
-        (mask_init, emit_init),
-        (logprobs_mask, logprobs_emit, logit_paddings.transpose()),
-    )
-
-    last_alpha_mask = (
-        alphas_mask[-1]
-        .at[:, 1:]
-        .set(jnp.logaddexp(alphas_mask[-1, :, 1:], alphas_emit[-1]))
-    )
-
-    return -last_alpha_mask[jnp.arange(batch_size), target_length]
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/numpy.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -764,17 +764,17 @@
     return jnp.mod(x1, x2)
 
 
 def moveaxis(x, source, destination):
     return jnp.moveaxis(x, source=source, destination=destination)
 
 
-def nan_to_num(x):
+def nan_to_num(x, nan=0.0, posinf=None, neginf=None):
     x = convert_to_tensor(x)
-    return jnp.nan_to_num(x)
+    return jnp.nan_to_num(x, nan=nan, posinf=posinf, neginf=neginf)
 
 
 def ndim(x):
     return jnp.ndim(x)
 
 
 def nonzero(x):
@@ -1019,14 +1019,18 @@
     return jnp.vdot(x1, x2)
 
 
 def vstack(xs):
     return jnp.vstack(xs)
 
 
+def vectorize(pyfunc):
+    return jnp.vectorize(pyfunc)
+
+
 def where(condition, x1, x2):
     return jnp.where(condition, x1, x2)
 
 
 @sparse.elementwise_division
 def divide(x1, x2):
     x1 = convert_to_tensor(x1)
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/random.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/rnn.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/sparse.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/trainer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/core.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/image.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/math.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/nn.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/nn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,386 +1,471 @@
-import jax
-import numpy as np
-from jax import lax
-from jax import numpy as jnp
+import torch
+import torch.nn.functional as tnn
 
+from keras.src import tree
 from keras.src.backend import standardize_data_format
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common.backend_utils import (
-    compute_conv_transpose_padding_args_for_jax,
+    compute_conv_transpose_padding_args_for_torch,
 )
 from keras.src.backend.config import epsilon
-from keras.src.backend.numpy.core import cast
-from keras.src.backend.numpy.core import convert_to_tensor
-from keras.src.backend.numpy.core import is_tensor
-from keras.src.utils.module_utils import scipy
+from keras.src.backend.torch.core import cast
+from keras.src.backend.torch.core import convert_to_tensor
+from keras.src.backend.torch.core import get_device
+from keras.src.backend.torch.numpy import expand_dims
+from keras.src.backend.torch.numpy import maximum
+from keras.src.backend.torch.numpy import where
+from keras.src.utils.argument_validation import standardize_tuple
 
 
 def relu(x):
     x = convert_to_tensor(x)
-    return np.maximum(x, np.array(0.0, x.dtype))
+    return tnn.relu(x)
 
 
 def relu6(x):
     x = convert_to_tensor(x)
-    # np.clip incorrectly promote bfloat16 to float32, so we replace it with
-    # np.minimum and np.maximum here
-    return np.minimum(
-        np.maximum(x, np.array(0.0, x.dtype)), np.array(6.0, x.dtype)
-    )
+    return tnn.relu6(x)
 
 
 def sigmoid(x):
     x = convert_to_tensor(x)
-    return np.array(1.0, x.dtype) / (np.array(1.0, x.dtype) + np.exp(-x))
+    return tnn.sigmoid(x)
 
 
 def tanh(x):
-    return np.tanh(x)
+    x = convert_to_tensor(x)
+    return tnn.tanh(x)
 
 
 def softplus(x):
     x = convert_to_tensor(x)
-    return np.logaddexp(x, np.array(0.0, x.dtype))
+    return tnn.softplus(x)
 
 
 def softsign(x):
     x = convert_to_tensor(x)
-    return x / (np.array(1.0, x.dtype) + np.abs(x))
+    return tnn.softsign(x)
 
 
 def silu(x):
     x = convert_to_tensor(x)
-    return x * sigmoid(x)
+    return tnn.silu(x)
 
 
 def log_sigmoid(x):
     x = convert_to_tensor(x)
-    return -softplus(-x)
+    return tnn.logsigmoid(x)
 
 
 def leaky_relu(x, negative_slope=0.2):
     x = convert_to_tensor(x)
-    return np.maximum(x, np.array(negative_slope, x.dtype) * x)
+    return tnn.leaky_relu(x, negative_slope=negative_slope)
 
 
 def hard_sigmoid(x):
-    # python numbers will be promoted to float64 by np, so it's necessary to
-    # first convert the python numbers to np scalars
-    x = x / np.array(6.0, x.dtype) + np.array(0.5, x.dtype)
-    return np.where(
-        x <= 0.0,
-        np.array(0.0, x.dtype),
-        np.where(x >= 1.0, np.array(1.0, x.dtype), x),
-    )
+    x = convert_to_tensor(x)
+    return tnn.hardsigmoid(x)
 
 
 def hard_silu(x):
-    return x * hard_sigmoid(x)
+    x = convert_to_tensor(x)
+    return tnn.hardswish(x)
 
 
 def elu(x, alpha=1.0):
     x = convert_to_tensor(x)
-    return np.where(
-        x >= np.array(0.0, x.dtype), x, np.array(alpha, x.dtype) * np.expm1(x)
-    )
+    return tnn.elu(x, alpha)
 
 
-def selu(
-    x,
-    alpha=1.6732632423543772848170429916717,
-    scale=1.0507009873554804934193349852946,
-):
+def selu(x):
     x = convert_to_tensor(x)
-    return np.array(scale, x.dtype) * elu(x, alpha)
+    return tnn.selu(x)
 
 
 def gelu(x, approximate=True):
+    # TODO: torch.nn.gelu expects string approximate of `"none"` or `"tanh"`
     x = convert_to_tensor(x)
-    # followed by JAX's implementation
     if approximate:
-        sqrt_2_over_pi = np.sqrt(2 / np.pi).astype(x.dtype)
-        cdf = np.array(0.5, x.dtype) * (
-            np.array(1.0, x.dtype)
-            + np.tanh(
-                sqrt_2_over_pi
-                * (x + np.array(0.044715, x.dtype) * (x**3).astype(x.dtype))
-            )
-        )
-        return x * cdf
-    else:
-        sqrt_2 = np.sqrt(2).astype(x.dtype)
-        return (
-            x
-            * (scipy.special.erf(x / sqrt_2) + 1).astype(x.dtype)
-            / np.array(2, x.dtype)
-        )
+        return tnn.gelu(x, approximate="tanh")
+    return tnn.gelu(x)
 
 
-def softmax(x, axis=None):
-    exp_x = np.exp(x - np.max(x, axis=axis, keepdims=True))
-    return exp_x / np.sum(exp_x, axis=axis, keepdims=True)
+def softmax(x, axis=-1):
+    x = convert_to_tensor(x)
+    dtype = standardize_dtype(x.dtype)
+    # TODO: tnn.softmax doesn't support float16 using cpu
+    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
+        x = cast(x, "float32")
+    if axis is None:
+        # Unlike numpy, PyTorch will handle axis=None as axis=-1.
+        # We need this workaround for the reduction on every dim.
+        output = torch.reshape(x, [-1])
+        output = tnn.softmax(output, dim=-1)
+        output = torch.reshape(output, x.shape)
+    else:
+        output = tnn.softmax(x, dim=axis)
+    return cast(output, dtype)
 
 
-def log_softmax(x, axis=None):
-    max_x = np.max(x, axis=axis, keepdims=True)
-    logsumexp = np.log(np.exp(x - max_x).sum(axis=axis, keepdims=True))
-    return x - max_x - logsumexp
+def log_softmax(x, axis=-1):
+    x = convert_to_tensor(x)
+    dtype = standardize_dtype(x.dtype)
+    # TODO: tnn.log_softmax doesn't support float16 using cpu
+    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
+        x = cast(x, "float32")
+    if axis is None:
+        # Unlike numpy, PyTorch will handle axis=None as axis=-1.
+        # We need this workaround for the reduction on every dim.
+        output = torch.reshape(x, [-1])
+        output = tnn.log_softmax(output, dim=-1)
+        output = torch.reshape(output, x.shape)
+    else:
+        output = tnn.log_softmax(x, dim=axis)
+    return cast(output, dtype)
 
 
-def _convert_to_spatial_operand(
-    x,
-    num_spatial_dims,
-    data_format="channels_last",
-    include_batch_and_channels=True,
+def _compute_padding_length(
+    input_length, kernel_length, stride, dilation_rate=1
 ):
-    # Helper function that converts an operand to a spatial operand.
-    x = (x,) * num_spatial_dims if isinstance(x, int) else x
-    if not include_batch_and_channels:
-        return x
-    if data_format == "channels_last":
-        x = (1,) + x + (1,)
-    else:
-        x = (1,) + (1,) + x
-    return x
+    """Compute padding length along one dimension."""
+    total_padding_length = (
+        dilation_rate * (kernel_length - 1) - (input_length - 1) % stride
+    )
+    left_padding = total_padding_length // 2
+    right_padding = (total_padding_length + 1) // 2
+    return (left_padding, right_padding)
 
 
-def _pool(
-    inputs,
-    initial_value,
-    reduce_fn,
-    pool_size,
-    strides=None,
-    padding="valid",
+def _apply_same_padding(
+    inputs, kernel_size, strides, operation_type, dilation_rate=1
 ):
-    """Helper function to define pooling functions.
+    """Apply same padding to the input tensor.
 
-    Args:
-        inputs: input data of shape `N+2`.
-        initial_value: the initial value for the reduction.
-        reduce_fn: a reduce function of the form `(T, T) -> T`.
-        pool_size: a sequence of `N` integers, representing the window size to
-            reduce over.
-        strides: a sequence of `N` integers, representing the inter-window
-            strides (default: `(1, ..., 1)`).
-        padding: either the string `same` or `valid`.
+    This function will evaluate if the padding value is compatible with torch
+    functions. To avoid calling `pad()` as much as possible, which may cause
+    performance or memory issues, when compatible, it does not apply the padding
+    to the tensor, but returns the input tensor and the padding value to pass to
+    the torch functions. If not compatible, it returns the padded tensor and 0
+    as the padding value.
 
     Returns:
-        The output of the reduction for each window slice.
+        tensor: A padded tensor or the inputs.
+        padding: The padding value, ready to pass to the torch functions.
     """
-    if padding not in ("same", "valid"):
-        raise ValueError(
-            f"Invalid padding '{padding}', must be 'same' or 'valid'."
-        )
-    padding = padding.upper()
-    return np.array(
-        lax.reduce_window(
-            inputs,
-            initial_value,
-            reduce_fn,
-            pool_size,
-            strides,
-            padding,
-        )
+    spatial_shape = inputs.shape[2:]
+    num_spatial_dims = len(spatial_shape)
+    padding = ()
+
+    for i in range(num_spatial_dims):
+        if operation_type == "pooling":
+            padding_size = _compute_padding_length(
+                spatial_shape[i], kernel_size[i], strides[i]
+            )
+            mode = "replicate"
+        else:
+            dilation_rate = standardize_tuple(
+                dilation_rate, num_spatial_dims, "dilation_rate"
+            )
+            padding_size = _compute_padding_length(
+                spatial_shape[i], kernel_size[i], strides[i], dilation_rate[i]
+            )
+            mode = "constant"
+        padding = (padding_size,) + padding
+
+    if all([left == right for left, right in padding]):
+        return inputs, [left for left, _ in padding]
+
+    flattened_padding = tuple(
+        value for left_and_right in padding for value in left_and_right
     )
+    return tnn.pad(inputs, pad=flattened_padding, mode=mode), 0
+
+
+def _transpose_spatial_inputs(inputs):
+    num_spatial_dims = inputs.ndim - 2
+    # Torch pooling does not support `channels_last` format, so
+    # we need to transpose to `channels_first` format.
+    if num_spatial_dims == 1:
+        inputs = torch.permute(inputs, (0, 2, 1))
+    elif num_spatial_dims == 2:
+        inputs = torch.permute(inputs, (0, 3, 1, 2))
+    elif num_spatial_dims == 3:
+        inputs = torch.permute(inputs, (0, 4, 1, 2, 3))
+    else:
+        raise ValueError(
+            "Inputs must have ndim=3, 4 or 5, "
+            "corresponding to 1D, 2D and 3D inputs. "
+            f"Received input shape: {inputs.shape}."
+        )
+    return inputs
+
+
+def _transpose_spatial_outputs(outputs):
+    # Undo the transpose in `_transpose_spatial_inputs`.
+    num_spatial_dims = len(outputs.shape) - 2
+    if num_spatial_dims == 1:
+        outputs = torch.permute(outputs, (0, 2, 1))
+    elif num_spatial_dims == 2:
+        outputs = torch.permute(outputs, (0, 2, 3, 1))
+    elif num_spatial_dims == 3:
+        outputs = torch.permute(outputs, (0, 2, 3, 4, 1))
+    return outputs
+
+
+def _transpose_conv_kernel(kernel):
+    # Torch requires conv kernel of format
+    # `(out_channels, in_channels, spatial_dims)`, we need to transpose.
+    num_spatial_dims = len(kernel.shape) - 2
+    if num_spatial_dims == 1:
+        kernel = torch.permute(kernel, (2, 1, 0))
+    elif num_spatial_dims == 2:
+        kernel = torch.permute(kernel, (3, 2, 0, 1))
+    elif num_spatial_dims == 3:
+        kernel = torch.permute(kernel, (4, 3, 0, 1, 2))
+    return kernel
 
 
 def max_pool(
     inputs,
     pool_size,
     strides=None,
     padding="valid",
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    inputs = convert_to_tensor(inputs)
     num_spatial_dims = inputs.ndim - 2
-    pool_size = _convert_to_spatial_operand(
-        pool_size, num_spatial_dims, data_format
-    )
-    strides = pool_size if strides is None else strides
-    strides = _convert_to_spatial_operand(
-        strides, num_spatial_dims, data_format
-    )
-    return _pool(inputs, -jnp.inf, lax.max, pool_size, strides, padding)
+    pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
+    if strides is None:
+        strides = pool_size
+    else:
+        strides = standardize_tuple(strides, num_spatial_dims, "strides")
+
+    data_format = standardize_data_format(data_format)
+    if data_format == "channels_last":
+        inputs = _transpose_spatial_inputs(inputs)
+
+    if padding == "same":
+        # Torch does not natively support `"same"` padding, we need to manually
+        # apply the right amount of padding to `inputs`.
+        inputs, padding = _apply_same_padding(
+            inputs, pool_size, strides, operation_type="pooling"
+        )
+    else:
+        padding = 0
+
+    device = get_device()
+    # Torch max pooling ops do not support symbolic tensors.
+    # Create a real tensor to execute the ops.
+    if device == "meta":
+        inputs = torch.empty(
+            size=inputs.shape, dtype=inputs.dtype, device="cpu"
+        )
+
+    if num_spatial_dims == 1:
+        outputs = tnn.max_pool1d(
+            inputs, kernel_size=pool_size, stride=strides, padding=padding
+        )
+    elif num_spatial_dims == 2:
+        outputs = tnn.max_pool2d(
+            inputs, kernel_size=pool_size, stride=strides, padding=padding
+        )
+    elif num_spatial_dims == 3:
+        outputs = tnn.max_pool3d(
+            inputs, kernel_size=pool_size, stride=strides, padding=padding
+        )
+    else:
+        raise ValueError(
+            "Inputs to pooling op must have ndim=3, 4 or 5, "
+            "corresponding to 1D, 2D and 3D inputs. "
+            f"Received input shape: {inputs.shape}."
+        )
+
+    outputs = outputs.to(device)
+    if data_format == "channels_last":
+        outputs = _transpose_spatial_outputs(outputs)
+    return outputs
 
 
 def average_pool(
     inputs,
     pool_size,
-    strides,
-    padding,
+    strides=None,
+    padding="valid",
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    inputs = convert_to_tensor(inputs)
     num_spatial_dims = inputs.ndim - 2
-    pool_size = _convert_to_spatial_operand(
-        pool_size, num_spatial_dims, data_format
-    )
-    strides = pool_size if strides is None else strides
-    strides = _convert_to_spatial_operand(
-        strides, num_spatial_dims, data_format
-    )
-
-    pooled = _pool(inputs, 0.0, lax.add, pool_size, strides, padding)
-    if padding == "valid":
-        # Avoid the extra reduce_window.
-        return pooled / np.prod(pool_size)
-    else:
-        # Count the number of valid entries at each input point, then use that
-        # for computing average. Assumes that any two arrays of same shape will
-        # be padded the same. Avoid broadcasting on axis where pooling is
-        # skipped.
-        shape = [
-            (a if b != 1 else 1) for (a, b) in zip(inputs.shape, pool_size)
-        ]
-        window_counts = _pool(
-            jnp.ones(shape, inputs.dtype),
-            0.0,
-            lax.add,
-            pool_size,
-            strides,
-            padding,
-        )
-        return pooled / window_counts
-
-
-def _convert_to_lax_conv_dimension_numbers(
-    num_spatial_dims,
-    data_format="channels_last",
-    transpose=False,
-):
-    """Create a `lax.ConvDimensionNumbers` for the given inputs."""
-    num_dims = num_spatial_dims + 2
+    pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
+    if strides is None:
+        strides = pool_size
+    else:
+        strides = standardize_tuple(strides, num_spatial_dims, "strides")
 
+    data_format = standardize_data_format(data_format)
     if data_format == "channels_last":
-        spatial_dims = tuple(range(1, num_dims - 1))
-        inputs_dn = (0, num_dims - 1) + spatial_dims
-    else:
-        spatial_dims = tuple(range(2, num_dims))
-        inputs_dn = (0, 1) + spatial_dims
+        inputs = _transpose_spatial_inputs(inputs)
+    padding_value = 0
+    if padding == "same":
+        spatial_shape = inputs.shape[2:]
+        num_spatial_dims = len(spatial_shape)
+        padding_value = []
+        uneven_padding = []
+
+        for i in range(num_spatial_dims):
+            padding_size = _compute_padding_length(
+                spatial_shape[i], pool_size[i], strides[i]
+            )
+            # Torch only supports even padding on each dim, to replicate the
+            # behavior of "same" padding of `tf.keras` as much as possible,
+            # we need to pad evenly using the shorter padding.
+            padding_value.append(padding_size[0])
+            if padding_size[0] != padding_size[1]:
+                # Handle unequal padding.
+                # `torch.nn.pad` sets padding value in the reverse order.
+                uneven_padding = [0, 1] + uneven_padding
+        # Only call tnn.pad when needed.
+        if len(uneven_padding) > 0:
+            inputs = tnn.pad(inputs, uneven_padding)
 
-    if transpose:
-        kernel_dn = (num_dims - 2, num_dims - 1) + tuple(range(num_dims - 2))
+    if num_spatial_dims == 1:
+        outputs = tnn.avg_pool1d(
+            inputs,
+            kernel_size=pool_size,
+            stride=strides,
+            padding=padding_value,
+            count_include_pad=False,
+        )
+    elif num_spatial_dims == 2:
+        outputs = tnn.avg_pool2d(
+            inputs,
+            kernel_size=pool_size,
+            stride=strides,
+            padding=padding_value,
+            count_include_pad=False,
+        )
+    elif num_spatial_dims == 3:
+        outputs = tnn.avg_pool3d(
+            inputs,
+            kernel_size=pool_size,
+            stride=strides,
+            padding=padding_value,
+            count_include_pad=False,
+        )
     else:
-        kernel_dn = (num_dims - 1, num_dims - 2) + tuple(range(num_dims - 2))
-
-    return lax.ConvDimensionNumbers(
-        lhs_spec=inputs_dn, rhs_spec=kernel_dn, out_spec=inputs_dn
-    )
+        raise ValueError(
+            "Inputs to pooling op must have ndim=3, 4 or 5, "
+            "corresponding to 1D, 2D and 3D inputs. "
+            f"Received input shape: {inputs.shape}."
+        )
+    if data_format == "channels_last":
+        outputs = _transpose_spatial_outputs(outputs)
+    return outputs
 
 
 def conv(
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    inputs = convert_to_tensor(inputs)
+    kernel = convert_to_tensor(kernel)
     num_spatial_dims = inputs.ndim - 2
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
+    strides = standardize_tuple(strides, num_spatial_dims, "strides")
+
+    data_format = standardize_data_format(data_format)
     if data_format == "channels_last":
-        channels = inputs.shape[-1]
-    else:
-        channels = inputs.shape[1]
-    kernel_in_channels = kernel.shape[-2]
+        inputs = _transpose_spatial_inputs(inputs)
+    # Transpose kernel from keras format to torch format.
+    kernel = _transpose_conv_kernel(kernel)
+    if padding == "same" and any(d != 1 for d in tree.flatten(strides)):
+        # Torch does not support this case in conv2d().
+        # Manually pad the tensor.
+        inputs, padding = _apply_same_padding(
+            inputs,
+            kernel.shape[2:],
+            strides,
+            operation_type="conv",
+            dilation_rate=dilation_rate,
+        )
+    channels = inputs.shape[1]
+    kernel_in_channels = kernel.shape[1]
     if channels % kernel_in_channels > 0:
         raise ValueError(
             "The number of input channels must be evenly divisible by "
-            f"kernel's in_channels. Received input channels {channels} and "
-            f"kernel in_channels {kernel_in_channels}. "
+            f"kernel.shape[1]. Received: inputs.shape={inputs.shape}, "
+            f"kernel.shape={kernel.shape}"
         )
-    feature_group_count = channels // kernel_in_channels
-    return np.array(
-        jax.lax.conv_general_dilated(
+    groups = channels // kernel_in_channels
+    if num_spatial_dims == 1:
+        outputs = tnn.conv1d(
             inputs,
-            kernel if is_tensor(kernel) else kernel.numpy(),
-            strides,
-            padding,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            feature_group_count=feature_group_count,
+            kernel,
+            stride=strides,
+            dilation=dilation_rate,
+            groups=groups,
+            padding=padding,
         )
-    )
+    elif num_spatial_dims == 2:
+        outputs = tnn.conv2d(
+            inputs,
+            kernel,
+            stride=strides,
+            dilation=dilation_rate,
+            groups=groups,
+            padding=padding,
+        )
+    elif num_spatial_dims == 3:
+        outputs = tnn.conv3d(
+            inputs,
+            kernel,
+            stride=strides,
+            dilation=dilation_rate,
+            groups=groups,
+            padding=padding,
+        )
+    else:
+        raise ValueError(
+            "Inputs to conv operation should have ndim=3, 4, or 5,"
+            "corresponding to 1D, 2D and 3D inputs. Received input "
+            f"shape: {inputs.shape}."
+        )
+
+    if data_format == "channels_last":
+        outputs = _transpose_spatial_outputs(outputs)
+    return outputs
 
 
 def depthwise_conv(
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    feature_group_count = (
-        inputs.shape[-1] if data_format == "channels_last" else inputs.shape[1]
-    )
-    kernel = jnp.reshape(
-        kernel if is_tensor(kernel) else kernel.numpy(),
-        kernel.shape[:-2] + (1, feature_group_count * kernel.shape[-1]),
-    )
-    return np.array(
-        jax.lax.conv_general_dilated(
-            inputs,
-            kernel,
-            strides,
-            padding,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            feature_group_count=feature_group_count,
-        )
+    kernel = convert_to_tensor(kernel)
+    kernel = torch.reshape(
+        kernel, kernel.shape[:-2] + (1, kernel.shape[-2] * kernel.shape[-1])
     )
+    return conv(inputs, kernel, strides, padding, data_format, dilation_rate)
 
 
 def separable_conv(
     inputs,
     depthwise_kernel,
     pointwise_kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
     depthwise_conv_output = depthwise_conv(
         inputs,
         depthwise_kernel,
         strides,
         padding,
         data_format,
         dilation_rate,
@@ -400,100 +485,117 @@
     kernel,
     strides=1,
     padding="valid",
     output_padding=None,
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    inputs = convert_to_tensor(inputs)
+    kernel = convert_to_tensor(kernel)
     num_spatial_dims = inputs.ndim - 2
-    padding_values = compute_conv_transpose_padding_args_for_jax(
+    strides = standardize_tuple(strides, num_spatial_dims, "strides")
+
+    data_format = standardize_data_format(data_format)
+    (
+        torch_padding,
+        torch_output_padding,
+    ) = compute_conv_transpose_padding_args_for_torch(
         input_shape=inputs.shape,
         kernel_shape=kernel.shape,
         strides=strides,
         padding=padding,
         output_padding=output_padding,
         dilation_rate=dilation_rate,
     )
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
+    if data_format == "channels_last":
+        inputs = _transpose_spatial_inputs(inputs)
+    # Transpose kernel from keras format to torch format.
+    kernel = _transpose_conv_kernel(kernel)
+    kernel_spatial_shape = kernel.shape[2:]
+    if isinstance(dilation_rate, int):
+        dilation_rate = [dilation_rate] * len(kernel_spatial_shape)
 
-    return np.array(
-        jax.lax.conv_transpose(
+    if num_spatial_dims == 1:
+        outputs = tnn.conv_transpose1d(
             inputs,
-            kernel if is_tensor(kernel) else kernel.numpy(),
-            strides,
-            padding=padding_values,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            transpose_kernel=True,
+            kernel,
+            stride=strides,
+            padding=torch_padding,
+            output_padding=torch_output_padding,
+            dilation=dilation_rate,
         )
-    )
+    elif num_spatial_dims == 2:
+        outputs = tnn.conv_transpose2d(
+            inputs,
+            kernel,
+            stride=strides,
+            padding=torch_padding,
+            output_padding=torch_output_padding,
+            dilation=dilation_rate,
+        )
+    elif num_spatial_dims == 3:
+        outputs = tnn.conv_transpose3d(
+            inputs,
+            kernel,
+            stride=strides,
+            padding=torch_padding,
+            output_padding=torch_output_padding,
+            dilation=dilation_rate,
+        )
+    else:
+        raise ValueError(
+            "Inputs to conv transpose operation should have ndim=3, 4, or 5,"
+            "corresponding to 1D, 2D and 3D inputs. Received input "
+            f"shape: {inputs.shape}."
+        )
+    if data_format == "channels_last":
+        outputs = _transpose_spatial_outputs(outputs)
+    return outputs
 
 
 def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
     if sparse:
-        raise ValueError("Unsupported value `sparse=True` with numpy backend")
-    x = convert_to_tensor(x)
-    input_shape = x.shape
-
-    # Shrink the last dimension if the shape is (..., 1).
-    if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
-        input_shape = tuple(input_shape[:-1])
-
-    x = x.reshape(-1)
-    if not num_classes:
-        num_classes = np.max(x) + 1
-
-    batch_size = x.shape[0]
-    categorical = np.zeros((batch_size, num_classes), dtype=dtype)
-    valid_indices = x >= 0
-    categorical[np.arange(batch_size)[valid_indices], x[valid_indices]] = 1
-
-    # First, reshape the array with the extra dimension at the end
-    output_shape = input_shape + (num_classes,)
-    categorical = np.reshape(categorical, output_shape)
-
-    # Then, move this new dimension to the right place (according to axis)
-    if axis != -1:
-        categorical = np.moveaxis(categorical, -1, axis)
-
-    return categorical
+        raise ValueError("Unsupported value `sparse=True` with torch backend")
+    # Axis is the output axis. By default, PyTorch, outputs to last axis.
+    # If axis is not last, change output to axis and shift remaining elements.
+    x = convert_to_tensor(x, dtype=torch.long)
+
+    # Torch one_hot does not natively handle negative values, so we add some
+    # manual handling for negatives in the input to one_hot by using max(x, 0).
+    # The output will have some invalid results, so we set them back to 0 using
+    # `where` afterwards.
+    output = tnn.one_hot(maximum(x, 0), num_classes)
+    output = where(expand_dims(x, axis=-1) >= 0, output, 0)
+    output = convert_to_tensor(output, dtype=dtype)
+    dims = output.dim()
+    if axis != -1 and axis != dims:
+        new_axes_order = list(range(dims))
+        new_axes_order[axis] = -1  # Shifts output to axis position
+        # Shift remaining axes with offset by 1 since output moved to `axis`.
+        for ax in range(axis + 1, dims):
+            new_axes_order[ax] -= 1
+        output = output.permute(new_axes_order)
+    return output
 
 
 def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
     if sparse:
-        raise ValueError("Unsupported value `sparse=True` with numpy backend")
+        raise ValueError("Unsupported value `sparse=True` with torch backend")
     x = convert_to_tensor(x)
     reduction_axis = 1 if len(x.shape) > 1 else 0
-    outputs = np.max(
+    outputs = torch.amax(
         one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
-        axis=reduction_axis,
+        dim=reduction_axis,
     )
     return outputs
 
 
 def categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = np.array(target)
-    output = np.array(output)
+    target = convert_to_tensor(target)
+    output = convert_to_tensor(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
@@ -501,117 +603,177 @@
         raise ValueError(
             "Arguments `target` and `output` must be at least rank 1. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
-        log_prob = log_softmax(output, axis=axis)
+        log_prob = tnn.log_softmax(output, dim=axis)
     else:
-        output = output / np.sum(output, axis, keepdims=True)
-        output = np.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = np.log(output)
-    return -np.sum(target * log_prob, axis=axis)
+        output = output / torch.sum(output, dim=axis, keepdim=True)
+        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = torch.log(output)
+    return -torch.sum(target * log_prob, dim=axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = np.array(target, dtype="int32")
-    output = np.array(output)
+    target = convert_to_tensor(target, dtype=torch.long)
+    output = convert_to_tensor(output)
+
     if len(target.shape) == len(output.shape) and target.shape[-1] == 1:
-        target = np.squeeze(target, axis=-1)
+        target = torch.squeeze(target, dim=-1)
 
     if len(output.shape) < 1:
         raise ValueError(
             "Argument `output` must be at least rank 1. "
             "Received: "
             f"output.shape={output.shape}"
         )
     if target.shape != output.shape[:-1]:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape "
             "up until the last dimension: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
     if from_logits:
-        log_prob = log_softmax(output, axis=axis)
+        log_prob = tnn.log_softmax(output, dim=axis)
     else:
-        output = output / np.sum(output, axis, keepdims=True)
-        output = np.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = np.log(output)
+        output = output / torch.sum(output, dim=axis, keepdim=True)
+        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = torch.log(output)
     target = one_hot(target, output.shape[axis], axis=axis)
-    return -np.sum(target * log_prob, axis=axis)
+    return -torch.sum(target * log_prob, dim=axis)
 
 
 def binary_crossentropy(target, output, from_logits=False):
-    target = np.array(target)
-    output = np.array(output)
+    target = convert_to_tensor(target)
+    output = convert_to_tensor(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
-
+    # By default, PyTorch, does reduction of `sum` over all rows,
+    # change reduction to `none` to keep dim
     if from_logits:
-        output = sigmoid(output)
-
-    output = np.clip(output, epsilon(), 1.0 - epsilon())
-    bce = target * np.log(output)
-    bce += (1.0 - target) * np.log(1.0 - output)
-    return -bce
+        return tnn.binary_cross_entropy_with_logits(
+            output, target, reduction="none"
+        )
+    else:
+        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        return tnn.binary_cross_entropy(output, target, reduction="none")
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     if synchronized:
         raise NotImplementedError(
-            "Argument synchronized=True is not supported with NumPy."
+            "Argument synchronized=True is not supported with PyTorch."
         )
-    axes = tuple(axes) if isinstance(axes, list) else axes
+    x = convert_to_tensor(x)
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
     ori_dtype = standardize_dtype(x.dtype)
     if ori_dtype == "float16":
         need_cast = True
         x = cast(x, "float32")
 
-    mean = np.mean(x, axes, keepdims=True)
+    mean = torch.mean(x, dim=axes, keepdim=True)
 
     # The variance is computed using $Var = E[|x|^2] - |E[x]|^2$, It is faster
     # but less numerically stable.
-    variance = np.mean(np.square(x), axis=axes, keepdims=True) - np.square(mean)
+    # Note: stop_gradient does not change the gradient to the mean, because that
+    # gradient is zero.
+    variance = torch.mean(
+        torch.square(x), dim=axes, keepdim=True
+    ) - torch.square(mean)
 
     if not keepdims:
-        mean = np.squeeze(mean, axes)
-        variance = np.squeeze(variance, axes)
+        mean = torch.squeeze(mean, axes)
+        variance = torch.squeeze(variance, axes)
     if need_cast:
         # avoid overflow and underflow when casting from float16 to float32
-        mean = np.clip(mean, np.finfo(np.float16).min, np.finfo(np.float16).max)
-        variance = np.clip(
-            variance, np.finfo(np.float16).min, np.finfo(np.float16).max
+        mean = torch.clip(
+            mean,
+            torch.finfo(torch.float16).min,
+            torch.finfo(torch.float16).max,
+        )
+        variance = torch.clip(
+            variance,
+            torch.finfo(torch.float16).min,
+            torch.finfo(torch.float16).max,
         )
         mean = cast(mean, ori_dtype)
         variance = cast(variance, ori_dtype)
     return mean, variance
 
 
 def batch_normalization(
     x, mean, variance, axis, offset=None, scale=None, epsilon=1e-3
 ):
+    x = convert_to_tensor(x)
+    mean = convert_to_tensor(mean)
+    variance = convert_to_tensor(variance)
+
     shape = [1] * len(x.shape)
     shape[axis] = mean.shape[0]
-    mean = np.reshape(mean, shape)
-    variance = np.reshape(variance, shape)
+    mean = torch.reshape(mean, shape)
+    variance = torch.reshape(variance, shape)
 
-    inv = 1.0 / np.sqrt(variance + epsilon)
+    if offset is not None:
+        offset = convert_to_tensor(offset)
+        offset = torch.reshape(offset, shape)
+    else:
+        offset = torch.zeros_like(mean)
     if scale is not None:
-        scale = np.reshape(scale, shape)
-        inv = inv * scale
+        scale = convert_to_tensor(scale)
+        scale = torch.reshape(scale, shape)
+    else:
+        scale = torch.ones_like(variance)
 
-    res = -mean * inv
-    if offset is not None:
-        offset = np.reshape(offset, shape)
-        res = res + offset
+    return (
+        x.subtract(mean)
+        .mul_(variance.add(epsilon).rsqrt_().mul(scale))
+        .add_(offset)
+    )
+
+
+def ctc_loss(
+    target,
+    output,
+    target_length,
+    output_length,
+    mask_index=0,
+):
+    target = convert_to_tensor(target)
+    output = convert_to_tensor(output)
+    target_length = convert_to_tensor(target_length)
+    output_length = convert_to_tensor(output_length)
+
+    output = torch.transpose(output, 1, 0)
+    logits = tnn.log_softmax(output, dim=-1)
 
-    return x * inv + res
+    return tnn.ctc_loss(
+        logits,
+        target,
+        output_length,
+        target_length,
+        blank=mask_index,
+        reduction="none",
+    )
+
+
+def ctc_decode(
+    inputs,
+    sequence_length,
+    strategy,
+    beam_width=100,
+    top_paths=1,
+    merge_repeated=True,
+    mask_index=None,
+):
+    raise NotImplementedError(
+        "Torch backend does not yet support CTC decoding."
+    )
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -684,16 +684,16 @@
     return np.mod(x1, x2)
 
 
 def moveaxis(x, source, destination):
     return np.moveaxis(x, source=source, destination=destination)
 
 
-def nan_to_num(x):
-    return np.nan_to_num(x)
+def nan_to_num(x, nan=0.0, posinf=None, neginf=None):
+    return np.nan_to_num(x, nan=nan, posinf=posinf, neginf=neginf)
 
 
 def ndim(x):
     return np.ndim(x)
 
 
 def nonzero(x):
@@ -933,14 +933,18 @@
         dtype = dtypes.result_type(*dtype_set)
         xs = tree.map_structure(
             lambda x: convert_to_tensor(x).astype(dtype), xs
         )
     return np.vstack(xs)
 
 
+def vectorize(pyfunc):
+    return np.vectorize(pyfunc)
+
+
 def where(condition, x1, x2):
     if x1 is not None and x2 is not None:
         if not isinstance(x1, (int, float)):
             x1 = convert_to_tensor(x1)
         if not isinstance(x2, (int, float)):
             x2 = convert_to_tensor(x2)
         dtype = dtypes.result_type(
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/random.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/distribute_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/distribute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/name_scope_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/name_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/nn.py`

 * *Files 3% similar despite different names*

```diff
@@ -442,15 +442,15 @@
         padding=padding.upper(),
         data_format=tf_data_format,
         dilations=dilation_rate,
     )
 
 
 def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
-    x = convert_to_tensor(x)
+    x = convert_to_tensor(x, dtype="int64")
     if dtype is None:
         dtype = "float32"
     if sparse:
         # We don't use `tf.sparse.bincount`, it doesn't handle negative indices
         # and only support rank 1 and 2 tensors (`one_hot` adds a dimension).
         if axis < 0:
             axis = axis + len(x.shape) + 1
@@ -793,38 +793,53 @@
 def ctc_loss(
     target,
     output,
     target_length,
     output_length,
     mask_index=0,
 ):
-    """Runs CTC (Connectionist Temporal Classification) loss on each
-    batch element.
-
-    Arguments:
-        target: Tensor `(batch_size, max_length)` containing the
-            target sequences in integer format.
-        output: Tensor `(batch_size, max_length, num_classes)`
-            containing the output of the softmax.
-        target_length: Tensor `(batch_size,)` containing the sequence length
-            for each target sequence in the batch.
-        output_length: Tensor `(batch_size,)` containing the sequence length
-            for each output sequence in the batch.
-        mask_index: The value in `target` and `output` that represents the
-            blank label.
-
-    Returns:
-        A tensor of shape `(batch_size,)` containing the CTC loss for each
-        sample in the batch.
-    """
     target = tf.convert_to_tensor(target)
     target = tf.cast(target, dtype="int32")
     output = tf.convert_to_tensor(output)
     output = tf.cast(output, dtype="float32")
     return tf.nn.ctc_loss(
         labels=target,
         logits=output,
         label_length=target_length,
         logit_length=output_length,
         blank_index=mask_index,
         logits_time_major=False,
     )
+
+
+def ctc_decode(
+    inputs,
+    sequence_length,
+    strategy,
+    beam_width=100,
+    top_paths=1,
+    merge_repeated=True,
+    mask_index=None,
+):
+    inputs = tf.convert_to_tensor(inputs)
+    inputs = tf.transpose(inputs, (1, 0, 2))
+
+    sequence_length = tf.convert_to_tensor(sequence_length, dtype="int32")
+    if strategy == "greedy":
+        return tf.nn.ctc_greedy_decoder(
+            inputs=inputs,
+            sequence_length=sequence_length,
+            merge_repeated=merge_repeated,
+            blank_index=mask_index,
+        )
+    elif strategy == "beam_search":
+        return tf.nn.ctc_beam_search_decoder(
+            inputs=inputs,
+            sequence_length=sequence_length,
+            beam_width=beam_width,
+            top_paths=top_paths,
+        )
+    else:
+        raise ValueError(
+            f"Invalid strategy {strategy}. Supported values are "
+            "'greedy' and 'beam_search'."
+        )
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1527,30 +1527,34 @@
         return x
     perm = [i for i in range(x.ndim) if i not in _source]
     for dest, src in sorted(zip(_destination, _source)):
         perm.insert(dest, src)
     return tf.transpose(x, perm)
 
 
-def nan_to_num(x):
+def nan_to_num(x, nan=0.0, posinf=None, neginf=None):
     x = convert_to_tensor(x)
 
     dtype = x.dtype
     dtype_as_dtype = tf.as_dtype(dtype)
     if dtype_as_dtype.is_integer or not dtype_as_dtype.is_numeric:
         return x
 
-    # Replace NaN with 0
-    x = tf.where(tf.math.is_nan(x), tf.constant(0, dtype), x)
+    # Replace NaN with `nan`
+    x = tf.where(tf.math.is_nan(x), tf.constant(nan, dtype), x)
 
-    # Replace positive infinity with dtype.max
-    x = tf.where(tf.math.is_inf(x) & (x > 0), tf.constant(dtype.max, dtype), x)
-
-    # Replace negative infinity with dtype.min
-    x = tf.where(tf.math.is_inf(x) & (x < 0), tf.constant(dtype.min, dtype), x)
+    # Replace positive infinity with `posinf` or `dtype.max`
+    if posinf is None:
+        posinf = dtype.max
+    x = tf.where(tf.math.is_inf(x) & (x > 0), tf.constant(posinf, dtype), x)
+
+    # Replace negative infinity with `neginf` or `dtype.min`
+    if neginf is None:
+        neginf = dtype.min
+    x = tf.where(tf.math.is_inf(x) & (x < 0), tf.constant(neginf, dtype), x)
 
     return x
 
 
 def ndim(x):
     x = convert_to_tensor(x)
     return x.ndim
@@ -2148,14 +2152,22 @@
     dtype_set = set([getattr(x, "dtype", type(x)) for x in xs])
     if len(dtype_set) > 1:
         dtype = dtypes.result_type(*dtype_set)
         xs = tree.map_structure(lambda x: convert_to_tensor(x, dtype), xs)
     return tf.concat(xs, axis=0)
 
 
+def vectorize(pyfunc):
+    @functools.wraps(pyfunc)
+    def wrapped(x):
+        return tf.vectorized_map(pyfunc, x)
+
+    return wrapped
+
+
 def where(condition, x1, x2):
     condition = tf.cast(condition, "bool")
     if x1 is not None and x2 is not None:
         if not isinstance(x1, (int, float)):
             x1 = convert_to_tensor(x1)
         if not isinstance(x2, (int, float)):
             x2 = convert_to_tensor(x2)
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/optimizer_distribute_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/optimizer_distribute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/saved_model_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/saved_model_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/core.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/image.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/layer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/linalg.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/math.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/nn.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/jax/nn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,471 +1,348 @@
-import torch
-import torch.nn.functional as tnn
+import jax
+import jax.experimental.sparse as jax_sparse
+import jax.numpy as jnp
+import numpy as np
+from jax import lax
+from jax import nn as jnn
 
-from keras.src import tree
 from keras.src.backend import standardize_data_format
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common.backend_utils import (
-    compute_conv_transpose_padding_args_for_torch,
+    compute_conv_transpose_padding_args_for_jax,
 )
 from keras.src.backend.config import epsilon
-from keras.src.backend.torch.core import cast
-from keras.src.backend.torch.core import convert_to_tensor
-from keras.src.backend.torch.core import get_device
-from keras.src.backend.torch.numpy import expand_dims
-from keras.src.backend.torch.numpy import maximum
-from keras.src.backend.torch.numpy import where
-from keras.src.utils.argument_validation import standardize_tuple
+from keras.src.backend.jax.core import cast
+from keras.src.backend.jax.core import convert_to_tensor
 
 
 def relu(x):
     x = convert_to_tensor(x)
-    return tnn.relu(x)
+    return jnn.relu(x)
 
 
 def relu6(x):
     x = convert_to_tensor(x)
-    return tnn.relu6(x)
+    return jnn.relu6(x)
 
 
 def sigmoid(x):
     x = convert_to_tensor(x)
-    return tnn.sigmoid(x)
+    return jnn.sigmoid(x)
 
 
 def tanh(x):
     x = convert_to_tensor(x)
-    return tnn.tanh(x)
+    return jnn.tanh(x)
 
 
 def softplus(x):
     x = convert_to_tensor(x)
-    return tnn.softplus(x)
+    return jnn.softplus(x)
 
 
 def softsign(x):
     x = convert_to_tensor(x)
-    return tnn.softsign(x)
+    return jnn.soft_sign(x)
 
 
 def silu(x):
     x = convert_to_tensor(x)
-    return tnn.silu(x)
+    return jnn.silu(x)
 
 
 def log_sigmoid(x):
     x = convert_to_tensor(x)
-    return tnn.logsigmoid(x)
+    return jnn.log_sigmoid(x)
 
 
 def leaky_relu(x, negative_slope=0.2):
     x = convert_to_tensor(x)
-    return tnn.leaky_relu(x, negative_slope=negative_slope)
+    return jnn.leaky_relu(x, negative_slope=negative_slope)
 
 
 def hard_sigmoid(x):
     x = convert_to_tensor(x)
-    return tnn.hardsigmoid(x)
+    return jnn.hard_sigmoid(x)
 
 
 def hard_silu(x):
     x = convert_to_tensor(x)
-    return tnn.hardswish(x)
+    return jnn.hard_silu(x)
 
 
 def elu(x, alpha=1.0):
     x = convert_to_tensor(x)
-    return tnn.elu(x, alpha)
+    return jnn.elu(x, alpha=alpha)
 
 
 def selu(x):
     x = convert_to_tensor(x)
-    return tnn.selu(x)
+    return jnn.selu(x)
 
 
 def gelu(x, approximate=True):
-    # TODO: torch.nn.gelu expects string approximate of `"none"` or `"tanh"`
     x = convert_to_tensor(x)
-    if approximate:
-        return tnn.gelu(x, approximate="tanh")
-    return tnn.gelu(x)
+    return jnn.gelu(x, approximate)
 
 
 def softmax(x, axis=-1):
     x = convert_to_tensor(x)
-    dtype = standardize_dtype(x.dtype)
-    # TODO: tnn.softmax doesn't support float16 using cpu
-    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
-        x = cast(x, "float32")
-    if axis is None:
-        # Unlike numpy, PyTorch will handle axis=None as axis=-1.
-        # We need this workaround for the reduction on every dim.
-        output = torch.reshape(x, [-1])
-        output = tnn.softmax(output, dim=-1)
-        output = torch.reshape(output, x.shape)
-    else:
-        output = tnn.softmax(x, dim=axis)
-    return cast(output, dtype)
+    return jnn.softmax(x, axis=axis)
 
 
 def log_softmax(x, axis=-1):
     x = convert_to_tensor(x)
-    dtype = standardize_dtype(x.dtype)
-    # TODO: tnn.log_softmax doesn't support float16 using cpu
-    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
-        x = cast(x, "float32")
-    if axis is None:
-        # Unlike numpy, PyTorch will handle axis=None as axis=-1.
-        # We need this workaround for the reduction on every dim.
-        output = torch.reshape(x, [-1])
-        output = tnn.log_softmax(output, dim=-1)
-        output = torch.reshape(output, x.shape)
-    else:
-        output = tnn.log_softmax(x, dim=axis)
-    return cast(output, dtype)
+    return jnn.log_softmax(x, axis=axis)
 
 
-def _compute_padding_length(
-    input_length, kernel_length, stride, dilation_rate=1
+def _convert_to_spatial_operand(
+    x,
+    num_spatial_dims,
+    data_format="channels_last",
+    include_batch_and_channels=True,
 ):
-    """Compute padding length along one dimension."""
-    total_padding_length = (
-        dilation_rate * (kernel_length - 1) - (input_length - 1) % stride
-    )
-    left_padding = total_padding_length // 2
-    right_padding = (total_padding_length + 1) // 2
-    return (left_padding, right_padding)
+    # Helper function that converts an operand to a spatial operand.
+    x = (x,) * num_spatial_dims if isinstance(x, int) else x
+    if not include_batch_and_channels:
+        return x
+    if data_format == "channels_last":
+        x = (1,) + x + (1,)
+    else:
+        x = (1,) + (1,) + x
+    return x
 
 
-def _apply_same_padding(
-    inputs, kernel_size, strides, operation_type, dilation_rate=1
+def _pool(
+    inputs,
+    initial_value,
+    reduce_fn,
+    pool_size,
+    strides=None,
+    padding="valid",
 ):
-    """Apply same padding to the input tensor.
+    """Helper function to define pooling functions.
 
-    This function will evaluate if the padding value is compatible with torch
-    functions. To avoid calling `pad()` as much as possible, which may cause
-    performance or memory issues, when compatible, it does not apply the padding
-    to the tensor, but returns the input tensor and the padding value to pass to
-    the torch functions. If not compatible, it returns the padded tensor and 0
-    as the padding value.
+    Args:
+        inputs: input data of shape `N+2`.
+        initial_value: the initial value for the reduction.
+        reduce_fn: a reduce function of the form `(T, T) -> T`.
+        pool_size: a sequence of `N` integers, representing the window size to
+            reduce over.
+        strides: a sequence of `N` integers, representing the inter-window
+            strides (default: `(1, ..., 1)`).
+        padding: either the string `same` or `valid`.
 
     Returns:
-        tensor: A padded tensor or the inputs.
-        padding: The padding value, ready to pass to the torch functions.
+        The output of the reduction for each window slice.
     """
-    spatial_shape = inputs.shape[2:]
-    num_spatial_dims = len(spatial_shape)
-    padding = ()
-
-    for i in range(num_spatial_dims):
-        if operation_type == "pooling":
-            padding_size = _compute_padding_length(
-                spatial_shape[i], kernel_size[i], strides[i]
-            )
-            mode = "replicate"
-        else:
-            dilation_rate = standardize_tuple(
-                dilation_rate, num_spatial_dims, "dilation_rate"
-            )
-            padding_size = _compute_padding_length(
-                spatial_shape[i], kernel_size[i], strides[i], dilation_rate[i]
-            )
-            mode = "constant"
-        padding = (padding_size,) + padding
-
-    if all([left == right for left, right in padding]):
-        return inputs, [left for left, _ in padding]
-
-    flattened_padding = tuple(
-        value for left_and_right in padding for value in left_and_right
-    )
-    return tnn.pad(inputs, pad=flattened_padding, mode=mode), 0
-
-
-def _transpose_spatial_inputs(inputs):
-    num_spatial_dims = inputs.ndim - 2
-    # Torch pooling does not support `channels_last` format, so
-    # we need to transpose to `channels_first` format.
-    if num_spatial_dims == 1:
-        inputs = torch.permute(inputs, (0, 2, 1))
-    elif num_spatial_dims == 2:
-        inputs = torch.permute(inputs, (0, 3, 1, 2))
-    elif num_spatial_dims == 3:
-        inputs = torch.permute(inputs, (0, 4, 1, 2, 3))
-    else:
+    if padding not in ("same", "valid"):
         raise ValueError(
-            "Inputs must have ndim=3, 4 or 5, "
-            "corresponding to 1D, 2D and 3D inputs. "
-            f"Received input shape: {inputs.shape}."
-        )
-    return inputs
-
-
-def _transpose_spatial_outputs(outputs):
-    # Undo the transpose in `_transpose_spatial_inputs`.
-    num_spatial_dims = len(outputs.shape) - 2
-    if num_spatial_dims == 1:
-        outputs = torch.permute(outputs, (0, 2, 1))
-    elif num_spatial_dims == 2:
-        outputs = torch.permute(outputs, (0, 2, 3, 1))
-    elif num_spatial_dims == 3:
-        outputs = torch.permute(outputs, (0, 2, 3, 4, 1))
-    return outputs
-
-
-def _transpose_conv_kernel(kernel):
-    # Torch requires conv kernel of format
-    # `(out_channels, in_channels, spatial_dims)`, we need to transpose.
-    num_spatial_dims = len(kernel.shape) - 2
-    if num_spatial_dims == 1:
-        kernel = torch.permute(kernel, (2, 1, 0))
-    elif num_spatial_dims == 2:
-        kernel = torch.permute(kernel, (3, 2, 0, 1))
-    elif num_spatial_dims == 3:
-        kernel = torch.permute(kernel, (4, 3, 0, 1, 2))
-    return kernel
+            f"Invalid padding '{padding}', must be 'same' or 'valid'."
+        )
+    padding = padding.upper()
+    return lax.reduce_window(
+        inputs,
+        initial_value,
+        reduce_fn,
+        pool_size,
+        strides,
+        padding,
+    )
 
 
 def max_pool(
     inputs,
     pool_size,
     strides=None,
     padding="valid",
     data_format=None,
 ):
-    inputs = convert_to_tensor(inputs)
-    num_spatial_dims = inputs.ndim - 2
-    pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
-    if strides is None:
-        strides = pool_size
-    else:
-        strides = standardize_tuple(strides, num_spatial_dims, "strides")
-
     data_format = standardize_data_format(data_format)
-    if data_format == "channels_last":
-        inputs = _transpose_spatial_inputs(inputs)
-
-    if padding == "same":
-        # Torch does not natively support `"same"` padding, we need to manually
-        # apply the right amount of padding to `inputs`.
-        inputs, padding = _apply_same_padding(
-            inputs, pool_size, strides, operation_type="pooling"
-        )
-    else:
-        padding = 0
-
-    device = get_device()
-    # Torch max pooling ops do not support symbolic tensors.
-    # Create a real tensor to execute the ops.
-    if device == "meta":
-        inputs = torch.empty(
-            size=inputs.shape, dtype=inputs.dtype, device="cpu"
-        )
-
-    if num_spatial_dims == 1:
-        outputs = tnn.max_pool1d(
-            inputs, kernel_size=pool_size, stride=strides, padding=padding
-        )
-    elif num_spatial_dims == 2:
-        outputs = tnn.max_pool2d(
-            inputs, kernel_size=pool_size, stride=strides, padding=padding
-        )
-    elif num_spatial_dims == 3:
-        outputs = tnn.max_pool3d(
-            inputs, kernel_size=pool_size, stride=strides, padding=padding
-        )
-    else:
-        raise ValueError(
-            "Inputs to pooling op must have ndim=3, 4 or 5, "
-            "corresponding to 1D, 2D and 3D inputs. "
-            f"Received input shape: {inputs.shape}."
-        )
-
-    outputs = outputs.to(device)
-    if data_format == "channels_last":
-        outputs = _transpose_spatial_outputs(outputs)
-    return outputs
+    num_spatial_dims = inputs.ndim - 2
+    pool_size = _convert_to_spatial_operand(
+        pool_size, num_spatial_dims, data_format
+    )
+    strides = pool_size if strides is None else strides
+    strides = _convert_to_spatial_operand(
+        strides, num_spatial_dims, data_format
+    )
+    return _pool(inputs, -jnp.inf, lax.max, pool_size, strides, padding)
 
 
 def average_pool(
     inputs,
     pool_size,
-    strides=None,
-    padding="valid",
+    strides,
+    padding,
     data_format=None,
 ):
-    inputs = convert_to_tensor(inputs)
+    data_format = standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
-    pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
-    if strides is None:
-        strides = pool_size
-    else:
-        strides = standardize_tuple(strides, num_spatial_dims, "strides")
+    pool_size = _convert_to_spatial_operand(
+        pool_size, num_spatial_dims, data_format
+    )
+    strides = pool_size if strides is None else strides
+    strides = _convert_to_spatial_operand(
+        strides, num_spatial_dims, data_format
+    )
+
+    pooled = _pool(inputs, 0.0, lax.add, pool_size, strides, padding)
+    if padding == "valid":
+        # Avoid the extra reduce_window.
+        return pooled / np.prod(pool_size)
+    else:
+        # Count the number of valid entries at each input point, then use that
+        # for computing average. Assumes that any two arrays of same shape will
+        # be padded the same. Avoid broadcasting on axis where pooling is
+        # skipped.
+        shape = [
+            (a if b != 1 else 1) for (a, b) in zip(inputs.shape, pool_size)
+        ]
+        window_counts = _pool(
+            jnp.ones(shape, inputs.dtype),
+            0.0,
+            lax.add,
+            pool_size,
+            strides,
+            padding,
+        )
+        return pooled / window_counts
+
+
+def _convert_to_lax_conv_dimension_numbers(
+    num_spatial_dims,
+    data_format="channels_last",
+    transpose=False,
+):
+    """Create a `lax.ConvDimensionNumbers` for the given inputs."""
+    num_dims = num_spatial_dims + 2
 
-    data_format = standardize_data_format(data_format)
     if data_format == "channels_last":
-        inputs = _transpose_spatial_inputs(inputs)
-    padding_value = 0
-    if padding == "same":
-        spatial_shape = inputs.shape[2:]
-        num_spatial_dims = len(spatial_shape)
-        padding_value = []
-        uneven_padding = []
-
-        for i in range(num_spatial_dims):
-            padding_size = _compute_padding_length(
-                spatial_shape[i], pool_size[i], strides[i]
-            )
-            # Torch only supports even padding on each dim, to replicate the
-            # behavior of "same" padding of `tf.keras` as much as possible,
-            # we need to pad evenly using the shorter padding.
-            padding_value.append(padding_size[0])
-            if padding_size[0] != padding_size[1]:
-                # Handle unequal padding.
-                # `torch.nn.pad` sets padding value in the reverse order.
-                uneven_padding = [0, 1] + uneven_padding
-        # Only call tnn.pad when needed.
-        if len(uneven_padding) > 0:
-            inputs = tnn.pad(inputs, uneven_padding)
+        spatial_dims = tuple(range(1, num_dims - 1))
+        inputs_dn = (0, num_dims - 1) + spatial_dims
+    else:
+        spatial_dims = tuple(range(2, num_dims))
+        inputs_dn = (0, 1) + spatial_dims
 
-    if num_spatial_dims == 1:
-        outputs = tnn.avg_pool1d(
-            inputs,
-            kernel_size=pool_size,
-            stride=strides,
-            padding=padding_value,
-            count_include_pad=False,
-        )
-    elif num_spatial_dims == 2:
-        outputs = tnn.avg_pool2d(
-            inputs,
-            kernel_size=pool_size,
-            stride=strides,
-            padding=padding_value,
-            count_include_pad=False,
-        )
-    elif num_spatial_dims == 3:
-        outputs = tnn.avg_pool3d(
-            inputs,
-            kernel_size=pool_size,
-            stride=strides,
-            padding=padding_value,
-            count_include_pad=False,
-        )
+    if transpose:
+        kernel_dn = (num_dims - 2, num_dims - 1) + tuple(range(num_dims - 2))
     else:
-        raise ValueError(
-            "Inputs to pooling op must have ndim=3, 4 or 5, "
-            "corresponding to 1D, 2D and 3D inputs. "
-            f"Received input shape: {inputs.shape}."
-        )
-    if data_format == "channels_last":
-        outputs = _transpose_spatial_outputs(outputs)
-    return outputs
+        kernel_dn = (num_dims - 1, num_dims - 2) + tuple(range(num_dims - 2))
+
+    return lax.ConvDimensionNumbers(
+        lhs_spec=inputs_dn, rhs_spec=kernel_dn, out_spec=inputs_dn
+    )
 
 
 def conv(
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    inputs = convert_to_tensor(inputs)
-    kernel = convert_to_tensor(kernel)
-    num_spatial_dims = inputs.ndim - 2
-    strides = standardize_tuple(strides, num_spatial_dims, "strides")
-
     data_format = standardize_data_format(data_format)
+    num_spatial_dims = inputs.ndim - 2
+    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
+        num_spatial_dims,
+        data_format,
+        transpose=False,
+    )
+    strides = _convert_to_spatial_operand(
+        strides,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
+    dilation_rate = _convert_to_spatial_operand(
+        dilation_rate,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
     if data_format == "channels_last":
-        inputs = _transpose_spatial_inputs(inputs)
-    # Transpose kernel from keras format to torch format.
-    kernel = _transpose_conv_kernel(kernel)
-    if padding == "same" and any(d != 1 for d in tree.flatten(strides)):
-        # Torch does not support this case in conv2d().
-        # Manually pad the tensor.
-        inputs, padding = _apply_same_padding(
-            inputs,
-            kernel.shape[2:],
-            strides,
-            operation_type="conv",
-            dilation_rate=dilation_rate,
-        )
-    channels = inputs.shape[1]
-    kernel_in_channels = kernel.shape[1]
+        channels = inputs.shape[-1]
+    else:
+        channels = inputs.shape[1]
+    kernel_in_channels = kernel.shape[-2]
     if channels % kernel_in_channels > 0:
         raise ValueError(
             "The number of input channels must be evenly divisible by "
-            f"kernel.shape[1]. Received: inputs.shape={inputs.shape}, "
-            f"kernel.shape={kernel.shape}"
-        )
-    groups = channels // kernel_in_channels
-    if num_spatial_dims == 1:
-        outputs = tnn.conv1d(
-            inputs,
-            kernel,
-            stride=strides,
-            dilation=dilation_rate,
-            groups=groups,
-            padding=padding,
-        )
-    elif num_spatial_dims == 2:
-        outputs = tnn.conv2d(
-            inputs,
-            kernel,
-            stride=strides,
-            dilation=dilation_rate,
-            groups=groups,
-            padding=padding,
-        )
-    elif num_spatial_dims == 3:
-        outputs = tnn.conv3d(
-            inputs,
-            kernel,
-            stride=strides,
-            dilation=dilation_rate,
-            groups=groups,
-            padding=padding,
-        )
-    else:
-        raise ValueError(
-            "Inputs to conv operation should have ndim=3, 4, or 5,"
-            "corresponding to 1D, 2D and 3D inputs. Received input "
-            f"shape: {inputs.shape}."
+            f"kernel's in_channels. Received input channels {channels} and "
+            f"kernel in_channels {kernel_in_channels}. "
         )
-
-    if data_format == "channels_last":
-        outputs = _transpose_spatial_outputs(outputs)
-    return outputs
+    feature_group_count = channels // kernel_in_channels
+    return jax.lax.conv_general_dilated(
+        convert_to_tensor(inputs),
+        convert_to_tensor(kernel),
+        strides,
+        padding,
+        rhs_dilation=dilation_rate,
+        dimension_numbers=dimension_numbers,
+        feature_group_count=feature_group_count,
+    )
 
 
 def depthwise_conv(
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    kernel = convert_to_tensor(kernel)
-    kernel = torch.reshape(
-        kernel, kernel.shape[:-2] + (1, kernel.shape[-2] * kernel.shape[-1])
+    data_format = standardize_data_format(data_format)
+    num_spatial_dims = inputs.ndim - 2
+    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
+        num_spatial_dims,
+        data_format,
+        transpose=False,
+    )
+    strides = _convert_to_spatial_operand(
+        strides,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
+    dilation_rate = _convert_to_spatial_operand(
+        dilation_rate,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
+    feature_group_count = (
+        inputs.shape[-1] if data_format == "channels_last" else inputs.shape[1]
+    )
+    kernel = jnp.reshape(
+        kernel,
+        kernel.shape[:-2] + (1, feature_group_count * kernel.shape[-1]),
+    )
+    return jax.lax.conv_general_dilated(
+        inputs,
+        kernel,
+        strides,
+        padding,
+        rhs_dilation=dilation_rate,
+        dimension_numbers=dimension_numbers,
+        feature_group_count=feature_group_count,
     )
-    return conv(inputs, kernel, strides, padding, data_format, dilation_rate)
 
 
 def separable_conv(
     inputs,
     depthwise_kernel,
     pointwise_kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
+    data_format = standardize_data_format(data_format)
     depthwise_conv_output = depthwise_conv(
         inputs,
         depthwise_kernel,
         strides,
         padding,
         data_format,
         dilation_rate,
@@ -485,117 +362,107 @@
     kernel,
     strides=1,
     padding="valid",
     output_padding=None,
     data_format=None,
     dilation_rate=1,
 ):
-    inputs = convert_to_tensor(inputs)
-    kernel = convert_to_tensor(kernel)
-    num_spatial_dims = inputs.ndim - 2
-    strides = standardize_tuple(strides, num_spatial_dims, "strides")
-
     data_format = standardize_data_format(data_format)
-    (
-        torch_padding,
-        torch_output_padding,
-    ) = compute_conv_transpose_padding_args_for_torch(
+    num_spatial_dims = inputs.ndim - 2
+    padding_values = compute_conv_transpose_padding_args_for_jax(
         input_shape=inputs.shape,
         kernel_shape=kernel.shape,
         strides=strides,
         padding=padding,
         output_padding=output_padding,
         dilation_rate=dilation_rate,
     )
-    if data_format == "channels_last":
-        inputs = _transpose_spatial_inputs(inputs)
-    # Transpose kernel from keras format to torch format.
-    kernel = _transpose_conv_kernel(kernel)
-    kernel_spatial_shape = kernel.shape[2:]
-    if isinstance(dilation_rate, int):
-        dilation_rate = [dilation_rate] * len(kernel_spatial_shape)
+    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
+        num_spatial_dims,
+        data_format,
+        transpose=False,
+    )
+    strides = _convert_to_spatial_operand(
+        strides,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
+    dilation_rate = _convert_to_spatial_operand(
+        dilation_rate,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
 
-    if num_spatial_dims == 1:
-        outputs = tnn.conv_transpose1d(
-            inputs,
-            kernel,
-            stride=strides,
-            padding=torch_padding,
-            output_padding=torch_output_padding,
-            dilation=dilation_rate,
-        )
-    elif num_spatial_dims == 2:
-        outputs = tnn.conv_transpose2d(
-            inputs,
-            kernel,
-            stride=strides,
-            padding=torch_padding,
-            output_padding=torch_output_padding,
-            dilation=dilation_rate,
-        )
-    elif num_spatial_dims == 3:
-        outputs = tnn.conv_transpose3d(
-            inputs,
-            kernel,
-            stride=strides,
-            padding=torch_padding,
-            output_padding=torch_output_padding,
-            dilation=dilation_rate,
-        )
-    else:
-        raise ValueError(
-            "Inputs to conv transpose operation should have ndim=3, 4, or 5,"
-            "corresponding to 1D, 2D and 3D inputs. Received input "
-            f"shape: {inputs.shape}."
-        )
-    if data_format == "channels_last":
-        outputs = _transpose_spatial_outputs(outputs)
-    return outputs
+    return jax.lax.conv_transpose(
+        inputs,
+        kernel,
+        strides,
+        padding=padding_values,
+        rhs_dilation=dilation_rate,
+        dimension_numbers=dimension_numbers,
+        transpose_kernel=True,
+    )
 
 
 def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
+    x = convert_to_tensor(x)
     if sparse:
-        raise ValueError("Unsupported value `sparse=True` with torch backend")
-    # Axis is the output axis. By default, PyTorch, outputs to last axis.
-    # If axis is not last, change output to axis and shift remaining elements.
-    x = convert_to_tensor(x, dtype=torch.long)
-
-    # Torch one_hot does not natively handle negative values, so we add some
-    # manual handling for negatives in the input to one_hot by using max(x, 0).
-    # The output will have some invalid results, so we set them back to 0 using
-    # `where` afterwards.
-    output = tnn.one_hot(maximum(x, 0), num_classes)
-    output = where(expand_dims(x, axis=-1) >= 0, output, 0)
-    output = convert_to_tensor(output, dtype=dtype)
-    dims = output.dim()
-    if axis != -1 and axis != dims:
-        new_axes_order = list(range(dims))
-        new_axes_order[axis] = -1  # Shifts output to axis position
-        # Shift remaining axes with offset by 1 since output moved to `axis`.
-        for ax in range(axis + 1, dims):
-            new_axes_order[ax] -= 1
-        output = output.permute(new_axes_order)
-    return output
+        if axis < 0:
+            axis = axis + len(x.shape) + 1
+        if dtype is None:
+            dtype = "float32"
+        # We deal with negative inputs by having zeros in the output although
+        # it's useless. It makes shapes static.
+        values = jnp.greater_equal(jnp.ravel(x), 0).astype(dtype)
+        values_count = values.shape[0]
+        indices = [jnp.arange(dim) for dim in x.shape]
+        indices = jnp.meshgrid(*indices, indexing="ij")
+        indices.insert(axis, jnp.maximum(x, 0))  # Deal with negative indices
+        indices = [a.reshape(values_count, 1).astype("int32") for a in indices]
+        indices = jnp.concatenate(indices, axis=1)
+        shape = list(x.shape)
+        shape.insert(axis, num_classes)
+        shape = tuple(shape)
+        return jax_sparse.BCOO(
+            (values, indices),
+            shape=shape,
+            indices_sorted=True,
+            unique_indices=True,
+        )
+    return jnn.one_hot(x, num_classes, axis=axis, dtype=dtype)
 
 
 def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
-    if sparse:
-        raise ValueError("Unsupported value `sparse=True` with torch backend")
     x = convert_to_tensor(x)
     reduction_axis = 1 if len(x.shape) > 1 else 0
-    outputs = torch.amax(
+    if sparse:
+        result = one_hot(
+            x, num_classes, axis=axis, dtype="int32", sparse=sparse
+        )
+        # JAX's BCOO does not support max reduction, use sum and compare with 0.
+        result = jax_sparse.bcoo_reduce_sum(result, axes=(reduction_axis,))
+        result = jax_sparse.bcoo_sum_duplicates(result)
+        values = jnp.greater_equal(result.data, 0).astype(dtype)
+        return jax_sparse.BCOO(
+            (values, result.indices),
+            shape=result.shape,
+            indices_sorted=True,
+            unique_indices=True,
+        )
+    return jnp.max(
         one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
-        dim=reduction_axis,
+        axis=reduction_axis,
     )
-    return outputs
 
 
 def categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = convert_to_tensor(target)
-    output = convert_to_tensor(output)
+    target = jnp.array(target)
+    output = jnp.array(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
@@ -603,163 +470,425 @@
         raise ValueError(
             "Arguments `target` and `output` must be at least rank 1. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
-        log_prob = tnn.log_softmax(output, dim=axis)
+        log_prob = jax.nn.log_softmax(output, axis=axis)
     else:
-        output = output / torch.sum(output, dim=axis, keepdim=True)
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = torch.log(output)
-    return -torch.sum(target * log_prob, dim=axis)
+        output = output / jnp.sum(output, axis, keepdims=True)
+        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = jnp.log(output)
+    return -jnp.sum(target * log_prob, axis=axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = convert_to_tensor(target, dtype=torch.long)
-    output = convert_to_tensor(output)
-
+    target = jnp.array(target, dtype="int32")
+    output = jnp.array(output)
     if len(target.shape) == len(output.shape) and target.shape[-1] == 1:
-        target = torch.squeeze(target, dim=-1)
+        target = jnp.squeeze(target, axis=-1)
 
     if len(output.shape) < 1:
         raise ValueError(
             "Argument `output` must be at least rank 1. "
             "Received: "
             f"output.shape={output.shape}"
         )
     if target.shape != output.shape[:-1]:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape "
             "up until the last dimension: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
     if from_logits:
-        log_prob = tnn.log_softmax(output, dim=axis)
+        log_prob = jax.nn.log_softmax(output, axis=axis)
     else:
-        output = output / torch.sum(output, dim=axis, keepdim=True)
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = torch.log(output)
-    target = one_hot(target, output.shape[axis], axis=axis)
-    return -torch.sum(target * log_prob, dim=axis)
+        output = output / jnp.sum(output, axis, keepdims=True)
+        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = jnp.log(output)
+    target = jnn.one_hot(target, output.shape[axis], axis=axis)
+    return -jnp.sum(target * log_prob, axis=axis)
 
 
 def binary_crossentropy(target, output, from_logits=False):
-    target = convert_to_tensor(target)
-    output = convert_to_tensor(output)
+    target = jnp.array(target)
+    output = jnp.array(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
-    # By default, PyTorch, does reduction of `sum` over all rows,
-    # change reduction to `none` to keep dim
+
     if from_logits:
-        return tnn.binary_cross_entropy_with_logits(
-            output, target, reduction="none"
-        )
-    else:
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
-        return tnn.binary_cross_entropy(output, target, reduction="none")
+        log_logits = jax.nn.log_sigmoid(output)
+        log_neg_logits = jax.nn.log_sigmoid(-output)
+        return -1.0 * target * log_logits - (1.0 - target) * log_neg_logits
+
+    output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+    bce = target * jnp.log(output)
+    bce += (1.0 - target) * jnp.log(1.0 - output)
+    return -bce
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     if synchronized:
         raise NotImplementedError(
-            "Argument synchronized=True is not supported with PyTorch."
+            "Argument synchronized=True is not supported with JAX."
         )
-    x = convert_to_tensor(x)
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
     ori_dtype = standardize_dtype(x.dtype)
-    if ori_dtype == "float16":
+    if ori_dtype in ("float16", "bfloat16"):
         need_cast = True
         x = cast(x, "float32")
 
-    mean = torch.mean(x, dim=axes, keepdim=True)
-
-    # The variance is computed using $Var = E[|x|^2] - |E[x]|^2$, It is faster
-    # but less numerically stable.
-    # Note: stop_gradient does not change the gradient to the mean, because that
-    # gradient is zero.
-    variance = torch.mean(
-        torch.square(x), dim=axes, keepdim=True
-    ) - torch.square(mean)
+    mean = jnp.mean(x, axes, keepdims=True)
+    variance = jnp.var(x, axis=axes, keepdims=True)
 
     if not keepdims:
-        mean = torch.squeeze(mean, axes)
-        variance = torch.squeeze(variance, axes)
+        mean = jnp.squeeze(mean, axes)
+        variance = jnp.squeeze(variance, axes)
     if need_cast:
         # avoid overflow and underflow when casting from float16 to float32
-        mean = torch.clip(
-            mean,
-            torch.finfo(torch.float16).min,
-            torch.finfo(torch.float16).max,
-        )
-        variance = torch.clip(
-            variance,
-            torch.finfo(torch.float16).min,
-            torch.finfo(torch.float16).max,
+        mean = jnp.clip(
+            mean, jnp.finfo(jnp.float16).min, jnp.finfo(jnp.float16).max
+        )
+        variance = jnp.clip(
+            variance, jnp.finfo(jnp.float16).min, jnp.finfo(jnp.float16).max
         )
         mean = cast(mean, ori_dtype)
         variance = cast(variance, ori_dtype)
     return mean, variance
 
 
 def batch_normalization(
     x, mean, variance, axis, offset=None, scale=None, epsilon=1e-3
 ):
-    x = convert_to_tensor(x)
-    mean = convert_to_tensor(mean)
-    variance = convert_to_tensor(variance)
-
     shape = [1] * len(x.shape)
     shape[axis] = mean.shape[0]
-    mean = torch.reshape(mean, shape)
-    variance = torch.reshape(variance, shape)
+    mean = jnp.reshape(mean, shape)
+    variance = jnp.reshape(variance, shape)
 
-    if offset is not None:
-        offset = convert_to_tensor(offset)
-        offset = torch.reshape(offset, shape)
-    else:
-        offset = torch.zeros_like(mean)
+    inv = jax.lax.rsqrt(variance + epsilon)
     if scale is not None:
-        scale = convert_to_tensor(scale)
-        scale = torch.reshape(scale, shape)
-    else:
-        scale = torch.ones_like(variance)
+        scale = jnp.reshape(scale, shape)
+        inv = inv * scale
 
-    return (
-        x.subtract(mean)
-        .mul_(variance.add(epsilon).rsqrt_().mul(scale))
-        .add_(offset)
-    )
+    res = -mean * inv
+    if offset is not None:
+        offset = jnp.reshape(offset, shape)
+        res = res + offset
+
+    return jnp.add(x * inv, res)
 
 
 def ctc_loss(
     target,
     output,
     target_length,
     output_length,
     mask_index=0,
 ):
-    target = convert_to_tensor(target)
-    output = convert_to_tensor(output)
-    target_length = convert_to_tensor(target_length)
-    output_length = convert_to_tensor(output_length)
-
-    output = torch.transpose(output, 1, 0)
-    logits = tnn.log_softmax(output, dim=-1)
-
-    return tnn.ctc_loss(
-        logits,
-        target,
-        output_length,
-        target_length,
-        blank=mask_index,
-        reduction="none",
+    batch_size, _, _ = output.shape
+    batch_size, max_target_length = target.shape
+
+    output = output.transpose((1, 0, 2))
+    target = target.transpose((1, 0)).astype("int32")
+
+    logits = jnn.log_softmax(output)
+    mgrid_t, mgrid_b = jnp.meshgrid(
+        jnp.arange(max_target_length), jnp.arange(batch_size)
+    )
+    logprobs_emit = logits[mgrid_t, mgrid_b, target[:, :, None]]
+    logprobs_mask = logits[:, :, mask_index]
+
+    logit_paddings = jnp.array(
+        jnp.arange(max_target_length) < output_length[:, None],
+        dtype=jnp.float32,
+    )
+
+    repeat = jnp.array(target[1:] == target[:-1])
+    repeat = jnp.pad(repeat, ((0, 1), (0, 0))).transpose((1, 0))
+
+    _logepsilon = -100000.0
+
+    def _iterate(prev, x):
+        prev_mask, prev_emit = prev
+        logprob_mask, logprob_emit, pad = x
+
+        prev_mask_orig = prev_mask
+        prev_mask = prev_mask.at[:, 1:].set(
+            jnp.logaddexp(prev_mask[:, 1:], prev_emit + _logepsilon * repeat),
+        )
+        emit = jnp.logaddexp(
+            prev_mask[:, :-1] + logprob_emit, prev_emit + logprob_emit
+        )
+
+        mask = prev_mask + logprob_mask[:, None]
+        mask = mask.at[:, 1:].set(
+            jnp.logaddexp(
+                mask[:, 1:],
+                prev_emit + logprob_mask[:, None] + _logepsilon * (1 - repeat),
+            )
+        )
+
+        pad = pad[:, None]
+        emit = emit * pad + prev_emit * (1 - pad)
+        mask = mask * pad + prev_mask_orig * (1 - pad)
+
+        return (mask, emit), (mask, emit)
+
+    mask_init = jnp.full((batch_size, max_target_length + 1), _logepsilon)
+    mask_init = mask_init.at[:, 0].set(0.0)
+    emit_init = jnp.full((batch_size, max_target_length), _logepsilon)
+
+    _, (alphas_mask, alphas_emit) = lax.scan(
+        _iterate,
+        (mask_init, emit_init),
+        (logprobs_mask, logprobs_emit, logit_paddings.transpose()),
+    )
+
+    last_alpha_mask = (
+        alphas_mask[-1]
+        .at[:, 1:]
+        .set(jnp.logaddexp(alphas_mask[-1, :, 1:], alphas_emit[-1]))
+    )
+
+    return -last_alpha_mask[jnp.arange(batch_size), target_length]
+
+
+def ctc_greedy_decode(
+    inputs,
+    sequence_length,
+    merge_repeated=True,
+    mask_index=None,
+):
+    inputs = jnp.array(inputs)
+    sequence_length = jnp.array(sequence_length, dtype=jnp.int32)
+
+    if mask_index is None:
+        mask_index = inputs.shape[-1] - 1
+
+    indices = jnp.argmax(inputs, axis=-1)
+    scores = jnp.max(inputs, axis=-1)
+
+    seqlen_mask = jnp.arange(inputs.shape[1])[None, :]
+    seqlen_mask = seqlen_mask >= sequence_length[:, None]
+
+    if merge_repeated:
+        repeat = indices[:, 1:] == indices[:, :-1]
+        repeat = jnp.pad(repeat, ((0, 0), (1, 0)))
+
+        indices = jnp.where(repeat, mask_index, indices)
+    else:
+        repeat = jnp.zeros_like(indices, dtype=bool)
+
+    indices = jnp.where(seqlen_mask, mask_index, indices)
+    indices = [batch[batch != mask_index] for batch in indices]
+    max_len = max(len(batch) for batch in indices)
+    indices = jnp.array(
+        [jnp.pad(batch, (0, max_len - len(batch))) for batch in indices]
+    )
+
+    scores = jnp.where(seqlen_mask, 0.0, scores)
+    scores = -jnp.sum(scores, axis=1)[:, None]
+
+    return [indices], scores
+
+
+def ctc_beam_search_decode(
+    inputs,
+    sequence_length,
+    beam_width=100,
+    top_paths=1,
+    mask_index=None,
+):
+    inputs = jnp.array(inputs)
+    sequence_length = jnp.array(sequence_length)
+
+    batch_size, max_seq_len, num_classes = inputs.shape
+    inputs = jnn.log_softmax(inputs)
+    seqlen_mask = jnp.arange(max_seq_len)[None, :] >= sequence_length[:, None]
+
+    if mask_index is None:
+        mask_index = num_classes - 1
+
+    # This is a workaround for the fact that jnp.argsort does not support
+    # the order parameter which is used to break ties when scores are equal.
+    # For compatibility with the tensorflow implementation, we flip the inputs
+    # and the mask_index, and then flip the classes back to the correct indices
+    inputs = jnp.flip(inputs, axis=2)
+    mask_index = num_classes - mask_index - 1
+
+    _pad = -1
+
+    init_paths = jnp.full(
+        (batch_size, 2 * beam_width, max_seq_len), _pad, dtype=jnp.int32
     )
+
+    num_init_paths = jnp.min(jnp.array([num_classes, beam_width]))
+    max_classes = jnp.argsort(inputs[:, 0], axis=1)[:, -num_init_paths:]
+    init_classes = jnp.where(max_classes == mask_index, _pad, max_classes)
+    init_paths = init_paths.at[:, :num_init_paths, 0].set(init_classes)
+
+    init_scores = (
+        jnp.full((batch_size, 2 * beam_width), -jnp.inf)
+        .at[:, :num_init_paths]
+        .set(jnp.take_along_axis(inputs[:, 0], max_classes, axis=1))
+    )
+    init_masked = init_paths[:, :, 0] == _pad
+
+    def _extend_paths(paths, scores, masked, x):
+        paths = jnp.repeat(paths, num_classes, axis=0)
+        scores = jnp.repeat(scores, num_classes)
+        masked = jnp.repeat(masked, num_classes)
+
+        path_tail_index = jnp.argmax(paths == _pad, axis=1)
+        paths_arange = jnp.arange(2 * beam_width * num_classes)
+        path_tails = paths[paths_arange, path_tail_index - 1]
+        path_tails = jnp.where(path_tail_index == 0, _pad, path_tails)
+
+        classes = jnp.arange(num_classes).at[mask_index].set(_pad)
+        classes = jnp.tile(classes, 2 * beam_width)
+
+        prev_masked = masked
+        masked = classes == _pad
+
+        masked_repeat = ~prev_masked & (path_tails == classes)
+        classes = jnp.where(masked_repeat, _pad, classes)
+        paths = paths.at[paths_arange, path_tail_index].set(classes)
+
+        x = jnp.tile(x, 2 * beam_width)
+        scores = scores + x
+
+        return paths, scores, masked
+
+    def _merge_scores(unique_inverse, scores):
+        scores_max = jnp.max(scores)
+        scores_exp = jnp.exp(scores - scores_max)
+        scores = jnp.zeros_like(scores).at[unique_inverse].add(scores_exp)
+        scores = jnp.log(scores) + scores_max
+        return scores
+
+    def _prune_paths(paths, scores, masked):
+        paths, unique_inverse = jnp.unique(
+            paths,
+            return_inverse=True,
+            size=2 * num_classes * beam_width,
+            axis=0,
+            fill_value=_pad,
+        )
+        unique_inverse = jnp.squeeze(unique_inverse, axis=1)
+
+        emit_scores = jnp.where(masked, -jnp.inf, scores)
+        mask_scores = jnp.where(masked, scores, -jnp.inf)
+
+        emit_scores = _merge_scores(unique_inverse, emit_scores)
+        mask_scores = _merge_scores(unique_inverse, mask_scores)
+
+        total_scores = jnp.logaddexp(emit_scores, mask_scores)
+        top_indices = jnp.argsort(total_scores)[-beam_width:]
+
+        paths = paths[top_indices]
+        emit_scores = emit_scores[top_indices]
+        mask_scores = mask_scores[top_indices]
+
+        paths = jnp.tile(paths, (2, 1))
+        scores = jnp.concatenate([emit_scores, mask_scores])
+        masked = jnp.concatenate(
+            [jnp.zeros(beam_width, bool), jnp.ones(beam_width, bool)]
+        )
+
+        return paths, scores, masked
+
+    def _decode_step(paths, scores, masked, x):
+        paths, scores, masked = _extend_paths(paths, scores, masked, x)
+        paths, scores, masked = _prune_paths(paths, scores, masked)
+        return paths, scores, masked
+
+    def _step(prev, x):
+        paths, scores, masked = prev
+        x, seqlen_mask = x
+
+        paths, scores, masked = lax.cond(
+            seqlen_mask,
+            lambda paths, scores, masked, x: (paths, scores, masked),
+            _decode_step,
+            paths,
+            scores,
+            masked,
+            x,
+        )
+
+        return (paths, scores, masked), None
+
+    def _decode_batch(
+        init_paths, init_scores, init_masked, inputs, seqlen_mask
+    ):
+        (paths, scores, masked), _ = lax.scan(
+            _step,
+            (init_paths, init_scores, init_masked),
+            (inputs[1:], seqlen_mask[1:]),
+        )
+
+        paths, unique_inverse = jnp.unique(
+            paths,
+            return_inverse=True,
+            size=2 * num_classes * beam_width,
+            axis=0,
+            fill_value=_pad,
+        )
+        unique_inverse = jnp.squeeze(unique_inverse, axis=1)
+        scores = _merge_scores(unique_inverse, scores)
+
+        top_indices = jnp.argsort(scores)[-top_paths:][::-1]
+        paths = paths[top_indices]
+        scores = scores[top_indices]
+
+        return paths, scores
+
+    paths, scores = jax.vmap(_decode_batch)(
+        init_paths, init_scores, init_masked, inputs, seqlen_mask
+    )
+
+    # convert classes back to the correct indices
+    paths = jnp.where(paths == _pad, _pad, num_classes - paths - 1)
+
+    lengths = jnp.argmax(paths == _pad, axis=2)
+    lengths = jnp.max(lengths, axis=0)
+    paths = jnp.where(paths == _pad, 0, paths)
+
+    paths = paths.transpose((1, 0, 2))
+    paths = [path[:, :length] for path, length in zip(paths, lengths)]
+
+    return paths, scores
+
+
+def ctc_decode(
+    inputs,
+    sequence_length,
+    strategy,
+    beam_width=100,
+    top_paths=1,
+    merge_repeated=True,
+    mask_index=None,
+):
+    if strategy == "greedy":
+        return ctc_greedy_decode(
+            inputs,
+            sequence_length,
+            merge_repeated=merge_repeated,
+            mask_index=mask_index,
+        )
+    else:
+        return ctc_beam_search_decode(
+            inputs,
+            sequence_length,
+            beam_width=beam_width,
+            top_paths=top_paths,
+            mask_index=mask_index,
+        )
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/numpy.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import builtins
+import functools
 import math
 
 import torch
 
 from keras.src.backend import KerasTensor
 from keras.src.backend import config
 from keras.src.backend.common import dtypes
@@ -990,17 +991,17 @@
 
 
 def moveaxis(x, source, destination):
     x = convert_to_tensor(x)
     return torch.moveaxis(x, source=source, destination=destination)
 
 
-def nan_to_num(x):
+def nan_to_num(x, nan=0.0, posinf=None, neginf=None):
     x = convert_to_tensor(x)
-    return torch.nan_to_num(x)
+    return torch.nan_to_num(x, nan=nan, posinf=posinf, neginf=neginf)
 
 
 def ndim(x):
     x = convert_to_tensor(x)
     return x.ndim
 
 
@@ -1408,14 +1409,22 @@
 
 
 def vstack(xs):
     xs = [convert_to_tensor(x) for x in xs]
     return torch.vstack(xs)
 
 
+def vectorize(pyfunc):
+    @functools.wraps(pyfunc)
+    def wrapped(x):
+        return torch.vmap(pyfunc, x)
+
+    return wrapped
+
+
 def where(condition, x1, x2):
     condition = convert_to_tensor(condition, dtype=bool)
     if x1 is not None and x2 is not None:
         x1 = convert_to_tensor(x1)
         x2 = convert_to_tensor(x2)
         return torch.where(condition, x1, x2)
     else:
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/random.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/rnn.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/trainer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/backup_and_restore_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/backup_and_restore_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback_list.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/callback_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/csv_logger_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/csv_logger_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/early_stopping_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/early_stopping_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/history.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/lambda_callback_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/lambda_callback_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/learning_rate_scheduler_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/learning_rate_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/model_checkpoint_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/model_checkpoint_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/reduce_lr_on_plateau_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/reduce_lr_on_plateau_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/remote_monitor_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/remote_monitor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/swap_ema_weights_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/swap_ema_weights_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/tensorboard_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/tensorboard_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/terminate_on_nan_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/callbacks/terminate_on_nan_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/constraints/constraints.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/constraints/constraints_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/constraints/constraints_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/boston_housing.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/california_housing.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar10.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar100.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/imdb.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/mnist.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/reuters.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/distribution/distribution_lib_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/distribution/distribution_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/dtype_policy_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/dtype_policies/dtype_policy_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/export/export_lib.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/export/export_lib_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/export/export_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/constant_initializers_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/initializers/constant_initializers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/initializer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/random_initializers.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/random_initializers_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/initializers/random_initializers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/activation.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/activation_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/activation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/elu.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/elu_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/elu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/leaky_relu_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/leaky_relu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/prelu.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/prelu_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/prelu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/relu.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/relu_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/relu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/softmax.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/softmax_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/activations/softmax_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/additive_attention_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/additive_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/attention.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/attention_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/grouped_query_attention_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/grouped_query_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/multi_head_attention_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/attention/multi_head_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv_transpose_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/conv_transpose_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/depthwise_conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/convolutional/separable_conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/dense.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/dense_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/dense_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/einsum_dense.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,17 @@
             self._input_expand_axes,
             self._kernel_expand_axes,
             self._input_squeeze_axes,
             self._kernel_squeeze_axes,
             self._custom_gradient_equation,
             self._kernel_reverse_transpose_axes,
         ) = _analyze_quantization_info(self.equation, self.input_spec.ndim)
-        self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
+        self.inputs_quantizer = quantizers.AbsMaxQuantizer(
+            axis=self._input_reduced_axes
+        )
         self._kernel = self.add_weight(
             name="kernel",
             shape=kernel_shape,
             initializer=kernel_initializer,
             dtype="int8",
             trainable=False,
         )
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/einsum_dense_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/einsum_dense_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,14 +466,36 @@
         layer.build((2, 4))
         self.assertEqual(backend.standardize_dtype(layer._kernel.dtype), "int8")
         self.assertEqual(
             backend.standardize_dtype(layer.kernel_scale.dtype), "float32"
         )
 
     @parameterized.named_parameters(
+        ("btnh,nhd->btd", "btnh,nhd->btd", (None, 8), (1, 2, 2, 4)),
+        ("btd,ndh->btnh", "btd,ndh->btnh", (None, 2, 8), (1, 2, 4)),
+        ("btd,df->btf", "btd,df->btf", (None, 4), (1, 2, 4)),
+    )
+    @pytest.mark.skipif(
+        backend.backend() == "numpy",
+        reason=f"{backend.backend()} does not support ops.custom_gradient.",
+    )
+    def test_quantize_int8_with_specific_equations(
+        self, equation, output_shape, input_shape
+    ):
+        layer = layers.EinsumDense(equation=equation, output_shape=output_shape)
+        layer.build(input_shape)
+        x = ops.random.uniform(input_shape)
+        y_float = layer(x)
+
+        layer.quantize("int8")
+        y_quantized = layer(x)
+        mse = ops.mean(ops.square(y_float - y_quantized))
+        self.assertLess(mse, 1e-3)  # A weak correctness test
+
+    @parameterized.named_parameters(
         ("int8", "int8"),
         ("float8", "float8"),
     )
     def test_quantize_on_unbuilt_layer(self, mode):
         layer = layers.EinsumDense(
             equation="ab,bcd->acd",
             output_shape=(8, 32),
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/embedding.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/embedding_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/embedding_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/identity.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/identity_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/identity_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/input_layer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/input_layer_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/input_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/lambda_layer_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/lambda_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/masking.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/masking_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/masking_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/wrapper.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/wrapper_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/core/wrapper_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/input_spec.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/layer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/layer_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/add.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/average.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/dot.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/maximum.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/merging_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/merging_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/minimum.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/multiply.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/subtract.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/batch_normalization_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/batch_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/group_normalization_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/group_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/layer_normalization_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/layer_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/spectral_normalization_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/spectral_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/unit_normalization_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/normalization/unit_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/average_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_average_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/global_max_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/pooling/max_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/audio_preprocessing_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/audio_preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/category_encoding_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/category_encoding_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/center_crop_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/center_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/discretization_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/discretization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/feature_space_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/feature_space_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashed_crossing_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/hashed_crossing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashing_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/hashing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/index_lookup_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/index_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/integer_lookup_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/integer_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/normalization_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_brightness_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_brightness_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_contrast_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_contrast_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_crop_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_flip_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_flip_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_rotation_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_rotation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_translation_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_translation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_zoom_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/random_zoom_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/rescaling_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/rescaling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/resizing_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/resizing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/string_lookup_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/string_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/text_vectorization_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/text_vectorization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/activity_regularization_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/activity_regularization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/alpha_dropout_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/alpha_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/dropout_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_dropout_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/gaussian_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_noise_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/gaussian_noise_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/spatial_dropout_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/regularization/spatial_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping1d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping2d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping3d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/cropping3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/flatten_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/flatten_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/permute_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/permute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/repeat_vector_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/repeat_vector_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/reshape_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/reshape_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling1d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling2d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling3d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/up_sampling3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding1d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding2d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding3d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/reshaping/zero_padding3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/bidirectional_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/bidirectional_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm1d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm2d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm3d_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/conv_lstm_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/dropout_rnn_cell_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/dropout_rnn_cell_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/gru.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/gru_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/gru_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/lstm_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/lstm_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/rnn_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/rnn_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/simple_rnn_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/simple_rnn_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/stacked_rnn_cells_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/stacked_rnn_cells_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/time_distributed_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/layers/rnn/time_distributed_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/backend.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/layers.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/losses.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/json_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/json_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/legacy_h5_format_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/legacy_h5_format_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/losses/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/losses/loss.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/losses/loss_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/losses/loss_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/losses/losses.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/losses/losses_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/losses/losses_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/accuracy_metrics_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/accuracy_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/confusion_metrics_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/confusion_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/f_score_metrics_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/f_score_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/hinge_metrics_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/hinge_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/iou_metrics_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/iou_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metric.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metric_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/metric_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/probabilistic_metrics_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/probabilistic_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/reduction_metrics_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/reduction_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/regression_metrics_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/metrics/regression_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/models/cloning.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/models/cloning_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/models/cloning_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/models/functional.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/models/functional_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/models/functional_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/models/model.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/models/model_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/models/model_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/models/sequential.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/models/sequential_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/models/sequential_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/models/variable_mapping.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/models/variable_mapping_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/models/variable_mapping_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/core.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/core_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/core_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/function.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/function_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/function_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/image.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/image_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/image_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/linalg.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/linalg_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/linalg_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/math.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/math_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/math_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/nn.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/nn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1869,14 +1869,74 @@
             target, output, target_length, output_length
         )
     return backend.nn.ctc_loss(
         target, output, target_length, output_length, mask_index
     )
 
 
+@keras_export(
+    [
+        "keras.ops.ctc_decode",
+        "keras.ops.nn.ctc_decode",
+    ]
+)
+def ctc_decode(
+    inputs,
+    sequence_lengths,
+    strategy,
+    beam_width=100,
+    top_paths=1,
+    merge_repeated=True,
+    mask_index=None,
+):
+    """Decodes the output of a CTC model.
+
+    Args:
+        inputs: A tensor of shape `(batch_size, max_length, num_classes)`
+            containing the logits (output of the model).
+        sequence_lengths: A tensor of shape `(batch_size,)` containing the
+            sequence lengths for the batch.
+        strategy: A string for the decoding strategy. Supported values are
+            `"greedy"` and `"beam_search"`.
+        beam_width: An integer scalar beam width used in beam search.
+            Defaults to 100.
+        top_paths: An integer scalar, the number of top paths to return.
+            Defaults to 1.
+        merge_repeated: A boolean scalar, whether to merge repeated
+            labels in the output. Defaults to `True`.
+        mask_index: An integer scalar, the index of the mask character in
+            the vocabulary. Defaults to `None`.
+
+    Returns:
+        A tuple containing:
+
+        - A list of decoded sequences.
+        - A list of the negative of the sum of the probability logits
+        (if strategy is `"greedy"`) or the log probability (if strategy is
+        `"beam_search"`) for each sequence.
+    """
+
+    if any_symbolic_tensors((inputs, sequence_lengths)):
+        raise NotImplementedError(
+            "CTC decoding is not supported with KerasTensors. Use it "
+            "inside the call() method of a Layer or the predict_step "
+            "method of a model."
+        )
+
+    return backend.nn.ctc_decode(
+        inputs=inputs,
+        sequence_length=sequence_lengths,
+        strategy=strategy,
+        beam_width=beam_width,
+        top_paths=top_paths,
+        merge_repeated=merge_repeated,
+        mask_index=mask_index,
+    )
+
+
 class Normalize(Operation):
     def __init__(self, axis=-1, order=2):
         super().__init__()
         self.axis = axis
         self.order = order
 
     def compute_output_spec(self, x):
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/nn_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/nn_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1899,14 +1899,75 @@
 
         label_length = np.array([3, 2])
         output_length = np.array([3, 2])
 
         result = knn.ctc_loss(labels, outputs, label_length, output_length)
         self.assertAllClose(result, np.array([3.4411672, 1.91680186]))
 
+    @pytest.mark.skipif(
+        backend.backend() not in ["tensorflow", "jax"],
+        reason="CTC decode only supported for TF and JAX backends",
+    )
+    def test_ctc_decode(self):
+        inputs = np.array(
+            [
+                [
+                    [0.1, 0.4, 0.2, 0.4],
+                    [0.3, 0.3, 0.4, 0.2],
+                    [0.3, 0.2, 0.4, 0.3],
+                ],
+                [
+                    [0.1, 0.4, 0.7, 0.2],
+                    [0.3, 0.3, 0.4, 0.1],
+                    [0.2, 0.1, 0.1, 0.5],
+                ],
+                [
+                    [0.1, 0.4, 0.2, 0.7],
+                    [0.3, 0.3, 0.2, 0.7],
+                    [0.3, 0.2, 0.4, 0.1],
+                ],
+            ]
+        )
+        labels = np.array([[1, 2], [2, 0], [0, 0]])
+        score_labels = np.array([[-1.2], [-1.6], [-0.7]])
+
+        (decoded,), scores = knn.ctc_decode(
+            inputs, sequence_lengths=[3, 3, 1], strategy="greedy"
+        )
+
+        self.assertAllClose(decoded, labels)
+        self.assertAllClose(scores, score_labels)
+
+        labels = [
+            np.array([[1, 2], [2, 0], [0, 0]]),
+            np.array([[2, 0], [2, 0], [1, 0]]),
+        ]
+        score_labels = np.array(
+            [
+                [-2.33578291, -2.44335217],
+                [-2.22499622, -2.25768432],
+                [-1.0633859, -1.3633859],
+            ]
+        )
+
+        beam_width = 4
+        top_paths = 2
+
+        decoded, scores = knn.ctc_decode(
+            inputs,
+            sequence_lengths=[3, 3, 1],
+            strategy="beam_search",
+            beam_width=beam_width,
+            top_paths=top_paths,
+        )
+
+        for i in range(top_paths):
+            self.assertAllClose(decoded[i], labels[i])
+        self.assertAllClose(scores, score_labels)
+
     def test_normalize(self):
         x = np.array([[1, 2, 3], [1, 2, 3]], dtype=np.float32)
         self.assertAllClose(
             knn.normalize(x, axis=None),
             [
                 [0.18898225, 0.3779645, 0.56694674],
                 [0.18898225, 0.3779645, 0.56694674],
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/node.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/node_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/node_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/numpy.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -3951,34 +3951,52 @@
     """
     if any_symbolic_tensors((x,)):
         return Moveaxis(source, destination).symbolic_call(x)
     return backend.numpy.moveaxis(x, source=source, destination=destination)
 
 
 class NanToNum(Operation):
+    def __init__(self, nan=0.0, posinf=None, neginf=None):
+        super().__init__()
+        self.nan = nan
+        self.posinf = posinf
+        self.neginf = neginf
+
     def call(self, x):
-        return backend.numpy.nan_to_num(x)
+        return backend.numpy.nan_to_num(
+            x, nan=self.nan, posinf=self.posinf, neginf=self.neginf
+        )
+
+    def compute_output_spec(self, x):
+        return KerasTensor(x.shape, dtype=x.dtype)
 
 
 @keras_export(
     [
         "keras.ops.nan_to_num",
         "keras.ops.numpy.nan_to_num",
     ]
 )
-def nan_to_num(x):
+def nan_to_num(x, nan=0.0, posinf=None, neginf=None):
     """Replace NaN with zero and infinity with large finite numbers.
 
     Args:
         x: Input data.
+        nan: Optional float or int. Value to replace `NaN` entries with.
+        posinf: Optional float or int.
+            Value to replace positive infinity with.
+        neginf: Optional float or int.
+            Value to replace negative infinity with.
 
     Returns:
         `x`, with non-finite values replaced.
     """
-    return backend.numpy.nan_to_num(x)
+    if any_symbolic_tensors((x,)):
+        return NanToNum(nan=nan, posinf=posinf, neginf=neginf).symbolic_call(x)
+    return backend.numpy.nan_to_num(x, nan=nan, posinf=posinf, neginf=neginf)
 
 
 class Ndim(Operation):
     def call(self, x):
         return backend.numpy.ndim(
             x,
         )
@@ -5393,14 +5411,43 @@
         Output tensor.
     """
     if any_symbolic_tensors((x1, x2)):
         return Vdot().symbolic_call(x1, x2)
     return backend.numpy.vdot(x1, x2)
 
 
+@keras_export(["keras.ops.vectorize", "keras.ops.numpy.vectorize"])
+def vectorize(pyfunc):
+    """Turn a function into a vectorized function.
+
+    Example:
+
+    ```python
+    def myfunc(a, b):
+        return a + b
+
+    vfunc = np.vectorize(myfunc)
+    y = vfunc([1, 2, 3, 4], 2)  # Returns Tensor([3, 4, 5, 6])
+    ```
+
+    Args:
+        pyfunc: Callable of a single tensor argument.
+
+    Returns:
+        A new function that applies `pyfunc` to every element
+        of its input along axis 0 (the batch axis).
+    """
+    if not callable(pyfunc):
+        raise ValueError(
+            "Expected argument `pyfunc` to be a callable. "
+            f"Received: pyfunc={pyfunc}"
+        )
+    return backend.numpy.vectorize(pyfunc)
+
+
 class Vstack(Operation):
     def call(self, xs):
         return backend.numpy.vstack(xs)
 
     def compute_output_spec(self, xs):
         first_shape = xs[0].shape
         total_size_on_axis = 0
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/numpy_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/numpy_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -4246,14 +4246,42 @@
 
         x = backend.KerasTensor((6,))
         condlist = [x < 3, x > 3]
         choicelist = [x, x**2]
         y = knp.select(condlist, choicelist, 42)
         self.assertEqual(y.shape, (6,))
 
+    def test_nan_to_num(self):
+        x = knp.array([1.0, np.nan, np.inf, -np.inf])
+        self.assertAllClose(
+            knp.nan_to_num(x), [1.0, 0.0, 3.402823e38, -3.402823e38]
+        )
+        self.assertAllClose(
+            knp.NanToNum()(x), [1.0, 0.0, 3.402823e38, -3.402823e38]
+        )
+        self.assertAllClose(
+            knp.nan_to_num(x, nan=2, posinf=3, neginf=4), [1.0, 2.0, 3.0, 4.0]
+        )
+        self.assertAllClose(
+            knp.NanToNum(nan=2, posinf=3, neginf=4)(x), [1.0, 2.0, 3.0, 4.0]
+        )
+
+        x = backend.KerasTensor((3, 4))
+        self.assertEqual(
+            knp.NanToNum(nan=2, posinf=3, neginf=4)(x).shape, (3, 4)
+        )
+
+    def test_vectorize(self):
+        def myfunc(a, b):
+            return a + b
+
+        vfunc = np.vectorize(myfunc)
+        y = vfunc([1, 2, 3, 4], 2)
+        self.assertAllClose(y, [3, 4, 5, 6])
+
 
 class NumpyArrayCreateOpsCorrectnessTest(testing.TestCase):
     def test_ones(self):
         self.assertAllClose(knp.ones([2, 3]), np.ones([2, 3]))
         self.assertAllClose(knp.Ones()([2, 3]), np.ones([2, 3]))
 
     def test_zeros(self):
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/operation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/operation_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/ops/symbolic_arguments_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/ops/symbolic_arguments_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adadelta.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adadelta_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adadelta_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adafactor.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adafactor_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adafactor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adagrad.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adagrad_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adagrad_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adam.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adam_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adam_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamax.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamax_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adamax_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamw.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamw_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/adamw_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/ftrl.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/ftrl_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/ftrl_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/lion.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/lion_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/lion_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/loss_scale_optimizer_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/loss_scale_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/nadam.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/nadam_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/nadam_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer_sparse_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/optimizer_sparse_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/optimizer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/rmsprop_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/rmsprop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/learning_rate_schedule_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/schedules/learning_rate_schedule_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/sgd.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/sgd_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/optimizers/sgd_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/quantizers.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/quantizers_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/quantizers/quantizers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/random/random.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/random/random_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/random/random_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/random/seed_generator.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/random/seed_generator_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/random/seed_generator_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/regularizers.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/regularizers_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/regularizers/regularizers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/saving/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/saving/object_registration.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/saving/object_registration_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/saving/object_registration_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_api.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_api_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/saving/saving_api_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_lib.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_lib_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/saving/saving_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/saving/serialization_lib.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/saving/serialization_lib_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/saving/serialization_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_case.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/testing/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/compile_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/compile_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/compile_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_data_adapter_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/array_data_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/generator_data_adapter_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/generator_data_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/py_dataset_adapter_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/py_dataset_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/epoch_iterator_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/epoch_iterator_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/trainer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/trainer_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/trainers/trainer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/tree/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/tree/optree_impl.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/tree/tree_api.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/tree/tree_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/tree/tree_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/__init__.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/argument_validation.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/audio_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/audio_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/backend_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/code_stats.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/code_stats_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/code_stats_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/dataset_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/dtype_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/dtype_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/dtype_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/file_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/file_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/file_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/image_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/io_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/io_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/io_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/jax_layer.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/jax_layer_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/jax_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/model_visualization.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/module_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/naming.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/naming_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/naming_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/numerical_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/numerical_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/numerical_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/progbar.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/python_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/python_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/python_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/rng_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/rng_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/rng_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/sequence_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/sequence_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/sequence_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/summary_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/summary_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/summary_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/text_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/text_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/tf_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/timeseries_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/timeseries_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/torch_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/torch_utils_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/torch_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/traceback_utils.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/tracking.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,18 +142,18 @@
         super().__init__(values or [])
 
     def append(self, value):
         if self.tracker:
             self.tracker.track(value)
         super().append(value)
 
-    def insert(self, value):
+    def insert(self, index, value):
         if self.tracker:
             self.tracker.track(value)
-        super().insert(value)
+        super().insert(index, value)
 
     def extend(self, values):
         if self.tracker:
             values = [self.tracker.track(v) for v in values]
         super().extend(values)
 
     def remove(self, value):
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras/src/utils/tracking_test.py` & `keras_nightly-3.3.0.dev2024042103/keras/src/utils/tracking_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.3.0.dev2024042103/keras_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.0.dev2024042003
+Version: 3.3.0.dev2024042103
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.3.0.dev2024042103/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/pyproject.toml` & `keras_nightly-3.3.0.dev2024042103/pyproject.toml`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042003/setup.py` & `keras_nightly-3.3.0.dev2024042103/setup.py`

 * *Files identical despite different names*

