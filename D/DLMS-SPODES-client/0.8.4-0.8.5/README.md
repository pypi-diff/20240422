# Comparing `tmp/DLMS_SPODES_client-0.8.4.tar.gz` & `tmp/DLMS_SPODES_client-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_client-0.8.4.tar", last modified: Fri Apr 19 04:49:07 2024, max compression
+gzip compressed data, was "DLMS_SPODES_client-0.8.5.tar", last modified: Mon Apr 22 07:37:50 2024, max compression
```

## Comparing `DLMS_SPODES_client-0.8.4.tar` & `DLMS_SPODES_client-0.8.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 04:49:07.673970 DLMS_SPODES_client-0.8.4/
--rw-rw-rw-   0        0        0      526 2024-04-19 04:49:07.672969 DLMS_SPODES_client-0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.8.4/README.md
--rw-rw-rw-   0        0        0      836 2024-04-19 04:49:00.000000 DLMS_SPODES_client-0.8.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 04:49:07.673970 DLMS_SPODES_client-0.8.4/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.8.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 04:49:07.453972 DLMS_SPODES_client-0.8.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 04:49:07.469969 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/
--rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/FCS16.py
--rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/__init__.py
--rw-rw-rw-   0        0        0   115315 2024-04-18 10:32:20.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/client.py
-drwxrwxrwx   0        0        0        0 2024-04-19 04:49:07.441979 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_common/
-drwxrwxrwx   0        0        0        0 2024-04-19 04:49:07.554975 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_common/enums/
--rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
--rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 04:49:07.600972 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/
--rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
--rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/CountType.py
--rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
--rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
--rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
--rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
--rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
--rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
--rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
--rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
--rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
--rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
--rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
--rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
--rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
--rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
--rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
--rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
--rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 04:49:07.656971 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/
--rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
--rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
--rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
--rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
--rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
--rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
--rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
--rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
--rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
--rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
--rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
--rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
--rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
--rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
--rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
--rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
--rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
--rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
--rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
--rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
--rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
--rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
--rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
--rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 04:49:07.659000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/internal/
--rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
--rw-rw-rw-   0        0        0     1908 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/logger.py
--rw-rw-rw-   0        0        0     5575 2024-04-18 10:32:20.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/servers.py
--rw-rw-rw-   0        0        0     3609 2024-04-15 10:18:59.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/services.py
--rw-rw-rw-   0        0        0    43920 2024-04-18 12:42:38.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/task.py
-drwxrwxrwx   0        0        0        0 2024-04-19 04:49:07.485001 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client.egg-info/
--rw-rw-rw-   0        0        0      526 2024-04-19 04:49:07.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3251 2024-04-19 04:49:07.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 04:49:07.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-19 04:49:07.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2024-04-19 04:49:07.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-19 04:49:07.000000 DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.8.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 04:49:07.670986 DLMS_SPODES_client-0.8.4/test/
--rw-rw-rw-   0        0        0       30 2024-04-15 07:35:51.000000 DLMS_SPODES_client-0.8.4/test/name2.csv
--rw-rw-rw-   0        0        0     8415 2024-04-18 07:59:03.000000 DLMS_SPODES_client-0.8.4/test/test_Client.py
--rw-rw-rw-   0        0        0      167 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.4/test/test_logger.py
--rw-rw-rw-   0        0        0      247 2024-04-15 08:13:39.000000 DLMS_SPODES_client-0.8.4/test/test_services.py
--rw-rw-rw-   0        0        0      290 2024-04-15 08:24:50.000000 DLMS_SPODES_client-0.8.4/test/конфигурация GSM.csv
+drwxrwxrwx   0        0        0        0 2024-04-22 07:37:50.714684 DLMS_SPODES_client-0.8.5/
+-rw-rw-rw-   0        0        0      526 2024-04-22 07:37:50.713689 DLMS_SPODES_client-0.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.8.5/README.md
+-rw-rw-rw-   0        0        0      836 2024-04-22 07:33:19.000000 DLMS_SPODES_client-0.8.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-22 07:37:50.714684 DLMS_SPODES_client-0.8.5/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:37:50.536681 DLMS_SPODES_client-0.8.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 07:37:50.555681 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/
+-rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/FCS16.py
+-rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/__init__.py
+-rw-rw-rw-   0        0        0   115215 2024-04-22 05:45:45.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:37:50.526681 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_common/
+drwxrwxrwx   0        0        0        0 2024-04-22 07:37:50.577681 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_common/enums/
+-rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:37:50.633682 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/
+-rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
+-rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/CountType.py
+-rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
+-rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
+-rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
+-rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
+-rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
+-rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
+-rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
+-rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
+-rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
+-rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
+-rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
+-rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
+-rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
+-rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
+-rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:37:50.697683 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/
+-rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
+-rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
+-rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
+-rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
+-rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
+-rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
+-rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
+-rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
+-rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
+-rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
+-rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
+-rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
+-rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
+-rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
+-rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
+-rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
+-rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
+-rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
+-rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
+-rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
+-rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
+-rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
+-rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:37:50.699688 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/internal/
+-rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
+-rw-rw-rw-   0        0        0     1908 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/logger.py
+-rw-rw-rw-   0        0        0     4992 2024-04-22 07:11:32.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/servers.py
+-rw-rw-rw-   0        0        0     3609 2024-04-15 10:18:59.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/services.py
+-rw-rw-rw-   0        0        0    45655 2024-04-22 07:11:32.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/task.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:37:50.571682 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-04-22 07:37:50.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3251 2024-04-22 07:37:50.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 07:37:50.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-22 07:37:50.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2024-04-22 07:37:50.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-22 07:37:50.000000 DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.8.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:37:50.710684 DLMS_SPODES_client-0.8.5/test/
+-rw-rw-rw-   0        0        0       30 2024-04-15 07:35:51.000000 DLMS_SPODES_client-0.8.5/test/name2.csv
+-rw-rw-rw-   0        0        0     9995 2024-04-22 05:57:16.000000 DLMS_SPODES_client-0.8.5/test/test_Client.py
+-rw-rw-rw-   0        0        0      167 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.5/test/test_logger.py
+-rw-rw-rw-   0        0        0      247 2024-04-15 08:13:39.000000 DLMS_SPODES_client-0.8.5/test/test_services.py
+-rw-rw-rw-   0        0        0      290 2024-04-15 08:24:50.000000 DLMS_SPODES_client-0.8.5/test/конфигурация GSM.csv
```

### Comparing `DLMS_SPODES_client-0.8.4/PKG-INFO` & `DLMS_SPODES_client-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_client
-Version: 0.8.4
+Version: 0.8.5
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.8.4/pyproject.toml` & `DLMS_SPODES_client-0.8.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_client"
-version = "0.8.4"
+version = "0.8.5"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
     "DLMS-SPODES == 0.69.6",
     "DLMS-SPODES-communications >= 1.2.4",
     "pycryptodomex>=3.15"
```

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/FCS16.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/FCS16.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/client.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,25 +92,33 @@
         """ more importance error or None if errors is absence"""
         try:
             return reduce(lambda a, b: a if a.importance > b.importance else b, self.keys())
         except TypeError:  # errors is empty
             return None
 
 
-class ConnectionState(IntFlag):
+class OSI(IntFlag):
     NONE = 0
-    """no connection"""
-    HDLC = auto()
-    """HDLC level"""
-    DLMS = auto()
-    """DLMS association level."""
+    PHYSICAL = auto()
+    DATA_LINK = auto()
+    NETWORK = auto()
+    TRANSPORT = auto()
+    SESSION = auto()
+    PRESENTATION = auto()
+    APPLICATION = auto()
 
     def __str__(self):
         return self.name
 
+    def __sub__(self, other):
+        return self.__class__(super(OSI, self).__sub__(other))
+
+    def __add__(self, other):
+        return self.__class__(super(OSI, self).__sub__(other))
+
 
 class State(ABC):
 
     @abstractmethod
     def __str__(self):
         """"""
 
@@ -150,15 +158,15 @@
             return False
 
 
 class Client:
     id: str | None
     __del_cb: Callable[[str], bool] | None
     status: Status  # todo all remove to state
-    connection_state: ConnectionState
+    level: OSI
     log_file: TextIO
     media: Network | SerialPort | RS485 | BLE | base.StreamBase | None
     lock: threading.Lock
     errors: Errors
     last_transfer_time: datetime.timedelta | None
     connection_time_release: int
     received_frames: Deque[frame.Frame]
@@ -237,15 +245,16 @@
         self.reply = GXReplyData()
         """ use gurux reply class now """
 
         self.received_frames = deque()
         """ HDLC frames container from server """
 
         self.send_frames = deque()
-        self.connection_state = ConnectionState.NONE
+        self.level = OSI.NONE
+        """OSI level"""
         self.settings = GXDLMSSettings(False)
         self.settings.interfaceType = InterfaceType.HDLC
 
         self.media = media
         """ physical layer """
 
         # TODO: TEMPORARY COMMENT
@@ -578,15 +587,15 @@
                 case XDLMSAPDU.GLO_READ_REQUEST | XDLMSAPDU.GLO_WRITE_REQUEST | XDLMSAPDU.GLO_GET_REQUEST | XDLMSAPDU.GLO_SET_REQUEST | XDLMSAPDU.GLO_ACTION_REQUEST | \
                      XDLMSAPDU.DED_GET_REQUEST | XDLMSAPDU.DED_SET_REQUEST | XDLMSAPDU.DED_ACTION_REQUEST:
                     if self.settings.cipher is None:
                         raise ValueError("Secure connection is not supported.")
                     if (self.reply.moreData & RequestTypes.FRAME) == 0:
                         self.reply.data.position = self.reply.data.position - 1
                         p = None
-                        if self.settings.cipher.dedicatedKey and (self.connection_state & ConnectionState.DLMS) != 0:
+                        if self.settings.cipher.dedicatedKey and (OSI.APPLICATION in self.level):
                             p = AesGcmParameter(self.settings.sourceSystemTitle, self.settings.cipher.dedicatedKey, self.settings.cipher.authenticationKey)
                         else:
                             p = AesGcmParameter(self.settings.sourceSystemTitle, self.settings.cipher.blockCipherKey, self.settings.cipher.authenticationKey)
                         tmp = GXCiphering.decrypt(self.settings.cipher, p, self.reply.data)
                         self.reply.data.clear()
                         self.reply.data.set(tmp)
                         self.reply.command = XDLMSAPDU(self.reply.data.getUInt8())
@@ -602,15 +611,15 @@
                     if self.settings.cipher is None:
                         raise ValueError("Secure connection is not supported.")
                     if (self.reply.moreData & RequestTypes.FRAME) == 0:
                         self.reply.data.position = self.reply.data.position - 1
                         bb = GXByteBuffer(self.reply.data)
                         self.reply.data.size = self.reply.data.position = index
                         p = None
-                        if self.settings.cipher.dedicatedKey and (self.connection_state & ConnectionState.DLMS) != 0:
+                        if self.settings.cipher.dedicatedKey and (OSI.APPLICATION in self.level):
                             p = AesGcmParameter(0, self.settings.sourceSystemTitle, self.settings.cipher.dedicatedKey, self.settings.cipher.authenticationKey)
                         else:
                             p = AesGcmParameter(0, self.settings.sourceSystemTitle, self.settings.cipher.blockCipherKey, self.settings.cipher.authenticationKey)
                         self.reply.data.set(GXCiphering.decrypt(self.settings.cipher, p, bb))
                         self.reply.command = None
                         self.getPdu()
                         self.reply.cipherIndex = self.reply.data.size
@@ -1056,34 +1065,34 @@
             self.log(logL.INFO, F"set2 to {self} communication channel: {self.media}")
         except Exception as e:
             self.log(logL.ERR, F"not set to {self} communication channel by {value}")
 
     async def close(self):
         """close """
         self.log(logL.DEB, "close")
-        if self.connection_state != ConnectionState.NONE:
+        if self.level > OSI.DATA_LINK:
             try:
                 # Release is call only for secured connections. All meters are not supporting Release and it's causing problems.
                 if self.settings.interfaceType == InterfaceType.WRAPPER or \
                         (self.settings.interfaceType == InterfaceType.HDLC and self.settings.cipher.security != Security.NONE):
                     self.releaseRequest()
                     await self.read_data_block()
             except Exception:
                 self.log(logL.WARN, "don't support release ReleaseRequest")
                 pass
                 #  All meters don't support release.
             finally:
-                self.connection_state = ConnectionState.HDLC
+                self.level = OSI.DATA_LINK
             # hdlc close
             try:
                 res = await self.disconnect_request()
                 # todo: handle res
             except Exception as e:
                 self.log(logL.ERR, F'Disconnect request ERROR: {e.args[0]}')
-        self.connection_state = ConnectionState.NONE
+        self.level -= OSI.DATA_LINK
         if self.status == Status.CONNECTED:
             self.status = Status.READY
 
     async def disconnect_request(self):
         """ Sent to server DISC """
         if self.settings.interfaceType == InterfaceType.HDLC:
             self.add_frames_to_queue(frame.Control.DISC_P)
@@ -1146,15 +1155,15 @@
         tmp = self.secure(ic, self.settings.ctoSChallenge, bytes(secret))
         challenge = cdt.OctetString(bytearray(tmp))
         equals = challenge == value
         if not equals:
             self.log(logL.DEB, "Invalid StoC:" + GXByteBuffer.hex(value, True) + "-" + GXByteBuffer.hex(tmp, True))
         if not equals:
             raise Exception("parseApplicationAssociationResponse failed. " + " Server to Client do not match.")
-        self.connection_state |= ConnectionState.DLMS
+        self.level |= OSI.APPLICATION
 
     def secure(self, ic, data, secret: bytes) -> bytes:
         """ TODO: """
         if not isinstance(secret, bytes):
             raise ValueError(F'cipher is not bytes type, got {secret.__class__}')
         #  Get server Challenge.
         challenge = GXByteBuffer()
@@ -1547,15 +1556,15 @@
         return resultDiagnosticValue
 
     def parseAareResponse(self, reply) -> AcseServiceUser:
         """ TODO: need refactoring. Parses the AARE response.  Parse method will update the following data: DLMSVersion, MaxReceivePDUSize, UseLogicalNameReferencing, LNSettings or SNSettings,
         LNSettings or SNSettings will be updated, depending on the referencing, Logical name or Short name.
         Received data. GXDLMSClient#aarqRequest GXDLMSClient#useLogicalNameReferencing GXDLMSClient#negotiatedConformance GXDLMSClient#proposedConformance """
         if (ret := self.parseAARE(reply)) != AcseServiceUser.AUTHENTICATION_REQUIRED:
-            self.connection_state = self.connection_state | ConnectionState.DLMS
+            self.level |= OSI.APPLICATION
         if self.settings.dlmsVersion != 6:
             raise ValueError("Invalid DLMS version number.")
         return ret
 
     def generate_user_information(self, cipher, encryptedData) -> bytes:
         info = pack('B', BerType.CONTEXT | BerType.CONSTRUCTED | AARQapdu.USER_INFORMATION)
         if not cipher or not cipher.isCiphered():
@@ -1605,15 +1614,14 @@
             self.proposed_conformance.contents,
             self.receive_pdu_size)
         return info
 
     def aarqRequest(self, m_id: mechanism_id.MechanismIdElement):
         """ Generate AARQ request.  Because all_ meters can't read all_ data in one packet, the packet must be split first, by using SplitDataToPackets method.  AARQ request as
         byte array. @see GXDLMSClient#parseAareResponse """
-        self.connection_state = self.connection_state & ~ConnectionState.DLMS
         info = bytes()
         self.settings.resetBlockIndex()
         self.settings.setStoCChallenge(None)
         # if self.auto_increase_invoke_ID:
         #     self.settings.setInvokeID(0)
         # else:
         #     self.settings.setInvokeID(1)
@@ -1914,15 +1922,15 @@
             info = pack('H', len(info)) + info
         buff = GXByteBuffer(info)
         if self.settings.getUseLogicalNameReferencing():
             p = GXDLMSLNParameters(self.settings, 0, ACSEAPDU.RLRQ, 0, buff, None, 0xff)
             reply = self.getLnMessages(p)
         else:
             reply = self.getSnMessages(GXDLMSSNParameters(self.settings, ACSEAPDU.RLRQ, 0xFF, 0xFF, None, buff))
-        self.connection_state = self.connection_state & ~ConnectionState.DLMS
+        self.level -= OSI.APPLICATION
         return reply
 
     @classmethod
     def getGloMessage(cls, command: XDLMSAPDU | ACSEAPDU) -> XDLMSAPDU | ACSEAPDU:
         """ Get used glo message. Executed command. Integer value of glo message."""
         match command:
             case XDLMSAPDU.READ_REQUEST:      return XDLMSAPDU.GLO_READ_REQUEST
@@ -1956,15 +1964,15 @@
             case _:                         raise Exception("Invalid DED command.")
 
     def cipher0(self, p: GXDLMSLNParameters, data: GXByteBuffer):
         cmd = 0
         key = None
         cipher = p.settings.cipher
         if not self.negotiated_conformance.general_protection:
-            if cipher.dedicatedKey and (p.connection_state & ConnectionState.DLMS) != 0:
+            if cipher.dedicatedKey and (OSI.APPLICATION in self.level):  # todo: maybe level is wrong
                 cmd = self.getDedMessage(p.command)
                 key = cipher.dedicatedKey
             else:
                 cmd = self.getGloMessage(p.command)
                 key = cipher.blockCipherKey
         else:
             if cipher.dedicatedKey:
@@ -1995,15 +2003,14 @@
     def current_association(self) -> AssociationLN:
         return self.objects.getAssociationBySAP(self.SAP)
 
     def get_SNRM_request(self):
         """ Generates SNRM request.  his method is used to generate send SNRMRequest. Before the SNRM request can be generated, at least the following properties must be set:
         ClientAddress, ServerAddress.
         According to IEC 62056-47: when communicating using TCP/IP, the SNRM request is not send. """
-        self.connection_state = ConnectionState.NONE
         self.add_frames_to_queue(control=frame.Control.SNRM_P)
 
     def add_frames_to_queue(self, control: frame.Control, data: bytes = bytes()):
         """ Create and set new frames to queue """
         new_frames: Deque[frame.Frame] = deque()
         """ frames container """
         if control == frame.Control.SNRM_P:
```

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/__init__.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/logger.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/logger.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/services.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/services.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client/task.py` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,59 @@
 from DLMS_SPODES.cosem_interface_classes import collection, overview
 from DLMS_SPODES.types import cdt, ut, cst
 from DLMS_SPODES.hdlc import frame
 from DLMS_SPODES.enums import Transmit, Application
 from DLMS_SPODES.obis import media_id
 from DLMS_SPODES.firmwares import get_firmware
 from DLMS_SPODES.cosem_interface_classes.image_transfer import image_transfer_status as i_t_status
-from .client import Client, pdu, logL, AppVersion, ConnectionState, Status, Security, Data, Conformance, mechanism_id, AcseServiceUser, State
+from .client import Client, pdu, logL, AppVersion, OSI, Status, Security, Data, Conformance, mechanism_id, AcseServiceUser, State
 
 
 class ExTask(ABC):
     """Exchange task for DLMS client"""
+    async def run(self, c: Client):
+        """exception handling block"""
+        try:
+            return await self.physical(c)
+        except (ConnectionRefusedError, TimeoutError) as e:
+            c.set_error(Transmit.NO_PORT, e.args[0])
+            return False  # todo: maybe never connected
+        except exc.DLMSException as e:
+            c.set_error(e.error, e.args[0])
+        except Exception as e:
+            c.log(logL.INFO, F'UNKNOWN ERROR: {e}...')
+            c.set_error(Transmit.UNKNOWN, F'При обмене{e}')
+        except asyncio.CancelledError as e:
+            c.set_error(Transmit.ABORT, "ручная остановка")
+            await c.close()  # todo: change to DiscRequest
+        finally:
+            c.received_frames.clear()  # for next exchange need clear all received frames. todo: this bag, remove in future
+
+    async def physical(self, c: Client):
+        if OSI.PHYSICAL not in c.level:
+            if not c.media.is_open():
+                await c.media.open()
+            c.level = OSI.PHYSICAL
+            c.set_error(Transmit.OK, "Open port")
+            c.log(logL.INFO, F"Open port communication channel: {c.media}")
+            if c.objects is None:
+                await InitType().exchange(c, is_public=True)
+                await c.close()  # todo: change to DiscRequest, or make not closed
+            ret = await self.exchange(c, is_public=True if isinstance(self, InitType) else False)
+            await c.close()  # todo: change to DiscRequest
+            return ret
+
     async def exchange(self, c: Client, is_public: bool = False):
-        if c.connection_state == ConnectionState.NONE:
+        if OSI.DATA_LINK not in c.level:
             if await get_HDLC(c, is_public) is False:
                 return False
         return await self.exchange_HDLC(c, is_public)
 
     async def exchange_HDLC(self, c: Client, is_public: bool = False):
-        if c.connection_state == ConnectionState.HDLC:
+        if OSI.APPLICATION not in c.level:
             if await get_AARE(c, is_public) is False:
                 return False
         return await self.exchange2(c)
 
     @abstractmethod
     async def exchange2(self, c: Client):
         """common exchange in session"""
@@ -61,15 +93,15 @@
         if c.settings.cipher.dedicatedKey:
             c.log(logL.DEB, F"Dedicated key: {c.settings.cipher.dedicatedKey.hex()}")
     # SNRM
     c.get_SNRM_request()
     c.status = Status.READ
     await c.read_data_block()
     c.status = Status.EXCHANGE
-    c.connection_state = ConnectionState.HDLC
+    c.level = OSI.DATA_LINK
     c.reply.clear()
     return True
 
 
 async def get_AARE(c: Client, is_public: bool = False) -> bool:
     if c.invocationCounter and c.settings.cipher is not None and c.settings.cipher.security != Security.NONE:
         # create IC object. TODO: remove it after close connection, maybe???
@@ -82,15 +114,16 @@
                                             version=cdt.Unsigned(0))
         tmp_client_SAP = c.current_association.associated_partners_id.client_SAP
         challenge = c.settings.ctoSChallenge
         try:
             c.objects.getIECHDLCSetup(c.get_channel_index()).set_from_info(c.reply.data.get_data())
             c.aarqRequest(c.m_id)
             await c.read_data_block()
-            c.parseAareResponse(c.reply.data)
+            ret = c.parseAareResponse(c.reply.data)
+            c.level |= OSI.APPLICATION  # todo: it's must be result of <ret> look down
             c.reply.clear()
             await c.read_attribute(IC, 2)
             c.settings.cipher.invocationCounter = 1 + IC.value.decode()
             c.log(logL.DEB, "Invocation counter: " + str(c.settings.cipher.invocationCounter))
             # disconnect
             if c.media and c.media.is_open():
                 c.log(logL.DEB, "DisconnectRequest")
@@ -142,14 +175,15 @@
 
     c.aarqRequest(mechanism_id.NONE if is_public else c.m_id)
     await c.read_data_block()
         # await c.read_attr(ut.CosemAttributeDescriptor((collection.ClassID.ASSOCIATION_LN, ut.CosemObjectInstanceId("0.0.40.0.0.255"), ut.CosemObjectAttributeId(6)))) # for test only
     match c.parseAareResponse(c.reply.data):
         case AcseServiceUser.NULL:
             c.log(logL.INFO, 'Authentication success')
+            c.level |= OSI.APPLICATION
         case AcseServiceUser.AUTHENTICATION_FAILURE as diag if is_public:
             c.log(logL.WARN, F'On Public connection type got {diag.name}, broad force turn ON')
         case AcseServiceUser.AUTHENTICATION_REQUIRED:
             c.reply.clear()
             c.getApplicationAssociationRequest()
             await c.read_data_block()
             c.parseApplicationAssociationResponse()
@@ -176,22 +210,25 @@
 class Loop(ExTask):
     task: ExTask
     func: Callable[[Any], bool]
     delay: int
     attempt_amount: int = 0
     """0 is never end loop"""
 
-    async def exchange2(self, c: Client):
+    async def run(self, c: Client):
         attempt = count()
-        while not self.func(await self.task.exchange(c)):
+        while not self.func(await super(Loop, self).run(c)):
             if next(attempt) == self.attempt_amount:
                 return False
             await asyncio.sleep(self.delay)
         return True
 
+    async def exchange2(self, c: Client):
+        return await self.task.exchange(c)
+
 
 class Sequence(ExTask):
     """for exchange task sequence"""
     tasks: list[ExTask]
     __is_exchange: bool
 
     def __init__(self, *tasks: ExTask):
@@ -217,17 +254,17 @@
                 res = e
             ret.append(res)
         return ret
 
 
 class InitType(ExTask):
     """nothing params"""
-    async def exchange(self, c: Client, is_public: bool = False):
-        await c.close()  # close hdlc before init
-        return await super(InitType, self).exchange(c, is_public=True)
+    # async def exchange(self, c: Client, is_public: bool = False):
+    #     await c.close()  # close hdlc before init
+    #     return await super(InitType, self).exchange(c, is_public=True)
 
     async def exchange2(self, c: Client):
         # read LDN
         data = await c.read_attr(collection.AttrDesc.LDN_VALUE)
         ldn = octet_string.LDN(data)
         # find device_id(type for Russia)
         type_value, _ = cdt.get_instance_and_pdu_from_value(await c.read_attr(ut.CosemAttributeDescriptor((1, "0.0.96.1.1.255", 2))))
```

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client.egg-info/PKG-INFO` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-client
-Version: 0.8.4
+Version: 0.8.5
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.8.4/src/DLMS_SPODES_client.egg-info/SOURCES.txt` & `DLMS_SPODES_client-0.8.5/src/DLMS_SPODES_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.4/test/test_Client.py` & `DLMS_SPODES_client-0.8.5/test/test_Client.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,37 +34,61 @@
     def test_Loop(self):
         def foo(res):
             return res == cdt.Long(4)
 
         t_server = TransactionServer(
             clients=[
                 client := Client(
-                    secret="30 30 30 30 30 30 30 30",
+                    secret="30 30 30 30 30 30 30 3030 30 30 30 30 30 30 30",
                     addr_size=-1)
             ],
             tsk=task.Loop(
                 task=task.ReadAttribute(
                     ln="0.0.1.0.0.255",
                     index=3),
-                func=lambda res: res == cdt.Long(4),
+                # func=lambda res: res == cdt.Long(4),
+                func=foo,
                 delay=2,
                 attempt_amount=5
             )
         )
-        client.m_id.set(1)
+        client.m_id.set(2)
+        client.SAP.set(0x30)  # for KPZ
+
         # client.device_address.set(0)
         client.media = AsyncSerial(
             port="COM13",
             inactivity_timeout=3
         )
         t_server.start()
         while not t_server.results.is_complete():
             time.sleep(1)
         print("stop")
 
+    def test_simple_read(self):
+        t_server = TransactionServer(
+            clients=[
+                client := Client(
+                    addr_size=-1)
+            ],
+            tsk=task.ReadAttribute(
+                ln="0.0.1.0.0.255",
+                index=2)
+        )
+        # client.m_id.set(2)
+        # client.SAP.set(0x30)  # for KPZ
+        client.media = AsyncSerial(
+            port="COM13",
+            inactivity_timeout=3
+        )
+        t_server.start()
+        while not t_server.results.is_complete():
+            time.sleep(1)
+        print("stop")
+
     def test_async_network(self):
         client = Client(
             secret="30 30 30 30 30 30 30 30",
             addr_size=1,
             conformance="010000000001111000011101")
         type_ = "4d324d5f31"
         ver = "1.5.7"
@@ -202,25 +226,35 @@
         while not t_server.results.is_complete():
             time.sleep(1)
         a = t_server.results[0]
         print(t_server)
 
     def test_firmware_update(self):
         client = Client(
-            secret="30 30 30 30 30 30 30 30",
+            # secret="30 30 30 30 30 30 30 30",    # for 101, 102, 103, 104 before ver 1.0
+            secret="30 30 30 30 30 30 30 30 30 30 30 30 30 30 30 30",  # for KPZ
             conformance="010000000001111000011101",
             media=AsyncSerial(
                 port="COM13",
                 inactivity_timeout=3))
-        # client.SAP.set(0x30)  # for KPZ
-        # client.m_id.set(2)  # for KPZ
-        client.m_id.set(1)  # for 101, 102, 103, 104 before ver 1.0
-        client.transmit_pdu_size = 128
+        client.SAP.set(0x30)  # for KPZ
+        client.m_id.set(2)  # for KPZ
+        client2 = Client(
+            # secret="30 30 30 30 30 30 30 30",    # for 101, 102, 103, 104 before ver 1.0
+            secret="30 30 30 30 30 30 30 30 30 30 30 30 30 30 30 30",  # for KPZ
+            conformance="010000000001111000011101",
+            media=AsyncSerial(
+                port="COM3",
+                inactivity_timeout=3))
+        client2.SAP.set(0x30)  # for KPZ
+        client2.m_id.set(2)  # for KPZ
+        # client.m_id.set(1)  # for 101, 102, 103, 104 before ver 1.0
+        # client.transmit_pdu_size = 128
         t_server = TransactionServer(
-            clients=[client],
+            clients=[client, client2],
             tsk=task.UpdateFirmware())
         t_server.start()
 
         while not t_server.results.is_complete():
             time.sleep(1)
             print(f"{t_server.results.is_complete()=}")
         a = t_server.results[0]
@@ -243,7 +277,19 @@
                 index=2
             ))
         t_server.start()
 
         while not t_server.results.is_complete():
             time.sleep(1)
         print(f"{t_server.results.is_complete()=}")
+
+    def test_OSI(self):
+        from src.DLMS_SPODES_client.client import OSI
+
+        level = OSI.PHYSICAL | OSI.DATA_LINK
+        print(level)
+        print(OSI.PHYSICAL not in level)
+        level |= OSI.APPLICATION
+        print(level)
+        level -= OSI.APPLICATION
+        print(level)
+
```

