# Comparing `tmp/capycli-2.3.0.tar.gz` & `tmp/capycli-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capycli-2.3.0.tar", max compression
+gzip compressed data, was "capycli-2.4.0.tar", max compression
```

## Comparing `capycli-2.3.0.tar` & `capycli-2.4.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     6267 2023-05-17 09:09:21.101912 capycli-2.3.0/capycli/__init__.py
--rw-r--r--   0        0        0      445 2023-05-17 09:09:21.102694 capycli-2.3.0/capycli/__main__.py
--rw-r--r--   0        0        0      376 2023-05-17 09:09:21.103422 capycli-2.3.0/capycli/bom/__init__.py
--rw-r--r--   0        0        0     7179 2024-01-28 14:53:16.289861 capycli-2.3.0/capycli/bom/bom_convert.py
--rw-r--r--   0        0        0     8410 2024-01-28 15:04:23.907189 capycli-2.3.0/capycli/bom/check_bom.py
--rw-r--r--   0        0        0     8986 2024-01-28 15:05:06.505097 capycli-2.3.0/capycli/bom/check_bom_item_status.py
--rw-r--r--   0        0        0    11158 2024-01-28 14:53:16.309388 capycli-2.3.0/capycli/bom/check_granularity.py
--rw-r--r--   0        0        0    30972 2024-01-28 15:05:23.289811 capycli-2.3.0/capycli/bom/create_components.py
--rw-r--r--   0        0        0     2337 2024-01-28 14:53:16.324753 capycli-2.3.0/capycli/bom/csv.py
--rw-r--r--   0        0        0    10969 2024-01-28 14:53:16.329827 capycli-2.3.0/capycli/bom/diff_bom.py
--rw-r--r--   0        0        0     8927 2024-01-28 14:53:16.329827 capycli-2.3.0/capycli/bom/download_sources.py
--rw-r--r--   0        0        0    13074 2024-01-28 14:53:16.339751 capycli-2.3.0/capycli/bom/filter_bom.py
--rw-r--r--   0        0        0    29044 2024-02-20 21:21:58.815954 capycli-2.3.0/capycli/bom/findsources.py
--rw-r--r--   0        0        0     4931 2024-01-28 14:53:16.354988 capycli-2.3.0/capycli/bom/handle_bom.py
--rw-r--r--   0        0        0     2423 2024-01-28 14:53:16.359544 capycli-2.3.0/capycli/bom/html.py
--rw-r--r--   0        0        0    12485 2024-01-28 14:53:16.359544 capycli-2.3.0/capycli/bom/legacy.py
--rw-r--r--   0        0        0     5878 2023-05-17 09:09:21.119771 capycli-2.3.0/capycli/bom/legacy_cx.py
--rw-r--r--   0        0        0    46924 2024-01-28 14:53:16.370105 capycli-2.3.0/capycli/bom/map_bom.py
--rw-r--r--   0        0        0     6219 2024-01-28 14:53:16.379638 capycli-2.3.0/capycli/bom/merge_bom.py
--rw-r--r--   0        0        0     2915 2024-01-28 14:53:16.379638 capycli-2.3.0/capycli/bom/plaintext.py
--rw-r--r--   0        0        0     3017 2024-01-28 14:53:16.389753 capycli-2.3.0/capycli/bom/show_bom.py
--rw-r--r--   0        0        0      350 2023-05-17 09:09:21.122947 capycli-2.3.0/capycli/common/__init__.py
--rw-r--r--   0        0        0    24813 2024-01-28 14:53:16.389753 capycli-2.3.0/capycli/common/capycli_bom_support.py
--rw-r--r--   0        0        0     6025 2024-01-28 14:53:16.403123 capycli-2.3.0/capycli/common/comparable_version.py
--rw-r--r--   0        0        0     9025 2024-01-28 14:53:16.409692 capycli-2.3.0/capycli/common/component_cache.py
--rw-r--r--   0        0        0     2097 2023-05-17 09:09:21.126220 capycli-2.3.0/capycli/common/dependencies_base.py
--rw-r--r--   0        0        0      741 2024-01-28 14:53:16.409692 capycli-2.3.0/capycli/common/file_support.py
--rw-r--r--   0        0        0     4063 2024-01-28 14:53:16.419864 capycli-2.3.0/capycli/common/html_support.py
--rw-r--r--   0        0        0     1192 2024-01-28 14:53:16.419864 capycli-2.3.0/capycli/common/json_support.py
--rw-r--r--   0        0        0     4266 2024-01-28 14:53:16.429366 capycli-2.3.0/capycli/common/map_result.py
--rw-r--r--   0        0        0     1732 2024-01-28 14:53:16.439635 capycli-2.3.0/capycli/common/print.py
--rw-r--r--   0        0        0     7613 2024-01-28 14:53:16.439635 capycli-2.3.0/capycli/common/purl_service.py
--rw-r--r--   0        0        0     3419 2024-01-28 21:52:10.032716 capycli-2.3.0/capycli/common/purl_store.py
--rw-r--r--   0        0        0     3310 2024-01-28 14:53:16.453230 capycli-2.3.0/capycli/common/purl_utils.py
--rw-r--r--   0        0        0     7012 2024-01-28 15:06:20.190107 capycli-2.3.0/capycli/common/script_base.py
--rw-r--r--   0        0        0     2971 2024-01-28 14:53:16.470534 capycli-2.3.0/capycli/common/script_support.py
--rw-r--r--   0        0        0      329 2023-05-17 09:09:21.130298 capycli-2.3.0/capycli/data/__init__.py
--rw-r--r--   0        0        0   278377 2024-04-02 20:00:29.579607 capycli-2.3.0/capycli/data/granularity_list.csv
--rw-r--r--   0        0        0      344 2023-05-17 09:09:21.130298 capycli-2.3.0/capycli/dependencies/__init__.py
--rw-r--r--   0        0        0     2752 2024-01-28 14:53:16.470534 capycli-2.3.0/capycli/dependencies/handle_dependencies.py
--rw-r--r--   0        0        0    12549 2024-01-28 17:43:25.157496 capycli-2.3.0/capycli/dependencies/javascript.py
--rw-r--r--   0        0        0    13907 2024-03-08 13:04:38.749772 capycli-2.3.0/capycli/dependencies/maven_list.py
--rw-r--r--   0        0        0     5385 2024-01-28 14:53:16.489438 capycli-2.3.0/capycli/dependencies/maven_pom.py
--rw-r--r--   0        0        0     7085 2024-01-28 14:53:16.503455 capycli-2.3.0/capycli/dependencies/nuget.py
--rw-r--r--   0        0        0    19145 2024-01-28 14:53:16.509561 capycli-2.3.0/capycli/dependencies/python.py
--rw-r--r--   0        0        0      363 2023-05-17 09:09:21.133323 capycli-2.3.0/capycli/main/__init__.py
--rw-r--r--   0        0        0     5904 2024-01-28 14:53:16.529337 capycli-2.3.0/capycli/main/application.py
--rw-r--r--   0        0        0     4061 2024-01-28 14:53:16.529337 capycli-2.3.0/capycli/main/argument_parser.py
--rw-r--r--   0        0        0      881 2024-01-28 14:53:16.539568 capycli-2.3.0/capycli/main/cli.py
--rw-r--r--   0        0        0      441 2023-05-17 09:09:21.135549 capycli-2.3.0/capycli/main/exceptions.py
--rw-r--r--   0        0        0    15371 2024-04-05 15:03:15.504828 capycli-2.3.0/capycli/main/options.py
--rw-r--r--   0        0        0     1653 2024-04-05 15:03:15.504828 capycli-2.3.0/capycli/main/result_codes.py
--rw-r--r--   0        0        0     1572 2024-01-28 14:53:16.553253 capycli-2.3.0/capycli/mapping/handle_mapping.py
--rw-r--r--   0        0        0     7200 2024-01-28 14:53:16.553253 capycli-2.3.0/capycli/mapping/mapping_to_html.py
--rw-r--r--   0        0        0     8347 2024-01-28 14:53:16.564831 capycli-2.3.0/capycli/mapping/mapping_to_xlsx.py
--rw-r--r--   0        0        0     1643 2024-01-28 14:53:16.570018 capycli-2.3.0/capycli/moverview/handle_moverview.py
--rw-r--r--   0        0        0     4840 2024-01-28 14:53:16.570018 capycli-2.3.0/capycli/moverview/moverview_to_html.py
--rw-r--r--   0        0        0     7224 2024-01-28 14:53:16.579565 capycli-2.3.0/capycli/moverview/moverview_to_xlsx.py
--rw-r--r--   0        0        0      330 2023-05-17 09:09:21.138795 capycli-2.3.0/capycli/project/__init__.py
--rw-r--r--   0        0        0    13931 2024-04-05 15:03:15.504828 capycli-2.3.0/capycli/project/check_prerequisites.py
--rw-r--r--   0        0        0     9756 2024-01-28 15:06:45.340845 capycli-2.3.0/capycli/project/create_bom.py
--rw-r--r--   0        0        0    16458 2024-04-05 15:03:15.504828 capycli-2.3.0/capycli/project/create_project.py
--rw-r--r--   0        0        0    23442 2024-04-05 14:37:40.708729 capycli-2.3.0/capycli/project/create_readme.py
--rw-r--r--   0        0        0     5605 2024-01-28 14:53:16.609443 capycli-2.3.0/capycli/project/find_project.py
--rw-r--r--   0        0        0    10955 2024-04-05 15:03:15.504828 capycli-2.3.0/capycli/project/get_license_info.py
--rw-r--r--   0        0        0     4454 2024-01-28 14:53:16.629590 capycli-2.3.0/capycli/project/handle_project.py
--rw-r--r--   0        0        0     9000 2024-01-28 15:02:03.962221 capycli-2.3.0/capycli/project/show_ecc.py
--rw-r--r--   0        0        0     8329 2024-01-28 14:53:16.639627 capycli-2.3.0/capycli/project/show_licenses.py
--rw-r--r--   0        0        0    10069 2024-01-28 14:53:16.639627 capycli-2.3.0/capycli/project/show_project.py
--rw-r--r--   0        0        0     9709 2024-01-28 15:07:26.594053 capycli-2.3.0/capycli/project/show_vulnerabilities.py
--rw-r--r--   0        0        0     1218 2024-01-28 14:56:39.309682 capycli-2.3.0/License.md
-drwxr-xr-x   0        0        0        0 2023-05-17 09:11:25.459479 capycli-2.3.0/LICENSES/
--rw-r--r--   0        0        0     3107 2024-04-05 15:03:15.504828 capycli-2.3.0/pyproject.toml
--rw-r--r--   0        0        0    13026 2024-04-05 15:03:15.504828 capycli-2.3.0/Readme.md
--rw-r--r--   0        0        0    14532 1970-01-01 00:00:00.000000 capycli-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6267 2023-05-17 09:09:21.101912 capycli-2.4.0/capycli/__init__.py
+-rw-r--r--   0        0        0      445 2023-05-17 09:09:21.102694 capycli-2.4.0/capycli/__main__.py
+-rw-r--r--   0        0        0      376 2023-05-17 09:09:21.103422 capycli-2.4.0/capycli/bom/__init__.py
+-rw-r--r--   0        0        0     7179 2024-01-28 14:53:16.289861 capycli-2.4.0/capycli/bom/bom_convert.py
+-rw-r--r--   0        0        0     8410 2024-01-28 15:04:23.907189 capycli-2.4.0/capycli/bom/check_bom.py
+-rw-r--r--   0        0        0     8986 2024-01-28 15:05:06.505097 capycli-2.4.0/capycli/bom/check_bom_item_status.py
+-rw-r--r--   0        0        0    11158 2024-01-28 14:53:16.309388 capycli-2.4.0/capycli/bom/check_granularity.py
+-rw-r--r--   0        0        0    30972 2024-01-28 15:05:23.289811 capycli-2.4.0/capycli/bom/create_components.py
+-rw-r--r--   0        0        0     2337 2024-01-28 14:53:16.324753 capycli-2.4.0/capycli/bom/csv.py
+-rw-r--r--   0        0        0    10969 2024-01-28 14:53:16.329827 capycli-2.4.0/capycli/bom/diff_bom.py
+-rw-r--r--   0        0        0     8927 2024-01-28 14:53:16.329827 capycli-2.4.0/capycli/bom/download_sources.py
+-rw-r--r--   0        0        0    13074 2024-01-28 14:53:16.339751 capycli-2.4.0/capycli/bom/filter_bom.py
+-rw-r--r--   0        0        0    29044 2024-02-20 21:21:58.815954 capycli-2.4.0/capycli/bom/findsources.py
+-rw-r--r--   0        0        0     4931 2024-01-28 14:53:16.354988 capycli-2.4.0/capycli/bom/handle_bom.py
+-rw-r--r--   0        0        0     2423 2024-01-28 14:53:16.359544 capycli-2.4.0/capycli/bom/html.py
+-rw-r--r--   0        0        0    12485 2024-04-20 10:10:45.715247 capycli-2.4.0/capycli/bom/legacy.py
+-rw-r--r--   0        0        0     5878 2023-05-17 09:09:21.119771 capycli-2.4.0/capycli/bom/legacy_cx.py
+-rw-r--r--   0        0        0    46924 2024-01-28 14:53:16.370105 capycli-2.4.0/capycli/bom/map_bom.py
+-rw-r--r--   0        0        0     6219 2024-01-28 14:53:16.379638 capycli-2.4.0/capycli/bom/merge_bom.py
+-rw-r--r--   0        0        0     2915 2024-01-28 14:53:16.379638 capycli-2.4.0/capycli/bom/plaintext.py
+-rw-r--r--   0        0        0     3017 2024-01-28 14:53:16.389753 capycli-2.4.0/capycli/bom/show_bom.py
+-rw-r--r--   0        0        0      350 2023-05-17 09:09:21.122947 capycli-2.4.0/capycli/common/__init__.py
+-rw-r--r--   0        0        0    24813 2024-01-28 14:53:16.389753 capycli-2.4.0/capycli/common/capycli_bom_support.py
+-rw-r--r--   0        0        0     6025 2024-01-28 14:53:16.403123 capycli-2.4.0/capycli/common/comparable_version.py
+-rw-r--r--   0        0        0     9025 2024-01-28 14:53:16.409692 capycli-2.4.0/capycli/common/component_cache.py
+-rw-r--r--   0        0        0     2097 2023-05-17 09:09:21.126220 capycli-2.4.0/capycli/common/dependencies_base.py
+-rw-r--r--   0        0        0      741 2024-01-28 14:53:16.409692 capycli-2.4.0/capycli/common/file_support.py
+-rw-r--r--   0        0        0     4063 2024-01-28 14:53:16.419864 capycli-2.4.0/capycli/common/html_support.py
+-rw-r--r--   0        0        0     1192 2024-01-28 14:53:16.419864 capycli-2.4.0/capycli/common/json_support.py
+-rw-r--r--   0        0        0     4266 2024-01-28 14:53:16.429366 capycli-2.4.0/capycli/common/map_result.py
+-rw-r--r--   0        0        0     1732 2024-01-28 14:53:16.439635 capycli-2.4.0/capycli/common/print.py
+-rw-r--r--   0        0        0     7613 2024-01-28 14:53:16.439635 capycli-2.4.0/capycli/common/purl_service.py
+-rw-r--r--   0        0        0     3419 2024-01-28 21:52:10.032716 capycli-2.4.0/capycli/common/purl_store.py
+-rw-r--r--   0        0        0     3310 2024-01-28 14:53:16.453230 capycli-2.4.0/capycli/common/purl_utils.py
+-rw-r--r--   0        0        0     7012 2024-01-28 15:06:20.190107 capycli-2.4.0/capycli/common/script_base.py
+-rw-r--r--   0        0        0     2971 2024-01-28 14:53:16.470534 capycli-2.4.0/capycli/common/script_support.py
+-rw-r--r--   0        0        0      329 2023-05-17 09:09:21.130298 capycli-2.4.0/capycli/data/__init__.py
+-rw-r--r--   0        0        0   278377 2024-04-02 20:00:29.579607 capycli-2.4.0/capycli/data/granularity_list.csv
+-rw-r--r--   0        0        0      344 2023-05-17 09:09:21.130298 capycli-2.4.0/capycli/dependencies/__init__.py
+-rw-r--r--   0        0        0     2752 2024-01-28 14:53:16.470534 capycli-2.4.0/capycli/dependencies/handle_dependencies.py
+-rw-r--r--   0        0        0    12549 2024-01-28 17:43:25.157496 capycli-2.4.0/capycli/dependencies/javascript.py
+-rw-r--r--   0        0        0    13907 2024-03-08 13:04:38.749772 capycli-2.4.0/capycli/dependencies/maven_list.py
+-rw-r--r--   0        0        0     5385 2024-01-28 14:53:16.489438 capycli-2.4.0/capycli/dependencies/maven_pom.py
+-rw-r--r--   0        0        0     7085 2024-01-28 14:53:16.503455 capycli-2.4.0/capycli/dependencies/nuget.py
+-rw-r--r--   0        0        0    19145 2024-01-28 14:53:16.509561 capycli-2.4.0/capycli/dependencies/python.py
+-rw-r--r--   0        0        0      363 2023-05-17 09:09:21.133323 capycli-2.4.0/capycli/main/__init__.py
+-rw-r--r--   0        0        0     5904 2024-01-28 14:53:16.529337 capycli-2.4.0/capycli/main/application.py
+-rw-r--r--   0        0        0     4061 2024-01-28 14:53:16.529337 capycli-2.4.0/capycli/main/argument_parser.py
+-rw-r--r--   0        0        0      881 2024-01-28 14:53:16.539568 capycli-2.4.0/capycli/main/cli.py
+-rw-r--r--   0        0        0      441 2023-05-17 09:09:21.135549 capycli-2.4.0/capycli/main/exceptions.py
+-rw-r--r--   0        0        0    15371 2024-04-05 15:03:15.504828 capycli-2.4.0/capycli/main/options.py
+-rw-r--r--   0        0        0     1653 2024-04-05 15:03:15.504828 capycli-2.4.0/capycli/main/result_codes.py
+-rw-r--r--   0        0        0     1572 2024-01-28 14:53:16.553253 capycli-2.4.0/capycli/mapping/handle_mapping.py
+-rw-r--r--   0        0        0     7200 2024-01-28 14:53:16.553253 capycli-2.4.0/capycli/mapping/mapping_to_html.py
+-rw-r--r--   0        0        0     8347 2024-01-28 14:53:16.564831 capycli-2.4.0/capycli/mapping/mapping_to_xlsx.py
+-rw-r--r--   0        0        0     1643 2024-01-28 14:53:16.570018 capycli-2.4.0/capycli/moverview/handle_moverview.py
+-rw-r--r--   0        0        0     4840 2024-01-28 14:53:16.570018 capycli-2.4.0/capycli/moverview/moverview_to_html.py
+-rw-r--r--   0        0        0     7224 2024-01-28 14:53:16.579565 capycli-2.4.0/capycli/moverview/moverview_to_xlsx.py
+-rw-r--r--   0        0        0      330 2023-05-17 09:09:21.138795 capycli-2.4.0/capycli/project/__init__.py
+-rw-r--r--   0        0        0    14001 2024-04-22 05:42:34.188323 capycli-2.4.0/capycli/project/check_prerequisites.py
+-rw-r--r--   0        0        0     9756 2024-01-28 15:06:45.340845 capycli-2.4.0/capycli/project/create_bom.py
+-rw-r--r--   0        0        0    16466 2024-04-22 05:42:34.188323 capycli-2.4.0/capycli/project/create_project.py
+-rw-r--r--   0        0        0    23458 2024-04-22 05:42:34.188323 capycli-2.4.0/capycli/project/create_readme.py
+-rw-r--r--   0        0        0     5605 2024-01-28 14:53:16.609443 capycli-2.4.0/capycli/project/find_project.py
+-rw-r--r--   0        0        0    11011 2024-04-22 05:42:34.188323 capycli-2.4.0/capycli/project/get_license_info.py
+-rw-r--r--   0        0        0     4454 2024-01-28 14:53:16.629590 capycli-2.4.0/capycli/project/handle_project.py
+-rw-r--r--   0        0        0     9098 2024-04-22 05:42:34.188323 capycli-2.4.0/capycli/project/show_ecc.py
+-rw-r--r--   0        0        0     8351 2024-04-22 05:42:34.188323 capycli-2.4.0/capycli/project/show_licenses.py
+-rw-r--r--   0        0        0    10132 2024-04-22 05:42:34.188323 capycli-2.4.0/capycli/project/show_project.py
+-rw-r--r--   0        0        0    10138 2024-04-22 05:42:34.188323 capycli-2.4.0/capycli/project/show_vulnerabilities.py
+-rw-r--r--   0        0        0     1218 2024-01-28 14:56:39.309682 capycli-2.4.0/License.md
+drwxr-xr-x   0        0        0        0 2023-05-17 09:11:25.459479 capycli-2.4.0/LICENSES/
+-rw-r--r--   0        0        0     3107 2024-04-22 05:48:09.531443 capycli-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13026 2024-04-05 15:03:15.504828 capycli-2.4.0/Readme.md
+-rw-r--r--   0        0        0    14532 1970-01-01 00:00:00.000000 capycli-2.4.0/PKG-INFO
```

### Comparing `capycli-2.3.0/capycli/__init__.py` & `capycli-2.4.0/capycli/__init__.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/bom_convert.py` & `capycli-2.4.0/capycli/bom/bom_convert.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/check_bom.py` & `capycli-2.4.0/capycli/bom/check_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/check_bom_item_status.py` & `capycli-2.4.0/capycli/bom/check_bom_item_status.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/check_granularity.py` & `capycli-2.4.0/capycli/bom/check_granularity.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/create_components.py` & `capycli-2.4.0/capycli/bom/create_components.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/csv.py` & `capycli-2.4.0/capycli/bom/csv.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/diff_bom.py` & `capycli-2.4.0/capycli/bom/diff_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/download_sources.py` & `capycli-2.4.0/capycli/bom/download_sources.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/filter_bom.py` & `capycli-2.4.0/capycli/bom/filter_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/findsources.py` & `capycli-2.4.0/capycli/bom/findsources.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/handle_bom.py` & `capycli-2.4.0/capycli/bom/handle_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/html.py` & `capycli-2.4.0/capycli/bom/html.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/legacy.py` & `capycli-2.4.0/capycli/bom/legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,28 +143,28 @@
                 value=releaseMainlineState)
             cxcomp.properties.add(prop)
 
         sourceFileUrl = item.get("SourceFileUrl", "")
         if sourceFileUrl:
             ext_ref = ExternalReference(
                 reference_type=ExternalReferenceType.DISTRIBUTION,
-                comment=CaPyCliBom.SOURCE_URL_COMMENT,
+                comment=CaPyCliBom.SOURCE_FILE_COMMENT,
                 url=XsUri(sourceFileUrl))
             hash = item.get("SourceFileHash", "")
             if hash:
                 ext_ref.hashes.add(HashType(
                     algorithm=HashAlgorithm.SHA_1,
                     hash_value=hash))
             cxcomp.external_references.add(ext_ref)
         else:
             sourceUrl = item.get("SourceUrl", "")
             if sourceUrl:
                 ext_ref = ExternalReference(
                     reference_type=ExternalReferenceType.DISTRIBUTION,
-                    comment=CaPyCliBom.SOURCE_FILE_COMMENT,
+                    comment=CaPyCliBom.SOURCE_URL_COMMENT,
                     url=XsUri(sourceUrl))
                 hash = item.get("SourceFileHash", "")
                 if hash:
                     ext_ref.hashes.add(HashType(
                         algorithm=HashAlgorithm.SHA_1,
                         hash_value=hash))
                 cxcomp.external_references.add(ext_ref)
```

### Comparing `capycli-2.3.0/capycli/bom/legacy_cx.py` & `capycli-2.4.0/capycli/bom/legacy_cx.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/map_bom.py` & `capycli-2.4.0/capycli/bom/map_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/merge_bom.py` & `capycli-2.4.0/capycli/bom/merge_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/plaintext.py` & `capycli-2.4.0/capycli/bom/plaintext.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/bom/show_bom.py` & `capycli-2.4.0/capycli/bom/show_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/capycli_bom_support.py` & `capycli-2.4.0/capycli/common/capycli_bom_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/comparable_version.py` & `capycli-2.4.0/capycli/common/comparable_version.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/component_cache.py` & `capycli-2.4.0/capycli/common/component_cache.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/dependencies_base.py` & `capycli-2.4.0/capycli/common/dependencies_base.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/file_support.py` & `capycli-2.4.0/capycli/common/file_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/html_support.py` & `capycli-2.4.0/capycli/common/html_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/json_support.py` & `capycli-2.4.0/capycli/common/json_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/map_result.py` & `capycli-2.4.0/capycli/common/map_result.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/print.py` & `capycli-2.4.0/capycli/common/print.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/purl_service.py` & `capycli-2.4.0/capycli/common/purl_service.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/purl_store.py` & `capycli-2.4.0/capycli/common/purl_store.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/purl_utils.py` & `capycli-2.4.0/capycli/common/purl_utils.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/script_base.py` & `capycli-2.4.0/capycli/common/script_base.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/common/script_support.py` & `capycli-2.4.0/capycli/common/script_support.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/data/granularity_list.csv` & `capycli-2.4.0/capycli/data/granularity_list.csv`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/dependencies/handle_dependencies.py` & `capycli-2.4.0/capycli/dependencies/handle_dependencies.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/dependencies/javascript.py` & `capycli-2.4.0/capycli/dependencies/javascript.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/dependencies/maven_list.py` & `capycli-2.4.0/capycli/dependencies/maven_list.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/dependencies/maven_pom.py` & `capycli-2.4.0/capycli/dependencies/maven_pom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/dependencies/nuget.py` & `capycli-2.4.0/capycli/dependencies/nuget.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/dependencies/python.py` & `capycli-2.4.0/capycli/dependencies/python.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/main/application.py` & `capycli-2.4.0/capycli/main/application.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/main/argument_parser.py` & `capycli-2.4.0/capycli/main/argument_parser.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/main/cli.py` & `capycli-2.4.0/capycli/main/cli.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/main/options.py` & `capycli-2.4.0/capycli/main/options.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/main/result_codes.py` & `capycli-2.4.0/capycli/main/result_codes.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/mapping/handle_mapping.py` & `capycli-2.4.0/capycli/mapping/handle_mapping.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/mapping/mapping_to_html.py` & `capycli-2.4.0/capycli/mapping/mapping_to_html.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/mapping/mapping_to_xlsx.py` & `capycli-2.4.0/capycli/mapping/mapping_to_xlsx.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/moverview/handle_moverview.py` & `capycli-2.4.0/capycli/moverview/handle_moverview.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/moverview/moverview_to_html.py` & `capycli-2.4.0/capycli/moverview/moverview_to_html.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/moverview/moverview_to_xlsx.py` & `capycli-2.4.0/capycli/moverview/moverview_to_xlsx.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/project/check_prerequisites.py` & `capycli-2.4.0/capycli/project/check_prerequisites.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,33 +24,33 @@
 
 
 class CheckPrerequisites(capycli.common.script_base.ScriptBase):
     """Checks whether all prerequisites for a successfull software clearing are fulfilled."""
 
     def get_clearing_state(self, project: Dict[str, Any], href: str) -> str:
         """Returns the clearing state of the given component/release"""
-        rel = project["linkedReleases"]
+        rel = project.get("linkedReleases", [])
         for key in rel:
             if key["release"] == href:
-                return key["mainlineState"]
+                return key.get("mainlineState", "")
 
         return ""
 
     def get_source_code(self, release: Dict[str, Any]) -> List[Dict[str, Any]]:
         """Return list of attachment infos for all source code attachments"""
         if "_embedded" not in release:
             return []
 
         if "sw360:attachments" not in release["_embedded"]:
             return []
 
         att = [
             entry
             for entry in release["_embedded"]["sw360:attachments"]
-            if entry["attachmentType"] in ("SOURCE", "SOURCE_SELF")
+            if entry.get("attachmentType", "") in ("SOURCE", "SOURCE_SELF")
         ]
         return att
 
     def get_component_management_id(self, release: Dict[str, Any]) -> Dict[Any, Any]:
         """Retries the first component management id"""
         if "externalIds" not in release:
             return {}
@@ -117,15 +117,15 @@
         print_text("  Project name: " + project["name"] + ", " + project["version"])
         print_text("  Clearing state: " + project.get("clearingState", "UNKNOWN"))
 
         if not project.get("projectOwner", None):
             print_yellow("  No project owner specified!")
             has_errors = True
         else:
-            print_green("  Project owner: " + project["projectOwner"])
+            print_green("  Project owner: " + project.get("projectOwner", "UNKNOWN"))
 
         if not project.get("projectResponsible", None):
             print_yellow("  No project responsible specified!")
             has_errors = True
         else:
             print_green(
                 "  Project responsible: "
@@ -137,15 +137,15 @@
             print_green(
                 "  Security responsible(s): "
                 + self.list_to_string(project["securityResponsibles"]))
 
         if not project.get("tag", None):
             print_yellow("  No tag specified!")
         else:
-            print_green("  Tag: " + project["tag"])
+            print_green("  Tag: " + project.get("tag", "UNKNOWN"))
 
         if "sw360:projects" in project["_embedded"]:
             linked_projects = project["_embedded"]["sw360:projects"]
             if linked_projects:
                 print_text("\n  Linked projects: ")
                 for key in linked_projects:
                     print_text("    " + key["name"] + ", " + key["version"])
@@ -192,22 +192,22 @@
                         has_errors = True
                     else:
                         assert len(bom_item) == 1
                         bom_sha1 = CycloneDxSupport.get_source_file_hash(bom_item[0])
 
                 source = self.get_source_code(release)
                 for source_info in source:
-                    source_name = source_info["filename"]
+                    source_name = source_info.get("filename", "")
                     if "-SOURCES.JAR" in source_name.upper():
                         print_yellow(
                             "      Source " +
                             source_name +
                             " seems to be from Maven!")
                     if bom_sha1:
-                        if bom_sha1 != source_info["sha1"]:
+                        if bom_sha1 != source_info.get("sha1", ""):
                             print_red(
                                 "      SHA1 for source " +
                                 source_name +
                                 " does not match!")
                             self.check_checkStatus(source_info)
                         else:
                             print_green(
```

### Comparing `capycli-2.3.0/capycli/project/create_bom.py` & `capycli-2.4.0/capycli/project/create_bom.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/project/create_project.py` & `capycli-2.4.0/capycli/project/create_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         for attachment in attachments:
             if 'file' not in attachment:
                 print_yellow("  No file specified to upload")
             else:
                 filename = os.path.basename(attachment['file'])
                 upload = True
                 for project_attachment in project_attachments:
-                    if project_attachment['filename'] == filename:
+                    if project_attachment.get('filename', '') == filename:
                         print_yellow(
                             "  Attachment file " + filename +
                             " already exists! Please check manually")
                         upload = False
                         continue
 
                 if not os.path.isfile(attachment['file']):
```

### Comparing `capycli-2.3.0/capycli/project/create_readme.py` & `capycli-2.4.0/capycli/project/create_readme.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,16 +449,16 @@
             config = json.loads(text)
         return config
 
     def read_cli_files(self, config: Dict[str, Any]) -> List[CliFile]:
         """Reads all CLI files"""
         cli_files: List[CliFile] = []
         unique_components = []
-        for file in config["Components"]:
-            component_name = file["ComponentName"]
+        for file in config.get("Components", []):
+            component_name = file.get("ComponentName", "")
             if component_name not in unique_components:
                 unique_components.append(component_name)
             else:
                 print_yellow("        Multiple CLI files exist for the same component - manual review needed!")
             filename = file["CliFile"]
             if os.path.isfile(filename):
                 print_text("    Reading", component_name, "...")
```

### Comparing `capycli-2.3.0/capycli/project/find_project.py` & `capycli-2.4.0/capycli/project/find_project.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/project/get_license_info.py` & `capycli-2.4.0/capycli/project/get_license_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         attachment_infos = release["_embedded"]["sw360:attachments"]
         for key in attachment_infos:
             att_href = key["_links"]["self"]["href"]
             attachment = self.client.get_attachment_by_url(att_href)
             if not attachment:
                 continue
-            if not attachment["attachmentType"] == "COMPONENT_LICENSE_INFO_XML":
+            if not attachment.get("attachmentType", "") == "COMPONENT_LICENSE_INFO_XML":
                 continue
 
             release_id = self.client.get_id_from_href(release["_links"]["self"]["href"])
             attachment_id = self.client.get_id_from_href(att_href)
 
             fileinfo = {}
             filename = os.path.join(folder, attachment.get("filename", ""))
@@ -147,20 +147,20 @@
 
                 count = 0
                 warning_shown = False
                 cli_files = self.get_cli_files_for_release(release, target_folder, no_overwrite)
                 for cli_file in cli_files:
                     comp = {}
                     comp["ComponentName"] = component_name
-                    comp["CliFile"] = cli_file["filename"]
-                    comp["CreatedBy"] = cli_file["createdBy"]
-                    comp["CreatedOn"] = cli_file["createdOn"]
-                    comp["CheckedBy"] = cli_file["checkedBy"]
-                    comp["CheckedTeam"] = cli_file["checkedTeam"]
-                    comp["CheckStatus"] = cli_file["checkStatus"]
+                    comp["CliFile"] = cli_file.get("filename", "")
+                    comp["CreatedBy"] = cli_file.get("createdBy", "")
+                    comp["CreatedOn"] = cli_file.get("createdOn", "")
+                    comp["CheckedBy"] = cli_file.get("checkedBy", "")
+                    comp["CheckedTeam"] = cli_file.get("checkedTeam", "")
+                    comp["CheckStatus"] = cli_file.get("checkStatus", "")
 
                     count += 1
                     if count > 1:
                         if not use_all_files:
                             continue
 
                         if not warning_shown:
```

### Comparing `capycli-2.3.0/capycli/project/handle_project.py` & `capycli-2.4.0/capycli/project/handle_project.py`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/capycli/project/show_ecc.py` & `capycli-2.4.0/capycli/project/show_ecc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ﻿# -------------------------------------------------------------------------------
-# Copyright (c) 2022-2023 Siemens
+# Copyright (c) 2022-2024 Siemens
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 import logging
@@ -25,17 +25,17 @@
 
     def show_project_status(self, result: Dict[str, Any]) -> None:
         if not result:
             return
 
         print_text("  Project name: " + result["Name"] + ", " + result["Version"])
         if "ProjectResponsible" in result:
-            print("  Project responsible: " + result["ProjectResponsible"])
-        print_text("  Project owner: " + result["ProjectOwner"])
-        print_text("  Clearing state: " + result["ClearingState"])
+            print("  Project responsible: " + result.get("ProjectResponsible", "Unknown"))
+        print_text("  Project owner: " + result.get("ProjectOwner", "Unknown"))
+        print_text("  Clearing state: " + result.get("ClearingState", "Unknown"))
 
         if len(result["Projects"]) > 0:
             print("\n  Linked projects: ")
             for project in result["Projects"]:
                 print_text("    " + project["Name"] + ", " + project["Version"])
         else:
             print_text("\n    No linked projects")
@@ -88,18 +88,18 @@
 
         if not self.project:
             print_red("  ERROR: unable to read project data!")
             sys.exit(ResultCode.RESULT_ERROR_ACCESSING_SW360)
 
         result["Name"] = self.project["name"]
         result["Version"] = self.project["version"]
-        result["ProjectOwner"] = self.project["projectOwner"]
-        result["ProjectResponsible"] = self.project["projectResponsible"]
-        result["SecurityResponsibles"] = self.project["securityResponsibles"]
-        result["BusinessUnit"] = self.project["businessUnit"]
+        result["ProjectOwner"] = self.project.get("projectOwner", "Unknown")
+        result["ProjectResponsible"] = self.project.get("projectResponsible", "Unknown")
+        result["SecurityResponsibles"] = self.project.get("securityResponsibles", [])
+        result["BusinessUnit"] = self.project.get("businessUnit", "Unknown")
         result["Tag"] = self.project["tag"]
         if "clearingState" in self.project:
             result["ClearingState"] = self.project["clearingState"]
         else:
             result["ClearingState"] = "OPEN"
         result["ProjectLink"] = (
             self.sw360_url + "group/guest/projects/-/project/detail/" + project_id
```

### Comparing `capycli-2.3.0/capycli/project/show_licenses.py` & `capycli-2.4.0/capycli/project/show_licenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ﻿# -------------------------------------------------------------------------------
-# Copyright (c) 2019-23 Siemens
+# Copyright (c) 2019-24 Siemens
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 import logging
@@ -138,16 +138,16 @@
             sys.exit(ResultCode.RESULT_ERROR_ACCESSING_SW360)
 
         if not project:
             print_red("Unable to read project!")
             return
 
         print_text("  Project name: " + project["name"] + ", " + project["version"])
-        print_text("  Project owner: " + project["projectOwner"])
-        print_text("  Clearing state: " + project["clearingState"])
+        print_text("  Project owner: " + project.get("projectOwner", "???"))
+        print_text("  Clearing state: " + project.get("clearingState", "???"))
         if self.nodelete:
             print_text("  Temp folder", tempfolder, "will not get deleted.")
 
         self.global_license_list = []
         if "sw360:releases" in project["_embedded"]:
             print_text("\nComponents: ")
             releases = project["_embedded"]["sw360:releases"]
```

### Comparing `capycli-2.3.0/capycli/project/show_project.py` & `capycli-2.4.0/capycli/project/show_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ﻿# -------------------------------------------------------------------------------
-# Copyright (c) 2019-23 Siemens
+# Copyright (c) 2019-24 Siemens
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 import logging
@@ -24,30 +24,30 @@
 class ShowProject(capycli.common.script_base.ScriptBase):
     """Show project details."""
     def get_clearing_state(self, proj: Optional[Dict[str, Any]], href: str) -> str:
         """Returns the clearing state of the given component/release"""
         if not proj:
             return ""
 
-        rel = proj["linkedReleases"]
+        rel = proj.get("linkedReleases", [])
         for key in rel:
-            if key["release"] == href:
-                return key["mainlineState"]
+            if key.get("release", "") == href:
+                return key.get("mainlineState", "???")
 
         return ""
 
     def show_project_status(self, result: Dict[str, Any]) -> None:
         if not result:
             return
 
         print_text("  Project name: " + result["Name"] + ", " + result["Version"])
         if "ProjectResponsible" in result:
             print_text("  Project responsible: " + result["ProjectResponsible"])
-        print_text("  Project owner: " + result["ProjectOwner"])
-        print_text("  Clearing state: " + result["ClearingState"])
+        print_text("  Project owner: " + result.get("ProjectOwner", "???"))
+        print_text("  Clearing state: " + result.get("ClearingState", "???"))
 
         if len(result["Projects"]) > 0:
             print_text("\n  Linked projects: ")
             for project in result["Projects"]:
                 print_text("    " + project["Name"] + ", " + project["Version"])
         else:
             print_text("\n    No linked projects")
@@ -134,16 +134,16 @@
                 try:
                     release_details = self.client.get_release_by_url(href)
                     if not release_details:
                         print_red("  ERROR: unable to access project:")
                         sys.exit(ResultCode.RESULT_ERROR_ACCESSING_SW360)
 
                     # capycli.common.json_support.print_json(release_details)
-                    rel_item["ClearingState"] = release_details["clearingState"]
-                    rel_item["ReleaseMainlineState"] = release_details.get("mainlineState", "")
+                    rel_item["ClearingState"] = release_details.get("clearingState", "???")
+                    rel_item["ReleaseMainlineState"] = release_details.get("mainlineState", "???")
                     rel_item["SourceAvailable"] = "False"
                     if "externalIds" in release_details:
                         rel_item["ExternalIds"] = release_details["externalIds"]
                     if "_embedded" in release_details:
                         if "sw360:attachments" in release_details["_embedded"]:
                             att = release_details["_embedded"]["sw360:attachments"]
                             for key in att:
```

### Comparing `capycli-2.3.0/capycli/project/show_vulnerabilities.py` & `capycli-2.4.0/capycli/project/show_vulnerabilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -126,15 +126,21 @@
 
         # capycli.common.json_support.write_json_to_file(vuls, "vuls.json")
         if "_embedded" not in vuls:
             return report
 
         # 2022-07-01: SW360 changed "sw360:vulnerabilityDToes" to "sw360:vulnerabilityDTOes" - arrgghhh
         if "sw360:vulnerabilityDTOes" not in vuls["_embedded"]:
-            return report
+            if "sw360:vulnerabilityDTes" not in vuls["_embedded"]:
+                vuls["_embedded"]["sw360:vulnerabilityDTOes"] = vuls["_embedded"]["sw360:vulnerabilityDTes"]
+            elif "sw360:vulnerabilities" not in vuls["_embedded"]:
+                vuls["_embedded"]["sw360:vulnerabilityDTOes"] = vuls["_embedded"]["sw360:vulnerabilities"]
+
+            if "sw360:vulnerabilityDTOes" not in vuls["_embedded"]:
+                return report
 
         report["Vulnerabilities"] = vuls["_embedded"]["sw360:vulnerabilityDTOes"]
 
         print_text("\nVulnerabilities: ")
         if len(report["Vulnerabilities"]) == 0:
             print_green("  No security vulnerabilities known or feature not enabled\n")
```

### Comparing `capycli-2.3.0/License.md` & `capycli-2.4.0/License.md`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/pyproject.toml` & `capycli-2.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: (c) 2018-2024 Siemens
 # SPDX-License-Identifier: MIT
 
 [tool.poetry]
 name = "capycli"
-version = "2.3.0"
+version = "2.4.0"
 description = "CaPyCli - Clearing Automation Python Command Line Interface for SW360"
 authors = ["Thomas Graf <thomas.graf@siemens.com>"]
 license = "MIT"
 readme="Readme.md"
 repository = "https://github.com/sw360/capycli"
 homepage = "https://github.com/sw360/capycli"
 keywords = ["sw360", "cli, automation", "license", "compliance", "clearing"]
@@ -38,17 +38,17 @@
 colorama = "^0.4.3"
 requests = "^2.31.0" # fix CVE-2023-32681 
 semver = "3.0.2"
 packageurl-python = ">0.8, <1.0"
 pyjwt = "^1.7.1"
 openpyxl = "^3.0.3"
 requirements-parser = "0.5.0"
-sw360 = "^1.4.0"
+sw360 = "^1.5.0"
 wheel = "^0.38.4"
-cli-support = "2.0.0"
+cli-support = "2.0.1"
 chardet = "5.2.0"
 cyclonedx-python-lib = ">3.1.1"
 cyclonedx-bom = "^3.11.0"
 tomli = "^2.0.1"
 dateparser = "^1.1.8"
 urllib3 = "*"
 importlib-resources = "^5.12.0"
```

### Comparing `capycli-2.3.0/Readme.md` & `capycli-2.4.0/Readme.md`

 * *Files identical despite different names*

### Comparing `capycli-2.3.0/PKG-INFO` & `capycli-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capycli
-Version: 2.3.0
+Version: 2.4.0
 Summary: CaPyCli - Clearing Automation Python Command Line Interface for SW360
 Home-page: https://github.com/sw360/capycli
 License: MIT
 Keywords: sw360,cli, automation,license,compliance,clearing
 Author: Thomas Graf
 Author-email: thomas.graf@siemens.com
 Requires-Python: >=3.8,<4.0
@@ -17,27 +17,27 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: chardet (==5.2.0)
-Requires-Dist: cli-support (==2.0.0)
+Requires-Dist: cli-support (==2.0.1)
 Requires-Dist: colorama (>=0.4.3,<0.5.0)
 Requires-Dist: cyclonedx-bom (>=3.11.0,<4.0.0)
 Requires-Dist: cyclonedx-python-lib (>3.1.1)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: importlib-resources (>=5.12.0,<6.0.0)
 Requires-Dist: openpyxl (>=3.0.3,<4.0.0)
 Requires-Dist: packageurl-python (>0.8,<1.0)
 Requires-Dist: pyjwt (>=1.7.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requirements-parser (==0.5.0)
 Requires-Dist: semver (==3.0.2)
-Requires-Dist: sw360 (>=1.4.0,<2.0.0)
+Requires-Dist: sw360 (>=1.5.0,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: urllib3
 Requires-Dist: wheel (>=0.38.4,<0.39.0)
 Project-URL: Repository, https://github.com/sw360/capycli
 Project-URL: issues, https://github.com/sw360/capycli/issues
 Description-Content-Type: text/markdown
```

