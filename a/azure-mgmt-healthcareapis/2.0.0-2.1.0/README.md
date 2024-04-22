# Comparing `tmp/azure-mgmt-healthcareapis-2.0.0.tar.gz` & `tmp/azure-mgmt-healthcareapis-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-healthcareapis-2.0.0.tar", last modified: Wed Dec 20 02:48:58 2023, max compression
+gzip compressed data, was "azure-mgmt-healthcareapis-2.1.0.tar", last modified: Mon Apr 22 03:09:12 2024, max compression
```

## Comparing `azure-mgmt-healthcareapis-2.0.0.tar` & `azure-mgmt-healthcareapis-2.1.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:48:58.852185 azure-mgmt-healthcareapis-2.0.0/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6767 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      220 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     9917 2023-12-20 02:48:58.852185 azure-mgmt-healthcareapis-2.0.0/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2053 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      636 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:48:58.844185 azure-mgmt-healthcareapis-2.0.0/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:48:58.844185 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:48:58.844185 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      931 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3517 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8355 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/_healthcare_apis_management_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1530 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79289 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:48:58.848185 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      878 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3565 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8539 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/_healthcare_apis_management_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1530 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:48:58.848185 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2114 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39212 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_dicom_services_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6836 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_fhir_destinations_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39027 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_fhir_services_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24967 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_iot_connector_fhir_destination_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39240 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_iot_connectors_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4875 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_operation_results_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5851 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28555 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_private_endpoint_connections_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8137 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_private_link_resources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46727 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_services_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28719 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_workspace_private_endpoint_connections_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9827 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_workspace_private_link_resources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40600 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_workspaces_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:48:58.848185 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8428 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4167 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/models/_healthcare_apis_management_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   143872 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:48:58.852185 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2114 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47070 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_dicom_services_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8442 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_fhir_destinations_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46773 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_fhir_services_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30492 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_iot_connector_fhir_destination_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47098 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_iot_connectors_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6179 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_operation_results_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6548 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34889 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_private_endpoint_connections_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11112 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_private_link_resources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    55670 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_services_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35071 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_workspace_private_endpoint_connections_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12681 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_workspace_private_link_resources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48365 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_workspaces_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:48:58.852185 azure-mgmt-healthcareapis-2.0.0/azure_mgmt_healthcareapis.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     9917 2023-12-20 02:48:58.000000 azure-mgmt-healthcareapis-2.0.0/azure_mgmt_healthcareapis.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3302 2023-12-20 02:48:58.000000 azure-mgmt-healthcareapis-2.0.0/azure_mgmt_healthcareapis.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-12-20 02:48:58.000000 azure-mgmt-healthcareapis-2.0.0/azure_mgmt_healthcareapis.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-12-20 02:48:58.000000 azure-mgmt-healthcareapis-2.0.0/azure_mgmt_healthcareapis.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      124 2023-12-20 02:48:58.000000 azure-mgmt-healthcareapis-2.0.0/azure_mgmt_healthcareapis.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-12-20 02:48:58.000000 azure-mgmt-healthcareapis-2.0.0/azure_mgmt_healthcareapis.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-12-20 02:48:58.852185 azure-mgmt-healthcareapis-2.0.0/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2869 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:48:58.852185 azure-mgmt-healthcareapis-2.0.0/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3921 2023-12-20 02:48:17.000000 azure-mgmt-healthcareapis-2.0.0/tests/disable_test_cli_mgmt_healthcareapis.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:09:12.789788 azure-mgmt-healthcareapis-2.1.0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7036 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      220 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10006 2024-04-22 03:09:12.789788 azure-mgmt-healthcareapis-2.1.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2053 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      638 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:09:12.777788 azure-mgmt-healthcareapis-2.1.0/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:09:12.777788 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:09:12.777788 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      931 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3448 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9407 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/_healthcare_apis_management_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1530 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:09:12.777788 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      878 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3496 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9615 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/_healthcare_apis_management_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1530 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:09:12.781788 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2114 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32501 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_dicom_services_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6454 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_fhir_destinations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32327 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_fhir_services_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20898 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_iot_connector_fhir_destination_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32529 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_iot_connectors_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4611 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_operation_results_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5649 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24270 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7517 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39489 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_services_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24454 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_workspace_private_endpoint_connections_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9165 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_workspace_private_link_resources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33902 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_workspaces_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:09:12.781788 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8797 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4348 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/models/_healthcare_apis_management_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   150192 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:09:12.785788 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2114 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40429 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_dicom_services_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8060 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_fhir_destinations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40143 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_fhir_services_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26463 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_iot_connector_fhir_destination_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40457 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_iot_connectors_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5915 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_operation_results_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6346 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30644 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10492 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_private_link_resources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48502 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_services_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30846 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_workspace_private_endpoint_connections_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12019 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_workspace_private_link_resources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41737 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_workspaces_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:09:12.785788 azure-mgmt-healthcareapis-2.1.0/azure_mgmt_healthcareapis.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10006 2024-04-22 03:09:12.000000 azure-mgmt-healthcareapis-2.1.0/azure_mgmt_healthcareapis.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3302 2024-04-22 03:09:12.000000 azure-mgmt-healthcareapis-2.1.0/azure_mgmt_healthcareapis.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-22 03:09:12.000000 azure-mgmt-healthcareapis-2.1.0/azure_mgmt_healthcareapis.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-22 03:09:12.000000 azure-mgmt-healthcareapis-2.1.0/azure_mgmt_healthcareapis.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-04-22 03:09:12.000000 azure-mgmt-healthcareapis-2.1.0/azure_mgmt_healthcareapis.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-22 03:09:12.000000 azure-mgmt-healthcareapis-2.1.0/azure_mgmt_healthcareapis.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-22 03:09:12.789788 azure-mgmt-healthcareapis-2.1.0/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2796 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:09:12.789788 azure-mgmt-healthcareapis-2.1.0/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3921 2024-04-22 03:07:56.000000 azure-mgmt-healthcareapis-2.1.0/tests/disable_test_cli_mgmt_healthcareapis.py
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/CHANGELOG.md` & `azure-mgmt-healthcareapis-2.1.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Release History
 
+## 2.1.0 (2024-04-22)
+
+### Features Added
+
+  - Model DicomService has a new parameter enable_data_partitions
+  - Model DicomService has a new parameter storage_configuration
+  - Model FhirServiceAuthenticationConfiguration has a new parameter smart_identity_providers
+
 ## 2.0.0 (2023-12-18)
 
 ### Features Added
 
   - Model DicomService has a new parameter cors_configuration
   - Model DicomService has a new parameter encryption
   - Model DicomService has a new parameter event_state
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/LICENSE` & `azure-mgmt-healthcareapis-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/PKG-INFO` & `azure-mgmt-healthcareapis-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-healthcareapis
-Version: 2.0.0
+Version: 2.1.0
 Summary: Microsoft Azure Health Care Apis Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-common~=1.1
-Requires-Dist: azure-mgmt-core<2.0.0,>=1.3.2
-Requires-Dist: typing-extensions>=4.3.0; python_version < "3.8.0"
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Health Care Apis Management Client Library.
-This package has been tested with Python 3.7+.
+This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 ## Getting started
 
 ### Prerequisites
 
-- Python 3.7+ is required to use this package.
+- Python 3.8+ is required to use this package.
 - [Azure subscription](https://azure.microsoft.com/free/)
 
 ### Install the package
 
 ```bash
 pip install azure-mgmt-healthcareapis
 pip install azure-identity
@@ -86,14 +82,22 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.1.0 (2024-04-22)
+
+### Features Added
+
+  - Model DicomService has a new parameter enable_data_partitions
+  - Model DicomService has a new parameter storage_configuration
+  - Model FhirServiceAuthenticationConfiguration has a new parameter smart_identity_providers
+
 ## 2.0.0 (2023-12-18)
 
 ### Features Added
 
   - Model DicomService has a new parameter cors_configuration
   - Model DicomService has a new parameter encryption
   - Model DicomService has a new parameter event_state
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/README.md` & `azure-mgmt-healthcareapis-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Health Care Apis Management Client Library.
-This package has been tested with Python 3.7+.
+This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 ## Getting started
 
 ### Prerequisites
 
-- Python 3.7+ is required to use this package.
+- Python 3.8+ is required to use this package.
 - [Azure subscription](https://azure.microsoft.com/free/)
 
 ### Install the package
 
 ```bash
 pip install azure-mgmt-healthcareapis
 pip install azure-identity
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/_meta.json` & `azure-mgmt-healthcareapis-2.1.0/_meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'autorest_command'": "'autorest specification/healthcareapis/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 '*

 * *                       "--version=3.9.7 --version-tolerant=False'",*

 * * "'commit'": "'0e1d8ac4d5ca8a76479870db0a04aebe4fc3eab0'",*

 * * "'use'": " […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.7",
-    "autorest_command": "autorest specification/healthcareapis/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.7.1 --use=@autorest/modelerfour@4.26.2 --version=3.9.7 --version-tolerant=False",
-    "commit": "583e15ceb4cf23dc23b2300bd352f16d781e69ac",
+    "autorest_command": "autorest specification/healthcareapis/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 --version=3.9.7 --version-tolerant=False",
+    "commit": "0e1d8ac4d5ca8a76479870db0a04aebe4fc3eab0",
     "readme": "specification/healthcareapis/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.7.1",
-        "@autorest/modelerfour@4.26.2"
+        "@autorest/python@6.13.7",
+        "@autorest/modelerfour@4.27.0"
     ]
 }
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/__init__.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/_configuration.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,63 +4,62 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
-from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
 from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
-class HealthcareApisManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class HealthcareApisManagementClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for HealthcareApisManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-11-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-03-31". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(HealthcareApisManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-11-01")
+        api_version: str = kwargs.pop("api_version", "2024-03-31")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-healthcareapis/{}".format(VERSION))
+        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
         self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
             self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/_healthcare_apis_management_client.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/_healthcare_apis_management_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
+from azure.core.pipeline import policies
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
+from azure.mgmt.core.policies import ARMAutoResourceProviderRegistrationPolicy
 
 from . import models as _models
 from ._configuration import HealthcareApisManagementClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
     DicomServicesOperations,
     FhirDestinationsOperations,
@@ -73,15 +75,15 @@
     :vartype operation_results: azure.mgmt.healthcareapis.operations.OperationResultsOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-11-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-03-31". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -90,15 +92,33 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = HealthcareApisManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        _policies = kwargs.pop("policies", None)
+        if _policies is None:
+            _policies = [
+                policies.RequestIdPolicy(**kwargs),
+                self._config.headers_policy,
+                self._config.user_agent_policy,
+                self._config.proxy_policy,
+                policies.ContentDecodePolicy(**kwargs),
+                ARMAutoResourceProviderRegistrationPolicy(),
+                self._config.redirect_policy,
+                self._config.retry_policy,
+                self._config.authentication_policy,
+                self._config.custom_hook_policy,
+                self._config.logging_policy,
+                policies.DistributedTracingPolicy(**kwargs),
+                policies.SensitiveHeaderCleanupPolicy(**kwargs) if self._config.redirect_policy else None,
+                self._config.http_logging_policy,
+            ]
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.services = ServicesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.private_endpoint_connections = PrivateEndpointConnectionsOperations(
@@ -124,15 +144,15 @@
             self._client, self._config, self._serialize, self._deserialize
         )
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.operation_results = OperationResultsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
+    def _send_request(self, request: HttpRequest, *, stream: bool = False, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = client._send_request(request)
         <HttpResponse: 200 OK>
@@ -144,15 +164,15 @@
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
-        return self._client.send_request(request_copy, **kwargs)
+        return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
 
     def close(self) -> None:
         self._client.close()
 
     def __enter__(self) -> "HealthcareApisManagementClient":
         self._client.__enter__()
         return self
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/_patch.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/_serialization.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
-from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
-from azure.core.serialization import NULL as AzureCoreNull
+from azure.core.exceptions import DeserializationError, SerializationError
+from azure.core.serialization import NULL as CoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
 ModelType = TypeVar("ModelType", bound="Model")
 JSON = MutableMapping[str, Any]
 
 
@@ -120,15 +120,15 @@
                     if isinstance(data, unicode):  # type: ignore
                         # If I'm Python 2.7 and unicode XML will scream if I try a "fromstring" on unicode string
                         data_as_str = data_as_str.encode(encoding="utf-8")  # type: ignore
                 except NameError:
                     pass
 
                 return ET.fromstring(data_as_str)  # nosec
-            except ET.ParseError:
+            except ET.ParseError as err:
                 # It might be because the server has an issue, and returned JSON with
                 # content-type XML....
                 # So let's try a JSON load, and if it's still broken
                 # let's flow the initial exception
                 def _json_attemp(data):
                     try:
                         return True, json.loads(data)
@@ -139,15 +139,15 @@
                 if success:
                     return json_result
                 # If i'm here, it's not JSON, it's not XML, let's scream
                 # and raise the last context in this block (the XML exception)
                 # The function hack is because Py2.7 messes up with exception
                 # context otherwise.
                 _LOGGER.critical("Wasn't XML not JSON, failing")
-                raise_with_traceback(DeserializationError, "XML is invalid")
+                raise DeserializationError("XML is invalid") from err
         raise DeserializationError("Cannot deserialize content-type: {}".format(content_type))
 
     @classmethod
     def deserialize_from_http_generics(cls, body_bytes: Optional[Union[AnyStr, IO]], headers: Mapping) -> Any:
         """Deserialize from HTTP response.
 
         Use bytes and headers to NOT use any requests/aiohttp or whatever
@@ -166,21 +166,14 @@
             content_type = "application/json"
 
         if body_bytes:
             return cls.deserialize_from_text(body_bytes, content_type)
         return None
 
 
-try:
-    basestring  # type: ignore
-    unicode_str = unicode  # type: ignore
-except NameError:
-    basestring = str
-    unicode_str = str
-
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
 
@@ -291,15 +284,15 @@
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
     def __init__(self, **kwargs: Any) -> None:
-        self.additional_properties: Dict[str, Any] = {}
+        self.additional_properties: Optional[Dict[str, Any]] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
@@ -336,26 +329,26 @@
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
     def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
-        """Return the JSON that would be sent to azure from this model.
+        """Return the JSON that would be sent to server from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
+        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)  # type: ignore
 
     def as_dict(
         self,
         keep_readonly: bool = True,
         key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
         **kwargs: Any
     ) -> JSON:
@@ -386,15 +379,15 @@
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param function key_transformer: A key transformer function.
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)
+        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)  # type: ignore
 
     @classmethod
     def _infer_class_models(cls):
         try:
             str_models = cls.__module__.rsplit(".", 1)[0]
             models = sys.modules[str_models]
             client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
@@ -411,15 +404,15 @@
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        return deserializer(cls.__name__, data, content_type=content_type)
+        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
 
     @classmethod
     def from_dict(
         cls: Type[ModelType],
         data: Any,
         key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
         content_type: Optional[str] = None,
@@ -441,15 +434,15 @@
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
-        return deserializer(cls.__name__, data, content_type=content_type)
+        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
 
     @classmethod
     def _flatten_subtype(cls, key, objects):
         if "_subtype_map" not in cls.__dict__:
             return {}
         result = dict(cls._subtype_map[key])
         for valuetype in cls._subtype_map[key].values():
@@ -541,15 +534,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -557,15 +550,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -645,15 +638,15 @@
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
                             serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
-                            local_node.text = unicode_str(new_attr)
+                            local_node.text = str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
                             new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
@@ -664,15 +657,15 @@
                             _serialized = _serialized[k]
                 except ValueError as err:
                     if isinstance(err, SerializationError):
                         raise
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
-            raise_with_traceback(SerializationError, msg, err)
+            raise SerializationError(msg) from err
         else:
             return serialized
 
     def body(self, data, data_type, **kwargs):
         """Serialize data intended for a request body.
 
         :param data: The data to be serialized.
@@ -706,15 +699,15 @@
                     deserializer.key_extractors = [
                         rest_key_case_insensitive_extractor,
                         attribute_key_case_insensitive_extractor,
                         last_rest_key_case_insensitive_extractor,
                     ]
                 data = deserializer._deserialize(data_type, data)
             except DeserializationError as err:
-                raise_with_traceback(SerializationError, "Unable to build a model: " + str(err), err)
+                raise SerializationError("Unable to build a model: " + str(err)) from err
 
         return self._serialize(data, data_type, **kwargs)
 
     def url(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL path.
 
         :param data: The data to be serialized.
@@ -726,38 +719,39 @@
         try:
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
 
             if kwargs.get("skip_quote") is True:
                 output = str(output)
+                output = output.replace("{", quote("{")).replace("}", quote("}"))
             else:
                 output = quote(str(output), safe="")
         except SerializationError:
             raise TypeError("{} must be type {}.".format(name, data_type))
         else:
             return output
 
     def query(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL query.
 
         :param data: The data to be serialized.
         :param str data_type: The type to be serialized from.
         :keyword bool skip_quote: Whether to skip quote the serialized result.
         Defaults to False.
-        :rtype: str
+        :rtype: str, list
         :raises: TypeError if serialization fails.
         :raises: ValueError if data is None
         """
         try:
             # Treat the list aside, since we don't want to encode the div separator
             if data_type.startswith("["):
                 internal_data_type = data_type[1:-1]
                 do_quote = not kwargs.get("skip_quote", False)
-                return str(self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs))
+                return self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs)
 
             # Not a list, regular serialization
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
             if kwargs.get("skip_quote") is True:
                 output = str(output)
@@ -800,15 +794,15 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
-            if data is AzureCoreNull:
+            if data is CoreNull:
                 return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
@@ -820,15 +814,15 @@
 
             iter_type = data_type[0] + data_type[-1]
             if iter_type in self.serialize_type:
                 return self.serialize_type[iter_type](data, data_type[1:-1], **kwargs)
 
         except (ValueError, TypeError) as err:
             msg = "Unable to serialize value: {!r} as type: {!r}."
-            raise_with_traceback(SerializationError, msg.format(data, data_type), err)
+            raise SerializationError(msg.format(data, data_type)) from err
         else:
             return self._serialize(data, **kwargs)
 
     @classmethod
     def _get_custom_serializers(cls, data_type, **kwargs):
         custom_serializer = kwargs.get("basic_types_serializers", {}).get(data_type)
         if custom_serializer:
@@ -989,15 +983,15 @@
         if isinstance(attr, ET.Element):
             return attr
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.serialize_basic(attr, self.basic_types[obj_type], **kwargs)
         if obj_type is _long_type:
             return self.serialize_long(attr)
-        if obj_type is unicode_str:
+        if obj_type is str:
             return self.serialize_unicode(attr)
         if obj_type is datetime.datetime:
             return self.serialize_iso(attr)
         if obj_type is datetime.date:
             return self.serialize_date(attr)
         if obj_type is datetime.time:
             return self.serialize_time(attr)
@@ -1166,18 +1160,18 @@
                 microseconds = "." + microseconds
             date = "{:04}-{:02}-{:02}T{:02}:{:02}:{:02}".format(
                 utc.tm_year, utc.tm_mon, utc.tm_mday, utc.tm_hour, utc.tm_min, utc.tm_sec
             )
             return date + microseconds + "Z"
         except (ValueError, OverflowError) as err:
             msg = "Unable to serialize datetime object."
-            raise_with_traceback(SerializationError, msg, err)
+            raise SerializationError(msg) from err
         except AttributeError as err:
             msg = "ISO-8601 object must be valid Datetime object."
-            raise_with_traceback(TypeError, msg, err)
+            raise TypeError(msg) from err
 
     @staticmethod
     def serialize_unix(attr, **kwargs):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
 
         :param Datetime attr: Object to be serialized.
@@ -1205,15 +1199,14 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
-            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     return working_data.get(key)
 
 
 def rest_key_case_insensitive_extractor(attr, attr_desc, data):
@@ -1226,15 +1219,14 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = attribute_key_case_insensitive_extractor(working_key, None, working_data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
-            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     if working_data:
         return attribute_key_case_insensitive_extractor(key, None, working_data)
 
 
@@ -1367,15 +1359,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1387,15 +1379,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1440,15 +1432,15 @@
                     setattr(data, attr, self._deserialize(local_type, value))
                 return data
             except AttributeError:
                 return
 
         response, class_name = self._classify_target(target_obj, data)
 
-        if isinstance(response, basestring):
+        if isinstance(response, str):
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
@@ -1477,15 +1469,15 @@
                             continue
                         raw_value = found_value
 
                 value = self.deserialize_data(raw_value, attr_desc["type"])
                 d_attrs[attr] = value
         except (AttributeError, TypeError, KeyError) as err:
             msg = "Unable to deserialize to object: " + class_name  # type: ignore
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             additional_properties = self._build_additional_properties(attributes, data)
             return self._instantiate_model(response, d_attrs, additional_properties)
 
     def _build_additional_properties(self, attribute_map, data):
         if not self.additional_properties_detection:
             return None
@@ -1511,22 +1503,22 @@
 
         :param str target: The target object type to deserialize to.
         :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
-        if isinstance(target, basestring):
+        if isinstance(target, str):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
-            target = target._classify(data, self.dependencies)
+            target = target._classify(data, self.dependencies)  # type: ignore
         except AttributeError:
             pass  # Target is not a Model, no classify
         return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
@@ -1574,15 +1566,15 @@
         if hasattr(raw_data, "body"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
-        if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
+        if isinstance(raw_data, (str, bytes)) or hasattr(raw_data, "read"):
             return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
@@ -1648,15 +1640,15 @@
                 if isinstance(data, ET.Element):
                     data = data.text
                 return self.deserialize_enum(data, obj_type)
 
         except (ValueError, TypeError, AttributeError) as err:
             msg = "Unable to deserialize response data."
             msg += " Data: {}, {}".format(data, data_type)
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return self._deserialize(obj_type, data)
 
     def deserialize_iter(self, attr, iter_type):
         """Deserialize an iterable.
 
         :param list attr: Iterable to be deserialized.
@@ -1696,15 +1688,15 @@
         :raises: TypeError if non-builtin datatype encountered.
         """
         if attr is None:
             return None
         if isinstance(attr, ET.Element):
             # Do no recurse on XML, just return the tree as-is
             return attr
-        if isinstance(attr, basestring):
+        if isinstance(attr, str):
             return self.deserialize_basic(attr, "str")
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.deserialize_basic(attr, self.basic_types[obj_type])
         if obj_type is _long_type:
             return self.deserialize_long(attr)
 
@@ -1753,15 +1745,15 @@
                     # None or '', node <a/> with a strong type is None.
                     # Don't try to model "empty bool" or "empty int"
                     return None
 
         if data_type == "bool":
             if attr in [True, False, 1, 0]:
                 return bool(attr)
-            elif isinstance(attr, basestring):
+            elif isinstance(attr, str):
                 if attr.lower() in ["true", "1"]:
                     return True
                 elif attr.lower() in ["false", "0"]:
                     return False
             raise TypeError("Invalid boolean value: {}".format(attr))
 
         if data_type == "str":
@@ -1804,15 +1796,14 @@
         """
         if isinstance(data, enum_obj) or data is None:
             return data
         if isinstance(data, Enum):
             data = data.value
         if isinstance(data, int):
             # Workaround. We might consider remove it in the future.
-            # https://github.com/Azure/azure-rest-api-specs/issues/141
             try:
                 return list(enum_obj.__members__.values())[data]
             except IndexError:
                 error = "{!r} is not a valid index for enum {!r}"
                 raise DeserializationError(error.format(data, enum_obj))
         try:
             return enum_obj(str(data))
@@ -1858,18 +1849,18 @@
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)  # type: ignore
+            return decimal.Decimal(str(attr))  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
 
         :param str attr: response string to be deserialized.
         :rtype: long or int
@@ -1889,15 +1880,15 @@
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
             duration = isodate.parse_duration(attr)
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize duration object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return duration
 
     @staticmethod
     def deserialize_date(attr):
         """Deserialize ISO-8601 formatted string into Date object.
 
@@ -1906,15 +1897,15 @@
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         # This must NOT use defaultmonth/defaultday. Using None ensure this raises an exception.
-        return isodate.parse_date(attr, defaultmonth=None, defaultday=None)
+        return isodate.parse_date(attr, defaultmonth=0, defaultday=0)
 
     @staticmethod
     def deserialize_time(attr):
         """Deserialize ISO-8601 formatted string into time object.
 
         :param str attr: response string to be deserialized.
         :rtype: datetime.time
@@ -1941,15 +1932,15 @@
             date_obj = datetime.datetime(
                 *parsed_date[:6], tzinfo=_FixedOffset(datetime.timedelta(minutes=(parsed_date[9] or 0) / 60))
             )
             if not date_obj.tzinfo:
                 date_obj = date_obj.astimezone(tz=TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to rfc datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
 
     @staticmethod
     def deserialize_iso(attr):
         """Deserialize ISO-8601 formatted string into Datetime object.
 
@@ -1978,15 +1969,15 @@
 
             date_obj = isodate.parse_datetime(attr)
             test_utc = date_obj.utctimetuple()
             if test_utc.tm_year > 9999 or test_utc.tm_year < 1:
                 raise OverflowError("Hit max or min date")
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
 
     @staticmethod
     def deserialize_unix(attr):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
@@ -1994,13 +1985,14 @@
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
             attr = int(attr.text)  # type: ignore
         try:
+            attr = int(attr)
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/_vendor.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/__init__.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/_configuration.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,63 +4,62 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
-from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
 from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class HealthcareApisManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class HealthcareApisManagementClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for HealthcareApisManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-11-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-03-31". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(HealthcareApisManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-11-01")
+        api_version: str = kwargs.pop("api_version", "2024-03-31")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-healthcareapis/{}".format(VERSION))
+        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
         self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
             self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/_healthcare_apis_management_client.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/_healthcare_apis_management_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
+from azure.core.pipeline import policies
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
+from azure.mgmt.core.policies import AsyncARMAutoResourceProviderRegistrationPolicy
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import HealthcareApisManagementClientConfiguration
 from .operations import (
     DicomServicesOperations,
     FhirDestinationsOperations,
@@ -73,15 +75,15 @@
     :vartype operation_results: azure.mgmt.healthcareapis.aio.operations.OperationResultsOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-11-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-03-31". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -90,15 +92,33 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = HealthcareApisManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        _policies = kwargs.pop("policies", None)
+        if _policies is None:
+            _policies = [
+                policies.RequestIdPolicy(**kwargs),
+                self._config.headers_policy,
+                self._config.user_agent_policy,
+                self._config.proxy_policy,
+                policies.ContentDecodePolicy(**kwargs),
+                AsyncARMAutoResourceProviderRegistrationPolicy(),
+                self._config.redirect_policy,
+                self._config.retry_policy,
+                self._config.authentication_policy,
+                self._config.custom_hook_policy,
+                self._config.logging_policy,
+                policies.DistributedTracingPolicy(**kwargs),
+                policies.SensitiveHeaderCleanupPolicy(**kwargs) if self._config.redirect_policy else None,
+                self._config.http_logging_policy,
+            ]
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.services = ServicesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.private_endpoint_connections = PrivateEndpointConnectionsOperations(
@@ -124,15 +144,17 @@
             self._client, self._config, self._serialize, self._deserialize
         )
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.operation_results = OperationResultsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
+    def _send_request(
+        self, request: HttpRequest, *, stream: bool = False, **kwargs: Any
+    ) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = await client._send_request(request)
         <AsyncHttpResponse: 200 OK>
@@ -144,15 +166,15 @@
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.AsyncHttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
-        return self._client.send_request(request_copy, **kwargs)
+        return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
 
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "HealthcareApisManagementClient":
         await self._client.__aenter__()
         return self
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/_patch.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/__init__.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_dicom_services_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_dicom_services_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -69,15 +69,14 @@
         """Lists all DICOM Services for the given workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DicomService or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.DicomService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -91,87 +90,81 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_workspace_request(
+                _request = build_list_by_workspace_request(
                     resource_group_name=resource_group_name,
                     workspace_name=workspace_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_workspace.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("DicomServiceCollection", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_workspace.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices"
-    }
-
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, workspace_name: str, dicom_service_name: str, **kwargs: Any
     ) -> _models.DicomService:
         """Gets the properties of the specified DICOM Service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param dicom_service_name: The name of DICOM Service resource. Required.
         :type dicom_service_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DicomService or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.DicomService
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -182,56 +175,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DicomService] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             dicom_service_name=dicom_service_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("DicomService", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
+        return deserialized  # type: ignore
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         workspace_name: str,
         dicom_service_name: str,
-        dicomservice: Union[_models.DicomService, IO],
+        dicomservice: Union[_models.DicomService, IO[bytes]],
         **kwargs: Any
     ) -> _models.DicomService:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -249,33 +237,32 @@
         _json = None
         _content = None
         if isinstance(dicomservice, (IOBase, bytes)):
             _content = dicomservice
         else:
             _json = self._serialize.body(dicomservice, "DicomService")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             dicom_service_name=dicom_service_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
@@ -291,18 +278,14 @@
             deserialized = self._deserialize("DicomService", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
-
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         dicom_service_name: str,
         dicomservice: _models.DicomService,
@@ -321,35 +304,27 @@
         :type dicom_service_name: str
         :param dicomservice: The parameters for creating or updating a Dicom Service resource.
          Required.
         :type dicomservice: ~azure.mgmt.healthcareapis.models.DicomService
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either DicomService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.DicomService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         dicom_service_name: str,
-        dicomservice: IO,
+        dicomservice: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.DicomService]:
         """Creates or updates a DICOM Service resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
@@ -357,64 +332,45 @@
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param dicom_service_name: The name of DICOM Service resource. Required.
         :type dicom_service_name: str
         :param dicomservice: The parameters for creating or updating a Dicom Service resource.
          Required.
-        :type dicomservice: IO
+        :type dicomservice: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either DicomService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.DicomService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         dicom_service_name: str,
-        dicomservice: Union[_models.DicomService, IO],
+        dicomservice: Union[_models.DicomService, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.DicomService]:
         """Creates or updates a DICOM Service resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param dicom_service_name: The name of DICOM Service resource. Required.
         :type dicom_service_name: str
         :param dicomservice: The parameters for creating or updating a Dicom Service resource. Is
-         either a DicomService type or a IO type. Required.
-        :type dicomservice: ~azure.mgmt.healthcareapis.models.DicomService or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         either a DicomService type or a IO[bytes] type. Required.
+        :type dicomservice: ~azure.mgmt.healthcareapis.models.DicomService or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either DicomService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.DicomService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -439,42 +395,40 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("DicomService", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.DicomService].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
+        return AsyncLROPoller[_models.DicomService](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _update_initial(
         self,
         resource_group_name: str,
         dicom_service_name: str,
         workspace_name: str,
-        dicomservice_patch_resource: Union[_models.DicomServicePatchResource, IO],
+        dicomservice_patch_resource: Union[_models.DicomServicePatchResource, IO[bytes]],
         **kwargs: Any
     ) -> _models.DicomService:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -492,33 +446,32 @@
         _json = None
         _content = None
         if isinstance(dicomservice_patch_resource, (IOBase, bytes)):
             _content = dicomservice_patch_resource
         else:
             _json = self._serialize.body(dicomservice_patch_resource, "DicomServicePatchResource")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             dicom_service_name=dicom_service_name,
             workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
@@ -531,18 +484,14 @@
             deserialized = self._deserialize("DicomService", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
-
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         dicom_service_name: str,
         workspace_name: str,
         dicomservice_patch_resource: _models.DicomServicePatchResource,
@@ -560,100 +509,73 @@
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param dicomservice_patch_resource: The parameters for updating a Dicom Service. Required.
         :type dicomservice_patch_resource: ~azure.mgmt.healthcareapis.models.DicomServicePatchResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either DicomService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.DicomService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         dicom_service_name: str,
         workspace_name: str,
-        dicomservice_patch_resource: IO,
+        dicomservice_patch_resource: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.DicomService]:
         """Patch DICOM Service details.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param dicom_service_name: The name of DICOM Service resource. Required.
         :type dicom_service_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param dicomservice_patch_resource: The parameters for updating a Dicom Service. Required.
-        :type dicomservice_patch_resource: IO
+        :type dicomservice_patch_resource: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either DicomService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.DicomService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_update(
         self,
         resource_group_name: str,
         dicom_service_name: str,
         workspace_name: str,
-        dicomservice_patch_resource: Union[_models.DicomServicePatchResource, IO],
+        dicomservice_patch_resource: Union[_models.DicomServicePatchResource, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.DicomService]:
         """Patch DICOM Service details.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param dicom_service_name: The name of DICOM Service resource. Required.
         :type dicom_service_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param dicomservice_patch_resource: The parameters for updating a Dicom Service. Is either a
-         DicomServicePatchResource type or a IO type. Required.
+         DicomServicePatchResource type or a IO[bytes] type. Required.
         :type dicomservice_patch_resource: ~azure.mgmt.healthcareapis.models.DicomServicePatchResource
-         or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either DicomService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.DicomService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -678,35 +600,33 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("DicomService", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.DicomService].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
+        return AsyncLROPoller[_models.DicomService](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, dicom_service_name: str, workspace_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -717,67 +637,54 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             dicom_service_name=dicom_service_name,
             workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, dicom_service_name: str, workspace_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Deletes a DICOM Service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param dicom_service_name: The name of DICOM Service resource. Required.
         :type dicom_service_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -797,27 +704,23 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_fhir_destinations_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_fhir_destinations_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -61,15 +61,14 @@
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either IotFhirDestination or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.IotFhirDestination]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -84,66 +83,61 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_iot_connector_request(
+                _request = build_list_by_iot_connector_request(
                     resource_group_name=resource_group_name,
                     workspace_name=workspace_name,
                     iot_connector_name=iot_connector_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_iot_connector.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("IotFhirDestinationCollection", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list_by_iot_connector.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations"
-    }
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_fhir_services_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_fhir_services_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -69,15 +69,14 @@
         """Lists all FHIR Services for the given workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either FhirService or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -91,87 +90,81 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_workspace_request(
+                _request = build_list_by_workspace_request(
                     resource_group_name=resource_group_name,
                     workspace_name=workspace_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_workspace.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("FhirServiceCollection", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_workspace.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices"
-    }
-
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, workspace_name: str, fhir_service_name: str, **kwargs: Any
     ) -> _models.FhirService:
         """Gets the properties of the specified FHIR Service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FhirService or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.FhirService
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -182,56 +175,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.FhirService] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             fhir_service_name=fhir_service_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("FhirService", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
+        return deserialized  # type: ignore
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         workspace_name: str,
         fhir_service_name: str,
-        fhirservice: Union[_models.FhirService, IO],
+        fhirservice: Union[_models.FhirService, IO[bytes]],
         **kwargs: Any
     ) -> _models.FhirService:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -249,33 +237,32 @@
         _json = None
         _content = None
         if isinstance(fhirservice, (IOBase, bytes)):
             _content = fhirservice
         else:
             _json = self._serialize.body(fhirservice, "FhirService")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             fhir_service_name=fhir_service_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
@@ -291,18 +278,14 @@
             deserialized = self._deserialize("FhirService", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
-
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         fhir_service_name: str,
         fhirservice: _models.FhirService,
@@ -320,99 +303,72 @@
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param fhirservice: The parameters for creating or updating a Fhir Service resource. Required.
         :type fhirservice: ~azure.mgmt.healthcareapis.models.FhirService
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         fhir_service_name: str,
-        fhirservice: IO,
+        fhirservice: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.FhirService]:
         """Creates or updates a FHIR Service resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param fhirservice: The parameters for creating or updating a Fhir Service resource. Required.
-        :type fhirservice: IO
+        :type fhirservice: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         fhir_service_name: str,
-        fhirservice: Union[_models.FhirService, IO],
+        fhirservice: Union[_models.FhirService, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.FhirService]:
         """Creates or updates a FHIR Service resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param fhirservice: The parameters for creating or updating a Fhir Service resource. Is either
-         a FhirService type or a IO type. Required.
-        :type fhirservice: ~azure.mgmt.healthcareapis.models.FhirService or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         a FhirService type or a IO[bytes] type. Required.
+        :type fhirservice: ~azure.mgmt.healthcareapis.models.FhirService or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -437,42 +393,40 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("FhirService", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.FhirService].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
+        return AsyncLROPoller[_models.FhirService](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _update_initial(
         self,
         resource_group_name: str,
         fhir_service_name: str,
         workspace_name: str,
-        fhirservice_patch_resource: Union[_models.FhirServicePatchResource, IO],
+        fhirservice_patch_resource: Union[_models.FhirServicePatchResource, IO[bytes]],
         **kwargs: Any
     ) -> _models.FhirService:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -490,33 +444,32 @@
         _json = None
         _content = None
         if isinstance(fhirservice_patch_resource, (IOBase, bytes)):
             _content = fhirservice_patch_resource
         else:
             _json = self._serialize.body(fhirservice_patch_resource, "FhirServicePatchResource")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             fhir_service_name=fhir_service_name,
             workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
@@ -529,18 +482,14 @@
             deserialized = self._deserialize("FhirService", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
-
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         fhir_service_name: str,
         workspace_name: str,
         fhirservice_patch_resource: _models.FhirServicePatchResource,
@@ -558,100 +507,73 @@
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhirservice_patch_resource: The parameters for updating a Fhir Service. Required.
         :type fhirservice_patch_resource: ~azure.mgmt.healthcareapis.models.FhirServicePatchResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         fhir_service_name: str,
         workspace_name: str,
-        fhirservice_patch_resource: IO,
+        fhirservice_patch_resource: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.FhirService]:
         """Patch FHIR Service details.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhirservice_patch_resource: The parameters for updating a Fhir Service. Required.
-        :type fhirservice_patch_resource: IO
+        :type fhirservice_patch_resource: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_update(
         self,
         resource_group_name: str,
         fhir_service_name: str,
         workspace_name: str,
-        fhirservice_patch_resource: Union[_models.FhirServicePatchResource, IO],
+        fhirservice_patch_resource: Union[_models.FhirServicePatchResource, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.FhirService]:
         """Patch FHIR Service details.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhirservice_patch_resource: The parameters for updating a Fhir Service. Is either a
-         FhirServicePatchResource type or a IO type. Required.
+         FhirServicePatchResource type or a IO[bytes] type. Required.
         :type fhirservice_patch_resource: ~azure.mgmt.healthcareapis.models.FhirServicePatchResource or
-         IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         IO[bytes]
         :return: An instance of AsyncLROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -676,35 +598,33 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("FhirService", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.FhirService].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
+        return AsyncLROPoller[_models.FhirService](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, fhir_service_name: str, workspace_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -715,67 +635,54 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             fhir_service_name=fhir_service_name,
             workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, fhir_service_name: str, workspace_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Deletes a FHIR Service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -795,27 +702,23 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_iot_connector_fhir_destination_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_iot_connector_fhir_destination_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -14,55 +14,189 @@
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
-from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._iot_connector_fhir_destination_operations import (
-    build_create_or_update_request,
-    build_delete_request,
-    build_get_request,
-)
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_get_request(
+    resource_group_name: str,
+    workspace_name: str,
+    iot_connector_name: str,
+    fhir_destination_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
+        "iotConnectorName": _SERIALIZER.url(
+            "iot_connector_name", iot_connector_name, "str", max_length=24, min_length=3
+        ),
+        "fhirDestinationName": _SERIALIZER.url(
+            "fhir_destination_name", fhir_destination_name, "str", max_length=24, min_length=3
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_create_or_update_request(
+    resource_group_name: str,
+    workspace_name: str,
+    iot_connector_name: str,
+    fhir_destination_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
+        "iotConnectorName": _SERIALIZER.url(
+            "iot_connector_name", iot_connector_name, "str", max_length=24, min_length=3
+        ),
+        "fhirDestinationName": _SERIALIZER.url(
+            "fhir_destination_name", fhir_destination_name, "str", max_length=24, min_length=3
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_delete_request(
+    resource_group_name: str,
+    workspace_name: str,
+    iot_connector_name: str,
+    fhir_destination_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
+        "iotConnectorName": _SERIALIZER.url(
+            "iot_connector_name", iot_connector_name, "str", max_length=24, min_length=3
+        ),
+        "fhirDestinationName": _SERIALIZER.url(
+            "fhir_destination_name", fhir_destination_name, "str", max_length=24, min_length=3
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class IotConnectorFhirDestinationOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.healthcareapis.aio.HealthcareApisManagementClient`'s
+        :class:`~azure.mgmt.healthcareapis.HealthcareApisManagementClient`'s
         :attr:`iot_connector_fhir_destination` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace_async
-    async def get(
+    @distributed_trace
+    def get(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
         fhir_destination_name: str,
         **kwargs: Any
     ) -> _models.IotFhirDestination:
@@ -73,15 +207,14 @@
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param fhir_destination_name: The name of IoT Connector FHIR destination resource. Required.
         :type fhir_destination_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: IotFhirDestination or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.IotFhirDestination
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -92,58 +225,53 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.IotFhirDestination] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             iot_connector_name=iot_connector_name,
             fhir_destination_name=fhir_destination_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("IotFhirDestination", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}"
-    }
+        return deserialized  # type: ignore
 
-    async def _create_or_update_initial(
+    def _create_or_update_initial(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
         fhir_destination_name: str,
-        iot_fhir_destination: Union[_models.IotFhirDestination, IO],
+        iot_fhir_destination: Union[_models.IotFhirDestination, IO[bytes]],
         **kwargs: Any
     ) -> _models.IotFhirDestination:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -161,34 +289,33 @@
         _json = None
         _content = None
         if isinstance(iot_fhir_destination, (IOBase, bytes)):
             _content = iot_fhir_destination
         else:
             _json = self._serialize.body(iot_fhir_destination, "IotFhirDestination")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             iot_connector_name=iot_connector_name,
             fhir_destination_name=fhir_destination_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
@@ -204,30 +331,26 @@
             deserialized = self._deserialize("IotFhirDestination", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}"
-    }
-
     @overload
-    async def begin_create_or_update(
+    def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
         fhir_destination_name: str,
         iot_fhir_destination: _models.IotFhirDestination,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.IotFhirDestination]:
+    ) -> LROPoller[_models.IotFhirDestination]:
         """Creates or updates an IoT Connector FHIR destination resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
@@ -237,125 +360,95 @@
         :type fhir_destination_name: str
         :param iot_fhir_destination: The parameters for creating or updating an IoT Connector FHIR
          destination resource. Required.
         :type iot_fhir_destination: ~azure.mgmt.healthcareapis.models.IotFhirDestination
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either IotFhirDestination or the result of
+        :return: An instance of LROPoller that returns either IotFhirDestination or the result of
          cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.IotFhirDestination]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotFhirDestination]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_create_or_update(
+    def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
         fhir_destination_name: str,
-        iot_fhir_destination: IO,
+        iot_fhir_destination: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.IotFhirDestination]:
+    ) -> LROPoller[_models.IotFhirDestination]:
         """Creates or updates an IoT Connector FHIR destination resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param fhir_destination_name: The name of IoT Connector FHIR destination resource. Required.
         :type fhir_destination_name: str
         :param iot_fhir_destination: The parameters for creating or updating an IoT Connector FHIR
          destination resource. Required.
-        :type iot_fhir_destination: IO
+        :type iot_fhir_destination: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either IotFhirDestination or the result of
+        :return: An instance of LROPoller that returns either IotFhirDestination or the result of
          cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.IotFhirDestination]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotFhirDestination]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def begin_create_or_update(
+    @distributed_trace
+    def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
         fhir_destination_name: str,
-        iot_fhir_destination: Union[_models.IotFhirDestination, IO],
+        iot_fhir_destination: Union[_models.IotFhirDestination, IO[bytes]],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.IotFhirDestination]:
+    ) -> LROPoller[_models.IotFhirDestination]:
         """Creates or updates an IoT Connector FHIR destination resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param fhir_destination_name: The name of IoT Connector FHIR destination resource. Required.
         :type fhir_destination_name: str
         :param iot_fhir_destination: The parameters for creating or updating an IoT Connector FHIR
-         destination resource. Is either a IotFhirDestination type or a IO type. Required.
-        :type iot_fhir_destination: ~azure.mgmt.healthcareapis.models.IotFhirDestination or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either IotFhirDestination or the result of
+         destination resource. Is either a IotFhirDestination type or a IO[bytes] type. Required.
+        :type iot_fhir_destination: ~azure.mgmt.healthcareapis.models.IotFhirDestination or IO[bytes]
+        :return: An instance of LROPoller that returns either IotFhirDestination or the result of
          cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.IotFhirDestination]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotFhirDestination]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.IotFhirDestination] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(
+            raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 workspace_name=workspace_name,
                 iot_connector_name=iot_connector_name,
                 fhir_destination_name=fhir_destination_name,
                 iot_fhir_destination=iot_fhir_destination,
                 api_version=api_version,
                 content_type=content_type,
@@ -365,37 +458,35 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("IotFhirDestination", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[_models.IotFhirDestination].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}"
-    }
+        return LROPoller[_models.IotFhirDestination](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
+    def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
         fhir_destination_name: str,
         **kwargs: Any
     ) -> None:
@@ -409,116 +500,99 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             iot_connector_name=iot_connector_name,
             fhir_destination_name=fhir_destination_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, {})  # type: ignore
 
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}"
-    }
-
-    @distributed_trace_async
-    async def begin_delete(
+    @distributed_trace
+    def begin_delete(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
         fhir_destination_name: str,
         **kwargs: Any
-    ) -> AsyncLROPoller[None]:
+    ) -> LROPoller[None]:
         """Deletes an IoT Connector FHIR destination.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param fhir_destination_name: The name of IoT Connector FHIR destination resource. Required.
         :type fhir_destination_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._delete_initial(  # type: ignore
+            raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 workspace_name=workspace_name,
                 iot_connector_name=iot_connector_name,
                 fhir_destination_name=fhir_destination_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_iot_connectors_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_iot_connectors_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -69,15 +69,14 @@
         """Lists all IoT Connectors for the given workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either IotConnector or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -91,87 +90,81 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_workspace_request(
+                _request = build_list_by_workspace_request(
                     resource_group_name=resource_group_name,
                     workspace_name=workspace_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_workspace.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("IotConnectorCollection", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_workspace.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors"
-    }
-
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, workspace_name: str, iot_connector_name: str, **kwargs: Any
     ) -> _models.IotConnector:
         """Gets the properties of the specified IoT Connector.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: IotConnector or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.IotConnector
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -182,56 +175,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.IotConnector] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             iot_connector_name=iot_connector_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("IotConnector", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
+        return deserialized  # type: ignore
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
-        iot_connector: Union[_models.IotConnector, IO],
+        iot_connector: Union[_models.IotConnector, IO[bytes]],
         **kwargs: Any
     ) -> _models.IotConnector:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -249,33 +237,32 @@
         _json = None
         _content = None
         if isinstance(iot_connector, (IOBase, bytes)):
             _content = iot_connector
         else:
             _json = self._serialize.body(iot_connector, "IotConnector")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             iot_connector_name=iot_connector_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
@@ -291,18 +278,14 @@
             deserialized = self._deserialize("IotConnector", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
-
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
         iot_connector: _models.IotConnector,
@@ -321,35 +304,27 @@
         :type iot_connector_name: str
         :param iot_connector: The parameters for creating or updating an IoT Connectors resource.
          Required.
         :type iot_connector: ~azure.mgmt.healthcareapis.models.IotConnector
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
-        iot_connector: IO,
+        iot_connector: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.IotConnector]:
         """Creates or updates an IoT Connector resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
@@ -357,64 +332,45 @@
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param iot_connector: The parameters for creating or updating an IoT Connectors resource.
          Required.
-        :type iot_connector: IO
+        :type iot_connector: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
-        iot_connector: Union[_models.IotConnector, IO],
+        iot_connector: Union[_models.IotConnector, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.IotConnector]:
         """Creates or updates an IoT Connector resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param iot_connector: The parameters for creating or updating an IoT Connectors resource. Is
-         either a IotConnector type or a IO type. Required.
-        :type iot_connector: ~azure.mgmt.healthcareapis.models.IotConnector or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         either a IotConnector type or a IO[bytes] type. Required.
+        :type iot_connector: ~azure.mgmt.healthcareapis.models.IotConnector or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -439,42 +395,40 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("IotConnector", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.IotConnector].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
+        return AsyncLROPoller[_models.IotConnector](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _update_initial(
         self,
         resource_group_name: str,
         iot_connector_name: str,
         workspace_name: str,
-        iot_connector_patch_resource: Union[_models.IotConnectorPatchResource, IO],
+        iot_connector_patch_resource: Union[_models.IotConnectorPatchResource, IO[bytes]],
         **kwargs: Any
     ) -> _models.IotConnector:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -492,33 +446,32 @@
         _json = None
         _content = None
         if isinstance(iot_connector_patch_resource, (IOBase, bytes)):
             _content = iot_connector_patch_resource
         else:
             _json = self._serialize.body(iot_connector_patch_resource, "IotConnectorPatchResource")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             iot_connector_name=iot_connector_name,
             workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
@@ -531,18 +484,14 @@
             deserialized = self._deserialize("IotConnector", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
-
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         iot_connector_name: str,
         workspace_name: str,
         iot_connector_patch_resource: _models.IotConnectorPatchResource,
@@ -560,100 +509,73 @@
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_patch_resource: The parameters for updating an IoT Connector. Required.
         :type iot_connector_patch_resource: ~azure.mgmt.healthcareapis.models.IotConnectorPatchResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         iot_connector_name: str,
         workspace_name: str,
-        iot_connector_patch_resource: IO,
+        iot_connector_patch_resource: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.IotConnector]:
         """Patch an IoT Connector.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_patch_resource: The parameters for updating an IoT Connector. Required.
-        :type iot_connector_patch_resource: IO
+        :type iot_connector_patch_resource: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_update(
         self,
         resource_group_name: str,
         iot_connector_name: str,
         workspace_name: str,
-        iot_connector_patch_resource: Union[_models.IotConnectorPatchResource, IO],
+        iot_connector_patch_resource: Union[_models.IotConnectorPatchResource, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.IotConnector]:
         """Patch an IoT Connector.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_patch_resource: The parameters for updating an IoT Connector. Is either a
-         IotConnectorPatchResource type or a IO type. Required.
+         IotConnectorPatchResource type or a IO[bytes] type. Required.
         :type iot_connector_patch_resource: ~azure.mgmt.healthcareapis.models.IotConnectorPatchResource
-         or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -678,35 +600,33 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("IotConnector", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.IotConnector].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
+        return AsyncLROPoller[_models.IotConnector](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, iot_connector_name: str, workspace_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -717,67 +637,54 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             iot_connector_name=iot_connector_name,
             workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, iot_connector_name: str, workspace_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Deletes an IoT Connector.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -797,27 +704,23 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_operation_results_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_operation_results_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -56,15 +56,14 @@
     ) -> _models.OperationResultsDescription:
         """Get the operation result for a long running operation.
 
         :param location_name: The location of the operation. Required.
         :type location_name: str
         :param operation_result_id: The ID of the operation result to get. Required.
         :type operation_result_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: OperationResultsDescription or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.OperationResultsDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -75,41 +74,36 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationResultsDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             location_name=location_name,
             operation_result_id=operation_result_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("OperationResultsDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HealthcareApis/locations/{locationName}/operationresults/{operationResultId}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -52,15 +52,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.OperationDetail"]:
         """Lists all of the available operations supported by Microsoft Healthcare resource provider.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either OperationDetail or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.OperationDetail]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -75,60 +74,57 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ListOperations", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/providers/Microsoft.HealthcareApis/operations"}
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_patch.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_private_endpoint_connections_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -68,15 +68,14 @@
         """Lists all private endpoint connections for a service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param resource_name: The name of the service instance. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateEndpointConnectionDescription or the result
          of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -92,88 +91,82 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_service_request(
+                _request = build_list_by_service_request(
                     resource_group_name=resource_group_name,
                     resource_name=resource_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_service.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("PrivateEndpointConnectionListResultDescription", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_service.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections"
-    }
-
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> _models.PrivateEndpointConnectionDescription:
         """Gets the specified private endpoint connection associated with the service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param resource_name: The name of the service instance. Required.
         :type resource_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateEndpointConnectionDescription or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -184,56 +177,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateEndpointConnectionDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return deserialized  # type: ignore
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         resource_name: str,
         private_endpoint_connection_name: str,
-        properties: Union[_models.PrivateEndpointConnection, IO],
+        properties: Union[_models.PrivateEndpointConnection, IO[bytes]],
         **kwargs: Any
     ) -> _models.PrivateEndpointConnectionDescription:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -251,52 +239,47 @@
         _json = None
         _content = None
         if isinstance(properties, (IOBase, bytes)):
             _content = properties
         else:
             _json = self._serialize.body(properties, "PrivateEndpointConnection")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
         private_endpoint_connection_name: str,
@@ -316,36 +299,28 @@
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
         :param properties: The private endpoint connection properties. Required.
         :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnection
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnectionDescription
          or the result of cls(response)
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
         private_endpoint_connection_name: str,
-        properties: IO,
+        properties: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.PrivateEndpointConnectionDescription]:
         """Update the state of the specified private endpoint connection associated with the service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
@@ -353,66 +328,47 @@
         :type resource_group_name: str
         :param resource_name: The name of the service instance. Required.
         :type resource_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
         :param properties: The private endpoint connection properties. Required.
-        :type properties: IO
+        :type properties: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnectionDescription
          or the result of cls(response)
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
         private_endpoint_connection_name: str,
-        properties: Union[_models.PrivateEndpointConnection, IO],
+        properties: Union[_models.PrivateEndpointConnection, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.PrivateEndpointConnectionDescription]:
         """Update the state of the specified private endpoint connection associated with the service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param resource_name: The name of the service instance. Required.
         :type resource_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
         :param properties: The private endpoint connection properties. Is either a
-         PrivateEndpointConnection type or a IO type. Required.
-        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnection or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         PrivateEndpointConnection type or a IO[bytes] type. Required.
+        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnection or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnectionDescription
          or the result of cls(response)
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
@@ -438,35 +394,33 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.PrivateEndpointConnectionDescription].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return AsyncLROPoller[_models.PrivateEndpointConnectionDescription](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -477,45 +431,40 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Deletes a private endpoint connection.
 
@@ -523,22 +472,14 @@
          Required.
         :type resource_group_name: str
         :param resource_name: The name of the service instance. Required.
         :type resource_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -558,27 +499,23 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_private_link_resources_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_private_link_resources_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -57,15 +57,14 @@
         """Gets the private link resources that need to be created for a service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param resource_name: The name of the service instance. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkResourceListResultDescription or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.PrivateLinkResourceListResultDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -76,63 +75,57 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkResourceListResultDescription] = kwargs.pop("cls", None)
 
-        request = build_list_by_service_request(
+        _request = build_list_by_service_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.list_by_service.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkResourceListResultDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    list_by_service.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateLinkResources"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, resource_name: str, group_name: str, **kwargs: Any
     ) -> _models.PrivateLinkResourceDescription:
         """Gets a private link resource that need to be created for a service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param resource_name: The name of the service instance. Required.
         :type resource_name: str
         :param group_name: The name of the private link resource group. Required.
         :type group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkResourceDescription or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.PrivateLinkResourceDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -143,42 +136,37 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkResourceDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             group_name=group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkResourceDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateLinkResources/{groupName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_services_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_workspaces_operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,595 +1,858 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._services_operations import (
-    build_check_name_availability_request,
-    build_create_or_update_request,
-    build_delete_request,
-    build_get_request,
-    build_list_by_resource_group_request,
-    build_list_request,
-    build_update_request,
-)
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.HealthcareApis/workspaces")
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+    }
 
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
-class ServicesOperations:
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_get_request(
+    resource_group_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_create_or_update_request(
+    resource_group_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_update_request(
+    resource_group_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_delete_request(
+    resource_group_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+class WorkspacesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.healthcareapis.aio.HealthcareApisManagementClient`'s
-        :attr:`services` attribute.
+        :class:`~azure.mgmt.healthcareapis.HealthcareApisManagementClient`'s
+        :attr:`workspaces` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace_async
-    async def get(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.ServicesDescription:
-        """Get the metadata of a service instance.
+    @distributed_trace
+    def list_by_subscription(self, **kwargs: Any) -> Iterable["_models.Workspace"]:
+        """Lists all the available workspaces under the specified subscription.
+
+        :return: An iterator like instance of either Workspace or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.Workspace]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WorkspaceList] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                _request = build_list_by_subscription_request(
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("WorkspaceList", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, iter(list_of_elem)
+
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+            return pipeline_response
+
+        return ItemPaged(get_next, extract_data)
+
+    @distributed_trace
+    def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.Workspace"]:
+        """Lists all the available workspaces under the specified resource group.
+
+        :param resource_group_name: The name of the resource group that contains the service instance.
+         Required.
+        :type resource_group_name: str
+        :return: An iterator like instance of either Workspace or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.Workspace]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.WorkspaceList] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                _request = build_list_by_resource_group_request(
+                    resource_group_name=resource_group_name,
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("WorkspaceList", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, iter(list_of_elem)
+
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+            return pipeline_response
+
+        return ItemPaged(get_next, extract_data)
+
+    @distributed_trace
+    def get(self, resource_group_name: str, workspace_name: str, **kwargs: Any) -> _models.Workspace:
+        """Gets the properties of the specified workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: ServicesDescription or the result of cls(response)
-        :rtype: ~azure.mgmt.healthcareapis.models.ServicesDescription
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
+        :return: Workspace or the result of cls(response)
+        :rtype: ~azure.mgmt.healthcareapis.models.Workspace
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
+        cls: ClsType[_models.Workspace] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
-            resource_name=resource_name,
+            workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("ServicesDescription", pipeline_response)
+        deserialized = self._deserialize("Workspace", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}"
-    }
+        return deserialized  # type: ignore
 
-    async def _create_or_update_initial(
+    def _create_or_update_initial(
         self,
         resource_group_name: str,
-        resource_name: str,
-        service_description: Union[_models.ServicesDescription, IO],
+        workspace_name: str,
+        workspace: Union[_models.Workspace, IO[bytes]],
         **kwargs: Any
-    ) -> _models.ServicesDescription:
+    ) -> _models.Workspace:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
+        cls: ClsType[_models.Workspace] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(service_description, (IOBase, bytes)):
-            _content = service_description
+        if isinstance(workspace, (IOBase, bytes)):
+            _content = workspace
         else:
-            _json = self._serialize.body(service_description, "ServicesDescription")
+            _json = self._serialize.body(workspace, "Workspace")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
-            resource_name=resource_name,
+            workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 201]:
+        if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize("ServicesDescription", pipeline_response)
+            deserialized = self._deserialize("Workspace", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize("ServicesDescription", pipeline_response)
+            deserialized = self._deserialize("Workspace", pipeline_response)
+
+        if response.status_code == 202:
+            deserialized = self._deserialize("Workspace", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}"
-    }
-
     @overload
-    async def begin_create_or_update(
+    def begin_create_or_update(
         self,
         resource_group_name: str,
-        resource_name: str,
-        service_description: _models.ServicesDescription,
+        workspace_name: str,
+        workspace: _models.Workspace,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ServicesDescription]:
-        """Create or update the metadata of a service instance.
+    ) -> LROPoller[_models.Workspace]:
+        """Creates or updates a workspace resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
-        :param service_description: The service instance metadata. Required.
-        :type service_description: ~azure.mgmt.healthcareapis.models.ServicesDescription
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
+        :param workspace: The parameters for creating or updating a healthcare workspace. Required.
+        :type workspace: ~azure.mgmt.healthcareapis.models.Workspace
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
-         cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
+        :return: An instance of LROPoller that returns either Workspace or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.Workspace]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_create_or_update(
+    def begin_create_or_update(
         self,
         resource_group_name: str,
-        resource_name: str,
-        service_description: IO,
+        workspace_name: str,
+        workspace: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ServicesDescription]:
-        """Create or update the metadata of a service instance.
+    ) -> LROPoller[_models.Workspace]:
+        """Creates or updates a workspace resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
-        :param service_description: The service instance metadata. Required.
-        :type service_description: IO
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
+        :param workspace: The parameters for creating or updating a healthcare workspace. Required.
+        :type workspace: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
-         cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
+        :return: An instance of LROPoller that returns either Workspace or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.Workspace]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def begin_create_or_update(
+    @distributed_trace
+    def begin_create_or_update(
         self,
         resource_group_name: str,
-        resource_name: str,
-        service_description: Union[_models.ServicesDescription, IO],
+        workspace_name: str,
+        workspace: Union[_models.Workspace, IO[bytes]],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ServicesDescription]:
-        """Create or update the metadata of a service instance.
+    ) -> LROPoller[_models.Workspace]:
+        """Creates or updates a workspace resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
-        :param service_description: The service instance metadata. Is either a ServicesDescription type
-         or a IO type. Required.
-        :type service_description: ~azure.mgmt.healthcareapis.models.ServicesDescription or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
-         cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
+        :param workspace: The parameters for creating or updating a healthcare workspace. Is either a
+         Workspace type or a IO[bytes] type. Required.
+        :type workspace: ~azure.mgmt.healthcareapis.models.Workspace or IO[bytes]
+        :return: An instance of LROPoller that returns either Workspace or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.Workspace]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        cls: ClsType[_models.Workspace] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(
+            raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
-                resource_name=resource_name,
-                service_description=service_description,
+                workspace_name=workspace_name,
+                workspace=workspace,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("ServicesDescription", pipeline_response)
+            deserialized = self._deserialize("Workspace", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[_models.Workspace].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}"
-    }
+        return LROPoller[_models.Workspace](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    async def _update_initial(
+    def _update_initial(
         self,
         resource_group_name: str,
-        resource_name: str,
-        service_patch_description: Union[_models.ServicesPatchDescription, IO],
+        workspace_name: str,
+        workspace_patch_resource: Union[_models.WorkspacePatchResource, IO[bytes]],
         **kwargs: Any
-    ) -> _models.ServicesDescription:
+    ) -> _models.Workspace:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
+        cls: ClsType[_models.Workspace] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(service_patch_description, (IOBase, bytes)):
-            _content = service_patch_description
+        if isinstance(workspace_patch_resource, (IOBase, bytes)):
+            _content = workspace_patch_resource
         else:
-            _json = self._serialize.body(service_patch_description, "ServicesPatchDescription")
+            _json = self._serialize.body(workspace_patch_resource, "WorkspacePatchResource")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
-            resource_name=resource_name,
+            workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("ServicesDescription", pipeline_response)
+        if response.status_code == 200:
+            deserialized = self._deserialize("Workspace", pipeline_response)
 
-        if cls:
-            return cls(pipeline_response, deserialized, {})
+        if response.status_code == 202:
+            deserialized = self._deserialize("Workspace", pipeline_response)
 
-        return deserialized
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
-    async def begin_update(
+    def begin_update(
         self,
         resource_group_name: str,
-        resource_name: str,
-        service_patch_description: _models.ServicesPatchDescription,
+        workspace_name: str,
+        workspace_patch_resource: _models.WorkspacePatchResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ServicesDescription]:
-        """Update the metadata of a service instance.
+    ) -> LROPoller[_models.Workspace]:
+        """Patch workspace details.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
-        :param service_patch_description: The service instance metadata and security metadata.
-         Required.
-        :type service_patch_description: ~azure.mgmt.healthcareapis.models.ServicesPatchDescription
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
+        :param workspace_patch_resource: The parameters for updating a specified workspace. Required.
+        :type workspace_patch_resource: ~azure.mgmt.healthcareapis.models.WorkspacePatchResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
-         cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
+        :return: An instance of LROPoller that returns either Workspace or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.Workspace]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_update(
+    def begin_update(
         self,
         resource_group_name: str,
-        resource_name: str,
-        service_patch_description: IO,
+        workspace_name: str,
+        workspace_patch_resource: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ServicesDescription]:
-        """Update the metadata of a service instance.
+    ) -> LROPoller[_models.Workspace]:
+        """Patch workspace details.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
-        :param service_patch_description: The service instance metadata and security metadata.
-         Required.
-        :type service_patch_description: IO
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
+        :param workspace_patch_resource: The parameters for updating a specified workspace. Required.
+        :type workspace_patch_resource: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
-         cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
+        :return: An instance of LROPoller that returns either Workspace or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.Workspace]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def begin_update(
+    @distributed_trace
+    def begin_update(
         self,
         resource_group_name: str,
-        resource_name: str,
-        service_patch_description: Union[_models.ServicesPatchDescription, IO],
+        workspace_name: str,
+        workspace_patch_resource: Union[_models.WorkspacePatchResource, IO[bytes]],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.ServicesDescription]:
-        """Update the metadata of a service instance.
+    ) -> LROPoller[_models.Workspace]:
+        """Patch workspace details.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
-        :param service_patch_description: The service instance metadata and security metadata. Is
-         either a ServicesPatchDescription type or a IO type. Required.
-        :type service_patch_description: ~azure.mgmt.healthcareapis.models.ServicesPatchDescription or
-         IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
-         cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
+        :param workspace_patch_resource: The parameters for updating a specified workspace. Is either a
+         WorkspacePatchResource type or a IO[bytes] type. Required.
+        :type workspace_patch_resource: ~azure.mgmt.healthcareapis.models.WorkspacePatchResource or
+         IO[bytes]
+        :return: An instance of LROPoller that returns either Workspace or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.Workspace]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        cls: ClsType[_models.Workspace] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._update_initial(
+            raw_result = self._update_initial(
                 resource_group_name=resource_group_name,
-                resource_name=resource_name,
-                service_patch_description=service_patch_description,
+                workspace_name=workspace_name,
+                workspace_patch_resource=workspace_patch_resource,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("ServicesDescription", pipeline_response)
+            deserialized = self._deserialize("Workspace", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[_models.Workspace].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}"
-    }
+        return LROPoller[_models.Workspace](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, resource_name: str, **kwargs: Any
+    def _delete_initial(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, workspace_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -597,394 +860,84 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
-            resource_name=resource_name,
+            workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [202, 204]:
+        if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, {})  # type: ignore
 
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}"
-    }
-
-    @distributed_trace_async
-    async def begin_delete(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
-        """Delete a service instance.
+    @distributed_trace
+    def begin_delete(self, resource_group_name: str, workspace_name: str, **kwargs: Any) -> LROPoller[None]:
+        """Deletes a specified workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._delete_initial(  # type: ignore
+            raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
-                resource_name=resource_name,
+                workspace_name=workspace_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}"
-    }
-
-    @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.ServicesDescription"]:
-        """Get all the service instances in a subscription.
-
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ServicesDescription or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.ServicesDescription]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.ServicesDescriptionListResult] = kwargs.pop("cls", None)
-
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        def prepare_request(next_link=None):
-            if not next_link:
-
-                request = build_list_request(
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("ServicesDescriptionListResult", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
-
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-            return pipeline_response
-
-        return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.HealthcareApis/services"}
-
-    @distributed_trace
-    def list_by_resource_group(
-        self, resource_group_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.ServicesDescription"]:
-        """Get all the service instances in a resource group.
-
-        :param resource_group_name: The name of the resource group that contains the service instance.
-         Required.
-        :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ServicesDescription or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.ServicesDescription]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.ServicesDescriptionListResult] = kwargs.pop("cls", None)
-
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        def prepare_request(next_link=None):
-            if not next_link:
-
-                request = build_list_by_resource_group_request(
-                    resource_group_name=resource_group_name,
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("ServicesDescriptionListResult", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
-
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-            return pipeline_response
-
-        return AsyncItemPaged(get_next, extract_data)
-
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services"
-    }
-
-    @overload
-    async def check_name_availability(
-        self,
-        check_name_availability_inputs: _models.CheckNameAvailabilityParameters,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.ServicesNameAvailabilityInfo:
-        """Check if a service instance name is available.
-
-        :param check_name_availability_inputs: Set the name parameter in the
-         CheckNameAvailabilityParameters structure to the name of the service instance to check.
-         Required.
-        :type check_name_availability_inputs:
-         ~azure.mgmt.healthcareapis.models.CheckNameAvailabilityParameters
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: ServicesNameAvailabilityInfo or the result of cls(response)
-        :rtype: ~azure.mgmt.healthcareapis.models.ServicesNameAvailabilityInfo
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @overload
-    async def check_name_availability(
-        self, check_name_availability_inputs: IO, *, content_type: str = "application/json", **kwargs: Any
-    ) -> _models.ServicesNameAvailabilityInfo:
-        """Check if a service instance name is available.
-
-        :param check_name_availability_inputs: Set the name parameter in the
-         CheckNameAvailabilityParameters structure to the name of the service instance to check.
-         Required.
-        :type check_name_availability_inputs: IO
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: ServicesNameAvailabilityInfo or the result of cls(response)
-        :rtype: ~azure.mgmt.healthcareapis.models.ServicesNameAvailabilityInfo
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @distributed_trace_async
-    async def check_name_availability(
-        self, check_name_availability_inputs: Union[_models.CheckNameAvailabilityParameters, IO], **kwargs: Any
-    ) -> _models.ServicesNameAvailabilityInfo:
-        """Check if a service instance name is available.
-
-        :param check_name_availability_inputs: Set the name parameter in the
-         CheckNameAvailabilityParameters structure to the name of the service instance to check. Is
-         either a CheckNameAvailabilityParameters type or a IO type. Required.
-        :type check_name_availability_inputs:
-         ~azure.mgmt.healthcareapis.models.CheckNameAvailabilityParameters or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: ServicesNameAvailabilityInfo or the result of cls(response)
-        :rtype: ~azure.mgmt.healthcareapis.models.ServicesNameAvailabilityInfo
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.ServicesNameAvailabilityInfo] = kwargs.pop("cls", None)
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(check_name_availability_inputs, (IOBase, bytes)):
-            _content = check_name_availability_inputs
-        else:
-            _json = self._serialize.body(check_name_availability_inputs, "CheckNameAvailabilityParameters")
-
-        request = build_check_name_availability_request(
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            template_url=self.check_name_availability.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("ServicesNameAvailabilityInfo", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
-
-    check_name_availability.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HealthcareApis/checkNameAvailability"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_workspace_private_endpoint_connections_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_private_endpoint_connections_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,238 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._workspace_private_endpoint_connections_operations import (
-    build_create_or_update_request,
-    build_delete_request,
-    build_get_request,
-    build_list_by_workspace_request,
-)
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_list_by_service_request(
+    resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_get_request(
+    resource_group_name: str,
+    resource_name: str,
+    private_endpoint_connection_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
+        "privateEndpointConnectionName": _SERIALIZER.url(
+            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_create_or_update_request(
+    resource_group_name: str,
+    resource_name: str,
+    private_endpoint_connection_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
+        "privateEndpointConnectionName": _SERIALIZER.url(
+            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_delete_request(
+    resource_group_name: str,
+    resource_name: str,
+    private_endpoint_connection_name: str,
+    subscription_id: str,
+    **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
+        "privateEndpointConnectionName": _SERIALIZER.url(
+            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
-class WorkspacePrivateEndpointConnectionsOperations:
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+class PrivateEndpointConnectionsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.healthcareapis.aio.HealthcareApisManagementClient`'s
-        :attr:`workspace_private_endpoint_connections` attribute.
+        :class:`~azure.mgmt.healthcareapis.HealthcareApisManagementClient`'s
+        :attr:`private_endpoint_connections` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list_by_workspace(
-        self, resource_group_name: str, workspace_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.PrivateEndpointConnectionDescription"]:
-        """Lists all private endpoint connections for a workspace.
+    def list_by_service(
+        self, resource_group_name: str, resource_name: str, **kwargs: Any
+    ) -> Iterable["_models.PrivateEndpointConnectionDescription"]:
+        """Lists all private endpoint connections for a service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
         :return: An iterator like instance of either PrivateEndpointConnectionDescription or the result
          of cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
+         ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateEndpointConnectionListResultDescription] = kwargs.pop("cls", None)
@@ -92,88 +244,82 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_workspace_request(
+                _request = build_list_by_service_request(
                     resource_group_name=resource_group_name,
-                    workspace_name=workspace_name,
+                    resource_name=resource_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_workspace.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-        async def extract_data(pipeline_response):
+        def extract_data(pipeline_response):
             deserialized = self._deserialize("PrivateEndpointConnectionListResultDescription", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return None, AsyncList(list_of_elem)
+            return None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
             _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
-
-    list_by_workspace.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateEndpointConnections"
-    }
+        return ItemPaged(get_next, extract_data)
 
-    @distributed_trace_async
-    async def get(
-        self, resource_group_name: str, workspace_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    @distributed_trace
+    def get(
+        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> _models.PrivateEndpointConnectionDescription:
-        """Gets the specified private endpoint connection associated with the workspace.
+        """Gets the specified private endpoint connection associated with the service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateEndpointConnectionDescription or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -184,56 +330,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateEndpointConnectionDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
-            workspace_name=workspace_name,
+            resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return deserialized  # type: ignore
 
-    async def _create_or_update_initial(
+    def _create_or_update_initial(
         self,
         resource_group_name: str,
-        workspace_name: str,
+        resource_name: str,
         private_endpoint_connection_name: str,
-        properties: Union[_models.PrivateEndpointConnectionDescription, IO],
+        properties: Union[_models.PrivateEndpointConnection, IO[bytes]],
         **kwargs: Any
     ) -> _models.PrivateEndpointConnectionDescription:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -249,227 +390,193 @@
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(properties, (IOBase, bytes)):
             _content = properties
         else:
-            _json = self._serialize.body(properties, "PrivateEndpointConnectionDescription")
+            _json = self._serialize.body(properties, "PrivateEndpointConnection")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
-            workspace_name=workspace_name,
+            resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
-    async def begin_create_or_update(
+    def begin_create_or_update(
         self,
         resource_group_name: str,
-        workspace_name: str,
+        resource_name: str,
         private_endpoint_connection_name: str,
-        properties: _models.PrivateEndpointConnectionDescription,
+        properties: _models.PrivateEndpointConnection,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.PrivateEndpointConnectionDescription]:
-        """Update the state of the specified private endpoint connection associated with the workspace.
+    ) -> LROPoller[_models.PrivateEndpointConnectionDescription]:
+        """Update the state of the specified private endpoint connection associated with the service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
         :param properties: The private endpoint connection properties. Required.
-        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription
+        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnection
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnectionDescription
-         or the result of cls(response)
+        :return: An instance of LROPoller that returns either PrivateEndpointConnectionDescription or
+         the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
+         ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_create_or_update(
+    def begin_create_or_update(
         self,
         resource_group_name: str,
-        workspace_name: str,
+        resource_name: str,
         private_endpoint_connection_name: str,
-        properties: IO,
+        properties: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.PrivateEndpointConnectionDescription]:
-        """Update the state of the specified private endpoint connection associated with the workspace.
+    ) -> LROPoller[_models.PrivateEndpointConnectionDescription]:
+        """Update the state of the specified private endpoint connection associated with the service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
         :param properties: The private endpoint connection properties. Required.
-        :type properties: IO
+        :type properties: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnectionDescription
-         or the result of cls(response)
+        :return: An instance of LROPoller that returns either PrivateEndpointConnectionDescription or
+         the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
+         ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def begin_create_or_update(
+    @distributed_trace
+    def begin_create_or_update(
         self,
         resource_group_name: str,
-        workspace_name: str,
+        resource_name: str,
         private_endpoint_connection_name: str,
-        properties: Union[_models.PrivateEndpointConnectionDescription, IO],
+        properties: Union[_models.PrivateEndpointConnection, IO[bytes]],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.PrivateEndpointConnectionDescription]:
-        """Update the state of the specified private endpoint connection associated with the workspace.
+    ) -> LROPoller[_models.PrivateEndpointConnectionDescription]:
+        """Update the state of the specified private endpoint connection associated with the service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
         :param properties: The private endpoint connection properties. Is either a
-         PrivateEndpointConnectionDescription type or a IO type. Required.
-        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnectionDescription
-         or the result of cls(response)
+         PrivateEndpointConnection type or a IO[bytes] type. Required.
+        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnection or IO[bytes]
+        :return: An instance of LROPoller that returns either PrivateEndpointConnectionDescription or
+         the result of cls(response)
         :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
+         ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PrivateEndpointConnectionDescription] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(
+            raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
-                workspace_name=workspace_name,
+                resource_name=resource_name,
                 private_endpoint_connection_name=private_endpoint_connection_name,
                 properties=properties,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[_models.PrivateEndpointConnectionDescription].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return LROPoller[_models.PrivateEndpointConnectionDescription](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, workspace_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    def _delete_initial(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -477,108 +584,91 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
-            workspace_name=workspace_name,
+            resource_name=resource_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, {})  # type: ignore
 
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
-
-    @distributed_trace_async
-    async def begin_delete(
-        self, resource_group_name: str, workspace_name: str, private_endpoint_connection_name: str, **kwargs: Any
-    ) -> AsyncLROPoller[None]:
+    @distributed_trace
+    def begin_delete(
+        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    ) -> LROPoller[None]:
         """Deletes a private endpoint connection.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._delete_initial(  # type: ignore
+            raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
-                workspace_name=workspace_name,
+                resource_name=resource_name,
                 private_endpoint_connection_name=private_endpoint_connection_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_workspace_private_link_resources_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_workspace_private_link_resources_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -63,15 +63,14 @@
         """Gets the private link resources that need to be created for a workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateLinkResourceDescription or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.PrivateLinkResourceDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -87,87 +86,81 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_workspace_request(
+                _request = build_list_by_workspace_request(
                     resource_group_name=resource_group_name,
                     workspace_name=workspace_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_workspace.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("PrivateLinkResourceListResultDescription", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_workspace.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateLinkResources"
-    }
-
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, workspace_name: str, group_name: str, **kwargs: Any
     ) -> _models.PrivateLinkResourceDescription:
         """Gets a private link resource that need to be created for a workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param group_name: The name of the private link resource group. Required.
         :type group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkResourceDescription or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.PrivateLinkResourceDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -178,42 +171,37 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkResourceDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             group_name=group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkResourceDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateLinkResources/{groupName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/aio/operations/_workspaces_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_services_operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -27,728 +27,495 @@
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._workspaces_operations import (
+from ...operations._services_operations import (
+    build_check_name_availability_request,
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_resource_group_request,
-    build_list_by_subscription_request,
+    build_list_request,
     build_update_request,
 )
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class WorkspacesOperations:
+class ServicesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.healthcareapis.aio.HealthcareApisManagementClient`'s
-        :attr:`workspaces` attribute.
+        :attr:`services` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace
-    def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.Workspace"]:
-        """Lists all the available workspaces under the specified subscription.
-
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either Workspace or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.Workspace]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.WorkspaceList] = kwargs.pop("cls", None)
-
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        def prepare_request(next_link=None):
-            if not next_link:
-
-                request = build_list_by_subscription_request(
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list_by_subscription.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("WorkspaceList", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
-
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-            return pipeline_response
-
-        return AsyncItemPaged(get_next, extract_data)
-
-    list_by_subscription.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HealthcareApis/workspaces"
-    }
-
-    @distributed_trace
-    def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.Workspace"]:
-        """Lists all the available workspaces under the specified resource group.
-
-        :param resource_group_name: The name of the resource group that contains the service instance.
-         Required.
-        :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either Workspace or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.Workspace]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.WorkspaceList] = kwargs.pop("cls", None)
-
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        def prepare_request(next_link=None):
-            if not next_link:
-
-                request = build_list_by_resource_group_request(
-                    resource_group_name=resource_group_name,
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("WorkspaceList", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
-
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-            return pipeline_response
-
-        return AsyncItemPaged(get_next, extract_data)
-
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces"
-    }
-
     @distributed_trace_async
-    async def get(self, resource_group_name: str, workspace_name: str, **kwargs: Any) -> _models.Workspace:
-        """Gets the properties of the specified workspace.
+    async def get(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.ServicesDescription:
+        """Get the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Workspace or the result of cls(response)
-        :rtype: ~azure.mgmt.healthcareapis.models.Workspace
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :return: ServicesDescription or the result of cls(response)
+        :rtype: ~azure.mgmt.healthcareapis.models.ServicesDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.Workspace] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
-            workspace_name=workspace_name,
+            resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("Workspace", pipeline_response)
+        deserialized = self._deserialize("ServicesDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}"
-    }
+        return deserialized  # type: ignore
 
     async def _create_or_update_initial(
-        self, resource_group_name: str, workspace_name: str, workspace: Union[_models.Workspace, IO], **kwargs: Any
-    ) -> _models.Workspace:
+        self,
+        resource_group_name: str,
+        resource_name: str,
+        service_description: Union[_models.ServicesDescription, IO[bytes]],
+        **kwargs: Any
+    ) -> _models.ServicesDescription:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.Workspace] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(workspace, (IOBase, bytes)):
-            _content = workspace
+        if isinstance(service_description, (IOBase, bytes)):
+            _content = service_description
         else:
-            _json = self._serialize.body(workspace, "Workspace")
+            _json = self._serialize.body(service_description, "ServicesDescription")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
-            workspace_name=workspace_name,
+            resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 201, 202]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize("Workspace", pipeline_response)
+            deserialized = self._deserialize("ServicesDescription", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize("Workspace", pipeline_response)
-
-        if response.status_code == 202:
-            deserialized = self._deserialize("Workspace", pipeline_response)
+            deserialized = self._deserialize("ServicesDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}"
-    }
-
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
-        workspace_name: str,
-        workspace: _models.Workspace,
+        resource_name: str,
+        service_description: _models.ServicesDescription,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.Workspace]:
-        """Creates or updates a workspace resource with the specified parameters.
+    ) -> AsyncLROPoller[_models.ServicesDescription]:
+        """Create or update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param workspace: The parameters for creating or updating a healthcare workspace. Required.
-        :type workspace: ~azure.mgmt.healthcareapis.models.Workspace
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_description: The service instance metadata. Required.
+        :type service_description: ~azure.mgmt.healthcareapis.models.ServicesDescription
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either Workspace or the result of
+        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.Workspace]
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
-        workspace_name: str,
-        workspace: IO,
+        resource_name: str,
+        service_description: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.Workspace]:
-        """Creates or updates a workspace resource with the specified parameters.
+    ) -> AsyncLROPoller[_models.ServicesDescription]:
+        """Create or update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param workspace: The parameters for creating or updating a healthcare workspace. Required.
-        :type workspace: IO
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_description: The service instance metadata. Required.
+        :type service_description: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either Workspace or the result of
+        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.Workspace]
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
-        self, resource_group_name: str, workspace_name: str, workspace: Union[_models.Workspace, IO], **kwargs: Any
-    ) -> AsyncLROPoller[_models.Workspace]:
-        """Creates or updates a workspace resource with the specified parameters.
+        self,
+        resource_group_name: str,
+        resource_name: str,
+        service_description: Union[_models.ServicesDescription, IO[bytes]],
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.ServicesDescription]:
+        """Create or update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param workspace: The parameters for creating or updating a healthcare workspace. Is either a
-         Workspace type or a IO type. Required.
-        :type workspace: ~azure.mgmt.healthcareapis.models.Workspace or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either Workspace or the result of
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_description: The service instance metadata. Is either a ServicesDescription type
+         or a IO[bytes] type. Required.
+        :type service_description: ~azure.mgmt.healthcareapis.models.ServicesDescription or IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.Workspace]
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.Workspace] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
                 resource_group_name=resource_group_name,
-                workspace_name=workspace_name,
-                workspace=workspace,
+                resource_name=resource_name,
+                service_description=service_description,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("Workspace", pipeline_response)
+            deserialized = self._deserialize("ServicesDescription", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.ServicesDescription].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}"
-    }
+        return AsyncLROPoller[_models.ServicesDescription](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _update_initial(
         self,
         resource_group_name: str,
-        workspace_name: str,
-        workspace_patch_resource: Union[_models.WorkspacePatchResource, IO],
+        resource_name: str,
+        service_patch_description: Union[_models.ServicesPatchDescription, IO[bytes]],
         **kwargs: Any
-    ) -> _models.Workspace:
+    ) -> _models.ServicesDescription:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.Workspace] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(workspace_patch_resource, (IOBase, bytes)):
-            _content = workspace_patch_resource
+        if isinstance(service_patch_description, (IOBase, bytes)):
+            _content = service_patch_description
         else:
-            _json = self._serialize.body(workspace_patch_resource, "WorkspacePatchResource")
+            _json = self._serialize.body(service_patch_description, "ServicesPatchDescription")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
-            workspace_name=workspace_name,
+            resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202]:
+        if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        if response.status_code == 200:
-            deserialized = self._deserialize("Workspace", pipeline_response)
-
-        if response.status_code == 202:
-            deserialized = self._deserialize("Workspace", pipeline_response)
+        deserialized = self._deserialize("ServicesDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}"
-    }
-
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
-        workspace_name: str,
-        workspace_patch_resource: _models.WorkspacePatchResource,
+        resource_name: str,
+        service_patch_description: _models.ServicesPatchDescription,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.Workspace]:
-        """Patch workspace details.
+    ) -> AsyncLROPoller[_models.ServicesDescription]:
+        """Update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param workspace_patch_resource: The parameters for updating a specified workspace. Required.
-        :type workspace_patch_resource: ~azure.mgmt.healthcareapis.models.WorkspacePatchResource
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_patch_description: The service instance metadata and security metadata.
+         Required.
+        :type service_patch_description: ~azure.mgmt.healthcareapis.models.ServicesPatchDescription
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either Workspace or the result of
+        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.Workspace]
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
-        workspace_name: str,
-        workspace_patch_resource: IO,
+        resource_name: str,
+        service_patch_description: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.Workspace]:
-        """Patch workspace details.
+    ) -> AsyncLROPoller[_models.ServicesDescription]:
+        """Update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param workspace_patch_resource: The parameters for updating a specified workspace. Required.
-        :type workspace_patch_resource: IO
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_patch_description: The service instance metadata and security metadata.
+         Required.
+        :type service_patch_description: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either Workspace or the result of
+        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.Workspace]
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_update(
         self,
         resource_group_name: str,
-        workspace_name: str,
-        workspace_patch_resource: Union[_models.WorkspacePatchResource, IO],
+        resource_name: str,
+        service_patch_description: Union[_models.ServicesPatchDescription, IO[bytes]],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.Workspace]:
-        """Patch workspace details.
+    ) -> AsyncLROPoller[_models.ServicesDescription]:
+        """Update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param workspace_patch_resource: The parameters for updating a specified workspace. Is either a
-         WorkspacePatchResource type or a IO type. Required.
-        :type workspace_patch_resource: ~azure.mgmt.healthcareapis.models.WorkspacePatchResource or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either Workspace or the result of
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_patch_description: The service instance metadata and security metadata. Is
+         either a ServicesPatchDescription type or a IO[bytes] type. Required.
+        :type service_patch_description: ~azure.mgmt.healthcareapis.models.ServicesPatchDescription or
+         IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.Workspace]
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.Workspace] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._update_initial(
                 resource_group_name=resource_group_name,
-                workspace_name=workspace_name,
-                workspace_patch_resource=workspace_patch_resource,
+                resource_name=resource_name,
+                service_patch_description=service_patch_description,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("Workspace", pipeline_response)
+            deserialized = self._deserialize("ServicesDescription", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.ServicesDescription].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}"
-    }
+        return AsyncLROPoller[_models.ServicesDescription](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, workspace_name: str, **kwargs: Any
+        self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -756,62 +523,49 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
-            workspace_name=workspace_name,
+            resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202, 204]:
+        if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace_async
-    async def begin_delete(self, resource_group_name: str, workspace_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
-        """Deletes a specified workspace.
+    async def begin_delete(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
+        """Delete a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -819,38 +573,306 @@
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
-                workspace_name=workspace_name,
+                resource_name=resource_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+
+    @distributed_trace
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.ServicesDescription"]:
+        """Get all the service instances in a subscription.
+
+        :return: An iterator like instance of either ServicesDescription or the result of cls(response)
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.ServicesDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ServicesDescriptionListResult] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                _request = build_list_request(
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("ServicesDescriptionListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, AsyncList(list_of_elem)
+
+        async def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+            return pipeline_response
+
+        return AsyncItemPaged(get_next, extract_data)
+
+    @distributed_trace
+    def list_by_resource_group(
+        self, resource_group_name: str, **kwargs: Any
+    ) -> AsyncIterable["_models.ServicesDescription"]:
+        """Get all the service instances in a resource group.
+
+        :param resource_group_name: The name of the resource group that contains the service instance.
+         Required.
+        :type resource_group_name: str
+        :return: An iterator like instance of either ServicesDescription or the result of cls(response)
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.ServicesDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ServicesDescriptionListResult] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                _request = build_list_by_resource_group_request(
+                    resource_group_name=resource_group_name,
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("ServicesDescriptionListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, AsyncList(list_of_elem)
+
+        async def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+            return pipeline_response
+
+        return AsyncItemPaged(get_next, extract_data)
+
+    @overload
+    async def check_name_availability(
+        self,
+        check_name_availability_inputs: _models.CheckNameAvailabilityParameters,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.ServicesNameAvailabilityInfo:
+        """Check if a service instance name is available.
+
+        :param check_name_availability_inputs: Set the name parameter in the
+         CheckNameAvailabilityParameters structure to the name of the service instance to check.
+         Required.
+        :type check_name_availability_inputs:
+         ~azure.mgmt.healthcareapis.models.CheckNameAvailabilityParameters
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: ServicesNameAvailabilityInfo or the result of cls(response)
+        :rtype: ~azure.mgmt.healthcareapis.models.ServicesNameAvailabilityInfo
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def check_name_availability(
+        self, check_name_availability_inputs: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.ServicesNameAvailabilityInfo:
+        """Check if a service instance name is available.
 
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}"
-    }
+        :param check_name_availability_inputs: Set the name parameter in the
+         CheckNameAvailabilityParameters structure to the name of the service instance to check.
+         Required.
+        :type check_name_availability_inputs: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: ServicesNameAvailabilityInfo or the result of cls(response)
+        :rtype: ~azure.mgmt.healthcareapis.models.ServicesNameAvailabilityInfo
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def check_name_availability(
+        self, check_name_availability_inputs: Union[_models.CheckNameAvailabilityParameters, IO[bytes]], **kwargs: Any
+    ) -> _models.ServicesNameAvailabilityInfo:
+        """Check if a service instance name is available.
+
+        :param check_name_availability_inputs: Set the name parameter in the
+         CheckNameAvailabilityParameters structure to the name of the service instance to check. Is
+         either a CheckNameAvailabilityParameters type or a IO[bytes] type. Required.
+        :type check_name_availability_inputs:
+         ~azure.mgmt.healthcareapis.models.CheckNameAvailabilityParameters or IO[bytes]
+        :return: ServicesNameAvailabilityInfo or the result of cls(response)
+        :rtype: ~azure.mgmt.healthcareapis.models.ServicesNameAvailabilityInfo
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ServicesNameAvailabilityInfo] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(check_name_availability_inputs, (IOBase, bytes)):
+            _content = check_name_availability_inputs
+        else:
+            _json = self._serialize.body(check_name_availability_inputs, "CheckNameAvailabilityParameters")
+
+        _request = build_check_name_availability_request(
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("ServicesNameAvailabilityInfo", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/models/__init__.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 from ._models_py3 import ServicesDescription
 from ._models_py3 import ServicesDescriptionListResult
 from ._models_py3 import ServicesNameAvailabilityInfo
 from ._models_py3 import ServicesPatchDescription
 from ._models_py3 import ServicesProperties
 from ._models_py3 import ServicesResource
 from ._models_py3 import ServicesResourceIdentity
+from ._models_py3 import SmartIdentityProviderApplication
+from ._models_py3 import SmartIdentityProviderConfiguration
+from ._models_py3 import StorageConfiguration
 from ._models_py3 import SystemData
 from ._models_py3 import TaggedResource
 from ._models_py3 import UserAssignedIdentity
 from ._models_py3 import Workspace
 from ._models_py3 import WorkspaceList
 from ._models_py3 import WorkspacePatchResource
 from ._models_py3 import WorkspaceProperties
@@ -94,14 +97,15 @@
 from ._healthcare_apis_management_client_enums import PrivateEndpointConnectionProvisioningState
 from ._healthcare_apis_management_client_enums import PrivateEndpointServiceConnectionStatus
 from ._healthcare_apis_management_client_enums import ProvisioningState
 from ._healthcare_apis_management_client_enums import PublicNetworkAccess
 from ._healthcare_apis_management_client_enums import ServiceEventState
 from ._healthcare_apis_management_client_enums import ServiceManagedIdentityType
 from ._healthcare_apis_management_client_enums import ServiceNameUnavailabilityReason
+from ._healthcare_apis_management_client_enums import SmartDataActions
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "CheckNameAvailabilityParameters",
     "CorsConfiguration",
@@ -168,14 +172,17 @@
     "ServicesDescription",
     "ServicesDescriptionListResult",
     "ServicesNameAvailabilityInfo",
     "ServicesPatchDescription",
     "ServicesProperties",
     "ServicesResource",
     "ServicesResourceIdentity",
+    "SmartIdentityProviderApplication",
+    "SmartIdentityProviderConfiguration",
+    "StorageConfiguration",
     "SystemData",
     "TaggedResource",
     "UserAssignedIdentity",
     "Workspace",
     "WorkspaceList",
     "WorkspacePatchResource",
     "WorkspaceProperties",
@@ -190,10 +197,11 @@
     "PrivateEndpointConnectionProvisioningState",
     "PrivateEndpointServiceConnectionStatus",
     "ProvisioningState",
     "PublicNetworkAccess",
     "ServiceEventState",
     "ServiceManagedIdentityType",
     "ServiceNameUnavailabilityReason",
+    "SmartDataActions",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/models/_healthcare_apis_management_client_enums.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/models/_healthcare_apis_management_client_enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,7 +134,13 @@
 
 
 class ServiceNameUnavailabilityReason(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The reason for unavailability."""
 
     INVALID = "Invalid"
     ALREADY_EXISTS = "AlreadyExists"
+
+
+class SmartDataActions(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The Data Actions that can be enabled for a Smart Identity Provider Application."""
+
+    READ = "Read"
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/models/_models_py3.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/models/_models_py3.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     from .. import models as _models
 JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 
 
 class CheckNameAvailabilityParameters(_serialization.Model):
     """Input values.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar name: The name of the service instance to check. Required.
     :vartype name: str
     :ivar type: The fully qualified resource type which includes provider namespace. Required.
     :vartype type: str
     """
 
@@ -345,14 +345,18 @@
      networks while private endpoint is enabled. Known values are: "Enabled" and "Disabled".
     :vartype public_network_access: str or ~azure.mgmt.healthcareapis.models.PublicNetworkAccess
     :ivar event_state: DICOM Service event support status. Known values are: "Disabled", "Enabled",
      and "Updating".
     :vartype event_state: str or ~azure.mgmt.healthcareapis.models.ServiceEventState
     :ivar encryption: The encryption settings of the DICOM service.
     :vartype encryption: ~azure.mgmt.healthcareapis.models.Encryption
+    :ivar storage_configuration: The configuration of external storage account.
+    :vartype storage_configuration: ~azure.mgmt.healthcareapis.models.StorageConfiguration
+    :ivar enable_data_partitions: If data partitions is enabled or not.
+    :vartype enable_data_partitions: bool
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True, "pattern": r"^[a-z0-9][a-z0-9-]{1,21}[a-z0-9]$"},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
@@ -381,27 +385,31 @@
         "private_endpoint_connections": {
             "key": "properties.privateEndpointConnections",
             "type": "[PrivateEndpointConnection]",
         },
         "public_network_access": {"key": "properties.publicNetworkAccess", "type": "str"},
         "event_state": {"key": "properties.eventState", "type": "str"},
         "encryption": {"key": "properties.encryption", "type": "Encryption"},
+        "storage_configuration": {"key": "properties.storageConfiguration", "type": "StorageConfiguration"},
+        "enable_data_partitions": {"key": "properties.enableDataPartitions", "type": "bool"},
     }
 
     def __init__(
         self,
         *,
         identity: Optional["_models.ServiceManagedIdentityIdentity"] = None,
         etag: Optional[str] = None,
         location: Optional[str] = None,
         tags: Optional[Dict[str, str]] = None,
         authentication_configuration: Optional["_models.DicomServiceAuthenticationConfiguration"] = None,
         cors_configuration: Optional["_models.CorsConfiguration"] = None,
         public_network_access: Optional[Union[str, "_models.PublicNetworkAccess"]] = None,
         encryption: Optional["_models.Encryption"] = None,
+        storage_configuration: Optional["_models.StorageConfiguration"] = None,
+        enable_data_partitions: Optional[bool] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword identity: Setting indicating whether the service has a managed identity associated
          with it.
         :paramtype identity: ~azure.mgmt.healthcareapis.models.ServiceManagedIdentityIdentity
         :keyword etag: An etag associated with the resource, used for optimistic concurrency when
@@ -417,26 +425,32 @@
         :keyword cors_configuration: Dicom Service Cors configuration.
         :paramtype cors_configuration: ~azure.mgmt.healthcareapis.models.CorsConfiguration
         :keyword public_network_access: Control permission for data plane traffic coming from public
          networks while private endpoint is enabled. Known values are: "Enabled" and "Disabled".
         :paramtype public_network_access: str or ~azure.mgmt.healthcareapis.models.PublicNetworkAccess
         :keyword encryption: The encryption settings of the DICOM service.
         :paramtype encryption: ~azure.mgmt.healthcareapis.models.Encryption
+        :keyword storage_configuration: The configuration of external storage account.
+        :paramtype storage_configuration: ~azure.mgmt.healthcareapis.models.StorageConfiguration
+        :keyword enable_data_partitions: If data partitions is enabled or not.
+        :paramtype enable_data_partitions: bool
         """
         super().__init__(etag=etag, location=location, tags=tags, identity=identity, **kwargs)
         self.identity = identity
         self.system_data = None
         self.provisioning_state = None
         self.authentication_configuration = authentication_configuration
         self.cors_configuration = cors_configuration
         self.service_url = None
         self.private_endpoint_connections = None
         self.public_network_access = public_network_access
         self.event_state = None
         self.encryption = encryption
+        self.storage_configuration = storage_configuration
+        self.enable_data_partitions = enable_data_partitions
         self.id = None
         self.name = None
         self.type = None
         self.etag = etag
         self.location = location
         self.tags = tags
 
@@ -878,42 +892,53 @@
 
     :ivar authority: The authority url for the service.
     :vartype authority: str
     :ivar audience: The audience url for the service.
     :vartype audience: str
     :ivar smart_proxy_enabled: If the SMART on FHIR proxy is enabled.
     :vartype smart_proxy_enabled: bool
+    :ivar smart_identity_providers: The array of identity provider configurations for SMART on FHIR
+     authentication.
+    :vartype smart_identity_providers:
+     list[~azure.mgmt.healthcareapis.models.SmartIdentityProviderConfiguration]
     """
 
     _attribute_map = {
         "authority": {"key": "authority", "type": "str"},
         "audience": {"key": "audience", "type": "str"},
         "smart_proxy_enabled": {"key": "smartProxyEnabled", "type": "bool"},
+        "smart_identity_providers": {"key": "smartIdentityProviders", "type": "[SmartIdentityProviderConfiguration]"},
     }
 
     def __init__(
         self,
         *,
         authority: Optional[str] = None,
         audience: Optional[str] = None,
         smart_proxy_enabled: Optional[bool] = None,
+        smart_identity_providers: Optional[List["_models.SmartIdentityProviderConfiguration"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword authority: The authority url for the service.
         :paramtype authority: str
         :keyword audience: The audience url for the service.
         :paramtype audience: str
         :keyword smart_proxy_enabled: If the SMART on FHIR proxy is enabled.
         :paramtype smart_proxy_enabled: bool
+        :keyword smart_identity_providers: The array of identity provider configurations for SMART on
+         FHIR authentication.
+        :paramtype smart_identity_providers:
+         list[~azure.mgmt.healthcareapis.models.SmartIdentityProviderConfiguration]
         """
         super().__init__(**kwargs)
         self.authority = authority
         self.audience = audience
         self.smart_proxy_enabled = smart_proxy_enabled
+        self.smart_identity_providers = smart_identity_providers
 
 
 class FhirServiceCollection(_serialization.Model):
     """A collection of Fhir services.
 
     :ivar next_link: The link used to get the next page of Fhir Services.
     :vartype next_link: str
@@ -1295,15 +1320,15 @@
 
     def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.provisioning_state = None
 
 
-class IotEventHubIngestionEndpointConfiguration(_serialization.Model):
+class IotEventHubIngestionEndpointConfiguration(_serialization.Model):  # pylint: disable=name-too-long
     """Event Hub ingestion endpoint configuration.
 
     :ivar event_hub_name: Event Hub name to connect to.
     :vartype event_hub_name: str
     :ivar consumer_group: Consumer group of the event hub to connected to.
     :vartype consumer_group: str
     :ivar fully_qualified_event_hub_namespace: Fully qualified namespace of the Event Hub to
@@ -1341,15 +1366,15 @@
 
 
 class IotFhirDestination(LocationBasedResource):
     """IoT Connector FHIR destination definition.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: The resource identifier.
     :vartype id: str
     :ivar name: The resource name.
     :vartype name: str
     :ivar type: The resource type.
     :vartype type: str
@@ -1466,15 +1491,15 @@
 
 
 class IotFhirDestinationProperties(IotDestinationProperties):
     """IoT Connector destination properties for an Azure FHIR service.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar provisioning_state: The provisioning state. Known values are: "Deleting", "Succeeded",
      "Creating", "Accepted", "Verifying", "Updating", "Failed", "Canceled", "Deprovisioned",
      "Moving", "Suspended", "Warned", and "SystemMaintenance".
     :vartype provisioning_state: str or ~azure.mgmt.healthcareapis.models.ProvisioningState
     :ivar resource_identity_resolution_type: Determines how resource identity is resolved on the
      destination. Required. Known values are: "Create" and "Lookup".
@@ -1989,15 +2014,15 @@
 
 class Resource(_serialization.Model):
     """Common fields that are returned in the response for all Azure Resource Manager resources.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     """
@@ -2024,15 +2049,15 @@
 
 class PrivateEndpointConnection(Resource):
     """The Private Endpoint Connection resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar private_endpoint: The resource of private end point.
@@ -2089,15 +2114,15 @@
 
 class PrivateEndpointConnectionDescription(PrivateEndpointConnection):
     """The Private Endpoint Connection resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar private_endpoint: The resource of private end point.
@@ -2174,15 +2199,15 @@
         :keyword value: Array of private endpoint connections.
         :paramtype value: list[~azure.mgmt.healthcareapis.models.PrivateEndpointConnection]
         """
         super().__init__(**kwargs)
         self.value = value
 
 
-class PrivateEndpointConnectionListResultDescription(_serialization.Model):
+class PrivateEndpointConnectionListResultDescription(_serialization.Model):  # pylint: disable=name-too-long
     """List of private endpoint connection associated with the specified storage account.
 
     :ivar value: Array of private endpoint connections.
     :vartype value: list[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
     """
 
     _attribute_map = {
@@ -2202,15 +2227,15 @@
 
 class PrivateLinkResource(Resource):
     """A private link resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar group_id: The private link resource group id.
@@ -2251,15 +2276,15 @@
 
 class PrivateLinkResourceDescription(PrivateLinkResource):
     """The Private Endpoint Connection resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar group_id: The private link resource group id.
@@ -2403,15 +2428,15 @@
         self.default = default
         self.resource_type_overrides = resource_type_overrides
 
 
 class ServiceAccessPolicyEntry(_serialization.Model):
     """An access policy entry.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar object_id: An Azure AD object ID (User or Apps) that is allowed access to the FHIR
      service. Required.
     :vartype object_id: str
     """
 
     _validation = {
@@ -2671,29 +2696,29 @@
 
 
 class ServiceManagedIdentityIdentity(_serialization.Model):
     """Setting indicating whether the service has a managed identity associated with it.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar type: Type of identity being specified, currently SystemAssigned and None are allowed.
      Required. Known values are: "None", "SystemAssigned", "UserAssigned", and
      "SystemAssigned,UserAssigned".
     :vartype type: str or ~azure.mgmt.healthcareapis.models.ServiceManagedIdentityType
     :ivar principal_id: The service principal ID of the system assigned identity. This property
      will only be provided for a system assigned identity.
     :vartype principal_id: str
     :ivar tenant_id: The tenant ID of the system assigned identity. This property will only be
      provided for a system assigned identity.
     :vartype tenant_id: str
     :ivar user_assigned_identities: The set of user assigned identities associated with the
      resource. The userAssignedIdentities dictionary keys will be ARM resource ids in the form:
-     '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}.
+     '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}.  # pylint: disable=line-too-long
      The dictionary values can be empty objects ({}) in requests.
     :vartype user_assigned_identities: dict[str,
      ~azure.mgmt.healthcareapis.models.UserAssignedIdentity]
     """
 
     _validation = {
         "type": {"required": True},
@@ -2718,15 +2743,15 @@
         """
         :keyword type: Type of identity being specified, currently SystemAssigned and None are allowed.
          Required. Known values are: "None", "SystemAssigned", "UserAssigned", and
          "SystemAssigned,UserAssigned".
         :paramtype type: str or ~azure.mgmt.healthcareapis.models.ServiceManagedIdentityType
         :keyword user_assigned_identities: The set of user assigned identities associated with the
          resource. The userAssignedIdentities dictionary keys will be ARM resource ids in the form:
-         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}.
+         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}.  # pylint: disable=line-too-long
          The dictionary values can be empty objects ({}) in requests.
         :paramtype user_assigned_identities: dict[str,
          ~azure.mgmt.healthcareapis.models.UserAssignedIdentity]
         """
         super().__init__(**kwargs)
         self.type = type
         self.principal_id = None
@@ -2774,15 +2799,15 @@
 
 
 class ServicesResource(_serialization.Model):
     """The common properties of a service.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: The resource identifier.
     :vartype id: str
     :ivar name: The resource name.
     :vartype name: str
     :ivar type: The resource type.
     :vartype type: str
@@ -2857,15 +2882,15 @@
 
 
 class ServicesDescription(ServicesResource):
     """The description of the service.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: The resource identifier.
     :vartype id: str
     :ivar name: The resource name.
     :vartype name: str
     :ivar type: The resource type.
     :vartype type: str
@@ -3222,14 +3247,125 @@
         """
         super().__init__(**kwargs)
         self.principal_id = None
         self.tenant_id = None
         self.type = type
 
 
+class SmartIdentityProviderApplication(_serialization.Model):
+    """An Application configured in the Identity Provider used to access FHIR resources.
+
+    :ivar client_id: The application client id defined in the identity provider. This value will be
+     used to validate bearer tokens against the given authority.
+    :vartype client_id: str
+    :ivar audience: The audience that will be used to validate bearer tokens against the given
+     authority.
+    :vartype audience: str
+    :ivar allowed_data_actions: The actions that are permitted to be performed on FHIR resources
+     for the application.
+    :vartype allowed_data_actions: list[str or ~azure.mgmt.healthcareapis.models.SmartDataActions]
+    """
+
+    _attribute_map = {
+        "client_id": {"key": "clientId", "type": "str"},
+        "audience": {"key": "audience", "type": "str"},
+        "allowed_data_actions": {"key": "allowedDataActions", "type": "[str]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        client_id: Optional[str] = None,
+        audience: Optional[str] = None,
+        allowed_data_actions: Optional[List[Union[str, "_models.SmartDataActions"]]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword client_id: The application client id defined in the identity provider. This value will
+         be used to validate bearer tokens against the given authority.
+        :paramtype client_id: str
+        :keyword audience: The audience that will be used to validate bearer tokens against the given
+         authority.
+        :paramtype audience: str
+        :keyword allowed_data_actions: The actions that are permitted to be performed on FHIR resources
+         for the application.
+        :paramtype allowed_data_actions: list[str or
+         ~azure.mgmt.healthcareapis.models.SmartDataActions]
+        """
+        super().__init__(**kwargs)
+        self.client_id = client_id
+        self.audience = audience
+        self.allowed_data_actions = allowed_data_actions
+
+
+class SmartIdentityProviderConfiguration(_serialization.Model):
+    """An object to configure an identity provider for use with SMART on FHIR authentication.
+
+    :ivar authority: The identity provider token authority also known as the token issuing
+     authority.
+    :vartype authority: str
+    :ivar applications: The array of identity provider applications for SMART on FHIR
+     authentication.
+    :vartype applications: list[~azure.mgmt.healthcareapis.models.SmartIdentityProviderApplication]
+    """
+
+    _attribute_map = {
+        "authority": {"key": "authority", "type": "str"},
+        "applications": {"key": "applications", "type": "[SmartIdentityProviderApplication]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        authority: Optional[str] = None,
+        applications: Optional[List["_models.SmartIdentityProviderApplication"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword authority: The identity provider token authority also known as the token issuing
+         authority.
+        :paramtype authority: str
+        :keyword applications: The array of identity provider applications for SMART on FHIR
+         authentication.
+        :paramtype applications:
+         list[~azure.mgmt.healthcareapis.models.SmartIdentityProviderApplication]
+        """
+        super().__init__(**kwargs)
+        self.authority = authority
+        self.applications = applications
+
+
+class StorageConfiguration(_serialization.Model):
+    """The configuration of connected storage.
+
+    :ivar storage_resource_id: The resource id of connected storage account.
+    :vartype storage_resource_id: str
+    :ivar file_system_name: The filesystem name of connected storage account.
+    :vartype file_system_name: str
+    """
+
+    _attribute_map = {
+        "storage_resource_id": {"key": "storageResourceId", "type": "str"},
+        "file_system_name": {"key": "fileSystemName", "type": "str"},
+    }
+
+    def __init__(
+        self, *, storage_resource_id: Optional[str] = None, file_system_name: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword storage_resource_id: The resource id of connected storage account.
+        :paramtype storage_resource_id: str
+        :keyword file_system_name: The filesystem name of connected storage account.
+        :paramtype file_system_name: str
+        """
+        super().__init__(**kwargs)
+        self.storage_resource_id = storage_resource_id
+        self.file_system_name = file_system_name
+
+
 class SystemData(_serialization.Model):
     """Metadata pertaining to creation and last modification of the resource.
 
     :ivar created_by: The identity that created the resource.
     :vartype created_by: str
     :ivar created_by_type: The type of identity that created the resource. Known values are:
      "User", "Application", "ManagedIdentity", and "Key".
@@ -3416,25 +3552,14 @@
 class WorkspacePatchResource(ResourceTags):
     """Workspace patch properties.
 
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     """
 
-    _attribute_map = {
-        "tags": {"key": "tags", "type": "{str}"},
-    }
-
-    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
-        """
-        :keyword tags: Resource tags.
-        :paramtype tags: dict[str, str]
-        """
-        super().__init__(tags=tags, **kwargs)
-
 
 class WorkspaceProperties(_serialization.Model):
     """Workspaces resource specific properties.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar provisioning_state: The provisioning state. Known values are: "Deleting", "Succeeded",
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/models/_patch.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/__init__.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_dicom_services_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_services_operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -35,860 +35,694 @@
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_list_by_workspace_request(
-    resource_group_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
-) -> HttpRequest:
+def build_get_request(resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_get_request(
-    resource_group_name: str, workspace_name: str, dicom_service_name: str, subscription_id: str, **kwargs: Any
+def build_create_or_update_request(
+    resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
-        "dicomServiceName": _SERIALIZER.url(
-            "dicom_service_name", dicom_service_name, "str", max_length=24, min_length=3
-        ),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_create_or_update_request(
-    resource_group_name: str, workspace_name: str, dicom_service_name: str, subscription_id: str, **kwargs: Any
+def build_update_request(
+    resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
-        "dicomServiceName": _SERIALIZER.url(
-            "dicom_service_name", dicom_service_name, "str", max_length=24, min_length=3
-        ),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
+    return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_update_request(
-    resource_group_name: str, dicom_service_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
+def build_delete_request(
+    resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
-    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
         ),
+        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.HealthcareApis/services")
+    path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "dicomServiceName": _SERIALIZER.url(
-            "dicom_service_name", dicom_service_name, "str", max_length=24, min_length=3
-        ),
-        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_delete_request(
-    resource_group_name: str, dicom_service_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
-) -> HttpRequest:
+def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
         ),
-        "dicomServiceName": _SERIALIZER.url(
-            "dicom_service_name", dicom_service_name, "str", max_length=24, min_length=3
-        ),
-        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_check_name_availability_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.HealthcareApis/checkNameAvailability"
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class DicomServicesOperations:
+class ServicesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.healthcareapis.HealthcareApisManagementClient`'s
-        :attr:`dicom_services` attribute.
+        :attr:`services` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list_by_workspace(
-        self, resource_group_name: str, workspace_name: str, **kwargs: Any
-    ) -> Iterable["_models.DicomService"]:
-        """Lists all DICOM Services for the given workspace.
-
-        :param resource_group_name: The name of the resource group that contains the service instance.
-         Required.
-        :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either DicomService or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.DicomService]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.DicomServiceCollection] = kwargs.pop("cls", None)
-
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        def prepare_request(next_link=None):
-            if not next_link:
-
-                request = build_list_by_workspace_request(
-                    resource_group_name=resource_group_name,
-                    workspace_name=workspace_name,
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list_by_workspace.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        def extract_data(pipeline_response):
-            deserialized = self._deserialize("DicomServiceCollection", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, iter(list_of_elem)
-
-        def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            _stream = False
-            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
-            )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-            return pipeline_response
-
-        return ItemPaged(get_next, extract_data)
-
-    list_by_workspace.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices"
-    }
-
-    @distributed_trace
-    def get(
-        self, resource_group_name: str, workspace_name: str, dicom_service_name: str, **kwargs: Any
-    ) -> _models.DicomService:
-        """Gets the properties of the specified DICOM Service.
+    def get(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> _models.ServicesDescription:
+        """Get the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param dicom_service_name: The name of DICOM Service resource. Required.
-        :type dicom_service_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: DicomService or the result of cls(response)
-        :rtype: ~azure.mgmt.healthcareapis.models.DicomService
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :return: ServicesDescription or the result of cls(response)
+        :rtype: ~azure.mgmt.healthcareapis.models.ServicesDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.DicomService] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
-            workspace_name=workspace_name,
-            dicom_service_name=dicom_service_name,
+            resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("DicomService", pipeline_response)
+        deserialized = self._deserialize("ServicesDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
+        return deserialized  # type: ignore
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
-        workspace_name: str,
-        dicom_service_name: str,
-        dicomservice: Union[_models.DicomService, IO],
+        resource_name: str,
+        service_description: Union[_models.ServicesDescription, IO[bytes]],
         **kwargs: Any
-    ) -> _models.DicomService:
+    ) -> _models.ServicesDescription:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.DicomService] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(dicomservice, (IOBase, bytes)):
-            _content = dicomservice
+        if isinstance(service_description, (IOBase, bytes)):
+            _content = service_description
         else:
-            _json = self._serialize.body(dicomservice, "DicomService")
+            _json = self._serialize.body(service_description, "ServicesDescription")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
-            workspace_name=workspace_name,
-            dicom_service_name=dicom_service_name,
+            resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 201, 202]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if response.status_code == 200:
-            deserialized = self._deserialize("DicomService", pipeline_response)
+            deserialized = self._deserialize("ServicesDescription", pipeline_response)
 
         if response.status_code == 201:
-            deserialized = self._deserialize("DicomService", pipeline_response)
-
-        if response.status_code == 202:
-            deserialized = self._deserialize("DicomService", pipeline_response)
+            deserialized = self._deserialize("ServicesDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
-
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
-        workspace_name: str,
-        dicom_service_name: str,
-        dicomservice: _models.DicomService,
+        resource_name: str,
+        service_description: _models.ServicesDescription,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.DicomService]:
-        """Creates or updates a DICOM Service resource with the specified parameters.
+    ) -> LROPoller[_models.ServicesDescription]:
+        """Create or update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param dicom_service_name: The name of DICOM Service resource. Required.
-        :type dicom_service_name: str
-        :param dicomservice: The parameters for creating or updating a Dicom Service resource.
-         Required.
-        :type dicomservice: ~azure.mgmt.healthcareapis.models.DicomService
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_description: The service instance metadata. Required.
+        :type service_description: ~azure.mgmt.healthcareapis.models.ServicesDescription
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either DicomService or the result of
+        :return: An instance of LROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.DicomService]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
-        workspace_name: str,
-        dicom_service_name: str,
-        dicomservice: IO,
+        resource_name: str,
+        service_description: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.DicomService]:
-        """Creates or updates a DICOM Service resource with the specified parameters.
+    ) -> LROPoller[_models.ServicesDescription]:
+        """Create or update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param dicom_service_name: The name of DICOM Service resource. Required.
-        :type dicom_service_name: str
-        :param dicomservice: The parameters for creating or updating a Dicom Service resource.
-         Required.
-        :type dicomservice: IO
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_description: The service instance metadata. Required.
+        :type service_description: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either DicomService or the result of
+        :return: An instance of LROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.DicomService]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
-        workspace_name: str,
-        dicom_service_name: str,
-        dicomservice: Union[_models.DicomService, IO],
+        resource_name: str,
+        service_description: Union[_models.ServicesDescription, IO[bytes]],
         **kwargs: Any
-    ) -> LROPoller[_models.DicomService]:
-        """Creates or updates a DICOM Service resource with the specified parameters.
+    ) -> LROPoller[_models.ServicesDescription]:
+        """Create or update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param dicom_service_name: The name of DICOM Service resource. Required.
-        :type dicom_service_name: str
-        :param dicomservice: The parameters for creating or updating a Dicom Service resource. Is
-         either a DicomService type or a IO type. Required.
-        :type dicomservice: ~azure.mgmt.healthcareapis.models.DicomService or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either DicomService or the result of
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_description: The service instance metadata. Is either a ServicesDescription type
+         or a IO[bytes] type. Required.
+        :type service_description: ~azure.mgmt.healthcareapis.models.ServicesDescription or IO[bytes]
+        :return: An instance of LROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.DicomService]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.DicomService] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
-                workspace_name=workspace_name,
-                dicom_service_name=dicom_service_name,
-                dicomservice=dicomservice,
+                resource_name=resource_name,
+                service_description=service_description,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("DicomService", pipeline_response)
+            deserialized = self._deserialize("ServicesDescription", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.ServicesDescription].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
+        return LROPoller[_models.ServicesDescription](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _update_initial(
         self,
         resource_group_name: str,
-        dicom_service_name: str,
-        workspace_name: str,
-        dicomservice_patch_resource: Union[_models.DicomServicePatchResource, IO],
+        resource_name: str,
+        service_patch_description: Union[_models.ServicesPatchDescription, IO[bytes]],
         **kwargs: Any
-    ) -> _models.DicomService:
+    ) -> _models.ServicesDescription:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.DicomService] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(dicomservice_patch_resource, (IOBase, bytes)):
-            _content = dicomservice_patch_resource
+        if isinstance(service_patch_description, (IOBase, bytes)):
+            _content = service_patch_description
         else:
-            _json = self._serialize.body(dicomservice_patch_resource, "DicomServicePatchResource")
+            _json = self._serialize.body(service_patch_description, "ServicesPatchDescription")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
-            dicom_service_name=dicom_service_name,
-            workspace_name=workspace_name,
+            resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202]:
+        if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        if response.status_code == 200:
-            deserialized = self._deserialize("DicomService", pipeline_response)
-
-        if response.status_code == 202:
-            deserialized = self._deserialize("DicomService", pipeline_response)
+        deserialized = self._deserialize("ServicesDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
-
     @overload
     def begin_update(
         self,
         resource_group_name: str,
-        dicom_service_name: str,
-        workspace_name: str,
-        dicomservice_patch_resource: _models.DicomServicePatchResource,
+        resource_name: str,
+        service_patch_description: _models.ServicesPatchDescription,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.DicomService]:
-        """Patch DICOM Service details.
+    ) -> LROPoller[_models.ServicesDescription]:
+        """Update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param dicom_service_name: The name of DICOM Service resource. Required.
-        :type dicom_service_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param dicomservice_patch_resource: The parameters for updating a Dicom Service. Required.
-        :type dicomservice_patch_resource: ~azure.mgmt.healthcareapis.models.DicomServicePatchResource
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_patch_description: The service instance metadata and security metadata.
+         Required.
+        :type service_patch_description: ~azure.mgmt.healthcareapis.models.ServicesPatchDescription
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either DicomService or the result of
+        :return: An instance of LROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.DicomService]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
-        dicom_service_name: str,
-        workspace_name: str,
-        dicomservice_patch_resource: IO,
+        resource_name: str,
+        service_patch_description: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.DicomService]:
-        """Patch DICOM Service details.
+    ) -> LROPoller[_models.ServicesDescription]:
+        """Update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param dicom_service_name: The name of DICOM Service resource. Required.
-        :type dicom_service_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param dicomservice_patch_resource: The parameters for updating a Dicom Service. Required.
-        :type dicomservice_patch_resource: IO
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_patch_description: The service instance metadata and security metadata.
+         Required.
+        :type service_patch_description: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either DicomService or the result of
+        :return: An instance of LROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.DicomService]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_update(
         self,
         resource_group_name: str,
-        dicom_service_name: str,
-        workspace_name: str,
-        dicomservice_patch_resource: Union[_models.DicomServicePatchResource, IO],
+        resource_name: str,
+        service_patch_description: Union[_models.ServicesPatchDescription, IO[bytes]],
         **kwargs: Any
-    ) -> LROPoller[_models.DicomService]:
-        """Patch DICOM Service details.
+    ) -> LROPoller[_models.ServicesDescription]:
+        """Update the metadata of a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param dicom_service_name: The name of DICOM Service resource. Required.
-        :type dicom_service_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :param dicomservice_patch_resource: The parameters for updating a Dicom Service. Is either a
-         DicomServicePatchResource type or a IO type. Required.
-        :type dicomservice_patch_resource: ~azure.mgmt.healthcareapis.models.DicomServicePatchResource
-         or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either DicomService or the result of
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
+        :param service_patch_description: The service instance metadata and security metadata. Is
+         either a ServicesPatchDescription type or a IO[bytes] type. Required.
+        :type service_patch_description: ~azure.mgmt.healthcareapis.models.ServicesPatchDescription or
+         IO[bytes]
+        :return: An instance of LROPoller that returns either ServicesDescription or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.DicomService]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.ServicesDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.DicomService] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ServicesDescription] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._update_initial(
                 resource_group_name=resource_group_name,
-                dicom_service_name=dicom_service_name,
-                workspace_name=workspace_name,
-                dicomservice_patch_resource=dicomservice_patch_resource,
+                resource_name=resource_name,
+                service_patch_description=service_patch_description,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("DicomService", pipeline_response)
+            deserialized = self._deserialize("ServicesDescription", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.ServicesDescription].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
+        return LROPoller[_models.ServicesDescription](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, dicom_service_name: str, workspace_name: str, **kwargs: Any
+        self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -896,67 +730,49 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
-            dicom_service_name=dicom_service_name,
-            workspace_name=workspace_name,
+            resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202, 204]:
+        if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace
-    def begin_delete(
-        self, resource_group_name: str, dicom_service_name: str, workspace_name: str, **kwargs: Any
-    ) -> LROPoller[None]:
-        """Deletes a DICOM Service.
+    def begin_delete(self, resource_group_name: str, resource_name: str, **kwargs: Any) -> LROPoller[None]:
+        """Delete a service instance.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param dicom_service_name: The name of DICOM Service resource. Required.
-        :type dicom_service_name: str
-        :param workspace_name: The name of workspace resource. Required.
-        :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param resource_name: The name of the service instance. Required.
+        :type resource_name: str
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -964,39 +780,304 @@
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
-                dicom_service_name=dicom_service_name,
-                workspace_name=workspace_name,
+                resource_name=resource_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/dicomservices/{dicomServiceName}"
-    }
+    @distributed_trace
+    def list(self, **kwargs: Any) -> Iterable["_models.ServicesDescription"]:
+        """Get all the service instances in a subscription.
+
+        :return: An iterator like instance of either ServicesDescription or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.ServicesDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ServicesDescriptionListResult] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                _request = build_list_request(
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("ServicesDescriptionListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, iter(list_of_elem)
+
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+            return pipeline_response
+
+        return ItemPaged(get_next, extract_data)
+
+    @distributed_trace
+    def list_by_resource_group(
+        self, resource_group_name: str, **kwargs: Any
+    ) -> Iterable["_models.ServicesDescription"]:
+        """Get all the service instances in a resource group.
+
+        :param resource_group_name: The name of the resource group that contains the service instance.
+         Required.
+        :type resource_group_name: str
+        :return: An iterator like instance of either ServicesDescription or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.ServicesDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ServicesDescriptionListResult] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                _request = build_list_by_resource_group_request(
+                    resource_group_name=resource_group_name,
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("ServicesDescriptionListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, iter(list_of_elem)
+
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+            return pipeline_response
+
+        return ItemPaged(get_next, extract_data)
+
+    @overload
+    def check_name_availability(
+        self,
+        check_name_availability_inputs: _models.CheckNameAvailabilityParameters,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.ServicesNameAvailabilityInfo:
+        """Check if a service instance name is available.
+
+        :param check_name_availability_inputs: Set the name parameter in the
+         CheckNameAvailabilityParameters structure to the name of the service instance to check.
+         Required.
+        :type check_name_availability_inputs:
+         ~azure.mgmt.healthcareapis.models.CheckNameAvailabilityParameters
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: ServicesNameAvailabilityInfo or the result of cls(response)
+        :rtype: ~azure.mgmt.healthcareapis.models.ServicesNameAvailabilityInfo
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def check_name_availability(
+        self, check_name_availability_inputs: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.ServicesNameAvailabilityInfo:
+        """Check if a service instance name is available.
+
+        :param check_name_availability_inputs: Set the name parameter in the
+         CheckNameAvailabilityParameters structure to the name of the service instance to check.
+         Required.
+        :type check_name_availability_inputs: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: ServicesNameAvailabilityInfo or the result of cls(response)
+        :rtype: ~azure.mgmt.healthcareapis.models.ServicesNameAvailabilityInfo
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def check_name_availability(
+        self, check_name_availability_inputs: Union[_models.CheckNameAvailabilityParameters, IO[bytes]], **kwargs: Any
+    ) -> _models.ServicesNameAvailabilityInfo:
+        """Check if a service instance name is available.
+
+        :param check_name_availability_inputs: Set the name parameter in the
+         CheckNameAvailabilityParameters structure to the name of the service instance to check. Is
+         either a CheckNameAvailabilityParameters type or a IO[bytes] type. Required.
+        :type check_name_availability_inputs:
+         ~azure.mgmt.healthcareapis.models.CheckNameAvailabilityParameters or IO[bytes]
+        :return: ServicesNameAvailabilityInfo or the result of cls(response)
+        :rtype: ~azure.mgmt.healthcareapis.models.ServicesNameAvailabilityInfo
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.ServicesNameAvailabilityInfo] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(check_name_availability_inputs, (IOBase, bytes)):
+            _content = check_name_availability_inputs
+        else:
+            _json = self._serialize.body(check_name_availability_inputs, "CheckNameAvailabilityParameters")
+
+        _request = build_check_name_availability_request(
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("ServicesNameAvailabilityInfo", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_fhir_destinations_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_fhir_destinations_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -38,15 +38,15 @@
 
 def build_list_by_iot_connector_request(
     resource_group_name: str, workspace_name: str, iot_connector_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations",
     )  # pylint: disable=line-too-long
@@ -100,15 +100,14 @@
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either IotFhirDestination or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.IotFhirDestination]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -122,66 +121,61 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_iot_connector_request(
+                _request = build_list_by_iot_connector_request(
                     resource_group_name=resource_group_name,
                     workspace_name=workspace_name,
                     iot_connector_name=iot_connector_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_iot_connector.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("IotFhirDestinationCollection", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list_by_iot_connector.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations"
-    }
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_fhir_services_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_fhir_services_operations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -41,15 +41,15 @@
 
 def build_list_by_workspace_request(
     resource_group_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices",
     )  # pylint: disable=line-too-long
@@ -74,15 +74,15 @@
 
 def build_get_request(
     resource_group_name: str, workspace_name: str, fhir_service_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}",
     )  # pylint: disable=line-too-long
@@ -108,15 +108,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, workspace_name: str, fhir_service_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}",
@@ -145,15 +145,15 @@
 
 def build_update_request(
     resource_group_name: str, fhir_service_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}",
@@ -182,15 +182,15 @@
 
 def build_delete_request(
     resource_group_name: str, fhir_service_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}",
     )  # pylint: disable=line-too-long
@@ -240,15 +240,14 @@
         """Lists all FHIR Services for the given workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either FhirService or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -262,87 +261,81 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_workspace_request(
+                _request = build_list_by_workspace_request(
                     resource_group_name=resource_group_name,
                     workspace_name=workspace_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_workspace.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("FhirServiceCollection", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_workspace.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices"
-    }
-
     @distributed_trace
     def get(
         self, resource_group_name: str, workspace_name: str, fhir_service_name: str, **kwargs: Any
     ) -> _models.FhirService:
         """Gets the properties of the specified FHIR Service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: FhirService or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.FhirService
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -353,56 +346,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.FhirService] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             fhir_service_name=fhir_service_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("FhirService", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
+        return deserialized  # type: ignore
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         workspace_name: str,
         fhir_service_name: str,
-        fhirservice: Union[_models.FhirService, IO],
+        fhirservice: Union[_models.FhirService, IO[bytes]],
         **kwargs: Any
     ) -> _models.FhirService:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -420,33 +408,32 @@
         _json = None
         _content = None
         if isinstance(fhirservice, (IOBase, bytes)):
             _content = fhirservice
         else:
             _json = self._serialize.body(fhirservice, "FhirService")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             fhir_service_name=fhir_service_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
@@ -462,18 +449,14 @@
             deserialized = self._deserialize("FhirService", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
-
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         fhir_service_name: str,
         fhirservice: _models.FhirService,
@@ -491,99 +474,72 @@
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param fhirservice: The parameters for creating or updating a Fhir Service resource. Required.
         :type fhirservice: ~azure.mgmt.healthcareapis.models.FhirService
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         fhir_service_name: str,
-        fhirservice: IO,
+        fhirservice: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.FhirService]:
         """Creates or updates a FHIR Service resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param fhirservice: The parameters for creating or updating a Fhir Service resource. Required.
-        :type fhirservice: IO
+        :type fhirservice: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         fhir_service_name: str,
-        fhirservice: Union[_models.FhirService, IO],
+        fhirservice: Union[_models.FhirService, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.FhirService]:
         """Creates or updates a FHIR Service resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param fhirservice: The parameters for creating or updating a Fhir Service resource. Is either
-         a FhirService type or a IO type. Required.
-        :type fhirservice: ~azure.mgmt.healthcareapis.models.FhirService or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         a FhirService type or a IO[bytes] type. Required.
+        :type fhirservice: ~azure.mgmt.healthcareapis.models.FhirService or IO[bytes]
         :return: An instance of LROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -608,42 +564,40 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("FhirService", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.FhirService].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
+        return LROPoller[_models.FhirService](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _update_initial(
         self,
         resource_group_name: str,
         fhir_service_name: str,
         workspace_name: str,
-        fhirservice_patch_resource: Union[_models.FhirServicePatchResource, IO],
+        fhirservice_patch_resource: Union[_models.FhirServicePatchResource, IO[bytes]],
         **kwargs: Any
     ) -> _models.FhirService:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -661,33 +615,32 @@
         _json = None
         _content = None
         if isinstance(fhirservice_patch_resource, (IOBase, bytes)):
             _content = fhirservice_patch_resource
         else:
             _json = self._serialize.body(fhirservice_patch_resource, "FhirServicePatchResource")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             fhir_service_name=fhir_service_name,
             workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
@@ -700,18 +653,14 @@
             deserialized = self._deserialize("FhirService", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
-
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         fhir_service_name: str,
         workspace_name: str,
         fhirservice_patch_resource: _models.FhirServicePatchResource,
@@ -729,100 +678,73 @@
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhirservice_patch_resource: The parameters for updating a Fhir Service. Required.
         :type fhirservice_patch_resource: ~azure.mgmt.healthcareapis.models.FhirServicePatchResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         fhir_service_name: str,
         workspace_name: str,
-        fhirservice_patch_resource: IO,
+        fhirservice_patch_resource: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.FhirService]:
         """Patch FHIR Service details.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhirservice_patch_resource: The parameters for updating a Fhir Service. Required.
-        :type fhirservice_patch_resource: IO
+        :type fhirservice_patch_resource: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_update(
         self,
         resource_group_name: str,
         fhir_service_name: str,
         workspace_name: str,
-        fhirservice_patch_resource: Union[_models.FhirServicePatchResource, IO],
+        fhirservice_patch_resource: Union[_models.FhirServicePatchResource, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.FhirService]:
         """Patch FHIR Service details.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param fhirservice_patch_resource: The parameters for updating a Fhir Service. Is either a
-         FhirServicePatchResource type or a IO type. Required.
+         FhirServicePatchResource type or a IO[bytes] type. Required.
         :type fhirservice_patch_resource: ~azure.mgmt.healthcareapis.models.FhirServicePatchResource or
-         IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         IO[bytes]
         :return: An instance of LROPoller that returns either FhirService or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.FhirService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -847,35 +769,33 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("FhirService", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.FhirService].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
+        return LROPoller[_models.FhirService](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, fhir_service_name: str, workspace_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -886,67 +806,54 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             fhir_service_name=fhir_service_name,
             workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, fhir_service_name: str, workspace_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Deletes a FHIR Service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param fhir_service_name: The name of FHIR Service resource. Required.
         :type fhir_service_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -966,27 +873,23 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/fhirservices/{fhirServiceName}"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_iot_connector_fhir_destination_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_workspace_private_endpoint_connections_operations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
+import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
@@ -33,44 +35,73 @@
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
+def build_list_by_workspace_request(
+    resource_group_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateEndpointConnections",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
+        ),
+        "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 def build_get_request(
     resource_group_name: str,
     workspace_name: str,
-    iot_connector_name: str,
-    fhir_destination_name: str,
+    private_endpoint_connection_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateEndpointConnections/{privateEndpointConnectionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
-        "iotConnectorName": _SERIALIZER.url(
-            "iot_connector_name", iot_connector_name, "str", max_length=24, min_length=3
-        ),
-        "fhirDestinationName": _SERIALIZER.url(
-            "fhir_destination_name", fhir_destination_name, "str", max_length=24, min_length=3
+        "privateEndpointConnectionName": _SERIALIZER.url(
+            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
         ),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -80,42 +111,38 @@
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_or_update_request(
     resource_group_name: str,
     workspace_name: str,
-    iot_connector_name: str,
-    fhir_destination_name: str,
+    private_endpoint_connection_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateEndpointConnections/{privateEndpointConnectionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
         ),
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
-        "iotConnectorName": _SERIALIZER.url(
-            "iot_connector_name", iot_connector_name, "str", max_length=24, min_length=3
-        ),
-        "fhirDestinationName": _SERIALIZER.url(
-            "fhir_destination_name", fhir_destination_name, "str", max_length=24, min_length=3
+        "privateEndpointConnectionName": _SERIALIZER.url(
+            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
         ),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -127,412 +154,430 @@
 
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_delete_request(
     resource_group_name: str,
     workspace_name: str,
-    iot_connector_name: str,
-    fhir_destination_name: str,
+    private_endpoint_connection_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateEndpointConnections/{privateEndpointConnectionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
         ),
         "workspaceName": _SERIALIZER.url("workspace_name", workspace_name, "str", max_length=24, min_length=3),
-        "iotConnectorName": _SERIALIZER.url(
-            "iot_connector_name", iot_connector_name, "str", max_length=24, min_length=3
-        ),
-        "fhirDestinationName": _SERIALIZER.url(
-            "fhir_destination_name", fhir_destination_name, "str", max_length=24, min_length=3
+        "privateEndpointConnectionName": _SERIALIZER.url(
+            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
         ),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class IotConnectorFhirDestinationOperations:
+class WorkspacePrivateEndpointConnectionsOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.healthcareapis.HealthcareApisManagementClient`'s
-        :attr:`iot_connector_fhir_destination` attribute.
+        :attr:`workspace_private_endpoint_connections` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
+    def list_by_workspace(
+        self, resource_group_name: str, workspace_name: str, **kwargs: Any
+    ) -> Iterable["_models.PrivateEndpointConnectionDescription"]:
+        """Lists all private endpoint connections for a workspace.
+
+        :param resource_group_name: The name of the resource group that contains the service instance.
+         Required.
+        :type resource_group_name: str
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
+        :return: An iterator like instance of either PrivateEndpointConnectionDescription or the result
+         of cls(response)
+        :rtype:
+         ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.PrivateEndpointConnectionListResultDescription] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                _request = build_list_by_workspace_request(
+                    resource_group_name=resource_group_name,
+                    workspace_name=workspace_name,
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("PrivateEndpointConnectionListResultDescription", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return None, iter(list_of_elem)
+
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+            return pipeline_response
+
+        return ItemPaged(get_next, extract_data)
+
+    @distributed_trace
     def get(
-        self,
-        resource_group_name: str,
-        workspace_name: str,
-        iot_connector_name: str,
-        fhir_destination_name: str,
-        **kwargs: Any
-    ) -> _models.IotFhirDestination:
-        """Gets the properties of the specified Iot Connector FHIR destination.
+        self, resource_group_name: str, workspace_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    ) -> _models.PrivateEndpointConnectionDescription:
+        """Gets the specified private endpoint connection associated with the workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :param iot_connector_name: The name of IoT Connector resource. Required.
-        :type iot_connector_name: str
-        :param fhir_destination_name: The name of IoT Connector FHIR destination resource. Required.
-        :type fhir_destination_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: IotFhirDestination or the result of cls(response)
-        :rtype: ~azure.mgmt.healthcareapis.models.IotFhirDestination
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
+        :type private_endpoint_connection_name: str
+        :return: PrivateEndpointConnectionDescription or the result of cls(response)
+        :rtype: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.IotFhirDestination] = kwargs.pop("cls", None)
+        cls: ClsType[_models.PrivateEndpointConnectionDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
-            iot_connector_name=iot_connector_name,
-            fhir_destination_name=fhir_destination_name,
+            private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("IotFhirDestination", pipeline_response)
+        deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}"
-    }
+        return deserialized  # type: ignore
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         workspace_name: str,
-        iot_connector_name: str,
-        fhir_destination_name: str,
-        iot_fhir_destination: Union[_models.IotFhirDestination, IO],
+        private_endpoint_connection_name: str,
+        properties: Union[_models.PrivateEndpointConnectionDescription, IO[bytes]],
         **kwargs: Any
-    ) -> _models.IotFhirDestination:
+    ) -> _models.PrivateEndpointConnectionDescription:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.IotFhirDestination] = kwargs.pop("cls", None)
+        cls: ClsType[_models.PrivateEndpointConnectionDescription] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(iot_fhir_destination, (IOBase, bytes)):
-            _content = iot_fhir_destination
+        if isinstance(properties, (IOBase, bytes)):
+            _content = properties
         else:
-            _json = self._serialize.body(iot_fhir_destination, "IotFhirDestination")
+            _json = self._serialize.body(properties, "PrivateEndpointConnectionDescription")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
-            iot_connector_name=iot_connector_name,
-            fhir_destination_name=fhir_destination_name,
+            private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 201, 202]:
+        if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        if response.status_code == 200:
-            deserialized = self._deserialize("IotFhirDestination", pipeline_response)
-
-        if response.status_code == 201:
-            deserialized = self._deserialize("IotFhirDestination", pipeline_response)
-
-        if response.status_code == 202:
-            deserialized = self._deserialize("IotFhirDestination", pipeline_response)
+        deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}"
-    }
-
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
-        iot_connector_name: str,
-        fhir_destination_name: str,
-        iot_fhir_destination: _models.IotFhirDestination,
+        private_endpoint_connection_name: str,
+        properties: _models.PrivateEndpointConnectionDescription,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.IotFhirDestination]:
-        """Creates or updates an IoT Connector FHIR destination resource with the specified parameters.
+    ) -> LROPoller[_models.PrivateEndpointConnectionDescription]:
+        """Update the state of the specified private endpoint connection associated with the workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :param iot_connector_name: The name of IoT Connector resource. Required.
-        :type iot_connector_name: str
-        :param fhir_destination_name: The name of IoT Connector FHIR destination resource. Required.
-        :type fhir_destination_name: str
-        :param iot_fhir_destination: The parameters for creating or updating an IoT Connector FHIR
-         destination resource. Required.
-        :type iot_fhir_destination: ~azure.mgmt.healthcareapis.models.IotFhirDestination
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
+        :type private_endpoint_connection_name: str
+        :param properties: The private endpoint connection properties. Required.
+        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either IotFhirDestination or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotFhirDestination]
+        :return: An instance of LROPoller that returns either PrivateEndpointConnectionDescription or
+         the result of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
-        iot_connector_name: str,
-        fhir_destination_name: str,
-        iot_fhir_destination: IO,
+        private_endpoint_connection_name: str,
+        properties: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.IotFhirDestination]:
-        """Creates or updates an IoT Connector FHIR destination resource with the specified parameters.
+    ) -> LROPoller[_models.PrivateEndpointConnectionDescription]:
+        """Update the state of the specified private endpoint connection associated with the workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :param iot_connector_name: The name of IoT Connector resource. Required.
-        :type iot_connector_name: str
-        :param fhir_destination_name: The name of IoT Connector FHIR destination resource. Required.
-        :type fhir_destination_name: str
-        :param iot_fhir_destination: The parameters for creating or updating an IoT Connector FHIR
-         destination resource. Required.
-        :type iot_fhir_destination: IO
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
+        :type private_endpoint_connection_name: str
+        :param properties: The private endpoint connection properties. Required.
+        :type properties: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either IotFhirDestination or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotFhirDestination]
+        :return: An instance of LROPoller that returns either PrivateEndpointConnectionDescription or
+         the result of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
-        iot_connector_name: str,
-        fhir_destination_name: str,
-        iot_fhir_destination: Union[_models.IotFhirDestination, IO],
+        private_endpoint_connection_name: str,
+        properties: Union[_models.PrivateEndpointConnectionDescription, IO[bytes]],
         **kwargs: Any
-    ) -> LROPoller[_models.IotFhirDestination]:
-        """Creates or updates an IoT Connector FHIR destination resource with the specified parameters.
+    ) -> LROPoller[_models.PrivateEndpointConnectionDescription]:
+        """Update the state of the specified private endpoint connection associated with the workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :param iot_connector_name: The name of IoT Connector resource. Required.
-        :type iot_connector_name: str
-        :param fhir_destination_name: The name of IoT Connector FHIR destination resource. Required.
-        :type fhir_destination_name: str
-        :param iot_fhir_destination: The parameters for creating or updating an IoT Connector FHIR
-         destination resource. Is either a IotFhirDestination type or a IO type. Required.
-        :type iot_fhir_destination: ~azure.mgmt.healthcareapis.models.IotFhirDestination or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either IotFhirDestination or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotFhirDestination]
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
+        :type private_endpoint_connection_name: str
+        :param properties: The private endpoint connection properties. Is either a
+         PrivateEndpointConnectionDescription type or a IO[bytes] type. Required.
+        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription or
+         IO[bytes]
+        :return: An instance of LROPoller that returns either PrivateEndpointConnectionDescription or
+         the result of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.IotFhirDestination] = kwargs.pop("cls", None)
+        cls: ClsType[_models.PrivateEndpointConnectionDescription] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 workspace_name=workspace_name,
-                iot_connector_name=iot_connector_name,
-                fhir_destination_name=fhir_destination_name,
-                iot_fhir_destination=iot_fhir_destination,
+                private_endpoint_connection_name=private_endpoint_connection_name,
+                properties=properties,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("IotFhirDestination", pipeline_response)
+            deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.PrivateEndpointConnectionDescription].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}"
-    }
+        return LROPoller[_models.PrivateEndpointConnectionDescription](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self,
-        resource_group_name: str,
-        workspace_name: str,
-        iot_connector_name: str,
-        fhir_destination_name: str,
-        **kwargs: Any
+        self, resource_group_name: str, workspace_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -540,75 +585,55 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
-            iot_connector_name=iot_connector_name,
-            fhir_destination_name=fhir_destination_name,
+            private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace
     def begin_delete(
-        self,
-        resource_group_name: str,
-        workspace_name: str,
-        iot_connector_name: str,
-        fhir_destination_name: str,
-        **kwargs: Any
+        self, resource_group_name: str, workspace_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> LROPoller[None]:
-        """Deletes an IoT Connector FHIR destination.
+        """Deletes a private endpoint connection.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :param iot_connector_name: The name of IoT Connector resource. Required.
-        :type iot_connector_name: str
-        :param fhir_destination_name: The name of IoT Connector FHIR destination resource. Required.
-        :type fhir_destination_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param private_endpoint_connection_name: The name of the private endpoint connection associated
+         with the Azure resource. Required.
+        :type private_endpoint_connection_name: str
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -617,39 +642,34 @@
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 workspace_name=workspace_name,
-                iot_connector_name=iot_connector_name,
-                fhir_destination_name=fhir_destination_name,
+                private_endpoint_connection_name=private_endpoint_connection_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}/fhirdestinations/{fhirDestinationName}"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_iot_connectors_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_iot_connectors_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -41,15 +41,15 @@
 
 def build_list_by_workspace_request(
     resource_group_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors",
     )  # pylint: disable=line-too-long
@@ -74,15 +74,15 @@
 
 def build_get_request(
     resource_group_name: str, workspace_name: str, iot_connector_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}",
     )  # pylint: disable=line-too-long
@@ -110,15 +110,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, workspace_name: str, iot_connector_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}",
@@ -149,15 +149,15 @@
 
 def build_update_request(
     resource_group_name: str, iot_connector_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}",
@@ -188,15 +188,15 @@
 
 def build_delete_request(
     resource_group_name: str, iot_connector_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}",
     )  # pylint: disable=line-too-long
@@ -248,15 +248,14 @@
         """Lists all IoT Connectors for the given workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either IotConnector or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -270,87 +269,81 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_workspace_request(
+                _request = build_list_by_workspace_request(
                     resource_group_name=resource_group_name,
                     workspace_name=workspace_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_workspace.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("IotConnectorCollection", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_workspace.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors"
-    }
-
     @distributed_trace
     def get(
         self, resource_group_name: str, workspace_name: str, iot_connector_name: str, **kwargs: Any
     ) -> _models.IotConnector:
         """Gets the properties of the specified IoT Connector.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: IotConnector or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.IotConnector
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -361,56 +354,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.IotConnector] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             iot_connector_name=iot_connector_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("IotConnector", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
+        return deserialized  # type: ignore
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
-        iot_connector: Union[_models.IotConnector, IO],
+        iot_connector: Union[_models.IotConnector, IO[bytes]],
         **kwargs: Any
     ) -> _models.IotConnector:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -428,33 +416,32 @@
         _json = None
         _content = None
         if isinstance(iot_connector, (IOBase, bytes)):
             _content = iot_connector
         else:
             _json = self._serialize.body(iot_connector, "IotConnector")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             iot_connector_name=iot_connector_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
@@ -470,18 +457,14 @@
             deserialized = self._deserialize("IotConnector", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
-
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
         iot_connector: _models.IotConnector,
@@ -500,35 +483,27 @@
         :type iot_connector_name: str
         :param iot_connector: The parameters for creating or updating an IoT Connectors resource.
          Required.
         :type iot_connector: ~azure.mgmt.healthcareapis.models.IotConnector
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
-        iot_connector: IO,
+        iot_connector: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.IotConnector]:
         """Creates or updates an IoT Connector resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
@@ -536,64 +511,45 @@
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param iot_connector: The parameters for creating or updating an IoT Connectors resource.
          Required.
-        :type iot_connector: IO
+        :type iot_connector: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
         workspace_name: str,
         iot_connector_name: str,
-        iot_connector: Union[_models.IotConnector, IO],
+        iot_connector: Union[_models.IotConnector, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.IotConnector]:
         """Creates or updates an IoT Connector resource with the specified parameters.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param iot_connector: The parameters for creating or updating an IoT Connectors resource. Is
-         either a IotConnector type or a IO type. Required.
-        :type iot_connector: ~azure.mgmt.healthcareapis.models.IotConnector or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         either a IotConnector type or a IO[bytes] type. Required.
+        :type iot_connector: ~azure.mgmt.healthcareapis.models.IotConnector or IO[bytes]
         :return: An instance of LROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -618,42 +574,40 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("IotConnector", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.IotConnector].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
+        return LROPoller[_models.IotConnector](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _update_initial(
         self,
         resource_group_name: str,
         iot_connector_name: str,
         workspace_name: str,
-        iot_connector_patch_resource: Union[_models.IotConnectorPatchResource, IO],
+        iot_connector_patch_resource: Union[_models.IotConnectorPatchResource, IO[bytes]],
         **kwargs: Any
     ) -> _models.IotConnector:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -671,33 +625,32 @@
         _json = None
         _content = None
         if isinstance(iot_connector_patch_resource, (IOBase, bytes)):
             _content = iot_connector_patch_resource
         else:
             _json = self._serialize.body(iot_connector_patch_resource, "IotConnectorPatchResource")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             iot_connector_name=iot_connector_name,
             workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
@@ -710,18 +663,14 @@
             deserialized = self._deserialize("IotConnector", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
-
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         iot_connector_name: str,
         workspace_name: str,
         iot_connector_patch_resource: _models.IotConnectorPatchResource,
@@ -739,100 +688,73 @@
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_patch_resource: The parameters for updating an IoT Connector. Required.
         :type iot_connector_patch_resource: ~azure.mgmt.healthcareapis.models.IotConnectorPatchResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         iot_connector_name: str,
         workspace_name: str,
-        iot_connector_patch_resource: IO,
+        iot_connector_patch_resource: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.IotConnector]:
         """Patch an IoT Connector.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_patch_resource: The parameters for updating an IoT Connector. Required.
-        :type iot_connector_patch_resource: IO
+        :type iot_connector_patch_resource: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_update(
         self,
         resource_group_name: str,
         iot_connector_name: str,
         workspace_name: str,
-        iot_connector_patch_resource: Union[_models.IotConnectorPatchResource, IO],
+        iot_connector_patch_resource: Union[_models.IotConnectorPatchResource, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.IotConnector]:
         """Patch an IoT Connector.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param iot_connector_patch_resource: The parameters for updating an IoT Connector. Is either a
-         IotConnectorPatchResource type or a IO type. Required.
+         IotConnectorPatchResource type or a IO[bytes] type. Required.
         :type iot_connector_patch_resource: ~azure.mgmt.healthcareapis.models.IotConnectorPatchResource
-         or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         or IO[bytes]
         :return: An instance of LROPoller that returns either IotConnector or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.IotConnector]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -857,35 +779,33 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("IotConnector", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.IotConnector].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
+        return LROPoller[_models.IotConnector](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, iot_connector_name: str, workspace_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -896,67 +816,54 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             iot_connector_name=iot_connector_name,
             workspace_name=workspace_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.Error, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, iot_connector_name: str, workspace_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Deletes an IoT Connector.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param iot_connector_name: The name of IoT Connector resource. Required.
         :type iot_connector_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -976,27 +883,23 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/iotconnectors/{iotConnectorName}"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_operation_results_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_operation_results_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -34,15 +34,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(location_name: str, operation_result_id: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.HealthcareApis/locations/{locationName}/operationresults/{operationResultId}",
     )  # pylint: disable=line-too-long
@@ -86,15 +86,14 @@
     def get(self, location_name: str, operation_result_id: str, **kwargs: Any) -> _models.OperationResultsDescription:
         """Get the operation result for a long running operation.
 
         :param location_name: The location of the operation. Required.
         :type location_name: str
         :param operation_result_id: The ID of the operation result to get. Required.
         :type operation_result_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: OperationResultsDescription or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.OperationResultsDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -105,41 +104,36 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationResultsDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             location_name=location_name,
             operation_result_id=operation_result_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("OperationResultsDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HealthcareApis/locations/{locationName}/operationresults/{operationResultId}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -36,15 +36,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.HealthcareApis/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -74,15 +74,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.OperationDetail"]:
         """Lists all of the available operations supported by Microsoft Healthcare resource provider.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either OperationDetail or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.OperationDetail]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -96,60 +95,57 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ListOperations", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/providers/Microsoft.HealthcareApis/operations"}
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_patch.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/aio/operations/_workspace_private_endpoint_connections_operations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,239 +1,85 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
+from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
-from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpResponse
-from azure.core.polling import LROPoller, NoPolling, PollingMethod
+from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.arm_polling import ARMPolling
+from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
-from .. import models as _models
-from .._serialization import Serializer
-from .._vendor import _convert_request
+from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._workspace_private_endpoint_connections_operations import (
+    build_create_or_update_request,
+    build_delete_request,
+    build_get_request,
+    build_list_by_workspace_request,
+)
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-_SERIALIZER = Serializer()
-_SERIALIZER.client_side_validation = False
-
-
-def build_list_by_service_request(
-    resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
-        ),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_get_request(
-    resource_group_name: str,
-    resource_name: str,
-    private_endpoint_connection_name: str,
-    subscription_id: str,
-    **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
-        ),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
-        "privateEndpointConnectionName": _SERIALIZER.url(
-            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
-        ),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_create_or_update_request(
-    resource_group_name: str,
-    resource_name: str,
-    private_endpoint_connection_name: str,
-    subscription_id: str,
-    **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
-    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
-        ),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
-        "privateEndpointConnectionName": _SERIALIZER.url(
-            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
-        ),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_delete_request(
-    resource_group_name: str,
-    resource_name: str,
-    private_endpoint_connection_name: str,
-    subscription_id: str,
-    **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "resourceGroupName": _SERIALIZER.url(
-            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1, pattern=r"^[-\w\._\(\)]+$"
-        ),
-        "resourceName": _SERIALIZER.url("resource_name", resource_name, "str", max_length=24, min_length=3),
-        "privateEndpointConnectionName": _SERIALIZER.url(
-            "private_endpoint_connection_name", private_endpoint_connection_name, "str"
-        ),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
-
-class PrivateEndpointConnectionsOperations:
+class WorkspacePrivateEndpointConnectionsOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.healthcareapis.HealthcareApisManagementClient`'s
-        :attr:`private_endpoint_connections` attribute.
+        :class:`~azure.mgmt.healthcareapis.aio.HealthcareApisManagementClient`'s
+        :attr:`workspace_private_endpoint_connections` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list_by_service(
-        self, resource_group_name: str, resource_name: str, **kwargs: Any
-    ) -> Iterable["_models.PrivateEndpointConnectionDescription"]:
-        """Lists all private endpoint connections for a service.
+    def list_by_workspace(
+        self, resource_group_name: str, workspace_name: str, **kwargs: Any
+    ) -> AsyncIterable["_models.PrivateEndpointConnectionDescription"]:
+        """Lists all private endpoint connections for a workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
         :return: An iterator like instance of either PrivateEndpointConnectionDescription or the result
          of cls(response)
         :rtype:
-         ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateEndpointConnectionListResultDescription] = kwargs.pop("cls", None)
@@ -245,88 +91,82 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_service_request(
+                _request = build_list_by_workspace_request(
                     resource_group_name=resource_group_name,
-                    resource_name=resource_name,
+                    workspace_name=workspace_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_service.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-        def extract_data(pipeline_response):
+        async def extract_data(pipeline_response):
             deserialized = self._deserialize("PrivateEndpointConnectionListResultDescription", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return None, iter(list_of_elem)
+            return None, AsyncList(list_of_elem)
 
-        def get_next(next_link=None):
-            request = prepare_request(next_link)
+        async def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
             _stream = False
-            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return ItemPaged(get_next, extract_data)
-
-    list_by_service.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections"
-    }
+        return AsyncItemPaged(get_next, extract_data)
 
-    @distributed_trace
-    def get(
-        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    @distributed_trace_async
+    async def get(
+        self, resource_group_name: str, workspace_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> _models.PrivateEndpointConnectionDescription:
-        """Gets the specified private endpoint connection associated with the service.
+        """Gets the specified private endpoint connection associated with the workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateEndpointConnectionDescription or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -337,56 +177,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateEndpointConnectionDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
-            resource_name=resource_name,
+            workspace_name=workspace_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return deserialized  # type: ignore
 
-    def _create_or_update_initial(
+    async def _create_or_update_initial(
         self,
         resource_group_name: str,
-        resource_name: str,
+        workspace_name: str,
         private_endpoint_connection_name: str,
-        properties: Union[_models.PrivateEndpointConnection, IO],
+        properties: Union[_models.PrivateEndpointConnectionDescription, IO[bytes]],
         **kwargs: Any
     ) -> _models.PrivateEndpointConnectionDescription:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -402,227 +237,194 @@
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
         if isinstance(properties, (IOBase, bytes)):
             _content = properties
         else:
-            _json = self._serialize.body(properties, "PrivateEndpointConnection")
+            _json = self._serialize.body(properties, "PrivateEndpointConnectionDescription")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
-            resource_name=resource_name,
+            workspace_name=workspace_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
-    def begin_create_or_update(
+    async def begin_create_or_update(
         self,
         resource_group_name: str,
-        resource_name: str,
+        workspace_name: str,
         private_endpoint_connection_name: str,
-        properties: _models.PrivateEndpointConnection,
+        properties: _models.PrivateEndpointConnectionDescription,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.PrivateEndpointConnectionDescription]:
-        """Update the state of the specified private endpoint connection associated with the service.
+    ) -> AsyncLROPoller[_models.PrivateEndpointConnectionDescription]:
+        """Update the state of the specified private endpoint connection associated with the workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
         :param properties: The private endpoint connection properties. Required.
-        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnection
+        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either PrivateEndpointConnectionDescription or
-         the result of cls(response)
+        :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnectionDescription
+         or the result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    def begin_create_or_update(
+    async def begin_create_or_update(
         self,
         resource_group_name: str,
-        resource_name: str,
+        workspace_name: str,
         private_endpoint_connection_name: str,
-        properties: IO,
+        properties: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.PrivateEndpointConnectionDescription]:
-        """Update the state of the specified private endpoint connection associated with the service.
+    ) -> AsyncLROPoller[_models.PrivateEndpointConnectionDescription]:
+        """Update the state of the specified private endpoint connection associated with the workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
         :param properties: The private endpoint connection properties. Required.
-        :type properties: IO
+        :type properties: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either PrivateEndpointConnectionDescription or
-         the result of cls(response)
+        :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnectionDescription
+         or the result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace
-    def begin_create_or_update(
+    @distributed_trace_async
+    async def begin_create_or_update(
         self,
         resource_group_name: str,
-        resource_name: str,
+        workspace_name: str,
         private_endpoint_connection_name: str,
-        properties: Union[_models.PrivateEndpointConnection, IO],
+        properties: Union[_models.PrivateEndpointConnectionDescription, IO[bytes]],
         **kwargs: Any
-    ) -> LROPoller[_models.PrivateEndpointConnectionDescription]:
-        """Update the state of the specified private endpoint connection associated with the service.
+    ) -> AsyncLROPoller[_models.PrivateEndpointConnectionDescription]:
+        """Update the state of the specified private endpoint connection associated with the workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
         :param properties: The private endpoint connection properties. Is either a
-         PrivateEndpointConnection type or a IO type. Required.
-        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnection or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either PrivateEndpointConnectionDescription or
-         the result of cls(response)
+         PrivateEndpointConnectionDescription type or a IO[bytes] type. Required.
+        :type properties: ~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription or
+         IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnectionDescription
+         or the result of cls(response)
         :rtype:
-         ~azure.core.polling.LROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.healthcareapis.models.PrivateEndpointConnectionDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PrivateEndpointConnectionDescription] = kwargs.pop("cls", None)
-        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._create_or_update_initial(
+            raw_result = await self._create_or_update_initial(
                 resource_group_name=resource_group_name,
-                resource_name=resource_name,
+                workspace_name=workspace_name,
                 private_endpoint_connection_name=private_endpoint_connection_name,
                 properties=properties,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("PrivateEndpointConnectionDescription", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(PollingMethod, NoPolling())
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.PrivateEndpointConnectionDescription].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return AsyncLROPoller[_models.PrivateEndpointConnectionDescription](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, workspace_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -630,108 +432,91 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
-            resource_name=resource_name,
+            workspace_name=workspace_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
 
-    @distributed_trace
-    def begin_delete(
-        self, resource_group_name: str, resource_name: str, private_endpoint_connection_name: str, **kwargs: Any
-    ) -> LROPoller[None]:
+    @distributed_trace_async
+    async def begin_delete(
+        self, resource_group_name: str, workspace_name: str, private_endpoint_connection_name: str, **kwargs: Any
+    ) -> AsyncLROPoller[None]:
         """Deletes a private endpoint connection.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
-        :param resource_name: The name of the service instance. Required.
-        :type resource_name: str
+        :param workspace_name: The name of workspace resource. Required.
+        :type workspace_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection associated
          with the Azure resource. Required.
         :type private_endpoint_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.LROPoller[None]
+        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._delete_initial(  # type: ignore
+            raw_result = await self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
-                resource_name=resource_name,
+                workspace_name=workspace_name,
                 private_endpoint_connection_name=private_endpoint_connection_name,
                 api_version=api_version,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
-            polling_method = cast(PollingMethod, NoPolling())
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_private_link_resources_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_private_link_resources_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -36,15 +36,15 @@
 
 def build_list_by_service_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateLinkResources",
     )  # pylint: disable=line-too-long
@@ -69,15 +69,15 @@
 
 def build_get_request(
     resource_group_name: str, resource_name: str, group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateLinkResources/{groupName}",
     )  # pylint: disable=line-too-long
@@ -127,15 +127,14 @@
         """Gets the private link resources that need to be created for a service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param resource_name: The name of the service instance. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkResourceListResultDescription or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.PrivateLinkResourceListResultDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -146,63 +145,57 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkResourceListResultDescription] = kwargs.pop("cls", None)
 
-        request = build_list_by_service_request(
+        _request = build_list_by_service_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.list_by_service.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkResourceListResultDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    list_by_service.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateLinkResources"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def get(
         self, resource_group_name: str, resource_name: str, group_name: str, **kwargs: Any
     ) -> _models.PrivateLinkResourceDescription:
         """Gets a private link resource that need to be created for a service.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param resource_name: The name of the service instance. Required.
         :type resource_name: str
         :param group_name: The name of the private link resource group. Required.
         :type group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkResourceDescription or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.PrivateLinkResourceDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -213,42 +206,37 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkResourceDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             group_name=group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkResourceDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/services/{resourceName}/privateLinkResources/{groupName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure/mgmt/healthcareapis/operations/_workspace_private_link_resources_operations.py` & `azure-mgmt-healthcareapis-2.1.0/azure/mgmt/healthcareapis/operations/_workspace_private_link_resources_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -38,15 +38,15 @@
 
 def build_list_by_workspace_request(
     resource_group_name: str, workspace_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateLinkResources",
     )  # pylint: disable=line-too-long
@@ -71,15 +71,15 @@
 
 def build_get_request(
     resource_group_name: str, workspace_name: str, group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateLinkResources/{groupName}",
     )  # pylint: disable=line-too-long
@@ -129,15 +129,14 @@
         """Gets the private link resources that need to be created for a workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateLinkResourceDescription or the result of
          cls(response)
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.healthcareapis.models.PrivateLinkResourceDescription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -153,87 +152,81 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_workspace_request(
+                _request = build_list_by_workspace_request(
                     resource_group_name=resource_group_name,
                     workspace_name=workspace_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_workspace.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("PrivateLinkResourceListResultDescription", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_workspace.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateLinkResources"
-    }
-
     @distributed_trace
     def get(
         self, resource_group_name: str, workspace_name: str, group_name: str, **kwargs: Any
     ) -> _models.PrivateLinkResourceDescription:
         """Gets a private link resource that need to be created for a workspace.
 
         :param resource_group_name: The name of the resource group that contains the service instance.
          Required.
         :type resource_group_name: str
         :param workspace_name: The name of workspace resource. Required.
         :type workspace_name: str
         :param group_name: The name of the private link resource group. Required.
         :type group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkResourceDescription or the result of cls(response)
         :rtype: ~azure.mgmt.healthcareapis.models.PrivateLinkResourceDescription
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -244,42 +237,37 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkResourceDescription] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             workspace_name=workspace_name,
             group_name=group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorDetails, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkResourceDescription", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HealthcareApis/workspaces/{workspaceName}/privateLinkResources/{groupName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure_mgmt_healthcareapis.egg-info/PKG-INFO` & `azure-mgmt-healthcareapis-2.1.0/azure_mgmt_healthcareapis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-healthcareapis
-Version: 2.0.0
+Version: 2.1.0
 Summary: Microsoft Azure Health Care Apis Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-common~=1.1
-Requires-Dist: azure-mgmt-core<2.0.0,>=1.3.2
-Requires-Dist: typing-extensions>=4.3.0; python_version < "3.8.0"
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Health Care Apis Management Client Library.
-This package has been tested with Python 3.7+.
+This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 ## Getting started
 
 ### Prerequisites
 
-- Python 3.7+ is required to use this package.
+- Python 3.8+ is required to use this package.
 - [Azure subscription](https://azure.microsoft.com/free/)
 
 ### Install the package
 
 ```bash
 pip install azure-mgmt-healthcareapis
 pip install azure-identity
@@ -86,14 +82,22 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.1.0 (2024-04-22)
+
+### Features Added
+
+  - Model DicomService has a new parameter enable_data_partitions
+  - Model DicomService has a new parameter storage_configuration
+  - Model FhirServiceAuthenticationConfiguration has a new parameter smart_identity_providers
+
 ## 2.0.0 (2023-12-18)
 
 ### Features Added
 
   - Model DicomService has a new parameter cors_configuration
   - Model DicomService has a new parameter encryption
   - Model DicomService has a new parameter event_state
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/azure_mgmt_healthcareapis.egg-info/SOURCES.txt` & `azure-mgmt-healthcareapis-2.1.0/azure_mgmt_healthcareapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-mgmt-healthcareapis-2.0.0/setup.py` & `azure-mgmt-healthcareapis-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,19 +49,19 @@
     url="https://github.com/Azure/azure-sdk-for-python",
     keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
     packages=find_packages(
         exclude=[
             "tests",
             # Exclude packages that will be covered by PEP420 or nspkg
@@ -70,14 +70,13 @@
         ]
     ),
     include_package_data=True,
     package_data={
         "pytyped": ["py.typed"],
     },
     install_requires=[
-        "isodate<1.0.0,>=0.6.1",
-        "azure-common~=1.1",
-        "azure-mgmt-core>=1.3.2,<2.0.0",
-        "typing-extensions>=4.3.0; python_version<'3.8.0'",
+        "isodate>=0.6.1",
+        "azure-common>=1.1",
+        "azure-mgmt-core>=1.3.2",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

### Comparing `azure-mgmt-healthcareapis-2.0.0/tests/disable_test_cli_mgmt_healthcareapis.py` & `azure-mgmt-healthcareapis-2.1.0/tests/disable_test_cli_mgmt_healthcareapis.py`

 * *Files identical despite different names*

