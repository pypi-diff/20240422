# Comparing `tmp/houdini_package_manager-1.1.2.tar.gz` & `tmp/houdini_package_manager-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "houdini_package_manager-1.1.2.tar", max compression
+gzip compressed data, was "houdini_package_manager-1.1.3.tar", max compression
```

## Comparing `houdini_package_manager-1.1.2.tar` & `houdini_package_manager-1.1.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    34523 2024-04-09 04:44:02.947486 houdini_package_manager-1.1.2/LICENSE
--rw-r--r--   0        0        0     7059 2024-04-09 04:44:02.947486 houdini_package_manager-1.1.2/README.md
--rw-r--r--   0        0        0       22 2024-04-09 04:44:03.067484 houdini_package_manager-1.1.2/houdini_package_manager/__init__.py
--rw-r--r--   0        0        0     1936 2024-04-09 04:44:03.067484 houdini_package_manager-1.1.2/houdini_package_manager/main.py
--rw-r--r--   0        0        0     1975 2024-04-09 04:44:03.067484 houdini_package_manager-1.1.2/houdini_package_manager/meta/meta_tools.py
--rw-r--r--   0        0        0   614544 2024-04-09 04:44:03.071484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Black.ttf
--rw-r--r--   0        0        0   672480 2024-04-09 04:44:03.075484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf
--rw-r--r--   0        0        0   657188 2024-04-09 04:44:03.079484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Bold.ttf
--rw-r--r--   0        0        0   699008 2024-04-09 04:44:03.083484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0        0        0   723544 2024-04-09 04:44:03.087484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Italic.ttf
--rw-r--r--   0        0        0   644556 2024-04-09 04:44:03.091484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Light.ttf
--rw-r--r--   0        0        0   658212 2024-04-09 04:44:03.095484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf
--rw-r--r--   0        0        0   637068 2024-04-09 04:44:03.095484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Medium.ttf
--rw-r--r--   0        0        0   695588 2024-04-09 04:44:03.099484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf
--rw-r--r--   0        0        0   657212 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Regular.ttf
--rw-r--r--   0        0        0      332 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add.svg
--rw-r--r--   0        0        0      329 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_hover.svg
--rw-r--r--   0        0        0    10421 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages.svg
--rw-r--r--   0        0        0    10472 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_confirm.svg
--rw-r--r--   0        0        0    10475 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg
--rw-r--r--   0        0        0    10424 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_hover.svg
--rw-r--r--   0        0        0     1991 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/bug.svg
--rw-r--r--   0        0        0     1988 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/bug_hover.svg
--rw-r--r--   0        0        0      803 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/clear_selection.svg
--rw-r--r--   0        0        0      800 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/clear_selection_hover.svg
--rw-r--r--   0        0        0      427 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/delete.svg
--rw-r--r--   0        0        0      424 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/delete_hover.svg
--rw-r--r--   0        0        0      505 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/docs.svg
--rw-r--r--   0        0        0      502 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/docs_hover.svg
--rw-r--r--   0        0        0      455 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/file.svg
--rw-r--r--   0        0        0      452 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/file_hover.svg
--rw-r--r--   0        0        0      382 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/folder.svg
--rw-r--r--   0        0        0      379 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/folder_hover.svg
--rw-r--r--   0        0        0     4286 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm.ico
--rw-r--r--   0        0        0      566 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm.svg
--rw-r--r--   0        0        0      598 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_ICO.svg
--rw-r--r--   0        0        0      591 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_grey.svg
--rw-r--r--   0        0        0      588 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_grey_hover.svg
--rw-r--r--   0        0        0      569 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_hover.svg
--rw-r--r--   0        0        0      571 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_icon.svg
--rw-r--r--   0        0        0      696 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/invert_selection.svg
--rw-r--r--   0        0        0      693 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/invert_selection_hover.svg
--rw-r--r--   0        0        0      323 2024-04-09 04:44:03.103484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/migrate.svg
--rw-r--r--   0        0        0      320 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/migrate_hover.svg
--rw-r--r--   0        0        0     1455 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh.svg
--rw-r--r--   0        0        0     1625 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_all.svg
--rw-r--r--   0        0        0     1622 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_all_hover.svg
--rw-r--r--   0        0        0     1452 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_hover.svg
--rw-r--r--   0        0        0      484 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/remove.svg
--rw-r--r--   0        0        0      390 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/remove_all_items.svg
--rw-r--r--   0        0        0      387 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/remove_all_items_hover.svg
--rw-r--r--   0        0        0      502 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/remove_hover.svg
--rw-r--r--   0        0        0      837 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/repo.svg
--rw-r--r--   0        0        0      834 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/repo_hover.svg
--rw-r--r--   0        0        0      224 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/toggle_off.svg
--rw-r--r--   0        0        0      221 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/toggle_off_hover.svg
--rw-r--r--   0        0        0      334 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/toggle_on.svg
--rw-r--r--   0        0        0      331 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/toggle_on_hover.svg
--rw-r--r--   0        0        0      677 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/warning.svg
--rw-r--r--   0        0        0      680 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/warning_hover.svg
--rw-r--r--   0        0        0      868 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/utils.py
--rw-r--r--   0        0        0      655 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/actions.py
--rw-r--r--   0        0        0    22508 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/add_packages_layout.py
--rw-r--r--   0        0        0     3574 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/custom_widgets.py
--rw-r--r--   0        0        0     3840 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/dialogs.py
--rw-r--r--   0        0        0     7350 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/main_window.py
--rw-r--r--   0        0        0    21983 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/packages_layout.py
--rw-r--r--   0        0        0    12686 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/widgets/packages_table.py
--rw-r--r--   0        0        0    34452 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/wrangle/config_control.py
--rw-r--r--   0        0        0     1126 2024-04-09 04:44:03.107484 houdini_package_manager-1.1.2/houdini_package_manager/wrangle/package_templates.py
--rw-r--r--   0        0        0     2109 2024-04-09 04:44:23.039289 houdini_package_manager-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     7740 1970-01-01 00:00:00.000000 houdini_package_manager-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-22 01:00:33.438748 houdini_package_manager-1.1.3/LICENSE
+-rw-r--r--   0        0        0     7059 2024-04-22 01:00:33.438748 houdini_package_manager-1.1.3/README.md
+-rw-r--r--   0        0        0       22 2024-04-22 01:00:33.554749 houdini_package_manager-1.1.3/houdini_package_manager/__init__.py
+-rw-r--r--   0        0        0     1936 2024-04-22 01:00:33.554749 houdini_package_manager-1.1.3/houdini_package_manager/main.py
+-rw-r--r--   0        0        0     1975 2024-04-22 01:00:33.554749 houdini_package_manager-1.1.3/houdini_package_manager/meta/meta_tools.py
+-rw-r--r--   0        0        0   614544 2024-04-22 01:00:33.558749 houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Black.ttf
+-rw-r--r--   0        0        0   672480 2024-04-22 01:00:33.562749 houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf
+-rw-r--r--   0        0        0   657188 2024-04-22 01:00:33.566749 houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Bold.ttf
+-rw-r--r--   0        0        0   699008 2024-04-22 01:00:33.570749 houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0        0        0   723544 2024-04-22 01:00:33.574749 houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Italic.ttf
+-rw-r--r--   0        0        0   644556 2024-04-22 01:00:33.578749 houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Light.ttf
+-rw-r--r--   0        0        0   658212 2024-04-22 01:00:33.582749 houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0        0        0   637068 2024-04-22 01:00:33.586749 houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Medium.ttf
+-rw-r--r--   0        0        0   695588 2024-04-22 01:00:33.590749 houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf
+-rw-r--r--   0        0        0   657212 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Regular.ttf
+-rw-r--r--   0        0        0      332 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/add.svg
+-rw-r--r--   0        0        0      329 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/add_hover.svg
+-rw-r--r--   0        0        0    10421 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/add_packages.svg
+-rw-r--r--   0        0        0    10472 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/add_packages_confirm.svg
+-rw-r--r--   0        0        0    10475 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg
+-rw-r--r--   0        0        0    10424 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/add_packages_hover.svg
+-rw-r--r--   0        0        0     1991 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/bug.svg
+-rw-r--r--   0        0        0     1988 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/bug_hover.svg
+-rw-r--r--   0        0        0      803 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/clear_selection.svg
+-rw-r--r--   0        0        0      800 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/clear_selection_hover.svg
+-rw-r--r--   0        0        0      427 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/delete.svg
+-rw-r--r--   0        0        0      424 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/delete_hover.svg
+-rw-r--r--   0        0        0      505 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/docs.svg
+-rw-r--r--   0        0        0      502 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/docs_hover.svg
+-rw-r--r--   0        0        0      455 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/file.svg
+-rw-r--r--   0        0        0      452 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/file_hover.svg
+-rw-r--r--   0        0        0      382 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/folder.svg
+-rw-r--r--   0        0        0      379 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/folder_hover.svg
+-rw-r--r--   0        0        0     4286 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm.ico
+-rw-r--r--   0        0        0      566 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm.svg
+-rw-r--r--   0        0        0      598 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm_ICO.svg
+-rw-r--r--   0        0        0      591 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm_grey.svg
+-rw-r--r--   0        0        0      588 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm_grey_hover.svg
+-rw-r--r--   0        0        0      569 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm_hover.svg
+-rw-r--r--   0        0        0      571 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm_icon.svg
+-rw-r--r--   0        0        0      696 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/invert_selection.svg
+-rw-r--r--   0        0        0      693 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/invert_selection_hover.svg
+-rw-r--r--   0        0        0      323 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/migrate.svg
+-rw-r--r--   0        0        0      320 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/migrate_hover.svg
+-rw-r--r--   0        0        0     1455 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/refresh.svg
+-rw-r--r--   0        0        0     1625 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/refresh_all.svg
+-rw-r--r--   0        0        0     1622 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/refresh_all_hover.svg
+-rw-r--r--   0        0        0     1452 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/refresh_hover.svg
+-rw-r--r--   0        0        0      484 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/remove.svg
+-rw-r--r--   0        0        0      390 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/remove_all_items.svg
+-rw-r--r--   0        0        0      387 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/remove_all_items_hover.svg
+-rw-r--r--   0        0        0      502 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/remove_hover.svg
+-rw-r--r--   0        0        0      837 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/repo.svg
+-rw-r--r--   0        0        0      834 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/repo_hover.svg
+-rw-r--r--   0        0        0      224 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/toggle_off.svg
+-rw-r--r--   0        0        0      221 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/toggle_off_hover.svg
+-rw-r--r--   0        0        0      334 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/toggle_on.svg
+-rw-r--r--   0        0        0      331 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/toggle_on_hover.svg
+-rw-r--r--   0        0        0      677 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/warning.svg
+-rw-r--r--   0        0        0      680 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/warning_hover.svg
+-rw-r--r--   0        0        0      868 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/utils.py
+-rw-r--r--   0        0        0      655 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/widgets/actions.py
+-rw-r--r--   0        0        0    22508 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/widgets/add_packages_layout.py
+-rw-r--r--   0        0        0     3574 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/widgets/custom_widgets.py
+-rw-r--r--   0        0        0     3840 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/widgets/dialogs.py
+-rw-r--r--   0        0        0     7350 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/widgets/main_window.py
+-rw-r--r--   0        0        0    21983 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/widgets/packages_layout.py
+-rw-r--r--   0        0        0    12695 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/widgets/packages_table.py
+-rw-r--r--   0        0        0    35138 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/wrangle/config_control.py
+-rw-r--r--   0        0        0     1138 2024-04-22 01:00:33.594749 houdini_package_manager-1.1.3/houdini_package_manager/wrangle/package_templates.py
+-rw-r--r--   0        0        0     2109 2024-04-22 01:00:55.950932 houdini_package_manager-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7740 1970-01-01 00:00:00.000000 houdini_package_manager-1.1.3/PKG-INFO
```

### Comparing `houdini_package_manager-1.1.2/LICENSE` & `houdini_package_manager-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/README.md` & `houdini_package_manager-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/main.py` & `houdini_package_manager-1.1.3/houdini_package_manager/main.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/meta/meta_tools.py` & `houdini_package_manager-1.1.3/houdini_package_manager/meta/meta_tools.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Black.ttf` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Bold.ttf` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Italic.ttf` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Light.ttf` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Medium.ttf` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Medium.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/fonts/Lato-Regular.ttf` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/add_packages.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_confirm.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/add_packages_confirm.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/add_packages_hover.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/add_packages_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/bug.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/bug.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/bug_hover.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/bug_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/clear_selection.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/clear_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/clear_selection_hover.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/clear_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm.ico` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm.ico`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_ICO.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm_ICO.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_grey.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm_grey.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_grey_hover.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm_grey_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_hover.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/hpm_icon.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/hpm_icon.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/invert_selection.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/invert_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/invert_selection_hover.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/invert_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/refresh.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_all.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/refresh_all.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_all_hover.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/refresh_all_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/refresh_hover.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/refresh_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/repo.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/repo.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/repo_hover.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/repo_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/warning.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/resources/icons/warning_hover.svg` & `houdini_package_manager-1.1.3/houdini_package_manager/resources/icons/warning_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/utils.py` & `houdini_package_manager-1.1.3/houdini_package_manager/utils.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/widgets/actions.py` & `houdini_package_manager-1.1.3/houdini_package_manager/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/widgets/add_packages_layout.py` & `houdini_package_manager-1.1.3/houdini_package_manager/widgets/add_packages_layout.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/widgets/custom_widgets.py` & `houdini_package_manager-1.1.3/houdini_package_manager/widgets/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/widgets/dialogs.py` & `houdini_package_manager-1.1.3/houdini_package_manager/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/widgets/main_window.py` & `houdini_package_manager-1.1.3/houdini_package_manager/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/widgets/packages_layout.py` & `houdini_package_manager-1.1.3/houdini_package_manager/widgets/packages_layout.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/widgets/packages_table.py` & `houdini_package_manager-1.1.3/houdini_package_manager/widgets/packages_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         button_warning.clicked.connect(parent.open_path)
 
         return button_warning
 
     @staticmethod
     def label_no_plugin_data() -> QLabel:
         # if there's no plugin data
-        label = QLabel("No plugin data")
+        label = QLabel("No plugin folder found.")
         return label
 
     @staticmethod
     def combo_plugins(parent, value) -> QComboBox:
         combo = DropDown(parent)
         value = [str(path) for path in value]
```

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/wrangle/config_control.py` & `houdini_package_manager-1.1.3/houdini_package_manager/wrangle/config_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         metadata = dict(item.split(" := ") for item in metadata if len(item) > 0)
         for key, value in metadata.items():  # remove first and last quotes
             if value[0] in ["'", '"'] and value[-1] in ["'", '"']:
                 metadata[key] = value[1:-1]
 
         return metadata
 
-    def this_houdini_python_version(self) -> Path or None:
+    def this_houdini_python_version(self) -> Union[Path, None]:
         """
         Finds the latest installed version of Python that shipped with this Houdini (Windows only).
         Returns a Path object of the python directory.
         """
 
         hou_folders = os.listdir(self.HFS)
         python_folders = [folder for folder in hou_folders if re.match(r"python\d+", folder)]
@@ -650,33 +650,46 @@
         for path in plugin_paths_from_config:
             if path in self._hconfig_plugin_paths:
                 self._plugin_paths.append(path)
 
     def _load(self) -> None:
         """
         Load json contents.
-        Handles invalid json such as directory paths with single \\ character delimiters.
+        Handles invalid json. If the json cannot be recovered, an empty dict will be set.
         """
 
         if not isinstance(self.config_path, Path):
             raise TypeError("path must be a pathlib.Path object.")
 
-        # convert invalid json values that are paths with '\' to '\\' to prevent json loading error
         class JSONPathDecoder(json.JSONDecoder):
+            """
+            Tries to parse invalid json into valid json by accounting for some possible errors.
+            """
+
             def decode(self, s, **kwargs):
                 regex_replacements = [
-                    (re.compile(r"([^\\])\\([^\\])"), r"\1\\\\\2"),
-                    (re.compile(r",(\s*])"), r"\1"),
+                    (re.compile(r"([^\\])\\([^\\])"), r"\1\\\\\2"),  # Fix single backslashes in paths
+                    (re.compile(r",(\s*[\]}])"), r"\1"),  # Remove extraneous commas at the end of objects and arrays
+                    (re.compile(r"}\s*{"), r"}, {"),  # Fix missing commas between objects
                 ]
                 for regex, replacement in regex_replacements:
                     s = regex.sub(replacement, s)
                 return super().decode(s, **kwargs)
 
-        with open(self.config_path) as f:
-            data = json.load(f, cls=JSONPathDecoder)
+        try:
+            with open(self.config_path) as f:
+                data = json.load(f)
+        except json.decoder.JSONDecodeError:
+            logging.warning(f"Invalid json (might fail to resolve/parse): {self.config_path}")
+            self.warnings.append("Invalid JSON! Fix errors and refresh this table.")
+            try:
+                with open(self.config_path) as f:
+                    data = json.load(f, cls=JSONPathDecoder)
+            except Exception:  # final catch all for all other broken json errors
+                data = {}
 
         self._raw_json = data
         self.config = data
 
     def _flatten_package(self, data, prefix=None) -> list:
         """
         Recursively traverses a JSON-like data structure and returns a list of paths
```

### Comparing `houdini_package_manager-1.1.2/houdini_package_manager/wrangle/package_templates.py` & `houdini_package_manager-1.1.3/houdini_package_manager/wrangle/package_templates.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class PackageTemplates:
     """
     Various package template formats.
     """
 
     @staticmethod
-    def standard(houdini_path: Path):
+    def standard(path_to_plugin: Path):
         """
         A standard package template.
 
         Houdini will recognize:
             HOUDINI_PATH
             hpath (Shortcut to set HOUDINI_PATH. "path" has been deprecated in favor of hpath.)
             HOUDINI_TOOLBAR_PATH
@@ -20,22 +20,22 @@
             enable
             recommends
 
         Note: Do not include empty values for some keys, like recommends,
         because it was cause Houdini to crash on startup.
         """
 
-        if not houdini_path.exists():
-            raise FileNotFoundError(f"Does not exist: {houdini_path}")
+        if not path_to_plugin.exists():
+            raise FileNotFoundError(f"Does not exist: {path_to_plugin}")
 
-        houdini_path = str(houdini_path)
+        path_to_plugin = str(path_to_plugin)
 
         package = {
             "env": [
-                {"HOUDINI_PATH": houdini_path},
+                {"HOUDINI_PATH": path_to_plugin},
                 {"HOUDINI_OTLSCAN_PATH": "$HOUDINI_PATH/otls"},
                 {"HOUDINI_TOOLBAR_PATH": "$HOUDINI_PATH/toolbar"},
                 {"PYTHONPATH": "$HOUDINI_PATH/scripts/python"},
             ]
         }
 
         return package
```

### Comparing `houdini_package_manager-1.1.2/pyproject.toml` & `houdini_package_manager-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "houdini_package_manager"
-version = "1.1.2"
+version = "1.1.3"
 description = "GUI package manager for Houdini"
 authors = ["Ariff Jeff <ariffjeff@icloud.com>"]
 repository = "https://github.com/ariffjeff/houdini-package-manager"
 documentation = "https://ariffjeff.github.io/houdini-package-manager/"
 readme = "README.md"
 packages = [
   {include = "houdini_package_manager"}
```

### Comparing `houdini_package_manager-1.1.2/PKG-INFO` & `houdini_package_manager-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: houdini_package_manager
-Version: 1.1.2
+Version: 1.1.3
 Summary: GUI package manager for Houdini
 Home-page: https://github.com/ariffjeff/houdini-package-manager
 Author: Ariff Jeff
 Author-email: ariffjeff@icloud.com
 Requires-Python: >=3.10.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

