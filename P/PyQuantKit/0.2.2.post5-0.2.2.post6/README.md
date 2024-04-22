# Comparing `tmp/PyQuantKit-0.2.2.post5.tar.gz` & `tmp/PyQuantKit-0.2.2.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQuantKit-0.2.2.post5.tar", last modified: Wed Mar 13 05:50:27 2024, max compression
+gzip compressed data, was "PyQuantKit-0.2.2.post6.tar", last modified: Mon Apr 22 08:13:44 2024, max compression
```

## Comparing `PyQuantKit-0.2.2.post5.tar` & `PyQuantKit-0.2.2.post6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2024-03-13 05:50:27.317143 PyQuantKit-0.2.2.post5/
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     1066 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post5/LICENSE
--rw-r--r--   0 bolun     (1000) bolun     (1000)      610 2024-03-13 05:50:27.317143 PyQuantKit-0.2.2.post5/PKG-INFO
-drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2024-03-13 05:50:27.317143 PyQuantKit-0.2.2.post5/PyQuantKit/
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    35885 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post5/PyQuantKit/ConsoleUtils.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    51859 2024-03-13 05:50:03.000000 PyQuantKit-0.2.2.post5/PyQuantKit/MarketUtils_lite.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    68097 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post5/PyQuantKit/MarketUtils_old.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    16240 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post5/PyQuantKit/TechnicalAnalysis.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)    19560 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post5/PyQuantKit/TradeUtils.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     7923 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post5/PyQuantKit/_FinanceDecimal.py
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     2976 2024-03-13 05:50:19.000000 PyQuantKit-0.2.2.post5/PyQuantKit/__init__.py
-drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2024-03-13 05:50:27.317143 PyQuantKit-0.2.2.post5/PyQuantKit.egg-info/
--rw-r--r--   0 bolun     (1000) bolun     (1000)      610 2024-03-13 05:50:27.000000 PyQuantKit-0.2.2.post5/PyQuantKit.egg-info/PKG-INFO
--rw-rw-r--   0 bolun     (1000) bolun     (1000)      393 2024-03-13 05:50:27.000000 PyQuantKit-0.2.2.post5/PyQuantKit.egg-info/SOURCES.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)        1 2024-03-13 05:50:27.000000 PyQuantKit-0.2.2.post5/PyQuantKit.egg-info/dependency_links.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       13 2024-03-13 05:50:27.000000 PyQuantKit-0.2.2.post5/PyQuantKit.egg-info/requires.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       11 2024-03-13 05:50:27.000000 PyQuantKit-0.2.2.post5/PyQuantKit.egg-info/top_level.txt
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       53 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post5/README.md
--rw-rw-r--   0 bolun     (1000) bolun     (1000)       38 2024-03-13 05:50:27.317143 PyQuantKit-0.2.2.post5/setup.cfg
--rw-rw-r--   0 bolun     (1000) bolun     (1000)     1491 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post5/setup.py
+drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2024-04-22 08:13:44.302621 PyQuantKit-0.2.2.post6/
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)     1066 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/LICENSE
+-rw-r--r--   0 bolun     (1000) bolun     (1000)      610 2024-04-22 08:13:44.302621 PyQuantKit-0.2.2.post6/PKG-INFO
+drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2024-04-22 08:13:44.298621 PyQuantKit-0.2.2.post6/PyQuantKit/
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)    35885 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/PyQuantKit/ConsoleUtils.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)    51884 2024-04-22 08:13:10.000000 PyQuantKit-0.2.2.post6/PyQuantKit/MarketUtils_lite.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)    68097 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/PyQuantKit/MarketUtils_old.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)    16240 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/PyQuantKit/TechnicalAnalysis.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)    19560 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/PyQuantKit/TradeUtils.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)     7923 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/PyQuantKit/_FinanceDecimal.py
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)     2976 2024-04-22 08:13:32.000000 PyQuantKit-0.2.2.post6/PyQuantKit/__init__.py
+drwxrwxr-x   0 bolun     (1000) bolun     (1000)        0 2024-04-22 08:13:44.302621 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/
+-rw-r--r--   0 bolun     (1000) bolun     (1000)      610 2024-04-22 08:13:44.000000 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/PKG-INFO
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)      393 2024-04-22 08:13:44.000000 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)        1 2024-04-22 08:13:44.000000 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)       13 2024-04-22 08:13:44.000000 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/requires.txt
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)       11 2024-04-22 08:13:44.000000 PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/top_level.txt
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)       53 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/README.md
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)       38 2024-04-22 08:13:44.302621 PyQuantKit-0.2.2.post6/setup.cfg
+-rw-rw-r--   0 bolun     (1000) bolun     (1000)     1491 2024-03-11 05:58:48.000000 PyQuantKit-0.2.2.post6/setup.py
```

### Comparing `PyQuantKit-0.2.2.post5/LICENSE` & `PyQuantKit-0.2.2.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.2.post5/PKG-INFO` & `PyQuantKit-0.2.2.post6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQuantKit
-Version: 0.2.2.post5
+Version: 0.2.2.post6
 Summary: Python Toolkit for Quantitative Finance
 Home-page: https://github.com/BolunHan/PyQuantKit.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PyQuantKit-0.2.2.post5/PyQuantKit/ConsoleUtils.py` & `PyQuantKit-0.2.2.post6/PyQuantKit/ConsoleUtils.py`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.2.post5/PyQuantKit/MarketUtils_lite.py` & `PyQuantKit-0.2.2.post6/PyQuantKit/MarketUtils_lite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1414,22 +1414,22 @@
         self.total_trade_count.value = market_data['total_trade_count']
 
     def to_market_data(self) -> TickData:
         tick_data = TickData(
             ticker=self.ticker.value,
             timestamp=self.timestamp.value,
             last_price=self.last_price.value,
-            bid_price=self.last_price.value,
-            bid_volume=self.last_price.value,
-            ask_price=self.last_price.value,
-            ask_volume=self.last_price.value,
+            bid_price=self.bid_price.value,
+            bid_volume=self.bid_volume.value,
+            ask_price=self.ask_price.value,
+            ask_volume=self.ask_volume.value,
             order_book=None,
-            total_traded_volume=self.last_price.value,
-            total_traded_notional=self.last_price.value,
-            total_trade_count=self.last_price.value,
+            total_traded_volume=self.total_traded_volume.value,
+            total_traded_notional=self.total_traded_notional.value,
+            total_trade_count=self.total_trade_count.value,
         )
 
         return tick_data
 
 
 class TransactionDataBuffer(_MarketDataMemoryBuffer):
     def __init__(self):
```

### Comparing `PyQuantKit-0.2.2.post5/PyQuantKit/MarketUtils_old.py` & `PyQuantKit-0.2.2.post6/PyQuantKit/MarketUtils_old.py`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.2.post5/PyQuantKit/TechnicalAnalysis.py` & `PyQuantKit-0.2.2.post6/PyQuantKit/TechnicalAnalysis.py`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.2.post5/PyQuantKit/TradeUtils.py` & `PyQuantKit-0.2.2.post6/PyQuantKit/TradeUtils.py`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.2.post5/PyQuantKit/_FinanceDecimal.py` & `PyQuantKit-0.2.2.post6/PyQuantKit/_FinanceDecimal.py`

 * *Files identical despite different names*

### Comparing `PyQuantKit-0.2.2.post5/PyQuantKit/__init__.py` & `PyQuantKit-0.2.2.post6/PyQuantKit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = '0.2.2.post5'
+__version__ = '0.2.2.post6'
 
 import logging
 import sys
 import time
 
 LOGGER: logging.Logger | None = None
 LOG_LEVEL = logging.INFO
```

### Comparing `PyQuantKit-0.2.2.post5/PyQuantKit.egg-info/PKG-INFO` & `PyQuantKit-0.2.2.post6/PyQuantKit.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQuantKit
-Version: 0.2.2.post5
+Version: 0.2.2.post6
 Summary: Python Toolkit for Quantitative Finance
 Home-page: https://github.com/BolunHan/PyQuantKit.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PyQuantKit-0.2.2.post5/setup.py` & `PyQuantKit-0.2.2.post6/setup.py`

 * *Files identical despite different names*

