# Comparing `tmp/openparse-0.5.2.tar.gz` & `tmp/openparse-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openparse-0.5.2.tar", last modified: Thu Apr 11 14:23:20 2024, max compression
+gzip compressed data, was "openparse-0.5.3.tar", last modified: Mon Apr 22 03:56:20 2024, max compression
```

## Comparing `openparse-0.5.2.tar` & `openparse-0.5.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-11 14:23:14.000000 openparse-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-11 14:23:20.915871 openparse-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-11 14:23:14.000000 openparse-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-11 14:23:14.000000 openparse-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:23:20.915871 openparse-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.903871 openparse-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.907871 openparse-0.5.2/src/evals/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:23:14.000000 openparse-0.5.2/src/evals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-11 14:23:14.000000 openparse-0.5.2/src/evals/run_evals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.907871 openparse-0.5.2/src/openparse/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/doc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.907871 openparse-0.5.2/src/openparse/processing/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/processing/basic_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/processing/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/processing/semantic_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/tables/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/tables/pymupdf/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/pymupdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/pymupdf/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/tables/table_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/table_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/table_transformers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/table_transformers/ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/table_transformers/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/tables/unitable/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/tabular_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/unitable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/text/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/text/pdfminer/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/pdfminer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/pdfminer/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/text/pymupdf/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/pymupdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/pymupdf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/openparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/processing/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/processing/test_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/tables/pymupdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/pymupdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/pymupdf/test_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/tables/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/transformers/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/transformers/test_ml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/tables/unitable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/unitable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   190851 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/unitable/sample_pred_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/unitable/test_pred_to_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/test_doc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/test_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.903871 openparse-0.5.2/src/tests/text/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/text/pdf_miner/
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/text/pdf_miner/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.141723 openparse-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-22 03:56:13.000000 openparse-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-22 03:56:20.141723 openparse-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-22 03:56:13.000000 openparse-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-22 03:56:13.000000 openparse-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 03:56:20.141723 openparse-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.129723 openparse-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.133723 openparse-0.5.3/src/evals/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 03:56:13.000000 openparse-0.5.3/src/evals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-22 03:56:13.000000 openparse-0.5.3/src/evals/run_evals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.133723 openparse-0.5.3/src/openparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/doc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.133723 openparse-0.5.3/src/openparse/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/processing/basic_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/processing/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/processing/semantic_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.137724 openparse-0.5.3/src/openparse/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.137724 openparse-0.5.3/src/openparse/tables/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/pymupdf/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.137724 openparse-0.5.3/src/openparse/tables/table_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/table_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/table_transformers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/table_transformers/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/table_transformers/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.137724 openparse-0.5.3/src/openparse/tables/unitable/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/unitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/unitable/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/unitable/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/unitable/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/unitable/tabular_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/unitable/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/unitable/unitable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/unitable/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/tables/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.137724 openparse-0.5.3/src/openparse/text/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/text/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.137724 openparse-0.5.3/src/openparse/text/pdfminer/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/text/pdfminer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/text/pdfminer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.137724 openparse-0.5.3/src/openparse/text/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/text/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/text/pymupdf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-22 03:56:13.000000 openparse-0.5.3/src/openparse/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.141723 openparse-0.5.3/src/openparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-22 03:56:20.000000 openparse-0.5.3/src/openparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-22 03:56:20.000000 openparse-0.5.3/src/openparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 03:56:20.000000 openparse-0.5.3/src/openparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-22 03:56:20.000000 openparse-0.5.3/src/openparse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-22 03:56:20.000000 openparse-0.5.3/src/openparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 03:56:20.000000 openparse-0.5.3/src/openparse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.141723 openparse-0.5.3/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.141723 openparse-0.5.3/src/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/processing/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/processing/test_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.141723 openparse-0.5.3/src/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.141723 openparse-0.5.3/src/tests/tables/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/tables/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/tables/pymupdf/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.141723 openparse-0.5.3/src/tests/tables/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/tables/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/tables/transformers/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/tables/transformers/test_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.141723 openparse-0.5.3/src/tests/tables/unitable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/tables/unitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190851 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/tables/unitable/sample_pred_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/tables/unitable/test_pred_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/test_doc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/test_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.133723 openparse-0.5.3/src/tests/text/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:56:20.141723 openparse-0.5.3/src/tests/text/pdf_miner/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-22 03:56:13.000000 openparse-0.5.3/src/tests/text/pdf_miner/test_core.py
```

### Comparing `openparse-0.5.2/LICENSE` & `openparse-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/PKG-INFO` & `openparse-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.5.2
+Version: 0.5.3
 Summary: Streamlines the process of preparing documents for LLM's.
 Author-email: Sergey Filimonov <hello@sergey.fyi>
 Project-URL: homepage, https://github.com/Filimoa/open-parse
 Project-URL: repository, https://github.com/Filimoa/open-parse
 Project-URL: documentation, https://filimoa.github.io/open-parse
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `openparse-0.5.2/README.md` & `openparse-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/pyproject.toml` & `openparse-0.5.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openparse"
 description = "Streamlines the process of preparing documents for LLM's."
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.5.2"
+version = "0.5.3"
 authors = [{name = "Sergey Filimonov", email = "hello@sergey.fyi"}]
 dependencies = [
     "PyMuPDF >= 1.23.2",
     "pillow >= 8.3",
     "pydantic >= 2.0",
     "pypdf >= 4.0.0",
     "pdfminer.six >= 20200401",
```

### Comparing `openparse-0.5.2/src/evals/run_evals.py` & `openparse-0.5.3/src/evals/run_evals.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/__init__.py` & `openparse-0.5.3/src/openparse/__init__.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/cli.py` & `openparse-0.5.3/src/openparse/cli.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/config.py` & `openparse-0.5.3/src/openparse/config.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/doc_parser.py` & `openparse-0.5.3/src/openparse/doc_parser.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/pdf.py` & `openparse-0.5.3/src/openparse/pdf.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/processing/__init__.py` & `openparse-0.5.3/src/openparse/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/processing/basic_transforms.py` & `openparse-0.5.3/src/openparse/processing/basic_transforms.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/processing/ingest.py` & `openparse-0.5.3/src/openparse/processing/ingest.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/processing/semantic_transforms.py` & `openparse-0.5.3/src/openparse/processing/semantic_transforms.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/schemas.py` & `openparse-0.5.3/src/openparse/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/tables/parse.py` & `openparse-0.5.3/src/openparse/tables/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,19 @@
 ) -> List[TableElement]:
     pdoc = doc.to_pymupdf_doc()
     tables = []
     for page_num, page in enumerate(pdoc):
         tabs = page.find_tables()
         for i, tab in enumerate(tabs.tables):
             headers = tab.header.names
+            for j, header in enumerate(headers):
+                if header is None:
+                    headers[j] = ""
+                else:
+                    headers[j] = header.strip()
             lines = tab.extract()
 
             if parsing_args.table_output_format == "str":
                 text = pymupdf.output_to_markdown(headers, lines)
             elif parsing_args.table_output_format == "markdown":
                 text = pymupdf.output_to_markdown(headers, lines)
             elif parsing_args.table_output_format == "html":
```

### Comparing `openparse-0.5.2/src/openparse/tables/pymupdf/parse.py` & `openparse-0.5.3/src/openparse/tables/pymupdf/parse.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 def output_to_markdown(headers: List[str], rows: List[List[str]]) -> str:
     markdown_output = "| " + " | ".join(headers) + " |\n"
     markdown_output += "|---" * len(headers) + "|\n"
 
     for row in rows:
-        processed_row = [" " if cell in [None, ""] else cell for cell in row]
+        processed_row = [" " if cell in [None, ""] else cell.replace("\n", " ") for cell in row]
         markdown_output += "| " + " | ".join(processed_row) + " |\n"
 
     return markdown_output
 
 
 def combine_header_and_table_bboxes(
     bbox1: Tuple[float, float, float, float], bbox2: Tuple[float, float, float, float]
```

### Comparing `openparse-0.5.2/src/openparse/tables/table_transformers/geometry.py` & `openparse-0.5.3/src/openparse/tables/table_transformers/geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/tables/table_transformers/ml.py` & `openparse-0.5.3/src/openparse/tables/table_transformers/ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/tables/table_transformers/schemas.py` & `openparse-0.5.3/src/openparse/tables/table_transformers/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/tables/unitable/config.py` & `openparse-0.5.3/src/openparse/tables/unitable/config.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/tables/unitable/core.py` & `openparse-0.5.3/src/openparse/tables/unitable/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/tables/unitable/schemas.py` & `openparse-0.5.3/src/openparse/tables/unitable/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/tables/unitable/tabular_transformer.py` & `openparse-0.5.3/src/openparse/tables/unitable/tabular_transformer.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/tables/unitable/tokens.py` & `openparse-0.5.3/src/openparse/tables/unitable/tokens.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/tables/unitable/unitable_model.py` & `openparse-0.5.3/src/openparse/tables/unitable/unitable_model.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/tables/unitable/utils.py` & `openparse-0.5.3/src/openparse/tables/unitable/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/tables/utils.py` & `openparse-0.5.3/src/openparse/tables/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/text/parse.py` & `openparse-0.5.3/src/openparse/text/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/text/pdfminer/core.py` & `openparse-0.5.3/src/openparse/text/pdfminer/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/text/pymupdf/core.py` & `openparse-0.5.3/src/openparse/text/pymupdf/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/types.py` & `openparse-0.5.3/src/openparse/types.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/openparse/version.py` & `openparse-0.5.3/src/openparse/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-OPEN_PARSE_VERSION = "0.5.2"
+OPEN_PARSE_VERSION = "0.5.3"
 
 
 def version_info() -> str:
     """Return complete version information for OpenParse and its dependencies."""
     import importlib.metadata as importlib_metadata
     import platform
     import sys
```

### Comparing `openparse-0.5.2/src/openparse.egg-info/PKG-INFO` & `openparse-0.5.3/src/openparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.5.2
+Version: 0.5.3
 Summary: Streamlines the process of preparing documents for LLM's.
 Author-email: Sergey Filimonov <hello@sergey.fyi>
 Project-URL: homepage, https://github.com/Filimoa/open-parse
 Project-URL: repository, https://github.com/Filimoa/open-parse
 Project-URL: documentation, https://filimoa.github.io/open-parse
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `openparse-0.5.2/src/openparse.egg-info/SOURCES.txt` & `openparse-0.5.3/src/openparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/tests/processing/test_pipeline.py` & `openparse-0.5.3/src/tests/processing/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/tests/processing/test_steps.py` & `openparse-0.5.3/src/tests/processing/test_steps.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/tests/tables/pymupdf/test_parse.py` & `openparse-0.5.3/src/tests/tables/pymupdf/test_parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/tests/tables/transformers/test_geometry.py` & `openparse-0.5.3/src/tests/tables/transformers/test_geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/tests/tables/transformers/test_ml.py` & `openparse-0.5.3/src/tests/tables/transformers/test_ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/tests/tables/unitable/sample_pred_outputs.py` & `openparse-0.5.3/src/tests/tables/unitable/sample_pred_outputs.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/tests/tables/unitable/test_pred_to_schema.py` & `openparse-0.5.3/src/tests/tables/unitable/test_pred_to_schema.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/tests/test_doc_parser.py` & `openparse-0.5.3/src/tests/test_doc_parser.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/tests/test_schemas.py` & `openparse-0.5.3/src/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.2/src/tests/text/pdf_miner/test_core.py` & `openparse-0.5.3/src/tests/text/pdf_miner/test_core.py`

 * *Files identical despite different names*

