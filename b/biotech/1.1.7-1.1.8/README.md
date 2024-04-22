# Comparing `tmp/biotech-1.1.7.tar.gz` & `tmp/biotech-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotech-1.1.7.tar", max compression
+gzip compressed data, was "biotech-1.1.8.tar", max compression
```

## Comparing `biotech-1.1.7.tar` & `biotech-1.1.8.tar`

### file list

```diff
@@ -1,739 +1,739 @@
--rwxr-xr-x   0        0        0      211 2024-04-20 04:40:12.925620 biotech-1.1.7/license.S.HTML
--rwxr-xr-x   0        0        0     1144 2024-04-22 01:19:00.612990 biotech-1.1.7/pyproject.toml
--rwxr-xr-x   0        0        0     3866 2024-04-20 04:40:12.929620 biotech-1.1.7/readme.md
--rwxr-xr-x   0        0        0     1353 2024-04-22 01:00:02.912088 biotech-1.1.7/venue.S.HTML
--rwxr-xr-x   0        0        0   838272 2024-04-20 04:40:12.929620 biotech-1.1.7/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
--rwxr-xr-x   0        0        0     1270 2024-04-20 04:40:12.929620 biotech-1.1.7/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
--rwxr-xr-x   0        0        0     4125 2024-04-20 04:40:12.929620 biotech-1.1.7/venues/stages/biotech/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      663 2024-04-22 01:17:56.413671 biotech-1.1.7/venues/stages/biotech/___itinerary/maybes.s.HTML
--rwxr-xr-x   0        0        0      190 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout/script.py
--rwxr-xr-x   0        0        0     1255 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout/start.py
--rwxr-xr-x   0        0        0      189 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
--rwxr-xr-x   0        0        0      186 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
--rwxr-xr-x   0        0        0      190 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
--rwxr-xr-x   0        0        0     1141 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
--rwxr-xr-x   0        0        0      385 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/__glossary/biotech_1
--rwxr-xr-x   0        0        0      114 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/__glossary/glossary.S.HTML
--rwxr-xr-x   0        0        0      130 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/__init__.py
--rwxr-xr-x   0        0        0    37279 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0     1252 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_book/advanced tutorial.s.HTML
--rwxr-xr-x   0        0        0     1786 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_book/book.s.HTML
--rwxr-xr-x   0        0        0      542 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_book/relevant.s.HTML
--rwxr-xr-x   0        0        0     2007 2024-04-22 00:54:52.470209 biotech-1.1.7/venues/stages/biotech/_clique/__init__.py
--rw-r--r--   0        0        0     2334 2024-04-22 01:02:39.250779 biotech-1.1.7/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4457 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      691 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0  1436985 2024-04-22 01:04:15.725916 biotech-1.1.7/venues/stages/biotech/_status/DB/records.json
--rw-r--r--   0        0        0     1172 2024-04-20 04:44:34.660565 biotech-1.1.7/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
--rwxr-xr-x   0        0        0     1589 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
--rwxr-xr-x   0        0        0     1116 2024-04-20 04:40:12.933620 biotech-1.1.7/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
--rwxr-xr-x   0        0        0     1487 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/establish.py
--rwxr-xr-x   0        0        0       83 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      720 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/-01_start/status_1.py
--rwxr-xr-x   0        0        0      101 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/00_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      793 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/00_start/status_1.py
--rwxr-xr-x   0        0        0      282 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/01/stasis/path_1_health.py
--rwxr-xr-x   0        0        0      265 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/01/stasis/path_2_health.py
--rwxr-xr-x   0        0        0     1161 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/01/status_1.py
--rwxr-xr-x   0        0        0      321 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/02/stasis/1_health.py
--rwxr-xr-x   0        0        0        2 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/02/stasis/2_health.py
--rwxr-xr-x   0        0        0       50 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/02/stasis/modules/MODULE_1.py
--rwxr-xr-x   0        0        0     1214 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/02/status_1.py
--rwxr-xr-x   0        0        0      794 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py
--rwxr-xr-x   0        0        0       35 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      939 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py
--rwxr-xr-x   0        0        0      289 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      942 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py
--rwxr-xr-x   0        0        0      518 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py
--rwxr-xr-x   0        0        0      155 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      867 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/05__file__/status_1.py
--rwxr-xr-x   0        0        0      311 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/06_various/stasis/1_health.py
--rwxr-xr-x   0        0        0       31 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/06_various/stasis/2_health.py
--rwxr-xr-x   0        0        0        0 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/06_various/stasis/3_health.py
--rwxr-xr-x   0        0        0      955 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/06_various/status_1.py
--rwxr-xr-x   0        0        0      160 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/07/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0      809 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/07/status_1.py
--rwxr-xr-x   0        0        0       73 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/08_DB/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0     1561 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/08_DB/status_1.py
--rwxr-xr-x   0        0        0   103233 2024-04-22 01:03:50.394146 biotech-1.1.7/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json
--rwxr-xr-x   0        0        0      119 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0      124 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_2.py
--rwxr-xr-x   0        0        0        7 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_3.py
--rwxr-xr-x   0        0        0     1442 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py
--rw-r--r--   0        0        0      357 2024-04-20 04:45:57.075380 biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       96 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1189 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
--rw-r--r--   0        0        0      316 2024-04-20 04:46:07.863238 biotech-1.1.7/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       77 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1250 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/monitors/11/status_1.py
--rwxr-xr-x   0        0        0      984 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/status.proc.py
--rwxr-xr-x   0        0        0      256 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status/status.s.HTML
--rwxr-xr-x   0        0        0     1483 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0      406 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
--rwxr-xr-x   0        0        0      358 2024-04-20 04:40:12.969620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
--rwxr-xr-x   0        0        0   542989 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
--rwxr-xr-x   0        0        0      919 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/_status_advanced/status.proc.py
--rwxr-xr-x   0        0        0     1772 2024-04-21 23:18:15.551401 biotech-1.1.7/venues/stages/biotech/architecture.s.HTML
--rwxr-xr-x   0        0        0      241 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/emojis.S.HTML
--rwxr-xr-x   0        0        0      286 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/license.S.HTML
--rwxr-xr-x   0        0        0     3068 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/module.s.HTML
--rw-r--r--   0        0        0     1596 2024-04-20 04:44:35.492552 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      640 2024-04-20 04:44:35.500552 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      259 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
--rwxr-xr-x   0        0        0     1478 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      366 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/paths.py
--rwxr-xr-x   0        0        0      666 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
--rwxr-xr-x   0        0        0      562 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
--rw-r--r--   0        0        0     1165 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4141 2024-04-20 21:08:19.573336 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
--rw-r--r--   0        0        0     3925 2024-04-20 21:08:23.925315 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      999 2024-04-20 04:44:36.652534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0     2881 2024-04-20 21:08:11.873375 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
--rw-r--r--   0        0        0     1152 2024-04-20 04:44:36.652534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      653 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
--rwxr-xr-x   0        0        0     3566 2024-04-20 20:59:25.531411 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
--rwxr-xr-x   0        0        0      769 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
--rw-r--r--   0        0        0     2031 2024-04-20 04:44:36.644534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
--rw-r--r--   0        0        0     2159 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      420 2024-04-20 04:44:36.644534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
--rw-r--r--   0        0        0      728 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
--rwxr-xr-x   0        0        0     3451 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
--rwxr-xr-x   0        0        0     3235 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
--rwxr-xr-x   0        0        0      193 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
--rwxr-xr-x   0        0        0      514 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
--rwxr-xr-x   0        0        0     2440 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
--rw-r--r--   0        0        0     2352 2024-04-20 04:44:36.644534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      849 2024-04-20 21:06:01.973995 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
--rw-r--r--   0        0        0     4019 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
--rw-r--r--   0        0        0     1634 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
--rw-r--r--   0        0        0     2916 2024-04-20 04:40:12.973620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/no_records.py
--rwxr-xr-x   0        0        0      754 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
--rw-r--r--   0        0        0     1826 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1128 2024-04-20 21:04:00.238519 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
--rwxr-xr-x   0        0        0     8732 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
--rwxr-xr-x   0        0        0     3652 2024-04-20 21:04:51.502306 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
--rw-r--r--   0        0        0     2202 2024-04-20 21:06:01.969995 biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      834 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
--rw-r--r--   0        0        0      951 2024-04-20 04:45:40.247606 biotech-1.1.7/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      648 2024-04-20 04:44:36.652534 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
--rw-r--r--   0        0        0     1904 2024-04-20 04:44:36.652534 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      706 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/dynamic_port.py
--rwxr-xr-x   0        0        0     2161 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/on.py
--rwxr-xr-x   0        0        0     2200 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
--rwxr-xr-x   0        0        0     2957 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
--rwxr-xr-x   0        0        0     1441 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
--rwxr-xr-x   0        0        0      774 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
--rwxr-xr-x   0        0        0     1336 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      309 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      562 2024-04-20 04:44:37.516521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      660 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      547 2024-04-20 04:44:37.504521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      908 2024-04-20 04:44:37.504521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
--rw-r--r--   0        0        0      636 2024-04-20 04:44:37.516521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
--rwxr-xr-x   0        0        0      289 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
--rwxr-xr-x   0        0        0      803 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
--rwxr-xr-x   0        0        0      378 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
--rwxr-xr-x   0        0        0      321 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
--rwxr-xr-x   0        0        0     2182 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
--rw-r--r--   0        0        0     2125 2024-04-20 04:44:37.516521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1828 2024-04-20 04:44:37.524521 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0     2295 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
--rw-r--r--   0        0        0        2 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/start.py
--rwxr-xr-x   0        0        0      132 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
--rwxr-xr-x   0        0        0      152 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4699 2024-04-20 04:44:34.600566 biotech-1.1.7/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      374 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/intro.S.HTML
--rwxr-xr-x   0        0        0     6305 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/on.py
--rw-r--r--   0        0        0     2906 2024-04-20 04:44:35.492552 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
--rw-r--r--   0        0        0     4000 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/adventure.py
--rw-r--r--   0        0        0     1330 2024-04-20 04:44:35.500552 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      905 2024-04-20 04:44:35.500552 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      959 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
--rwxr-xr-x   0        0        0      614 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
--rwxr-xr-x   0        0        0      138 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/intro.proc.py
--rwxr-xr-x   0        0        0     3084 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/keg/__init__.py
--rw-r--r--   0        0        0     3068 2024-04-20 04:44:35.492552 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       89 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/variables/__init__.py
--rw-r--r--   0        0        0      245 2024-04-20 04:44:35.492552 biotech-1.1.7/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      172 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/procedures/procedures.S.HTML
--rwxr-xr-x   0        0        0      823 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
--rwxr-xr-x   0        0        0     3031 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
--rw-r--r--   0        0        0      933 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1061 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/aggregate/__init__.py
--rwxr-xr-x   0        0        0     1053 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      708 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__init__.py
--rw-r--r--   0        0        0      673 2024-04-20 04:44:36.644534 biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1069 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      764 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/exceptions.py
--rwxr-xr-x   0        0        0     1190 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
--rwxr-xr-x   0        0        0     2446 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__init__.py
--rw-r--r--   0        0        0     2491 2024-04-20 04:41:49.823732 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4471 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1050 2024-04-20 04:40:12.977620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     1920 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
--rwxr-xr-x   0        0        0       24 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
--rwxr-xr-x   0        0        0       24 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
--rwxr-xr-x   0        0        0      751 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
--rwxr-xr-x   0        0        0     1981 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__init__.py
--rw-r--r--   0        0        0     2283 2024-04-20 04:41:49.835732 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4019 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3843 2024-04-20 04:44:34.576567 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
--rwxr-xr-x   0        0        0     4426 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
--rwxr-xr-x   0        0        0     3559 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/treasury.py
--rwxr-xr-x   0        0        0     1727 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/help_documentation/shares.s.HTML
--rwxr-xr-x   0        0        0     1055 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1558 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/implicit/proc/__init__.py
--rwxr-xr-x   0        0        0     1158 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/implicit/thread/__init__.py
--rw-r--r--   0        0        0      855 2024-04-20 04:44:34.624566 biotech-1.1.7/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       90 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
--rwxr-xr-x   0        0        0      598 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
--rw-r--r--   0        0        0      731 2024-04-20 04:44:35.492552 biotech-1.1.7/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
--rwxr-xr-x   0        0        0      470 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/printout/bracket.py
--rwxr-xr-x   0        0        0      740 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/printout/passes.py
--rwxr-xr-x   0        0        0     2261 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2166 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__init__.py
--rw-r--r--   0        0        0     1997 2024-04-20 04:44:34.600566 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     2184 2024-04-20 04:44:34.604566 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
--rw-r--r--   0        0        0      919 2024-04-20 04:44:36.648534 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
--rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/implicit.py
--rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
--rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
--rwxr-xr-x   0        0        0      195 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/process_on.S.HTML
--rw-r--r--   0        0        0      832 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/sub/explicit.py
--rw-r--r--   0        0        0     1015 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/process_on/sub/implicit.py
--rwxr-xr-x   0        0        0     1470 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/quay/garage.py
--rwxr-xr-x   0        0        0     2546 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_1.py
--rwxr-xr-x   0        0        0     1612 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_2.py
--rwxr-xr-x   0        0        0      551 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_3.py
--rwxr-xr-x   0        0        0     1083 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_4.py
--rwxr-xr-x   0        0        0     1448 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
--rw-r--r--   0        0        0     1464 2024-04-20 04:44:36.652534 biotech-1.1.7/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      274 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
--rw-r--r--   0        0        0      246 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/report_formats/report_formats.S.HTML
--rw-r--r--   0        0        0     1772 2024-04-20 04:44:34.604566 biotech-1.1.7/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
--rwxr-xr-x   0        0        0      461 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/show/show.S.HTML
--rwxr-xr-x   0        0        0     2295 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/show/variable.py
--rwxr-xr-x   0        0        0      654 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
--rwxr-xr-x   0        0        0      454 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
--rwxr-xr-x   0        0        0      273 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/one.py
--rwxr-xr-x   0        0        0      406 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/sequentially.py
--rwxr-xr-x   0        0        0      532 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/start--/simultaneously.py
--rwxr-xr-x   0        0        0       76 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/topics/topics.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-20 04:40:12.981620 biotech-1.1.7/venues/stages/biotech/variables/__init__.py
--rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.7/PKG-INFO
+-rwxr-xr-x   0        0        0      211 2024-04-20 04:40:12.925620 biotech-1.1.8/license.S.HTML
+-rwxr-xr-x   0        0        0     1144 2024-04-22 03:04:49.837366 biotech-1.1.8/pyproject.toml
+-rwxr-xr-x   0        0        0     3866 2024-04-20 04:40:12.929620 biotech-1.1.8/readme.md
+-rwxr-xr-x   0        0        0     1362 2024-04-22 02:57:06.910722 biotech-1.1.8/venue.S.HTML
+-rwxr-xr-x   0        0        0   838272 2024-04-20 04:40:12.929620 biotech-1.1.8/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
+-rwxr-xr-x   0        0        0     1270 2024-04-20 04:40:12.929620 biotech-1.1.8/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
+-rwxr-xr-x   0        0        0     4125 2024-04-20 04:40:12.929620 biotech-1.1.8/venues/stages/biotech/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      663 2024-04-22 01:17:56.413671 biotech-1.1.8/venues/stages/biotech/___itinerary/maybes.s.HTML
+-rwxr-xr-x   0        0        0      190 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/___itinerary/processes/errout/script.py
+-rwxr-xr-x   0        0        0     1255 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/___itinerary/processes/errout/start.py
+-rwxr-xr-x   0        0        0      189 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
+-rwxr-xr-x   0        0        0      186 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
+-rwxr-xr-x   0        0        0      190 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
+-rwxr-xr-x   0        0        0     1141 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
+-rwxr-xr-x   0        0        0      385 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/__glossary/biotech_1
+-rwxr-xr-x   0        0        0      114 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/__glossary/glossary.S.HTML
+-rwxr-xr-x   0        0        0      130 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/__init__.py
+-rwxr-xr-x   0        0        0    37279 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0     1252 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/_book/advanced tutorial.s.HTML
+-rwxr-xr-x   0        0        0     1786 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/_book/book.s.HTML
+-rwxr-xr-x   0        0        0      542 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/_book/relevant.s.HTML
+-rwxr-xr-x   0        0        0     2007 2024-04-22 00:54:52.470209 biotech-1.1.8/venues/stages/biotech/_clique/__init__.py
+-rw-r--r--   0        0        0     2334 2024-04-22 01:02:39.250779 biotech-1.1.8/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4457 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      691 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0  1440191 2024-04-22 03:01:09.419929 biotech-1.1.8/venues/stages/biotech/_status/DB/records.json
+-rw-r--r--   0        0        0     1172 2024-04-20 04:44:34.660565 biotech-1.1.8/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1589 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1116 2024-04-20 04:40:12.933620 biotech-1.1.8/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1487 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/establish.py
+-rwxr-xr-x   0        0        0       83 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/-01_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      720 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/-01_start/status_1.py
+-rwxr-xr-x   0        0        0      101 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/00_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      793 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/00_start/status_1.py
+-rwxr-xr-x   0        0        0      282 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/01/stasis/path_1_health.py
+-rwxr-xr-x   0        0        0      265 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/01/stasis/path_2_health.py
+-rwxr-xr-x   0        0        0     1161 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/01/status_1.py
+-rwxr-xr-x   0        0        0      321 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/02/stasis/1_health.py
+-rwxr-xr-x   0        0        0        2 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/02/stasis/2_health.py
+-rwxr-xr-x   0        0        0       50 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/02/stasis/modules/MODULE_1.py
+-rwxr-xr-x   0        0        0     1214 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/02/status_1.py
+-rwxr-xr-x   0        0        0      794 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py
+-rwxr-xr-x   0        0        0       35 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/04.0_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      939 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      289 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/04.1_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      942 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      518 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py
+-rwxr-xr-x   0        0        0      155 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/05__file__/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      867 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/05__file__/status_1.py
+-rwxr-xr-x   0        0        0      311 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/06_various/stasis/1_health.py
+-rwxr-xr-x   0        0        0       31 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/06_various/stasis/2_health.py
+-rwxr-xr-x   0        0        0        0 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/06_various/stasis/3_health.py
+-rwxr-xr-x   0        0        0      955 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/06_various/status_1.py
+-rwxr-xr-x   0        0        0      160 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/07/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0      809 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/07/status_1.py
+-rwxr-xr-x   0        0        0       73 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/08_DB/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0     1561 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/08_DB/status_1.py
+-rwxr-xr-x   0        0        0   103550 2024-04-22 03:00:51.312138 biotech-1.1.8/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      119 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0      124 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_2.py
+-rwxr-xr-x   0        0        0        7 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/guarantees/guarantee_3.py
+-rwxr-xr-x   0        0        0     1442 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py
+-rw-r--r--   0        0        0      357 2024-04-20 04:45:57.075380 biotech-1.1.8/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1189 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
+-rw-r--r--   0        0        0      316 2024-04-20 04:46:07.863238 biotech-1.1.8/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       77 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1250 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/monitors/11/status_1.py
+-rwxr-xr-x   0        0        0      984 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/status.proc.py
+-rwxr-xr-x   0        0        0      256 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status/status.s.HTML
+-rwxr-xr-x   0        0        0     1483 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.937620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.941620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.949620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.953620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.957620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.961620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.965620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0      406 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
+-rwxr-xr-x   0        0        0      358 2024-04-20 04:40:12.969620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
+-rwxr-xr-x   0        0        0   542989 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      919 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/_status_advanced/status.proc.py
+-rwxr-xr-x   0        0        0     1772 2024-04-21 23:18:15.551401 biotech-1.1.8/venues/stages/biotech/architecture.s.HTML
+-rwxr-xr-x   0        0        0      241 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/emojis.S.HTML
+-rwxr-xr-x   0        0        0      286 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/license.S.HTML
+-rwxr-xr-x   0        0        0     3068 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/module.s.HTML
+-rw-r--r--   0        0        0     1567 2024-04-22 02:58:40.501648 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      640 2024-04-20 04:44:35.500552 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      259 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
+-rwxr-xr-x   0        0        0     1479 2024-04-22 02:58:38.869667 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      366 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/paths.py
+-rwxr-xr-x   0        0        0      666 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
+-rwxr-xr-x   0        0        0      562 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
+-rw-r--r--   0        0        0     1165 2024-04-20 04:44:36.648534 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4141 2024-04-20 21:08:19.573336 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
+-rw-r--r--   0        0        0     3925 2024-04-20 21:08:23.925315 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      999 2024-04-20 04:44:36.652534 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0     2881 2024-04-20 21:08:11.873375 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
+-rw-r--r--   0        0        0     1152 2024-04-20 04:44:36.652534 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      653 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
+-rwxr-xr-x   0        0        0     3566 2024-04-20 20:59:25.531411 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
+-rwxr-xr-x   0        0        0      769 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
+-rw-r--r--   0        0        0     2031 2024-04-20 04:44:36.644534 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
+-rw-r--r--   0        0        0     2159 2024-04-20 04:44:36.648534 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      420 2024-04-20 04:44:36.644534 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
+-rw-r--r--   0        0        0      728 2024-04-20 04:44:36.648534 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3451 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
+-rwxr-xr-x   0        0        0     3235 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
+-rwxr-xr-x   0        0        0      193 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
+-rwxr-xr-x   0        0        0      514 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
+-rwxr-xr-x   0        0        0     2440 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
+-rw-r--r--   0        0        0     2352 2024-04-20 04:44:36.644534 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      849 2024-04-20 21:06:01.973995 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
+-rw-r--r--   0        0        0     4019 2024-04-20 04:44:36.648534 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
+-rw-r--r--   0        0        0     1634 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py
+-rw-r--r--   0        0        0     2916 2024-04-20 04:40:12.973620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/no_records.py
+-rwxr-xr-x   0        0        0      754 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
+-rw-r--r--   0        0        0     1826 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-20 04:44:36.648534 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1128 2024-04-20 21:04:00.238519 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
+-rwxr-xr-x   0        0        0     8732 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
+-rwxr-xr-x   0        0        0     3652 2024-04-20 21:04:51.502306 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
+-rw-r--r--   0        0        0     2202 2024-04-20 21:06:01.969995 biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      834 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-20 04:45:40.247606 biotech-1.1.8/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      648 2024-04-20 04:44:36.652534 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
+-rw-r--r--   0        0        0     1904 2024-04-20 04:44:36.652534 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      706 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/dynamic_port.py
+-rwxr-xr-x   0        0        0     2161 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/on.py
+-rwxr-xr-x   0        0        0     2228 2024-04-22 02:59:36.345004 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
+-rwxr-xr-x   0        0        0     2957 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
+-rwxr-xr-x   0        0        0     1441 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
+-rwxr-xr-x   0        0        0      774 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
+-rwxr-xr-x   0        0        0     1336 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      309 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      562 2024-04-20 04:44:37.516521 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      660 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      547 2024-04-20 04:44:37.504521 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2024-04-20 04:44:37.504521 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
+-rw-r--r--   0        0        0      636 2024-04-20 04:44:37.516521 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      289 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
+-rwxr-xr-x   0        0        0      803 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
+-rwxr-xr-x   0        0        0      378 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
+-rwxr-xr-x   0        0        0      321 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
+-rwxr-xr-x   0        0        0     2182 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
+-rw-r--r--   0        0        0     2125 2024-04-20 04:44:37.516521 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1828 2024-04-20 04:44:37.524521 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2295 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
+-rw-r--r--   0        0        0        2 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/start.py
+-rwxr-xr-x   0        0        0      132 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
+-rwxr-xr-x   0        0        0      152 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4699 2024-04-22 02:56:35.411082 biotech-1.1.8/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      374 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/intro/intro.S.HTML
+-rwxr-xr-x   0        0        0     6311 2024-04-22 02:56:31.411128 biotech-1.1.8/venues/stages/biotech/procedures/intro/on.py
+-rw-r--r--   0        0        0     2906 2024-04-20 04:44:35.492552 biotech-1.1.8/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
+-rw-r--r--   0        0        0     4000 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/intro/process/adventure.py
+-rw-r--r--   0        0        0     1330 2024-04-20 04:44:35.500552 biotech-1.1.8/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      905 2024-04-20 04:44:35.500552 biotech-1.1.8/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      959 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      614 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
+-rwxr-xr-x   0        0        0      138 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/intro/process/intro.proc.py
+-rwxr-xr-x   0        0        0     3084 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/intro/process/keg/__init__.py
+-rw-r--r--   0        0        0     3068 2024-04-20 04:44:35.492552 biotech-1.1.8/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       89 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/intro/process/variables/__init__.py
+-rw-r--r--   0        0        0      245 2024-04-20 04:44:35.492552 biotech-1.1.8/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      172 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/procedures/procedures.S.HTML
+-rwxr-xr-x   0        0        0      823 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3031 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
+-rw-r--r--   0        0        0      933 2024-04-20 04:44:36.648534 biotech-1.1.8/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1061 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/aggregate/__init__.py
+-rwxr-xr-x   0        0        0     1053 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      708 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/alarm_parser/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-20 04:44:36.644534 biotech-1.1.8/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1069 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      764 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/exceptions.py
+-rwxr-xr-x   0        0        0     1190 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
+-rwxr-xr-x   0        0        0     2446 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/__init__.py
+-rw-r--r--   0        0        0     2491 2024-04-20 04:41:49.823732 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4471 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1050 2024-04-20 04:40:12.977620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1920 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
+-rwxr-xr-x   0        0        0       24 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
+-rwxr-xr-x   0        0        0       24 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
+-rwxr-xr-x   0        0        0      751 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
+-rwxr-xr-x   0        0        0     1981 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/__init__.py
+-rw-r--r--   0        0        0     2283 2024-04-20 04:41:49.835732 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4019 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3843 2024-04-20 04:44:34.576567 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4426 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3559 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/treasury.py
+-rwxr-xr-x   0        0        0     1727 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/help_documentation/shares.s.HTML
+-rwxr-xr-x   0        0        0     1055 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1558 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/implicit/proc/__init__.py
+-rwxr-xr-x   0        0        0     1158 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/implicit/thread/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-20 04:44:34.624566 biotech-1.1.8/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       90 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
+-rw-r--r--   0        0        0      731 2024-04-20 04:44:35.492552 biotech-1.1.8/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
+-rwxr-xr-x   0        0        0      470 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/printout/bracket.py
+-rwxr-xr-x   0        0        0      740 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/printout/passes.py
+-rwxr-xr-x   0        0        0     2261 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2166 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/__init__.py
+-rw-r--r--   0        0        0     1997 2024-04-20 04:44:34.600566 biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     2184 2024-04-20 04:44:34.604566 biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
+-rw-r--r--   0        0        0      919 2024-04-20 04:44:36.648534 biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1956 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
+-rwxr-xr-x   0        0        0      195 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/process_on/process_on.S.HTML
+-rw-r--r--   0        0        0      832 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/process_on/sub/explicit.py
+-rw-r--r--   0        0        0     1015 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/process_on/sub/implicit.py
+-rwxr-xr-x   0        0        0     1470 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/quay/garage.py
+-rwxr-xr-x   0        0        0     2546 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/quay/implicit_process_test_1.py
+-rwxr-xr-x   0        0        0     1612 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/quay/implicit_process_test_2.py
+-rwxr-xr-x   0        0        0      551 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/quay/implicit_process_test_3.py
+-rwxr-xr-x   0        0        0     1083 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/quay/implicit_process_test_4.py
+-rwxr-xr-x   0        0        0     1448 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
+-rw-r--r--   0        0        0     1464 2024-04-20 04:44:36.652534 biotech-1.1.8/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      274 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/report_formats/report_formats.S.HTML
+-rw-r--r--   0        0        0     1772 2024-04-20 04:44:34.604566 biotech-1.1.8/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0      461 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/show/show.S.HTML
+-rwxr-xr-x   0        0        0     2295 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/show/variable.py
+-rwxr-xr-x   0        0        0      654 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
+-rwxr-xr-x   0        0        0      454 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
+-rwxr-xr-x   0        0        0      567 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
+-rwxr-xr-x   0        0        0      273 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/start--/one.py
+-rwxr-xr-x   0        0        0      406 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/start--/sequentially.py
+-rwxr-xr-x   0        0        0      532 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/start--/simultaneously.py
+-rwxr-xr-x   0        0        0       76 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/topics/topics.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-20 04:40:12.981620 biotech-1.1.8/venues/stages/biotech/variables/__init__.py
+-rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.8/PKG-INFO
```

### Comparing `biotech-1.1.7/pyproject.toml` & `biotech-1.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 [tool.poetry]
 name = "biotech"
-version = "1.1.7"
+version = "1.1.8"
 description = "A health monitoring stack"
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "biotech", from = "venues/stages" }
 ]
```

### Comparing `biotech-1.1.7/readme.md` & `biotech-1.1.8/readme.md`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venue.S.HTML` & `biotech-1.1.8/venue.S.HTML`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	
 	<h2>docker</h2>
 		docker network create --subnet=192.168.0.0/24 container_network
 		docker run --network container_network --ip 192.168.0.102 -v .:/biotech -it jumps:v2.1.0
 		docker exec -it a6599081a9fb bash 
 
 	<h2>install</h2>
-		python3 moves/install.py
+		python3 /biotech/moves/install.py
 
 	<h2>source</h2>
 		source source.sh
 
 	<h2>git</h2>
 		git push --set-upstream git@gitlab.com:status600/climates/biotech.git performance
```

### Comparing `biotech-1.1.7/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg` & `biotech-1.1.8/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML` & `biotech-1.1.8/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/___itinerary/itinerary.S.HTML` & `biotech-1.1.8/venues/stages/biotech/___itinerary/itinerary.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/___itinerary/maybes.s.HTML` & `biotech-1.1.8/venues/stages/biotech/___itinerary/maybes.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout/start.py` & `biotech-1.1.8/venues/stages/biotech/___itinerary/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/___itinerary/processes/errout_v2/start.py` & `biotech-1.1.8/venues/stages/biotech/___itinerary/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/__license/options/gpl-3.0-standalone.html` & `biotech-1.1.8/venues/stages/biotech/__license/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_book/advanced tutorial.s.HTML` & `biotech-1.1.8/venues/stages/biotech/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_book/book.s.HTML` & `biotech-1.1.8/venues/stages/biotech/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_book/relevant.s.HTML` & `biotech-1.1.8/venues/stages/biotech/_book/relevant.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_clique/__init__.py` & `biotech-1.1.8/venues/stages/biotech/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/DB/records.json` & `biotech-1.1.8/venues/stages/biotech/_status/DB/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998759305210918%*

 * *Differences: {"'_default'": "{'403': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'_status/monitors/-01_start/status_1.py'), ('empty', False), ('parsed', True), "*

 * *               "('stats', OrderedDict([('passes', 1), ('alarms', 0)])), ('checks', "*

 * *               "[OrderedDict([('check', 'check 1'), ('passed', True), ('elapsed', "*

 * *               "[3.372792344998743, 'seconds'])])])]), OrderedDict([('path', "*

 * *               "'_status/monitors/00_start/status_1.py'), ('empty', False), ('parsed', True), " […]*

```diff
@@ -55639,14 +55639,293 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 14
                 },
                 "empty": 0
             }
         },
+        "403": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.372792344998743,
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
+                                3.3448753870034125,
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
+                                3.7060522270003275,
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
+                                3.3461565079996944,
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
+                                2.386960840001848,
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
+                                3.5941098090006562,
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
+                                3.3458310210007767,
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
+                                3.635593068000162,
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
+                                3.3550518729971373,
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
+                                3.4145061249982973,
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
+                                3.7253021290016477,
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
+                                3.632736952000414,
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
+                                8.490565883003,
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
+                                3.3400201780023053,
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

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/establish.py` & `biotech-1.1.8/venues/stages/biotech/_status/establish.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/-01_start/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/-01_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/00_start/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/00_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/01/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/01/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/02/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/02/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/03_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/04.0_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/04.1_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/05__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/05__file__/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/05__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/06_various/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/06_various/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/07/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/07/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/08_DB/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/08_DB/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/08_DB/variable/status_db/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979591836734694%*

 * *Differences: {"'_default'": "{'245': OrderedDict([('paths', [OrderedDict([('checks', [OrderedDict([('check', "*

 * *               "'check 1'), ('elapsed', [2.993001544382423e-06, 'seconds']), ('passed', True)])]), "*

 * *               "('empty', False), ('parsed', True), ('path', 'guarantee_1.py'), ('records', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('passes', 1)]))])]), ('alarms', []), "*

 * *               "('stats', OrderedDict([('alarms', 0), ('checks', OrderedDict([('alarms', 0), "*

 * *               "('passes' […]*

```diff
@@ -6119,14 +6119,47 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
         },
+        "245": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.993001544382423e-06,
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

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/09_aggregation_format_and_exit/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/monitors/11/status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status/monitors/11/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status/status.proc.py` & `biotech-1.1.8/venues/stages/biotech/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py` & `biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json` & `biotech-1.1.8/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/_status_advanced/status.proc.py` & `biotech-1.1.8/venues/stages/biotech/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/architecture.s.HTML` & `biotech-1.1.8/venues/stages/biotech/architecture.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/module.s.HTML` & `biotech-1.1.8/venues/stages/biotech/module.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 20 04:40:12 2024 UTC, .py size: 1478 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2c47 2366 c605 0000  o.......,G#f....
+00000000: 6f0d 0d0a 0000 0000 5ed2 2566 c705 0000  o.......^.%f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 5a00 0900 0900 6401 6402 6c01 6d02 5a03  Z.....d.d.l.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 0200 0100 6d06  ..d.d.l.m.....m.
 00000050: 5a07 0100 6401 6403 6c08 6d09 0200 0100  Z...d.d.l.m.....
 00000060: 6d0a 5a0b 0100 6401 6403 6c0c 6d0d 0200  m.Z...d.d.l.m...
 00000070: 0100 6d0e 5a0f 0100 6401 6404 6c10 6d11  ..m.Z...d.d.l.m.
@@ -25,76 +25,74 @@
 00000180: 6e29 01da 1370 726f 6365 7373 5f6f 6e5f  n)...process_on_
 00000190: 696d 706c 6963 6974 2901 da0d 7368 6f77  implicit)...show
 000001a0: 5f76 6172 6961 626c 65e9 0100 0000 2901  _variable.....).
 000001b0: da1f 6669 6e64 5f61 6767 7265 6761 746f  ..find_aggregato
 000001c0: 725f 7072 6f63 6564 7572 655f 7061 7468  r_procedure_path
 000001d0: 7329 01da 0846 7261 6374 696f 6e63 0200  s)...Fractionc..
 000001e0: 0000 0000 0000 0000 0000 0700 0000 0600  ................
-000001f0: 0000 4300 0000 7372 0000 0074 0064 0164  ..C...sr...t.d.d
+000001f0: 0000 4300 0000 7368 0000 0074 0064 0164  ..C...sh...t.d.d
 00000200: 0264 038d 0201 0064 047d 0274 0183 007d  .d.....d.}.t...}
 00000210: 0364 057c 039b 0064 067c 009b 009d 047d  .d.|...d.|.....}
 00000220: 0474 026a 03a0 04a1 007d 0564 07a0 0567  .t.j.....}.d...g
 00000230: 0074 066a 07a2 01a1 017c 0564 083c 0074  .t.j.....|.d.<.t
 00000240: 087c 0464 007c 0564 0964 0a8d 047d 0674  .|.d.|.d.d...}.t
-00000250: 09a0 0a64 0ba1 0101 0074 0064 0c7c 0669  ...d.....t.d.|.i
-00000260: 0164 0264 038d 0201 007c 0653 0029 0d4e  .d.d.....|.S.).N
-00000270: da17 6167 6772 6567 6174 6f72 5f70 726f  ..aggregator_pro
-00000280: 6365 6475 7265 5f6f 6eda 0963 6f6e 6465  cedure_on..conde
-00000290: 6e73 6564 2901 da04 6d6f 6465 69a8 6100  nsed)...modei.a.
-000002a0: 007a 0870 7974 686f 6e33 207a 1120 6b65  .z.python3 z. ke
-000002b0: 6720 6f70 656e 202d 2d70 6f72 7420 fa01  g open --port ..
-000002c0: 3ada 0a50 5954 484f 4e50 4154 48da 0a61  :..PYTHONPATH..a
-000002d0: 6767 7265 6761 746f 7229 03da 0343 5744  ggregator)...CWD
-000002e0: da03 656e 76da 046e 616d 6572 0600 0000  ..env..namer....
-000002f0: 7a19 7468 6520 6167 6772 6567 6174 6f72  z.the aggregator
-00000300: 2070 726f 6365 6475 7265 3a29 0b72 0500   procedure:).r..
-00000310: 0000 7207 0000 00da 026f 73da 0765 6e76  ..r......os..env
-00000320: 6972 6f6e da04 636f 7079 da04 6a6f 696e  iron..copy..join
-00000330: da03 7379 73da 0470 6174 6872 0400 0000  ..sys..pathr....
-00000340: da04 7469 6d65 da05 736c 6565 7029 07da  ..time..sleep)..
-00000350: 0470 6f72 74da 0670 6163 6b65 74da 0b6c  .port..packet..l
-00000360: 696d 6974 5f73 7461 7274 da18 7061 7468  imit_start..path
-00000370: 5f6f 665f 7468 655f 7363 616e 5f70 726f  _of_the_scan_pro
-00000380: 6365 7373 da0e 7072 6f63 6573 735f 7374  cess..process_st
-00000390: 7269 6e67 da13 7072 6f63 6573 735f 656e  ring..process_en
-000003a0: 7669 726f 6e6d 656e 74da 0b74 6865 5f76  vironment..the_v
-000003b0: 656e 7475 7265 a900 7221 0000 00fa 442f  enture..r!....D/
-000003c0: 6269 6f74 6563 682f 7665 6e75 6573 2f73  biotech/venues/s
-000003d0: 7461 6765 732f 6269 6f74 6563 682f 7072  tages/biotech/pr
-000003e0: 6f63 6564 7572 6573 2f61 6767 7265 6761  ocedures/aggrega
-000003f0: 746f 725f 7072 6f63 6564 7572 652f 6f6e  tor_procedure/on
-00000400: 2e70 7972 0900 0000 2e00 0000 732c 0000  .pyr........s,..
-00000410: 000c 0404 0206 020e 0202 ff0a 0406 0104  ................
-00000420: 010a ff02 0402 0102 0202 0102 0106 fb0a  ................
-00000430: 0802 0104 0102 ff02 0206 fe04 0472 0900  .............r..
-00000440: 0000 2921 da07 5f5f 646f 635f 5fda 1762  ..)!..__doc__..b
-00000450: 6f74 616e 6973 742e 6379 636c 652e 7072  otanist.cycle.pr
-00000460: 6573 656e 7473 7202 0000 00da 0e63 7963  esentsr......cyc
-00000470: 6c65 5f70 7265 7365 6e74 73da 1b62 6f74  le_presents..bot
-00000480: 616e 6973 742e 7072 6f63 6573 7365 732e  anist.processes.
-00000490: 6d75 6c74 6970 6c65 da09 7072 6f63 6573  multiple..proces
-000004a0: 7365 73da 086d 756c 7469 706c 65da 0a6d  ses..multiple..m
-000004b0: 756c 7469 5f70 726f 63da 1462 6f74 616e  ulti_proc..botan
-000004c0: 6973 742e 6379 636c 652e 6c6f 6f70 73da  ist.cycle.loops.
-000004d0: 0563 7963 6c65 da05 6c6f 6f70 73da 0b63  .cycle..loops..c
-000004e0: 7963 6c65 5f6c 6f6f 7073 da1b 626f 7461  ycle_loops..bota
-000004f0: 6e69 7374 2e70 6f72 7473 5f76 322e 6176  nist.ports_v2.av
-00000500: 6169 6c61 626c 65da 0870 6f72 7473 5f76  ailable..ports_v
-00000510: 32da 0961 7661 696c 6162 6c65 da0e 6176  2..available..av
-00000520: 6169 6c61 626c 655f 706f 7274 da22 6269  ailable_port."bi
-00000530: 6f74 6563 682e 746f 7069 6373 2e70 726f  otech.topics.pro
-00000540: 6365 7373 5f6f 6e2e 705f 6578 7065 6374  cess_on.p_expect
-00000550: 7203 0000 00da 2b62 696f 7465 6368 2e74  r.....+biotech.t
-00000560: 6f70 6963 732e 7072 6f63 6573 735f 6f6e  opics.process_on
-00000570: 2e70 5f65 7870 6563 742e 696d 706c 6963  .p_expect.implic
-00000580: 6974 7204 0000 00da 1c62 696f 7465 6368  itr......biotech
-00000590: 2e74 6f70 6963 732e 7368 6f77 2e76 6172  .topics.show.var
-000005a0: 6961 626c 6572 0500 0000 da05 7061 7468  iabler......path
-000005b0: 7372 0700 0000 da07 7065 7870 6563 74da  sr......pexpect.
-000005c0: 0472 6963 6872 1600 0000 da04 6a73 6f6e  .richr......json
-000005d0: 7212 0000 00da 0966 7261 6374 696f 6e73  r......fractions
-000005e0: 7208 0000 0072 1800 0000 7209 0000 0072  r....r....r....r
-000005f0: 2100 0000 7221 0000 0072 2100 0000 7222  !...r!...r!...r"
-00000600: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000610: 0073 2600 0000 0401 0205 0209 0c06 1201  .s&.............
-00000620: 1201 1201 0c02 0c01 0c01 0c02 0803 0801  ................
-00000630: 0803 0801 0801 0c01 0801 0c04            ............
+00000250: 0064 0b7c 0669 0164 0264 038d 0201 007c  .d.|.i.d.d.....|
+00000260: 0653 0029 0c4e da17 6167 6772 6567 6174  .S.).N..aggregat
+00000270: 6f72 5f70 726f 6365 6475 7265 5f6f 6eda  or_procedure_on.
+00000280: 0963 6f6e 6465 6e73 6564 2901 da04 6d6f  .condensed)...mo
+00000290: 6465 69a8 6100 007a 0870 7974 686f 6e33  dei.a..z.python3
+000002a0: 207a 1120 6b65 6720 6f70 656e 202d 2d70   z. keg open --p
+000002b0: 6f72 7420 fa01 3ada 0a50 5954 484f 4e50  ort ..:..PYTHONP
+000002c0: 4154 48da 0a61 6767 7265 6761 746f 7229  ATH..aggregator)
+000002d0: 03da 0343 5744 da03 656e 76da 046e 616d  ...CWD..env..nam
+000002e0: 657a 1974 6865 2061 6767 7265 6761 746f  ez.the aggregato
+000002f0: 7220 7072 6f63 6564 7572 653a 2909 7205  r procedure:).r.
+00000300: 0000 0072 0700 0000 da02 6f73 da07 656e  ...r......os..en
+00000310: 7669 726f 6eda 0463 6f70 79da 046a 6f69  viron..copy..joi
+00000320: 6eda 0373 7973 da04 7061 7468 7204 0000  n..sys..pathr...
+00000330: 0029 07da 0470 6f72 74da 0670 6163 6b65  .)...port..packe
+00000340: 74da 0b6c 696d 6974 5f73 7461 7274 da18  t..limit_start..
+00000350: 7061 7468 5f6f 665f 7468 655f 7363 616e  path_of_the_scan
+00000360: 5f70 726f 6365 7373 da0e 7072 6f63 6573  _process..proces
+00000370: 735f 7374 7269 6e67 da13 7072 6f63 6573  s_string..proces
+00000380: 735f 656e 7669 726f 6e6d 656e 74da 0b74  s_environment..t
+00000390: 6865 5f76 656e 7475 7265 a900 721f 0000  he_venture..r...
+000003a0: 00fa 442f 6269 6f74 6563 682f 7665 6e75  ..D/biotech/venu
+000003b0: 6573 2f73 7461 6765 732f 6269 6f74 6563  es/stages/biotec
+000003c0: 682f 7072 6f63 6564 7572 6573 2f61 6767  h/procedures/agg
+000003d0: 7265 6761 746f 725f 7072 6f63 6564 7572  regator_procedur
+000003e0: 652f 6f6e 2e70 7972 0900 0000 2e00 0000  e/on.pyr........
+000003f0: 732a 0000 000c 0404 0206 020e 0202 ff0a  s*..............
+00000400: 0406 0104 010a ff02 0402 0102 0202 0102  ................
+00000410: 0106 fb02 0904 0102 ff02 0206 fe04 0472  ...............r
+00000420: 0900 0000 2921 da07 5f5f 646f 635f 5fda  ....)!..__doc__.
+00000430: 1762 6f74 616e 6973 742e 6379 636c 652e  .botanist.cycle.
+00000440: 7072 6573 656e 7473 7202 0000 00da 0e63  presentsr......c
+00000450: 7963 6c65 5f70 7265 7365 6e74 73da 1b62  ycle_presents..b
+00000460: 6f74 616e 6973 742e 7072 6f63 6573 7365  otanist.processe
+00000470: 732e 6d75 6c74 6970 6c65 da09 7072 6f63  s.multiple..proc
+00000480: 6573 7365 73da 086d 756c 7469 706c 65da  esses..multiple.
+00000490: 0a6d 756c 7469 5f70 726f 63da 1462 6f74  .multi_proc..bot
+000004a0: 616e 6973 742e 6379 636c 652e 6c6f 6f70  anist.cycle.loop
+000004b0: 73da 0563 7963 6c65 da05 6c6f 6f70 73da  s..cycle..loops.
+000004c0: 0b63 7963 6c65 5f6c 6f6f 7073 da1b 626f  .cycle_loops..bo
+000004d0: 7461 6e69 7374 2e70 6f72 7473 5f76 322e  tanist.ports_v2.
+000004e0: 6176 6169 6c61 626c 65da 0870 6f72 7473  available..ports
+000004f0: 5f76 32da 0961 7661 696c 6162 6c65 da0e  _v2..available..
+00000500: 6176 6169 6c61 626c 655f 706f 7274 da22  available_port."
+00000510: 6269 6f74 6563 682e 746f 7069 6373 2e70  biotech.topics.p
+00000520: 726f 6365 7373 5f6f 6e2e 705f 6578 7065  rocess_on.p_expe
+00000530: 6374 7203 0000 00da 2b62 696f 7465 6368  ctr.....+biotech
+00000540: 2e74 6f70 6963 732e 7072 6f63 6573 735f  .topics.process_
+00000550: 6f6e 2e70 5f65 7870 6563 742e 696d 706c  on.p_expect.impl
+00000560: 6963 6974 7204 0000 00da 1c62 696f 7465  icitr......biote
+00000570: 6368 2e74 6f70 6963 732e 7368 6f77 2e76  ch.topics.show.v
+00000580: 6172 6961 626c 6572 0500 0000 da05 7061  ariabler......pa
+00000590: 7468 7372 0700 0000 da07 7065 7870 6563  thsr......pexpec
+000005a0: 74da 0472 6963 6872 1600 0000 da04 6a73  t..richr......js
+000005b0: 6f6e 7212 0000 00da 0966 7261 6374 696f  onr......fractio
+000005c0: 6e73 7208 0000 00da 0474 696d 6572 0900  nsr......timer..
+000005d0: 0000 721f 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+000005e0: 0072 2000 0000 da08 3c6d 6f64 756c 653e  .r .....<module>
+000005f0: 0100 0000 7326 0000 0004 0102 0502 090c  ....s&..........
+00000600: 0612 0112 0112 010c 020c 010c 010c 0208  ................
+00000610: 0308 0108 0308 0108 010c 0108 010c 04    ...............
```

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/on.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/on.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 		process_string,
 		
 		CWD = None,
 		env = process_environment,
 		name = "aggregator"
 	)
 	
-	time.sleep (1)
+	#time.sleep (1)
 	show_variable ({
 		'the aggregator procedure:': the_venture
 	}, mode = "condensed")
 
 	return the_venture
```

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/global_time_limit_exceeded.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/no_records.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/alarm_checks/no_records.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py` & `biotech-1.1.8/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/dynamic_port.py` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/dynamic_port.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/on.py` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 			"relative_path": status_relative_path
 		}
 	)
 	
 	#
 	#	elapsed check
 	#
-	time.sleep (1)
+	#time.sleep (1)
 	
 	try:
 		#----
 		#
 		
 		#
 		#----
@@ -101,12 +101,12 @@
 		}
 	)
 
 	time.sleep (1)
 
 	exit ()
 
-
-main ();
+if __name__ == "__main__":
+	main ();
 
 
 #send_post_request (host, port, "/", proceeds)
```

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py` & `biotech-1.1.8/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 20 04:40:12 2024 UTC, .py size: 6305 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2c47 2366 a118 0000  o.......,G#f....
+00000000: 6f0d 0d0a 0000 0000 dfd1 2566 a718 0000  o.........%f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 5a06 6400 6405 6c07  ..d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6404 6c0a  m.Z.m.Z...d.d.l.
 00000070: 5a0a 6400 6404 6c0b 5a0b 6400 6404 6c0c  Z.d.d.l.Z.d.d.l.
@@ -173,45 +173,45 @@
 00000ac0: 2a40 2069 6e74 726f 2f6f 6e2e 7079 203a  *@ intro/on.py :
 00000ad0: 3a20 6166 7465 7220 7072 6f63 6573 7320  : after process 
 00000ae0: 6f6e 2069 6d70 6c69 6369 7454 7a22 6368  on implicitTz"ch
 00000af0: 6563 6b69 6e67 2069 6620 6973 2074 6865  ecking if is the
 00000b00: 2069 6e74 726f 2068 6172 626f 7220 6f6e   intro harbor on
 00000b10: 7236 0000 007a 1852 6573 706f 6e73 6520  r6...z.Response 
 00000b20: 626f 6479 2074 6f20 2f69 735f 6f6e 3ada  body to /is_on:.
-00000b30: 0379 6573 7217 0000 007a 1c73 656e 6469  .yesr....z.sendi
-00000b40: 6e67 2074 6865 2076 6172 6961 626c 6573  ng the variables
-00000b50: 2070 6163 6b65 747a 062f 7374 6172 7429   packetz./start)
-00000b60: 01da 046a 736f 6eda 0872 6563 6569 7665  ...json..receive
-00000b70: 647a 102f 6973 5f72 6570 6f72 745f 7265  dz./is_report_re
-00000b80: 6164 797a 112f 6973 5f72 6570 6f72 745f  adyz./is_report_
-00000b90: 7265 6164 793a 7a0b 2f74 6865 5f72 6570  ready:z./the_rep
-00000ba0: 6f72 747a 2e54 6865 2069 6e74 726f 2070  ortz.The intro p
-00000bb0: 726f 6365 7373 2073 7461 7274 6572 2072  rocess starter r
-00000bc0: 6563 6569 7665 6420 7468 655f 7265 706f  eceived the_repo
-00000bd0: 7274 2eda 0672 6570 6f72 7429 01da 0865  rt...report)...e
-00000be0: 7869 7374 5f6f 6b7a 0c72 6563 6f72 6473  xist_okz.records
-00000bf0: 2e6a 736f 6e72 2700 0000 7228 0000 0072  .jsonr'...r(...r
-00000c00: 2900 0000 2903 7227 0000 0072 2800 0000  )...).r'...r(...
-00000c10: 7229 0000 0046 6300 0000 0000 0000 0000  r)...Fc.........
-00000c20: 0000 0001 0000 000a 0000 0013 0000 0073  ...............s
-00000c30: b200 0000 7400 6401 8301 0100 8802 6402  ....t.d.......d.
-00000c40: 6b02 7211 7401 a002 6403 a101 0100 8802  k.r.t...d.......
-00000c50: 6402 6b02 7308 8801 6404 1900 a003 a100  d.k.s...d.......
-00000c60: 0100 8800 6405 6b02 7257 7400 6406 8301  ....d.k.rWt.d...
-00000c70: 0100 7a15 7400 6407 8801 6404 1900 a004  ..z.t.d...d.....
-00000c80: a100 8302 0100 8801 6404 1900 a004 a100  ........d.......
-00000c90: 6402 6b02 7233 6402 8900 5700 6e17 0400  d.k.r3d...W.n...
-00000ca0: 7405 794b 0100 7d00 0100 7a0b 7400 6408  t.yK..}...z.t.d.
-00000cb0: 7c00 8302 0100 5700 5900 6400 7d00 7e00  |.....W.Y.d.}.~.
-00000cc0: 6e05 6400 7d00 7e00 7701 7700 7401 a002  n.d.}.~.w.w.t...
-00000cd0: 6403 a101 0100 8800 6405 6b02 731b 6400  d.......d.k.s.d.
-00000ce0: 5300 6400 5300 2909 4e7a 1c77 6169 7469  S.d.S.).Nz.waiti
-00000cf0: 6e67 2066 6f72 206f 6666 2074 6f20 6265  ng for off to be
-00000d00: 2063 616c 6c65 6446 6700 0000 0000 00d0   calledFg.......
-00000d10: 3f72 4200 0000 547a 1b77 6169 7469 6e67  ?rB...Tz.waiting
+00000b30: 0379 6573 e700 0000 0000 00d0 3f7a 1c73  .yes........?z.s
+00000b40: 656e 6469 6e67 2074 6865 2076 6172 6961  ending the varia
+00000b50: 626c 6573 2070 6163 6b65 747a 062f 7374  bles packetz./st
+00000b60: 6172 7429 01da 046a 736f 6eda 0872 6563  art)...json..rec
+00000b70: 6569 7665 647a 102f 6973 5f72 6570 6f72  eivedz./is_repor
+00000b80: 745f 7265 6164 797a 112f 6973 5f72 6570  t_readyz./is_rep
+00000b90: 6f72 745f 7265 6164 793a 7a0b 2f74 6865  ort_ready:z./the
+00000ba0: 5f72 6570 6f72 747a 2e54 6865 2069 6e74  _reportz.The int
+00000bb0: 726f 2070 726f 6365 7373 2073 7461 7274  ro process start
+00000bc0: 6572 2072 6563 6569 7665 6420 7468 655f  er received the_
+00000bd0: 7265 706f 7274 2eda 0672 6570 6f72 7429  report...report)
+00000be0: 01da 0865 7869 7374 5f6f 6b7a 0c72 6563  ...exist_okz.rec
+00000bf0: 6f72 6473 2e6a 736f 6e72 2700 0000 7228  ords.jsonr'...r(
+00000c00: 0000 0072 2900 0000 2903 7227 0000 0072  ...r)...).r'...r
+00000c10: 2800 0000 7229 0000 0046 6300 0000 0000  (...r)...Fc.....
+00000c20: 0000 0000 0000 0001 0000 000a 0000 0013  ................
+00000c30: 0000 0073 b200 0000 7400 6401 8301 0100  ...s....t.d.....
+00000c40: 8802 6402 6b02 7211 7401 a002 6403 a101  ..d.k.r.t...d...
+00000c50: 0100 8802 6402 6b02 7308 8801 6404 1900  ....d.k.s...d...
+00000c60: a003 a100 0100 8800 6405 6b02 7257 7400  ........d.k.rWt.
+00000c70: 6406 8301 0100 7a15 7400 6407 8801 6404  d.....z.t.d...d.
+00000c80: 1900 a004 a100 8302 0100 8801 6404 1900  ............d...
+00000c90: a004 a100 6402 6b02 7233 6402 8900 5700  ....d.k.r3d...W.
+00000ca0: 6e17 0400 7405 794b 0100 7d00 0100 7a0b  n...t.yK..}...z.
+00000cb0: 7400 6408 7c00 8302 0100 5700 5900 6400  t.d.|.....W.Y.d.
+00000cc0: 7d00 7e00 6e05 6400 7d00 7e00 7701 7700  }.~.n.d.}.~.w.w.
+00000cd0: 7401 a002 6403 a101 0100 8800 6405 6b02  t...d.......d.k.
+00000ce0: 731b 6400 5300 6400 5300 2909 4e7a 1c77  s.d.S.d.S.).Nz.w
+00000cf0: 6169 7469 6e67 2066 6f72 206f 6666 2074  aiting for off t
+00000d00: 6f20 6265 2063 616c 6c65 6446 724a 0000  o be calledFrJ..
+00000d10: 0072 4200 0000 547a 1b77 6169 7469 6e67  .rB...Tz.waiting
 00000d20: 2066 6f72 2070 726f 6365 7373 2074 6f20   for process to 
 00000d30: 6578 6974 7a09 6973 5f61 6c69 7665 3a7a  exitz.is_alive:z
 00000d40: 0a65 7863 6570 7469 6f6e 3a29 0672 4400  .exception:).rD.
 00000d50: 0000 da04 7469 6d65 da05 736c 6565 7072  ....time..sleepr
 00000d60: 4300 0000 da08 6973 5f61 6c69 7665 723a  C.....is_aliver:
 00000d70: 0000 0072 4500 0000 2903 da0a 6261 7272  ...rE...)...barr
 00000d80: 6963 6164 6564 7247 0000 00da 0874 6865  icadedrG.....the
@@ -223,44 +223,44 @@
 00000de0: 6e2e 3c6c 6f63 616c 733e 2e62 6163 6b67  n.<locals>.backg
 00000df0: 726f 756e 645f 7461 736b 2901 da06 7461  round_task)...ta
 00000e00: 7267 6574 6300 0000 0000 0000 0000 0000  rgetc...........
 00000e10: 0000 0000 0003 0000 0013 0000 0073 2a00  .............s*.
 00000e20: 0000 6401 8901 8800 6401 6b02 7213 7400  ..d.....d.k.r.t.
 00000e30: 6402 8301 0100 7401 a002 6403 a101 0100  d.....t...d.....
 00000e40: 8800 6401 6b02 7306 6400 5300 2904 4e54  ..d.k.s.d.S.).NT
-00000e50: 7251 0000 0072 1700 0000 2903 7244 0000  rQ...r....).rD..
-00000e60: 0072 4e00 0000 724f 0000 0072 1100 0000  .rN...rO...r....
-00000e70: 2902 7251 0000 0072 5200 0000 7211 0000  ).rQ...rR...r...
+00000e50: 7252 0000 0072 4a00 0000 2903 7244 0000  rR...rJ...).rD..
+00000e60: 0072 4f00 0000 7250 0000 0072 1100 0000  .rO...rP...r....
+00000e70: 2902 7252 0000 0072 5300 0000 7211 0000  ).rR...rS...r...
 00000e80: 0072 1200 0000 da08 7475 726e 5f6f 6666  .r......turn_off
 00000e90: 4401 0000 730c 0000 0004 0408 0208 010a  D...s...........
 00000ea0: 0108 fe04 047a 146f 6e2e 3c6c 6f63 616c  .....z.on.<local
 00000eb0: 733e 2e74 7572 6e5f 6f66 6629 0272 2500  s>.turn_off).r%.
 00000ec0: 0000 7226 0000 0029 2072 0300 0000 da02  ..r&...) r......
 00000ed0: 6f73 da07 656e 7669 726f 6eda 0463 6f70  os..environ..cop
 00000ee0: 7972 0800 0000 da03 7379 73da 0470 6174  yr......sys..pat
-00000ef0: 6872 0f00 0000 724a 0000 00da 0564 756d  hr....rJ.....dum
+00000ef0: 6872 0f00 0000 724b 0000 00da 0564 756d  hr....rK.....dum
 00000f00: 7073 7202 0000 0072 1300 0000 da06 6174  psr....r......at
 00000f10: 6578 6974 da08 7265 6769 7374 6572 7244  exit..registerrD
 00000f20: 0000 0072 3700 0000 7238 0000 00da 0474  ...r7...r8.....t
-00000f30: 6578 7472 3a00 0000 724e 0000 0072 4f00  extr:...rN...rO.
+00000f30: 6578 7472 3a00 0000 724f 0000 0072 5000  extr:...rO...rP.
 00000f40: 0000 da05 7061 7463 68da 056c 6f61 6473  ....patch..loads
 00000f50: da04 7479 7065 da08 6d61 6b65 6469 7273  ..type..makedirs
 00000f60: 7209 0000 0072 0500 0000 da06 696e 7365  r....r......inse
 00000f70: 7274 da05 636c 6f73 65da 0974 6872 6561  rt..close..threa
 00000f80: 6469 6e67 da06 5468 7265 6164 722e 0000  ding..Threadr...
 00000f90: 0029 0fda 0670 6163 6b65 7472 1e00 0000  .)...packetr....
 00000fa0: da0d 7265 636f 7264 735f 6c65 7665 6cda  ..records_level.
 00000fb0: 1370 726f 6365 7373 5f65 6e76 6972 6f6e  .process_environ
 00000fc0: 6d65 6e74 7235 0000 0072 3f00 0000 7248  mentr5...r?...rH
 00000fd0: 0000 0072 3c00 0000 7246 0000 0072 2d00  ...r<...rF...r-.
 00000fe0: 0000 da07 6462 5f66 696c 65da 0264 6272  ....db_file..dbr
-00000ff0: 5300 0000 da11 6261 636b 6772 6f75 6e64  S.....background
-00001000: 5f74 6872 6561 6472 5500 0000 7211 0000  _threadrU...r...
-00001010: 0029 0472 5100 0000 723e 0000 0072 4700  .).rQ...r>...rG.
-00001020: 0000 7252 0000 0072 1200 0000 722b 0000  ..rR...r....r+..
+00000ff0: 5400 0000 da11 6261 636b 6772 6f75 6e64  T.....background
+00001000: 5f74 6872 6561 6472 5600 0000 7211 0000  _threadrV...r...
+00001010: 0029 0472 5200 0000 723e 0000 0072 4700  .).rR...r>...rG.
+00001020: 0000 7253 0000 0072 1200 0000 722b 0000  ..rS...r....r+..
 00001030: 0065 0000 0073 d200 0000 1001 0202 0801  .e...s..........
 00001040: 06ff 0205 0804 0801 0801 0801 0803 0a01  ................
 00001050: 0402 0c03 0802 0a02 0601 0401 0aff 0c04  ................
 00001060: 0a01 0e02 0801 0203 0208 0c03 0610 0202  ................
 00001070: 0204 0801 0203 0201 06fb 0c08 0a08 0202  ................
 00001080: 0203 0c10 0202 0201 0801 0401 0601 04ff  ................
 00001090: 0c03 0a02 0401 04ff 0e03 0801 0c01 0880  ................
@@ -276,19 +276,19 @@
 00001130: 5f65 7870 6563 742e 696d 706c 6963 6974  _expect.implicit
 00001140: 7202 0000 00da 1c62 696f 7465 6368 2e74  r......biotech.t
 00001150: 6f70 6963 732e 7368 6f77 2e76 6172 6961  opics.show.varia
 00001160: 626c 6572 0300 0000 da1e 6269 6f74 6563  bler......biotec
 00001170: 682e 746f 7069 6373 2e69 6d70 6c69 6369  h.topics.implici
 00001180: 742e 7468 7265 6164 7204 0000 00da 0472  t.threadr......r
 00001190: 6963 68da 0674 696e 7964 6272 0500 0000  ich..tinydbr....
-000011a0: 7206 0000 0072 3700 0000 725c 0000 00da  r....r7...r\....
-000011b0: 0467 6c6f 6272 4a00 0000 720a 0000 00da  .globrJ...r.....
+000011a0: 7206 0000 0072 3700 0000 725d 0000 00da  r....r7...r]....
+000011b0: 0467 6c6f 6272 4b00 0000 720a 0000 00da  .globrK...r.....
 000011c0: 076f 732e 7061 7468 7207 0000 0072 0800  .os.pathr....r..
-000011d0: 0000 7209 0000 0072 5600 0000 7259 0000  ..r....rV...rY..
-000011e0: 0072 6500 0000 724e 0000 0072 1300 0000  .re...rN...r....
+000011d0: 0000 7209 0000 0072 5700 0000 725a 0000  ..r....rW...rZ..
+000011e0: 0072 6600 0000 724f 0000 0072 1300 0000  .rf...rO...r....
 000011f0: 722e 0000 0072 2b00 0000 7211 0000 0072  r....r+...r....r
 00001200: 1100 0000 7211 0000 0072 1200 0000 da08  ....r....r......
 00001210: 3c6d 6f64 756c 653e 0100 0000 733a 0000  <module>....s:..
 00001220: 000c 030c 010c 0108 0410 0108 0108 0308  ................
 00001230: 0108 0108 0114 0108 0108 0108 0108 0108  ................
 00001240: 0402 0602 0502 0102 0802 0102 0202 0202  ................
 00001250: 0102 0202 0102 020a e60c 45              ..........E
```

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/intro/on.py` & `biotech-1.1.8/venues/stages/biotech/procedures/intro/on.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
 			if (response.text == "yes"):
 				break;
 			
 		except Exception as E:
 			print (E)
 			pass;
 			
-		time.sleep (1)
+		time.sleep (.25)
 	
 
 	show_variable ("sending the variables packet", mode = "condensed")
 	
 	'''
 		objective: send the packet to the intro quay
 	'''
@@ -252,15 +252,15 @@
 			if (response.text == "yes"):
 				break;
 			
 		except Exception as E:
 			print (E)
 			pass;
 			
-		time.sleep (1)
+		time.sleep (.25)
 	
 	
 	
 	response = requests.get (
 		intro_quay_URL + "/the_report"
 	)
 	the_report = json.loads (response.text);
@@ -325,15 +325,15 @@
 		nonlocal the_stop;
 		nonlocal barricaded;
 		
 		the_stop = True
 		
 		while barricaded == True:
 			print ("barricaded")	
-			time.sleep (1)
+			time.sleep (.25)
 		
 		return;
 
 	return {
 		"off": turn_off,
 		"proceeds": the_report
 	}
```

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/adventure.py` & `biotech-1.1.8/venues/stages/biotech/procedures/intro/process/adventure.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py` & `biotech-1.1.8/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py` & `biotech-1.1.8/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/keg/__init__.py` & `biotech-1.1.8/venues/stages/biotech/procedures/intro/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/aggregate/__init__.py` & `biotech-1.1.8/venues/stages/biotech/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__init__.py` & `biotech-1.1.8/venues/stages/biotech/topics/alarm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/exceptions.py` & `biotech-1.1.8/venues/stages/biotech/topics/exceptions.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__init__.py` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__init__.py` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/basin/treasury.py` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/basin/treasury.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/help_documentation/shares.s.HTML` & `biotech-1.1.8/venues/stages/biotech/topics/help_documentation/shares.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/implicit/proc/__init__.py` & `biotech-1.1.8/venues/stages/biotech/topics/implicit/proc/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/implicit/thread/__init__.py` & `biotech-1.1.8/venues/stages/biotech/topics/implicit/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/printout/passes.py` & `biotech-1.1.8/venues/stages/biotech/topics/printout/passes.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__init__.py` & `biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/implicit.py` & `biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/process_on/p_expect/parse_records.py` & `biotech-1.1.8/venues/stages/biotech/topics/process_on/p_expect/parse_records.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/process_on/sub/explicit.py` & `biotech-1.1.8/venues/stages/biotech/topics/process_on/sub/explicit.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/process_on/sub/implicit.py` & `biotech-1.1.8/venues/stages/biotech/topics/process_on/sub/implicit.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/quay/garage.py` & `biotech-1.1.8/venues/stages/biotech/topics/quay/garage.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_1.py` & `biotech-1.1.8/venues/stages/biotech/topics/quay/implicit_process_test_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_2.py` & `biotech-1.1.8/venues/stages/biotech/topics/quay/implicit_process_test_2.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_3.py` & `biotech-1.1.8/venues/stages/biotech/topics/quay/implicit_process_test_3.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/quay/implicit_process_test_4.py` & `biotech-1.1.8/venues/stages/biotech/topics/quay/implicit_process_test_4.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py` & `biotech-1.1.8/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/show/variable.py` & `biotech-1.1.8/venues/stages/biotech/topics/show/variable.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc` & `biotech-1.1.8/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/venues/stages/biotech/topics/start--/simultaneously.py` & `biotech-1.1.8/venues/stages/biotech/topics/start--/simultaneously.py`

 * *Files identical despite different names*

### Comparing `biotech-1.1.7/PKG-INFO` & `biotech-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotech
-Version: 1.1.7
+Version: 1.1.8
 Summary: A health monitoring stack
 License: GPL-3.0-only
 Keywords: alarms,screening,monitors,cybernetics,neurons,nervous system,bioelectric,homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

