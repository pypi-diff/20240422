# Comparing `tmp/NiceFlow-0.0.4-py3-none-any.whl.zip` & `tmp/NiceFlow-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,29 @@
-Zip file size: 95899 bytes, number of entries: 135
+Zip file size: 101517 bytes, number of entries: 142
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 NiceFlow/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 NiceFlow/cli/__init__.py
--rw-rw-rw-  2.0 fat     7129 b- defN 24-Feb-01 13:45 NiceFlow/cli/cli.py
+-rw-rw-rw-  2.0 fat     8890 b- defN 24-Feb-16 13:38 NiceFlow/cli/cli.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 NiceFlow/cluster/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 NiceFlow/cluster/master.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 NiceFlow/cluster/operator.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 NiceFlow/cluster/worker.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 NiceFlow/common/__init__.py
 -rw-rw-rw-  2.0 fat     8764 b- defN 23-Dec-25 14:14 NiceFlow/common/ftp_util.py
 -rw-rw-rw-  2.0 fat     1358 b- defN 23-Nov-23 02:04 NiceFlow/common/hdfs_util.py
--rw-rw-rw-  2.0 fat      238 b- defN 24-Jan-30 06:42 NiceFlow/common/module_util.py
+-rw-rw-rw-  2.0 fat      236 b- defN 24-Apr-02 10:31 NiceFlow/common/module_util.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 NiceFlow/core/__init__.py
 -rw-rw-rw-  2.0 fat      813 b- defN 23-Nov-15 14:38 NiceFlow/core/db_logging_handler.py
 -rw-rw-rw-  2.0 fat      244 b- defN 23-Nov-15 14:38 NiceFlow/core/db_plugin.py
 -rw-rw-rw-  2.0 fat     4284 b- defN 24-Jan-29 08:16 NiceFlow/core/flow.py
 -rw-rw-rw-  2.0 fat      127 b- defN 23-Nov-15 14:38 NiceFlow/core/flow_log.py
 -rw-rw-rw-  2.0 fat      130 b- defN 23-Nov-15 14:38 NiceFlow/core/flow_log_handler.py
+-rw-rw-rw-  2.0 fat       72 b- defN 24-Apr-02 10:34 NiceFlow/core/functions.py
 -rw-rw-rw-  2.0 fat     6517 b- defN 23-Dec-19 06:32 NiceFlow/core/manager.py
 -rw-rw-rw-  2.0 fat     2939 b- defN 23-Nov-15 14:38 NiceFlow/core/mysqldb_logging_handler.py
--rw-rw-rw-  2.0 fat     4024 b- defN 24-Jan-25 02:56 NiceFlow/core/plugin.py
+-rw-rw-rw-  2.0 fat     4188 b- defN 24-Apr-10 14:25 NiceFlow/core/plugin.py
 -rw-rw-rw-  2.0 fat     1755 b- defN 23-Nov-15 14:38 NiceFlow/core/plugin_field.py
 -rw-rw-rw-  2.0 fat      123 b- defN 23-Nov-15 14:38 NiceFlow/core/plugin_log.py
 -rw-rw-rw-  2.0 fat     1214 b- defN 23-Nov-15 14:38 NiceFlow/core/plugin_time_record.py
 -rw-rw-rw-  2.0 fat      811 b- defN 23-Nov-15 14:38 NiceFlow/core/states.py
 -rw-rw-rw-  2.0 fat     2288 b- defN 24-Jan-23 07:08 NiceFlow/core/tool.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 NiceFlow/core/exception/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 NiceFlow/core/exception/flow_exception.py
@@ -31,107 +32,113 @@
 -rw-rw-rw-  2.0 fat     1825 b- defN 23-Nov-15 14:38 NiceFlow/core/utils/encrypt_data.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-29 08:06 NiceFlow/log/__init__.py
 -rw-rw-rw-  2.0 fat      127 b- defN 23-Nov-15 14:38 NiceFlow/log/flow_log.py
 -rw-rw-rw-  2.0 fat      130 b- defN 23-Nov-15 14:38 NiceFlow/log/flow_log_handler.py
 -rw-rw-rw-  2.0 fat     2937 b- defN 24-Jan-29 08:08 NiceFlow/log/mysqldb_logging_handler.py
 -rw-rw-rw-  2.0 fat      123 b- defN 23-Nov-15 14:38 NiceFlow/log/plugin_log.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 NiceFlow/plugins/__init__.py
+-rw-rw-rw-  2.0 fat     1310 b- defN 24-Apr-02 10:37 NiceFlow/plugins/add_field.py
+-rw-rw-rw-  2.0 fat      956 b- defN 24-Mar-11 15:31 NiceFlow/plugins/agg.py
 -rw-rw-rw-  2.0 fat     1110 b- defN 23-Nov-15 14:38 NiceFlow/plugins/akshare_input.py
 -rw-rw-rw-  2.0 fat     1164 b- defN 23-Dec-09 04:33 NiceFlow/plugins/ck_input.py
 -rw-rw-rw-  2.0 fat     1678 b- defN 23-Dec-09 04:33 NiceFlow/plugins/ck_output.py
--rw-rw-rw-  2.0 fat      665 b- defN 23-Nov-28 13:47 NiceFlow/plugins/console.py
+-rw-rw-rw-  2.0 fat      665 b- defN 24-Feb-20 03:35 NiceFlow/plugins/console.py
 -rw-rw-rw-  2.0 fat     1168 b- defN 23-Dec-09 04:33 NiceFlow/plugins/cos_input.py
 -rw-rw-rw-  2.0 fat     1172 b- defN 23-Dec-09 04:33 NiceFlow/plugins/cos_output.py
--rw-rw-rw-  2.0 fat      762 b- defN 24-Jan-03 14:14 NiceFlow/plugins/csv_input.py
--rw-rw-rw-  2.0 fat      637 b- defN 23-Nov-15 14:38 NiceFlow/plugins/csv_output.py
+-rw-rw-rw-  2.0 fat     1440 b- defN 24-Apr-16 08:28 NiceFlow/plugins/csv_input.py
+-rw-rw-rw-  2.0 fat      636 b- defN 24-Apr-12 10:04 NiceFlow/plugins/csv_output.py
 -rw-rw-rw-  2.0 fat     1168 b- defN 23-Dec-09 04:33 NiceFlow/plugins/db2_input.py
 -rw-rw-rw-  2.0 fat     1172 b- defN 23-Dec-09 04:33 NiceFlow/plugins/db2_output.py
 -rw-rw-rw-  2.0 fat     1007 b- defN 23-Dec-25 13:32 NiceFlow/plugins/db_execute.py
 -rw-rw-rw-  2.0 fat      716 b- defN 24-Jan-19 12:24 NiceFlow/plugins/duckdb_input.py
 -rw-rw-rw-  2.0 fat      779 b- defN 24-Jan-03 14:14 NiceFlow/plugins/duckdb_output.py
 -rw-rw-rw-  2.0 fat     1288 b- defN 23-Dec-05 04:58 NiceFlow/plugins/duplicate.py
 -rw-rw-rw-  2.0 fat      547 b- defN 23-Dec-06 13:10 NiceFlow/plugins/email.py
--rw-rw-rw-  2.0 fat     1164 b- defN 23-Dec-09 04:33 NiceFlow/plugins/es_input.py
--rw-rw-rw-  2.0 fat     1678 b- defN 23-Dec-09 04:33 NiceFlow/plugins/es_output.py
+-rw-rw-rw-  2.0 fat     1415 b- defN 24-Feb-19 08:03 NiceFlow/plugins/es_input.py
+-rw-rw-rw-  2.0 fat     1491 b- defN 24-Feb-19 07:54 NiceFlow/plugins/es_output.py
 -rw-rw-rw-  2.0 fat      800 b- defN 23-Dec-05 09:44 NiceFlow/plugins/excel_input.py
 -rw-rw-rw-  2.0 fat      954 b- defN 24-Jan-29 07:17 NiceFlow/plugins/excel_output.py
--rw-rw-rw-  2.0 fat     1820 b- defN 23-Dec-06 13:32 NiceFlow/plugins/faker_input.py
+-rw-rw-rw-  2.0 fat     1197 b- defN 24-Feb-20 07:06 NiceFlow/plugins/faker_input.py
 -rw-rw-rw-  2.0 fat      809 b- defN 23-Dec-25 13:32 NiceFlow/plugins/filter.py
 -rw-rw-rw-  2.0 fat     2385 b- defN 24-Jan-25 02:59 NiceFlow/plugins/for.py
--rw-rw-rw-  2.0 fat      699 b- defN 23-Dec-25 14:17 NiceFlow/plugins/ftp_input.py
+-rw-rw-rw-  2.0 fat      623 b- defN 24-Mar-12 05:56 NiceFlow/plugins/ftp_input.py
 -rw-rw-rw-  2.0 fat     1172 b- defN 23-Dec-09 04:33 NiceFlow/plugins/ftp_output.py
+-rw-rw-rw-  2.0 fat     1718 b- defN 24-Apr-15 14:26 NiceFlow/plugins/function.py
 -rw-rw-rw-  2.0 fat     1017 b- defN 24-Jan-24 04:11 NiceFlow/plugins/hdfs_input.py
 -rw-rw-rw-  2.0 fat     2302 b- defN 24-Jan-25 03:08 NiceFlow/plugins/hdfs_output.py
 -rw-rw-rw-  2.0 fat      651 b- defN 23-Nov-15 14:38 NiceFlow/plugins/hive_input.py
 -rw-rw-rw-  2.0 fat      642 b- defN 23-Nov-15 14:38 NiceFlow/plugins/hive_output.py
 -rw-rw-rw-  2.0 fat      568 b- defN 23-Nov-15 14:38 NiceFlow/plugins/html_output.py
 -rw-rw-rw-  2.0 fat     1174 b- defN 23-Dec-09 04:33 NiceFlow/plugins/html_parse_input.py
 -rw-rw-rw-  2.0 fat     1672 b- defN 23-Nov-15 14:38 NiceFlow/plugins/http_input.py
 -rw-rw-rw-  2.0 fat     1742 b- defN 23-Nov-15 14:38 NiceFlow/plugins/http_output.py
 -rw-rw-rw-  2.0 fat     1414 b- defN 23-Nov-15 14:38 NiceFlow/plugins/if.py
 -rw-rw-rw-  2.0 fat      494 b- defN 23-Nov-15 14:38 NiceFlow/plugins/join.py
--rw-rw-rw-  2.0 fat      654 b- defN 23-Nov-15 14:38 NiceFlow/plugins/kafka_input.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 24-Apr-07 08:20 NiceFlow/plugins/kafka_input.py
 -rw-rw-rw-  2.0 fat      659 b- defN 23-Nov-15 14:38 NiceFlow/plugins/kafka_output.py
 -rw-rw-rw-  2.0 fat     3159 b- defN 23-Nov-27 16:32 NiceFlow/plugins/mapping.py
 -rw-rw-rw-  2.0 fat      708 b- defN 24-Jan-29 07:17 NiceFlow/plugins/markdown_output.py
 -rw-rw-rw-  2.0 fat     1385 b- defN 23-Nov-15 14:38 NiceFlow/plugins/mask.py
--rw-rw-rw-  2.0 fat      631 b- defN 23-Nov-15 14:38 NiceFlow/plugins/mongo_input.py
+-rw-rw-rw-  2.0 fat      689 b- defN 24-Feb-19 08:28 NiceFlow/plugins/mongo_input.py
 -rw-rw-rw-  2.0 fat      825 b- defN 23-Nov-15 14:38 NiceFlow/plugins/mongo_output.py
--rw-rw-rw-  2.0 fat     1606 b- defN 24-Jan-29 07:46 NiceFlow/plugins/mqtt_input.py
+-rw-rw-rw-  2.0 fat     2594 b- defN 24-Mar-31 08:43 NiceFlow/plugins/mqtt_input.py
 -rw-rw-rw-  2.0 fat     1442 b- defN 23-Nov-15 14:38 NiceFlow/plugins/mqtt_output.py
 -rw-rw-rw-  2.0 fat     2313 b- defN 24-Jan-24 09:30 NiceFlow/plugins/mysql_input.py
 -rw-rw-rw-  2.0 fat     3883 b- defN 24-Jan-04 14:08 NiceFlow/plugins/mysql_output.py
 -rw-rw-rw-  2.0 fat     1112 b- defN 23-Dec-04 15:11 NiceFlow/plugins/odps_input.py
 -rw-rw-rw-  2.0 fat     1400 b- defN 23-Nov-20 08:47 NiceFlow/plugins/odps_output.py
 -rw-rw-rw-  2.0 fat     1257 b- defN 23-Dec-25 13:32 NiceFlow/plugins/oracle_input.py
 -rw-rw-rw-  2.0 fat     1460 b- defN 23-Nov-23 03:01 NiceFlow/plugins/oracle_output.py
 -rw-rw-rw-  2.0 fat      659 b- defN 23-Nov-15 14:38 NiceFlow/plugins/paimon_input.py
 -rw-rw-rw-  2.0 fat      666 b- defN 23-Nov-15 14:38 NiceFlow/plugins/paimon_output.py
 -rw-rw-rw-  2.0 fat      539 b- defN 23-Nov-15 14:38 NiceFlow/plugins/parquet_input.py
 -rw-rw-rw-  2.0 fat      606 b- defN 23-Nov-15 14:38 NiceFlow/plugins/parquet_output.py
--rw-rw-rw-  2.0 fat      525 b- defN 23-Nov-15 14:38 NiceFlow/plugins/pivot.py
+-rw-rw-rw-  2.0 fat      764 b- defN 24-Mar-12 05:54 NiceFlow/plugins/pivot.py
 -rw-rw-rw-  2.0 fat     1262 b- defN 23-Dec-25 13:32 NiceFlow/plugins/postgre_input.py
 -rw-rw-rw-  2.0 fat     1233 b- defN 23-Dec-25 13:32 NiceFlow/plugins/postgre_output.py
 -rw-rw-rw-  2.0 fat      617 b- defN 23-Nov-28 08:40 NiceFlow/plugins/printer.py
 -rw-rw-rw-  2.0 fat     1446 b- defN 23-Nov-15 14:38 NiceFlow/plugins/pulsar_input.py
 -rw-rw-rw-  2.0 fat     1446 b- defN 23-Nov-15 14:38 NiceFlow/plugins/pulsar_output.py
 -rw-rw-rw-  2.0 fat      534 b- defN 23-Nov-15 14:38 NiceFlow/plugins/regular_extract.py
 -rw-rw-rw-  2.0 fat      799 b- defN 23-Nov-15 14:38 NiceFlow/plugins/rename.py
 -rw-rw-rw-  2.0 fat     1164 b- defN 23-Dec-09 04:33 NiceFlow/plugins/s3_input.py
 -rw-rw-rw-  2.0 fat     1168 b- defN 23-Dec-09 04:33 NiceFlow/plugins/s3_output.py
 -rw-rw-rw-  2.0 fat      796 b- defN 23-Nov-15 14:38 NiceFlow/plugins/samples.py
 -rw-rw-rw-  2.0 fat      915 b- defN 23-Dec-08 03:25 NiceFlow/plugins/sequence.py
 -rw-rw-rw-  2.0 fat      947 b- defN 23-Nov-15 14:38 NiceFlow/plugins/sort.py
 -rw-rw-rw-  2.0 fat      879 b- defN 23-Dec-25 13:32 NiceFlow/plugins/spider.py
+-rw-rw-rw-  2.0 fat     1018 b- defN 24-Mar-31 12:29 NiceFlow/plugins/split_field_to_rows.py
 -rw-rw-rw-  2.0 fat      861 b- defN 24-Jan-19 10:00 NiceFlow/plugins/sql.py
 -rw-rw-rw-  2.0 fat     1160 b- defN 23-Nov-23 01:44 NiceFlow/plugins/sqlserver_input.py
 -rw-rw-rw-  2.0 fat     1184 b- defN 23-Nov-23 01:44 NiceFlow/plugins/sqlserver_output.py
 -rw-rw-rw-  2.0 fat      463 b- defN 23-Nov-15 14:38 NiceFlow/plugins/starter.py
 -rw-rw-rw-  2.0 fat      544 b- defN 23-Nov-15 14:38 NiceFlow/plugins/sub_flow.py
 -rw-rw-rw-  2.0 fat      511 b- defN 23-Nov-15 14:38 NiceFlow/plugins/switch.py
 -rw-rw-rw-  2.0 fat     2759 b- defN 23-Dec-25 13:32 NiceFlow/plugins/table_schema_convert.py
 -rw-rw-rw-  2.0 fat      533 b- defN 23-Nov-15 14:38 NiceFlow/plugins/unpivot.py
 -rw-rw-rw-  2.0 fat      692 b- defN 23-Nov-15 14:38 NiceFlow/plugins/variable.py
 -rw-rw-rw-  2.0 fat     1424 b- defN 23-Nov-15 14:38 NiceFlow/plugins/while.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-16 14:16 NiceFlow/server/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-15 14:38 test/__init__.py
 -rw-rw-rw-  2.0 fat     5586 b- defN 23-Dec-29 09:32 test/a_test.py
 -rw-rw-rw-  2.0 fat     2142 b- defN 24-Jan-30 06:55 test/base_test.py
 -rw-rw-rw-  2.0 fat     1079 b- defN 23-Nov-15 14:38 test/binlog_test.py
 -rw-rw-rw-  2.0 fat     2726 b- defN 23-Dec-06 15:53 test/connectx_test.py
 -rw-rw-rw-  2.0 fat     4690 b- defN 23-Nov-15 14:38 test/dt_test.py
 -rw-rw-rw-  2.0 fat     3437 b- defN 24-Jan-23 10:29 test/duckdb_test.py
--rw-rw-rw-  2.0 fat     1809 b- defN 24-Jan-29 08:07 test/flow_test.py
+-rw-rw-rw-  2.0 fat     1813 b- defN 24-Feb-20 03:05 test/flow_test.py
 -rw-rw-rw-  2.0 fat      907 b- defN 23-Dec-25 14:17 test/ftp_test.py
 -rw-rw-rw-  2.0 fat      298 b- defN 23-Nov-15 14:38 test/git_test.py
+-rw-rw-rw-  2.0 fat     1236 b- defN 24-Feb-02 09:06 test/pandas_test.py
 -rw-rw-rw-  2.0 fat     2672 b- defN 23-Nov-20 02:42 test/plugin_input_test.py
 -rw-rw-rw-  2.0 fat     2388 b- defN 23-Dec-06 14:20 test/plugin_output_test.py
 -rw-rw-rw-  2.0 fat     4318 b- defN 23-Dec-07 07:27 test/plugin_transform.py
 -rw-rw-rw-  2.0 fat     1070 b- defN 23-Dec-09 04:29 test/real_test.py
 -rw-rw-rw-  2.0 fat     1626 b- defN 24-Jan-24 03:11 test/sqlglot_test.py
 -rw-rw-rw-  2.0 fat     1280 b- defN 23-Nov-15 14:38 test/uuid_test.py
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Feb-01 13:45 NiceFlow-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9420 b- defN 24-Feb-01 13:45 NiceFlow-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-01 13:45 NiceFlow-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 24-Feb-01 13:45 NiceFlow-0.0.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       14 b- defN 24-Feb-01 13:45 NiceFlow-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    11367 b- defN 24-Feb-01 13:45 NiceFlow-0.0.4.dist-info/RECORD
-135 files, 203445 bytes uncompressed, 77967 bytes compressed:  61.7%
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-22 03:14 NiceFlow-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11804 b- defN 24-Apr-22 03:14 NiceFlow-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-22 03:14 NiceFlow-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 24-Apr-22 03:14 NiceFlow-0.0.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-22 03:14 NiceFlow-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    11954 b- defN 24-Apr-22 03:14 NiceFlow-0.0.5.dist-info/RECORD
+142 files, 216819 bytes uncompressed, 82671 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -45,14 +45,17 @@
 
 Filename: NiceFlow/core/flow_log.py
 Comment: 
 
 Filename: NiceFlow/core/flow_log_handler.py
 Comment: 
 
+Filename: NiceFlow/core/functions.py
+Comment: 
+
 Filename: NiceFlow/core/manager.py
 Comment: 
 
 Filename: NiceFlow/core/mysqldb_logging_handler.py
 Comment: 
 
 Filename: NiceFlow/core/plugin.py
@@ -102,14 +105,20 @@
 
 Filename: NiceFlow/log/plugin_log.py
 Comment: 
 
 Filename: NiceFlow/plugins/__init__.py
 Comment: 
 
+Filename: NiceFlow/plugins/add_field.py
+Comment: 
+
+Filename: NiceFlow/plugins/agg.py
+Comment: 
+
 Filename: NiceFlow/plugins/akshare_input.py
 Comment: 
 
 Filename: NiceFlow/plugins/ck_input.py
 Comment: 
 
 Filename: NiceFlow/plugins/ck_output.py
@@ -174,14 +183,17 @@
 
 Filename: NiceFlow/plugins/ftp_input.py
 Comment: 
 
 Filename: NiceFlow/plugins/ftp_output.py
 Comment: 
 
+Filename: NiceFlow/plugins/function.py
+Comment: 
+
 Filename: NiceFlow/plugins/hdfs_input.py
 Comment: 
 
 Filename: NiceFlow/plugins/hdfs_output.py
 Comment: 
 
 Filename: NiceFlow/plugins/hive_input.py
@@ -303,14 +315,17 @@
 
 Filename: NiceFlow/plugins/sort.py
 Comment: 
 
 Filename: NiceFlow/plugins/spider.py
 Comment: 
 
+Filename: NiceFlow/plugins/split_field_to_rows.py
+Comment: 
+
 Filename: NiceFlow/plugins/sql.py
 Comment: 
 
 Filename: NiceFlow/plugins/sqlserver_input.py
 Comment: 
 
 Filename: NiceFlow/plugins/sqlserver_output.py
@@ -333,14 +348,17 @@
 
 Filename: NiceFlow/plugins/variable.py
 Comment: 
 
 Filename: NiceFlow/plugins/while.py
 Comment: 
 
+Filename: NiceFlow/server/__init__.py
+Comment: 
+
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/a_test.py
 Comment: 
 
 Filename: test/base_test.py
@@ -363,14 +381,17 @@
 
 Filename: test/ftp_test.py
 Comment: 
 
 Filename: test/git_test.py
 Comment: 
 
+Filename: test/pandas_test.py
+Comment: 
+
 Filename: test/plugin_input_test.py
 Comment: 
 
 Filename: test/plugin_output_test.py
 Comment: 
 
 Filename: test/plugin_transform.py
@@ -381,26 +402,26 @@
 
 Filename: test/sqlglot_test.py
 Comment: 
 
 Filename: test/uuid_test.py
 Comment: 
 
-Filename: NiceFlow-0.0.4.dist-info/LICENSE
+Filename: NiceFlow-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: NiceFlow-0.0.4.dist-info/METADATA
+Filename: NiceFlow-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: NiceFlow-0.0.4.dist-info/WHEEL
+Filename: NiceFlow-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: NiceFlow-0.0.4.dist-info/entry_points.txt
+Filename: NiceFlow-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: NiceFlow-0.0.4.dist-info/top_level.txt
+Filename: NiceFlow-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: NiceFlow-0.0.4.dist-info/RECORD
+Filename: NiceFlow-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## NiceFlow/cli/cli.py

```diff
@@ -39,32 +39,41 @@
 @cli.command('sql', short_help='sql a data ')
 @click.option("--sql_script", default="", help="sql脚本语句，支持多行")
 @click.option("--sql_path", default="", help="sql脚本文件")
 @click.option("--db_path", default="", help="输入duckdb数据库的路径，不存在则为内存模式[可选]")
 @click.option("--res_path", default="", help="输入文件路径，该路径下的文件会被自动加载到db中[可选]")
 @click.option("--function_path", default="", help="输入函数路径，该路径为python文件,可以作为数据库自定义函数使用[可选]")
 @click.option("--result_path", default="", help="输入结果路径,支持csv,json,parquet,txt,excel,clipboard当输入为clipboard时,结果直接写入剪贴板")
+@click.option("--is_overwrite", default="False", help="是否重新加载数据")
+@click.option("--all_varchar", default="", help="是否全为varchar类型")
 def sql(sql_script: str = None, sql_path: str = None, db_path: str = None, res_path: str = None,
-        function_path: str = None, result_path: str = None):
+        function_path: str = None, result_path: str = None, is_overwrite=False, all_varchar=False):
     if db_path:
         con = duckdb.connect(db_path)
     else:
         con = duckdb.connect()
     # 自动加载目录下的res文件
     if res_path:
         for file in os.listdir(res_path):
             table_path = res_path + "/" + file
             if len(file.split(".")) <= 1:
                 continue
             table_name = file.split(".")[0]
             file_suffix = file.split(".")[1]
+
+            # 表存在并且不是覆盖模式，则跳过
+            table_name_result = con.execute(f'''SELECT * FROM sqlite_master WHERE type='table' AND name='{table_name}';''')
+            if is_overwrite is False and len(table_name_result.fetchall()) > 0:
+                continue
+
+            # 表需要重新加载
             if file_suffix.lower() == "csv":
                 con.sql(f'''
                 drop table if EXISTS  {table_name};
-                CREATE TABLE {table_name} AS SELECT * FROM read_csv_auto('{table_path}',header = true);
+                CREATE TABLE {table_name} AS SELECT * FROM read_csv_auto('{table_path}',header = true,ALL_VARCHAR={all_varchar});
                 ''')
             if file_suffix.lower() == "parquet":
                 con.sql(f'''
                 drop table if EXISTS  {table_name};
                 CREATE TABLE {table_name} AS SELECT * FROM read_parquet('{table_path}');
                 ''')
             if file_suffix.lower() == "xlsx":
@@ -75,19 +84,21 @@
                 CREATE TABLE {table_name} AS SELECT * FROM st_read('{table_path}');
                 ''')
             if file_suffix.lower() == "json":
                 con.sql(f'''
                 drop table if EXISTS  {table_name};
                 CREATE TABLE {table_name} AS SELECT * FROM read_json('{table_path}',auto_detect=true);
                 ''')
+    # 加载自定义函数
     if function_path:
         module = load_module(function_path)
         items = inspect.getmembers(module, inspect.isfunction)
         for item in items:
             con.create_function(item[0], item[1])
+    #
     if sql_script:
         duck_df = con.sql(sql_script)
     else:
         with open(sql_path, "r", encoding='utf8') as f:
             duck_df = con.sql(f.read())
 
     if duck_df is not None:
@@ -158,14 +169,50 @@
                     if decrypt is None:
                         return
                     node_properties[key] = decrypt
     with open(path, 'w', encoding='utf8') as fp:
         json.dump(flow_json, fp, indent=2, ensure_ascii=False)
 
 
+
+@cli.command('serve', short_help='启动server服务')
+@click.password_option()
+def serve():
+
+    pass
+
+
+
+@cli.command('client', short_help='客户端可以提交任务到服务端，查看服务端相关内容')
+@click.password_option()
+def decrypt(path: str, password: str):
+    from NiceFlow.core.utils.encrypt_data import EncryptData
+
+    eg = EncryptData(password)
+    with open(path, 'r', encoding='utf8') as fp:
+        flow_json = json.load(fp)
+        nodes_array: json = flow_json["nodes"]
+        # 组装node,edge
+        for node_json in nodes_array:
+            node_properties: json = node_json["properties"]
+            items = node_properties.items()
+            for key, value in items:
+                if key in ["password", "passwd"]:
+                    decrypt_content = re.findall("AES\\((.*)\\)", value)[0]
+                    decrypt = eg.decrypt(decrypt_content)
+                    if decrypt is None:
+                        return
+                    node_properties[key] = decrypt
+    with open(path, 'w', encoding='utf8') as fp:
+        json.dump(flow_json, fp, indent=2, ensure_ascii=False)
+
+
+
+
+
 if __name__ == '__main__':
     sql_script = '''
     select * from total_RQ_DEVICE_20240130;
     '''
     duck_df = sql(sql_script, db_path=None,
                   res_path="C:/Users/xiaow/Desktop/22/test",
                   function_path="C:/Users/xiaow/Desktop/22/test/common_function.py",
```

## NiceFlow/common/module_util.py

```diff
@@ -1,7 +1,6 @@
 import importlib.util
 def load_module(module_path):
     spec = importlib.util.spec_from_file_location("module", module_path)
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     return module
-
```

## NiceFlow/core/plugin.py

```diff
@@ -54,15 +54,14 @@
     def init(self, param: json, flow):
         self.id = param["id"]
         self.type = param["type"]
         self.name = param["name"]
         self.param = param["properties"]
         self.flow = flow
 
-
     def set_result(self, df: duckdb.DuckDBPyRelation = None):
         # 设置结果
         self.df_count = 0 if df is None else len(df)
         # 如果是最后一个节点则将结果信息给到flow
         if len(self.next_nodes) == 0:
             self.flow.set_result(self.name, df)
 
@@ -70,14 +69,19 @@
             node._pre_result_dict[self.name] = df
         # 执行下一步
         for node in self.next_nodes:
             self.signal.connect(node.receiver, sender=self)
         self.after_execute()
         self.signal.send(self)
 
+    # 获取字段信息
+    def query_field(self) -> dict:
+        df: duckdb.DuckDBPyRelation =  self.flow.get_result()[self.name]
+        return df.dtypes
+
     # 关闭资源
     def close(self):
         if self.status != "STOP":
             self.status = "STOP"
             # 执行下一步
             for node in self.next_nodes:
                 node.close()
@@ -116,7 +120,8 @@
     def to_json(self):
         return {
             "name": self.name,
             "id": self.id,
             "type": self.type,
             "properties": self.param
         }
+
```

## NiceFlow/plugins/csv_input.py

```diff
@@ -1,9 +1,11 @@
 import json
 
+import duckdb.duckdb
+
 from NiceFlow.core.flow import Flow
 from NiceFlow.core.plugin import IPlugin
 
 
 class StringConverter(dict):
     def __contains__(self, item):
         return True
@@ -18,16 +20,27 @@
 class CsvInput(IPlugin):
 
     def init(self, param: json, flow: Flow):
         super(CsvInput, self).init(param, flow)
 
     def execute(self):
         super(CsvInput, self).execute()
-        file_name = self.param["file_name"]
-        csv_df = self.flow.con.read_csv(file_name,header=True)
+        filename = self.param["filename"]
+        header = self.param.get("header", True)
+        all_varchar = self.param.get("all_varchar", None)
+        compression = self.param.get("compression", "auto")
+        delimiter = self.param.get("delimiter", ",")
+        names = self.param.get("names", [])
+        sample_size = self.param.get("sample_size", 20480)
+        dtype = self.param.get("dtype", {})
+        encoding = self.param.get("encoding", None)
+        skip = self.param.get("skip", None)
+
+        csv_df = duckdb.read_csv(name=filename, header=header, compression=compression, sep=delimiter, dtype=dtype,
+                                 encoding=encoding, sample_size=sample_size, all_varchar=all_varchar,skiprows=skip, names=names)
         self.set_result(csv_df)
 
     def to_json(self):
         super(CsvInput, self).to_json()
 
     def close(self):
         super(CsvInput, self).close()
```

## NiceFlow/plugins/csv_output.py

```diff
@@ -7,15 +7,15 @@
 class CsvOutput(IPlugin):
 
     def init(self, param: json, flow: Flow):
         super(CsvOutput, self).init(param, flow)
 
     def execute(self):
         super(CsvOutput, self).execute()
-        file_name = self.param["file_name"]
+        file_name = self.param["filename"]
         # 获取上一步结果
         pre_node = self.pre_nodes[0]
         duck_df = self._pre_result_dict[pre_node.name]
         df = duck_df.to_df()
         df.to_csv(file_name, index=False)
 
         self.set_result(None)
```

## NiceFlow/plugins/es_input.py

```diff
@@ -1,39 +1,48 @@
 import json
 
 import duckdb
 import pandas as pd
-from clickhouse_driver import Client
+from elasticsearch import Elasticsearch
 
 from NiceFlow.core.flow import Flow
 from NiceFlow.core.plugin import IPlugin
 
 
 class ESInput(IPlugin):
 
     def init(self, param: json, flow: Flow):
         super(ESInput, self).init(param, flow)
 
     def execute(self):
         super(ESInput, self).execute()
         # param信息
-        host = self.param["host"]
-        port = self.param.get("port", 9000)
-        db = self.param["db"]
-        user = self.param.get("username", "default")
-        password = self.param.get("password", "")
-        table = self.param.get("table", "")
-        sql = self.param.get("sql", "")
+        url = self.param["url"]
+        index = self.param.get("index", "")
+        query = self.param.get("query", "")
+        basic_auth = self.param.get("basic_auth", None)
 
         # 配置数据库
-        client = Client(host=host, port=port, database=db, user=user, password=password)
-
-        # 读取数据
-        data,columns = client.execute(sql,with_column_types=True)
-        real_columns = [item[0] for item in columns]
-        df = pd.DataFrame(data,columns=real_columns)
-        ck_df = duckdb.from_df(df)
+        es = Elasticsearch(hosts=url,basic_auth=basic_auth)
+        res = es.search(index=index, scroll='1m', body=query)
+        sid = res['_scroll_id']
+        scroll_size_max = res['hits']['total']['value']
+        count = 0
+        print(scroll_size_max)
+
+        save_data = []
+        while count < scroll_size_max:
+            for data in res['hits']['hits']:
+                save_data.append(data['_source'])
+                count += 1
+            res = es.scroll(scroll_id=sid, scroll='2m')
+            sid = res['_scroll_id']
+
+        # 清除scroll_id
+        es.clear_scroll(scroll_id=sid)
+        df = pd.DataFrame(save_data)
+        duck_df = duckdb.from_df(df)
         # 写入结果
-        self.set_result(ck_df)
+        self.set_result(duck_df)
 
     def to_json(self):
         super(ESInput, self).to_json()
```

## NiceFlow/plugins/es_output.py

```diff
@@ -1,51 +1,48 @@
 import json
 
-from clickhouse_driver import Client
-from pyarrow import RecordBatch
+from pandas import DataFrame
+from elasticsearch import Elasticsearch, helpers
 
 from NiceFlow.core.flow import Flow
 from NiceFlow.core.plugin import IPlugin
-from loguru import  logger
+from loguru import logger
+
 
 class ESOutput(IPlugin):
 
     def init(self, param: json, flow: Flow):
         super(ESOutput, self).init(param, flow)
 
     def execute(self):
         super(ESOutput, self).execute()
         # 获取上一步结果
         pre_node = self.pre_nodes[0]
-        df = self._pre_result_dict[pre_node.name]
+        duck_df = self._pre_result_dict[pre_node.name]
         logger.debug(self.param)
 
         # param信息
-        host = self.param["host"]
-        port = self.param.get("port", 9000)
-        db = self.param["db"]
-        user = self.param.get("username", "default")
-        password = self.param.get("password", "")
-        table = self.param.get("table", "")
-        batch_size = self.param.get("batch_size", 100)
+        url = self.param["url"]
+        index = self.param.get("index", "")
+        batch_size = self.param.get("batch_size", 20000)
+        basic_auth = self.param.get("basic_auth", None)
 
         # 配置数据库
-        client = Client(host=host, port=port, database=db, user=user, password=password)
+        es = Elasticsearch(hosts=url,basic_auth=basic_auth)
         # 批量写数据库
-        total_count = len(df.to_df())
-        rel = df.fetch_arrow_reader(batch_size)
-        logger.info(f"总记录数据为 {total_count}")
-        count = 0
-        while True:
-            batch: RecordBatch = rel.read_next_batch()
-            sql = f'INSERT INTO {table}  VALUES '
-            # 写数据库
-            client.execute(sql, batch.to_pandas().to_dict(orient="records"), types_check=False)
-
-            count = count + 1
-            logger.debug(f"执行次数{count}")
+        df = duck_df.to_df()
+        list_df = [df[i:i + batch_size] for i in range(0, df.shape[0], batch_size)]
+        for i, df_chunk in enumerate(list_df):
+            helpers.bulk(es, self.generate_actions(df_chunk, index))
 
-            if total_count <= count * batch_size:
-                break
+        self.set_result(duck_df)
 
     def to_json(self):
         super(ESOutput, self).to_json()
+
+    def generate_actions(self,df: DataFrame, index_name: str):
+        for _, row in df.iterrows():
+            yield {
+                "_op_type": "index",
+                "_index": index_name,
+                "_source": row.to_dict()
+            }
```

## NiceFlow/plugins/faker_input.py

```diff
@@ -9,50 +9,36 @@
 from NiceFlow.core.plugin import IPlugin
 
 
 class FakerInput(IPlugin):
 
     def __init__(self):
         super().__init__()
-        # 缓存编译字节码
-        self.compile_dict = {}
-        # 创建一个duckdb连接
-        self.con = duckdb.connect()
-
-    def init(self, param: json,flow:Flow):
-        super(FakerInput, self).init(param,flow)
-        #  编译字节码对象
-        columns = self.param.get("columns",[])
-        for column in columns:
-            exec_str = "faker.{}()".format(column)
-            compile_obj = compile(exec_str, '', 'eval')
-            self.compile_dict[column] = compile_obj
+
+    def init(self, param: json, flow: Flow):
+        super(FakerInput, self).init(param, flow)
 
     def execute(self):
         super(FakerInput, self).execute()
         rows = self.param["rows"]
-        columns = self.param.get("columns",[])
-        randoms = self.param.get("randoms",[])
-        list_map = []
-        # faker不能去掉，因为compile_obj为动态编译
+        columns = self.param.get("columns", [])
+        randoms = self.param.get("randoms", [])
+
         faker = Faker('zh-CN')
-        for i in range(rows):
-            current_row = {}
-            for column in columns:
-                compile_obj = self.compile_dict[column]
-                value = eval(compile_obj)
-                current_row[column] = value
-            for element in randoms:
-                key = element["key"]
-                values = element["values"]
-                value = random.choice(values)
-                current_row[key] = value
-            list_map.append(current_row)
+        result = {}
+        for column in columns:
+            faker_generator = getattr(faker, column)
+            result[column] = [faker_generator() for _ in range(rows)]
+
+        for element in randoms:
+            key = element["key"]
+            values = element["values"]
+            result[key] = [random.choice(values) for _ in range(rows)]
 
         # 组装最后的结果
-        df = pd.DataFrame(list_map)
-        rel = self.con.from_df(df)
+        df = pd.DataFrame(result)
+        duck_df = duckdb.from_df(df)
         # 设置下一步结果
-        self.set_result(rel)
+        self.set_result(duck_df)
 
     def to_json(self):
         super(FakerInput, self).to_json()
```

## NiceFlow/plugins/ftp_input.py

```diff
@@ -1,13 +1,9 @@
 import json
 
-import duckdb
-import pandas as pd
-from clickhouse_driver import Client
-
 from NiceFlow.core.flow import Flow
 from NiceFlow.core.plugin import IPlugin
 
 
 class FtpInput(IPlugin):
 
     def init(self, param: json, flow: Flow):
```

## NiceFlow/plugins/kafka_input.py

```diff
@@ -1,26 +1,52 @@
 import json
+import threading
 
-from confluent_kafka import Consumer
+from kafka import KafkaConsumer
 
 from NiceFlow.core.flow import Flow
 from NiceFlow.core.plugin import IPlugin
 
 
 class KafkaInput(IPlugin):
 
+    def stop(self):
+        self.stop_event.set()
+
     def init(self, param: json, flow: Flow):
         super(KafkaInput, self).init(param, flow)
+        self.stop_event = threading.Event()
 
     def execute(self):
         super(KafkaInput, self).execute()
-        conf = {'bootstrap.servers': 'host1:9092,host2:9092',
-                'group.id': 'foo',
-                'auto.offset.reset': 'smallest'}
 
-        consumer = Consumer(conf)
+        # param信息
+        hosts = self.param.get("hosts", [])
+        topic = self.param.get("topic", "")
+
+        consumer = KafkaConsumer(bootstrap_servers=hosts,
+                                 auto_offset_reset='earliest',
+                                 consumer_timeout_ms=1000)
+        # 订阅要消费的主题
+        consumer.subscribe(topics=[topic])
+        while not self.stop_event.is_set():
+            for message in consumer:
+                print(message)
+                if self.stop_event.is_set():
+                    break
+
+        consumer.close()
+
+        # while True:
+        #     msg = consumer.poll()
+        #     json_data = json.loads(msg)
+        #     if isinstance(json_data,list):
+        #         df = pd.DataFrame(json_data)
+        #     else:
+        #         df = pd.DataFrame([json_data])
+        #     ck_df = duckdb.from_df(df)
+        #     # 写入结果
+        #     self.set_result(ck_df)
 
     def to_json(self):
         super(KafkaInput, self).to_json()
 
-    def close(self):
-        super(KafkaInput, self).close()
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## NiceFlow/plugins/mongo_input.py

```diff
@@ -1,9 +1,10 @@
 import json
 
+import duckdb
 import pandas as pd
 from pymongo import MongoClient
 
 from NiceFlow.core.plugin import IPlugin
 
 
 class MongoInput(IPlugin):
@@ -17,11 +18,12 @@
 
     def execute(self):
         super(MongoInput, self).execute()
 
         db = self.client['database_name']
         collection = db['collection_name']
         df = pd.DataFrame(list(collection.find()))
-        self.set_result(df)
+        duck_df = duckdb.from_df(df)
+        self.set_result(duck_df)
 
     def to_json(self):
         super(MongoInput, self).to_json()
```

## NiceFlow/plugins/mqtt_input.py

```diff
@@ -2,52 +2,79 @@
 
 import duckdb
 import pandas as pd
 
 from NiceFlow.core.flow import Flow
 from NiceFlow.core.plugin import IPlugin
 import paho.mqtt.client as mqtt
-from paho.mqtt import client as mqtt_client
 
 
 class MqttInput(IPlugin):
 
     def init(self, param: json, flow: Flow):
         super(MqttInput, self).init(param, flow)
 
     def on_connect(self, client, userdata, flags, rc):
-        print("Connected with result code " + str(rc))
-        client.subscribe("$SYS/#")
-
-    def subscribe(self,client: mqtt_client):
-        def on_message(client, userdata, msg):
-            print(f"Received `{msg.payload.decode()}` from `{msg.topic}` topic")
-            print(msg.topic + " " + str(msg.payload))
-            df = pd.DataFrame(msg.payload)
-            ck_df = duckdb.from_df(df)
-            # 写入结果
-            self.set_result(ck_df)
-
+        # 0: Connection successful
+        # 1: Connection refused - incorrect protocol version
+        # 2: Connection refused - invalid client identifier
+        # 3: Connection refused - server unavailable
+        # 4: Connection refused - bad username or password
+        # 5: Connection refused - not authorised
+        # 6-255: Currently unused.
+        if rc == 0:
+            print("Connection successful")
+        if rc == 1:
+            print("Connection refused - incorrect protocol version")
+        if rc == 2:
+            print("Connection refused - invalid client identifier")
+        if rc == 3:
+            print("Connection refused - server unavailable")
+        if rc == 4:
+            print("Connection refused - bad username or password")
+        if rc == 5:
+            print("Connection refused - not authorised")
+        if rc!=0:
+            return
+        # 在连接建立后订阅主题
         client.subscribe(self.topic)
-        client.on_message = on_message
+
+    def on_message(self, client, userdata, msg):
+        msg_str = msg.payload.decode('utf-8')
+        json_data = json.loads(msg_str)
+        if isinstance(json_data,list):
+            df = pd.DataFrame(json_data)
+        else:
+            df = pd.DataFrame([json_data])
+        ck_df = duckdb.from_df(df)
+        # 写入结果
+        self.set_result(ck_df)
 
     def execute(self):
         super(MqttInput, self).execute()
 
         # param信息
         host = self.param["host"]
         port = self.param.get("port", 1883)
         self.topic = self.param.get("topic", "")
+        username = self.param.get("username", None)
+        password = self.param.get("password", None)
         clientId = self.param.get("client_id", "")
 
         # 配置数据库
         if clientId:
             client = mqtt.Client(client_id=clientId)
         else:
             client = mqtt.Client()
+
+        # 配置消息回调
         client.on_connect = self.on_connect
         client.on_message = self.on_message
+
+        if username:
+            client.username_pw_set(username=username, password=password)
+
         client.connect(host, port)
         client.loop_forever()
 
     def to_json(self):
         super(MqttInput, self).to_json()
```

## NiceFlow/plugins/pivot.py

```diff
@@ -1,22 +1,28 @@
 import json
 
+import duckdb
+
 from NiceFlow.core.flow import Flow
 from NiceFlow.core.plugin import IPlugin
 
 
 class Pivot(IPlugin):
 
     def init(self, param: json,flow:Flow):
         super(Pivot, self).init(param,flow)
 
     def execute(self):
         super(Pivot, self).execute()
+        # PIVOT Cities ON Year USING sum(Population);
+        key = self.param["key"]
+        value = self.param["value"]
+        agg = self.param["agg"]
 
-        self.param[""]
         # 获取上一步结果
         pre_node = self.pre_nodes[0]
-        pre_df = self._pre_result_dict[pre_node.name]
-        self.set_result(pre_df)
+        duck_df = self._pre_result_dict[pre_node.name]
+        result_df = duckdb.sql(f"PIVOT duck_df ON {key} USING by {agg}({value}) ")
+        self.set_result(result_df)
 
     def to_json(self):
         super(Pivot, self).to_json()
```

## test/flow_test.py

```diff
@@ -26,16 +26,16 @@
             "file_name": "F:/07_数据源大全/store_order/channel.csv",
             "row": 20
         }
         myFlow.set_param(flow_param)
         myFlow.run()
 
     def test_mysql_log_handler(self):
-        handler = MySQLDBLogHandler()
-        Flow.register_log_handler(handler)
+        # handler = MySQLDBLogHandler()
+        # Flow.register_log_handler(handler)
         path = getProjectPath() + "/doc/faker_input_console.json"
         myFlow: Flow = FlowManager.read(path)
 
         myFlow.run()
 
     def test_project_root_path(self):
         path = getProjectPath() + "/doc/real/excel_input_many_excel_output.json"
```

## Comparing `NiceFlow-0.0.4.dist-info/LICENSE` & `NiceFlow-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `NiceFlow-0.0.4.dist-info/METADATA` & `NiceFlow-0.0.5.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: NiceFlow
-Version: 0.0.4
+Version: 0.0.5
 Summary: ETL数据处理/数据迁移/数据分析工具
 Home-page: https://www.seeoo.top
 Author: BleethNie
 Author-email: xiao5406710@foxmail.com
 Platform: python3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: duckdb >=0.9.2
+Requires-Dist: duckdb >=0.10.1
 Requires-Dist: pandas >=2.1.0
 Requires-Dist: loguru >=0.7.2
 Requires-Dist: click >=8.1.7
 Requires-Dist: blinker >=1.7.0
 Requires-Dist: pycryptodome ==3.20.0
 
 ## NiceFlow
 
-> 类似Kettle数据ETL工具，同时比Kettle更加易用和轻量
+> 类似Kettle数据ETL工具，同时比Kettle更加易用和轻量,底层基于duckdb,速度超快，是一款可以让普通用户快速使用的数据处理工具,基于插件机制，
+> 可以快速配置各种数据处理工作流，让数据处理工作流就像搭积木一样，简单易用。
 
 ### 特性
 
 - 基于python的插件机制,目前提供70+插件,同时支持自定义插件
 - 基于json的flow任务，支持自定义任务配置
+- 底层基于duckdb的内存数据库，支持sql脚本和json配置,支持亿级别的数据进行join查询，并且毫秒出结果
+
+#### 示例
+
+![img1.png](doc/doc/img/demo1.png)
+
+![img2.png](doc/doc/img/demo2.png)
+
 
-![img.png](doc/doc/img/demo.png)
 
 ### 安装依赖
 
 ```shell
 pip install NiceFlow
 ```
 
@@ -167,51 +175,54 @@
 
 ### 插件使用说明文档
 
 #### 输入
 
 | 插件              | 功能                | 完成情况 | 文档                            |
 |-----------------|-------------------|------|-------------------------------|
-| Starter         | 启动器               | 完成   | [启动器](doc/doc/Starter.md)     |
+| Starter         | 启动器               |    | [启动器](doc/doc/Starter.md)     |
 | CsvInput        | 读取CSV数据           | 完成   | [CSV输入](doc/doc/CSVInput.md ) |
 | FakerInput      | 假数据生成             | 完成   |  [假数据生成](doc/doc/FakerInput.md) |       
 | ParquetInput    | 读取Parquet数据       | 完成   | [Parquet输入](doc/doc/ParquetInput.md)    |    
 | ExcelInput      | 读取Excel数据         | 完成   | [Excel输入](doc/doc/ExcelInput.md) |           
 | MySQLInput      | 读取MySQL数据         | 完成   | [MySQL输入](doc/doc/MySQLInput.md) |           
 | DuckDBInput     | 读取DuckDB数据        | 完成   | [DuckDB输入](doc/doc/DuckDBInput.md) |         
 | AkshareInput    | 读取金融股票等财经数据       | 完成   | [Akshare输入](doc/doc/AkshareInput.md) |
 | ClickHouseInput | 读取ClickHouse数据    | 完成   | [ClickHouse输入](doc/doc/ClickHouseInput.md) |
 | OdpsInput       | 读取MaxCompute数据    | 完成   | [Odps输入](doc/doc/OdpsInput.md) |           
 | ESInput         | 读取Elasticsearch数据 | 完成   | [Elasticsearch输入](doc/doc/ESInput.md) |         
 | MongoDBInput    | 读取MongoDB数据       | 完成   | [MongoDB输入](doc/doc/MongoDBInput.md) |
-| MqttInput       | 从Mqtt Broker读取数据  |    | [MqttInput输入](doc/doc/MqttInput.md) |
+| MqttInput       | 从Mqtt Broker读取数据  |  完成  | [MqttInput输入](doc/doc/MqttInput.md) |
 
 #### 转换
 
-| 插件             | 功能   | 完成情况 | 文档                       |
-|----------------|------|------|--------------------------|
-| Filter         | 过滤器  | 完成   | [过滤器](doc/doc/Filter.md) |
-| Mapping        | 映射器  | 完成   | [映射器](doc/doc/Mapping.md)    |
-| For            | 遍历器  | 完成   | [遍历器](doc/doc/For.md)    |  
-| IF             | 条件判断器 | 完成   | [条件判断器](doc/doc/IF.md) |
-| Join           | 连接器  | 完成   | [连接器](doc/doc/Join.md)  |
-| Mask           | 脱敏器  | 完成   | [脱敏器](doc/doc/Mask.md) |
-| Pivot          | 透视表  | 完成   | [透视表](doc/doc/Pivot.md) |
-| Printer        | 打印器  | 完成   | [打印器](doc/doc/Printer.md) |
-| RegularExtract | 正则提取器 |      | [正则提取器](doc/doc/RegularExtract.md) |  
-| Rename         | 重命名器 | 完成   | [重命名器](doc/doc/Rename.md) |
-| Samples        | 采样器  | 完成   | [采样器](doc/doc/Samples.md) |
-| Sort           | 排序器  | 完成   | [排序器](doc/doc/Sort.md) |
-| Sql            | SQL转换器 | 完成   | [SQL转换器](doc/doc/SqlTransform.md) |
-| Switch         | 条件转换器 |      | [条件转换器](doc/doc/Switch.md) |
-| Unpivot        | 取消透视表 | 完成   | [取消透视表](doc/doc/Unpivot.md) |
-| Variable       | 变量转换器 | 完成   | [变量转换器](doc/doc/Variants.md) |
-| While          | 循环转换器 | 完成   | [循环转换器](doc/doc/While.md) |
-| Duplicate      | 去重器  | 完成   | [去重器](doc/doc/Duplicate.md) |
-| Console        | 控制台打印 | 完成   | [控制台输出](doc/doc/Console.md)    |
+| 插件               | 功能      | 完成情况 | 文档                                 |
+|------------------|---------|------|------------------------------------|
+| Filter           | 过滤器     | 完成   | [过滤器](doc/doc/Filter.md)           |
+| Mapping          | 映射器     | 完成   | [映射器](doc/doc/Mapping.md)          |
+| For              | 遍历器     | 完成   | [遍历器](doc/doc/For.md)              |  
+| IF               | 条件判断器   | 完成   | [条件判断器](doc/doc/IF.md)             |
+| Join             | 连接器     | 完成   | [连接器](doc/doc/Join.md)             |
+| Mask             | 脱敏器     | 完成   | [脱敏器](doc/doc/Mask.md)             |
+| Pivot            | 透视表     | 完成   | [透视表](doc/doc/Pivot.md)            |
+| Printer          | 打印器     | 完成   | [打印器](doc/doc/Printer.md)          |
+| RegularExtract   | 正则提取器   |      | [正则提取器](doc/doc/RegularExtract.md) |  
+| Rename           | 重命名器    | 完成   | [重命名器](doc/doc/Rename.md)          |
+| Samples          | 采样器     | 完成   | [采样器](doc/doc/Samples.md)          |
+| Sort             | 排序器     | 完成   | [排序器](doc/doc/Sort.md)             |
+| Sql              | SQL转换器  | 完成   | [SQL转换器](doc/doc/SqlTransform.md)  |
+| Switch           | 条件转换器   |      | [条件转换器](doc/doc/Switch.md)         |
+| Unpivot          | 取消透视表   | 完成   | [取消透视表](doc/doc/Unpivot.md)        |
+| Variable         | 变量转换器   | 完成   | [变量转换器](doc/doc/Variants.md)       |
+| While            | 循环转换器   | 完成   | [循环转换器](doc/doc/While.md)          |
+| Duplicate        | 去重器     | 完成   | [去重器](doc/doc/Duplicate.md)        |
+| Console          | 控制台打印   | 完成   | [控制台输出](doc/doc/Console.md)        |
+| SplitFieldToRows | 列拆分为多行  |  完成  | [列转行](doc/doc/SplitFieldToRows.md) |
+| Function         | 动态函数 |  完成  | [动态函数](doc/doc/Function.md)         |
+
 
 #### 输出
 
 | 插件              | 功能           | 完成情况 | 文档                            |
 |-----------------|------------|------|-------------------------------|
 | FileOutput      | 文件输出           | 完成   | [文件输出](doc/doc/FileOutput.md) |
 | KafkaOutput     | Kafka输出          | 完成   | [Kafka输出](doc/doc/KafkaOutput.md) |
@@ -234,9 +245,53 @@
 | ExcelOutput     | Excel输出          | 完成   | [Excel输出](doc/doc/ExcelOutput.md) |  
 | EsOutput        | Elasticsearch输出 |      |      |
 | DuckOutput      | DuckDB输出         |      |      |
 | CsvOutput       | CSV输出           | 完成   | [CSV输出](doc/doc/CsvOutput.md) |
 | CosOutput       | COS输出           |      |      |
 | ClickHouseOutput | ClickHouse输出    |      |      |
 
+#### 自定义脚本插件[PyScript]
+
+- 系统内置PyScript插件，该插件没有固定内容，可以自定义脚本,如下所示
+
+```json
+{
+  "flow": {
+    "name": "",
+    "uid": "",
+    "param": {
+
+    } },
+  "nodes": [
+    {
+      "id": "FakerInput",
+      "name": "read1",
+      "type": "input",
+      "properties": {
+        "rows":10000,
+        "columns": ["name","address","city","street_address","date_of_birth","phone_number"],
+        "randoms":[
+          {"key":"sex","values":["男","女","未知"]}
+        ]
+      }
+    },
+    {
+      "id": "PyScript",
+      "name": "write1",
+      "type": "output",
+      "properties": {
+        "content": "import json\n\nfrom NiceFlow.core.flow import Flow\nfrom NiceFlow.core.plugin import IPlugin\n\n\nclass PyScript(IPlugin):\n\n    def init(self, param: json, flow: Flow):\n        super(PyScript, self).init(param, flow)\n\n    def execute(self):\n        super(PyScript, self).execute()\n        row = int(self.param.get(\"row\",10))\n\n        # 获取上一步结果\n        pre_node = self.pre_nodes[0]\n        PyScript_df = self._pre_result_dict[pre_node.name]\n        PyScript_df.limit(row).show()\n        self.set_result(PyScript_df)\n\n\n    def to_json(self):\n        super(PyScript, self).to_json()\n\n    def close(self):\n        super(PyScript, self).close()"
+      }
+    }
+  ],
+  "edges": [
+    {
+      "startId": "read1",
+      "endId": "write1"
+    }
+  ]
+}
+```
+
+
 ### 数据实战
```

## Comparing `NiceFlow-0.0.4.dist-info/RECORD` & `NiceFlow-0.0.5.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 NiceFlow/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 NiceFlow/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-NiceFlow/cli/cli.py,sha256=3ivAUZHJ9LU4uO5ORJh8w3FozXkTw5o4Ok0R8YBQth0,7129
+NiceFlow/cli/cli.py,sha256=4oT6lpes7gXDo2Mwa7M6amp5_rEfAOc54FwjtY2RlQQ,8890
 NiceFlow/cluster/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 NiceFlow/cluster/master.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 NiceFlow/cluster/operator.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 NiceFlow/cluster/worker.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 NiceFlow/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 NiceFlow/common/ftp_util.py,sha256=bm2WW_1XDKx2xmshPCmGyMRdT-K0PXja8oyyaUcMlhU,8764
 NiceFlow/common/hdfs_util.py,sha256=prQOf1_2FNAe5Yf7iK5jpKCcVPdJGO4PailrXNg3iQc,1358
-NiceFlow/common/module_util.py,sha256=yiDpUKKw0rmz9ECnAO0iVURmgTC12o75mhZ0qQkwVbo,238
+NiceFlow/common/module_util.py,sha256=Wtu5Ep_ssZBpgLqwIcz_t7DjkB2W0qMWKlgKrlJWJgE,236
 NiceFlow/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 NiceFlow/core/db_logging_handler.py,sha256=OJeOGnWy9BRoY1s5LVqcyHu4a1kt_hSmwDUA46r9Xog,813
 NiceFlow/core/db_plugin.py,sha256=Ek6Jiehqjs6uk08VEhdK5LAxrAIlfLRS1CMlsWBFSbc,244
 NiceFlow/core/flow.py,sha256=5nqKoArm2o8PLQpUOyJ1zdH1aCozL65ahxO-mYKEkrM,4284
 NiceFlow/core/flow_log.py,sha256=LbN4MeQ5ZLSqZfcc6Zsa-3VYzSdRNbEWr9Pa89HJm_8,127
 NiceFlow/core/flow_log_handler.py,sha256=Yak0x-6u77R5g6AdLVfLHrtwgk1w8wx0vp6aiVpxwSI,130
+NiceFlow/core/functions.py,sha256=jJWG-GnKETGmm9RwmneXa5JdbrER8o0Ht7igYF0Atd0,72
 NiceFlow/core/manager.py,sha256=DMopgnfQGQmAL2WNGMwjab-i-Apt5LZsxziow5XPIg4,6517
 NiceFlow/core/mysqldb_logging_handler.py,sha256=Yl-6eBtSLH4TG0-RsktyV9ny55LmQuYJ5ZP_46EAoYc,2939
-NiceFlow/core/plugin.py,sha256=49y134uILBE8hJ_0ieEnw0lfS5rBxozRshs4INMen94,4024
+NiceFlow/core/plugin.py,sha256=VrQ4eMJiG4amMj6hUp7EadDX1mZR05F6OF3qInNxQgE,4188
 NiceFlow/core/plugin_field.py,sha256=qF_oHMK3l7UVAWKeIfNt3e81qjK2fBgaNrq_HvzD0Ws,1755
 NiceFlow/core/plugin_log.py,sha256=Bn5-w2PLyQX6OSrxEjkq-7SKDAAXS1Ld7l7La2Q5HoI,123
 NiceFlow/core/plugin_time_record.py,sha256=Tphn8I78AvjeMRJmdhrpFZYksBjpDDTAojw3MwJk9g8,1214
 NiceFlow/core/states.py,sha256=7iVjcP-s6x8uX9WOd919NI2t8iR1PPoToTiwbBRDxMQ,811
 NiceFlow/core/tool.py,sha256=yP1ja2F8ltJZo5go15PPF79iAR44OZwXv2eHuS-ZNrs,2288
 NiceFlow/core/exception/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 NiceFlow/core/exception/flow_exception.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -30,106 +31,112 @@
 NiceFlow/core/utils/encrypt_data.py,sha256=el8CHVcJmSLia8nnsCPgWg3TXD9UNQHLUnVIC081CZk,1825
 NiceFlow/log/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 NiceFlow/log/flow_log.py,sha256=LbN4MeQ5ZLSqZfcc6Zsa-3VYzSdRNbEWr9Pa89HJm_8,127
 NiceFlow/log/flow_log_handler.py,sha256=Yak0x-6u77R5g6AdLVfLHrtwgk1w8wx0vp6aiVpxwSI,130
 NiceFlow/log/mysqldb_logging_handler.py,sha256=3PPF68T5WfyPdiEIZyzyN_Y0h1ejp8qvJ6-MnxLKyRQ,2937
 NiceFlow/log/plugin_log.py,sha256=Bn5-w2PLyQX6OSrxEjkq-7SKDAAXS1Ld7l7La2Q5HoI,123
 NiceFlow/plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+NiceFlow/plugins/add_field.py,sha256=rfqqrbv2CHTQ-gUGBsz44b71G3gQ-l8s3V8cNECDuPw,1310
+NiceFlow/plugins/agg.py,sha256=hAxM1sHkslrtsOzD_druMUmXHHn5yyttGHoH-U9nAHk,956
 NiceFlow/plugins/akshare_input.py,sha256=bLokKR9pQZcnY5gb55hXBbYIrNbczFVV6KlUBRtnT7g,1110
 NiceFlow/plugins/ck_input.py,sha256=NstUBuXM8OCF1h9PFKJTYzJEXpgfGWPjbVYoJI92y_g,1164
 NiceFlow/plugins/ck_output.py,sha256=BDN8PMahGypnyrkjq2QfiPWl4B087pVJIp1s9TGXXeM,1678
 NiceFlow/plugins/console.py,sha256=a-YO7S1zCwnV9UEk14YaQMvUlwxQUgzdueEfYgBMS44,665
 NiceFlow/plugins/cos_input.py,sha256=781WfWIFzUAzHsuuqVMXhSDO08noE_XCqGy1s_nQgao,1168
 NiceFlow/plugins/cos_output.py,sha256=G1EdRRxSWaBP5cAGZ5uF3V3y-MfFjruB-DnG0bsH_E4,1172
-NiceFlow/plugins/csv_input.py,sha256=tguUbxPD75jZKuuUosz-7LZp8SiYW6OADLDfKge6Cuo,762
-NiceFlow/plugins/csv_output.py,sha256=HWEYL2y8eOrtwwokZokALERN6rfNAz-Z7BzLs_BxorU,637
+NiceFlow/plugins/csv_input.py,sha256=I5LJCz_CC3pKrhxmC-4MkZyM8hicyZHS8oQHGK_SwqE,1440
+NiceFlow/plugins/csv_output.py,sha256=bZN48qoX2lXP8d_6Z-0gc4OK3LMCbZSerZr1F5wiWJI,636
 NiceFlow/plugins/db2_input.py,sha256=fCStrnSbEHUmN4pzFSRW6Y-q3JutQios_cA-VLlrH6A,1168
 NiceFlow/plugins/db2_output.py,sha256=SZi5Zt26Onvma7MI9uxYk2mE7iESgQv_w9UR7QnAwrk,1172
 NiceFlow/plugins/db_execute.py,sha256=z_mzQWwjMHukUj-OxrlM1CvEqT_w2a6mmre91BziW-w,1007
 NiceFlow/plugins/duckdb_input.py,sha256=fVdqXMqWSMlnwNdSGY_CJiaOaU9hrrvk0JB70xb6_7c,716
 NiceFlow/plugins/duckdb_output.py,sha256=QL_S8KU9ukB7SGv0j0lc5lnNWXTMJCRSzQAMXFOZJ3M,779
 NiceFlow/plugins/duplicate.py,sha256=owLpMmWBxHE663wP1bdj9P_AzyLhRszczKZ0B0VHq-g,1288
 NiceFlow/plugins/email.py,sha256=bJGbgW6OgX5KOuoOIj96TZEHkILhZF_PF_0JEoeT2ng,547
-NiceFlow/plugins/es_input.py,sha256=MJDChGy-Qq-UGbqHkgjfCVezXxJpFEny_W9-m_eSVQk,1164
-NiceFlow/plugins/es_output.py,sha256=a1llnWNK0vjFy9eO8t35qDbN-Ju4fp_PHLyDnH5IyfA,1678
+NiceFlow/plugins/es_input.py,sha256=vL38Fex79AxzJ3Jx5oaVpvwbN2ZesjFc1waUkGfSCe0,1415
+NiceFlow/plugins/es_output.py,sha256=FI9IbjOZE85mEZG1lwIM8hnUFQQFfadGw2kmn25OOKI,1491
 NiceFlow/plugins/excel_input.py,sha256=mJajo1WfGZ1tcXHUZlTbYEfVvX_vsuatim62G2hmR9k,800
 NiceFlow/plugins/excel_output.py,sha256=4VZVYdzI3lz-gaTtU_WmNJwZBwOqWIsfXTY6YuIbUyc,954
-NiceFlow/plugins/faker_input.py,sha256=bZmCpFpeA1_bRNWvU_BmN1-_wRy62zOWA_TO6dpFWtc,1820
+NiceFlow/plugins/faker_input.py,sha256=xWS0UV1E-lgRvtasGjy7zbeRGb1KL4RndhBBjNoUUlk,1197
 NiceFlow/plugins/filter.py,sha256=LR1fDRdFlhyLVst-p3JAfJnzq3ctAbYHe9U799jOOzg,809
 NiceFlow/plugins/for.py,sha256=D3Yze10l1OPDRuCtJFAJpi96nCvvzNyKodBt1K4Zs4Y,2385
-NiceFlow/plugins/ftp_input.py,sha256=Mk_HO15PK_25IJ-sXeTcAj05dRXBBDcmHgsytKa1eWQ,699
+NiceFlow/plugins/ftp_input.py,sha256=_NP0SOiy7gn2GAza6dd4M8IJYFCgan9Pba5mldXRf50,623
 NiceFlow/plugins/ftp_output.py,sha256=ztnUBUozdgQ0HqPRql87PZRbJxiZ2lpJ29hvgy0C2uA,1172
+NiceFlow/plugins/function.py,sha256=ya5xIDvJ2Np0cjACIS8bePHxWYCy-1gur6-rp6fMwns,1718
 NiceFlow/plugins/hdfs_input.py,sha256=cmJ6Dg53omXewXyH_4cmZqUfhvRDPoek251QGL4Nt20,1017
 NiceFlow/plugins/hdfs_output.py,sha256=Jem_u7VwLow2CqG5_UyyOcYzVs6Bwiiep6kwIZ4jDd4,2302
 NiceFlow/plugins/hive_input.py,sha256=iiC9vsj1eXYCPfiUL-hZyMIM1kqKgIe_oTrgewIjpv0,651
 NiceFlow/plugins/hive_output.py,sha256=ixlwoEqZiy8sT36Sla3C5cZyFXWeIKyEvUpImdcUDjE,642
 NiceFlow/plugins/html_output.py,sha256=2LT-6roc7s8DVxJRQE7-slOlXIO4waUWbJErfXEzA3Y,568
 NiceFlow/plugins/html_parse_input.py,sha256=21R-1M8M0jDGetzrGQLow_oB0zjk7X18_7bg53oxowU,1174
 NiceFlow/plugins/http_input.py,sha256=sssmsuZbyXJAnneAKHMYaE5OUM9RleWDLIQ0sDtV_jU,1672
 NiceFlow/plugins/http_output.py,sha256=kM6oxqnzZSx5yYCht9W6S3rj8iTJTNgWIDmsbjRiSOI,1742
 NiceFlow/plugins/if.py,sha256=Mk7b1Dkb0C30L7Lz5POEKmfPvfaL1FWaWH0yMX-PNkc,1414
 NiceFlow/plugins/join.py,sha256=yqiwi_j3-B9-CMngk6a1Er8mMXMN8qRc-ffNLufEBME,494
-NiceFlow/plugins/kafka_input.py,sha256=WbjkR9iwWB3SzJ-TCXm9p_Zc9vBCzniquHoZsFHdD4o,654
+NiceFlow/plugins/kafka_input.py,sha256=jUmas-LpndLgfF8nDH39h0CB7QRpe5hcdSEMCeVS6Pc,1493
 NiceFlow/plugins/kafka_output.py,sha256=21fZmaHfi3C-Y5ScijUR2zri7wrjMdvPiQNA3S-ZGAw,659
 NiceFlow/plugins/mapping.py,sha256=KWs6g4vJTAFSK3hs1P2Gk9zJWpCyBFxaQzDvUVX4reo,3159
 NiceFlow/plugins/markdown_output.py,sha256=T2C_KhFs52xFOzDdWMWNF9Nb9yHZQ-i_R26bDG9yuA0,708
 NiceFlow/plugins/mask.py,sha256=JfhkWhUWBidoTdBLkO-1S_SZl03jnmtdR4gg2zKVgfA,1385
-NiceFlow/plugins/mongo_input.py,sha256=0XLPUfL9l9jkscoVxlAxQo3RmKMkU3P4xJGyeSPp0OY,631
+NiceFlow/plugins/mongo_input.py,sha256=J2oF7PpgLf07emZKR-haWsUOUQ661lDq3Um2oDVytzY,689
 NiceFlow/plugins/mongo_output.py,sha256=FVqWfZYT7GI3tpgsIKfX3i8Iv6Sg3zU5qUTrV04oGiE,825
-NiceFlow/plugins/mqtt_input.py,sha256=u34P0vt1_v7fbfUAIgH7hqIRsVsjC9wE4_bB5fEIiAY,1606
+NiceFlow/plugins/mqtt_input.py,sha256=Kk_1e_SgvWPbFHdG_5-rybOEI_IwKj2cueuKssb7itM,2594
 NiceFlow/plugins/mqtt_output.py,sha256=dT0s-6OH1ZN3bZ0NWbzRn3GWRhMR1TLiaS8OelMXVUc,1442
 NiceFlow/plugins/mysql_input.py,sha256=ulUwWYEv4B5CWYh7rizvZWXxfJYSw2KDhpV4iGxDH4E,2313
 NiceFlow/plugins/mysql_output.py,sha256=_bxLFSQ50icTowMLga796lQPMf4jEZBppE1aqMssf5Q,3883
 NiceFlow/plugins/odps_input.py,sha256=mdr_OCcaM4lZp44JY8Zc34KPR4VqXhKgRVQwPIOiMlc,1112
 NiceFlow/plugins/odps_output.py,sha256=EtgH8pviCvbmTbfOK0y9Mzk08MCH5vfakk3QJGu_5Rs,1400
 NiceFlow/plugins/oracle_input.py,sha256=cShOQnQ8arvbVnrz73mU9b4GPuPufomVql56SWrJeHQ,1257
 NiceFlow/plugins/oracle_output.py,sha256=oOUK0VKTNOOeDbegsnp7gPvJ4cVt9V15yS21onJ0PSE,1460
 NiceFlow/plugins/paimon_input.py,sha256=BFnXqb_fACudBemY7BkAzvsRDAFf0vyN56RKHGFgdhA,659
 NiceFlow/plugins/paimon_output.py,sha256=lemoy0GSiVjF9J95jNbX03IOxkGBzTcispFyUYnoCV0,666
 NiceFlow/plugins/parquet_input.py,sha256=7vdC6__SKWVzwofP75YJXH1nPRxw0lqNzn4EbScgs20,539
 NiceFlow/plugins/parquet_output.py,sha256=VV1IS_ZAjzN4YSFPmzKlwJGDQjyu35T92SVUlsVLgjI,606
-NiceFlow/plugins/pivot.py,sha256=ave2GxGP5UG0GBNC1fk7ASzyg9LpRn4XQGeKv4iOlNc,525
+NiceFlow/plugins/pivot.py,sha256=FRLUPvtZERvUFo6p1IKuCQWXfB1liDbBfVeygsPXs9o,764
 NiceFlow/plugins/postgre_input.py,sha256=qXOCVH2D8fQbqdy_ICtoad_mlk6hivIWfgBVZnvVxc8,1262
 NiceFlow/plugins/postgre_output.py,sha256=qfCl0egg0SDxAT1j6d37vgOBzk43J8cEfjtY1psRRtY,1233
 NiceFlow/plugins/printer.py,sha256=9yh61PjfOgF6qESzAAt3BR9VFCRboxyl3avieyrb6lw,617
 NiceFlow/plugins/pulsar_input.py,sha256=o2npTCyzlHDg9iaXU1ip2xKB6w6sMqz9IwyxK_MFZgk,1446
 NiceFlow/plugins/pulsar_output.py,sha256=o2npTCyzlHDg9iaXU1ip2xKB6w6sMqz9IwyxK_MFZgk,1446
 NiceFlow/plugins/regular_extract.py,sha256=tazhaJIxWQJ7krg7Vu1R-YW8KN8cqskNorAZzIbClss,534
 NiceFlow/plugins/rename.py,sha256=wx7apLJyFV-ju5G5wSJ5SbR3jRi09cxXQM0z05tIjA0,799
 NiceFlow/plugins/s3_input.py,sha256=KHuPyc-_-jJQj6f5s_PfyR3OSAPgdcrUy-Vft0eyj9M,1164
 NiceFlow/plugins/s3_output.py,sha256=Sgse714dV4p6N8QglAnVZ8Rtr_40El_Q8um32Lap0PI,1168
 NiceFlow/plugins/samples.py,sha256=V0MGOccmXudw7ahvq0zEb2IaEPaF8uXkvTpaVqkG9y8,796
 NiceFlow/plugins/sequence.py,sha256=SeET6D_TrKYATRW4R2FNS9XmcCwOCYCgOrR3E5qNIr8,915
 NiceFlow/plugins/sort.py,sha256=zy4rv6vxggh0qgEjSwt6acBWntTbI_8MGWCylRhdh4I,947
 NiceFlow/plugins/spider.py,sha256=M75szlgvQ00o5Z3BCdDYraWVNTBQpAMjvAFMhDhbPxY,879
+NiceFlow/plugins/split_field_to_rows.py,sha256=rg2Bkq73U0G46CAZfnRTyjJUWX_PX3sssX05vu340HM,1018
 NiceFlow/plugins/sql.py,sha256=m-nVTGE8BXxqdDRWshWDyKwsH5rxKr0t2ActxioKIU4,861
 NiceFlow/plugins/sqlserver_input.py,sha256=pj9p-zodWZYIz6RlKK84LkZ2k46fDwK-8brKQYjMknk,1160
 NiceFlow/plugins/sqlserver_output.py,sha256=nzssSnwfdYDZAY8i-t2EIy8sAtT6VD41JLAITechZA4,1184
 NiceFlow/plugins/starter.py,sha256=5746oAM1lxBmnEBY3KNfDBJPzdK2TuFI7zIr0xvASEo,463
 NiceFlow/plugins/sub_flow.py,sha256=4sZLCiW-oM3z_kW-pOIX7Shn7rM2AD1MVjvkjkKIEhM,544
 NiceFlow/plugins/switch.py,sha256=YFtsxwkoS3LeoxGjdsWugNraOhWwESt60_zrQtRcUIY,511
 NiceFlow/plugins/table_schema_convert.py,sha256=zPQQ-MrqnTsAMdsg8Y4FNIOJ2vzuDIMsi_I6zrJtSAQ,2759
 NiceFlow/plugins/unpivot.py,sha256=QPUgSkaNGu7xuJ4swnIYrK5hcW84Sa1FbvmS8RDawOU,533
 NiceFlow/plugins/variable.py,sha256=s9FOccGVx51KX5gvQAlo9WUfgvH8uFq_DDVpz0zHxWA,692
 NiceFlow/plugins/while.py,sha256=vkp5o9szrNFQErdPAWAhxqr4Ts7jlh9TUkUiGErgw5k,1424
+NiceFlow/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/a_test.py,sha256=l_t9qKoPFfdGY5Oz932IE2j53MWCOvigLe9XXX-s_ls,5586
 test/base_test.py,sha256=UwBQUbsAr8kfSCRpbzAOrKPrL0mupGhj84ynIWhuMCo,2142
 test/binlog_test.py,sha256=C8yJTt02DKZcLzkz9a-SEzomXTu6Ox8l7v75ZdnhtO4,1079
 test/connectx_test.py,sha256=iWpEbU8eku81ByP4Ggk2fm_L88SXfbHGpd0IjmmppFE,2726
 test/dt_test.py,sha256=4-8Mgm5zOaqyiOTo-DtATT4o3ugbHpJRcsmkW9xGsLw,4690
 test/duckdb_test.py,sha256=GJKvC5o-r4GuStzwKm2mHIaYMn69jLx4SlzBCmuWIrg,3437
-test/flow_test.py,sha256=VepZFsntAcdW4wPHIKgwLZbpIu4581Xv6kssKuWy_80,1809
+test/flow_test.py,sha256=zBYuDSU4-MioXA-ZG-R0kLJ9MUcHNt741xKqevoUqG4,1813
 test/ftp_test.py,sha256=3k2RB0BzLBlAO85QFsNHKoMpyKQkg8sW-i5143GLtBY,907
 test/git_test.py,sha256=iVQzi2SD3i5849960dSvSLHjiOVwlgHKlUWT636D6J0,298
+test/pandas_test.py,sha256=7pXx6ExVkikNDglAzSEp68Mx2ZCJF2TObWRD2dSpdFY,1236
 test/plugin_input_test.py,sha256=SALyNwtUT6X2xRRJE4DwB4kuagKPgInFHODFoIHJvAY,2672
 test/plugin_output_test.py,sha256=QjSNZRwWPxAnie6TpFqlzaqh1sMbdpmlKeoXA0ftnVs,2388
 test/plugin_transform.py,sha256=z8xhGioCgdIi39hkldnLYUVt1AVRpg36UkiEWDWF1as,4318
 test/real_test.py,sha256=QTWPK3_pweAujTORcEqzgECEb6kuGzGNbbK-tru-4uU,1070
 test/sqlglot_test.py,sha256=px1Ctwl-ijbT7ac-X0dN29HfHPiNOouiyOap0VAadQE,1626
 test/uuid_test.py,sha256=WIi6HKW1lAfVRliDjd3wIu_63l6D9C1Pyfq-efF4_VE,1280
-NiceFlow-0.0.4.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-NiceFlow-0.0.4.dist-info/METADATA,sha256=NvASy1dv76vPIL3-rlAMVMxfYqPv35NHLuo60j9yX70,9420
-NiceFlow-0.0.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-NiceFlow-0.0.4.dist-info/entry_points.txt,sha256=GkPfqTEcc_Mu-IBi2teygJbV86uLFsTyQTehy-CIljM,50
-NiceFlow-0.0.4.dist-info/top_level.txt,sha256=osiw4GlHif-My11ggVu0HW6vcSMCu2ZqKalBe0YJttw,14
-NiceFlow-0.0.4.dist-info/RECORD,,
+NiceFlow-0.0.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+NiceFlow-0.0.5.dist-info/METADATA,sha256=SBe24svhTHIR_ZwJWnEIjhed_oFAJ9SFxTwVxcQ3FIM,11804
+NiceFlow-0.0.5.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+NiceFlow-0.0.5.dist-info/entry_points.txt,sha256=GkPfqTEcc_Mu-IBi2teygJbV86uLFsTyQTehy-CIljM,50
+NiceFlow-0.0.5.dist-info/top_level.txt,sha256=osiw4GlHif-My11ggVu0HW6vcSMCu2ZqKalBe0YJttw,14
+NiceFlow-0.0.5.dist-info/RECORD,,
```

