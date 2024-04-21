# Comparing `tmp/pkscreener-0.44.20240421.282.tar.gz` & `tmp/pkscreener-0.44.20240421.283.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240421.282.tar", last modified: Sun Apr 21 04:43:19 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240421.283.tar", last modified: Sun Apr 21 05:41:11 2024, max compression
```

## Comparing `pkscreener-0.44.20240421.282.tar` & `pkscreener-0.44.20240421.283.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 04:43:19.500488 pkscreener-0.44.20240421.282/
--rw-rw-rw-   0        0        0     1086 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-21 04:43:19.500488 pkscreener-0.44.20240421.282/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 04:43:19.484864 pkscreener-0.44.20240421.282/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 04:43:19.500488 pkscreener-0.44.20240421.282/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25172 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9489 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7018 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3237 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29415 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17734 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8120 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   112347 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    47534 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    79711 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-21 04:43:12.000000 pkscreener-0.44.20240421.282/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   120943 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    48027 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    22817 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-21 04:43:19.484864 pkscreener-0.44.20240421.282/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-21 04:43:19.000000 pkscreener-0.44.20240421.282/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-21 04:43:19.500488 pkscreener-0.44.20240421.282/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-21 04:39:25.000000 pkscreener-0.44.20240421.282/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:41:11.508213 pkscreener-0.44.20240421.283/
+-rw-rw-rw-   0        0        0     1086 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-21 05:41:11.508213 pkscreener-0.44.20240421.283/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 05:41:11.492584 pkscreener-0.44.20240421.283/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:41:11.508213 pkscreener-0.44.20240421.283/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25172 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9489 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7018 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3237 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29415 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17730 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8120 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   112347 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    47854 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    79711 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-21 05:41:05.000000 pkscreener-0.44.20240421.283/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   120948 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    48027 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    22817 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-21 05:41:11.492584 pkscreener-0.44.20240421.283/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-21 05:41:11.000000 pkscreener-0.44.20240421.283/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-21 05:41:11.000000 pkscreener-0.44.20240421.283/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 05:41:11.000000 pkscreener-0.44.20240421.283/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-21 05:41:11.000000 pkscreener-0.44.20240421.283/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-21 05:41:11.000000 pkscreener-0.44.20240421.283/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-21 05:41:11.000000 pkscreener-0.44.20240421.283/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-21 05:41:11.508213 pkscreener-0.44.20240421.283/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-21 05:38:18.000000 pkscreener-0.44.20240421.283/setup.py
```

### Comparing `pkscreener-0.44.20240421.282/LICENSE` & `pkscreener-0.44.20240421.283/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/LICENSE-Others` & `pkscreener-0.44.20240421.283/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/PKG-INFO` & `pkscreener-0.44.20240421.283/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240421.282
+Version: 0.44.20240421.283
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240421.282.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240421.283.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.282/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.282/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.282/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240421.282/README.md` & `pkscreener-0.44.20240421.283/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.282/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.282/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.282/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240421.282/pkscreener/__init__.py` & `pkscreener-0.44.20240421.283/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/PKScanRunner.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                             len(listStockCodes),
                             PKScanRunner.configManager.cacheEnabled,
                             stock,
                             newlyListedOnly,
                             downloadOnly,
                             volumeRatio,
                             testBuild,
-                            userArgs.log,
+                            userArgs,
                             daysInPast,
                             (
                                 backtestPeriod
                                 if menuOption == "B"
                                 else PKScanRunner.configManager.effectiveDaysToLookback
                             ),
                             default_logger().level,
```

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/StockScreener.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         totalSymbols,
         shouldCache,
         stock,
         newlyListedOnly,
         downloadOnly,
         volumeRatio,
         testbuild=False,
-        printCounter=False,
+        userArgs=None,
         backtestDuration=0,
         backtestPeriodToLookback=30,
         logLevel=logging.NOTSET,
         portfolio=False,
         testData = None,
         hostRef=None,
     ):
@@ -86,14 +86,15 @@
         self.configManager = configManager
         screeningDictionary, saveDictionary = self.initResultDictionaries()
         fullData = None
         processedData = None
         fetcher = hostRef.fetcher
         screener = hostRef.screener
         candlePatterns = hostRef.candlePatterns
+        printCounter = userArgs.log if (userArgs is not None and userArgs.log is not None) else False
         userArgsLog = printCounter
         start_time = time.time()
         try:
             with hostRef.processingCounter.get_lock():
                 hostRef.processingCounter.value += 1
 
             volumeRatio, period = self.determineBasicConfigs(stock, newlyListedOnly, volumeRatio, logLevel, hostRef, configManager, screener, userArgsLog)
@@ -471,51 +472,52 @@
                         or (executeOption in [12,13,14,15,16,17,18,19,20,23,24,25] and isValidityCheckMet)
                         or (executeOption == 21 and (mfiStake > 0 and reversalOption in [3,5]))
                         or (executeOption == 21 and (mfiStake < 0 and reversalOption in [6,7]))
                         or (executeOption == 21 and (fairValueDiff > 0 and reversalOption in [8]))
                         or (executeOption == 21 and (fairValueDiff < 0 and reversalOption in [9]))
                         or (executeOption == 26)
                     ):
+                        isNotMonitoringDashboard = userArgs.monitor is None
                         # Now screen for common ones to improve performance
-                        if not (executeOption == 6 and reversalOption == 7):
+                        if isNotMonitoringDashboard and not (executeOption == 6 and reversalOption == 7):
                             if sys.version_info >= (3, 11):
                                 with SuppressOutput(suppress_stderr=True, suppress_stdout=True):
                                     screener.validateLorentzian(
                                         fullData,
                                         screeningDictionary,
                                         saveDictionary,
                                         lookFor=maLength, # 1 =Buy, 2 =Sell, 3 = Any
                                     )
-                        if not (executeOption in [1,2]):
+                        if isNotMonitoringDashboard and not (executeOption in [1,2]):
                             screener.findBreakoutValue(
                                 processedData,
                                 screeningDictionary,
                                 saveDictionary,
                                 daysToLookback=configManager.daysToLookback,
                                 alreadyBrokenout=(executeOption == 2),
                             )
-                        if executeOption != 3:
+                        if isNotMonitoringDashboard and executeOption != 3:
                             screener.validateConsolidation(
                                 processedData,
                                 screeningDictionary,
                                 saveDictionary,
                                 percentage=configManager.consolidationPercentage,
                             )
                         if executeOption != 5:
                             screener.validateRSI(
                                 processedData, screeningDictionary, saveDictionary, minRSI, maxRSI
                             )
                         screener.find52WeekHighLow(
                             fullData, saveDictionary, screeningDictionary
                         )
-                        if executeOption != 8:
+                        if isNotMonitoringDashboard and executeOption != 8:
                             screener.validateCCI(
                                 processedData, screeningDictionary, saveDictionary, minRSI, maxRSI
                             )
-                        if executeOption != 21 and backtestDuration == 0:
+                        if isNotMonitoringDashboard and executeOption != 21 and backtestDuration == 0:
                             # We don't need to have MFI or fair value data for backtesting because those
                             # are anyways only available for days in the past.
                             # For executeOption 21, we'd have already got the mfiStake and fairValueDiff
                             # Find general trend, MFI data and fairvalue only after the stocks are already screened
                             screener.findUptrend(
                                 fullData,
                                 screeningDictionary,
```

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/classes/keys.py` & `pkscreener-0.44.20240421.283/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/courbd.ttf` & `pkscreener-0.44.20240421.283/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/globals.py` & `pkscreener-0.44.20240421.283/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,15 +541,15 @@
             return initPostLevel1Execution(indexOption, executeOption, retrial=True)
     return indexOption, executeOption
 
 def labelDataForPrinting(screenResults, saveResults, configManager, volumeRatio,executeOption, reversalOption):
     # Publish to gSheet with https://github.com/burnash/gspread
     global menuChoiceHierarchy, userPassedArgs
     try:
-        isTrading = PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()
+        isTrading = PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]
         if isTrading or userPassedArgs.monitor:
             screenResults['RSI'] = screenResults['RSI'].astype(str) + "/" + screenResults['RSIi'].astype(str)
             saveResults['RSI'] = saveResults['RSI'].astype(str) + "/" + saveResults['RSIi'].astype(str)
         sortKey = ["Volume"] if "RSI" not in menuChoiceHierarchy else ("RSIi" if isTrading else "RSI")
         ascending = [False if "RSI" not in menuChoiceHierarchy else True]
         if executeOption == 21:
             if reversalOption in [3,5,6,7]:
@@ -618,15 +618,15 @@
 
 def isInterrupted():
     global keyboardInterruptEventFired
     return keyboardInterruptEventFired
 
 def refreshStockData():
     global stockDict, loadedStockData
-    stockDict = None
+    # stockDict = None
     loadedStockData = False
 
 # @tracelog
 def main(userArgs=None,optionalFinalOutcome_df=None):
     global screenResults, selectedChoice, defaultAnswer, menuChoiceHierarchy, screenCounter, screenResultsCounter, stockDict, userPassedArgs, loadedStockData, keyboardInterruptEvent, loadCount, maLength, newlyListedOnly, keyboardInterruptEventFired,strategyFilter, elapsed_time, start_time
     selectedChoice = {"0": "", "1": "", "2": "", "3": "", "4": ""}
     elapsed_time = 0
```

### Comparing `pkscreener-0.44.20240421.282/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240421.283/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240421.283/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240421.283/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240421.283/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240421.282
+Version: 0.44.20240421.283
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240421.282.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240421.283.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.282/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.282/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240420.281/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240421.282/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240421.282/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240421.283/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240421.282/setup.py` & `pkscreener-0.44.20240421.283/setup.py`

 * *Files identical despite different names*

