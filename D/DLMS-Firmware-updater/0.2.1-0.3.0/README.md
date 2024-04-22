# Comparing `tmp/DLMS_Firmware_updater-0.2.1.tar.gz` & `tmp/DLMS_Firmware_updater-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_Firmware_updater-0.2.1.tar", last modified: Mon Apr 15 10:30:30 2024, max compression
+gzip compressed data, was "DLMS_Firmware_updater-0.3.0.tar", last modified: Mon Apr 22 08:50:06 2024, max compression
```

## Comparing `DLMS_Firmware_updater-0.2.1.tar` & `DLMS_Firmware_updater-0.3.0.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.710527 DLMS_Firmware_updater-0.2.1/
--rw-rw-rw-   0        0        0      141 2024-04-08 12:09:56.000000 DLMS_Firmware_updater-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      569 2024-04-15 10:30:30.709525 DLMS_Firmware_updater-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-04-05 11:46:13.000000 DLMS_Firmware_updater-0.2.1/README.md
--rw-rw-rw-   0        0        0     1115 2024-04-15 10:27:37.000000 DLMS_Firmware_updater-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 10:30:30.710527 DLMS_Firmware_updater-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0       45 2024-04-08 11:38:51.000000 DLMS_Firmware_updater-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.294226 DLMS_Firmware_updater-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.371525 DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:48:37.000000 DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/__init__.py
--rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/config.toml
--rw-rw-rw-   0        0        0     3612 2024-04-12 13:09:16.000000 DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/main.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.401531 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/
--rw-rw-rw-   0        0        0      569 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5345 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-15 10:30:30.000000 DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.417531 DLMS_Firmware_updater-0.2.1/test/
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.422525 DLMS_Firmware_updater-0.2.1/test/Firmwares/
--rw-rw-rw-   0        0        0  1766884 2024-02-16 08:53:58.000000 DLMS_Firmware_updater-0.2.1/test/Firmwares/firmwares.dat
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.302269 DLMS_Firmware_updater-0.2.1/test/Types/
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.297223 DLMS_Firmware_updater-0.2.1/test/Types/101/
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.489528 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/
--rw-rw-rw-   0        0        0    57842 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.14.typ
--rw-rw-rw-   0        0        0    50536 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.16.typ
--rw-rw-rw-   0        0        0    52759 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.26.typ
--rw-rw-rw-   0        0        0    34300 2023-12-21 03:55:07.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.39.typ
--rw-rw-rw-   0        0        0    52661 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.43.typ
--rw-rw-rw-   0        0        0    58232 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.45.typ
--rw-rw-rw-   0        0        0    57145 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.46.typ
--rw-rw-rw-   0        0        0    75612 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.48.typ
--rw-rw-rw-   0        0        0    34417 2023-12-21 04:16:11.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.49.typ
--rw-rw-rw-   0        0        0   116670 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.53.typ
--rw-rw-rw-   0        0        0    81183 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.54.typ
--rw-rw-rw-   0        0        0     3996 2023-11-27 13:04:23.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.1.0.typ
--rw-rw-rw-   0        0        0   105296 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.2.0.typ
--rw-rw-rw-   0        0        0   104149 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.0.typ
--rw-rw-rw-   0        0        0   110418 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.30.typ
--rw-rw-rw-   0        0        0   109427 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.7.typ
--rw-rw-rw-   0        0        0   113952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.9.typ
--rw-rw-rw-   0        0        0     2940 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.4.0.typ
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.299226 DLMS_Firmware_updater-0.2.1/test/Types/102/
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.530527 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/
--rw-rw-rw-   0        0        0    52751 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.20.typ
--rw-rw-rw-   0        0        0    54303 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.26.typ
--rw-rw-rw-   0        0        0    36789 2023-12-20 11:05:11.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.39.typ
--rw-rw-rw-   0        0        0    54404 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.41.typ
--rw-rw-rw-   0        0        0    54502 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.43.typ
--rw-rw-rw-   0        0        0    60174 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.45.typ
--rw-rw-rw-   0        0        0    78025 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.48.typ
--rw-rw-rw-   0        0        0    37934 2023-12-20 11:30:16.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.49.typ
--rw-rw-rw-   0        0        0   115968 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.53.typ
--rw-rw-rw-   0        0        0     3974 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.1.0.typ
--rw-rw-rw-   0        0        0   114434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.2.0.typ
--rw-rw-rw-   0        0        0   114952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.0.typ
--rw-rw-rw-   0        0        0   133762 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.30.typ
--rw-rw-rw-   0        0        0   116367 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.5.typ
--rw-rw-rw-   0        0        0   128811 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.7.typ
--rw-rw-rw-   0        0        0   136629 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.300277 DLMS_Firmware_updater-0.2.1/test/Types/103/
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.566527 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/
--rw-rw-rw-   0        0        0    50538 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.16.typ
--rw-rw-rw-   0        0        0    52761 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.26.typ
--rw-rw-rw-   0        0        0    34302 2023-12-20 11:53:57.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.39.typ
--rw-rw-rw-   0        0        0    52960 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.43.typ
--rw-rw-rw-   0        0        0    58627 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.45.typ
--rw-rw-rw-   0        0        0    75853 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.48.typ
--rw-rw-rw-   0        0        0    34419 2023-12-21 03:44:07.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.49.typ
--rw-rw-rw-   0        0        0   117000 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.1.0.typ
--rw-rw-rw-   0        0        0   105032 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.2.0.typ
--rw-rw-rw-   0        0        0   104156 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.0.typ
--rw-rw-rw-   0        0        0   110280 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.30.typ
--rw-rw-rw-   0        0        0   109434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.7.typ
--rw-rw-rw-   0        0        0   113959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.301256 DLMS_Firmware_updater-0.2.1/test/Types/104/
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.601526 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/
--rw-rw-rw-   0        0        0    52848 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.20.typ
--rw-rw-rw-   0        0        0    54310 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.26.typ
--rw-rw-rw-   0        0        0    36791 2023-12-20 10:26:34.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.39.typ
--rw-rw-rw-   0        0        0    54724 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.43.typ
--rw-rw-rw-   0        0        0    60391 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.45.typ
--rw-rw-rw-   0        0        0    78146 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.48.typ
--rw-rw-rw-   0        0        0    37935 2023-12-20 10:46:38.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.49.typ
--rw-rw-rw-   0        0        0   118764 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.1.0.typ
--rw-rw-rw-   0        0        0   114441 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.2.0.typ
--rw-rw-rw-   0        0        0   114959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.0.typ
--rw-rw-rw-   0        0        0   133694 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.30.typ
--rw-rw-rw-   0        0        0   128818 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.7.typ
--rw-rw-rw-   0        0        0   136636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.604527 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.626563 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.0.typ
--rw-rw-rw-   0        0        0   147549 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.15.typ
--rw-rw-rw-   0        0        0   146973 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.16.typ
--rw-rw-rw-   0        0        0   146964 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.17.typ
--rw-rw-rw-   0        0        0   145262 2023-10-31 09:20:28.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.0.typ
--rw-rw-rw-   0        0        0    87888 2023-11-16 05:19:14.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.3.typ
--rw-rw-rw-   0        0        0    88315 2023-11-29 12:34:20.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.7.typ
--rw-rw-rw-   0        0        0    88966 2023-12-15 08:12:51.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.6.1.typ
--rw-rw-rw-   0        0        0    89042 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.650537 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.0.typ
--rw-rw-rw-   0        0        0   173570 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.10.typ
--rw-rw-rw-   0        0        0   172860 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.12.typ
--rw-rw-rw-   0        0        0    96832 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.15.typ
--rw-rw-rw-   0        0        0   170726 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.16.typ
--rw-rw-rw-   0        0        0   170785 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.17.typ
--rw-rw-rw-   0        0        0   168739 2023-10-31 11:55:04.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.5.0.typ
--rw-rw-rw-   0        0        0   102599 2023-11-29 12:38:13.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.5.7.typ
--rw-rw-rw-   0        0        0   103542 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.668526 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.0.typ
--rw-rw-rw-   0        0        0   147636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.15.typ
--rw-rw-rw-   0        0        0   147060 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.16.typ
--rw-rw-rw-   0        0        0   147052 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.17.typ
--rw-rw-rw-   0        0        0   145337 2023-10-31 11:55:11.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.5.0.typ
--rw-rw-rw-   0        0        0    88727 2023-11-29 12:38:31.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.5.7.typ
--rw-rw-rw-   0        0        0    89162 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.687526 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.0.typ
--rw-rw-rw-   0        0        0   172819 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.15.typ
--rw-rw-rw-   0        0        0   170738 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.16.typ
--rw-rw-rw-   0        0        0   170642 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.17.typ
--rw-rw-rw-   0        0        0   168751 2023-10-31 12:05:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.5.0.typ
--rw-rw-rw-   0        0        0   102731 2023-11-29 12:38:38.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.5.7.typ
--rw-rw-rw-   0        0        0   103458 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-15 10:30:30.707527 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.0.typ
--rw-rw-rw-   0        0        0   171345 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.12.typ
--rw-rw-rw-   0        0        0   172600 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.15.typ
--rw-rw-rw-   0        0        0   170800 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.16.typ
--rw-rw-rw-   0        0        0   170867 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.17.typ
--rw-rw-rw-   0        0        0   168765 2023-10-31 14:32:35.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.5.0.typ
--rw-rw-rw-   0        0        0   102803 2023-11-29 12:38:49.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.5.7.typ
--rw-rw-rw-   0        0        0   103828 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.6.2.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.1/test/Types/KPZ/image_transfer_1.typ
--rw-rw-rw-   0        0        0   762665 2024-04-12 13:31:06.000000 DLMS_Firmware_updater-0.2.1/test/client_log.txt
--rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.2.1/test/config.toml
--rw-rw-rw-   0        0        0      387 2024-04-12 13:11:37.000000 DLMS_Firmware_updater-0.2.1/test/test_updater.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.935197 DLMS_Firmware_updater-0.3.0/
+-rw-rw-rw-   0        0        0      141 2024-04-08 12:09:56.000000 DLMS_Firmware_updater-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      569 2024-04-22 08:50:06.934201 DLMS_Firmware_updater-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-04-05 11:46:13.000000 DLMS_Firmware_updater-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1115 2024-04-22 08:41:15.000000 DLMS_Firmware_updater-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-22 08:50:06.935197 DLMS_Firmware_updater-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       45 2024-04-08 11:38:51.000000 DLMS_Firmware_updater-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.558198 DLMS_Firmware_updater-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.579199 DLMS_Firmware_updater-0.3.0/src/DLMSFirmwareUpdater/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:48:37.000000 DLMS_Firmware_updater-0.3.0/src/DLMSFirmwareUpdater/__init__.py
+-rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.3.0/src/DLMSFirmwareUpdater/config.toml
+-rw-rw-rw-   0        0        0     3764 2024-04-22 08:48:53.000000 DLMS_Firmware_updater-0.3.0/src/DLMSFirmwareUpdater/main.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.592202 DLMS_Firmware_updater-0.3.0/src/DLMS_Firmware_updater.egg-info/
+-rw-rw-rw-   0        0        0      569 2024-04-22 08:50:06.000000 DLMS_Firmware_updater-0.3.0/src/DLMS_Firmware_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5345 2024-04-22 08:50:06.000000 DLMS_Firmware_updater-0.3.0/src/DLMS_Firmware_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 08:50:06.000000 DLMS_Firmware_updater-0.3.0/src/DLMS_Firmware_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-22 08:50:06.000000 DLMS_Firmware_updater-0.3.0/src/DLMS_Firmware_updater.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2024-04-22 08:50:06.000000 DLMS_Firmware_updater-0.3.0/src/DLMS_Firmware_updater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-22 08:50:06.000000 DLMS_Firmware_updater-0.3.0/src/DLMS_Firmware_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.599198 DLMS_Firmware_updater-0.3.0/test/
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.602201 DLMS_Firmware_updater-0.3.0/test/Firmwares/
+-rw-rw-rw-   0        0        0  1766884 2024-02-16 08:53:58.000000 DLMS_Firmware_updater-0.3.0/test/Firmwares/firmwares.dat
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.564200 DLMS_Firmware_updater-0.3.0/test/Types/
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.561205 DLMS_Firmware_updater-0.3.0/test/Types/101/
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.662197 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/
+-rw-rw-rw-   0        0        0    57842 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.14.typ
+-rw-rw-rw-   0        0        0    50536 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.16.typ
+-rw-rw-rw-   0        0        0    52759 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.26.typ
+-rw-rw-rw-   0        0        0    34300 2023-12-21 03:55:07.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.39.typ
+-rw-rw-rw-   0        0        0    52661 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.43.typ
+-rw-rw-rw-   0        0        0    58232 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.45.typ
+-rw-rw-rw-   0        0        0    57145 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.46.typ
+-rw-rw-rw-   0        0        0    75612 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.48.typ
+-rw-rw-rw-   0        0        0    34417 2023-12-21 04:16:11.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.49.typ
+-rw-rw-rw-   0        0        0   116670 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.53.typ
+-rw-rw-rw-   0        0        0    81183 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.54.typ
+-rw-rw-rw-   0        0        0     3996 2023-11-27 13:04:23.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.1.0.typ
+-rw-rw-rw-   0        0        0   105296 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.2.0.typ
+-rw-rw-rw-   0        0        0   104149 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.3.0.typ
+-rw-rw-rw-   0        0        0   110418 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.3.30.typ
+-rw-rw-rw-   0        0        0   109427 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.3.7.typ
+-rw-rw-rw-   0        0        0   113952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.3.9.typ
+-rw-rw-rw-   0        0        0     2940 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.4.0.typ
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.562202 DLMS_Firmware_updater-0.3.0/test/Types/102/
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.713198 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/
+-rw-rw-rw-   0        0        0    52751 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.20.typ
+-rw-rw-rw-   0        0        0    54303 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.26.typ
+-rw-rw-rw-   0        0        0    36789 2023-12-20 11:05:11.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.39.typ
+-rw-rw-rw-   0        0        0    54404 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.41.typ
+-rw-rw-rw-   0        0        0    54502 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.43.typ
+-rw-rw-rw-   0        0        0    60174 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.45.typ
+-rw-rw-rw-   0        0        0    78025 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.48.typ
+-rw-rw-rw-   0        0        0    37934 2023-12-20 11:30:16.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.49.typ
+-rw-rw-rw-   0        0        0   115968 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.53.typ
+-rw-rw-rw-   0        0        0     3974 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.1.0.typ
+-rw-rw-rw-   0        0        0   114434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.2.0.typ
+-rw-rw-rw-   0        0        0   114952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.3.0.typ
+-rw-rw-rw-   0        0        0   133762 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.3.30.typ
+-rw-rw-rw-   0        0        0   116367 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.3.5.typ
+-rw-rw-rw-   0        0        0   128811 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.3.7.typ
+-rw-rw-rw-   0        0        0   136629 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.563199 DLMS_Firmware_updater-0.3.0/test/Types/103/
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.755198 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/
+-rw-rw-rw-   0        0        0    50538 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.16.typ
+-rw-rw-rw-   0        0        0    52761 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.26.typ
+-rw-rw-rw-   0        0        0    34302 2023-12-20 11:53:57.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.39.typ
+-rw-rw-rw-   0        0        0    52960 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.43.typ
+-rw-rw-rw-   0        0        0    58627 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.45.typ
+-rw-rw-rw-   0        0        0    75853 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.48.typ
+-rw-rw-rw-   0        0        0    34419 2023-12-21 03:44:07.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.49.typ
+-rw-rw-rw-   0        0        0   117000 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.53.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.1.0.typ
+-rw-rw-rw-   0        0        0   105032 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.2.0.typ
+-rw-rw-rw-   0        0        0   104156 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.3.0.typ
+-rw-rw-rw-   0        0        0   110280 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.3.30.typ
+-rw-rw-rw-   0        0        0   109434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.3.7.typ
+-rw-rw-rw-   0        0        0   113959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.564200 DLMS_Firmware_updater-0.3.0/test/Types/104/
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.797198 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/
+-rw-rw-rw-   0        0        0    52848 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.20.typ
+-rw-rw-rw-   0        0        0    54310 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.26.typ
+-rw-rw-rw-   0        0        0    36791 2023-12-20 10:26:34.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.39.typ
+-rw-rw-rw-   0        0        0    54724 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.43.typ
+-rw-rw-rw-   0        0        0    60391 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.45.typ
+-rw-rw-rw-   0        0        0    78146 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.48.typ
+-rw-rw-rw-   0        0        0    37935 2023-12-20 10:46:38.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.49.typ
+-rw-rw-rw-   0        0        0   118764 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.53.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.1.0.typ
+-rw-rw-rw-   0        0        0   114441 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.2.0.typ
+-rw-rw-rw-   0        0        0   114959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.3.0.typ
+-rw-rw-rw-   0        0        0   133694 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.3.30.typ
+-rw-rw-rw-   0        0        0   128818 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.3.7.typ
+-rw-rw-rw-   0        0        0   136636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.800197 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.830199 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/
+-rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.4.0.typ
+-rw-rw-rw-   0        0        0   147549 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.4.15.typ
+-rw-rw-rw-   0        0        0   146973 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.4.16.typ
+-rw-rw-rw-   0        0        0   146964 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.4.17.typ
+-rw-rw-rw-   0        0        0   145262 2023-10-31 09:20:28.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.5.0.typ
+-rw-rw-rw-   0        0        0    87888 2023-11-16 05:19:14.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.5.3.typ
+-rw-rw-rw-   0        0        0    88315 2023-11-29 12:34:20.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.5.7.typ
+-rw-rw-rw-   0        0        0    88966 2023-12-15 08:12:51.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.6.1.typ
+-rw-rw-rw-   0        0        0    89042 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.856200 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.0.typ
+-rw-rw-rw-   0        0        0   173570 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.10.typ
+-rw-rw-rw-   0        0        0   172860 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.12.typ
+-rw-rw-rw-   0        0        0    96832 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.15.typ
+-rw-rw-rw-   0        0        0   170726 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.16.typ
+-rw-rw-rw-   0        0        0   170785 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.17.typ
+-rw-rw-rw-   0        0        0   168739 2023-10-31 11:55:04.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.5.0.typ
+-rw-rw-rw-   0        0        0   102599 2023-11-29 12:38:13.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.5.7.typ
+-rw-rw-rw-   0        0        0   103542 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.878198 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.4.0.typ
+-rw-rw-rw-   0        0        0   147636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.4.15.typ
+-rw-rw-rw-   0        0        0   147060 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.4.16.typ
+-rw-rw-rw-   0        0        0   147052 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.4.17.typ
+-rw-rw-rw-   0        0        0   145337 2023-10-31 11:55:11.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.5.0.typ
+-rw-rw-rw-   0        0        0    88727 2023-11-29 12:38:31.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.5.7.typ
+-rw-rw-rw-   0        0        0    89162 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.901198 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.4.0.typ
+-rw-rw-rw-   0        0        0   172819 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.4.15.typ
+-rw-rw-rw-   0        0        0   170738 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.4.16.typ
+-rw-rw-rw-   0        0        0   170642 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.4.17.typ
+-rw-rw-rw-   0        0        0   168751 2023-10-31 12:05:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.5.0.typ
+-rw-rw-rw-   0        0        0   102731 2023-11-29 12:38:38.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.5.7.typ
+-rw-rw-rw-   0        0        0   103458 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-22 08:50:06.931196 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.0.typ
+-rw-rw-rw-   0        0        0   171345 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.12.typ
+-rw-rw-rw-   0        0        0   172600 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.15.typ
+-rw-rw-rw-   0        0        0   170800 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.16.typ
+-rw-rw-rw-   0        0        0   170867 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.17.typ
+-rw-rw-rw-   0        0        0   168765 2023-10-31 14:32:35.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.5.0.typ
+-rw-rw-rw-   0        0        0   102803 2023-11-29 12:38:49.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.5.7.typ
+-rw-rw-rw-   0        0        0   103828 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.6.2.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.3.0/test/Types/KPZ/image_transfer_1.typ
+-rw-rw-rw-   0        0        0   775359 2024-04-22 08:44:09.000000 DLMS_Firmware_updater-0.3.0/test/client_log.txt
+-rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.3.0/test/config.toml
+-rw-rw-rw-   0        0        0      387 2024-04-12 13:11:37.000000 DLMS_Firmware_updater-0.3.0/test/test_updater.py
```

### Comparing `DLMS_Firmware_updater-0.2.1/PKG-INFO` & `DLMS_Firmware_updater-0.3.0/src/DLMS_Firmware_updater.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: DLMS_Firmware_updater
-Version: 0.2.1
+Name: DLMS-Firmware-updater
+Version: 0.3.0
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSFirmwareUpdater_project
 Keywords: dlms,spodes,client,firmware,update
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_Firmware_updater-0.2.1/pyproject.toml` & `DLMS_Firmware_updater-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 [tool.setuptools.package-data]
 DLMSFirmwareUpdater = ["*.toml", "*.dat", "*.typ"]
 #exclude = ["test*", "dummy"]  # alternatively: `exclude = ["additional*"]`
 #namespaces = false
 
 [project]
 name = "DLMS_Firmware_updater"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
-    "DLMS_SPODES_client == 0.7.8",
+    "DLMS_SPODES_client == 0.8.6",
     "pyinstaller >= 6.2",
     "build >= 1.2.1"
 ]
 description="dlms-spodes"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords=["dlms", "spodes", "client", "firmware", "update"]
```

### Comparing `DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/config.toml` & `DLMS_Firmware_updater-0.3.0/src/DLMSFirmwareUpdater/config.toml`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/src/DLMSFirmwareUpdater/main.py` & `DLMS_Firmware_updater-0.3.0/src/DLMSFirmwareUpdater/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import argparse
 import time
 
 from DLMS_SPODES_client.servers import TransactionServer, Result
 from DLMS_SPODES_client import task, services
-from DLMS_SPODES_client.client import Client, logL
+from DLMS_SPODES_client.client import Client, logL, IDFactory
 from DLMS_SPODES_communications import AsyncSerial, AsyncNetwork
 
 
+id_factory = IDFactory("#")
+
+
 def main():
     parser = argparse.ArgumentParser(
         description="Update Firmware Program for DLMS meters")
     parser.add_argument(
         '-t', '--type',
         choices=("File", "Serial", "Net"),
         required=True,
@@ -69,23 +72,26 @@
         help="output result file"
     )
     args = parser.parse_args()
     if (source := args.type) in ("Serial", "Net"):
         clients = [c := Client(
                         SAP=args.sap,
                         secret=args.secret.hex(),
-                        addr_size=-1)]
+                        addr_size=-1,
+                        id_=id_factory.create())]
         c.m_id.set(args.mechanism_id)
         c.device_address.set(args.da)
         c_t = AsyncSerial if source == "Serial" else AsyncNetwork
         c.media = c_t(*args.p)
         c.media.inactivity_timeout = args.timeout
     elif source == "File":
         if len(args.p) == 1:
-            clients = services.get_client_from_csv(file_name=args.p[0])
+            clients = services.get_client_from_csv(
+                file_name=args.p[0],
+                id_factory=id_factory)
         else:
             raise ValueError("-p for \"File\" must have 1 file name")
     else:
          raise ValueError(F"unknown {source=}")
     t_server = TransactionServer(
         clients=clients,
         tsk=task.Loop(
```

### Comparing `DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/PKG-INFO` & `DLMS_Firmware_updater-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: DLMS-Firmware-updater
-Version: 0.2.1
+Name: DLMS_Firmware_updater
+Version: 0.3.0
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSFirmwareUpdater_project
 Keywords: dlms,spodes,client,firmware,update
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_Firmware_updater-0.2.1/src/DLMS_Firmware_updater.egg-info/SOURCES.txt` & `DLMS_Firmware_updater-0.3.0/src/DLMS_Firmware_updater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Firmwares/firmwares.dat` & `DLMS_Firmware_updater-0.3.0/test/Firmwares/firmwares.dat`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.14.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.14.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.16.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.26.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.39.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.43.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.45.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.46.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.46.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.48.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.49.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.53.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/0.0.54.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/0.0.54.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.1.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.1.9.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.2.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.2.5.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.30.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.7.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.3.9.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/101/09054d324d5f31/1.4.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/101/09054d324d5f31/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.20.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.20.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.26.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.39.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.41.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.41.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.43.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.45.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.48.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.49.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/0.0.53.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.1.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.1.9.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.2.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.2.5.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.30.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.5.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.3.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.7.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/102/09054d324d5f33/1.3.9.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/102/09054d324d5f33/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.16.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.26.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.39.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.43.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.45.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.48.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.49.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/0.0.53.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.1.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.1.9.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.2.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.2.5.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.30.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.7.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/103/09064d324d5f3153/1.3.9.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/103/09064d324d5f3153/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.20.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.20.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.26.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.39.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.43.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.45.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.48.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.49.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/0.0.53.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.1.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.1.9.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.2.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.2.5.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.30.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.7.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/104/09064d324d5f3353/1.3.9.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/104/09064d324d5f3353/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.15.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.16.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.17.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.4.22.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.3.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.5.3.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.5.7.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.6.1.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.6.1.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f31/1.6.2.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f31/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.10.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.10.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.12.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.12.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.15.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.16.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.17.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.4.22.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.5.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.5.7.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09054d324d5f33/1.6.2.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09054d324d5f33/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.15.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.16.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.17.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.4.22.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.5.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.5.7.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3153/1.6.2.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3153/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.15.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.16.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.17.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.4.22.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.5.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.5.7.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3353/1.6.2.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3353/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.12.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.12.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.15.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.16.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.17.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.4.22.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.5.0.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.5.7.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/09064d324d5f3354/1.6.2.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/09064d324d5f3354/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/Types/KPZ/image_transfer_1.typ` & `DLMS_Firmware_updater-0.3.0/test/Types/KPZ/image_transfer_1.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.2.1/test/client_log.txt` & `DLMS_Firmware_updater-0.3.0/test/client_log.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1077,7 +1077,92 @@
 KPZ101000017410: 12.04 16:31 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S6_R7_PF DA:48 SA:1/16  Info[9]:e6 e7 00 c4 01 c1 00 16 05
 KPZ101000017410: 12.04 16:31 - DLMSClient.DLMS_SPODES_client.logger - INFO - obj.image_transfer_status=ImageTransferStatus(Активация данных инициированна)
 KPZ101000017410: 12.04 16:31 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: DISC_P DA:1/16 SA:48 
 KPZ101000017410: 12.04 16:31 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:48 SA:1/16  Info[22]:81 80 13 05 01 ef 06 02 04 00 07 04 00 00 00 01 08 04 00 00 00 01
 KPZ101000017410: 12.04 16:31 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - DisconnectRequest
 KPZ101000017410: 12.04 16:31 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Close communication channel: AsyncSerial(port='COM13', inactivity_timeout=1)
 KPZ101000017410: 12.04 16:31 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Close media: AsyncSerial(port='COM13', inactivity_timeout=1)
+#common: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - Open port communication channel: AsyncSerial(port='COM13', inactivity_timeout=1)
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - c.SA=Address(upper_address=16, lower_address=None) c.DA=Address(upper_address=1, lower_address=16)
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: SNRM_P DA:1/16 SA:16  Info[11]:81 80 08 05 02 07 ee 06 02 07 ee
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:16 SA:1/16  Info[22]:81 80 13 05 01 ef 06 02 04 00 07 04 00 00 00 01 08 04 00 00 00 01
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - negotiation setup: NEGOTIATION: 1024->[info_size]->239 1->[window]->1
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S0_R0_PF DA:1/16 SA:16  Info[34]:e6 e6 00 60 1d a1 09 06 07 60 85 74 05 08 01 01 be 10 04 0e 01 00 00 00 06 5f 1f 04 00 7f ff ff 04 00
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S0_R1_PF DA:16 SA:1/16  Info[46]:e6 e7 00 61 29 a1 09 06 07 60 85 74 05 08 01 01 a2 03 02 01 00 a3 05 a1 03 02 01 00 be 10 04 0e 08 00 06 5f 1f 04 00 00 10 10 04 00 00 07
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - SET CONFORMANCE: 000000000001000000010000
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - Authentication success
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S1_R1_PF DA:1/16 SA:16  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 2a 00 00 ff 02 00
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S1_R2_PF DA:16 SA:1/16  Info[21]:e6 e7 00 c4 01 c1 00 09 0c 31 30 31 30 30 30 30 31 37 34 31 30
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S2_R2_PF DA:1/16 SA:16  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 60 01 01 ff 02 00
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S2_R3_PF DA:16 SA:1/16  Info[14]:e6 e7 00 c4 01 c1 00 09 05 4d 32 4d 5f 31
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S3_R3_PF DA:1/16 SA:16  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 00 02 01 ff 02 00
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S3_R4_PF DA:16 SA:1/16  Info[8]:e6 e7 00 c4 01 c1 01 04
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S4_R4_PF DA:1/16 SA:16  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 60 01 02 ff 02 00
+None: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S4_R5_PF DA:16 SA:1/16  Info[15]:e6 e7 00 c4 01 c1 00 09 06 31 2e 33 2e 33 30
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - added 197 DLMS objects
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - close
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: DISC_P DA:1/16 SA:16 
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:16 SA:1/16  Info[22]:81 80 13 05 01 ef 06 02 04 00 07 04 00 00 00 01 08 04 00 00 00 01
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - c.SA=Address(upper_address=48, lower_address=None) c.DA=Address(upper_address=1, lower_address=16)
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: SNRM_P DA:1/16 SA:48  Info[10]:81 80 07 05 02 04 00 06 01 ef
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:48 SA:1/16  Info[22]:81 80 13 05 01 ef 06 02 04 00 07 04 00 00 00 01 08 04 00 00 00 01
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - negotiation setup: NEGOTIATION: 1024->[info_size]->239 1->[window]->1
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S0_R0_PF DA:1/16 SA:48  Info[67]:e6 e6 00 60 3e a1 09 06 07 60 85 74 05 08 01 01 8a 02 07 80 8b 07 60 85 74 05 08 02 02 ac 12 80 10 00 ad 46 a3 7c cd 50 aa ea 13 5a 9f 51 4f 7d ce be 10 04 0e 01 00 00 00 06 5f 1f 04 00 7f ff ff 04 00
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S0_R1_PF DA:48 SA:1/16  Info[79]:e6 e7 00 61 4a a1 09 06 07 60 85 74 05 08 01 01 a2 03 02 01 00 a3 05 a1 03 02 01 0e 88 02 07 80 89 07 60 85 74 05 08 02 02 aa 12 80 10 06 58 d7 f9 16 0f 12 33 7c ae 1e 95 b7 97 bf 9c be 10 04 0e 08 00 06 5f 1f 04 00 00 18 9d 04 00 00 07
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - SET CONFORMANCE: 000000000001100010011101
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S1_R1_PF DA:1/16 SA:48  Info[34]:e6 e6 00 c3 01 c1 00 0f 00 00 28 00 03 ff 01 01 09 10 e7 c9 b3 63 fc 14 1b 1e 5b c9 2c 4d 43 06 c0 bc
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S1_R2_PF DA:48 SA:1/16  Info[27]:e6 e7 00 c7 01 c1 00 01 00 09 10 fd ca 8b 15 9c 83 df cf ea 99 d2 33 b6 ce 10 45
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S2_R2_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 2a 00 00 ff 02 00
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S2_R3_PF DA:48 SA:1/16  Info[21]:e6 e7 00 c4 01 c1 00 09 0c 31 30 31 30 30 30 30 31 37 34 31 30
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S3_R3_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 80 64 00 ff 02 00
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S3_R4_PF DA:48 SA:1/16  Info[27]:e6 e7 00 c4 01 c1 00 0a 12 30 30 30 38 50 57 52 4d 5f 4d 32 4d 5f 31 5f 46 34 5f
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S4_R4_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 60 01 02 ff 02 00
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S4_R5_PF DA:48 SA:1/16  Info[15]:e6 e7 00 c4 01 c1 00 09 06 31 2e 33 2e 33 30
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S5_R5_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 00 ff 02 00
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S5_R6_PF DA:48 SA:1/16  Info[12]:e6 e7 00 c4 01 c1 00 06 00 00 02 00
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S6_R6_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 00 ff 06 00
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S6_R7_PF DA:48 SA:1/16  Info[9]:e6 e7 00 c4 01 c1 00 16 01
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S7_R7_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 80 ff 02 00
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S7_R0_PF DA:48 SA:1/16  Info[12]:e6 e7 00 c4 01 c1 00 06 00 00 02 00
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - c.objects.server_ver[0]=AppVersion(1, 3, 30) is actual
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - boot_version=8 is actual
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S0_R0_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 80 64 00 ff 02 00
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S0_R1_PF DA:48 SA:1/16  Info[27]:e6 e7 00 c4 01 c1 00 0a 12 30 30 30 38 50 57 52 4d 5f 4d 32 4d 5f 31 5f 46 34 5f
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - close
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: DISC_P DA:1/16 SA:48 
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:48 SA:1/16  Info[22]:81 80 13 05 01 ef 06 02 04 00 07 04 00 00 00 01 08 04 00 00 00 01
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Close communication channel: AsyncSerial(port='COM13', inactivity_timeout=1)
+101000017410: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для 101000017410 обновление: Удачно
+#common: 22.04 11:11 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#common: 22.04 11:12 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+None: 22.04 11:13 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для None обновление: Неудачно
+None: 22.04 11:13 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+None: 22.04 11:13 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+None: 22.04 11:13 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+None: 22.04 11:13 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+None: 22.04 11:14 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+None: 22.04 11:14 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+None: 22.04 11:14 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+None: 22.04 11:14 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+None: 22.04 11:14 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для None обновление: Неудачно
+None: 22.04 11:14 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для None обновление: Неудачно
+#common: 22.04 11:26 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+None: 22.04 11:27 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для None обновление: Неудачно
+None: 22.04 11:27 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+None: 22.04 11:27 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+#common: 22.04 11:41 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+None: 22.04 11:42 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для None обновление: Неудачно
+None: 22.04 11:42 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+None: 22.04 11:42 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+#common: 22.04 11:42 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#0: 22.04 11:42 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для #0 обновление: Неудачно
+#2: 22.04 11:42 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+#1: 22.04 11:42 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+#2: 22.04 11:43 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+#1: 22.04 11:43 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+#2: 22.04 11:43 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+#1: 22.04 11:43 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+#2: 22.04 11:44 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+#1: 22.04 11:44 - DLMSClient.DLMS_SPODES_client.logger - INFO - UNKNOWN ERROR: [WinError 121] Превышен таймаут семафора...
+#1: 22.04 11:44 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для #1 обновление: Неудачно
+#2: 22.04 11:44 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для #2 обновление: Неудачно
```

### Comparing `DLMS_Firmware_updater-0.2.1/test/config.toml` & `DLMS_Firmware_updater-0.3.0/test/config.toml`

 * *Files identical despite different names*

