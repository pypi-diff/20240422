# Comparing `tmp/oresat_dxwifi-0.3.3.tar.gz` & `tmp/oresat_dxwifi-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_dxwifi-0.3.3.tar", last modified: Sun Apr 21 23:47:46 2024, max compression
+gzip compressed data, was "oresat_dxwifi-0.3.4.tar", last modified: Mon Apr 22 04:32:00 2024, max compression
```

## Comparing `oresat_dxwifi-0.3.3.tar` & `oresat_dxwifi-0.3.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.469994 oresat_dxwifi-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.457994 oresat_dxwifi-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.457994 oresat_dxwifi-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-21 23:47:46.469994 oresat_dxwifi-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/build-deb.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.457994 oresat_dxwifi-0.3.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   100917 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/docs/images/hgs-browser.png
--rw-r--r--   0 runner    (1001) docker     (127)    90640 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/docs/images/olaf-browser.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/kill-olaf
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat-dxwifi-software-server.service
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat-mon-iface.service
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat-vcan-iface.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/camera/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/camera/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/camera/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/camera/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/camera/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/resources/temperature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/services/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/services/configs/camera_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/services/oresat_live.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/services/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/templates/oresat_live.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.465994 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.469994 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/configs/transmission_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/startmonitor.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)  4381644 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/tx_module.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.469994 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 23:47:46.469994 oresat_dxwifi-0.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/start-vcan
--rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/startmonitor.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.768724 oresat_dxwifi-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.752724 oresat_dxwifi-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.756724 oresat_dxwifi-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-22 04:32:00.768724 oresat_dxwifi-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/build-deb.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.752724 oresat_dxwifi-0.3.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.756724 oresat_dxwifi-0.3.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   100917 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/docs/images/hgs-browser.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90640 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/docs/images/olaf-browser.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/kill-olaf
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat-dxwifi-software-server.service
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat-mon-iface.service
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat-vcan-iface.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.756724 oresat_dxwifi-0.3.4/oresat_dxwifi/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 04:32:00.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.760724 oresat_dxwifi-0.3.4/oresat_dxwifi/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/camera/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/camera/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/camera/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/camera/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.760724 oresat_dxwifi-0.3.4/oresat_dxwifi/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/resources/temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.760724 oresat_dxwifi-0.3.4/oresat_dxwifi/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.760724 oresat_dxwifi-0.3.4/oresat_dxwifi/services/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/services/configs/camera_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/services/oresat_live.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.760724 oresat_dxwifi-0.3.4/oresat_dxwifi/services/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.760724 oresat_dxwifi-0.3.4/oresat_dxwifi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/templates/oresat_live.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.760724 oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.768724 oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/configs/transmission_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/startmonitor.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4381644 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/tx_module.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:00.768724 oresat_dxwifi-0.3.4/oresat_dxwifi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-22 04:32:00.000000 oresat_dxwifi-0.3.4/oresat_dxwifi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-22 04:32:00.000000 oresat_dxwifi-0.3.4/oresat_dxwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 04:32:00.000000 oresat_dxwifi-0.3.4/oresat_dxwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 04:32:00.000000 oresat_dxwifi-0.3.4/oresat_dxwifi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-22 04:32:00.000000 oresat_dxwifi-0.3.4/oresat_dxwifi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-22 04:32:00.000000 oresat_dxwifi-0.3.4/oresat_dxwifi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 04:32:00.768724 oresat_dxwifi-0.3.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/start-vcan
+-rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-04-22 04:31:55.000000 oresat_dxwifi-0.3.4/startmonitor.sh
```

### Comparing `oresat_dxwifi-0.3.3/.github/workflows/pypi.yaml` & `oresat_dxwifi-0.3.4/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/.gitignore` & `oresat_dxwifi-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/LICENSE` & `oresat_dxwifi-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/PKG-INFO` & `oresat_dxwifi-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.3.3
+Version: 0.3.4
 Summary: OreSat DxWiFi OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat_dxwifi-0.3.3/README.md` & `oresat_dxwifi-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/build-deb.sh` & `oresat_dxwifi-0.3.4/build-deb.sh`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/docs/images/hgs-browser.png` & `oresat_dxwifi-0.3.4/docs/images/hgs-browser.png`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/docs/images/olaf-browser.png` & `oresat_dxwifi-0.3.4/docs/images/olaf-browser.png`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/__main__.py` & `oresat_dxwifi-0.3.4/oresat_dxwifi/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/camera/CMakeLists.txt` & `oresat_dxwifi-0.3.4/oresat_dxwifi/camera/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/camera/README.md` & `oresat_dxwifi-0.3.4/oresat_dxwifi/camera/README.md`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/camera/frame.py` & `oresat_dxwifi-0.3.4/oresat_dxwifi/camera/frame.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/camera/interface.py` & `oresat_dxwifi-0.3.4/oresat_dxwifi/camera/interface.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/resources/temperature.py` & `oresat_dxwifi-0.3.4/oresat_dxwifi/resources/temperature.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/services/oresat_live.py` & `oresat_dxwifi-0.3.4/oresat_dxwifi/services/oresat_live.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,19 +45,24 @@
     """Service for capturing and transmitting video"""
 
     def __init__(self):
         """Initializes camera interface and sets state"""
         super().__init__()
         self.state = State.BOOT
 
+        # start mon0
+        subprocess.call(["startmonitor.sh"])
+
         self.firmware_folder = "/lib/firmware/ath9k_htc"
         self.firmware_file = os.path.join(self.firmware_folder, "htc_9271-1.dev.0.fw")
         
-        self.IMAGE_OUPUT_DIRECTORY = "/oresat-live-output/frames"   # Make sure directory exists
-        self.VIDEO_OUTPUT_DIRECTORY = "/oresat-live-output/videos"  # Make sure directory exists
+        self.IMAGE_OUPUT_DIRECTORY = "/oresat-live-output/frames"
+
+        if not os.path.isdir(self.IMAGE_OUPUT_DIRECTORY):
+            os.mkdir(self.IMAGE_OUPUT_DIRECTORY)
 
         configs = self.load_configs()
 
         self.camera = CameraInterface(
             configs["width"],
             configs["height"],
             self.IMAGE_OUPUT_DIRECTORY,
@@ -113,15 +118,15 @@
             logger.info(f"Bit rate is already set to {value}")
             return
         
         subprocess.call(["ln", "-sf", f"{value}.fw", self.firmware_file])
         subprocess.call(["rmmod", "ath9k_htc"])
         subprocess.call(["modprobe", "ath9k-htc"])
         time.sleep(2)
-        subprocess.call(["startmonitor"])
+        subprocess.call(["startmonitor.sh"])
 
     def on_end(self) -> None:
         """Sets status state to OFF"""
         self.state = State.OFF
 
     def capture(self) -> None:
         """Facilitates image capture and the corresponding state changes"""
```

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif` & `oresat_dxwifi-0.3.4/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/templates/oresat_live.html` & `oresat_dxwifi-0.3.4/oresat_dxwifi/templates/oresat_live.html`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/configs/transmission_configs.yaml` & `oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/configs/transmission_configs.yaml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/defaults.py` & `oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/defaults.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/startmonitor.sh` & `oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/startmonitor.sh`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/transmission.py` & `oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/transmission.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/tx_module.so` & `oresat_dxwifi-0.3.4/oresat_dxwifi/transmission/tx_module.so`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/PKG-INFO` & `oresat_dxwifi-0.3.4/oresat_dxwifi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.3.3
+Version: 0.3.4
 Summary: OreSat DxWiFi OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/SOURCES.txt` & `oresat_dxwifi-0.3.4/oresat_dxwifi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/pyproject.toml` & `oresat_dxwifi-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.3/startmonitor.sh` & `oresat_dxwifi-0.3.4/startmonitor.sh`

 * *Files identical despite different names*

