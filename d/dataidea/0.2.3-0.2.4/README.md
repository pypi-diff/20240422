# Comparing `tmp/dataidea-0.2.3.tar.gz` & `tmp/dataidea-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataidea-0.2.3.tar", max compression
+gzip compressed data, was "dataidea-0.2.4.tar", max compression
```

## Comparing `dataidea-0.2.3.tar` & `dataidea-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       41 2024-04-18 17:10:00.344848 dataidea-0.2.3/README.md
--rw-r--r--   0        0        0      229 2024-04-19 06:31:05.013813 dataidea-0.2.3/dataidea/datasets/cluster.csv
--rw-r--r--   0        0        0     4645 2024-04-19 06:33:56.213774 dataidea-0.2.3/dataidea/datasets/demo.csv
--rw-r--r--   0        0        0    47391 2024-04-19 06:31:05.017817 dataidea-0.2.3/dataidea/datasets/fpl.csv
--rw-r--r--   0        0        0      370 2024-04-19 06:31:05.021821 dataidea-0.2.3/dataidea/datasets/homeprices.csv
--rw-r--r--   0        0        0  2091239 2024-04-19 06:31:05.025825 dataidea-0.2.3/dataidea/datasets/melbourne.csv
--rw-r--r--   0        0        0      302 2024-04-19 06:31:05.029829 dataidea-0.2.3/dataidea/datasets/music.csv
--rw-r--r--   0        0        0      656 2024-04-19 06:31:05.029829 dataidea-0.2.3/dataidea/datasets/salaries.csv
--rw-r--r--   0        0        0   108285 2024-04-19 06:31:05.029829 dataidea-0.2.3/dataidea/datasets/titanic.csv
--rw-r--r--   0        0        0  1355781 2024-04-19 06:31:05.033833 dataidea-0.2.3/dataidea/datasets/vgsales.csv
--rw-r--r--   0        0        0      217 2024-04-19 06:31:05.033833 dataidea-0.2.3/dataidea/datasets/weather.csv
--rw-r--r--   0        0        0      822 2024-04-19 07:57:01.831308 dataidea-0.2.3/dataidea/datasets.py
--rw-r--r--   0        0        0      210 2024-04-19 05:07:03.723401 dataidea-0.2.3/dataidea/feature_selection.py
--rw-r--r--   0        0        0      469 2024-04-19 07:45:59.402478 dataidea-0.2.3/dataidea/models.py
--rw-r--r--   0        0        0      196 2024-04-19 07:58:11.939142 dataidea-0.2.3/dataidea/packages.py
--rw-r--r--   0        0        0      989 2024-04-19 10:31:36.565744 dataidea-0.2.3/dataidea/tabular.py
--rw-r--r--   0        0        0      481 2024-04-19 10:43:39.882622 dataidea-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 dataidea-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     8646 2024-04-21 19:27:31.509014 dataidea-0.2.4/README.md
+-rw-r--r--   0        0        0      229 2024-04-19 06:31:05.013813 dataidea-0.2.4/dataidea/datasets/cluster.csv
+-rw-r--r--   0        0        0     4645 2024-04-19 06:33:56.213774 dataidea-0.2.4/dataidea/datasets/demo.csv
+-rw-r--r--   0        0        0    47391 2024-04-19 06:31:05.017817 dataidea-0.2.4/dataidea/datasets/fpl.csv
+-rw-r--r--   0        0        0      370 2024-04-19 06:31:05.021821 dataidea-0.2.4/dataidea/datasets/homeprices.csv
+-rw-r--r--   0        0        0  2091239 2024-04-19 06:31:05.025825 dataidea-0.2.4/dataidea/datasets/melbourne.csv
+-rw-r--r--   0        0        0      302 2024-04-19 06:31:05.029829 dataidea-0.2.4/dataidea/datasets/music.csv
+-rw-r--r--   0        0        0      656 2024-04-19 06:31:05.029829 dataidea-0.2.4/dataidea/datasets/salaries.csv
+-rw-r--r--   0        0        0   108285 2024-04-19 06:31:05.029829 dataidea-0.2.4/dataidea/datasets/titanic.csv
+-rw-r--r--   0        0        0  1355781 2024-04-19 06:31:05.033833 dataidea-0.2.4/dataidea/datasets/vgsales.csv
+-rw-r--r--   0        0        0      217 2024-04-19 06:31:05.033833 dataidea-0.2.4/dataidea/datasets/weather.csv
+-rw-r--r--   0        0        0     3767 2024-04-21 10:09:01.374308 dataidea-0.2.4/dataidea/datasets.py
+-rw-r--r--   0        0        0      210 2024-04-19 05:07:03.723401 dataidea-0.2.4/dataidea/feature_selection.py
+-rw-r--r--   0        0        0     2816 2024-04-21 19:11:14.394771 dataidea-0.2.4/dataidea/models.py
+-rw-r--r--   0        0        0      167 2024-04-21 19:28:54.845536 dataidea-0.2.4/dataidea/packages.py
+-rw-r--r--   0        0        0      284 2024-04-20 15:08:51.951883 dataidea-0.2.4/dataidea/statistics.py
+-rw-r--r--   0        0        0       96 2024-04-20 14:03:53.712195 dataidea-0.2.4/dataidea/tabular.py
+-rw-r--r--   0        0        0      481 2024-04-21 19:28:23.018071 dataidea-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     9445 1970-01-01 00:00:00.000000 dataidea-0.2.4/PKG-INFO
```

### Comparing `dataidea-0.2.3/dataidea/datasets/demo.csv` & `dataidea-0.2.4/dataidea/datasets/demo.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.3/dataidea/datasets/fpl.csv` & `dataidea-0.2.4/dataidea/datasets/fpl.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.3/dataidea/datasets/melbourne.csv` & `dataidea-0.2.4/dataidea/datasets/melbourne.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.3/dataidea/datasets/salaries.csv` & `dataidea-0.2.4/dataidea/datasets/salaries.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.3/dataidea/datasets/titanic.csv` & `dataidea-0.2.4/dataidea/datasets/titanic.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.3/dataidea/datasets/vgsales.csv` & `dataidea-0.2.4/dataidea/datasets/vgsales.csv`

 * *Files identical despite different names*

