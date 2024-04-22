# Comparing `tmp/biotech-1.1.6.tar.gz` & `tmp/biotech-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotech-1.1.6.tar", max compression
+gzip compressed data, was "biotech-1.1.7.tar", max compression
```

## Comparing `biotech-1.1.6.tar` & `biotech-1.1.7.tar`

### file list

```diff
@@ -1,760 +1,739 @@
--rwxr-xr-x   0        0        0      211 2024-04-20 04:40:12.925620 biotech-1.1.6/license.S.HTML
--rwxr-xr-x   0        0        0     1145 2024-04-20 04:52:15.431517 biotech-1.1.6/pyproject.toml
--rwxr-xr-x   0        0        0     3866 2024-04-20 04:40:12.929620 biotech-1.1.6/readme.md
--rwxr-xr-x   0        0        0     2331 2024-04-20 04:40:12.929620 biotech-1.1.6/venue.S.HTML
--rwxr-xr-x   0        0        0   838272 2024-04-20 04:40:12.929620 biotech-1.1.6/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
--rwxr-xr-x   0        0        0     1270 2024-04-20 04:40:12.929620 biotech-1.1.6/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
--rwxr-xr-x   0        0        0     4125 2024-04-20 04:40:12.929620 biotech-1.1.6/venues/stages/biotech/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      645 2024-04-20 04:40:12.929620 biotech-1.1.6/venues/stages/biotech/___itinerary/maybes.s.HTML
--rwxr-xr-x   0        0        0      190 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/___itinerary/processes/errout/script.py
--rwxr-xr-x   0        0        0     1255 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/___itinerary/processes/errout/start.py
--rwxr-xr-x   0        0        0      189 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
--rwxr-xr-x   0        0        0      186 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
--rwxr-xr-x   0        0        0      190 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
--rwxr-xr-x   0        0        0     1141 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
--rwxr-xr-x   0        0        0      385 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/__glossary/biotech_1
--rwxr-xr-x   0        0        0      114 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/__glossary/glossary.S.HTML
--rwxr-xr-x   0        0        0      130 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/__init__.py
--rwxr-xr-x   0        0        0    37279 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0     1252 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/_book/advanced tutorial.s.HTML
--rwxr-xr-x   0        0        0     1786 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/_book/book.s.HTML
--rwxr-xr-x   0        0        0      542 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/_book/relevant.s.HTML
--rwxr-xr-x   0        0        0     2129 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/_clique/__init__.py
--rw-r--r--   0        0        0     2493 2024-04-20 04:41:49.823732 biotech-1.1.6/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4457 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      691 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0  1430585 2024-04-20 04:51:24.751948 biotech-1.1.6/venues/stages/biotech/_status/DB/records.json
--rw-r--r--   0        0        0     1172 2024-04-20 04:44:34.660565 biotech-1.1.6/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
--rwxr-xr-x   0        0        0     1589 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
--rwxr-xr-x   0        0        0     1116 2024-04-20 04:40:12.933620 biotech-1.1.6/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
--rwxr-xr-x   0        0        0     1487 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/establish.py
--rw-r--r--   0        0        0      324 2024-04-20 04:44:38.572504 biotech-1.1.6/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       83 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      720 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/-01_start/status_1.py
--rw-r--r--   0        0        0      321 2024-04-20 04:44:45.344400 biotech-1.1.6/venues/stages/biotech/_status/monitors/00_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      101 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/00_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      793 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/00_start/status_1.py
--rw-r--r--   0        0        0      565 2024-04-20 04:44:51.964300 biotech-1.1.6/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_1_health.cpython-310.pyc
--rw-r--r--   0        0        0      453 2024-04-20 04:44:51.964300 biotech-1.1.6/venues/stages/biotech/_status/monitors/01/stasis/__pycache__/path_2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      282 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/01/stasis/path_1_health.py
--rwxr-xr-x   0        0        0      265 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/01/stasis/path_2_health.py
--rwxr-xr-x   0        0        0     1161 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/01/status_1.py
--rwxr-xr-x   0        0        0      321 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/02/stasis/1_health.py
--rwxr-xr-x   0        0        0        2 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/02/stasis/2_health.py
--rw-r--r--   0        0        0      628 2024-04-20 04:44:58.652199 biotech-1.1.6/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/1_health.cpython-310.pyc
--rw-r--r--   0        0        0      162 2024-04-20 04:44:58.648199 biotech-1.1.6/venues/stages/biotech/_status/monitors/02/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0       50 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/02/stasis/modules/MODULE_1.py
--rw-r--r--   0        0        0      287 2024-04-20 04:44:58.652199 biotech-1.1.6/venues/stages/biotech/_status/monitors/02/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1214 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/02/status_1.py
--rwxr-xr-x   0        0        0      794 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py
--rwxr-xr-x   0        0        0       35 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/1_health.py
--rw-r--r--   0        0        0      213 2024-04-20 04:45:10.040032 biotech-1.1.6/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      939 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py
--rwxr-xr-x   0        0        0      289 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/1_health.py
--rw-r--r--   0        0        0      522 2024-04-20 04:45:16.759935 biotech-1.1.6/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      942 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py
--rwxr-xr-x   0        0        0      518 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py
--rwxr-xr-x   0        0        0      155 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/MODULE_1.py
--rw-r--r--   0        0        0      377 2024-04-20 04:45:23.475839 biotech-1.1.6/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
--rw-r--r--   0        0        0      779 2024-04-20 04:45:23.475839 biotech-1.1.6/venues/stages/biotech/_status/monitors/05__file__/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      867 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/05__file__/status_1.py
--rwxr-xr-x   0        0        0      311 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/06_various/stasis/1_health.py
--rwxr-xr-x   0        0        0       31 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/06_various/stasis/2_health.py
--rwxr-xr-x   0        0        0        0 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/06_various/stasis/3_health.py
--rw-r--r--   0        0        0     1037 2024-04-20 04:45:30.111746 biotech-1.1.6/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/1_health.cpython-310.pyc
--rw-r--r--   0        0        0      184 2024-04-20 04:45:30.103746 biotech-1.1.6/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/2_health.cpython-310.pyc
--rw-r--r--   0        0        0      170 2024-04-20 04:45:30.111746 biotech-1.1.6/venues/stages/biotech/_status/monitors/06_various/stasis/__pycache__/3_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      955 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/06_various/status_1.py
--rw-r--r--   0        0        0      467 2024-04-20 04:45:36.839653 biotech-1.1.6/venues/stages/biotech/_status/monitors/07/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      160 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/07/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0      809 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/07/status_1.py
--rw-r--r--   0        0        0      311 2024-04-20 04:45:43.555561 biotech-1.1.6/venues/stages/biotech/_status/monitors/08_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       73 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/08_DB/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0     1561 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/08_DB/status_1.py
--rwxr-xr-x   0        0        0   102598 2024-04-20 04:50:59.436169 biotech-1.1.6/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json
--rw-r--r--   0        0        0      453 2024-04-20 04:45:50.339470 biotech-1.1.6/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rw-r--r--   0        0        0      455 2024-04-20 04:45:50.339470 biotech-1.1.6/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rw-r--r--   0        0        0      215 2024-04-20 04:45:50.339470 biotech-1.1.6/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      119 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0      124 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_2.py
--rwxr-xr-x   0        0        0        7 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_3.py
--rwxr-xr-x   0        0        0     1442 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py
--rw-r--r--   0        0        0      357 2024-04-20 04:45:57.075380 biotech-1.1.6/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       96 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1189 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
--rw-r--r--   0        0        0      316 2024-04-20 04:46:07.863238 biotech-1.1.6/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       77 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1250 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/monitors/11/status_1.py
--rwxr-xr-x   0        0        0      984 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/status.proc.py
--rwxr-xr-x   0        0        0      256 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status/status.s.HTML
--rwxr-xr-x   0        0        0     1483 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0      406 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
--rwxr-xr-x   0        0        0      358 2024-04-20 04:40:12.969620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
--rwxr-xr-x   0        0        0   542989 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
--rwxr-xr-x   0        0        0      919 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/_status_advanced/status.proc.py
--rwxr-xr-x   0        0        0     1779 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/architecture.s.HTML
--rwxr-xr-x   0        0        0      241 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/emojis.S.HTML
--rwxr-xr-x   0        0        0      286 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/license.S.HTML
--rwxr-xr-x   0        0        0     3068 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/module.s.HTML
--rw-r--r--   0        0        0     1596 2024-04-20 04:44:35.492552 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      640 2024-04-20 04:44:35.500552 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      259 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
--rwxr-xr-x   0        0        0     1478 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      366 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/paths.py
--rwxr-xr-x   0        0        0      666 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
--rwxr-xr-x   0        0        0      562 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
--rw-r--r--   0        0        0     1165 2024-04-20 04:44:36.648534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3738 2024-04-20 04:49:29.508999 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
--rw-r--r--   0        0        0     3545 2024-04-20 04:49:50.852795 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      999 2024-04-20 04:44:36.652534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0     2881 2024-04-20 04:44:36.652534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
--rw-r--r--   0        0        0     1152 2024-04-20 04:44:36.652534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      653 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
--rwxr-xr-x   0        0        0     3572 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
--rwxr-xr-x   0        0        0      769 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
--rw-r--r--   0        0        0     2031 2024-04-20 04:44:36.644534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
--rw-r--r--   0        0        0     2159 2024-04-20 04:44:36.648534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      420 2024-04-20 04:44:36.644534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
--rw-r--r--   0        0        0      728 2024-04-20 04:44:36.648534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
--rwxr-xr-x   0        0        0     3451 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
--rwxr-xr-x   0        0        0     3235 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
--rwxr-xr-x   0        0        0      193 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
--rwxr-xr-x   0        0        0      514 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
--rwxr-xr-x   0        0        0     2440 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
--rw-r--r--   0        0        0     2352 2024-04-20 04:44:36.644534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      799 2024-04-20 04:44:36.648534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
--rw-r--r--   0        0        0     4019 2024-04-20 04:44:36.648534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
--rw-r--r--   0        0        0     1303 2024-04-20 04:44:36.648534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/__pycache__/global_time_limit_exceeded.cpython-310.pyc
--rw-r--r--   0        0        0     1634 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
--rw-r--r--   0        0        0     2916 2024-04-20 04:40:12.973620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/no_records.py
--rwxr-xr-x   0        0        0      754 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
--rw-r--r--   0        0        0     1826 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-20 04:44:36.648534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      996 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
--rwxr-xr-x   0        0        0     8732 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
--rwxr-xr-x   0        0        0     3561 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
--rw-r--r--   0        0        0     2178 2024-04-20 04:44:36.644534 biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      834 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
--rw-r--r--   0        0        0      951 2024-04-20 04:45:40.247606 biotech-1.1.6/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      648 2024-04-20 04:44:36.652534 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
--rw-r--r--   0        0        0     1904 2024-04-20 04:44:36.652534 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      706 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/dynamic_port.py
--rwxr-xr-x   0        0        0     2161 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/on.py
--rwxr-xr-x   0        0        0     2200 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
--rwxr-xr-x   0        0        0     2957 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
--rwxr-xr-x   0        0        0     1441 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
--rwxr-xr-x   0        0        0      774 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
--rwxr-xr-x   0        0        0     1336 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      309 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      562 2024-04-20 04:44:37.516521 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      660 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      547 2024-04-20 04:44:37.504521 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      908 2024-04-20 04:44:37.504521 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
--rw-r--r--   0        0        0      636 2024-04-20 04:44:37.516521 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      289 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
--rwxr-xr-x   0        0        0      803 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
--rwxr-xr-x   0        0        0      378 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
--rwxr-xr-x   0        0        0      321 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
--rwxr-xr-x   0        0        0     2182 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
--rw-r--r--   0        0        0     2125 2024-04-20 04:44:37.516521 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1828 2024-04-20 04:44:37.524521 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0     2295 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
--rw-r--r--   0        0        0        2 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/start.py
--rwxr-xr-x   0        0        0      132 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
--rwxr-xr-x   0        0        0      152 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4699 2024-04-20 04:44:34.600566 biotech-1.1.6/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      374 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/intro/intro.S.HTML
--rwxr-xr-x   0        0        0     6305 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/intro/on.py
--rw-r--r--   0        0        0     2906 2024-04-20 04:44:35.492552 biotech-1.1.6/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
--rw-r--r--   0        0        0     4000 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/intro/process/adventure.py
--rw-r--r--   0        0        0     1330 2024-04-20 04:44:35.500552 biotech-1.1.6/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      905 2024-04-20 04:44:35.500552 biotech-1.1.6/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      959 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      614 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
--rwxr-xr-x   0        0        0      138 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/intro/process/intro.proc.py
--rwxr-xr-x   0        0        0     3084 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/intro/process/keg/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-20 04:44:35.492552 biotech-1.1.6/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       89 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/intro/process/variables/__init__.py
--rw-r--r--   0        0        0      245 2024-04-20 04:44:35.492552 biotech-1.1.6/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      172 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/procedures/procedures.S.HTML
--rwxr-xr-x   0        0        0      823 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
--rwxr-xr-x   0        0        0     3031 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
--rw-r--r--   0        0        0      933 2024-04-20 04:44:36.648534 biotech-1.1.6/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1061 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/aggregate/__init__.py
--rwxr-xr-x   0        0        0     1053 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      708 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/alarm_parser/__init__.py
--rw-r--r--   0        0        0      673 2024-04-20 04:44:36.644534 biotech-1.1.6/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1069 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      764 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/exceptions.py
--rwxr-xr-x   0        0        0     1190 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
--rwxr-xr-x   0        0        0     2446 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/__init__.py
--rw-r--r--   0        0        0     2491 2024-04-20 04:41:49.823732 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4471 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1050 2024-04-20 04:40:12.977620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     1920 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
--rwxr-xr-x   0        0        0       24 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
--rwxr-xr-x   0        0        0       24 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
--rwxr-xr-x   0        0        0      751 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
--rwxr-xr-x   0        0        0     1981 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/__init__.py
--rw-r--r--   0        0        0     2283 2024-04-20 04:41:49.835732 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4019 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3843 2024-04-20 04:44:34.576567 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
--rwxr-xr-x   0        0        0     4426 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
--rwxr-xr-x   0        0        0     3559 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/treasury.py
--rwxr-xr-x   0        0        0     1727 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/help_documentation/shares.s.HTML
--rwxr-xr-x   0        0        0     1055 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1558 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/implicit/proc/__init__.py
--rwxr-xr-x   0        0        0     1158 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/implicit/thread/__init__.py
--rw-r--r--   0        0        0      855 2024-04-20 04:44:34.624566 biotech-1.1.6/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       90 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
--rw-r--r--   0        0        0      731 2024-04-20 04:44:35.492552 biotech-1.1.6/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
--rwxr-xr-x   0        0        0      470 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/printout/bracket.py
--rwxr-xr-x   0        0        0      740 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/printout/passes.py
--rwxr-xr-x   0        0        0     2261 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2166 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/__init__.py
--rw-r--r--   0        0        0     1997 2024-04-20 04:44:34.600566 biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     2184 2024-04-20 04:44:34.604566 biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
--rw-r--r--   0        0        0      919 2024-04-20 04:44:36.648534 biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
--rwxr-xr-x   0        0        0      195 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/process_on/process_on.S.HTML
--rw-r--r--   0        0        0     1093 2024-04-20 04:44:36.652534 biotech-1.1.6/venues/stages/biotech/topics/process_on/sub/__pycache__/implicit.cpython-310.pyc
--rw-r--r--   0        0        0      832 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/process_on/sub/explicit.py
--rw-r--r--   0        0        0     1015 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/process_on/sub/implicit.py
--rwxr-xr-x   0        0        0     1470 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/quay/garage.py
--rwxr-xr-x   0        0        0     2546 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/quay/implicit_process_test_1.py
--rwxr-xr-x   0        0        0     1612 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/quay/implicit_process_test_2.py
--rwxr-xr-x   0        0        0      551 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/quay/implicit_process_test_3.py
--rwxr-xr-x   0        0        0     1083 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/quay/implicit_process_test_4.py
--rwxr-xr-x   0        0        0     1448 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
--rw-r--r--   0        0        0     1464 2024-04-20 04:44:36.652534 biotech-1.1.6/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      274 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
--rw-r--r--   0        0        0      246 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/report_formats/report_formats.S.HTML
--rw-r--r--   0        0        0     1772 2024-04-20 04:44:34.604566 biotech-1.1.6/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0      461 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/show/show.S.HTML
--rwxr-xr-x   0        0        0     2295 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/show/variable.py
--rwxr-xr-x   0        0        0      654 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
--rwxr-xr-x   0        0        0      454 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
--rwxr-xr-x   0        0        0      273 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/start--/one.py
--rwxr-xr-x   0        0        0      406 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/start--/sequentially.py
--rwxr-xr-x   0        0        0      532 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/start--/simultaneously.py
--rwxr-xr-x   0        0        0       76 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/topics/topics.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-20 04:40:12.981620 biotech-1.1.6/venues/stages/biotech/variables/__init__.py
--rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0      211 2024-04-20 04:40:12.925620 biotech-1.1.7/license.S.HTML
+-rwxr-xr-x   0        0        0     1144 2024-04-22 01:19:00.612990 biotech-1.1.7/pyproject.toml
+-rwxr-xr-x   0        0        0     3866 2024-04-20 04:40:12.929620 biotech-1.1.7/readme.md
+-rwxr-xr-x   0        0        0     1353 2024-04-22 01:00:02.912088 biotech-1.1.7/venue.S.HTML
+-rwxr-xr-x   0        0        0   838272 2024-04-20 04:40:12.929620 biotech-1.1.7/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
+-rwxr-xr-x   0        0        0     1270 2024-04-20 04:40:12.929620 biotech-1.1.7/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
+-rwxr-xr-x   0        0        0     4125 2024-04-20 04:40:12.929620 biotech-1.1.7/venues/stages/biotech/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      663 2024-04-22 01:17:56.413671 biotech-1.1.7/venues/stages/biotech/___itinerary/maybes.s.HTML
+-rwxr-xr-x   0        0        0      190 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout/script.py
+-rwxr-xr-x   0        0        0     1255 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout/start.py
+-rwxr-xr-x   0        0        0      189 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
+-rwxr-xr-x   0        0        0      186 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
+-rwxr-xr-x   0        0        0      190 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
+-rwxr-xr-x   0        0        0     1141 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
+-rwxr-xr-x   0        0        0      385 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/__glossary/biotech_1
+-rwxr-xr-x   0        0        0      114 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/__glossary/glossary.S.HTML
+-rwxr-xr-x   0        0        0      130 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/__init__.py
+-rwxr-xr-x   0        0        0    37279 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0     1252 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_book/advanced tutorial.s.HTML
+-rwxr-xr-x   0        0        0     1786 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_book/book.s.HTML
+-rwxr-xr-x   0        0        0      542 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_book/relevant.s.HTML
+-rwxr-xr-x   0        0        0     2007 2024-04-22 00:54:52.470209 biotech-1.1.7/venues/stages/biotech/_clique/__init__.py
+-rw-r--r--   0        0        0     2334 2024-04-22 01:02:39.250779 biotech-1.1.7/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4457 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      691 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0  1436985 2024-04-22 01:04:15.725916 biotech-1.1.7/venues/stages/biotech/_status/DB/records.json
+-rw-r--r--   0        0        0     1172 2024-04-20 04:44:34.660565 biotech-1.1.7/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1589 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1116 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1487 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/establish.py
+-rwxr-xr-x   0        0        0       83 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      720 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/-01_start/status_1.py
+-rwxr-xr-x   0        0        0      101 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/00_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      793 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/00_start/status_1.py
+-rwxr-xr-x   0        0        0      282 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/01/stasis/path_1_health.py
+-rwxr-xr-x   0        0        0      265 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/01/stasis/path_2_health.py
+-rwxr-xr-x   0        0        0     1161 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/01/status_1.py
+-rwxr-xr-x   0        0        0      321 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/02/stasis/1_health.py
+-rwxr-xr-x   0        0        0        2 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/02/stasis/2_health.py
+-rwxr-xr-x   0        0        0       50 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/02/stasis/modules/MODULE_1.py
+-rwxr-xr-x   0        0        0     1214 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/02/status_1.py
+-rwxr-xr-x   0        0        0      794 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py
+-rwxr-xr-x   0        0        0       35 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      939 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      289 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      942 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      518 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py
+-rwxr-xr-x   0        0        0      155 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      867 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/05__file__/status_1.py
+-rwxr-xr-x   0        0        0      311 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/06_various/stasis/1_health.py
+-rwxr-xr-x   0        0        0       31 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/06_various/stasis/2_health.py
+-rwxr-xr-x   0        0        0        0 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/06_various/stasis/3_health.py
+-rwxr-xr-x   0        0        0      955 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/06_various/status_1.py
+-rwxr-xr-x   0        0        0      160 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/07/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0      809 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/07/status_1.py
+-rwxr-xr-x   0        0        0       73 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/08_DB/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0     1561 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/08_DB/status_1.py
+-rwxr-xr-x   0        0        0   103233 2024-04-22 01:03:50.394146 biotech-1.1.7/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      119 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0      124 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_2.py
+-rwxr-xr-x   0        0        0        7 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_3.py
+-rwxr-xr-x   0        0        0     1442 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py
+-rw-r--r--   0        0        0      357 2024-04-20 04:45:57.075380 biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1189 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
+-rw-r--r--   0        0        0      316 2024-04-20 04:46:07.863238 biotech-1.1.7/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       77 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1250 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/11/status_1.py
+-rwxr-xr-x   0        0        0      984 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/status.proc.py
+-rwxr-xr-x   0        0        0      256 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/status.s.HTML
+-rwxr-xr-x   0        0        0     1483 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0      406 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
+-rwxr-xr-x   0        0        0      358 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
+-rwxr-xr-x   0        0        0   542989 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/_status_advanced/status.proc.py
+-rwxr-xr-x   0        0        0     1772 2024-04-21 23:18:15.551401 biotech-1.1.7/venues/stages/biotech/architecture.s.HTML
+-rwxr-xr-x   0        0        0      241 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/emojis.S.HTML
+-rwxr-xr-x   0        0        0      286 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/license.S.HTML
+-rwxr-xr-x   0        0        0     3068 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/module.s.HTML
+-rw-r--r--   0        0        0     1596 2024-04-20 04:44:35.492552 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      640 2024-04-20 04:44:35.500552 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      259 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
+-rwxr-xr-x   0        0        0     1478 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      366 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/paths.py
+-rwxr-xr-x   0        0        0      666 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
+-rwxr-xr-x   0        0        0      562 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
+-rw-r--r--   0        0        0     1165 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4141 2024-04-20 21:08:19.573336 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
+-rw-r--r--   0        0        0     3925 2024-04-20 21:08:23.925315 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      999 2024-04-20 04:44:36.652534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0     2881 2024-04-20 21:08:11.873375 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
+-rw-r--r--   0        0        0     1152 2024-04-20 04:44:36.652534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      653 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
+-rwxr-xr-x   0        0        0     3566 2024-04-20 20:59:25.531411 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
+-rwxr-xr-x   0        0        0      769 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
+-rw-r--r--   0        0        0     2031 2024-04-20 04:44:36.644534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
+-rw-r--r--   0        0        0     2159 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      420 2024-04-20 04:44:36.644534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
+-rw-r--r--   0        0        0      728 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3451 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
+-rwxr-xr-x   0        0        0     3235 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
+-rwxr-xr-x   0        0        0      193 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
+-rwxr-xr-x   0        0        0      514 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
+-rwxr-xr-x   0        0        0     2440 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
+-rw-r--r--   0        0        0     2352 2024-04-20 04:44:36.644534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      849 2024-04-20 21:06:01.973995 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
+-rw-r--r--   0        0        0     4019 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
+-rw-r--r--   0        0        0     1634 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
+-rw-r--r--   0        0        0     2916 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/no_records.py
+-rwxr-xr-x   0        0        0      754 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
+-rw-r--r--   0        0        0     1826 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1128 2024-04-20 21:04:00.238519 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
+-rwxr-xr-x   0        0        0     8732 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
+-rwxr-xr-x   0        0        0     3652 2024-04-20 21:04:51.502306 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
+-rw-r--r--   0        0        0     2202 2024-04-20 21:06:01.969995 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      834 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-20 04:45:40.247606 biotech-1.1.7/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      648 2024-04-20 04:44:36.652534 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
+-rw-r--r--   0        0        0     1904 2024-04-20 04:44:36.652534 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      706 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/dynamic_port.py
+-rwxr-xr-x   0        0        0     2161 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/on.py
+-rwxr-xr-x   0        0        0     2200 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
+-rwxr-xr-x   0        0        0     2957 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
+-rwxr-xr-x   0        0        0     1441 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
+-rwxr-xr-x   0        0        0      774 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
+-rwxr-xr-x   0        0        0     1336 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      309 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      562 2024-04-20 04:44:37.516521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      660 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      547 2024-04-20 04:44:37.504521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2024-04-20 04:44:37.504521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
+-rw-r--r--   0        0        0      636 2024-04-20 04:44:37.516521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      289 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
+-rwxr-xr-x   0        0        0      803 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
+-rwxr-xr-x   0        0        0      378 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
+-rwxr-xr-x   0        0        0      321 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
+-rwxr-xr-x   0        0        0     2182 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
+-rw-r--r--   0        0        0     2125 2024-04-20 04:44:37.516521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1828 2024-04-20 04:44:37.524521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2295 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
+-rw-r--r--   0        0        0        2 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/start.py
+-rwxr-xr-x   0        0        0      132 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
+-rwxr-xr-x   0        0        0      152 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4699 2024-04-20 04:44:34.600566 biotech-1.1.7/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      374 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/intro.S.HTML
+-rwxr-xr-x   0        0        0     6305 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/on.py
+-rw-r--r--   0        0        0     2906 2024-04-20 04:44:35.492552 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
+-rw-r--r--   0        0        0     4000 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/adventure.py
+-rw-r--r--   0        0        0     1330 2024-04-20 04:44:35.500552 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      905 2024-04-20 04:44:35.500552 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      959 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      614 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
+-rwxr-xr-x   0        0        0      138 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/intro.proc.py
+-rwxr-xr-x   0        0        0     3084 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/keg/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-20 04:44:35.492552 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       89 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/variables/__init__.py
+-rw-r--r--   0        0        0      245 2024-04-20 04:44:35.492552 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      172 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/procedures.S.HTML
+-rwxr-xr-x   0        0        0      823 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3031 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
+-rw-r--r--   0        0        0      933 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1061 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/aggregate/__init__.py
+-rwxr-xr-x   0        0        0     1053 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      708 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-20 04:44:36.644534 biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1069 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      764 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/exceptions.py
+-rwxr-xr-x   0        0        0     1190 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
+-rwxr-xr-x   0        0        0     2446 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__init__.py
+-rw-r--r--   0        0        0     2491 2024-04-20 04:41:49.823732 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4471 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1050 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1920 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
+-rwxr-xr-x   0        0        0       24 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
+-rwxr-xr-x   0        0        0       24 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
+-rwxr-xr-x   0        0        0      751 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
+-rwxr-xr-x   0        0        0     1981 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__init__.py
+-rw-r--r--   0        0        0     2283 2024-04-20 04:41:49.835732 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4019 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3843 2024-04-20 04:44:34.576567 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4426 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3559 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/treasury.py
+-rwxr-xr-x   0        0        0     1727 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/shares.s.HTML
+-rwxr-xr-x   0        0        0     1055 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1558 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/implicit/proc/__init__.py
+-rwxr-xr-x   0        0        0     1158 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/implicit/thread/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-20 04:44:34.624566 biotech-1.1.7/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       90 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
+-rw-r--r--   0        0        0      731 2024-04-20 04:44:35.492552 biotech-1.1.7/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
+-rwxr-xr-x   0        0        0      470 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/printout/bracket.py
+-rwxr-xr-x   0        0        0      740 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/printout/passes.py
+-rwxr-xr-x   0        0        0     2261 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2166 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__init__.py
+-rw-r--r--   0        0        0     1997 2024-04-20 04:44:34.600566 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     2184 2024-04-20 04:44:34.604566 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
+-rw-r--r--   0        0        0      919 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
+-rwxr-xr-x   0        0        0      195 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/process_on.S.HTML
+-rw-r--r--   0        0        0      832 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/sub/explicit.py
+-rw-r--r--   0        0        0     1015 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/sub/implicit.py
+-rwxr-xr-x   0        0        0     1470 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/quay/garage.py
+-rwxr-xr-x   0        0        0     2546 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_1.py
+-rwxr-xr-x   0        0        0     1612 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_2.py
+-rwxr-xr-x   0        0        0      551 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_3.py
+-rwxr-xr-x   0        0        0     1083 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_4.py
+-rwxr-xr-x   0        0        0     1448 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
+-rw-r--r--   0        0        0     1464 2024-04-20 04:44:36.652534 biotech-1.1.7/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      274 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/report_formats/report_formats.S.HTML
+-rw-r--r--   0        0        0     1772 2024-04-20 04:44:34.604566 biotech-1.1.7/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0      461 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/show/show.S.HTML
+-rwxr-xr-x   0        0        0     2295 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/show/variable.py
+-rwxr-xr-x   0        0        0      654 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
+-rwxr-xr-x   0        0        0      454 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
+-rwxr-xr-x   0        0        0      567 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
+-rwxr-xr-x   0        0        0      273 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/one.py
+-rwxr-xr-x   0        0        0      406 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/sequentially.py
+-rwxr-xr-x   0        0        0      532 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/simultaneously.py
+-rwxr-xr-x   0        0        0       76 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/topics.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/variables/__init__.py
+-rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.7/PKG-INFO
```

### Comparing `biotech-1.1.6/pyproject.toml` & `biotech-1.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 [tool.poetry]
 name = "biotech"
-version = "1.1.6"
+version = "1.1.7"
 description = "A health monitoring stack"
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "biotech", from = "venues/stages" }
 ]
@@ -49,15 +49,14 @@
 
 	"augmentation",
 	"enhancement",
 	"improvements"
 ]
 
 
-
 [tool.poetry.dependencies]
 python = "^3.10"
 body-scan = "^1.1.1"
 botanist = "^1.0.0"
 click = "^8.1.7"
 coverage = "^7.4.4"
 flask = "^3.0.3"
```

### Comparing `biotech-1.1.6/readme.md` & `biotech-1.1.7/readme.md`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg` & `biotech-1.1.7/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML` & `biotech-1.1.7/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/___itinerary/itinerary.S.HTML` & `biotech-1.1.7/venues/stages/biotech/___itinerary/itinerary.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/___itinerary/maybes.s.HTML` & `biotech-1.1.7/venues/stages/biotech/___itinerary/maybes.s.HTML`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 <pre>
 
 
 	maybes:
 		[ ] linter:
 			[ ] https://docs.astral.sh/ruff/
 			[ ] https://pypi.org/project/ruff/
-			[ ] https://black.readthedocs.io/en/stable/
 			
 		[ ] static typing:
 			[ ] mypy
 		
 		https://github.com/PyCQA/flake8
 		
 		
@@ -33,8 +32,10 @@
 		
 				cwd of each process = directory that the status file is in...
 		
 		[ ] { "aliases", "binaries" } for processes		
 				
 			or you can just find the absolute path...	
 				
+		[ ] https://github.com/sparckles/robyn?tab=readme-ov-file
+				
 </pre>
```

### Comparing `biotech-1.1.6/venues/stages/biotech/___itinerary/processes/errout/start.py` & `biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/___itinerary/processes/errout_v2/start.py` & `biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/__license/options/gpl-3.0-standalone.html` & `biotech-1.1.7/venues/stages/biotech/__license/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_book/advanced tutorial.s.HTML` & `biotech-1.1.7/venues/stages/biotech/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_book/book.s.HTML` & `biotech-1.1.7/venues/stages/biotech/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_book/relevant.s.HTML` & `biotech-1.1.7/venues/stages/biotech/_book/relevant.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_clique/__init__.py` & `biotech-1.1.7/venues/stages/biotech/_clique/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 
 
-print ('biotech')
+#print ('biotech')
 
+#
+#
+import biotech
 import biotech.topics.help_documentation as help_documentation
-	
+import biotech._status.establish as establish_status
+#
+#
 import click	
-	
+#
+#
 import pathlib
 import time
 from os.path import dirname, join, normpath
+import os
+#
+#
 
 def the_help_procedure (
 	port = ""
 ):
 	this_directory = pathlib.Path (__file__).parent.resolve ()
 	this_module = str (normpath (join (this_directory, "..")))
 
@@ -38,53 +47,45 @@
 	@click.option ('--port', default = "20000")
 	def help (port):
 		the_help_procedure (port)
 		
 	@click.command ("internal-status")
 	@click.option ('--glob-string', default = "")
 	def biotech_biotech (glob_string):
-
 		if (len (glob_string) >= 1):
-			import pathlib
-			from os.path import dirname, join, normpath
 			this_folder = pathlib.Path (__file__).parent.resolve ()
 
 			structures = normpath (join (this_folder, "../../.."))
 			monitors = str (normpath (join (this_folder, "..")))
 	
 			glob_string = monitors + "/" + glob_string
 	
-		import biotech._status.establish as establish_status
 		establish_status.start (
 			glob_string = glob_string
 		)
 	
 
 	@click.command ("status")
 	@click.option ('--simultaneous', default = "yes")
 	@click.option ('--glob-string', default = "/**/status_*.py")
 	def status (simultaneous, glob_string):
-		import pathlib
-		from os.path import dirname, join, normpath
 		this_directory = pathlib.Path (__file__).parent.resolve ()
 		this_module = str (normpath (join (this_directory, "..")))
 
-		import os
 		CWD = os.getcwd ()
 		
 		if (simultaneous == "yes"):
 			simultaneous_bool = True
 		elif (simultaneous == "no"):
 			simultaneous_bool = False
 		else:
 			print ("'--simultaneous yes' or '--simultaneous no'")
 			exit ()
 			
 
-		import biotech
 		biotech.start (
 			glob_string = CWD + glob_string,
 			simultaneous = simultaneous
 		)
 
 
 	group.add_command (help)
```

### Comparing `biotech-1.1.6/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/DB/records.json` & `biotech-1.1.7/venues/stages/biotech/_status/DB/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975124378109452%*

 * *Differences: {"'_default'": "{'401': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'_status/monitors/-01_start/status_1.py'), ('empty', False), ('parsed', True), "*

 * *               "('stats', OrderedDict([('passes', 1), ('alarms', 0)])), ('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('passed', True), ('elapsed', "*

 * *               "[6.090184608001437, 'seconds'])])])]), OrderedDict([('path', "*

 * *               "'_status/monitors/00_start/status_1.py'), ('empty', False), ('parsed', True), " […]*

```diff
@@ -55081,14 +55081,572 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 14
                 },
                 "empty": 0
             }
         },
+        "401": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.090184608001437,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-01_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.06965271899935,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/00_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.166153869000482,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/01/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.089839799999027,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/02/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.133875969999281,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/03_empty_glob/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.079449643000771,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.0_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.081750616998761,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.1_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.148715408000498,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/05__file__/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.067526546001318,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.168750250000812,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/07/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "tinyDB database can be utilized",
+                            "elapsed": [
+                                6.178109918999326,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/08_DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.086354699000367,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/09_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                10.103048934999606,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/10_time_limits/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.056221467999421,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/11/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 14
+                },
+                "empty": 0
+            }
+        },
+        "402": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.069437695998204,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-01_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.086694315999921,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/00_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.148998116001167,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/01/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.060186165999767,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/02/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                4.1231546599992726,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/03_empty_glob/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.091005686001154,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.0_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.08395776800171,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/04.1_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.168502227999852,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/05__file__/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.059685883999919,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/06_various/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                6.134682105999673,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/07/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "tinyDB database can be utilized",
+                            "elapsed": [
+                                6.212993906003248,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/08_DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.116894830000092,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/09_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                10.120352387999446,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/10_time_limits/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                6.09040485499645,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/11/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 14
+                },
+                "empty": 0
+            }
+        },
         "41": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
```

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/establish.py` & `biotech-1.1.7/venues/stages/biotech/_status/establish.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/-01_start/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/-01_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/00_start/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/00_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/01/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/01/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/02/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/02/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/05__file__/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/05__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/06_various/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/06_various/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/07/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/07/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/08_DB/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/08_DB/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959016393442623%*

 * *Differences: {"'_default'": "{'243': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [1.278300078411121e-05, 'seconds']), ('passed', True)])]), "*

 * *               "('empty', False), ('parsed', True), ('path', 'guarantee_1.py'), ('records', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('passes', 1)]))])]), ('alarms', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('checks', OrderedDict([('alarms', 0), "*

 * *               "('passes' […]*

```diff
@@ -6053,14 +6053,80 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
         },
+        "243": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.278300078411121e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "guarantee_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "244": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.7491001674206927e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "guarantee_1.py",
+                    "records": [],
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
         "25": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
```

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/monitors/11/status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status/monitors/11/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status/status.proc.py` & `biotech-1.1.7/venues/stages/biotech/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py` & `biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json` & `biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/_status_advanced/status.proc.py` & `biotech-1.1.7/venues/stages/biotech/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/architecture.s.HTML` & `biotech-1.1.7/venues/stages/biotech/architecture.s.HTML`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 p {
 	display: inline;
 	font-size: 1.5em;
 }
 
 </style>
 <pre>
-	
 
 	<h1>The Architecture</h1>
 	
 	<h2>Important</h2>
 	<p>
 		Don't use "biotech" for these modules,
 		
@@ -64,15 +63,14 @@
 		
 			As in, biotech perhaps shouldn't include a module that
 			requires biotech for status assertation.
 		
 			Therefore the directed acyclic chart of status check frameworks is:
 				
 				[ unit test, pytest ] -> "body_scan" -> biotech
-				
 			
 			
 				
 	</p>
 	
 	<h2>The Structure</h2>
 		<h3>
```

#### html2text {}

```diff
@@ -1,8 +1,7 @@
-	
 
 	
 ************ TThhee AArrcchhiitteeccttuurree ************
 
 	
 	
 ********** IImmppoorrttaanntt **********
@@ -30,15 +29,14 @@
 		
 			As in, biotech perhaps shouldn't include a module that
 			requires biotech for status assertation.
 		
 			Therefore the directed acyclic chart of status check frameworks is:
 				
 				[ unit test, pytest ] -> "body_scan" -> biotech
-
```

### Comparing `biotech-1.1.6/venues/stages/biotech/module.s.HTML` & `biotech-1.1.7/venues/stages/biotech/module.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/on.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,26 +49,43 @@
 		This is what starts the aggregator
 	'''
 	paths_patch (app, aggregator_procedure_port = port)
 
 	@app.route ("/", methods = [ 'GET' ])
 	def home_get ():	
 		return jsonify ({
-			'/health_scan/<path:health_scan_path>': [ "get" ],
-			'/health_scans/paths': [ "get" ],
+			'/data/health_scan/<path:health_scan_path>': [ "get" ],
+			'/data/health_scans/paths': [ "get" ],
 			'/on': [ "get" ],
 			'/anomalies': [ "get" ]
 		})
 
 
 	@app.route ("/on", methods = [ 'GET' ])
 	def on_get ():	
 		return "yes"
 		
-	@app.route ("/anomalies", methods = [ 'GET' ])
+	@app.route ("/data/proceeds", methods = [ 'GET' ])
+	def on_data_proceeds ():	
+		try:
+			aggregator_variables = retrieve_aggregator_variables ()
+			
+			return jsonify ({
+				"proceeds built": aggregator_variables ["proceeds_built"],
+				"proceeds": aggregator_variables ["proceeds"]
+			})			
+			
+		except Exception as E:
+			print (E)
+		
+			pass;
+	
+		return "not parseable"	
+		
+	@app.route ("/data/anomalies", methods = [ 'GET' ])
 	def on_anomalies ():	
 		try:
 			aggregator_variables = retrieve_aggregator_variables ()
 			
 			exception_count = 0
 			parsed_anomalies = []
 			unparsed_anomalies = aggregator_variables ["anomalies"]
@@ -91,21 +108,20 @@
 			
 		
 			pass;
 			
 		return "not parseable"
 
 
-	@app.route ("/waiting_for", methods = [ 'GET' ])
+	@app.route ("/data/waiting_for", methods = [ 'GET' ])
 	def on_waiting_for ():	
 		try:
 			aggregator_variables = retrieve_aggregator_variables ()
 			internal_statuses = aggregator_variables ["internal_statuses"]
 
-			
 			waiting_for = []
 			for status_path in internal_statuses:
 				occurrences = "not parseable"
 				try:
 					occurrences = aggregator_variables ["internal_statuses"] [ status_path ] ["occurrences"]
 				except Exception:
 					pass;
@@ -139,26 +155,26 @@
 			pass;
 			
 		return "not parseable"
 	
 	
 
 	
-	@app.route ('/health_scans/paths', methods = [ 'GET' ])
+	@app.route ('/data/health_scans/paths', methods = [ 'GET' ])
 	def on__get__health_scans__paths ():	
 		aggregator_variables = retrieve_aggregator_variables ()
 		
 		the_paths = {}
 		
 		for path in aggregator_variables ["internal_statuses"]:
 			the_paths [ path ] = ""
 	
 		return jsonify (the_paths)
 		
-	@app.route ('/health_scan/<path:health_scan_path>', methods = [ 'GET' ])
+	@app.route ('/data/health_scan/<path:health_scan_path>', methods = [ 'GET' ])
 	def on__get__health_scan__path (health_scan_path):	
 		return "yes"
 	
 	
 	the_health_scan_started (app)
 	
 	done_with_scan (app)
```

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 20 04:49:29 2024 UTC, .py size: 3738 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5949 2366 9a0e 0000  o.......YI#f....
+00000000: 6f0d 0d0a 0000 0000 c32e 2466 2d10 0000  o.........$f-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6405 6406 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6407 6c07 6d09 5a09 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6408 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  d.l.m.Z.m.Z.m.Z.
@@ -26,197 +26,221 @@
 00000190: 0000 2901 da1d 7265 7472 6965 7665 5f61  ..)...retrieve_a
 000001a0: 6767 7265 6761 746f 725f 7661 7269 6162  ggregator_variab
 000001b0: 6c65 7329 01da 0b61 6464 5f61 6e6f 6d61  les)...add_anoma
 000001c0: 6c79 2903 da05 466c 6173 6bda 0772 6571  ly)...Flask..req
 000001d0: 7565 7374 da07 6a73 6f6e 6966 794e 2903  uest..jsonifyN).
 000001e0: da07 6469 726e 616d 65da 046a 6f69 6eda  ..dirname..join.
 000001f0: 086e 6f72 6d70 6174 6863 0200 0000 0000  .normpathc......
-00000200: 0000 0000 0000 0900 0000 0500 0000 4300  ..............C.
-00000210: 0000 73dc 0000 007c 0164 016b 0572 0974  ..s....|.d.k.r.t
+00000200: 0000 0000 0000 0a00 0000 0500 0000 4300  ..............C.
+00000210: 0000 73f4 0000 007c 0164 016b 0572 0974  ..s....|.d.k.r.t
 00000220: 0064 027c 0083 0201 0074 0164 0383 017d  .d.|.....t.d...}
 00000230: 0209 0074 027c 027c 0064 048d 0201 007c  ...t.|.|.d.....|
 00000240: 026a 0364 0564 0667 0164 078d 0264 0864  .j.d.d.g.d...d.d
 00000250: 0984 0083 017d 037c 026a 0364 0a64 0667  .....}.|.j.d.d.g
 00000260: 0164 078d 0264 0b64 0c84 0083 017d 047c  .d...d.d.....}.|
 00000270: 026a 0364 0d64 0667 0164 078d 0264 0e64  .j.d.d.g.d...d.d
 00000280: 0f84 0083 017d 057c 026a 0364 1064 0667  .....}.|.j.d.d.g
 00000290: 0164 078d 0264 1164 1284 0083 017d 067c  .d...d.d.....}.|
 000002a0: 026a 0364 1364 0667 0164 078d 0264 1464  .j.d.d.g.d...d.d
 000002b0: 1584 0083 017d 077c 026a 0364 1664 0667  .....}.|.j.d.d.g
-000002c0: 0164 078d 0264 1764 1884 0083 017d 0874  .d...d.d.....}.t
-000002d0: 047c 0283 0101 0074 057c 0283 0101 007c  .|.....t.|.....|
-000002e0: 026a 0664 197c 0064 1a64 1b8d 0301 0064  .j.d.|.d.d.....d
-000002f0: 0053 0029 1c4e 7201 0000 007a 216f 7065  .S.).Nr....z!ope
-00000300: 6e69 6e67 2073 6361 6e20 7072 6f63 6573  ning scan proces
-00000310: 7320 6b65 6720 6f6e 2070 6f72 743a 7a11  s keg on port:z.
-00000320: 6167 6772 6567 6174 6f72 2068 6172 626f  aggregator harbo
-00000330: 7229 01da 1961 6767 7265 6761 746f 725f  r)...aggregator_
-00000340: 7072 6f63 6564 7572 655f 706f 7274 fa01  procedure_port..
-00000350: 2fda 0347 4554 2901 da07 6d65 7468 6f64  /..GET)...method
-00000360: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
-00000370: 0000 0600 0000 5300 0000 731a 0000 0074  ......S...s....t
-00000380: 0064 0167 0164 0167 0164 0167 0164 0167  .d.g.d.g.d.g.d.g
-00000390: 0164 029c 0483 0153 0029 034e da03 6765  .d.....S.).N..ge
-000003a0: 7429 04fa 242f 6865 616c 7468 5f73 6361  t)..$/health_sca
-000003b0: 6e2f 3c70 6174 683a 6865 616c 7468 5f73  n/<path:health_s
-000003c0: 6361 6e5f 7061 7468 3efa 132f 6865 616c  can_path>../heal
-000003d0: 7468 5f73 6361 6e73 2f70 6174 6873 fa03  th_scans/paths..
-000003e0: 2f6f 6efa 0a2f 616e 6f6d 616c 6965 7329  /on../anomalies)
-000003f0: 0172 0a00 0000 a900 7217 0000 0072 1700  .r......r....r..
-00000400: 0000 fa56 2f62 696f 7465 6368 2f76 656e  ...V/biotech/ven
-00000410: 7565 732f 7374 6167 6573 2f62 696f 7465  ues/stages/biote
-00000420: 6368 2f70 726f 6365 6475 7265 732f 6167  ch/procedures/ag
-00000430: 6772 6567 6174 6f72 5f70 726f 6365 6475  gregator_procedu
-00000440: 7265 2f70 726f 6365 7373 2f6b 6567 2f5f  re/process/keg/_
-00000450: 5f69 6e69 745f 5f2e 7079 da08 686f 6d65  _init__.py..home
-00000460: 5f67 6574 3500 0000 730c 0000 0002 0204  _get5...s.......
-00000470: 0104 0104 0104 0108 fc7a 1d6f 7065 6e5f  .........z.open_
-00000480: 6861 7262 6f72 2e3c 6c6f 6361 6c73 3e2e  harbor.<locals>.
-00000490: 686f 6d65 5f67 6574 7215 0000 0063 0000  home_getr....c..
-000004a0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-000004b0: 0000 5300 0000 f304 0000 0064 0153 00a9  ..S........d.S..
-000004c0: 024e da03 7965 7372 1700 0000 7217 0000  .N..yesr....r...
-000004d0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
-000004e0: da06 6f6e 5f67 6574 3f00 0000 f302 0000  ..on_get?.......
-000004f0: 0004 027a 1b6f 7065 6e5f 6861 7262 6f72  ...z.open_harbor
-00000500: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f67 6574  .<locals>.on_get
-00000510: 7216 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000520: 0000 0600 0000 0b00 0000 5300 0000 73c0  ..........S...s.
-00000530: 0000 007a 4874 0083 007d 0064 017d 0167  ...zHt...}.d.}.g
-00000540: 007d 027c 0064 0219 007d 037c 0344 005d  .}.|.d...}.|.D.]
-00000550: 307d 047a 0c7c 02a0 0174 026a 037c 0364  0}.z.|...t.j.|.d
-00000560: 0364 048d 02a1 0101 0057 0071 0e04 0074  .d.......W.q...t
-00000570: 0479 3e01 007d 0501 007a 1674 0564 057c  .y>..}...z.t.d.|
-00000580: 0583 0201 0074 0564 0674 067c 0583 0183  .....t.d.t.|....
-00000590: 0201 007c 0164 0737 007d 0157 0059 0064  ...|.d.7.}.W.Y.d
-000005a0: 007d 057e 0571 0e64 007d 057e 0577 0177  .}.~.q.d.}.~.w.w
-000005b0: 0074 077c 0064 0219 007c 0164 089c 0283  .t.|.d...|.d....
-000005c0: 0157 0053 0004 0074 0479 5f01 007d 0501  .W.S...t.y_..}..
-000005d0: 007a 0b74 057c 0583 0101 0057 0059 0064  .z.t.|.....W.Y.d
-000005e0: 007d 057e 0564 0953 0064 007d 057e 0577  .}.~.d.S.d.}.~.w
-000005f0: 0177 0029 0a4e 7205 0000 00da 0961 6e6f  .w.).Nr......ano
-00000600: 6d61 6c69 6573 e904 0000 0029 01da 0669  malies.....)...i
-00000610: 6e64 656e 747a 1a61 6e6f 6d61 6c79 2070  ndentz.anomaly p
-00000620: 6172 7369 6e67 2065 7863 6570 7469 6f6e  arsing exception
-00000630: 3a7a 2161 6e6f 6d61 6c79 2070 6172 7369  :z!anomaly parsi
-00000640: 6e67 2073 7472 696e 6720 6578 6365 7074  ng string except
-00000650: 696f 6e3a 7201 0000 0029 0272 1f00 0000  ion:r....).r....
-00000660: da0f 6578 6365 7074 696f 6e5f 636f 756e  ..exception_coun
-00000670: 74fa 0d6e 6f74 2070 6172 7365 6162 6c65  t..not parseable
-00000680: 2908 7206 0000 00da 0661 7070 656e 64da  ).r......append.
-00000690: 046a 736f 6eda 0564 756d 7073 da09 4578  .json..dumps..Ex
-000006a0: 6365 7074 696f 6eda 0570 7269 6e74 da03  ception..print..
-000006b0: 7374 7272 0a00 0000 2906 da14 6167 6772  strr....)...aggr
-000006c0: 6567 6174 6f72 5f76 6172 6961 626c 6573  egator_variables
-000006d0: 7222 0000 00da 1070 6172 7365 645f 616e  r".....parsed_an
-000006e0: 6f6d 616c 6965 73da 1275 6e70 6172 7365  omalies..unparse
-000006f0: 645f 616e 6f6d 616c 6965 73da 0761 6e6f  d_anomalies..ano
-00000700: 6d61 6c79 da01 4572 1700 0000 7217 0000  maly..Er....r...
-00000710: 0072 1800 0000 da0c 6f6e 5f61 6e6f 6d61  .r......on_anoma
-00000720: 6c69 6573 4300 0000 7330 0000 0002 0206  liesC...s0......
-00000730: 0104 0204 0108 0108 0102 0118 010e 010a  ................
-00000740: 010e 0114 0208 8002 fc02 0606 0102 010a  ................
-00000750: fe0e 0508 010a 0304 0208 8002 fa7a 216f  .............z!o
-00000760: 7065 6e5f 6861 7262 6f72 2e3c 6c6f 6361  pen_harbor.<loca
-00000770: 6c73 3e2e 6f6e 5f61 6e6f 6d61 6c69 6573  ls>.on_anomalies
-00000780: 7a0c 2f77 6169 7469 6e67 5f66 6f72 6300  z./waiting_forc.
-00000790: 0000 0000 0000 0000 0000 0008 0000 000a  ................
-000007a0: 0000 0053 0000 0073 0801 0000 7a6b 7400  ...S...s....zkt.
-000007b0: 8300 7d00 7c00 6401 1900 7d01 6700 7d02  ..}.|.d...}.g.}.
-000007c0: 7c01 4400 5d58 7d03 6402 7d04 7a0a 7c00  |.D.]X}.d.}.z.|.
-000007d0: 6401 1900 7c03 1900 6403 1900 7d04 5700  d...|...d...}.W.
-000007e0: 6e09 0400 7401 7923 0100 0100 0100 5900  n...t.y#......Y.
-000007f0: 6e01 7700 6402 7d05 7a0a 7c00 6401 1900  n.w.d.}.z.|.d...
-00000800: 7c03 1900 6404 1900 7d05 5700 6e09 0400  |...d...}.W.n...
-00000810: 7401 7939 0100 0100 0100 5900 6e01 7700  t.y9......Y.n.w.
-00000820: 6402 7d06 7a0a 7c00 6401 1900 7c03 1900  d.}.z.|.d...|...
-00000830: 6405 1900 7d06 5700 6e09 0400 7401 794f  d...}.W.n...t.yO
-00000840: 0100 0100 0100 5900 6e01 7700 7c01 7c03  ......Y.n.w.|.|.
-00000850: 1900 6406 1900 6407 1900 6408 6b03 7264  ..d...d...d.k.rd
-00000860: 7c02 a002 7c03 7c04 7c05 7c06 6409 9c04  |...|.|.|.|.d...
-00000870: a101 0100 710c 7403 640a 7c02 6901 8301  ....q.t.d.|.i...
-00000880: 5700 5300 0400 7401 7983 0100 7d07 0100  W.S...t.y...}...
-00000890: 7a0c 7404 640b 7c07 8302 0100 5700 5900  z.t.d.|.....W.Y.
-000008a0: 6400 7d07 7e07 6402 5300 6400 7d07 7e07  d.}.~.d.S.d.}.~.
-000008b0: 7701 7700 290c 4eda 1169 6e74 6572 6e61  w.w.).N..interna
-000008c0: 6c5f 7374 6174 7573 6573 7223 0000 00da  l_statusesr#....
-000008d0: 0b6f 6363 7572 7265 6e63 6573 da07 7265  .occurrences..re
-000008e0: 636f 7264 73da 0574 696d 6573 da06 7374  cords..times..st
-000008f0: 6174 7573 da07 7072 6f63 6573 73da 0464  atus..process..d
-00000900: 6f6e 6529 04da 0470 6174 6872 3100 0000  one)...pathr1...
-00000910: 7232 0000 0072 3300 0000 da0b 7761 6974  r2...r3.....wait
-00000920: 696e 675f 666f 727a 0a65 7863 6570 7469  ing_forz.excepti
-00000930: 6f6e 3a29 0572 0600 0000 7227 0000 0072  on:).r....r'...r
-00000940: 2400 0000 720a 0000 0072 2800 0000 2908  $...r....r(...).
-00000950: 722a 0000 0072 3000 0000 7238 0000 00da  r*...r0...r8....
-00000960: 0b73 7461 7475 735f 7061 7468 7231 0000  .status_pathr1..
-00000970: 0072 3200 0000 7233 0000 0072 2e00 0000  .r2...r3...r....
-00000980: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
-00000990: 0e6f 6e5f 7761 6974 696e 675f 666f 7262  .on_waiting_forb
-000009a0: 0000 0073 5000 0000 0202 0601 0801 0403  ...sP...........
-000009b0: 0801 0401 0201 1401 0c01 0401 02ff 0403  ................
-000009c0: 0201 1401 0c01 0401 02ff 0403 0201 1401  ................
-000009d0: 0c01 0401 02ff 1403 0401 0201 0201 0201  ................
-000009e0: 0201 08fc 0280 0207 0401 08ff 0e04 0a01  ................
-000009f0: 0a01 0402 0880 02fc 7a23 6f70 656e 5f68  ........z#open_h
-00000a00: 6172 626f 722e 3c6c 6f63 616c 733e 2e6f  arbor.<locals>.o
-00000a10: 6e5f 7761 6974 696e 675f 666f 7272 1400  n_waiting_forr..
-00000a20: 0000 6300 0000 0000 0000 0000 0000 0003  ..c.............
-00000a30: 0000 0004 0000 0053 0000 0073 2800 0000  .......S...s(...
-00000a40: 7400 8300 7d00 6900 7d01 7c00 6401 1900  t...}.i.}.|.d...
-00000a50: 4400 5d06 7d02 6402 7c01 7c02 3c00 7109  D.].}.d.|.|.<.q.
-00000a60: 7401 7c01 8301 5300 2903 4e72 3000 0000  t.|...S.).Nr0...
-00000a70: da00 2902 7206 0000 0072 0a00 0000 2903  ..).r....r....).
-00000a80: 722a 0000 00da 0974 6865 5f70 6174 6873  r*.....the_paths
-00000a90: 7237 0000 0072 1700 0000 7217 0000 0072  r7...r....r....r
-00000aa0: 1800 0000 da1c 6f6e 5f5f 6765 745f 5f68  ......on__get__h
-00000ab0: 6561 6c74 685f 7363 616e 735f 5f70 6174  ealth_scans__pat
-00000ac0: 6873 9200 0000 730a 0000 0006 0204 020c  hs....s.........
-00000ad0: 020a 0108 027a 316f 7065 6e5f 6861 7262  .....z1open_harb
-00000ae0: 6f72 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f5f  or.<locals>.on__
-00000af0: 6765 745f 5f68 6561 6c74 685f 7363 616e  get__health_scan
-00000b00: 735f 5f70 6174 6873 7213 0000 0063 0100  s__pathsr....c..
-00000b10: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-00000b20: 0000 5300 0000 721a 0000 0072 1b00 0000  ..S...r....r....
-00000b30: 7217 0000 0029 01da 1068 6561 6c74 685f  r....)...health_
-00000b40: 7363 616e 5f70 6174 6872 1700 0000 7217  scan_pathr....r.
-00000b50: 0000 0072 1800 0000 da1a 6f6e 5f5f 6765  ...r......on__ge
-00000b60: 745f 5f68 6561 6c74 685f 7363 616e 5f5f  t__health_scan__
-00000b70: 7061 7468 9d00 0000 721e 0000 007a 2f6f  path....r....z/o
-00000b80: 7065 6e5f 6861 7262 6f72 2e3c 6c6f 6361  pen_harbor.<loca
-00000b90: 6c73 3e2e 6f6e 5f5f 6765 745f 5f68 6561  ls>.on__get__hea
-00000ba0: 6c74 685f 7363 616e 5f5f 7061 7468 7a07  lth_scan__pathz.
-00000bb0: 302e 302e 302e 3046 2902 da04 706f 7274  0.0.0.0F)...port
-00000bc0: da05 6465 6275 6729 0772 2800 0000 7208  ..debug).r(...r.
-00000bd0: 0000 0072 0300 0000 da05 726f 7574 6572  ...r......router
-00000be0: 0400 0000 7202 0000 00da 0372 756e 2909  ....r......run).
-00000bf0: 7240 0000 0072 3200 0000 da03 6170 7072  r@...r2.....appr
-00000c00: 1900 0000 721d 0000 0072 2f00 0000 723a  ....r....r/...r:
-00000c10: 0000 0072 3d00 0000 723f 0000 0072 1700  ...r=...r?...r..
-00000c20: 0000 7217 0000 0072 1800 0000 da0b 6f70  ..r....r......op
-00000c30: 656e 5f68 6172 626f 7225 0000 0073 3000  en_harbor%...s0.
-00000c40: 0000 0804 0a01 0804 0202 0c03 0e02 0a01  ................
-00000c50: 0e09 0a01 0e03 0a01 0e1e 0a01 0e2f 0a01  ............./..
-00000c60: 0e0a 0a01 0804 0802 0404 0201 0201 0201  ................
-00000c70: 0afd 7245 0000 0029 0272 0500 0000 7205  ..rE...).r....r.
-00000c80: 0000 0029 1ada 075f 5f64 6f63 5f5f da15  ...)...__doc__..
-00000c90: 7370 6163 6573 2e64 6f6e 655f 7769 7468  spaces.done_with
-00000ca0: 5f73 6361 6e72 0200 0000 da12 7370 6163  _scanr......spac
-00000cb0: 6573 2e70 6174 6873 5f70 6174 6368 7203  es.paths_patchr.
-00000cc0: 0000 00da 1e73 7061 6365 732e 7468 655f  .....spaces.the_
-00000cd0: 6865 616c 7468 5f73 6361 6e5f 7374 6172  health_scan_star
-00000ce0: 7465 6472 0400 0000 da39 6269 6f74 6563  tedr.....9biotec
-00000cf0: 682e 7072 6f63 6564 7572 6573 2e61 6767  h.procedures.agg
-00000d00: 7265 6761 746f 725f 7072 6f63 6564 7572  regator_procedur
-00000d10: 652e 7072 6f63 6573 732e 7661 7269 6162  e.process.variab
-00000d20: 6c65 7372 0600 0000 7207 0000 00da 0566  lesr....r......f
-00000d30: 6c61 736b 7208 0000 0072 0900 0000 720a  laskr....r....r.
-00000d40: 0000 00da 0472 6963 6872 2500 0000 da07  .....richr%.....
-00000d50: 7061 7468 6c69 62da 026f 73da 076f 732e  pathlib..os..os.
-00000d60: 7061 7468 720b 0000 0072 0c00 0000 720d  pathr....r....r.
-00000d70: 0000 00da 0373 7973 da09 7468 7265 6164  .....sys..thread
-00000d80: 696e 67da 0474 696d 6572 4500 0000 7217  ing..timerE...r.
-00000d90: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-00000da0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000db0: 7324 0000 0004 020c 0c0c 010c 010c 020c  s$..............
-00000dc0: 0114 0308 0108 0308 0108 0114 0108 0108  ................
-00000dd0: 0108 0102 0502 010e fe                   .........
+000002c0: 0164 078d 0264 1764 1884 0083 017d 087c  .d...d.d.....}.|
+000002d0: 026a 0364 1964 0667 0164 078d 0264 1a64  .j.d.d.g.d...d.d
+000002e0: 1b84 0083 017d 0974 047c 0283 0101 0074  .....}.t.|.....t
+000002f0: 057c 0283 0101 007c 026a 0664 1c7c 0064  .|.....|.j.d.|.d
+00000300: 1d64 1e8d 0301 0064 0053 0029 1f4e 7201  .d.....d.S.).Nr.
+00000310: 0000 007a 216f 7065 6e69 6e67 2073 6361  ...z!opening sca
+00000320: 6e20 7072 6f63 6573 7320 6b65 6720 6f6e  n process keg on
+00000330: 2070 6f72 743a 7a11 6167 6772 6567 6174   port:z.aggregat
+00000340: 6f72 2068 6172 626f 7229 01da 1961 6767  or harbor)...agg
+00000350: 7265 6761 746f 725f 7072 6f63 6564 7572  regator_procedur
+00000360: 655f 706f 7274 fa01 2fda 0347 4554 2901  e_port../..GET).
+00000370: da07 6d65 7468 6f64 7363 0000 0000 0000  ..methodsc......
+00000380: 0000 0000 0000 0000 0000 0600 0000 5300  ..............S.
+00000390: 0000 731a 0000 0074 0064 0167 0164 0167  ..s....t.d.g.d.g
+000003a0: 0164 0167 0164 0167 0164 029c 0483 0153  .d.g.d.g.d.....S
+000003b0: 0029 034e da03 6765 7429 04fa 292f 6461  .).N..get)..)/da
+000003c0: 7461 2f68 6561 6c74 685f 7363 616e 2f3c  ta/health_scan/<
+000003d0: 7061 7468 3a68 6561 6c74 685f 7363 616e  path:health_scan
+000003e0: 5f70 6174 683e fa18 2f64 6174 612f 6865  _path>../data/he
+000003f0: 616c 7468 5f73 6361 6e73 2f70 6174 6873  alth_scans/paths
+00000400: fa03 2f6f 6e7a 0a2f 616e 6f6d 616c 6965  ../onz./anomalie
+00000410: 7329 0172 0a00 0000 a900 7216 0000 0072  s).r......r....r
+00000420: 1600 0000 fa56 2f62 696f 7465 6368 2f76  .....V/biotech/v
+00000430: 656e 7565 732f 7374 6167 6573 2f62 696f  enues/stages/bio
+00000440: 7465 6368 2f70 726f 6365 6475 7265 732f  tech/procedures/
+00000450: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
+00000460: 6475 7265 2f70 726f 6365 7373 2f6b 6567  dure/process/keg
+00000470: 2f5f 5f69 6e69 745f 5f2e 7079 da08 686f  /__init__.py..ho
+00000480: 6d65 5f67 6574 3500 0000 730c 0000 0002  me_get5...s.....
+00000490: 0204 0104 0104 0104 0108 fc7a 1d6f 7065  ...........z.ope
+000004a0: 6e5f 6861 7262 6f72 2e3c 6c6f 6361 6c73  n_harbor.<locals
+000004b0: 3e2e 686f 6d65 5f67 6574 7215 0000 0063  >.home_getr....c
+000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004d0: 0100 0000 5300 0000 f304 0000 0064 0153  ....S........d.S
+000004e0: 00a9 024e da03 7965 7372 1600 0000 7216  ...N..yesr....r.
+000004f0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00000500: 0000 da06 6f6e 5f67 6574 3f00 0000 f302  ....on_get?.....
+00000510: 0000 0004 027a 1b6f 7065 6e5f 6861 7262  .....z.open_harb
+00000520: 6f72 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f67  or.<locals>.on_g
+00000530: 6574 7a0e 2f64 6174 612f 7072 6f63 6565  etz./data/procee
+00000540: 6473 6300 0000 0000 0000 0000 0000 0002  dsc.............
+00000550: 0000 000a 0000 0053 0000 0073 4e00 0000  .......S...sN...
+00000560: 7a0f 7400 8300 7d00 7401 7c00 6401 1900  z.t...}.t.|.d...
+00000570: 7c00 6402 1900 6403 9c02 8301 5700 5300  |.d...d.....W.S.
+00000580: 0400 7402 7926 0100 7d01 0100 7a0b 7403  ..t.y&..}...z.t.
+00000590: 7c01 8301 0100 5700 5900 6400 7d01 7e01  |.....W.Y.d.}.~.
+000005a0: 6404 5300 6400 7d01 7e01 7701 7700 2905  d.S.d.}.~.w.w.).
+000005b0: 4eda 0e70 726f 6365 6564 735f 6275 696c  N..proceeds_buil
+000005c0: 74da 0870 726f 6365 6564 7329 027a 0e70  t..proceeds).z.p
+000005d0: 726f 6365 6564 7320 6275 696c 7472 1f00  roceeds builtr..
+000005e0: 0000 fa0d 6e6f 7420 7061 7273 6561 626c  ....not parseabl
+000005f0: 6529 0472 0600 0000 720a 0000 00da 0945  e).r....r......E
+00000600: 7863 6570 7469 6f6e da05 7072 696e 7429  xception..print)
+00000610: 02da 1461 6767 7265 6761 746f 725f 7661  ...aggregator_va
+00000620: 7269 6162 6c65 73da 0145 7216 0000 0072  riables..Er....r
+00000630: 1600 0000 7217 0000 00da 106f 6e5f 6461  ....r......on_da
+00000640: 7461 5f70 726f 6365 6564 7343 0000 0073  ta_proceedsC...s
+00000650: 1800 0000 0202 0601 0202 0601 0601 0afe  ................
+00000660: 0e05 0801 0a02 0402 0880 02fb 7a25 6f70  ............z%op
+00000670: 656e 5f68 6172 626f 722e 3c6c 6f63 616c  en_harbor.<local
+00000680: 733e 2e6f 6e5f 6461 7461 5f70 726f 6365  s>.on_data_proce
+00000690: 6564 737a 0f2f 6461 7461 2f61 6e6f 6d61  edsz./data/anoma
+000006a0: 6c69 6573 6300 0000 0000 0000 0000 0000  liesc...........
+000006b0: 0006 0000 000b 0000 0053 0000 0073 c000  .........S...s..
+000006c0: 0000 7a48 7400 8300 7d00 6401 7d01 6700  ..zHt...}.d.}.g.
+000006d0: 7d02 7c00 6402 1900 7d03 7c03 4400 5d30  }.|.d...}.|.D.]0
+000006e0: 7d04 7a0c 7c02 a001 7402 6a03 7c03 6403  }.z.|...t.j.|.d.
+000006f0: 6404 8d02 a101 0100 5700 710e 0400 7404  d.......W.q...t.
+00000700: 793e 0100 7d05 0100 7a16 7405 6405 7c05  y>..}...z.t.d.|.
+00000710: 8302 0100 7405 6406 7406 7c05 8301 8302  ....t.d.t.|.....
+00000720: 0100 7c01 6407 3700 7d01 5700 5900 6400  ..|.d.7.}.W.Y.d.
+00000730: 7d05 7e05 710e 6400 7d05 7e05 7701 7700  }.~.q.d.}.~.w.w.
+00000740: 7407 7c00 6402 1900 7c01 6408 9c02 8301  t.|.d...|.d.....
+00000750: 5700 5300 0400 7404 795f 0100 7d05 0100  W.S...t.y_..}...
+00000760: 7a0b 7405 7c05 8301 0100 5700 5900 6400  z.t.|.....W.Y.d.
+00000770: 7d05 7e05 6409 5300 6400 7d05 7e05 7701  }.~.d.S.d.}.~.w.
+00000780: 7700 290a 4e72 0500 0000 da09 616e 6f6d  w.).Nr......anom
+00000790: 616c 6965 73e9 0400 0000 2901 da06 696e  alies.....)...in
+000007a0: 6465 6e74 7a1a 616e 6f6d 616c 7920 7061  dentz.anomaly pa
+000007b0: 7273 696e 6720 6578 6365 7074 696f 6e3a  rsing exception:
+000007c0: 7a21 616e 6f6d 616c 7920 7061 7273 696e  z!anomaly parsin
+000007d0: 6720 7374 7269 6e67 2065 7863 6570 7469  g string excepti
+000007e0: 6f6e 3a72 0100 0000 2902 7226 0000 00da  on:r....).r&....
+000007f0: 0f65 7863 6570 7469 6f6e 5f63 6f75 6e74  .exception_count
+00000800: 7220 0000 0029 0872 0600 0000 da06 6170  r ...).r......ap
+00000810: 7065 6e64 da04 6a73 6f6e da05 6475 6d70  pend..json..dump
+00000820: 7372 2100 0000 7222 0000 00da 0373 7472  sr!...r".....str
+00000830: 720a 0000 0029 0672 2300 0000 7229 0000  r....).r#...r)..
+00000840: 00da 1070 6172 7365 645f 616e 6f6d 616c  ...parsed_anomal
+00000850: 6965 73da 1275 6e70 6172 7365 645f 616e  ies..unparsed_an
+00000860: 6f6d 616c 6965 73da 0761 6e6f 6d61 6c79  omalies..anomaly
+00000870: 7224 0000 0072 1600 0000 7216 0000 0072  r$...r....r....r
+00000880: 1700 0000 da0c 6f6e 5f61 6e6f 6d61 6c69  ......on_anomali
+00000890: 6573 5400 0000 7330 0000 0002 0206 0104  esT...s0........
+000008a0: 0204 0108 0108 0102 0118 010e 010a 010e  ................
+000008b0: 0114 0208 8002 fc02 0606 0102 010a fe0e  ................
+000008c0: 0508 010a 0304 0208 8002 fa7a 216f 7065  ...........z!ope
+000008d0: 6e5f 6861 7262 6f72 2e3c 6c6f 6361 6c73  n_harbor.<locals
+000008e0: 3e2e 6f6e 5f61 6e6f 6d61 6c69 6573 7a11  >.on_anomaliesz.
+000008f0: 2f64 6174 612f 7761 6974 696e 675f 666f  /data/waiting_fo
+00000900: 7263 0000 0000 0000 0000 0000 0000 0800  rc..............
+00000910: 0000 0a00 0000 5300 0000 7308 0100 007a  ......S...s....z
+00000920: 6b74 0083 007d 007c 0064 0119 007d 0167  kt...}.|.d...}.g
+00000930: 007d 027c 0144 005d 587d 0364 027d 047a  .}.|.D.]X}.d.}.z
+00000940: 0a7c 0064 0119 007c 0319 0064 0319 007d  .|.d...|...d...}
+00000950: 0457 006e 0904 0074 0179 2301 0001 0001  .W.n...t.y#.....
+00000960: 0059 006e 0177 0064 027d 057a 0a7c 0064  .Y.n.w.d.}.z.|.d
+00000970: 0119 007c 0319 0064 0419 007d 0557 006e  ...|...d...}.W.n
+00000980: 0904 0074 0179 3901 0001 0001 0059 006e  ...t.y9......Y.n
+00000990: 0177 0064 027d 067a 0a7c 0064 0119 007c  .w.d.}.z.|.d...|
+000009a0: 0319 0064 0519 007d 0657 006e 0904 0074  ...d...}.W.n...t
+000009b0: 0179 4f01 0001 0001 0059 006e 0177 007c  .yO......Y.n.w.|
+000009c0: 017c 0319 0064 0619 0064 0719 0064 086b  .|...d...d...d.k
+000009d0: 0372 647c 02a0 027c 037c 047c 057c 0664  .rd|...|.|.|.|.d
+000009e0: 099c 04a1 0101 0071 0c74 0364 0a7c 0269  .......q.t.d.|.i
+000009f0: 0183 0157 0053 0004 0074 0179 8301 007d  ...W.S...t.y...}
+00000a00: 0701 007a 0c74 0464 0b7c 0783 0201 0057  ...z.t.d.|.....W
+00000a10: 0059 0064 007d 077e 0764 0253 0064 007d  .Y.d.}.~.d.S.d.}
+00000a20: 077e 0777 0177 0029 0c4e da11 696e 7465  .~.w.w.).N..inte
+00000a30: 726e 616c 5f73 7461 7475 7365 7372 2000  rnal_statusesr .
+00000a40: 0000 da0b 6f63 6375 7272 656e 6365 73da  ....occurrences.
+00000a50: 0772 6563 6f72 6473 da05 7469 6d65 73da  .records..times.
+00000a60: 0673 7461 7475 73da 0770 726f 6365 7373  .status..process
+00000a70: da04 646f 6e65 2904 da04 7061 7468 7233  ..done)...pathr3
+00000a80: 0000 0072 3400 0000 7235 0000 00da 0b77  ...r4...r5.....w
+00000a90: 6169 7469 6e67 5f66 6f72 7a0a 6578 6365  aiting_forz.exce
+00000aa0: 7074 696f 6e3a 2905 7206 0000 0072 2100  ption:).r....r!.
+00000ab0: 0000 722a 0000 0072 0a00 0000 7222 0000  ..r*...r....r"..
+00000ac0: 0029 0872 2300 0000 7232 0000 0072 3a00  .).r#...r2...r:.
+00000ad0: 0000 da0b 7374 6174 7573 5f70 6174 6872  ....status_pathr
+00000ae0: 3300 0000 7234 0000 0072 3500 0000 7224  3...r4...r5...r$
+00000af0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00000b00: 0000 da0e 6f6e 5f77 6169 7469 6e67 5f66  ....on_waiting_f
+00000b10: 6f72 7300 0000 7350 0000 0002 0206 0108  ors...sP........
+00000b20: 0104 0208 0104 0102 0114 010c 0104 0102  ................
+00000b30: ff04 0302 0114 010c 0104 0102 ff04 0302  ................
+00000b40: 0114 010c 0104 0102 ff14 0304 0102 0102  ................
+00000b50: 0102 0102 0108 fc02 8002 0704 0108 ff0e  ................
+00000b60: 040a 010a 0104 0208 8002 fc7a 236f 7065  ...........z#ope
+00000b70: 6e5f 6861 7262 6f72 2e3c 6c6f 6361 6c73  n_harbor.<locals
+00000b80: 3e2e 6f6e 5f77 6169 7469 6e67 5f66 6f72  >.on_waiting_for
+00000b90: 7214 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000ba0: 0000 0300 0000 0400 0000 5300 0000 7328  ..........S...s(
+00000bb0: 0000 0074 0083 007d 0069 007d 017c 0064  ...t...}.i.}.|.d
+00000bc0: 0119 0044 005d 067d 0264 027c 017c 023c  ...D.].}.d.|.|.<
+00000bd0: 0071 0974 017c 0183 0153 0029 034e 7232  .q.t.|...S.).Nr2
+00000be0: 0000 00da 0029 0272 0600 0000 720a 0000  .....).r....r...
+00000bf0: 0029 0372 2300 0000 da09 7468 655f 7061  .).r#.....the_pa
+00000c00: 7468 7372 3900 0000 7216 0000 0072 1600  thsr9...r....r..
+00000c10: 0000 7217 0000 00da 1c6f 6e5f 5f67 6574  ..r......on__get
+00000c20: 5f5f 6865 616c 7468 5f73 6361 6e73 5f5f  __health_scans__
+00000c30: 7061 7468 73a2 0000 0073 0a00 0000 0602  paths....s......
+00000c40: 0402 0c02 0a01 0802 7a31 6f70 656e 5f68  ........z1open_h
+00000c50: 6172 626f 722e 3c6c 6f63 616c 733e 2e6f  arbor.<locals>.o
+00000c60: 6e5f 5f67 6574 5f5f 6865 616c 7468 5f73  n__get__health_s
+00000c70: 6361 6e73 5f5f 7061 7468 7372 1300 0000  cans__pathsr....
+00000c80: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000c90: 0001 0000 0053 0000 0072 1900 0000 721a  .....S...r....r.
+00000ca0: 0000 0072 1600 0000 2901 da10 6865 616c  ...r....)...heal
+00000cb0: 7468 5f73 6361 6e5f 7061 7468 7216 0000  th_scan_pathr...
+00000cc0: 0072 1600 0000 7217 0000 00da 1a6f 6e5f  .r....r......on_
+00000cd0: 5f67 6574 5f5f 6865 616c 7468 5f73 6361  _get__health_sca
+00000ce0: 6e5f 5f70 6174 68ad 0000 0072 1d00 0000  n__path....r....
+00000cf0: 7a2f 6f70 656e 5f68 6172 626f 722e 3c6c  z/open_harbor.<l
+00000d00: 6f63 616c 733e 2e6f 6e5f 5f67 6574 5f5f  ocals>.on__get__
+00000d10: 6865 616c 7468 5f73 6361 6e5f 5f70 6174  health_scan__pat
+00000d20: 687a 0730 2e30 2e30 2e30 4629 02da 0470  hz.0.0.0.0F)...p
+00000d30: 6f72 74da 0564 6562 7567 2907 7222 0000  ort..debug).r"..
+00000d40: 0072 0800 0000 7203 0000 00da 0572 6f75  .r....r......rou
+00000d50: 7465 7204 0000 0072 0200 0000 da03 7275  ter....r......ru
+00000d60: 6e29 0a72 4200 0000 7234 0000 00da 0361  n).rB...r4.....a
+00000d70: 7070 7218 0000 0072 1c00 0000 7225 0000  ppr....r....r%..
+00000d80: 0072 3100 0000 723c 0000 0072 3f00 0000  .r1...r<...r?...
+00000d90: 7241 0000 0072 1600 0000 7216 0000 0072  rA...r....r....r
+00000da0: 1700 0000 da0b 6f70 656e 5f68 6172 626f  ......open_harbo
+00000db0: 7225 0000 0073 3400 0000 0804 0a01 0804  r%...s4.........
+00000dc0: 0202 0c03 0e02 0a01 0e09 0a01 0e03 0a01  ................
+00000dd0: 0e10 0a01 0e1e 0a01 0e2e 0a01 0e0a 0a01  ................
+00000de0: 0804 0802 0404 0201 0201 0201 0afd 7247  ..............rG
+00000df0: 0000 0029 0272 0500 0000 7205 0000 0029  ...).r....r....)
+00000e00: 1ada 075f 5f64 6f63 5f5f da15 7370 6163  ...__doc__..spac
+00000e10: 6573 2e64 6f6e 655f 7769 7468 5f73 6361  es.done_with_sca
+00000e20: 6e72 0200 0000 da12 7370 6163 6573 2e70  nr......spaces.p
+00000e30: 6174 6873 5f70 6174 6368 7203 0000 00da  aths_patchr.....
+00000e40: 1e73 7061 6365 732e 7468 655f 6865 616c  .spaces.the_heal
+00000e50: 7468 5f73 6361 6e5f 7374 6172 7465 6472  th_scan_startedr
+00000e60: 0400 0000 da39 6269 6f74 6563 682e 7072  .....9biotech.pr
+00000e70: 6f63 6564 7572 6573 2e61 6767 7265 6761  ocedures.aggrega
+00000e80: 746f 725f 7072 6f63 6564 7572 652e 7072  tor_procedure.pr
+00000e90: 6f63 6573 732e 7661 7269 6162 6c65 7372  ocess.variablesr
+00000ea0: 0600 0000 7207 0000 00da 0566 6c61 736b  ....r......flask
+00000eb0: 7208 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
+00000ec0: 0472 6963 6872 2b00 0000 da07 7061 7468  .richr+.....path
+00000ed0: 6c69 62da 026f 73da 076f 732e 7061 7468  lib..os..os.path
+00000ee0: 720b 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000ef0: 0373 7973 da09 7468 7265 6164 696e 67da  .sys..threading.
+00000f00: 0474 696d 6572 4700 0000 7216 0000 0072  .timerG...r....r
+00000f10: 1600 0000 7216 0000 0072 1700 0000 da08  ....r....r......
+00000f20: 3c6d 6f64 756c 653e 0100 0000 7324 0000  <module>....s$..
+00000f30: 0004 020c 0c0c 010c 010c 020c 0114 0308  ................
+00000f40: 0108 0308 0108 0114 0108 0108 0108 0102  ................
+00000f50: 0502 010e fe                             .....
```

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 20 04:40:12 2024 UTC, .py size: 3572 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2c47 2366 f40d 0000  o.......,G#f....
+00000000: 6f0d 0d0a 0000 0000 ad2c 2466 ee0d 0000  o........,$f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
@@ -118,15 +118,15 @@
 00000750: 7265 5f70 6f72 7472 1400 0000 7215 0000  re_portr....r...
 00000760: 00a9 00fa 602f 6269 6f74 6563 682f 7665  ....`/biotech/ve
 00000770: 6e75 6573 2f73 7461 6765 732f 6269 6f74  nues/stages/biot
 00000780: 6563 682f 7072 6f63 6564 7572 6573 2f61  ech/procedures/a
 00000790: 6767 7265 6761 746f 725f 7072 6f63 6564  ggregator_proced
 000007a0: 7572 652f 7072 6f63 6573 732f 6b65 672f  ure/process/keg/
 000007b0: 7370 6163 6573 2f70 6174 6873 5f70 6174  spaces/paths_pat
-000007c0: 6368 2e70 79da 0776 656e 7475 7265 6100  ch.py..venturea.
+000007c0: 6368 2e70 79da 0776 656e 7475 7265 5f00  ch.py..venture_.
 000007d0: 0000 7324 0000 000a 0114 021c 010c 0214  ..s$............
 000007e0: 0202 0202 0202 0202 0104 0302 ff04 fa06  ................
 000007f0: ff10 0d14 0114 0114 0204 037a 3170 6174  ...........z1pat
 00000800: 6873 5f70 6174 6368 2e3c 6c6f 6361 6c73  hs_patch.<locals
 00000810: 3e2e 7061 7468 735f 7061 7463 682e 3c6c  >.paths_patch.<l
 00000820: 6f63 616c 733e 2e76 656e 7475 7265 2903  ocals>.venture).
 00000830: da08 6361 7061 6369 7479 da05 6974 656d  ..capacity..item
@@ -138,15 +138,15 @@
 00000890: 6163 6b65 7472 1300 0000 7216 0000 0072  acketr....r....r
 000008a0: 1700 0000 7230 0000 00da 0870 726f 6365  ....r0.....proce
 000008b0: 6564 7372 2300 0000 a901 722d 0000 0029  edsr#.....r-...)
 000008c0: 0272 1400 0000 7215 0000 0072 2f00 0000  .r....r....r/...
 000008d0: da0b 7061 7468 735f 7061 7463 6824 0000  ..paths_patch$..
 000008e0: 0073 3c00 0000 0c13 1201 0c01 0804 0802  .s<.............
 000008f0: 0801 0802 0801 0807 0c01 0803 0c01 0202  ................
-00000900: 0203 0201 0201 04fe 0807 1006 0422 0201  ............."..
+00000900: 0203 0201 0201 04fe 0806 1005 0422 0201  ............."..
 00000910: 0201 0201 0201 06fd 0206 040b 08fc 0a01  ................
 00000920: 0403 7a20 7061 7468 735f 7061 7463 682e  ..z paths_patch.
 00000930: 3c6c 6f63 616c 733e 2e70 6174 6873 5f70  <locals>.paths_p
 00000940: 6174 6368 2901 da05 726f 7574 6529 03da  atch)...route)..
 00000950: 0361 7070 722d 0000 0072 3c00 0000 722e  .appr-...r<...r.
 00000960: 0000 0072 3b00 0000 722f 0000 0072 3c00  ...r;...r/...r<.
 00000970: 0000 1f00 0000 7304 0000 000e 0512 0172  ......s........r
```

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,21 +83,19 @@
 		'''
 		setup_internal_statuses (
 			status_check_paths,
 			relative_path
 		)
 		
 		
-		
 		aggregator_variables ["internal_statuses_built"] = "yes"
 		#
 		# ----
 		
 		
-		
 		def venture (status_check_path):
 			rel_path = format_path (status_check_path, relative_path);
 		
 			aggregator_variables ["internal_statuses"] [ rel_path ] ["occurrences"] ["scan process venture started"] = "yes"
 			aggregator_variables ["internal_statuses"] [ rel_path ] ["times"] ["venture started"] = str (time.time ())
 		
 			start_time = str (time.time ())
```

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/no_records.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/no_records.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,18 +29,25 @@
 		#if (the_internal_statuses [ internal_status ] [ "status" ] [ "scan" ] != "done"):
 		#	return;
 	
 		if (the_internal_statuses [ internal_status ] [ "status" ] [ "process" ] != "done"):
 			return;
 	
 
+	#
+	#
+	#
+	aggregator_variables ["proceeds"] = aggregate_stats ()
+	aggregator_variables ["proceeds_built"] = "yes"
+	
+
 	'''
 		if not bounced, then send done
 	'''	
 	send_done (
 		host = aggregator_variables ["intro_harbor"] ["host"],
 		port = aggregator_variables ["intro_harbor"] ["port"],
 		
-		proceeds = aggregate_stats ()
+		proceeds = aggregator_variables ["proceeds"]
 	)
 	
 	return "sent"
```

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py` & `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,31 +63,34 @@
 	
 	#
 	#
 	#
 	"internal_statuses": {},
 	"internal_statuses_built": "no",
 	
+	"proceeds": {},
+	"proceeds_built": "no",
+	
 	"anomalies": []
 }
 
 def add_anomaly (anomaly):
-	print ("add_anomaly?", anomaly)
-
 	try:
 		is_JSON = json.dumps (anomaly)
 	
 		aggregator_variables ["anomalies"].append (anomaly)
 		
 		show_variable ({
 			"anomaly": anomaly
 		})
 		
 	except Exception as E:
 		show_variable ("An anomaly couldn't be added.")
+		aggregator_variables ["anomalies"].append ("An anomaly couldn't be added.")
+		
 		print ("exception:", E)
 
 
 def setup_internal_statuses (
 	status_check_paths,
 	relative_path
 ):
```

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py` & `biotech-1.1.7/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/dynamic_port.py` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/dynamic_port.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/on.py` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py` & `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/intro/on.py` & `biotech-1.1.7/venues/stages/biotech/procedures/intro/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/intro/process/adventure.py` & `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/adventure.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py` & `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py` & `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/intro/process/keg/__init__.py` & `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/aggregate/__init__.py` & `biotech-1.1.7/venues/stages/biotech/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/alarm_parser/__init__.py` & `biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/exceptions.py` & `biotech-1.1.7/venues/stages/biotech/topics/exceptions.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/__init__.py` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/__init__.py` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/basin/treasury.py` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/treasury.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/help_documentation/shares.s.HTML` & `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/shares.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/implicit/proc/__init__.py` & `biotech-1.1.7/venues/stages/biotech/topics/implicit/proc/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/implicit/thread/__init__.py` & `biotech-1.1.7/venues/stages/biotech/topics/implicit/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/printout/passes.py` & `biotech-1.1.7/venues/stages/biotech/topics/printout/passes.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/__init__.py` & `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/implicit.py` & `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/process_on/p_expect/parse_records.py` & `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/process_on/sub/explicit.py` & `biotech-1.1.7/venues/stages/biotech/topics/process_on/sub/explicit.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/process_on/sub/implicit.py` & `biotech-1.1.7/venues/stages/biotech/topics/process_on/sub/implicit.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/quay/garage.py` & `biotech-1.1.7/venues/stages/biotech/topics/quay/garage.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/quay/implicit_process_test_1.py` & `biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/quay/implicit_process_test_2.py` & `biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_2.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/quay/implicit_process_test_3.py` & `biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_3.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/quay/implicit_process_test_4.py` & `biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_4.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py` & `biotech-1.1.7/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/show/variable.py` & `biotech-1.1.7/venues/stages/biotech/topics/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc` & `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/venues/stages/biotech/topics/start--/simultaneously.py` & `biotech-1.1.7/venues/stages/biotech/topics/start--/simultaneously.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.6/PKG-INFO` & `biotech-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotech
-Version: 1.1.6
+Version: 1.1.7
 Summary: A health monitoring stack
 License: GPL-3.0-only
 Keywords: alarms,screening,monitors,cybernetics,neurons,nervous system,bioelectric,homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

