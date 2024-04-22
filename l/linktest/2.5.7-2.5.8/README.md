# Comparing `tmp/linktest-2.5.7.tar.gz` & `tmp/linktest-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.5.7.tar", last modified: Sat Apr 20 05:53:44 2024, max compression
+gzip compressed data, was "linktest-2.5.8.tar", last modified: Mon Apr 22 06:52:25 2024, max compression
```

## Comparing `linktest-2.5.7.tar` & `linktest-2.5.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-20 05:53:44.207859 linktest-2.5.7/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-20 05:53:44.207630 linktest-2.5.7/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-20 05:53:44.202529 linktest-2.5.7/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-19 02:39:47.000000 linktest-2.5.7/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-19 09:36:23.000000 linktest-2.5.7/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15760 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34732 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105788 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-19 02:39:55.000000 linktest-2.5.7/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13430 2024-04-19 09:59:20.000000 linktest-2.5.7/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-17 08:14:17.000000 linktest-2.5.7/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-20 05:53:44.207326 linktest-2.5.7/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-20 05:53:43.000000 linktest-2.5.7/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-20 05:53:43.000000 linktest-2.5.7/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-20 05:53:43.000000 linktest-2.5.7/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-20 05:53:43.000000 linktest-2.5.7/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-20 05:53:43.000000 linktest-2.5.7/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-20 05:53:44.207907 linktest-2.5.7/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-20 05:53:38.000000 linktest-2.5.7/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-22 06:52:25.281407 linktest-2.5.8/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-22 06:52:25.281186 linktest-2.5.8/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-22 06:52:25.279598 linktest-2.5.8/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-22 06:48:17.000000 linktest-2.5.8/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16684 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15760 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34732 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105788 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-22 06:48:22.000000 linktest-2.5.8/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14214 2024-04-22 06:46:24.000000 linktest-2.5.8/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-20 05:54:55.000000 linktest-2.5.8/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-22 06:52:25.280954 linktest-2.5.8/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-22 06:52:25.000000 linktest-2.5.8/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-22 06:52:25.000000 linktest-2.5.8/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-22 06:52:25.000000 linktest-2.5.8/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-22 06:52:25.000000 linktest-2.5.8/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-22 06:52:25.000000 linktest-2.5.8/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-22 06:52:25.281444 linktest-2.5.8/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-22 06:52:10.000000 linktest-2.5.8/setup.py
```

### Comparing `linktest-2.5.7/linktest/appium_utils.py` & `linktest-2.5.8/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/auto_generate_testcase_list.py` & `linktest-2.5.8/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.5.8/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/base_testcase.py` & `linktest-2.5.8/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/clean_data.py` & `linktest-2.5.8/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/conver_xml_into_db.py` & `linktest-2.5.8/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/database_helper.py` & `linktest-2.5.8/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/date_utilities.py` & `linktest-2.5.8/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/doctor.py` & `linktest-2.5.8/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/framework_log.py` & `linktest-2.5.8/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/generate_html_log.py` & `linktest-2.5.8/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/get_adb_devices.py` & `linktest-2.5.8/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/get_ios_devices_list.py` & `linktest-2.5.8/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/get_platform_info.py` & `linktest-2.5.8/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/get_project_info.py` & `linktest-2.5.8/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/html_report.py` & `linktest-2.5.8/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/logged_requests.py` & `linktest-2.5.8/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/main.py` & `linktest-2.5.8/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/memory_usage.py` & `linktest-2.5.8/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/re_func.py` & `linktest-2.5.8/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/run.py` & `linktest-2.5.8/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/run_testcase_thread.py` & `linktest-2.5.8/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/scp_report_to_specified_path.py` & `linktest-2.5.8/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/selenium_helper.py` & `linktest-2.5.8/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/timeout_thread.py` & `linktest-2.5.8/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/ui_testcase.py` & `linktest-2.5.8/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/update_config.py` & `linktest-2.5.8/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest/webdriver_wrapper.py` & `linktest-2.5.8/linktest/webdriver_wrapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 import os
 import typing
 from typing import List
 from typing import Dict
 from typing import Optional
 from typing import Union
 
+from selenium.webdriver import Keys
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.options import BaseOptions
 from selenium.webdriver.common.print_page_options import PrintOptions
 from selenium.webdriver.common.timeouts import Timeouts
 
 from selenium.webdriver import Chrome
 from selenium.webdriver.common.by import By
@@ -89,15 +90,31 @@
         self.logger.info(msg)
 
         if AUTO_SCREENSHOT_ON_ACTION:
             self.webdriver_wrapper.save_screenshot()
 
     def send_keys(self, *value):
         self.element.send_keys(*value)
-        self._log_action("send_keys", *value)
+
+        if value and value[0] == Keys.ENTER:
+            self._log_action("send_keys", "Keys.ENTER")
+        elif value and value[0] == Keys.CANCEL:
+            self._log_action("send_keys", "Keys.CANCEL")
+        elif value and value[0] == Keys.ESCAPE:
+            self._log_action("send_keys", "Keys.ESCAPE")
+        elif value and value[0] == Keys.SPACE:
+            self._log_action("send_keys", "Keys.SPACE")
+        elif value and value[0] == Keys.TAB:
+            self._log_action("send_keys", "Keys.TAB")
+        elif value and value[0] == Keys.BACKSPACE:
+            self._log_action("send_keys", "Keys.BACKSPACE")
+        elif value and value[0] == Keys.DELETE:
+            self._log_action("send_keys", "Keys.DELETE")
+        else:
+            self._log_action("send_keys", *value)
 
     def click(self):
         self.element.click()
         self._log_action("click")
 
     def clear(self):
         self.element.clear()
```

### Comparing `linktest-2.5.7/linktest/xml_report.py` & `linktest-2.5.8/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.7/linktest.egg-info/SOURCES.txt` & `linktest-2.5.8/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

