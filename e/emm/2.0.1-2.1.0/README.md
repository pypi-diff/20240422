# Comparing `tmp/emm-2.0.1.tar.gz` & `tmp/emm-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emm-2.0.1.tar", last modified: Fri Feb 16 19:53:58 2024, max compression
+gzip compressed data, was "emm-2.1.0.tar", last modified: Mon Apr 22 07:53:12 2024, max compression
```

## Comparing `emm-2.0.1.tar` & `emm-2.1.0.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.258265 emm-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.226264 emm-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.230264 emm-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-16 19:53:50.000000 emm-2.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-16 19:53:50.000000 emm-2.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-16 19:53:50.000000 emm-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-16 19:53:50.000000 emm-2.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-16 19:53:50.000000 emm-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-16 19:53:50.000000 emm-2.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-02-16 19:53:58.258265 emm-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-02-16 19:53:50.000000 emm-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.226264 emm-2.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.230264 emm-2.0.1/docs/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      289 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/autogenerate.sh
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.234264 emm-2.0.1/docs/sphinx/source/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/api_index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.aggregation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.features.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.helper.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.indexing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.loggers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.rst
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.supervised_model.rst
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/emm.threshold.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/fitting.rst
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/parameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/persistence.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-02-16 19:53:50.000000 emm-2.0.1/docs/sphinx/source/spark.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.234264 emm-2.0.1/emm/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-02-16 19:53:50.000000 emm-2.0.1/emm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.238264 emm-2.0.1/emm/aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-16 19:53:50.000000 emm-2.0.1/emm/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-02-16 19:53:50.000000 emm-2.0.1/emm/aggregation/base_entity_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-02-16 19:53:50.000000 emm-2.0.1/emm/aggregation/pandas_entity_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-02-16 19:53:50.000000 emm-2.0.1/emm/aggregation/spark_entity_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.238264 emm-2.0.1/emm/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-16 19:53:50.000000 emm-2.0.1/emm/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-16 19:53:50.000000 emm-2.0.1/emm/base/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-16 19:53:50.000000 emm-2.0.1/emm/base/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.238264 emm-2.0.1/emm/data/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-16 19:53:50.000000 emm-2.0.1/emm/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-16 19:53:50.000000 emm-2.0.1/emm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-02-16 19:53:50.000000 emm-2.0.1/emm/data/create_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-02-16 19:53:50.000000 emm-2.0.1/emm/data/negative_data_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-02-16 19:53:50.000000 emm-2.0.1/emm/data/noiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-02-16 19:53:50.000000 emm-2.0.1/emm/data/prepare_name_pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-02-16 19:53:50.000000 emm-2.0.1/emm/data/unittest_sample_namepairs.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.238264 emm-2.0.1/emm/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-02-16 19:53:50.000000 emm-2.0.1/emm/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-16 19:53:50.000000 emm-2.0.1/emm/features/base_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-02-16 19:53:50.000000 emm-2.0.1/emm/features/features_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-02-16 19:53:50.000000 emm-2.0.1/emm/features/features_lef.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-02-16 19:53:50.000000 emm-2.0.1/emm/features/features_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-02-16 19:53:50.000000 emm-2.0.1/emm/features/features_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-02-16 19:53:50.000000 emm-2.0.1/emm/features/features_vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-02-16 19:53:50.000000 emm-2.0.1/emm/features/pandas_feature_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.242265 emm-2.0.1/emm/helper/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-16 19:53:50.000000 emm-2.0.1/emm/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-02-16 19:53:50.000000 emm-2.0.1/emm/helper/blocking_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-02-16 19:53:50.000000 emm-2.0.1/emm/helper/custom_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-02-16 19:53:50.000000 emm-2.0.1/emm/helper/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-16 19:53:50.000000 emm-2.0.1/emm/helper/sklearn_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-02-16 19:53:50.000000 emm-2.0.1/emm/helper/spark_custom_reader_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-02-16 19:53:50.000000 emm-2.0.1/emm/helper/spark_ml_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-02-16 19:53:50.000000 emm-2.0.1/emm/helper/spark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-02-16 19:53:50.000000 emm-2.0.1/emm/helper/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.242265 emm-2.0.1/emm/indexing/
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/base_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/pandas_candidate_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/pandas_cos_sim_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/pandas_naive_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/pandas_normalized_tfidf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/pandas_sni.py
--rw-r--r--   0 runner    (1001) docker     (127)    15490 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/spark_candidate_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/spark_character_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    31776 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/spark_cos_sim_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/spark_indexing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/spark_normalized_tfidf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/spark_sni.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-16 19:53:50.000000 emm-2.0.1/emm/indexing/spark_word_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.242265 emm-2.0.1/emm/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-16 19:53:50.000000 emm-2.0.1/emm/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-02-16 19:53:50.000000 emm-2.0.1/emm/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-02-16 19:53:50.000000 emm-2.0.1/emm/loggers/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-02-16 19:53:50.000000 emm-2.0.1/emm/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.246265 emm-2.0.1/emm/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-02-16 19:53:50.000000 emm-2.0.1/emm/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14514 2024-02-16 19:53:50.000000 emm-2.0.1/emm/pipeline/base_entity_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    38661 2024-02-16 19:53:50.000000 emm-2.0.1/emm/pipeline/pandas_entity_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    39097 2024-02-16 19:53:50.000000 emm-2.0.1/emm/pipeline/spark_entity_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.246265 emm-2.0.1/emm/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-02-16 19:53:50.000000 emm-2.0.1/emm/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-02-16 19:53:50.000000 emm-2.0.1/emm/preprocessing/abbreviation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-02-16 19:53:50.000000 emm-2.0.1/emm/preprocessing/base_name_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-02-16 19:53:50.000000 emm-2.0.1/emm/preprocessing/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-16 19:53:50.000000 emm-2.0.1/emm/preprocessing/pandas_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-02-16 19:53:50.000000 emm-2.0.1/emm/preprocessing/pandas_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-02-16 19:53:50.000000 emm-2.0.1/emm/preprocessing/spark_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-02-16 19:53:50.000000 emm-2.0.1/emm/preprocessing/spark_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-02-16 19:53:50.000000 emm-2.0.1/emm/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.246265 emm-2.0.1/emm/supervised_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-02-16 19:53:50.000000 emm-2.0.1/emm/supervised_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-02-16 19:53:50.000000 emm-2.0.1/emm/supervised_model/base_supervised_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-02-16 19:53:50.000000 emm-2.0.1/emm/supervised_model/pandas_supervised_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-02-16 19:53:50.000000 emm-2.0.1/emm/supervised_model/spark_supervised_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.246265 emm-2.0.1/emm/threshold/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-16 19:53:50.000000 emm-2.0.1/emm/threshold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-02-16 19:53:50.000000 emm-2.0.1/emm/threshold/threshold_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-16 19:53:50.000000 emm-2.0.1/emm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.254265 emm-2.0.1/emm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-02-16 19:53:58.000000 emm-2.0.1/emm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-02-16 19:53:58.000000 emm-2.0.1/emm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 19:53:58.000000 emm-2.0.1/emm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-16 19:53:58.000000 emm-2.0.1/emm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-16 19:53:58.000000 emm-2.0.1/emm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-02-16 19:53:50.000000 emm-2.0.1/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.246265 emm-2.0.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-02-16 19:53:50.000000 emm-2.0.1/notebooks/01-entity-matching-pandas-version.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-02-16 19:53:50.000000 emm-2.0.1/notebooks/02-entity-matching-spark-version.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-02-16 19:53:50.000000 emm-2.0.1/notebooks/03-entity-matching-training-pandas-version.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-02-16 19:53:50.000000 emm-2.0.1/notebooks/04-entity-matching-aggregation-pandas-version.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-02-16 19:53:50.000000 emm-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 19:53:58.258265 emm-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.246265 emm-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-16 19:53:50.000000 emm-2.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.246265 emm-2.0.1/tests/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:50.000000 emm-2.0.1/tests/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-02-16 19:53:50.000000 emm-2.0.1/tests/benchmark/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-02-16 19:53:50.000000 emm-2.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.250265 emm-2.0.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:50.000000 emm-2.0.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-02-16 19:53:50.000000 emm-2.0.1/tests/integration/test_artificial_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-02-16 19:53:50.000000 emm-2.0.1/tests/integration/test_em_add_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26454 2024-02-16 19:53:50.000000 emm-2.0.1/tests/integration/test_entity_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-02-16 19:53:50.000000 emm-2.0.1/tests/integration/test_indexers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-02-16 19:53:50.000000 emm-2.0.1/tests/integration/test_normalized_tfidf.py
--rw-r--r--   0 runner    (1001) docker     (127)    36602 2024-02-16 19:53:50.000000 emm-2.0.1/tests/integration/test_pandas_em.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-02-16 19:53:50.000000 emm-2.0.1/tests/integration/test_readme_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-02-16 19:53:50.000000 emm-2.0.1/tests/integration/test_spark_vs_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-02-16 19:53:50.000000 emm-2.0.1/tests/integration/test_supervised.py
--rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-02-16 19:53:50.000000 emm-2.0.1/tests/integration/test_training_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.250265 emm-2.0.1/tests/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:50.000000 emm-2.0.1/tests/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-02-16 19:53:50.000000 emm-2.0.1/tests/notebooks/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:58.254265 emm-2.0.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_abbreviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_carry_on_cols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_commonshorthands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_cos_sim_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_custom_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_entity_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_features_abbreviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_features_lef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_features_vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_name_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_negative_sample_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_threshold_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-02-16 19:53:50.000000 emm-2.0.1/tests/unit/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-02-16 19:53:50.000000 emm-2.0.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.351721 emm-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.323721 emm-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.327721 emm-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-22 07:53:05.000000 emm-2.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-22 07:53:05.000000 emm-2.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-22 07:53:05.000000 emm-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 07:53:05.000000 emm-2.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 07:53:05.000000 emm-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-22 07:53:05.000000 emm-2.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-22 07:53:12.351721 emm-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-22 07:53:05.000000 emm-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.323721 emm-2.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.327721 emm-2.1.0/docs/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      289 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/autogenerate.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.331721 emm-2.1.0/docs/sphinx/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/api_index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.aggregation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.helper.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.indexing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.loggers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.supervised_model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/emm.threshold.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/fitting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/persistence.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-22 07:53:05.000000 emm-2.1.0/docs/sphinx/source/spark.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.331721 emm-2.1.0/emm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-22 07:53:05.000000 emm-2.1.0/emm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.335721 emm-2.1.0/emm/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-22 07:53:05.000000 emm-2.1.0/emm/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-22 07:53:05.000000 emm-2.1.0/emm/aggregation/base_entity_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-04-22 07:53:05.000000 emm-2.1.0/emm/aggregation/pandas_entity_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-04-22 07:53:05.000000 emm-2.1.0/emm/aggregation/spark_entity_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.335721 emm-2.1.0/emm/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 07:53:06.000000 emm-2.1.0/emm/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-22 07:53:06.000000 emm-2.1.0/emm/base/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-22 07:53:06.000000 emm-2.1.0/emm/base/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.335721 emm-2.1.0/emm/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/create_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/negative_data_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/noiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/prepare_name_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-22 07:53:06.000000 emm-2.1.0/emm/data/unittest_sample_namepairs.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.335721 emm-2.1.0/emm/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/base_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/features_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/features_lef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/features_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/features_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/features_vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-04-22 07:53:06.000000 emm-2.1.0/emm/features/pandas_feature_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.339721 emm-2.1.0/emm/helper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/blocking_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/custom_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/sklearn_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/spark_custom_reader_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/spark_ml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/spark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-04-22 07:53:06.000000 emm-2.1.0/emm/helper/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.339721 emm-2.1.0/emm/indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/base_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/pandas_candidate_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/pandas_cos_sim_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/pandas_naive_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/pandas_normalized_tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/pandas_sni.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15490 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_candidate_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_character_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31776 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_cos_sim_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_indexing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_normalized_tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_sni.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-22 07:53:06.000000 emm-2.1.0/emm/indexing/spark_word_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.339721 emm-2.1.0/emm/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-22 07:53:06.000000 emm-2.1.0/emm/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-22 07:53:06.000000 emm-2.1.0/emm/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-22 07:53:06.000000 emm-2.1.0/emm/loggers/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-22 07:53:06.000000 emm-2.1.0/emm/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.339721 emm-2.1.0/emm/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-22 07:53:06.000000 emm-2.1.0/emm/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14514 2024-04-22 07:53:06.000000 emm-2.1.0/emm/pipeline/base_entity_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38661 2024-04-22 07:53:06.000000 emm-2.1.0/emm/pipeline/pandas_entity_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39097 2024-04-22 07:53:06.000000 emm-2.1.0/emm/pipeline/spark_entity_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/emm/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/abbreviation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/base_name_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/pandas_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/pandas_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/spark_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-22 07:53:06.000000 emm-2.1.0/emm/preprocessing/spark_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-22 07:53:06.000000 emm-2.1.0/emm/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/emm/supervised_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-22 07:53:06.000000 emm-2.1.0/emm/supervised_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-22 07:53:06.000000 emm-2.1.0/emm/supervised_model/base_supervised_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-22 07:53:06.000000 emm-2.1.0/emm/supervised_model/pandas_supervised_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-04-22 07:53:06.000000 emm-2.1.0/emm/supervised_model/spark_supervised_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/emm/threshold/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 07:53:06.000000 emm-2.1.0/emm/threshold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-04-22 07:53:06.000000 emm-2.1.0/emm/threshold/threshold_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-22 07:53:06.000000 emm-2.1.0/emm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.347721 emm-2.1.0/emm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-22 07:53:12.000000 emm-2.1.0/emm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-22 07:53:12.000000 emm-2.1.0/emm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 07:53:12.000000 emm-2.1.0/emm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-22 07:53:12.000000 emm-2.1.0/emm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 07:53:12.000000 emm-2.1.0/emm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-04-22 07:53:06.000000 emm-2.1.0/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    14338 2024-04-22 07:53:06.000000 emm-2.1.0/notebooks/01-entity-matching-pandas-version.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-04-22 07:53:06.000000 emm-2.1.0/notebooks/02-entity-matching-spark-version.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-04-22 07:53:06.000000 emm-2.1.0/notebooks/03-entity-matching-training-pandas-version.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-22 07:53:06.000000 emm-2.1.0/notebooks/04-entity-matching-aggregation-pandas-version.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-22 07:53:06.000000 emm-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 07:53:12.351721 emm-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 07:53:06.000000 emm-2.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.343721 emm-2.1.0/tests/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:06.000000 emm-2.1.0/tests/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-22 07:53:06.000000 emm-2.1.0/tests/benchmark/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-22 07:53:06.000000 emm-2.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.347721 emm-2.1.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_artificial_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_em_add_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26454 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_entity_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_indexers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_normalized_tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36602 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_pandas_em.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_readme_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_spark_vs_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_supervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-04-22 07:53:06.000000 emm-2.1.0/tests/integration/test_training_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.347721 emm-2.1.0/tests/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:06.000000 emm-2.1.0/tests/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-22 07:53:06.000000 emm-2.1.0/tests/notebooks/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:12.347721 emm-2.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_abbreviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_carry_on_cols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_commonshorthands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_cos_sim_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_custom_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_entity_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_features_abbreviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_features_lef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_features_vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_name_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_negative_sample_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_threshold_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-22 07:53:06.000000 emm-2.1.0/tests/unit/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-22 07:53:06.000000 emm-2.1.0/tests/utils.py
```

### Comparing `emm-2.0.1/.github/workflows/test.yml` & `emm-2.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/LICENSE` & `emm-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/NOTICE` & `emm-2.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/PKG-INFO` & `emm-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emm
-Version: 2.0.1
+Version: 2.1.0
 Summary: Entity Matching Model package
 Author-email: Max Baak <max.baak@ing.com>, Stephane Collot <stephane.collot@gmail.com>, Apoorva Mahajan <apoorva.mahajan@ing.com>, Tomasz Waleń <tomasz.walen@ing.com>, Simon Brugman <simon.brugman@ing.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: numpy>=1.20.1
@@ -14,15 +14,15 @@
 Requires-Dist: jinja2
 Requires-Dist: rapidfuzz<3.0.0
 Requires-Dist: regex
 Requires-Dist: urllib3
 Requires-Dist: recordlinkage
 Requires-Dist: cleanco>=2.2
 Requires-Dist: xgboost
-Requires-Dist: sparse-dot-topn>=0.3.3
+Requires-Dist: sparse-dot-topn>=1.1.1
 Requires-Dist: joblib
 Requires-Dist: pyarrow>=6.0.1
 Requires-Dist: requests
 Requires-Dist: unidecode
 Provides-Extra: spark
 Requires-Dist: pyspark>=3.1; python_version < "3.11" and extra == "spark"
 Requires-Dist: numpy<1.24.0; extra == "spark"
```

### Comparing `emm-2.0.1/README.md` & `emm-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/Makefile` & `emm-2.1.0/docs/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/README.rst` & `emm-2.1.0/docs/sphinx/README.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/make.bat` & `emm-2.1.0/docs/sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/conf.py` & `emm-2.1.0/docs/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/emm.aggregation.rst` & `emm-2.1.0/docs/sphinx/source/emm.aggregation.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/emm.data.rst` & `emm-2.1.0/docs/sphinx/source/emm.data.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/emm.features.rst` & `emm-2.1.0/docs/sphinx/source/emm.features.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/emm.helper.rst` & `emm-2.1.0/docs/sphinx/source/emm.helper.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/emm.indexing.rst` & `emm-2.1.0/docs/sphinx/source/emm.indexing.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/emm.pipeline.rst` & `emm-2.1.0/docs/sphinx/source/emm.pipeline.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/emm.preprocessing.rst` & `emm-2.1.0/docs/sphinx/source/emm.preprocessing.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/emm.rst` & `emm-2.1.0/docs/sphinx/source/emm.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/emm.supervised_model.rst` & `emm-2.1.0/docs/sphinx/source/emm.supervised_model.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/fitting.rst` & `emm-2.1.0/docs/sphinx/source/fitting.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/overview.rst` & `emm-2.1.0/docs/sphinx/source/overview.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/parameters.rst` & `emm-2.1.0/docs/sphinx/source/parameters.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/persistence.rst` & `emm-2.1.0/docs/sphinx/source/persistence.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/pipeline.rst` & `emm-2.1.0/docs/sphinx/source/pipeline.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/docs/sphinx/source/spark.rst` & `emm-2.1.0/docs/sphinx/source/spark.rst`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/__init__.py` & `emm-2.1.0/emm/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/aggregation/__init__.py` & `emm-2.1.0/emm/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/aggregation/base_entity_aggregation.py` & `emm-2.1.0/emm/aggregation/base_entity_aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,15 @@
         gt_uid_col: str = "gt_uid",
         name_col: str = "name_col",
         freq_col: str = "counterparty_account_count_distinct",
         output_col: str = "agg_score",
         preprocessed_col: str = "preprocessed",
         gt_name_col: str = "gt_name",
         gt_preprocessed_col: str = "gt_preprocessed",
+        correct_col: str = "correct",
         aggregation_method: Literal["max_frequency_nm_score", "mean_score"] = "max_frequency_nm_score",
         blacklist: list | None = None,
         positive_set_col: str = "positive_set",
     ) -> None:
         self.score_col = score_col
         self.account_col = account_col
         self.index_col = index_col
@@ -153,14 +154,15 @@
         self.gt_uid_col = gt_uid_col
         self.name_col = name_col
         self.freq_col = freq_col
         self.output_col = output_col
         self.preprocessed_col = preprocessed_col
         self.gt_name_col = gt_name_col
         self.gt_preprocessed_col = gt_preprocessed_col
+        self.correct_col = correct_col
         self.aggregation_method = aggregation_method
         self.blacklist = blacklist or []
         self.positive_set_col = positive_set_col
 
         # perform very basic preprocessing to blacklist, remove abbreviations, to lower, etc.
         self.blacklist = [preprocess(name) for name in self.blacklist]
         super().__init__()
```

### Comparing `emm-2.0.1/emm/aggregation/pandas_entity_aggregation.py` & `emm-2.1.0/emm/aggregation/pandas_entity_aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         gt_uid_col: str = "gt_uid",
         name_col: str = "name",
         freq_col: str = "counterparty_account_count_distinct",
         output_col: str = "agg_score",
         preprocessed_col: str = "preprocessed",
         gt_name_col: str = "gt_name",
         gt_preprocessed_col: str = "gt_preprocessed",
+        correct_col: str = "correct",
         aggregation_method: Literal["max_frequency_nm_score", "mean_score"] = "max_frequency_nm_score",
         blacklist: list[str] | None = None,
     ) -> None:
         """Pandas name-matching aggregation code
 
         Last and optional step in PandasEntityMatching.
 
@@ -76,14 +77,15 @@
             gt_uid_col: ground truth uid column, default is "gt_uid".
             name_col: name column, default is "name".
             freq_col: name frequency column, default is "counterparty_account_count_distinct".
             output_col: Name of column to store the final score
             preprocessed_col: Name of column of preprocessed input
             gt_name_col: ground truth name column, default is "gt_name".
             gt_preprocessed_col: column name of preprocessed ground truth names, default is "preprocessed".
+            correct_col: column indicating correct matches, if present. default is "correct". optional.
             aggregation_method: default is "max_frequency_nm_score", alternative is "mean_score".
             blacklist: blacklist of names to skip in clustering.
         """
         BaseEntityAggregation.__init__(
             self,
             score_col=score_col,
             account_col=account_col,
@@ -93,14 +95,15 @@
             gt_uid_col=gt_uid_col,
             name_col=name_col,
             freq_col=freq_col,
             output_col=output_col,
             preprocessed_col=preprocessed_col,
             gt_name_col=gt_name_col,
             gt_preprocessed_col=gt_preprocessed_col,
+            correct_col=correct_col,
             aggregation_method=aggregation_method,
             blacklist=blacklist or [],
         )
 
     def fit(self, X: pd.DataFrame, y: pd.Series | None = None) -> TransformerMixin:
         """Dummy function, no fitting is required."""
         return self
```

### Comparing `emm-2.0.1/emm/aggregation/spark_entity_aggregation.py` & `emm-2.1.0/emm/aggregation/spark_entity_aggregation.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import copy
 from typing import TYPE_CHECKING, Literal
 
 from pyspark.ml import Transformer
 from pyspark.ml.util import DefaultParamsReadable, DefaultParamsWritable
 from pyspark.sql.functions import col, lit
 from pyspark.sql.pandas.functions import PandasUDFType, pandas_udf
-from pyspark.sql.types import FloatType, IntegerType, StringType, StructField
+from pyspark.sql.types import BooleanType, FloatType, IntegerType, StringType, StructField
 
 from emm.aggregation.base_entity_aggregation import BaseEntityAggregation, matching_max_candidate
 from emm.helper.spark_custom_reader_writer import SparkReadable, SparkWriteable
 from emm.helper.spark_utils import set_spark_job_group
 from emm.loggers.logger import logger
 
 if TYPE_CHECKING:
@@ -45,15 +45,18 @@
 
     SERIALIZE_ATTRIBUTES = (
         "score_col",
         "index_col",
         "uid_col",
         "freq_col",
         "output_col",
-        "processed_col",
+        "preprocessed_col",
+        "gt_name_col",
+        "gt_preprocessed_col",
+        "correct_col",
         "aggregation_method",
         "blacklist",
     )
 
     def __init__(
         self,
         score_col: str = "nm_score",
@@ -62,14 +65,15 @@
         account_col: str = "account",
         name_col: str = "name",
         freq_col: str = "counterparty_account_count_distinct",
         output_col: str = "agg_score",
         preprocessed_col: str = "preprocessed",
         gt_name_col: str = "gt_name",
         gt_preprocessed_col: str = "gt_preprocessed",
+        correct_col: str = "correct",
         aggregation_method: Literal["max_frequency_nm_score", "mean_score"] = "max_frequency_nm_score",
         blacklist: list | None = None,
     ) -> None:
         """Spark name-matching aggregation code
 
         Last and optional step in SparkEntityMatching.
 
@@ -94,14 +98,15 @@
             account_col: account column, default is "account".
             name_col: name column, default is "name".
             freq_col: name frequency column, default is "counterparty_account_count_distinct".
             output_col: Name of column to store the final score
             preprocessed_col: Name of column of preprocessed input, default is "preprocessed".
             gt_name_col: ground truth name column, default is "gt_name".
             gt_preprocessed_col: column name of preprocessed ground truth names. default is "gt_preprocessed".
+            correct_col: column indicating correct matches, pass-thru if present. default is "correct". optional.
             aggregation_method: default is "max_frequency_nm_score", alternative is "mean_score".
             blacklist: blacklist of names to skip in clustering.
         """
         Transformer.__init__(self)
         BaseEntityAggregation.__init__(
             self,
             score_col=score_col,
@@ -111,14 +116,15 @@
             freq_col=freq_col,
             account_col=account_col,
             aggregation_method=aggregation_method,
             output_col=output_col,
             preprocessed_col=preprocessed_col,
             gt_name_col=gt_name_col,
             gt_preprocessed_col=gt_preprocessed_col,
+            correct_col=correct_col,
             blacklist=blacklist or [],
         )
 
     def _transform(self, dataframe):
         """Combine scores of a group of name-pair candidates that belong together.
 
         Natch a group of company names that belong together, to a company name in the ground truth.
@@ -141,28 +147,30 @@
         schema.add(StructField(self.output_col, FloatType(), True))
         schema.add(StructField(self.score_col, FloatType(), True))
         schema.add(StructField(self.name_col, StringType(), True))
         schema.add(StructField(self.preprocessed_col, StringType(), True))
         schema.add(StructField(self.freq_col, IntegerType(), True))
         schema.add(StructField(self.gt_name_col, StringType(), True))
         schema.add(StructField(self.gt_preprocessed_col, StringType(), True))
+        # pass through the correct-match column if present on training or test sets; useful for accuracy testing
+        if self.correct_col in dataframe.columns:
+            schema.add(StructField(self.correct_col, BooleanType(), True))
 
         @pandas_udf(schema, PandasUDFType.GROUPED_MAP)
         def matching_max_candidate_wrapper(_, df) -> pd.DataFrame:
             df = matching_max_candidate(
                 df,
                 group=gt_group,
                 score_col=self.score_col,
                 name_col=self.name_col,
                 account_col=self.account_col,
                 freq_col=self.freq_col,
                 output_col=self.output_col,
                 aggregation_method=self.aggregation_method,
             )
-
             return df[[c.name for c in schema]]
 
         # remove all irrelevant non-matches before applying account matching
         dataframe = dataframe.filter(col(self.gt_uid_col).isNotNull())
 
         # filter out all processed names that are in blacklist or empty.
         dataframe = self.remove_blacklisted_names(df=dataframe, preprocessed_col=self.preprocessed_col)
```

### Comparing `emm-2.0.1/emm/base/__init__.py` & `emm-2.1.0/emm/base/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/base/module.py` & `emm-2.1.0/emm/base/module.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/base/pipeline.py` & `emm-2.1.0/emm/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/data/__init__.py` & `emm-2.1.0/emm/data/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/data/create_data.py` & `emm-2.1.0/emm/data/create_data.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/data/negative_data_creation.py` & `emm-2.1.0/emm/data/negative_data_creation.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/data/noiser.py` & `emm-2.1.0/emm/data/noiser.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/data/prepare_name_pairs.py` & `emm-2.1.0/emm/data/prepare_name_pairs.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/data/unittest_sample_namepairs.csv.gz` & `emm-2.1.0/emm/data/unittest_sample_namepairs.csv.gz`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/features/__init__.py` & `emm-2.1.0/emm/features/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/features/base_feature_extractor.py` & `emm-2.1.0/emm/features/base_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/features/features_extra.py` & `emm-2.1.0/emm/features/features_extra.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/features/features_lef.py` & `emm-2.1.0/emm/features/features_lef.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/features/features_name.py` & `emm-2.1.0/emm/features/features_name.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/features/features_rank.py` & `emm-2.1.0/emm/features/features_rank.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/features/features_vocabulary.py` & `emm-2.1.0/emm/features/features_vocabulary.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/features/pandas_feature_extractor.py` & `emm-2.1.0/emm/features/pandas_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/helper/__init__.py` & `emm-2.1.0/emm/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/helper/blocking_functions.py` & `emm-2.1.0/emm/helper/blocking_functions.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/helper/custom_path.py` & `emm-2.1.0/emm/helper/custom_path.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/helper/io.py` & `emm-2.1.0/emm/helper/io.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/helper/sklearn_pipeline.py` & `emm-2.1.0/emm/helper/sklearn_pipeline.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/helper/spark_custom_reader_writer.py` & `emm-2.1.0/emm/helper/spark_custom_reader_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -210,14 +210,38 @@
             "sparkKW": self.spark_session_kw,
             "composition": self._composition,
             "file_format": self.file_format,
             "store_kws": self.store_kws,
         }
         return json.dumps(metadata, separators=[",", ":"])
 
+    def format(self, file_format: str):
+        """Set the file format of ground truth datasets that are saved
+
+        Args:
+            file_format: storage format of spark dataframes, default is parquet.
+
+        Returns:
+            self
+        """
+        self.file_format = file_format
+        return self
+
+    def options(self, **kwargs):
+        """Set the other file storage options of ground truth datasets that are saved
+
+        Args:
+            kwargs: storage kw-args, passed on to: sdf.write.save(path, format=self.file_format, **self.kwargs)
+
+        Returns:
+            self
+        """
+        self.store_kws = kwargs
+        return self
+
 
 class SparkCustomReader(MLReader):
     """Spark Custom class reader"""
 
     def __init__(self, cls) -> None:
         """Spark custom reader class
```

### Comparing `emm-2.0.1/emm/helper/spark_ml_pipeline.py` & `emm-2.1.0/emm/helper/spark_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/helper/spark_utils.py` & `emm-2.1.0/emm/helper/spark_utils.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/helper/util.py` & `emm-2.1.0/emm/helper/util.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/__init__.py` & `emm-2.1.0/emm/indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/base_indexer.py` & `emm-2.1.0/emm/indexing/base_indexer.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/pandas_candidate_selection.py` & `emm-2.1.0/emm/indexing/pandas_candidate_selection.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/pandas_cos_sim_matcher.py` & `emm-2.1.0/emm/indexing/pandas_cos_sim_matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing import Any, Callable, Generator, Literal
 
 import numpy as np
 import pandas as pd
 import scipy
 import scipy.sparse
 from sklearn.base import TransformerMixin
-from sparse_dot_topn import awesome_cossim_topn
+from sparse_dot_topn import sp_matmul_topn
 
 from emm.helper.util import groupby
 from emm.indexing.base_indexer import CosSimBaseIndexer
 from emm.indexing.pandas_normalized_tfidf import PandasNormalizedTfidfVectorizer
 from emm.loggers import Timer
 from emm.loggers.logger import logger
 
@@ -231,21 +231,21 @@
         assert X_enc.dtype == self.dtype
         logger.debug(f"calculating cossim gt_enc_t={gt_enc_t!r} X_enc={X_enc!r}")
         cs_list = []
         # Here we use chunks/partition_size just to get a progress bar
         # np.array_split cannot be used here due to sparse array X_enc
         X_chunks = [X_enc[i : i + self.partition_size] for i in range(0, X_enc.shape[0], self.partition_size)]
         for X_chunk in X_chunks:
-            cossim = awesome_cossim_topn(
+            cossim = sp_matmul_topn(
                 X_chunk,
                 gt_enc_t,
-                self.num_candidates,
-                self.cos_sim_lower_bound,
-                n_jobs=self.n_jobs,
-                use_threads=self.n_jobs > 1,
+                top_n=self.num_candidates,
+                threshold=self.cos_sim_lower_bound,
+                n_threads=self.n_jobs,
+                sort=True,
             )
             cs_list.append(cossim)
         return scipy.sparse.vstack(cs_list, dtype=self.dtype)
 
     def _spark_cossim(
         self, gt_enc_t: scipy.sparse.csr_matrix, X_enc: scipy.sparse.csr_matrix
     ) -> scipy.sparse.csr_matrix:
@@ -258,17 +258,15 @@
         # np.array_split cannot be used here due to sparse array X_enc
         X_chunks = [X_enc[i : i + self.partition_size] for i in range(0, X_enc.shape[0], self.partition_size)]
         rdd = sc.parallelize(X_chunks, len(X_chunks))
 
         def calc(
             row: scipy.sparse.csr_matrix, num_candidates: scipy.sparse.csr_matrix, cos_sim_lower_bound: float
         ) -> scipy.sparse.csr_matrix:
-            left = row
-            right = spark_gt.value
-            return awesome_cossim_topn(left, right, num_candidates, cos_sim_lower_bound)
+            return sp_matmul_topn(row, spark_gt.value, num_candidates, threshold=cos_sim_lower_bound)
 
         cs_rdd = rdd.map(
             partial(calc, num_candidates=self.num_candidates, cos_sim_lower_bound=self.cos_sim_lower_bound)
         )
         cs_list = cs_rdd.collect()
         return scipy.sparse.vstack(cs_list, dtype=self.dtype)
```

### Comparing `emm-2.0.1/emm/indexing/pandas_naive_indexer.py` & `emm-2.1.0/emm/indexing/pandas_naive_indexer.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/pandas_normalized_tfidf.py` & `emm-2.1.0/emm/indexing/pandas_normalized_tfidf.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,13 +158,14 @@
 
         Returns:
             normalized tfidf vectors of names
         """
         if effective_n_jobs(n_jobs) == 1:
             return self.transform(X=X)
 
+        chunk_size = int(np.ceil(len(X) / effective_n_jobs(n_jobs)))
+        X_chunks = [X.iloc[i : i + chunk_size] for i in range(0, len(X), chunk_size)]
+
         transform_splits = Parallel(n_jobs=n_jobs, backend="threading")(
-            delayed(self.transform)(X_split)
-            for X_split in np.array_split(X, effective_n_jobs(n_jobs))
-            if len(X_split) > 0
+            delayed(self.transform)(X_split) for X_split in X_chunks if len(X_split) > 0
         )
         return sp.vstack(transform_splits)
```

### Comparing `emm-2.0.1/emm/indexing/pandas_sni.py` & `emm-2.1.0/emm/indexing/pandas_sni.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/spark_candidate_selection.py` & `emm-2.1.0/emm/indexing/spark_candidate_selection.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/spark_character_tokenizer.py` & `emm-2.1.0/emm/indexing/spark_character_tokenizer.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/spark_cos_sim_matcher.py` & `emm-2.1.0/emm/indexing/spark_cos_sim_matcher.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/spark_indexing_utils.py` & `emm-2.1.0/emm/indexing/spark_indexing_utils.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/spark_normalized_tfidf.py` & `emm-2.1.0/emm/indexing/spark_normalized_tfidf.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/spark_sni.py` & `emm-2.1.0/emm/indexing/spark_sni.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/indexing/spark_word_tokenizer.py` & `emm-2.1.0/emm/indexing/spark_word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/loggers/__init__.py` & `emm-2.1.0/emm/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/loggers/logger.py` & `emm-2.1.0/emm/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/loggers/timer.py` & `emm-2.1.0/emm/loggers/timer.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/parameters.py` & `emm-2.1.0/emm/parameters.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/pipeline/__init__.py` & `emm-2.1.0/emm/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/pipeline/base_entity_matching.py` & `emm-2.1.0/emm/pipeline/base_entity_matching.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/pipeline/pandas_entity_matching.py` & `emm-2.1.0/emm/pipeline/pandas_entity_matching.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/pipeline/spark_entity_matching.py` & `emm-2.1.0/emm/pipeline/spark_entity_matching.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/preprocessing/__init__.py` & `emm-2.1.0/emm/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/preprocessing/abbreviation_util.py` & `emm-2.1.0/emm/preprocessing/abbreviation_util.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/preprocessing/base_name_preprocessor.py` & `emm-2.1.0/emm/preprocessing/base_name_preprocessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,31 +32,34 @@
 DEFINED_PIPELINE_DICT = {
     "preprocess_name": [
         "strip_accents_unicode",
         "replace_punctuation",
         "remove_newline",
         "strip_punctuation",  # normal way: remove punctuation, handle unicode, lower and trim
         "handle_lower_trim",
+        "remove_extra_space",
     ],
     "preprocess_with_punctuation": [
         "strip_accents_unicode",
         "replace_punctuation",
         "remove_newline",
         "insert_space_around_punctuation",  # punctuation will be kept. Must be work with
         "handle_lower_trim",
+        "remove_extra_space",
     ],
     "preprocess_merge_abbr": [
         "strip_accents_unicode",
         "replace_punctuation",
         "remove_newline",
         "merge_abbreviations",  # merge all abbreviation
         "merge_&",
         "strip_punctuation",
         "handle_lower_trim",
         "map_shorthands",
+        "remove_extra_space",
     ],
     "preprocess_merge_legal_abbr": [
         "strip_accents_unicode",
         "replace_punctuation",
         "remove_newline",
         "handle_lower",  # merge only legal form abbreviation
         "merge_legal_form_abbreviations",
```

### Comparing `emm-2.0.1/emm/preprocessing/functions.py` & `emm-2.1.0/emm/preprocessing/functions.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/preprocessing/pandas_functions.py` & `emm-2.1.0/emm/preprocessing/pandas_functions.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/preprocessing/pandas_preprocessor.py` & `emm-2.1.0/emm/preprocessing/pandas_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 from __future__ import annotations
 
 from functools import partial
 from typing import Any, Callable, Mapping
 
-import numpy as np
 import pandas as pd
 from sklearn.base import TransformerMixin
 
 from emm.loggers import Timer
 from emm.loggers.logger import logger
 from emm.preprocessing.base_name_preprocessor import AbstractPreprocessor, create_func_dict
 
@@ -105,18 +104,19 @@
         return self.transform(X, **extra_params)
 
     def _spark_apply_steps(
         self, series: pd.Series, preprocess_list: list[Any], func_dict: Mapping[str, Any], chunk_size: int = 10**4
     ) -> pd.Series:
         # Remark: 'chunk_size' is not the same as 'partition_size'
         # because here we just do name preprocessing and that can be done with much larger partitions
-        # than 'partition_size' that is designed to handle the fact that cosine similarity creates 10 times more data after the candidate generation
+        # than 'partition_size' that is designed to handle the fact that cosine similarity creates 10 times more data
+        # after the candidate generation
 
         with Timer("PandasPreprocessor._spark_apply_steps") as timer:
-            X_chunks = np.array_split(series, (len(series) + chunk_size - 1) // chunk_size)
+            X_chunks = [series.iloc[i : i + chunk_size] for i in range(0, len(series), chunk_size)]
             sc = self.spark_session.sparkContext
             rdd = sc.parallelize(X_chunks, len(X_chunks))
 
             def calc(chunk, funcs):
                 for func in funcs:
                     chunk = func(chunk)
                 return chunk.index.values, chunk.values
```

### Comparing `emm-2.0.1/emm/preprocessing/spark_functions.py` & `emm-2.1.0/emm/preprocessing/spark_functions.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/preprocessing/spark_preprocessor.py` & `emm-2.1.0/emm/preprocessing/spark_preprocessor.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/resources.py` & `emm-2.1.0/emm/resources.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/supervised_model/__init__.py` & `emm-2.1.0/emm/supervised_model/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/supervised_model/base_supervised_model.py` & `emm-2.1.0/emm/supervised_model/base_supervised_model.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/supervised_model/pandas_supervised_model.py` & `emm-2.1.0/emm/supervised_model/pandas_supervised_model.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/supervised_model/spark_supervised_model.py` & `emm-2.1.0/emm/supervised_model/spark_supervised_model.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/threshold/__init__.py` & `emm-2.1.0/emm/threshold/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/threshold/threshold_decision.py` & `emm-2.1.0/emm/threshold/threshold_decision.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm/version.py` & `emm-2.1.0/emm/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-VERSION = "2.0.1"
+VERSION = "2.1.0"
 
 __version__ = VERSION
```

### Comparing `emm-2.0.1/emm.egg-info/PKG-INFO` & `emm-2.1.0/emm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emm
-Version: 2.0.1
+Version: 2.1.0
 Summary: Entity Matching Model package
 Author-email: Max Baak <max.baak@ing.com>, Stephane Collot <stephane.collot@gmail.com>, Apoorva Mahajan <apoorva.mahajan@ing.com>, Tomasz Waleń <tomasz.walen@ing.com>, Simon Brugman <simon.brugman@ing.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: numpy>=1.20.1
@@ -14,15 +14,15 @@
 Requires-Dist: jinja2
 Requires-Dist: rapidfuzz<3.0.0
 Requires-Dist: regex
 Requires-Dist: urllib3
 Requires-Dist: recordlinkage
 Requires-Dist: cleanco>=2.2
 Requires-Dist: xgboost
-Requires-Dist: sparse-dot-topn>=0.3.3
+Requires-Dist: sparse-dot-topn>=1.1.1
 Requires-Dist: joblib
 Requires-Dist: pyarrow>=6.0.1
 Requires-Dist: requests
 Requires-Dist: unidecode
 Provides-Extra: spark
 Requires-Dist: pyspark>=3.1; python_version < "3.11" and extra == "spark"
 Requires-Dist: numpy<1.24.0; extra == "spark"
```

### Comparing `emm-2.0.1/emm.egg-info/SOURCES.txt` & `emm-2.1.0/emm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/emm.egg-info/requires.txt` & `emm-2.1.0/emm.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jinja2
 rapidfuzz<3.0.0
 regex
 urllib3
 recordlinkage
 cleanco>=2.2
 xgboost
-sparse-dot-topn>=0.3.3
+sparse-dot-topn>=1.1.1
 joblib
 pyarrow>=6.0.1
 requests
 unidecode
 
 [dev]
 pre-commit
```

### Comparing `emm-2.0.1/example.py` & `emm-2.1.0/example.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/notebooks/01-entity-matching-pandas-version.ipynb` & `emm-2.1.0/notebooks/01-entity-matching-pandas-version.ipynb`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/notebooks/02-entity-matching-spark-version.ipynb` & `emm-2.1.0/notebooks/02-entity-matching-spark-version.ipynb`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/notebooks/03-entity-matching-training-pandas-version.ipynb` & `emm-2.1.0/notebooks/03-entity-matching-training-pandas-version.ipynb`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/notebooks/04-entity-matching-aggregation-pandas-version.ipynb` & `emm-2.1.0/notebooks/04-entity-matching-aggregation-pandas-version.ipynb`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/pyproject.toml` & `emm-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,15 @@
   "rapidfuzz<3.0.0",
   "regex",
   "urllib3",
   "recordlinkage",
   "cleanco>=2.2",
   # It is important to fix the version of xgboost for reproducible classification scores
   "xgboost",
-  # Necessary to fix numpy issue
-  "sparse-dot-topn>=0.3.3",
+  "sparse-dot-topn>=1.1.1",
   "joblib",
   "pyarrow>=6.0.1", # seems to work with spark 3.1.2 - 3.3.1
   "requests",
   "unidecode"
 ]
 dynamic = ["version"]
```

### Comparing `emm-2.0.1/tests/__init__.py` & `emm-2.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/benchmark/test_bench.py` & `emm-2.1.0/tests/benchmark/test_bench.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/conftest.py` & `emm-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/integration/test_artificial_integration.py` & `emm-2.1.0/tests/integration/test_artificial_integration.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/integration/test_em_add_model.py` & `emm-2.1.0/tests/integration/test_em_add_model.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/integration/test_entity_matching.py` & `emm-2.1.0/tests/integration/test_entity_matching.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/integration/test_indexers.py` & `emm-2.1.0/tests/integration/test_indexers.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         PandasSortedNeighbourhoodIndexer(input_col="preprocessed", window_length=5),
     ]
     em_params = {"name_only": True, "entity_id_col": "id", "name_col": "name", "indexers": indexers}
     p = PandasEntityMatching(em_params)
     p.fit(gt)
     res = p.transform(names)
 
-    assert len(res) == 118
+    assert len(res) == 117
 
 
 @pytest.mark.skipif(not spark_installed, reason="spark not found")
 def test_indexer_objects_spark(kvk_training_dataset, spark_session):
     gt, names = split_gt_and_names(kvk_training_dataset)
     gt = gt[:1000]
     names = names[:10]
@@ -235,15 +235,15 @@
         SparkSortedNeighbourhoodIndexer(window_length=5),
     ]
     em_params = {"name_only": True, "entity_id_col": "id", "name_col": "name", "indexers": indexers}
     p = SparkEntityMatching(em_params)
     p.fit(sgt)
     res = p.transform(snames)
 
-    assert res.count() == 118
+    assert res.count() == 117
 
 
 def test_naive_indexer_pandas(kvk_training_dataset):
     gt, names = split_gt_and_names(kvk_training_dataset)
     gt = gt[:10]
     names = names[:10]
```

### Comparing `emm-2.0.1/tests/integration/test_normalized_tfidf.py` & `emm-2.1.0/tests/integration/test_normalized_tfidf.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/integration/test_pandas_em.py` & `emm-2.1.0/tests/integration/test_pandas_em.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/integration/test_readme_example.py` & `emm-2.1.0/tests/integration/test_readme_example.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/integration/test_spark_vs_pandas.py` & `emm-2.1.0/tests/integration/test_spark_vs_pandas.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/integration/test_supervised.py` & `emm-2.1.0/tests/integration/test_supervised.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         "X_feat_score_0_dist_to_max",
         "X_feat_score_0_dist_to_min",
         "X_feat_score_0_ptp",
         "X_feat_score_0_diff_to_next",
         "X_feat_score_0_diff_to_prev",
     ]
 
-    assert len(res) == 118
+    assert len(res) == 117
     assert all(feat in res.columns for feat in features)
     assert (res["X_feat_norm_jaro"] > 0).all()
 
 
 @pytest.mark.skipif(not spark_installed, reason="spark not found")
 def test_return_sm_features_spark(kvk_training_dataset, spark_session):
     gt, names = split_gt_and_names(kvk_training_dataset)
@@ -198,9 +198,9 @@
         "X_feat_score_0_dist_to_max",
         "X_feat_score_0_dist_to_min",
         "X_feat_score_0_ptp",
         "X_feat_score_0_diff_to_next",
         "X_feat_score_0_diff_to_prev",
     ]
 
-    assert res.count() == 118
+    assert res.count() == 117
     assert all(feat in res.columns for feat in features)
```

### Comparing `emm-2.0.1/tests/integration/test_training_classifier.py` & `emm-2.1.0/tests/integration/test_training_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         ],
     }
     p = PandasEntityMatching(em_params)
     p.fit(gt)
 
     p.increase_window_by_one_step()
     res = p.transform(names)
-    assert len(res) == 327
+    assert len(res) == 324
     assert res["rank_0"].max() == 11
     assert res["rank_1"].max() == 3
     assert res["rank_1"].min() == -3
 
 
 def test_decrease_window_pandas(kvk_training_dataset):
     gt, names = split_gt_and_names(kvk_training_dataset)
@@ -69,15 +69,15 @@
         ],
     }
     p = PandasEntityMatching(em_params)
     p.fit(gt)
 
     p.decrease_window_by_one_step()
     res = p.transform(names)
-    assert len(res) == 227
+    assert len(res) == 226
     assert res["rank_0"].max() == 9
     assert res["rank_1"].max() == 1
     assert res["rank_1"].min() == -1
 
 
 @pytest.mark.skipif(not spark_installed, reason="spark not found")
 def test_increase_window_spark(kvk_training_dataset, spark_session):
@@ -98,15 +98,15 @@
         ],
     }
     p = SparkEntityMatching(em_params)
     p.fit(sgt)
 
     p.increase_window_by_one_step()
     res = p.transform(snames)
-    assert res.count() == 327
+    assert res.count() == 324
 
 
 @pytest.mark.skipif(not spark_installed, reason="spark not found")
 def test_decrease_window_spark(kvk_training_dataset, spark_session):
     gt, names = split_gt_and_names(kvk_training_dataset)
     gt = gt[:1000]
     names = names[:25]
@@ -124,15 +124,15 @@
         ],
     }
     p = SparkEntityMatching(em_params)
     p.fit(sgt)
 
     p.decrease_window_by_one_step()
     res = p.transform(snames)
-    assert res.count() == 227
+    assert res.count() == 226
 
 
 def test_create_name_pairs_pandas(kvk_training_dataset):
     gt, names = split_gt_and_names(kvk_training_dataset)
     gt = gt[:1000]
     names = names[:25]
 
@@ -147,21 +147,21 @@
     }
     p = PandasEntityMatching(em_params)
     p.fit(gt)
 
     train = p.create_training_name_pairs(names, create_negative_sample_fraction=0.5, random_seed=42)
 
     assert isinstance(train, pd.DataFrame)
-    assert len(train) == 277
+    assert len(train) == 274
     assert "correct" in train.columns
     assert "no_candidate" in train.columns
     assert "positive_set" in train.columns
     vc = train["positive_set"].value_counts().to_dict()
-    assert vc[False] == 152
-    assert vc[True] == 125
+    assert vc[False] == 148
+    assert vc[True] == 126
 
 
 @pytest.mark.skipif(not spark_installed, reason="spark not found")
 def test_create_name_pairs_spark(kvk_training_dataset, spark_session):
     gt, names = split_gt_and_names(kvk_training_dataset)
     gt = gt[:1000]
     names = names[:25]
@@ -180,21 +180,21 @@
     }
     p = SparkEntityMatching(em_params)
     p.fit(sgt)
 
     train = p.create_training_name_pairs(snames, create_negative_sample_fraction=0.5, random_seed=42)
 
     assert isinstance(train, pd.DataFrame)
-    assert len(train) == 277
+    assert len(train) == 274
     assert "correct" in train.columns
     assert "no_candidate" in train.columns
     assert "positive_set" in train.columns
     vc = train["positive_set"].value_counts().to_dict()
-    assert vc[False] == 152
-    assert vc[True] == 125
+    assert vc[False] == 148
+    assert vc[True] == 126
 
 
 def test_fit_classifier_pandas(kvk_training_dataset):
     gt, names = split_gt_and_names(kvk_training_dataset)
     gt = gt[:1000]
     train_names = names[:100]
     test_names = names[100:110]
```

### Comparing `emm-2.0.1/tests/notebooks/test_notebooks.py` & `emm-2.1.0/tests/notebooks/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_abbreviations.py` & `emm-2.1.0/tests/unit/test_abbreviations.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_carry_on_cols.py` & `emm-2.1.0/tests/unit/test_carry_on_cols.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_commonshorthands.py` & `emm-2.1.0/tests/unit/test_commonshorthands.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_cos_sim_matcher.py` & `emm-2.1.0/tests/unit/test_cos_sim_matcher.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_custom_path.py` & `emm-2.1.0/tests/unit/test_custom_path.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_data.py` & `emm-2.1.0/tests/unit/test_data.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_entity_aggregation.py` & `emm-2.1.0/tests/unit/test_entity_aggregation.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_feature_extractor.py` & `emm-2.1.0/tests/unit/test_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_features_abbreviations.py` & `emm-2.1.0/tests/unit/test_features_abbreviations.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_features_lef.py` & `emm-2.1.0/tests/unit/test_features_lef.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_features_vocabulary.py` & `emm-2.1.0/tests/unit/test_features_vocabulary.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_name_preprocessing.py` & `emm-2.1.0/tests/unit/test_name_preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,21 +52,21 @@
             ["Tzu-Sun_BV.a;b,c_ä", "ąćęłńóśźżĄĆĘŁŃÓŚŹŻ", "Café"],
             ["Tzu-Sun_BV.a;b,c_a", "acelnoszzACELNOSZZ", "Cafe"],
         ),
         ("merge_&", ["xyz & abc C&D"], ["xyz & abc CD"]),
         (
             "preprocess_name",
             ["Tzu-Sun_BV.a;b,c_ä", "Tzu-Sun_BV  morethan1space"],
-            ["tzu sun bv a b c a", "tzu sun bv  morethan1space"],
+            ["tzu sun bv a b c a", "tzu sun bv morethan1space"],
         ),
         ("preprocess_with_punctuation", ["Tzu-Sun_BV.a;b,c_ä"], ["tzu - sun _ bv . a ; b , c _ a"]),
         (
             "preprocess_merge_abbr",
             ["Tzu-Sun_B.V.a;b,c_ä", "Z. S. B. V.", "Z Sun B V", "Z. Sun B.V.", "Z Sun B.V"],
-            ["tzu sun b v a b c a", "zsbv", "z sun bv", "z  sun bv", "z sun bv"],
+            ["tzu sun b v a b c a", "zsbv", "z sun bv", "z sun bv", "z sun bv"],
         ),
         (
             "preprocess_merge_legal_abbr",
             [
                 "Tzu-Sun B. V.",
                 "Tzu-Sun B.V",
                 "Tzu-Sun B V",
@@ -189,15 +189,15 @@
             ]
         }
     )
 
     out = pandas_preprocessor.transform(df)["preprocessed"].tolist()
     expect = [
         "b n consult b v",
-        "stichting vrienden van laurens  pax intrantibus",
-        "nicren  n v",
-        "scheepvaartbedrijf absurdia  inc",
+        "stichting vrienden van laurens pax intrantibus",
+        "nicren n v",
+        "scheepvaartbedrijf absurdia inc",
         "aeoa aeoa inc",
         "ss ss german co",
     ]
 
     assert out == expect
```

### Comparing `emm-2.0.1/tests/unit/test_negative_sample_creation.py` & `emm-2.1.0/tests/unit/test_negative_sample_creation.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_serialization.py` & `emm-2.1.0/tests/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_threshold_decision.py` & `emm-2.1.0/tests/unit/test_threshold_decision.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_timer.py` & `emm-2.1.0/tests/unit/test_timer.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/unit/test_util.py` & `emm-2.1.0/tests/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `emm-2.0.1/tests/utils.py` & `emm-2.1.0/tests/utils.py`

 * *Files identical despite different names*

