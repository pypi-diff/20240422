# Comparing `tmp/auto-test-common-1.1.99.tar.gz` & `tmp/auto-test-common-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-1.1.99.tar", last modified: Thu Apr 11 08:55:14 2024, max compression
+gzip compressed data, was "auto-test-common-2.0.0.tar", last modified: Mon Apr 22 00:32:02 2024, max compression
```

## Comparing `auto-test-common-1.1.99.tar` & `auto-test-common-2.0.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.066594 auto-test-common-1.1.99/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 08:55:14.066709 auto-test-common-1.1.99/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:13.989069 auto-test-common-1.1.99/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      629 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-11 08:55:13.000000 auto-test-common-1.1.99/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:13.989996 auto-test-common-1.1.99/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.1.99/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:13.993699 auto-test-common-1.1.99/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.1.99/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    12431 2024-04-10 07:06:14.000000 auto-test-common-1.1.99/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-1.1.99/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-1.1.99/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:13.998256 auto-test-common-1.1.99/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.1.99/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7580 2024-04-11 08:54:57.000000 auto-test-common-1.1.99/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-1.1.99/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:13.999884 auto-test-common-1.1.99/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.99/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-1.1.99/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.009620 auto-test-common-1.1.99/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.1.99/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    25566 2024-04-11 02:38:06.000000 auto-test-common-1.1.99/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)    12127 2024-04-11 02:38:06.000000 auto-test-common-1.1.99/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-1.1.99/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.024995 auto-test-common-1.1.99/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.99/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.1.99/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.1.99/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-1.1.99/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.028067 auto-test-common-1.1.99/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-1.1.99/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-1.1.99/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-1.1.99/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.036513 auto-test-common-1.1.99/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-1.1.99/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.1.99/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11874 2024-01-09 02:15:13.000000 auto-test-common-1.1.99/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.1.99/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-1.1.99/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-1.1.99/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.037822 auto-test-common-1.1.99/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.1.99/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.1.99/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.046427 auto-test-common-1.1.99/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-1.1.99/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.1.99/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.1.99/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-1.1.99/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-1.1.99/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-1.1.99/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-11 08:55:14.066069 auto-test-common-1.1.99/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.1.99/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-1.1.99/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-1.1.99/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-1.1.99/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-1.1.99/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-1.1.99/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13091 2024-04-11 02:00:51.000000 auto-test-common-1.1.99/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.1.99/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-1.1.99/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.1.99/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-1.1.99/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-1.1.99/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-1.1.99/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      444 2024-04-11 08:55:14.067330 auto-test-common-1.1.99/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-1.1.99/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.096751 auto-test-common-2.0.0/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-04-22 00:32:02.096876 auto-test-common-2.0.0/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.058120 auto-test-common-2.0.0/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.058475 auto-test-common-2.0.0/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.0/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.060533 auto-test-common-2.0.0/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.0/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    12431 2024-04-10 07:06:14.000000 auto-test-common-2.0.0/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-2.0.0/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-2.0.0/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.063182 auto-test-common-2.0.0/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.0/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7336 2024-04-11 08:58:42.000000 auto-test-common-2.0.0/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.0/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.064138 auto-test-common-2.0.0/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.0/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.0/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.067462 auto-test-common-2.0.0/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.0/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    25952 2024-04-16 09:39:15.000000 auto-test-common-2.0.0/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)    12127 2024-04-11 02:38:06.000000 auto-test-common-2.0.0/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.0/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.072388 auto-test-common-2.0.0/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.0/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.0/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.0/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-2.0.0/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.075106 auto-test-common-2.0.0/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.0/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.0/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.0/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.080418 auto-test-common-2.0.0/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-2.0.0/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.0/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-18 06:49:09.000000 auto-test-common-2.0.0/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.0/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-2.0.0/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.0/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.081365 auto-test-common-2.0.0/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.0/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.085284 auto-test-common-2.0.0/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.0/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.0/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.0/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.0/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.0/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-2.0.0/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.095960 auto-test-common-2.0.0/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.0/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-2.0.0/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-2.0.0/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-2.0.0/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-2.0.0/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-2.0.0/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-16 09:39:15.000000 auto-test-common-2.0.0/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.0/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.0/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.0/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-2.0.0/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.0/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-2.0.0/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      443 2024-04-22 00:32:02.097529 auto-test-common-2.0.0/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-2.0.0/setup.py
```

### Comparing `auto-test-common-1.1.99/PKG-INFO` & `auto-test-common-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.99
+Version: 2.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.99/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-2.0.0/auto_test_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 1.1.99
+Version: 2.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-1.1.99/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-2.0.0/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/auto_test_common.egg-info/requires.txt` & `auto-test-common-2.0.0/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/autotest/base_requests.py` & `auto-test-common-2.0.0/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/autotest/handle_allure.py` & `auto-test-common-2.0.0/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/autotest/handle_assert.py` & `auto-test-common-2.0.0/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/common/api_driver.py` & `auto-test-common-2.0.0/common/common/api_driver.py`

 * *Files 10% similar despite different names*

```diff
@@ -127,31 +127,27 @@
                     from common.file.handle_system import adjust_path
                     _path = adjust_path(data[key])
                     if os.path.exists(path.join(TEST_FILE_PATH, _path)):
                         all_path = os.sep.join([TEST_FILE_PATH, _path])
                         from common.file.handle_system import adjust_path
                         all_path = adjust_path(all_path)
                         data[key] = (data[key], open(all_path, 'rb'))
-                    else:
-                        loguru.logger.warning('在file目录未找到上传文件【警告】')
                 elif isinstance(data[key], tuple):
                     from common.file.handle_system import adjust_path
                     _path = adjust_path(data[key][1])
                     if os.path.exists(path.join(TEST_FILE_PATH, _path)):
                         if data[key].__len__() == 3:
                             all_path = os.sep.join(TEST_FILE_PATH, _path)
                             from common.file.handle_system import adjust_path
                             all_path = adjust_path(all_path)
                             data[key] = (data[key][0], open(all_path, 'rb'), data[key][2])
                         elif data[key].__len__() == 2:
                             all_path = os.sep.join(TEST_FILE_PATH, _path)
                             from common.file.handle_system import adjust_path
                             all_path = adjust_path(all_path)
                             data[key] = (data[key][0], open(all_path, 'rb'))
-                    else:
-                        loguru.logger.warning('在file目录未找到上传文件【警告】')
                 else:
                     data = data
         return data
```

### Comparing `auto-test-common-1.1.99/common/common/constant.py` & `auto-test-common-2.0.0/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/common/test.py` & `auto-test-common-2.0.0/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/config/config.py` & `auto-test-common-2.0.0/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/data/data_process.py` & `auto-test-common-2.0.0/common/data/data_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,14 +374,15 @@
         _date = str(_date).strip()
         if len(_date) > 10:
             ts = int(time.mktime(time.strptime(_date, "%Y-%m-%d %H:%M:%S")))
         else:
             ts = int(time.mktime(time.strptime(_date, "%Y-%m-%d")))
         return ts
 
+
     @classmethod
     def check_test_data(self, testdatas:list):
         _testDatas = []
         casename = "00000"
         caseno = "00000"
         try:
             for testdata in testdatas:
@@ -396,41 +397,46 @@
                     if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
                         if casename != "00000" or caseno != "00000":
                             _testDatas.append(testdata)
                         else:
                             logger.warning(f"用例脚本文件未关联用例名称或者用例编号【检查用例】用例信息:{str(testdata)}")
                     else:
                         if casename != "00000" or caseno != "00000":
+                            _caseInfo = ServicePlatForm.getCaseInfoByNameOrID(caseno, casename)
+                            testdata[Constant.CASE_NO] = _caseInfo['key']
+                            testdata[Constant.CASE_TITLE] = _caseInfo['summary']
                             if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
                                 cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
                                 _list = ServicePlatForm.getCaseRun(cycleId, caseno, casename)
                                 if 'status' in _list:
                                     if _list['status'] == Constant.STATUS_PRE or _list['status'] == Constant.STATUS_AUTOTEST:
                                         ServicePlatForm.updateByRunid(_list['caserunid'], Constant.STATUS_AUTOTEST_PARA, "")
-                                        #_caseInfo = ServicePlatForm.getCaseInfoByNameOrID(caseno, casename)
-                                        # testdata[Constant.CASE_NO] = _caseInfo['key']
-                                        # testdata[Constant.CASE_TITLE] = _caseInfo['summary']
                                         testdata[Constant.CASE_NO] = caseno
                                         testdata[Constant.CASE_TITLE] = casename
                                         _testDatas.append(testdata)
-                                        print_debug(f'用例编号:{caseno} 用例名称:{casename} 周期编号:{cycleId} 用例信息:{str(_list)} 添加到执行队列')
+                                        print_debug(
+                                            f'用例编号:{caseno} 用例名称:{casename} 周期编号:{cycleId} 用例信息:{str(_list)} 添加到执行队列')
                                     else:
-                                        logger.info(f'用例编号:{caseno} 用例名称:{casename} 周期编号:{cycleId} 用例信息:{str(_list)} 无需添加执行队列')
+                                        logger.info(
+                                            f'用例编号:{caseno} 用例名称:{casename} 周期编号:{cycleId} 用例信息:{str(_list)} 无需添加执行队列')
                                 else:
                                     logger.info(f"获取周期中的测试用例信息异常【{cycleId},{caseno},{casename}】:{_list}")
+                            elif DataProcess.isNotNull(get_system_key(Constant.TEST_CASE_NAME_LIST)):
+                                if testdata[Constant.CASE_TITLE] in eval(get_system_key(Constant.TEST_CASE_NAME_LIST)):
+                                    _testDatas.append(testdata)
                             else:
                                 if Constant.CASE_STATUS in testdata:
                                     if testdata[Constant.CASE_STATUS].strip() != '否':
                                         _testDatas.append(testdata)
                                 else:
                                     _testDatas.append(testdata)
                         else:
                             logger.warning(f"用例脚本文件未关联用例名称或者用例编号【检查用例】用例信息:{str(testdata)}")
                 else:
-                    logger.warning(f"不复合单条测试数据标准:{testdatas}")
+                    logger.warning(f"单条测试数据不是一个字典用例信息【用例字典检查】用例信息:{testdata}")
             print_debug("处理前参数化测试数据:" + str(_testDatas))
             return _testDatas
         except Exception as e:
             logger.info(f'检查数据中用例属性错误信息测试数据:{testdatas} 用例名称：{casename} 用例编号：{caseno} 异常信息:'+repr(e))
         return _testDatas
 
     @classmethod
```

### Comparing `auto-test-common-1.1.99/common/data/handle_common.py` & `auto-test-common-2.0.0/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/data/template_data.py` & `auto-test-common-2.0.0/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/db/handle_db.py` & `auto-test-common-2.0.0/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/db/handle_db_batch.py` & `auto-test-common-2.0.0/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/db/handle_mongo.py` & `auto-test-common-2.0.0/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/db/handle_mysqldb.py` & `auto-test-common-2.0.0/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/db/handle_oracle.py` & `auto-test-common-2.0.0/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/db/handle_sqlserver.py` & `auto-test-common-2.0.0/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/driver/ui_page.py` & `auto-test-common-2.0.0/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/file/ReadFile.py` & `auto-test-common-2.0.0/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/file/handle_excel.py` & `auto-test-common-2.0.0/common/file/handle_excel.py`

 * *Files 7% similar despite different names*

```diff
@@ -195,66 +195,54 @@
     exlSpace = sh.merged_cells.ranges
 
     for spaceData in exlSpace:
         datavalue = spaceData.start_cell.value
         # print(datavalue)
         return datavalue
 
-def excel_to_list(data_file, sheet,_index:int=1,_filter:dict=None, _replace: bool=True, _checkData:bool=True):
+def excel_to_list(data_file, sheet, _index:int=1, _filter:dict=None,  _replace: bool=True):
     """
     读取Excel中特定sheet的数据，按行将数据存入数组datalist
     :param data_file:Excel文件目录
     :param sheet:需要读取的sheet名称
     :return:datalist
     """
     data_file = adjust_path_data(data_file)
-    data_list = []  # 新建个空列表，来存储所有的数据
-    wb = xlrd.open_workbook(data_file)  # 打开excel
-    sh = wb.sheet_by_name(sheet)  # 获取工作簿
-    # 获取标题行数据
-    #header = sh.row_values(0)
-    # 跳过标题行，从第二行开始取数据
+    data_list = []
+    wb = xlrd.open_workbook(data_file)
+    sh = wb.sheet_by_name(sheet)
     for row in range(_index, sh.nrows):
         d = dict()
-        # 将标题和每行数据组装成字典
         for col in range(0, sh.ncols):
-            # 获取指定单元格数据(行，列)
             cell_data = sh.cell_value(row, col)
             ctype = sh.cell(row, col).ctype
             if ctype == 2 and cell_data % 1 == 0.0:
                 cell_data = int(cell_data)
             if ctype == 3:
                 date = datetime(*xldate_as_tuple(cell_data, 0))
                 cell_data = date.strftime('%Y-%m-%d')
             col_title = sh.cell_value(0, col).strip()
             d[col_title] = cell_data
             d['$'+col_title] = cell_data
             d[col_title+'_cell'] = {"row": row, "col": col}
-        if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
-            casename = format_caseName(d[Constant.CASE_TITLE])
-            caseNo = d[Constant.CASE_NO]
-            if DataProcess.isNotNull(casename) or DataProcess.isNotNull(caseNo):
-                data_list.append(d)
-            else:
-                logger.info("用例脚本未关联用例名称或者用例编号【未关联用例名称或者编号】")
+        if _replace:
+            temp = DataBus.get_data(d)
+            temp['_excelPath'] = data_file
+            temp['_sheetName'] = sheet
         else:
-            if check_excel_data(d, _filter, _checkData):
-                if _replace:
-                    temp = DataBus.get_data(d)
-                    temp['_excelPath'] = data_file
-                    temp['_sheetName'] = sheet
-                else:
-                    temp = d
-                    temp['_excelPath'] = data_file
-                    temp['_sheetName'] = sheet
-                print_info(f'添加单个参数化用例数据: {temp}')
-                _caseInfo = ServicePlatForm.getCaseInfoByNameOrID(temp[Constant.CASE_NO], temp[Constant.CASE_TITLE])
-                temp[Constant.CASE_NO] = _caseInfo['key']
-                temp[Constant.CASE_TITLE] = _caseInfo['summary']
-                data_list.append(temp)
+            temp = d
+            temp['_excelPath'] = data_file
+            temp['_sheetName'] = sheet
+        print_info(f'添加单个参数化用例数据: {temp}')
+        if DataProcess.isNotNull(_filter):
+            for k, v in _filter.items():
+                if temp[k] == v:
+                    data_list.append(temp)
+        else:
+            data_list.append(temp)
         print_info(f'用例参数化数据: {data_list}')
     return data_list
 
 def check_excel_data(testdata:dict, _filter, _checkData):
     if _checkData:
         casename = format_caseName(testdata[Constant.CASE_TITLE])
         caseNo = testdata[Constant.CASE_NO]
```

### Comparing `auto-test-common-1.1.99/common/file/handle_file.py` & `auto-test-common-2.0.0/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/file/handle_reques.py` & `auto-test-common-2.0.0/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/file/handle_system.py` & `auto-test-common-2.0.0/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/file/handle_yaml.py` & `auto-test-common-2.0.0/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/mq/handle_rabbit.py` & `auto-test-common-2.0.0/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plat/ATF_platform.py` & `auto-test-common-2.0.0/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plat/jenkin_platform.py` & `auto-test-common-2.0.0/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plat/jira_platform.py` & `auto-test-common-2.0.0/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plat/mysql_platform.py` & `auto-test-common-2.0.0/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plat/service_platform.py` & `auto-test-common-2.0.0/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plugin/allure_plugin.py` & `auto-test-common-2.0.0/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plugin/assert_plugin.py` & `auto-test-common-2.0.0/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plugin/atf_plugin.py` & `auto-test-common-2.0.0/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plugin/data_bus.py` & `auto-test-common-2.0.0/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plugin/data_plugin.py` & `auto-test-common-2.0.0/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plugin/file_plugin.py` & `auto-test-common-2.0.0/common/plugin/file_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,23 +74,23 @@
                     logger.info(f"文件路径:{file_name_temp} Sheet:{sheet} 脚本用例文已经被处理")
             else:
                 set_system_key(Constant.SYNC_EXCEL_SHEET,excel_sheet.strip()+";")
                 logger.info(f"文件路径:{file_name_temp} Sheet:{sheet} 脚本用例文件开始同步")
                 _list = excel_to_list(file_name_temp, sheet, _index)
                 _list = DataProcess.check_test_data(_list)
         else:
-            _list = excel_to_list(file_name_temp, sheet, _index, _filter,  _replace, _checkData=True)
+            _list = excel_to_list(file_name_temp, sheet, _index, _filter,  _replace)
             _list = DataProcess.check_test_data(_list)
             _list = DataProcess.list_dict_duplicate_removal_byKey(_list, Constant.CASE_TITLE)
             _list = DataProcess.list_dict_duplicate_removal_byKey(_list, Constant.CASE_NO)
             for _temp in _list:
                 for key in _temp.keys():
                     _fileName, _sheet, _filter = self.handle_excel_data(_temp[key],file_name,sheet)
                     if DataProcess.isNotNull(_fileName):
-                        _subData = excel_to_list(path.join(file_path, _fileName), _sheet, _index, _filter, _replace, _checkData=False)
+                        _subData = excel_to_list(path.join(file_path, _fileName), _sheet, _index, _filter, _replace)
                         if _subData.__len__() > 0:
                             _temp[key] = _subData[0]
                             _temp["$"+key] = _subData
         return _list
 
     @classmethod
     def handle_excel_data(self, _str:str, _fileName:str, _sheetName:str):
```

### Comparing `auto-test-common-1.1.99/common/plugin/hooks_plugin.py` & `auto-test-common-2.0.0/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plugin/pytest_playwright.py` & `auto-test-common-2.0.0/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plugin/pytest_plugin.py` & `auto-test-common-2.0.0/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plugin/template_plugin.py` & `auto-test-common-2.0.0/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/common/plugin/yaml_plugin.py` & `auto-test-common-2.0.0/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.1.99/setup.py` & `auto-test-common-2.0.0/setup.py`

 * *Files identical despite different names*

