# Comparing `tmp/azure-mgmt-recoveryservices-2.5.0.tar.gz` & `tmp/azure-mgmt-recoveryservices-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-recoveryservices-2.5.0.tar", last modified: Tue Sep  5 06:56:36 2023, max compression
+gzip compressed data, was "azure-mgmt-recoveryservices-3.0.0.tar", last modified: Mon Apr 22 03:17:05 2024, max compression
```

## Comparing `azure-mgmt-recoveryservices-2.5.0.tar` & `azure-mgmt-recoveryservices-3.0.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-09-05 06:56:36.206990 azure-mgmt-recoveryservices-2.5.0/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9745 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      222 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12820 2023-09-05 06:56:36.206990 azure-mgmt-recoveryservices-2.5.0/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2167 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      640 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-09-05 06:56:36.198990 azure-mgmt-recoveryservices-2.5.0/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-09-05 06:56:36.198990 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-09-05 06:56:36.198990 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      906 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3495 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6800 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/_recovery_services_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79289 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1326 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-09-05 06:56:36.198990 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      853 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3543 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6983 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/_recovery_services_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1066 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-09-05 06:56:36.202990 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1699 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5814 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9692 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_private_link_resources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7317 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_recovery_services_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15971 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_recovery_services_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4866 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_registered_identities_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6369 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_replication_usages_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6322 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_usages_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8899 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_vault_certificates_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17709 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_vault_extended_info_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35764 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_vaults_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-09-05 06:56:36.202990 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7439 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   113360 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/models/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6177 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/models/_recovery_services_client_enums.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-09-05 06:56:36.202990 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1699 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6501 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12437 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_private_link_resources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10205 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_recovery_services_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18861 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_recovery_services_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6098 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_registered_identities_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7652 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_replication_usages_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7635 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_usages_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10586 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_vault_certificates_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22222 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_vault_extended_info_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    43277 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_vaults_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-09-05 06:56:36.202990 azure-mgmt-recoveryservices-2.5.0/azure_mgmt_recoveryservices.egg-info/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12820 2023-09-05 06:56:36.000000 azure-mgmt-recoveryservices-2.5.0/azure_mgmt_recoveryservices.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2929 2023-09-05 06:56:36.000000 azure-mgmt-recoveryservices-2.5.0/azure_mgmt_recoveryservices.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-09-05 06:56:36.000000 azure-mgmt-recoveryservices-2.5.0/azure_mgmt_recoveryservices.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-09-05 06:56:35.000000 azure-mgmt-recoveryservices-2.5.0/azure_mgmt_recoveryservices.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      124 2023-09-05 06:56:36.000000 azure-mgmt-recoveryservices-2.5.0/azure_mgmt_recoveryservices.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-09-05 06:56:36.000000 azure-mgmt-recoveryservices-2.5.0/azure_mgmt_recoveryservices.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-09-05 06:56:36.206990 azure-mgmt-recoveryservices-2.5.0/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2861 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-09-05 06:56:36.206990 azure-mgmt-recoveryservices-2.5.0/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3519 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/tests/disable_test_mgmt_recoveryservices.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3552 2023-09-05 06:55:40.000000 azure-mgmt-recoveryservices-2.5.0/tests/recoveryservices_testcase.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:17:05.262845 azure-mgmt-recoveryservices-3.0.0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10590 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      222 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13520 2024-04-22 03:17:05.262845 azure-mgmt-recoveryservices-3.0.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2021 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      642 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:17:05.250846 azure-mgmt-recoveryservices-3.0.0/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:17:05.250846 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:17:05.250846 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      906 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3434 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7852 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/_recovery_services_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1326 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:17:05.254846 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      853 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3482 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8059 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/_recovery_services_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1066 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:17:05.254846 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1699 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5610 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9054 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6652 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_recovery_services_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14721 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_recovery_services_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4550 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_registered_identities_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6059 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_replication_usages_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6003 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_usages_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8278 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_vault_certificates_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16097 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_vault_extended_info_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33728 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_vaults_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:17:05.258845 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7739 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   120144 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/models/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6669 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/models/_recovery_services_client_enums.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:17:05.258845 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1699 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6297 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11799 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_private_link_resources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9540 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_recovery_services_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17611 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_recovery_services_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5782 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_registered_identities_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7342 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_replication_usages_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7316 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_usages_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9965 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_vault_certificates_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20610 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_vault_extended_info_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41810 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_vaults_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:17:05.258845 azure-mgmt-recoveryservices-3.0.0/azure_mgmt_recoveryservices.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13520 2024-04-22 03:17:05.000000 azure-mgmt-recoveryservices-3.0.0/azure_mgmt_recoveryservices.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2929 2024-04-22 03:17:05.000000 azure-mgmt-recoveryservices-3.0.0/azure_mgmt_recoveryservices.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-22 03:17:05.000000 azure-mgmt-recoveryservices-3.0.0/azure_mgmt_recoveryservices.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-22 03:17:04.000000 azure-mgmt-recoveryservices-3.0.0/azure_mgmt_recoveryservices.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-04-22 03:17:05.000000 azure-mgmt-recoveryservices-3.0.0/azure_mgmt_recoveryservices.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-22 03:17:05.000000 azure-mgmt-recoveryservices-3.0.0/azure_mgmt_recoveryservices.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-22 03:17:05.262845 azure-mgmt-recoveryservices-3.0.0/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2788 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-22 03:17:05.262845 azure-mgmt-recoveryservices-3.0.0/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3519 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/tests/disable_test_mgmt_recoveryservices.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3552 2024-04-22 03:15:33.000000 azure-mgmt-recoveryservices-3.0.0/tests/recoveryservices_testcase.py
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/CHANGELOG.md` & `azure-mgmt-recoveryservices-3.0.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # Release History
 
+## 3.0.0 (2024-04-22)
+
+### Features Added
+
+  - Model AzureMonitorAlertSettings has a new parameter alerts_for_all_failover_issues
+  - Model AzureMonitorAlertSettings has a new parameter alerts_for_all_replication_issues
+  - Model ClassicAlertSettings has a new parameter email_notifications_for_site_recovery
+  - Model SoftDeleteSettings has a new parameter enhanced_security_state
+  - Model VaultProperties has a new parameter bcdr_security_level
+  - Model VaultProperties has a new parameter resource_guard_operation_requests
+  - Operation VaultsOperations.begin_create_or_update has a new optional parameter x_ms_authorization_auxiliary
+  - Operation VaultsOperations.begin_update has a new optional parameter x_ms_authorization_auxiliary
+
+### Breaking Changes
+
+  - Renamed operation VaultsOperations.delete to VaultsOperations.begin_delete
+
 ## 2.5.0 (2023-09-05)
 
 ### Features Added
 
   - Model SecuritySettings has a new parameter multi_user_authorization
   - Model SecuritySettings has a new parameter soft_delete_settings
   - Model VaultProperties has a new parameter secure_score
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/LICENSE` & `azure-mgmt-recoveryservices-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/PKG-INFO` & `azure-mgmt-recoveryservices-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-recoveryservices
-Version: 2.5.0
+Version: 3.0.0
 Summary: Microsoft Azure Recovery Services Client Library for Python
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
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Recovery Services Client Library.
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
 pip install azure-mgmt-recoveryservices
 pip install azure-identity
@@ -80,18 +80,32 @@
 ## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
-![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-recoveryservices%2FREADME.png)
+# Release History
 
+## 3.0.0 (2024-04-22)
 
-# Release History
+### Features Added
+
+  - Model AzureMonitorAlertSettings has a new parameter alerts_for_all_failover_issues
+  - Model AzureMonitorAlertSettings has a new parameter alerts_for_all_replication_issues
+  - Model ClassicAlertSettings has a new parameter email_notifications_for_site_recovery
+  - Model SoftDeleteSettings has a new parameter enhanced_security_state
+  - Model VaultProperties has a new parameter bcdr_security_level
+  - Model VaultProperties has a new parameter resource_guard_operation_requests
+  - Operation VaultsOperations.begin_create_or_update has a new optional parameter x_ms_authorization_auxiliary
+  - Operation VaultsOperations.begin_update has a new optional parameter x_ms_authorization_auxiliary
+
+### Breaking Changes
+
+  - Renamed operation VaultsOperations.delete to VaultsOperations.begin_delete
 
 ## 2.5.0 (2023-09-05)
 
 ### Features Added
 
   - Model SecuritySettings has a new parameter multi_user_authorization
   - Model SecuritySettings has a new parameter soft_delete_settings
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/README.md` & `azure-mgmt-recoveryservices-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Recovery Services Client Library.
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
 pip install azure-mgmt-recoveryservices
 pip install azure-identity
@@ -55,10 +55,7 @@
 ## Next steps
 
 ## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
-
-
-![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-recoveryservices%2FREADME.png)
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/_meta.json` & `azure-mgmt-recoveryservices-3.0.0/_meta.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'autorest_command'": "'autorest specification/recoveryservices/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 '*

 * *                       "--version=3.9.7 --version-tolerant=False'",*

 * * "'commit'": "'c4e661cdf92c8f579574008d0cd11874cc303da0'",*

 * * "'use'": […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.7",
-    "autorest_command": "autorest specification/recoveryservices/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.7.1 --use=@autorest/modelerfour@4.26.2 --version=3.9.7 --version-tolerant=False",
-    "commit": "277c98958d4dd87af68a6192009644704239778e",
+    "autorest_command": "autorest specification/recoveryservices/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 --version=3.9.7 --version-tolerant=False",
+    "commit": "c4e661cdf92c8f579574008d0cd11874cc303da0",
     "readme": "specification/recoveryservices/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.7.1",
-        "@autorest/modelerfour@4.26.2"
+        "@autorest/python@6.13.7",
+        "@autorest/modelerfour@4.27.0"
     ]
 }
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/__init__.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/_configuration.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/_configuration.py`

 * *Files 6% similar despite different names*

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
 
 
-class RecoveryServicesClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class RecoveryServicesClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for RecoveryServicesClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-04-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-04-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(RecoveryServicesClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-04-01")
+        api_version: str = kwargs.pop("api_version", "2024-04-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-recoveryservices/{}".format(VERSION))
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

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/_patch.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/_recovery_services_client.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/_recovery_services_client.py`

 * *Files 10% similar despite different names*

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
 from ._configuration import RecoveryServicesClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
     Operations,
     PrivateLinkResourcesOperations,
@@ -61,15 +63,15 @@
     :vartype usages: azure.mgmt.recoveryservices.operations.UsagesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-04-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-04-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -78,15 +80,33 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = RecoveryServicesClientConfiguration(
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
         self.vault_certificates = VaultCertificatesOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -106,15 +126,15 @@
         self.vaults = VaultsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.vault_extended_info = VaultExtendedInfoOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.usages = UsagesOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
+    def _send_request(self, request: HttpRequest, *, stream: bool = False, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = client._send_request(request)
         <HttpResponse: 200 OK>
@@ -126,15 +146,15 @@
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
 
     def __enter__(self) -> "RecoveryServicesClient":
         self._client.__enter__()
         return self
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/_serialization.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/_serialization.py`

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

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/_vendor.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/__init__.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/_configuration.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/_configuration.py`

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
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
 from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class RecoveryServicesClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class RecoveryServicesClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for RecoveryServicesClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-04-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-04-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(RecoveryServicesClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-04-01")
+        api_version: str = kwargs.pop("api_version", "2024-04-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-recoveryservices/{}".format(VERSION))
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

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/_patch.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/_recovery_services_client.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/_recovery_services_client.py`

 * *Files 13% similar despite different names*

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
 from ._configuration import RecoveryServicesClientConfiguration
 from .operations import (
     Operations,
     PrivateLinkResourcesOperations,
@@ -64,15 +66,15 @@
     :vartype usages: azure.mgmt.recoveryservices.aio.operations.UsagesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-04-01". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-04-01". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -81,15 +83,33 @@
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = RecoveryServicesClientConfiguration(
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
         self.vault_certificates = VaultCertificatesOperations(
             self._client, self._config, self._serialize, self._deserialize
@@ -109,15 +129,17 @@
         self.vaults = VaultsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.vault_extended_info = VaultExtendedInfoOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.usages = UsagesOperations(self._client, self._config, self._serialize, self._deserialize)
 
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
@@ -129,15 +151,15 @@
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
 
     async def __aenter__(self) -> "RecoveryServicesClient":
         await self._client.__aenter__()
         return self
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/_vendor.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/__init__.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_operations.py`

 * *Files 4% similar despite different names*

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
@@ -53,15 +53,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.ClientDiscoveryValueForSingleApi"]:
         """Returns the list of available operations.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ClientDiscoveryValueForSingleApi or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.recoveryservices.models.ClientDiscoveryValueForSingleApi]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -77,59 +76,56 @@
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
             deserialized = self._deserialize("ClientDiscoveryResponse", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/providers/Microsoft.RecoveryServices/operations"}
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_patch.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_private_link_resources_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_private_link_resources_operations.py`

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
@@ -63,15 +63,14 @@
         Returns the list of private link resources that need to be created for Backup and SiteRecovery.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateLinkResource or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.recoveryservices.models.PrivateLinkResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -86,72 +85,67 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     vault_name=vault_name,
                     subscription_id=self._config.subscription_id,
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
             deserialized = self._deserialize("PrivateLinkResources", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/privateLinkResources"
-    }
-
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, vault_name: str, private_link_resource_name: str, **kwargs: Any
     ) -> _models.PrivateLinkResource:
         """Returns a specified private link resource that need to be created for Backup and SiteRecovery.
 
         Returns a specified private link resource that need to be created for Backup and SiteRecovery.
@@ -159,15 +153,14 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param private_link_resource_name: Required.
         :type private_link_resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkResource or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.PrivateLinkResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -178,41 +171,36 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkResource] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             private_link_resource_name=private_link_resource_name,
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/privateLinkResources/{privateLinkResourceName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_recovery_services_client_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_recovery_services_client_operations.py`

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
@@ -45,15 +45,14 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param operation_id: Required.
         :type operation_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: OperationResource or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.OperationResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -64,63 +63,57 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationResource] = kwargs.pop("cls", None)
 
-        request = build_get_operation_status_request(
+        _request = build_get_operation_status_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_operation_status.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("OperationResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get_operation_status.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/operationStatus/{operationId}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace_async
     async def get_operation_result(
         self, resource_group_name: str, vault_name: str, operation_id: str, **kwargs: Any
     ) -> Optional[_models.Vault]:
         """Gets the operation result for a resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param operation_id: Required.
         :type operation_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Vault or None or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.Vault or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -131,43 +124,38 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.Vault]] = kwargs.pop("cls", None)
 
-        request = build_get_operation_result_request(
+        _request = build_get_operation_result_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_operation_result.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("Vault", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_operation_result.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/operationResults/{operationId}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_recovery_services_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_recovery_services_operations.py`

 * *Files 8% similar despite different names*

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
@@ -14,53 +14,119 @@
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
-from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._recovery_services_operations import (
-    build_capabilities_request,
-    build_check_name_availability_request,
-)
-from .._vendor import RecoveryServicesClientMixinABC
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import RecoveryServicesClientMixinABC, _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_check_name_availability_request(
+    resource_group_name: str, location: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/locations/{location}/checkNameAvailability",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "location": _SERIALIZER.url("location", location, "str"),
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
+
+
+def build_capabilities_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/providers/Microsoft.RecoveryServices/locations/{location}/capabilities",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "location": _SERIALIZER.url("location", location, "str"),
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
 
 
 class RecoveryServicesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.recoveryservices.aio.RecoveryServicesClient`'s
+        :class:`~azure.mgmt.recoveryservices.RecoveryServicesClient`'s
         :attr:`recovery_services` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @overload
-    async def check_name_availability(
+    def check_name_availability(
         self,
         resource_group_name: str,
         location: str,
         input: _models.CheckNameAvailabilityParameters,
         *,
         content_type: str = "application/json",
         **kwargs: Any
@@ -83,26 +149,25 @@
         :param location: Location of the resource. Required.
         :type location: str
         :param input: Contains information about Resource type and Resource name. Required.
         :type input: ~azure.mgmt.recoveryservices.models.CheckNameAvailabilityParameters
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResult or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.CheckNameAvailabilityResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def check_name_availability(
+    def check_name_availability(
         self,
         resource_group_name: str,
         location: str,
-        input: IO,
+        input: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResult:
         """API to check for resource name availability.
         A name is available if no other resource exists that has the same SubscriptionId, Resource Name
         and Type
@@ -117,30 +182,29 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param location: Location of the resource. Required.
         :type location: str
         :param input: Contains information about Resource type and Resource name. Required.
-        :type input: IO
+        :type input: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResult or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.CheckNameAvailabilityResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def check_name_availability(
+    @distributed_trace
+    def check_name_availability(
         self,
         resource_group_name: str,
         location: str,
-        input: Union[_models.CheckNameAvailabilityParameters, IO],
+        input: Union[_models.CheckNameAvailabilityParameters, IO[bytes]],
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResult:
         """API to check for resource name availability.
         A name is available if no other resource exists that has the same SubscriptionId, Resource Name
         and Type
         or if one or more such resources exist, each of these must be GC'd and their time of deletion
         be more than 24 Hours Ago.
@@ -153,20 +217,16 @@
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param location: Location of the resource. Required.
         :type location: str
         :param input: Contains information about Resource type and Resource name. Is either a
-         CheckNameAvailabilityParameters type or a IO type. Required.
-        :type input: ~azure.mgmt.recoveryservices.models.CheckNameAvailabilityParameters or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         CheckNameAvailabilityParameters type or a IO[bytes] type. Required.
+        :type input: ~azure.mgmt.recoveryservices.models.CheckNameAvailabilityParameters or IO[bytes]
         :return: CheckNameAvailabilityResult or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.CheckNameAvailabilityResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -186,53 +246,48 @@
         _json = None
         _content = None
         if isinstance(input, (IOBase, bytes)):
             _content = input
         else:
             _json = self._serialize.body(input, "CheckNameAvailabilityParameters")
 
-        request = build_check_name_availability_request(
+        _request = build_check_name_availability_request(
             resource_group_name=resource_group_name,
             location=location,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.check_name_availability.metadata["url"],
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("CheckNameAvailabilityResult", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    check_name_availability.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/locations/{location}/checkNameAvailability"
-    }
+        return deserialized  # type: ignore
 
     @overload
-    async def capabilities(
+    def capabilities(
         self,
         location: str,
         input: _models.ResourceCapabilities,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CapabilitiesResponse:
@@ -244,59 +299,53 @@
         :type location: str
         :param input: Contains information about Resource type and properties to get capabilities.
          Required.
         :type input: ~azure.mgmt.recoveryservices.models.ResourceCapabilities
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CapabilitiesResponse or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.CapabilitiesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def capabilities(
-        self, location: str, input: IO, *, content_type: str = "application/json", **kwargs: Any
+    def capabilities(
+        self, location: str, input: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
     ) -> _models.CapabilitiesResponse:
         """API to get details about capabilities provided by Microsoft.RecoveryServices RP.
 
         API to get details about capabilities provided by Microsoft.RecoveryServices RP.
 
         :param location: Location of the resource. Required.
         :type location: str
         :param input: Contains information about Resource type and properties to get capabilities.
          Required.
-        :type input: IO
+        :type input: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CapabilitiesResponse or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.CapabilitiesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def capabilities(
-        self, location: str, input: Union[_models.ResourceCapabilities, IO], **kwargs: Any
+    @distributed_trace
+    def capabilities(
+        self, location: str, input: Union[_models.ResourceCapabilities, IO[bytes]], **kwargs: Any
     ) -> _models.CapabilitiesResponse:
         """API to get details about capabilities provided by Microsoft.RecoveryServices RP.
 
         API to get details about capabilities provided by Microsoft.RecoveryServices RP.
 
         :param location: Location of the resource. Required.
         :type location: str
         :param input: Contains information about Resource type and properties to get capabilities. Is
-         either a ResourceCapabilities type or a IO type. Required.
-        :type input: ~azure.mgmt.recoveryservices.models.ResourceCapabilities or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         either a ResourceCapabilities type or a IO[bytes] type. Required.
+        :type input: ~azure.mgmt.recoveryservices.models.ResourceCapabilities or IO[bytes]
         :return: CapabilitiesResponse or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.CapabilitiesResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -316,42 +365,37 @@
         _json = None
         _content = None
         if isinstance(input, (IOBase, bytes)):
             _content = input
         else:
             _json = self._serialize.body(input, "ResourceCapabilities")
 
-        request = build_capabilities_request(
+        _request = build_capabilities_request(
             location=location,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.capabilities.metadata["url"],
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("CapabilitiesResponse", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    capabilities.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.RecoveryServices/locations/{location}/capabilities"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_registered_identities_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_registered_identities_operations.py`

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
@@ -60,15 +60,14 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param identity_name: Name of the protection container to unregister. Required.
         :type identity_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -79,37 +78,32 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             identity_name=identity_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
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
 
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    delete.metadata = {
-        "url": "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/registeredIdentities/{identityName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_replication_usages_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_replication_usages_operations.py`

 * *Files 8% similar despite different names*

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
@@ -60,15 +60,14 @@
         """Fetches the replication usages of the vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ReplicationUsage or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.recoveryservices.models.ReplicationUsage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -83,64 +82,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     vault_name=vault_name,
                     subscription_id=self._config.subscription_id,
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
             deserialized = self._deserialize("ReplicationUsageList", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/replicationUsages"
-    }
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_usages_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_usages_operations.py`

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
@@ -60,15 +60,14 @@
         """Fetches the usages of the vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either VaultUsage or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.recoveryservices.models.VaultUsage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -82,64 +81,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_vaults_request(
+                _request = build_list_by_vaults_request(
                     resource_group_name=resource_group_name,
                     vault_name=vault_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_vaults.metadata["url"],
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
             deserialized = self._deserialize("VaultUsageList", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list_by_vaults.metadata = {
-        "url": "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/usages"
-    }
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_vault_certificates_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_vault_certificates_operations.py`

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
@@ -73,76 +73,70 @@
         :param certificate_name: Certificate friendly name. Required.
         :type certificate_name: str
         :param certificate_request: Input parameters for uploading the vault certificate. Required.
         :type certificate_request: ~azure.mgmt.recoveryservices.models.CertificateRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: VaultCertificateResponse or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultCertificateResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create(
         self,
         resource_group_name: str,
         vault_name: str,
         certificate_name: str,
-        certificate_request: IO,
+        certificate_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.VaultCertificateResponse:
         """Uploads a certificate for a resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param certificate_name: Certificate friendly name. Required.
         :type certificate_name: str
         :param certificate_request: Input parameters for uploading the vault certificate. Required.
-        :type certificate_request: IO
+        :type certificate_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: VaultCertificateResponse or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultCertificateResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create(
         self,
         resource_group_name: str,
         vault_name: str,
         certificate_name: str,
-        certificate_request: Union[_models.CertificateRequest, IO],
+        certificate_request: Union[_models.CertificateRequest, IO[bytes]],
         **kwargs: Any
     ) -> _models.VaultCertificateResponse:
         """Uploads a certificate for a resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param certificate_name: Certificate friendly name. Required.
         :type certificate_name: str
         :param certificate_request: Input parameters for uploading the vault certificate. Is either a
-         CertificateRequest type or a IO type. Required.
-        :type certificate_request: ~azure.mgmt.recoveryservices.models.CertificateRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         CertificateRequest type or a IO[bytes] type. Required.
+        :type certificate_request: ~azure.mgmt.recoveryservices.models.CertificateRequest or IO[bytes]
         :return: VaultCertificateResponse or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultCertificateResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -162,44 +156,39 @@
         _json = None
         _content = None
         if isinstance(certificate_request, (IOBase, bytes)):
             _content = certificate_request
         else:
             _json = self._serialize.body(certificate_request, "CertificateRequest")
 
-        request = build_create_request(
+        _request = build_create_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create.metadata["url"],
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("VaultCertificateResponse", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    create.metadata = {
-        "url": "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/certificates/{certificateName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_vault_extended_info_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_vault_extended_info_operations.py`

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
@@ -61,15 +61,14 @@
         """Get the vault extended info.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: VaultExtendedInfoResource or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -80,47 +79,42 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.VaultExtendedInfoResource] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("VaultExtendedInfoResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/extendedInformation/vaultExtendedInfo"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
         resource_extended_info_details: _models.VaultExtendedInfoResource,
@@ -137,71 +131,65 @@
         :type vault_name: str
         :param resource_extended_info_details: Details of ResourceExtendedInfo. Required.
         :type resource_extended_info_details:
          ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: VaultExtendedInfoResource or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
-        resource_extended_info_details: IO,
+        resource_extended_info_details: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.VaultExtendedInfoResource:
         """Create vault extended info.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param resource_extended_info_details: Details of ResourceExtendedInfo. Required.
-        :type resource_extended_info_details: IO
+        :type resource_extended_info_details: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: VaultExtendedInfoResource or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
-        resource_extended_info_details: Union[_models.VaultExtendedInfoResource, IO],
+        resource_extended_info_details: Union[_models.VaultExtendedInfoResource, IO[bytes]],
         **kwargs: Any
     ) -> _models.VaultExtendedInfoResource:
         """Create vault extended info.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param resource_extended_info_details: Details of ResourceExtendedInfo. Is either a
-         VaultExtendedInfoResource type or a IO type. Required.
+         VaultExtendedInfoResource type or a IO[bytes] type. Required.
         :type resource_extended_info_details:
-         ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource or IO[bytes]
         :return: VaultExtendedInfoResource or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -221,50 +209,45 @@
         _json = None
         _content = None
         if isinstance(resource_extended_info_details, (IOBase, bytes)):
             _content = resource_extended_info_details
         else:
             _json = self._serialize.body(resource_extended_info_details, "VaultExtendedInfoResource")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update.metadata["url"],
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("VaultExtendedInfoResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/extendedInformation/vaultExtendedInfo"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def update(
         self,
         resource_group_name: str,
         vault_name: str,
         resource_extended_info_details: _models.VaultExtendedInfoResource,
@@ -281,71 +264,65 @@
         :type vault_name: str
         :param resource_extended_info_details: Details of ResourceExtendedInfo. Required.
         :type resource_extended_info_details:
          ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: VaultExtendedInfoResource or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update(
         self,
         resource_group_name: str,
         vault_name: str,
-        resource_extended_info_details: IO,
+        resource_extended_info_details: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.VaultExtendedInfoResource:
         """Update vault extended info.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param resource_extended_info_details: Details of ResourceExtendedInfo. Required.
-        :type resource_extended_info_details: IO
+        :type resource_extended_info_details: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: VaultExtendedInfoResource or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update(
         self,
         resource_group_name: str,
         vault_name: str,
-        resource_extended_info_details: Union[_models.VaultExtendedInfoResource, IO],
+        resource_extended_info_details: Union[_models.VaultExtendedInfoResource, IO[bytes]],
         **kwargs: Any
     ) -> _models.VaultExtendedInfoResource:
         """Update vault extended info.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param resource_extended_info_details: Details of ResourceExtendedInfo. Is either a
-         VaultExtendedInfoResource type or a IO type. Required.
+         VaultExtendedInfoResource type or a IO[bytes] type. Required.
         :type resource_extended_info_details:
-         ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource or IO[bytes]
         :return: VaultExtendedInfoResource or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -365,43 +342,38 @@
         _json = None
         _content = None
         if isinstance(resource_extended_info_details, (IOBase, bytes)):
             _content = resource_extended_info_details
         else:
             _json = self._serialize.body(resource_extended_info_details, "VaultExtendedInfoResource")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.update.metadata["url"],
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("VaultExtendedInfoResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/extendedInformation/vaultExtendedInfo"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/aio/operations/_vaults_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/aio/operations/_vaults_operations.py`

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
@@ -64,15 +64,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list_by_subscription_id(self, **kwargs: Any) -> AsyncIterable["_models.Vault"]:
         """Fetches all the resources of the specified type in the subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Vault or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -86,78 +85,72 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_subscription_id_request(
+                _request = build_list_by_subscription_id_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_subscription_id.metadata["url"],
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
             deserialized = self._deserialize("VaultList", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_subscription_id.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.RecoveryServices/vaults"
-    }
-
     @distributed_trace
     def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.Vault"]:
         """Retrieve a list of Vaults.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Vault or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -171,81 +164,75 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_resource_group_request(
+                _request = build_list_by_resource_group_request(
                     resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
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
             deserialized = self._deserialize("VaultList", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults"
-    }
-
     @distributed_trace_async
     async def get(self, resource_group_name: str, vault_name: str, **kwargs: Any) -> _models.Vault:
         """Get the Vault details.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Vault or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.Vault
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -256,50 +243,50 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Vault] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("Vault", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
+        return deserialized  # type: ignore
 
     async def _create_or_update_initial(
-        self, resource_group_name: str, vault_name: str, vault: Union[_models.Vault, IO], **kwargs: Any
+        self,
+        resource_group_name: str,
+        vault_name: str,
+        vault: Union[_models.Vault, IO[bytes]],
+        x_ms_authorization_auxiliary: Optional[str] = None,
+        **kwargs: Any
     ) -> _models.Vault:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -316,32 +303,32 @@
         _json = None
         _content = None
         if isinstance(vault, (IOBase, bytes)):
             _content = vault
         else:
             _json = self._serialize.body(vault, "Vault")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
+            x_ms_authorization_auxiliary=x_ms_authorization_auxiliary,
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
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -353,113 +340,95 @@
             deserialized = self._deserialize("Vault", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
-
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
         vault: _models.Vault,
+        x_ms_authorization_auxiliary: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Vault]:
         """Creates or updates a Recovery Services vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param vault: Recovery Services Vault to be created. Required.
         :type vault: ~azure.mgmt.recoveryservices.models.Vault
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
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
         :return: An instance of AsyncLROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
-        vault: IO,
+        vault: IO[bytes],
+        x_ms_authorization_auxiliary: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Vault]:
         """Creates or updates a Recovery Services vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param vault: Recovery Services Vault to be created. Required.
-        :type vault: IO
+        :type vault: IO[bytes]
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
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
         :return: An instance of AsyncLROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
-        self, resource_group_name: str, vault_name: str, vault: Union[_models.Vault, IO], **kwargs: Any
+        self,
+        resource_group_name: str,
+        vault_name: str,
+        vault: Union[_models.Vault, IO[bytes]],
+        x_ms_authorization_auxiliary: Optional[str] = None,
+        **kwargs: Any
     ) -> AsyncLROPoller[_models.Vault]:
         """Creates or updates a Recovery Services vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :param vault: Recovery Services Vault to be created. Is either a Vault type or a IO type.
-         Required.
-        :type vault: ~azure.mgmt.recoveryservices.models.Vault or IO
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
+        :param vault: Recovery Services Vault to be created. Is either a Vault type or a IO[bytes]
+         type. Required.
+        :type vault: ~azure.mgmt.recoveryservices.models.Vault or IO[bytes]
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
         :return: An instance of AsyncLROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -470,110 +439,153 @@
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 vault_name=vault_name,
                 vault=vault,
+                x_ms_authorization_auxiliary=x_ms_authorization_auxiliary,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Vault", pipeline_response)
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
+            return AsyncLROPoller[_models.Vault].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
+        return AsyncLROPoller[_models.Vault](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    @distributed_trace_async
-    async def delete(  # pylint: disable=inconsistent-return-statements
+    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> None:
-        """Deletes a vault.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param vault_name: The name of the recovery services vault. Required.
-        :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
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
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
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
 
-        if response.status_code not in [200]:
+        if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)  # type: ignore
+
+    @distributed_trace_async
+    async def begin_delete(self, resource_group_name: str, vault_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
+        """Deletes a vault.
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param vault_name: The name of the recovery services vault. Required.
+        :type vault_name: str
+        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._delete_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                vault_name=vault_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+            if cls:
+                return cls(pipeline_response, None, {})  # type: ignore
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller[None].from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     async def _update_initial(
-        self, resource_group_name: str, vault_name: str, vault: Union[_models.PatchVault, IO], **kwargs: Any
+        self,
+        resource_group_name: str,
+        vault_name: str,
+        vault: Union[_models.PatchVault, IO[bytes]],
+        x_ms_authorization_auxiliary: Optional[str] = None,
+        **kwargs: Any
     ) -> Optional[_models.Vault]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -590,148 +602,130 @@
         _json = None
         _content = None
         if isinstance(vault, (IOBase, bytes)):
             _content = vault
         else:
             _json = self._serialize.body(vault, "PatchVault")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
+            x_ms_authorization_auxiliary=x_ms_authorization_auxiliary,
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("Vault", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         vault_name: str,
         vault: _models.PatchVault,
+        x_ms_authorization_auxiliary: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Vault]:
         """Updates the vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param vault: Recovery Services Vault to be created. Required.
         :type vault: ~azure.mgmt.recoveryservices.models.PatchVault
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
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
         :return: An instance of AsyncLROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_update(
         self,
         resource_group_name: str,
         vault_name: str,
-        vault: IO,
+        vault: IO[bytes],
+        x_ms_authorization_auxiliary: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.Vault]:
         """Updates the vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param vault: Recovery Services Vault to be created. Required.
-        :type vault: IO
+        :type vault: IO[bytes]
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
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
         :return: An instance of AsyncLROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_update(
-        self, resource_group_name: str, vault_name: str, vault: Union[_models.PatchVault, IO], **kwargs: Any
+        self,
+        resource_group_name: str,
+        vault_name: str,
+        vault: Union[_models.PatchVault, IO[bytes]],
+        x_ms_authorization_auxiliary: Optional[str] = None,
+        **kwargs: Any
     ) -> AsyncLROPoller[_models.Vault]:
         """Updates the vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :param vault: Recovery Services Vault to be created. Is either a PatchVault type or a IO type.
-         Required.
-        :type vault: ~azure.mgmt.recoveryservices.models.PatchVault or IO
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
+        :param vault: Recovery Services Vault to be created. Is either a PatchVault type or a IO[bytes]
+         type. Required.
+        :type vault: ~azure.mgmt.recoveryservices.models.PatchVault or IO[bytes]
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
         :return: An instance of AsyncLROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -742,40 +736,39 @@
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = await self._update_initial(
                 resource_group_name=resource_group_name,
                 vault_name=vault_name,
                 vault=vault,
+                x_ms_authorization_auxiliary=x_ms_authorization_auxiliary,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Vault", pipeline_response)
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
+            return AsyncLROPoller[_models.Vault].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
+        return AsyncLROPoller[_models.Vault](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/models/__init__.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from ._models_py3 import CmkKekIdentity
 from ._models_py3 import CmkKeyVaultProperties
 from ._models_py3 import CrossSubscriptionRestoreSettings
 from ._models_py3 import DNSZone
 from ._models_py3 import DNSZoneResponse
 from ._models_py3 import Error
 from ._models_py3 import ErrorAdditionalInfo
+from ._models_py3 import ErrorDetail
+from ._models_py3 import ErrorResponse
 from ._models_py3 import IdentityData
 from ._models_py3 import ImmutabilitySettings
 from ._models_py3 import JobsSummary
 from ._models_py3 import MonitoringSettings
 from ._models_py3 import MonitoringSummary
 from ._models_py3 import NameInfo
 from ._models_py3 import OperationResource
@@ -68,18 +70,20 @@
 from ._models_py3 import VaultPropertiesMoveDetails
 from ._models_py3 import VaultPropertiesRedundancySettings
 from ._models_py3 import VaultUsage
 from ._models_py3 import VaultUsageList
 
 from ._recovery_services_client_enums import AlertsState
 from ._recovery_services_client_enums import AuthType
+from ._recovery_services_client_enums import BCDRSecurityLevel
 from ._recovery_services_client_enums import BackupStorageVersion
 from ._recovery_services_client_enums import CreatedByType
 from ._recovery_services_client_enums import CrossRegionRestore
 from ._recovery_services_client_enums import CrossSubscriptionRestoreState
+from ._recovery_services_client_enums import EnhancedSecurityState
 from ._recovery_services_client_enums import ImmutabilityState
 from ._recovery_services_client_enums import InfrastructureEncryptionState
 from ._recovery_services_client_enums import MultiUserAuthorization
 from ._recovery_services_client_enums import PrivateEndpointConnectionStatus
 from ._recovery_services_client_enums import ProvisioningState
 from ._recovery_services_client_enums import PublicNetworkAccess
 from ._recovery_services_client_enums import ResourceIdentityType
@@ -115,14 +119,16 @@
     "CmkKekIdentity",
     "CmkKeyVaultProperties",
     "CrossSubscriptionRestoreSettings",
     "DNSZone",
     "DNSZoneResponse",
     "Error",
     "ErrorAdditionalInfo",
+    "ErrorDetail",
+    "ErrorResponse",
     "IdentityData",
     "ImmutabilitySettings",
     "JobsSummary",
     "MonitoringSettings",
     "MonitoringSummary",
     "NameInfo",
     "OperationResource",
@@ -159,18 +165,20 @@
     "VaultPropertiesEncryption",
     "VaultPropertiesMoveDetails",
     "VaultPropertiesRedundancySettings",
     "VaultUsage",
     "VaultUsageList",
     "AlertsState",
     "AuthType",
+    "BCDRSecurityLevel",
     "BackupStorageVersion",
     "CreatedByType",
     "CrossRegionRestore",
     "CrossSubscriptionRestoreState",
+    "EnhancedSecurityState",
     "ImmutabilityState",
     "InfrastructureEncryptionState",
     "MultiUserAuthorization",
     "PrivateEndpointConnectionStatus",
     "ProvisioningState",
     "PublicNetworkAccess",
     "ResourceIdentityType",
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/models/_models_py3.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/models/_models_py3.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,49 @@
 
 
 class AzureMonitorAlertSettings(_serialization.Model):
     """Settings for Azure Monitor based alerts.
 
     :ivar alerts_for_all_job_failures: Known values are: "Enabled" and "Disabled".
     :vartype alerts_for_all_job_failures: str or ~azure.mgmt.recoveryservices.models.AlertsState
+    :ivar alerts_for_all_replication_issues: Known values are: "Enabled" and "Disabled".
+    :vartype alerts_for_all_replication_issues: str or
+     ~azure.mgmt.recoveryservices.models.AlertsState
+    :ivar alerts_for_all_failover_issues: Known values are: "Enabled" and "Disabled".
+    :vartype alerts_for_all_failover_issues: str or ~azure.mgmt.recoveryservices.models.AlertsState
     """
 
     _attribute_map = {
         "alerts_for_all_job_failures": {"key": "alertsForAllJobFailures", "type": "str"},
+        "alerts_for_all_replication_issues": {"key": "alertsForAllReplicationIssues", "type": "str"},
+        "alerts_for_all_failover_issues": {"key": "alertsForAllFailoverIssues", "type": "str"},
     }
 
     def __init__(
-        self, *, alerts_for_all_job_failures: Optional[Union[str, "_models.AlertsState"]] = None, **kwargs: Any
+        self,
+        *,
+        alerts_for_all_job_failures: Optional[Union[str, "_models.AlertsState"]] = None,
+        alerts_for_all_replication_issues: Optional[Union[str, "_models.AlertsState"]] = None,
+        alerts_for_all_failover_issues: Optional[Union[str, "_models.AlertsState"]] = None,
+        **kwargs: Any
     ) -> None:
         """
         :keyword alerts_for_all_job_failures: Known values are: "Enabled" and "Disabled".
         :paramtype alerts_for_all_job_failures: str or ~azure.mgmt.recoveryservices.models.AlertsState
+        :keyword alerts_for_all_replication_issues: Known values are: "Enabled" and "Disabled".
+        :paramtype alerts_for_all_replication_issues: str or
+         ~azure.mgmt.recoveryservices.models.AlertsState
+        :keyword alerts_for_all_failover_issues: Known values are: "Enabled" and "Disabled".
+        :paramtype alerts_for_all_failover_issues: str or
+         ~azure.mgmt.recoveryservices.models.AlertsState
         """
         super().__init__(**kwargs)
         self.alerts_for_all_job_failures = alerts_for_all_job_failures
+        self.alerts_for_all_replication_issues = alerts_for_all_replication_issues
+        self.alerts_for_all_failover_issues = alerts_for_all_failover_issues
 
 
 class CapabilitiesProperties(_serialization.Model):
     """Capabilities information.
 
     :ivar dns_zones:
     :vartype dns_zones: list[~azure.mgmt.recoveryservices.models.DNSZone]
@@ -58,15 +78,15 @@
         super().__init__(**kwargs)
         self.dns_zones = dns_zones
 
 
 class ResourceCapabilitiesBase(_serialization.Model):
     """Base class for request and response capabilities information for Microsoft.RecoveryServices.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar type: Describes the Resource type: Microsoft.RecoveryServices/Vaults. Required.
     :vartype type: str
     """
 
     _validation = {
         "type": {"required": True},
@@ -84,15 +104,15 @@
         super().__init__(**kwargs)
         self.type = type
 
 
 class CapabilitiesResponse(ResourceCapabilitiesBase):
     """Capabilities response for Microsoft.RecoveryServices.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar type: Describes the Resource type: Microsoft.RecoveryServices/Vaults. Required.
     :vartype type: str
     :ivar properties: Capabilities properties in response.
     :vartype properties: ~azure.mgmt.recoveryservices.models.CapabilitiesResponseProperties
     """
 
@@ -225,30 +245,42 @@
 
 
 class ClassicAlertSettings(_serialization.Model):
     """Settings for classic alerts.
 
     :ivar alerts_for_critical_operations: Known values are: "Enabled" and "Disabled".
     :vartype alerts_for_critical_operations: str or ~azure.mgmt.recoveryservices.models.AlertsState
+    :ivar email_notifications_for_site_recovery: Known values are: "Enabled" and "Disabled".
+    :vartype email_notifications_for_site_recovery: str or
+     ~azure.mgmt.recoveryservices.models.AlertsState
     """
 
     _attribute_map = {
         "alerts_for_critical_operations": {"key": "alertsForCriticalOperations", "type": "str"},
+        "email_notifications_for_site_recovery": {"key": "emailNotificationsForSiteRecovery", "type": "str"},
     }
 
     def __init__(
-        self, *, alerts_for_critical_operations: Optional[Union[str, "_models.AlertsState"]] = None, **kwargs: Any
+        self,
+        *,
+        alerts_for_critical_operations: Optional[Union[str, "_models.AlertsState"]] = None,
+        email_notifications_for_site_recovery: Optional[Union[str, "_models.AlertsState"]] = None,
+        **kwargs: Any
     ) -> None:
         """
         :keyword alerts_for_critical_operations: Known values are: "Enabled" and "Disabled".
         :paramtype alerts_for_critical_operations: str or
          ~azure.mgmt.recoveryservices.models.AlertsState
+        :keyword email_notifications_for_site_recovery: Known values are: "Enabled" and "Disabled".
+        :paramtype email_notifications_for_site_recovery: str or
+         ~azure.mgmt.recoveryservices.models.AlertsState
         """
         super().__init__(**kwargs)
         self.alerts_for_critical_operations = alerts_for_critical_operations
+        self.email_notifications_for_site_recovery = email_notifications_for_site_recovery
 
 
 class ClientDiscoveryDisplay(_serialization.Model):
     """Localized display information of an operation.
 
     :ivar provider: Name of the provider for display purposes.
     :vartype provider: str
@@ -673,33 +705,97 @@
     def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.info = None
         self.type = None
 
 
+class ErrorDetail(_serialization.Model):
+    """The error detail.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar code: The error code.
+    :vartype code: str
+    :ivar message: The error message.
+    :vartype message: str
+    :ivar target: The error target.
+    :vartype target: str
+    :ivar details: The error details.
+    :vartype details: list[~azure.mgmt.recoveryservices.models.ErrorDetail]
+    :ivar additional_info: The error additional info.
+    :vartype additional_info: list[~azure.mgmt.recoveryservices.models.ErrorAdditionalInfo]
+    """
+
+    _validation = {
+        "code": {"readonly": True},
+        "message": {"readonly": True},
+        "target": {"readonly": True},
+        "details": {"readonly": True},
+        "additional_info": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "code": {"key": "code", "type": "str"},
+        "message": {"key": "message", "type": "str"},
+        "target": {"key": "target", "type": "str"},
+        "details": {"key": "details", "type": "[ErrorDetail]"},
+        "additional_info": {"key": "additionalInfo", "type": "[ErrorAdditionalInfo]"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.code = None
+        self.message = None
+        self.target = None
+        self.details = None
+        self.additional_info = None
+
+
+class ErrorResponse(_serialization.Model):
+    """Common error response for all Azure Resource Manager APIs to return error details for failed
+    operations. (This also follows the OData error response format.).
+
+    :ivar error: The error object.
+    :vartype error: ~azure.mgmt.recoveryservices.models.ErrorDetail
+    """
+
+    _attribute_map = {
+        "error": {"key": "error", "type": "ErrorDetail"},
+    }
+
+    def __init__(self, *, error: Optional["_models.ErrorDetail"] = None, **kwargs: Any) -> None:
+        """
+        :keyword error: The error object.
+        :paramtype error: ~azure.mgmt.recoveryservices.models.ErrorDetail
+        """
+        super().__init__(**kwargs)
+        self.error = error
+
+
 class IdentityData(_serialization.Model):
     """Identity for the resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar principal_id: The principal ID of resource identity.
     :vartype principal_id: str
     :ivar tenant_id: The tenant ID of resource.
     :vartype tenant_id: str
     :ivar type: The type of managed identity used. The type 'SystemAssigned, UserAssigned' includes
      both an implicitly created identity and a set of user-assigned identities. The type 'None' will
      remove any identities. Required. Known values are: "SystemAssigned", "None", "UserAssigned",
      and "SystemAssigned, UserAssigned".
     :vartype type: str or ~azure.mgmt.recoveryservices.models.ResourceIdentityType
     :ivar user_assigned_identities: The list of user-assigned identities associated with the
      resource. The user-assigned identity dictionary keys will be ARM resource ids in the form:
-     '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}'.
+     '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}'.  # pylint: disable=line-too-long
     :vartype user_assigned_identities: dict[str, ~azure.mgmt.recoveryservices.models.UserIdentity]
     """
 
     _validation = {
         "principal_id": {"readonly": True},
         "tenant_id": {"readonly": True},
         "type": {"required": True},
@@ -723,15 +819,15 @@
         :keyword type: The type of managed identity used. The type 'SystemAssigned, UserAssigned'
          includes both an implicitly created identity and a set of user-assigned identities. The type
          'None' will remove any identities. Required. Known values are: "SystemAssigned", "None",
          "UserAssigned", and "SystemAssigned, UserAssigned".
         :paramtype type: str or ~azure.mgmt.recoveryservices.models.ResourceIdentityType
         :keyword user_assigned_identities: The list of user-assigned identities associated with the
          resource. The user-assigned identity dictionary keys will be ARM resource ids in the form:
-         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}'.
+         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ManagedIdentity/userAssignedIdentities/{identityName}'.  # pylint: disable=line-too-long
         :paramtype user_assigned_identities: dict[str,
          ~azure.mgmt.recoveryservices.models.UserIdentity]
         """
         super().__init__(**kwargs)
         self.principal_id = None
         self.tenant_id = None
         self.type = type
@@ -1227,15 +1323,15 @@
 
 class PrivateEndpointConnectionVaultProperties(_serialization.Model):
     """Information to be stored in Vault properties as an element of privateEndpointConnections List.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Format of id
-     subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.[Service]/{resource}/{resourceName}/privateEndpointConnections/{connectionName}.
+     subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.[Service]/{resource}/{resourceName}/privateEndpointConnections/{connectionName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar properties: Private Endpoint Connection Response Properties.
     :vartype properties: ~azure.mgmt.recoveryservices.models.PrivateEndpointConnection
     :ivar name: The name of the private Endpoint Connection.
     :vartype name: str
     :ivar type: The type, which will be of the format,
      Microsoft.RecoveryServices/vaults/privateEndpointConnections.
@@ -1500,15 +1596,15 @@
         super().__init__(**kwargs)
         self.value = value
 
 
 class ResourceCapabilities(ResourceCapabilitiesBase):
     """Input to get capabilities information for Microsoft.RecoveryServices.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar type: Describes the Resource type: Microsoft.RecoveryServices/Vaults. Required.
     :vartype type: str
     :ivar properties: Capabilities information.
     :vartype properties: ~azure.mgmt.recoveryservices.models.CapabilitiesProperties
     """
 
@@ -1536,15 +1632,15 @@
 
 class ResourceCertificateDetails(_serialization.Model):
     """Certificate details representing the Vault credentials.
 
     You probably want to use the sub-classes and not this class directly. Known sub-classes are:
     ResourceCertificateAndAcsDetails, ResourceCertificateAndAadDetails
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar auth_type: This property will be used as the discriminator for deciding the specific
      types in the polymorphic chain of types. Required.
     :vartype auth_type: str
     :ivar certificate: The base64 encoded certificate raw data string.
     :vartype certificate: bytes
     :ivar friendly_name: Certificate friendly name.
@@ -1628,15 +1724,15 @@
         self.valid_from = valid_from
         self.valid_to = valid_to
 
 
 class ResourceCertificateAndAadDetails(ResourceCertificateDetails):  # pylint: disable=too-many-instance-attributes
     """Certificate details representing the Vault credentials for AAD.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar auth_type: This property will be used as the discriminator for deciding the specific
      types in the polymorphic chain of types. Required.
     :vartype auth_type: str
     :ivar certificate: The base64 encoded certificate raw data string.
     :vartype certificate: bytes
     :ivar friendly_name: Certificate friendly name.
@@ -1769,15 +1865,15 @@
         self.service_resource_id = service_resource_id
         self.aad_audience = aad_audience
 
 
 class ResourceCertificateAndAcsDetails(ResourceCertificateDetails):  # pylint: disable=too-many-instance-attributes
     """Certificate details representing the Vault credentials for ACS.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar auth_type: This property will be used as the discriminator for deciding the specific
      types in the polymorphic chain of types. Required.
     :vartype auth_type: str
     :ivar certificate: The base64 encoded certificate raw data string.
     :vartype certificate: bytes
     :ivar friendly_name: Certificate friendly name.
@@ -1954,15 +2050,15 @@
         self.soft_delete_settings = soft_delete_settings
         self.multi_user_authorization = None
 
 
 class Sku(_serialization.Model):
     """Identifies the unique system identifier for each Azure resource.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar name: Name of SKU is RS0 (Recovery Services 0th version) and the tier is standard tier.
      They do not have affect on backend storage redundancy or any other vault settings. To manage
      storage redundancy, use the backupstorageconfig. Required. Known values are: "Standard" and
      "RS0".
     :vartype name: str or ~azure.mgmt.recoveryservices.models.SkuName
     :ivar tier: The Sku tier.
@@ -2023,37 +2119,48 @@
 class SoftDeleteSettings(_serialization.Model):
     """Soft delete Settings of vault.
 
     :ivar soft_delete_state: Known values are: "Invalid", "Enabled", "Disabled", and "AlwaysON".
     :vartype soft_delete_state: str or ~azure.mgmt.recoveryservices.models.SoftDeleteState
     :ivar soft_delete_retention_period_in_days: Soft delete retention period in days.
     :vartype soft_delete_retention_period_in_days: int
+    :ivar enhanced_security_state: Known values are: "Invalid", "Enabled", "Disabled", and
+     "AlwaysON".
+    :vartype enhanced_security_state: str or
+     ~azure.mgmt.recoveryservices.models.EnhancedSecurityState
     """
 
     _attribute_map = {
         "soft_delete_state": {"key": "softDeleteState", "type": "str"},
         "soft_delete_retention_period_in_days": {"key": "softDeleteRetentionPeriodInDays", "type": "int"},
+        "enhanced_security_state": {"key": "enhancedSecurityState", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         soft_delete_state: Optional[Union[str, "_models.SoftDeleteState"]] = None,
         soft_delete_retention_period_in_days: Optional[int] = None,
+        enhanced_security_state: Optional[Union[str, "_models.EnhancedSecurityState"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword soft_delete_state: Known values are: "Invalid", "Enabled", "Disabled", and "AlwaysON".
         :paramtype soft_delete_state: str or ~azure.mgmt.recoveryservices.models.SoftDeleteState
         :keyword soft_delete_retention_period_in_days: Soft delete retention period in days.
         :paramtype soft_delete_retention_period_in_days: int
+        :keyword enhanced_security_state: Known values are: "Invalid", "Enabled", "Disabled", and
+         "AlwaysON".
+        :paramtype enhanced_security_state: str or
+         ~azure.mgmt.recoveryservices.models.EnhancedSecurityState
         """
         super().__init__(**kwargs)
         self.soft_delete_state = soft_delete_state
         self.soft_delete_retention_period_in_days = soft_delete_retention_period_in_days
+        self.enhanced_security_state = enhanced_security_state
 
 
 class SystemData(_serialization.Model):
     """Metadata pertaining to creation and last modification of the resource.
 
     :ivar created_by: The identity that created the resource.
     :vartype created_by: str
@@ -2117,15 +2224,15 @@
 
 
 class TrackedResource(Resource):
     """Tracked resource with location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Resource Id represents the complete path to the resource.
     :vartype id: str
     :ivar name: Resource name associated with the resource.
     :vartype name: str
     :ivar type: Resource type represents the complete path of the form
      Namespace/ResourceType/ResourceType/...
@@ -2264,15 +2371,15 @@
 
 
 class Vault(TrackedResource):
     """Resource information, as returned by the resource provider.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Resource Id represents the complete path to the resource.
     :vartype id: str
     :ivar name: Resource name associated with the resource.
     :vartype name: str
     :ivar type: Resource type represents the complete path of the form
      Namespace/ResourceType/ResourceType/...
@@ -2531,24 +2638,31 @@
     :vartype redundancy_settings:
      ~azure.mgmt.recoveryservices.models.VaultPropertiesRedundancySettings
     :ivar security_settings: Security Settings of the vault.
     :vartype security_settings: ~azure.mgmt.recoveryservices.models.SecuritySettings
     :ivar secure_score: Secure Score of Recovery Services Vault. Known values are: "None",
      "Minimum", "Adequate", and "Maximum".
     :vartype secure_score: str or ~azure.mgmt.recoveryservices.models.SecureScoreLevel
+    :ivar bcdr_security_level: Security levels of Recovery Services Vault for business continuity
+     and disaster recovery. Known values are: "Poor", "Fair", "Good", and "Excellent".
+    :vartype bcdr_security_level: str or ~azure.mgmt.recoveryservices.models.BCDRSecurityLevel
+    :ivar resource_guard_operation_requests: ResourceGuardOperationRequests on which LAC check will
+     be performed.
+    :vartype resource_guard_operation_requests: list[str]
     """
 
     _validation = {
         "provisioning_state": {"readonly": True},
         "private_endpoint_connections": {"readonly": True},
         "private_endpoint_state_for_backup": {"readonly": True},
         "private_endpoint_state_for_site_recovery": {"readonly": True},
         "move_state": {"readonly": True},
         "backup_storage_version": {"readonly": True},
         "secure_score": {"readonly": True},
+        "bcdr_security_level": {"readonly": True},
     }
 
     _attribute_map = {
         "provisioning_state": {"key": "provisioningState", "type": "str"},
         "upgrade_details": {"key": "upgradeDetails", "type": "UpgradeDetails"},
         "private_endpoint_connections": {
             "key": "privateEndpointConnections",
@@ -2562,27 +2676,30 @@
         "backup_storage_version": {"key": "backupStorageVersion", "type": "str"},
         "public_network_access": {"key": "publicNetworkAccess", "type": "str"},
         "monitoring_settings": {"key": "monitoringSettings", "type": "MonitoringSettings"},
         "restore_settings": {"key": "restoreSettings", "type": "RestoreSettings"},
         "redundancy_settings": {"key": "redundancySettings", "type": "VaultPropertiesRedundancySettings"},
         "security_settings": {"key": "securitySettings", "type": "SecuritySettings"},
         "secure_score": {"key": "secureScore", "type": "str"},
+        "bcdr_security_level": {"key": "bcdrSecurityLevel", "type": "str"},
+        "resource_guard_operation_requests": {"key": "resourceGuardOperationRequests", "type": "[str]"},
     }
 
     def __init__(
         self,
         *,
         upgrade_details: Optional["_models.UpgradeDetails"] = None,
         encryption: Optional["_models.VaultPropertiesEncryption"] = None,
         move_details: Optional["_models.VaultPropertiesMoveDetails"] = None,
         public_network_access: Optional[Union[str, "_models.PublicNetworkAccess"]] = None,
         monitoring_settings: Optional["_models.MonitoringSettings"] = None,
         restore_settings: Optional["_models.RestoreSettings"] = None,
         redundancy_settings: Optional["_models.VaultPropertiesRedundancySettings"] = None,
         security_settings: Optional["_models.SecuritySettings"] = None,
+        resource_guard_operation_requests: Optional[List[str]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword upgrade_details: Details for upgrading vault.
         :paramtype upgrade_details: ~azure.mgmt.recoveryservices.models.UpgradeDetails
         :keyword encryption: Customer Managed Key details of the resource.
         :paramtype encryption: ~azure.mgmt.recoveryservices.models.VaultPropertiesEncryption
@@ -2598,14 +2715,17 @@
         :keyword restore_settings: Restore Settings of the vault.
         :paramtype restore_settings: ~azure.mgmt.recoveryservices.models.RestoreSettings
         :keyword redundancy_settings: The redundancy Settings of a Vault.
         :paramtype redundancy_settings:
          ~azure.mgmt.recoveryservices.models.VaultPropertiesRedundancySettings
         :keyword security_settings: Security Settings of the vault.
         :paramtype security_settings: ~azure.mgmt.recoveryservices.models.SecuritySettings
+        :keyword resource_guard_operation_requests: ResourceGuardOperationRequests on which LAC check
+         will be performed.
+        :paramtype resource_guard_operation_requests: list[str]
         """
         super().__init__(**kwargs)
         self.provisioning_state = None
         self.upgrade_details = upgrade_details
         self.private_endpoint_connections = None
         self.private_endpoint_state_for_backup = None
         self.private_endpoint_state_for_site_recovery = None
@@ -2615,14 +2735,16 @@
         self.backup_storage_version = None
         self.public_network_access = public_network_access
         self.monitoring_settings = monitoring_settings
         self.restore_settings = restore_settings
         self.redundancy_settings = redundancy_settings
         self.security_settings = security_settings
         self.secure_score = None
+        self.bcdr_security_level = None
+        self.resource_guard_operation_requests = resource_guard_operation_requests
 
 
 class VaultPropertiesEncryption(_serialization.Model):
     """Customer Managed Key details of the resource.
 
     :ivar key_vault_properties: The properties of the Key Vault which hosts CMK.
     :vartype key_vault_properties: ~azure.mgmt.recoveryservices.models.CmkKeyVaultProperties
@@ -2706,40 +2828,47 @@
         self.source_resource_id = None
         self.target_resource_id = None
 
 
 class VaultPropertiesRedundancySettings(_serialization.Model):
     """The redundancy Settings of a Vault.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     :ivar standard_tier_storage_redundancy: The storage redundancy setting of a vault. Known values
-     are: "LocallyRedundant", "GeoRedundant", and "ZoneRedundant".
+     are: "Invalid", "LocallyRedundant", "GeoRedundant", and "ZoneRedundant".
     :vartype standard_tier_storage_redundancy: str or
      ~azure.mgmt.recoveryservices.models.StandardTierStorageRedundancy
     :ivar cross_region_restore: Flag to show if Cross Region Restore is enabled on the Vault or
      not. Known values are: "Enabled" and "Disabled".
     :vartype cross_region_restore: str or ~azure.mgmt.recoveryservices.models.CrossRegionRestore
     """
 
-    _validation = {
-        "standard_tier_storage_redundancy": {"readonly": True},
-        "cross_region_restore": {"readonly": True},
-    }
-
     _attribute_map = {
         "standard_tier_storage_redundancy": {"key": "standardTierStorageRedundancy", "type": "str"},
         "cross_region_restore": {"key": "crossRegionRestore", "type": "str"},
     }
 
-    def __init__(self, **kwargs: Any) -> None:
-        """ """
+    def __init__(
+        self,
+        *,
+        standard_tier_storage_redundancy: Optional[Union[str, "_models.StandardTierStorageRedundancy"]] = None,
+        cross_region_restore: Optional[Union[str, "_models.CrossRegionRestore"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword standard_tier_storage_redundancy: The storage redundancy setting of a vault. Known
+         values are: "Invalid", "LocallyRedundant", "GeoRedundant", and "ZoneRedundant".
+        :paramtype standard_tier_storage_redundancy: str or
+         ~azure.mgmt.recoveryservices.models.StandardTierStorageRedundancy
+        :keyword cross_region_restore: Flag to show if Cross Region Restore is enabled on the Vault or
+         not. Known values are: "Enabled" and "Disabled".
+        :paramtype cross_region_restore: str or ~azure.mgmt.recoveryservices.models.CrossRegionRestore
+        """
         super().__init__(**kwargs)
-        self.standard_tier_storage_redundancy = None
-        self.cross_region_restore = None
+        self.standard_tier_storage_redundancy = standard_tier_storage_redundancy
+        self.cross_region_restore = cross_region_restore
 
 
 class VaultUsage(_serialization.Model):
     """Usages of a vault.
 
     :ivar unit: Unit of the usage. Known values are: "Count", "Bytes", "Seconds", "Percent",
      "CountPerSecond", and "BytesPerSecond".
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/models/_patch.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/models/_recovery_services_client_enums.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/models/_recovery_services_client_enums.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,23 @@
     """Backup storage version."""
 
     V1 = "V1"
     V2 = "V2"
     UNASSIGNED = "Unassigned"
 
 
+class BCDRSecurityLevel(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Security levels of Recovery Services Vault for business continuity and disaster recovery."""
+
+    POOR = "Poor"
+    FAIR = "Fair"
+    GOOD = "Good"
+    EXCELLENT = "Excellent"
+
+
 class CreatedByType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of identity that created the resource."""
 
     USER = "User"
     APPLICATION = "Application"
     MANAGED_IDENTITY = "ManagedIdentity"
     KEY = "Key"
@@ -55,14 +64,23 @@
     """CrossSubscriptionRestoreState."""
 
     ENABLED = "Enabled"
     DISABLED = "Disabled"
     PERMANENTLY_DISABLED = "PermanentlyDisabled"
 
 
+class EnhancedSecurityState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """EnhancedSecurityState."""
+
+    INVALID = "Invalid"
+    ENABLED = "Enabled"
+    DISABLED = "Disabled"
+    ALWAYS_ON = "AlwaysON"
+
+
 class ImmutabilityState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """ImmutabilityState."""
 
     DISABLED = "Disabled"
     UNLOCKED = "Unlocked"
     LOCKED = "Locked"
 
@@ -161,14 +179,15 @@
     DISABLED = "Disabled"
     ALWAYS_ON = "AlwaysON"
 
 
 class StandardTierStorageRedundancy(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The storage redundancy setting of a vault."""
 
+    INVALID = "Invalid"
     LOCALLY_REDUNDANT = "LocallyRedundant"
     GEO_REDUNDANT = "GeoRedundant"
     ZONE_REDUNDANT = "ZoneRedundant"
 
 
 class TriggerType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The way the vault upgrade was triggered."""
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/__init__.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_operations.py`

 * *Files 4% similar despite different names*

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
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.RecoveryServices/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -74,15 +74,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.ClientDiscoveryValueForSingleApi"]:
         """Returns the list of available operations.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ClientDiscoveryValueForSingleApi or the result of
          cls(response)
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.recoveryservices.models.ClientDiscoveryValueForSingleApi]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -98,59 +97,56 @@
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
             deserialized = self._deserialize("ClientDiscoveryResponse", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/providers/Microsoft.RecoveryServices/operations"}
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_patch.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_private_link_resources_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_private_link_resources_operations.py`

 * *Files 4% similar despite different names*

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
 
 
 def build_list_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/privateLinkResources",
     )  # pylint: disable=line-too-long
@@ -69,15 +69,15 @@
 
 def build_get_request(
     resource_group_name: str, vault_name: str, private_link_resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/privateLinkResources/{privateLinkResourceName}",
     )  # pylint: disable=line-too-long
@@ -127,15 +127,14 @@
         Returns the list of private link resources that need to be created for Backup and SiteRecovery.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateLinkResource or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.recoveryservices.models.PrivateLinkResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -149,72 +148,67 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     vault_name=vault_name,
                     subscription_id=self._config.subscription_id,
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
             deserialized = self._deserialize("PrivateLinkResources", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/privateLinkResources"
-    }
-
     @distributed_trace
     def get(
         self, resource_group_name: str, vault_name: str, private_link_resource_name: str, **kwargs: Any
     ) -> _models.PrivateLinkResource:
         """Returns a specified private link resource that need to be created for Backup and SiteRecovery.
 
         Returns a specified private link resource that need to be created for Backup and SiteRecovery.
@@ -222,15 +216,14 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param private_link_resource_name: Required.
         :type private_link_resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkResource or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.PrivateLinkResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -241,41 +234,36 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkResource] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             private_link_resource_name=private_link_resource_name,
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/privateLinkResources/{privateLinkResourceName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_recovery_services_client_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_recovery_services_client_operations.py`

 * *Files 4% similar despite different names*

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
 
 def build_get_operation_status_request(
     resource_group_name: str, vault_name: str, operation_id: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/operationStatus/{operationId}",
     )  # pylint: disable=line-too-long
@@ -70,15 +70,15 @@
 
 def build_get_operation_result_request(
     resource_group_name: str, vault_name: str, operation_id: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/operationResults/{operationId}",
     )  # pylint: disable=line-too-long
@@ -112,15 +112,14 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param operation_id: Required.
         :type operation_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: OperationResource or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.OperationResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -131,63 +130,57 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationResource] = kwargs.pop("cls", None)
 
-        request = build_get_operation_status_request(
+        _request = build_get_operation_status_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_operation_status.metadata["url"],
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("OperationResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get_operation_status.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/operationStatus/{operationId}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def get_operation_result(
         self, resource_group_name: str, vault_name: str, operation_id: str, **kwargs: Any
     ) -> Optional[_models.Vault]:
         """Gets the operation result for a resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param operation_id: Required.
         :type operation_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Vault or None or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.Vault or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -198,43 +191,38 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.Vault]] = kwargs.pop("cls", None)
 
-        request = build_get_operation_result_request(
+        _request = build_get_operation_result_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             operation_id=operation_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_operation_result.metadata["url"],
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("Vault", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get_operation_result.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/operationResults/{operationId}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_recovery_services_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_vault_extended_info_operations.py`

 * *Files 19% similar despite different names*

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
@@ -31,210 +31,266 @@
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_check_name_availability_request(
-    resource_group_name: str, location: str, subscription_id: str, **kwargs: Any
+def build_get_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/extendedInformation/vaultExtendedInfo",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
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
+    resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/locations/{location}/checkNameAvailability",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/extendedInformation/vaultExtendedInfo",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "location": _SERIALIZER.url("location", location, "str"),
+        "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_capabilities_request(location: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_update_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/providers/Microsoft.RecoveryServices/locations/{location}/capabilities",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/extendedInformation/vaultExtendedInfo",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "location": _SERIALIZER.url("location", location, "str"),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "vaultName": _SERIALIZER.url("vault_name", vault_name, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+    return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class RecoveryServicesOperations:
+class VaultExtendedInfoOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.recoveryservices.RecoveryServicesClient`'s
-        :attr:`recovery_services` attribute.
+        :attr:`vault_extended_info` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
+    @distributed_trace
+    def get(self, resource_group_name: str, vault_name: str, **kwargs: Any) -> _models.VaultExtendedInfoResource:
+        """Get the vault extended info.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param vault_name: The name of the recovery services vault. Required.
+        :type vault_name: str
+        :return: VaultExtendedInfoResource or the result of cls(response)
+        :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
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
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.VaultExtendedInfoResource] = kwargs.pop("cls", None)
+
+        _request = build_get_request(
+            resource_group_name=resource_group_name,
+            vault_name=vault_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
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
+            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("VaultExtendedInfoResource", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
     @overload
-    def check_name_availability(
+    def create_or_update(
         self,
         resource_group_name: str,
-        location: str,
-        input: _models.CheckNameAvailabilityParameters,
+        vault_name: str,
+        resource_extended_info_details: _models.VaultExtendedInfoResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.CheckNameAvailabilityResult:
-        """API to check for resource name availability.
-        A name is available if no other resource exists that has the same SubscriptionId, Resource Name
-        and Type
-        or if one or more such resources exist, each of these must be GC'd and their time of deletion
-        be more than 24 Hours Ago.
-
-        API to check for resource name availability.
-        A name is available if no other resource exists that has the same SubscriptionId, Resource Name
-        and Type
-        or if one or more such resources exist, each of these must be GC'd and their time of deletion
-        be more than 24 Hours Ago.
+    ) -> _models.VaultExtendedInfoResource:
+        """Create vault extended info.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param location: Location of the resource. Required.
-        :type location: str
-        :param input: Contains information about Resource type and Resource name. Required.
-        :type input: ~azure.mgmt.recoveryservices.models.CheckNameAvailabilityParameters
+        :param vault_name: The name of the recovery services vault. Required.
+        :type vault_name: str
+        :param resource_extended_info_details: Details of ResourceExtendedInfo. Required.
+        :type resource_extended_info_details:
+         ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CheckNameAvailabilityResult or the result of cls(response)
-        :rtype: ~azure.mgmt.recoveryservices.models.CheckNameAvailabilityResult
+        :return: VaultExtendedInfoResource or the result of cls(response)
+        :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    def check_name_availability(
+    def create_or_update(
         self,
         resource_group_name: str,
-        location: str,
-        input: IO,
+        vault_name: str,
+        resource_extended_info_details: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.CheckNameAvailabilityResult:
-        """API to check for resource name availability.
-        A name is available if no other resource exists that has the same SubscriptionId, Resource Name
-        and Type
-        or if one or more such resources exist, each of these must be GC'd and their time of deletion
-        be more than 24 Hours Ago.
-
-        API to check for resource name availability.
-        A name is available if no other resource exists that has the same SubscriptionId, Resource Name
-        and Type
-        or if one or more such resources exist, each of these must be GC'd and their time of deletion
-        be more than 24 Hours Ago.
+    ) -> _models.VaultExtendedInfoResource:
+        """Create vault extended info.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param location: Location of the resource. Required.
-        :type location: str
-        :param input: Contains information about Resource type and Resource name. Required.
-        :type input: IO
+        :param vault_name: The name of the recovery services vault. Required.
+        :type vault_name: str
+        :param resource_extended_info_details: Details of ResourceExtendedInfo. Required.
+        :type resource_extended_info_details: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CheckNameAvailabilityResult or the result of cls(response)
-        :rtype: ~azure.mgmt.recoveryservices.models.CheckNameAvailabilityResult
+        :return: VaultExtendedInfoResource or the result of cls(response)
+        :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
-    def check_name_availability(
+    def create_or_update(
         self,
         resource_group_name: str,
-        location: str,
-        input: Union[_models.CheckNameAvailabilityParameters, IO],
+        vault_name: str,
+        resource_extended_info_details: Union[_models.VaultExtendedInfoResource, IO[bytes]],
         **kwargs: Any
-    ) -> _models.CheckNameAvailabilityResult:
-        """API to check for resource name availability.
-        A name is available if no other resource exists that has the same SubscriptionId, Resource Name
-        and Type
-        or if one or more such resources exist, each of these must be GC'd and their time of deletion
-        be more than 24 Hours Ago.
-
-        API to check for resource name availability.
-        A name is available if no other resource exists that has the same SubscriptionId, Resource Name
-        and Type
-        or if one or more such resources exist, each of these must be GC'd and their time of deletion
-        be more than 24 Hours Ago.
+    ) -> _models.VaultExtendedInfoResource:
+        """Create vault extended info.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param location: Location of the resource. Required.
-        :type location: str
-        :param input: Contains information about Resource type and Resource name. Is either a
-         CheckNameAvailabilityParameters type or a IO type. Required.
-        :type input: ~azure.mgmt.recoveryservices.models.CheckNameAvailabilityParameters or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CheckNameAvailabilityResult or the result of cls(response)
-        :rtype: ~azure.mgmt.recoveryservices.models.CheckNameAvailabilityResult
+        :param vault_name: The name of the recovery services vault. Required.
+        :type vault_name: str
+        :param resource_extended_info_details: Details of ResourceExtendedInfo. Is either a
+         VaultExtendedInfoResource type or a IO[bytes] type. Required.
+        :type resource_extended_info_details:
+         ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource or IO[bytes]
+        :return: VaultExtendedInfoResource or the result of cls(response)
+        :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -242,129 +298,132 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.CheckNameAvailabilityResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.VaultExtendedInfoResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(input, (IOBase, bytes)):
-            _content = input
+        if isinstance(resource_extended_info_details, (IOBase, bytes)):
+            _content = resource_extended_info_details
         else:
-            _json = self._serialize.body(input, "CheckNameAvailabilityParameters")
+            _json = self._serialize.body(resource_extended_info_details, "VaultExtendedInfoResource")
 
-        request = build_check_name_availability_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
-            location=location,
+            vault_name=vault_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.check_name_availability.metadata["url"],
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("CheckNameAvailabilityResult", pipeline_response)
+        deserialized = self._deserialize("VaultExtendedInfoResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    check_name_availability.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/locations/{location}/checkNameAvailability"
-    }
+        return deserialized  # type: ignore
 
     @overload
-    def capabilities(
+    def update(
         self,
-        location: str,
-        input: _models.ResourceCapabilities,
+        resource_group_name: str,
+        vault_name: str,
+        resource_extended_info_details: _models.VaultExtendedInfoResource,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.CapabilitiesResponse:
-        """API to get details about capabilities provided by Microsoft.RecoveryServices RP.
-
-        API to get details about capabilities provided by Microsoft.RecoveryServices RP.
+    ) -> _models.VaultExtendedInfoResource:
+        """Update vault extended info.
 
-        :param location: Location of the resource. Required.
-        :type location: str
-        :param input: Contains information about Resource type and properties to get capabilities.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
-        :type input: ~azure.mgmt.recoveryservices.models.ResourceCapabilities
+        :type resource_group_name: str
+        :param vault_name: The name of the recovery services vault. Required.
+        :type vault_name: str
+        :param resource_extended_info_details: Details of ResourceExtendedInfo. Required.
+        :type resource_extended_info_details:
+         ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CapabilitiesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.recoveryservices.models.CapabilitiesResponse
+        :return: VaultExtendedInfoResource or the result of cls(response)
+        :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    def capabilities(
-        self, location: str, input: IO, *, content_type: str = "application/json", **kwargs: Any
-    ) -> _models.CapabilitiesResponse:
-        """API to get details about capabilities provided by Microsoft.RecoveryServices RP.
-
-        API to get details about capabilities provided by Microsoft.RecoveryServices RP.
-
-        :param location: Location of the resource. Required.
-        :type location: str
-        :param input: Contains information about Resource type and properties to get capabilities.
+    def update(
+        self,
+        resource_group_name: str,
+        vault_name: str,
+        resource_extended_info_details: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.VaultExtendedInfoResource:
+        """Update vault extended info.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
-        :type input: IO
+        :type resource_group_name: str
+        :param vault_name: The name of the recovery services vault. Required.
+        :type vault_name: str
+        :param resource_extended_info_details: Details of ResourceExtendedInfo. Required.
+        :type resource_extended_info_details: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CapabilitiesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.recoveryservices.models.CapabilitiesResponse
+        :return: VaultExtendedInfoResource or the result of cls(response)
+        :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
-    def capabilities(
-        self, location: str, input: Union[_models.ResourceCapabilities, IO], **kwargs: Any
-    ) -> _models.CapabilitiesResponse:
-        """API to get details about capabilities provided by Microsoft.RecoveryServices RP.
-
-        API to get details about capabilities provided by Microsoft.RecoveryServices RP.
-
-        :param location: Location of the resource. Required.
-        :type location: str
-        :param input: Contains information about Resource type and properties to get capabilities. Is
-         either a ResourceCapabilities type or a IO type. Required.
-        :type input: ~azure.mgmt.recoveryservices.models.ResourceCapabilities or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: CapabilitiesResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.recoveryservices.models.CapabilitiesResponse
+    def update(
+        self,
+        resource_group_name: str,
+        vault_name: str,
+        resource_extended_info_details: Union[_models.VaultExtendedInfoResource, IO[bytes]],
+        **kwargs: Any
+    ) -> _models.VaultExtendedInfoResource:
+        """Update vault extended info.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param vault_name: The name of the recovery services vault. Required.
+        :type vault_name: str
+        :param resource_extended_info_details: Details of ResourceExtendedInfo. Is either a
+         VaultExtendedInfoResource type or a IO[bytes] type. Required.
+        :type resource_extended_info_details:
+         ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource or IO[bytes]
+        :return: VaultExtendedInfoResource or the result of cls(response)
+        :rtype: ~azure.mgmt.recoveryservices.models.VaultExtendedInfoResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -372,52 +431,48 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.CapabilitiesResponse] = kwargs.pop("cls", None)
+        cls: ClsType[_models.VaultExtendedInfoResource] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(input, (IOBase, bytes)):
-            _content = input
+        if isinstance(resource_extended_info_details, (IOBase, bytes)):
+            _content = resource_extended_info_details
         else:
-            _json = self._serialize.body(input, "ResourceCapabilities")
+            _json = self._serialize.body(resource_extended_info_details, "VaultExtendedInfoResource")
 
-        request = build_capabilities_request(
-            location=location,
+        _request = build_update_request(
+            resource_group_name=resource_group_name,
+            vault_name=vault_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.capabilities.metadata["url"],
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("CapabilitiesResponse", pipeline_response)
+        deserialized = self._deserialize("VaultExtendedInfoResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    capabilities.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.RecoveryServices/locations/{location}/capabilities"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_registered_identities_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_registered_identities_operations.py`

 * *Files 4% similar despite different names*

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
@@ -35,15 +35,15 @@
 
 
 def build_delete_request(
     resource_group_name: str, vault_name: str, identity_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/registeredIdentities/{identityName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
@@ -90,15 +90,14 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param identity_name: Name of the protection container to unregister. Required.
         :type identity_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -109,37 +108,32 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             identity_name=identity_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
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
 
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
-            return cls(pipeline_response, None, {})
-
-    delete.metadata = {
-        "url": "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/registeredIdentities/{identityName}"
-    }
+            return cls(pipeline_response, None, {})  # type: ignore
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_replication_usages_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_replication_usages_operations.py`

 * *Files 4% similar despite different names*

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
 
 
 def build_list_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/replicationUsages",
     )  # pylint: disable=line-too-long
@@ -91,15 +91,14 @@
         """Fetches the replication usages of the vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ReplicationUsage or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.recoveryservices.models.ReplicationUsage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -113,64 +112,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     vault_name=vault_name,
                     subscription_id=self._config.subscription_id,
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
             deserialized = self._deserialize("ReplicationUsageList", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/replicationUsages"
-    }
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_usages_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_usages_operations.py`

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
@@ -38,15 +38,15 @@
 
 def build_list_by_vaults_request(
     resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/usages",
     )  # pylint: disable=line-too-long
@@ -95,15 +95,14 @@
         """Fetches the usages of the vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either VaultUsage or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.recoveryservices.models.VaultUsage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -117,64 +116,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_vaults_request(
+                _request = build_list_by_vaults_request(
                     resource_group_name=resource_group_name,
                     vault_name=vault_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_vaults.metadata["url"],
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
             deserialized = self._deserialize("VaultUsageList", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list_by_vaults.metadata = {
-        "url": "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/usages"
-    }
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_vault_certificates_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_vault_certificates_operations.py`

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
@@ -37,15 +37,15 @@
 
 def build_create_request(
     resource_group_name: str, vault_name: str, certificate_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/certificates/{certificateName}",
@@ -112,76 +112,70 @@
         :param certificate_name: Certificate friendly name. Required.
         :type certificate_name: str
         :param certificate_request: Input parameters for uploading the vault certificate. Required.
         :type certificate_request: ~azure.mgmt.recoveryservices.models.CertificateRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: VaultCertificateResponse or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultCertificateResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create(
         self,
         resource_group_name: str,
         vault_name: str,
         certificate_name: str,
-        certificate_request: IO,
+        certificate_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.VaultCertificateResponse:
         """Uploads a certificate for a resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param certificate_name: Certificate friendly name. Required.
         :type certificate_name: str
         :param certificate_request: Input parameters for uploading the vault certificate. Required.
-        :type certificate_request: IO
+        :type certificate_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: VaultCertificateResponse or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultCertificateResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create(
         self,
         resource_group_name: str,
         vault_name: str,
         certificate_name: str,
-        certificate_request: Union[_models.CertificateRequest, IO],
+        certificate_request: Union[_models.CertificateRequest, IO[bytes]],
         **kwargs: Any
     ) -> _models.VaultCertificateResponse:
         """Uploads a certificate for a resource.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param certificate_name: Certificate friendly name. Required.
         :type certificate_name: str
         :param certificate_request: Input parameters for uploading the vault certificate. Is either a
-         CertificateRequest type or a IO type. Required.
-        :type certificate_request: ~azure.mgmt.recoveryservices.models.CertificateRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         CertificateRequest type or a IO[bytes] type. Required.
+        :type certificate_request: ~azure.mgmt.recoveryservices.models.CertificateRequest or IO[bytes]
         :return: VaultCertificateResponse or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.VaultCertificateResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -201,44 +195,39 @@
         _json = None
         _content = None
         if isinstance(certificate_request, (IOBase, bytes)):
             _content = certificate_request
         else:
             _json = self._serialize.body(certificate_request, "CertificateRequest")
 
-        request = build_create_request(
+        _request = build_create_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             certificate_name=certificate_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create.metadata["url"],
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("VaultCertificateResponse", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    create.metadata = {
-        "url": "/Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/certificates/{certificateName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure/mgmt/recoveryservices/operations/_vaults_operations.py` & `azure-mgmt-recoveryservices-3.0.0/azure/mgmt/recoveryservices/operations/_vaults_operations.py`

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
@@ -39,15 +39,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_by_subscription_id_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.RecoveryServices/vaults")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
@@ -63,15 +63,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults",
     )  # pylint: disable=line-too-long
@@ -93,15 +93,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}",
     )  # pylint: disable=line-too-long
@@ -121,20 +121,25 @@
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_or_update_request(
-    resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any
+    resource_group_name: str,
+    vault_name: str,
+    subscription_id: str,
+    *,
+    x_ms_authorization_auxiliary: Optional[str] = None,
+    **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}",
@@ -149,26 +154,30 @@
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
+    if x_ms_authorization_auxiliary is not None:
+        _headers["x-ms-authorization-auxiliary"] = _SERIALIZER.header(
+            "x_ms_authorization_auxiliary", x_ms_authorization_auxiliary, "str"
+        )
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_delete_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}",
     )  # pylint: disable=line-too-long
@@ -187,19 +196,26 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_update_request(resource_group_name: str, vault_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_update_request(
+    resource_group_name: str,
+    vault_name: str,
+    subscription_id: str,
+    *,
+    x_ms_authorization_auxiliary: Optional[str] = None,
+    **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-04-01"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}",
@@ -214,14 +230,18 @@
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
+    if x_ms_authorization_auxiliary is not None:
+        _headers["x-ms-authorization-auxiliary"] = _SERIALIZER.header(
+            "x_ms_authorization_auxiliary", x_ms_authorization_auxiliary, "str"
+        )
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
@@ -244,15 +264,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list_by_subscription_id(self, **kwargs: Any) -> Iterable["_models.Vault"]:
         """Fetches all the resources of the specified type in the subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Vault or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -266,78 +285,72 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_subscription_id_request(
+                _request = build_list_by_subscription_id_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_subscription_id.metadata["url"],
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
             deserialized = self._deserialize("VaultList", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_subscription_id.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.RecoveryServices/vaults"
-    }
-
     @distributed_trace
     def list_by_resource_group(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.Vault"]:
         """Retrieve a list of Vaults.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Vault or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -351,81 +364,75 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_resource_group_request(
+                _request = build_list_by_resource_group_request(
                     resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
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
             deserialized = self._deserialize("VaultList", pipeline_response)
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
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults"
-    }
-
     @distributed_trace
     def get(self, resource_group_name: str, vault_name: str, **kwargs: Any) -> _models.Vault:
         """Get the Vault details.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Vault or the result of cls(response)
         :rtype: ~azure.mgmt.recoveryservices.models.Vault
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -436,50 +443,50 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.Vault] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("Vault", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
+        return deserialized  # type: ignore
 
     def _create_or_update_initial(
-        self, resource_group_name: str, vault_name: str, vault: Union[_models.Vault, IO], **kwargs: Any
+        self,
+        resource_group_name: str,
+        vault_name: str,
+        vault: Union[_models.Vault, IO[bytes]],
+        x_ms_authorization_auxiliary: Optional[str] = None,
+        **kwargs: Any
     ) -> _models.Vault:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -496,32 +503,32 @@
         _json = None
         _content = None
         if isinstance(vault, (IOBase, bytes)):
             _content = vault
         else:
             _json = self._serialize.body(vault, "Vault")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
+            x_ms_authorization_auxiliary=x_ms_authorization_auxiliary,
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
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
@@ -533,113 +540,95 @@
             deserialized = self._deserialize("Vault", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
-
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
         vault: _models.Vault,
+        x_ms_authorization_auxiliary: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.Vault]:
         """Creates or updates a Recovery Services vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param vault: Recovery Services Vault to be created. Required.
         :type vault: ~azure.mgmt.recoveryservices.models.Vault
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
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
         :return: An instance of LROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         vault_name: str,
-        vault: IO,
+        vault: IO[bytes],
+        x_ms_authorization_auxiliary: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.Vault]:
         """Creates or updates a Recovery Services vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param vault: Recovery Services Vault to be created. Required.
-        :type vault: IO
+        :type vault: IO[bytes]
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
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
         :return: An instance of LROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
-        self, resource_group_name: str, vault_name: str, vault: Union[_models.Vault, IO], **kwargs: Any
+        self,
+        resource_group_name: str,
+        vault_name: str,
+        vault: Union[_models.Vault, IO[bytes]],
+        x_ms_authorization_auxiliary: Optional[str] = None,
+        **kwargs: Any
     ) -> LROPoller[_models.Vault]:
         """Creates or updates a Recovery Services vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :param vault: Recovery Services Vault to be created. Is either a Vault type or a IO type.
-         Required.
-        :type vault: ~azure.mgmt.recoveryservices.models.Vault or IO
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
+        :param vault: Recovery Services Vault to be created. Is either a Vault type or a IO[bytes]
+         type. Required.
+        :type vault: ~azure.mgmt.recoveryservices.models.Vault or IO[bytes]
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
         :return: An instance of LROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -650,110 +639,153 @@
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 vault_name=vault_name,
                 vault=vault,
+                x_ms_authorization_auxiliary=x_ms_authorization_auxiliary,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Vault", pipeline_response)
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
+            return LROPoller[_models.Vault].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
+        return LROPoller[_models.Vault](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    @distributed_trace
-    def delete(  # pylint: disable=inconsistent-return-statements
+    def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, vault_name: str, **kwargs: Any
     ) -> None:
-        """Deletes a vault.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param vault_name: The name of the recovery services vault. Required.
-        :type vault_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
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
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
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
 
-        if response.status_code not in [200]:
+        if response.status_code not in [202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
+    @distributed_trace
+    def begin_delete(self, resource_group_name: str, vault_name: str, **kwargs: Any) -> LROPoller[None]:
+        """Deletes a vault.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param vault_name: The name of the recovery services vault. Required.
+        :type vault_name: str
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._delete_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                vault_name=vault_name,
+                api_version=api_version,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
+            if cls:
+                return cls(pipeline_response, None, {})  # type: ignore
+
+        if polling is True:
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller[None].from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     def _update_initial(
-        self, resource_group_name: str, vault_name: str, vault: Union[_models.PatchVault, IO], **kwargs: Any
+        self,
+        resource_group_name: str,
+        vault_name: str,
+        vault: Union[_models.PatchVault, IO[bytes]],
+        x_ms_authorization_auxiliary: Optional[str] = None,
+        **kwargs: Any
     ) -> Optional[_models.Vault]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -770,148 +802,130 @@
         _json = None
         _content = None
         if isinstance(vault, (IOBase, bytes)):
             _content = vault
         else:
             _json = self._serialize.body(vault, "PatchVault")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             vault_name=vault_name,
             subscription_id=self._config.subscription_id,
+            x_ms_authorization_auxiliary=x_ms_authorization_auxiliary,
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
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("Vault", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         vault_name: str,
         vault: _models.PatchVault,
+        x_ms_authorization_auxiliary: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.Vault]:
         """Updates the vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param vault: Recovery Services Vault to be created. Required.
         :type vault: ~azure.mgmt.recoveryservices.models.PatchVault
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
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
         :return: An instance of LROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         vault_name: str,
-        vault: IO,
+        vault: IO[bytes],
+        x_ms_authorization_auxiliary: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.Vault]:
         """Updates the vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
         :param vault: Recovery Services Vault to be created. Required.
-        :type vault: IO
+        :type vault: IO[bytes]
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
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
         :return: An instance of LROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_update(
-        self, resource_group_name: str, vault_name: str, vault: Union[_models.PatchVault, IO], **kwargs: Any
+        self,
+        resource_group_name: str,
+        vault_name: str,
+        vault: Union[_models.PatchVault, IO[bytes]],
+        x_ms_authorization_auxiliary: Optional[str] = None,
+        **kwargs: Any
     ) -> LROPoller[_models.Vault]:
         """Updates the vault.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param vault_name: The name of the recovery services vault. Required.
         :type vault_name: str
-        :param vault: Recovery Services Vault to be created. Is either a PatchVault type or a IO type.
-         Required.
-        :type vault: ~azure.mgmt.recoveryservices.models.PatchVault or IO
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
+        :param vault: Recovery Services Vault to be created. Is either a PatchVault type or a IO[bytes]
+         type. Required.
+        :type vault: ~azure.mgmt.recoveryservices.models.PatchVault or IO[bytes]
+        :param x_ms_authorization_auxiliary: Default value is None.
+        :type x_ms_authorization_auxiliary: str
         :return: An instance of LROPoller that returns either Vault or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.recoveryservices.models.Vault]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -922,40 +936,39 @@
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._update_initial(
                 resource_group_name=resource_group_name,
                 vault_name=vault_name,
                 vault=vault,
+                x_ms_authorization_auxiliary=x_ms_authorization_auxiliary,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("Vault", pipeline_response)
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
+            return LROPoller[_models.Vault].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}"
-    }
+        return LROPoller[_models.Vault](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure_mgmt_recoveryservices.egg-info/PKG-INFO` & `azure-mgmt-recoveryservices-3.0.0/azure_mgmt_recoveryservices.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-recoveryservices
-Version: 2.5.0
+Version: 3.0.0
 Summary: Microsoft Azure Recovery Services Client Library for Python
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
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Recovery Services Client Library.
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
 pip install azure-mgmt-recoveryservices
 pip install azure-identity
@@ -80,18 +80,32 @@
 ## Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
-![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-recoveryservices%2FREADME.png)
+# Release History
 
+## 3.0.0 (2024-04-22)
 
-# Release History
+### Features Added
+
+  - Model AzureMonitorAlertSettings has a new parameter alerts_for_all_failover_issues
+  - Model AzureMonitorAlertSettings has a new parameter alerts_for_all_replication_issues
+  - Model ClassicAlertSettings has a new parameter email_notifications_for_site_recovery
+  - Model SoftDeleteSettings has a new parameter enhanced_security_state
+  - Model VaultProperties has a new parameter bcdr_security_level
+  - Model VaultProperties has a new parameter resource_guard_operation_requests
+  - Operation VaultsOperations.begin_create_or_update has a new optional parameter x_ms_authorization_auxiliary
+  - Operation VaultsOperations.begin_update has a new optional parameter x_ms_authorization_auxiliary
+
+### Breaking Changes
+
+  - Renamed operation VaultsOperations.delete to VaultsOperations.begin_delete
 
 ## 2.5.0 (2023-09-05)
 
 ### Features Added
 
   - Model SecuritySettings has a new parameter multi_user_authorization
   - Model SecuritySettings has a new parameter soft_delete_settings
```

### Comparing `azure-mgmt-recoveryservices-2.5.0/azure_mgmt_recoveryservices.egg-info/SOURCES.txt` & `azure-mgmt-recoveryservices-3.0.0/azure_mgmt_recoveryservices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/setup.py` & `azure-mgmt-recoveryservices-3.0.0/setup.py`

 * *Files 6% similar despite different names*

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

### Comparing `azure-mgmt-recoveryservices-2.5.0/tests/disable_test_mgmt_recoveryservices.py` & `azure-mgmt-recoveryservices-3.0.0/tests/disable_test_mgmt_recoveryservices.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-recoveryservices-2.5.0/tests/recoveryservices_testcase.py` & `azure-mgmt-recoveryservices-3.0.0/tests/recoveryservices_testcase.py`

 * *Files identical despite different names*

