# Comparing `tmp/perfact-zodbsync-23.1.0.tar.gz` & `tmp/perfact_zodbsync-23.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfact-zodbsync-23.1.0.tar", last modified: Fri Mar  1 11:44:58 2024, max compression
+gzip compressed data, was "perfact_zodbsync-23.1.1.tar", last modified: Mon Apr 22 06:23:54 2024, max compression
```

## Comparing `perfact-zodbsync-23.1.0.tar` & `perfact_zodbsync-23.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-03-01 11:44:58.986252 perfact-zodbsync-23.1.0/
-drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-03-01 11:44:58.978252 perfact-zodbsync-23.1.0/.github/
-drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-03-01 11:44:58.982252 perfact-zodbsync-23.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 vdick     (1000) vdick     (1000)      834 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 vdick     (1000) vdick     (1000)      126 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0 vdick     (1000) vdick     (1000)      595 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-03-01 11:44:58.982252 perfact-zodbsync-23.1.0/.github/workflows/
--rw-r--r--   0 vdick     (1000) vdick     (1000)      576 2024-01-31 09:09:11.000000 perfact-zodbsync-23.1.0/.github/workflows/check.yml
--rw-r--r--   0 vdick     (1000) vdick     (1000)       82 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/.gitignore
--rw-r--r--   0 vdick     (1000) vdick     (1000)     9807 2024-03-01 11:39:24.000000 perfact-zodbsync-23.1.0/CHANGELOG
--rw-r--r--   0 vdick     (1000) vdick     (1000)    18009 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/LICENSE.txt
--rw-r--r--   0 vdick     (1000) vdick     (1000)        0 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/MANIFEST.in
--rw-r--r--   0 vdick     (1000) vdick     (1000)    13614 2024-03-01 11:44:58.986252 perfact-zodbsync-23.1.0/PKG-INFO
--rw-r--r--   0 vdick     (1000) vdick     (1000)    12915 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/README.md
--rw-r--r--   0 vdick     (1000) vdick     (1000)     1361 2024-01-31 09:09:11.000000 perfact-zodbsync-23.1.0/config.py
-drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-03-01 11:44:58.982252 perfact-zodbsync-23.1.0/perfact/
--rw-r--r--   0 vdick     (1000) vdick     (1000)       75 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/__init__.py
-drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-03-01 11:44:58.982252 perfact-zodbsync-23.1.0/perfact/zodbsync/
--rw-r--r--   0 vdick     (1000) vdick     (1000)      190 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/__init__.py
-drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-03-01 11:44:58.982252 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/
--rw-r--r--   0 vdick     (1000) vdick     (1000)        0 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/__init__.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     1625 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/checkout.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     1018 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/execute.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)      643 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/freeze.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     1817 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/layer_hash.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)      698 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/layer_init.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     2536 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/layer_update.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     1950 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/pick.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     1426 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/playback.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     4300 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/record.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     3612 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/reformat.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)      831 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/reset.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     6080 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/upload.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)    16953 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/watch.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)      471 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/commands/with_lock.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     4851 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/extedit.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     7199 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/helpers.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     4489 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/main.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     8075 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/object_mixins.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)    16504 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/object_types.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     1688 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/scripts.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)    11828 2024-02-26 11:44:43.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/subcommand.py
-drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-03-01 11:44:58.982252 perfact-zodbsync-23.1.0/perfact/zodbsync/tests/
--rw-r--r--   0 vdick     (1000) vdick     (1000)        0 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/tests/__init__.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     3865 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/tests/environment.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)     3082 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/tests/test_helpers.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)    73142 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/tests/test_sync.py
--rw-r--r--   0 vdick     (1000) vdick     (1000)    37496 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/perfact/zodbsync/zodbsync.py
-drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-03-01 11:44:58.986252 perfact-zodbsync-23.1.0/perfact_zodbsync.egg-info/
--rw-r--r--   0 vdick     (1000) vdick     (1000)    13614 2024-03-01 11:44:58.000000 perfact-zodbsync-23.1.0/perfact_zodbsync.egg-info/PKG-INFO
--rw-r--r--   0 vdick     (1000) vdick     (1000)     1464 2024-03-01 11:44:58.000000 perfact-zodbsync-23.1.0/perfact_zodbsync.egg-info/SOURCES.txt
--rw-r--r--   0 vdick     (1000) vdick     (1000)        1 2024-03-01 11:44:58.000000 perfact-zodbsync-23.1.0/perfact_zodbsync.egg-info/dependency_links.txt
--rw-r--r--   0 vdick     (1000) vdick     (1000)      181 2024-03-01 11:44:58.000000 perfact-zodbsync-23.1.0/perfact_zodbsync.egg-info/entry_points.txt
--rw-r--r--   0 vdick     (1000) vdick     (1000)       19 2024-03-01 11:44:58.000000 perfact-zodbsync-23.1.0/perfact_zodbsync.egg-info/requires.txt
--rw-r--r--   0 vdick     (1000) vdick     (1000)        8 2024-03-01 11:44:58.000000 perfact-zodbsync-23.1.0/perfact_zodbsync.egg-info/top_level.txt
--rw-r--r--   0 vdick     (1000) vdick     (1000)     1111 2024-01-24 13:44:34.000000 perfact-zodbsync-23.1.0/pyproject.toml
--rw-r--r--   0 vdick     (1000) vdick     (1000)       38 2024-03-01 11:44:58.986252 perfact-zodbsync-23.1.0/setup.cfg
--rw-r--r--   0 vdick     (1000) vdick     (1000)      705 2024-03-01 11:39:05.000000 perfact-zodbsync-23.1.0/tox.ini
+drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-04-22 06:23:54.897430 perfact_zodbsync-23.1.1/
+drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-04-22 06:23:54.885430 perfact_zodbsync-23.1.1/.github/
+drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-04-22 06:23:54.889430 perfact_zodbsync-23.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 vdick     (1000) vdick     (1000)      834 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 vdick     (1000) vdick     (1000)      126 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 vdick     (1000) vdick     (1000)      595 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-04-22 06:23:54.889430 perfact_zodbsync-23.1.1/.github/workflows/
+-rw-r--r--   0 vdick     (1000) vdick     (1000)      576 2024-01-31 09:09:11.000000 perfact_zodbsync-23.1.1/.github/workflows/check.yml
+-rw-r--r--   0 vdick     (1000) vdick     (1000)       82 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/.gitignore
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     9866 2024-04-22 06:20:15.000000 perfact_zodbsync-23.1.1/CHANGELOG
+-rw-r--r--   0 vdick     (1000) vdick     (1000)    18009 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/LICENSE.txt
+-rw-r--r--   0 vdick     (1000) vdick     (1000)        0 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/MANIFEST.in
+-rw-r--r--   0 vdick     (1000) vdick     (1000)    13614 2024-04-22 06:23:54.897430 perfact_zodbsync-23.1.1/PKG-INFO
+-rw-r--r--   0 vdick     (1000) vdick     (1000)    12915 2024-03-01 11:39:05.000000 perfact_zodbsync-23.1.1/README.md
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     1361 2024-01-31 09:09:11.000000 perfact_zodbsync-23.1.1/config.py
+drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-04-22 06:23:54.889430 perfact_zodbsync-23.1.1/perfact/
+-rw-r--r--   0 vdick     (1000) vdick     (1000)       75 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/__init__.py
+drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-04-22 06:23:54.893430 perfact_zodbsync-23.1.1/perfact/zodbsync/
+-rw-r--r--   0 vdick     (1000) vdick     (1000)      240 2024-04-22 06:19:42.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/__init__.py
+drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-04-22 06:23:54.897430 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/
+-rw-r--r--   0 vdick     (1000) vdick     (1000)        0 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/__init__.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     1625 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/checkout.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     1018 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/execute.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)      643 2024-03-01 11:39:05.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/freeze.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     1817 2024-03-01 11:39:05.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/layer_hash.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)      698 2024-03-01 11:39:05.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/layer_init.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     2536 2024-03-01 11:39:05.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/layer_update.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     1950 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/pick.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     1426 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/playback.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     4300 2024-03-01 11:39:05.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/record.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     3612 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/reformat.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)      831 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/reset.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     6080 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/upload.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)    16953 2024-03-01 11:39:05.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/watch.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)      471 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/commands/with_lock.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     4851 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/extedit.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     7517 2024-04-22 06:19:42.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/helpers.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     4489 2024-03-01 11:39:05.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/main.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     8075 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/object_mixins.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)    16504 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/object_types.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     1688 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/scripts.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)    11828 2024-02-26 11:44:43.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/subcommand.py
+drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-04-22 06:23:54.897430 perfact_zodbsync-23.1.1/perfact/zodbsync/tests/
+-rw-r--r--   0 vdick     (1000) vdick     (1000)        0 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/tests/__init__.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     3865 2024-03-01 11:39:05.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/tests/environment.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     3082 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/tests/test_helpers.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)    73142 2024-04-19 21:06:03.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/tests/test_sync.py
+-rw-r--r--   0 vdick     (1000) vdick     (1000)    37339 2024-04-22 06:19:42.000000 perfact_zodbsync-23.1.1/perfact/zodbsync/zodbsync.py
+drwxr-xr-x   0 vdick     (1000) vdick     (1000)        0 2024-04-22 06:23:54.897430 perfact_zodbsync-23.1.1/perfact_zodbsync.egg-info/
+-rw-r--r--   0 vdick     (1000) vdick     (1000)    13614 2024-04-22 06:23:54.000000 perfact_zodbsync-23.1.1/perfact_zodbsync.egg-info/PKG-INFO
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     1464 2024-04-22 06:23:54.000000 perfact_zodbsync-23.1.1/perfact_zodbsync.egg-info/SOURCES.txt
+-rw-r--r--   0 vdick     (1000) vdick     (1000)        1 2024-04-22 06:23:54.000000 perfact_zodbsync-23.1.1/perfact_zodbsync.egg-info/dependency_links.txt
+-rw-r--r--   0 vdick     (1000) vdick     (1000)      181 2024-04-22 06:23:54.000000 perfact_zodbsync-23.1.1/perfact_zodbsync.egg-info/entry_points.txt
+-rw-r--r--   0 vdick     (1000) vdick     (1000)       19 2024-04-22 06:23:54.000000 perfact_zodbsync-23.1.1/perfact_zodbsync.egg-info/requires.txt
+-rw-r--r--   0 vdick     (1000) vdick     (1000)        8 2024-04-22 06:23:54.000000 perfact_zodbsync-23.1.1/perfact_zodbsync.egg-info/top_level.txt
+-rw-r--r--   0 vdick     (1000) vdick     (1000)     1111 2024-01-24 13:44:34.000000 perfact_zodbsync-23.1.1/pyproject.toml
+-rw-r--r--   0 vdick     (1000) vdick     (1000)       38 2024-04-22 06:23:54.897430 perfact_zodbsync-23.1.1/setup.cfg
+-rw-r--r--   0 vdick     (1000) vdick     (1000)      705 2024-03-01 11:39:05.000000 perfact_zodbsync-23.1.1/tox.ini
```

### Comparing `perfact-zodbsync-23.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `perfact_zodbsync-23.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `perfact_zodbsync-23.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/.github/workflows/check.yml` & `perfact_zodbsync-23.1.1/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/CHANGELOG` & `perfact_zodbsync-23.1.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+23.1.1
+  * Add method that exposes reading the db_modtime
+
 23.1.0
   * Update README
   * Explicitly name git branch in tests
   * Add configuration option playback_hook
 
 22.2.5
   * Omit title attributes if they are callable.
```

### Comparing `perfact-zodbsync-23.1.0/LICENSE.txt` & `perfact_zodbsync-23.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/PKG-INFO` & `perfact_zodbsync-23.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfact-zodbsync
-Version: 23.1.0
+Version: 23.1.1
 Summary: Synchronize ZODB objects with a file system structure
 Author-email: Ján Jockusch <jan.jockusch@perfact.de>, Viktor Dick <viktor.dick@perfact.de>
 Project-URL: Homepage, https://github.com/perfact/zodbsync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Framework :: Zope
```

### Comparing `perfact-zodbsync-23.1.0/README.md` & `perfact_zodbsync-23.1.1/README.md`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/config.py` & `perfact_zodbsync-23.1.1/config.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/checkout.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/execute.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/execute.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/freeze.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/layer_hash.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/layer_hash.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/layer_init.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/layer_init.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/layer_update.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/layer_update.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/pick.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/pick.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/playback.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/playback.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/record.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/record.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/reformat.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/reformat.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/reset.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/reset.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/upload.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/upload.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/commands/watch.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/extedit.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/extedit.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/helpers.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,7 +229,21 @@
         if arr[pos] == 255:
             arr[pos] = 0
             pos -= 1
         else:
             arr[pos] += 1
             break
     return bytes(arr)
+
+
+def obj_modtime(obj):  # pragma: no cover
+    '''
+    Allow access to private method of an object to read out the modtime.
+    '''
+    return obj._p_mtime
+
+
+def db_modtime(context):  # pragma: no cover
+    """
+    Allow access to a modtime for the whole ZODB.
+    """
+    return context._p_jar._db.lastTransaction()
```

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/main.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/main.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/object_mixins.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/object_mixins.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/object_types.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/object_types.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/scripts.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/scripts.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/subcommand.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/subcommand.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/tests/environment.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/tests/environment.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/tests/test_helpers.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/tests/test_sync.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/perfact/zodbsync/zodbsync.py` & `perfact_zodbsync-23.1.1/perfact/zodbsync/zodbsync.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,21 +166,14 @@
         children = temp_obj.manage_cutObjects(temp_obj.objectIds())
         obj.manage_pasteObjects(children)
         parent.manage_delObjects([temp_id])
 
     return obj
 
 
-def obj_modtime(obj):  # pragma: no cover
-    '''
-    Allow access to private method of an object to read out the modtime.
-    '''
-    return obj._p_mtime
-
-
 class ZODBSync:
     '''A ZODBSync instance is capable of mirroring a part of the ZODB
     object tree in the file system.
 
     By default, the syncer creates a subdirectory "__root__" in the
     given directory and can use the methods "record()" and
     "playback()" to get all objects from the ZODB or write them back,
```

### Comparing `perfact-zodbsync-23.1.0/perfact_zodbsync.egg-info/PKG-INFO` & `perfact_zodbsync-23.1.1/perfact_zodbsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfact-zodbsync
-Version: 23.1.0
+Version: 23.1.1
 Summary: Synchronize ZODB objects with a file system structure
 Author-email: Ján Jockusch <jan.jockusch@perfact.de>, Viktor Dick <viktor.dick@perfact.de>
 Project-URL: Homepage, https://github.com/perfact/zodbsync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Framework :: Zope
```

### Comparing `perfact-zodbsync-23.1.0/perfact_zodbsync.egg-info/SOURCES.txt` & `perfact_zodbsync-23.1.1/perfact_zodbsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/pyproject.toml` & `perfact_zodbsync-23.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `perfact-zodbsync-23.1.0/tox.ini` & `perfact_zodbsync-23.1.1/tox.ini`

 * *Files identical despite different names*

