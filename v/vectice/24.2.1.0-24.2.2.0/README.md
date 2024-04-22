# Comparing `tmp/vectice-24.2.1.0.tar.gz` & `tmp/vectice-24.2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-24.2.1.0.tar", last modified: Mon Apr 15 11:27:31 2024, max compression
+gzip compressed data, was "vectice-24.2.2.0.tar", last modified: Mon Apr 22 08:07:13 2024, max compression
```

## Comparing `vectice-24.2.1.0.tar` & `vectice-24.2.2.0.tar`

### file list

```diff
@@ -1,168 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.995369 vectice-24.2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 11:27:27.000000 vectice-24.2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-15 11:27:30.995369 vectice-24.2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 11:27:27.000000 vectice-24.2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-15 11:27:27.000000 vectice-24.2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 11:27:30.995369 vectice-24.2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-15 11:27:27.000000 vectice-24.2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.955368 vectice-24.2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.955368 vectice-24.2.1.0/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.963368 vectice-24.2.1.0/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.967368 vectice-24.2.1.0/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/entity_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/json_to_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/json_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/organization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.971368 vectice-24.2.1.0/src/vectice/autolog/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.971368 vectice-24.2.1.0/src/vectice/autolog/asset_services/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/catboost_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/keras_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/lightgbm_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/metric_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/pandas_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/pyspark_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/sklearn_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/asset_services/vectice_asset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/autolog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/autolog_asset_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    29286 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/autolog_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/autolog/model_library.py
--rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.975369 vectice-24.2.1.0/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/additional_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/code_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19789 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/model_exp_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/model_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.975369 vectice-24.2.1.0/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.979369 vectice-24.2.1.0/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/databricks_table_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.983369 vectice-24.2.1.0/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/dataframe_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/pyspark_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/no_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/resource/snowflake_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.983369 vectice-24.2.1.0/src/vectice/services/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/services/iteration_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/services/phase_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.983369 vectice-24.2.1.0/src/vectice/types/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.983369 vectice-24.2.1.0/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/code_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 11:27:27.000000 vectice-24.2.1.0/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:30.983369 vectice-24.2.1.0/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-15 11:27:30.000000 vectice-24.2.1.0/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-04-15 11:27:30.000000 vectice-24.2.1.0/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:27:30.000000 vectice-24.2.1.0/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-15 11:27:30.000000 vectice-24.2.1.0/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 11:27:30.000000 vectice-24.2.1.0/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.081815 vectice-24.2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 08:06:59.000000 vectice-24.2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-22 08:07:13.081815 vectice-24.2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-22 08:06:59.000000 vectice-24.2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 08:06:59.000000 vectice-24.2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-22 08:07:13.081815 vectice-24.2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-22 08:06:59.000000 vectice-24.2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.041815 vectice-24.2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.045815 vectice-24.2.2.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.049815 vectice-24.2.2.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12109 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.057815 vectice-24.2.2.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/json_to_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/organization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.057815 vectice-24.2.2.0/src/vectice/autolog/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.061815 vectice-24.2.2.0/src/vectice/autolog/asset_services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/catboost_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/keras_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/lightgbm_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/metric_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/pandas_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/pyspark_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/pytorch_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/sklearn_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/asset_services/vectice_asset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/autolog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/autolog_asset_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30734 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/autolog_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/autolog/model_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21843 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.065815 vectice-24.2.2.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/additional_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19022 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/model_exp_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/model_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.065815 vectice-24.2.2.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.065815 vectice-24.2.2.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/databricks_table_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.069815 vectice-24.2.2.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/dataframe_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/pyspark_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/no_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/resource/snowflake_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.069815 vectice-24.2.2.0/src/vectice/models/test_library/
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/test_library/binary_classification_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.069815 vectice-24.2.2.0/src/vectice/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/services/iteration_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/services/phase_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.069815 vectice-24.2.2.0/src/vectice/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.073815 vectice-24.2.2.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/code_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-22 08:06:59.000000 vectice-24.2.2.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:07:13.073815 vectice-24.2.2.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-22 08:07:13.000000 vectice-24.2.2.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-22 08:07:13.000000 vectice-24.2.2.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:07:13.000000 vectice-24.2.2.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-22 08:07:13.000000 vectice-24.2.2.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 08:07:13.000000 vectice-24.2.2.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-24.2.1.0/LICENSE` & `vectice-24.2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/PKG-INFO` & `vectice-24.2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.1.0
+Version: 24.2.2.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -88,21 +88,25 @@
 Requires-Dist: tensorflow; extra == "test"
 Requires-Dist: keras; extra == "test"
 Requires-Dist: snowflake-snowpark-python; extra == "test"
 Requires-Dist: seaborn; extra == "test"
 Requires-Dist: xgboost; extra == "test"
 Requires-Dist: kaleido; extra == "test"
 Requires-Dist: catboost; extra == "test"
+Requires-Dist: torch; extra == "test"
 Provides-Extra: gcs
 Requires-Dist: google-cloud-storage>=1.17.0; extra == "gcs"
 Requires-Dist: google-cloud-bigquery; extra == "gcs"
 Provides-Extra: s3
 Requires-Dist: boto3; extra == "s3"
 Provides-Extra: autolog
 Requires-Dist: IPython; extra == "autolog"
-Requires-Dist: plotly; extra == "autolog"
+Provides-Extra: validation
+Requires-Dist: shap; extra == "validation"
+Requires-Dist: scipy; extra == "validation"
+Requires-Dist: pandas; extra == "validation"
 
 Auto-documentation for ML projects & their governance. View https://github.com/vectice/GettingStarted to get started.
 
 # Documentation
 
 Official documentation for Vectice can be found at https://docs.vectice.com.
```

### Comparing `vectice-24.2.1.0/pyproject.toml` & `vectice-24.2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/setup.py` & `vectice-24.2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,18 +96,20 @@
             "tensorflow",
             "keras",
             "snowflake-snowpark-python",
             "seaborn",
             "xgboost",
             "kaleido",
             "catboost",
+            "torch",
         ],
         "gcs": ["google-cloud-storage>=1.17.0", "google-cloud-bigquery"],
         "s3": ["boto3"],
-        "autolog": ["IPython", "plotly"],
+        "autolog": ["IPython"],
+        "validation": ["shap", "scipy", "pandas"],
     },
     classifiers=[
         "Topic :: Internet",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `vectice-24.2.1.0/src/vectice/__init__.py` & `vectice-24.2.2.0/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/_auth.py` & `vectice-24.2.2.0/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/attachment.py` & `vectice-24.2.2.0/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/client.py` & `vectice-24.2.2.0/src/vectice/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,29 +26,28 @@
     ArtifactName,
     ModelRegisterInput,
     ModelRegisterOutput,
     ModelVersionOutput,
     ModelVersionStatus,
     PagedResponse,
     PropertyInput,
-    StepOutput,
+    RequirementOutput,
 )
 from vectice.api.json.code_version import CodeVersion
 from vectice.api.json.dataset_register import DatasetRegisterInput, DatasetRegisterOutput
 from vectice.api.json.dataset_representation import DatasetRepresentationOutput
 from vectice.api.json.dataset_version import DatasetVersionOutput
 from vectice.api.json.dataset_version_representation import DatasetVersionRepresentationOutput
 from vectice.api.json.iteration import IterationContextInput, IterationStatus
 from vectice.api.json.metric import MetricInput
 from vectice.api.json.model_representation import ModelRepresentationOutput
 from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput, ModelVersionUpdateInput
 from vectice.api.json.organization_config import OrgConfigOutput
 from vectice.api.phase import PhaseApi
 from vectice.api.project import ProjectApi
-from vectice.api.step import StepApi
 from vectice.api.version import VersionApi
 from vectice.api.workspace import WorkspaceApi
 from vectice.models.dataset import Dataset
 from vectice.models.iteration import Iteration
 from vectice.models.model import Model
 from vectice.models.phase import Phase
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
@@ -261,32 +260,23 @@
         if project_id is None:
             raise MissingReferenceError("project")
         return PhaseApi(self._gql_client, self.auth).get_phase(phase, project_id)
 
     def get_full_phase(self, phase: str) -> PhaseOutput:
         return PhaseApi(self._gql_client, self.auth).get_phase(phase=phase, full=True)
 
-    def get_step_by_name(self, step_reference: str, iteration_id: str) -> StepOutput:
-        return StepApi(self._gql_client, self.auth).get_step(step_reference, iteration_id)
-
     def list_sections(self, iteration_id: str) -> IterationOutput:
         return IterationApi(self._gql_client, self.auth).list_sections(iteration_id)
 
-    def list_steps(self, iteration_id: str, populate: bool = True) -> PagedResponse[StepOutput]:
-        return StepApi(self._gql_client, self.auth).list_steps(iteration_id, populate)
-
-    def add_iteration_step_artifact(self, step_id: int, artifact: IterationStepArtifactInput) -> StepOutput:
-        return StepApi(self._gql_client, self.auth).add_iteration_step_artifact(artifact, step_id)
-
     def list_iterations(
         self, phase: str, only_mine: bool = False, statuses: list[IterationStatus] | None = None
     ) -> PagedResponse[IterationOutput]:
         return IterationApi(self._gql_client, self.auth).list_iterations(phase, only_mine, statuses)
 
-    def list_step_definitions(self, phase: str) -> PagedResponse[StepOutput]:
+    def list_step_definitions(self, phase: str) -> PagedResponse[RequirementOutput]:
         return PhaseApi(self._gql_client, self.auth).list_step_definitions(phase)
 
     def get_last_iteration(self, phase_id: str) -> IterationOutput:
         return IterationApi(self._gql_client, self.auth).get_last_iteration(phase_id)
 
     def get_active_iteration_or_create(self, phase_id: str) -> IterationOutput:
         return IterationApi(self._gql_client, self.auth).get_active_iteration_or_create(phase_id)
```

### Comparing `vectice-24.2.1.0/src/vectice/api/gql_api.py` & `vectice-24.2.2.0/src/vectice/api/gql_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     IterationStepArtifact,
     ModelRegisterOutput,
     OrgConfigOutput,
     PagedResponse,
     PhaseOutput,
     ProjectOutput,
     PublicConfigOutput,
-    StepOutput,
+    RequirementOutput,
+    SectionOutput,
     UserActivity,
     UserAndDefaultWorkspaceOutput,
     WorkspaceOutput,
 )
 from vectice.api.json.dataset_representation import DatasetRepresentationOutput
 from vectice.api.json.dataset_version_representation import DatasetVersionRepresentationOutput
 from vectice.api.json.entity_file import EntityFileOutput
@@ -76,29 +77,29 @@
                 return self.parse_item(data)
 
     def _build_map(self):
         return {
             "Workspace": WorkspaceOutput,
             "Project": ProjectOutput,
             "Phase": PhaseOutput,
-            "IterationStep": StepOutput,
+            "IterationStep": SectionOutput,
             "Iteration": IterationOutput,
             "IterationStepArtifact": IterationStepArtifact,
             "DatasetRegisterResultOutput": DatasetRegisterOutput,
             "ModelRegisterResultOutput": ModelRegisterOutput,
             "DataSet": DatasetRepresentationOutput,
             "DataSetVersion": DatasetVersionRepresentationOutput,
             "EntityFile": EntityFileOutput,
             "Model": ModelRepresentationOutput,
             "ModelVersion": ModelVersionRepresentationOutput,
             "UserActivity": UserActivity,
             "Code": CodeOutput,
             "PublicConfigOutput": PublicConfigOutput,
             "UserAndDefaultWorkspaceOutput": UserAndDefaultWorkspaceOutput,
-            "StepDefinition": StepOutput,
+            "StepDefinition": RequirementOutput,
             "OrgConfigOutput": OrgConfigOutput,
         }
 
 
 class GqlApi:
     def __init__(self, client: Client, auth: Auth):
         self.client: Client = client
```

### Comparing `vectice-24.2.1.0/src/vectice/api/gql_dataset.py` & `vectice-24.2.2.0/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/gql_entity_file.py` & `vectice-24.2.2.0/src/vectice/api/gql_entity_file.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/gql_feature_flag.py` & `vectice-24.2.2.0/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/gql_metric.py` & `vectice-24.2.2.0/src/vectice/api/gql_metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/gql_model.py` & `vectice-24.2.2.0/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/gql_organization.py` & `vectice-24.2.2.0/src/vectice/api/gql_organization.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/gql_property.py` & `vectice-24.2.2.0/src/vectice/api/gql_property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/gql_user_workspace_api.py` & `vectice-24.2.2.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/http_error.py` & `vectice-24.2.2.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/http_error_handlers.py` & `vectice-24.2.2.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/iteration.py` & `vectice-24.2.2.0/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/__init__.py` & `vectice-24.2.2.0/src/vectice/api/json/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 from vectice.api.json.organization_config import OrgConfigOutput
 from vectice.api.json.page import Page
 from vectice.api.json.paged_response import PagedResponse
 from vectice.api.json.phase import PhaseOutput
 from vectice.api.json.project import ProjectOutput
 from vectice.api.json.property import PropertyInput, PropertyOutput
 from vectice.api.json.public_config import ArtifactName, PublicConfigOutput
-from vectice.api.json.step import StepOutput
+from vectice.api.json.requirement import RequirementOutput
+from vectice.api.json.section import SectionOutput
 from vectice.api.json.user_and_workspace import UserAndDefaultWorkspaceOutput
 from vectice.api.json.workspace import WorkspaceInput, WorkspaceOutput
 
 __all__ = [
     "ArtifactVersion",
     "VersionStrategy",
     "AttachmentOutput",
@@ -48,15 +49,16 @@
     "PropertyOutput",
     "FileMetadata",
     "FileMetadataType",
     "WorkspaceOutput",
     "WorkspaceInput",
     "Page",
     "PhaseOutput",
-    "StepOutput",
+    "RequirementOutput",
+    "SectionOutput",
     "IterationInput",
     "IterationOutput",
     "IterationStatus",
     "IterationStepArtifactInput",
     "IterationStepArtifact",
     "IterationStepArtifactType",
     "DatasetRegisterOutput",
```

### Comparing `vectice-24.2.1.0/src/vectice/api/json/artifact_version.py` & `vectice-24.2.2.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/code.py` & `vectice-24.2.2.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/code_version.py` & `vectice-24.2.2.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/dataset_register.py` & `vectice-24.2.2.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/dataset_representation.py` & `vectice-24.2.2.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/dataset_version.py` & `vectice-24.2.2.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/dataset_version_representation.py` & `vectice-24.2.2.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/files_metadata.py` & `vectice-24.2.2.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/iteration.py` & `vectice-24.2.2.0/src/vectice/api/json/iteration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import TYPE_CHECKING, Any
+from typing import Any
 
 from vectice.api.json.json_type import TJSON
 from vectice.api.json.paged_response import PagedResponse
-from vectice.api.json.step import PhaseOutput
-
-if TYPE_CHECKING:
-    from vectice.api.json.step import StepOutput
+from vectice.api.json.phase import PhaseOutput
+from vectice.api.json.section import SectionOutput
 
 
 class IterationStatus(Enum):
     NotStarted = "NotStarted"
     InProgress = "InProgress"
     InReview = "InReview"
     Abandoned = "Abandoned"
@@ -149,28 +147,20 @@
         return int(self["index"])
 
     @property
     def name(self) -> str:
         return str(self["name"])
 
     @property
-    def sections(self) -> PagedResponse[StepOutput]:
+    def sections(self) -> PagedResponse[SectionOutput]:
         from vectice.api.gql_api import Parser
 
         return Parser().parse_paged_response(self["sections"])
 
     @property
-    def steps(self) -> list[StepOutput]:
-        from vectice.api.json.step import StepOutput
-
-        steps_json = self["steps"]
-        steps = [StepOutput(step) for step in steps_json]
-        return steps
-
-    @property
     def alias(self) -> str:
         return str(self["alias"])
 
     @property
     def status(self) -> IterationStatus:
         return IterationStatus(self["status"])
```

### Comparing `vectice-24.2.1.0/src/vectice/api/json/json_to_class.py` & `vectice-24.2.2.0/src/vectice/api/json/json_to_class.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/last_assets.py` & `vectice-24.2.2.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/metric.py` & `vectice-24.2.2.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/model.py` & `vectice-24.2.2.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/model_register.py` & `vectice-24.2.2.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/model_representation.py` & `vectice-24.2.2.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/model_version.py` & `vectice-24.2.2.0/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/model_version_representation.py` & `vectice-24.2.2.0/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/paged_response.py` & `vectice-24.2.2.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/phase.py` & `vectice-24.2.2.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/project.py` & `vectice-24.2.2.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/property.py` & `vectice-24.2.2.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/public_config.py` & `vectice-24.2.2.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/user_and_workspace.py` & `vectice-24.2.2.0/src/vectice/api/json/user_and_workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/json/workspace.py` & `vectice-24.2.2.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/phase.py` & `vectice-24.2.2.0/src/vectice/api/phase.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from vectice.api.gql_api import GqlApi, Parser
 from vectice.utils.api_utils import INDEX_ORDERED, PAGINATE_OUTPUT, get_page_input
 from vectice.utils.vectice_ids_regex import PHASE_VID_REG
 
 if TYPE_CHECKING:
     from vectice.api.json.paged_response import PagedResponse
     from vectice.api.json.phase import PhaseOutput
-    from vectice.api.json.step import StepOutput
+    from vectice.api.json.requirement import RequirementOutput
 
 
 _RETURNS = """vecticeId
               name
               status
               index
               owner {
@@ -126,15 +126,15 @@
         try:
             response = self.execute(query_built, variables)
             phase_output: PhaseOutput = Parser().parse_item(response[gql_query])
             return phase_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "phase", phase)
 
-    def list_step_definitions(self, parent_id: str) -> PagedResponse[StepOutput]:
+    def list_step_definitions(self, parent_id: str) -> PagedResponse[RequirementOutput]:
         gql_query = "getStepDefinitionList"
         alias_filter = {"parentId": parent_id}
         returns = _STEP_DEFINITION_RETURNS
         variable_types = "$filters:BaseDocumentationListFiltersInput!,$order:ListOrderInput,$page:PageInput"
         kw = "filters:$filters,order:$order,page:$page"
         variables = {
             "filters": alias_filter,
@@ -147,11 +147,11 @@
             returns=returns,
             keyword_arguments=kw,
             query=True,
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
-            requirements: PagedResponse[StepOutput] = Parser().parse_paged_response(response[gql_query])
+            requirements: PagedResponse[RequirementOutput] = Parser().parse_paged_response(response[gql_query])
             return requirements
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "phase", "list")
```

### Comparing `vectice-24.2.1.0/src/vectice/api/project.py` & `vectice-24.2.2.0/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/rest_api.py` & `vectice-24.2.2.0/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/version.py` & `vectice-24.2.2.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/api/workspace.py` & `vectice-24.2.2.0/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/autolog/asset_services/__init__.py` & `vectice-24.2.2.0/src/vectice/autolog/asset_services/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from vectice.autolog.asset_services.catboost_service import AutologCatboostService
 from vectice.autolog.asset_services.keras_service import AutologKerasService
 from vectice.autolog.asset_services.lightgbm_service import AutologLightgbmService
 from vectice.autolog.asset_services.pandas_service import AutologPandasService
 from vectice.autolog.asset_services.pyspark_service import AutologPysparkService
+from vectice.autolog.asset_services.pytorch_service import AutologPytorchService
 from vectice.autolog.asset_services.sklearn_service import AutologSklearnService
 from vectice.autolog.asset_services.vectice_asset_service import (
     AutologVecticeAssetService,
     TVecticeObjects,
     VecticeObjectClasses,
     VecticeObjectTypes,
 )
 
 __all__ = [
     "AutologPandasService",
     "AutologPysparkService",
+    "AutologPytorchService",
     "AutologCatboostService",
     "AutologKerasService",
     "AutologLightgbmService",
     "AutologSklearnService",
     "AutologVecticeAssetService",
     "TVecticeObjects",
     "VecticeObjectTypes",
```

### Comparing `vectice-24.2.1.0/src/vectice/autolog/asset_services/catboost_service.py` & `vectice-24.2.2.0/src/vectice/autolog/asset_services/catboost_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/autolog/asset_services/keras_service.py` & `vectice-24.2.2.0/src/vectice/autolog/asset_services/keras_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/autolog/asset_services/lightgbm_service.py` & `vectice-24.2.2.0/src/vectice/autolog/asset_services/lightgbm_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/autolog/asset_services/sklearn_service.py` & `vectice-24.2.2.0/src/vectice/autolog/asset_services/sklearn_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/autolog/asset_services/vectice_asset_service.py` & `vectice-24.2.2.0/src/vectice/autolog/asset_services/vectice_asset_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from __future__ import annotations
 
 from typing import TypedDict, TypeVar
 
 from vectice.models.dataset import Dataset
 from vectice.models.model import Model
 from vectice.models.table import Table
+from vectice.models.validation import ValidationModel
 
-VecticeObjectTypes = TypeVar("VecticeObjectTypes", Dataset, Model, Table)
-TVecticeObjects = TypedDict(
-    "TVecticeObjects",
-    {"variable": str, "vectice_object": VecticeObjectTypes},
-)
-VecticeObjectClasses = (Dataset, Model, Table)
+VecticeObjectTypes = TypeVar("VecticeObjectTypes", Dataset, Model, Table, ValidationModel)
+TVecticeObjects = TypedDict("TVecticeObjects", {"variable": str, "vectice_object": VecticeObjectTypes})
+VecticeObjectClasses = (Dataset, Model, Table, ValidationModel)
 
 
 class AutologVecticeAssetService:
     def __init__(self, key: str, asset: VecticeObjectTypes):
         self._asset = asset
         self._key = key
```

### Comparing `vectice-24.2.1.0/src/vectice/autolog/autolog.py` & `vectice-24.2.2.0/src/vectice/autolog/autolog.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     ```
 
 2.** Supported libraries and environment:**
     Vectice automatically identifies and log assets encapsulated within a specified list of supported libraries and environement mentioned below
 
 NOTE: **Supported libraries and environment**
     - Dataframe: Pandas, Spark.
-    - Model: Scikit, Xgboost, Lightgbm, Catboost, Keras.
+    - Model: Scikit, Xgboost, Lightgbm, Catboost, Keras, Pytorch.
     - Graphs: Matplotlib, Seaborn, Plotly.
     - Environments: Colab, Jupyter, Vertex, SageMaker, Databricks, Pycharm and VScode notebook.
 
 3.** General behavior:**
     Vectice autolog provides three methods: autolog.config, autolog.notebook, and autolog.cell. These methods are designed to log every asset to Vectice existing as a variable in the notebook's memory. It is important to review the specific behaviors outlined in the documentation for each of these three methods.
 
 NOTE: **IMPORTANT INFORMATION**
```

### Comparing `vectice-24.2.1.0/src/vectice/autolog/autolog_asset_factory.py` & `vectice-24.2.2.0/src/vectice/autolog/autolog_asset_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from vectice.api.http_error_handlers import VecticeException
 from vectice.autolog.asset_services import (
     AutologCatboostService,
     AutologKerasService,
     AutologLightgbmService,
     AutologPandasService,
     AutologPysparkService,
+    AutologPytorchService,
     AutologSklearnService,
     AutologVecticeAssetService,
     VecticeObjectClasses,
 )
 
 
 class IAutologService(Protocol):
@@ -27,14 +28,15 @@
     def get_asset_service(key: str, asset: Any, data: dict) -> IAutologService:
         is_pandas = find_spec("pandas") is not None
         is_pyspark = find_spec("pyspark") is not None
         is_lgbm = find_spec("lightgbm") is not None
         is_sklearn = find_spec("sklearn") is not None
         is_catboost = find_spec("catboost") is not None
         is_keras = find_spec("keras") is not None
+        is_pytorch = find_spec("torch") is not None
 
         if is_pandas:
             from pandas import DataFrame
 
             if isinstance(asset, DataFrame):
                 return AutologPandasService(key, asset)
 
@@ -58,14 +60,20 @@
 
         if is_keras:
             from keras.models import Model as KerasModel
 
             if isinstance(asset, KerasModel):
                 return AutologKerasService(key, asset, data)
 
+        if is_pytorch:
+            from torch.nn import Module
+
+            if isinstance(asset, Module):
+                return AutologPytorchService(key, asset, data)
+
         if isinstance(asset, VecticeObjectClasses):
             return AutologVecticeAssetService(key, asset)  # type: ignore[reportArgumentType]
 
         if is_sklearn:
             return AutologSklearnService(key, asset, data)
 
         raise VecticeException(f"Asset {asset} of type ({type(asset)!r}) not handled")
```

### Comparing `vectice-24.2.1.0/src/vectice/autolog/autolog_class.py` & `vectice-24.2.2.0/src/vectice/autolog/autolog_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,34 +15,36 @@
 import PIL.Image as Image
 from typing_extensions import TypedDict
 
 from vectice.api.http_error_handlers import VecticeException
 from vectice.autolog.autolog_asset_factory import AssetFactory
 from vectice.autolog.model_library import ModelLibrary
 from vectice.models.dataset import Dataset
+from vectice.models.model import Model
 from vectice.models.table import Table
 from vectice.utils.code_parser import VariableVisitor, parse_comments, preprocess_code
 
 if TYPE_CHECKING:
     from tempfile import TemporaryDirectory
 
     from catboost.core import CatBoost
     from keras import Model as KerasModel
     from keras.layers import InputLayer
     from lightgbm.basic import Booster
     from pandas import DataFrame
     from pyspark.sql import DataFrame as SparkDF
     from sklearn.base import BaseEstimator
+    from torch.nn import Module as TorchModel
 
     # Vectice Object types
     from vectice.autolog.asset_services import TVecticeObjects
     from vectice.models import Phase
     from vectice.models.resource.metadata.db_metadata import TableType
 
-    ModelTypes = TypeVar("ModelTypes", BaseEstimator, Booster, CatBoost, KerasModel)
+    ModelTypes = TypeVar("ModelTypes", BaseEstimator, Booster, CatBoost, KerasModel, TorchModel)
     TModel = TypedDict(
         "TModel",
         {
             "variable": str,
             "model": ModelTypes,
             "library": ModelLibrary,
             "metrics": dict,
@@ -183,15 +185,17 @@
         # check if graphs have been commented out before getting saved graphs
         _remove_commented_graphs()
         # get the saved graphs
         saved_graphs = _get_saved_graphs()
         # check if running already and that there aren't saved graphs as saved graphs are the priority
         if not running and not saved_graphs and _check_graph_libraries(cell_content):
             running = True
-            ipython.run_cell_magic("capture", plot_name, cell_content)  # type: ignore
+            # Remove autolog from cell so we don't create an extra iteration
+            clean_cell = re.sub(r"autolog.*?$", "", cell_content)
+            ipython.run_cell_magic("capture", plot_name, clean_cell)  # type: ignore
             # Check if plot name is already in our list as we don't want duplicates
             if plot_name not in GRAPHS:
                 GRAPHS.append(plot_name)
         # remove event graph if save graph true, prevents double capturing
         if saved_graphs and plot_name in GRAPHS:
             GRAPHS.remove(plot_name)
         running = False
@@ -477,14 +481,38 @@
                     self._iteration_service.log_comment(comment)
         # Logging for comments captured
         all_comments_logged.discard(None)
         filtered_comments = list(filter(lambda comment: comment is not None, still_comments_to_log))
         if filtered_comments or all_comments_logged:
             _logger.info(f"Comments logged in iteration {self._iteration.name!r}.")
 
+    def _format_pytorch_params(self, model: TorchModel) -> dict[str, Any]:
+        params: dict[str, Any] = {}
+
+        model_layers = list(model.children())
+        # Get the parameters of each layer
+        total_params = sum(param.numel() for param in model.parameters())
+        for i, layer in enumerate(model_layers):
+            layer_params = sum(param.numel() for param in layer.parameters())
+            output_shape = layer.out_features if hasattr(layer, "out_features") else None
+            params[f"Layer-{i}"] = {
+                "name": layer._get_name(),  # pyright: ignore[reportPrivateUsage]
+                "param": layer_params,
+                "output shape": output_shape,
+            }
+            params["Total # of weights"] = total_params
+
+        return params
+
+    def _get_pytorch_info(self, model: TorchModel) -> tuple[str, dict[str, Any]] | tuple[None, None]:
+        try:
+            return "torch", self._format_pytorch_params(model)
+        except Exception:
+            return None, None
+
     def _log_assets(
         self,
         assets: list[TModel | TDataset | TVecticeObjects],
     ):
         # all comments and variables
         all_comments_and_variables = self._get_all_cells_comments()
         # Unique comment set
@@ -522,14 +550,16 @@
             return self._get_sklearn_or_xgboost_or_lgbm_info(model)  # pyright: ignore[reportArgumentType]
         if library is ModelLibrary.LIGHTGBM:
             return self._get_lightgbm_info(model)  # pyright: ignore[reportArgumentType]
         if library is ModelLibrary.CATBOOST:
             return self._get_catboost_info(model)  # pyright: ignore[reportArgumentType]
         if library is ModelLibrary.KERAS:
             return self._get_keras_info(model)  # pyright: ignore[reportArgumentType]
+        if library is ModelLibrary.PYTORCH:
+            return self._get_pytorch_info(model)  # pyright: ignore[reportArgumentType]
         return None, None
 
     def _check_for_single_model(self):
         model_list = [asset for asset in self._assets if "model" in asset]
         if len(model_list) > 1:
             return False
         return True
@@ -544,16 +574,14 @@
         for data in self._vectice_data:
             cell_metrics = MetricService(data["cell"])._get_model_metrics(data)  # type: ignore[reportPrivateUsage]
             if cell_metrics:
                 metrics.update(cell_metrics)
         return metrics
 
     def _log_model(self, model: TModel):
-        from vectice import Model
-
         temp_dir: TemporaryDirectory | None = None
         temp_file_path: str | None = None
         if model["library"] is ModelLibrary.KERAS:
             graph = None
 
             try:
                 from keras.utils import plot_model
@@ -597,28 +625,27 @@
         if temp_dir is not None:
             temp_dir.cleanup()
 
     def _log_vectice_asset(self, asset: TVecticeObjects) -> None:
         asset_to_log = asset["vectice_object"]
         asset_name = asset["variable"]
         if isinstance(asset_to_log, Dataset):
-            dataset = asset_to_log
-            dataset_name = dataset.name if dataset.name else asset_name
+            dataset_name = asset_to_log.name if asset_to_log.name else asset_name
             self._iteration_service.log_dataset(asset_to_log)
             _logger.info(f"Dataset {dataset_name!r} logged in iteration {self._iteration.name!r}.")
         elif isinstance(asset_to_log, Table):
-            table = asset_to_log
-            table_name = table.name if table.name else asset_name
+            table_name = asset_to_log.name if asset_to_log.name else asset_name
             self._iteration_service.log_table(asset_to_log)
-            _logger.info(f"Table {table_name!r} logged in iteration {self._iteration.name!r}.")
-        else:
-            model = asset_to_log
-            model_name = model.name if model.name else asset_name
+            _logger.info(f"Table {table_name!r} logged in iteration {self._iteration.index!r}.")
+        elif isinstance(asset_to_log, Model):
+            model_name = asset_to_log.name if asset_to_log.name else asset_name
             self._iteration_service.log_model(asset_to_log)
-            _logger.info(f"Model {model_name!r} logged in iteration {self._iteration.name!r}.")
+            _logger.info(f"Model {model_name!r} logged in iteration {self._iteration.index!r}.")
+        else:
+            self._iteration._log_validation_model(asset_to_log)  # pyright: ignore[reportPrivateUsage]
 
     def _log_dataset(self, dataset: TDataset) -> None:
         from vectice import Dataset, DatasetType, FileResource, NoResource
 
         resource = self._get_dataset_resource(dataset)
         dataset_name = f"{self._iteration.phase.id}-{dataset['variable']}"
         no_resource_dataset = Dataset(
```

### Comparing `vectice-24.2.1.0/src/vectice/connection.py` & `vectice-24.2.2.0/src/vectice/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,15 @@
             The desired iteration.
         """
         if not re.search(ITERATION_VID_REG, iteration):
             raise InvalidIdError("iteration", iteration)
         output = self._client.get_iteration_by_id(iteration, True)
         logging_output = dedent(
             f"""
-                Iteration number {output.index!r} successfully retrieved.
+                Iteration {output.name!r} successfully retrieved.
 
                 For quick access to the Iteration in the Vectice web app, visit:
                 {self._client.auth.api_base_url}/browse/iteration/{output.id}"""
         ).lstrip()
         _logger.info(logging_output)
         return self._build_iteration_from_output(output)
```

### Comparing `vectice-24.2.1.0/src/vectice/models/__init__.py` & `vectice-24.2.2.0/src/vectice/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,22 @@
 from vectice.models.attachment_container import AttachmentContainer
 from vectice.models.errors import VecticeError
 from vectice.models.iteration import Iteration
 from vectice.models.metric import Metric
 from vectice.models.phase import Phase
 from vectice.models.project import Project
 from vectice.models.property import Property
-from vectice.models.step import Step
 from vectice.models.workspace import Workspace
 
 __all__ = [
     "AttachmentContainer",
     "Metric",
     "Property",
     "Project",
     "VecticeError",
     "Workspace",
     "Phase",
-    "Step",
     "Iteration",
     "AdditionalInfo",
     "ExtraInfo",
     "Framework",
 ]
```

### Comparing `vectice-24.2.1.0/src/vectice/models/additional_info.py` & `vectice-24.2.2.0/src/vectice/models/additional_info.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/attachment_container.py` & `vectice-24.2.2.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/code_version.py` & `vectice-24.2.2.0/src/vectice/models/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/dataset.py` & `vectice-24.2.2.0/src/vectice/models/dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/iteration.py` & `vectice-24.2.2.0/src/vectice/models/iteration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 from __future__ import annotations
 
 import logging
-from contextlib import suppress
 from io import IOBase
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any, ClassVar
 
 from PIL.Image import Image
 from rich.table import Table as RichTable
 
-from vectice.api.http_error_handlers import ArtifactVersionIdExistingError, NoStepsInPhaseError, VecticeException
+from vectice.api.http_error_handlers import ArtifactVersionIdExistingError, VecticeException
 from vectice.api.json.iteration import (
     IterationInput,
     IterationOutput,
     IterationStatus,
     IterationStepArtifactInput,
 )
-from vectice.models.step import Step
+from vectice.models.validation import ValidationModel
 from vectice.services.iteration_service import IterationService
 from vectice.utils.common_utils import (
     check_read_only,
     ensure_correct_project_id_from_representation_objs,
-    get_step_type,
     temp_print,
 )
-from vectice.utils.deprecation import deprecate
 from vectice.utils.instance_helper import is_image_or_file
 from vectice.utils.last_assets import (
     assign_asset_version_logging,
     comment_or_image_logging,
     register_dataset_logging,
     register_model_logging,
     table_logging,
@@ -105,51 +102,24 @@
         self.__dict__ = {}
         self._id = output.id
         self._index = output.index
         self._name = output.name
         self._phase = phase
         self._status = output.status
         self._client = client
-        self._steps = self._populate_steps()
         self._service = IterationService(self, self._client)
 
     def __repr__(self) -> str:
         return f"Iteration (name={self._name}, status={get_iteration_status(self._status)})"
 
     def __eq__(self, other: object):
         if not isinstance(other, Iteration):
             return NotImplemented
         return self.id == other.id
 
-    def _populate_steps(self) -> dict[str, Step]:
-        with suppress(NoStepsInPhaseError):
-            step_output = self._client.list_steps(self.id, True).list
-            steps = [get_step_type(step_output=item, iteration=self) for item in step_output]
-            check = {step.slug: step for step in steps}
-            return check
-        return {}
-
-    def __getattr__(self, item: str) -> Step:
-        if item in self.__dict__:
-            return self.__dict__[item]
-        if item in super().__getattribute__("_steps"):
-            step_item = self._steps[item]
-            step = self._client.get_step_by_name(step_item.name, self.id)
-            return get_step_type(step_output=step, iteration=self)
-        raise AttributeError(f"The attribute '{item}' does not exist.")
-
-    def __setattr__(self, attr_name: str, attr_value: Any):
-        if hasattr(self, "_steps") and attr_name in super().__getattribute__("_steps"):
-            self._steps[attr_name] = self._steps[attr_name].step_factory_and_update(value=attr_value)
-        # adding name handling but not sure this raise condition is necessary, don't want to break other things
-        elif hasattr(self, "__dict__") and attr_name not in self.__slots__ and attr_name != "name":
-            raise AttributeError(f"The attribute '{attr_name}' does not exist.")
-        else:
-            super().__setattr__(attr_name, attr_value)
-
     @property
     def id(self) -> str:
         """The iteration's identifier.
 
         Returns:
             The iteration's identifier.
         """
@@ -271,29 +241,14 @@
             """
         ).lstrip()
 
         temp_print(description)
         temp_print(table=rich_table)
         temp_print(link)
 
-    @deprecate(
-        warn_at="23.4",
-        fail_at="24.1",
-        remove_at="24.2",
-        reason="Steps are deprecated. Please use iteration.list_sections() instead.",
-    )
-    def list_steps(self) -> None:
-        """WARNING: **DEPRECATED** To list the sections of your iteration, use list_sections() instead.
-
-        Prints a list of steps belonging to the iteration in a tabular format, limited to the first 10 steps. A link is provided to view the remaining steps.
-
-        Returns:
-            None
-        """
-
     def cancel(self) -> None:
         """Cancel the iteration."""
         iteration_input = IterationInput(status=IterationStatus.Abandoned.name)
         self._client.update_iteration(self.id, iteration_input)
         self._status = IterationStatus.Abandoned
         _logger.info(f"Iteration {self.name} cancelled.")
 
@@ -447,14 +402,16 @@
             self._assign_version_representation(asset, section)
 
         elif isinstance(asset, Model):
             self._log_model(asset, section)
 
         elif isinstance(asset, Dataset):
             self._log_dataset(asset, section)
+        elif isinstance(asset, ValidationModel):
+            self._log_validation_model(asset, section)
         else:
             raise TypeError(f"Expected Image, Comment, Dataset or a Model, got {type(asset)}")
 
     def _log_image_or_file(self, asset: str | IOBase | Image, section: str | None = None):
         filename = self._service.log_image_or_file(asset, section)
         comment_or_image_logging(self, _logger, section, filename)
 
@@ -501,14 +458,38 @@
         model_data, attachments_output, success_pickle = self._service.log_model(asset, section)
         register_model_logging(self, model_data, asset, attachments_output, success_pickle, _logger, section)
 
     def _log_dataset(self, asset: Dataset, section: str | None = None):
         dataset_output, attachments_output = self._service.log_dataset(asset, section)
         register_dataset_logging(self, dataset_output, asset, attachments_output, _logger, section)
 
+    def _log_validation_model(self, asset: ValidationModel, section: str | None = None):
+        from vectice.models.representation.model_version_representation import ModelVersionRepresentation
+
+        self._client.assert_feature_flag_or_raise("validation-library")
+
+        validated = asset.execute_test()
+        metrics = validated.get("metrics") if len(validated.get("metrics")) > 0 else None
+        properties = validated.get("properties") if len(validated.get("properties")) > 0 else None
+        attachments = validated.get("attachments") if len(validated.get("attachments")) > 0 else None
+
+        if asset.asset:
+            mdv = ModelVersionRepresentation(output=self._client.get_model_version(asset.asset), client=self._client)
+            mdv.update(metrics=metrics, properties=properties, attachments=attachments)
+            self._assign_version_representation(mdv)
+        else:
+            if attachments is not None:
+                for attachment in attachments:
+                    self._log_image_or_file(attachment, section)
+
+        tables = validated.get("table")
+        if tables is not None:
+            for table in tables:
+                self._log_table(table, section)
+
     def _get_asset_type_from_asset_representation(
         self,
         asset: TAssetType,
     ):
         from vectice.models.representation.dataset_representation import DatasetRepresentation
         from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
         from vectice.models.representation.model_representation import ModelRepresentation
```

### Comparing `vectice-24.2.1.0/src/vectice/models/metric.py` & `vectice-24.2.2.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/model.py` & `vectice-24.2.2.0/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/model_exp_tracker.py` & `vectice-24.2.2.0/src/vectice/models/model_exp_tracker.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/model_mlflow.py` & `vectice-24.2.2.0/src/vectice/models/model_mlflow.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/phase.py` & `vectice-24.2.2.0/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/project.py` & `vectice-24.2.2.0/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/property.py` & `vectice-24.2.2.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/representation/dataset_representation.py` & `vectice-24.2.2.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/representation/dataset_version_representation.py` & `vectice-24.2.2.0/src/vectice/models/representation/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/representation/model_representation.py` & `vectice-24.2.2.0/src/vectice/models/representation/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/representation/model_version_representation.py` & `vectice-24.2.2.0/src/vectice/models/representation/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/__init__.py` & `vectice-24.2.2.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/base.py` & `vectice-24.2.2.0/src/vectice/models/resource/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/bigquery_resource.py` & `vectice-24.2.2.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/databricks_table_resource.py` & `vectice-24.2.2.0/src/vectice/models/resource/databricks_table_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/description.py` & `vectice-24.2.2.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/file_resource.py` & `vectice-24.2.2.0/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/gcs_resource.py` & `vectice-24.2.2.0/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/__init__.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/base.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/dataframe_config.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/dataframe_config.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pandas_default.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_pyspark_pandas.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_resource.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/df_wrapper_spark_df.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/metadata/source.py` & `vectice-24.2.2.0/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/no_resource.py` & `vectice-24.2.2.0/src/vectice/models/resource/no_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/s3_resource.py` & `vectice-24.2.2.0/src/vectice/models/resource/s3_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/resource/snowflake_resource.py` & `vectice-24.2.2.0/src/vectice/models/resource/snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/table.py` & `vectice-24.2.2.0/src/vectice/models/table.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/models/workspace.py` & `vectice-24.2.2.0/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/services/iteration_service.py` & `vectice-24.2.2.0/src/vectice/services/iteration_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/services/phase_service.py` & `vectice-24.2.2.0/src/vectice/services/phase_service.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/types/version.py` & `vectice-24.2.2.0/src/vectice/types/version.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/utils/code_parser.py` & `vectice-24.2.2.0/src/vectice/utils/code_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,28 +3,32 @@
 import ast
 import re
 from collections import OrderedDict
 from typing import Any
 
 
 class VariableVisitor(ast.NodeVisitor):
-    def __init__(self):
+    def __init__(self, model_metrics: bool = False):
         self.variables: OrderedDict[str, None] = OrderedDict()
         self.processed_variables: set[str] = set()
         self.function_call_args: set[str] = set()
         self.function_call_kwargs: set[str] = set()
         self.variable_calls: set[str] = set()
         self.vectice_call_vars: set[str] = set()
+        self.metric_variables: set[str] = set()
+        self.model_metrics = model_metrics
 
     ##### Implement NodeVisitor methods
 
     def visit_Assign(self, node: ast.Assign) -> None:  # noqa: N802
         for target in node.targets:
             self._extract_variables_from_target(target)
         self.generic_visit(node)
+        if self.model_metrics:
+            self._extract_metric_vars(node)
 
     def visit_Name(self, node: ast.Name) -> None:  # noqa: N802
         var_name = node.id
         # get functions args and kwargs
         args_kwargs = self.function_call_args.union(self.function_call_kwargs)
         all_processed_vars = self.processed_variables.union(self.variable_calls)
         if var_name not in all_processed_vars and var_name not in args_kwargs:
@@ -69,14 +73,34 @@
         if isinstance(target, ast.Name):
             self.visit_Name(target)
         elif isinstance(target, ast.Tuple):
             for element in target.elts:
                 if isinstance(element, ast.Name):
                     self.visit_Name(element)
 
+    def _add_metric_variables(self, metric_variable: str, node: ast.Assign) -> None:
+        try:
+            function_call_name = node.value.func.id  # pyright: ignore[reportAttributeAccessIssue]
+        except Exception:
+            function_call_name = None
+
+        is_metric_call = self._is_metric_call_vars(function_call_name) if function_call_name else False
+
+        if is_metric_call:
+            self.metric_variables.add(metric_variable)
+
+    def _extract_metric_vars(self, node: ast.Assign) -> None:
+        # Get the variable
+        for target in node.targets:
+            metric_variable = None
+            if isinstance(target, ast.Name):
+                metric_variable = target.id
+            if metric_variable:
+                self._add_metric_variables(metric_variable, node)
+
     def _get_arg_or_kwarg_val(self, arg: Any) -> Any | None:
         try:
             # arg value
             return arg.id
         except AttributeError:
             pass
         try:
@@ -108,14 +132,29 @@
             "BigQueryResource",
             "DatabricksTableResource",
         ]
         if func_name in vectice_functions:
             return True
         return False
 
+    def _is_metric_call_vars(self, func_name: str) -> bool:
+        from sklearn.metrics import (
+            _classification,  # pyright: ignore[reportPrivateUsage]
+            _ranking,  # pyright: ignore[reportPrivateUsage]
+            _regression,  # pyright: ignore[reportPrivateUsage]
+            _scorer,  # pyright: ignore[reportPrivateUsage]
+            cluster,  # pyright: ignore[reportPrivateUsage]
+        )
+
+        all_metrics = dir(_ranking) + dir(_scorer) + dir(cluster) + dir(_regression) + dir(_classification)
+
+        if func_name in all_metrics:
+            return True
+        return False
+
 
 def parse_comments(code: str) -> list[dict]:
     # Get all comments and variables
     comments_and_variables = r"##\s*(.*?)(?:$|\n)|(.+?)\s*=\s*.*?(?:$|\n)"
     all_comments_and_variables = []
     for idx, match in enumerate(re.findall(comments_and_variables, code)):
         comment, variable = match
```

### Comparing `vectice-24.2.1.0/src/vectice/utils/common_utils.py` & `vectice-24.2.2.0/src/vectice/utils/common_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,36 +7,33 @@
 import re
 from contextlib import contextmanager
 from enum import Enum
 from io import BufferedReader, BytesIO, IOBase
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Union
 
-from gql.transport.exceptions import TransportQueryError
 from PIL import Image, ImageFile
 from rich.console import Console
 from rich.table import Table
 
 from vectice.api.http_error_handlers import VecticeException
 from vectice.api.json.iteration import IterationStatus
 from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput
-from vectice.api.json.step import StepOutput, StepType
 from vectice.models.attachment_container import AttachmentContainer
 from vectice.models.metric import Metric
 from vectice.models.property import Property
 
 if TYPE_CHECKING:
     from vectice.api.client import Client
     from vectice.api.json import AttachmentOutput
     from vectice.api.json.dataset_version import DatasetVersionOutput
     from vectice.api.json.model_version import ModelVersionOutput
     from vectice.models.dataset import Dataset
     from vectice.models.iteration import Iteration
     from vectice.models.model import Model
-    from vectice.models.step import Step
 
 
 @contextmanager
 def hide_logs(package: str):
     old_level = logging.getLogger(package).level
     try:
         logging.getLogger(package).setLevel(logging.ERROR)
@@ -61,74 +58,14 @@
     if refresh_iteration._status in {  # pyright: ignore[reportPrivateUsage]
         IterationStatus.Completed,
         IterationStatus.Abandoned,
     }:
         raise RuntimeError(f"The Iteration is {refresh_iteration.status} and is read-only.")
 
 
-def get_step_type(
-    step_output: StepOutput,
-    iteration: Iteration,
-) -> Step:
-    # TODO: cyclic imports
-    from vectice.models.step import Step
-    from vectice.models.step_dataset import StepDataset
-    from vectice.models.step_image import StepImage
-    from vectice.models.step_model import StepModel
-    from vectice.models.step_number import StepNumber
-    from vectice.models.step_string import StepString
-
-    artifacts = step_output.artifacts
-    step = Step(
-        id=step_output.id,
-        iteration=iteration,
-        name=step_output.name,
-        index=step_output.index,
-        slug=step_output.slug,
-        description=step_output.description,
-        artifacts=artifacts,
-        step_type=StepType.Step,
-    )
-
-    def _get_number(text: int | float | str):
-        try:
-            return float(text)
-        except ValueError:
-            return text
-
-    if (
-        artifacts is not None  # pyright: ignore[reportUnnecessaryIsInstance, reportUnnecessaryComparison]
-        and len(artifacts) >= 1  # pyright: ignore[reportUnnecessaryIsInstance, reportUnnecessaryComparison]
-    ):
-        artifact = artifacts[len(artifacts) - 1]
-        if artifact.dataset_version_id is not None:
-            return StepDataset(step, artifact)
-        if artifact.model_version_id is not None:
-            return StepModel(step, artifact)
-        if artifact.entity_file_id:
-            image = _get_image_info(iteration, artifact.entity_file_id)
-            return step if image is None else StepImage(step, image)
-        if artifact.text:
-            str_or_float = _get_number(artifact.text)
-            return (
-                StepNumber(step, str_or_float)
-                if isinstance(str_or_float, float)
-                else StepString(step, str(str_or_float))
-            )
-    return step
-
-
-def _get_image_info(iteration: Iteration, entity_file_id: int):
-    try:
-        image = iteration._client.get_entity_file_by_id(entity_file_id)  # pyright: ignore[reportPrivateUsage]
-        return image.file_name
-    except TransportQueryError:
-        return None
-
-
 def check_image_path(path: str) -> bool:
     if _check_for_comment(path):
         return False
     try:
         check_path = Path(path).exists()
     except OSError:
         return False
```

### Comparing `vectice-24.2.1.0/src/vectice/utils/configuration.py` & `vectice-24.2.2.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/utils/deprecation.py` & `vectice-24.2.2.0/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/utils/instance_helper.py` & `vectice-24.2.2.0/src/vectice/utils/instance_helper.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/utils/last_assets.py` & `vectice-24.2.2.0/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice/utils/logging_utils.py` & `vectice-24.2.2.0/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-24.2.1.0/src/vectice.egg-info/PKG-INFO` & `vectice-24.2.2.0/src/vectice.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 24.2.1.0
+Version: 24.2.2.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
@@ -88,21 +88,25 @@
 Requires-Dist: tensorflow; extra == "test"
 Requires-Dist: keras; extra == "test"
 Requires-Dist: snowflake-snowpark-python; extra == "test"
 Requires-Dist: seaborn; extra == "test"
 Requires-Dist: xgboost; extra == "test"
 Requires-Dist: kaleido; extra == "test"
 Requires-Dist: catboost; extra == "test"
+Requires-Dist: torch; extra == "test"
 Provides-Extra: gcs
 Requires-Dist: google-cloud-storage>=1.17.0; extra == "gcs"
 Requires-Dist: google-cloud-bigquery; extra == "gcs"
 Provides-Extra: s3
 Requires-Dist: boto3; extra == "s3"
 Provides-Extra: autolog
 Requires-Dist: IPython; extra == "autolog"
-Requires-Dist: plotly; extra == "autolog"
+Provides-Extra: validation
+Requires-Dist: shap; extra == "validation"
+Requires-Dist: scipy; extra == "validation"
+Requires-Dist: pandas; extra == "validation"
 
 Auto-documentation for ML projects & their governance. View https://github.com/vectice/GettingStarted to get started.
 
 # Documentation
 
 Official documentation for Vectice can be found at https://docs.vectice.com.
```

### Comparing `vectice-24.2.1.0/src/vectice.egg-info/SOURCES.txt` & `vectice-24.2.2.0/src/vectice.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 src/vectice/api/http_error.py
 src/vectice/api/http_error_handlers.py
 src/vectice/api/iteration.py
 src/vectice/api/json_object.py
 src/vectice/api/phase.py
 src/vectice/api/project.py
 src/vectice/api/rest_api.py
-src/vectice/api/step.py
 src/vectice/api/version.py
 src/vectice/api/workspace.py
 src/vectice/api/json/__init__.py
 src/vectice/api/json/artifact_version.py
 src/vectice/api/json/attachment.py
 src/vectice/api/json/code.py
 src/vectice/api/json/code_version.py
@@ -62,29 +61,31 @@
 src/vectice/api/json/organization_config.py
 src/vectice/api/json/page.py
 src/vectice/api/json/paged_response.py
 src/vectice/api/json/phase.py
 src/vectice/api/json/project.py
 src/vectice/api/json/property.py
 src/vectice/api/json/public_config.py
-src/vectice/api/json/step.py
+src/vectice/api/json/requirement.py
+src/vectice/api/json/section.py
 src/vectice/api/json/user_and_workspace.py
 src/vectice/api/json/workspace.py
 src/vectice/autolog/__init__.py
 src/vectice/autolog/autolog.py
 src/vectice/autolog/autolog_asset_factory.py
 src/vectice/autolog/autolog_class.py
 src/vectice/autolog/model_library.py
 src/vectice/autolog/asset_services/__init__.py
 src/vectice/autolog/asset_services/catboost_service.py
 src/vectice/autolog/asset_services/keras_service.py
 src/vectice/autolog/asset_services/lightgbm_service.py
 src/vectice/autolog/asset_services/metric_service.py
 src/vectice/autolog/asset_services/pandas_service.py
 src/vectice/autolog/asset_services/pyspark_service.py
+src/vectice/autolog/asset_services/pytorch_service.py
 src/vectice/autolog/asset_services/sklearn_service.py
 src/vectice/autolog/asset_services/vectice_asset_service.py
 src/vectice/models/__init__.py
 src/vectice/models/additional_info.py
 src/vectice/models/attachment_container.py
 src/vectice/models/code_version.py
 src/vectice/models/dataset.py
@@ -93,21 +94,16 @@
 src/vectice/models/metric.py
 src/vectice/models/model.py
 src/vectice/models/model_exp_tracker.py
 src/vectice/models/model_mlflow.py
 src/vectice/models/phase.py
 src/vectice/models/project.py
 src/vectice/models/property.py
-src/vectice/models/step.py
-src/vectice/models/step_dataset.py
-src/vectice/models/step_image.py
-src/vectice/models/step_model.py
-src/vectice/models/step_number.py
-src/vectice/models/step_string.py
 src/vectice/models/table.py
+src/vectice/models/validation.py
 src/vectice/models/workspace.py
 src/vectice/models/representation/__init__.py
 src/vectice/models/representation/dataset_representation.py
 src/vectice/models/representation/dataset_version_representation.py
 src/vectice/models/representation/model_representation.py
 src/vectice/models/representation/model_version_representation.py
 src/vectice/models/resource/__init__.py
@@ -131,14 +127,15 @@
 src/vectice/models/resource/metadata/df_wrapper_resource.py
 src/vectice/models/resource/metadata/df_wrapper_spark_df.py
 src/vectice/models/resource/metadata/extra_metadata.py
 src/vectice/models/resource/metadata/files_metadata.py
 src/vectice/models/resource/metadata/pyspark_pandas_dataframe_typing.py
 src/vectice/models/resource/metadata/pyspark_typing.py
 src/vectice/models/resource/metadata/source.py
+src/vectice/models/test_library/binary_classification_test.py
 src/vectice/services/__init__.py
 src/vectice/services/iteration_service.py
 src/vectice/services/phase_service.py
 src/vectice/types/version.py
 src/vectice/utils/__init__.py
 src/vectice/utils/api_utils.py
 src/vectice/utils/code_parser.py
```

### Comparing `vectice-24.2.1.0/src/vectice.egg-info/requires.txt` & `vectice-24.2.2.0/src/vectice.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 Pillow
 pandas
 typing-extensions>=4.5.0
 dataclasses-json==0.5.8
 
 [autolog]
 IPython
-plotly
 
 [dev]
 black==24.2.0
 gitpython
 pyright==1.1.354
 ruff
 types-requests
@@ -70,7 +69,13 @@
 catboost
 tensorflow
 keras
 snowflake-snowpark-python
 seaborn
 xgboost
 kaleido
+torch
+
+[validation]
+shap
+scipy
+pandas
```

