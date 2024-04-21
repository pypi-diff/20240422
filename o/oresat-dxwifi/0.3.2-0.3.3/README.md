# Comparing `tmp/oresat_dxwifi-0.3.2.tar.gz` & `tmp/oresat_dxwifi-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_dxwifi-0.3.2.tar", last modified: Fri Apr 19 02:47:38 2024, max compression
+gzip compressed data, was "oresat_dxwifi-0.3.3.tar", last modified: Sun Apr 21 23:47:46 2024, max compression
```

## Comparing `oresat_dxwifi-0.3.2.tar` & `oresat_dxwifi-0.3.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.861395 oresat_dxwifi-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.845395 oresat_dxwifi-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.849395 oresat_dxwifi-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-19 02:47:38.861395 oresat_dxwifi-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/build-deb.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.845395 oresat_dxwifi-0.3.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.849395 oresat_dxwifi-0.3.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   100917 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/docs/images/hgs-browser.png
--rw-r--r--   0 runner    (1001) docker     (127)    90640 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/docs/images/olaf-browser.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/kill-olaf
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat-dxwifi-software-server.service
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat-mon-iface.service
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat-vcan-iface.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.849395 oresat_dxwifi-0.3.2/oresat_dxwifi/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 02:47:38.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.853395 oresat_dxwifi-0.3.2/oresat_dxwifi/camera/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/camera/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/camera/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/camera/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/camera/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.853395 oresat_dxwifi-0.3.2/oresat_dxwifi/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/resources/temperature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.853395 oresat_dxwifi-0.3.2/oresat_dxwifi/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.853395 oresat_dxwifi-0.3.2/oresat_dxwifi/services/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/services/configs/camera_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/services/oresat_live.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.853395 oresat_dxwifi-0.3.2/oresat_dxwifi/services/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.853395 oresat_dxwifi-0.3.2/oresat_dxwifi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/templates/oresat_live.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.853395 oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.857396 oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/configs/transmission_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/startmonitor.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)  4381644 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/tx_module.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:38.861395 oresat_dxwifi-0.3.2/oresat_dxwifi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-19 02:47:38.000000 oresat_dxwifi-0.3.2/oresat_dxwifi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-19 02:47:38.000000 oresat_dxwifi-0.3.2/oresat_dxwifi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:47:38.000000 oresat_dxwifi-0.3.2/oresat_dxwifi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 02:47:38.000000 oresat_dxwifi-0.3.2/oresat_dxwifi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 02:47:38.000000 oresat_dxwifi-0.3.2/oresat_dxwifi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-19 02:47:38.000000 oresat_dxwifi-0.3.2/oresat_dxwifi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 02:47:38.861395 oresat_dxwifi-0.3.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/start-vcan
--rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-04-19 02:47:30.000000 oresat_dxwifi-0.3.2/startmonitor.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.469994 oresat_dxwifi-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.457994 oresat_dxwifi-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.457994 oresat_dxwifi-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-21 23:47:46.469994 oresat_dxwifi-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/build-deb.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.457994 oresat_dxwifi-0.3.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   100917 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/docs/images/hgs-browser.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90640 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/docs/images/olaf-browser.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/kill-olaf
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat-dxwifi-software-server.service
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat-mon-iface.service
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat-vcan-iface.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/camera/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/camera/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/camera/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/camera/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/resources/temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/services/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/services/configs/camera_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/services/oresat_live.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/services/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.461994 oresat_dxwifi-0.3.3/oresat_dxwifi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/templates/oresat_live.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.465994 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.469994 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/configs/transmission_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/startmonitor.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4381644 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/tx_module.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:47:46.469994 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-21 23:47:46.000000 oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 23:47:46.469994 oresat_dxwifi-0.3.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/start-vcan
+-rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-04-21 23:47:41.000000 oresat_dxwifi-0.3.3/startmonitor.sh
```

### Comparing `oresat_dxwifi-0.3.2/.github/workflows/pypi.yaml` & `oresat_dxwifi-0.3.3/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/.gitignore` & `oresat_dxwifi-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/LICENSE` & `oresat_dxwifi-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/PKG-INFO` & `oresat_dxwifi-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.3.2
+Version: 0.3.3
 Summary: OreSat DxWiFi OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat_dxwifi-0.3.2/README.md` & `oresat_dxwifi-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/build-deb.sh` & `oresat_dxwifi-0.3.3/build-deb.sh`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/docs/images/hgs-browser.png` & `oresat_dxwifi-0.3.3/docs/images/hgs-browser.png`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/docs/images/olaf-browser.png` & `oresat_dxwifi-0.3.3/docs/images/olaf-browser.png`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/__main__.py` & `oresat_dxwifi-0.3.3/oresat_dxwifi/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def oresat_live_template():
     return render_olaf_template('oresat_live.html', name='Oresat Live')
 
 
 def main():
     """DxWiFi OLAF app main"""
 
-    args, _ = olaf_setup(NodeId.DXWIFI)
+    args, _ = olaf_setup("dxwifi")
     mock_args = [i.lower() for i in args.mock_hw]
     mock_radio = "radio" in mock_args or "all" in mock_args
 
     app.od["versions"]["sw_version"].value = __version__
 
     app.add_resource(TemperatureResource(is_mock_adc=mock_radio))
```

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/camera/CMakeLists.txt` & `oresat_dxwifi-0.3.3/oresat_dxwifi/camera/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/camera/README.md` & `oresat_dxwifi-0.3.3/oresat_dxwifi/camera/README.md`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/camera/frame.py` & `oresat_dxwifi-0.3.3/oresat_dxwifi/camera/frame.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/camera/interface.py` & `oresat_dxwifi-0.3.3/oresat_dxwifi/camera/interface.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/resources/temperature.py` & `oresat_dxwifi-0.3.3/oresat_dxwifi/resources/temperature.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/services/oresat_live.py` & `oresat_dxwifi-0.3.3/oresat_dxwifi/services/oresat_live.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 class State(IntEnum):
     OFF = 0
     BOOT = 1
     STANDBY = 2
     FILMING = 3
     TRANSMISSION = 4
+    PURGE = 5
     ERROR = 0xFF
 
 
 # OFF: OreSat Live is off (informational only)
 # BOOT: OreSat Live is starting (informational only)
 # STANDBY: Ready to film or transmit on request
 # FILMING: Capturing and encoding video
@@ -28,17 +29,18 @@
 #
 # @TODO Make more complete use of OFF, BOOT, and ERROR? For example, these may
 #       become useful if the camera system is converted to use only Python
 #       (e.g., v4l2py library) or if more libdxwifi bindings are used.
 STATE_TRANSITIONS = {
     State.OFF: [State.BOOT],
     State.BOOT: [State.STANDBY],
-    State.STANDBY: [State.FILMING, State.TRANSMISSION],
+    State.STANDBY: [State.FILMING, State.TRANSMISSION, State.PURGE],
     State.FILMING: [State.STANDBY, State.ERROR],
     State.TRANSMISSION: [State.STANDBY, State.ERROR],
+    State.PURGE: [State.STANDBY],
     State.ERROR: [State.STANDBY],
 }
 
 
 class OresatLiveService(Service):
     """Service for capturing and transmitting video"""
 
@@ -91,18 +93,20 @@
             "transmission",
             subindex="bit_rate",
             read_cb=self.get_bit_rate,
             write_cb=self.update_bit_rate
         )
 
     def get_bit_rate(self):
+        """returns the given bit rate of the transmission"""
         fw_file = subprocess.check_output(["readlink", self.firmware_file]).decode('ascii')
         return int(fw_file.split(".")[0])
     
     def update_bit_rate(self, value: int):
+        """Update the bit rate (by way of firmware blobs) of the transmission"""
         valid_rates = [1, 2, 5, 11, 12, 18, 36, 48, 54]
 
         if value not in valid_rates:
             logger.warn(f"Bit rate of {value} is not valid. Valid Values: {valid_rates}")
             return
 
         if self.get_bit_rate() == value:
@@ -116,57 +120,69 @@
         subprocess.call(["startmonitor"])
 
     def on_end(self) -> None:
         """Sets status state to OFF"""
         self.state = State.OFF
 
     def capture(self) -> None:
-        """Facilitates video capture and the corresponding state changes"""
+        """Facilitates image capture and the corresponding state changes"""
         self.state = State.FILMING
 
         try:
             self.camera.create_images(self.node.od["capture"], self.node.od["transmission"]["as_tar"].value)
             self.state = State.STANDBY
         except Exception as error:
             self.state = State.ERROR
             logger.error("Something went wrong with camera capture...")
             logger.error(error)
 
     def transmit_file(self, filestr) -> None:
+        """Transmit file at given path string"""
         try:
             tx = Transmitter(filestr, self.node.od["transmission"]["enable_pa"].value)
             logger.info(f'Transmitting {filestr}...')
             p = Process(target=tx.transmit)
             p.start()
             p.join()
         except Exception as e:
             logger.error(f"Unable to transmit {filestr} due to {e}")
             self.state = State.ERROR
 
         self.node.od["transmission"]["images_transmitted"].value += 1
 
     def transmit_file_test(self) -> None:
-        """Transmits all the videos in the video output directory."""
+        """Transmits the static color bars image"""
         self.state = State.TRANSMISSION
         cur_dir = os.path.dirname(os.path.realpath(__file__))
         self.transmit_file(os.path.join(cur_dir, "static/SMPTE_Color_Bars.gif"))
         self.state = State.STANDBY
 
     def transmit(self) -> None:
-        """Transmits all the videos in the video output directory."""
+        """Transmits all the images in the image output directory."""
         self.state = State.TRANSMISSION
 
         files = os.listdir(self.IMAGE_OUPUT_DIRECTORY)
 
         for f in files:
             f = os.path.join(self.IMAGE_OUPUT_DIRECTORY, f)
             self.transmit_file(f)
 
         self.state = State.STANDBY
 
+    def purge(self) -> None:
+        """Deletes all the files in the image directory"""
+        self.state = State.PURGE
+
+        files = os.listdir(self.IMAGE_OUPUT_DIRECTORY)
+        for f in files:
+            f = os.path.join(self.IMAGE_OUPUT_DIRECTORY, f)
+            os.unlink(f)
+
+        self.state = State.STANDBY
+
     def on_state_read(self) -> State:
         """Returns the current state (called on SDO read of status)."""
         return self.state.value
 
     def on_state_write(self, data: int) -> None:
         """Sets state if valid (called on SDO write of status).
 
@@ -189,10 +205,12 @@
             if self.state == State.FILMING:
                 self.capture()
             elif self.state == State.TRANSMISSION:
                 if self.node.od["transmission"]["static_image"].value:
                     self.transmit_file_test()
                 else:
                     self.transmit()
+            elif self.state == State.PURGE:
+                self.purge()
 
         else:
             logger.error(f"Invalid state change: {self.state.name} -> {new_state.name}")
```

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif` & `oresat_dxwifi-0.3.3/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/templates/oresat_live.html` & `oresat_dxwifi-0.3.3/oresat_dxwifi/templates/oresat_live.html`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/configs/transmission_configs.yaml` & `oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/configs/transmission_configs.yaml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/defaults.py` & `oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/defaults.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/startmonitor.sh` & `oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/startmonitor.sh`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/transmission.py` & `oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/transmission.py`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi/transmission/tx_module.so` & `oresat_dxwifi-0.3.3/oresat_dxwifi/transmission/tx_module.so`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi.egg-info/PKG-INFO` & `oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-dxwifi
-Version: 0.3.2
+Version: 0.3.3
 Summary: OreSat DxWiFi OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `oresat_dxwifi-0.3.2/oresat_dxwifi.egg-info/SOURCES.txt` & `oresat_dxwifi-0.3.3/oresat_dxwifi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/pyproject.toml` & `oresat_dxwifi-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oresat_dxwifi-0.3.2/startmonitor.sh` & `oresat_dxwifi-0.3.3/startmonitor.sh`

 * *Files identical despite different names*

