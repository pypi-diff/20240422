# Comparing `tmp/ul-db-utils-3.2.5.tar.gz` & `tmp/ul-db-utils-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-db-utils-3.2.5.tar", last modified: Fri Apr 19 07:54:58 2024, max compression
+gzip compressed data, was "ul-db-utils-3.3.0.tar", last modified: Mon Apr 22 07:48:31 2024, max compression
```

## Comparing `ul-db-utils-3.2.5.tar` & `ul-db-utils-3.3.0.tar`

### file list

```diff
@@ -1,105 +1,112 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.940595 ul-db-utils-3.2.5/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7093 2024-04-19 07:54:58.940595 ul-db-utils-3.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6419 2023-05-19 17:51:56.000000 ul-db-utils-3.2.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 07:54:58.940595 ul-db-utils-3.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2074 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.836590 ul-db-utils-3.2.5/ul_db_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.848591 ul-db-utils-3.2.5/ul_db_utils/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-02-21 11:19:06.000000 ul-db-utils-3.2.5/ul_db_utils/commands/cmd_action.py
--rw-rw-rw-   0 root         (0) root         (0)     2464 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/commands/cmd_docs.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/commands/cmd_dump.py
--rw-rw-rw-   0 root         (0) root         (0)     3894 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/commands/cmd_restore.py
--rw-rw-rw-   0 root         (0) root         (0)     1236 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/commands/cmd_waiting.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/commands/doc_request_sql.sql
--rw-rw-rw-   0 root         (0) root         (0)     1049 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.852591 ul-db-utils-3.2.5/ul_db_utils/errors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/errors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/errors/compare_null_error.py
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/errors/db_error.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/errors/db_filter_error.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/errors/db_sort_error.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/errors/deletion_not_allowed.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/errors/multiple_objects_returned.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/errors/unknow_field_error.py
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/errors/update_column_not_allowed_error.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/errors/update_not_allowed.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.888593 ul-db-utils-3.2.5/ul_db_utils/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/model/api_user.py
--rw-rw-rw-   0 root         (0) root         (0)     5705 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/model/base_api_user_log_model.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2024-02-21 11:19:06.000000 ul-db-utils-3.2.5/ul_db_utils/model/base_document.py
--rw-rw-rw-   0 root         (0) root         (0)     3157 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/model/base_immutable_model.py
--rw-rw-rw-   0 root         (0) root         (0)     5809 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/model/base_mater_pg_view.py
--rw-rw-rw-   0 root         (0) root         (0)     4304 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/model/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3865 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/model/base_undeletable_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4897 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/model/base_undeletable_user_log_model.py
--rw-rw-rw-   0 root         (0) root         (0)     5423 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/model/base_user_log_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.892593 ul-db-utils-3.2.5/ul_db_utils/model/media_storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/model/media_storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/model/media_storage/media_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1261 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/model/media_storage/media_file_download_link.py
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/model/media_storage/media_file_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.892593 ul-db-utils-3.2.5/ul_db_utils/model/methods/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/model/methods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/model/methods/make_immutable_column.py
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/model/referense_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.916594 ul-db-utils-3.2.5/ul_db_utils/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11888 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/modules/audit.sql
--rw-rw-rw-   0 root         (0) root         (0)     1691 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/modules/audit_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2106 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/modules/custom_query.py
--rw-rw-rw-   0 root         (0) root         (0)     5798 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/modules/db.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/modules/db_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.916594 ul-db-utils-3.2.5/ul_db_utils/modules/mongo_db_modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/modules/mongo_db_modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4062 2024-02-21 11:19:06.000000 ul-db-utils-3.2.5/ul_db_utils/modules/mongo_db_modules/db.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/modules/mongo_db_modules/db_context.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/modules/transaction_commit.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.924594 ul-db-utils-3.2.5/ul_db_utils/search/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13824 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/search/db_search.py
--rw-rw-rw-   0 root         (0) root         (0)     1153 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/search/doc_db_search.py
--rw-rw-rw-   0 root         (0) root         (0)     9316 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/search/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.936595 ul-db-utils-3.2.5/ul_db_utils/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-02-21 11:19:06.000000 ul-db-utils-3.2.5/ul_db_utils/utils/camel_to_snake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.940595 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:54:57.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_bool.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_choices.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_dict_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_dict_keys_choice.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_dict_keys_strict.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_dict_str_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_dict_upper_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_float.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_int.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_int_positive.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_len.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_list.py
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_list_of.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_positive_int_non_zero.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_set.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_str.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_type.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_url_with_scheme_and_netloc.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2024-02-21 11:19:06.000000 ul-db-utils-3.2.5/ul_db_utils/utils/ensure_db_object_exists.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2024-02-21 11:19:06.000000 ul-db-utils-3.2.5/ul_db_utils/utils/filter_conversion_doc_db.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/get_model_template.py
--rw-rw-rw-   0 root         (0) root         (0)     2153 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/query_soft_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/remove_duplicated_spaces_of_string.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-02-21 11:19:06.000000 ul-db-utils-3.2.5/ul_db_utils/utils/types.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-12-07 08:13:25.000000 ul-db-utils-3.2.5/ul_db_utils/utils/waiting_for_mongo.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-06-22 12:16:47.000000 ul-db-utils-3.2.5/ul_db_utils/utils/waiting_for_postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:54:58.836590 ul-db-utils-3.2.5/ul_db_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7093 2024-04-19 07:54:58.000000 ul-db-utils-3.2.5/ul_db_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3457 2024-04-19 07:54:58.000000 ul-db-utils-3.2.5/ul_db_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 07:54:58.000000 ul-db-utils-3.2.5/ul_db_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-19 07:54:58.000000 ul-db-utils-3.2.5/ul_db_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      504 2024-04-19 07:54:58.000000 ul-db-utils-3.2.5/ul_db_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-19 07:54:58.000000 ul-db-utils-3.2.5/ul_db_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.953299 ul-db-utils-3.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7093 2024-04-22 07:48:31.953299 ul-db-utils-3.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6419 2023-04-21 10:27:38.000000 ul-db-utils-3.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 07:48:31.953299 ul-db-utils-3.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2074 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.853296 ul-db-utils-3.3.0/ul_db_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.885297 ul-db-utils-3.3.0/ul_db_utils/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2023-12-20 09:16:29.000000 ul-db-utils-3.3.0/ul_db_utils/commands/cmd_action.py
+-rw-rw-rw-   0 root         (0) root         (0)     2464 2023-09-20 12:05:30.000000 ul-db-utils-3.3.0/ul_db_utils/commands/cmd_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/commands/cmd_dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/commands/cmd_restore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2023-11-29 15:18:45.000000 ul-db-utils-3.3.0/ul_db_utils/commands/cmd_waiting.py
+-rw-rw-rw-   0 root         (0) root         (0)      794 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/commands/doc_request_sql.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2023-09-20 12:05:30.000000 ul-db-utils-3.3.0/ul_db_utils/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.901297 ul-db-utils-3.3.0/ul_db_utils/errors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/errors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/errors/compare_null_error.py
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/errors/db_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/errors/db_filter_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/errors/db_sort_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/errors/deletion_not_allowed.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/errors/multiple_objects_returned.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/errors/unknow_field_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/errors/update_column_not_allowed_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/errors/update_not_allowed.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.905298 ul-db-utils-3.3.0/ul_db_utils/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      695 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/api_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     5739 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/base_api_user_log_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-12-20 09:16:29.000000 ul-db-utils-3.3.0/ul_db_utils/model/base_document.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/base_immutable_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5826 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/base_mater_pg_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     4355 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/base_undeletable_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4931 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/base_undeletable_user_log_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     5457 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/base_user_log_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.905298 ul-db-utils-3.3.0/ul_db_utils/model/media_storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/media_storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/media_storage/media_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/media_storage/media_file_download_link.py
+-rw-rw-rw-   0 root         (0) root         (0)      695 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/media_storage/media_file_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.905298 ul-db-utils-3.3.0/ul_db_utils/model/methods/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/methods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/methods/make_immutable_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/model/referense_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.905298 ul-db-utils-3.3.0/ul_db_utils/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11888 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/modules/audit.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/modules/audit_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.905298 ul-db-utils-3.3.0/ul_db_utils/modules/mongo_db_modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/modules/mongo_db_modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4062 2023-12-20 09:16:29.000000 ul-db-utils-3.3.0/ul_db_utils/modules/mongo_db_modules/db.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-11-29 15:18:45.000000 ul-db-utils-3.3.0/ul_db_utils/modules/mongo_db_modules/db_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.913298 ul-db-utils-3.3.0/ul_db_utils/modules/postgres_modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/modules/postgres_modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/modules/postgres_modules/custom_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     5798 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/modules/postgres_modules/db.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/modules/postgres_modules/db_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/modules/postgres_modules/transaction_commit.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.913298 ul-db-utils-3.3.0/ul_db_utils/repository/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/repository/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/repository/abstract_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/repository/mongoengine_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     1819 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/repository/sqlalchemy_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.925298 ul-db-utils-3.3.0/ul_db_utils/search/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13824 2023-09-20 12:05:30.000000 ul-db-utils-3.3.0/ul_db_utils/search/db_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/search/doc_db_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     9316 2023-09-20 12:05:30.000000 ul-db-utils-3.3.0/ul_db_utils/search/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.937299 ul-db-utils-3.3.0/ul_db_utils/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-12-20 09:16:29.000000 ul-db-utils-3.3.0/ul_db_utils/utils/camel_to_snake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.953299 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_bool.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_choices.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_dict_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_dict_keys_choice.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_dict_keys_strict.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_dict_str_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_dict_upper_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_float.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_int.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_int_positive.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_len.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_list.py
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_list_of.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_positive_int_non_zero.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_set.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_str.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_url_with_scheme_and_netloc.py
+-rw-rw-rw-   0 root         (0) root         (0)      511 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/utils/ensure_db_object_exists.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2023-12-20 09:16:29.000000 ul-db-utils-3.3.0/ul_db_utils/utils/filter_conversion_doc_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/utils/get_model_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2024-04-22 07:48:28.000000 ul-db-utils-3.3.0/ul_db_utils/utils/query_soft_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/remove_duplicated_spaces_of_string.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-12-20 09:16:29.000000 ul-db-utils-3.3.0/ul_db_utils/utils/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-11-29 15:18:45.000000 ul-db-utils-3.3.0/ul_db_utils/utils/waiting_for_mongo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-08-15 07:54:33.000000 ul-db-utils-3.3.0/ul_db_utils/utils/waiting_for_postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 07:48:31.857296 ul-db-utils-3.3.0/ul_db_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7093 2024-04-22 07:48:31.000000 ul-db-utils-3.3.0/ul_db_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3752 2024-04-22 07:48:31.000000 ul-db-utils-3.3.0/ul_db_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 07:48:31.000000 ul-db-utils-3.3.0/ul_db_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-22 07:48:31.000000 ul-db-utils-3.3.0/ul_db_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-22 07:48:31.000000 ul-db-utils-3.3.0/ul_db_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-22 07:48:31.000000 ul-db-utils-3.3.0/ul_db_utils.egg-info/top_level.txt
```

### Comparing `ul-db-utils-3.2.5/PKG-INFO` & `ul-db-utils-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-db-utils
-Version: 3.2.5
+Version: 3.3.0
 Summary: Python ul db utils
 Home-page: https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/db-utils.git
 Author: Unic-lab
 Author-email: 
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-db-utils-3.2.5/README.md` & `ul-db-utils-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/setup.py` & `ul-db-utils-3.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-db-utils',
-    version='3.2.5',
+    version='3.3.0',
     description='Python ul db utils',
     author='Unic-lab',
     author_email='',
     url='https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/db-utils.git',
     packages=find_packages(include=['ul_db_utils*']),
     platforms='any',
     package_data={
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/commands/cmd_action.py` & `ul-db-utils-3.3.0/ul_db_utils/commands/cmd_action.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/commands/cmd_docs.py` & `ul-db-utils-3.3.0/ul_db_utils/commands/cmd_docs.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/commands/cmd_dump.py` & `ul-db-utils-3.3.0/ul_db_utils/commands/cmd_dump.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/commands/cmd_restore.py` & `ul-db-utils-3.3.0/ul_db_utils/commands/cmd_restore.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/commands/cmd_waiting.py` & `ul-db-utils-3.3.0/ul_db_utils/commands/cmd_waiting.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/commands/doc_request_sql.sql` & `ul-db-utils-3.3.0/ul_db_utils/commands/doc_request_sql.sql`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/conf.py` & `ul-db-utils-3.3.0/ul_db_utils/conf.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/main.py` & `ul-db-utils-3.3.0/ul_db_utils/main.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/api_user.py` & `ul-db-utils-3.3.0/ul_db_utils/model/api_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sqlalchemy.dialects.postgresql import ARRAY
 
 from ul_db_utils.model.base_model import BaseModel
-from ul_db_utils.modules.db import db
+from ul_db_utils.modules.postgres_modules.db import db
 
 
 class ApiUser(BaseModel):
     __tablename__ = 'api_user'
     __table_args__ = {"comment": "Пользователь API"}
 
     date_expiration = db.Column(db.DateTime(), nullable=False, comment="Срок действия доступа")
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/base_api_user_log_model.py` & `ul-db-utils-3.3.0/ul_db_utils/model/base_api_user_log_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from sqlalchemy import inspect
 from sqlalchemy.dialects.postgresql import UUID as PG_UUID
 from sqlalchemy.engine.base import Connection
 from sqlalchemy.ext.declarative import declared_attr
 
 from ul_db_utils.model.base_model import BaseModel
 from ul_db_utils.model.base_user_log_model import BaseUserLogModel
-from ul_db_utils.modules import transaction_commit
-from ul_db_utils.modules.db import db, DbMapper
+from ul_db_utils.modules.postgres_modules import transaction_commit
+from ul_db_utils.modules.postgres_modules.db import db, DbMapper
 
 
 class BaseApiUserLogModel(BaseModel):
 
     __abstract__ = True
 
     @declared_attr
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/base_immutable_model.py` & `ul-db-utils-3.3.0/ul_db_utils/model/base_immutable_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from flask_sqlalchemy import BaseQuery
 from sqlalchemy.dialects.postgresql import UUID as PG_UUID
 from sqlalchemy.engine.base import Connection
 from sqlalchemy_serializer import SerializerMixin
 
 from ul_db_utils.errors.deletion_not_allowed import DeletionNotAllowedError
 from ul_db_utils.errors.update_not_allowed import UpdateNotAllowedError
-from ul_db_utils.modules import transaction_commit
-from ul_db_utils.modules.db import db, DbModel, DbMapper
+from ul_db_utils.modules.postgres_modules import transaction_commit
+from ul_db_utils.modules.postgres_modules.db import db, DbModel, DbMapper
 
 
 class BaseImmutableModel(DbModel, SerializerMixin):
     __abstract__ = True
 
     query_class = BaseQuery
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/base_mater_pg_view.py` & `ul-db-utils-3.3.0/ul_db_utils/model/base_mater_pg_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List
 
 from flask_sqlalchemy import BaseQuery
 from sqlalchemy import text
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy_serializer import SerializerMixin
 
-from ul_db_utils.modules.db import db, DbModel
+from ul_db_utils.modules.postgres_modules.db import db, DbModel
 from ul_db_utils.utils.ensure.ensure_list import ensure_list
 from ul_db_utils.utils.remove_duplicated_spaces_of_string import remove_duplicated_spaces_of_string
 
 
 class BaseMaterializedPGView(DbModel, SerializerMixin):
     id = db.Column(UUID(as_uuid=True), primary_key=True, default=uuid.uuid4, comment="Идентификатор записи")
     last_refresh_date = db.Column(db.DateTime(), nullable=False, comment="Дата последнего обновления")
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/base_model.py` & `ul-db-utils-3.3.0/ul_db_utils/model/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import Optional
 
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy.engine.base import Connection
 from sqlalchemy.inspection import inspect
 from sqlalchemy_serializer import SerializerMixin
 
-from ul_db_utils.modules import transaction_commit
-from ul_db_utils.modules.custom_query import CustomQuery
-from ul_db_utils.modules.db import db, DbModel, DbMapper
+from ul_db_utils.modules.postgres_modules import transaction_commit
+from ul_db_utils.modules.postgres_modules.custom_query import CustomQuery
+from ul_db_utils.modules.postgres_modules.db import db, DbModel, DbMapper
 
 
 class BaseModel(DbModel, SerializerMixin):
 
     __abstract__ = True
 
     query_class = CustomQuery
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/base_undeletable_model.py` & `ul-db-utils-3.3.0/ul_db_utils/model/base_undeletable_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from flask_sqlalchemy import BaseQuery
 from sqlalchemy.dialects.postgresql import UUID as PG_UUID
 from sqlalchemy.engine.base import Connection
 from sqlalchemy.inspection import inspect
 from sqlalchemy_serializer import SerializerMixin
 
 from ul_db_utils.errors.deletion_not_allowed import DeletionNotAllowedError
-from ul_db_utils.modules import transaction_commit
-from ul_db_utils.modules.db import db, DbModel, DbMapper
+from ul_db_utils.modules.postgres_modules import transaction_commit
+from ul_db_utils.modules.postgres_modules.db import db, DbModel, DbMapper
 
 
 class BaseUndeletableModel(DbModel, SerializerMixin):
 
     __abstract__ = True
 
     query_class = BaseQuery
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/base_undeletable_user_log_model.py` & `ul-db-utils-3.3.0/ul_db_utils/model/base_undeletable_user_log_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from sqlalchemy import inspect
 from sqlalchemy.dialects.postgresql import UUID as PG_UUID
 from sqlalchemy.engine.base import Connection
 
 from ul_db_utils.errors.deletion_not_allowed import DeletionNotAllowedError
 from ul_db_utils.model.base_undeletable_model import BaseUndeletableModel
-from ul_db_utils.modules import transaction_commit
-from ul_db_utils.modules.db import db, DbMapper
+from ul_db_utils.modules.postgres_modules import transaction_commit
+from ul_db_utils.modules.postgres_modules.db import db, DbMapper
 
 
 class BaseUndeletableUserLogModel(BaseUndeletableModel):
 
     __abstract__ = True
 
     user_created_id = db.Column(PG_UUID(as_uuid=True), nullable=False, comment="Идентификатор пользователя, создавшего запись")
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/base_user_log_model.py` & `ul-db-utils-3.3.0/ul_db_utils/model/base_user_log_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from uuid import UUID
 
 from sqlalchemy import inspect
 from sqlalchemy.dialects.postgresql import UUID as PG_UUID
 from sqlalchemy.engine.base import Connection
 
 from ul_db_utils.model.base_model import BaseModel
-from ul_db_utils.modules import transaction_commit
-from ul_db_utils.modules.db import db, DbMapper
+from ul_db_utils.modules.postgres_modules import transaction_commit
+from ul_db_utils.modules.postgres_modules.db import db, DbMapper
 
 
 class BaseUserLogModel(BaseModel):
 
     __abstract__ = True
 
     user_created_id = db.Column(PG_UUID(as_uuid=True), nullable=False, comment="Идентификатор пользователя, создавшего запись")
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/media_storage/media_file.py` & `ul-db-utils-3.3.0/ul_db_utils/model/media_storage/media_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy.dialects.postgresql import UUID
 
 from ul_db_utils.model.base_immutable_model import BaseImmutableModel
 from ul_db_utils.model.methods.make_immutable_column import make_immutable_column
-from ul_db_utils.modules.custom_query import CustomQuery
-from ul_db_utils.modules.db import db
+from ul_db_utils.modules.postgres_modules.custom_query import CustomQuery
+from ul_db_utils.modules.postgres_modules.db import db
 
 
 class MediaFile(BaseImmutableModel):
     """
       Model for media-storage-service
       git: /unic-lab/libraries/common-services/media-storage
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/media_storage/media_file_download_link.py` & `ul-db-utils-3.3.0/ul_db_utils/model/media_storage/media_file_download_link.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy.dialects.postgresql import UUID
 
 from ul_db_utils.model.base_user_log_model import BaseUserLogModel
 from ul_db_utils.model.methods.make_immutable_column import make_immutable_column
-from ul_db_utils.modules.custom_query import CustomQuery
-from ul_db_utils.modules.db import db
+from ul_db_utils.modules.postgres_modules.custom_query import CustomQuery
+from ul_db_utils.modules.postgres_modules.db import db
 
 
 class MediaFileDownloadLink(BaseUserLogModel):
     """
       Model for media-storage-service
       git: /unic-lab/libraries/common-services/media-storage
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/media_storage/media_file_type.py` & `ul-db-utils-3.3.0/ul_db_utils/model/media_storage/media_file_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import uuid
 
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy_serializer import SerializerMixin
 
-from ul_db_utils.modules.db import db, DbModel
+from ul_db_utils.modules.postgres_modules.db import db, DbModel
 
 
 class MediaFileType(DbModel, SerializerMixin):
     """
     Model for media-storage-service
     git: /unic-lab/libraries/common-services/media-storage
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/methods/make_immutable_column.py` & `ul-db-utils-3.3.0/ul_db_utils/model/methods/make_immutable_column.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from asyncio import Event
 from typing import Any
 
 from sqlalchemy.util import symbol
 
 from ul_db_utils.errors.update_column_not_allowed_error import UpdateColumnNotAllowedError
-from ul_db_utils.modules.db import DbColumn, DbModel, db
+from ul_db_utils.modules.postgres_modules.db import DbColumn, DbModel, db
 
 
 def make_immutable_column(col: DbColumn) -> None:
     @db.event.listens_for(col, 'set')
     def immutable_column_set_listener(target: DbModel, value: Any, old_value: Any, initiator: Event) -> None:
         if old_value != symbol('NEVER_SET') and old_value != symbol('NO_VALUE') and old_value != value:
             raise UpdateColumnNotAllowedError(f'Cannot update column {col.name} on model {col.class_.__name__} from {old_value} to {value}: column is non-updatable.')
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/model/referense_link.py` & `ul-db-utils-3.3.0/ul_db_utils/model/referense_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ul_db_utils.model.base_user_log_model import BaseUserLogModel
-from ul_db_utils.modules.db import db
+from ul_db_utils.modules.postgres_modules.db import db
 
 
 class ReferenceLink(BaseUserLogModel):
     """
     Model for reference-links-service
     git: /unic-lab/libraries/common-services/reference-links
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/modules/audit.sql` & `ul-db-utils-3.3.0/ul_db_utils/modules/audit.sql`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/modules/audit_manager.py` & `ul-db-utils-3.3.0/ul_db_utils/modules/audit_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
-from sqlalchemy import text, inspect
+from sqlalchemy import text
 
-from ul_db_utils.modules.db import db
+from ul_db_utils.modules.postgres_modules.db import db
 
 AUDIT_SQL_FILE_PATH = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'audit.sql')
 
 
 def add_table_to_audit(table_name: str) -> None:
     sql_command = f"SELECT audit.audit_table('public.{table_name}');"
     with db.engine.connect().execution_options(autocommit=True) as conn:
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/modules/custom_query.py` & `ul-db-utils-3.3.0/ul_db_utils/modules/postgres_modules/custom_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, Any, Union, TYPE_CHECKING
 
 from flask_sqlalchemy import BaseQuery
 
 if TYPE_CHECKING:
     from sqlalchemy.orm.mapper import Mapper
 
-from ul_db_utils.modules.db import db
+from ul_db_utils.modules.postgres_modules.db import db
 
 
 class CustomQuery(BaseQuery):  # type: ignore
     """Overwrite Base Query with additional filters"""
 
     def __new__(cls, *args: 'Mapper', **kwargs: Union[Any, Dict[str, Any]]) -> 'CustomQuery':
         # get new object BaseQuery
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/modules/db.py` & `ul-db-utils-3.3.0/ul_db_utils/modules/postgres_modules/db.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/modules/db_context.py` & `ul-db-utils-3.3.0/ul_db_utils/modules/postgres_modules/db_context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import wraps
 from typing import Any, Callable, cast, TypeVar
 
-from ul_db_utils.modules import db
+from ul_db_utils.modules.postgres_modules import db
 
 TFn = TypeVar("TFn", bound=Callable[..., Any])
 
 
 def db_app_context(fn: TFn) -> TFn:
     assert db.initialized_sdk is not None, 'you must initialize db-config'
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/modules/mongo_db_modules/db.py` & `ul-db-utils-3.3.0/ul_db_utils/modules/mongo_db_modules/db.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/modules/mongo_db_modules/db_context.py` & `ul-db-utils-3.3.0/ul_db_utils/modules/mongo_db_modules/db_context.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/search/db_search.py` & `ul-db-utils-3.3.0/ul_db_utils/search/db_search.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/search/doc_db_search.py` & `ul-db-utils-3.3.0/ul_db_utils/search/doc_db_search.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/search/helpers.py` & `ul-db-utils-3.3.0/ul_db_utils/search/helpers.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/utils/ensure/ensure_dict_keys_strict.py` & `ul-db-utils-3.3.0/ul_db_utils/utils/ensure/ensure_dict_keys_strict.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/utils/filter_conversion_doc_db.py` & `ul-db-utils-3.3.0/ul_db_utils/utils/filter_conversion_doc_db.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/utils/get_model_template.py` & `ul-db-utils-3.3.0/ul_db_utils/utils/get_model_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ul_db_utils.modules.db import db, DbModel
+from ul_db_utils.modules.postgres_modules.db import db, DbModel
 from ul_db_utils.model.base_model import BaseModel
 from ul_db_utils.model.base_user_log_model import BaseUserLogModel
 from typing import Any, Dict, List, Union
 
 
 def get_models_template(model: Union[List[DbModel], DbModel]) -> Dict[str, Any]:
     base_user_log_model_columns = BaseUserLogModel.__dict__.keys()
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/utils/query_soft_delete.py` & `ul-db-utils-3.3.0/ul_db_utils/utils/query_soft_delete.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from uuid import UUID
 
 from sqlalchemy.exc import NoResultFound as NoResultFoundError
 
 from ul_db_utils.model.base_api_user_log_model import BaseApiUserLogModel
 from ul_db_utils.model.base_model import BaseModel
 from ul_db_utils.model.base_user_log_model import BaseUserLogModel
-from ul_db_utils.modules.custom_query import CustomQuery
+from ul_db_utils.modules.postgres_modules.custom_query import CustomQuery
 
 
 def query_soft_delete(
     model: Union[Type[BaseModel], Type[BaseUserLogModel], Type[BaseApiUserLogModel]],
     instance_id: UUID,
     user_modified_id: Optional[UUID] = None,
     query: Optional[CustomQuery] = None,
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils/utils/waiting_for_mongo.py` & `ul-db-utils-3.3.0/ul_db_utils/utils/waiting_for_mongo.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils/utils/waiting_for_postgres.py` & `ul-db-utils-3.3.0/ul_db_utils/utils/waiting_for_postgres.py`

 * *Files identical despite different names*

### Comparing `ul-db-utils-3.2.5/ul_db_utils.egg-info/PKG-INFO` & `ul-db-utils-3.3.0/ul_db_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-db-utils
-Version: 3.2.5
+Version: 3.3.0
 Summary: Python ul db utils
 Home-page: https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/db-utils.git
 Author: Unic-lab
 Author-email: 
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-db-utils-3.2.5/ul_db_utils.egg-info/SOURCES.txt` & `ul-db-utils-3.3.0/ul_db_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,21 +44,26 @@
 ul_db_utils/model/media_storage/media_file_download_link.py
 ul_db_utils/model/media_storage/media_file_type.py
 ul_db_utils/model/methods/__init__.py
 ul_db_utils/model/methods/make_immutable_column.py
 ul_db_utils/modules/__init__.py
 ul_db_utils/modules/audit.sql
 ul_db_utils/modules/audit_manager.py
-ul_db_utils/modules/custom_query.py
-ul_db_utils/modules/db.py
-ul_db_utils/modules/db_context.py
-ul_db_utils/modules/transaction_commit.py
 ul_db_utils/modules/mongo_db_modules/__init__.py
 ul_db_utils/modules/mongo_db_modules/db.py
 ul_db_utils/modules/mongo_db_modules/db_context.py
+ul_db_utils/modules/postgres_modules/__init__.py
+ul_db_utils/modules/postgres_modules/custom_query.py
+ul_db_utils/modules/postgres_modules/db.py
+ul_db_utils/modules/postgres_modules/db_context.py
+ul_db_utils/modules/postgres_modules/transaction_commit.py
+ul_db_utils/repository/__init__.py
+ul_db_utils/repository/abstract_repository.py
+ul_db_utils/repository/mongoengine_repository.py
+ul_db_utils/repository/sqlalchemy_repository.py
 ul_db_utils/search/__init__.py
 ul_db_utils/search/db_search.py
 ul_db_utils/search/doc_db_search.py
 ul_db_utils/search/helpers.py
 ul_db_utils/utils/__init__.py
 ul_db_utils/utils/camel_to_snake.py
 ul_db_utils/utils/ensure_db_object_exists.py
```

