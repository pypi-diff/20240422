# Comparing `tmp/UEVaultManager-1.9.4.tar.gz` & `tmp/UEVaultManager-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.9.4.tar", last modified: Wed Sep  6 07:13:55 2023, max compression
+gzip compressed data, was "UEVaultManager-1.9.5.tar", last modified: Wed Sep  6 07:46:14 2023, max compression
```

## Comparing `UEVaultManager-1.9.4.tar` & `UEVaultManager-1.9.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.451888 UEVaultManager-1.9.4/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.9.4/LICENSE
--rw-rw-rw-   0        0        0     6539 2023-09-06 07:13:55.451888 UEVaultManager-1.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     5693 2023-06-26 15:46:12.000000 UEVaultManager-1.9.4/README.md
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.423889 UEVaultManager-1.9.4/UEVaultManager/
--rw-rw-rw-   0        0        0      782 2023-09-06 07:13:38.000000 UEVaultManager-1.9.4/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.428888 UEVaultManager-1.9.4/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-08-04 12:51:09.000000 UEVaultManager-1.9.4/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    32928 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3145 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.430888 UEVaultManager-1.9.4/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.9.4/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.9.4/UEVaultManager/assets/checked_16.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.9.4/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.9.4/UEVaultManager/assets/unchecked_16.png
--rw-rw-rw-   0        0        0    85524 2023-09-06 06:38:05.000000 UEVaultManager-1.9.4/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    49798 2023-09-06 06:22:56.000000 UEVaultManager-1.9.4/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.431888 UEVaultManager-1.9.4/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-08-04 12:51:09.000000 UEVaultManager-1.9.4/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.432888 UEVaultManager-1.9.4/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-08-04 12:51:09.000000 UEVaultManager-1.9.4/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38946 2023-09-06 06:38:05.000000 UEVaultManager-1.9.4/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12394 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.435888 UEVaultManager-1.9.4/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-08-04 12:51:10.000000 UEVaultManager-1.9.4/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     1296 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0    23992 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      825 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0      732 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.443888 UEVaultManager-1.9.4/UEVaultManager/models/
--rw-rw-rw-   0        0        0     2560 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/UEAssetClass.py
--rw-rw-rw-   0        0        0    52668 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/UEAssetDbHandlerClass.py
--rw-rw-rw-   0        0        0    37242 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/UEAssetScraperClass.py
--rw-rw-rw-   0        0        0       16 2023-08-04 12:51:11.000000 UEVaultManager-1.9.4/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4719 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4513 2023-09-04 16:58:32.000000 UEVaultManager-1.9.4/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     2857 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0    17792 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/csv_sql_fields.py
--rw-rw-rw-   0        0        0     3638 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5236 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0      258 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     5888 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30495 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/manifest.py
--rw-rw-rw-   0        0        0     3280 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/models/types.py
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.444888 UEVaultManager-1.9.4/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-08-04 12:51:11.000000 UEVaultManager-1.9.4/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0     2353 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.447889 UEVaultManager-1.9.4/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0       16 2023-09-05 08:43:46.000000 UEVaultManager-1.9.4/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0    15391 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0    14393 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/tkgui/modules/functions_no_deps.py
--rw-rw-rw-   0        0        0     5059 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/tkgui/modules/globals.py
--rw-rw-rw-   0        0        0     1650 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/tkgui/modules/types.py
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.450888 UEVaultManager-1.9.4/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-08-04 12:51:14.000000 UEVaultManager-1.9.4/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0    10007 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1557 2023-08-04 12:51:13.000000 UEVaultManager-1.9.4/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10651 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-08-04 12:51:14.000000 UEVaultManager-1.9.4/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      751 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7267 2023-09-05 16:59:59.000000 UEVaultManager-1.9.4/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-09-06 07:13:55.427888 UEVaultManager-1.9.4/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     6539 2023-09-06 07:13:55.000000 UEVaultManager-1.9.4/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1896 2023-09-06 07:13:55.000000 UEVaultManager-1.9.4/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-06 07:13:55.000000 UEVaultManager-1.9.4/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-09-06 07:13:55.000000 UEVaultManager-1.9.4/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      335 2023-09-06 07:13:55.000000 UEVaultManager-1.9.4/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-09-06 07:13:55.000000 UEVaultManager-1.9.4/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      487 2023-06-26 09:40:30.000000 UEVaultManager-1.9.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-06 07:13:55.451888 UEVaultManager-1.9.4/setup.cfg
--rw-rw-rw-   0        0        0     3560 2023-08-04 12:50:54.000000 UEVaultManager-1.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.937807 UEVaultManager-1.9.5/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.9.5/LICENSE
+-rw-rw-rw-   0        0        0     6539 2023-09-06 07:46:14.936810 UEVaultManager-1.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5693 2023-06-26 15:46:12.000000 UEVaultManager-1.9.5/README.md
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.908804 UEVaultManager-1.9.5/UEVaultManager/
+-rw-rw-rw-   0        0        0      782 2023-09-06 07:46:09.000000 UEVaultManager-1.9.5/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.913805 UEVaultManager-1.9.5/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-08-04 12:51:09.000000 UEVaultManager-1.9.5/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    32928 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3145 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.915805 UEVaultManager-1.9.5/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.9.5/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.9.5/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.9.5/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.9.5/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    85524 2023-09-06 07:45:42.000000 UEVaultManager-1.9.5/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    49798 2023-09-06 06:22:56.000000 UEVaultManager-1.9.5/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.916806 UEVaultManager-1.9.5/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-08-04 12:51:09.000000 UEVaultManager-1.9.5/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.917806 UEVaultManager-1.9.5/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-08-04 12:51:09.000000 UEVaultManager-1.9.5/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38946 2023-09-06 06:38:05.000000 UEVaultManager-1.9.5/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12394 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.920805 UEVaultManager-1.9.5/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-08-04 12:51:10.000000 UEVaultManager-1.9.5/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     1296 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0    23992 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      825 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0      732 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.928805 UEVaultManager-1.9.5/UEVaultManager/models/
+-rw-rw-rw-   0        0        0     2560 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/UEAssetClass.py
+-rw-rw-rw-   0        0        0    52668 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/UEAssetDbHandlerClass.py
+-rw-rw-rw-   0        0        0    37242 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/UEAssetScraperClass.py
+-rw-rw-rw-   0        0        0       16 2023-08-04 12:51:11.000000 UEVaultManager-1.9.5/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4719 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4513 2023-09-04 16:58:32.000000 UEVaultManager-1.9.5/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2857 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0    17792 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/csv_sql_fields.py
+-rw-rw-rw-   0        0        0     3638 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5236 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      258 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5888 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30495 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/manifest.py
+-rw-rw-rw-   0        0        0     3280 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/models/types.py
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.929805 UEVaultManager-1.9.5/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-08-04 12:51:11.000000 UEVaultManager-1.9.5/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     2353 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.932805 UEVaultManager-1.9.5/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0       16 2023-09-05 08:43:46.000000 UEVaultManager-1.9.5/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0    15391 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0    14393 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/tkgui/modules/functions_no_deps.py
+-rw-rw-rw-   0        0        0     5059 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/tkgui/modules/globals.py
+-rw-rw-rw-   0        0        0     1650 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/tkgui/modules/types.py
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.936810 UEVaultManager-1.9.5/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-08-04 12:51:14.000000 UEVaultManager-1.9.5/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0    10007 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1557 2023-08-04 12:51:13.000000 UEVaultManager-1.9.5/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10651 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-08-04 12:51:14.000000 UEVaultManager-1.9.5/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      751 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7267 2023-09-05 16:59:59.000000 UEVaultManager-1.9.5/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-09-06 07:46:14.911806 UEVaultManager-1.9.5/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     6539 2023-09-06 07:46:14.000000 UEVaultManager-1.9.5/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1896 2023-09-06 07:46:14.000000 UEVaultManager-1.9.5/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-06 07:46:14.000000 UEVaultManager-1.9.5/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-09-06 07:46:14.000000 UEVaultManager-1.9.5/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      335 2023-09-06 07:46:14.000000 UEVaultManager-1.9.5/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-09-06 07:46:14.000000 UEVaultManager-1.9.5/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      487 2023-06-26 09:40:30.000000 UEVaultManager-1.9.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-09-06 07:46:14.937807 UEVaultManager-1.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     3560 2023-08-04 12:50:54.000000 UEVaultManager-1.9.5/setup.py
```

### Comparing `UEVaultManager-1.9.4/LICENSE` & `UEVaultManager-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/PKG-INFO` & `UEVaultManager-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.9.4
+Version: 1.9.5
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -64,8 +64,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.9.4 ## codename: Capricorn+4
+ UEVaultManager ## version:1.9.5 ## codename: Capricorn+5
```

### Comparing `UEVaultManager-1.9.4/README.md` & `UEVaultManager-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/__init__.py` & `UEVaultManager-1.9.5/UEVaultManager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.9.4'
+__version__ = '1.9.5'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
 # 4 Phoenix Ikki
 # 5 Leo Aiolia
 # 5 Virgo Shaka
 # 6 Libra Dohko
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
 # 9 Capricorn Shura
-__codename__ = 'Capricorn+4'
+__codename__ = 'Capricorn+5'
 # 10 Aquarius Camus
 # 11 Pisces Aphrodite
 __author__ = 'Laurent Ongaro'
 __author_email__ = 'laurent@gameamea.com'
 __description__ = 'Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine'
 __copyright__ = f'{year} {__author__}'
 __license__ = 'GPL-3'
```

### Comparing `UEVaultManager-1.9.4/UEVaultManager/api/egs.py` & `UEVaultManager-1.9.5/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/api/uevm.py` & `UEVaultManager-1.9.5/UEVaultManager/api/uevm.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.9.5/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/assets/main.ico` & `UEVaultManager-1.9.5/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/cli.py` & `UEVaultManager-1.9.5/UEVaultManager/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/core.py` & `UEVaultManager-1.9.5/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.9.5/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.9.5/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.9.5/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.9.5/UEVaultManager/lfs/uevmlfs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.9.5/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.9.5/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/UEAssetClass.py` & `UEVaultManager-1.9.5/UEVaultManager/models/UEAssetClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/UEAssetDbHandlerClass.py` & `UEVaultManager-1.9.5/UEVaultManager/models/UEAssetDbHandlerClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/UEAssetScraperClass.py` & `UEVaultManager-1.9.5/UEVaultManager/models/UEAssetScraperClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/app.py` & `UEVaultManager-1.9.5/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/chunk.py` & `UEVaultManager-1.9.5/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/config.py` & `UEVaultManager-1.9.5/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/csv_sql_fields.py` & `UEVaultManager-1.9.5/UEVaultManager/models/csv_sql_fields.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/downloading.py` & `UEVaultManager-1.9.5/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/egl.py` & `UEVaultManager-1.9.5/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.9.5/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/manifest.py` & `UEVaultManager-1.9.5/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/models/types.py` & `UEVaultManager-1.9.5/UEVaultManager/models/types.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.9.5/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.9.5/UEVaultManager/tkgui/modules/functions.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/tkgui/modules/functions_no_deps.py` & `UEVaultManager-1.9.5/UEVaultManager/tkgui/modules/functions_no_deps.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.9.5/UEVaultManager/tkgui/modules/globals.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/tkgui/modules/types.py` & `UEVaultManager-1.9.5/UEVaultManager/tkgui/modules/types.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/utils/cli.py` & `UEVaultManager-1.9.5/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.9.5/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.9.5/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.9.5/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.9.5/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.9.5/UEVaultManager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.9.4
+Version: 1.9.5
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -64,8 +64,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.9.4 ## codename: Capricorn+4
+ UEVaultManager ## version:1.9.5 ## codename: Capricorn+5
```

### Comparing `UEVaultManager-1.9.4/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.9.5/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.9.4/setup.py` & `UEVaultManager-1.9.5/setup.py`

 * *Files identical despite different names*

