# Comparing `tmp/aacommons-0.2.7.tar.gz` & `tmp/aacommons-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aacommons-0.2.7.tar", last modified: Thu May  4 12:37:50 2023, max compression
+gzip compressed data, was "aacommons-0.2.8.tar", last modified: Mon Apr 22 06:04:01 2024, max compression
```

## Comparing `aacommons-0.2.7.tar` & `aacommons-0.2.8.tar`

### file list

```diff
@@ -1,56 +1,53 @@
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/
--rw-rw-r--   0 apang     (1000) apang     (1000)      623 2021-11-13 04:56:04.000000 aacommons-0.2.7/LICENSE
--rw-rw-r--   0 apang     (1000) apang     (1000)       16 2021-11-13 04:56:04.000000 aacommons-0.2.7/MANIFEST.in
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/NOTICE
--rw-rw-r--   0 apang     (1000) apang     (1000)      317 2023-05-04 12:37:50.313813 aacommons-0.2.7/PKG-INFO
--rw-rw-r--   0 apang     (1000) apang     (1000)      102 2021-11-13 04:56:04.000000 aacommons-0.2.7/README.rst
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.309813 aacommons-0.2.7/aacommons/
--rw-rw-r--   0 apang     (1000) apang     (1000)      686 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/__init__.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.309813 aacommons-0.2.7/aacommons/contentprovider/
--rw-rw-r--   0 apang     (1000) apang     (1000)    13694 2021-11-22 11:50:54.000000 aacommons-0.2.7/aacommons/contentprovider/ContentProvider.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     5107 2023-05-04 12:24:06.000000 aacommons-0.2.7/aacommons/contentprovider/RedisStore.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      877 2021-11-22 09:25:18.000000 aacommons-0.2.7/aacommons/contentprovider/__init__.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      955 2021-11-13 07:54:13.000000 aacommons-0.2.7/aacommons/contentprovider/util.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.309813 aacommons-0.2.7/aacommons/dataparser/
--rwxrwxr-x   0 apang     (1000) apang     (1000)     8951 2021-11-13 08:30:24.000000 aacommons-0.2.7/aacommons/dataparser/AirRecorder.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/__init__.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/aacommons/dataparser/cli/
--rw-rw-r--   0 apang     (1000) apang     (1000)     5632 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/AbstractTableParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     1268 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/CliParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     1174 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/CliParserBase.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     2339 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/GenericJsonCsvTableParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     7230 2022-02-11 08:47:35.000000 aacommons-0.2.7/aacommons/dataparser/cli/GenericRegexTableParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     3541 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     5710 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosDpStd.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     4455 2022-09-26 06:48:33.000000 aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosSmart.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     5561 2023-05-04 12:35:43.000000 aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosStd.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     8061 2023-05-04 12:35:43.000000 aacommons-0.2.7/aacommons/dataparser/cli/TableHelpers.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/__init__.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/aacommons/dataparser/cli/arcli/
--rw-rw-r--   0 apang     (1000) apang     (1000)     7506 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliContentProvider.py
--rwxrwxr-x   0 apang     (1000) apang     (1000)     5566 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliContext.py
--rw-rw-r--   0 apang     (1000) apang     (1000)    19680 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliDocuments.py
--rwxrwxr-x   0 apang     (1000) apang     (1000)    55157 2023-05-04 12:35:43.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliParser.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     2778 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliParserRequest.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     1288 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliResult.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     8585 2023-05-04 12:35:43.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliSampleRunner.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/dataparser/cli/arcli/__init__.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/aacommons/helpers/
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/helpers/__init__.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     2122 2021-11-13 08:32:41.000000 aacommons-0.2.7/aacommons/helpers/get_my_ip.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     2938 2023-02-23 00:48:58.000000 aacommons-0.2.7/aacommons/helpers/jstyleson_lint.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/aacommons/misc/
--rw-rw-r--   0 apang     (1000) apang     (1000)    23940 2021-11-30 08:07:06.000000 aacommons-0.2.7/aacommons/misc/Stats.py
--rw-rw-r--   0 apang     (1000) apang     (1000)      608 2021-11-13 04:56:04.000000 aacommons-0.2.7/aacommons/misc/__init__.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.309813 aacommons-0.2.7/aacommons.egg-info/
--rw-rw-r--   0 apang     (1000) apang     (1000)      317 2023-05-04 12:37:50.000000 aacommons-0.2.7/aacommons.egg-info/PKG-INFO
--rw-rw-r--   0 apang     (1000) apang     (1000)     1621 2023-05-04 12:37:50.000000 aacommons-0.2.7/aacommons.egg-info/SOURCES.txt
--rw-rw-r--   0 apang     (1000) apang     (1000)        1 2023-05-04 12:37:50.000000 aacommons-0.2.7/aacommons.egg-info/dependency_links.txt
--rw-rw-r--   0 apang     (1000) apang     (1000)       54 2023-05-04 12:37:50.000000 aacommons-0.2.7/aacommons.egg-info/requires.txt
--rw-rw-r--   0 apang     (1000) apang     (1000)       10 2023-05-04 12:37:50.000000 aacommons-0.2.7/aacommons.egg-info/top_level.txt
--rw-rw-r--   0 apang     (1000) apang     (1000)       38 2023-05-04 12:37:50.313813 aacommons-0.2.7/setup.cfg
--rwxrwxr-x   0 apang     (1000) apang     (1000)      611 2023-05-04 12:36:47.000000 aacommons-0.2.7/setup.py
-drwxrwxr-x   0 apang     (1000) apang     (1000)        0 2023-05-04 12:37:50.313813 aacommons-0.2.7/tests/
--rw-rw-r--   0 apang     (1000) apang     (1000)     3197 2021-11-13 04:56:04.000000 aacommons-0.2.7/tests/test_dataparser_airrecorder.py
--rw-rw-r--   0 apang     (1000) apang     (1000)    24217 2023-02-23 00:48:58.000000 aacommons-0.2.7/tests/test_dataparser_cli.py
--rw-rw-r--   0 apang     (1000) apang     (1000)     3611 2022-02-11 08:47:35.000000 aacommons-0.2.7/tests/test_table_helpers.py
+drwxr-xr-x   0 tbastian   (503) staff       (20)        0 2024-04-22 06:04:01.203920 aacommons-0.2.8/
+-rw-r--r--   0 tbastian   (503) staff       (20)      623 2020-11-21 07:21:19.000000 aacommons-0.2.8/LICENSE
+-rw-r--r--   0 tbastian   (503) staff       (20)       16 2020-11-14 08:26:33.000000 aacommons-0.2.8/MANIFEST.in
+-rw-r--r--   0 tbastian   (503) staff       (20)      608 2020-11-21 07:23:38.000000 aacommons-0.2.8/NOTICE
+-rw-r--r--   0 tbastian   (503) staff       (20)      317 2024-04-22 06:04:01.203758 aacommons-0.2.8/PKG-INFO
+-rw-r--r--   0 tbastian   (503) staff       (20)      102 2021-03-25 10:05:06.000000 aacommons-0.2.8/README.rst
+drwxr-xr-x   0 tbastian   (503) staff       (20)        0 2024-04-22 06:04:01.194029 aacommons-0.2.8/aacommons/
+-rw-r--r--   0 tbastian   (503) staff       (20)      686 2020-12-15 14:31:40.000000 aacommons-0.2.8/aacommons/__init__.py
+drwxr-xr-x   0 tbastian   (503) staff       (20)        0 2024-04-22 06:04:01.196320 aacommons-0.2.8/aacommons/contentprovider/
+-rw-r--r--   0 tbastian   (503) staff       (20)    13694 2021-11-23 05:46:16.000000 aacommons-0.2.8/aacommons/contentprovider/ContentProvider.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     5107 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/contentprovider/RedisStore.py
+-rw-r--r--   0 tbastian   (503) staff       (20)      877 2021-11-22 09:57:55.000000 aacommons-0.2.8/aacommons/contentprovider/__init__.py
+-rw-r--r--   0 tbastian   (503) staff       (20)      955 2021-11-22 09:57:55.000000 aacommons-0.2.8/aacommons/contentprovider/util.py
+drwxr-xr-x   0 tbastian   (503) staff       (20)        0 2024-04-22 06:04:01.196935 aacommons-0.2.8/aacommons/dataparser/
+-rwxr-xr-x   0 tbastian   (503) staff       (20)     8951 2021-11-22 09:57:55.000000 aacommons-0.2.8/aacommons/dataparser/AirRecorder.py
+-rw-r--r--   0 tbastian   (503) staff       (20)      608 2020-11-19 15:08:12.000000 aacommons-0.2.8/aacommons/dataparser/__init__.py
+drwxr-xr-x   0 tbastian   (503) staff       (20)        0 2024-04-22 06:04:01.200307 aacommons-0.2.8/aacommons/dataparser/cli/
+-rw-r--r--   0 tbastian   (503) staff       (20)     5632 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/dataparser/cli/AbstractTableParser.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     1268 2021-08-08 16:45:50.000000 aacommons-0.2.8/aacommons/dataparser/cli/CliParser.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     1174 2021-08-08 16:45:50.000000 aacommons-0.2.8/aacommons/dataparser/cli/CliParserBase.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     2339 2021-01-04 09:55:37.000000 aacommons-0.2.8/aacommons/dataparser/cli/GenericJsonCsvTableParser.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     7230 2022-02-08 09:49:09.000000 aacommons-0.2.8/aacommons/dataparser/cli/GenericRegexTableParser.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     3722 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/dataparser/cli/RowColumnTableParser.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     6463 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/dataparser/cli/RowColumnTableParserAcxStd.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     5710 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/dataparser/cli/RowColumnTableParserAosDpStd.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     4455 2022-09-22 08:38:16.000000 aacommons-0.2.8/aacommons/dataparser/cli/RowColumnTableParserAosSmart.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     5561 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/dataparser/cli/RowColumnTableParserAosStd.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     8772 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/dataparser/cli/TableHelpers.py
+-rw-r--r--   0 tbastian   (503) staff       (20)      608 2020-11-19 15:08:48.000000 aacommons-0.2.8/aacommons/dataparser/cli/__init__.py
+drwxr-xr-x   0 tbastian   (503) staff       (20)        0 2024-04-22 06:04:01.202221 aacommons-0.2.8/aacommons/dataparser/cli/arcli/
+-rw-r--r--   0 tbastian   (503) staff       (20)     7506 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliContentProvider.py
+-rwxr-xr-x   0 tbastian   (503) staff       (20)     5566 2021-08-08 16:45:50.000000 aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliContext.py
+-rw-r--r--   0 tbastian   (503) staff       (20)    19680 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliDocuments.py
+-rwxr-xr-x   0 tbastian   (503) staff       (20)    55157 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliParser.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     2778 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliParserRequest.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     1288 2021-08-08 16:45:50.000000 aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliResult.py
+-rw-r--r--   0 tbastian   (503) staff       (20)    10668 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliSampleRunner.py
+-rw-r--r--   0 tbastian   (503) staff       (20)      608 2021-08-08 16:45:50.000000 aacommons-0.2.8/aacommons/dataparser/cli/arcli/__init__.py
+drwxr-xr-x   0 tbastian   (503) staff       (20)        0 2024-04-22 06:04:01.202937 aacommons-0.2.8/aacommons/helpers/
+-rw-r--r--   0 tbastian   (503) staff       (20)      608 2020-11-19 15:08:12.000000 aacommons-0.2.8/aacommons/helpers/__init__.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     2122 2021-11-22 09:57:55.000000 aacommons-0.2.8/aacommons/helpers/get_my_ip.py
+-rw-r--r--   0 tbastian   (503) staff       (20)     2938 2024-04-21 17:14:33.000000 aacommons-0.2.8/aacommons/helpers/jstyleson_lint.py
+drwxr-xr-x   0 tbastian   (503) staff       (20)        0 2024-04-22 06:04:01.203508 aacommons-0.2.8/aacommons/misc/
+-rw-r--r--   0 tbastian   (503) staff       (20)    23940 2021-12-15 06:39:51.000000 aacommons-0.2.8/aacommons/misc/Stats.py
+-rw-r--r--   0 tbastian   (503) staff       (20)      608 2020-11-19 15:08:12.000000 aacommons-0.2.8/aacommons/misc/__init__.py
+drwxr-xr-x   0 tbastian   (503) staff       (20)        0 2024-04-22 06:04:01.195302 aacommons-0.2.8/aacommons.egg-info/
+-rw-r--r--   0 tbastian   (503) staff       (20)      317 2024-04-22 06:04:01.000000 aacommons-0.2.8/aacommons.egg-info/PKG-INFO
+-rw-r--r--   0 tbastian   (503) staff       (20)     1582 2024-04-22 06:04:01.000000 aacommons-0.2.8/aacommons.egg-info/SOURCES.txt
+-rw-r--r--   0 tbastian   (503) staff       (20)        1 2024-04-22 06:04:01.000000 aacommons-0.2.8/aacommons.egg-info/dependency_links.txt
+-rw-r--r--   0 tbastian   (503) staff       (20)       54 2024-04-22 06:04:01.000000 aacommons-0.2.8/aacommons.egg-info/requires.txt
+-rw-r--r--   0 tbastian   (503) staff       (20)       10 2024-04-22 06:04:01.000000 aacommons-0.2.8/aacommons.egg-info/top_level.txt
+-rw-r--r--   0 tbastian   (503) staff       (20)       38 2024-04-22 06:04:01.203996 aacommons-0.2.8/setup.cfg
+-rwxr-xr-x   0 tbastian   (503) staff       (20)      611 2024-04-21 17:14:33.000000 aacommons-0.2.8/setup.py
```

### Comparing `aacommons-0.2.7/LICENSE` & `aacommons-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/NOTICE` & `aacommons-0.2.8/NOTICE`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/__init__.py` & `aacommons-0.2.8/aacommons/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/contentprovider/ContentProvider.py` & `aacommons-0.2.8/aacommons/contentprovider/ContentProvider.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/contentprovider/RedisStore.py` & `aacommons-0.2.8/aacommons/contentprovider/RedisStore.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/contentprovider/__init__.py` & `aacommons-0.2.8/aacommons/contentprovider/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/contentprovider/util.py` & `aacommons-0.2.8/aacommons/contentprovider/util.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/AirRecorder.py` & `aacommons-0.2.8/aacommons/dataparser/AirRecorder.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/__init__.py` & `aacommons-0.2.8/aacommons/dataparser/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/AbstractTableParser.py` & `aacommons-0.2.8/aacommons/dataparser/cli/AbstractTableParser.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/CliParser.py` & `aacommons-0.2.8/aacommons/dataparser/cli/CliParser.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/CliParserBase.py` & `aacommons-0.2.8/aacommons/dataparser/cli/CliParserBase.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/GenericJsonCsvTableParser.py` & `aacommons-0.2.8/aacommons/dataparser/cli/GenericJsonCsvTableParser.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/GenericRegexTableParser.py` & `aacommons-0.2.8/aacommons/dataparser/cli/GenericRegexTableParser.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParser.py` & `aacommons-0.2.8/aacommons/dataparser/cli/RowColumnTableParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 '''
 
 import logging
 import re
 from .AbstractTableParser import AbstractTableParser
 from .GenericJsonCsvTableParser import GenericJsonCsvTableParser
 from .GenericRegexTableParser import GenericRegexTableParser
+from .RowColumnTableParserAcxStd import RowColumnTableParserAcxStd
 from .RowColumnTableParserAosDpStd import RowColumnTableParserAosDpStd
 from .RowColumnTableParserAosSmart import RowColumnTableParserAosSmart
 from .RowColumnTableParserAosStd import RowColumnTableParserAosStd
 
 
 # Logger
 log = logging.getLogger(__name__)
@@ -87,14 +88,17 @@
 
         elif parserName == "generic-regex":
             self.parser = GenericRegexTableParser(source, tableOptions)
 
         elif parserName == "generic-json-csv":
             self.parser = GenericJsonCsvTableParser(source, tableOptions)
 
+        elif parserName == "acx-std":
+            self.parser = RowColumnTableParserAcxStd(source, tableOptions)
+
         else:
             raise Exception("unknown table parser: " + parserName)
 
     def process(self):
         self.parser.process()
 
     def getTables(self):
```

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosDpStd.py` & `aacommons-0.2.8/aacommons/dataparser/cli/RowColumnTableParserAosDpStd.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosSmart.py` & `aacommons-0.2.8/aacommons/dataparser/cli/RowColumnTableParserAosSmart.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/RowColumnTableParserAosStd.py` & `aacommons-0.2.8/aacommons/dataparser/cli/RowColumnTableParserAosStd.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/TableHelpers.py` & `aacommons-0.2.8/aacommons/dataparser/cli/TableHelpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,26 +42,28 @@
 
 TABLE OPTIONS
 -------------
 Dictionary that contains common table options and parser specific table options.
 The table parser MUST always be specified.
 
 {
-   "parser": "aos-std|aos-dp-std|aos-smart|generic-regex|generic-json-csv"
+   "parser": "acx-std|aos-std|aos-dp-std|aos-smart|generic-regex|generic-json-csv"
    [, "begin": "<begin>" ]
    [, "data.trim": false|true ]
    [, "end": "<end>" ]
    [, "json.lines": "<key>" ]
    [, "marker": "<marker>" ]
    [, <parser specific table options> ]
 }
 
 TABLE PARSERS
 -------------
 Following table parsers are available (key 'parser'):
+- "acx-std": understands standard ACX table output such as "show vlan",
+             "show interface link-status", "show environment power-supply", etc...
 - "aos-std": understands standard AOS table output such as "show ap active",
              "show user", "show ap bss-table", etc...
 - "aos-dp-std": understands standard AOS datapath table output such as
                 "show datapath tunnel table", etc...
 - "aos-smart": understands "smart" AOS table output such as
                 "show datapath tunnel smart", etc...
 - "generic-regex": generic regular expression based table parser.
@@ -90,14 +92,23 @@
 - "json.lines": "<key>". By default input is assumed to be text. When "json.lines" is specified, input is expected
                 to be a JSON object where the "json.lines" provided key specifies an array of text lines, such as:
                 { "_data": [ "line1", "line2", "line3" ] } (i.e. "json.lines": "_data")
                 Default: None
 - "data.trim": true|false. When true, all table values have beginning and ending white-spaces trimmed.
                Default: true
 
+acx-std TABLE PARSER OPTIONS
+----------------------------
+- "marker": "<marker>". header marker. Default "--------".
+                        The first marker signals the begin of the table header and is optional.
+                        The second marker is required and signals the end of the table header.
+- "marker.search.lines": "<# lines to search>". Provide number of lines to search for marker. Default 10.
+- "stop.on.empty.line": true or false, defaults to true. When true, parsers stops on first
+                        blank/empty line.
+
 aos-std TABLE PARSER OPTIONS
 ----------------------------
 - "marker.search.lines": "<# lines to search>". Provide number of lines to search for marker. Default 10.
 - "marker.table.offset": "<# lines>". Number of lines between marker and start of a table header (row of -----). Default 2.
 
 aos-dp-std TABLE PARSER OPTIONS
 -------------------------------
```

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/__init__.py` & `aacommons-0.2.8/aacommons/dataparser/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliContentProvider.py` & `aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliContentProvider.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliContext.py` & `aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliContext.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliDocuments.py` & `aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliDocuments.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliParser.py` & `aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliParser.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliParserRequest.py` & `aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliParserRequest.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliResult.py` & `aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliResult.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/arcli/ArCliSampleRunner.py` & `aacommons-0.2.8/aacommons/dataparser/cli/arcli/ArCliSampleRunner.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 #
 
 '''
 #
 # ARCLI sample runner.
 #
-# Authors: Thomas Bastian
+# Authors: Thomas Bastian, Jeff Goff
 #
 '''
 
 '''
 # Parameters
 '''
 '''
@@ -31,14 +31,15 @@
 
 import argparse
 import logging.config
 import json
 import os
 import sys
 import time
+from aacommons.dataparser.AirRecorder import LogFileReaderGenerator
 from aacommons.dataparser.cli.CliParser import CliParserFactory
 from aacommons.dataparser.cli.arcli.ArCliParserRequest import ArCliParserRequest
 from aacommons.dataparser.cli.arcli.ArCliContentProvider import ArCliContentProvider
 
 
 LOGGING_CONFIG = {
     'version': 1,
@@ -121,49 +122,76 @@
         print(indent, command)
         for rd in resultData:
             printResult(rd, indent + "  ")
     else:
         raise Exception("not a tuple or list")
 
 
-def parseContent(documents, label, command, content, toStdout=True, outputFormat="text", **kwargs):
+def parseContent(documents, label, command, content, arlog, toStdout=True, outputFormat="text", **kwargs):
     devMode = kwargs.get('dev', False)
     dos2unix = kwargs.get('dos2unix', False)
 
     # notify
     if devMode:
         print("Dev mode is on, exceptions will raise")
 
     # Instantiate parser
     contentProvider = ArCliContentProvider(documents)
     cliParser = CliParserFactory.getParser("ARCLI", arCliConfig=contentProvider)
 
-    # Load content
-    f = open(content, 'r', encoding='utf8', errors='ignore')
-    content = f.read()
-    f.close()
-
-    if dos2unix:
-        # clean up files that have Windows line endings and other oddities
-        content = content.replace('\r', '')
-        content = content.replace('^M', '')
-
-    # Parse
-    parserRequest = ArCliParserRequest()
-    parserRequest['Source'] = "me"
-    parserRequest['Command'] = command
-    parserRequest['Stdout'] = content
-    parserRequest['Label'] = label
-    parserRequest['LocalBeginTime'] = time.time()
-    # raiseOnException=True to avoid silently consuming exceptions
-    # which is useful if we are poking around in the guts of aacommons
-    parserRequest['_raiseOnException'] = devMode
-    parserRequest['_raiseOnNocliCommandDef'] = devMode
-    r = cliParser.parse(parserRequest)
+    if arlog is not None:
+        # AirRecorder log file
+        outputResults = ""
+        results = LogFileReaderGenerator(arlog)
+        for result in results:
+            # Parse
+            if result.getQuery().getCommand() is None:
+                continue
+            parserRequest = ArCliParserRequest()
+            parserRequest['Source'] = "me"
+            parserRequest['Command'] = result.getQuery().getCommand()
+            parserRequest['Stdout'] = result.getStdout()
+            parserRequest['Label'] = label
+            parserRequest['LocalBeginTime'] = result.getLocalBeginTime()
+            # raiseOnException=True to avoid silently consuming exceptions
+            # which is useful if we are poking around in the guts of aacommons
+            parserRequest['_raiseOnException'] = devMode
+            parserRequest['_raiseOnNocliCommandDef'] = devMode
+            r = cliParser.parse(parserRequest)
+            o = outputResult(r, toStdout, outputFormat)
+            outputResults += str(o) + "\n"
+        return outputResults
 
+    else:
+        # Plain CLI output
+        f = open(content, 'r', encoding='utf8', errors='ignore')
+        content = f.read()
+        f.close()
+    
+        if dos2unix:
+            # clean up files that have Windows line endings and other oddities
+            content = content.replace('\r', '')
+            content = content.replace('^M', '')
+
+        # Parse
+        parserRequest = ArCliParserRequest()
+        parserRequest['Source'] = "me"
+        parserRequest['Command'] = command
+        parserRequest['Stdout'] = content
+        parserRequest['Label'] = label
+        parserRequest['LocalBeginTime'] = time.time()
+        # raiseOnException=True to avoid silently consuming exceptions
+        # which is useful if we are poking around in the guts of aacommons
+        parserRequest['_raiseOnException'] = devMode
+        parserRequest['_raiseOnNocliCommandDef'] = devMode
+        r = cliParser.parse(parserRequest)
+        return outputResult(r, toStdout, outputFormat)
+
+
+def outputResult(r, toStdout, outputFormat):
     if not toStdout:
         # caller wants the output for their own usage and/or want to silence stdout
         # take into account any requested outputFormats
         return formatAsJson(r, outputFormat, default=r)
 
     # Print results
     if r is None:
@@ -185,16 +213,20 @@
         self.p = p
 
         o = p.add_argument_group('Input Options')
         o.add_argument('-d', '--doc', help='Document file, default is ./arcli.json', default='arcli.json', metavar='FILENAME')
 
         labels = ['AOS', 'IAP', 'ACX', 'ASW', 'COMWARE']
         o.add_argument('-l', '--label', help=f'Document label, one of {", ".join(labels)}', choices=labels, metavar='LABEL', required=True)
-        o.add_argument('-c', '--cmd', help='Command to parse', metavar="CMD", required=True)
-        o.add_argument('-i', '--infile', help='Input file containing the device output', metavar='FILENAME', required=True)
+        # Two combinations are supported:
+        # --cmd --infile
+        # --arlog
+        o.add_argument('-c', '--cmd', help='Command to parse', metavar="CMD", required=False)
+        o.add_argument('-i', '--infile', help='Input file containing the raw device output', metavar='FILENAME', required=False)
+        o.add_argument('--arlog', help='AirRecorder log file containing the device output', metavar='FILENAME', required=False)
 
         o = p.add_argument_group('Output Options')
         o.add_argument('--json', help='Output will be formatted as JSON', action='store_true')
         o.add_argument('--jsonl', help='Output will be formatted as JSONL (one JSON record per line)', action='store_true')
         o.add_argument('-o', '--outfile', help='Write output to specified filename (instead of stdout)', default=None, metavar='FILENAME')
         o.add_argument('-n', '--no-stdout', help='Don\'t write output to stdout', action='store_true')
         
@@ -209,25 +241,32 @@
             if msg:
                 print('\n' + msg + '\n')
             self.p.print_help()
             sys.exit()
 
         args = self.p.parse_args()
 
-        if args.label is None and args.cmd is None and args.infile is None:
+        if args.label is None and args.cmd is None and args.infile is None and args.arlog is None:
             # catch the case of the script being run with no args before
             # any error about -d/--doc is thrown
             help_exit()
 
+        if args.arlog is not None and (args.cmd is not None or args.infile is not None):
+            help_exit(f'Error: --arlog cannot be combined with --cmd and/or --infile')
+        if args.arlog is None and (args.cmd is None or args.infile is None):
+            help_exit(f'Error: --cmd and --infile are required')
+
         # check provided files exists
         if not os.path.exists(args.doc):
             help_exit(f'Error: -d/--doc {args.doc} does not exist')
         
-        if not os.path.exists(args.infile):
+        if args.infile is not None and not os.path.exists(args.infile):
             help_exit(f'Error: -i/--infile {args.infile} does not exist')
+        if args.arlog is not None and not os.path.exists(args.arlog):
+            help_exit(f'Error: --arlog {args.arlog} does not exist')
 
         # setup the output format
         if args.json:
             args.outputFormat = 'json'
         elif args.jsonl:
             args.outputFormat = 'jsonl'
         else:
@@ -242,15 +281,15 @@
 
 if __name__ == '__main__':
 
     args = CLI().parse()
 
     if args.outfile:
         with open(args.outfile, 'w') as f:
-            f.write(str(parseContent(args.doc, args.label, args.cmd, args.infile, 
+            f.write(str(parseContent(args.doc, args.label, args.cmd, args.infile, args.arlog,
                                      toStdout=False, outputFormat=args.outputFormat, 
                                      dev=args.dev, dos2unix=args.dos2unix)))
         print(f'Script output written to {args.outfile}')
     else:
-        parseContent(args.doc, args.label, args.cmd, args.infile, 
+        parseContent(args.doc, args.label, args.cmd, args.infile, args.arlog,
                      toStdout=not args.no_stdout, outputFormat=args.outputFormat, 
                      dev=args.dev, dos2unix=args.dos2unix)
```

### Comparing `aacommons-0.2.7/aacommons/dataparser/cli/arcli/__init__.py` & `aacommons-0.2.8/aacommons/dataparser/cli/arcli/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/helpers/__init__.py` & `aacommons-0.2.8/aacommons/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/helpers/get_my_ip.py` & `aacommons-0.2.8/aacommons/helpers/get_my_ip.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/helpers/jstyleson_lint.py` & `aacommons-0.2.8/aacommons/helpers/jstyleson_lint.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/misc/Stats.py` & `aacommons-0.2.8/aacommons/misc/Stats.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons/misc/__init__.py` & `aacommons-0.2.8/aacommons/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `aacommons-0.2.7/aacommons.egg-info/SOURCES.txt` & `aacommons-0.2.8/aacommons.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 aacommons/dataparser/__init__.py
 aacommons/dataparser/cli/AbstractTableParser.py
 aacommons/dataparser/cli/CliParser.py
 aacommons/dataparser/cli/CliParserBase.py
 aacommons/dataparser/cli/GenericJsonCsvTableParser.py
 aacommons/dataparser/cli/GenericRegexTableParser.py
 aacommons/dataparser/cli/RowColumnTableParser.py
+aacommons/dataparser/cli/RowColumnTableParserAcxStd.py
 aacommons/dataparser/cli/RowColumnTableParserAosDpStd.py
 aacommons/dataparser/cli/RowColumnTableParserAosSmart.py
 aacommons/dataparser/cli/RowColumnTableParserAosStd.py
 aacommons/dataparser/cli/TableHelpers.py
 aacommons/dataparser/cli/__init__.py
 aacommons/dataparser/cli/arcli/ArCliContentProvider.py
 aacommons/dataparser/cli/arcli/ArCliContext.py
@@ -34,11 +35,8 @@
 aacommons/dataparser/cli/arcli/ArCliResult.py
 aacommons/dataparser/cli/arcli/ArCliSampleRunner.py
 aacommons/dataparser/cli/arcli/__init__.py
 aacommons/helpers/__init__.py
 aacommons/helpers/get_my_ip.py
 aacommons/helpers/jstyleson_lint.py
 aacommons/misc/Stats.py
-aacommons/misc/__init__.py
-tests/test_dataparser_airrecorder.py
-tests/test_dataparser_cli.py
-tests/test_table_helpers.py
+aacommons/misc/__init__.py
```

### Comparing `aacommons-0.2.7/setup.py` & `aacommons-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open('README.rst', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='aacommons',
-    version='0.2.7',
+    version='0.2.8',
     description='aacommons',
     long_description=readme,
     long_description_content_type='text/x-rst',
     author='Thomas Bastian, Jeffrey Goff, Albert Pang',
     url='',
     test_suite="tests",
     packages=find_packages(exclude=('tests', 'docs')),
```

