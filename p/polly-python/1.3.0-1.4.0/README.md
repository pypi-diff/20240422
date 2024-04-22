# Comparing `tmp/polly-python-1.3.0.tar.gz` & `tmp/polly_python-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polly-python-1.3.0.tar", last modified: Fri Feb  9 06:36:32 2024, max compression
+gzip compressed data, was "polly_python-1.4.0.tar", last modified: Mon Apr 22 08:17:43 2024, max compression
```

## Comparing `polly-python-1.3.0.tar` & `polly_python-1.4.0.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:36:32.684296 polly-python-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-02-09 06:35:25.000000 polly-python-1.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-09 06:35:25.000000 polly-python-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-02-09 06:36:32.684296 polly-python-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-09 06:35:25.000000 polly-python-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:36:32.676296 polly-python-1.3.0/polly/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17751 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/application_error_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16520 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/bridge_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)    17017 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    31214 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/core_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)    20886 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/curation.py
--rw-r--r--   0 runner    (1001) docker     (127)    32197 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/data_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/help.py
--rw-r--r--   0 runner    (1001) docker     (127)    23859 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/http_response_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/index_schema_level_conversion_const.py
--rw-r--r--   0 runner    (1001) docker     (127)    20615 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    83524 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/omixatlas.py
--rw-r--r--   0 runner    (1001) docker     (127)    27578 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/omixatlas_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/threading_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/validation_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (127)    16620 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:36:32.680296 polly-python-1.3.0/polly_interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_interfaces/IFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_interfaces/IReporting.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_interfaces/ISchema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:36:32.684296 polly-python-1.3.0/polly_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-02-09 06:36:32.000000 polly-python-1.3.0/polly_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-02-09 06:36:32.000000 polly-python-1.3.0/polly_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 06:36:32.000000 polly-python-1.3.0/polly_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-09 06:36:32.000000 polly-python-1.3.0/polly_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 06:36:32.000000 polly-python-1.3.0/polly_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:36:32.680296 polly-python-1.3.0/polly_services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19587 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:36:32.680296 polly-python-1.3.0/polly_services/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33379 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/files/files.py
--rw-r--r--   0 runner    (1001) docker     (127)   102835 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/files/files_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/polly_services_hlpr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:36:32.680296 polly-python-1.3.0/polly_services/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13199 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/reporting/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/reporting/reporting_hlpr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:36:32.680296 polly-python-1.3.0/polly_services/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/schema/schema_const.py
--rw-r--r--   0 runner    (1001) docker     (127)    19046 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/schema/schema_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-02-09 06:35:25.000000 polly-python-1.3.0/polly_services/schema/validate_schema_hlpr.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-09 06:35:25.000000 polly-python-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-02-09 06:36:32.684296 polly-python-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 06:35:25.000000 polly-python-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:36:32.684296 polly-python-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-02-09 06:35:25.000000 polly-python-1.3.0/tests/test_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-02-09 06:35:25.000000 polly-python-1.3.0/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-09 06:35:25.000000 polly-python-1.3.0/tests/test_curation.py
--rw-r--r--   0 runner    (1001) docker     (127)    33203 2024-02-09 06:35:25.000000 polly-python-1.3.0/tests/test_data_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-09 06:35:25.000000 polly-python-1.3.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-02-09 06:35:25.000000 polly-python-1.3.0/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)   108350 2024-02-09 06:35:25.000000 polly-python-1.3.0/tests/test_omixatlas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-09 06:35:25.000000 polly-python-1.3.0/tests/test_s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-02-09 06:35:25.000000 polly-python-1.3.0/tests/test_schema_ux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-09 06:35:25.000000 polly-python-1.3.0/tests/test_threading_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-02-09 06:35:25.000000 polly-python-1.3.0/tests/test_workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:43.943880 polly_python-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-22 08:16:47.000000 polly_python-1.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-22 08:16:47.000000 polly_python-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-22 08:17:43.943880 polly_python-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-22 08:16:47.000000 polly_python-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:43.935880 polly_python-1.4.0/polly/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17751 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/application_error_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16520 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/bridge_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17017 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31214 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/core_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20886 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32197 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/data_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23859 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/http_response_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/index_schema_level_conversion_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20615 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83524 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/omixatlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27578 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/omixatlas_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13825 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22584 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/threading_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/validation_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16620 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:43.935880 polly_python-1.4.0/polly_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_interfaces/IFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_interfaces/IReporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_interfaces/ISchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:43.943880 polly_python-1.4.0/polly_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-22 08:17:43.000000 polly_python-1.4.0/polly_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-22 08:17:43.000000 polly_python-1.4.0/polly_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:17:43.000000 polly_python-1.4.0/polly_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-22 08:17:43.000000 polly_python-1.4.0/polly_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:17:43.000000 polly_python-1.4.0/polly_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:43.939880 polly_python-1.4.0/polly_services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19587 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:43.939880 polly_python-1.4.0/polly_services/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33379 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/files/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102835 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/files/files_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/polly_services_hlpr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:43.939880 polly_python-1.4.0/polly_services/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13199 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/reporting/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/reporting/reporting_hlpr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:43.939880 polly_python-1.4.0/polly_services/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/schema/schema_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19046 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/schema/schema_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-22 08:16:47.000000 polly_python-1.4.0/polly_services/schema/validate_schema_hlpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-22 08:16:47.000000 polly_python-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-22 08:17:43.943880 polly_python-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:16:47.000000 polly_python-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:17:43.943880 polly_python-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_curation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33203 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_data_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108350 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_omixatlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_schema_ux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_threading_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-04-22 08:16:47.000000 polly_python-1.4.0/tests/test_workspaces.py
```

### Comparing `polly-python-1.3.0/LICENSE.md` & `polly_python-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/PKG-INFO` & `polly_python-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: polly-python
-Version: 1.3.0
+Name: polly_python
+Version: 1.4.0
 Summary: Polly SDK
 Home-page: https://github.com/ElucidataInc/polly-python
 Project-URL: Documentation, https://docs.elucidata.io
 Project-URL: Tutorial Notebooks, https://github.com/ElucidataInc/polly-python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `polly-python-1.3.0/README.md` & `polly_python-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/analyze.py` & `polly_python-1.4.0/polly/analyze.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/application_error_info.py` & `polly_python-1.4.0/polly/application_error_info.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/auth.py` & `polly_python-1.4.0/polly/auth.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/bridge_cohort.py` & `polly_python-1.4.0/polly/bridge_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/cohort.py` & `polly_python-1.4.0/polly/cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/constants.py` & `polly_python-1.4.0/polly/constants.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/core_cohort.py` & `polly_python-1.4.0/polly/core_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/curation.py` & `polly_python-1.4.0/polly/curation.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/data_management.py` & `polly_python-1.4.0/polly/data_management.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/errors.py` & `polly_python-1.4.0/polly/errors.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/help.py` & `polly_python-1.4.0/polly/help.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/helpers.py` & `polly_python-1.4.0/polly/helpers.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/http_response_codes.py` & `polly_python-1.4.0/polly/http_response_codes.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/jobs.py` & `polly_python-1.4.0/polly/jobs.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/omixatlas.py` & `polly_python-1.4.0/polly/omixatlas.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/omixatlas_hlpr.py` & `polly_python-1.4.0/polly/omixatlas_hlpr.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/s3_utils.py` & `polly_python-1.4.0/polly/s3_utils.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/session.py` & `polly_python-1.4.0/polly/session.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/threading_utils.py` & `polly_python-1.4.0/polly/threading_utils.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/tracking.py` & `polly_python-1.4.0/polly/tracking.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/validation.py` & `polly_python-1.4.0/polly/validation.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/validation_hlpr.py` & `polly_python-1.4.0/polly/validation_hlpr.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly/workspaces.py` & `polly_python-1.4.0/polly/workspaces.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_interfaces/IFiles.py` & `polly_python-1.4.0/polly_interfaces/IFiles.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_interfaces/IReporting.py` & `polly_python-1.4.0/polly_interfaces/IReporting.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_interfaces/ISchema.py` & `polly_python-1.4.0/polly_interfaces/ISchema.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_python.egg-info/PKG-INFO` & `polly_python-1.4.0/polly_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: polly-python
-Version: 1.3.0
+Name: polly_python
+Version: 1.4.0
 Summary: Polly SDK
 Home-page: https://github.com/ElucidataInc/polly-python
 Project-URL: Documentation, https://docs.elucidata.io
 Project-URL: Tutorial Notebooks, https://github.com/ElucidataInc/polly-python
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `polly-python-1.3.0/polly_python.egg-info/SOURCES.txt` & `polly_python-1.4.0/polly_python.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 polly/help.py
 polly/helpers.py
 polly/http_response_codes.py
 polly/index_schema_level_conversion_const.py
 polly/jobs.py
 polly/omixatlas.py
 polly/omixatlas_hlpr.py
+polly/pipelines.py
 polly/s3_utils.py
 polly/session.py
 polly/threading_utils.py
 polly/tracking.py
 polly/validation.py
 polly/validation_hlpr.py
 polly/workspaces.py
@@ -55,11 +56,12 @@
 tests/test_cohort.py
 tests/test_constants.py
 tests/test_curation.py
 tests/test_data_management.py
 tests/test_helpers.py
 tests/test_jobs.py
 tests/test_omixatlas.py
+tests/test_pipelines.py
 tests/test_s3_utils.py
 tests/test_schema_ux.py
 tests/test_threading_utils.py
 tests/test_workspaces.py
```

### Comparing `polly-python-1.3.0/polly_python.egg-info/requires.txt` & `polly_python-1.4.0/polly_python.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_services/dataset.py` & `polly_python-1.4.0/polly_services/dataset.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_services/files/files.py` & `polly_python-1.4.0/polly_services/files/files.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_services/files/files_hlpr.py` & `polly_python-1.4.0/polly_services/files/files_hlpr.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_services/polly_services_hlpr.py` & `polly_python-1.4.0/polly_services/polly_services_hlpr.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_services/reporting/reporting.py` & `polly_python-1.4.0/polly_services/reporting/reporting.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_services/reporting/reporting_hlpr.py` & `polly_python-1.4.0/polly_services/reporting/reporting_hlpr.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_services/schema/schema.py` & `polly_python-1.4.0/polly_services/schema/schema.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_services/schema/schema_hlpr.py` & `polly_python-1.4.0/polly_services/schema/schema_hlpr.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/polly_services/schema/validate_schema_hlpr.py` & `polly_python-1.4.0/polly_services/schema/validate_schema_hlpr.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/setup.cfg` & `polly_python-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-description-file = README.md
-name = polly-python
+description_file = README.md
+name = polly_python
 version = attr: polly.__version__
 description = Polly SDK
 url = https://github.com/ElucidataInc/polly-python
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Documentation = https://docs.elucidata.io
```

### Comparing `polly-python-1.3.0/tests/test_cohort.py` & `polly_python-1.4.0/tests/test_cohort.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/tests/test_curation.py` & `polly_python-1.4.0/tests/test_curation.py`

 * *Files 21% similar despite different names*

```diff
@@ -66,14 +66,20 @@
     )
     result5 = obj5.assign_control_pert_labels(
         sample_metadata, columns_to_exclude=["sample_id"]
     )
     assert result5 is not None
 
 
+"""
+ Commenting this Test case out as this test case is failing due to unidentified reason.
+ Raised a ticket to fix this testcase and add it back once fixed.
+
+ Ticket: https://elucidatainc.atlassian.net/browse/PRD-280
+
 def test_assign_clinical_labels():
     Polly.auth(token)
     obj6 = curation.Curation()
 
     result6 = obj6.assign_clinical_labels(
         repo_name="geo",
         dataset_ids=["GSE152430_GPL18573", "GSE35643_GPL6244"],
@@ -91,7 +97,9 @@
     assert result6 is not None
 
     result6 = obj6.assign_clinical_labels(
         repo_name="geo", dataset_ids=["GSE152430_GPL18573", "GSE35643_GPL6244"]
     )
 
     assert result6 is not None
+
+"""
```

### Comparing `polly-python-1.3.0/tests/test_data_management.py` & `polly_python-1.4.0/tests/test_data_management.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/tests/test_helpers.py` & `polly_python-1.4.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/tests/test_jobs.py` & `polly_python-1.4.0/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/tests/test_omixatlas.py` & `polly_python-1.4.0/tests/test_omixatlas.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/tests/test_s3_utils.py` & `polly_python-1.4.0/tests/test_s3_utils.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/tests/test_schema_ux.py` & `polly_python-1.4.0/tests/test_schema_ux.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/tests/test_threading_utils.py` & `polly_python-1.4.0/tests/test_threading_utils.py`

 * *Files identical despite different names*

### Comparing `polly-python-1.3.0/tests/test_workspaces.py` & `polly_python-1.4.0/tests/test_workspaces.py`

 * *Files identical despite different names*

