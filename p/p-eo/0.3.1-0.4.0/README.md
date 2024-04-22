# Comparing `tmp/p_eo-0.3.1-py3-none-any.whl.zip` & `tmp/p_eo-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 14773 bytes, number of entries: 16
--rw-r--r--  2.0 unx      250 b- defN 24-Apr-17 09:59 P_EO/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 09:59 P_EO/common/__init__.py
--rw-r--r--  2.0 unx      387 b- defN 24-Apr-17 09:59 P_EO/common/config.py
--rw-r--r--  2.0 unx     1619 b- defN 24-Apr-17 09:59 P_EO/common/error.py
--rw-r--r--  2.0 unx     1709 b- defN 24-Apr-17 09:59 P_EO/common/log.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 09:59 P_EO/core/__init__.py
--rw-r--r--  2.0 unx    10508 b- defN 24-Apr-17 09:59 P_EO/core/action.py
--rw-r--r--  2.0 unx     5372 b- defN 24-Apr-17 09:59 P_EO/core/driver.py
--rw-r--r--  2.0 unx     6456 b- defN 24-Apr-17 09:59 P_EO/core/elements.py
--rw-r--r--  2.0 unx     1161 b- defN 24-Apr-17 09:59 P_EO/core/javascript.py
--rw-r--r--  2.0 unx     1315 b- defN 24-Apr-17 09:59 P_EO/core/page.py
--rw-r--r--  2.0 unx    11558 b- defN 24-Apr-17 09:59 p_eo-0.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      319 b- defN 24-Apr-17 09:59 p_eo-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 09:59 p_eo-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-17 09:59 p_eo-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1208 b- defN 24-Apr-17 09:59 p_eo-0.3.1.dist-info/RECORD
-16 files, 41959 bytes uncompressed, 12811 bytes compressed:  69.5%
+Zip file size: 14994 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      318 b- defN 24-Apr-22 05:34 P_EO/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 05:34 P_EO/common/__init__.py
+-rw-r--r--  2.0 unx      387 b- defN 24-Apr-22 05:34 P_EO/common/config.py
+-rw-r--r--  2.0 unx     1619 b- defN 24-Apr-22 05:34 P_EO/common/error.py
+-rw-r--r--  2.0 unx     1709 b- defN 24-Apr-22 05:34 P_EO/common/log.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 05:34 P_EO/core/__init__.py
+-rw-r--r--  2.0 unx    10508 b- defN 24-Apr-22 05:34 P_EO/core/action.py
+-rw-r--r--  2.0 unx     6077 b- defN 24-Apr-22 05:34 P_EO/core/driver.py
+-rw-r--r--  2.0 unx     6456 b- defN 24-Apr-22 05:34 P_EO/core/elements.py
+-rw-r--r--  2.0 unx     1161 b- defN 24-Apr-22 05:34 P_EO/core/javascript.py
+-rw-r--r--  2.0 unx     1315 b- defN 24-Apr-22 05:34 P_EO/core/page.py
+-rw-r--r--  2.0 unx    11558 b- defN 24-Apr-22 05:35 p_eo-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      354 b- defN 24-Apr-22 05:35 p_eo-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 05:35 p_eo-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-22 05:35 p_eo-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1208 b- defN 24-Apr-22 05:35 p_eo-0.4.0.dist-info/RECORD
+16 files, 42767 bytes uncompressed, 13032 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: P_EO/core/javascript.py
 Comment: 
 
 Filename: P_EO/core/page.py
 Comment: 
 
-Filename: p_eo-0.3.1.dist-info/LICENSE
+Filename: p_eo-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: p_eo-0.3.1.dist-info/METADATA
+Filename: p_eo-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: p_eo-0.3.1.dist-info/WHEEL
+Filename: p_eo-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: p_eo-0.3.1.dist-info/top_level.txt
+Filename: p_eo-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: p_eo-0.3.1.dist-info/RECORD
+Filename: p_eo-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## P_EO/__init__.py

```diff
@@ -1,14 +1,16 @@
 from P_EO.common.config import Default, LogConfig
+from P_EO.core.driver import WebDriverManager
 from P_EO.core.elements import Element, Elements, IFrame
 from P_EO.core.page import Page
 
-VERSION = '0.3.1'
+VERSION = '0.4.0'
 
 __all__ = [
     Element,
     Elements,
     IFrame,
     Page,
     Default,
     LogConfig,
+    WebDriverManager,
 ]
```

## P_EO/core/driver.py

```diff
@@ -1,11 +1,13 @@
 import os.path
 import time
+from urllib.parse import urlparse
 
 from selenium.webdriver.remote.webdriver import WebDriver
+from webdrivermanager_cn import ChromeDriverManager, GeckodriverManager
 
 from P_EO.common.config import Default
 from P_EO.common.log import peo_logger
 from P_EO.core.javascript import JavaScript
 
 
 class Driver:
@@ -64,14 +66,22 @@
     def get_cur_url(self):
         """
         获取当前url
         :return:
         """
         return self.__d.current_url
 
+    @property
+    def get_cur_url_parser(self):
+        """
+        url解析器
+        :return:
+        """
+        return urlparse(self.get_cur_url)
+
     def open_url(self, url):
         """
         打开新url
         :param url:
         :return:
         """
         self.__d.get(url)
@@ -208,7 +218,25 @@
     @property
     def alert(self):
         """
         切换到 Alert 窗口
         :return:
         """
         return self.driver.switch_to.alert
+
+
+class WebDriverManager:
+    """
+    下载浏览器驱动
+    """
+
+    def __init__(self, driver_path: str = None, version='latest'):
+        self.__driver_path = driver_path
+        self.__version = version
+
+    @property
+    def chrome(self):
+        return ChromeDriverManager(self.__driver_path, self.__version).install()
+
+    @property
+    def firefox(self):
+        return GeckodriverManager(self.__driver_path, self.__version).install()
```

## Comparing `p_eo-0.3.1.dist-info/LICENSE` & `p_eo-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `p_eo-0.3.1.dist-info/RECORD` & `p_eo-0.4.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-P_EO/__init__.py,sha256=uPB9dpTLr7rP7RQ_W1PgiGZfwbFe_jkR4ekbHAlwGA0,250
+P_EO/__init__.py,sha256=otXgAJfLT64S5BLSa5DW31sHtCf4LHwVC68SYJ_pyGo,318
 P_EO/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 P_EO/common/config.py,sha256=J-AF4NgApJPT4SMlI2sfaErZfFhReXXobmr2nKenBXA,387
 P_EO/common/error.py,sha256=eoaHHTSo5sy6g1dtTfiRJNvwNc1ruDgv0tzHI67_lrE,1619
 P_EO/common/log.py,sha256=j6I7Cv8pXWMzeDr0tQ0AAvjBTBISnf2ojEfK_zn2sBs,1709
 P_EO/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 P_EO/core/action.py,sha256=Va1fqwMvbNi-IwHmoK-R-7iOWEAv-FcM-o5J3qHS4RA,10508
-P_EO/core/driver.py,sha256=nSaEp4xniNJYU9Q8NTrx_X1BmMA5OqxrPtXCyr7971M,5372
+P_EO/core/driver.py,sha256=opoSYYHmT2QESFZkBICtdr3Etue2gvuxpRswXOGg0lY,6077
 P_EO/core/elements.py,sha256=btoewjpUxst-tlU8x_TeKt9LFmbAHExshi3wOGbJCFA,6456
 P_EO/core/javascript.py,sha256=PqmqW_iq9GM4rdfGWXtdhmnP10WT0F2_Y9IFP4wlv38,1161
 P_EO/core/page.py,sha256=JuHxK9ERu0vZ_y7JOwL2ZQRTH221CUzQXVg7bcYo7V4,1315
-p_eo-0.3.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-p_eo-0.3.1.dist-info/METADATA,sha256=-hVSsUGBodfBRys6v9hu5Sw7FzZSwa2S__Y7aMLT73s,319
-p_eo-0.3.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-p_eo-0.3.1.dist-info/top_level.txt,sha256=l3zgFCnD5y70VQdYdQwMMn9JMvcXF1Qfn7Xnr6_2Nq8,5
-p_eo-0.3.1.dist-info/RECORD,,
+p_eo-0.4.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+p_eo-0.4.0.dist-info/METADATA,sha256=AKMoC4baxMFeu3k9rce8fCcGmbM5xSCePEaVYTeBYQs,354
+p_eo-0.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+p_eo-0.4.0.dist-info/top_level.txt,sha256=l3zgFCnD5y70VQdYdQwMMn9JMvcXF1Qfn7Xnr6_2Nq8,5
+p_eo-0.4.0.dist-info/RECORD,,
```

