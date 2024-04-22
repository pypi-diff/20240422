# Comparing `tmp/ayon-python-api-1.0.1.tar.gz` & `tmp/ayon-python-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-1.0.1.tar", last modified: Mon Feb 12 13:56:39 2024, max compression
+gzip compressed data, was "ayon-python-api-1.0.2.tar", last modified: Mon Apr 22 08:17:28 2024, max compression
```

## Comparing `ayon-python-api-1.0.1.tar` & `ayon-python-api-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:56:39.732430 ayon-python-api-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-02-12 13:56:39.732430 ayon-python-api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:56:39.728430 ayon-python-api-1.0.1/ayon_api/
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32126 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    81747 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/entity_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    20039 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/graphql_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    20987 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)   214855 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18136 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/ayon_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 13:56:39.732430 ayon-python-api-1.0.1/ayon_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-02-12 13:56:39.000000 ayon-python-api-1.0.1/ayon_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-12 13:56:39.000000 ayon-python-api-1.0.1/ayon_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 13:56:39.000000 ayon-python-api-1.0.1/ayon_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-12 13:56:39.000000 ayon-python-api-1.0.1/ayon_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 13:56:39.000000 ayon-python-api-1.0.1/ayon_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 13:56:39.732430 ayon-python-api-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-02-12 13:56:33.000000 ayon-python-api-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:28.876161 ayon-python-api-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-04-22 08:17:28.876161 ayon-python-api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:28.876161 ayon-python-api-1.0.2/ayon_api/
+-rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123859 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86216 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/entity_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21938 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42241 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)   247562 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/ayon_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:28.876161 ayon-python-api-1.0.2/ayon_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-04-22 08:17:28.000000 ayon-python-api-1.0.2/ayon_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-22 08:17:28.000000 ayon-python-api-1.0.2/ayon_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:17:28.000000 ayon-python-api-1.0.2/ayon_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-22 08:17:28.000000 ayon-python-api-1.0.2/ayon_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 08:17:28.000000 ayon-python-api-1.0.2/ayon_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:17:28.876161 ayon-python-api-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-22 08:17:20.000000 ayon-python-api-1.0.2/setup.py
```

### Comparing `ayon-python-api-1.0.1/LICENSE` & `ayon-python-api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.1/PKG-INFO` & `ayon-python-api-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-1.0.1/README.md` & `ayon-python-api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.1/ayon_api/__init__.py` & `ayon-python-api-1.0.2/ayon_api/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,199 +7,210 @@
 from .server_api import (
     ServerAPI,
 )
 
 from ._api import (
     GlobalServerAPI,
     ServiceContext,
-
     init_service,
-    get_service_name,
     get_service_addon_name,
     get_service_addon_version,
+    get_service_name,
     get_service_addon_settings,
-
     is_connection_created,
     create_connection,
     close_connection,
     change_token,
     set_environments,
     get_server_api_connection,
+    get_base_url,
+    get_rest_url,
+    get_ssl_verify,
+    set_ssl_verify,
+    get_cert,
+    set_cert,
+    get_timeout,
+    set_timeout,
+    get_max_retries,
+    set_max_retries,
     get_site_id,
     set_site_id,
     get_client_version,
     set_client_version,
     get_default_settings_variant,
     set_default_settings_variant,
     get_sender,
     set_sender,
-
-    get_base_url,
-    get_rest_url,
-
-    raw_get,
+    get_info,
+    get_server_version,
+    get_server_version_tuple,
+    get_users,
+    get_user,
     raw_post,
     raw_put,
     raw_patch,
+    raw_get,
     raw_delete,
-
-    get,
     post,
     put,
     patch,
+    get,
     delete,
-
-    get_timeout,
-    set_timeout,
-    get_max_retries,
-    set_max_retries,
-
     get_event,
     get_events,
-    dispatch_event,
     update_event,
+    dispatch_event,
     enroll_event_job,
-
     download_file,
     upload_file,
-
+    trigger_server_restart,
     query_graphql,
-
+    get_graphql_schema,
+    get_server_schema,
+    get_schemas,
+    get_attributes_schema,
+    reset_attributes_schema,
+    set_attribute_config,
+    remove_attribute_config,
+    get_attributes_for_type,
+    get_attributes_fields_for_type,
+    get_default_fields_for_type,
     get_addons_info,
     get_addon_url,
     download_addon_private_file,
-
     get_installers,
     create_installer,
     update_installer,
     delete_installer,
     download_installer,
     upload_installer,
-
     get_dependency_packages,
     create_dependency_package,
     update_dependency_package,
     delete_dependency_package,
-
     download_dependency_package,
     upload_dependency_package,
-
     upload_addon_zip,
-
     get_bundles,
     create_bundle,
     update_bundle,
     delete_bundle,
-
-    get_info,
-    get_server_version,
-    get_server_version_tuple,
-    get_user,
-    get_users,
-
-    get_attributes_for_type,
-    get_attributes_fields_for_type,
-    get_default_fields_for_type,
-
-    get_project_anatomy_preset,
     get_project_anatomy_presets,
+    get_default_anatomy_preset_name,
+    get_project_anatomy_preset,
+    get_build_in_anatomy_preset,
     get_project_roots_by_site,
     get_project_roots_for_site,
-
-    get_addon_site_settings_schema,
     get_addon_settings_schema,
-
+    get_addon_site_settings_schema,
     get_addon_studio_settings,
     get_addon_project_settings,
     get_addon_settings,
+    get_addon_site_settings,
     get_bundle_settings,
     get_addons_studio_settings,
     get_addons_project_settings,
     get_addons_settings,
-
     get_secrets,
     get_secret,
     save_secret,
     delete_secret,
-
+    get_rest_project,
+    get_rest_projects,
+    get_rest_entity_by_id,
+    get_rest_folder,
+    get_rest_task,
+    get_rest_product,
+    get_rest_version,
+    get_rest_representation,
     get_project_names,
     get_projects,
     get_project,
-    create_project,
-    update_project,
-    delete_project,
-
+    get_folders_hierarchy,
+    get_folders_rest,
+    get_folders,
     get_folder_by_id,
-    get_folder_by_name,
     get_folder_by_path,
-    get_folders,
-    get_folders_hierarchy,
-
+    get_folder_by_name,
+    get_folder_ids_with_products,
+    create_folder,
+    update_folder,
+    delete_folder,
     get_tasks,
-    get_task_by_id,
     get_task_by_name,
-
-    get_folder_ids_with_products,
+    get_task_by_id,
+    get_tasks_by_folder_paths,
+    get_tasks_by_folder_path,
+    get_task_by_folder_path,
+    create_task,
+    update_task,
+    delete_task,
+    get_products,
     get_product_by_id,
     get_product_by_name,
-    get_products,
     get_product_types,
     get_project_product_types,
     get_product_type_names,
-
+    create_product,
+    update_product,
+    delete_product,
+    get_versions,
     get_version_by_id,
     get_version_by_name,
-    version_is_latest,
-    get_versions,
-    get_hero_version_by_product_id,
     get_hero_version_by_id,
+    get_hero_version_by_product_id,
     get_hero_versions,
     get_last_versions,
     get_last_version_by_product_id,
     get_last_version_by_product_name,
+    version_is_latest,
+    create_version,
+    update_version,
+    delete_version,
+    get_representations,
     get_representation_by_id,
     get_representation_by_name,
-    get_representations,
     get_representations_parents,
     get_representation_parents,
     get_repre_ids_by_context_filters,
-
+    create_representation,
+    update_representation,
+    delete_representation,
     get_workfiles_info,
     get_workfile_info,
     get_workfile_info_by_id,
-
     get_thumbnail_by_id,
     get_thumbnail,
     get_folder_thumbnail,
     get_version_thumbnail,
     get_workfile_thumbnail,
     create_thumbnail,
     update_thumbnail,
-
+    create_project,
+    update_project,
+    delete_project,
     get_full_link_type_name,
     get_link_types,
     get_link_type,
     create_link_type,
     delete_link_type,
     make_sure_link_type_exists,
-
     create_link,
     delete_link,
     get_entities_links,
-    get_folder_links,
     get_folders_links,
-    get_task_links,
+    get_folder_links,
     get_tasks_links,
-    get_product_links,
+    get_task_links,
     get_products_links,
-    get_version_links,
+    get_product_links,
     get_versions_links,
+    get_version_links,
     get_representations_links,
     get_representation_links,
-
     send_batch_operations,
 )
 
 
 __all__ = (
     "__version__",
 
@@ -207,192 +218,205 @@
     "slugify_string",
     "create_dependency_package_basename",
 
     "ServerAPI",
 
     "GlobalServerAPI",
     "ServiceContext",
-
     "init_service",
-    "get_service_name",
     "get_service_addon_name",
     "get_service_addon_version",
+    "get_service_name",
     "get_service_addon_settings",
-
     "is_connection_created",
     "create_connection",
     "close_connection",
     "change_token",
     "set_environments",
     "get_server_api_connection",
+    "get_base_url",
+    "get_rest_url",
+    "get_ssl_verify",
+    "set_ssl_verify",
+    "get_cert",
+    "set_cert",
+    "get_timeout",
+    "set_timeout",
+    "get_max_retries",
+    "set_max_retries",
     "get_site_id",
     "set_site_id",
     "get_client_version",
     "set_client_version",
     "get_default_settings_variant",
     "set_default_settings_variant",
     "get_sender",
     "set_sender",
-
-    "get_base_url",
-    "get_rest_url",
-
-    "raw_get",
+    "get_info",
+    "get_server_version",
+    "get_server_version_tuple",
+    "get_users",
+    "get_user",
     "raw_post",
     "raw_put",
     "raw_patch",
+    "raw_get",
     "raw_delete",
-
-    "get",
     "post",
     "put",
     "patch",
+    "get",
     "delete",
-
-    "get_timeout",
-    "set_timeout",
-    "get_max_retries",
-    "set_max_retries",
-
     "get_event",
     "get_events",
-    "dispatch_event",
     "update_event",
+    "dispatch_event",
     "enroll_event_job",
-
     "download_file",
     "upload_file",
-
+    "trigger_server_restart",
     "query_graphql",
-
+    "get_graphql_schema",
+    "get_server_schema",
+    "get_schemas",
+    "get_attributes_schema",
+    "reset_attributes_schema",
+    "set_attribute_config",
+    "remove_attribute_config",
+    "get_attributes_for_type",
+    "get_attributes_fields_for_type",
+    "get_default_fields_for_type",
     "get_addons_info",
     "get_addon_url",
     "download_addon_private_file",
-
     "get_installers",
     "create_installer",
     "update_installer",
     "delete_installer",
     "download_installer",
     "upload_installer",
-
     "get_dependency_packages",
     "create_dependency_package",
     "update_dependency_package",
     "delete_dependency_package",
-
     "download_dependency_package",
     "upload_dependency_package",
-
     "upload_addon_zip",
-
     "get_bundles",
     "create_bundle",
     "update_bundle",
     "delete_bundle",
-
-    "get_info",
-    "get_server_version",
-    "get_server_version_tuple",
-    "get_user",
-    "get_users",
-
-    "get_attributes_for_type",
-    "get_attributes_fields_for_type",
-    "get_default_fields_for_type",
-
-    "get_project_anatomy_preset",
     "get_project_anatomy_presets",
+    "get_default_anatomy_preset_name",
+    "get_project_anatomy_preset",
+    "get_build_in_anatomy_preset",
     "get_project_roots_by_site",
     "get_project_roots_for_site",
-
-    "get_addon_site_settings_schema",
     "get_addon_settings_schema",
+    "get_addon_site_settings_schema",
     "get_addon_studio_settings",
     "get_addon_project_settings",
     "get_addon_settings",
+    "get_addon_site_settings",
     "get_bundle_settings",
     "get_addons_studio_settings",
     "get_addons_project_settings",
     "get_addons_settings",
-
     "get_secrets",
     "get_secret",
     "save_secret",
     "delete_secret",
-
+    "get_rest_project",
+    "get_rest_projects",
+    "get_rest_entity_by_id",
+    "get_rest_folder",
+    "get_rest_task",
+    "get_rest_product",
+    "get_rest_version",
+    "get_rest_representation",
     "get_project_names",
     "get_projects",
     "get_project",
-    "create_project",
-    "update_project",
-    "delete_project",
-
+    "get_folders_hierarchy",
+    "get_folders_rest",
+    "get_folders",
     "get_folder_by_id",
-    "get_folder_by_name",
     "get_folder_by_path",
-    "get_folders",
-
+    "get_folder_by_name",
+    "get_folder_ids_with_products",
+    "create_folder",
+    "update_folder",
+    "delete_folder",
     "get_tasks",
-    "get_task_by_id",
     "get_task_by_name",
-
-    "get_folder_ids_with_products",
+    "get_task_by_id",
+    "get_tasks_by_folder_paths",
+    "get_tasks_by_folder_path",
+    "get_task_by_folder_path",
+    "create_task",
+    "update_task",
+    "delete_task",
+    "get_products",
     "get_product_by_id",
     "get_product_by_name",
-    "get_products",
     "get_product_types",
     "get_project_product_types",
     "get_product_type_names",
-
+    "create_product",
+    "update_product",
+    "delete_product",
+    "get_versions",
     "get_version_by_id",
     "get_version_by_name",
-    "version_is_latest",
-    "get_versions",
-    "get_hero_version_by_product_id",
     "get_hero_version_by_id",
+    "get_hero_version_by_product_id",
     "get_hero_versions",
     "get_last_versions",
     "get_last_version_by_product_id",
     "get_last_version_by_product_name",
+    "version_is_latest",
+    "create_version",
+    "update_version",
+    "delete_version",
+    "get_representations",
     "get_representation_by_id",
     "get_representation_by_name",
-    "get_representations",
     "get_representations_parents",
     "get_representation_parents",
     "get_repre_ids_by_context_filters",
-
+    "create_representation",
+    "update_representation",
+    "delete_representation",
     "get_workfiles_info",
     "get_workfile_info",
     "get_workfile_info_by_id",
-
     "get_thumbnail_by_id",
     "get_thumbnail",
     "get_folder_thumbnail",
     "get_version_thumbnail",
     "get_workfile_thumbnail",
     "create_thumbnail",
     "update_thumbnail",
-
+    "create_project",
+    "update_project",
+    "delete_project",
     "get_full_link_type_name",
     "get_link_types",
     "get_link_type",
     "create_link_type",
     "delete_link_type",
     "make_sure_link_type_exists",
-
     "create_link",
     "delete_link",
     "get_entities_links",
-    "get_folder_links",
     "get_folders_links",
-    "get_task_links",
+    "get_folder_links",
     "get_tasks_links",
-    "get_product_links",
+    "get_task_links",
     "get_products_links",
-    "get_version_links",
+    "get_product_links",
     "get_versions_links",
+    "get_version_links",
     "get_representations_links",
     "get_representation_links",
-
     "send_batch_operations",
 )
```

### Comparing `ayon-python-api-1.0.1/ayon_api/constants.py` & `ayon-python-api-1.0.2/ayon_api/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,25 @@
     "updatedAt",
     "apiKeyPreview",
     "attrib.avatarUrl",
     "attrib.email",
     "attrib.fullName",
 }
 
+# --- Folder types ---
+DEFAULT_FOLDER_TYPE_FIELDS = {
+    "name",
+    "icon",
+}
+
+# --- Task types ---
+DEFAULT_TASK_TYPE_FIELDS = {
+    "name",
+}
+
 # --- Product types ---
 DEFAULT_PRODUCT_TYPE_FIELDS = {
     "name",
     "icon",
     "color",
 }
 
@@ -41,14 +52,17 @@
 DEFAULT_PROJECT_FIELDS = {
     "active",
     "name",
     "code",
     "config",
     "createdAt",
     "data",
+    "folderTypes",
+    "taskTypes",
+    "productTypes",
 }
 
 # --- Folders ---
 DEFAULT_FOLDER_FIELDS = {
     "id",
     "name",
     "label",
```

### Comparing `ayon-python-api-1.0.1/ayon_api/entity_hub.py` & `ayon-python-api-1.0.2/ayon_api/entity_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,15 @@
         existing_entity = self._entities_by_id.get(entity_id)
         if existing_entity is not None:
             return existing_entity
 
         if not entity_types:
             return None
 
+        entity_type = None
         entity_data = None
         for entity_type in entity_types:
             if entity_type == "folder":
                 entity_data = self._connection.get_folder_by_id(
                     self.project_name,
                     entity_id,
                     fields=self._get_folder_fields(),
@@ -453,36 +454,38 @@
             return
 
         parent.add_child(entity_id)
         self.reset_immutable_for_hierarchy_cache(parent_id)
 
     def _query_entity_children(self, entity):
         folder_fields = self._get_folder_fields()
+        task_fields = self._get_task_fields()
         tasks = []
         folders = []
         if entity.entity_type == "project":
             folders = list(self._connection.get_folders(
                 entity["name"],
                 parent_ids=[entity.id],
                 fields=folder_fields,
-                own_attributes=True
+                own_attributes=True,
             ))
 
         elif entity.entity_type == "folder":
             folders = list(self._connection.get_folders(
                 self.project_entity["name"],
                 parent_ids=[entity.id],
                 fields=folder_fields,
-                own_attributes=True
+                own_attributes=True,
             ))
 
             tasks = list(self._connection.get_tasks(
                 self.project_entity["name"],
                 folder_ids=[entity.id],
-                own_attributes=True
+                fields=task_fields,
+                own_attributes=True,
             ))
 
         children_ids = {
             child.id
             for child in self._entities_by_parent_id[entity.id]
         }
         for folder in folders:
@@ -597,30 +600,40 @@
     def _get_folder_fields(self):
         folder_fields = set(
             self._connection.get_default_fields_for_type("folder")
         )
         folder_fields.add("hasProducts")
         if self._allow_data_changes:
             folder_fields.add("data")
+        folder_fields |= {"status", "tags"}
         return folder_fields
 
+    def _get_task_fields(self):
+        task_fields = set(
+            self._connection.get_default_fields_for_type("task")
+        )
+        task_fields |= {"status", "tags"}
+        return task_fields
+
     def query_entities_from_server(self):
         """Query whole project at once."""
         project_entity = self.fill_project_from_server()
 
         folder_fields = self._get_folder_fields()
+        task_fields = self._get_task_fields()
 
         folders = self._connection.get_folders(
             project_entity.name,
             fields=folder_fields,
-            own_attributes=True
+            own_attributes=True,
         )
         tasks = self._connection.get_tasks(
             project_entity.name,
-            own_attributes=True
+            fields=task_fields,
+            own_attributes=True,
         )
         folders_by_parent_id = collections.defaultdict(list)
         for folder in folders:
             parent_id = folder["parentId"]
             folders_by_parent_id[parent_id].append(folder)
 
         tasks_by_parent_id = collections.defaultdict(list)
@@ -2347,14 +2360,27 @@
     def set_statuses(self, statuses):
         self._statuses_obj.set(statuses)
 
     folder_types = property(get_folder_types, set_folder_types)
     task_types = property(get_task_types, set_task_types)
     statuses = property(get_statuses, set_statuses)
 
+    def get_status_by_slugified_name(self, name):
+        """Find status by name.
+
+        Args:
+            name (str): Status name.
+
+
+        Returns:
+            Union[ProjectStatus, None]: Status object or None.
+
+        """
+        return self._statuses_obj.get_status_by_slugified_name(name)
+
     def lock(self):
         super(ProjectEntity, self).lock()
         self._orig_folder_types = copy.deepcopy(self._folder_types)
         self._orig_task_types = copy.deepcopy(self._task_types)
         self._statuses_obj.lock()
 
     @property
@@ -2415,26 +2441,44 @@
         created (Optional[bool]): Entity is new. When 'None' is passed the
             value is defined based on value of 'entity_id'.
     """
 
     entity_type = "folder"
     parent_entity_types = ["folder", "project"]
 
-    def __init__(self, folder_type, *args, label=None, path=None, **kwargs):
+    def __init__(
+        self,
+        folder_type,
+        *args,
+        label=None,
+        path=None,
+        tags=None,
+        status=UNKNOWN_VALUE,
+        **kwargs
+    ):
         super(FolderEntity, self).__init__(*args, **kwargs)
         # Autofill project as parent of folder if is not yet set
         # - this can be guessed only if folder was just created
         if self.created and self._parent_id is UNKNOWN_VALUE:
             self._parent_id = self.project_name
 
+        if tags is None:
+            tags = []
+        else:
+            tags = list(tags)
+
         self._folder_type = folder_type
         self._label = label
+        self._tags = copy.deepcopy(tags)
+        self._status = status
 
         self._orig_folder_type = folder_type
         self._orig_label = label
+        self._orig_status = status
+        self._orig_tags = copy.deepcopy(tags)
         # Know if folder has any products
         # - is used to know if folder allows hierarchy changes
         self._has_published_content = False
         self._path = path
 
     def get_folder_type(self):
         return self._folder_type
@@ -2448,14 +2492,60 @@
         return self._label
 
     def set_label(self, label):
         self._label = label
 
     label = property(get_label, set_label)
 
+    def get_status(self):
+        """Folder status.
+
+        Returns:
+            Union[str, UNKNOWN_VALUE]: Folder status or 'UNKNOWN_VALUE'.
+
+        """
+        return self._status
+
+    def set_status(self, status_name):
+        """Set folder status.
+
+        Args:
+            status_name (str): Status name.
+
+        """
+        project_entity = self._entity_hub.project_entity
+        status = project_entity.get_status_by_slugified_name(status_name)
+        if status is None:
+            raise ValueError(
+                f"Status {status_name} is not available on project."
+            )
+        self._status = status_name
+
+    status = property(get_status, set_status)
+
+    def get_tags(self):
+        """Folder tags.
+
+        Returns:
+            list[str]: Folder tags.
+
+        """
+        return self._tags
+
+    def set_tags(self, tags):
+        """Change tags.
+
+        Args:
+            tags (Iterable[str]): Tags.
+
+        """
+        self._tags = list(tags)
+
+    tags = property(get_tags, set_tags)
+
     def get_path(self, dynamic_value=True):
         if not dynamic_value:
             return self._path
 
         if self._path is None:
             parent = self.parent
             if parent.entity_type == "folder":
@@ -2494,28 +2584,36 @@
         if self.has_published_content:
             return True
         return None
 
     def lock(self):
         super(FolderEntity, self).lock()
         self._orig_folder_type = self._folder_type
+        self._orig_status = self._status
+        self._orig_tags = copy.deepcopy(self._tags)
 
     @property
     def changes(self):
         changes = self._get_default_changes()
 
         if self._orig_parent_id != self._parent_id:
             parent_id = self._parent_id
             if parent_id == self.project_name:
                 parent_id = None
             changes["parentId"] = parent_id
 
         if self._orig_folder_type != self._folder_type:
             changes["folderType"] = self._folder_type
 
+        if self._orig_status != self._status:
+            changes["status"] = self._status
+
+        if self._orig_tags != self._tags:
+            changes["tags"] = self._tags
+
         label = self._label
         if self._name == label:
             label = None
 
         if label != self._orig_label:
             changes["label"] = label
 
@@ -2526,14 +2624,16 @@
         parent_id = folder["parentId"]
         if parent_id is None:
             parent_id = entity_hub.project_entity.id
         return cls(
             folder["folderType"],
             label=folder["label"],
             path=folder["path"],
+            status=folder["status"],
+            tags=folder["tags"],
             entity_id=folder["id"],
             parent_id=parent_id,
             name=folder["name"],
             data=folder.get("data"),
             attribs=folder["ownAttrib"],
             active=folder["active"],
             thumbnail_id=folder["thumbnailId"],
@@ -2557,14 +2657,21 @@
             "folderType": self.folder_type,
             "parentId": parent_id,
         }
         attrib = self.attribs.to_dict()
         if attrib:
             output["attrib"] = attrib
 
+        # Add tags only if are available
+        if self.tags:
+            output["tags"] = list(self.tags)
+
+        if self.status is not UNKNOWN_VALUE:
+            output["status"] = self.status
+
         if self.active is not UNKNOWN_VALUE:
             output["active"] = self.active
 
         if self.thumbnail_id is not UNKNOWN_VALUE:
             output["thumbnailId"] = self.thumbnail_id
 
         if (
@@ -2595,28 +2702,47 @@
         created (Optional[bool]): Entity is new. When 'None' is passed the
             value is defined based on value of 'entity_id'.
     """
 
     entity_type = "task"
     parent_entity_types = ["folder"]
 
-    def __init__(self, task_type, *args, label=None, **kwargs):
+    def __init__(
+        self,
+        task_type,
+        *args,
+        label=None,
+        tags=None,
+        status=UNKNOWN_VALUE,
+        **kwargs
+    ):
         super(TaskEntity, self).__init__(*args, **kwargs)
 
+        if tags is None:
+            tags = []
+        else:
+            tags = list(tags)
+
         self._task_type = task_type
         self._label = label
+        self._status = status
+        self._tags = tags
 
         self._orig_task_type = task_type
         self._orig_label = label
+        self._orig_status = status
+        self._orig_tags = copy.deepcopy(tags)
 
         self._children_ids = set()
 
     def lock(self):
         super(TaskEntity, self).lock()
         self._orig_task_type = self._task_type
+        self._orig_status = self._status
+        self._orig_tags = copy.deepcopy(self._tags)
 
     def get_task_type(self):
         return self._task_type
 
     def set_task_type(self, task_type):
         self._task_type = task_type
 
@@ -2626,27 +2752,79 @@
         return self._label
 
     def set_label(self, label):
         self._label = label
 
     label = property(get_label, set_label)
 
+    def get_status(self):
+        """Folder status.
+
+        Returns:
+            Union[str, UNKNOWN_VALUE]: Folder status or 'UNKNOWN_VALUE'.
+
+        """
+        return self._status
+
+    def set_status(self, status_name):
+        """Set folder status.
+
+        Args:
+            status_name (str): Status name.
+
+        """
+        project_entity = self._entity_hub.project_entity
+        status = project_entity.get_status_by_slugified_name(status_name)
+        if status is None:
+            raise ValueError(
+                f"Status {status_name} is not available on project."
+            )
+        self._status = status_name
+
+    status = property(get_status, set_status)
+
+    def get_tags(self):
+        """Folder tags.
+
+        Returns:
+            list[str]: Folder tags.
+
+        """
+        return self._tags
+
+    def set_tags(self, tags):
+        """Change tags.
+
+        Args:
+            tags (Iterable[str]): Tags.
+
+        """
+        self._tags = list(tags)
+
+    tags = property(get_tags, set_tags)
+
     def add_child(self, child):
         raise ValueError("Task does not support to add children")
 
     @property
     def changes(self):
         changes = self._get_default_changes()
 
         if self._orig_parent_id != self._parent_id:
             changes["folderId"] = self._parent_id
 
         if self._orig_task_type != self._task_type:
             changes["taskType"] = self._task_type
 
+        if self._orig_status != self._status:
+            changes["status"] = self._status
+
+        if self._orig_tags != self._tags:
+            changes["tags"] = self._tags
+
         label = self._label
         if self._name == label:
             label = None
 
         if label != self._orig_label:
             changes["label"] = label
 
@@ -2654,14 +2832,16 @@
 
     @classmethod
     def from_entity_data(cls, task, entity_hub):
         return cls(
             task["taskType"],
             entity_id=task["id"],
             label=task["label"],
+            status=task["status"],
+            tags=task["tags"],
             parent_id=task["folderId"],
             name=task["name"],
             data=task.get("data"),
             attribs=task["ownAttrib"],
             active=task["active"],
             created=False,
             entity_hub=entity_hub
@@ -2680,13 +2860,19 @@
         attrib = self.attribs.to_dict()
         if attrib:
             output["attrib"] = attrib
 
         if self.active is not UNKNOWN_VALUE:
             output["active"] = self.active
 
+        if self.status is not UNKNOWN_VALUE:
+            output["status"] = self.status
+
+        if self.tags:
+            output["tags"] = self.tags
+
         if (
             self._entity_hub.allow_data_changes
             and self._data is not UNKNOWN_VALUE
         ):
             output["data"] = self._data
         return output
```

### Comparing `ayon-python-api-1.0.1/ayon_api/events.py` & `ayon-python-api-1.0.2/ayon_api/events.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.1/ayon_api/exceptions.py` & `ayon-python-api-1.0.2/ayon_api/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,14 +29,24 @@
     pass
 
 
 class ServerNotReached(ServerError):
     pass
 
 
+class UnsupportedServerVersion(ServerError):
+    """Server version does not support the requested operation.
+
+    This is used for known incompatibilities between the python api and
+        server. E.g. can be used when endpoint is not available anymore, or
+        is not yet available on server.
+    """
+    pass
+
+
 class RequestError(Exception):
     def __init__(self, message, response):
         self.response = response
         super(RequestError, self).__init__(message)
 
 
 class HTTPRequestError(RequestError):
```

### Comparing `ayon-python-api-1.0.1/ayon_api/graphql.py` & `ayon-python-api-1.0.2/ayon_api/graphql.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-1.0.1/ayon_api/graphql_queries.py` & `ayon-python-api-1.0.2/ayon_api/graphql_queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,14 +258,60 @@
             continue
 
         for k, v in value.items():
             query_queue.append((k, v, field))
     return query
 
 
+def tasks_by_folder_paths_graphql_query(fields):
+    query = GraphQlQuery("TasksByFolderPathQuery")
+    project_name_var = query.add_variable("projectName", "String!")
+    task_names_var = query.add_variable("taskNames", "[String!]")
+    task_types_var = query.add_variable("taskTypes", "[String!]")
+    folder_paths_var = query.add_variable("folderPaths", "[String!]")
+    assignees_any_var = query.add_variable("taskAssigneesAny", "[String!]")
+    assignees_all_var = query.add_variable("taskAssigneesAll", "[String!]")
+    statuses_var = query.add_variable("taskStatuses", "[String!]")
+    tags_var = query.add_variable("taskTags", "[String!]")
+
+    project_field = query.add_field("project")
+    project_field.set_filter("name", project_name_var)
+
+    folders_field = project_field.add_field_with_edges("folders")
+    folders_field.add_field("path")
+    folders_field.set_filter("paths", folder_paths_var)
+
+    tasks_field = folders_field.add_field_with_edges("tasks")
+    # WARNING: At moment when this been created 'names' filter is not supported
+    tasks_field.set_filter("names", task_names_var)
+    tasks_field.set_filter("taskTypes", task_types_var)
+    tasks_field.set_filter("assigneesAny", assignees_any_var)
+    tasks_field.set_filter("assignees", assignees_all_var)
+    tasks_field.set_filter("statuses", statuses_var)
+    tasks_field.set_filter("tags", tags_var)
+
+    nested_fields = fields_to_dict(fields)
+    add_links_fields(tasks_field, nested_fields)
+
+    query_queue = collections.deque()
+    for key, value in nested_fields.items():
+        query_queue.append((key, value, tasks_field))
+
+    while query_queue:
+        item = query_queue.popleft()
+        key, value, parent = item
+        field = parent.add_field(key)
+        if value is FIELD_VALUE:
+            continue
+
+        for k, v in value.items():
+            query_queue.append((k, v, field))
+    return query
+
+
 def products_graphql_query(fields):
     query = GraphQlQuery("ProductsQuery")
 
     project_name_var = query.add_variable("projectName", "String!")
     product_ids_var = query.add_variable("productIds", "[String!]")
     product_names_var = query.add_variable("productNames", "[String!]")
     folder_ids_var = query.add_variable("folderIds", "[String!]")
```

### Comparing `ayon-python-api-1.0.1/ayon_api/operations.py` & `ayon-python-api-1.0.2/ayon_api/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,771 +1,700 @@
 import os
-import copy
-import collections
+import re
+import datetime
 import uuid
-from abc import ABCMeta, abstractmethod
-
-import six
+import string
+import platform
+import collections
+try:
+    # Python 3
+    from urllib.parse import urlparse, urlencode
+except ImportError:
+    # Python 2
+    from urlparse import urlparse
+    from urllib import urlencode
+
+import requests
+import unidecode
+
+from .constants import (
+    SERVER_TIMEOUT_ENV_KEY,
+    DEFAULT_VARIANT_ENV_KEY,
+    SITE_ID_ENV_KEY,
+)
+from .exceptions import UrlError
+
+REMOVED_VALUE = object()
+NOT_SET = object()
+SLUGIFY_WHITELIST = string.ascii_letters + string.digits
+SLUGIFY_SEP_WHITELIST = " ,./\\;:!|*^#@~+-_="
+
+RepresentationParents = collections.namedtuple(
+    "RepresentationParents",
+    ("version", "product", "folder", "project")
+)
 
-from ._api import get_server_api_connection
-from .utils import create_entity_id, REMOVED_VALUE
 
+def get_default_timeout():
+    """Default value for requests timeout.
 
-def _create_or_convert_to_id(entity_id=None):
-    if entity_id is None:
-        return create_entity_id()
+    First looks for environment variable SERVER_TIMEOUT_ENV_KEY which
+    can affect timeout value. If not available then use 10.0 s.
 
-    # Validate if can be converted to uuid
-    uuid.UUID(entity_id)
-    return entity_id
+    Returns:
+        float: Timeout value in seconds.
 
+    """
+    try:
+        return float(os.environ.get(SERVER_TIMEOUT_ENV_KEY))
+    except (ValueError, TypeError):
+        pass
+    return 10.0
 
-def new_folder_entity(
-    name,
-    folder_type,
-    parent_id=None,
-    status=None,
-    tags=None,
-    attribs=None,
-    data=None,
-    thumbnail_id=None,
-    entity_id=None
-):
-    """Create skeleton data of folder entity.
 
-    Args:
-        name (str): Is considered as unique identifier of folder in project.
-        folder_type (str): Type of folder.
-        parent_id (Optional[str]): Parent folder id.
-        status (Optional[str]): Product status.
-        tags (Optional[List[str]]): List of tags.
-        attribs (Optional[Dict[str, Any]]): Explicitly set attributes
-            of folder.
-        data (Optional[Dict[str, Any]]): Custom folder data. Empty dictionary
-            is used if not passed.
-        thumbnail_id (Optional[str]): Thumbnail id related to folder.
-        entity_id (Optional[str]): Predefined id of entity. New id is
-            created if not passed.
+def get_default_settings_variant():
+    """Default settings variant.
 
     Returns:
-        Dict[str, Any]: Skeleton of folder entity.
+        str: Settings variant from environment variable or 'production'.
 
     """
-    if attribs is None:
-        attribs = {}
+    return os.environ.get(DEFAULT_VARIANT_ENV_KEY) or "production"
 
-    if data is None:
-        data = {}
 
-    if parent_id is not None:
-        parent_id = _create_or_convert_to_id(parent_id)
-
-    output = {
-        "id": _create_or_convert_to_id(entity_id),
-        "name": name,
-        # This will be ignored
-        "folderType": folder_type,
-        "parentId": parent_id,
-        "data": data,
-        "attrib": attribs,
-        "thumbnailId": thumbnail_id
-    }
-    if status:
-        output["status"] = status
-    if tags:
-        output["tags"] = tags
-    return output
+def get_default_site_id():
+    """Site id used for server connection.
 
+    Returns:
+        Union[str, None]: Site id from environment variable or None.
 
-def new_product_entity(
-    name,
-    product_type,
-    folder_id,
-    status=None,
-    tags=None,
-    attribs=None,
-    data=None,
-    entity_id=None
-):
-    """Create skeleton data of product entity.
+    """
+    return os.environ.get(SITE_ID_ENV_KEY)
 
-    Args:
-        name (str): Is considered as unique identifier of
-            product under folder.
-        product_type (str): Product type.
-        folder_id (str): Parent folder id.
-        status (Optional[str]): Product status.
-        tags (Optional[List[str]]): List of tags.
-        attribs (Optional[Dict[str, Any]]): Explicitly set attributes
-            of product.
-        data (Optional[Dict[str, Any]]): product entity data. Empty dictionary
-            is used if not passed.
-        entity_id (Optional[str]): Predefined id of entity. New id is
-            created if not passed.
 
-    Returns:
-        Dict[str, Any]: Skeleton of product entity.
+class ThumbnailContent:
+    """Wrapper for thumbnail content.
+
+    Args:
+        project_name (str): Project name.
+        thumbnail_id (Union[str, None]): Thumbnail id.
+        content_type (Union[str, None]): Content type e.g. 'image/png'.
+        content (Union[bytes, None]): Thumbnail content.
 
     """
-    if attribs is None:
-        attribs = {}
+    def __init__(self, project_name, thumbnail_id, content, content_type):
+        self.project_name = project_name
+        self.thumbnail_id = thumbnail_id
+        self.content_type = content_type
+        self.content = content or b""
 
-    if data is None:
-        data = {}
+    @property
+    def id(self):
+        """Wrapper for thumbnail id."""
+        return self.thumbnail_id
 
-    output = {
-        "id": _create_or_convert_to_id(entity_id),
-        "name": name,
-        "productType": product_type,
-        "attrib": attribs,
-        "data": data,
-        "folderId": _create_or_convert_to_id(folder_id),
-    }
-    if status:
-        output["status"] = status
-    if tags:
-        output["tags"] = tags
-    return output
+    @property
+    def is_valid(self):
+        """Content of thumbnail is valid.
 
+        Returns:
+            bool: Content is valid and can be used.
 
-def new_version_entity(
-    version,
-    product_id,
-    task_id=None,
-    thumbnail_id=None,
-    author=None,
-    status=None,
-    tags=None,
-    attribs=None,
-    data=None,
-    entity_id=None
-):
-    """Create skeleton data of version entity.
+        """
+        return (
+            self.thumbnail_id is not None
+            and self.content_type is not None
+        )
+
+
+def prepare_query_string(key_values):
+    """Prepare data to query string.
+
+    If there are any values a query starting with '?' is returned otherwise
+    an empty string.
 
     Args:
-        version (int): Is considered as unique identifier of version
-            under product.
-        product_id (str): Parent product id.
-        task_id (Optional[str]): Task id under which product was created.
-        thumbnail_id (Optional[str]): Thumbnail related to version.
-        author (Optional[str]): Name of version author.
-        status (Optional[str]): Version status.
-        tags (Optional[List[str]]): List of tags.
-        attribs (Optional[Dict[str, Any]]): Explicitly set attributes
-            of version.
-        data (Optional[Dict[str, Any]]): Version entity custom data.
-        entity_id (Optional[str]): Predefined id of entity. New id is
-            created if not passed.
+         dict[str, Any]: Query values.
 
     Returns:
-        Dict[str, Any]: Skeleton of version entity.
+        str: Query string.
 
     """
-    if attribs is None:
-        attribs = {}
-
-    if data is None:
-        data = {}
+    if not key_values:
+        return ""
+    return "?{}".format(urlencode(key_values))
 
-    if data is None:
-        data = {}
 
-    output = {
-        "id": _create_or_convert_to_id(entity_id),
-        "version": int(version),
-        "productId": _create_or_convert_to_id(product_id),
-        "attrib": attribs,
-        "data": data
-    }
-    if task_id:
-        output["taskId"] = task_id
-    if thumbnail_id:
-        output["thumbnailId"] = thumbnail_id
-    if author:
-        output["author"] = author
-    if tags:
-        output["tags"] = tags
-    if status:
-        output["status"] = status
-    return output
+def create_entity_id():
+    return uuid.uuid1().hex
 
 
-def new_hero_version_entity(
-    version,
-    product_id,
-    task_id=None,
-    thumbnail_id=None,
-    author=None,
-    status=None,
-    tags=None,
-    attribs=None,
-    data=None,
-    entity_id=None
-):
-    """Create skeleton data of hero version entity.
+def convert_entity_id(entity_id):
+    if not entity_id:
+        return None
 
-    Args:
-        version (int): Is considered as unique identifier of version
-            under product. Should be same as standard version if there is any.
-        product_id (str): Parent product id.
-        task_id (Optional[str]): Task id under which product was created.
-        thumbnail_id (Optional[str]): Thumbnail related to version.
-        author (Optional[str]): Name of version author.
-        status (Optional[str]): Version status.
-        tags (Optional[List[str]]): List of tags.
-        attribs (Optional[Dict[str, Any]]): Explicitly set attributes
-            of version.
-        data (Optional[Dict[str, Any]]): Version entity data.
-        entity_id (Optional[str]): Predefined id of entity. New id is
-            created if not passed.
+    if isinstance(entity_id, uuid.UUID):
+        return entity_id.hex
 
-    Returns:
-        Dict[str, Any]: Skeleton of version entity.
+    try:
+        return uuid.UUID(entity_id).hex
 
-    """
-    if attribs is None:
-        attribs = {}
+    except (TypeError, ValueError, AttributeError):
+        pass
+    return None
 
-    if data is None:
-        data = {}
 
-    output = {
-        "id": _create_or_convert_to_id(entity_id),
-        "version": -abs(int(version)),
-        "productId": product_id,
-        "attrib": attribs,
-        "data": data
-    }
-    if task_id:
-        output["taskId"] = task_id
-    if thumbnail_id:
-        output["thumbnailId"] = thumbnail_id
-    if author:
-        output["author"] = author
-    if tags:
-        output["tags"] = tags
-    if status:
-        output["status"] = status
+def convert_or_create_entity_id(entity_id=None):
+    output = convert_entity_id(entity_id)
+    if output is None:
+        output = create_entity_id()
     return output
 
 
-def new_representation_entity(
-    name,
-    version_id,
-    files,
-    status=None,
-    tags=None,
-    attribs=None,
-    data=None,
-    entity_id=None
+def entity_data_json_default(value):
+    if isinstance(value, datetime.datetime):
+        return int(value.timestamp())
+
+    raise TypeError(
+        "Object of type {} is not JSON serializable".format(str(type(value)))
+    )
+
+
+def slugify_string(
+    input_string,
+    separator="_",
+    slug_whitelist=SLUGIFY_WHITELIST,
+    split_chars=SLUGIFY_SEP_WHITELIST,
+    min_length=1,
+    lower=False,
+    make_set=False,
 ):
-    """Create skeleton data of representation entity.
+    """Slugify a text string.
 
-    Args:
-        name (str): Representation name considered as unique identifier
-            of representation under version.
-        version_id (str): Parent version id.
-        files (list[dict[str, str]]): List of files in representation.
-        status (Optional[str]): Representation status.
-        tags (Optional[List[str]]): List of tags.
-        attribs (Optional[Dict[str, Any]]): Explicitly set attributes
-            of representation.
-        data (Optional[Dict[str, Any]]): Representation entity data.
-        entity_id (Optional[str]): Predefined id of entity. New id is created
-            if not passed.
+    This function removes transliterates input string to ASCII, removes
+    special characters and use join resulting elements using
+    specified separator.
+
+    Args:
+        input_string (str): Input string to slugify
+        separator (str): A string used to separate returned elements
+            (default: "_")
+        slug_whitelist (str): Characters allowed in the output
+            (default: ascii letters, digits and the separator)
+        split_chars (str): Set of characters used for word splitting
+            (there is a sane default)
+        lower (bool): Convert to lower-case (default: False)
+        make_set (bool): Return "set" object instead of string.
+        min_length (int): Minimal length of an element (word).
 
     Returns:
-        Dict[str, Any]: Skeleton of representation entity.
+        Union[str, Set[str]]: Based on 'make_set' value returns slugified
+            string.
 
     """
-    if attribs is None:
-        attribs = {}
+    tmp_string = unidecode.unidecode(input_string)
+    if lower:
+        tmp_string = tmp_string.lower()
+
+    parts = [
+        # Remove all characters that are not in whitelist
+        re.sub("[^{}]".format(re.escape(slug_whitelist)), "", part)
+        # Split text into part by split characters
+        for part in re.split("[{}]".format(re.escape(split_chars)), tmp_string)
+    ]
+    # Filter text parts by length
+    filtered_parts = [
+        part
+        for part in parts
+        if len(part) >= min_length
+    ]
+    if make_set:
+        return set(filtered_parts)
+    return separator.join(filtered_parts)
+
+
+def failed_json_default(value):
+    return "< Failed value {} > {}".format(type(value), str(value))
+
+
+def prepare_attribute_changes(old_entity, new_entity, replace=False):
+    attrib_changes = {}
+    new_attrib = new_entity.get("attrib")
+    old_attrib = old_entity.get("attrib")
+    if new_attrib is None:
+        if not replace:
+            return attrib_changes
+        new_attrib = {}
+
+    if old_attrib is None:
+        return new_attrib
+
+    for attr, new_attr_value in new_attrib.items():
+        old_attr_value = old_attrib.get(attr)
+        if old_attr_value != new_attr_value:
+            attrib_changes[attr] = new_attr_value
+
+    if replace:
+        for attr in old_attrib:
+            if attr not in new_attrib:
+                attrib_changes[attr] = REMOVED_VALUE
+
+    return attrib_changes
+
+
+def prepare_entity_changes(old_entity, new_entity, replace=False):
+    """Prepare changes of entities."""
+    changes = {}
+    for key, new_value in new_entity.items():
+        if key == "attrib":
+            continue
+
+        old_value = old_entity.get(key)
+        if old_value != new_value:
+            changes[key] = new_value
+
+    if replace:
+        for key in old_entity:
+            if key not in new_entity:
+                changes[key] = REMOVED_VALUE
+
+    attr_changes = prepare_attribute_changes(old_entity, new_entity, replace)
+    if attr_changes:
+        changes["attrib"] = attr_changes
+    return changes
+
+
+def _try_parse_url(url):
+    try:
+        return urlparse(url)
+    except BaseException:
+        return None
+
+
+def _try_connect_to_server(url, timeout=None):
+    if timeout is None:
+        timeout = get_default_timeout()
+    try:
+        # TODO add validation if the url lead to AYON server
+        #   - this won't validate if the url lead to 'google.com'
+        requests.get(url, timeout=timeout)
+
+    except BaseException:
+        return False
+    return True
+
+
+def login_to_server(url, username, password, timeout=None):
+    """Use login to the server to receive token.
+
+    Args:
+        url (str): Server url.
+        username (str): User's username.
+        password (str): User's password.
+        timeout (Optional[float]): Timeout for request. Value from
+            'get_default_timeout' is used if not specified.
 
-    if data is None:
-        data = {}
+    Returns:
+        Union[str, None]: User's token if login was successfull.
+            Otherwise 'None'.
 
-    output = {
-        "id": _create_or_convert_to_id(entity_id),
-        "versionId": _create_or_convert_to_id(version_id),
-        "files": files,
-        "name": name,
-        "data": data,
-        "attrib": attribs
+    """
+    if timeout is None:
+        timeout = get_default_timeout()
+    headers = {"Content-Type": "application/json"}
+    response = requests.post(
+        "{}/api/auth/login".format(url),
+        headers=headers,
+        json={
+            "name": username,
+            "password": password
+        },
+        timeout=timeout,
+    )
+    token = None
+    # 200 - success
+    # 401 - invalid credentials
+    # *   - other issues
+    if response.status_code == 200:
+        token = response.json()["token"]
+    return token
+
+
+def logout_from_server(url, token, timeout=None):
+    """Logout from server and throw token away.
+
+    Args:
+        url (str): Url from which should be logged out.
+        token (str): Token which should be used to log out.
+        timeout (Optional[float]): Timeout for request. Value from
+            'get_default_timeout' is used if not specified.
+
+    """
+    if timeout is None:
+        timeout = get_default_timeout()
+    headers = {
+        "Content-Type": "application/json",
+        "Authorization": "Bearer {}".format(token)
     }
-    if tags:
-        output["tags"] = tags
-    if status:
-        output["status"] = status
-    return output
+    requests.post(
+        url + "/api/auth/logout",
+        headers=headers,
+        timeout=timeout,
+    )
 
 
-def new_workfile_info(
-    filepath,
-    task_id,
-    status=None,
-    tags=None,
-    attribs=None,
-    description=None,
-    data=None,
-    entity_id=None
-):
-    """Create skeleton data of workfile info entity.
+def is_token_valid(url, token, timeout=None):
+    """Check if token is valid.
 
-    Workfile entity is at this moment used primarily for artist notes.
+    Token can be a user token or service api key.
 
     Args:
-        filepath (str): Rootless workfile filepath.
-        task_id (str): Task under which was workfile created.
-        status (Optional[str]): Workfile status.
-        tags (Optional[List[str]]): Workfile tags.
-        attribs (Options[dic[str, Any]]): Explicitly set attributes.
-        description (Optional[str]): Workfile description.
-        data (Optional[Dict[str, Any]]): Additional metadata.
-        entity_id (Optional[str]): Predefined id of entity. New id is created
-            if not passed.
+        url (str): Server url.
+        token (str): User's token.
+        timeout (Optional[float]): Timeout for request. Value from
+            'get_default_timeout' is used if not specified.
 
     Returns:
-        Dict[str, Any]: Skeleton of workfile info entity.
+        bool: True if token is valid.
 
     """
-    if attribs is None:
-        attribs = {}
+    if timeout is None:
+        timeout = get_default_timeout()
 
-    if "extension" not in attribs:
-        attribs["extension"] = os.path.splitext(filepath)[-1]
-
-    if description:
-        attribs["description"] = description
+    base_headers = {
+        "Content-Type": "application/json",
+    }
+    for header_value in (
+        {"Authorization": "Bearer {}".format(token)},
+        {"X-Api-Key": token},
+    ):
+        headers = base_headers.copy()
+        headers.update(header_value)
+        response = requests.get(
+            "{}/api/users/me".format(url),
+            headers=headers,
+            timeout=timeout,
+        )
+        if response.status_code == 200:
+            return True
+    return False
 
-    if not data:
-        data = {}
 
-    output = {
-        "id": _create_or_convert_to_id(entity_id),
-        "taskId": task_id,
-        "path": filepath,
-        "data": data,
-        "attrib": attribs
-    }
-    if status:
-        output["status"] = status
+def validate_url(url, timeout=None):
+    """Validate url if is valid and server is available.
 
-    if tags:
-        output["tags"] = tags
-    return output
+    Validation checks if can be parsed as url and contains scheme.
 
+    Function will try to autofix url thus will return modified url when
+    connection to server works.
 
-@six.add_metaclass(ABCMeta)
-class AbstractOperation(object):
-    """Base operation class.
+    ```python
+    my_url = "my.server.url"
+    try:
+        # Store new url
+        validated_url = validate_url(my_url)
 
-    Opration represent a call into database. The call can create, change or
-    remove data.
+    except UrlError:
+        # Handle invalid url
+        ...
+    ```
 
     Args:
-        project_name (str): On which project operation will happen.
-        entity_type (str): Type of entity on which change happens.
-            e.g. 'folder', 'representation' etc.
+        url (str): Server url.
+        timeout (Optional[int]): Timeout in seconds for connection to server.
 
-    """
-    def __init__(self, project_name, entity_type, session):
-        self._project_name = project_name
-        self._entity_type = entity_type
-        self._session = session
-        self._id = str(uuid.uuid4())
+    Returns:
+        Url which was used to connect to server.
 
-    @property
-    def project_name(self):
-        return self._project_name
+    Raises:
+        UrlError: Error with short description and hints for user.
 
-    @property
-    def id(self):
-        """Identifier of operation."""
-        return self._id
+    """
+    stripperd_url = url.strip()
+    if not stripperd_url:
+        raise UrlError(
+            "Invalid url format. Url is empty.",
+            title="Invalid url format",
+            hints=["url seems to be empty"]
+        )
 
-    @property
-    def entity_type(self):
-        return self._entity_type
+    # Not sure if this is good idea?
+    modified_url = stripperd_url.rstrip("/")
+    parsed_url = _try_parse_url(modified_url)
+    universal_hints = [
+        "does the url work in browser?"
+    ]
+    if parsed_url is None:
+        raise UrlError(
+            "Invalid url format. Url cannot be parsed as url \"{}\".".format(
+                modified_url
+            ),
+            title="Invalid url format",
+            hints=universal_hints
+        )
 
-    @property
-    @abstractmethod
-    def operation_name(self):
-        """Stringified type of operation."""
-        pass
+    # Try add 'https://' scheme if is missing
+    # - this will trigger UrlError if both will crash
+    if not parsed_url.scheme:
+        new_url = "https://" + modified_url
+        if _try_connect_to_server(new_url, timeout=timeout):
+            return new_url
+
+    if _try_connect_to_server(modified_url, timeout=timeout):
+        return modified_url
+
+    hints = []
+    if "/" in parsed_url.path or not parsed_url.scheme:
+        new_path = parsed_url.path.split("/")[0]
+        if not parsed_url.scheme:
+            new_path = "https://" + new_path
 
-    def to_data(self):
-        """Convert opration to data that can be converted to json or others.
+        hints.append(
+            "did you mean \"{}\"?".format(parsed_url.scheme + new_path)
+        )
 
-        Returns:
-            Dict[str, Any]: Description of operation.
+    raise UrlError(
+        "Couldn't connect to server on \"{}\"".format(url),
+        title="Couldn't connect to server",
+        hints=hints + universal_hints
+    )
+
+
+class TransferProgress:
+    """Object to store progress of download/upload from/to server."""
+
+    def __init__(self):
+        self._started = False
+        self._transfer_done = False
+        self._transferred = 0
+        self._content_size = None
 
-        """
-        return {
-            "id": self._id,
-            "entity_type": self.entity_type,
-            "project_name": self.project_name,
-            "operation": self.operation_name
-        }
+        self._failed = False
+        self._fail_reason = None
 
+        self._source_url = "N/A"
+        self._destination_url = "N/A"
 
-class CreateOperation(AbstractOperation):
-    """Opeartion to create an entity.
+    def get_content_size(self):
+        """Content size in bytes.
 
-    Args:
-        project_name (str): On which project operation will happen.
-        entity_type (str): Type of entity on which change happens.
-            e.g. 'folder', 'representation' etc.
-        data (Dict[str, Any]): Data of entity that will be created.
-
-    """
-    operation_name = "create"
-
-    def __init__(self, project_name, entity_type, data, session):
-        if not data:
-            data = {}
-        else:
-            data = copy.deepcopy(dict(data))
-
-        if "id" not in data:
-            data["id"] = create_entity_id()
-
-        self._data = data
-        super(CreateOperation, self).__init__(
-            project_name, entity_type, session
-        )
+        Returns:
+            Union[int, None]: Content size in bytes or None
+                if is unknown.
+
+        """
+        return self._content_size
 
-    def __setitem__(self, key, value):
-        self.set_value(key, value)
+    def set_content_size(self, content_size):
+        """Set content size in bytes.
 
-    def __getitem__(self, key):
-        return self.data[key]
+        Args:
+            content_size (int): Content size in bytes.
 
-    def set_value(self, key, value):
-        self.data[key] = value
+        Raises:
+            ValueError: If content size was already set.
 
-    def get(self, key, *args, **kwargs):
-        return self.data.get(key, *args, **kwargs)
+        """
+        if self._content_size is not None:
+            raise ValueError("Content size was set more then once")
+        self._content_size = content_size
 
-    @property
-    def con(self):
-        return self.session.con
+    def get_started(self):
+        """Transfer was started.
 
-    @property
-    def session(self):
-        return self._session
+        Returns:
+            bool: True if transfer started.
 
-    @property
-    def entity_id(self):
-        return self._data["id"]
+        """
+        return self._started
 
-    @property
-    def data(self):
-        return self._data
+    def set_started(self):
+        """Mark that transfer started.
 
-    def to_data(self):
-        output = super(CreateOperation, self).to_data()
-        output["data"] = copy.deepcopy(self.data)
-        return output
-
-    def to_server_operation(self):
-        return {
-            "id": self.id,
-            "type": "create",
-            "entityType": self.entity_type,
-            "entityId": self.entity_id,
-            "data": self._data
-        }
+        Raises:
+            ValueError: If transfer was already started.
 
+        """
+        if self._started:
+            raise ValueError("Progress already started")
+        self._started = True
 
-class UpdateOperation(AbstractOperation):
-    """Operation to update an entity.
+    def get_transfer_done(self):
+        """Transfer finished.
 
-    Args:
-        project_name (str): On which project operation will happen.
-        entity_type (str): Type of entity on which change happens.
-            e.g. 'folder', 'representation' etc.
-        entity_id (str): Identifier of an entity.
-        update_data (Dict[str, Any]): Key -> value changes that will be set in
-            database. If value is set to 'REMOVED_VALUE' the key will be
-            removed. Only first level of dictionary is checked (on purpose).
+        Returns:
+            bool: Transfer finished.
 
-    """
-    operation_name = "update"
+        """
+        return self._transfer_done
 
-    def __init__(
-        self, project_name, entity_type, entity_id, update_data, session
-    ):
-        super(UpdateOperation, self).__init__(
-            project_name, entity_type, session
-        )
+    def set_transfer_done(self):
+        """Mark progress as transfer finished.
 
-        self._entity_id = entity_id
-        self._update_data = update_data
+        Raises:
+            ValueError: If progress was already marked as done
+                or wasn't started yet.
 
-    @property
-    def entity_id(self):
-        return self._entity_id
+        """
+        if self._transfer_done:
+            raise ValueError("Progress was already marked as done")
+        if not self._started:
+            raise ValueError("Progress didn't start yet")
+        self._transfer_done = True
 
-    @property
-    def update_data(self):
-        return self._update_data
+    def get_failed(self):
+        """Transfer failed.
 
-    @property
-    def con(self):
-        return self.session.con
+        Returns:
+            bool: True if transfer failed.
 
-    @property
-    def session(self):
-        return self._session
+        """
+        return self._failed
 
-    def to_data(self):
-        changes = {}
-        for key, value in self._update_data.items():
-            if value is REMOVED_VALUE:
-                value = None
-            changes[key] = value
-
-        output = super(UpdateOperation, self).to_data()
-        output.update({
-            "entity_id": self.entity_id,
-            "changes": changes
-        })
-        return output
+    def get_fail_reason(self):
+        """Get reason why transfer failed.
 
-    def to_server_operation(self):
-        if not self._update_data:
-            return None
+        Returns:
+            Union[str, None]: Reason why transfer
+                failed or None.
 
-        update_data = {}
-        for key, value in self._update_data.items():
-            if value is REMOVED_VALUE:
-                value = None
-            update_data[key] = value
-
-        return {
-            "id": self.id,
-            "type": "update",
-            "entityType": self.entity_type,
-            "entityId": self.entity_id,
-            "data": update_data
-        }
+        """
+        return self._fail_reason
 
+    def set_failed(self, reason):
+        """Mark progress as failed.
 
-class DeleteOperation(AbstractOperation):
-    """Opeartion to delete an entity.
+        Args:
+            reason (str): Reason why transfer failed.
 
-    Args:
-        project_name (str): On which project operation will happen.
-        entity_type (str): Type of entity on which change happens.
-            e.g. 'folder', 'representation' etc.
-        entity_id (str): Entity id that will be removed.
+        """
+        self._fail_reason = reason
+        self._failed = True
 
-    """
-    operation_name = "delete"
+    def get_transferred_size(self):
+        """Already transferred size in bytes.
 
-    def __init__(self, project_name, entity_type, entity_id, session):
-        self._entity_id = entity_id
+        Returns:
+            int: Already transferred size in bytes.
 
-        super(DeleteOperation, self).__init__(
-            project_name, entity_type, session
-        )
+        """
+        return self._transferred
 
-    @property
-    def entity_id(self):
-        return self._entity_id
+    def set_transferred_size(self, transferred):
+        """Set already transferred size in bytes.
 
-    @property
-    def con(self):
-        return self.session.con
+        Args:
+            transferred (int): Already transferred size in bytes.
 
-    @property
-    def session(self):
-        return self._session
+        """
+        self._transferred = transferred
 
-    def to_data(self):
-        output = super(DeleteOperation, self).to_data()
-        output["entity_id"] = self.entity_id
-        return output
-
-    def to_server_operation(self):
-        return {
-            "id": self.id,
-            "type": self.operation_name,
-            "entityId": self.entity_id,
-            "entityType": self.entity_type,
-        }
-
-
-class OperationsSession(object):
-    """Session storing operations that should happen in an order.
-
-    At this moment does not handle anything special can be sonsidered as
-    stupid list of operations that will happen after each other. If creation
-    of same entity is there multiple times it's handled in any way and entity
-    values are not validated.
+    def add_transferred_chunk(self, chunk_size):
+        """Add transferred chunk size in bytes.
 
-    All operations must be related to single project.
+        Args:
+            chunk_size (int): Add transferred chunk size
+                in bytes.
 
-    Args:
-        project_name (str): Project name to which are operations related.
+        """
+        self._transferred += chunk_size
 
-    """
-    def __init__(self, con=None):
-        if con is None:
-            con = get_server_api_connection()
-        self._con = con
-        self._project_cache = {}
-        self._operations = []
-        self._nested_operations = collections.defaultdict(list)
+    def get_source_url(self):
+        """Source url from where transfer happens.
 
-    @property
-    def con(self):
-        return self._con
+        Note:
+            Consider this as title. Must be set using
+                'set_source_url' or 'N/A' will be returned.
 
-    def get_project(self, project_name):
-        if project_name not in self._project_cache:
-            self._project_cache[project_name] = self.con.get_project(
-                project_name)
-        return copy.deepcopy(self._project_cache[project_name])
+        Returns:
+            str: Source url from where transfer happens.
 
-    def __len__(self):
-        return len(self._operations)
+        """
+        return self._source_url
 
-    def add(self, operation):
-        """Add operation to be processed.
+    def set_source_url(self, url):
+        """Set source url from where transfer happens.
 
         Args:
-            operation (BaseOperation): Operation that should be processed.
+            url (str): Source url from where transfer happens.
 
         """
-        if not isinstance(
-            operation,
-            (CreateOperation, UpdateOperation, DeleteOperation)
-        ):
-            raise TypeError("Expected Operation object got {}".format(
-                str(type(operation))
-            ))
+        self._source_url = url
 
-        self._operations.append(operation)
+    def get_destination_url(self):
+        """Destination url where transfer happens.
 
-    def append(self, operation):
-        """Add operation to be processed.
+        Note:
+            Consider this as title. Must be set using
+                'set_source_url' or 'N/A' will be returned.
 
-        Args:
-            operation (BaseOperation): Operation that should be processed.
+        Returns:
+            str: Destination url where transfer happens.
 
         """
-        self.add(operation)
+        return self._destination_url
 
-    def extend(self, operations):
-        """Add operations to be processed.
+    def set_destination_url(self, url):
+        """Set destination url where transfer happens.
 
         Args:
-            operations (List[BaseOperation]): Operations that should be
-                processed.
+            url (str): Destination url where transfer happens.
 
         """
-        for operation in operations:
-            self.add(operation)
+        self._destination_url = url
 
-    def remove(self, operation):
-        """Remove operation."""
-        self._operations.remove(operation)
-
-    def clear(self):
-        """Clear all registered operations."""
-        self._operations = []
-
-    def to_data(self):
-        return [
-            operation.to_data()
-            for operation in self._operations
-        ]
-
-    def commit(self):
-        """Commit session operations."""
-        operations, self._operations = self._operations, []
-        if not operations:
-            return
-
-        operations_by_project = collections.defaultdict(list)
-        for operation in operations:
-            operations_by_project[operation.project_name].append(operation)
-
-        for project_name, operations in operations_by_project.items():
-            operations_body = []
-            for operation in operations:
-                body = operation.to_server_operation()
-                if body is not None:
-                    operations_body.append(body)
-
-            self._con.send_batch_operations(
-                project_name, operations_body, can_fail=False
-            )
+    @property
+    def is_running(self):
+        """Check if transfer is running.
 
-    def create_entity(self, project_name, entity_type, data, nested_id=None):
-        """Fast access to 'CreateOperation'.
+        Returns:
+            bool: True if transfer is running.
 
-        Args:
-            project_name (str): On which project the creation happens.
-            entity_type (str): Which entity type will be created.
-            data (Dicst[str, Any]): Entity data.
-            nested_id (str): Id of other operation from which is triggered
-                operation -> Operations can trigger suboperations but they
-                must be added to operations list after it's parent is added.
+        """
+        if (
+            not self.started
+            or self.transfer_done
+            or self.failed
+        ):
+            return False
+        return True
+
+    @property
+    def transfer_progress(self):
+        """Get transfer progress in percents.
 
         Returns:
-            CreateOperation: Object of update operation.
+            Union[float, None]: Transfer progress in percents or 'None'
+                if content size is unknown.
 
         """
-        operation = CreateOperation(
-            project_name, entity_type, data, self
-        )
-
-        if nested_id:
-            self._nested_operations[nested_id].append(operation)
-        else:
-            self.add(operation)
-            if operation.id in self._nested_operations:
-                self.extend(self._nested_operations.pop(operation.id))
+        if self._content_size is None:
+            return None
+        return (self._transferred * 100.0) / float(self._content_size)
 
-        return operation
+    content_size = property(get_content_size, set_content_size)
+    started = property(get_started)
+    transfer_done = property(get_transfer_done)
+    failed = property(get_failed)
+    fail_reason = property(get_fail_reason)
+    source_url = property(get_source_url, set_source_url)
+    destination_url = property(get_destination_url, set_destination_url)
+    transferred_size = property(get_transferred_size, set_transferred_size)
 
-    def update_entity(
-        self, project_name, entity_type, entity_id, update_data, nested_id=None
-    ):
-        """Fast access to 'UpdateOperation'.
 
-        Returns:
-            UpdateOperation: Object of update operation.
+def create_dependency_package_basename(platform_name=None):
+    """Create basename for dependency package file.
 
-        """
-        operation = UpdateOperation(
-            project_name, entity_type, entity_id, update_data, self
-        )
-        if nested_id:
-            self._nested_operations[nested_id].append(operation)
-        else:
-            self.add(operation)
-            if operation.id in self._nested_operations:
-                self.extend(self._nested_operations.pop(operation.id))
-        return operation
+    Args:
+        platform_name (Optional[str]): Name of platform for which the
+            bundle is targeted. Default value is current platform.
 
-    def delete_entity(
-        self, project_name, entity_type, entity_id, nested_id=None
-    ):
-        """Fast access to 'DeleteOperation'.
+    Returns:
+        str: Dependency package name with timestamp and platform.
 
-        Returns:
-            DeleteOperation: Object of delete operation.
+    """
+    if platform_name is None:
+        platform_name = platform.system().lower()
 
-        """
-        operation = DeleteOperation(
-            project_name, entity_type, entity_id, self
-        )
-        if nested_id:
-            self._nested_operations[nested_id].append(operation)
-        else:
-            self.add(operation)
-            if operation.id in self._nested_operations:
-                self.extend(self._nested_operations.pop(operation.id))
-        return operation
+    now_date = datetime.datetime.now()
+    time_stamp = now_date.strftime("%y%m%d%H%M")
+    return "ayon_{}_{}".format(time_stamp, platform_name)
```

### Comparing `ayon-python-api-1.0.1/ayon_api/server_api.py` & `ayon-python-api-1.0.2/ayon_api/server_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     try:
         from simplejson import JSONDecodeError as RequestsJSONDecodeError
     except ImportError:
         from json import JSONDecodeError as RequestsJSONDecodeError
 
 from .constants import (
     SERVER_RETRIES_ENV_KEY,
+    DEFAULT_FOLDER_TYPE_FIELDS,
+    DEFAULT_TASK_TYPE_FIELDS,
     DEFAULT_PRODUCT_TYPE_FIELDS,
     DEFAULT_PROJECT_FIELDS,
     DEFAULT_FOLDER_FIELDS,
     DEFAULT_TASK_FIELDS,
     DEFAULT_PRODUCT_FIELDS,
     DEFAULT_VERSION_FIELDS,
     DEFAULT_REPRESENTATION_FIELDS,
@@ -54,14 +56,15 @@
 from .graphql_queries import (
     project_graphql_query,
     projects_graphql_query,
     project_product_types_query,
     product_types_query,
     folders_graphql_query,
     tasks_graphql_query,
+    tasks_by_folder_paths_graphql_query,
     products_graphql_query,
     versions_graphql_query,
     representations_graphql_query,
     representations_parents_qraphql_query,
     workfiles_info_graphql_query,
     events_graphql_query,
     users_graphql_query,
@@ -69,31 +72,31 @@
 from .exceptions import (
     FailedOperations,
     UnauthorizedError,
     AuthenticationError,
     ServerNotReached,
     ServerError,
     HTTPRequestError,
+    UnsupportedServerVersion,
 )
 from .utils import (
     RepresentationParents,
     prepare_query_string,
     logout_from_server,
     create_entity_id,
     entity_data_json_default,
     failed_json_default,
     TransferProgress,
-    create_dependency_package_basename,
     ThumbnailContent,
     get_default_timeout,
     get_default_settings_variant,
     get_default_site_id,
+    NOT_SET,
 )
 
-_PLACEHOLDER = object()
 PatternType = type(re.compile(""))
 JSONDecodeError = getattr(json, "JSONDecodeError", ValueError)
 # This should be collected from server schema
 PROJECT_NAME_ALLOWED_SYMBOLS = "a-zA-Z0-9_"
 PROJECT_NAME_REGEX = re.compile(
     "^[{}]+$".format(PROJECT_NAME_ALLOWED_SYMBOLS)
 )
@@ -383,15 +386,15 @@
     default_download_chunk_size = 1024 * 1024
     default_upload_chunk_size = 1024 * 1024
 
     def __init__(
         self,
         base_url,
         token=None,
-        site_id=_PLACEHOLDER,
+        site_id=NOT_SET,
         client_version=None,
         default_settings_variant=None,
         sender=None,
         ssl_verify=None,
         cert=None,
         create_session=True,
         timeout=None,
@@ -403,15 +406,15 @@
         base_url = base_url.rstrip("/")
         self._base_url = base_url
         self._rest_url = "{}/api".format(base_url)
         self._graphql_url = "{}/graphql".format(base_url)
         self._log = None
         self._access_token = token
         # Allow to have 'site_id' to 'None'
-        if site_id is _PLACEHOLDER:
+        if site_id is NOT_SET:
             site_id = get_default_site_id()
         self._site_id = site_id
         self._client_version = client_version
         self._default_settings_variant = (
             default_settings_variant
             or get_default_settings_variant()
         )
@@ -1306,15 +1309,15 @@
     def get_event(self, event_id):
         """Query full event data by id.
 
         Events received using event server do not contain full information. To
         get the full event information is required to receive it explicitly.
 
         Args:
-            event_id (str): Id of event.
+            event_id (str): Event id.
 
         Returns:
             dict[str, Any]: Full event data.
 
         """
         response = self.get("events/{}".format(event_id))
         response.raise_for_status()
@@ -1470,15 +1473,15 @@
         store=True,
     ):
         """Dispatch event to server.
 
         Args:
             topic (str): Event topic used for filtering of listeners.
             sender (Optional[str]): Sender of event.
-            hash (Optional[str]): Event hash.
+            event_hash (Optional[str]): Event hash.
             project_name (Optional[str]): Project name.
             username (Optional[str]): Username which triggered event.
             dependencies (Optional[list[str]]): List of event id dependencies.
             description (Optional[str]): Description of event.
             summary (Optional[dict[str, Any]]): Summary of event that can be used
                 for simple filtering on listeners.
             payload (Optional[dict[str, Any]]): Full payload of event data with
@@ -2042,14 +2045,20 @@
             entity_type_defaults = (
                 DEFAULT_REPRESENTATION_FIELDS
                 | REPRESENTATION_FILES_FIELDS
             )
             if not self.graphql_allows_data_in_query:
                 entity_type_defaults.discard("data")
 
+        elif entity_type == "folderType":
+            entity_type_defaults = set(DEFAULT_FOLDER_TYPE_FIELDS)
+
+        elif entity_type == "taskType":
+            entity_type_defaults = set(DEFAULT_TASK_TYPE_FIELDS)
+
         elif entity_type == "productType":
             entity_type_defaults = set(DEFAULT_PRODUCT_TYPE_FIELDS)
 
         elif entity_type == "workfile":
             entity_type_defaults = set(DEFAULT_WORKFILE_INFO_FIELDS)
             if not self.graphql_allows_data_in_query:
                 entity_type_defaults.discard("data")
@@ -2698,33 +2707,66 @@
             list[dict[str, str]]: Anatomy presets available on server.
 
         """
         result = self.get("anatomy/presets")
         result.raise_for_status()
         return result.data.get("presets") or []
 
+    def get_default_anatomy_preset_name(self):
+        """Name of default anatomy preset.
+
+        Primary preset is used as default preset. But when primary preset is
+        not set a built-in is used instead. Built-in preset is named '_'.
+
+        Returns:
+            str: Name of preset that can be used by
+                'get_project_anatomy_preset'.
+
+        """
+        for preset in self.get_project_anatomy_presets():
+            if preset.get("primary"):
+                return preset["name"]
+        return "_"
+
     def get_project_anatomy_preset(self, preset_name=None):
         """Anatomy preset values by name.
 
         Get anatomy preset values by preset name. Primary preset is returned
         if preset name is set to 'None'.
 
         Args:
             preset_name (Optional[str]): Preset name.
 
         Returns:
             dict[str, Any]: Anatomy preset values.
 
         """
         if preset_name is None:
-            preset_name = "_"
+            preset_name = "__primary__"
+            major, minor, patch, _, _ = self.server_version_tuple
+            if (major, minor, patch) < (1, 0, 8):
+                preset_name = self.get_default_anatomy_preset_name()
+
         result = self.get("anatomy/presets/{}".format(preset_name))
         result.raise_for_status()
         return result.data
 
+    def get_build_in_anatomy_preset(self):
+        """Get built-in anatomy preset.
+
+        Returns:
+            dict[str, Any]: Built-in anatomy preset.
+
+        """
+        preset_name = "__builtin__"
+        major, minor, patch, _, _ = self.server_version_tuple
+        if (major, minor, patch) < (1, 0, 8):
+            preset_name = "_"
+        return self.get_project_anatomy_preset(preset_name)
+
     def get_project_roots_by_site(self, project_name):
         """Root overrides per site name.
 
         Method is based on logged user and can't be received for any other
         user on server.
 
         Output will contain only roots per site id used by logged user.
@@ -2744,15 +2786,15 @@
         """Root overrides for site.
 
         If site id is not passed a site set in current api object is used
         instead.
 
         Args:
             project_name (str): Name of project.
-            site_id (Optional[str]): Id of site for which want to receive
+            site_id (Optional[str]): Site id for which want to receive
                 site overrides.
 
         Returns:
             dict[str, str]: Root values by root name or None if
                 site does not have overrides.
 
         """
@@ -3049,15 +3091,15 @@
                 'only_values=True' then output should be same as before.
 
         Args:
             bundle_name (Optional[str]): Name of bundle for which should be
                 settings received.
             variant (Optional[Literal['production', 'staging']]): Name of
                 settings variant. Used 'default_settings_variant' by default.
-            site_id (Optional[str]): Id of site for which want to receive
+            site_id (Optional[str]): Site id for which want to receive
                 site overrides.
             use_site (bool): To force disable option of using site overrides
                 set to 'False'. In that case won't be applied any site
                 overrides.
             only_values (Optional[bool]): Output will contain only settings
                 values without metadata about addons.
 
@@ -3111,15 +3153,15 @@
         Args:
             project_name (str): Name of project for which are settings
                 received.
             bundle_name (Optional[str]): Name of bundle for which should be
                 settings received.
             variant (Optional[Literal['production', 'staging']]): Name of
                 settings variant. Used 'default_settings_variant' by default.
-            site_id (Optional[str]): Id of site for which want to receive
+            site_id (Optional[str]): Site id for which want to receive
                 site overrides.
             use_site (bool): To force disable option of using site overrides
                 set to 'False'. In that case won't be applied any site
                 overrides.
             only_values (Optional[bool]): Output will contain only settings
                 values without metadata about addons.
 
@@ -3257,15 +3299,14 @@
             "secrets/{}".format(secret_name),
             name=secret_name,
             value=secret_value,
         )
         response.raise_for_status()
         return response.data
 
-
     def delete_secret(self, secret_name):
         """Delete secret by name.
 
         Args:
             secret_name (str): Name of secret to delete.
 
         """
@@ -3389,14 +3430,57 @@
         data = response.data
         project_names = []
         if data:
             for project in data["projects"]:
                 project_names.append(project["name"])
         return project_names
 
+    def _should_use_rest_project(self, fields=None):
+        """Fetch of project must be done using REST endpoint.
+
+        Returns:
+            bool: REST endpoint must be used to get requested fields.
+
+        """
+        if fields is None:
+            return True
+        for field in fields:
+            if field.startswith("config"):
+                return True
+        return False
+
+    def _prepare_project_fields(self, fields, own_attributes):
+        if "attrib" in fields:
+            fields.remove("attrib")
+            fields |= self.get_attributes_fields_for_type("project")
+
+        if "folderTypes" in fields:
+            fields.remove("folderTypes")
+            fields |= {
+                "folderTypes.{}".format(name)
+                for name in self.get_default_fields_for_type("folderType")
+            }
+
+        if "taskTypes" in fields:
+            fields.remove("taskTypes")
+            fields |= {
+                "taskTypes.{}".format(name)
+                for name in self.get_default_fields_for_type("taskType")
+            }
+
+        if "productTypes" in fields:
+            fields.remove("productTypes")
+            fields |= {
+                "productTypes.{}".format(name)
+                for name in self.get_default_fields_for_type("productType")
+            }
+
+        if own_attributes:
+            fields.add("ownAttrib")
+
     def get_projects(
         self, active=True, library=None, fields=None, own_attributes=False
     ):
         """Get projects.
 
         Args:
             active (Optional[bool]): Filter active or inactive projects.
@@ -3408,44 +3492,33 @@
             own_attributes (Optional[bool]): Attribute values that are
                 not explicitly set on entity will have 'None' value.
 
         Returns:
             Generator[dict[str, Any]]: Queried projects.
 
         """
-        if fields is None:
-            use_rest = True
-        else:
-            use_rest = False
+        if fields is not None:
             fields = set(fields)
-            for field in fields:
-                if field.startswith("config"):
-                    use_rest = True
-                    break
 
+        use_rest = self._should_use_rest_project(fields)
         if use_rest:
             for project in self.get_rest_projects(active, library):
                 if own_attributes:
                     fill_own_attribs(project)
                 yield project
+            return
 
-        else:
-            if "attrib" in fields:
-                fields.remove("attrib")
-                fields |= self.get_attributes_fields_for_type("project")
-
-            if own_attributes:
-                fields.add("ownAttrib")
+        self._prepare_project_fields(fields, own_attributes)
 
-            query = projects_graphql_query(fields)
-            for parsed_data in query.continuous_query(self):
-                for project in parsed_data["projects"]:
-                    if own_attributes:
-                        fill_own_attribs(project)
-                    yield project
+        query = projects_graphql_query(fields)
+        for parsed_data in query.continuous_query(self):
+            for project in parsed_data["projects"]:
+                if own_attributes:
+                    fill_own_attribs(project)
+                yield project
 
     def get_project(self, project_name, fields=None, own_attributes=False):
         """Get project.
 
         Args:
             project_name (str): Name of project.
             fields (Optional[Iterable[str]]): fields to be queried
@@ -3454,48 +3527,34 @@
                 not explicitly set on entity will have 'None' value.
 
         Returns:
             Union[dict[str, Any], None]: Project entity data or None
                 if project was not found.
 
         """
-        use_rest = True
         if fields is not None:
-            use_rest = False
-            _fields = set()
-            for field in fields:
-                if field.startswith("config") or field == "data":
-                    use_rest = True
-                    break
-                _fields.add(field)
-
-            fields = _fields
+            fields = set(fields)
 
+        use_rest = self._should_use_rest_project(fields)
         if use_rest:
-            project = self.get_rest_project(project_name)
-            if own_attributes:
-                fill_own_attribs(project)
-            return project
+            return self.get_rest_project(project_name)
 
-        if "attrib" in fields:
-            fields.remove("attrib")
-            fields |= self.get_attributes_fields_for_type("project")
+        self._prepare_project_fields(fields, own_attributes)
 
-        if own_attributes:
-            fields.add("ownAttrib")
         query = project_graphql_query(fields)
         query.set_variable_value("projectName", project_name)
 
         parsed_data = query.query(self)
 
         project = parsed_data["project"]
         if project is not None:
             project["name"] = project_name
             if own_attributes:
                 fill_own_attribs(project)
+
         return project
 
     def get_folders_hierarchy(
         self,
         project_name,
         search_string=None,
         folder_types=None
@@ -3549,14 +3608,70 @@
 
         response = self.get(
             "projects/{}/hierarchy{}".format(project_name, query)
         )
         response.raise_for_status()
         return response.data
 
+    def get_folders_rest(self, project_name, include_attrib=False):
+        """Get simplified flat list of all project folders.
+
+        Get all project folders in single REST call. This can be faster than
+            using 'get_folders' method which is using GraphQl, but does not
+            allow any filtering, and set of fields is defined
+            by server backend.
+
+        Example::
+
+            [
+                {
+                    "id": "112233445566",
+                    "parentId": "112233445567",
+                    "path": "/root/parent/child",
+                    "parents": ["root", "parent"],
+                    "name": "child",
+                    "label": "Child",
+                    "folderType": "Folder",
+                    "hasTasks": False,
+                    "hasChildren": False,
+                    "taskNames": [
+                        "Compositing",
+                    ],
+                    "status": "In Progress",
+                    "attrib": {},
+                    "ownAttrib": [],
+                    "updatedAt": "2023-06-12T15:37:02.420260",
+                },
+                ...
+            ]
+
+        Args:
+            project_name (str): Project name.
+            include_attrib (Optional[bool]): Include attribute values
+                in output. Slower to query.
+
+        Returns:
+            list[dict[str, Any]]: List of folder entities.
+
+        """
+        major, minor, patch, _, _ = self.server_version_tuple
+        if (major, minor, patch) < (1, 0, 8):
+            raise UnsupportedServerVersion(
+                "Function 'get_folders_rest' is supported"
+                " for AYON server 1.0.8 and above."
+            )
+        query = "?attrib={}".format(
+            "true" if include_attrib else "false"
+        )
+        response = self.get(
+            "projects/{}/folders{}".format(project_name, query)
+        )
+        response.raise_for_status()
+        return response.data["folders"]
+
     def get_folders(
         self,
         project_name,
         folder_ids=None,
         folder_paths=None,
         folder_names=None,
         folder_types=None,
@@ -3868,14 +3983,162 @@
         parsed_data = query.query(self)
         folders = parsed_data["project"]["folders"]
         return {
             folder["id"]
             for folder in folders
         }
 
+    def create_folder(
+        self,
+        project_name,
+        name,
+        folder_type=None,
+        parent_id=None,
+        label=None,
+        attrib=None,
+        data=None,
+        tags=None,
+        status=None,
+        active=None,
+        thumbnail_id=None,
+        folder_id=None,
+    ):
+        """Create new folder.
+
+        Args:
+            project_name (str): Project name.
+            name (str): Folder name.
+            folder_type (Optional[str]): Folder type.
+            parent_id (Optional[str]): Parent folder id. Parent is project
+                if is ``None``.
+            label (Optional[str]): Label of folder.
+            attrib (Optional[dict[str, Any]]): Folder attributes.
+            data (Optional[dict[str, Any]]): Folder data.
+            tags (Optional[Iterable[str]]): Folder tags.
+            status (Optional[str]): Folder status.
+            active (Optional[bool]): Folder active state.
+            thumbnail_id (Optional[str]): Folder thumbnail id.
+            folder_id (Optional[str]): Folder id. If not passed new id is
+                generated.
+
+        Returns:
+            str: Entity id.
+
+        """
+        if not folder_id:
+            folder_id = create_entity_id()
+        create_data = {
+            "id": folder_id,
+            "name": name,
+        }
+        for key, value in (
+            ("folderType", folder_type),
+            ("parentId", parent_id),
+            ("label", label),
+            ("attrib", attrib),
+            ("data", data),
+            ("tags", tags),
+            ("status", status),
+            ("active", active),
+            ("thumbnailId", thumbnail_id),
+        ):
+            if value is not None:
+                create_data[key] = value
+
+        response = self.post(
+            "projects/{}/folders".format(project_name),
+            **create_data
+        )
+        response.raise_for_status()
+        return folder_id
+
+    def update_folder(
+        self,
+        project_name,
+        folder_id,
+        name=None,
+        folder_type=None,
+        parent_id=NOT_SET,
+        label=NOT_SET,
+        attrib=None,
+        data=None,
+        tags=None,
+        status=None,
+        active=None,
+        thumbnail_id=NOT_SET,
+    ):
+        """Update folder entity on server.
+
+        Do not pass ``parent_id``, ``label`` amd ``thumbnail_id`` if you don't
+            want to change their values. Value ``None`` would unset
+            their value.
+
+        Update of ``data`` will override existing value on folder entity.
+
+        Update of ``attrib`` does change only passed attributes. If you want
+            to unset value, use ``None``.
+
+        Args:
+            project_name (str): Project name.
+            folder_id (str): Folder id.
+            name (Optional[str]): New name.
+            folder_type (Optional[str]): New folder type.
+            parent_id (Optional[Union[str, None]]): New parent folder id.
+            label (Optional[Union[str, None]]): New label.
+            attrib (Optional[dict[str, Any]]): New attributes.
+            data (Optional[dict[str, Any]]): New data.
+            tags (Optional[Iterable[str]]): New tags.
+            status (Optional[str]): New status.
+            active (Optional[bool]): New active state.
+            thumbnail_id (Optional[Union[str, None]]): New thumbnail id.
+
+        """
+        update_data = {}
+        for key, value in (
+            ("name", name),
+            ("folderType", folder_type),
+            ("attrib", attrib),
+            ("data", data),
+            ("tags", tags),
+            ("status", status),
+            ("active", active),
+        ):
+            if value is not None:
+                update_data[key] = value
+
+        for key, value in (
+            ("label", label),
+            ("parentId", parent_id),
+            ("thumbnailId", thumbnail_id),
+        ):
+            if value is not NOT_SET:
+                update_data[key] = value
+
+        response = self.patch(
+            "projects/{}/folders/{}".format(project_name, folder_id),
+            **update_data
+        )
+        response.raise_for_status()
+
+    def delete_folder(self, project_name, folder_id, force=False):
+        """Delete folder.
+
+        Args:
+            project_name (str): Project name.
+            folder_id (str): Folder id to delete.
+            force (Optional[bool]): Folder delete folder with all children
+                folder, products, versions and representations.
+
+        """
+        url = "projects/{}/folders/{}".format(project_name, folder_id)
+        if force:
+            url += "?force=true"
+        response = self.delete(url)
+        response.raise_for_status()
+
     def get_tasks(
         self,
         project_name,
         task_ids=None,
         task_names=None,
         task_types=None,
         folder_ids=None,
@@ -4021,15 +4284,15 @@
         """Query task entity by name and folder id.
 
         Args:
             project_name (str): Name of project where to look for queried
                 entities.
             folder_id (str): Folder id.
             task_name (str): Task name
-            fields (Optional[Iterable[str]): Fields that should be returned.
+            fields (Optional[Iterable[str]]): Fields that should be returned.
                 All fields are returned if 'None' is passed.
             own_attributes (Optional[bool]): Attribute values that are
                 not explicitly set on entity will have 'None' value.
 
         Returns:
             Union[dict, None]: Task entity data or None if was not found.
 
@@ -4054,15 +4317,15 @@
     ):
         """Query task entity by id.
 
         Args:
             project_name (str): Name of project where to look for queried
                 entities.
             task_id (str): Task id.
-            fields (Optional[Iterable[str]): Fields that should be returned.
+            fields (Optional[Iterable[str]]): Fields that should be returned.
                 All fields are returned if 'None' is passed.
             own_attributes (Optional[bool]): Attribute values that are
                 not explicitly set on entity will have 'None' value.
 
         Returns:
             Union[dict, None]: Task entity data or None if was not found.
 
@@ -4073,14 +4336,386 @@
             active=None,
             fields=fields,
             own_attributes=own_attributes
         ):
             return task
         return None
 
+    def get_tasks_by_folder_paths(
+        self,
+        project_name,
+        folder_paths,
+        task_names=None,
+        task_types=None,
+        assignees=None,
+        assignees_all=None,
+        statuses=None,
+        tags=None,
+        active=True,
+        fields=None,
+        own_attributes=False
+    ):
+        """Query task entities from server by folder paths.
+
+        Args:
+            project_name (str): Name of project.
+            folder_paths (list[str]): Folder paths.
+            task_names (Iterable[str]): Task names used for filtering.
+            task_types (Iterable[str]): Task types used for filtering.
+            assignees (Optional[Iterable[str]]): Task assignees used for
+                filtering. All tasks with any of passed assignees are
+                returned.
+            assignees_all (Optional[Iterable[str]]): Task assignees used
+                for filtering. Task must have all of passed assignees to be
+                returned.
+            statuses (Optional[Iterable[str]]): Task statuses used for
+                filtering.
+            tags (Optional[Iterable[str]]): Task tags used for
+                filtering.
+            active (Optional[bool]): Filter active/inactive tasks.
+                Both are returned if is set to None.
+            fields (Optional[Iterable[str]]): Fields to be queried for
+                folder. All possible folder fields are returned
+                if 'None' is passed.
+            own_attributes (Optional[bool]): Attribute values that are
+                not explicitly set on entity will have 'None' value.
+
+        Returns:
+            dict[dict[str, list[dict[str, Any]]]: Task entities by
+                folder path.
+
+        """
+        folder_paths = set(folder_paths)
+        if not project_name or not folder_paths:
+            return
+
+        filters = {
+            "projectName": project_name,
+            "folderPaths": list(folder_paths),
+        }
+
+        if task_names is not None:
+            task_names = set(task_names)
+            if not task_names:
+                return
+            filters["taskNames"] = list(task_names)
+
+        if task_types is not None:
+            task_types = set(task_types)
+            if not task_types:
+                return
+            filters["taskTypes"] = list(task_types)
+
+        if assignees is not None:
+            assignees = set(assignees)
+            if not assignees:
+                return
+            filters["taskAssigneesAny"] = list(assignees)
+
+        if assignees_all is not None:
+            assignees_all = set(assignees_all)
+            if not assignees_all:
+                return
+            filters["taskAssigneesAll"] = list(assignees_all)
+
+        if statuses is not None:
+            statuses = set(statuses)
+            if not statuses:
+                return
+            filters["taskStatuses"] = list(statuses)
+
+        if tags is not None:
+            tags = set(tags)
+            if not tags:
+                return
+            filters["taskTags"] = list(tags)
+
+        if not fields:
+            fields = self.get_default_fields_for_type("task")
+        else:
+            fields = set(fields)
+            if "attrib" in fields:
+                fields.remove("attrib")
+                fields |= self.get_attributes_fields_for_type("task")
+
+        use_rest = False
+        if "data" in fields and not self.graphql_allows_data_in_query:
+            use_rest = True
+            fields = {"id"}
+
+        if active is not None:
+            fields.add("active")
+
+        if own_attributes:
+            fields.add("ownAttrib")
+
+        query = tasks_by_folder_paths_graphql_query(fields)
+        for attr, filter_value in filters.items():
+            query.set_variable_value(attr, filter_value)
+
+        output = {
+            folder_path: []
+            for folder_path in folder_paths
+        }
+        for parsed_data in query.continuous_query(self):
+            for folder in parsed_data["project"]["folders"]:
+                folder_path = folder["path"]
+                for task in folder["tasks"]:
+                    if active is not None and active is not task["active"]:
+                        continue
+
+                    if use_rest:
+                        task = self.get_rest_task(project_name, task["id"])
+                    else:
+                        self._convert_entity_data(task)
+
+                    if own_attributes:
+                        fill_own_attribs(task)
+                    output[folder_path].append(task)
+        return output
+
+    def get_tasks_by_folder_path(
+        self,
+        project_name,
+        folder_path,
+        task_names=None,
+        task_types=None,
+        assignees=None,
+        assignees_all=None,
+        statuses=None,
+        tags=None,
+        active=True,
+        fields=None,
+        own_attributes=False
+    ):
+        """Query task entities from server by folder path.
+
+        Args:
+            project_name (str): Name of project.
+            folder_path (str): Folder path.
+            task_names (Iterable[str]): Task names used for filtering.
+            task_types (Iterable[str]): Task types used for filtering.
+            assignees (Optional[Iterable[str]]): Task assignees used for
+                filtering. All tasks with any of passed assignees are
+                returned.
+            assignees_all (Optional[Iterable[str]]): Task assignees used
+                for filtering. Task must have all of passed assignees to be
+                returned.
+            statuses (Optional[Iterable[str]]): Task statuses used for
+                filtering.
+            tags (Optional[Iterable[str]]): Task tags used for
+                filtering.
+            active (Optional[bool]): Filter active/inactive tasks.
+                Both are returned if is set to None.
+            fields (Optional[Iterable[str]]): Fields to be queried for
+                folder. All possible folder fields are returned
+                if 'None' is passed.
+            own_attributes (Optional[bool]): Attribute values that are
+                not explicitly set on entity will have 'None' value.
+
+        """
+        return self.get_tasks_by_folder_paths(
+            project_name,
+            [folder_path],
+            task_names,
+            task_types=task_types,
+            assignees=assignees,
+            assignees_all=assignees_all,
+            statuses=statuses,
+            tags=tags,
+            active=active,
+            fields=fields,
+            own_attributes=own_attributes
+        )[folder_path]
+
+    def get_task_by_folder_path(
+        self,
+        project_name,
+        folder_path,
+        task_name,
+        fields=None,
+        own_attributes=False
+    ):
+        """Query task entity by folder path and task name.
+
+        Args:
+            project_name (str): Project name.
+            folder_path (str): Folder path.
+            task_name (str): Task name.
+            fields (Optional[Iterable[str]]): Task fields that should
+                be returned.
+            own_attributes (Optional[bool]): Attribute values that are
+                not explicitly set on entity will have 'None' value.
+
+        Returns:
+            Union[dict[str, Any], None]: Task entity data or None if was
+                not found.
+
+        """
+        for task in self.get_tasks_by_folder_path(
+            project_name,
+            folder_path,
+            active=None,
+            task_names=[task_name],
+            fields=fields,
+            own_attributes=own_attributes,
+        ):
+            return task
+        return None
+
+    def create_task(
+        self,
+        project_name,
+        name,
+        task_type,
+        folder_id,
+        label=None,
+        assignees=None,
+        attrib=None,
+        data=None,
+        tags=None,
+        status=None,
+        active=None,
+        thumbnail_id=None,
+        task_id=None,
+    ):
+        """Create new task.
+
+        Args:
+            project_name (str): Project name.
+            name (str): Folder name.
+            task_type (str): Task type.
+            folder_id (str): Parent folder id.
+            label (Optional[str]): Label of folder.
+            assignees (Optional[Iterable[str]]): Task assignees.
+            attrib (Optional[dict[str, Any]]): Task attributes.
+            data (Optional[dict[str, Any]]): Task data.
+            tags (Optional[Iterable[str]]): Task tags.
+            status (Optional[str]): Task status.
+            active (Optional[bool]): Task active state.
+            thumbnail_id (Optional[str]): Task thumbnail id.
+            task_id (Optional[str]): Task id. If not passed new id is
+                generated.
+
+        Returns:
+            str: Task id.
+
+        """
+        if not task_id:
+            task_id = create_entity_id()
+        create_data = {
+            "id": task_id,
+            "name": name,
+            "taskType": task_type,
+            "folderId": folder_id,
+        }
+        for key, value in (
+            ("label", label),
+            ("attrib", attrib),
+            ("data", data),
+            ("tags", tags),
+            ("status", status),
+            ("assignees", assignees),
+            ("active", active),
+            ("thumbnailId", thumbnail_id),
+        ):
+            if value is not None:
+                create_data[key] = value
+
+        response = self.post(
+            "projects/{}/tasks".format(project_name),
+            **create_data
+        )
+        response.raise_for_status()
+        return folder_id
+
+    def update_task(
+        self,
+        project_name,
+        task_id,
+        name=None,
+        task_type=None,
+        folder_id=None,
+        label=NOT_SET,
+        assignees=None,
+        attrib=None,
+        data=None,
+        tags=None,
+        status=None,
+        active=None,
+        thumbnail_id=NOT_SET,
+    ):
+        """Update task entity on server.
+
+        Do not pass ``label`` amd ``thumbnail_id`` if you don't
+            want to change their values. Value ``None`` would unset
+            their value.
+
+        Update of ``data`` will override existing value on folder entity.
+
+        Update of ``attrib`` does change only passed attributes. If you want
+            to unset value, use ``None``.
+
+        Args:
+            project_name (str): Project name.
+            task_id (str): Task id.
+            name (Optional[str]): New name.
+            task_type (Optional[str]): New task type.
+            folder_id (Optional[str]): New folder id.
+            label (Optional[Union[str, None]]): New label.
+            assignees (Optional[str]): New assignees.
+            attrib (Optional[dict[str, Any]]): New attributes.
+            data (Optional[dict[str, Any]]): New data.
+            tags (Optional[Iterable[str]]): New tags.
+            status (Optional[str]): New status.
+            active (Optional[bool]): New active state.
+            thumbnail_id (Optional[Union[str, None]]): New thumbnail id.
+
+        """
+        update_data = {}
+        for key, value in (
+            ("name", name),
+            ("taskType", task_type),
+            ("folderId", folder_id),
+            ("assignees", assignees),
+            ("attrib", attrib),
+            ("data", data),
+            ("tags", tags),
+            ("status", status),
+            ("active", active),
+        ):
+            if value is not None:
+                update_data[key] = value
+
+        for key, value in (
+            ("label", label),
+            ("thumbnailId", thumbnail_id),
+        ):
+            if value is not NOT_SET:
+                update_data[key] = value
+
+        response = self.patch(
+            "projects/{}/tasks/{}".format(project_name, task_id),
+            **update_data
+        )
+        response.raise_for_status()
+
+    def delete_task(self, project_name, task_id):
+        """Delete task.
+
+        Args:
+            project_name (str): Project name.
+            task_id (str): Task id to delete.
+
+        """
+        response = self.delete(
+            "projects/{}/tasks/{}".format(project_name, task_id)
+        )
+        response.raise_for_status()
+
     def _filter_product(
         self, project_name, product, active, own_attributes, use_rest
     ):
         if active is not None and product["active"] is not active:
             return None
 
         if use_rest:
@@ -4419,14 +5054,137 @@
         return {
             product_info["name"]
             for product_info in self.get_project_product_types(
                 project_name, fields=["name"]
             )
         }
 
+    def create_product(
+        self,
+        project_name,
+        name,
+        product_type,
+        folder_id,
+        attrib=None,
+        data=None,
+        tags=None,
+        status=None,
+        active=None,
+        product_id=None,
+    ):
+        """Create new product.
+
+        Args:
+            project_name (str): Project name.
+            name (str): Product name.
+            product_type (str): Product type.
+            folder_id (str): Parent folder id.
+            attrib (Optional[dict[str, Any]]): Product attributes.
+            data (Optional[dict[str, Any]]): Product data.
+            tags (Optional[Iterable[str]]): Product tags.
+            status (Optional[str]): Product status.
+            active (Optional[bool]): Product active state.
+            product_id (Optional[str]): Product id. If not passed new id is
+                generated.
+
+        Returns:
+            str: Product id.
+
+        """
+        if not product_id:
+            product_id = create_entity_id()
+        create_data = {
+            "id": product_id,
+            "name": name,
+            "productType": product_type,
+            "folderId": folder_id,
+        }
+        for key, value in (
+            ("attrib", attrib),
+            ("data", data),
+            ("tags", tags),
+            ("status", status),
+            ("active", active),
+        ):
+            if value is not None:
+                create_data[key] = value
+
+        response = self.post(
+            "projects/{}/products".format(project_name),
+            **create_data
+        )
+        response.raise_for_status()
+        return product_id
+
+    def update_product(
+        self,
+        project_name,
+        product_id,
+        name=None,
+        folder_id=None,
+        product_type=None,
+        attrib=None,
+        data=None,
+        tags=None,
+        status=None,
+        active=None,
+    ):
+        """Update product entity on server.
+
+        Update of ``data`` will override existing value on folder entity.
+
+        Update of ``attrib`` does change only passed attributes. If you want
+            to unset value, use ``None``.
+
+        Args:
+            project_name (str): Project name.
+            product_id (str): Product id.
+            name (Optional[str]): New product name.
+            folder_id (Optional[str]): New product id.
+            product_type (Optional[str]): New product type.
+            attrib (Optional[dict[str, Any]]): New product attributes.
+            data (Optional[dict[str, Any]]): New product data.
+            tags (Optional[Iterable[str]]): New product tags.
+            status (Optional[str]): New product status.
+            active (Optional[bool]): New product active state.
+
+        """
+        update_data = {}
+        for key, value in (
+            ("name", name),
+            ("productType", product_type),
+            ("folderId", folder_id),
+            ("attrib", attrib),
+            ("data", data),
+            ("tags", tags),
+            ("status", status),
+            ("active", active),
+        ):
+            if value is not None:
+                update_data[key] = value
+
+        response = self.patch(
+            "projects/{}/products/{}".format(project_name, product_id),
+            **update_data
+        )
+        response.raise_for_status()
+
+    def delete_product(self, project_name, product_id):
+        """Delete product.
+
+        Args:
+            project_name (str): Project name.
+            product_id (str): Product id to delete.
+
+        """
+        response = self.delete(
+            "projects/{}/products/{}".format(project_name, product_id)
+        )
+        response.raise_for_status()
+
     def get_versions(
         self,
         project_name,
         version_ids=None,
         product_ids=None,
         versions=None,
         hero=True,
@@ -4785,14 +5543,15 @@
             fields = set(fields)
             fields.add("productId")
 
         versions = self.get_versions(
             project_name,
             product_ids=product_ids,
             latest=True,
+            hero=False,
             active=active,
             fields=fields,
             own_attributes=own_attributes
         )
         return {
             version["productId"]: version
             for version in versions
@@ -4822,14 +5581,15 @@
             Union[dict[str, Any], None]: Queried version entity or None.
 
         """
         versions = self.get_versions(
             project_name,
             product_ids=[product_id],
             latest=True,
+            hero=False,
             active=active,
             fields=fields,
             own_attributes=own_attributes
         )
         for version in versions:
             return version
         return None
@@ -4847,28 +5607,28 @@
 
         Args:
             project_name (str): Project where to look for representation.
             product_name (str): Product name.
             folder_id (str): Folder id.
             active (Optional[bool]): Receive active/inactive entities.
                 Both are returned when 'None' is passed.
-            fields (Optional[Iterable[str]): fields to be queried
+            fields (Optional[Iterable[str]]): fields to be queried
                 for representations.
             own_attributes (Optional[bool]): Attribute values that are
                 not explicitly set on entity will have 'None' value.
 
         Returns:
             Union[dict[str, Any], None]: Queried version entity or None.
 
         """
         if not folder_id:
             return None
 
         product = self.get_product_by_name(
-            project_name, product_name, folder_id, fields=["_id"]
+            project_name, product_name, folder_id, fields={"id"}
         )
         if not product:
             return None
         return self.get_last_version_by_product_id(
             project_name,
             product["id"],
             active=active,
@@ -4904,14 +5664,156 @@
 
         parsed_data = query.query(self)
         latest_version = (
             parsed_data["project"]["version"]["product"]["latestVersion"]
         )
         return latest_version["id"] == version_id
 
+    def create_version(
+        self,
+        project_name,
+        version,
+        product_id,
+        task_id=None,
+        author=None,
+        attrib=None,
+        data=None,
+        tags=None,
+        status=None,
+        active=None,
+        thumbnail_id=None,
+        version_id=None,
+    ):
+        """Create new version.
+
+        Args:
+            project_name (str): Project name.
+            version (int): Version.
+            product_id (str): Parent product id.
+            task_id (Optional[str]): Parent task id.
+            author (Optional[str]): Version author.
+            attrib (Optional[dict[str, Any]]): Version attributes.
+            data (Optional[dict[str, Any]]): Version data.
+            tags (Optional[Iterable[str]]): Version tags.
+            status (Optional[str]): Version status.
+            active (Optional[bool]): Version active state.
+            thumbnail_id (Optional[str]): Version thumbnail id.
+            version_id (Optional[str]): Version id. If not passed new id is
+                generated.
+
+        Returns:
+            str: Version id.
+
+        """
+        if not version_id:
+            version_id = create_entity_id()
+        create_data = {
+            "id": version_id,
+            "version": version,
+            "productId": product_id,
+        }
+        for key, value in (
+            ("taskId", task_id),
+            ("author", author),
+            ("attrib", attrib),
+            ("data", data),
+            ("tags", tags),
+            ("status", status),
+            ("active", active),
+            ("thumbnailId", thumbnail_id),
+        ):
+            if value is not None:
+                create_data[key] = value
+
+        response = self.post(
+            "projects/{}/versions".format(project_name),
+            **create_data
+        )
+        response.raise_for_status()
+        return version_id
+
+    def update_version(
+        self,
+        project_name,
+        version_id,
+        version=None,
+        product_id=None,
+        task_id=NOT_SET,
+        attrib=None,
+        data=None,
+        tags=None,
+        status=None,
+        active=None,
+        thumbnail_id=NOT_SET,
+    ):
+        """Update version entity on server.
+
+        Do not pass ``task_id`` amd ``thumbnail_id`` if you don't
+            want to change their values. Value ``None`` would unset
+            their value.
+
+        Update of ``data`` will override existing value on folder entity.
+
+        Update of ``attrib`` does change only passed attributes. If you want
+            to unset value, use ``None``.
+
+        Args:
+            project_name (str): Project name.
+            version_id (str): Version id.
+            version (Optional[int]): New version.
+            product_id (Optional[str]): New product id.
+            task_id (Optional[Union[str, None]]): New task id.
+            attrib (Optional[dict[str, Any]]): New attributes.
+            data (Optional[dict[str, Any]]): New data.
+            tags (Optional[Iterable[str]]): New tags.
+            status (Optional[str]): New status.
+            active (Optional[bool]): New active state.
+            thumbnail_id (Optional[Union[str, None]]): New thumbnail id.
+
+        """
+        update_data = {}
+        for key, value in (
+            ("version", version),
+            ("productId", product_id),
+            ("taskId", task_id),
+            ("attrib", attrib),
+            ("data", data),
+            ("tags", tags),
+            ("status", status),
+            ("active", active),
+        ):
+            if value is not None:
+                update_data[key] = value
+
+        for key, value in (
+            ("taskId", task_id),
+            ("thumbnailId", thumbnail_id),
+        ):
+            if value is not NOT_SET:
+                update_data[key] = value
+
+        response = self.patch(
+            "projects/{}/versions/{}".format(project_name, version_id),
+            **update_data
+        )
+        response.raise_for_status()
+
+    def delete_version(self, project_name, version_id):
+        """Delete version.
+
+        Args:
+            project_name (str): Project name.
+            version_id (str): Version id to delete.
+
+        """
+        response = self.delete(
+            "projects/{}/versions/{}".format(project_name, version_id)
+        )
+        response.raise_for_status()
+
     def _representation_conversion(self, representation):
         if "context" in representation:
             orig_context = representation["context"]
             context = {}
             if orig_context and orig_context != "null":
                 context = json.loads(orig_context)
             representation["context"] = context
@@ -4992,14 +5894,18 @@
 
         if active is not None:
             fields.add("active")
 
         if own_attributes:
             fields.add("ownAttrib")
 
+        if "files" in fields:
+            fields.discard("files")
+            fields |= REPRESENTATION_FILES_FIELDS
+
         filters = {
             "projectName": project_name
         }
 
         if representation_ids is not None:
             representation_ids = set(representation_ids)
             if not representation_ids:
@@ -5223,15 +6129,16 @@
         database. The context may contain project, folder, task name or
         product name, product type and many more. This implementation gives
         option to quickly filter representation based on representation data
         in database.
 
         Context filters have defined structure. To define filter of nested
             subfield use dot '.' as delimiter (For example 'task.name').
-        Filter values can be regex filters. String or 're.Pattern' can be used.
+        Filter values can be regex filters. String or ``re.Pattern`` can
+            be used.
 
         Args:
             project_name (str): Project where to look for representations.
             context_filters (dict[str, list[str]]): Filters of context fields.
             representation_names (Optional[Iterable[str]]): Representation
                 names, can be used as additional filter for representations
                 by their names.
@@ -5274,15 +6181,14 @@
         body_context_filters = []
         for key, filters in context_filters.items():
             if not isinstance(filters, (set, list, tuple)):
                 raise TypeError(
                     "Expected 'set', 'list', 'tuple' got {}".format(
                         str(type(filters))))
 
-
             new_filters = set()
             for filter_value in filters:
                 if isinstance(filter_value, PatternType):
                     filter_value = filter_value.pattern
                 new_filters.add(filter_value)
 
             body_context_filters.append({
@@ -5294,14 +6200,142 @@
             "projects/{}/repreContextFilter".format(project_name),
             context=body_context_filters,
             **filter_body
         )
         response.raise_for_status()
         return response.data["ids"]
 
+    def create_representation(
+        self,
+        project_name,
+        name,
+        version_id,
+        files=None,
+        attrib=None,
+        data=None,
+        tags=None,
+        status=None,
+        active=None,
+        representation_id=None,
+    ):
+        """Create new representation.
+
+        Args:
+            project_name (str): Project name.
+            name (str): Representation name.
+            version_id (str): Parent version id.
+            files (Optional[list[dict]]): Representation files information.
+            attrib (Optional[dict[str, Any]]): Representation attributes.
+            data (Optional[dict[str, Any]]): Representation data.
+            tags (Optional[Iterable[str]]): Representation tags.
+            status (Optional[str]): Representation status.
+            active (Optional[bool]): Representation active state.
+            representation_id (Optional[str]): Representation id. If not
+                passed new id is generated.
+
+        Returns:
+            str: Representation id.
+
+        """
+        if not representation_id:
+            representation_id = create_entity_id()
+        create_data = {
+            "id": representation_id,
+            "name": name,
+            "versionId": version_id,
+        }
+        for key, value in (
+            ("files", files),
+            ("attrib", attrib),
+            ("data", data),
+            ("tags", tags),
+            ("status", status),
+            ("active", active),
+        ):
+            if value is not None:
+                create_data[key] = value
+
+        response = self.post(
+            "projects/{}/representations".format(project_name),
+            **create_data
+        )
+        response.raise_for_status()
+        return representation_id
+
+    def update_representation(
+        self,
+        project_name,
+        representation_id,
+        name=None,
+        version_id=None,
+        files=None,
+        attrib=None,
+        data=None,
+        tags=None,
+        status=None,
+        active=None,
+    ):
+        """Update representation entity on server.
+
+        Update of ``data`` will override existing value on folder entity.
+
+        Update of ``attrib`` does change only passed attributes. If you want
+            to unset value, use ``None``.
+
+        Args:
+            project_name (str): Project name.
+            representation_id (str): Representation id.
+            name (Optional[str]): New name.
+            version_id (Optional[str]): New version id.
+            files (Optional[list[dict]]): New files
+                information.
+            attrib (Optional[dict[str, Any]]): New attributes.
+            data (Optional[dict[str, Any]]): New data.
+            tags (Optional[Iterable[str]]): New tags.
+            status (Optional[str]): New status.
+            active (Optional[bool]): New active state.
+
+        """
+        update_data = {}
+        for key, value in (
+            ("name", name),
+            ("versionId", version_id),
+            ("files", files),
+            ("attrib", attrib),
+            ("data", data),
+            ("tags", tags),
+            ("status", status),
+            ("active", active),
+        ):
+            if value is not None:
+                update_data[key] = value
+
+        response = self.patch(
+            "projects/{}/representations/{}".format(
+                project_name, representation_id
+            ),
+            **update_data
+        )
+        response.raise_for_status()
+
+    def delete_representation(self, project_name, representation_id):
+        """Delete representation.
+
+        Args:
+            project_name (str): Project name.
+            representation_id (str): Representation id to delete.
+
+        """
+        response = self.delete(
+            "projects/{}/representation/{}".format(
+                project_name, representation_id
+            )
+        )
+        response.raise_for_status()
+
     def get_workfiles_info(
         self,
         project_name,
         workfile_ids=None,
         task_ids=None,
         paths=None,
         path_regex=None,
@@ -5703,15 +6737,15 @@
     def create_project(
         self,
         project_name,
         project_code,
         library_project=False,
         preset_name=None
     ):
-        """Create project using Ayon settings.
+        """Create project using AYON settings.
 
         This project creation function is not validating project entity on
         creation. It is because project entity is created blindly with only
         minimum required information about project which is name and code.
 
         Entered project name must be unique and project must not exist yet.
 
@@ -6020,17 +7054,17 @@
             {
                 "id": "59a212c0d2e211eda0e20242ac120002"
             }
 
         Args:
             project_name (str): Project where the link is created.
             link_type_name (str): Type of link.
-            input_id (str): Id of input entity.
+            input_id (str): Input entity id.
             input_type (str): Entity type of input entity.
-            output_id (str): Id of output entity.
+            output_id (str): Output entity id.
             output_type (str): Entity type of output entity.
             link_name (Optional[str]): Name of link.
                 Available from server version '1.0.0-rc.6'.
 
         Returns:
             dict[str, str]: Information about link.
 
@@ -6049,15 +7083,15 @@
         rel_regex = re.compile(r"rc\.[0-5]")
         if (
             ((major, minor, patch) == (1, 0, 0) and rel_regex.match(rel))
             or (major, minor, patch) < (1, 0, 0)
         ):
             kwargs["link"] = full_link_type_name
             if link_name:
-                raise NotImplementedError((
+                raise UnsupportedServerVersion((
                     "Link name is not supported"
                     " for version of AYON server {}"
                 ).format(self.server_version))
         else:
             kwargs["linkType"] = full_link_type_name
 
         if link_name:
```

### Comparing `ayon-python-api-1.0.1/ayon_python_api.egg-info/PKG-INFO` & `ayon-python-api-1.0.2/ayon_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-1.0.1/pyproject.toml` & `ayon-python-api-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ayon-python-api"
-version = "1.0.1"
+version = "1.0.2"
 description = "AYON Python API"
 license = {file = "LICENSE"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     {name = "ynput.io", email = "info@ynput.io"}
 ]
 keywords = ["AYON", "ynput", "OpenPype", "vfx"]
@@ -27,15 +27,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ayon-python-api"
-version = "1.0.1"
+version = "1.0.2"
 description = "AYON Python API"
 authors = [
     "ynput.io <info@ynput.io>"
 ]
 
 [tool.poetry.dependencies]
 python = ">=2.7,>=3.6.5"
```

### Comparing `ayon-python-api-1.0.1/setup.py` & `ayon-python-api-1.0.2/setup.py`

 * *Files identical despite different names*

