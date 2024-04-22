# Comparing `tmp/PyAibote-1.4.0.tar.gz` & `tmp/PyAibote-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAibote-1.4.0.tar", last modified: Fri Apr 12 00:37:11 2024, max compression
+gzip compressed data, was "PyAibote-1.4.1.tar", last modified: Mon Apr 22 03:40:19 2024, max compression
```

## Comparing `PyAibote-1.4.0.tar` & `PyAibote-1.4.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 00:37:11.570955 PyAibote-1.4.0/
--rw-rw-rw-   0        0        0     1089 2024-04-12 00:37:11.569955 PyAibote-1.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 00:37:10.862958 PyAibote-1.4.0/PyAibote/
--rw-rw-rw-   0        0        0     2788 2024-03-19 01:40:59.000000 PyAibote-1.4.0/PyAibote/AndroidBot.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:37:11.030957 PyAibote-1.4.0/PyAibote/AndroidBotModel/
--rw-rw-rw-   0        0        0     7670 2024-02-27 11:01:39.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
--rw-rw-rw-   0        0        0     2401 2024-04-11 06:32:49.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/AndroidLoadWait.py
--rw-rw-rw-   0        0        0     3104 2024-03-19 01:39:35.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/ColorFindingOperation.py
--rw-rw-rw-   0        0        0     6238 2024-01-18 22:33:52.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/Control.py
--rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/CoordinateOperation.py
--rw-rw-rw-   0        0        0    13015 2024-01-17 22:58:26.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0    18577 2024-04-12 00:30:00.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/EquipmentOperation.py
--rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/FileTransfer.py
--rw-rw-rw-   0        0        0     8280 2024-03-28 05:05:11.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/MapFindingOperation.py
--rw-rw-rw-   0        0        0     9150 2024-04-11 15:01:41.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/OcrCorrelation.py
--rw-rw-rw-   0        0        0     1207 2024-01-17 06:31:31.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
--rw-rw-rw-   0        0        0     9303 2024-01-18 00:26:45.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/ScreenshotOperation.py
--rw-rw-rw-   0        0        0     2012 2024-04-02 11:03:01.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/UrlRequest.py
--rw-rw-rw-   0        0        0     4476 2024-01-18 22:34:37.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     1867 2024-01-20 10:06:51.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/YoloService.py
--rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.4.0/PyAibote/AndroidBotModel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:37:11.137958 PyAibote-1.4.0/PyAibote/CommonUse/
--rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.4.0/PyAibote/CommonUse/ChatGenerative.py
--rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.4.0/PyAibote/CommonUse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:37:11.195958 PyAibote-1.4.0/PyAibote/Tool/
--rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.4.0/PyAibote/Tool/DatabaseFunc.py
--rw-rw-rw-   0        0        0     2188 2024-03-19 01:39:35.000000 PyAibote-1.4.0/PyAibote/Tool/DebugStartDriver.py
--rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.4.0/PyAibote/Tool/Logger.py
--rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.4.0/PyAibote/Tool/LoggerFunc.py
--rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.4.0/PyAibote/Tool/SendTcpData.py
--rw-rw-rw-   0        0        0      532 2024-01-13 09:10:40.000000 PyAibote-1.4.0/PyAibote/Tool/SocketServer.py
--rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.4.0/PyAibote/Tool/Sqlite3DataBase.py
--rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.4.0/PyAibote/Tool/UniversalFunction.py
--rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.4.0/PyAibote/Tool/WriteReadFileFunc.py
--rw-rw-rw-   0        0        0      550 2024-03-19 01:40:59.000000 PyAibote-1.4.0/PyAibote/Tool/__init__.py
--rw-rw-rw-   0        0        0     1998 2024-03-19 01:40:59.000000 PyAibote-1.4.0/PyAibote/WebBot.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:37:11.433959 PyAibote-1.4.0/PyAibote/WebBotModel/
--rw-rw-rw-   0        0        0     3645 2024-01-26 01:18:21.000000 PyAibote-1.4.0/PyAibote/WebBotModel/CookiesOperation.py
--rw-rw-rw-   0        0        0      978 2024-04-11 09:33:52.000000 PyAibote-1.4.0/PyAibote/WebBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    11550 2024-04-04 13:28:08.000000 PyAibote-1.4.0/PyAibote/WebBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.4.0/PyAibote/WebBotModel/IframeOperation.py
--rw-rw-rw-   0        0        0      890 2024-01-18 22:24:31.000000 PyAibote-1.4.0/PyAibote/WebBotModel/JSinjection.py
--rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.4.0/PyAibote/WebBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     3993 2024-01-13 12:29:13.000000 PyAibote-1.4.0/PyAibote/WebBotModel/PagesAndNavigation.py
--rw-rw-rw-   0        0        0     1091 2024-01-18 22:23:35.000000 PyAibote-1.4.0/PyAibote/WebBotModel/PopUpWindow.py
--rw-rw-rw-   0        0        0     3433 2024-04-11 06:33:06.000000 PyAibote-1.4.0/PyAibote/WebBotModel/WebLoadWait.py
--rw-rw-rw-   0        0        0     5606 2024-01-25 23:04:37.000000 PyAibote-1.4.0/PyAibote/WebBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0      654 2024-02-15 23:42:13.000000 PyAibote-1.4.0/PyAibote/WebBotModel/__init__.py
--rw-rw-rw-   0        0        0     4186 2024-03-19 01:40:59.000000 PyAibote-1.4.0/PyAibote/WindowsBot.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:37:11.567957 PyAibote-1.4.0/PyAibote/WindowsBotModel/
--rw-rw-rw-   0        0        0    20130 2024-03-28 05:07:36.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/ColorOperation.py
--rw-rw-rw-   0        0        0    21461 2024-03-28 05:02:42.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/DigitalHumanOperation.py
--rw-rw-rw-   0        0        0     1928 2024-04-12 00:34:19.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    14186 2024-01-18 22:29:18.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0     5207 2024-01-22 22:39:26.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/ExcelOperation.py
--rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     8395 2024-03-19 01:39:35.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/OcrOperation.py
--rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/OtherOperations.py
--rw-rw-rw-   0        0        0     2379 2024-03-22 11:06:00.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/SystemOperation.py
--rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     6402 2024-01-22 23:49:04.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/VoiceService.py
--rw-rw-rw-   0        0        0     7513 2024-01-18 22:31:38.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/WinHidCorrelation.py
--rw-rw-rw-   0        0        0     2424 2024-04-11 06:32:59.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/WinLoadWait.py
--rw-rw-rw-   0        0        0     8941 2024-04-11 09:46:20.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0     2936 2024-01-14 20:29:30.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/YoloOperation.py
--rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.4.0/PyAibote/WindowsBotModel/__init__.py
--rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.4.0/PyAibote/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 00:37:10.893959 PyAibote-1.4.0/PyAibote.egg-info/
--rw-rw-rw-   0        0        0     1089 2024-04-12 00:37:10.000000 PyAibote-1.4.0/PyAibote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2493 2024-04-12 00:37:10.000000 PyAibote-1.4.0/PyAibote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 00:37:10.000000 PyAibote-1.4.0/PyAibote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-12 00:37:10.000000 PyAibote-1.4.0/PyAibote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 00:37:10.000000 PyAibote-1.4.0/PyAibote.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9118 2024-04-11 10:04:43.000000 PyAibote-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 00:37:11.570955 PyAibote-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1425 2024-04-12 00:36:13.000000 PyAibote-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:40:19.765513 PyAibote-1.4.1/
+-rw-rw-rw-   0        0        0     1089 2024-04-22 03:40:19.764513 PyAibote-1.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-22 03:40:19.171737 PyAibote-1.4.1/PyAibote/
+-rw-rw-rw-   0        0        0     2788 2024-03-19 01:40:59.000000 PyAibote-1.4.1/PyAibote/AndroidBot.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:40:19.272735 PyAibote-1.4.1/PyAibote/AndroidBotModel/
+-rw-rw-rw-   0        0        0     7670 2024-02-27 11:01:39.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
+-rw-rw-rw-   0        0        0     2385 2024-04-22 03:35:50.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/AndroidLoadWait.py
+-rw-rw-rw-   0        0        0     3104 2024-03-19 01:39:35.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/ColorFindingOperation.py
+-rw-rw-rw-   0        0        0     6238 2024-01-18 22:33:52.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/Control.py
+-rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/CoordinateOperation.py
+-rw-rw-rw-   0        0        0    13015 2024-01-17 22:58:26.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0    18577 2024-04-12 00:30:00.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/EquipmentOperation.py
+-rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/FileTransfer.py
+-rw-rw-rw-   0        0        0     8280 2024-03-28 05:05:11.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/MapFindingOperation.py
+-rw-rw-rw-   0        0        0     9150 2024-04-11 15:01:41.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/OcrCorrelation.py
+-rw-rw-rw-   0        0        0     1207 2024-01-17 06:31:31.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
+-rw-rw-rw-   0        0        0     9303 2024-01-18 00:26:45.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/ScreenshotOperation.py
+-rw-rw-rw-   0        0        0     2012 2024-04-02 11:03:01.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/UrlRequest.py
+-rw-rw-rw-   0        0        0     4476 2024-01-18 22:34:37.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     1867 2024-01-20 10:06:51.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/YoloService.py
+-rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.4.1/PyAibote/AndroidBotModel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:40:19.303737 PyAibote-1.4.1/PyAibote/CommonUse/
+-rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.4.1/PyAibote/CommonUse/ChatGenerative.py
+-rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.4.1/PyAibote/CommonUse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:40:19.434395 PyAibote-1.4.1/PyAibote/Tool/
+-rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.4.1/PyAibote/Tool/DatabaseFunc.py
+-rw-rw-rw-   0        0        0     2188 2024-03-19 01:39:35.000000 PyAibote-1.4.1/PyAibote/Tool/DebugStartDriver.py
+-rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.4.1/PyAibote/Tool/Logger.py
+-rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.4.1/PyAibote/Tool/LoggerFunc.py
+-rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.4.1/PyAibote/Tool/SendTcpData.py
+-rw-rw-rw-   0        0        0      532 2024-01-13 09:10:40.000000 PyAibote-1.4.1/PyAibote/Tool/SocketServer.py
+-rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.4.1/PyAibote/Tool/Sqlite3DataBase.py
+-rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.4.1/PyAibote/Tool/UniversalFunction.py
+-rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.4.1/PyAibote/Tool/WriteReadFileFunc.py
+-rw-rw-rw-   0        0        0      550 2024-03-19 01:40:59.000000 PyAibote-1.4.1/PyAibote/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1998 2024-03-19 01:40:59.000000 PyAibote-1.4.1/PyAibote/WebBot.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:40:19.564313 PyAibote-1.4.1/PyAibote/WebBotModel/
+-rw-rw-rw-   0        0        0     3645 2024-01-26 01:18:21.000000 PyAibote-1.4.1/PyAibote/WebBotModel/CookiesOperation.py
+-rw-rw-rw-   0        0        0      978 2024-04-11 09:33:52.000000 PyAibote-1.4.1/PyAibote/WebBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    11550 2024-04-04 13:28:08.000000 PyAibote-1.4.1/PyAibote/WebBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.4.1/PyAibote/WebBotModel/IframeOperation.py
+-rw-rw-rw-   0        0        0      890 2024-01-18 22:24:31.000000 PyAibote-1.4.1/PyAibote/WebBotModel/JSinjection.py
+-rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.4.1/PyAibote/WebBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     3993 2024-01-13 12:29:13.000000 PyAibote-1.4.1/PyAibote/WebBotModel/PagesAndNavigation.py
+-rw-rw-rw-   0        0        0     1091 2024-01-18 22:23:35.000000 PyAibote-1.4.1/PyAibote/WebBotModel/PopUpWindow.py
+-rw-rw-rw-   0        0        0     3425 2024-04-22 03:36:11.000000 PyAibote-1.4.1/PyAibote/WebBotModel/WebLoadWait.py
+-rw-rw-rw-   0        0        0     5606 2024-01-25 23:04:37.000000 PyAibote-1.4.1/PyAibote/WebBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0      654 2024-02-15 23:42:13.000000 PyAibote-1.4.1/PyAibote/WebBotModel/__init__.py
+-rw-rw-rw-   0        0        0     4186 2024-03-19 01:40:59.000000 PyAibote-1.4.1/PyAibote/WindowsBot.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:40:19.762513 PyAibote-1.4.1/PyAibote/WindowsBotModel/
+-rw-rw-rw-   0        0        0    20130 2024-03-28 05:07:36.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/ColorOperation.py
+-rw-rw-rw-   0        0        0    21461 2024-03-28 05:02:42.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/DigitalHumanOperation.py
+-rw-rw-rw-   0        0        0     1928 2024-04-12 00:34:19.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    14186 2024-01-18 22:29:18.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0     5207 2024-01-22 22:39:26.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/ExcelOperation.py
+-rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     8395 2024-03-19 01:39:35.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/OcrOperation.py
+-rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/OtherOperations.py
+-rw-rw-rw-   0        0        0     2379 2024-03-22 11:06:00.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/SystemOperation.py
+-rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     6402 2024-01-22 23:49:04.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/VoiceService.py
+-rw-rw-rw-   0        0        0     7513 2024-01-18 22:31:38.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/WinHidCorrelation.py
+-rw-rw-rw-   0        0        0     2416 2024-04-22 03:36:27.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/WinLoadWait.py
+-rw-rw-rw-   0        0        0     8941 2024-04-11 09:46:20.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0     2936 2024-01-14 20:29:30.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/YoloOperation.py
+-rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.4.1/PyAibote/WindowsBotModel/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.4.1/PyAibote/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:40:19.196736 PyAibote-1.4.1/PyAibote.egg-info/
+-rw-rw-rw-   0        0        0     1089 2024-04-22 03:40:18.000000 PyAibote-1.4.1/PyAibote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2493 2024-04-22 03:40:18.000000 PyAibote-1.4.1/PyAibote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 03:40:18.000000 PyAibote-1.4.1/PyAibote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-22 03:40:18.000000 PyAibote-1.4.1/PyAibote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-22 03:40:18.000000 PyAibote-1.4.1/PyAibote.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9118 2024-04-11 10:04:43.000000 PyAibote-1.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 03:40:19.765513 PyAibote-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2024-04-22 03:39:09.000000 PyAibote-1.4.1/setup.py
```

### Comparing `PyAibote-1.4.0/PKG-INFO` & `PyAibote-1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.4.0
+Version: 1.4.1
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7,<4.0
```

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBot.py` & `PyAibote-1.4.1/PyAibote/AndroidBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/AndroidHidCorrelation.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/AndroidHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/AndroidLoadWait.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/AndroidLoadWait.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     Show_Waiting_Throwing = False
 
     def _Send(self,data):
         if len(data) > 10000:
             self.debug(rf"->>> {data[:100]}......")
         else:
             self.debug(rf"->>> {data}")
-                    
+
         self.request.sendall(data)
         response = self.request.recv(87654)
         if response == b"":
             raise ConnectionAbortedError(f"{self.client_address[0]}:{self.client_address[1]} Client disconnects")
         data_length, data = response.split(b"/", 1)
-        while int(data_length) > len(response):
-            response += self.request.recv(87654)
-
+        while int(data_length) > len(data):
+            data += self.request.recv(87654)
+            
         response = response.decode('UTF-8')
         if len(response) > 10000:
             self.debug(rf"<-<- {response[:100]}......")
         else:
             self.debug(rf"<-<- {response}")
         return response
```

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/ColorFindingOperation.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/ColorFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/Control.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/Control.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/CoordinateOperation.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/CoordinateOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/ElementOperation.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/EquipmentOperation.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/EquipmentOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/FileTransfer.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/FileTransfer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/MapFindingOperation.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/MapFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/OcrCorrelation.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/OcrCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/ScreenProjectionOperation.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/ScreenProjectionOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/ScreenshotOperation.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/ScreenshotOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/UrlRequest.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/UrlRequest.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/VerificationCodeOperation.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/YoloService.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/YoloService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/AndroidBotModel/__init__.py` & `PyAibote-1.4.1/PyAibote/AndroidBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/CommonUse/ChatGenerative.py` & `PyAibote-1.4.1/PyAibote/CommonUse/ChatGenerative.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/Tool/DatabaseFunc.py` & `PyAibote-1.4.1/PyAibote/Tool/DatabaseFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/Tool/DebugStartDriver.py` & `PyAibote-1.4.1/PyAibote/Tool/DebugStartDriver.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/Tool/Logger.py` & `PyAibote-1.4.1/PyAibote/Tool/Logger.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/Tool/LoggerFunc.py` & `PyAibote-1.4.1/PyAibote/Tool/LoggerFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/Tool/SendTcpData.py` & `PyAibote-1.4.1/PyAibote/Tool/SendTcpData.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/Tool/SocketServer.py` & `PyAibote-1.4.1/PyAibote/Tool/SocketServer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/Tool/Sqlite3DataBase.py` & `PyAibote-1.4.1/PyAibote/Tool/Sqlite3DataBase.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/Tool/UniversalFunction.py` & `PyAibote-1.4.1/PyAibote/Tool/UniversalFunction.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/Tool/WriteReadFileFunc.py` & `PyAibote-1.4.1/PyAibote/Tool/WriteReadFileFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/Tool/__init__.py` & `PyAibote-1.4.1/PyAibote/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WebBot.py` & `PyAibote-1.4.1/PyAibote/WebBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WebBotModel/CookiesOperation.py` & `PyAibote-1.4.1/PyAibote/WebBotModel/CookiesOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WebBotModel/DrivingOperation.py` & `PyAibote-1.4.1/PyAibote/WebBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WebBotModel/ElementOperation.py` & `PyAibote-1.4.1/PyAibote/WebBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WebBotModel/IframeOperation.py` & `PyAibote-1.4.1/PyAibote/WebBotModel/IframeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WebBotModel/JSinjection.py` & `PyAibote-1.4.1/PyAibote/WebBotModel/JSinjection.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WebBotModel/KeymouseOperation.py` & `PyAibote-1.4.1/PyAibote/WebBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WebBotModel/PagesAndNavigation.py` & `PyAibote-1.4.1/PyAibote/WebBotModel/PagesAndNavigation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WebBotModel/PopUpWindow.py` & `PyAibote-1.4.1/PyAibote/WebBotModel/PopUpWindow.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WebBotModel/WebLoadWait.py` & `PyAibote-1.4.1/PyAibote/WebBotModel/WebLoadWait.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         self.debug(rf"->>> {data}")
 
         self.request.sendall(data)
         response = self.request.recv(87654)
         if response == b"":
             raise ConnectionAbortedError(f"{self.client_address[0]}:{self.client_address[1]} Client disconnects")
         data_length, data = response.split(b"/", 1)
-        while int(data_length) > len(response):
-            response += self.request.recv(87654)
+        while int(data_length) > len(data):
+            data += self.request.recv(87654)
 
         response = response.decode('UTF-8')
         if len(response) > 10000:
             self.debug(rf"<-<- {response[:100]}......")
         else:
             self.debug(rf"<-<- {response}")
         if response == b"":
```

### Comparing `PyAibote-1.4.0/PyAibote/WebBotModel/WindowOperation.py` & `PyAibote-1.4.1/PyAibote/WebBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WebBotModel/__init__.py` & `PyAibote-1.4.1/PyAibote/WebBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBot.py` & `PyAibote-1.4.1/PyAibote/WindowsBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/ColorOperation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/ColorOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/DigitalHumanOperation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/DigitalHumanOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/DrivingOperation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/ElementOperation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/ExcelOperation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/ExcelOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/KeymouseOperation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/OcrOperation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/OcrOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/OtherOperations.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/OtherOperations.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/SystemOperation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/SystemOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/VerificationCodeOperation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/VoiceService.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/VoiceService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/WinHidCorrelation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/WinHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/WinLoadWait.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/WinLoadWait.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         self.debug(rf"->>> {data}")
 
         self.request.sendall(data)
         response = self.request.recv(87654)
         if response == b"":
             raise ConnectionAbortedError(f"{self.client_address[0]}:{self.client_address[1]} Client disconnects")
         data_length, data = response.split(b"/", 1)
-        while int(data_length) > len(response):
-            response += self.request.recv(87654)
+        while int(data_length) > len(data):
+            data += self.request.recv(87654)
 
         response = response.decode('UTF-8')
         if len(response) > 10000:
             self.debug(rf"<-<- {response[:100]}......")
         else:
             self.debug(rf"<-<- {response}")
         if response == b"":
```

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/WindowOperation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/YoloOperation.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/YoloOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote/WindowsBotModel/__init__.py` & `PyAibote-1.4.1/PyAibote/WindowsBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/PyAibote.egg-info/PKG-INFO` & `PyAibote-1.4.1/PyAibote.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.4.0
+Version: 1.4.1
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7,<4.0
```

### Comparing `PyAibote-1.4.0/PyAibote.egg-info/SOURCES.txt` & `PyAibote-1.4.1/PyAibote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/README.md` & `PyAibote-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.0/setup.py` & `PyAibote-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Pillow",
     "requests",
     "pymysql"
 ]
 
 setup(
     name="PyAibote", 
-    version="1.4.0", 
+    version="1.4.1", 
     author="Riven", 
     author_email="pyaibote@163.com", 
     description="A pure code RPA office automation framework, which supports Android, Browser and Windows", 
     long_description="Support Android native APP and H5 interface elements and color positioning. The speed of element location is 10 times that of Appium framework, and the color location of 2340*1080 image only takes 50 milliseconds, It supports the positioning of window interface elements and colors developed by Windows applications,. NET, WinForm, WPF, QT, Java (GUI libraries such JAVA(Swing and AWT) and Electron. The exclusive xpath algorithm is concise and rapid, and the positioning speed of elements/colors is 3 times and 20 times that of visual RPA, respectively, All browsers and applications that support the chromium kernel. A web automation framework developed by C/C++ language based on browser kernel protocol. Ten times faster than Selenium", # 加载read_me的内容
     long_description_content_type="text/markdown", 
     url="https://www.pyaibote.com",  
     packages=packages,
```

