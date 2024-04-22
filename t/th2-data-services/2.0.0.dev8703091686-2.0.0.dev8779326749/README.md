# Comparing `tmp/th2_data_services-2.0.0.dev8703091686.tar.gz` & `tmp/th2_data_services-2.0.0.dev8779326749.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev8703091686.tar", last modified: Tue Apr 16 09:18:31 2024, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev8779326749.tar", last modified: Mon Apr 22 06:10:43 2024, max compression
```

## Comparing `th2_data_services-2.0.0.dev8703091686.tar` & `th2_data_services-2.0.0.dev8779326749.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 09:18:21.000000 th2_data_services-2.0.0.dev8703091686/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/_internal/perf_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    41567 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/dummy/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/_is_sorted_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/sse_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/stream_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/stream_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/stream_utils/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-16 09:17:21.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-16 09:18:30.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-16 09:18:31.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:18:30.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-16 09:18:30.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 09:18:30.000000 th2_data_services-2.0.0.dev8703091686/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 06:10:32.000000 th2_data_services-2.0.0.dev8779326749/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/_internal/perf_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/dummy/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/_is_sorted_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/sse_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/stream_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/stream_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/stream_utils/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-22 06:09:34.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 06:10:43.000000 th2_data_services-2.0.0.dev8779326749/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev8703091686/PKG-INFO` & `th2_data_services-2.0.0.dev8779326749/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3837 3033 3039 3136 3836 0a53 756d 6d61  8703091686.Summa
+00000040: 3837 3739 3332 3637 3439 0a53 756d 6d61  8779326749.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev8703091686/README.md` & `th2_data_services-2.0.0.dev8779326749/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/setup.py` & `th2_data_services-2.0.0.dev8779326749/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/_internal/__init__.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/_internal/perf_tests.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/_internal/perf_tests.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/config/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-
+from typing import Optional
 
 from th2_data_services.interfaces.utils.resolver import (
     EventFieldResolver,
     MessageFieldResolver,
     SubMessageFieldResolver,
     ExpandedMessageFieldResolver,
 )
@@ -23,18 +23,18 @@
 
 class TH2Config:
     def __init__(self) -> None:
         """Global configuration for the DS library."""
         # TODO - try to import here data_source in available.
 
         self.INTERACTIVE_MODE = False
-        self.EVENT_FIELDS_RESOLVER: EventFieldResolver = None
-        self.MESSAGE_FIELDS_RESOLVER: MessageFieldResolver = None
-        self.SUBMESSAGE_FIELDS_RESOLVER: SubMessageFieldResolver = None
-        self.EXPANDED_MESSAGE_FIELDS_RESOLVER: ExpandedMessageFieldResolver = None
+        self.EVENT_FIELDS_RESOLVER: Optional[EventFieldResolver] = None
+        self.MESSAGE_FIELDS_RESOLVER: Optional[MessageFieldResolver] = None
+        self.SUBMESSAGE_FIELDS_RESOLVER: Optional[SubMessageFieldResolver] = None
+        self.EXPANDED_MESSAGE_FIELDS_RESOLVER: Optional[ExpandedMessageFieldResolver] = None
         self.MAX_PATH: int = 255  # OS limitation. Both Windows and Linux
         self.FORBIDDEN_CHARACTERS_IN_FILENAME: str = '<>:"|?*/\\'
         self.FORBIDDEN_CHARACTERS_IN_FILENAME_CHANGE_TO: str = "_"
         self.DEFAULT_PICKLE_VERSION = 4
 
         # Aliases
         self.efr = self.EVENT_FIELDS_RESOLVER
@@ -52,15 +52,19 @@
             f"MAX_PATH={self.MAX_PATH}\n"
             f"FORBIDDEN_CHARACTERS_IN_FILENAME={self.FORBIDDEN_CHARACTERS_IN_FILENAME}\n"
             f"FORBIDDEN_CHARACTERS_IN_FILENAME_CHANGE_TO={self.FORBIDDEN_CHARACTERS_IN_FILENAME_CHANGE_TO}\n"
         )
         return s
 
     def setup_resolvers(
-        self, for_event, for_message, for_submessage, for_expanded_message
+        self,
+        for_event: EventFieldResolver,
+        for_message: MessageFieldResolver,
+        for_submessage: SubMessageFieldResolver,
+        for_expanded_message: ExpandedMessageFieldResolver,
     ) -> "TH2Config":
         """Use this to set up your custom resolvers.
 
         Args:
             for_event:
             for_message:
             for_submessage:
```

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/data.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     List,
     Optional,
     Union,
     Iterable,
     Iterator,
     Any,
     Generic,
+    BinaryIO,
 )
 from weakref import finalize
 import types
 from inspect import isgeneratorfunction
 from typing import TypeVar
 from th2_data_services.interfaces.adapter import IStreamAdapter, IRecordAdapter
 from th2_data_services.config import options as o
@@ -185,28 +186,28 @@
 
         self._id = id(self)
         self._cache_filename = f"{self._id}_{time()}.pickle"
         self._cache_path = Path("temp", self._cache_filename).resolve().absolute()
         self._pending_cache_path = (
             self._cache_path.with_name("[PENDING]" + self._cache_filename).resolve().absolute()
         )
-        self._cache_file_obj = None
-        self._len = None
+        self._cache_file_obj: Optional[BinaryIO] = None
+        self._len: Optional[int] = None
         self.workflow = DataWorkflow()
 
-        self._length_hint = None  # The value is populated when we use limit method.
-        self._cache_status = cache
+        self._length_hint: Optional[int] = None  # The value is populated when we use limit method.
+        self._cache_status: bool = cache
         # We use finalize instead of __del__ because __del__ won't be executed sometimes.
         # Read more about __del__ problems here: https://stackoverflow.com/a/2452895
         self._finalizer = finalize(self, self.__remove)
         # LOG         self._logger = _DataLogger(logger, {"id": self._id})
         # It used to indicate the number of current iteration of the Data object.
         # It's required if the same instance iterates several times in for-in loops.
         self.iter_num = 0  # Indicates what level of the loop the Data object is in.
-        self._stop_iteration = None
+        self._stop_iteration: Optional[bool] = None
         self._read_from_external_cache_file = False
         self.__metadata = {}
         self._pickle_version = pickle_version  # Default pickle protocol version
 
     # LOG         self._logger.info(
     # LOG            "New data object with data stream = '%s', cache = '%s' initialized", id(self._data_stream), cache
     # LOG        )
@@ -606,14 +607,15 @@
 
         return new_data
 
         # data = Data(source)
         # data._set_metadata(self.metadata)
         # return data
 
+    # TODO - probably it's better to rename to map_iter or something else ..
     def map_yield(self, callback_or_adapter: Union[Callable, IRecordAdapter]) -> "Data":
         """Maps the stream using callback function or adapter.
 
         Differences between map and map yield:
         1. map_yield is a wrapper function using map_stream.
         2. map_yield iterates over each item in record if callback returns
         a value, which is a list or tuple.
@@ -650,15 +652,17 @@
         data_obj = copy.copy(self)
         data_obj.workflow.add(
             WfLimitRecord(type="limit", callback=_build_limit_callback(num), limit=num)
         )
         data_obj._length_hint = num
         return data_obj
 
-    def sift(self, limit: int = None, skip: int = None) -> Generator[dict, None, None]:
+    def sift(
+        self, limit: Optional[int] = None, skip: Optional[int] = None
+    ) -> Generator[dict, None, None]:
         """Skips and limits records.
 
         Args:
             limit: Limited records.
             skip: Skipped records.
 
         Yields:
```

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/dummy/__init__.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/dummy/data_source.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/dummy/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/utils/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from abc import ABC, abstractmethod
 from datetime import datetime
-from typing import Generic, TypeVar
+from typing import Generic, TypeVar, Tuple
 
 TimestampType = TypeVar("TimestampType")
 
 """
 Some speed tests:
 =========================
 
@@ -37,27 +37,27 @@
         116 ns � 8.47 ns per loop (mean � std. dev. of 7 runs, 10,000,000 loops each)
 """
 
 
 class ITimestampConverter(ABC, Generic[TimestampType]):
     @classmethod
     @abstractmethod
-    def parse_timestamp(cls, timestamp: TimestampType) -> (str, str):
+    def parse_timestamp(cls, timestamp: TimestampType) -> Tuple[str, str]:
         """Returns string representation of Unix time.
 
         Separated for seconds and nanoseconds.
 
         Please note, nanoseconds can have zeroes from left.
 
         e.g. 2022-03-05T23:56:44.00123Z -> ('1646524604', '001230000')
         """
 
     @classmethod
     @abstractmethod
-    def parse_timestamp_int(cls, timestamp: TimestampType) -> (int, int):
+    def parse_timestamp_int(cls, timestamp: TimestampType) -> Tuple[int, int]:
         """Returns int representation of Unix time.
 
         Separated for seconds and nanoseconds.
 
         e.g. 2022-03-05T23:56:44.00123Z -> (1646524604, 001230000)
         """
```

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/interfaces/utils/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from abc import ABC, abstractmethod
-from typing import Dict, List, Any, Union
+from typing import Any, Dict, List, Union
 
 """
 The idea of using resolvers:
     It solves the problem of having a few DataSources with the same data,
     but with different ways to get it.
 
     These classes provide you getter methods.
@@ -157,21 +157,23 @@
     @abstractmethod
     def get_attached_event_ids(message) -> List[str]:
         pass
 
     @staticmethod
     @abstractmethod
     def expand_message(message) -> List[Dict[str, Any]]:
-        """Extract compounded message into list of individual messages.
+        """Extract a compounded message into a list of individual messages.
+
+        Use it with `data.map_yield` instead of `data.map`.
 
         Warnings:
             expand_message function is not backward-compatible.
-            If you use it in your scripts, there is no guarantee that everything will
-            work if you change data-source because different data-sources has different
-            messages structure.
+            If you use it in your scripts, there is no guarantee that everything
+            will work if you change data-source because different data-sources
+            have different messages structure.
 
         Args:
             message: Th2Message
 
         Returns:
             Iterable[Th2Message]
         """
```

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/_is_sorted_result.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/_is_sorted_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+from typing import Optional
 
 
 class IsSortedResult:
     """IsSortedResult is used by util methods that check whether a sequence of elements is sorted.
 
     The class provides some attributes that tells its user additional information about the sequence provided,
     for example: index of the first unsorted element.
@@ -22,12 +23,12 @@
 
     def __init__(self, status: bool = True):
         """IsSortedResult constructor.
 
         Args:
             status: Whether the sequence is sorted.
         """
-        self.status = status
-        self.first_unsorted = None
+        self.status: bool = status
+        self.first_unsorted: Optional[int] = None
 
     def __bool__(self):
         return self.status
```

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/decode_error_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from __future__ import annotations
 from codecs import register_error
 
 
-def handler(err: UnicodeDecodeError):
+def handler(err: UnicodeDecodeError) -> tuple[str, int]:
     """Decode error handler that tries change utf-8 character to Unicode."""
     return chr(err.object[err.start]), err.end
 
 
 UNICODE_REPLACE_HANDLER = "unicode_replace"
 
 register_error(UNICODE_REPLACE_HANDLER, handler)
```

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/path_utils.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/stream_utils/__init__.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/stream_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/stream_utils/stream_utils.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/stream_utils/stream_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev8779326749/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev8779326749/th2_data_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3837 3033 3039 3136 3836 0a53 756d 6d61  8703091686.Summa
+00000040: 3837 3739 3332 3637 3439 0a53 756d 6d61  8779326749.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev8779326749/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8703091686/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev8779326749/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

