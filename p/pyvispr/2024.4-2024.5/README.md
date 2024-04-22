# Comparing `tmp/pyvispr-2024.4.tar.gz` & `tmp/pyvispr-2024.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvispr-2024.4.tar", last modified: Fri Apr 19 14:42:39 2024, max compression
+gzip compressed data, was "pyvispr-2024.5.tar", last modified: Mon Apr 22 09:30:31 2024, max compression
```

## Comparing `pyvispr-2024.4.tar` & `pyvispr-2024.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/
--rwx------   0 eric      (1000) users      (984)      139 2024-04-05 18:00:47.000000 pyvispr-2024.4/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     5710 2024-04-19 14:42:39.524234 pyvispr-2024.4/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      642 2024-02-07 09:03:58.000000 pyvispr-2024.4/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2024.4/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     4652 2024-02-07 09:03:58.000000 pyvispr-2024.4/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.514234 pyvispr-2024.4/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.517568 pyvispr-2024.4/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     2421 2024-02-07 09:22:47.000000 pyvispr-2024.4/documentation/wiki/description.asciidoc
--rwx------   0 eric      (1000) users      (984)      112 2024-02-07 08:56:45.000000 pyvispr-2024.4/pyproject.toml
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.517568 pyvispr-2024.4/pyvispr/
--rwx------   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2024.4/pyvispr/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/catalog/factory/
--rwx------   0 eric      (1000) users      (984)     1715 2024-04-19 07:34:07.000000 pyvispr-2024.4/pyvispr/catalog/factory/image_256.py
--rwx------   0 eric      (1000) users      (984)     1804 2024-01-19 10:13:27.000000 pyvispr-2024.4/pyvispr/catalog/factory/image_loader.py
--rwx------   0 eric      (1000) users      (984)    15855 2024-04-19 14:39:58.000000 pyvispr-2024.4/pyvispr/catalog/factory/image_viewer.py
--rwx------   0 eric      (1000) users      (984)     1975 2024-01-19 10:13:27.000000 pyvispr-2024.4/pyvispr/catalog/factory/numexpr_calculator.py
--rwx------   0 eric      (1000) users      (984)     1818 2024-01-19 10:18:15.000000 pyvispr-2024.4/pyvispr/catalog/factory/value.py
--rwx------   0 eric      (1000) users      (984)     5762 2024-04-18 07:03:13.000000 pyvispr-2024.4/pyvispr/catalog/factory/value_viewer.py
--rwx------   0 eric      (1000) users      (984)     7691 2024-04-11 08:05:54.000000 pyvispr-2024.4/pyvispr/catalog/installer.py
--rwx------   0 eric      (1000) users      (984)     4160 2024-04-19 07:40:32.000000 pyvispr-2024.4/pyvispr/catalog/parser.py
--rwx------   0 eric      (1000) users      (984)     2226 2024-04-10 14:04:29.000000 pyvispr-2024.4/pyvispr/catalog/type.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/config/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/config/appearance/
--rwx------   0 eric      (1000) users      (984)     1584 2024-04-10 13:34:33.000000 pyvispr-2024.4/pyvispr/config/appearance/backend.py
--rw-r--r--   0 eric      (1000) users      (984)     1611 2024-04-10 13:52:01.000000 pyvispr-2024.4/pyvispr/config/appearance/behavior.py
--rwx------   0 eric      (1000) users      (984)     2662 2024-04-19 14:06:18.000000 pyvispr-2024.4/pyvispr/config/appearance/color.py
--rwx------   0 eric      (1000) users      (984)     1727 2024-04-19 14:06:38.000000 pyvispr-2024.4/pyvispr/config/appearance/geometry.py
--rwx------   0 eric      (1000) users      (984)     1788 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/config/path.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/constant/
--rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 14:04:29.000000 pyvispr-2024.4/pyvispr/constant/app.py
--rwx------   0 eric      (1000) users      (984)     1961 2024-01-22 14:35:46.000000 pyvispr-2024.4/pyvispr/constant/catalog.py
--rw-r--r--   0 eric      (1000) users      (984)     1654 2024-04-10 13:34:03.000000 pyvispr-2024.4/pyvispr/constant/function.py
--rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-10 13:51:28.000000 pyvispr-2024.4/pyvispr/constant/path.py
--rw-r--r--   0 eric      (1000) users      (984)     1610 2024-04-10 15:59:22.000000 pyvispr-2024.4/pyvispr/constant/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/constant/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1873 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/constant/widget/function_header.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 13:59:48.000000 pyvispr-2024.4/pyvispr/constant/widget/list.py
--rw-r--r--   0 eric      (1000) users      (984)     1969 2024-04-11 12:23:33.000000 pyvispr-2024.4/pyvispr/constant/widget/node.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/extension/
--rwx------   0 eric      (1000) users      (984)    11886 2024-04-19 06:09:59.000000 pyvispr-2024.4/pyvispr/extension/function.py
--rwx------   0 eric      (1000) users      (984)     2907 2024-04-19 07:15:15.000000 pyvispr-2024.4/pyvispr/extension/module.py
--rwx------   0 eric      (1000) users      (984)     1986 2024-01-19 10:18:15.000000 pyvispr-2024.4/pyvispr/extension/qt6.py
--rwx------   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2024.4/pyvispr/extension/string_.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.517568 pyvispr-2024.4/pyvispr/flow/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/flow/descriptive/
--rwx------   0 eric      (1000) users      (984)     7948 2024-04-19 07:15:25.000000 pyvispr-2024.4/pyvispr/flow/descriptive/node.py
--rwx------   0 eric      (1000) users      (984)     4489 2024-04-11 12:50:13.000000 pyvispr-2024.4/pyvispr/flow/descriptive/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/flow/functional/
--rwx------   0 eric      (1000) users      (984)     4471 2024-04-19 13:44:55.000000 pyvispr-2024.4/pyvispr/flow/functional/graph.py
--rwx------   0 eric      (1000) users      (984)     4508 2024-04-19 14:19:48.000000 pyvispr-2024.4/pyvispr/flow/functional/link.py
--rwx------   0 eric      (1000) users      (984)    10587 2024-04-19 14:36:55.000000 pyvispr-2024.4/pyvispr/flow/functional/node_isolated.py
--rwx------   0 eric      (1000) users      (984)     5179 2024-04-19 14:41:22.000000 pyvispr-2024.4/pyvispr/flow/functional/node_linked.py
--rwx------   0 eric      (1000) users      (984)     2548 2024-04-19 14:19:48.000000 pyvispr-2024.4/pyvispr/flow/functional/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/flow/visual/
--rwx------   0 eric      (1000) users      (984)    18596 2024-04-19 13:37:01.000000 pyvispr-2024.4/pyvispr/flow/visual/graph.py
--rw-r--r--   0 eric      (1000) users      (984)     1858 2024-04-10 15:51:00.000000 pyvispr-2024.4/pyvispr/flow/visual/ii_value.py
--rwx------   0 eric      (1000) users      (984)     6200 2024-04-11 08:06:24.000000 pyvispr-2024.4/pyvispr/flow/visual/link.py
--rwx------   0 eric      (1000) users      (984)    13289 2024-04-19 13:42:58.000000 pyvispr-2024.4/pyvispr/flow/visual/node.py
--rwx------   0 eric      (1000) users      (984)     1879 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/flow/visual/socket.py
--rwx------   0 eric      (1000) users      (984)     7879 2024-04-19 13:11:30.000000 pyvispr-2024.4/pyvispr/flow/visual/whiteboard.py
--rwx------   0 eric      (1000) users      (984)     1917 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/install.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.517568 pyvispr-2024.4/pyvispr/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/interface/storage/
--rwx------   0 eric      (1000) users      (984)     3187 2024-04-19 06:39:34.000000 pyvispr-2024.4/pyvispr/interface/storage/loading.py
--rwx------   0 eric      (1000) users      (984)     3592 2024-04-19 14:39:57.000000 pyvispr-2024.4/pyvispr/interface/storage/stowing.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/interface/window/
--rwx------   0 eric      (1000) users      (984)    16232 2024-04-19 06:27:12.000000 pyvispr-2024.4/pyvispr/interface/window/installer.py
--rwx------   0 eric      (1000) users      (984)     7880 2024-04-18 07:10:06.000000 pyvispr-2024.4/pyvispr/interface/window/runner.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/interface/window/widget/
--rwx------   0 eric      (1000) users      (984)    16183 2024-04-18 07:10:09.000000 pyvispr-2024.4/pyvispr/interface/window/widget/function_header.py
--rwx------   0 eric      (1000) users      (984)     4147 2024-04-18 07:06:06.000000 pyvispr-2024.4/pyvispr/interface/window/widget/list.py
--rwx------   0 eric      (1000) users      (984)     2533 2024-01-16 14:25:32.000000 pyvispr-2024.4/pyvispr/interface/window/widget/list_file.py
--rwx------   0 eric      (1000) users      (984)     2710 2024-04-18 11:56:51.000000 pyvispr-2024.4/pyvispr/interface/window/widget/list_function.py
--rwx------   0 eric      (1000) users      (984)     1925 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/interface/window/widget/list_module.py
--rwx------   0 eric      (1000) users      (984)     3942 2024-04-19 14:11:04.000000 pyvispr-2024.4/pyvispr/interface/window/widget/list_node.py
--rwx------   0 eric      (1000) users      (984)     2412 2024-04-18 07:06:19.000000 pyvispr-2024.4/pyvispr/interface/window/widget/menu.py
--rwx------   0 eric      (1000) users      (984)     1908 2024-04-11 10:07:56.000000 pyvispr-2024.4/pyvispr/run.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/runtime/
--rw-r--r--   0 eric      (1000) users      (984)     1713 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/runtime/backend.py
--rw-r--r--   0 eric      (1000) users      (984)     1625 2024-04-10 13:44:05.000000 pyvispr-2024.4/pyvispr/runtime/catalog.py
--rw-r--r--   0 eric      (1000) users      (984)     1718 2024-04-10 14:44:38.000000 pyvispr-2024.4/pyvispr/runtime/socket.py
--rwx------   0 eric      (1000) users      (984)     1577 2024-04-19 14:42:19.000000 pyvispr-2024.4/pyvispr/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     5710 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     2224 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       87 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)        8 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-17 16:13:58.000000 pyvispr-2024.4/requirements.txt
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-19 14:42:39.527568 pyvispr-2024.4/setup.cfg
--rwx------   0 eric      (1000) users      (984)     8530 2024-04-11 11:30:02.000000 pyvispr-2024.4/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.356288 pyvispr-2024.5/
+-rwx------   0 eric      (1000) users      (984)      139 2024-04-05 18:00:47.000000 pyvispr-2024.5/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     5710 2024-04-22 09:30:31.356288 pyvispr-2024.5/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      642 2024-02-07 09:03:58.000000 pyvispr-2024.5/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2024.5/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4652 2024-02-07 09:03:58.000000 pyvispr-2024.5/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.336288 pyvispr-2024.5/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.339621 pyvispr-2024.5/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     2421 2024-04-19 15:02:26.000000 pyvispr-2024.5/documentation/wiki/description.asciidoc
+-rwx------   0 eric      (1000) users      (984)      112 2024-02-07 08:56:45.000000 pyvispr-2024.5/pyproject.toml
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.339621 pyvispr-2024.5/pyvispr/
+-rwx------   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2024.5/pyvispr/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.339621 pyvispr-2024.5/pyvispr/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.339621 pyvispr-2024.5/pyvispr/catalog/factory/
+-rwx------   0 eric      (1000) users      (984)     1715 2024-04-19 07:34:07.000000 pyvispr-2024.5/pyvispr/catalog/factory/image_256.py
+-rwx------   0 eric      (1000) users      (984)     1804 2024-01-19 10:13:27.000000 pyvispr-2024.5/pyvispr/catalog/factory/image_loader.py
+-rwx------   0 eric      (1000) users      (984)    15900 2024-04-20 17:50:38.000000 pyvispr-2024.5/pyvispr/catalog/factory/image_viewer.py
+-rwx------   0 eric      (1000) users      (984)     1975 2024-01-19 10:13:27.000000 pyvispr-2024.5/pyvispr/catalog/factory/numexpr_calculator.py
+-rwx------   0 eric      (1000) users      (984)     1818 2024-01-19 10:18:15.000000 pyvispr-2024.5/pyvispr/catalog/factory/value.py
+-rwx------   0 eric      (1000) users      (984)     5939 2024-04-21 14:27:40.000000 pyvispr-2024.5/pyvispr/catalog/factory/value_viewer.py
+-rwx------   0 eric      (1000) users      (984)     7691 2024-04-11 08:05:54.000000 pyvispr-2024.5/pyvispr/catalog/installer.py
+-rwx------   0 eric      (1000) users      (984)     4160 2024-04-19 07:40:32.000000 pyvispr-2024.5/pyvispr/catalog/parser.py
+-rwx------   0 eric      (1000) users      (984)     2226 2024-04-10 14:04:29.000000 pyvispr-2024.5/pyvispr/catalog/type.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.339621 pyvispr-2024.5/pyvispr/config/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.342954 pyvispr-2024.5/pyvispr/config/appearance/
+-rwx------   0 eric      (1000) users      (984)     1584 2024-04-10 13:34:33.000000 pyvispr-2024.5/pyvispr/config/appearance/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1611 2024-04-10 13:52:01.000000 pyvispr-2024.5/pyvispr/config/appearance/behavior.py
+-rwx------   0 eric      (1000) users      (984)     2662 2024-04-19 14:06:18.000000 pyvispr-2024.5/pyvispr/config/appearance/color.py
+-rwx------   0 eric      (1000) users      (984)     1727 2024-04-19 14:06:38.000000 pyvispr-2024.5/pyvispr/config/appearance/geometry.py
+-rwx------   0 eric      (1000) users      (984)     1788 2024-04-10 14:04:53.000000 pyvispr-2024.5/pyvispr/config/path.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.342954 pyvispr-2024.5/pyvispr/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 14:04:29.000000 pyvispr-2024.5/pyvispr/constant/app.py
+-rwx------   0 eric      (1000) users      (984)     1961 2024-01-22 14:35:46.000000 pyvispr-2024.5/pyvispr/constant/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1654 2024-04-10 13:34:03.000000 pyvispr-2024.5/pyvispr/constant/function.py
+-rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-10 13:51:28.000000 pyvispr-2024.5/pyvispr/constant/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     1610 2024-04-10 15:59:22.000000 pyvispr-2024.5/pyvispr/constant/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.342954 pyvispr-2024.5/pyvispr/constant/widget/
+-rw-r--r--   0 eric      (1000) users      (984)     1873 2024-04-10 14:04:53.000000 pyvispr-2024.5/pyvispr/constant/widget/function_header.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 13:59:48.000000 pyvispr-2024.5/pyvispr/constant/widget/list.py
+-rw-r--r--   0 eric      (1000) users      (984)     1969 2024-04-11 12:23:33.000000 pyvispr-2024.5/pyvispr/constant/widget/node.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.346288 pyvispr-2024.5/pyvispr/extension/
+-rwx------   0 eric      (1000) users      (984)    11886 2024-04-19 06:09:59.000000 pyvispr-2024.5/pyvispr/extension/function.py
+-rwx------   0 eric      (1000) users      (984)     2907 2024-04-19 07:15:15.000000 pyvispr-2024.5/pyvispr/extension/module.py
+-rwx------   0 eric      (1000) users      (984)     1986 2024-01-19 10:18:15.000000 pyvispr-2024.5/pyvispr/extension/qt6.py
+-rwx------   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2024.5/pyvispr/extension/string_.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.336288 pyvispr-2024.5/pyvispr/flow/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.346288 pyvispr-2024.5/pyvispr/flow/descriptive/
+-rwx------   0 eric      (1000) users      (984)     7948 2024-04-19 07:15:25.000000 pyvispr-2024.5/pyvispr/flow/descriptive/node.py
+-rwx------   0 eric      (1000) users      (984)     4489 2024-04-11 12:50:13.000000 pyvispr-2024.5/pyvispr/flow/descriptive/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.349621 pyvispr-2024.5/pyvispr/flow/functional/
+-rwx------   0 eric      (1000) users      (984)     4471 2024-04-19 13:44:55.000000 pyvispr-2024.5/pyvispr/flow/functional/graph.py
+-rwx------   0 eric      (1000) users      (984)     4508 2024-04-19 14:19:48.000000 pyvispr-2024.5/pyvispr/flow/functional/link.py
+-rwx------   0 eric      (1000) users      (984)    10587 2024-04-19 14:36:55.000000 pyvispr-2024.5/pyvispr/flow/functional/node_isolated.py
+-rwx------   0 eric      (1000) users      (984)     5179 2024-04-19 14:41:22.000000 pyvispr-2024.5/pyvispr/flow/functional/node_linked.py
+-rwx------   0 eric      (1000) users      (984)     2548 2024-04-19 14:19:48.000000 pyvispr-2024.5/pyvispr/flow/functional/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.349621 pyvispr-2024.5/pyvispr/flow/visual/
+-rwx------   0 eric      (1000) users      (984)    18596 2024-04-19 13:37:01.000000 pyvispr-2024.5/pyvispr/flow/visual/graph.py
+-rw-r--r--   0 eric      (1000) users      (984)     1858 2024-04-10 15:51:00.000000 pyvispr-2024.5/pyvispr/flow/visual/ii_value.py
+-rwx------   0 eric      (1000) users      (984)     6200 2024-04-11 08:06:24.000000 pyvispr-2024.5/pyvispr/flow/visual/link.py
+-rwx------   0 eric      (1000) users      (984)    13289 2024-04-19 13:42:58.000000 pyvispr-2024.5/pyvispr/flow/visual/node.py
+-rwx------   0 eric      (1000) users      (984)     1879 2024-04-10 14:04:53.000000 pyvispr-2024.5/pyvispr/flow/visual/socket.py
+-rwx------   0 eric      (1000) users      (984)     7879 2024-04-19 13:11:30.000000 pyvispr-2024.5/pyvispr/flow/visual/whiteboard.py
+-rwx------   0 eric      (1000) users      (984)     1917 2024-04-10 14:04:53.000000 pyvispr-2024.5/pyvispr/install.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.336288 pyvispr-2024.5/pyvispr/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.352954 pyvispr-2024.5/pyvispr/interface/storage/
+-rwx------   0 eric      (1000) users      (984)     3187 2024-04-19 06:39:34.000000 pyvispr-2024.5/pyvispr/interface/storage/loading.py
+-rwx------   0 eric      (1000) users      (984)     3592 2024-04-19 14:39:57.000000 pyvispr-2024.5/pyvispr/interface/storage/stowing.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.352954 pyvispr-2024.5/pyvispr/interface/window/
+-rwx------   0 eric      (1000) users      (984)    16232 2024-04-19 06:27:12.000000 pyvispr-2024.5/pyvispr/interface/window/installer.py
+-rwx------   0 eric      (1000) users      (984)     7880 2024-04-18 07:10:06.000000 pyvispr-2024.5/pyvispr/interface/window/runner.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.356288 pyvispr-2024.5/pyvispr/interface/window/widget/
+-rwx------   0 eric      (1000) users      (984)    16183 2024-04-18 07:10:09.000000 pyvispr-2024.5/pyvispr/interface/window/widget/function_header.py
+-rwx------   0 eric      (1000) users      (984)     4147 2024-04-18 07:06:06.000000 pyvispr-2024.5/pyvispr/interface/window/widget/list.py
+-rwx------   0 eric      (1000) users      (984)     2533 2024-01-16 14:25:32.000000 pyvispr-2024.5/pyvispr/interface/window/widget/list_file.py
+-rwx------   0 eric      (1000) users      (984)     2710 2024-04-18 11:56:51.000000 pyvispr-2024.5/pyvispr/interface/window/widget/list_function.py
+-rwx------   0 eric      (1000) users      (984)     1925 2024-04-10 14:04:53.000000 pyvispr-2024.5/pyvispr/interface/window/widget/list_module.py
+-rwx------   0 eric      (1000) users      (984)     3942 2024-04-19 14:11:04.000000 pyvispr-2024.5/pyvispr/interface/window/widget/list_node.py
+-rwx------   0 eric      (1000) users      (984)     2412 2024-04-18 07:06:19.000000 pyvispr-2024.5/pyvispr/interface/window/widget/menu.py
+-rwx------   0 eric      (1000) users      (984)     1908 2024-04-11 10:07:56.000000 pyvispr-2024.5/pyvispr/run.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.356288 pyvispr-2024.5/pyvispr/runtime/
+-rw-r--r--   0 eric      (1000) users      (984)     1713 2024-04-10 14:04:53.000000 pyvispr-2024.5/pyvispr/runtime/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1625 2024-04-10 13:44:05.000000 pyvispr-2024.5/pyvispr/runtime/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1718 2024-04-10 14:44:38.000000 pyvispr-2024.5/pyvispr/runtime/socket.py
+-rwx------   0 eric      (1000) users      (984)     1577 2024-04-22 09:30:09.000000 pyvispr-2024.5/pyvispr/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-22 09:30:31.356288 pyvispr-2024.5/pyvispr.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     5710 2024-04-22 09:30:31.000000 pyvispr-2024.5/pyvispr.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     2224 2024-04-22 09:30:31.000000 pyvispr-2024.5/pyvispr.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-22 09:30:31.000000 pyvispr-2024.5/pyvispr.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       87 2024-04-22 09:30:31.000000 pyvispr-2024.5/pyvispr.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-22 09:30:31.000000 pyvispr-2024.5/pyvispr.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)        8 2024-04-22 09:30:31.000000 pyvispr-2024.5/pyvispr.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-17 16:13:58.000000 pyvispr-2024.5/requirements.txt
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-22 09:30:31.356288 pyvispr-2024.5/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     8530 2024-04-11 11:30:02.000000 pyvispr-2024.5/setup.py
```

### Comparing `pyvispr-2024.4/PKG-INFO` & `pyvispr-2024.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2024.4
+Version: 2024.5
 Summary: Visual Programming App for Python
-Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
+Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
-Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyVispr//-/wikis/home
-Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
+Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyvispr//-/wikis/home
+Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
 Keywords: Visual programming,Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.11
```

### Comparing `pyvispr-2024.4/README-COPYRIGHT-utf8.txt` & `pyvispr-2024.5/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/README-LICENCE-utf8.txt` & `pyvispr-2024.5/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/README.rst` & `pyvispr-2024.5/README.rst`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/documentation/wiki/description.asciidoc` & `pyvispr-2024.5/documentation/wiki/description.asciidoc`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 :AUTHOR: Eric Debreuve
 :EMAIL: eric.debreuve@cnrs.fr
 
 :PROJECT_NAME: pyVispr
 :SHORT_DESCRIPTION: Visual Programming App for Python
 :KEYWORDS: Visual programming, Python
 
-:REPOSITORY_NAME: pyVispr
+:REPOSITORY_NAME: pyvispr
 :REPOSITORY_USER: eric.debreuve
 :REPOSITORY_SITE: src.koda.cnrs.fr
 :DOCUMENTATION_SITE: -/wikis/home
 :SINCE_YEAR: 2017
 
 :LICENSE_SHORT: CeCILL-2.1
 :LICENCE_LONG: CEA CNRS Inria Logiciel Libre License, version 2.1
```

### Comparing `pyvispr-2024.4/pyvispr/__init__.py` & `pyvispr-2024.5/pyvispr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/catalog/factory/image_256.py` & `pyvispr-2024.5/pyvispr/catalog/factory/image_256.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/catalog/factory/image_loader.py` & `pyvispr-2024.5/pyvispr/catalog/factory/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/catalog/factory/image_viewer.py` & `pyvispr-2024.5/pyvispr/catalog/factory/image_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     else:
         global_min, global_max = min_value, max_value
 
     if depth < 4:
         only_colors = image
     else:
         only_colors = image[..., :3]
-    if global_max > global_min:
+    if (global_max > global_min) and ((global_min, global_max) != (0, 255)):
         factor = 255.0 / (global_max - global_min)
         only_colors = numpy.round(
             factor * (only_colors.astype(numpy.float64, copy=False) - global_min)
         )
     if depth < 4:
         np_img = only_colors
     else:
```

### Comparing `pyvispr-2024.4/pyvispr/catalog/factory/numexpr_calculator.py` & `pyvispr-2024.5/pyvispr/catalog/factory/numexpr_calculator.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/catalog/factory/value.py` & `pyvispr-2024.5/pyvispr/catalog/factory/value.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/catalog/factory/value_viewer.py` & `pyvispr-2024.5/pyvispr/catalog/factory/value_viewer.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,16 +29,19 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import collections.abc as cllt
 import pprint as pprt
 import typing as h
 
+import numpy
+import PyQt6.QtCore as core
 import PyQt6.QtGui as qtui
 import PyQt6.QtWidgets as wdgt
+from PyQt6.QtCore import QRunnable as task_base_t
 from PyQt6.QtCore import QThreadPool as thread_manager_t
 from pyvispr.extension.qt6 import ExecuteApp, QtApp
 from pyvispr.runtime.backend import SCREEN_BACKEND
 
 
 def pyVisprValueViewer(value: h.Any, /) -> None:
     """"""
@@ -51,111 +54,109 @@
     #     The code below makes it disappear, but the table is not correctly populated then.
     # if value_viewer.thread_manager is not None:
     #     value_viewer.thread_manager.waitForDone()
     # Test also somewhere (not here though; it does not work):
     # value_viewer.thread_manager.moveToThread(wdgt.QApplication.instance().thread())
 
 
+class task_t(task_base_t):
+    def __init__(
+        self,
+        viewer: wdgt.QTableView,
+        model: qtui.QStandardItemModel,
+        value: cllt.Iterable[cllt.Iterable],
+        /,
+    ) -> None:
+        """"""
+        task_base_t.__init__(self)
+        self.viewer = viewer
+        self.model = model
+        self.value = value
+
+    @core.pyqtSlot()
+    def run(self) -> None:
+        """"""
+        min_value, max_value = numpy.amin(self.value), numpy.amax(self.value)
+        if max_value > min_value:
+            color = qtui.QColor()
+            if (min_value, max_value) != (0, 255):
+                factor = 255.0 / (max_value - min_value)
+            else:
+                factor = None
+        else:
+            color = factor = None
+
+        for row in self.value:
+            cells = map(str, row)
+            cells = tuple(map(qtui.QStandardItem, cells))
+            if color is None:
+                for cell in cells:
+                    cell.setTextAlignment(core.Qt.AlignmentFlag.AlignRight)
+            else:
+                for cell, value in zip(cells, row):
+                    if factor is None:
+                        gray = value
+                    else:
+                        gray = int(round(factor * (value - min_value)))
+                    color.setRgb(255 - gray, 255, 255 - gray, 255)
+                    cell.setData(
+                        core.QVariant(qtui.QBrush(color)),
+                        core.Qt.ItemDataRole.BackgroundRole,
+                    )
+                    cell.setTextAlignment(core.Qt.AlignmentFlag.AlignRight)
+            self.model.appendRow(cells)
+
+        self.viewer.resizeRowsToContents()
+        self.viewer.resizeColumnsToContents()
+
+        self.viewer.setEnabled(True)
+
+        self.value = None
+
+
 class value_viewer_t(wdgt.QMainWindow):
     def __init__(self, value: h.Any, wdw: wdgt.QWidget, /) -> None:
         """"""
         super().__init__(wdw)
 
-        if _ValueIsASequenceOfSequences(value):
-            self.value = value
+        try:
+            as_array = numpy.array(value)
+        except:
+            as_array = None
+        if (
+            (as_array is not None)
+            and (as_array.ndim < 3)
+            and (as_array.size > 1)
+            and (
+                numpy.issubdtype(as_array.dtype, numpy.integer)
+                or numpy.issubdtype(as_array.dtype, numpy.floating)
+            )
+        ):
+            self.value = as_array
 
             self.viewer = wdgt.QTableView()
             self.viewer.setEnabled(False)
 
             self.model = qtui.QStandardItemModel(self.viewer)
             self.model.setColumnCount(max(_elm.__len__() for _elm in self.value))
 
             self.viewer.setModel(self.model)
 
-            self.thread_manager = thread_manager_t()
-            self.thread_manager.start(self.PopulateTable)
+            self.filling_task = task_t(self.viewer, self.model, self.value)
+            thread_manager_t.globalInstance().start(self.filling_task)
         else:
             as_str = pprt.pformat(value, width=120, compact=True, sort_dicts=False)
             self.viewer = wdgt.QTextEdit(as_str)
-            self.value = self.model = self.thread_manager = None
 
         done = wdgt.QPushButton("Done")
 
         layout = wdgt.QVBoxLayout()
         layout.addWidget(self.viewer)
         layout.addWidget(done)
 
         central = wdgt.QWidget()
         central.setLayout(layout)
         self.setCentralWidget(central)
 
         self.setWindowTitle("pyVispr Value Viewer")
 
         SCREEN_BACKEND.CreateMessageCanal(done, "clicked", self.close)
-
-    def PopulateTable(self) -> None:
-        """"""
-        self.value: cllt.Iterable[cllt.Iterable]
-        self.viewer: wdgt.QTableView
-        self.model: qtui.QStandardItemModel
-
-        for row in self.value:
-            cells = map(str, row)
-            cells = map(qtui.QStandardItem, cells)
-            self.model.appendRow(cells)
-
-        self.viewer.resizeRowsToContents()
-        self.viewer.resizeColumnsToContents()
-
-        self.viewer.setEnabled(True)
-
-        self.value = None
-
-
-def _ValueIsASequenceOfSequences(value: h.Any, /) -> bool:
-    """"""
-    return (
-        isinstance(value, cllt.Iterable)
-        and hasattr(value, "__len__")
-        and (value.__len__() > 0)
-        and isinstance(value[0], cllt.Iterable)
-        and hasattr(value[0], "__len__")
-        and (value[0].__len__() > 0)
-        and not isinstance(value[0][0], cllt.Iterable)
-    )
-
-
-# from __future__ import annotations
-# import PyQt6.QtCore as qtcr
-# class table_model_t(qtcr.QAbstractTableModel):
-#     @classmethod
-#     def NewWithData(cls, data: cllt.Iterable[cllt.Iterable]) -> table_model_t:
-#         """"""
-#         output = cls()
-#
-#         output._data = data
-#         output.n_rows = data.__len__()
-#         output.n_cols = max(_elm.__len__() for _elm in data)
-#
-#         return output
-#
-#     def rowCount(self, _: qtcr.QModelIndex = None) -> int:
-#         """"""
-#         return self.n_rows
-#
-#     def columnCount(self, _: qtcr.QModelIndex = None) -> int:
-#         """"""
-#         return self.n_cols
-#
-#     def data(
-#         self,
-#         index: qtcr.QModelIndex,
-#         role: qtcr.Qt.ItemDataRole = qtcr.Qt.ItemDataRole.DisplayRole,
-#     ) -> str | None:
-#         """"""
-#         if role == qtcr.Qt.ItemDataRole.DisplayRole:
-#             r_idx = index.row()
-#             if 0 <= r_idx < self.n_rows:
-#                 row = self._data[r_idx]
-#                 c_idx = index.column()
-#                 if 0 <= c_idx < row.__len__():
-#                     return row[c_idx]
```

### Comparing `pyvispr-2024.4/pyvispr/catalog/installer.py` & `pyvispr-2024.5/pyvispr/catalog/installer.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/catalog/parser.py` & `pyvispr-2024.5/pyvispr/catalog/parser.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/catalog/type.py` & `pyvispr-2024.5/pyvispr/catalog/type.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/config/appearance/backend.py` & `pyvispr-2024.5/pyvispr/config/appearance/backend.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/config/appearance/behavior.py` & `pyvispr-2024.5/pyvispr/config/appearance/behavior.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/config/appearance/color.py` & `pyvispr-2024.5/pyvispr/config/appearance/color.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/config/appearance/geometry.py` & `pyvispr-2024.5/pyvispr/config/appearance/geometry.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/config/path.py` & `pyvispr-2024.5/pyvispr/config/path.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/constant/app.py` & `pyvispr-2024.5/pyvispr/constant/app.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/constant/catalog.py` & `pyvispr-2024.5/pyvispr/constant/catalog.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/constant/function.py` & `pyvispr-2024.5/pyvispr/constant/function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/constant/path.py` & `pyvispr-2024.5/pyvispr/constant/path.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/constant/socket.py` & `pyvispr-2024.5/pyvispr/constant/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/constant/widget/function_header.py` & `pyvispr-2024.5/pyvispr/constant/widget/function_header.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/constant/widget/list.py` & `pyvispr-2024.5/pyvispr/constant/widget/list.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/constant/widget/node.py` & `pyvispr-2024.5/pyvispr/constant/widget/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/extension/function.py` & `pyvispr-2024.5/pyvispr/extension/function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/extension/module.py` & `pyvispr-2024.5/pyvispr/extension/module.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/extension/qt6.py` & `pyvispr-2024.5/pyvispr/extension/qt6.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/extension/string_.py` & `pyvispr-2024.5/pyvispr/extension/string_.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/descriptive/node.py` & `pyvispr-2024.5/pyvispr/flow/descriptive/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/descriptive/socket.py` & `pyvispr-2024.5/pyvispr/flow/descriptive/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/functional/graph.py` & `pyvispr-2024.5/pyvispr/flow/functional/graph.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/functional/link.py` & `pyvispr-2024.5/pyvispr/flow/functional/link.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/functional/node_isolated.py` & `pyvispr-2024.5/pyvispr/flow/functional/node_isolated.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/functional/node_linked.py` & `pyvispr-2024.5/pyvispr/flow/functional/node_linked.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/functional/socket.py` & `pyvispr-2024.5/pyvispr/flow/functional/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/visual/graph.py` & `pyvispr-2024.5/pyvispr/flow/visual/graph.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/visual/ii_value.py` & `pyvispr-2024.5/pyvispr/flow/visual/ii_value.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/visual/link.py` & `pyvispr-2024.5/pyvispr/flow/visual/link.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/visual/node.py` & `pyvispr-2024.5/pyvispr/flow/visual/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/visual/socket.py` & `pyvispr-2024.5/pyvispr/flow/visual/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/flow/visual/whiteboard.py` & `pyvispr-2024.5/pyvispr/flow/visual/whiteboard.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/install.py` & `pyvispr-2024.5/pyvispr/install.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/interface/storage/loading.py` & `pyvispr-2024.5/pyvispr/interface/storage/loading.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/interface/storage/stowing.py` & `pyvispr-2024.5/pyvispr/interface/storage/stowing.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/interface/window/installer.py` & `pyvispr-2024.5/pyvispr/interface/window/installer.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/interface/window/runner.py` & `pyvispr-2024.5/pyvispr/interface/window/runner.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/interface/window/widget/function_header.py` & `pyvispr-2024.5/pyvispr/interface/window/widget/function_header.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/interface/window/widget/list.py` & `pyvispr-2024.5/pyvispr/interface/window/widget/list.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/interface/window/widget/list_file.py` & `pyvispr-2024.5/pyvispr/interface/window/widget/list_file.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/interface/window/widget/list_function.py` & `pyvispr-2024.5/pyvispr/interface/window/widget/list_function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/interface/window/widget/list_module.py` & `pyvispr-2024.5/pyvispr/interface/window/widget/list_module.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/interface/window/widget/list_node.py` & `pyvispr-2024.5/pyvispr/interface/window/widget/list_node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/interface/window/widget/menu.py` & `pyvispr-2024.5/pyvispr/interface/window/widget/menu.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/run.py` & `pyvispr-2024.5/pyvispr/run.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/runtime/backend.py` & `pyvispr-2024.5/pyvispr/runtime/backend.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/runtime/catalog.py` & `pyvispr-2024.5/pyvispr/runtime/catalog.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/runtime/socket.py` & `pyvispr-2024.5/pyvispr/runtime/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/pyvispr/version.py` & `pyvispr-2024.5/pyvispr/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2024.4"
+__version__ = "2024.5"
```

### Comparing `pyvispr-2024.4/pyvispr.egg-info/PKG-INFO` & `pyvispr-2024.5/pyvispr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2024.4
+Version: 2024.5
 Summary: Visual Programming App for Python
-Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
+Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
-Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyVispr//-/wikis/home
-Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
+Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyvispr//-/wikis/home
+Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
 Keywords: Visual programming,Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.11
```

### Comparing `pyvispr-2024.4/pyvispr.egg-info/SOURCES.txt` & `pyvispr-2024.5/pyvispr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.4/setup.py` & `pyvispr-2024.5/setup.py`

 * *Files identical despite different names*

