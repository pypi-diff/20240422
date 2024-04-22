# Comparing `tmp/radiens-3.0.0b4.tar.gz` & `tmp/radiens-3.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radiens-3.0.0b4.tar", last modified: Tue Mar 12 16:41:49 2024, max compression
+gzip compressed data, was "radiens-3.0.0b5.tar", last modified: Wed Mar 27 16:33:48 2024, max compression
```

## Comparing `radiens-3.0.0b4.tar` & `radiens-3.0.0b5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.097851 radiens-3.0.0b4/
--rw-r--r--   0 akelly     (502) staff       (20)     1068 2024-02-20 17:19:00.000000 radiens-3.0.0b4/LICENSE
--rw-r--r--   0 akelly     (502) staff       (20)     2518 2024-03-12 16:41:49.097607 radiens-3.0.0b4/PKG-INFO
--rw-r--r--   0 akelly     (502) staff       (20)      156 2024-02-20 17:19:00.000000 radiens-3.0.0b4/README.md
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.085924 radiens-3.0.0b4/radiens/
--rw-r--r--   0 akelly     (502) staff       (20)      404 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)    17445 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/allego_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.087361 radiens-3.0.0b4/radiens/api/
--rw-r--r--   0 akelly     (502) staff       (20)       10 2024-02-20 17:19:00.000000 radiens-3.0.0b4/radiens/api/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)    24457 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/api/api_allego.py
--rw-r--r--   0 akelly     (502) staff       (20)     4524 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/api/api_curate.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.087946 radiens-3.0.0b4/radiens/api/api_utils/
--rw-r--r--   0 akelly     (502) staff       (20)       19 2024-02-28 17:36:10.000000 radiens-3.0.0b4/radiens/api/api_utils/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)    12256 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/api/api_utils/protocols.py
--rw-r--r--   0 akelly     (502) staff       (20)    10160 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/api/api_utils/util.py
--rw-r--r--   0 akelly     (502) staff       (20)    10359 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/api/api_videre.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.088300 radiens-3.0.0b4/radiens/auth/
--rw-r--r--   0 akelly     (502) staff       (20)       83 2024-02-20 17:19:00.000000 radiens-3.0.0b4/radiens/auth/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     3278 2024-02-20 17:19:00.000000 radiens-3.0.0b4/radiens/auth/interceptors.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.089844 radiens-3.0.0b4/radiens/cli/
--rw-r--r--   0 akelly     (502) staff       (20)       13 2024-02-28 17:36:10.000000 radiens-3.0.0b4/radiens/cli/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     9387 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/cli/allego.py
--rw-r--r--   0 akelly     (502) staff       (20)     7087 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/cli/file_sys.py
--rw-r--r--   0 akelly     (502) staff       (20)     1813 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/cli/main.py
--rw-r--r--   0 akelly     (502) staff       (20)    14132 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/cli/signal_metrics.py
--rw-r--r--   0 akelly     (502) staff       (20)     6012 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/cli/signals.py
--rw-r--r--   0 akelly     (502) staff       (20)     8216 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/cli/spike_sorter.py
--rw-r--r--   0 akelly     (502) staff       (20)     1813 2024-02-28 21:59:51.000000 radiens-3.0.0b4/radiens/cli/sys.py
--rw-r--r--   0 akelly     (502) staff       (20)     5374 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/cli/videre.py
--rw-r--r--   0 akelly     (502) staff       (20)    32842 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/curate_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.090372 radiens-3.0.0b4/radiens/exceptions/
--rw-r--r--   0 akelly     (502) staff       (20)      117 2024-02-28 17:36:10.000000 radiens-3.0.0b4/radiens/exceptions/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)      916 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/exceptions/grpc_error.py
--rw-r--r--   0 akelly     (502) staff       (20)      138 2024-02-28 17:36:10.000000 radiens-3.0.0b4/radiens/exceptions/scan_for_server_error.py
--rw-r--r--   0 akelly     (502) staff       (20)    14239 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/file_sys_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.093459 radiens-3.0.0b4/radiens/grpc_radiens/
--rw-r--r--   0 akelly     (502) staff       (20)       22 2024-02-28 17:36:10.000000 radiens-3.0.0b4/radiens/grpc_radiens/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)    31613 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/allegoserver_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)   159892 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/allegoserver_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    24570 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/biointerface_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/biointerface_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    76713 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/common_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/common_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)     7350 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/datasource_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/datasource_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    13824 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/pybridge_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)    27365 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/pybridge_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)     8649 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/radiens_dev_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/radiens_dev_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    16007 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/radiensserver_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)   172694 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/radiensserver_pb2_grpc.py
--rw-r--r--   0 akelly     (502) staff       (20)    23177 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/spikesorter_pb2.py
--rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-12 15:44:02.000000 radiens-3.0.0b4/radiens/grpc_radiens/spikesorter_pb2_grpc.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.095454 radiens-3.0.0b4/radiens/lib/
--rw-r--r--   0 akelly     (502) staff       (20)       13 2024-02-28 17:36:10.000000 radiens-3.0.0b4/radiens/lib/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     6207 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/lib/allego_lib.py
--rw-r--r--   0 akelly     (502) staff       (20)    15292 2024-03-12 16:37:03.000000 radiens-3.0.0b4/radiens/lib/channel_metadata.py
--rw-r--r--   0 akelly     (502) staff       (20)      166 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/lib/corelib.py
--rw-r--r--   0 akelly     (502) staff       (20)    10462 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/lib/dataset_metadata.py
--rw-r--r--   0 akelly     (502) staff       (20)     3660 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/lib/fsys.py
--rw-r--r--   0 akelly     (502) staff       (20)    11891 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/lib/sig_metrics.py
--rw-r--r--   0 akelly     (502) staff       (20)    11225 2024-03-12 16:37:03.000000 radiens-3.0.0b4/radiens/lib/signals_snapshot.py
--rw-r--r--   0 akelly     (502) staff       (20)     7434 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/lib/spike_sorter.py
--rw-r--r--   0 akelly     (502) staff       (20)    10914 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/lib/spikes.py
--rw-r--r--   0 akelly     (502) staff       (20)     7087 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/lib/summa.py
--rw-r--r--   0 akelly     (502) staff       (20)    26625 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/metrics_client.py
--rw-r--r--   0 akelly     (502) staff       (20)     8256 2024-03-12 16:37:03.000000 radiens-3.0.0b4/radiens/signals_client.py
--rw-r--r--   0 akelly     (502) staff       (20)    14790 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/spike_sorter_client.py
--rw-r--r--   0 akelly     (502) staff       (20)     7940 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/spikes_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.096244 radiens-3.0.0b4/radiens/utils/
--rw-r--r--   0 akelly     (502) staff       (20)       14 2024-02-20 17:19:00.000000 radiens-3.0.0b4/radiens/utils/__init__.py
--rw-r--r--   0 akelly     (502) staff       (20)     6138 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/utils/config.py
--rw-r--r--   0 akelly     (502) staff       (20)     4012 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/utils/constants.py
--rw-r--r--   0 akelly     (502) staff       (20)    16932 2024-03-12 16:37:03.000000 radiens-3.0.0b4/radiens/utils/enums.py
--rw-r--r--   0 akelly     (502) staff       (20)    12166 2024-03-11 16:22:46.000000 radiens-3.0.0b4/radiens/utils/util.py
--rw-r--r--   0 akelly     (502) staff       (20)       24 2024-03-12 16:41:48.000000 radiens-3.0.0b4/radiens/version.py
--rw-r--r--   0 akelly     (502) staff       (20)    13003 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/videre_client.py
--rw-r--r--   0 akelly     (502) staff       (20)     2602 2024-03-11 15:41:30.000000 radiens-3.0.0b4/radiens/workspace_client.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.086739 radiens-3.0.0b4/radiens.egg-info/
--rw-r--r--   0 akelly     (502) staff       (20)     2518 2024-03-12 16:41:49.000000 radiens-3.0.0b4/radiens.egg-info/PKG-INFO
--rw-r--r--   0 akelly     (502) staff       (20)     2328 2024-03-12 16:41:49.000000 radiens-3.0.0b4/radiens.egg-info/SOURCES.txt
--rw-r--r--   0 akelly     (502) staff       (20)        1 2024-03-12 16:41:49.000000 radiens-3.0.0b4/radiens.egg-info/dependency_links.txt
--rw-r--r--   0 akelly     (502) staff       (20)       49 2024-03-12 16:41:49.000000 radiens-3.0.0b4/radiens.egg-info/entry_points.txt
--rw-r--r--   0 akelly     (502) staff       (20)       54 2024-03-12 16:41:49.000000 radiens-3.0.0b4/radiens.egg-info/requires.txt
--rw-r--r--   0 akelly     (502) staff       (20)        8 2024-03-12 16:41:49.000000 radiens-3.0.0b4/radiens.egg-info/top_level.txt
--rw-r--r--   0 akelly     (502) staff       (20)       38 2024-03-12 16:41:49.097904 radiens-3.0.0b4/setup.cfg
--rw-r--r--   0 akelly     (502) staff       (20)     1294 2024-03-11 15:41:30.000000 radiens-3.0.0b4/setup.py
-drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-12 16:41:49.097233 radiens-3.0.0b4/tests/
--rw-r--r--   0 akelly     (502) staff       (20)      221 2024-02-20 17:19:00.000000 radiens-3.0.0b4/tests/test_Auth.py
--rw-r--r--   0 akelly     (502) staff       (20)     5186 2024-03-11 15:41:30.000000 radiens-3.0.0b4/tests/test_allego_client.py
--rw-r--r--   0 akelly     (502) staff       (20)     3277 2024-02-28 17:36:10.000000 radiens-3.0.0b4/tests/test_base_client.py
--rw-r--r--   0 akelly     (502) staff       (20)      346 2024-02-20 17:19:00.000000 radiens-3.0.0b4/tests/test_config.py
--rw-r--r--   0 akelly     (502) staff       (20)     6114 2024-03-11 15:41:30.000000 radiens-3.0.0b4/tests/test_curate_client.py
--rw-r--r--   0 akelly     (502) staff       (20)     4116 2024-03-11 15:41:30.000000 radiens-3.0.0b4/tests/test_videre_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.108742 radiens-3.0.0b5/
+-rw-r--r--   0 akelly     (502) staff       (20)     1068 2024-02-20 17:19:00.000000 radiens-3.0.0b5/LICENSE
+-rw-r--r--   0 akelly     (502) staff       (20)     2518 2024-03-27 16:33:48.108474 radiens-3.0.0b5/PKG-INFO
+-rw-r--r--   0 akelly     (502) staff       (20)      156 2024-02-20 17:19:00.000000 radiens-3.0.0b5/README.md
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.090028 radiens-3.0.0b5/radiens/
+-rw-r--r--   0 akelly     (502) staff       (20)      404 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    17445 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/allego_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.092019 radiens-3.0.0b5/radiens/api/
+-rw-r--r--   0 akelly     (502) staff       (20)       10 2024-02-20 17:19:00.000000 radiens-3.0.0b5/radiens/api/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    24457 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/api/api_allego.py
+-rw-r--r--   0 akelly     (502) staff       (20)     4524 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/api/api_curate.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.092841 radiens-3.0.0b5/radiens/api/api_utils/
+-rw-r--r--   0 akelly     (502) staff       (20)       19 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/api/api_utils/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    12256 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/api/api_utils/protocols.py
+-rw-r--r--   0 akelly     (502) staff       (20)    11102 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/api/api_utils/util.py
+-rw-r--r--   0 akelly     (502) staff       (20)    10359 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/api/api_videre.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.093294 radiens-3.0.0b5/radiens/auth/
+-rw-r--r--   0 akelly     (502) staff       (20)       83 2024-02-20 17:19:00.000000 radiens-3.0.0b5/radiens/auth/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     3278 2024-02-20 17:19:00.000000 radiens-3.0.0b5/radiens/auth/interceptors.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.095459 radiens-3.0.0b5/radiens/cli/
+-rw-r--r--   0 akelly     (502) staff       (20)       13 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/cli/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     9387 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/allego.py
+-rw-r--r--   0 akelly     (502) staff       (20)     7087 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/file_sys.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1813 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/main.py
+-rw-r--r--   0 akelly     (502) staff       (20)    14132 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/signal_metrics.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6012 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/signals.py
+-rw-r--r--   0 akelly     (502) staff       (20)     8216 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/spike_sorter.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1813 2024-02-28 21:59:51.000000 radiens-3.0.0b5/radiens/cli/sys.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5374 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/cli/videre.py
+-rw-r--r--   0 akelly     (502) staff       (20)    36686 2024-03-27 16:13:53.000000 radiens-3.0.0b5/radiens/curate_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.096248 radiens-3.0.0b5/radiens/exceptions/
+-rw-r--r--   0 akelly     (502) staff       (20)      117 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/exceptions/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     1077 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/exceptions/grpc_error.py
+-rw-r--r--   0 akelly     (502) staff       (20)      138 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/exceptions/scan_for_server_error.py
+-rw-r--r--   0 akelly     (502) staff       (20)    14239 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/file_sys_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.102212 radiens-3.0.0b5/radiens/grpc_radiens/
+-rw-r--r--   0 akelly     (502) staff       (20)       22 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/grpc_radiens/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)    33049 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/allegoserver_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)   159897 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/allegoserver_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    24570 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/biointerface_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/biointerface_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    76713 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/common_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/common_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)     7391 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/datasource_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/datasource_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    13824 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/pybridge_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)    27365 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/pybridge_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)     8740 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/radiens_dev_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/radiens_dev_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    16125 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/radiensserver_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)   174380 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/radiensserver_pb2_grpc.py
+-rw-r--r--   0 akelly     (502) staff       (20)    23177 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/spikesorter_pb2.py
+-rw-r--r--   0 akelly     (502) staff       (20)      159 2024-03-27 16:00:50.000000 radiens-3.0.0b5/radiens/grpc_radiens/spikesorter_pb2_grpc.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.104919 radiens-3.0.0b5/radiens/lib/
+-rw-r--r--   0 akelly     (502) staff       (20)       13 2024-02-28 17:36:10.000000 radiens-3.0.0b5/radiens/lib/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6207 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/allego_lib.py
+-rw-r--r--   0 akelly     (502) staff       (20)    15292 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/channel_metadata.py
+-rw-r--r--   0 akelly     (502) staff       (20)      166 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/corelib.py
+-rw-r--r--   0 akelly     (502) staff       (20)    10754 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/dataset_metadata.py
+-rw-r--r--   0 akelly     (502) staff       (20)     3660 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/fsys.py
+-rw-r--r--   0 akelly     (502) staff       (20)    11891 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/sig_metrics.py
+-rw-r--r--   0 akelly     (502) staff       (20)    11225 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/signals_snapshot.py
+-rw-r--r--   0 akelly     (502) staff       (20)     7434 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/spike_sorter.py
+-rw-r--r--   0 akelly     (502) staff       (20)    10914 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/spikes.py
+-rw-r--r--   0 akelly     (502) staff       (20)     7087 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/lib/summa.py
+-rw-r--r--   0 akelly     (502) staff       (20)    26625 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/metrics_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     8256 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/signals_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)    14790 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/spike_sorter_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     7940 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/spikes_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.106144 radiens-3.0.0b5/radiens/utils/
+-rw-r--r--   0 akelly     (502) staff       (20)       14 2024-02-20 17:19:00.000000 radiens-3.0.0b5/radiens/utils/__init__.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6138 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/utils/config.py
+-rw-r--r--   0 akelly     (502) staff       (20)     4232 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/utils/constants.py
+-rw-r--r--   0 akelly     (502) staff       (20)    17298 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/utils/enums.py
+-rw-r--r--   0 akelly     (502) staff       (20)    12166 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/utils/util.py
+-rw-r--r--   0 akelly     (502) staff       (20)       24 2024-03-27 16:33:47.000000 radiens-3.0.0b5/radiens/version.py
+-rw-r--r--   0 akelly     (502) staff       (20)    13003 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/videre_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     2602 2024-03-27 15:53:37.000000 radiens-3.0.0b5/radiens/workspace_client.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.090941 radiens-3.0.0b5/radiens.egg-info/
+-rw-r--r--   0 akelly     (502) staff       (20)     2518 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/PKG-INFO
+-rw-r--r--   0 akelly     (502) staff       (20)     2328 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/SOURCES.txt
+-rw-r--r--   0 akelly     (502) staff       (20)        1 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/dependency_links.txt
+-rw-r--r--   0 akelly     (502) staff       (20)       49 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/entry_points.txt
+-rw-r--r--   0 akelly     (502) staff       (20)       54 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/requires.txt
+-rw-r--r--   0 akelly     (502) staff       (20)        8 2024-03-27 16:33:48.000000 radiens-3.0.0b5/radiens.egg-info/top_level.txt
+-rw-r--r--   0 akelly     (502) staff       (20)       38 2024-03-27 16:33:48.108799 radiens-3.0.0b5/setup.cfg
+-rw-r--r--   0 akelly     (502) staff       (20)     1294 2024-03-27 15:53:37.000000 radiens-3.0.0b5/setup.py
+drwxr-xr-x   0 akelly     (502) staff       (20)        0 2024-03-27 16:33:48.108014 radiens-3.0.0b5/tests/
+-rw-r--r--   0 akelly     (502) staff       (20)      221 2024-02-20 17:19:00.000000 radiens-3.0.0b5/tests/test_Auth.py
+-rw-r--r--   0 akelly     (502) staff       (20)     5186 2024-03-27 15:53:37.000000 radiens-3.0.0b5/tests/test_allego_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     3277 2024-02-28 17:36:10.000000 radiens-3.0.0b5/tests/test_base_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)      346 2024-02-20 17:19:00.000000 radiens-3.0.0b5/tests/test_config.py
+-rw-r--r--   0 akelly     (502) staff       (20)     6114 2024-03-27 15:53:37.000000 radiens-3.0.0b5/tests/test_curate_client.py
+-rw-r--r--   0 akelly     (502) staff       (20)     4116 2024-03-27 15:53:37.000000 radiens-3.0.0b5/tests/test_videre_client.py
```

### Comparing `radiens-3.0.0b4/LICENSE` & `radiens-3.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/PKG-INFO` & `radiens-3.0.0b5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radiens
-Version: 3.0.0b4
+Version: 3.0.0b5
 Summary: provides python API to RADIENS analytics platform
 Home-page: http://neuronexus.github.io
 Author: NeuroNexus
 Author-email: dkipke@neuronexus.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `radiens-3.0.0b4/radiens/allego_client.py` & `radiens-3.0.0b5/radiens/allego_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/api/api_allego.py` & `radiens-3.0.0b5/radiens/api/api_allego.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/api/api_curate.py` & `radiens-3.0.0b5/radiens/api/api_curate.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/api/api_utils/protocols.py` & `radiens-3.0.0b5/radiens/api/api_utils/protocols.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/api/api_utils/util.py` & `radiens-3.0.0b5/radiens/api/api_utils/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import grpc
 import numpy as np
 import pandas as pd
 import radiens.utils.config as cfg
 from radiens.grpc_radiens import allegoserver_pb2, common_pb2
 from radiens.utils.constants import DEFAULT_HUB_ID, DEFAULT_IP
-from radiens.utils.enums import RadiensService
+from radiens.utils.enums import RadiensFileType, RadiensService
 
 
 def parse_stim_param_resp(resp: allegoserver_pb2.StimParamsReply):
     resp_dict = dict()
     for stim_sys_chan_idx, params in resp.params.items():
         resp_dict[stim_sys_chan_idx] = {}
         resp_dict[stim_sys_chan_idx]['stim_shape'] = params.stimShape
@@ -90,25 +90,55 @@
         return common_pb2.CSV
     if ext in ['.hdf5', '.h5']:
         return common_pb2.HDF5
     if ext in ['.nex5']:
         return common_pb2.NEX5
     if ext in ['.nwb']:
         return common_pb2.NWB
-    if ext in ['.kilosort2']:
+    if ext in ['.kilosort2', '.bin']:
         return common_pb2.KILOSORT2
     if ext in ['.nsx']:
         return common_pb2.NSX
     if ext in ['.tdt']:
         return common_pb2.TDT
     if ext in ['.spikes']:
         return common_pb2.SPIKES
     raise ValueError('{} is invalid or unknown file extension'.format(ext))
 
 
+def ext_to_radiens_file_type(ext: str):
+    return to_radiens_file_type(Path('file.' + ext))
+
+
+def to_suffix(file_type: RadiensFileType) -> str:
+    if file_type == RadiensFileType.RHD:
+        return ".rhd"
+    elif file_type == RadiensFileType.XDAT:
+        return ".xdat"
+    elif file_type == RadiensFileType.CSV:
+        return ".csv"
+    elif file_type == RadiensFileType.HDF5:
+        return ".h5"
+    elif file_type == RadiensFileType.NEX5:
+        return ".nex5"
+    elif file_type == RadiensFileType.NWB:
+        return ".nwb"
+    elif file_type == RadiensFileType.KILOSORT2:
+        return ".bin"
+    elif file_type == RadiensFileType.NSX:
+        return ".nsx"
+    elif file_type == RadiensFileType.TDT:
+        return ".tdt"
+    elif file_type == RadiensFileType.SPIKES:
+        return ".spikes"
+    else:
+        raise ValueError(
+            f"Invalid {RadiensFileType.__name__} value: {file_type}")
+
+
 def to_file_ext(file_type: common_pb2.RadixFileTypes):
     return common_pb2.RadixFileTypes.Name(file_type).lower()
 
 
 def path_to_source_sink_transform(p: Path) -> common_pb2.DataSourceSinkTransformParams:
     return common_pb2.DataSourceSinkTransformParams(dsrcName=p.expanduser().resolve().stem, path=str(p.expanduser().resolve().parent), fileType=to_radiens_file_type(p))
```

### Comparing `radiens-3.0.0b4/radiens/api/api_videre.py` & `radiens-3.0.0b5/radiens/api/api_videre.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/auth/interceptors.py` & `radiens-3.0.0b5/radiens/auth/interceptors.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/cli/allego.py` & `radiens-3.0.0b5/radiens/cli/allego.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/cli/file_sys.py` & `radiens-3.0.0b5/radiens/cli/file_sys.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/cli/main.py` & `radiens-3.0.0b5/radiens/cli/main.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/cli/signal_metrics.py` & `radiens-3.0.0b5/radiens/cli/signal_metrics.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/cli/signals.py` & `radiens-3.0.0b5/radiens/cli/signals.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/cli/spike_sorter.py` & `radiens-3.0.0b5/radiens/cli/spike_sorter.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/cli/sys.py` & `radiens-3.0.0b5/radiens/cli/sys.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/cli/videre.py` & `radiens-3.0.0b5/radiens/cli/videre.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/curate_client.py` & `radiens-3.0.0b5/radiens/curate_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,37 +2,44 @@
 import uuid
 import warnings
 from collections.abc import Iterable
 from pathlib import Path
 
 import radiens.api.api_curate as api_curate
 import radiens.api.api_videre as api_videre
+from grpc import RpcError
 from radiens.api.api_utils.protocols import (ProtocolAPI, TransformEdge,
                                              TransformNode)
-from radiens.api.api_utils.util import BaseClient, to_radiens_file_type
+from radiens.api.api_utils.util import (BaseClient, ext_to_radiens_file_type,
+                                        to_file_ext, to_radiens_file_type,
+                                        to_suffix)
+from radiens.exceptions.grpc_error import RpcException
+from radiens.file_sys_client import FileSystemClient
 from radiens.grpc_radiens import datasource_pb2
 from radiens.lib.dataset_metadata import DatasetMetadata
 from radiens.metrics_client import MetricsClient
 from radiens.spikes_client import SpikesClient
-from radiens.utils.constants import DEFAULT_HUB_ID
-from radiens.utils.enums import ClientType, RadiensService
+from radiens.utils.constants import (CONVERTIBLE_RADIENS_FILE_TYPES,
+                                     DEFAULT_HUB_ID)
+from radiens.utils.enums import ClientType, RadiensFileType, RadiensService
 from radiens.utils.util import rm_xdat_file
 from tqdm.autonotebook import tqdm
 
 
 class CurateClient(BaseClient):
     """
     CurateClient implements the radiens API for data curation. It matches and extends the functionality of the Radiens Curate UI app.
     """
 
     def __init__(self):
         """ """
         super().__init__()
         self._spikes = SpikesClient(self)
         self._metrics = MetricsClient(self)
+        self._fsys = FileSystemClient()
         self._dsp_stream = {}
 
     @property
     def hubs(self) -> dict:
         """
         dict of active radiens hubs, with hub ID as key.
         """
@@ -90,15 +97,15 @@
         to_del = []
         for stream_id in self.dsp_stream:
             if self.dsp_stream[stream_id]["stream"].done():
                 to_del.append(stream_id)
         for stream_id in to_del:
             del self.dsp_stream[stream_id]
 
-    def dsp_progress_bar(self, stream_id):
+    def progress_bar(self, stream_id):
         """
         Displays a progress bar showing the progress of the DSP stream running in the background.
         This function blocks until the background DSP stream is complete.
         This is an optional function that does not effect the DSP operation.
 
         Parameters:
             stream_id (str): stream ID of the requested DSP stream.
@@ -112,15 +119,15 @@
 
         See Also:
             :py:meth:`dsp_progress`
             :py:meth:`dsp_low_pass_filter`
 
         """
         pbar = tqdm(
-            total=self.dsp_stream[stream_id]["data_source"].duration_sec,
+            total=self.dsp_stream[stream_id]["data_source"].time_range.dur_sec,
             desc=stream_id,
             smoothing=0.9,
             bar_format="{desc}: {percentage:.1f}%|{bar}| {n:.2f}/{total_fmt} [{elapsed}<{remaining}]",
         )
         for progress in self.dsp_stream[stream_id]["stream"]:
             if progress.incrementSec is None:
                 warnings.warn(
@@ -208,25 +215,29 @@
         protocol.add_node(TransformNode('filt_lp').lowpass(cutoff_freq))
         protocol.add_edge(TransformEdge(
             'edge_0', protocol.nodes['src_0'].id, protocol.nodes['filt_lp'].id))
         protocol.add_node(TransformNode(
             'targ_0').datasource_sink(Path(target_path)))
         protocol.add_edge(TransformEdge(
             'edge_1', protocol.nodes['filt_lp'].id, protocol.nodes['targ_0'].id))
-        self._dsp_stream[protocol.id] = {'data_source': self._link_data_file(
-            Path(source_path)), 'protocol': protocol, 'stream': self._do_protocol(protocol, hub_name)}
+        self._dsp_stream[protocol.id] = {
+            'data_source': self._link_data_file(
+                Path(source_path)),
+            'protocol': protocol,
+            'stream': self._do_protocol(protocol, hub_name),
+        }
         self._clear_dataset(source_path)
         self._dsp_stream[protocol.id]["data_source"].clear_dataset_id()
         return protocol.id
 
     def dsp_high_pass_filter(
         self,
         cutoff_freq: float,
-        source_path: any,
-        target_path: any,
+        source_path: str | Path,
+        target_path: str | Path,
         force=False,
         hub_name=DEFAULT_HUB_ID,
     ):
         """
         Applies high-pass filter to source file to result in target file.
 
         The requested cut-off frequency must be < fs/2, where fs is the sample frequency of the source file.
@@ -249,25 +260,25 @@
             >>> client.dsp_high_pass_filter(20, './my_source_file', './my_output_file')
             None
         """
         if force:
             rm_xdat_file(Path(target_path))
         protocol = ProtocolAPI('hp_filter')
         protocol.add_node(TransformNode(
-            'src_0').datasource_source(source_path))
+            'src_0').datasource_source(Path(source_path)))
         protocol.add_node(TransformNode('filt_hp').highpass(cutoff_freq))
         protocol.add_edge(TransformEdge(
             'edge_0', protocol.nodes['src_0'].id, protocol.nodes['filt_hp'].id))
         protocol.add_node(TransformNode(
             'targ_0').datasource_sink(Path(target_path)))
         protocol.add_edge(TransformEdge(
             'edge_1', protocol.nodes['filt_hp'].id, protocol.nodes['targ_0'].id))
         self._dsp_stream[protocol.id] = {'data_source': self._link_data_file(
             Path(source_path)), 'protocol': protocol, 'stream': self._do_protocol(protocol, hub_name)}
-        self._clear_dataset(source_path)
+        self._clear_dataset(Path(source_path))
         self._dsp_stream[protocol.id]["data_source"].clear_dataset_id()
         return protocol.id
 
     def dsp_band_pass_filter(
         self,
         low_cutoff_freq: float,
         high_cutoff_freq,
@@ -653,14 +664,96 @@
             'edge_1', protocol.nodes['dec'].id, protocol.nodes['targ_0'].id))
         self._dsp_stream[protocol.id] = {'data_source': self._link_data_file(
             Path(source_path)), 'protocol': protocol, 'stream': self._do_protocol(protocol, hub_name)}
         self._clear_dataset(source_path)
         self._dsp_stream[protocol.id]["data_source"].clear_dataset_id()
         return protocol.id
 
+    def file_convert(
+            self,
+            source_path: Path,
+            dest_path: Path,
+            dest_file_type: str,
+            force=False,
+            hub_name=DEFAULT_HUB_ID,
+    ) -> str:
+        """
+        Converts source file to target file.
+
+        Parameters:
+            source_path (str, pathlib.Path): path to source file
+            target_path (str, pathlib.Path): path to target (output) file
+            force (bool): flag to force replacing target file if it exists
+            hub_name (str): radiens hub name (default=radiens.utils.constants.DEFAULT_HUB)
+
+        Returns:
+            stream_id (str): background DSP stream ID
+
+        Notes:
+            The source and target files
+        """
+
+        source_path = Path(source_path).expanduser().resolve()
+        source_path = Path(source_path.parent, source_path.stem)
+
+        dest_path = Path(dest_path).expanduser().resolve()
+        dest_path = Path(dest_path.parent, dest_path.stem)
+
+        # load source
+        try:
+            source_meta = self._link_data_file(Path(source_path))
+        except Exception as e:
+            raise ValueError("error loading source file", e)
+
+        if dest_path.suffix != "":
+            dest_file_type = RadiensFileType.parse(
+                ext_to_radiens_file_type(dest_path.suffix))
+        elif Path('file.'+dest_file_type).suffix != "":
+            dest_file_type = RadiensFileType.parse(
+                ext_to_radiens_file_type(Path('file.'+dest_file_type).suffix))
+        else:
+            warnings.warn(
+                'no file extension provided for target file. Assuming XDAT')
+            dest_file_type = RadiensFileType.XDAT
+
+        source_file_type = source_meta.file_type
+        if source_file_type == dest_file_type and dest_path.parent == source_path.parent and dest_path.stem == source_path.stem:
+            raise ValueError("source and target files are the same")
+
+        if source_file_type not in CONVERTIBLE_RADIENS_FILE_TYPES or dest_file_type not in CONVERTIBLE_RADIENS_FILE_TYPES:
+            raise ValueError(
+                f"file conversion between {source_file_type} and {dest_file_type} is not supported")
+
+        source_path = Path(str(source_path)+to_suffix(source_file_type))
+        dest_path = Path(str(dest_path)+to_suffix(dest_file_type))
+
+        if force:
+            try:
+                self._fsys.delete_files(dest_path)
+            except RpcException as e:
+                if "datasource does not exist" in map(
+                        lambda x: x.strip(), e.message.split(':')):
+                    pass
+                else:
+                    raise e
+
+        source_path = str(source_path)
+        protocol = ProtocolAPI('file_convert')
+        protocol.add_node(TransformNode(
+            'src_0').datasource_source(Path(source_path)))
+        protocol.add_node(TransformNode(
+            'targ_0').datasource_sink(Path(dest_path)))
+        protocol.add_edge(TransformEdge(
+            'edge_0', protocol.nodes['src_0'].id, protocol.nodes['targ_0'].id))
+        self._dsp_stream[protocol.id] = {'data_source': self._link_data_file(
+            Path(source_path)), 'protocol': protocol, 'stream': self._do_protocol(protocol, hub_name)}
+        self._clear_dataset(source_path)
+        self._dsp_stream[protocol.id]["data_source"].clear_dataset_id()
+        return protocol.id
+
     def dsp_slice_time(
         self,
         time_start: float,
         time_end: float,
         source_path: Path,
         target_path: Path,
         force=False,
```

### Comparing `radiens-3.0.0b4/radiens/exceptions/grpc_error.py` & `radiens-3.0.0b5/radiens/exceptions/grpc_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,9 +17,12 @@
         raise RpcException("Confirm {} is running".format(
             client_type), status_code) from None
     if status_code == StatusCode.UNAUTHENTICATED:
         raise RpcException("Invalid authentication", status_code) from None
     if status_code == StatusCode.RESOURCE_EXHAUSTED:
         raise RpcException("Data too big. Try smaller chunks",
                            status_code) from None
+    if status_code == StatusCode.UNKNOWN:
+        raise RpcException("Unknown error: {}".format(ex.details()),
+                           status_code) from None
     else:
         raise RpcError(ex) from None
```

### Comparing `radiens-3.0.0b4/radiens/file_sys_client.py` & `radiens-3.0.0b5/radiens/file_sys_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/grpc_radiens/allegoserver_pb2.py` & `radiens-3.0.0b5/radiens/grpc_radiens/allegoserver_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,160 +13,162 @@
 
 from . import common_pb2 as common__pb2
 from . import datasource_pb2 as datasource__pb2
 from . import biointerface_pb2 as biointerface__pb2
 from . import spikesorter_pb2 as spikesorter__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x61llegoserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\"4\n\x0eRestartRequest\x12\"\n\x04mode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\":\n\x11SetProfileRequest\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0c\n\x04type\x18\x02 \x02(\t\x12\x0b\n\x03\x64ur\x18\x03 \x02(\x02\"\xe9\x02\n\x10LogSystemRequest\x12\x34\n\x04mode\x18\x01 \x02(\x0e\x32&.allego.LogSystemRequest.LogSystemMode\x12=\n\x07outMode\x18\x02 \x01(\x0e\x32,.allego.LogSystemRequest.LogSystemOutputMode\x12\x16\n\x0eoutPathAndFile\x18\x03 \x01(\t\"|\n\rLogSystemMode\x12\n\n\x06\x63onfig\x10\x00\x12\n\n\x06status\x10\x01\x12\x0c\n\x08port_map\x10\x02\x12\n\n\x06pcache\x10\x03\x12\x0c\n\x08sigstats\x10\x04\x12\x11\n\rneurons_stats\x10\x06\x12\x18\n\x14\x62\x61se_signalgroup_map\x10\x07\"J\n\x13LogSystemOutputMode\x12\x12\n\x0eLOG_OUT_STDERR\x10\x00\x12\x0f\n\x0bLOG_OUT_CSV\x10\x01\x12\x0e\n\nLOG_OUT_MD\x10\x02\"4\n\x10SetStreamRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\"4\n\x10SetRecordRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\"~\n\x14SetConfigCoreRequest\x12\x10\n\x08sampFreq\x18\x01 \x01(\x01\x12\x0f\n\x07loopDur\x18\x02 \x01(\x01\x12\x19\n\x11pcachePersistence\x18\x03 \x01(\x01\x12(\n\x0b\x63\x61\x62leLength\x18\x04 \x01(\x0b\x32\x13.allego.CableLength\">\n\x0b\x43\x61\x62leLength\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x13\n\x0b\x63\x61\x62leLength\x18\x02 \x02(\x01\"f\n\x0c\x43\x61\x62leLengths\x12\t\n\x01\x41\x18\x01 \x02(\x01\x12\t\n\x01\x42\x18\x02 \x02(\x01\x12\t\n\x01\x43\x18\x03 \x02(\x01\x12\t\n\x01\x44\x18\x04 \x02(\x01\x12\t\n\x01\x45\x18\x05 \x02(\x01\x12\t\n\x01\x46\x18\x06 \x02(\x01\x12\t\n\x01G\x18\x07 \x02(\x01\x12\t\n\x01H\x18\x08 \x02(\x01\"\xb1\x01\n\nConfigCore\x12\x1c\n\x14\x61llegoCoreServerPort\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seSampFreq\x18\x03 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x04 \x02(\x05\x12*\n\x0c\x63\x61\x62leLengths\x18\x05 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x06 \x02(\x0e\x32\x14.allego.BackboneMode\"r\n\x0fRecordingStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x16\n\x0e\x61\x63tiveFileName\x18\x02 \x02(\t\x12\x10\n\x08\x64uration\x18\x03 \x02(\x01\x12\r\n\x05\x65rror\x18\x04 \x02(\t\"r\n\x0fStreamingStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x1a\n\x12primaryCacheTRange\x18\x02 \x03(\x01\x12\x1b\n\x13hardwareMemoryLevel\x18\x03 \x02(\x01\"\xda\x01\n\x0e\x42\x61\x63kboneStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\"\xc9\x02\n\x0f\x43onfigAndStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\x12\x14\n\x0c\x62\x61seSampFreq\x18\x06 \x02(\x01\x12*\n\x0c\x63\x61\x62leLengths\x18\x07 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x08 \x02(\x0e\x32\x14.allego.BackboneMode\"g\n\x0f\x43onfigRecording\x12\x14\n\x0c\x62\x61seFileName\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seFilePath\x18\x02 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x03 \x01(\x05\x12\x11\n\ttimeStamp\x18\x04 \x01(\x08\"V\n\x14\x44IOModeEventsRequest\x12\x0f\n\x07\x63hanIdx\x18\x02 \x02(\x05\x12\x16\n\x0e\x65ventThreshold\x18\x03 \x02(\x01\x12\x15\n\reventPolarity\x18\x04 \x02(\x08\"6\n\x14\x44IOModeManualRequest\x12\x0f\n\x07\x63hanIdx\x18\x01 \x02(\x05\x12\r\n\x05state\x18\x02 \x02(\x08\"s\n\x19\x44igitalOutChannelRegister\x12\x13\n\x0bmanualState\x18\x01 \x02(\x08\x12\x16\n\x0e\x65ventThreshold\x18\x02 \x02(\x01\x12\x15\n\reventPolarity\x18\x03 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x05\"q\n\x12\x44igitalOutRegister\x12\x1d\n\x04mode\x18\x01 \x02(\x0e\x32\x0f.allego.DIOMode\x12<\n\x11\x64outChanRegisters\x18\x02 \x03(\x0b\x32!.allego.DigitalOutChannelRegister\"\x1e\n\x0e\x44\x41\x43GainRequest\x12\x0c\n\x04gain\x18\x01 \x02(\x05\"9\n\x13\x44\x41\x43HighPassRegister\x12\x0e\n\x06\x65nable\x18\x01 \x02(\x08\x12\x12\n\ncutoffFreq\x18\x02 \x02(\x01\"w\n\x18\x41nalogOutChannelRegister\x12\x15\n\rPriNtvChanIdx\x18\x01 \x02(\x05\x12\x1b\n\x13\x41nalogOutNtvChanIdx\x18\x02 \x02(\x05\x12\x0e\n\x06Stream\x18\x03 \x02(\x05\x12\x17\n\x0fStreamOffsetIdx\x18\x04 \x02(\x05\"\x90\x01\n\x11\x41nalogOutRegister\x12;\n\x11\x61nalogOutChannels\x18\x01 \x03(\x0b\x32 .allego.AnalogOutChannelRegister\x12\x0c\n\x04gain\x18\x02 \x02(\x05\x12\x30\n\x0bhighpassReg\x18\x03 \x02(\x0b\x32\x1b.allego.DACHighPassRegister\"!\n\x0cSerialNumber\x12\x11\n\tserialNum\x18\x01 \x02(\t\"\x81\x01\n\x12SetSimPortsRequest\x12\x33\n\x07simPort\x18\x01 \x03(\x0b\x32\".allego.SetSimPortsRequest.SimPort\x1a\x36\n\x07SimPort\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07numChan\x18\x02 \x02(\x03\"4\n\x19SetHasGPIOExpanderRequest\x12\x17\n\x0fhasGPIOExpander\x18\x01 \x02(\x08\"\'\n\x14SetMuxChannelRequest\x12\x0f\n\x07\x63hannel\x18\x01 \x02(\x03\"\'\n\x14SetPotVoltageRequest\x12\x0f\n\x07voltage\x18\x01 \x02(\x02\"!\n\x10GetADCLevelReply\x12\r\n\x05level\x18\x01 \x02(\x02\"#\n\x12SetPotRangeRequest\x12\r\n\x05range\x18\x01 \x02(\x05\"!\n\x11SetPotModeRequest\x12\x0c\n\x04mode\x18\x01 \x02(\x08\")\n\x17SetPotCellEnableRequest\x12\x0e\n\x06\x65nable\x18\x01 \x02(\x08\",\n\x12ReadWireOutRequest\x12\x16\n\x0ewireOutAddress\x18\x01 \x02(\x03\"(\n\x10ReadWireOutReply\x12\x14\n\x0cwireOutValue\x18\x01 \x02(\x03\"\xc7\x02\n\x11LogsysConfigReply\x12(\n\nsystemMode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x03 \x02(\x05\x12\x1a\n\x12priCachePersistDur\x18\x04 \x02(\x01\x12!\n\x19priCacheStatsUpdatePeriod\x18\x05 \x02(\x01\x12\x12\n\nactiveSigs\x18\x06 \x02(\x05\x12\x10\n\x08priChans\x18\x07 \x02(\x05\x12\x10\n\x08\x61uxChans\x18\x08 \x02(\x05\x12\x10\n\x08\x64inChans\x18\t \x02(\x05\x12\x11\n\tdoutChans\x18\n \x02(\x05\x12\"\n\x08portSpec\x18\x0b \x03(\x0b\x32\x10.allego.PortInfo\x12\x19\n\x11numConnectedPorts\x18\x0c \x02(\x05\"Y\n\x08PortInfo\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\r\n\x05probe\x18\x02 \x02(\t\x12\x11\n\theadstage\x18\x03 \x02(\t\x12\x0f\n\x07numSigs\x18\x04 \x02(\x05\"c\n\x11LogsysStatusReply\x12\'\n\x07recStat\x18\x01 \x02(\x0b\x32\x16.allego.RecorderStatus\x12%\n\x07sysStat\x18\x02 \x02(\x0b\x32\x14.allego.SystemStatus\"\xba\x01\n\x0eRecorderStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x10\n\x08\x64uration\x18\x02 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\x03 \x02(\x01\x12\x11\n\tsizeBytes\x18\x04 \x02(\x05\x12\x0c\n\x04path\x18\x05 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x06 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x07 \x02(\x05\x12\x16\n\x0e\x61\x63tiveFileName\x18\x08 \x02(\t\"\x96\x03\n\x0cSystemStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x12\n\nnumPriSigs\x18\x03 \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x04 \x02(\x05\x12\x12\n\nnumDinSigs\x18\x05 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x06 \x02(\x05\x12\x13\n\x0btStampRange\x18\x07 \x03(\x03\x12\x0e\n\x06tRange\x18\x08 \x03(\x01\x12\x11\n\tstreamDur\x18\t \x02(\x01\x12\x14\n\x0cmeanChunkDur\x18\n \x02(\x01\x12\x1c\n\x14meanHardwareMemLevel\x18\x0b \x02(\x02\x12\x1b\n\x13maxHardwareMemLevel\x18\x0c \x02(\x02\x12\x1b\n\x13minHardwareMemLevel\x18\r \x02(\x02\x12\x1c\n\x14lastHardwareMemLevel\x18\x0e \x02(\x02\x12\x19\n\x11meanStreamLoopDur\x18\x0f \x02(\x01\x12\x18\n\x10streamEfficiency\x18\x10 \x02(\x01\"\xd8\x02\n\x11LogsysPcacheReply\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x18\n\x10minNumDatablocks\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x03\x12 \n\x18totalDatablocksProcessed\x18\x06 \x02(\x04\x12\x16\n\x0enumTimeSamples\x18\x07 \x02(\x03\x12\x1f\n\x17\x61llTimeMeanDatablockDur\x18\x08 \x02(\x01\x12\x15\n\rnumDataBlocks\x18\t \x02(\x05\x12\x0e\n\x06tRange\x18\n \x03(\x01\x12\x0f\n\x07tsRange\x18\x0b \x03(\x03\x12\x12\n\nnumPriSigs\x18\x0c \x02(\x05\x12\x12\n\nnumAuxSigs\x18\r \x02(\x05\x12\x12\n\nnumDinSigs\x18\x0e \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x0f \x02(\x05\"5\n\x10TriggerModeState\x12!\n\x04mode\x18\x01 \x02(\x0e\x32\x13.allego.TriggerMode\"*\n\x12LoadAllMosiRequest\x12\x14\n\x0cregisterVals\x18\x01 \x03(\x05\"\x15\n\x13TransmitMosiRequest\"5\n\x0f\x44umpMisoRequest\x12\x10\n\x08nSamples\x18\x01 \x02(\x05\x12\x10\n\x08\x66ileName\x18\x02 \x02(\t\"\xc6\x03\n\x15SinapsStatusRegisters\x12\x18\n\x10\x63\x61librationState\x18\x01 \x02(\x08\x12\x1b\n\x13\x63\x61librationProgress\x18\x02 \x02(\x01\x12\x1d\n\x15numActivePixelsShank0\x18\x03 \x02(\x05\x12\x1d\n\x15numActivePixelsShank1\x18\x04 \x02(\x05\x12\x1d\n\x15numActivePixelsShank2\x18\x05 \x02(\x05\x12\x1d\n\x15numActivePixelsShank3\x18\x06 \x02(\x05\x12\x0f\n\x07vRefFFA\x18\x07 \x02(\x01\x12\x0f\n\x07vRefFFB\x18\x08 \x02(\x01\x12\x0f\n\x07vRefFFC\x18\t \x02(\x01\x12\x0f\n\x07vRefFFD\x18\n \x02(\x01\x12\x10\n\x08isError0\x18\x0b \x02(\x08\x12\x10\n\x08isError1\x18\x0c \x02(\x08\x12\x10\n\x08isError2\x18\r \x02(\x08\x12\x10\n\x08isError3\x18\x0e \x02(\x08\x12\x13\n\x0bhostCounter\x18\x0f \x02(\x05\x12\x13\n\x0b\x66pgaCounter\x18\x10 \x02(\x05\x12\x17\n\x0f\x66irmwareVersion\x18\x11 \x02(\t\x12\x17\n\x0fprobeGeneration\x18\x12 \x02(\x05\x12\x12\n\nprobeModel\x18\x13 \x02(\x05\"%\n\x12\x46lashSinapsRequest\x12\x0f\n\x07\x62itfile\x18\x01 \x02(\t\"3\n\x0cHALdashboard\x12#\n\x04mode\x18\x01 \x02(\x0e\x32\x15.allego.AllegoHALmode\"\xbc\x06\n\nStimParams\x12$\n\tstimShape\x18\x01 \x02(\x0e\x32\x11.allego.StimShape\x12*\n\x0cstimPolarity\x18\x02 \x02(\x0e\x32\x14.allego.StimPolarity\x12\x1a\n\x12\x66irstPhaseDuration\x18\x03 \x02(\x01\x12\x1b\n\x13secondPhaseDuration\x18\x04 \x02(\x01\x12\x17\n\x0finterphaseDelay\x18\x05 \x02(\x01\x12\x1b\n\x13\x66irstPhaseAmplitude\x18\x06 \x02(\x01\x12\x1c\n\x14secondPhaseAmplitude\x18\x07 \x02(\x01\x12\x17\n\x0f\x62\x61selineVoltage\x18\x08 \x02(\x01\x12:\n\x12triggerEdgeOrLevel\x18\n \x02(\x0e\x32\x1e.allego.StimTriggerEdgeOrLevel\x12\x36\n\x10triggerHighOrLow\x18\x0b \x02(\x0e\x32\x1c.allego.StimTriggerHighOrLow\x12\x0f\n\x07\x65nabled\x18\x0c \x02(\x08\x12\x18\n\x10postTriggerDelay\x18\r \x02(\x01\x12.\n\x0cpulseOrTrain\x18\x0e \x02(\x0e\x32\x18.allego.StimPulseOrTrain\x12\x1a\n\x12numberOfStimPulses\x18\x0f \x02(\x05\x12\x18\n\x10pulseTrainPeriod\x18\x10 \x02(\x01\x12\x18\n\x10refractoryPeriod\x18\x11 \x02(\x01\x12\x18\n\x10preStimAmpSettle\x18\x12 \x02(\x01\x12\x19\n\x11postStimAmpSettle\x18\x13 \x02(\x01\x12\x19\n\x11maintainAmpSettle\x18\x14 \x02(\x08\x12\x17\n\x0f\x65nableAmpSettle\x18\x15 \x02(\x08\x12\x1d\n\x15postStimChargeRecovOn\x18\x16 \x02(\x01\x12\x1e\n\x16postStimChargeRecovOff\x18\x17 \x02(\x01\x12\x1c\n\x14\x65nableChargeRecovery\x18\x18 \x02(\x08\x12\x1f\n\x17triggerSourceIsKeypress\x18\x19 \x02(\x08\x12\x18\n\x10triggerSourceIdx\x18\x1a \x02(\x05\x12\x16\n\x0estimSysChanIdx\x18\x1b \x02(\x05\"\x89\x01\n\x0fStimParamsReply\x12\x33\n\x06params\x18\x01 \x03(\x0b\x32#.allego.StimParamsReply.ParamsEntry\x1a\x41\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.allego.StimParams:\x02\x38\x01\">\n\x18ManualStimTriggerRequest\x12\x0f\n\x07trigger\x18\x01 \x02(\x05\x12\x11\n\ttriggerOn\x18\x02 \x02(\x08\"1\n\x1eManualStimTriggerToggleRequest\x12\x0f\n\x07trigger\x18\x01 \x02(\x05\"5\n\x0fStimStepMessage\x12\"\n\x08stimStep\x18\x01 \x02(\x0e\x32\x10.allego.StimStep*!\n\nStreamMode\x12\t\n\x05S_OFF\x10\x00\x12\x08\n\x04S_ON\x10\x01*!\n\nRecordMode\x12\t\n\x05R_OFF\x10\x00\x12\x08\n\x04R_ON\x10\x01*\x9f\x04\n\x0c\x42\x61\x63kboneMode\x12\x10\n\x0cSMARTBOX_PRO\x10\x00\x12\x19\n\x15SMARTBOX_SIM_GEN_SINE\x10\x01\x12\x1b\n\x17SMARTBOX_SIM_GEN_SPIKES\x10\x02\x12\x1b\n\x17SMARTBOX_SIM_DATASOURCE\x10\x03\x12\x13\n\x0fOPEN_EPHYS_USB3\x10\x04\x12#\n\x1fINTAN_RECORDING_CONTROLLER_1024\x10\x05\x12\x14\n\x10SMARTBOX_CLASSIC\x10\x06\x12\"\n\x1eINTAN_RECORDING_CONTROLLER_512\x10\x07\x12\x13\n\x0fOPEN_EPHYS_USB2\x10\x08\x12\x0e\n\nINTAN_USB2\x10\t\x12 \n\x1cSMARTBOX_SIM_GEN_SINE_MAPPED\x10\n\x12#\n\x1fSMARTBOX_SIM_GEN_SINE_HIGH_FREQ\x10\x0b\x12$\n SMARTBOX_SIM_GEN_SINE_MULTI_BAND\x10\x0c\x12\x1b\n\x17SMARTBOX_PRO_SINAPS_256\x10\r\x12\x1c\n\x18SMARTBOX_PRO_SINAPS_1024\x10\x0e\x12\x10\n\x0cXDAQ_ONE_REC\x10\x0f\x12\x11\n\rXDAQ_ONE_STIM\x10\x10\x12\x11\n\rXDAQ_CORE_REC\x10\x11\x12\x12\n\x0eXDAQ_CORE_STIM\x10\x12\x12\x1b\n\x17SMARTBOX_PRO_SINAPS_512\x10\x13*,\n\x07\x44IOMode\x12\n\n\x06manual\x10\x00\x12\n\n\x06\x65vents\x10\x01\x12\t\n\x05gated\x10\x02*O\n\x0bTriggerMode\x12\x0b\n\x07T_DIN_0\x10\x00\x12\x0b\n\x07T_DIN_1\x10\x01\x12\x0c\n\x08T_DOUT_0\x10\x02\x12\x0c\n\x08T_DOUT_1\x10\x03\x12\n\n\x06T_NONE\x10\x04*q\n\rAllegoHALmode\x12\x11\n\rA_HAL_GENERIC\x10\x00\x12\x13\n\x0f\x41_HAL_SPIKESORT\x10\x01\x12\x14\n\x10\x41_HAL_MULTISCALE\x10\x02\x12\"\n\x1e\x41_HAL_MULTISCALE_BIDIRECTIONAL\x10\x03*W\n\tStimShape\x12\x0c\n\x08\x42IPHASIC\x10\x00\x12\x1d\n\x19\x42IPHASIC_INTERPHASE_DELAY\x10\x01\x12\r\n\tTRIPHASIC\x10\x02\x12\x0e\n\nMONOPHASIC\x10\x03*4\n\x0cStimPolarity\x12\x12\n\x0e\x43\x41THODIC_FIRST\x10\x00\x12\x10\n\x0c\x41NODIC_FIRST\x10\x01*3\n\x16StimTriggerEdgeOrLevel\x12\x0b\n\x07ST_EDGE\x10\x00\x12\x0c\n\x08ST_LEVEL\x10\x01*/\n\x14StimTriggerHighOrLow\x12\x0b\n\x07ST_HIGH\x10\x00\x12\n\n\x06ST_LOW\x10\x01*5\n\x10StimPulseOrTrain\x12\x10\n\x0cSINGLE_PULSE\x10\x00\x12\x0f\n\x0bPULSE_TRAIN\x10\x01*\x90\x02\n\x08StimStep\x12\x13\n\x0fStimStepSizeMin\x10\x00\x12\x14\n\x10StimStepSize10nA\x10\x01\x12\x14\n\x10StimStepSize20nA\x10\x02\x12\x14\n\x10StimStepSize50nA\x10\x03\x12\x15\n\x11StimStepSize100nA\x10\x04\x12\x15\n\x11StimStepSize200nA\x10\x05\x12\x15\n\x11StimStepSize500nA\x10\x06\x12\x13\n\x0fStimStepSize1uA\x10\x07\x12\x13\n\x0fStimStepSize2uA\x10\x08\x12\x13\n\x0fStimStepSize5uA\x10\t\x12\x14\n\x10StimStepSize10uA\x10\n\x12\x13\n\x0fStimStepSizeMax\x10\x0b\x32\xbe*\n\nAllegoCore\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\x07Restart\x12\x16.allego.RestartRequest\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12j\n\x1bGetStatusPollFieldsToUpdate\x12\'.allego.StatusPollFieldsToUpdateRequest\x1a .allego.StatusPollFieldsToUpdate\"\x00\x12R\n\x17GetOfflineLicenseStatus\x12\x17.allego.StandardRequest\x1a\x1c.allego.OfflineLicenseStatus\"\x00\x12\x46\n\rSetConfigCore\x12\x1c.allego.SetConfigCoreRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0fSetProfileState\x12\x19.allego.SetProfileRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x12SetConfigRecording\x12\x17.allego.ConfigRecording\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetStreamState\x12\x18.allego.SetStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetRecordState\x12\x18.allego.SetRecordRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOEvents\x12\x1c.allego.DIOModeEventsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOManual\x12\x1c.allego.DIOModeManualRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bSetDIOGated\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nSetDACGain\x12\x16.allego.DACGainRequest\x1a\x15.allego.StandardReply\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x0eSetDACHighPass\x12\x1b.allego.DACHighPassRegister\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetSimPorts\x12\x1a.allego.SetSimPortsRequest\x1a\x15.allego.StandardReply\"\x00\x12P\n\x12SetHasGPIOExpander\x12!.allego.SetHasGPIOExpanderRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetMuxChannel\x12\x1c.allego.SetMuxChannelRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetTriggerMode\x12\x18.allego.TriggerModeState\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetPotVoltage\x12\x1c.allego.SetPotVoltageRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetPotRange\x12\x1a.allego.SetPotRangeRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\nSetPotMode\x12\x19.allego.SetPotModeRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10SetPotCellEnable\x12\x1f.allego.SetPotCellEnableRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\rSetStimParams\x12\x12.allego.StimParams\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\rGetStimParams\x12\x17.allego.StandardRequest\x1a\x17.allego.StimParamsReply\"\x00\x12?\n\x0bSetStimStep\x12\x17.allego.StimStepMessage\x1a\x15.allego.StandardReply\"\x00\x12\x41\n\x0bGetStimStep\x12\x17.allego.StandardRequest\x1a\x17.allego.StimStepMessage\"\x00\x12N\n\x11ManualStimTrigger\x12 .allego.ManualStimTriggerRequest\x1a\x15.allego.StandardReply\"\x00\x12Z\n\x17ManualStimTriggerToggle\x12&.allego.ManualStimTriggerToggleRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\tGetConfig\x12\x17.allego.StandardRequest\x1a\x12.allego.ConfigCore\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12H\n\x12GetConfigRecording\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigRecording\"\x00\x12>\n\tGetStatus\x12\x17.allego.StandardRequest\x1a\x16.allego.BackboneStatus\"\x00\x12H\n\x12GetConfigAndStatus\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigAndStatus\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12\x42\n\x11GetIntanImpedance\x12\x18.allego.ImpedanceRequest\x1a\x11.allego.Impedance\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12\x42\n\tGetDIOReg\x12\x17.allego.StandardRequest\x1a\x1a.allego.DigitalOutRegister\"\x00\x12\x41\n\tGetDACReg\x12\x17.allego.StandardRequest\x1a\x19.allego.AnalogOutRegister\"\x00\x12<\n\tGetSerial\x12\x17.allego.StandardRequest\x1a\x14.allego.SerialNumber\"\x00\x12\x45\n\x0eGetTriggerMode\x12\x17.allego.StandardRequest\x1a\x18.allego.TriggerModeState\"\x00\x12\x42\n\x0bGetADCLevel\x12\x17.allego.StandardRequest\x1a\x18.allego.GetADCLevelReply\"\x00\x12\x45\n\x0bReadWireOut\x12\x1a.allego.ReadWireOutRequest\x1a\x18.allego.ReadWireOutReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12H\n\x0eGetSorterIDMap\x12\x17.allego.StandardRequest\x1a\x1b.allego.GetSorterIDMapReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tScanPorts\x12\x17.allego.StandardRequest\x1a\x13.allego.SignalGroup\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12O\n\x13GetDataSourceStatus\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceStatus\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bLoadAllMosi\x12\x1a.allego.LoadAllMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x0cTransmitMosi\x12\x1b.allego.TransmitMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\x08\x44umpMiso\x12\x17.allego.DumpMisoRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x18GetSinapsStatusRegisters\x12\x17.allego.StandardRequest\x1a\x1d.allego.SinapsStatusRegisters\"\x00\x12\x42\n\x0b\x46lashSinaps\x12\x1a.allego.FlashSinapsRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x16GetOrCreateEventViewer\x12\x15.allego.EventViewerID\x1a\x19.allego.EventViewerConfig\"\x00\x12G\n\x11UpdateEventViewer\x12\x19.allego.EventViewerConfig\x1a\x15.allego.StandardReply\"\x00\x12T\n\x15ListEventViewerEvents\x12\x15.allego.EventViewerID\x1a\".allego.ListEventViewerEventsReply\"\x00\x12U\n\x13GetEventViewerEvent\x12\".allego.GetEventViewerEventRequest\x1a\x18.allego.EventViewerEvent\"\x00\x12L\n\x10ListEventViewers\x12\x17.allego.StandardRequest\x1a\x1d.allego.ListEventViewersReply\"\x00\x12\x42\n\x0fGetHALdashboard\x12\x17.allego.StandardRequest\x1a\x14.allego.HALdashboard\"\x00\x32\xe4\x02\n\x07Pcache1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12J\n\x15GetHDSnapshotFromHead\x12\x1a.allego.HDSnapshotRequest2\x1a\x13.allego.HDSnapshot2\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12K\n\x12SetTimeRangeToHead\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x32\x8d\x04\n\x04Kpi1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x12K\n\x0bSetKpiParam\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x0bGetKpiParam\x12\x19.allego.DataSourceRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12I\n\x12SetKpiUpdatePeriod\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x0fSetKpiPacketDur\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x32\xa3\n\n\x08Neurons1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SpikeSorterSetParams\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x63\n\x17SpikeSorterGetDashboard\x12#.allego.SpikeSorterDashboardRequest\x1a!.allego.SpikeSorterDashboardReply\"\x00\x12i\n\x18SpikeSorterGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12\x61\n\x1a\x42iointerfaceGetSpikesDense\x12\x1e.allego.SpikesGetSpikesRequest\x1a!.allego.SpikesSpikeDataDenseReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12l\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x11.allego.TimeRange\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x12q\n\x15GetSpikeTrainAnalytic\x12+.allego.SpikesGetSpikeTrainAnalyticsRequest\x1a).allego.SpikesGetSpikeTrainAnalyticsReply\"\x00\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x61llegoserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\"4\n\x0eRestartRequest\x12\"\n\x04mode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\":\n\x11SetProfileRequest\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0c\n\x04type\x18\x02 \x02(\t\x12\x0b\n\x03\x64ur\x18\x03 \x02(\x02\"\xe9\x02\n\x10LogSystemRequest\x12\x34\n\x04mode\x18\x01 \x02(\x0e\x32&.allego.LogSystemRequest.LogSystemMode\x12=\n\x07outMode\x18\x02 \x01(\x0e\x32,.allego.LogSystemRequest.LogSystemOutputMode\x12\x16\n\x0eoutPathAndFile\x18\x03 \x01(\t\"|\n\rLogSystemMode\x12\n\n\x06\x63onfig\x10\x00\x12\n\n\x06status\x10\x01\x12\x0c\n\x08port_map\x10\x02\x12\n\n\x06pcache\x10\x03\x12\x0c\n\x08sigstats\x10\x04\x12\x11\n\rneurons_stats\x10\x06\x12\x18\n\x14\x62\x61se_signalgroup_map\x10\x07\"J\n\x13LogSystemOutputMode\x12\x12\n\x0eLOG_OUT_STDERR\x10\x00\x12\x0f\n\x0bLOG_OUT_CSV\x10\x01\x12\x0e\n\nLOG_OUT_MD\x10\x02\"4\n\x10SetStreamRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\"P\n\x10SetRecordRequest\x12 \n\x04mode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x1a\n\x04port\x18\x02 \x01(\x0e\x32\x0c.allego.Port\"~\n\x14SetConfigCoreRequest\x12\x10\n\x08sampFreq\x18\x01 \x01(\x01\x12\x0f\n\x07loopDur\x18\x02 \x01(\x01\x12\x19\n\x11pcachePersistence\x18\x03 \x01(\x01\x12(\n\x0b\x63\x61\x62leLength\x18\x04 \x01(\x0b\x32\x13.allego.CableLength\">\n\x0b\x43\x61\x62leLength\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x13\n\x0b\x63\x61\x62leLength\x18\x02 \x02(\x01\"f\n\x0c\x43\x61\x62leLengths\x12\t\n\x01\x41\x18\x01 \x02(\x01\x12\t\n\x01\x42\x18\x02 \x02(\x01\x12\t\n\x01\x43\x18\x03 \x02(\x01\x12\t\n\x01\x44\x18\x04 \x02(\x01\x12\t\n\x01\x45\x18\x05 \x02(\x01\x12\t\n\x01\x46\x18\x06 \x02(\x01\x12\t\n\x01G\x18\x07 \x02(\x01\x12\t\n\x01H\x18\x08 \x02(\x01\"\xb1\x01\n\nConfigCore\x12\x1c\n\x14\x61llegoCoreServerPort\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seSampFreq\x18\x03 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x04 \x02(\x05\x12*\n\x0c\x63\x61\x62leLengths\x18\x05 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x06 \x02(\x0e\x32\x14.allego.BackboneMode\"\xda\x03\n\x0fRecordingStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x16\n\x0e\x61\x63tiveFileName\x18\x02 \x02(\t\x12\x10\n\x08\x64uration\x18\x03 \x02(\x01\x12\r\n\x05\x65rror\x18\x04 \x02(\t\x12+\n\x0frecordModePortA\x18\x05 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortB\x18\x06 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortC\x18\x07 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortD\x18\x08 \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortE\x18\t \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortF\x18\n \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortG\x18\x0b \x01(\x0e\x32\x12.allego.RecordMode\x12+\n\x0frecordModePortH\x18\x0c \x01(\x0e\x32\x12.allego.RecordMode\"r\n\x0fStreamingStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x1a\n\x12primaryCacheTRange\x18\x02 \x03(\x01\x12\x1b\n\x13hardwareMemoryLevel\x18\x03 \x02(\x01\"\xda\x01\n\x0e\x42\x61\x63kboneStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\"\xc9\x02\n\x0f\x43onfigAndStatus\x12*\n\tstreaming\x18\x01 \x02(\x0b\x32\x17.allego.StreamingStatus\x12*\n\trecording\x18\x02 \x02(\x0b\x32\x17.allego.RecordingStatus\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x12\x13\n\x0bisConnected\x18\x04 \x02(\x08\x12\x32\n\x10gpioChannelCount\x18\x05 \x02(\x0b\x32\x18.allego.GPIOChannelCount\x12\x14\n\x0c\x62\x61seSampFreq\x18\x06 \x02(\x01\x12*\n\x0c\x63\x61\x62leLengths\x18\x07 \x02(\x0b\x32\x14.allego.CableLengths\x12*\n\x0c\x62\x61\x63kboneMode\x18\x08 \x02(\x0e\x32\x14.allego.BackboneMode\"\x9e\x01\n\x0f\x43onfigRecording\x12\x14\n\x0c\x62\x61seFileName\x18\x01 \x02(\t\x12\x14\n\x0c\x62\x61seFilePath\x18\x02 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x03 \x01(\x05\x12\x11\n\ttimeStamp\x18\x04 \x01(\x08\x12\x18\n\x10splitFilesByPort\x18\x05 \x01(\x08\x12\x1b\n\x13\x66orceStartAtTStamp0\x18\x06 \x01(\x08\"V\n\x14\x44IOModeEventsRequest\x12\x0f\n\x07\x63hanIdx\x18\x02 \x02(\x05\x12\x16\n\x0e\x65ventThreshold\x18\x03 \x02(\x01\x12\x15\n\reventPolarity\x18\x04 \x02(\x08\"6\n\x14\x44IOModeManualRequest\x12\x0f\n\x07\x63hanIdx\x18\x01 \x02(\x05\x12\r\n\x05state\x18\x02 \x02(\x08\"s\n\x19\x44igitalOutChannelRegister\x12\x13\n\x0bmanualState\x18\x01 \x02(\x08\x12\x16\n\x0e\x65ventThreshold\x18\x02 \x02(\x01\x12\x15\n\reventPolarity\x18\x03 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x05\"q\n\x12\x44igitalOutRegister\x12\x1d\n\x04mode\x18\x01 \x02(\x0e\x32\x0f.allego.DIOMode\x12<\n\x11\x64outChanRegisters\x18\x02 \x03(\x0b\x32!.allego.DigitalOutChannelRegister\"\x1e\n\x0e\x44\x41\x43GainRequest\x12\x0c\n\x04gain\x18\x01 \x02(\x05\"9\n\x13\x44\x41\x43HighPassRegister\x12\x0e\n\x06\x65nable\x18\x01 \x02(\x08\x12\x12\n\ncutoffFreq\x18\x02 \x02(\x01\"w\n\x18\x41nalogOutChannelRegister\x12\x15\n\rPriNtvChanIdx\x18\x01 \x02(\x05\x12\x1b\n\x13\x41nalogOutNtvChanIdx\x18\x02 \x02(\x05\x12\x0e\n\x06Stream\x18\x03 \x02(\x05\x12\x17\n\x0fStreamOffsetIdx\x18\x04 \x02(\x05\"\x90\x01\n\x11\x41nalogOutRegister\x12;\n\x11\x61nalogOutChannels\x18\x01 \x03(\x0b\x32 .allego.AnalogOutChannelRegister\x12\x0c\n\x04gain\x18\x02 \x02(\x05\x12\x30\n\x0bhighpassReg\x18\x03 \x02(\x0b\x32\x1b.allego.DACHighPassRegister\"!\n\x0cSerialNumber\x12\x11\n\tserialNum\x18\x01 \x02(\t\"\x81\x01\n\x12SetSimPortsRequest\x12\x33\n\x07simPort\x18\x01 \x03(\x0b\x32\".allego.SetSimPortsRequest.SimPort\x1a\x36\n\x07SimPort\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07numChan\x18\x02 \x02(\x03\"4\n\x19SetHasGPIOExpanderRequest\x12\x17\n\x0fhasGPIOExpander\x18\x01 \x02(\x08\"\'\n\x14SetMuxChannelRequest\x12\x0f\n\x07\x63hannel\x18\x01 \x02(\x03\"\'\n\x14SetPotVoltageRequest\x12\x0f\n\x07voltage\x18\x01 \x02(\x02\"!\n\x10GetADCLevelReply\x12\r\n\x05level\x18\x01 \x02(\x02\"#\n\x12SetPotRangeRequest\x12\r\n\x05range\x18\x01 \x02(\x05\"!\n\x11SetPotModeRequest\x12\x0c\n\x04mode\x18\x01 \x02(\x08\")\n\x17SetPotCellEnableRequest\x12\x0e\n\x06\x65nable\x18\x01 \x02(\x08\",\n\x12ReadWireOutRequest\x12\x16\n\x0ewireOutAddress\x18\x01 \x02(\x03\"(\n\x10ReadWireOutReply\x12\x14\n\x0cwireOutValue\x18\x01 \x02(\x03\"\xc7\x02\n\x11LogsysConfigReply\x12(\n\nsystemMode\x18\x01 \x02(\x0e\x32\x14.allego.BackboneMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x17\n\x0fstreamLoopDurMs\x18\x03 \x02(\x05\x12\x1a\n\x12priCachePersistDur\x18\x04 \x02(\x01\x12!\n\x19priCacheStatsUpdatePeriod\x18\x05 \x02(\x01\x12\x12\n\nactiveSigs\x18\x06 \x02(\x05\x12\x10\n\x08priChans\x18\x07 \x02(\x05\x12\x10\n\x08\x61uxChans\x18\x08 \x02(\x05\x12\x10\n\x08\x64inChans\x18\t \x02(\x05\x12\x11\n\tdoutChans\x18\n \x02(\x05\x12\"\n\x08portSpec\x18\x0b \x03(\x0b\x32\x10.allego.PortInfo\x12\x19\n\x11numConnectedPorts\x18\x0c \x02(\x05\"Y\n\x08PortInfo\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\r\n\x05probe\x18\x02 \x02(\t\x12\x11\n\theadstage\x18\x03 \x02(\t\x12\x0f\n\x07numSigs\x18\x04 \x02(\x05\"c\n\x11LogsysStatusReply\x12\'\n\x07recStat\x18\x01 \x02(\x0b\x32\x16.allego.RecorderStatus\x12%\n\x07sysStat\x18\x02 \x02(\x0b\x32\x14.allego.SystemStatus\"\xba\x01\n\x0eRecorderStatus\x12&\n\nrecordMode\x18\x01 \x02(\x0e\x32\x12.allego.RecordMode\x12\x10\n\x08\x64uration\x18\x02 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\x03 \x02(\x01\x12\x11\n\tsizeBytes\x18\x04 \x02(\x05\x12\x0c\n\x04path\x18\x05 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x06 \x02(\t\x12\x15\n\rdataSourceIdx\x18\x07 \x02(\x05\x12\x16\n\x0e\x61\x63tiveFileName\x18\x08 \x02(\t\"\x96\x03\n\x0cSystemStatus\x12&\n\nstreamMode\x18\x01 \x02(\x0e\x32\x12.allego.StreamMode\x12\x14\n\x0c\x62\x61seSampFreq\x18\x02 \x02(\x01\x12\x12\n\nnumPriSigs\x18\x03 \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x04 \x02(\x05\x12\x12\n\nnumDinSigs\x18\x05 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x06 \x02(\x05\x12\x13\n\x0btStampRange\x18\x07 \x03(\x03\x12\x0e\n\x06tRange\x18\x08 \x03(\x01\x12\x11\n\tstreamDur\x18\t \x02(\x01\x12\x14\n\x0cmeanChunkDur\x18\n \x02(\x01\x12\x1c\n\x14meanHardwareMemLevel\x18\x0b \x02(\x02\x12\x1b\n\x13maxHardwareMemLevel\x18\x0c \x02(\x02\x12\x1b\n\x13minHardwareMemLevel\x18\r \x02(\x02\x12\x1c\n\x14lastHardwareMemLevel\x18\x0e \x02(\x02\x12\x19\n\x11meanStreamLoopDur\x18\x0f \x02(\x01\x12\x18\n\x10streamEfficiency\x18\x10 \x02(\x01\"\xd8\x02\n\x11LogsysPcacheReply\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x18\n\x10minNumDatablocks\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x03\x12 \n\x18totalDatablocksProcessed\x18\x06 \x02(\x04\x12\x16\n\x0enumTimeSamples\x18\x07 \x02(\x03\x12\x1f\n\x17\x61llTimeMeanDatablockDur\x18\x08 \x02(\x01\x12\x15\n\rnumDataBlocks\x18\t \x02(\x05\x12\x0e\n\x06tRange\x18\n \x03(\x01\x12\x0f\n\x07tsRange\x18\x0b \x03(\x03\x12\x12\n\nnumPriSigs\x18\x0c \x02(\x05\x12\x12\n\nnumAuxSigs\x18\r \x02(\x05\x12\x12\n\nnumDinSigs\x18\x0e \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x0f \x02(\x05\"i\n\x11SetTriggerRequest\x12\'\n\x07\x63hannel\x18\x01 \x02(\x0e\x32\x16.allego.TriggerChannel\x12\x0f\n\x07\x65nabled\x18\x02 \x02(\x08\x12\x1a\n\x04port\x18\x03 \x01(\x0e\x32\x0c.allego.Port\"\\\n\x0cTriggerState\x12/\n\x0f\x65nabledChannels\x18\x01 \x03(\x0e\x32\x16.allego.TriggerChannel\x12\x1b\n\x05ports\x18\x02 \x03(\x0e\x32\x0c.allego.Port\"*\n\x12LoadAllMosiRequest\x12\x14\n\x0cregisterVals\x18\x01 \x03(\x05\"\x15\n\x13TransmitMosiRequest\"5\n\x0f\x44umpMisoRequest\x12\x10\n\x08nSamples\x18\x01 \x02(\x05\x12\x10\n\x08\x66ileName\x18\x02 \x02(\t\"\xc6\x03\n\x15SinapsStatusRegisters\x12\x18\n\x10\x63\x61librationState\x18\x01 \x02(\x08\x12\x1b\n\x13\x63\x61librationProgress\x18\x02 \x02(\x01\x12\x1d\n\x15numActivePixelsShank0\x18\x03 \x02(\x05\x12\x1d\n\x15numActivePixelsShank1\x18\x04 \x02(\x05\x12\x1d\n\x15numActivePixelsShank2\x18\x05 \x02(\x05\x12\x1d\n\x15numActivePixelsShank3\x18\x06 \x02(\x05\x12\x0f\n\x07vRefFFA\x18\x07 \x02(\x01\x12\x0f\n\x07vRefFFB\x18\x08 \x02(\x01\x12\x0f\n\x07vRefFFC\x18\t \x02(\x01\x12\x0f\n\x07vRefFFD\x18\n \x02(\x01\x12\x10\n\x08isError0\x18\x0b \x02(\x08\x12\x10\n\x08isError1\x18\x0c \x02(\x08\x12\x10\n\x08isError2\x18\r \x02(\x08\x12\x10\n\x08isError3\x18\x0e \x02(\x08\x12\x13\n\x0bhostCounter\x18\x0f \x02(\x05\x12\x13\n\x0b\x66pgaCounter\x18\x10 \x02(\x05\x12\x17\n\x0f\x66irmwareVersion\x18\x11 \x02(\t\x12\x17\n\x0fprobeGeneration\x18\x12 \x02(\x05\x12\x12\n\nprobeModel\x18\x13 \x02(\x05\"%\n\x12\x46lashSinapsRequest\x12\x0f\n\x07\x62itfile\x18\x01 \x02(\t\"3\n\x0cHALdashboard\x12#\n\x04mode\x18\x01 \x02(\x0e\x32\x15.allego.AllegoHALmode\"\xbc\x06\n\nStimParams\x12$\n\tstimShape\x18\x01 \x02(\x0e\x32\x11.allego.StimShape\x12*\n\x0cstimPolarity\x18\x02 \x02(\x0e\x32\x14.allego.StimPolarity\x12\x1a\n\x12\x66irstPhaseDuration\x18\x03 \x02(\x01\x12\x1b\n\x13secondPhaseDuration\x18\x04 \x02(\x01\x12\x17\n\x0finterphaseDelay\x18\x05 \x02(\x01\x12\x1b\n\x13\x66irstPhaseAmplitude\x18\x06 \x02(\x01\x12\x1c\n\x14secondPhaseAmplitude\x18\x07 \x02(\x01\x12\x17\n\x0f\x62\x61selineVoltage\x18\x08 \x02(\x01\x12:\n\x12triggerEdgeOrLevel\x18\n \x02(\x0e\x32\x1e.allego.StimTriggerEdgeOrLevel\x12\x36\n\x10triggerHighOrLow\x18\x0b \x02(\x0e\x32\x1c.allego.StimTriggerHighOrLow\x12\x0f\n\x07\x65nabled\x18\x0c \x02(\x08\x12\x18\n\x10postTriggerDelay\x18\r \x02(\x01\x12.\n\x0cpulseOrTrain\x18\x0e \x02(\x0e\x32\x18.allego.StimPulseOrTrain\x12\x1a\n\x12numberOfStimPulses\x18\x0f \x02(\x05\x12\x18\n\x10pulseTrainPeriod\x18\x10 \x02(\x01\x12\x18\n\x10refractoryPeriod\x18\x11 \x02(\x01\x12\x18\n\x10preStimAmpSettle\x18\x12 \x02(\x01\x12\x19\n\x11postStimAmpSettle\x18\x13 \x02(\x01\x12\x19\n\x11maintainAmpSettle\x18\x14 \x02(\x08\x12\x17\n\x0f\x65nableAmpSettle\x18\x15 \x02(\x08\x12\x1d\n\x15postStimChargeRecovOn\x18\x16 \x02(\x01\x12\x1e\n\x16postStimChargeRecovOff\x18\x17 \x02(\x01\x12\x1c\n\x14\x65nableChargeRecovery\x18\x18 \x02(\x08\x12\x1f\n\x17triggerSourceIsKeypress\x18\x19 \x02(\x08\x12\x18\n\x10triggerSourceIdx\x18\x1a \x02(\x05\x12\x16\n\x0estimSysChanIdx\x18\x1b \x02(\x05\"\x89\x01\n\x0fStimParamsReply\x12\x33\n\x06params\x18\x01 \x03(\x0b\x32#.allego.StimParamsReply.ParamsEntry\x1a\x41\n\x0bParamsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.allego.StimParams:\x02\x38\x01\">\n\x18ManualStimTriggerRequest\x12\x0f\n\x07trigger\x18\x01 \x02(\x05\x12\x11\n\ttriggerOn\x18\x02 \x02(\x08\"1\n\x1eManualStimTriggerToggleRequest\x12\x0f\n\x07trigger\x18\x01 \x02(\x05\"5\n\x0fStimStepMessage\x12\"\n\x08stimStep\x18\x01 \x02(\x0e\x32\x10.allego.StimStep*!\n\nStreamMode\x12\t\n\x05S_OFF\x10\x00\x12\x08\n\x04S_ON\x10\x01*!\n\nRecordMode\x12\t\n\x05R_OFF\x10\x00\x12\x08\n\x04R_ON\x10\x01*\x9f\x04\n\x0c\x42\x61\x63kboneMode\x12\x10\n\x0cSMARTBOX_PRO\x10\x00\x12\x19\n\x15SMARTBOX_SIM_GEN_SINE\x10\x01\x12\x1b\n\x17SMARTBOX_SIM_GEN_SPIKES\x10\x02\x12\x1b\n\x17SMARTBOX_SIM_DATASOURCE\x10\x03\x12\x13\n\x0fOPEN_EPHYS_USB3\x10\x04\x12#\n\x1fINTAN_RECORDING_CONTROLLER_1024\x10\x05\x12\x14\n\x10SMARTBOX_CLASSIC\x10\x06\x12\"\n\x1eINTAN_RECORDING_CONTROLLER_512\x10\x07\x12\x13\n\x0fOPEN_EPHYS_USB2\x10\x08\x12\x0e\n\nINTAN_USB2\x10\t\x12 \n\x1cSMARTBOX_SIM_GEN_SINE_MAPPED\x10\n\x12#\n\x1fSMARTBOX_SIM_GEN_SINE_HIGH_FREQ\x10\x0b\x12$\n SMARTBOX_SIM_GEN_SINE_MULTI_BAND\x10\x0c\x12\x1b\n\x17SMARTBOX_PRO_SINAPS_256\x10\r\x12\x1c\n\x18SMARTBOX_PRO_SINAPS_1024\x10\x0e\x12\x10\n\x0cXDAQ_ONE_REC\x10\x0f\x12\x11\n\rXDAQ_ONE_STIM\x10\x10\x12\x11\n\rXDAQ_CORE_REC\x10\x11\x12\x12\n\x0eXDAQ_CORE_STIM\x10\x12\x12\x1b\n\x17SMARTBOX_PRO_SINAPS_512\x10\x13*,\n\x07\x44IOMode\x12\n\n\x06manual\x10\x00\x12\n\n\x06\x65vents\x10\x01\x12\t\n\x05gated\x10\x02*\xf4\x01\n\x0eTriggerChannel\x12\x0b\n\x07T_DIN_0\x10\x00\x12\x0b\n\x07T_DIN_1\x10\x01\x12\x0b\n\x07T_DIN_2\x10\x02\x12\x0b\n\x07T_DIN_3\x10\x03\x12\x0b\n\x07T_DIN_4\x10\x04\x12\x0b\n\x07T_DIN_5\x10\x05\x12\x0b\n\x07T_DIN_6\x10\x06\x12\x0b\n\x07T_DIN_7\x10\x07\x12\x0c\n\x08T_DOUT_0\x10\x08\x12\x0c\n\x08T_DOUT_1\x10\t\x12\x0c\n\x08T_DOUT_2\x10\n\x12\x0c\n\x08T_DOUT_3\x10\x0b\x12\x0c\n\x08T_DOUT_4\x10\x0c\x12\x0c\n\x08T_DOUT_5\x10\r\x12\x0c\n\x08T_DOUT_6\x10\x0e\x12\x0c\n\x08T_DOUT_7\x10\x0f\x12\n\n\x06T_NONE\x10\x10*q\n\rAllegoHALmode\x12\x11\n\rA_HAL_GENERIC\x10\x00\x12\x13\n\x0f\x41_HAL_SPIKESORT\x10\x01\x12\x14\n\x10\x41_HAL_MULTISCALE\x10\x02\x12\"\n\x1e\x41_HAL_MULTISCALE_BIDIRECTIONAL\x10\x03*W\n\tStimShape\x12\x0c\n\x08\x42IPHASIC\x10\x00\x12\x1d\n\x19\x42IPHASIC_INTERPHASE_DELAY\x10\x01\x12\r\n\tTRIPHASIC\x10\x02\x12\x0e\n\nMONOPHASIC\x10\x03*4\n\x0cStimPolarity\x12\x12\n\x0e\x43\x41THODIC_FIRST\x10\x00\x12\x10\n\x0c\x41NODIC_FIRST\x10\x01*3\n\x16StimTriggerEdgeOrLevel\x12\x0b\n\x07ST_EDGE\x10\x00\x12\x0c\n\x08ST_LEVEL\x10\x01*/\n\x14StimTriggerHighOrLow\x12\x0b\n\x07ST_HIGH\x10\x00\x12\n\n\x06ST_LOW\x10\x01*5\n\x10StimPulseOrTrain\x12\x10\n\x0cSINGLE_PULSE\x10\x00\x12\x0f\n\x0bPULSE_TRAIN\x10\x01*\x90\x02\n\x08StimStep\x12\x13\n\x0fStimStepSizeMin\x10\x00\x12\x14\n\x10StimStepSize10nA\x10\x01\x12\x14\n\x10StimStepSize20nA\x10\x02\x12\x14\n\x10StimStepSize50nA\x10\x03\x12\x15\n\x11StimStepSize100nA\x10\x04\x12\x15\n\x11StimStepSize200nA\x10\x05\x12\x15\n\x11StimStepSize500nA\x10\x06\x12\x13\n\x0fStimStepSize1uA\x10\x07\x12\x13\n\x0fStimStepSize2uA\x10\x08\x12\x13\n\x0fStimStepSize5uA\x10\t\x12\x14\n\x10StimStepSize10uA\x10\n\x12\x13\n\x0fStimStepSizeMax\x10\x0b\x32\xbd*\n\nAllegoCore\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\x07Restart\x12\x16.allego.RestartRequest\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12j\n\x1bGetStatusPollFieldsToUpdate\x12\'.allego.StatusPollFieldsToUpdateRequest\x1a .allego.StatusPollFieldsToUpdate\"\x00\x12R\n\x17GetOfflineLicenseStatus\x12\x17.allego.StandardRequest\x1a\x1c.allego.OfflineLicenseStatus\"\x00\x12\x46\n\rSetConfigCore\x12\x1c.allego.SetConfigCoreRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0fSetProfileState\x12\x19.allego.SetProfileRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x12SetConfigRecording\x12\x17.allego.ConfigRecording\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetStreamState\x12\x18.allego.SetStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0eSetRecordState\x12\x18.allego.SetRecordRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOEvents\x12\x1c.allego.DIOModeEventsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cSetDIOManual\x12\x1c.allego.DIOModeManualRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bSetDIOGated\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nSetDACGain\x12\x16.allego.DACGainRequest\x1a\x15.allego.StandardReply\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x0eSetDACHighPass\x12\x1b.allego.DACHighPassRegister\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetSimPorts\x12\x1a.allego.SetSimPortsRequest\x1a\x15.allego.StandardReply\"\x00\x12P\n\x12SetHasGPIOExpander\x12!.allego.SetHasGPIOExpanderRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetMuxChannel\x12\x1c.allego.SetMuxChannelRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0fSetTriggerState\x12\x19.allego.SetTriggerRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\rSetPotVoltage\x12\x1c.allego.SetPotVoltageRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetPotRange\x12\x1a.allego.SetPotRangeRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\nSetPotMode\x12\x19.allego.SetPotModeRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10SetPotCellEnable\x12\x1f.allego.SetPotCellEnableRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\rSetStimParams\x12\x12.allego.StimParams\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\rGetStimParams\x12\x17.allego.StandardRequest\x1a\x17.allego.StimParamsReply\"\x00\x12?\n\x0bSetStimStep\x12\x17.allego.StimStepMessage\x1a\x15.allego.StandardReply\"\x00\x12\x41\n\x0bGetStimStep\x12\x17.allego.StandardRequest\x1a\x17.allego.StimStepMessage\"\x00\x12N\n\x11ManualStimTrigger\x12 .allego.ManualStimTriggerRequest\x1a\x15.allego.StandardReply\"\x00\x12Z\n\x17ManualStimTriggerToggle\x12&.allego.ManualStimTriggerToggleRequest\x1a\x15.allego.StandardReply\"\x00\x12:\n\tGetConfig\x12\x17.allego.StandardRequest\x1a\x12.allego.ConfigCore\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12H\n\x12GetConfigRecording\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigRecording\"\x00\x12>\n\tGetStatus\x12\x17.allego.StandardRequest\x1a\x16.allego.BackboneStatus\"\x00\x12H\n\x12GetConfigAndStatus\x12\x17.allego.StandardRequest\x1a\x17.allego.ConfigAndStatus\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12\x42\n\x11GetIntanImpedance\x12\x18.allego.ImpedanceRequest\x1a\x11.allego.Impedance\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12\x42\n\tGetDIOReg\x12\x17.allego.StandardRequest\x1a\x1a.allego.DigitalOutRegister\"\x00\x12\x41\n\tGetDACReg\x12\x17.allego.StandardRequest\x1a\x19.allego.AnalogOutRegister\"\x00\x12<\n\tGetSerial\x12\x17.allego.StandardRequest\x1a\x14.allego.SerialNumber\"\x00\x12\x42\n\x0fGetTriggerState\x12\x17.allego.StandardRequest\x1a\x14.allego.TriggerState\"\x00\x12\x42\n\x0bGetADCLevel\x12\x17.allego.StandardRequest\x1a\x18.allego.GetADCLevelReply\"\x00\x12\x45\n\x0bReadWireOut\x12\x1a.allego.ReadWireOutRequest\x1a\x18.allego.ReadWireOutReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12H\n\x0eGetSorterIDMap\x12\x17.allego.StandardRequest\x1a\x1b.allego.GetSorterIDMapReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tScanPorts\x12\x17.allego.StandardRequest\x1a\x13.allego.SignalGroup\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12O\n\x13GetDataSourceStatus\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceStatus\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12\x42\n\x0bLoadAllMosi\x12\x1a.allego.LoadAllMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x0cTransmitMosi\x12\x1b.allego.TransmitMosiRequest\x1a\x15.allego.StandardReply\"\x00\x12<\n\x08\x44umpMiso\x12\x17.allego.DumpMisoRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x18GetSinapsStatusRegisters\x12\x17.allego.StandardRequest\x1a\x1d.allego.SinapsStatusRegisters\"\x00\x12\x42\n\x0b\x46lashSinaps\x12\x1a.allego.FlashSinapsRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x16GetOrCreateEventViewer\x12\x15.allego.EventViewerID\x1a\x19.allego.EventViewerConfig\"\x00\x12G\n\x11UpdateEventViewer\x12\x19.allego.EventViewerConfig\x1a\x15.allego.StandardReply\"\x00\x12T\n\x15ListEventViewerEvents\x12\x15.allego.EventViewerID\x1a\".allego.ListEventViewerEventsReply\"\x00\x12U\n\x13GetEventViewerEvent\x12\".allego.GetEventViewerEventRequest\x1a\x18.allego.EventViewerEvent\"\x00\x12L\n\x10ListEventViewers\x12\x17.allego.StandardRequest\x1a\x1d.allego.ListEventViewersReply\"\x00\x12\x42\n\x0fGetHALdashboard\x12\x17.allego.StandardRequest\x1a\x14.allego.HALdashboard\"\x00\x32\xe4\x02\n\x07Pcache1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12J\n\x15GetHDSnapshotFromHead\x12\x1a.allego.HDSnapshotRequest2\x1a\x13.allego.HDSnapshot2\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12K\n\x12SetTimeRangeToHead\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x32\x8d\x04\n\x04Kpi1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x12K\n\x0bSetKpiParam\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x0bGetKpiParam\x12\x19.allego.DataSourceRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12I\n\x12SetKpiUpdatePeriod\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x46\n\x0fSetKpiPacketDur\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x32\xa3\n\n\x08Neurons1\x12?\n\x0bHealthcheck\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SpikeSorterSetParams\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x63\n\x17SpikeSorterGetDashboard\x12#.allego.SpikeSorterDashboardRequest\x1a!.allego.SpikeSorterDashboardReply\"\x00\x12i\n\x18SpikeSorterGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12\x61\n\x1a\x42iointerfaceGetSpikesDense\x12\x1e.allego.SpikesGetSpikesRequest\x1a!.allego.SpikesSpikeDataDenseReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12l\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x11.allego.TimeRange\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x12q\n\x15GetSpikeTrainAnalytic\x12+.allego.SpikesGetSpikeTrainAnalyticsRequest\x1a).allego.SpikesGetSpikeTrainAnalyticsReply\"\x00\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'allegoserver_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
   _STIMPARAMSREPLY_PARAMSENTRY._options = None
   _STIMPARAMSREPLY_PARAMSENTRY._serialized_options = b'8\001'
-  _STREAMMODE._serialized_start=6663
-  _STREAMMODE._serialized_end=6696
-  _RECORDMODE._serialized_start=6698
-  _RECORDMODE._serialized_end=6731
-  _BACKBONEMODE._serialized_start=6734
-  _BACKBONEMODE._serialized_end=7277
-  _DIOMODE._serialized_start=7279
-  _DIOMODE._serialized_end=7323
-  _TRIGGERMODE._serialized_start=7325
-  _TRIGGERMODE._serialized_end=7404
-  _ALLEGOHALMODE._serialized_start=7406
-  _ALLEGOHALMODE._serialized_end=7519
-  _STIMSHAPE._serialized_start=7521
-  _STIMSHAPE._serialized_end=7608
-  _STIMPOLARITY._serialized_start=7610
-  _STIMPOLARITY._serialized_end=7662
-  _STIMTRIGGEREDGEORLEVEL._serialized_start=7664
-  _STIMTRIGGEREDGEORLEVEL._serialized_end=7715
-  _STIMTRIGGERHIGHORLOW._serialized_start=7717
-  _STIMTRIGGERHIGHORLOW._serialized_end=7764
-  _STIMPULSEORTRAIN._serialized_start=7766
-  _STIMPULSEORTRAIN._serialized_end=7819
-  _STIMSTEP._serialized_start=7822
-  _STIMSTEP._serialized_end=8094
+  _STREAMMODE._serialized_start=7254
+  _STREAMMODE._serialized_end=7287
+  _RECORDMODE._serialized_start=7289
+  _RECORDMODE._serialized_end=7322
+  _BACKBONEMODE._serialized_start=7325
+  _BACKBONEMODE._serialized_end=7868
+  _DIOMODE._serialized_start=7870
+  _DIOMODE._serialized_end=7914
+  _TRIGGERCHANNEL._serialized_start=7917
+  _TRIGGERCHANNEL._serialized_end=8161
+  _ALLEGOHALMODE._serialized_start=8163
+  _ALLEGOHALMODE._serialized_end=8276
+  _STIMSHAPE._serialized_start=8278
+  _STIMSHAPE._serialized_end=8365
+  _STIMPOLARITY._serialized_start=8367
+  _STIMPOLARITY._serialized_end=8419
+  _STIMTRIGGEREDGEORLEVEL._serialized_start=8421
+  _STIMTRIGGEREDGEORLEVEL._serialized_end=8472
+  _STIMTRIGGERHIGHORLOW._serialized_start=8474
+  _STIMTRIGGERHIGHORLOW._serialized_end=8521
+  _STIMPULSEORTRAIN._serialized_start=8523
+  _STIMPULSEORTRAIN._serialized_end=8576
+  _STIMSTEP._serialized_start=8579
+  _STIMSTEP._serialized_end=8851
   _RESTARTREQUEST._serialized_start=101
   _RESTARTREQUEST._serialized_end=153
   _SETPROFILEREQUEST._serialized_start=155
   _SETPROFILEREQUEST._serialized_end=213
   _LOGSYSTEMREQUEST._serialized_start=216
   _LOGSYSTEMREQUEST._serialized_end=577
   _LOGSYSTEMREQUEST_LOGSYSTEMMODE._serialized_start=377
   _LOGSYSTEMREQUEST_LOGSYSTEMMODE._serialized_end=501
   _LOGSYSTEMREQUEST_LOGSYSTEMOUTPUTMODE._serialized_start=503
   _LOGSYSTEMREQUEST_LOGSYSTEMOUTPUTMODE._serialized_end=577
   _SETSTREAMREQUEST._serialized_start=579
   _SETSTREAMREQUEST._serialized_end=631
   _SETRECORDREQUEST._serialized_start=633
-  _SETRECORDREQUEST._serialized_end=685
-  _SETCONFIGCOREREQUEST._serialized_start=687
-  _SETCONFIGCOREREQUEST._serialized_end=813
-  _CABLELENGTH._serialized_start=815
-  _CABLELENGTH._serialized_end=877
-  _CABLELENGTHS._serialized_start=879
-  _CABLELENGTHS._serialized_end=981
-  _CONFIGCORE._serialized_start=984
-  _CONFIGCORE._serialized_end=1161
-  _RECORDINGSTATUS._serialized_start=1163
-  _RECORDINGSTATUS._serialized_end=1277
-  _STREAMINGSTATUS._serialized_start=1279
-  _STREAMINGSTATUS._serialized_end=1393
-  _BACKBONESTATUS._serialized_start=1396
-  _BACKBONESTATUS._serialized_end=1614
-  _CONFIGANDSTATUS._serialized_start=1617
-  _CONFIGANDSTATUS._serialized_end=1946
-  _CONFIGRECORDING._serialized_start=1948
-  _CONFIGRECORDING._serialized_end=2051
-  _DIOMODEEVENTSREQUEST._serialized_start=2053
-  _DIOMODEEVENTSREQUEST._serialized_end=2139
-  _DIOMODEMANUALREQUEST._serialized_start=2141
-  _DIOMODEMANUALREQUEST._serialized_end=2195
-  _DIGITALOUTCHANNELREGISTER._serialized_start=2197
-  _DIGITALOUTCHANNELREGISTER._serialized_end=2312
-  _DIGITALOUTREGISTER._serialized_start=2314
-  _DIGITALOUTREGISTER._serialized_end=2427
-  _DACGAINREQUEST._serialized_start=2429
-  _DACGAINREQUEST._serialized_end=2459
-  _DACHIGHPASSREGISTER._serialized_start=2461
-  _DACHIGHPASSREGISTER._serialized_end=2518
-  _ANALOGOUTCHANNELREGISTER._serialized_start=2520
-  _ANALOGOUTCHANNELREGISTER._serialized_end=2639
-  _ANALOGOUTREGISTER._serialized_start=2642
-  _ANALOGOUTREGISTER._serialized_end=2786
-  _SERIALNUMBER._serialized_start=2788
-  _SERIALNUMBER._serialized_end=2821
-  _SETSIMPORTSREQUEST._serialized_start=2824
-  _SETSIMPORTSREQUEST._serialized_end=2953
-  _SETSIMPORTSREQUEST_SIMPORT._serialized_start=2899
-  _SETSIMPORTSREQUEST_SIMPORT._serialized_end=2953
-  _SETHASGPIOEXPANDERREQUEST._serialized_start=2955
-  _SETHASGPIOEXPANDERREQUEST._serialized_end=3007
-  _SETMUXCHANNELREQUEST._serialized_start=3009
-  _SETMUXCHANNELREQUEST._serialized_end=3048
-  _SETPOTVOLTAGEREQUEST._serialized_start=3050
-  _SETPOTVOLTAGEREQUEST._serialized_end=3089
-  _GETADCLEVELREPLY._serialized_start=3091
-  _GETADCLEVELREPLY._serialized_end=3124
-  _SETPOTRANGEREQUEST._serialized_start=3126
-  _SETPOTRANGEREQUEST._serialized_end=3161
-  _SETPOTMODEREQUEST._serialized_start=3163
-  _SETPOTMODEREQUEST._serialized_end=3196
-  _SETPOTCELLENABLEREQUEST._serialized_start=3198
-  _SETPOTCELLENABLEREQUEST._serialized_end=3239
-  _READWIREOUTREQUEST._serialized_start=3241
-  _READWIREOUTREQUEST._serialized_end=3285
-  _READWIREOUTREPLY._serialized_start=3287
-  _READWIREOUTREPLY._serialized_end=3327
-  _LOGSYSCONFIGREPLY._serialized_start=3330
-  _LOGSYSCONFIGREPLY._serialized_end=3657
-  _PORTINFO._serialized_start=3659
-  _PORTINFO._serialized_end=3748
-  _LOGSYSSTATUSREPLY._serialized_start=3750
-  _LOGSYSSTATUSREPLY._serialized_end=3849
-  _RECORDERSTATUS._serialized_start=3852
-  _RECORDERSTATUS._serialized_end=4038
-  _SYSTEMSTATUS._serialized_start=4041
-  _SYSTEMSTATUS._serialized_end=4447
-  _LOGSYSPCACHEREPLY._serialized_start=4450
-  _LOGSYSPCACHEREPLY._serialized_end=4794
-  _TRIGGERMODESTATE._serialized_start=4796
-  _TRIGGERMODESTATE._serialized_end=4849
-  _LOADALLMOSIREQUEST._serialized_start=4851
-  _LOADALLMOSIREQUEST._serialized_end=4893
-  _TRANSMITMOSIREQUEST._serialized_start=4895
-  _TRANSMITMOSIREQUEST._serialized_end=4916
-  _DUMPMISOREQUEST._serialized_start=4918
-  _DUMPMISOREQUEST._serialized_end=4971
-  _SINAPSSTATUSREGISTERS._serialized_start=4974
-  _SINAPSSTATUSREGISTERS._serialized_end=5428
-  _FLASHSINAPSREQUEST._serialized_start=5430
-  _FLASHSINAPSREQUEST._serialized_end=5467
-  _HALDASHBOARD._serialized_start=5469
-  _HALDASHBOARD._serialized_end=5520
-  _STIMPARAMS._serialized_start=5523
-  _STIMPARAMS._serialized_end=6351
-  _STIMPARAMSREPLY._serialized_start=6354
-  _STIMPARAMSREPLY._serialized_end=6491
-  _STIMPARAMSREPLY_PARAMSENTRY._serialized_start=6426
-  _STIMPARAMSREPLY_PARAMSENTRY._serialized_end=6491
-  _MANUALSTIMTRIGGERREQUEST._serialized_start=6493
-  _MANUALSTIMTRIGGERREQUEST._serialized_end=6555
-  _MANUALSTIMTRIGGERTOGGLEREQUEST._serialized_start=6557
-  _MANUALSTIMTRIGGERTOGGLEREQUEST._serialized_end=6606
-  _STIMSTEPMESSAGE._serialized_start=6608
-  _STIMSTEPMESSAGE._serialized_end=6661
-  _ALLEGOCORE._serialized_start=8097
-  _ALLEGOCORE._serialized_end=13535
-  _PCACHE1._serialized_start=13538
-  _PCACHE1._serialized_end=13894
-  _KPI1._serialized_start=13897
-  _KPI1._serialized_end=14422
-  _NEURONS1._serialized_start=14425
-  _NEURONS1._serialized_end=15740
+  _SETRECORDREQUEST._serialized_end=713
+  _SETCONFIGCOREREQUEST._serialized_start=715
+  _SETCONFIGCOREREQUEST._serialized_end=841
+  _CABLELENGTH._serialized_start=843
+  _CABLELENGTH._serialized_end=905
+  _CABLELENGTHS._serialized_start=907
+  _CABLELENGTHS._serialized_end=1009
+  _CONFIGCORE._serialized_start=1012
+  _CONFIGCORE._serialized_end=1189
+  _RECORDINGSTATUS._serialized_start=1192
+  _RECORDINGSTATUS._serialized_end=1666
+  _STREAMINGSTATUS._serialized_start=1668
+  _STREAMINGSTATUS._serialized_end=1782
+  _BACKBONESTATUS._serialized_start=1785
+  _BACKBONESTATUS._serialized_end=2003
+  _CONFIGANDSTATUS._serialized_start=2006
+  _CONFIGANDSTATUS._serialized_end=2335
+  _CONFIGRECORDING._serialized_start=2338
+  _CONFIGRECORDING._serialized_end=2496
+  _DIOMODEEVENTSREQUEST._serialized_start=2498
+  _DIOMODEEVENTSREQUEST._serialized_end=2584
+  _DIOMODEMANUALREQUEST._serialized_start=2586
+  _DIOMODEMANUALREQUEST._serialized_end=2640
+  _DIGITALOUTCHANNELREGISTER._serialized_start=2642
+  _DIGITALOUTCHANNELREGISTER._serialized_end=2757
+  _DIGITALOUTREGISTER._serialized_start=2759
+  _DIGITALOUTREGISTER._serialized_end=2872
+  _DACGAINREQUEST._serialized_start=2874
+  _DACGAINREQUEST._serialized_end=2904
+  _DACHIGHPASSREGISTER._serialized_start=2906
+  _DACHIGHPASSREGISTER._serialized_end=2963
+  _ANALOGOUTCHANNELREGISTER._serialized_start=2965
+  _ANALOGOUTCHANNELREGISTER._serialized_end=3084
+  _ANALOGOUTREGISTER._serialized_start=3087
+  _ANALOGOUTREGISTER._serialized_end=3231
+  _SERIALNUMBER._serialized_start=3233
+  _SERIALNUMBER._serialized_end=3266
+  _SETSIMPORTSREQUEST._serialized_start=3269
+  _SETSIMPORTSREQUEST._serialized_end=3398
+  _SETSIMPORTSREQUEST_SIMPORT._serialized_start=3344
+  _SETSIMPORTSREQUEST_SIMPORT._serialized_end=3398
+  _SETHASGPIOEXPANDERREQUEST._serialized_start=3400
+  _SETHASGPIOEXPANDERREQUEST._serialized_end=3452
+  _SETMUXCHANNELREQUEST._serialized_start=3454
+  _SETMUXCHANNELREQUEST._serialized_end=3493
+  _SETPOTVOLTAGEREQUEST._serialized_start=3495
+  _SETPOTVOLTAGEREQUEST._serialized_end=3534
+  _GETADCLEVELREPLY._serialized_start=3536
+  _GETADCLEVELREPLY._serialized_end=3569
+  _SETPOTRANGEREQUEST._serialized_start=3571
+  _SETPOTRANGEREQUEST._serialized_end=3606
+  _SETPOTMODEREQUEST._serialized_start=3608
+  _SETPOTMODEREQUEST._serialized_end=3641
+  _SETPOTCELLENABLEREQUEST._serialized_start=3643
+  _SETPOTCELLENABLEREQUEST._serialized_end=3684
+  _READWIREOUTREQUEST._serialized_start=3686
+  _READWIREOUTREQUEST._serialized_end=3730
+  _READWIREOUTREPLY._serialized_start=3732
+  _READWIREOUTREPLY._serialized_end=3772
+  _LOGSYSCONFIGREPLY._serialized_start=3775
+  _LOGSYSCONFIGREPLY._serialized_end=4102
+  _PORTINFO._serialized_start=4104
+  _PORTINFO._serialized_end=4193
+  _LOGSYSSTATUSREPLY._serialized_start=4195
+  _LOGSYSSTATUSREPLY._serialized_end=4294
+  _RECORDERSTATUS._serialized_start=4297
+  _RECORDERSTATUS._serialized_end=4483
+  _SYSTEMSTATUS._serialized_start=4486
+  _SYSTEMSTATUS._serialized_end=4892
+  _LOGSYSPCACHEREPLY._serialized_start=4895
+  _LOGSYSPCACHEREPLY._serialized_end=5239
+  _SETTRIGGERREQUEST._serialized_start=5241
+  _SETTRIGGERREQUEST._serialized_end=5346
+  _TRIGGERSTATE._serialized_start=5348
+  _TRIGGERSTATE._serialized_end=5440
+  _LOADALLMOSIREQUEST._serialized_start=5442
+  _LOADALLMOSIREQUEST._serialized_end=5484
+  _TRANSMITMOSIREQUEST._serialized_start=5486
+  _TRANSMITMOSIREQUEST._serialized_end=5507
+  _DUMPMISOREQUEST._serialized_start=5509
+  _DUMPMISOREQUEST._serialized_end=5562
+  _SINAPSSTATUSREGISTERS._serialized_start=5565
+  _SINAPSSTATUSREGISTERS._serialized_end=6019
+  _FLASHSINAPSREQUEST._serialized_start=6021
+  _FLASHSINAPSREQUEST._serialized_end=6058
+  _HALDASHBOARD._serialized_start=6060
+  _HALDASHBOARD._serialized_end=6111
+  _STIMPARAMS._serialized_start=6114
+  _STIMPARAMS._serialized_end=6942
+  _STIMPARAMSREPLY._serialized_start=6945
+  _STIMPARAMSREPLY._serialized_end=7082
+  _STIMPARAMSREPLY_PARAMSENTRY._serialized_start=7017
+  _STIMPARAMSREPLY_PARAMSENTRY._serialized_end=7082
+  _MANUALSTIMTRIGGERREQUEST._serialized_start=7084
+  _MANUALSTIMTRIGGERREQUEST._serialized_end=7146
+  _MANUALSTIMTRIGGERTOGGLEREQUEST._serialized_start=7148
+  _MANUALSTIMTRIGGERTOGGLEREQUEST._serialized_end=7197
+  _STIMSTEPMESSAGE._serialized_start=7199
+  _STIMSTEPMESSAGE._serialized_end=7252
+  _ALLEGOCORE._serialized_start=8854
+  _ALLEGOCORE._serialized_end=14291
+  _PCACHE1._serialized_start=14294
+  _PCACHE1._serialized_end=14650
+  _KPI1._serialized_start=14653
+  _KPI1._serialized_end=15178
+  _NEURONS1._serialized_start=15181
+  _NEURONS1._serialized_end=16496
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-3.0.0b4/radiens/grpc_radiens/allegoserver_pb2_grpc.py` & `radiens-3.0.0b5/radiens/grpc_radiens/allegoserver_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,17 +129,17 @@
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.SetMuxChannel = channel.unary_unary(
                 '/allego.AllegoCore/SetMuxChannel',
                 request_serializer=allegoserver__pb2.SetMuxChannelRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
-        self.SetTriggerMode = channel.unary_unary(
-                '/allego.AllegoCore/SetTriggerMode',
-                request_serializer=allegoserver__pb2.TriggerModeState.SerializeToString,
+        self.SetTriggerState = channel.unary_unary(
+                '/allego.AllegoCore/SetTriggerState',
+                request_serializer=allegoserver__pb2.SetTriggerRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.SetPotVoltage = channel.unary_unary(
                 '/allego.AllegoCore/SetPotVoltage',
                 request_serializer=allegoserver__pb2.SetPotVoltageRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
@@ -244,18 +244,18 @@
                 response_deserializer=allegoserver__pb2.AnalogOutRegister.FromString,
                 )
         self.GetSerial = channel.unary_unary(
                 '/allego.AllegoCore/GetSerial',
                 request_serializer=common__pb2.StandardRequest.SerializeToString,
                 response_deserializer=allegoserver__pb2.SerialNumber.FromString,
                 )
-        self.GetTriggerMode = channel.unary_unary(
-                '/allego.AllegoCore/GetTriggerMode',
+        self.GetTriggerState = channel.unary_unary(
+                '/allego.AllegoCore/GetTriggerState',
                 request_serializer=common__pb2.StandardRequest.SerializeToString,
-                response_deserializer=allegoserver__pb2.TriggerModeState.FromString,
+                response_deserializer=allegoserver__pb2.TriggerState.FromString,
                 )
         self.GetADCLevel = channel.unary_unary(
                 '/allego.AllegoCore/GetADCLevel',
                 request_serializer=common__pb2.StandardRequest.SerializeToString,
                 response_deserializer=allegoserver__pb2.GetADCLevelReply.FromString,
                 )
         self.ReadWireOut = channel.unary_unary(
@@ -535,15 +535,15 @@
 
     def SetMuxChannel(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SetTriggerMode(self, request, context):
+    def SetTriggerState(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SetPotVoltage(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -674,15 +674,15 @@
 
     def GetSerial(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetTriggerMode(self, request, context):
+    def GetTriggerState(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetADCLevel(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -971,17 +971,17 @@
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'SetMuxChannel': grpc.unary_unary_rpc_method_handler(
                     servicer.SetMuxChannel,
                     request_deserializer=allegoserver__pb2.SetMuxChannelRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
-            'SetTriggerMode': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetTriggerMode,
-                    request_deserializer=allegoserver__pb2.TriggerModeState.FromString,
+            'SetTriggerState': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetTriggerState,
+                    request_deserializer=allegoserver__pb2.SetTriggerRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'SetPotVoltage': grpc.unary_unary_rpc_method_handler(
                     servicer.SetPotVoltage,
                     request_deserializer=allegoserver__pb2.SetPotVoltageRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
@@ -1086,18 +1086,18 @@
                     response_serializer=allegoserver__pb2.AnalogOutRegister.SerializeToString,
             ),
             'GetSerial': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSerial,
                     request_deserializer=common__pb2.StandardRequest.FromString,
                     response_serializer=allegoserver__pb2.SerialNumber.SerializeToString,
             ),
-            'GetTriggerMode': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetTriggerMode,
+            'GetTriggerState': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetTriggerState,
                     request_deserializer=common__pb2.StandardRequest.FromString,
-                    response_serializer=allegoserver__pb2.TriggerModeState.SerializeToString,
+                    response_serializer=allegoserver__pb2.TriggerState.SerializeToString,
             ),
             'GetADCLevel': grpc.unary_unary_rpc_method_handler(
                     servicer.GetADCLevel,
                     request_deserializer=common__pb2.StandardRequest.FromString,
                     response_serializer=allegoserver__pb2.GetADCLevelReply.SerializeToString,
             ),
             'ReadWireOut': grpc.unary_unary_rpc_method_handler(
@@ -1633,26 +1633,26 @@
         return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/SetMuxChannel',
             allegoserver__pb2.SetMuxChannelRequest.SerializeToString,
             common__pb2.StandardReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SetTriggerMode(request,
+    def SetTriggerState(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/SetTriggerMode',
-            allegoserver__pb2.TriggerModeState.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/SetTriggerState',
+            allegoserver__pb2.SetTriggerRequest.SerializeToString,
             common__pb2.StandardReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SetPotVoltage(request,
             target,
@@ -2024,27 +2024,27 @@
         return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/GetSerial',
             common__pb2.StandardRequest.SerializeToString,
             allegoserver__pb2.SerialNumber.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetTriggerMode(request,
+    def GetTriggerState(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/GetTriggerMode',
+        return grpc.experimental.unary_unary(request, target, '/allego.AllegoCore/GetTriggerState',
             common__pb2.StandardRequest.SerializeToString,
-            allegoserver__pb2.TriggerModeState.FromString,
+            allegoserver__pb2.TriggerState.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetADCLevel(request,
             target,
             options=(),
```

### Comparing `radiens-3.0.0b4/radiens/grpc_radiens/biointerface_pb2.py` & `radiens-3.0.0b5/radiens/grpc_radiens/biointerface_pb2.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/grpc_radiens/common_pb2.py` & `radiens-3.0.0b5/radiens/grpc_radiens/common_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x06\x61llego\x1a\x1fgoogle/protobuf/timestamp.proto\"@\n\x14OfflineLicenseStatus\x12\x12\n\nisVerified\x18\x01 \x02(\x08\x12\x14\n\x0chardwareUUID\x18\x02 \x02(\t\"C\n\x0f\x46irmwareVersion\x12\x0c\n\x04\x64\x61te\x18\x01 \x02(\t\x12\x10\n\x08majorRev\x18\x02 \x02(\x05\x12\x10\n\x08minorRev\x18\x03 \x02(\x05\"k\n\x10RadixEnvironment\x12\x0f\n\x07version\x18\x01 \x02(\t\x12\x14\n\x0cuserDataPath\x18\x02 \x02(\t\x12\x30\n\x0f\x66irmwareVersion\x18\x03 \x02(\x0b\x32\x17.allego.FirmwareVersion\"!\n\x0fStandardRequest\x12\x0e\n\x06regStr\x18\x02 \x03(\t\"/\n\rStandardReply\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\x12\x0e\n\x06regStr\x18\x02 \x03(\t\"&\n\rDACOffRequest\x12\x15\n\rstreamGroupId\x18\x01 \x01(\t\"\xba\x01\n\x13WorkspaceDescriptor\x12\n\n\x02iD\x18\x01 \x02(\t\x12!\n\x03\x61pp\x18\x02 \x02(\x0e\x32\x14.allego.WorkspaceApp\x12\x12\n\nisModified\x18\x03 \x02(\x08\x12\x19\n\x11timestampLastUsed\x18\x04 \x02(\t\x12\x19\n\x11timestampModified\x18\x05 \x02(\t\x12*\n\nannotation\x18\x06 \x02(\x0b\x32\x16.allego.AnnotateBundle\"\xb8\x01\n\x17WorkspaceControlRequest\x12&\n\x03\x63md\x18\x01 \x02(\x0e\x32\x19.allego.WorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12*\n\nannotation\x18\x03 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x1a\n\x12targetFullFileName\x18\x04 \x01(\t\x12\x18\n\x10isForceOverwrite\x18\x05 \x01(\x08\"\xd3\x01\n\x13GetWorkspaceRequest\x12)\n\x03\x63md\x18\x01 \x02(\x0e\x32\x1c.allego.GetWorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12\x14\n\x0cworkspaceDir\x18\x03 \x01(\t\x12%\n\x07\x61ppMask\x18\x04 \x01(\x0e\x32\x14.allego.WorkspaceApp\x12,\n\x0c\x61nnotateMask\x18\x05 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x11\n\tisBrowser\x18\x06 \x01(\x08\"\xab\x01\n\x11GetWorkspaceReply\x12\x43\n\rworkspaceDesc\x18\x01 \x03(\x0b\x32,.allego.GetWorkspaceReply.WorkspaceDescEntry\x1aQ\n\x12WorkspaceDescEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x1b.allego.WorkspaceDescriptor:\x02\x38\x01\"`\n\x18GetRadiensServersRequest\x12\x15\n\rhostIPaddress\x18\x01 \x02(\t\x12-\n\nserverType\x18\x02 \x01(\x0e\x32\x19.allego.RadiensServerType\"\x97\x02\n\nServerSpec\x12\x0c\n\x04host\x18\x01 \x02(\t\x12\x0b\n\x03pid\x18\x02 \x02(\x05\x12\x30\n\x07service\x18\x03 \x03(\x0b\x32\x1f.allego.ServerSpec.ServiceEntry\x12\x30\n\x05spawn\x18\x04 \x01(\x0b\x32!.allego.ServerSpec.SpawnedProcess\x1a\x1b\n\x0bGrpcService\x12\x0c\n\x04port\x18\x01 \x02(\x05\x1a\x1d\n\x0eSpawnedProcess\x12\x0b\n\x03pid\x18\x01 \x03(\x05\x1aN\n\x0cServiceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.allego.ServerSpec.GrpcService:\x02\x38\x01\"j\n\x13RadiensServersReply\x12(\n\x0c\x61llegoserver\x18\x01 \x03(\x0b\x32\x12.allego.ServerSpec\x12)\n\rradiensserver\x18\x02 \x03(\x0b\x32\x12.allego.ServerSpec\"-\n\x14SignalGroupIDRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\"\xc4\x01\n\tSignalMap\x12\x0f\n\x07siteIdx\x18\x01 \x03(\x05\x12\x13\n\x0b\x63ompSiteNum\x18\x02 \x03(\t\x12\x13\n\x0bposProbeUmX\x18\x03 \x03(\x01\x12\x13\n\x0bposProbeUmY\x18\x04 \x03(\x01\x12\x13\n\x0bposProbeUmZ\x18\x05 \x03(\x01\x12\x14\n\x0cposTissueUmX\x18\x06 \x03(\x01\x12\x14\n\x0cposTissueUmY\x18\x07 \x03(\x01\x12\x14\n\x0cposTissueUmZ\x18\x08 \x03(\x01\x12\x10\n\x08sensorID\x18\t \x03(\t\"=\n\x10GPIOChannelCount\x12\x0c\n\x04nAux\x18\x01 \x02(\x05\x12\x0c\n\x04nDin\x18\x02 \x02(\x05\x12\r\n\x05nDout\x18\x03 \x02(\x05\"D\n\x10PortChannelCount\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"Q\n\x0eSetPortRequest\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x10\n\x08probeUID\x18\x02 \x02(\t\x12\x11\n\thstageUID\x18\x03 \x02(\t\"\xe2\x02\n\x11HDSnapshotRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12=\n\npriSignals\x18\x03 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\nauxSignals\x18\x04 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\ndinSignals\x18\x05 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12>\n\x0b\x64outSignals\x18\x06 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x1a&\n\x0fSelectedSignals\x12\x13\n\x0bntvChanIdxs\x18\x01 \x03(\x05\"\x96\x01\n\x12HDSnapshotRequest2\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12)\n\x07selMode\x18\x03 \x01(\x0e\x32\x18.allego.TimeRangeSelMode\x12#\n\x06sigSel\x18\x04 \x01(\x0b\x32\x13.allego.SigSelector\"L\n\x15RadiensPyGraphicsArgs\x12\x12\n\ngraphicsID\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0f\n\x07\x66igSize\x18\x03 \x03(\x03\"\xdd\x02\n\nPSDRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12)\n\x07selMode\x18\x03 \x02(\x0e\x32\x18.allego.TimeRangeSelMode\x12!\n\x05stype\x18\x04 \x02(\x0e\x32\x12.allego.SignalType\x12\x0f\n\x07ntvIdxs\x18\x05 \x03(\x03\x12\x12\n\nresampleFs\x18\x06 \x01(\x01\x12&\n\x07wdwType\x18\x07 \x01(\x0e\x32\x15.allego.PSDWindowType\x12#\n\x07scaling\x18\x08 \x01(\x0e\x32\x12.allego.PSDScaling\x12\x11\n\tfreqRange\x18\t \x03(\x01\x12\x14\n\x0c\x63ollapseFreq\x18\n \x01(\x08\x12\x11\n\tdeltaFreq\x18\x0b \x01(\x01\x12\x0c\n\x04path\x18\r \x01(\t\x12\x13\n\x0bisReturnPSD\x18\x0e \x01(\x08\"\xa1\x02\n\x03PSD\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12\x1f\n\x02sG\x18\x03 \x02(\x0b\x32\x13.allego.SignalGroup\x12!\n\x05stype\x18\x04 \x02(\x0e\x32\x12.allego.SignalType\x12\x1d\n\x02tR\x18\x05 \x02(\x0b\x32\x11.allego.TimeRange\x12 \n\x03psd\x18\x06 \x02(\x0b\x32\x13.allego.DenseMatrix\x12\x0c\n\x04\x66req\x18\x07 \x03(\x01\x12\x14\n\x0c\x66reqBinWidth\x18\x08 \x02(\x01\x12\x11\n\tfreqRange\x18\x0b \x03(\x01\x12&\n\x07wdwType\x18\t \x01(\x0e\x32\x15.allego.PSDWindowType\x12#\n\x07scaling\x18\n \x01(\x0e\x32\x12.allego.PSDScaling\"e\n\x18RadiensPyGraphicsRequest\x12\x1c\n\x07psdData\x18\x01 \x01(\x0b\x32\x0b.allego.PSD\x12+\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\x1d.allego.RadiensPyGraphicsArgs\"^\n\x0bSigSelector\x12\x12\n\nampNtvIdxs\x18\x01 \x03(\x03\x12\x12\n\nainNtvIdxs\x18\x02 \x03(\x03\x12\x12\n\ndinNtvIdxs\x18\x03 \x03(\x03\x12\x13\n\x0b\x64outNtvIdxs\x18\x04 \x03(\x03\"]\n\x0eHDSnapshotMeta\x12\x11\n\tglobalMin\x18\x04 \x02(\x01\x12\x11\n\tglobalMax\x18\x05 \x02(\x01\x12%\n\x08sigGroup\x18\x06 \x01(\x0b\x32\x13.allego.SignalGroup\"\x9f\x02\n\nHDSnapshot\x12$\n\x04meta\x18\x01 \x02(\x0b\x32\x16.allego.HDSnapshotMeta\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x13\n\x0btimeSamples\x18\x03 \x02(\x0c\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12&\n\npriSignals\x18\x05 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\nauxSignals\x18\x06 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\ndinSignals\x18\x07 \x01(\x0b\x32\x12.allego.RawSignals\x12\'\n\x0b\x64outSignals\x18\x08 \x01(\x0b\x32\x12.allego.RawSignals\"@\n\x0bHDSnapshot2\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12\x1e\n\x04sigs\x18\x02 \x02(\x0b\x32\x10.allego.Signals2\"\xb9\x03\n\x11GetSignalsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x37\n\x06params\x18\x02 \x02(\x0b\x32\'.allego.GetSignalsRequest.GetSigsParams\x1a\xd3\x02\n\rGetSigsParams\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x0e\n\x06wdwSec\x18\x02 \x02(\x01\x12\x14\n\x0c\x63hanHeightPx\x18\x03 \x02(\x01\x12\x10\n\x08\x61mpFsrUv\x18\x04 \x02(\x01\x12\x17\n\x0fplotWidthPoints\x18\x05 \x02(\x01\x12\x11\n\tgpioOnTop\x18\x06 \x02(\x08\x12\x0f\n\x07\x61inFsrV\x18\x07 \x02(\x01\x12\x13\n\x0b\x63omponentID\x18\x08 \x02(\t\x12-\n\x0cresampleType\x18\t \x02(\x0e\x32\x17.allego.ResampleRoutine\x12\x11\n\tisHeatmap\x18\n \x02(\x08\x12\x1b\n\x13isNotApplyDSPstage2\x18\x0b \x01(\x08\x12\x13\n\x0b\x63lipToRange\x18\x0c \x02(\x08\x12\x17\n\x0f\x62\x61ndpassLowFreq\x18\r \x01(\x01\x12\x18\n\x10\x62\x61ndpassHighFreq\x18\x0e \x01(\x01\"[\n\nRawSignals\x12\r\n\x05shape\x18\x01 \x03(\x05\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\x12\x1d\n\x02tR\x18\x04 \x01(\x0b\x32\x11.allego.TimeRange\"\xe7\x01\n\x08Signals2\x12\x1f\n\x02sG\x18\x01 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12%\n\x03\x61mp\x18\x03 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12%\n\x03\x61in\x18\x04 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12%\n\x03\x64in\x18\x05 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12&\n\x04\x64out\x18\x06 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\"\x85\x02\n\x14ListSensorSpecsReply\x12\x41\n\x06probes\x18\x01 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\x45\n\nheadstages\x18\x02 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x1a:\n\x14SpecWithChannelCount\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"d\n\x16ListDataSourcesRequest\x12\x11\n\tdirectory\x18\x01 \x02(\t\x12&\n\x06sortBy\x18\x02 \x01(\x0e\x32\x16.allego.DataSourceSort\x12\x0f\n\x07\x64irList\x18\x03 \x03(\t\"\x1c\n\x07SortMap\x12\x11\n\tsorterIds\x18\x01 \x03(\t\">\n\x16GetSignalGroupIDsReply\x12\x12\n\ncontinuous\x18\x01 \x03(\t\x12\x10\n\x08\x64iscrete\x18\x02 \x03(\t\"\xa0\x01\n\x13GetSorterIDMapReply\x12\x43\n\x0csigToSortMap\x18\x01 \x03(\x0b\x32-.allego.GetSorterIDMapReply.SigToSortMapEntry\x1a\x44\n\x11SigToSortMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.allego.SortMap:\x02\x38\x01\"\xaf\x01\n\nDataSource\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x02(\t\x12\x17\n\x0f\x64urationSeconds\x18\x03 \x02(\x01\x12\x17\n\x0f\x64urationMinutes\x18\x04 \x02(\x01\x12\x15\n\rdurationHours\x18\x05 \x02(\x01\x12(\n\x08\x66ileType\x18\x06 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x12\n\nnumSignals\x18\x07 \x02(\x05\"o\n\x0e\x46ileDescriptor\x12\x0c\n\x04path\x18\x01 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x13\n\x0b\x66ileNameUID\x18\x04 \x01(\t\"\xd0\x01\n\x08TimeSpec\x12\x30\n\ttimeRange\x18\x01 \x01(\x0b\x32\x1b.allego.TimeSpec.TimeRangeLH\x00\x12:\n\x0etimestampRange\x18\x02 \x01(\x0b\x32 .allego.TimeSpec.TimestampRangeLH\x00\x1a\x1f\n\nTimeRangeL\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x1a)\n\x0fTimestampRangeL\x12\x16\n\x0etimestampRange\x18\x01 \x03(\x03\x42\n\n\x08timeDesc\"\xbe\x01\n\nSignalSpec\x12.\n\x07siteNum\x18\x01 \x01(\x0b\x32\x1b.allego.SignalSpec.SiteNumLH\x00\x12\x34\n\nntvChanIdx\x18\x02 \x01(\x0b\x32\x1e.allego.SignalSpec.NtvChanIdxLH\x00\x1a\x1b\n\x08SiteNumL\x12\x0f\n\x07siteNum\x18\x01 \x03(\x05\x1a!\n\x0bNtvChanIdxL\x12\x12\n\nntvChanIdx\x18\x01 \x03(\x05\x42\n\n\x08siteDesc\"\x8c\x06\n\rChannelRecord\x12\x10\n\x08\x63hanName\x18\x01 \x02(\t\x12$\n\x08\x63hanType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\x12\n\nntvChanIdx\x18\x03 \x02(\x05\x12\x0f\n\x07siteNum\x18\x04 \x02(\x05\x12\x15\n\rcolorGroupIdx\x18\x05 \x02(\x05\x12\x12\n\nisSelected\x18\x06 \x02(\x08\x12\x13\n\x0bisAudioLeft\x18\x07 \x02(\x08\x12\x1a\n\x04port\x18\x08 \x02(\x0e\x32\x0c.allego.Port\x12\x11\n\tsiteShape\x18\t \x02(\t\x12\x10\n\x08siteCtrX\x18\n \x02(\x01\x12\x10\n\x08siteCtrY\x18\x0b \x02(\x01\x12\x10\n\x08siteCtrZ\x18\x0c \x02(\x01\x12\x13\n\x0bsiteLimXMin\x18\r \x02(\x01\x12\x13\n\x0bsiteLimXMax\x18\x0e \x02(\x01\x12\x13\n\x0bsiteLimYMin\x18\x0f \x02(\x01\x12\x13\n\x0bsiteLimYMax\x18\x10 \x02(\x01\x12\x13\n\x0bsiteLimZMin\x18\x11 \x02(\x01\x12\x13\n\x0bsiteLimZMax\x18\x12 \x02(\x01\x12\x13\n\x0bsiteCtrTcsX\x18\x13 \x02(\x01\x12\x13\n\x0bsiteCtrTcsY\x18\x14 \x02(\x01\x12\x13\n\x0bsiteCtrTcsZ\x18\x15 \x02(\x01\x12\x13\n\x0bsensorUnits\x18\x16 \x02(\t\x12\x0e\n\x06\x61\x62sIdx\x18\x17 \x02(\x05\x12\x14\n\x0cisAudioRight\x18\x18 \x02(\x08\x12\x12\n\nsysChanIdx\x18\x19 \x02(\x05\x12\x17\n\x0fsiteAreaMicron2\x18\x1a \x01(\x01\x12\x11\n\tscsToTcsX\x18\x1b \x01(\x01\x12\x11\n\tscsToTcsY\x18\x1c \x01(\x01\x12\x11\n\tscsToTcsZ\x18\x1d \x01(\x01\x12\x10\n\x08sensorID\x18\x1e \x01(\t\x12\x0f\n\x07probeID\x18\x1f \x01(\t\x12\x13\n\x0bheadstageID\x18  \x01(\t\x12\x13\n\x0b\x64\x61tasetRidx\x18! \x01(\x05\x12\x13\n\x0b\x64\x61tasetAidx\x18\" \x01(\x05\x12\x13\n\x0bntvChanName\x18# \x01(\t\x12\x11\n\tsensorUID\x18$ \x01(\t\x12\x11\n\tsensorIdx\x18% \x01(\x05\"\x1f\n\x07XYCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"+\n\x08XYZCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\x12\t\n\x01z\x18\x03 \x02(\x01\"\x81\x03\n\x06Sensor\x12\x0f\n\x07probeId\x18\x01 \x02(\t\x12\x13\n\x0bheadstageId\x18\x02 \x02(\t\x12+\n\twireframe\x18\x03 \x02(\x0b\x32\x18.allego.Sensor.WireFrame\x12\x0c\n\x04xMin\x18\x04 \x02(\x01\x12\x0c\n\x04xMax\x18\x05 \x02(\x01\x12\x0c\n\x04yMin\x18\x06 \x02(\x01\x12\x0c\n\x04yMax\x18\x07 \x02(\x01\x12+\n\x08position\x18\x08 \x02(\x0b\x32\x19.allego.SensorPositionTcs\x12\x11\n\tsensorUID\x18\t \x01(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\n \x01(\x05\x12\x10\n\x08numSites\x18\x0b \x02(\x05\x12\x11\n\tsensorIdx\x18\x0c \x01(\x05\x1am\n\tWireFrame\x12\x1c\n\x03vtx\x18\x01 \x03(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxXlim\x18\x02 \x02(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxYlim\x18\x03 \x02(\x0b\x32\x0f.allego.XYCoord\"\x98\x02\n\x0eSensorPortSpec\x12\x1f\n\x07sensorA\x18\x01 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorB\x18\x02 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorC\x18\x03 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorD\x18\x04 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorE\x18\x05 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorF\x18\x06 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorG\x18\x07 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorH\x18\x08 \x03(\x0b\x32\x0e.allego.Sensor\"t\n\x10SignalGroupUnits\x12\x32\n\x05units\x18\x01 \x03(\x0b\x32#.allego.SignalGroupUnits.UnitsEntry\x1a,\n\nUnitsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\x80\x02\n\x0bSignalGroup\x12\'\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x15.allego.ChannelRecord\x12.\n\x0esensorPortSpec\x18\x02 \x02(\x0b\x32\x16.allego.SensorPortSpec\x12\x12\n\ndatasetUID\x18\x03 \x01(\t\x12\x10\n\x08sampFreq\x18\x04 \x01(\x01\x12\x13\n\x0bsourceLabel\x18\x05 \x01(\t\x12\x19\n\x11neighborMaxRadius\x18\x06 \x01(\x01\x12-\n\x0bsignalUnits\x18\x07 \x01(\x0b\x32\x18.allego.SignalGroupUnits\x12\x13\n\x0bhasDiscrete\x18\x08 \x01(\x08\"\x87\x01\n\x18\x43reateSignalGroupRequest\x12\x16\n\x0e\x64\x61taSourceName\x18\x01 \x02(\t\x12\x16\n\x0e\x64\x61taSourcePath\x18\x02 \x02(\t\x12$\n\x04type\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x15\n\rstreamGroupId\x18\x04 \x02(\t\"s\n\tSubOpSort\x12)\n\x04sort\x18\x01 \x03(\x0e\x32\x1b.allego.SubOpSort.SortField\";\n\tSortField\x12\x0e\n\nSITE_CTR_X\x10\x00\x12\x0e\n\nSITE_CTR_Y\x10\x01\x12\x0e\n\nSITE_CTR_Z\x10\x02\"\xa5\x03\n\x18UpdateSignalGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12=\n\toperation\x18\x02 \x02(\x0e\x32*.allego.UpdateSignalGroupRequest.Operation\x12\x42\n\taddRemove\x18\x03 \x01(\x0e\x32-.allego.UpdateSignalGroupRequest.SubOperationH\x00\x12#\n\x06sortOp\x18\x04 \x01(\x0b\x32\x11.allego.SubOpSortH\x00\x12\x16\n\nntvChanIdx\x18\x05 \x03(\x05\x42\x02\x10\x01\x12&\n\nsignalType\x18\x06 \x02(\x0e\x32\x12.allego.SignalType\x12\x11\n\tpropagate\x18\x07 \x01(\x08\"B\n\tOperation\x12\t\n\x05\x43OLOR\x10\x00\x12\n\n\x06SELECT\x10\x01\x12\x14\n\x10\x44\x45PRECATED_AUDIO\x10\x02\x12\x08\n\x04SORT\x10\x03\"#\n\x0cSubOperation\x12\x07\n\x03\x41\x44\x44\x10\x00\x12\n\n\x06REMOVE\x10\x01\x42\x0e\n\x0csubOperation\"T\n\x14SliceSignalGroupSpec\x12\x0e\n\x06sortBy\x18\x01 \x02(\t\x12\r\n\x05\x64\x65lim\x18\x02 \x02(\t\x12\x1d\n\x02tR\x18\x03 \x01(\x0b\x32\x11.allego.TimeRange\"X\n\x17SliceSignalGroupRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12*\n\x04spec\x18\x02 \x02(\x0b\x32\x1c.allego.SliceSignalGroupSpec\"\x88\x01\n\x15SliceSignalGroupReply\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12*\n\x04spec\x18\x02 \x02(\x0b\x32\x1c.allego.SliceSignalGroupSpec\x12\x1f\n\x02sG\x18\x03 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x0f\n\x07outcome\x18\x04 \x02(\t\"\x0f\n\rLicenseStatus\"u\n\x12SetDSPGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12$\n\tdspParams\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"\xf2\x02\n\tDSPParams\x12\x1d\n\x04type\x18\x01 \x02(\x0e\x32\x0f.allego.DSPType\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12\x0e\n\x04\x66req\x18\x03 \x01(\x01H\x00\x12\x36\n\x0c\x66reqSpecBand\x18\x04 \x01(\x0b\x32\x1e.allego.DSPParams.FreqSpecBandH\x00\x12\x17\n\rrefNtvChanIdx\x18\x08 \x01(\x05H\x00\x12\x16\n\x0enotchBandwidth\x18\x05 \x01(\x01\x12\x11\n\tuserLabel\x18\x06 \x02(\t\x12\x1a\n\x04port\x18\x07 \x02(\x0e\x32\x0c.allego.Port\x12\x18\n\x10targetNtvChanIdx\x18\t \x01(\x01\x12\r\n\x05isAux\x18\n \x02(\x08\x12\x12\n\nauxChanIdx\x18\x0b \x01(\x05\x1a\x31\n\x0c\x46reqSpecBand\x12\x0f\n\x07lowFreq\x18\x01 \x02(\x01\x12\x10\n\x08highFreq\x18\x02 \x02(\x01\x42\n\n\x08\x66reqSpec\"\x85\x01\n\x08\x44SPGroup\x12#\n\x08hardware\x18\x01 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage1\x18\x02 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage2\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"\x9a\x01\n\x10SetSensorRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07probeId\x18\x03 \x01(\t\x12\x13\n\x0bheadstageId\x18\x04 \x01(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\x05 \x01(\x05\x12\x13\n\x0bnumChannels\x18\x06 \x01(\x05\"m\n\x11SensorPositionTcs\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\x12\x11\n\tRingAngle\x18\x05 \x02(\x01\x12\x12\n\nAxialAngle\x18\x06 \x02(\x01\x12\x10\n\x08\x41rcAngle\x18\x07 \x02(\x01\"\x90\x01\n\x1bSetSensorPositionTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12+\n\x08position\x18\x03 \x02(\x0b\x32\x19.allego.SensorPositionTcs\x12\x11\n\tsensorIdx\x18\x04 \x01(\x05\"F\n\x0fSitePositionTcs\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\"\x7f\n\x1aSetSitePositionsTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12.\n\rsitePositions\x18\x03 \x03(\x0b\x32\x17.allego.SitePositionTcs\"Y\n\x17\x46\x65\x61tureStartStopRequest\x12\x0e\n\x06nodeId\x18\x01 \x02(\t\x12.\n\x0e\x66\x65\x61tureLicense\x18\x02 \x02(\x0e\x32\x16.allego.FeatureLicense\"!\n\x0cPrivacyReply\x12\x11\n\tisPrivate\x18\x02 \x02(\x08\"&\n\x11SetPrivacyRequest\x12\x11\n\tisPrivate\x18\x01 \x02(\x08\"7\n\x0b\x44\x65nseMatrix\x12\x0c\n\x04rows\x18\x01 \x02(\x03\x12\x0c\n\x04\x63ols\x18\x02 \x02(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\"\\\n\tHistogram\x12\r\n\x05stats\x18\x01 \x03(\x01\x12\x0e\n\x06\x63ounts\x18\x02 \x03(\x01\x12\x10\n\x08\x64ividers\x18\x03 \x03(\x01\x12\x0f\n\x07numBins\x18\x04 \x02(\x03\x12\r\n\x05isPDF\x18\x05 \x02(\x08\"Y\n\x0bKpiMetricID\x12$\n\x04mode\x18\x01 \x02(\x0e\x32\x16.allego.KpiMetricsMode\x12$\n\x04name\x18\x02 \x02(\x0e\x32\x16.allego.KpiMetricsEnum\"\x85\x01\n\tTimeRange\x12\x14\n\x0ctimeRangeSec\x18\x01 \x03(\x01\x12\x11\n\ttimestamp\x18\x02 \x03(\x03\x12\n\n\x02\x66s\x18\x03 \x02(\x01\x12\x15\n\rwallTimeStart\x18\x04 \x01(\t\x12,\n\x08wallTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"q\n\tBundleReq\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12$\n\x07metrics\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0e\n\x06isTail\x18\x05 \x02(\x08\"\x9d\x01\n\rKpiMetricsReq\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x1e\n\x03\x61rg\x18\x03 \x02(\x0b\x32\x11.allego.BundleReq\x12\x0e\n\x06isPlot\x18\x04 \x01(\x08\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x14\n\x0cisReturnData\x18\x06 \x01(\x08\"\x83\x03\n\x0eKpiMetricsData\x12\x12\n\nnumPackets\x18\x01 \x02(\x03\x12\x0f\n\x07numSigs\x18\x02 \x02(\x03\x12\x12\n\nnumMetrics\x18\x03 \x02(\x03\x12#\n\x06metric\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0f\n\x07pktIdxs\x18\x05 \x03(\x03\x12 \n\x03val\x18\x06 \x02(\x0b\x32\x13.allego.DenseMatrix\x12\x35\n\tstatsPkts\x18\x07 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x31\n\x05stats\x18\x08 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x14\n\x0cpacketDurSec\x18\t \x02(\x01\x12\x1d\n\x02tR\x18\n \x02(\x0b\x32\x11.allego.TimeRange\x1a\x41\n\x0bMetricStats\x12\x0c\n\x04mean\x18\x01 \x03(\x01\x12\n\n\x02sD\x18\x02 \x03(\x01\x12\x0b\n\x03max\x18\x03 \x03(\x01\x12\x0b\n\x03min\x18\x04 \x03(\x01\"w\n\x16KpiBundlePacketMetrics\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12#\n\x07sigType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\'\n\x07metrics\x18\x04 \x02(\x0b\x32\x16.allego.KpiMetricsData\"S\n\nKpiMetrics\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12.\n\x06\x62undle\x18\x02 \x02(\x0b\x32\x1e.allego.KpiBundlePacketMetrics\"c\n\x11KpiControlRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x14\n\x0cisAllBundles\x18\x03 \x01(\x08\":\n\x12SetKpiParamRequest\x12\x15\n\rstreamGroupId\x18\x01 \x01(\t\x12\r\n\x05param\x18\x02 \x01(\x01\",\n\x13GetKpiStatusRequest\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\"K\n\x12KpiStandardRequest\x12\x11\n\tdsourceID\x18\x02 \x03(\t\x12\"\n\x03\x63md\x18\x03 \x01(\x0e\x32\x15.allego.KpiScannerCmd\"\xba\x01\n\rKpiFileStatus\x12,\n\x07\x64source\x18\x01 \x03(\x0b\x32\x1b.allego.KpiFileStatus.State\x1a{\n\x05State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\nisComplete\x18\x02 \x01(\x08\x12\x12\n\ndsourceUID\x18\x03 \x01(\t\x12 \n\x05kpiTR\x18\x04 \x01(\x0b\x32\x11.allego.TimeRange\x12\x17\n\x0f\x66ilePathAndName\x18\x05 \x01(\t\"\xc7\x04\n\x0eKpiFileStatus2\x12>\n\x07\x64source\x18\x01 \x03(\x0b\x32-.allego.KpiFileStatus2.KpiDatasourceStateSpec\x1a\xe9\x01\n\tKPI_State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\nisComplete\x18\x02 \x01(\x08\x12\x14\n\x0c\x66racComplete\x18\x03 \x01(\x01\x12\x17\n\x0f\x66ilePathAndName\x18\x04 \x01(\t\x12 \n\x05kpiTR\x18\x05 \x01(\x0b\x32\x11.allego.TimeRange\x12\x14\n\x0cpacketDurSec\x18\x06 \x01(\x01\x12\x0e\n\x06numAmp\x18\x07 \x01(\x03\x12\x18\n\x10\x62ytesInBundlePkt\x18\x08 \x01(\x03\x12\x12\n\nnumPackets\x18\t \x01(\x03\x12\x12\n\ndatasetUID\x18\n \x01(\t\x1aq\n\x10\x44\x61tasource_State\x12\x17\n\x0f\x66ilePathAndName\x18\x01 \x01(\t\x12\x1d\n\x02TR\x18\x02 \x01(\x0b\x32\x11.allego.TimeRange\x12\x12\n\ndatasetUID\x18\x03 \x01(\t\x12\x11\n\tdsourceID\x18\x04 \x01(\t\x1a\x95\x01\n\x16KpiDatasourceStateSpec\x12\x37\n\x06source\x18\x01 \x02(\x0b\x32\'.allego.KpiFileStatus2.Datasource_State\x12-\n\x03kpi\x18\x02 \x02(\x0b\x32 .allego.KpiFileStatus2.KPI_State\x12\x13\n\x0bisSprinting\x18\x03 \x02(\x08\"\xfd\x01\n\x0fKpiFileMetadata\x12.\n\x07\x64source\x18\x01 \x03(\x0b\x32\x1d.allego.KpiFileMetadata.State\x1a\xb9\x01\n\x05State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\ndsourceUID\x18\x02 \x01(\t\x12\x11\n\tpacketDur\x18\x03 \x01(\x01\x12\x0c\n\x04nAMP\x18\x04 \x01(\x03\x12\x1b\n\x13\x62ytesInBundlePacket\x18\x05 \x01(\x03\x12\x12\n\nnumPackets\x18\x06 \x01(\x03\x12 \n\x05kpiTR\x18\x07 \x01(\x0b\x32\x11.allego.TimeRange\x12\x17\n\x0f\x66ilePathAndName\x18\x08 \x01(\t\"\xd3\x02\n\x0eKpiStatusReply\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x11\n\ttimeRange\x18\x03 \x01(\x01\x12\x16\n\x0etimestampRange\x18\x04 \x01(\x03\x12\x18\n\x10numPacketsMemory\x18\x05 \x02(\x03\x12\x11\n\tpacketDur\x18\x06 \x02(\x01\x12\x14\n\x0cupdatePeriod\x18\x07 \x02(\x01\x12\x13\n\x0bpersistence\x18\x08 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\t \x02(\x01\x12\x1d\n\x15isTrackingSignalCache\x18\x0b \x02(\x08\x12\x12\n\nnumPackets\x18\x0c \x02(\x03\x12\x13\n\x0bmemoryBytes\x18\r \x02(\x01\x12\n\n\x02\x66s\x18\x0e \x01(\x01\x12\x15\n\rwallTimeStart\x18\x0f \x01(\t\x12\x1d\n\x02tR\x18\x10 \x01(\x0b\x32\x11.allego.TimeRange\x12\x0f\n\x07numSigs\x18\x11 \x01(\x03\"\xe6\x02\n\x11SigKpiParamRecord\x12\x15\n\risEventDetect\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x11\n\teventThr0\x18\x03 \x02(\x01\x12\x11\n\teventThr1\x18\x04 \x02(\x01\x12\x13\n\x0b\x65ventThrSd0\x18\x05 \x02(\x01\x12\x13\n\x0b\x65ventThrSd1\x18\x06 \x02(\x01\x12\x11\n\tpreThrPts\x18\x07 \x02(\x05\x12\x12\n\npostThrPts\x18\x08 \x02(\x05\x12\x11\n\tevtDurPts\x18\t \x02(\x05\x12\x11\n\tshadowPts\x18\n \x02(\x05\x12\x0e\n\x06preThr\x18\x0b \x02(\x01\x12\x0f\n\x07postThr\x18\x0c \x02(\x01\x12\x0e\n\x06\x65vtDur\x18\r \x02(\x01\x12\x0e\n\x06shadow\x18\x0e \x02(\x01\x12\x11\n\tisSetThr0\x18\x0f \x02(\x08\x12\x11\n\tisSetThr1\x18\x10 \x02(\x08\x12\x10\n\x08isSDThr0\x18\x11 \x02(\x08\x12\x10\n\x08isSDThr1\x18\x12 \x02(\x08\"J\n\x0e\x41nnotateBundle\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\r\n\x05notes\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x01(\t\"]\n\x0fProjectMetadata\x12\x12\n\nprojectUID\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61seUID\x18\x02 \x01(\t\x12\x10\n\x08trialUID\x18\x03 \x01(\t\x12\x13\n\x0b\x61nnotateUID\x18\x04 \x03(\t\"3\n\x16SensorExtendedMetadata\x12\x19\n\x11sensorInstanceUID\x18\x01 \x01(\t\"%\n\x0fGonumMatrixList\x12\x12\n\nmdataBytes\x18\x01 \x02(\x0c\"6\n\x0fRadixMatrixList\x12#\n\x06matrix\x18\x01 \x03(\x0b\x32\x13.allego.RadixMatrix\"*\n\x0bRadixMatrix\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\x12\r\n\x05shape\x18\x02 \x03(\x05\"/\n\x10RadixMatrixBytes\x12\x0c\n\x04\x64\x61ta\x18\x01 \x02(\x0c\x12\r\n\x05shape\x18\x02 \x03(\x05\"8\n\x10RadixSignalsList\x12$\n\x06matrix\x18\x01 \x03(\x0b\x32\x14.allego.RadixSignals\"\xa9\x01\n\x0cRadixSignals\x12\x10\n\x08sampFreq\x18\x01 \x02(\x01\x12 \n\x03pri\x18\x02 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x61ux\x18\x03 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x64in\x18\x04 \x02(\x0b\x32\x13.allego.RadixMatrix\x12!\n\x04\x64out\x18\x05 \x02(\x0b\x32\x13.allego.RadixMatrix\"\x19\n\x0cVectorString\x12\t\n\x01x\x18\x01 \x03(\t\"\x1a\n\rVectorFloat64\x12\t\n\x01x\x18\x01 \x03(\x01\"G\n\x12VectorSliceFloat64\x12\"\n\x03vec\x18\x01 \x03(\x0b\x32\x15.allego.VectorFloat64\x12\r\n\x05label\x18\x02 \x01(\t\"\xde\x02\n\x14LogsysKpiStatusReply\x12\x1f\n\x05portA\x18\x01 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portB\x18\x02 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portC\x18\x03 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portD\x18\x04 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portE\x18\x05 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portF\x18\x06 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portG\x18\x07 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portH\x18\x08 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux0\x18\t \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux1\x18\n \x02(\x0b\x32\x10.allego.KpiCache\"\xfc\x02\n\x08KpiCache\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x15\n\rminNumPackets\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x05\x12\x12\n\nnumPackets\x18\x06 \x02(\x05\x12\x0e\n\x06tRange\x18\x07 \x03(\x01\x12\x0f\n\x07tsRange\x18\x08 \x03(\x03\x12\x15\n\rmeanPacketDur\x18\t \x02(\x01\x12\x19\n\x11meanCalcPacketDur\x18\n \x02(\x01\x12\x11\n\tpacketDur\x18\x0b \x02(\x01\x12\x1d\n\x15totalPacketsProcessed\x18\x0c \x02(\r\x12\x12\n\nsignalType\x18\r \x02(\t\x12\x12\n\nnumPriSigs\x18\x0e \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x0f \x02(\x05\x12\x12\n\nnumDinSigs\x18\x10 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x11 \x02(\x05\x12\x14\n\x0cupdatePeriod\x18\x12 \x02(\x01\"\xfa\x02\n\x12LogsysKpiTailReply\x12\"\n\x05portA\x18\x01 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portB\x18\x02 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portC\x18\x03 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portD\x18\x04 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portE\x18\x05 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portF\x18\x06 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portG\x18\x07 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portH\x18\x08 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux0\x18\t \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux1\x18\n \x01(\x0b\x32\x13.allego.KpiPortInfo\"3\n\x0bKpiPortInfo\x12$\n\x07kpiTail\x18\x01 \x03(\x0b\x32\x13.allego.KpiTailRows\"\xf4\x02\n\x0bKpiTailRows\x12\x10\n\x08wallTime\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x02(\x01\x12\x14\n\x0clocalSigType\x18\x03 \x02(\t\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x03\x12\x0b\n\x03\x64ur\x18\x05 \x02(\x01\x12\x0e\n\x06stdDev\x18\x06 \x02(\x01\x12\x0f\n\x07\x63StdDev\x18\x07 \x02(\x01\x12\x11\n\tabsEvtAmp\x18\x08 \x02(\x01\x12\x12\n\ncabsEvtAmp\x18\t \x02(\x01\x12\x0b\n\x03SNR\x18\n \x02(\x01\x12\x0c\n\x04\x63SNR\x18\x0b \x02(\x01\x12\x0f\n\x07numEvts\x18\x0c \x02(\x05\x12\x10\n\x08\x63numEvts\x18\r \x02(\x05\x12\x0f\n\x07\x65vtRate\x18\x0e \x02(\x01\x12\x10\n\x08\x63\x45vtRate\x18\x0f \x02(\x01\x12\x0b\n\x03max\x18\x10 \x02(\x01\x12\x0c\n\x04\x63max\x18\x11 \x02(\x01\x12\x0b\n\x03min\x18\x12 \x02(\x01\x12\x0c\n\x04\x63min\x18\x13 \x02(\x01\x12\x14\n\x0cmeanPosPkAmp\x18\x14 \x02(\x01\x12\x14\n\x0cmeanNegPkAmp\x18\x15 \x02(\x01\"*\n\x18WarehouseHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\"(\n\x19OutfitterGetDeviceRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x9e\x01\n\x11SensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x16\n\x0eisIncludeModel\x18\x03 \x01(\x08\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"z\n\x19RegisterSensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x11\n\tprofileID\x18\x03 \x02(\t\"\x92\x01\n\x1dSaveSensorCompInstanceRequest\x12 \n\x05probe\x18\x01 \x01(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x01(\x0b\x32\x15.allego.HeadstageDesc\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"&\n\tProbeDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"*\n\rHeadstageDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"`\n\x12GetSensorCompReply\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeSpec\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageSpec\"x\n\tProbeSpec\x12\x1f\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x11.allego.ProbeDesc\x12!\n\x05model\x18\x02 \x01(\x0b\x32\x12.allego.ProbeModel\x12\'\n\x08metaData\x18\x03 \x01(\x0b\x32\x15.allego.ProbeMetaData\"\x88\x01\n\rHeadstageSpec\x12#\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x15.allego.HeadstageDesc\x12%\n\x05model\x18\x02 \x01(\x0b\x32\x16.allego.HeadstageModel\x12+\n\x08metaData\x18\x03 \x01(\x0b\x32\x19.allego.HeadstageMetaData\"\xce\x04\n\nProbeModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12.\n\x04site\x18\x02 \x03(\x0b\x32 .allego.ProbeModel.ProbeSiteDesc\x12\x34\n\twireframe\x18\x03 \x02(\x0b\x32!.allego.ProbeModel.ProbeWireFrame\x12\x34\n\x0esiteOverallMin\x18\x05 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x34\n\x0esiteOverallMax\x18\x06 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x1a\xde\x01\n\rProbeSiteDesc\x12\x0c\n\x04\x61rea\x18\x01 \x02(\x01\x12\x0f\n\x07\x63\x65nterX\x18\x02 \x02(\x01\x12\x0f\n\x07\x63\x65nterY\x18\x03 \x02(\x01\x12\x0f\n\x07\x63\x65nterZ\x18\x04 \x02(\x01\x12\x11\n\tlimitXMax\x18\x05 \x02(\x01\x12\x11\n\tlimitXMin\x18\x06 \x02(\x01\x12\x11\n\tlimitYMax\x18\x07 \x02(\x01\x12\x11\n\tlimitYMin\x18\x08 \x02(\x01\x12\x11\n\tlimitZMax\x18\t \x02(\x01\x12\x11\n\tlimitZMin\x18\n \x02(\x01\x12\x0b\n\x03num\x18\x0b \x02(\x03\x12\r\n\x05shape\x18\x0c \x02(\t\x1a^\n\x0eProbeWireFrame\x12,\n\x06vertex\x18\x01 \x03(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x0e\n\x06limitX\x18\x02 \x03(\x01\x12\x0e\n\x06limitY\x18\x03 \x03(\x01\x1a!\n\tProbePtXY\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"_\n\rProbeMetaData\x12\x11\n\tprobeName\x18\x01 \x02(\t\x12\x10\n\x08numSites\x18\x02 \x02(\x05\x12\x13\n\x0b\x63\x61talogTags\x18\x03 \x02(\t\x12\x14\n\x0cinstanceTags\x18\x04 \x02(\t\"\x84\x01\n\x0eHeadstageModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12\x31\n\x04rows\x18\x02 \x03(\x0b\x32#.allego.HeadstageModel.HeadstageRow\x1a\x33\n\x0cHeadstageRow\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x03\x12\x0f\n\x07siteNum\x18\x02 \x02(\x03\"\x13\n\x11HeadstageMetaData\"5\n\x0bUserProfile\x12\x11\n\tprofileID\x18\x01 \x02(\t\x12\x13\n\x0blicenseCode\x18\x02 \x02(\t\"B\n\x16GetCurrentProfileReply\x12(\n\x0buserProfile\x18\x01 \x02(\x0b\x32\x13.allego.UserProfile\"@\n\x13GetAllProfilesReply\x12)\n\x0cuserProfiles\x18\x01 \x03(\x0b\x32\x13.allego.UserProfile\"-\n\x18SetCurrentProfileRequest\x12\x11\n\tprofileID\x18\x01 \x02(\t\"\x88\x01\n\x14ManageNodeOrgPayload\x12\r\n\x05orgID\x18\x01 \x01(\t\x12\x0f\n\x07orgName\x18\x02 \x01(\t\x12\x14\n\x0corgShortName\x18\x03 \x01(\t\x12\x0c\n\x04\x63ity\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\r\n\x05state\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"i\n\x14ManageNodeOrgRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\"S\n\x12ManageNodeOrgReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\xa2\x01\n\x14ManageNodeLabPayload\x12\r\n\x05labID\x18\x01 \x01(\t\x12\x0f\n\x07labDesc\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65pt\x18\x03 \x01(\t\x12\x14\n\x0corganization\x18\x04 \x01(\t\x12\x0f\n\x07\x61\x64minID\x18\x05 \x01(\t\x12\x11\n\tlabHeadID\x18\x06 \x01(\t\x12\x14\n\x0clabManagerID\x18\x07 \x01(\t\x12\x0c\n\x04tags\x18\x08 \x01(\t\"i\n\x14ManageNodeLabRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\"S\n\x12ManageNodeLabReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\x99\x01\n\x15ManageNodeUserPayload\x12\x0e\n\x06userID\x18\x01 \x01(\t\x12\x0c\n\x04Name\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\x0c\x12\"\n\x04role\x18\x04 \x01(\x0e\x32\x14.allego.UserRoleType\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x0f\n\x07labName\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"k\n\x15ManageNodeUserRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12.\n\x07payload\x18\x02 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\"U\n\x13ManageNodeUserReply\x12.\n\x07payload\x18\x01 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"6\n\x13\x43\x61talogProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"]\n\x10ProbeNodeRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12%\n\x07payload\x18\x02 \x03(\x0b\x32\x14.allego.ProbePayload\"7\n\x0eProbeNodeReply\x12%\n\x07payload\x18\x01 \x03(\x0b\x32\x14.allego.ProbePayload\"/\n\x0cProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"\xa5\x02\n\x0b\x45\x64gePayload\x12/\n\x06source\x18\x01 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12/\n\x06target\x18\x02 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12)\n\tedgeLabel\x18\x03 \x02(\x0e\x32\x16.allego.WorldEdgeLabel\x12-\n\tdirection\x18\x04 \x02(\x0e\x32\x1a.allego.WorldEdgeDirection\x1aZ\n\x0bGenericNode\x12%\n\x05label\x18\x01 \x02(\x0e\x32\x16.allego.WorldNodeLabel\x12\x11\n\tidPropKey\x18\x02 \x02(\t\x12\x11\n\tidPropVal\x18\x03 \x02(\t\"8\n\x10WorldEdgeRequest\x12$\n\x07payload\x18\x01 \x03(\x0b\x32\x13.allego.EdgePayload\"\x10\n\x0eWorldEdgeReply\"E\n\x11QueryWorldRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.WorldQueryCmd\x12\x0c\n\x04\x61rgs\x18\x02 \x03(\t\"\xe6\x01\n\rQueryWorldRec\x12)\n\x03org\x18\x01 \x01(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12)\n\x03lab\x18\x02 \x01(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12+\n\x04user\x18\x03 \x01(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12-\n\x08\x63\x61tProbe\x18\x04 \x01(\x0b\x32\x1b.allego.CatalogProbePayload\x12#\n\x05probe\x18\x05 \x01(\x0b\x32\x14.allego.ProbePayload\"9\n\x0fQueryWorldReply\x12&\n\x07payload\x18\x01 \x03(\x0b\x32\x15.allego.QueryWorldRec\"/\n\x1aHighLowPassTransformParams\x12\x11\n\tfrequency\x18\x01 \x02(\x01\"B\n\x13\x42\x61ndTransformParams\x12\x14\n\x0clowFrequency\x18\x01 \x02(\x01\x12\x15\n\rhighFrequency\x18\x02 \x02(\x01\"F\n\x14NotchTransformParams\x12\x16\n\x0enotchFrequency\x18\x01 \x02(\x01\x12\x16\n\x0enotchBandwidth\x18\x02 \x02(\x01\"\x14\n\x12\x43\x41RTransformParams\"2\n\x19VirtualRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\"K\n\x18PairedRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\x12\x18\n\x10targetNtvChanIdx\x18\x02 \x02(\x05\"i\n\x1d\x44\x61taSourceSinkTransformParams\x12\x10\n\x08\x64srcName\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\">\n\x18SliceTimeTransformParams\x12\x11\n\ttimeStart\x18\x01 \x02(\x01\x12\x0f\n\x07timeEnd\x18\x02 \x02(\x01\"n\n\x1cSliceChannelsTransformParams\x12\x13\n\x0bsysChanIdxs\x18\x01 \x03(\x05\x12(\n\x0bsignalGroup\x18\x02 \x01(\x0b\x32\x13.allego.SignalGroup\x12\x0f\n\x07\x64srcUid\x18\x03 \x01(\t\"1\n\x19\x44ownsampleTransformParams\x12\x14\n\x0csampleFactor\x18\x01 \x02(\x05\"\xdb\x01\n\x1aRemapSensorTransformParams\x12>\n\x07sensors\x18\x01 \x03(\x0b\x32-.allego.RemapSensorTransformParams.SensorSpec\x1a}\n\nSensorSpec\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07probeId\x18\x03 \x02(\t\x12\x13\n\x0bheadstageId\x18\x04 \x02(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\x05 \x01(\x05\x12\x13\n\x0bnumChannels\x18\x06 \x01(\x05\" \n\x08Position\x12\t\n\x01x\x18\x01 \x02(\x05\x12\t\n\x01y\x18\x02 \x02(\x05\"\x98\x06\n\rTransformNode\x12\n\n\x02id\x18\x01 \x02(\t\x12\'\n\x04type\x18\x02 \x02(\x0e\x32\x19.allego.TransformNodeType\x12\"\n\x08position\x18\x03 \x01(\x0b\x32\x10.allego.Position\x12\x0f\n\x07invalid\x18\x04 \x02(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x05 \x01(\t\x12=\n\x11highLowPassParams\x18\x06 \x01(\x0b\x32\".allego.HighLowPassTransformParams\x12/\n\nbandParams\x18\x07 \x01(\x0b\x32\x1b.allego.BandTransformParams\x12\x31\n\x0bnotchParams\x18\x08 \x01(\x0b\x32\x1c.allego.NotchTransformParams\x12-\n\tcarParams\x18\t \x01(\x0b\x32\x1a.allego.CARTransformParams\x12;\n\x10virtualRefParams\x18\n \x01(\x0b\x32!.allego.VirtualRefTransformParams\x12\x39\n\x0fpairedRefParams\x18\x0b \x01(\x0b\x32 .allego.PairedRefTransformParams\x12\x43\n\x14\x64\x61tasourceSinkParams\x18\x0c \x01(\x0b\x32%.allego.DataSourceSinkTransformParams\x12\x39\n\x0fsliceTimeParams\x18\r \x01(\x0b\x32 .allego.SliceTimeTransformParams\x12\x41\n\x13sliceChannelsParams\x18\x0e \x01(\x0b\x32$.allego.SliceChannelsTransformParams\x12;\n\x10\x64ownsampleParams\x18\x0f \x01(\x0b\x32!.allego.DownsampleTransformParams\x12=\n\x11remapSensorParams\x18\x10 \x01(\x0b\x32\".allego.RemapSensorTransformParams\";\n\rTransformEdge\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0e\n\x06source\x18\x02 \x02(\t\x12\x0e\n\x06target\x18\x03 \x02(\t\"t\n\x08Protocol\x12\n\n\x02id\x18\x01 \x02(\t\x12-\n\x0etransformNodes\x18\x02 \x03(\x0b\x32\x15.allego.TransformNode\x12-\n\x0etransformEdges\x18\x03 \x03(\x0b\x32\x15.allego.TransformEdge\"%\n\x0fProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\"B\n\x15RenameProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\x12\x15\n\rnewProtocolID\x18\x02 \x02(\t\";\n\x14GetAllProtocolsReply\x12#\n\tprotocols\x18\x01 \x03(\x0b\x32\x10.allego.Protocol\"{\n\x15\x41pplyProtocolProgress\x12\x1c\n\x14lastTimestampWritten\x18\x01 \x02(\x05\x12\x18\n\x10\x64srcTimestampEnd\x18\x02 \x02(\x05\x12\x14\n\x0c\x66racComplete\x18\x03 \x01(\x01\x12\x14\n\x0cincrementSec\x18\x04 \x01(\x01\"\x9a\x01\n\x1aSpikeSorterSetParamRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12,\n\x03\x63md\x18\x02 \x02(\x0e\x32\x1f.allego.SpikeSorterParamCommand\x12\x12\n\nregFloat64\x18\x03 \x03(\x01\x12\x0f\n\x07regBool\x18\x05 \x03(\x08\x12\x12\n\nntvChanIdx\x18\x06 \x03(\x05\"Q\n\x1bSpikeSorterSetParamsRequest\x12\x32\n\x06params\x18\x01 \x03(\x0b\x32\".allego.SpikeSorterSetParamRequest\"\xa7\x02\n\x1dSpikeSorterParamCommandRecord\x12\x11\n\tisEnabled\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x0b\n\x03thr\x18\x03 \x03(\x01\x12\r\n\x05thrSd\x18\x04 \x03(\x01\x12\x11\n\tthrWdwPts\x18\x05 \x03(\x05\x12\x0e\n\x06thrWdw\x18\x06 \x03(\x01\x12\x0e\n\x06shadow\x18\x07 \x02(\x01\x12\x11\n\tshadowPts\x18\x08 \x02(\x05\x12\x10\n\x08isSetThr\x18\t \x03(\x08\x12\x0f\n\x07weakThr\x18\n \x03(\x01\x12\x11\n\tweakThrSd\x18\x0b \x03(\x01\x12\x14\n\x0cisSetWeakThr\x18\x0c \x03(\x08\x12\x12\n\npeakWdwPts\x18\r \x03(\x05\x12\x0f\n\x07peakWdw\x18\x0e \x03(\x01\x12\x0c\n\x04isSD\x18\x0f \x02(\x08\"?\n\tKpiParams\x12\x32\n\x03rec\x18\x01 \x03(\x0b\x32%.allego.SpikeSorterParamCommandRecord\"J\n\x10\x44\x41\x43StreamRequest\x12\x0b\n\x03\x44\x41\x43\x18\x01 \x02(\x05\x12\x12\n\nNtvChanIdx\x18\x02 \x02(\x05\x12\x15\n\rstreamGroupId\x18\x03 \x01(\t\"\xde\x01\n\x11\x45ventViewerConfig\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x19\n\x11triggerSysChanIdx\x18\x03 \x01(\x05\x12\x1a\n\x12triggerThresholdUV\x18\x04 \x01(\x01\x12\x14\n\x0cpreTriggerMs\x18\x05 \x02(\x01\x12\x15\n\rpostTriggerMs\x18\x06 \x02(\x01\x12\'\n\x0btriggerType\x18\x07 \x01(\x0e\x32\x12.allego.SignalType\x12\x0e\n\x06ntvIdx\x18\x08 \x01(\x05\"=\n\rEventViewerID\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\"D\n\x1aGetEventViewerEventRequest\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x0f\n\x07\x65ventId\x18\x02 \x02(\t\"Y\n\x14\x45ventViewerEventDesc\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\"\x8f\x01\n\x10\x45ventViewerEvent\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12\x13\n\x0bsysChanIdxs\x18\x05 \x03(\x05\"a\n\x1aListEventViewerEventsReply\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12,\n\x06\x65vents\x18\x02 \x03(\x0b\x32\x1c.allego.EventViewerEventDesc\"D\n\x15ListEventViewersReply\x12+\n\x0c\x65ventViewers\x18\x01 \x03(\x0b\x32\x15.allego.EventViewerID\"3\n\x1fStatusPollFieldsToUpdateRequest\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\"^\n\x18StatusPollFieldsToUpdate\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\x12\x30\n\x0e\x66ieldsToUpdate\x18\x02 \x03(\x0e\x32\x18.allego.StatusPollFields\"\xa5\x01\n\x17\x44\x61shboardCommandRequest\x12\'\n\x08\x64\x61shType\x18\x01 \x01(\x0e\x32\x15.allego.DashboardType\x12\x32\n\x04\x61rgs\x18\x02 \x01(\x0b\x32$.allego.DashboardCommandRequest.Args\x1a-\n\x04\x41rgs\x12%\n\x03\x63md\x18\x01 \x02(\x0e\x32\x18.allego.DashboardCommand\"]\n\x13SelTableSignalGroup\x12\r\n\x05index\x18\x01 \x02(\t\x12\x15\n\rcriterionDesc\x18\x02 \x02(\t\x12\x0f\n\x07ntvIdxs\x18\x03 \x03(\x03\x12\x0f\n\x07numSigs\x18\x04 \x02(\x03\"?\n\x13SelectorTablesReply\x12(\n\x03sig\x18\x01 \x03(\x0b\x32\x1b.allego.SelTableSignalGroup\"\xfa\x02\n\x10\x44\x61taSourceStatus\x12%\n\x04type\x18\x01 \x02(\x0e\x32\x17.allego.SignalGroupType\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12\x10\n\x08\x64uration\x18\x04 \x02(\x01\x12(\n\x0bsignalGroup\x18\x06 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x17\n\x0fnumTotalSamples\x18\x07 \x02(\x03\x12\x12\n\nsampleFreq\x18\t \x01(\x01\x12\x0b\n\x03uid\x18\n \x02(\t\x12\x16\n\x0e\x64\x61taSourceType\x18\x0b \x02(\t\x12\x10\n\x08\x66ileType\x18\x0c \x02(\t\x12\x0c\n\x04mode\x18\r \x02(\t\x12\r\n\x05label\x18\x0e \x02(\t\x12\x0c\n\x04path\x18\x0f \x02(\t\x12\x14\n\x0c\x62\x61seFileName\x18\x10 \x02(\t\x12\x1d\n\x02tR\x18\x11 \x01(\x0b\x32\x11.allego.TimeRange\x12\x14\n\x0ckpiDsourceID\x18\x12 \x01(\t*\x96\x02\n\x0eRadixFileTypes\x12\x07\n\x03RHD\x10\x00\x12\x08\n\x04XDAT\x10\x01\x12\x07\n\x03\x43SV\x10\x02\x12\x08\n\x04HDF5\x10\x03\x12\x08\n\x04NEX5\x10\x04\x12\x07\n\x03NWB\x10\x05\x12\x10\n\x0c\x42IOINTERFACE\x10\x07\x12\r\n\tKILOSORT2\x10\x08\x12\x07\n\x03\x41NC\x10\t\x12\x0f\n\x0bSPKTRAIN_MU\x10\n\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_HDF5\x10\x0b\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_MAT5\x10\x0c\x12\x07\n\x03NSX\x10\r\x12\x07\n\x03PL2\x10\x0e\x12\x07\n\x03TDT\x10\x0f\x12\n\n\x06SPIKES\x10\x10\x12\x07\n\x03KPI\x10\x11\x12\x15\n\x11UNKNOWN_FILE_TYPE\x10\x12\x12\x0f\n\x0bMEAREC_HDF5\x10\x13*1\n\nSignalType\x12\x07\n\x03PRI\x10\x00\x12\x07\n\x03\x41UX\x10\x01\x12\x07\n\x03\x44IN\x10\x02\x12\x08\n\x04\x44OUT\x10\x03*:\n\x0fResampleRoutine\x12\t\n\x05NAIVE\x10\x00\x12\r\n\tRETENTIVE\x10\x01\x12\r\n\tANTIALIAS\x10\x03*>\n\x04Port\x12\x05\n\x01\x41\x10\x00\x12\x05\n\x01\x42\x10\x01\x12\x05\n\x01\x43\x10\x02\x12\x05\n\x01\x44\x10\x03\x12\x05\n\x01\x45\x10\x04\x12\x05\n\x01\x46\x10\x05\x12\x05\n\x01G\x10\x06\x12\x05\n\x01H\x10\x07*2\n\x0cWorkspaceApp\x12\n\n\x06\x41llego\x10\x00\x12\n\n\x06\x43urate\x10\x01\x12\n\n\x06Videre\x10\x02*\xa0\x01\n\x11WorkspaceCommands\x12\x0f\n\x0bWSPACE_Save\x10\x00\x12\x11\n\rWSPACE_SaveAs\x10\x01\x12\x11\n\rWSPACE_Export\x10\x02\x12\x11\n\rWSPACE_Import\x10\x03\x12\x11\n\rWSPACE_Delete\x10\x04\x12\x11\n\rWSPACE_Switch\x10\x07\x12\x1b\n\x17WSPACE_SwitchToLastUsed\x10\x08*C\n\x14GetWorkspaceCommands\x12\x13\n\x0fGET_WSPACE_List\x10\x01\x12\x16\n\x12GET_WSPACE_Current\x10\x02*8\n\x11RadiensServerType\x12\x10\n\x0c\x41llegoserver\x10\x00\x12\x11\n\rRadiensserver\x10\x01*\xae\x01\n\x0fGrpcServiceType\x12\x0f\n\x0b\x41LLEGO_CORE\x10\x00\x12\x11\n\rALLEGO_PCACHE\x10\x01\x12\x0e\n\nALLEGO_KPI\x10\x02\x12\x12\n\x0e\x41LLEGO_NEURONS\x10\x03\x12\x10\n\x0cRADIENS_CORE\x10\x04\x12\x18\n\x14RADIENS_SPIKE_SORTER\x10\x05\x12\x0f\n\x0bRADIENS_DEV\x10\x06\x12\x16\n\x12RADIENS_DASHBOARDS\x10\x07*?\n\x0e\x44\x65vDatasetType\x12\x08\n\x04\x42\x41SE\x10\x00\x12\t\n\x05TRAIN\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x08\n\x04TEST\x10\x03*C\n\rPSDWindowType\x12\x0f\n\x0bHAMMING_p01\x10\x00\x12\x0f\n\x0bHAMMING_p05\x10\x01\x12\x10\n\x0cPASS_THROUGH\x10\x02*\x1e\n\nPSDScaling\x12\x10\n\x0cPSD_ABSOLUTE\x10\x00*X\n\x0e\x44\x61taSourceSort\x12\x10\n\x0c\x44SOURCE_DATE\x10\x00\x12\x10\n\x0c\x44SOURCE_NAME\x10\x01\x12\x10\n\x0c\x44SOURCE_SIZE\x10\x02\x12\x10\n\x0c\x44SOURCE_TYPE\x10\x03*.\n\x0fSignalGroupType\x12\x11\n\rPRIMARY_CACHE\x10\x00\x12\x08\n\x04\x46ILE\x10\x03*\x81\x01\n\x07\x44SPType\x12\x0b\n\x07LOWPASS\x10\x00\x12\x0c\n\x08HIGHPASS\x10\x01\x12\x0c\n\x08\x42\x41NDPASS\x10\x02\x12\t\n\x05NOTCH\x10\x03\x12\x0c\n\x08\x42\x41NDSTOP\x10\x04\x12\x07\n\x03\x43\x41R\x10\x05\x12\x15\n\x11VIRTUAL_REFERENCE\x10\x06\x12\x14\n\x10PAIRED_REFERENCE\x10\x07*9\n\x0b\x46ilterStage\x12\x12\n\x0eSTAGE_HARDWARE\x10\x00\x12\n\n\x06STAGE1\x10\x01\x12\n\n\x06STAGE2\x10\x02*\xd3\x02\n\x0e\x46\x65\x61tureLicense\x12\x1a\n\x16\x46\x65\x61t_NoLicenseRequired\x10\x00\x12\x0c\n\x08\x46\x65\x61t_Any\x10\x01\x12\x0f\n\x0b\x46\x65\x61t_Power9\x10\x02\x12\x11\n\rFeat_RadixAPI\x10\x03\x12\x0e\n\nFeat_Scope\x10\x04\x12\x13\n\x0f\x46\x65\x61t_Electrodes\x10\x05\x12\x13\n\x0f\x46\x65\x61t_HDSnapshot\x10\x06\x12\x12\n\x0e\x46\x65\x61t_Impedance\x10\x07\x12\x10\n\x0c\x46\x65\x61t_Monitor\x10\x08\x12\x16\n\x12\x46\x65\x61t_SignalMetrics\x10\t\x12\x19\n\x15\x46\x65\x61t_SignalProcessing\x10\n\x12\x0f\n\x0b\x46\x65\x61t_System\x10\x0b\x12\x12\n\x0e\x46\x65\x61t_SpikeGrid\x10\x0c\x12\x14\n\x10\x46\x65\x61t_SpikeSorter\x10\r\x12\x0f\n\x0b\x46\x65\x61t_Raster\x10\x0e\x12\x14\n\x10\x46\x65\x61t_ThreeDModel\x10\x0f*\xed\x01\n\x10SummaryStatsEnum\x12\x10\n\x0cSS_STAT_MEAN\x10\x00\x12\x0e\n\nSS_STAT_SD\x10\x01\x12\x10\n\x0cSS_STAT_MODE\x10\x02\x12\x0f\n\x0bSS_STAT_MIN\x10\x03\x12\x0f\n\x0bSS_STAT_MAX\x10\x04\x12\x16\n\x12SS_STAT_MODE_COUNT\x10\x05\x12\x12\n\x0eSS_STAT_MEDIAN\x10\x06\x12\x0f\n\x0bSS_STAT_Q25\x10\x07\x12\x0f\n\x0bSS_STAT_Q75\x10\x08\x12\x10\n\x0cSS_STAT_SKEW\x10\t\x12\x14\n\x10SS_STAT_KURTOSIS\x10\n\x12\r\n\tSS_STAT_N\x10\x0b*_\n\x0eKpiMetricsMode\x12\x18\n\x14Kpi_MetricsMode_Base\x10\x00\x12\x17\n\x13Kpi_MetricsMode_Avg\x10\x01\x12\x1a\n\x16Kpi_MetricsMode_Stream\x10\x02*\xa1\x06\n\x0eKpiMetricsEnum\x12\x0f\n\x0bKPI_NUM_PTS\x10\x00\x12\x13\n\x0fKPI_NUM_PTS_ISI\x10\x01\x12\x0f\n\x0bKPI_DUR_SEC\x10\x02\x12\x0c\n\x08KPI_MEAN\x10\x03\x12\x0b\n\x07KPI_MIN\x10\x04\x12\x0f\n\x0bKPI_MIN_ISI\x10\x05\x12\x0b\n\x07KPI_MAX\x10\x06\x12\x0f\n\x0bKPI_MAX_ISI\x10\x07\x12\x0f\n\x0bKPI_MAX_ABS\x10\x08\x12\x13\n\x0fKPI_MAX_ABS_ISI\x10\t\x12\x15\n\x11KPI_TIMESTAMP_MIN\x10\n\x12\x15\n\x11KPI_TIMESTAMP_MAX\x10\x0b\x12\x18\n\x14KPI_MAX_MIN_DIFF_ABS\x10\x0c\x12\x1c\n\x18KPI_MAX_MIN_DIFF_ABS_ISI\x10\r\x12\n\n\x06KPI_SD\x10\x0e\x12\x0e\n\nKPI_SD_ISI\x10\x0f\x12\x0b\n\x07KPI_VAR\x10\x10\x12\x0f\n\x0bKPI_VAR_ISI\x10\x11\x12\x0b\n\x07KPI_RMS\x10\x12\x12\x0f\n\x0bKPI_RMS_ISI\x10\x13\x12\x10\n\x0cKPI_NOISE_UV\x10\x14\x12\x0b\n\x07KPI_SNR\x10\x15\x12\x12\n\x0eKPI_NUM_EVENTS\x10\x16\x12\x12\n\x0eKPI_EVENT_RATE\x10\x17\x12\x11\n\rKPI_EVENT_MAX\x10\x18\x12\x11\n\rKPI_EVENT_MIN\x10\x19\x12\x15\n\x11KPI_EVENT_MAX_ABS\x10\x1a\x12\x1e\n\x1aKPI_EVENT_MAX_MIN_DIFF_ABS\x10\x1b\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MIN\x10\x1c\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MAX\x10\x1d\x12\x1f\n\x1bKPI_EVENT_TIMESTAMP_MAX_ABS\x10\x1e\x12(\n$KPI_EVENT_TIMESTAMP_MAX_MIN_DIFF_ABS\x10\x1f\x12\x10\n\x0cKPI_MEAN_MAX\x10 \x12\x10\n\x0cKPI_MEAN_MIN\x10!\x12\x14\n\x10KPI_MEAN_MAX_ABS\x10\"\x12#\n\x1fKPI_EVENT_MEAN_MAX_MIN_DIFF_ABS\x10#\x12\"\n\x1eKPI_MAX_MIN_DIFF_ABS_AMPLIFIED\x10$*\x8b\x01\n\x13KpiMetricsStatsEnum\x12\x1e\n\x1aKPI_BDL_METRICS_STATS_MEAN\x10\x00\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MAX\x10\x01\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MIN\x10\x02\x12\x16\n\x12KPI_BDL_METRICS_SD\x10\x03*\xc0\x02\n\x19KpiBundlePacketsStatsEnum\x12\x14\n\x10KPI_BDL_NUM_SIGS\x10\x00\x12\x13\n\x0fKPI_BDL_DUR_SEC\x10\x01\x12\x1d\n\x19KPI_BDL_NUM_SIGS_W_EVENTS\x10\x02\x12\x15\n\x11KPI_BDL_SIG_YIELD\x10\x03\x12\x13\n\x0fKPI_BDL_RMS_AVG\x10\x04\x12\x13\n\x0fKPI_BDL_SNR_AVG\x10\x05\x12\x13\n\x0fKPI_BDL_SIG_MAX\x10\x06\x12\x13\n\x0fKPI_BDL_SIG_MIN\x10\x07\x12\x18\n\x14KPI_BDL_NOISE_UV_AVG\x10\x08\x12\x1c\n\x18KPI_BDL_NUM_EVENTS_TOTAL\x10\t\x12\x1a\n\x16KPI_BDL_NUM_EVENTS_AVG\x10\n\x12\x1a\n\x16KPI_BDL_EVENT_RATE_AVG\x10\x0b*F\n\x10TimeRangeSelMode\x12\x0e\n\nTRS_SUBSET\x10\x00\x12\x0f\n\x0bTRS_TO_HEAD\x10\x01\x12\x11\n\rTRS_FROM_HEAD\x10\x02*e\n\rKpiScannerCmd\x12\x13\n\x0fKPI_SCANNER_OFF\x10\x00\x12\x1e\n\x1aKPI_SCANNER_BESPOKE_SPRINT\x10\x01\x12\x1f\n\x1bKPI_SCANNER_STANDARD_SPRINT\x10\x02*N\n\x16OutfitterComponentType\x12\x16\n\x12OUTFIT_COMP_SENSOR\x10\x00\x12\x1c\n\x18OUTFIT_COMP_SPIKE_SORTER\x10\x01*}\n\x0eWorldNodeLabel\x12\x12\n\x0eWORLD_NODE_ORG\x10\x01\x12\x12\n\x0eWORLD_NODE_LAB\x10\x02\x12\x13\n\x0fWORLD_NODE_USER\x10\x03\x12\x18\n\x14WORLD_NODE_CAT_PROBE\x10\x04\x12\x14\n\x10WORLD_NODE_PROBE\x10\x05*\'\n\x0eWorldEdgeLabel\x12\x15\n\x11WORLD_EDGE_MEMBER\x10\x01*`\n\x12WorldEdgeDirection\x12\x18\n\x14WORLD_EDGE_DIR_RIGHT\x10\x01\x12\x17\n\x13WORLD_EDGE_DIR_LEFT\x10\x02\x12\x17\n\x13WORLD_EDGE_DIR_BOTH\x10\x03*\x9f\x01\n\x0cUserRoleType\x12\x0b\n\x07USER_PI\x10\x01\x12\x12\n\x0eUSER_SCIENTIST\x10\x02\x12\x11\n\rUSER_POST_DOC\x10\x03\x12\x15\n\x11USER_GRAD_STUDENT\x10\x04\x12\x13\n\x0fUSER_UG_STUDENT\x10\x05\x12\x10\n\x0cUSER_MANAGER\x10\x06\x12\r\n\tUSER_TECH\x10\x07\x12\x0e\n\nUSER_OTHER\x10\x08*G\n\rManageNodeCmd\x12\x10\n\x0cNODE_CMD_NEW\x10\x01\x12\x12\n\x0eNODE_CMD_MERGE\x10\x02\x12\x10\n\x0cNODE_CMD_DEL\x10\x03*\xe8\x01\n\rWorldQueryCmd\x12\x15\n\x11WQ_LIST_ALL_USERS\x10\x01\x12\x14\n\x10WQ_LIST_ALL_LABS\x10\x02\x12\x14\n\x10WQ_LIST_ALL_ORGS\x10\x03\x12\x1a\n\x16WQ_LIST_ALL_CAT_PROBES\x10\x04\x12\x16\n\x12WQ_LIST_ALL_PROBES\x10\x05\x12\x18\n\x14WQ_CAT_PROBE_BY_NAME\x10\x06\x12\x11\n\rWQ_USER_BY_ID\x10\x07\x12\x19\n\x15WQ_USER_AND_LAB_BY_ID\x10\x08\x12\x18\n\x14WQ2_LIST_ALL_DEVICES\x10\x1e*\x82\x02\n\x11TransformNodeType\x12\x10\n\x0cNOTCH_FILTER\x10\x00\x12\x13\n\x0f\x42\x41NDPASS_FILTER\x10\x01\x12\x13\n\x0f\x42\x41NDSTOP_FILTER\x10\x02\x12\x13\n\x0fHIGHPASS_FILTER\x10\x03\x12\x12\n\x0eLOWPASS_FILTER\x10\x04\x12\x0e\n\nPAIRED_REF\x10\x05\x12\x0f\n\x0bVIRTUAL_REF\x10\x06\x12\x0b\n\x07\x43\x41R_REF\x10\x07\x12\x0e\n\nSLICE_TIME\x10\t\x12\x12\n\x0eSLICE_CHANNELS\x10\n\x12\n\n\x06SOURCE\x10\x0b\x12\x08\n\x04SINK\x10\x0c\x12\x0e\n\nDOWNSAMPLE\x10\r\x12\x10\n\x0cREMAP_SENSOR\x10\x0e*\xdf\x01\n\x17SpikeSorterParamCommand\x12\x14\n\x10SORTER_THR_LEVEL\x10\x01\x12\x17\n\x13SORTER_THR_LEVEL_SD\x10\x04\x12\x12\n\x0eSORTER_THR_WDW\x10\x08\x12\x19\n\x15SORTER_WEAK_THR_LEVEL\x10\n\x12\x1c\n\x18SORTER_WEAK_THR_LEVEL_SD\x10\r\x12\x11\n\rSORTER_SHADOW\x10\x11\x12\x17\n\x13SORTER_THR_ACTIVATE\x10\x13\x12\x1c\n\x18SORTER_WEAK_THR_ACTIVATE\x10\x15*\x86\x04\n\x10StatusPollFields\x12\x19\n\x15PORT_CONNECTION_STATE\x10\x00\x12\x14\n\x10RECORDING_ERRORS\x10\x01\x12\x15\n\x11STREAM_TIME_RANGE\x10\x02\x12\x11\n\rSTREAM_STATUS\x10\x03\x12\x11\n\rRECORD_STATUS\x10\x04\x12\x16\n\x12GPIO_CHANNEL_COUNT\x10\x05\x12\x10\n\x0cIS_CONNECTED\x10\x06\x12\x0e\n\nRECORD_DUR\x10\x07\x12\x11\n\rBACKBONE_MODE\x10\t\x12\x10\n\x0cSIGNAL_GROUP\x10\n\x12\x14\n\x10SINAPS_REGISTERS\x10\x0b\x12\x14\n\x10RECORDING_CONFIG\x10\x0c\x12\x0b\n\x07\x46ILTERS\x10\r\x12\x17\n\x13\x45VENT_THRESH_PARAMS\x10\x0e\x12\x10\n\x0c\x44\x41\x43_REGISTER\x10\x0f\x12\x10\n\x0c\x44IO_REGISTER\x10\x10\x12\x10\n\x0cTRIGGER_MODE\x10\x11\x12\x11\n\rCABLE_LENGTHS\x10\x12\x12\x11\n\rEVENT_VIEWERS\x10\x13\x12\x0f\n\x0bSAMPLE_RATE\x10\x14\x12\x0e\n\nALL_FIELDS\x10\x15\x12\x16\n\x12SPIKE_SORTER_STATE\x10\x16\x12\x0f\n\x0bSTIM_PARAMS\x10\x17\x12\x19\n\x15SPIKE_SORTER_WARNINGS\x10\x18\x12\x12\n\x0eSTIM_STEP_SIZE\x10\x19*\x1b\n\rDashboardType\x12\n\n\x06\x44\x41SH_1\x10\x00*N\n\x10\x44\x61shboardCommand\x12\x11\n\rDASH_CMD_OPEN\x10\x00\x12\x12\n\x0e\x44\x41SH_CMD_CLOSE\x10\x01\x12\x13\n\x0f\x44\x41SH_CMD_UPDATE\x10\x02\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x06\x61llego\x1a\x1fgoogle/protobuf/timestamp.proto\"@\n\x14OfflineLicenseStatus\x12\x12\n\nisVerified\x18\x01 \x02(\x08\x12\x14\n\x0chardwareUUID\x18\x02 \x02(\t\"C\n\x0f\x46irmwareVersion\x12\x0c\n\x04\x64\x61te\x18\x01 \x02(\t\x12\x10\n\x08majorRev\x18\x02 \x02(\x05\x12\x10\n\x08minorRev\x18\x03 \x02(\x05\"k\n\x10RadixEnvironment\x12\x0f\n\x07version\x18\x01 \x02(\t\x12\x14\n\x0cuserDataPath\x18\x02 \x02(\t\x12\x30\n\x0f\x66irmwareVersion\x18\x03 \x02(\x0b\x32\x17.allego.FirmwareVersion\"!\n\x0fStandardRequest\x12\x0e\n\x06regStr\x18\x02 \x03(\t\"/\n\rStandardReply\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\x12\x0e\n\x06regStr\x18\x02 \x03(\t\"&\n\rDACOffRequest\x12\x15\n\rstreamGroupId\x18\x01 \x01(\t\"\xba\x01\n\x13WorkspaceDescriptor\x12\n\n\x02iD\x18\x01 \x02(\t\x12!\n\x03\x61pp\x18\x02 \x02(\x0e\x32\x14.allego.WorkspaceApp\x12\x12\n\nisModified\x18\x03 \x02(\x08\x12\x19\n\x11timestampLastUsed\x18\x04 \x02(\t\x12\x19\n\x11timestampModified\x18\x05 \x02(\t\x12*\n\nannotation\x18\x06 \x02(\x0b\x32\x16.allego.AnnotateBundle\"\xb8\x01\n\x17WorkspaceControlRequest\x12&\n\x03\x63md\x18\x01 \x02(\x0e\x32\x19.allego.WorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12*\n\nannotation\x18\x03 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x1a\n\x12targetFullFileName\x18\x04 \x01(\t\x12\x18\n\x10isForceOverwrite\x18\x05 \x01(\x08\"\xd3\x01\n\x13GetWorkspaceRequest\x12)\n\x03\x63md\x18\x01 \x02(\x0e\x32\x1c.allego.GetWorkspaceCommands\x12\x13\n\x0bworkspaceID\x18\x02 \x01(\t\x12\x14\n\x0cworkspaceDir\x18\x03 \x01(\t\x12%\n\x07\x61ppMask\x18\x04 \x01(\x0e\x32\x14.allego.WorkspaceApp\x12,\n\x0c\x61nnotateMask\x18\x05 \x01(\x0b\x32\x16.allego.AnnotateBundle\x12\x11\n\tisBrowser\x18\x06 \x01(\x08\"\xab\x01\n\x11GetWorkspaceReply\x12\x43\n\rworkspaceDesc\x18\x01 \x03(\x0b\x32,.allego.GetWorkspaceReply.WorkspaceDescEntry\x1aQ\n\x12WorkspaceDescEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x1b.allego.WorkspaceDescriptor:\x02\x38\x01\"`\n\x18GetRadiensServersRequest\x12\x15\n\rhostIPaddress\x18\x01 \x02(\t\x12-\n\nserverType\x18\x02 \x01(\x0e\x32\x19.allego.RadiensServerType\"\x97\x02\n\nServerSpec\x12\x0c\n\x04host\x18\x01 \x02(\t\x12\x0b\n\x03pid\x18\x02 \x02(\x05\x12\x30\n\x07service\x18\x03 \x03(\x0b\x32\x1f.allego.ServerSpec.ServiceEntry\x12\x30\n\x05spawn\x18\x04 \x01(\x0b\x32!.allego.ServerSpec.SpawnedProcess\x1a\x1b\n\x0bGrpcService\x12\x0c\n\x04port\x18\x01 \x02(\x05\x1a\x1d\n\x0eSpawnedProcess\x12\x0b\n\x03pid\x18\x01 \x03(\x05\x1aN\n\x0cServiceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.allego.ServerSpec.GrpcService:\x02\x38\x01\"j\n\x13RadiensServersReply\x12(\n\x0c\x61llegoserver\x18\x01 \x03(\x0b\x32\x12.allego.ServerSpec\x12)\n\rradiensserver\x18\x02 \x03(\x0b\x32\x12.allego.ServerSpec\"-\n\x14SignalGroupIDRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\"\xc4\x01\n\tSignalMap\x12\x0f\n\x07siteIdx\x18\x01 \x03(\x05\x12\x13\n\x0b\x63ompSiteNum\x18\x02 \x03(\t\x12\x13\n\x0bposProbeUmX\x18\x03 \x03(\x01\x12\x13\n\x0bposProbeUmY\x18\x04 \x03(\x01\x12\x13\n\x0bposProbeUmZ\x18\x05 \x03(\x01\x12\x14\n\x0cposTissueUmX\x18\x06 \x03(\x01\x12\x14\n\x0cposTissueUmY\x18\x07 \x03(\x01\x12\x14\n\x0cposTissueUmZ\x18\x08 \x03(\x01\x12\x10\n\x08sensorID\x18\t \x03(\t\"=\n\x10GPIOChannelCount\x12\x0c\n\x04nAux\x18\x01 \x02(\x05\x12\x0c\n\x04nDin\x18\x02 \x02(\x05\x12\r\n\x05nDout\x18\x03 \x02(\x05\"D\n\x10PortChannelCount\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"Q\n\x0eSetPortRequest\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\x12\x10\n\x08probeUID\x18\x02 \x02(\t\x12\x11\n\thstageUID\x18\x03 \x02(\t\"\xe2\x02\n\x11HDSnapshotRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12=\n\npriSignals\x18\x03 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\nauxSignals\x18\x04 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12=\n\ndinSignals\x18\x05 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x12>\n\x0b\x64outSignals\x18\x06 \x01(\x0b\x32).allego.HDSnapshotRequest.SelectedSignals\x1a&\n\x0fSelectedSignals\x12\x13\n\x0bntvChanIdxs\x18\x01 \x03(\x05\"\x96\x01\n\x12HDSnapshotRequest2\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12)\n\x07selMode\x18\x03 \x01(\x0e\x32\x18.allego.TimeRangeSelMode\x12#\n\x06sigSel\x18\x04 \x01(\x0b\x32\x13.allego.SigSelector\"L\n\x15RadiensPyGraphicsArgs\x12\x12\n\ngraphicsID\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0f\n\x07\x66igSize\x18\x03 \x03(\x03\"\xdd\x02\n\nPSDRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12)\n\x07selMode\x18\x03 \x02(\x0e\x32\x18.allego.TimeRangeSelMode\x12!\n\x05stype\x18\x04 \x02(\x0e\x32\x12.allego.SignalType\x12\x0f\n\x07ntvIdxs\x18\x05 \x03(\x03\x12\x12\n\nresampleFs\x18\x06 \x01(\x01\x12&\n\x07wdwType\x18\x07 \x01(\x0e\x32\x15.allego.PSDWindowType\x12#\n\x07scaling\x18\x08 \x01(\x0e\x32\x12.allego.PSDScaling\x12\x11\n\tfreqRange\x18\t \x03(\x01\x12\x14\n\x0c\x63ollapseFreq\x18\n \x01(\x08\x12\x11\n\tdeltaFreq\x18\x0b \x01(\x01\x12\x0c\n\x04path\x18\r \x01(\t\x12\x13\n\x0bisReturnPSD\x18\x0e \x01(\x08\"\xa1\x02\n\x03PSD\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12\x1f\n\x02sG\x18\x03 \x02(\x0b\x32\x13.allego.SignalGroup\x12!\n\x05stype\x18\x04 \x02(\x0e\x32\x12.allego.SignalType\x12\x1d\n\x02tR\x18\x05 \x02(\x0b\x32\x11.allego.TimeRange\x12 \n\x03psd\x18\x06 \x02(\x0b\x32\x13.allego.DenseMatrix\x12\x0c\n\x04\x66req\x18\x07 \x03(\x01\x12\x14\n\x0c\x66reqBinWidth\x18\x08 \x02(\x01\x12\x11\n\tfreqRange\x18\x0b \x03(\x01\x12&\n\x07wdwType\x18\t \x01(\x0e\x32\x15.allego.PSDWindowType\x12#\n\x07scaling\x18\n \x01(\x0e\x32\x12.allego.PSDScaling\"e\n\x18RadiensPyGraphicsRequest\x12\x1c\n\x07psdData\x18\x01 \x01(\x0b\x32\x0b.allego.PSD\x12+\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\x1d.allego.RadiensPyGraphicsArgs\"^\n\x0bSigSelector\x12\x12\n\nampNtvIdxs\x18\x01 \x03(\x03\x12\x12\n\nainNtvIdxs\x18\x02 \x03(\x03\x12\x12\n\ndinNtvIdxs\x18\x03 \x03(\x03\x12\x13\n\x0b\x64outNtvIdxs\x18\x04 \x03(\x03\"]\n\x0eHDSnapshotMeta\x12\x11\n\tglobalMin\x18\x04 \x02(\x01\x12\x11\n\tglobalMax\x18\x05 \x02(\x01\x12%\n\x08sigGroup\x18\x06 \x01(\x0b\x32\x13.allego.SignalGroup\"\x9f\x02\n\nHDSnapshot\x12$\n\x04meta\x18\x01 \x02(\x0b\x32\x16.allego.HDSnapshotMeta\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x13\n\x0btimeSamples\x18\x03 \x02(\x0c\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12&\n\npriSignals\x18\x05 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\nauxSignals\x18\x06 \x01(\x0b\x32\x12.allego.RawSignals\x12&\n\ndinSignals\x18\x07 \x01(\x0b\x32\x12.allego.RawSignals\x12\'\n\x0b\x64outSignals\x18\x08 \x01(\x0b\x32\x12.allego.RawSignals\"@\n\x0bHDSnapshot2\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12\x1e\n\x04sigs\x18\x02 \x02(\x0b\x32\x10.allego.Signals2\"\xb9\x03\n\x11GetSignalsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x37\n\x06params\x18\x02 \x02(\x0b\x32\'.allego.GetSignalsRequest.GetSigsParams\x1a\xd3\x02\n\rGetSigsParams\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x12\x0e\n\x06wdwSec\x18\x02 \x02(\x01\x12\x14\n\x0c\x63hanHeightPx\x18\x03 \x02(\x01\x12\x10\n\x08\x61mpFsrUv\x18\x04 \x02(\x01\x12\x17\n\x0fplotWidthPoints\x18\x05 \x02(\x01\x12\x11\n\tgpioOnTop\x18\x06 \x02(\x08\x12\x0f\n\x07\x61inFsrV\x18\x07 \x02(\x01\x12\x13\n\x0b\x63omponentID\x18\x08 \x02(\t\x12-\n\x0cresampleType\x18\t \x02(\x0e\x32\x17.allego.ResampleRoutine\x12\x11\n\tisHeatmap\x18\n \x02(\x08\x12\x1b\n\x13isNotApplyDSPstage2\x18\x0b \x01(\x08\x12\x13\n\x0b\x63lipToRange\x18\x0c \x02(\x08\x12\x17\n\x0f\x62\x61ndpassLowFreq\x18\r \x01(\x01\x12\x18\n\x10\x62\x61ndpassHighFreq\x18\x0e \x01(\x01\"[\n\nRawSignals\x12\r\n\x05shape\x18\x01 \x03(\x05\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\x12\x1d\n\x02tR\x18\x04 \x01(\x0b\x32\x11.allego.TimeRange\"\xe7\x01\n\x08Signals2\x12\x1f\n\x02sG\x18\x01 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12%\n\x03\x61mp\x18\x03 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12%\n\x03\x61in\x18\x04 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12%\n\x03\x64in\x18\x05 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\x12&\n\x04\x64out\x18\x06 \x01(\x0b\x32\x18.allego.RadixMatrixBytes\"\x85\x02\n\x14ListSensorSpecsReply\x12\x41\n\x06probes\x18\x01 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\x45\n\nheadstages\x18\x02 \x03(\x0b\x32\x31.allego.ListSensorSpecsReply.SpecWithChannelCount\x12\'\n\x05ports\x18\x03 \x03(\x0b\x32\x18.allego.PortChannelCount\x1a:\n\x14SpecWithChannelCount\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x14\n\x0c\x63hannelCount\x18\x02 \x02(\x05\"d\n\x16ListDataSourcesRequest\x12\x11\n\tdirectory\x18\x01 \x02(\t\x12&\n\x06sortBy\x18\x02 \x01(\x0e\x32\x16.allego.DataSourceSort\x12\x0f\n\x07\x64irList\x18\x03 \x03(\t\"\x1c\n\x07SortMap\x12\x11\n\tsorterIds\x18\x01 \x03(\t\">\n\x16GetSignalGroupIDsReply\x12\x12\n\ncontinuous\x18\x01 \x03(\t\x12\x10\n\x08\x64iscrete\x18\x02 \x03(\t\"\xa0\x01\n\x13GetSorterIDMapReply\x12\x43\n\x0csigToSortMap\x18\x01 \x03(\x0b\x32-.allego.GetSorterIDMapReply.SigToSortMapEntry\x1a\x44\n\x11SigToSortMapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.allego.SortMap:\x02\x38\x01\"\xaf\x01\n\nDataSource\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x02(\t\x12\x17\n\x0f\x64urationSeconds\x18\x03 \x02(\x01\x12\x17\n\x0f\x64urationMinutes\x18\x04 \x02(\x01\x12\x15\n\rdurationHours\x18\x05 \x02(\x01\x12(\n\x08\x66ileType\x18\x06 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x12\n\nnumSignals\x18\x07 \x02(\x05\"o\n\x0e\x46ileDescriptor\x12\x0c\n\x04path\x18\x01 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x13\n\x0b\x66ileNameUID\x18\x04 \x01(\t\"\xd0\x01\n\x08TimeSpec\x12\x30\n\ttimeRange\x18\x01 \x01(\x0b\x32\x1b.allego.TimeSpec.TimeRangeLH\x00\x12:\n\x0etimestampRange\x18\x02 \x01(\x0b\x32 .allego.TimeSpec.TimestampRangeLH\x00\x1a\x1f\n\nTimeRangeL\x12\x11\n\ttimeRange\x18\x01 \x03(\x01\x1a)\n\x0fTimestampRangeL\x12\x16\n\x0etimestampRange\x18\x01 \x03(\x03\x42\n\n\x08timeDesc\"\xbe\x01\n\nSignalSpec\x12.\n\x07siteNum\x18\x01 \x01(\x0b\x32\x1b.allego.SignalSpec.SiteNumLH\x00\x12\x34\n\nntvChanIdx\x18\x02 \x01(\x0b\x32\x1e.allego.SignalSpec.NtvChanIdxLH\x00\x1a\x1b\n\x08SiteNumL\x12\x0f\n\x07siteNum\x18\x01 \x03(\x05\x1a!\n\x0bNtvChanIdxL\x12\x12\n\nntvChanIdx\x18\x01 \x03(\x05\x42\n\n\x08siteDesc\"\x8c\x06\n\rChannelRecord\x12\x10\n\x08\x63hanName\x18\x01 \x02(\t\x12$\n\x08\x63hanType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\x12\n\nntvChanIdx\x18\x03 \x02(\x05\x12\x0f\n\x07siteNum\x18\x04 \x02(\x05\x12\x15\n\rcolorGroupIdx\x18\x05 \x02(\x05\x12\x12\n\nisSelected\x18\x06 \x02(\x08\x12\x13\n\x0bisAudioLeft\x18\x07 \x02(\x08\x12\x1a\n\x04port\x18\x08 \x02(\x0e\x32\x0c.allego.Port\x12\x11\n\tsiteShape\x18\t \x02(\t\x12\x10\n\x08siteCtrX\x18\n \x02(\x01\x12\x10\n\x08siteCtrY\x18\x0b \x02(\x01\x12\x10\n\x08siteCtrZ\x18\x0c \x02(\x01\x12\x13\n\x0bsiteLimXMin\x18\r \x02(\x01\x12\x13\n\x0bsiteLimXMax\x18\x0e \x02(\x01\x12\x13\n\x0bsiteLimYMin\x18\x0f \x02(\x01\x12\x13\n\x0bsiteLimYMax\x18\x10 \x02(\x01\x12\x13\n\x0bsiteLimZMin\x18\x11 \x02(\x01\x12\x13\n\x0bsiteLimZMax\x18\x12 \x02(\x01\x12\x13\n\x0bsiteCtrTcsX\x18\x13 \x02(\x01\x12\x13\n\x0bsiteCtrTcsY\x18\x14 \x02(\x01\x12\x13\n\x0bsiteCtrTcsZ\x18\x15 \x02(\x01\x12\x13\n\x0bsensorUnits\x18\x16 \x02(\t\x12\x0e\n\x06\x61\x62sIdx\x18\x17 \x02(\x05\x12\x14\n\x0cisAudioRight\x18\x18 \x02(\x08\x12\x12\n\nsysChanIdx\x18\x19 \x02(\x05\x12\x17\n\x0fsiteAreaMicron2\x18\x1a \x01(\x01\x12\x11\n\tscsToTcsX\x18\x1b \x01(\x01\x12\x11\n\tscsToTcsY\x18\x1c \x01(\x01\x12\x11\n\tscsToTcsZ\x18\x1d \x01(\x01\x12\x10\n\x08sensorID\x18\x1e \x01(\t\x12\x0f\n\x07probeID\x18\x1f \x01(\t\x12\x13\n\x0bheadstageID\x18  \x01(\t\x12\x13\n\x0b\x64\x61tasetRidx\x18! \x01(\x05\x12\x13\n\x0b\x64\x61tasetAidx\x18\" \x01(\x05\x12\x13\n\x0bntvChanName\x18# \x01(\t\x12\x11\n\tsensorUID\x18$ \x01(\t\x12\x11\n\tsensorIdx\x18% \x01(\x05\"\x1f\n\x07XYCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"+\n\x08XYZCoord\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\x12\t\n\x01z\x18\x03 \x02(\x01\"\x81\x03\n\x06Sensor\x12\x0f\n\x07probeId\x18\x01 \x02(\t\x12\x13\n\x0bheadstageId\x18\x02 \x02(\t\x12+\n\twireframe\x18\x03 \x02(\x0b\x32\x18.allego.Sensor.WireFrame\x12\x0c\n\x04xMin\x18\x04 \x02(\x01\x12\x0c\n\x04xMax\x18\x05 \x02(\x01\x12\x0c\n\x04yMin\x18\x06 \x02(\x01\x12\x0c\n\x04yMax\x18\x07 \x02(\x01\x12+\n\x08position\x18\x08 \x02(\x0b\x32\x19.allego.SensorPositionTcs\x12\x11\n\tsensorUID\x18\t \x01(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\n \x01(\x05\x12\x10\n\x08numSites\x18\x0b \x02(\x05\x12\x11\n\tsensorIdx\x18\x0c \x01(\x05\x1am\n\tWireFrame\x12\x1c\n\x03vtx\x18\x01 \x03(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxXlim\x18\x02 \x02(\x0b\x32\x0f.allego.XYCoord\x12 \n\x07vtxYlim\x18\x03 \x02(\x0b\x32\x0f.allego.XYCoord\"\x98\x02\n\x0eSensorPortSpec\x12\x1f\n\x07sensorA\x18\x01 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorB\x18\x02 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorC\x18\x03 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorD\x18\x04 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorE\x18\x05 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorF\x18\x06 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorG\x18\x07 \x03(\x0b\x32\x0e.allego.Sensor\x12\x1f\n\x07sensorH\x18\x08 \x03(\x0b\x32\x0e.allego.Sensor\"t\n\x10SignalGroupUnits\x12\x32\n\x05units\x18\x01 \x03(\x0b\x32#.allego.SignalGroupUnits.UnitsEntry\x1a,\n\nUnitsEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\x80\x02\n\x0bSignalGroup\x12\'\n\x08\x63hannels\x18\x01 \x03(\x0b\x32\x15.allego.ChannelRecord\x12.\n\x0esensorPortSpec\x18\x02 \x02(\x0b\x32\x16.allego.SensorPortSpec\x12\x12\n\ndatasetUID\x18\x03 \x01(\t\x12\x10\n\x08sampFreq\x18\x04 \x01(\x01\x12\x13\n\x0bsourceLabel\x18\x05 \x01(\t\x12\x19\n\x11neighborMaxRadius\x18\x06 \x01(\x01\x12-\n\x0bsignalUnits\x18\x07 \x01(\x0b\x32\x18.allego.SignalGroupUnits\x12\x13\n\x0bhasDiscrete\x18\x08 \x01(\x08\"\x87\x01\n\x18\x43reateSignalGroupRequest\x12\x16\n\x0e\x64\x61taSourceName\x18\x01 \x02(\t\x12\x16\n\x0e\x64\x61taSourcePath\x18\x02 \x02(\t\x12$\n\x04type\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\x12\x15\n\rstreamGroupId\x18\x04 \x02(\t\"s\n\tSubOpSort\x12)\n\x04sort\x18\x01 \x03(\x0e\x32\x1b.allego.SubOpSort.SortField\";\n\tSortField\x12\x0e\n\nSITE_CTR_X\x10\x00\x12\x0e\n\nSITE_CTR_Y\x10\x01\x12\x0e\n\nSITE_CTR_Z\x10\x02\"\xa5\x03\n\x18UpdateSignalGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12=\n\toperation\x18\x02 \x02(\x0e\x32*.allego.UpdateSignalGroupRequest.Operation\x12\x42\n\taddRemove\x18\x03 \x01(\x0e\x32-.allego.UpdateSignalGroupRequest.SubOperationH\x00\x12#\n\x06sortOp\x18\x04 \x01(\x0b\x32\x11.allego.SubOpSortH\x00\x12\x16\n\nntvChanIdx\x18\x05 \x03(\x05\x42\x02\x10\x01\x12&\n\nsignalType\x18\x06 \x02(\x0e\x32\x12.allego.SignalType\x12\x11\n\tpropagate\x18\x07 \x01(\x08\"B\n\tOperation\x12\t\n\x05\x43OLOR\x10\x00\x12\n\n\x06SELECT\x10\x01\x12\x14\n\x10\x44\x45PRECATED_AUDIO\x10\x02\x12\x08\n\x04SORT\x10\x03\"#\n\x0cSubOperation\x12\x07\n\x03\x41\x44\x44\x10\x00\x12\n\n\x06REMOVE\x10\x01\x42\x0e\n\x0csubOperation\"T\n\x14SliceSignalGroupSpec\x12\x0e\n\x06sortBy\x18\x01 \x02(\t\x12\r\n\x05\x64\x65lim\x18\x02 \x02(\t\x12\x1d\n\x02tR\x18\x03 \x01(\x0b\x32\x11.allego.TimeRange\"X\n\x17SliceSignalGroupRequest\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12*\n\x04spec\x18\x02 \x02(\x0b\x32\x1c.allego.SliceSignalGroupSpec\"\x88\x01\n\x15SliceSignalGroupReply\x12\x11\n\tdsourceID\x18\x01 \x01(\t\x12*\n\x04spec\x18\x02 \x02(\x0b\x32\x1c.allego.SliceSignalGroupSpec\x12\x1f\n\x02sG\x18\x03 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x0f\n\x07outcome\x18\x04 \x02(\t\"\x0f\n\rLicenseStatus\"u\n\x12SetDSPGroupRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12$\n\tdspParams\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"\xf2\x02\n\tDSPParams\x12\x1d\n\x04type\x18\x01 \x02(\x0e\x32\x0f.allego.DSPType\x12\"\n\x05stage\x18\x02 \x02(\x0e\x32\x13.allego.FilterStage\x12\x0e\n\x04\x66req\x18\x03 \x01(\x01H\x00\x12\x36\n\x0c\x66reqSpecBand\x18\x04 \x01(\x0b\x32\x1e.allego.DSPParams.FreqSpecBandH\x00\x12\x17\n\rrefNtvChanIdx\x18\x08 \x01(\x05H\x00\x12\x16\n\x0enotchBandwidth\x18\x05 \x01(\x01\x12\x11\n\tuserLabel\x18\x06 \x02(\t\x12\x1a\n\x04port\x18\x07 \x02(\x0e\x32\x0c.allego.Port\x12\x18\n\x10targetNtvChanIdx\x18\t \x01(\x01\x12\r\n\x05isAux\x18\n \x02(\x08\x12\x12\n\nauxChanIdx\x18\x0b \x01(\x05\x1a\x31\n\x0c\x46reqSpecBand\x12\x0f\n\x07lowFreq\x18\x01 \x02(\x01\x12\x10\n\x08highFreq\x18\x02 \x02(\x01\x42\n\n\x08\x66reqSpec\"\x85\x01\n\x08\x44SPGroup\x12#\n\x08hardware\x18\x01 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage1\x18\x02 \x03(\x0b\x32\x11.allego.DSPParams\x12)\n\x0esoftwareStage2\x18\x03 \x03(\x0b\x32\x11.allego.DSPParams\"\x9a\x01\n\x10SetSensorRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07probeId\x18\x03 \x01(\t\x12\x13\n\x0bheadstageId\x18\x04 \x01(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\x05 \x01(\x05\x12\x13\n\x0bnumChannels\x18\x06 \x01(\x05\"m\n\x11SensorPositionTcs\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\x12\x11\n\tRingAngle\x18\x05 \x02(\x01\x12\x12\n\nAxialAngle\x18\x06 \x02(\x01\x12\x10\n\x08\x41rcAngle\x18\x07 \x02(\x01\"\x90\x01\n\x1bSetSensorPositionTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12+\n\x08position\x18\x03 \x02(\x0b\x32\x19.allego.SensorPositionTcs\x12\x11\n\tsensorIdx\x18\x04 \x01(\x05\"F\n\x0fSitePositionTcs\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\t\n\x01X\x18\x02 \x02(\x01\x12\t\n\x01Y\x18\x03 \x02(\x01\x12\t\n\x01Z\x18\x04 \x02(\x01\"\x7f\n\x1aSetSitePositionsTcsRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12.\n\rsitePositions\x18\x03 \x03(\x0b\x32\x17.allego.SitePositionTcs\"Y\n\x17\x46\x65\x61tureStartStopRequest\x12\x0e\n\x06nodeId\x18\x01 \x02(\t\x12.\n\x0e\x66\x65\x61tureLicense\x18\x02 \x02(\x0e\x32\x16.allego.FeatureLicense\"!\n\x0cPrivacyReply\x12\x11\n\tisPrivate\x18\x02 \x02(\x08\"&\n\x11SetPrivacyRequest\x12\x11\n\tisPrivate\x18\x01 \x02(\x08\"7\n\x0b\x44\x65nseMatrix\x12\x0c\n\x04rows\x18\x01 \x02(\x03\x12\x0c\n\x04\x63ols\x18\x02 \x02(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\"\\\n\tHistogram\x12\r\n\x05stats\x18\x01 \x03(\x01\x12\x0e\n\x06\x63ounts\x18\x02 \x03(\x01\x12\x10\n\x08\x64ividers\x18\x03 \x03(\x01\x12\x0f\n\x07numBins\x18\x04 \x02(\x03\x12\r\n\x05isPDF\x18\x05 \x02(\x08\"Y\n\x0bKpiMetricID\x12$\n\x04mode\x18\x01 \x02(\x0e\x32\x16.allego.KpiMetricsMode\x12$\n\x04name\x18\x02 \x02(\x0e\x32\x16.allego.KpiMetricsEnum\"\x85\x01\n\tTimeRange\x12\x14\n\x0ctimeRangeSec\x18\x01 \x03(\x01\x12\x11\n\ttimestamp\x18\x02 \x03(\x03\x12\n\n\x02\x66s\x18\x03 \x02(\x01\x12\x15\n\rwallTimeStart\x18\x04 \x01(\t\x12,\n\x08wallTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"q\n\tBundleReq\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12\x1d\n\x02tR\x18\x02 \x02(\x0b\x32\x11.allego.TimeRange\x12$\n\x07metrics\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0e\n\x06isTail\x18\x05 \x02(\x08\"\x9d\x01\n\rKpiMetricsReq\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x1e\n\x03\x61rg\x18\x03 \x02(\x0b\x32\x11.allego.BundleReq\x12\x0e\n\x06isPlot\x18\x04 \x01(\x08\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x14\n\x0cisReturnData\x18\x06 \x01(\x08\"\x83\x03\n\x0eKpiMetricsData\x12\x12\n\nnumPackets\x18\x01 \x02(\x03\x12\x0f\n\x07numSigs\x18\x02 \x02(\x03\x12\x12\n\nnumMetrics\x18\x03 \x02(\x03\x12#\n\x06metric\x18\x04 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x0f\n\x07pktIdxs\x18\x05 \x03(\x03\x12 \n\x03val\x18\x06 \x02(\x0b\x32\x13.allego.DenseMatrix\x12\x35\n\tstatsPkts\x18\x07 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x31\n\x05stats\x18\x08 \x02(\x0b\x32\".allego.KpiMetricsData.MetricStats\x12\x14\n\x0cpacketDurSec\x18\t \x02(\x01\x12\x1d\n\x02tR\x18\n \x02(\x0b\x32\x11.allego.TimeRange\x1a\x41\n\x0bMetricStats\x12\x0c\n\x04mean\x18\x01 \x03(\x01\x12\n\n\x02sD\x18\x02 \x03(\x01\x12\x0b\n\x03max\x18\x03 \x03(\x01\x12\x0b\n\x03min\x18\x04 \x03(\x01\"w\n\x16KpiBundlePacketMetrics\x12\x0f\n\x07ntvIdxs\x18\x01 \x03(\x05\x12#\n\x07sigType\x18\x02 \x02(\x0e\x32\x12.allego.SignalType\x12\'\n\x07metrics\x18\x04 \x02(\x0b\x32\x16.allego.KpiMetricsData\"S\n\nKpiMetrics\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12.\n\x06\x62undle\x18\x02 \x02(\x0b\x32\x1e.allego.KpiBundlePacketMetrics\"c\n\x11KpiControlRequest\x12\x15\n\rstreamGroupId\x18\x01 \x02(\t\x12!\n\x05stype\x18\x02 \x01(\x0e\x32\x12.allego.SignalType\x12\x14\n\x0cisAllBundles\x18\x03 \x01(\x08\":\n\x12SetKpiParamRequest\x12\x15\n\rstreamGroupId\x18\x01 \x01(\t\x12\r\n\x05param\x18\x02 \x01(\x01\",\n\x13GetKpiStatusRequest\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\"K\n\x12KpiStandardRequest\x12\x11\n\tdsourceID\x18\x02 \x03(\t\x12\"\n\x03\x63md\x18\x03 \x01(\x0e\x32\x15.allego.KpiScannerCmd\"\xba\x01\n\rKpiFileStatus\x12,\n\x07\x64source\x18\x01 \x03(\x0b\x32\x1b.allego.KpiFileStatus.State\x1a{\n\x05State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\nisComplete\x18\x02 \x01(\x08\x12\x12\n\ndsourceUID\x18\x03 \x01(\t\x12 \n\x05kpiTR\x18\x04 \x01(\x0b\x32\x11.allego.TimeRange\x12\x17\n\x0f\x66ilePathAndName\x18\x05 \x01(\t\"\xc7\x04\n\x0eKpiFileStatus2\x12>\n\x07\x64source\x18\x01 \x03(\x0b\x32-.allego.KpiFileStatus2.KpiDatasourceStateSpec\x1a\xe9\x01\n\tKPI_State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\nisComplete\x18\x02 \x01(\x08\x12\x14\n\x0c\x66racComplete\x18\x03 \x01(\x01\x12\x17\n\x0f\x66ilePathAndName\x18\x04 \x01(\t\x12 \n\x05kpiTR\x18\x05 \x01(\x0b\x32\x11.allego.TimeRange\x12\x14\n\x0cpacketDurSec\x18\x06 \x01(\x01\x12\x0e\n\x06numAmp\x18\x07 \x01(\x03\x12\x18\n\x10\x62ytesInBundlePkt\x18\x08 \x01(\x03\x12\x12\n\nnumPackets\x18\t \x01(\x03\x12\x12\n\ndatasetUID\x18\n \x01(\t\x1aq\n\x10\x44\x61tasource_State\x12\x17\n\x0f\x66ilePathAndName\x18\x01 \x01(\t\x12\x1d\n\x02TR\x18\x02 \x01(\x0b\x32\x11.allego.TimeRange\x12\x12\n\ndatasetUID\x18\x03 \x01(\t\x12\x11\n\tdsourceID\x18\x04 \x01(\t\x1a\x95\x01\n\x16KpiDatasourceStateSpec\x12\x37\n\x06source\x18\x01 \x02(\x0b\x32\'.allego.KpiFileStatus2.Datasource_State\x12-\n\x03kpi\x18\x02 \x02(\x0b\x32 .allego.KpiFileStatus2.KPI_State\x12\x13\n\x0bisSprinting\x18\x03 \x02(\x08\"\xfd\x01\n\x0fKpiFileMetadata\x12.\n\x07\x64source\x18\x01 \x03(\x0b\x32\x1d.allego.KpiFileMetadata.State\x1a\xb9\x01\n\x05State\x12\x0f\n\x07isAvail\x18\x01 \x02(\x08\x12\x12\n\ndsourceUID\x18\x02 \x01(\t\x12\x11\n\tpacketDur\x18\x03 \x01(\x01\x12\x0c\n\x04nAMP\x18\x04 \x01(\x03\x12\x1b\n\x13\x62ytesInBundlePacket\x18\x05 \x01(\x03\x12\x12\n\nnumPackets\x18\x06 \x01(\x03\x12 \n\x05kpiTR\x18\x07 \x01(\x0b\x32\x11.allego.TimeRange\x12\x17\n\x0f\x66ilePathAndName\x18\x08 \x01(\t\"\xd3\x02\n\x0eKpiStatusReply\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x11\n\ttimeRange\x18\x03 \x01(\x01\x12\x16\n\x0etimestampRange\x18\x04 \x01(\x03\x12\x18\n\x10numPacketsMemory\x18\x05 \x02(\x03\x12\x11\n\tpacketDur\x18\x06 \x02(\x01\x12\x14\n\x0cupdatePeriod\x18\x07 \x02(\x01\x12\x13\n\x0bpersistence\x18\x08 \x02(\x01\x12\x0c\n\x04\x62\x65ta\x18\t \x02(\x01\x12\x1d\n\x15isTrackingSignalCache\x18\x0b \x02(\x08\x12\x12\n\nnumPackets\x18\x0c \x02(\x03\x12\x13\n\x0bmemoryBytes\x18\r \x02(\x01\x12\n\n\x02\x66s\x18\x0e \x01(\x01\x12\x15\n\rwallTimeStart\x18\x0f \x01(\t\x12\x1d\n\x02tR\x18\x10 \x01(\x0b\x32\x11.allego.TimeRange\x12\x0f\n\x07numSigs\x18\x11 \x01(\x03\"\xe6\x02\n\x11SigKpiParamRecord\x12\x15\n\risEventDetect\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x11\n\teventThr0\x18\x03 \x02(\x01\x12\x11\n\teventThr1\x18\x04 \x02(\x01\x12\x13\n\x0b\x65ventThrSd0\x18\x05 \x02(\x01\x12\x13\n\x0b\x65ventThrSd1\x18\x06 \x02(\x01\x12\x11\n\tpreThrPts\x18\x07 \x02(\x05\x12\x12\n\npostThrPts\x18\x08 \x02(\x05\x12\x11\n\tevtDurPts\x18\t \x02(\x05\x12\x11\n\tshadowPts\x18\n \x02(\x05\x12\x0e\n\x06preThr\x18\x0b \x02(\x01\x12\x0f\n\x07postThr\x18\x0c \x02(\x01\x12\x0e\n\x06\x65vtDur\x18\r \x02(\x01\x12\x0e\n\x06shadow\x18\x0e \x02(\x01\x12\x11\n\tisSetThr0\x18\x0f \x02(\x08\x12\x11\n\tisSetThr1\x18\x10 \x02(\x08\x12\x10\n\x08isSDThr0\x18\x11 \x02(\x08\x12\x10\n\x08isSDThr1\x18\x12 \x02(\x08\"J\n\x0e\x41nnotateBundle\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\r\n\x05notes\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x01(\t\"]\n\x0fProjectMetadata\x12\x12\n\nprojectUID\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61seUID\x18\x02 \x01(\t\x12\x10\n\x08trialUID\x18\x03 \x01(\t\x12\x13\n\x0b\x61nnotateUID\x18\x04 \x03(\t\"3\n\x16SensorExtendedMetadata\x12\x19\n\x11sensorInstanceUID\x18\x01 \x01(\t\"%\n\x0fGonumMatrixList\x12\x12\n\nmdataBytes\x18\x01 \x02(\x0c\"6\n\x0fRadixMatrixList\x12#\n\x06matrix\x18\x01 \x03(\x0b\x32\x13.allego.RadixMatrix\"*\n\x0bRadixMatrix\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\x12\r\n\x05shape\x18\x02 \x03(\x05\"/\n\x10RadixMatrixBytes\x12\x0c\n\x04\x64\x61ta\x18\x01 \x02(\x0c\x12\r\n\x05shape\x18\x02 \x03(\x05\"8\n\x10RadixSignalsList\x12$\n\x06matrix\x18\x01 \x03(\x0b\x32\x14.allego.RadixSignals\"\xa9\x01\n\x0cRadixSignals\x12\x10\n\x08sampFreq\x18\x01 \x02(\x01\x12 \n\x03pri\x18\x02 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x61ux\x18\x03 \x02(\x0b\x32\x13.allego.RadixMatrix\x12 \n\x03\x64in\x18\x04 \x02(\x0b\x32\x13.allego.RadixMatrix\x12!\n\x04\x64out\x18\x05 \x02(\x0b\x32\x13.allego.RadixMatrix\"\x19\n\x0cVectorString\x12\t\n\x01x\x18\x01 \x03(\t\"\x1a\n\rVectorFloat64\x12\t\n\x01x\x18\x01 \x03(\x01\"G\n\x12VectorSliceFloat64\x12\"\n\x03vec\x18\x01 \x03(\x0b\x32\x15.allego.VectorFloat64\x12\r\n\x05label\x18\x02 \x01(\t\"\xde\x02\n\x14LogsysKpiStatusReply\x12\x1f\n\x05portA\x18\x01 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portB\x18\x02 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portC\x18\x03 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portD\x18\x04 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portE\x18\x05 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portF\x18\x06 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portG\x18\x07 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1f\n\x05portH\x18\x08 \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux0\x18\t \x02(\x0b\x32\x10.allego.KpiCache\x12\x1e\n\x04\x61ux1\x18\n \x02(\x0b\x32\x10.allego.KpiCache\"\xfc\x02\n\x08KpiCache\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x10\n\x08sampFreq\x18\x02 \x02(\x01\x12\x12\n\npersistDur\x18\x03 \x02(\x01\x12\x15\n\rminNumPackets\x18\x04 \x02(\x05\x12\x11\n\tsizeBytes\x18\x05 \x02(\x05\x12\x12\n\nnumPackets\x18\x06 \x02(\x05\x12\x0e\n\x06tRange\x18\x07 \x03(\x01\x12\x0f\n\x07tsRange\x18\x08 \x03(\x03\x12\x15\n\rmeanPacketDur\x18\t \x02(\x01\x12\x19\n\x11meanCalcPacketDur\x18\n \x02(\x01\x12\x11\n\tpacketDur\x18\x0b \x02(\x01\x12\x1d\n\x15totalPacketsProcessed\x18\x0c \x02(\r\x12\x12\n\nsignalType\x18\r \x02(\t\x12\x12\n\nnumPriSigs\x18\x0e \x02(\x05\x12\x12\n\nnumAuxSigs\x18\x0f \x02(\x05\x12\x12\n\nnumDinSigs\x18\x10 \x02(\x05\x12\x13\n\x0bnumDoutSigs\x18\x11 \x02(\x05\x12\x14\n\x0cupdatePeriod\x18\x12 \x02(\x01\"\xfa\x02\n\x12LogsysKpiTailReply\x12\"\n\x05portA\x18\x01 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portB\x18\x02 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portC\x18\x03 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portD\x18\x04 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portE\x18\x05 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portF\x18\x06 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portG\x18\x07 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12\"\n\x05portH\x18\x08 \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux0\x18\t \x01(\x0b\x32\x13.allego.KpiPortInfo\x12!\n\x04\x61ux1\x18\n \x01(\x0b\x32\x13.allego.KpiPortInfo\"3\n\x0bKpiPortInfo\x12$\n\x07kpiTail\x18\x01 \x03(\x0b\x32\x13.allego.KpiTailRows\"\xf4\x02\n\x0bKpiTailRows\x12\x10\n\x08wallTime\x18\x01 \x02(\t\x12\x11\n\ttimeRange\x18\x02 \x02(\x01\x12\x14\n\x0clocalSigType\x18\x03 \x02(\t\x12\x12\n\nntvChanIdx\x18\x04 \x02(\x03\x12\x0b\n\x03\x64ur\x18\x05 \x02(\x01\x12\x0e\n\x06stdDev\x18\x06 \x02(\x01\x12\x0f\n\x07\x63StdDev\x18\x07 \x02(\x01\x12\x11\n\tabsEvtAmp\x18\x08 \x02(\x01\x12\x12\n\ncabsEvtAmp\x18\t \x02(\x01\x12\x0b\n\x03SNR\x18\n \x02(\x01\x12\x0c\n\x04\x63SNR\x18\x0b \x02(\x01\x12\x0f\n\x07numEvts\x18\x0c \x02(\x05\x12\x10\n\x08\x63numEvts\x18\r \x02(\x05\x12\x0f\n\x07\x65vtRate\x18\x0e \x02(\x01\x12\x10\n\x08\x63\x45vtRate\x18\x0f \x02(\x01\x12\x0b\n\x03max\x18\x10 \x02(\x01\x12\x0c\n\x04\x63max\x18\x11 \x02(\x01\x12\x0b\n\x03min\x18\x12 \x02(\x01\x12\x0c\n\x04\x63min\x18\x13 \x02(\x01\x12\x14\n\x0cmeanPosPkAmp\x18\x14 \x02(\x01\x12\x14\n\x0cmeanNegPkAmp\x18\x15 \x02(\x01\"*\n\x18WarehouseHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\"(\n\x19OutfitterGetDeviceRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x9e\x01\n\x11SensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x16\n\x0eisIncludeModel\x18\x03 \x01(\x08\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"z\n\x19RegisterSensorCompRequest\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageDesc\x12\x11\n\tprofileID\x18\x03 \x02(\t\"\x92\x01\n\x1dSaveSensorCompInstanceRequest\x12 \n\x05probe\x18\x01 \x01(\x0b\x32\x11.allego.ProbeDesc\x12(\n\theadstage\x18\x02 \x01(\x0b\x32\x15.allego.HeadstageDesc\x12\x19\n\x11isIncludeMetadata\x18\x04 \x01(\x08\x12\n\n\x02iD\x18\x05 \x01(\t\"&\n\tProbeDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"*\n\rHeadstageDesc\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\x0b\n\x03uID\x18\x02 \x01(\t\"`\n\x12GetSensorCompReply\x12 \n\x05probe\x18\x01 \x03(\x0b\x32\x11.allego.ProbeSpec\x12(\n\theadstage\x18\x02 \x03(\x0b\x32\x15.allego.HeadstageSpec\"x\n\tProbeSpec\x12\x1f\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x11.allego.ProbeDesc\x12!\n\x05model\x18\x02 \x01(\x0b\x32\x12.allego.ProbeModel\x12\'\n\x08metaData\x18\x03 \x01(\x0b\x32\x15.allego.ProbeMetaData\"\x88\x01\n\rHeadstageSpec\x12#\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x15.allego.HeadstageDesc\x12%\n\x05model\x18\x02 \x01(\x0b\x32\x16.allego.HeadstageModel\x12+\n\x08metaData\x18\x03 \x01(\x0b\x32\x19.allego.HeadstageMetaData\"\xce\x04\n\nProbeModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12.\n\x04site\x18\x02 \x03(\x0b\x32 .allego.ProbeModel.ProbeSiteDesc\x12\x34\n\twireframe\x18\x03 \x02(\x0b\x32!.allego.ProbeModel.ProbeWireFrame\x12\x34\n\x0esiteOverallMin\x18\x05 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x34\n\x0esiteOverallMax\x18\x06 \x02(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x1a\xde\x01\n\rProbeSiteDesc\x12\x0c\n\x04\x61rea\x18\x01 \x02(\x01\x12\x0f\n\x07\x63\x65nterX\x18\x02 \x02(\x01\x12\x0f\n\x07\x63\x65nterY\x18\x03 \x02(\x01\x12\x0f\n\x07\x63\x65nterZ\x18\x04 \x02(\x01\x12\x11\n\tlimitXMax\x18\x05 \x02(\x01\x12\x11\n\tlimitXMin\x18\x06 \x02(\x01\x12\x11\n\tlimitYMax\x18\x07 \x02(\x01\x12\x11\n\tlimitYMin\x18\x08 \x02(\x01\x12\x11\n\tlimitZMax\x18\t \x02(\x01\x12\x11\n\tlimitZMin\x18\n \x02(\x01\x12\x0b\n\x03num\x18\x0b \x02(\x03\x12\r\n\x05shape\x18\x0c \x02(\t\x1a^\n\x0eProbeWireFrame\x12,\n\x06vertex\x18\x01 \x03(\x0b\x32\x1c.allego.ProbeModel.ProbePtXY\x12\x0e\n\x06limitX\x18\x02 \x03(\x01\x12\x0e\n\x06limitY\x18\x03 \x03(\x01\x1a!\n\tProbePtXY\x12\t\n\x01x\x18\x01 \x02(\x01\x12\t\n\x01y\x18\x02 \x02(\x01\"_\n\rProbeMetaData\x12\x11\n\tprobeName\x18\x01 \x02(\t\x12\x10\n\x08numSites\x18\x02 \x02(\x05\x12\x13\n\x0b\x63\x61talogTags\x18\x03 \x02(\t\x12\x14\n\x0cinstanceTags\x18\x04 \x02(\t\"\x84\x01\n\x0eHeadstageModel\x12\n\n\x02iD\x18\x01 \x02(\t\x12\x31\n\x04rows\x18\x02 \x03(\x0b\x32#.allego.HeadstageModel.HeadstageRow\x1a\x33\n\x0cHeadstageRow\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x03\x12\x0f\n\x07siteNum\x18\x02 \x02(\x03\"\x13\n\x11HeadstageMetaData\"5\n\x0bUserProfile\x12\x11\n\tprofileID\x18\x01 \x02(\t\x12\x13\n\x0blicenseCode\x18\x02 \x02(\t\"B\n\x16GetCurrentProfileReply\x12(\n\x0buserProfile\x18\x01 \x02(\x0b\x32\x13.allego.UserProfile\"@\n\x13GetAllProfilesReply\x12)\n\x0cuserProfiles\x18\x01 \x03(\x0b\x32\x13.allego.UserProfile\"-\n\x18SetCurrentProfileRequest\x12\x11\n\tprofileID\x18\x01 \x02(\t\"\x88\x01\n\x14ManageNodeOrgPayload\x12\r\n\x05orgID\x18\x01 \x01(\t\x12\x0f\n\x07orgName\x18\x02 \x01(\t\x12\x14\n\x0corgShortName\x18\x03 \x01(\t\x12\x0c\n\x04\x63ity\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\r\n\x05state\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"i\n\x14ManageNodeOrgRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\"S\n\x12ManageNodeOrgReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\xa2\x01\n\x14ManageNodeLabPayload\x12\r\n\x05labID\x18\x01 \x01(\t\x12\x0f\n\x07labDesc\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65pt\x18\x03 \x01(\t\x12\x14\n\x0corganization\x18\x04 \x01(\t\x12\x0f\n\x07\x61\x64minID\x18\x05 \x01(\t\x12\x11\n\tlabHeadID\x18\x06 \x01(\t\x12\x14\n\x0clabManagerID\x18\x07 \x01(\t\x12\x0c\n\x04tags\x18\x08 \x01(\t\"i\n\x14ManageNodeLabRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12-\n\x07payload\x18\x02 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\"S\n\x12ManageNodeLabReply\x12-\n\x07payload\x18\x01 \x03(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"\x99\x01\n\x15ManageNodeUserPayload\x12\x0e\n\x06userID\x18\x01 \x01(\t\x12\x0c\n\x04Name\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\x0c\x12\"\n\x04role\x18\x04 \x01(\x0e\x32\x14.allego.UserRoleType\x12\r\n\x05\x65mail\x18\x05 \x01(\t\x12\x0f\n\x07labName\x18\x06 \x01(\t\x12\x0c\n\x04tags\x18\x07 \x01(\t\"k\n\x15ManageNodeUserRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12.\n\x07payload\x18\x02 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\"U\n\x13ManageNodeUserReply\x12.\n\x07payload\x18\x01 \x03(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12\x0e\n\x06\x65rrMsg\x18\x02 \x01(\t\"6\n\x13\x43\x61talogProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"]\n\x10ProbeNodeRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.ManageNodeCmd\x12%\n\x07payload\x18\x02 \x03(\x0b\x32\x14.allego.ProbePayload\"7\n\x0eProbeNodeReply\x12%\n\x07payload\x18\x01 \x03(\x0b\x32\x14.allego.ProbePayload\"/\n\x0cProbePayload\x12\x1f\n\x04spec\x18\x01 \x02(\x0b\x32\x11.allego.ProbeSpec\"\xa5\x02\n\x0b\x45\x64gePayload\x12/\n\x06source\x18\x01 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12/\n\x06target\x18\x02 \x02(\x0b\x32\x1f.allego.EdgePayload.GenericNode\x12)\n\tedgeLabel\x18\x03 \x02(\x0e\x32\x16.allego.WorldEdgeLabel\x12-\n\tdirection\x18\x04 \x02(\x0e\x32\x1a.allego.WorldEdgeDirection\x1aZ\n\x0bGenericNode\x12%\n\x05label\x18\x01 \x02(\x0e\x32\x16.allego.WorldNodeLabel\x12\x11\n\tidPropKey\x18\x02 \x02(\t\x12\x11\n\tidPropVal\x18\x03 \x02(\t\"8\n\x10WorldEdgeRequest\x12$\n\x07payload\x18\x01 \x03(\x0b\x32\x13.allego.EdgePayload\"\x10\n\x0eWorldEdgeReply\"E\n\x11QueryWorldRequest\x12\"\n\x03\x63md\x18\x01 \x02(\x0e\x32\x15.allego.WorldQueryCmd\x12\x0c\n\x04\x61rgs\x18\x02 \x03(\t\"\xe6\x01\n\rQueryWorldRec\x12)\n\x03org\x18\x01 \x01(\x0b\x32\x1c.allego.ManageNodeOrgPayload\x12)\n\x03lab\x18\x02 \x01(\x0b\x32\x1c.allego.ManageNodeLabPayload\x12+\n\x04user\x18\x03 \x01(\x0b\x32\x1d.allego.ManageNodeUserPayload\x12-\n\x08\x63\x61tProbe\x18\x04 \x01(\x0b\x32\x1b.allego.CatalogProbePayload\x12#\n\x05probe\x18\x05 \x01(\x0b\x32\x14.allego.ProbePayload\"9\n\x0fQueryWorldReply\x12&\n\x07payload\x18\x01 \x03(\x0b\x32\x15.allego.QueryWorldRec\"/\n\x1aHighLowPassTransformParams\x12\x11\n\tfrequency\x18\x01 \x02(\x01\"B\n\x13\x42\x61ndTransformParams\x12\x14\n\x0clowFrequency\x18\x01 \x02(\x01\x12\x15\n\rhighFrequency\x18\x02 \x02(\x01\"F\n\x14NotchTransformParams\x12\x16\n\x0enotchFrequency\x18\x01 \x02(\x01\x12\x16\n\x0enotchBandwidth\x18\x02 \x02(\x01\"\x14\n\x12\x43\x41RTransformParams\"2\n\x19VirtualRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\"K\n\x18PairedRefTransformParams\x12\x15\n\rrefNtvChanIdx\x18\x01 \x02(\x05\x12\x18\n\x10targetNtvChanIdx\x18\x02 \x02(\x05\"i\n\x1d\x44\x61taSourceSinkTransformParams\x12\x10\n\x08\x64srcName\x18\x01 \x02(\t\x12\x0c\n\x04path\x18\x02 \x02(\t\x12(\n\x08\x66ileType\x18\x03 \x02(\x0e\x32\x16.allego.RadixFileTypes\">\n\x18SliceTimeTransformParams\x12\x11\n\ttimeStart\x18\x01 \x02(\x01\x12\x0f\n\x07timeEnd\x18\x02 \x02(\x01\"n\n\x1cSliceChannelsTransformParams\x12\x13\n\x0bsysChanIdxs\x18\x01 \x03(\x05\x12(\n\x0bsignalGroup\x18\x02 \x01(\x0b\x32\x13.allego.SignalGroup\x12\x0f\n\x07\x64srcUid\x18\x03 \x01(\t\"1\n\x19\x44ownsampleTransformParams\x12\x14\n\x0csampleFactor\x18\x01 \x02(\x05\"\xec\x01\n\x1aRemapSensorTransformParams\x12>\n\x07sensors\x18\x01 \x03(\x0b\x32-.allego.RemapSensorTransformParams.SensorSpec\x12\x0f\n\x07\x64srcUid\x18\x03 \x01(\t\x1a}\n\nSensorSpec\x12\x1a\n\x04port\x18\x02 \x02(\x0e\x32\x0c.allego.Port\x12\x0f\n\x07probeId\x18\x03 \x02(\t\x12\x13\n\x0bheadstageId\x18\x04 \x02(\t\x12\x18\n\x10\x63onnectionNtvIdx\x18\x05 \x01(\x05\x12\x13\n\x0bnumChannels\x18\x06 \x01(\x05\" \n\x08Position\x12\t\n\x01x\x18\x01 \x02(\x05\x12\t\n\x01y\x18\x02 \x02(\x05\"\x98\x06\n\rTransformNode\x12\n\n\x02id\x18\x01 \x02(\t\x12\'\n\x04type\x18\x02 \x02(\x0e\x32\x19.allego.TransformNodeType\x12\"\n\x08position\x18\x03 \x01(\x0b\x32\x10.allego.Position\x12\x0f\n\x07invalid\x18\x04 \x02(\x08\x12\x14\n\x0c\x65rrorMessage\x18\x05 \x01(\t\x12=\n\x11highLowPassParams\x18\x06 \x01(\x0b\x32\".allego.HighLowPassTransformParams\x12/\n\nbandParams\x18\x07 \x01(\x0b\x32\x1b.allego.BandTransformParams\x12\x31\n\x0bnotchParams\x18\x08 \x01(\x0b\x32\x1c.allego.NotchTransformParams\x12-\n\tcarParams\x18\t \x01(\x0b\x32\x1a.allego.CARTransformParams\x12;\n\x10virtualRefParams\x18\n \x01(\x0b\x32!.allego.VirtualRefTransformParams\x12\x39\n\x0fpairedRefParams\x18\x0b \x01(\x0b\x32 .allego.PairedRefTransformParams\x12\x43\n\x14\x64\x61tasourceSinkParams\x18\x0c \x01(\x0b\x32%.allego.DataSourceSinkTransformParams\x12\x39\n\x0fsliceTimeParams\x18\r \x01(\x0b\x32 .allego.SliceTimeTransformParams\x12\x41\n\x13sliceChannelsParams\x18\x0e \x01(\x0b\x32$.allego.SliceChannelsTransformParams\x12;\n\x10\x64ownsampleParams\x18\x0f \x01(\x0b\x32!.allego.DownsampleTransformParams\x12=\n\x11remapSensorParams\x18\x10 \x01(\x0b\x32\".allego.RemapSensorTransformParams\";\n\rTransformEdge\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0e\n\x06source\x18\x02 \x02(\t\x12\x0e\n\x06target\x18\x03 \x02(\t\"t\n\x08Protocol\x12\n\n\x02id\x18\x01 \x02(\t\x12-\n\x0etransformNodes\x18\x02 \x03(\x0b\x32\x15.allego.TransformNode\x12-\n\x0etransformEdges\x18\x03 \x03(\x0b\x32\x15.allego.TransformEdge\"%\n\x0fProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\"B\n\x15RenameProtocolRequest\x12\x12\n\nprotocolID\x18\x01 \x02(\t\x12\x15\n\rnewProtocolID\x18\x02 \x02(\t\";\n\x14GetAllProtocolsReply\x12#\n\tprotocols\x18\x01 \x03(\x0b\x32\x10.allego.Protocol\"{\n\x15\x41pplyProtocolProgress\x12\x1c\n\x14lastTimestampWritten\x18\x01 \x02(\x05\x12\x18\n\x10\x64srcTimestampEnd\x18\x02 \x02(\x05\x12\x14\n\x0c\x66racComplete\x18\x03 \x01(\x01\x12\x14\n\x0cincrementSec\x18\x04 \x01(\x01\"\x9a\x01\n\x1aSpikeSorterSetParamRequest\x12\x15\n\rspikeSorterID\x18\x01 \x02(\t\x12,\n\x03\x63md\x18\x02 \x02(\x0e\x32\x1f.allego.SpikeSorterParamCommand\x12\x12\n\nregFloat64\x18\x03 \x03(\x01\x12\x0f\n\x07regBool\x18\x05 \x03(\x08\x12\x12\n\nntvChanIdx\x18\x06 \x03(\x05\"Q\n\x1bSpikeSorterSetParamsRequest\x12\x32\n\x06params\x18\x01 \x03(\x0b\x32\".allego.SpikeSorterSetParamRequest\"\xa7\x02\n\x1dSpikeSorterParamCommandRecord\x12\x11\n\tisEnabled\x18\x01 \x02(\x08\x12\x12\n\nntvChanIdx\x18\x02 \x02(\x05\x12\x0b\n\x03thr\x18\x03 \x03(\x01\x12\r\n\x05thrSd\x18\x04 \x03(\x01\x12\x11\n\tthrWdwPts\x18\x05 \x03(\x05\x12\x0e\n\x06thrWdw\x18\x06 \x03(\x01\x12\x0e\n\x06shadow\x18\x07 \x02(\x01\x12\x11\n\tshadowPts\x18\x08 \x02(\x05\x12\x10\n\x08isSetThr\x18\t \x03(\x08\x12\x0f\n\x07weakThr\x18\n \x03(\x01\x12\x11\n\tweakThrSd\x18\x0b \x03(\x01\x12\x14\n\x0cisSetWeakThr\x18\x0c \x03(\x08\x12\x12\n\npeakWdwPts\x18\r \x03(\x05\x12\x0f\n\x07peakWdw\x18\x0e \x03(\x01\x12\x0c\n\x04isSD\x18\x0f \x02(\x08\"?\n\tKpiParams\x12\x32\n\x03rec\x18\x01 \x03(\x0b\x32%.allego.SpikeSorterParamCommandRecord\"J\n\x10\x44\x41\x43StreamRequest\x12\x0b\n\x03\x44\x41\x43\x18\x01 \x02(\x05\x12\x12\n\nNtvChanIdx\x18\x02 \x02(\x05\x12\x15\n\rstreamGroupId\x18\x03 \x01(\t\"\xde\x01\n\x11\x45ventViewerConfig\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\x12\x19\n\x11triggerSysChanIdx\x18\x03 \x01(\x05\x12\x1a\n\x12triggerThresholdUV\x18\x04 \x01(\x01\x12\x14\n\x0cpreTriggerMs\x18\x05 \x02(\x01\x12\x15\n\rpostTriggerMs\x18\x06 \x02(\x01\x12\'\n\x0btriggerType\x18\x07 \x01(\x0e\x32\x12.allego.SignalType\x12\x0e\n\x06ntvIdx\x18\x08 \x01(\x05\"=\n\rEventViewerID\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x15\n\rstreamGroupId\x18\x02 \x02(\t\"D\n\x1aGetEventViewerEventRequest\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12\x0f\n\x07\x65ventId\x18\x02 \x02(\t\"Y\n\x14\x45ventViewerEventDesc\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\"\x8f\x01\n\x10\x45ventViewerEvent\x12\x0f\n\x07\x65ventId\x18\x01 \x02(\t\x12\x18\n\x10triggerTimestamp\x18\x02 \x02(\x03\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12#\n\x07signals\x18\x04 \x02(\x0b\x32\x12.allego.RawSignals\x12\x13\n\x0bsysChanIdxs\x18\x05 \x03(\x05\"a\n\x1aListEventViewerEventsReply\x12\x15\n\reventViewerId\x18\x01 \x02(\t\x12,\n\x06\x65vents\x18\x02 \x03(\x0b\x32\x1c.allego.EventViewerEventDesc\"D\n\x15ListEventViewersReply\x12+\n\x0c\x65ventViewers\x18\x01 \x03(\x0b\x32\x15.allego.EventViewerID\"3\n\x1fStatusPollFieldsToUpdateRequest\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\"^\n\x18StatusPollFieldsToUpdate\x12\x10\n\x08\x63lientId\x18\x01 \x02(\t\x12\x30\n\x0e\x66ieldsToUpdate\x18\x02 \x03(\x0e\x32\x18.allego.StatusPollFields\"\xa5\x01\n\x17\x44\x61shboardCommandRequest\x12\'\n\x08\x64\x61shType\x18\x01 \x01(\x0e\x32\x15.allego.DashboardType\x12\x32\n\x04\x61rgs\x18\x02 \x01(\x0b\x32$.allego.DashboardCommandRequest.Args\x1a-\n\x04\x41rgs\x12%\n\x03\x63md\x18\x01 \x02(\x0e\x32\x18.allego.DashboardCommand\"]\n\x13SelTableSignalGroup\x12\r\n\x05index\x18\x01 \x02(\t\x12\x15\n\rcriterionDesc\x18\x02 \x02(\t\x12\x0f\n\x07ntvIdxs\x18\x03 \x03(\x03\x12\x0f\n\x07numSigs\x18\x04 \x02(\x03\"?\n\x13SelectorTablesReply\x12(\n\x03sig\x18\x01 \x03(\x0b\x32\x1b.allego.SelTableSignalGroup\"\xfa\x02\n\x10\x44\x61taSourceStatus\x12%\n\x04type\x18\x01 \x02(\x0e\x32\x17.allego.SignalGroupType\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x16\n\x0etimestampRange\x18\x03 \x03(\x03\x12\x10\n\x08\x64uration\x18\x04 \x02(\x01\x12(\n\x0bsignalGroup\x18\x06 \x02(\x0b\x32\x13.allego.SignalGroup\x12\x17\n\x0fnumTotalSamples\x18\x07 \x02(\x03\x12\x12\n\nsampleFreq\x18\t \x01(\x01\x12\x0b\n\x03uid\x18\n \x02(\t\x12\x16\n\x0e\x64\x61taSourceType\x18\x0b \x02(\t\x12\x10\n\x08\x66ileType\x18\x0c \x02(\t\x12\x0c\n\x04mode\x18\r \x02(\t\x12\r\n\x05label\x18\x0e \x02(\t\x12\x0c\n\x04path\x18\x0f \x02(\t\x12\x14\n\x0c\x62\x61seFileName\x18\x10 \x02(\t\x12\x1d\n\x02tR\x18\x11 \x01(\x0b\x32\x11.allego.TimeRange\x12\x14\n\x0ckpiDsourceID\x18\x12 \x01(\t*\x96\x02\n\x0eRadixFileTypes\x12\x07\n\x03RHD\x10\x00\x12\x08\n\x04XDAT\x10\x01\x12\x07\n\x03\x43SV\x10\x02\x12\x08\n\x04HDF5\x10\x03\x12\x08\n\x04NEX5\x10\x04\x12\x07\n\x03NWB\x10\x05\x12\x10\n\x0c\x42IOINTERFACE\x10\x07\x12\r\n\tKILOSORT2\x10\x08\x12\x07\n\x03\x41NC\x10\t\x12\x0f\n\x0bSPKTRAIN_MU\x10\n\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_HDF5\x10\x0b\x12\x1b\n\x17\x42IO_RADIENS_EXPORT_MAT5\x10\x0c\x12\x07\n\x03NSX\x10\r\x12\x07\n\x03PL2\x10\x0e\x12\x07\n\x03TDT\x10\x0f\x12\n\n\x06SPIKES\x10\x10\x12\x07\n\x03KPI\x10\x11\x12\x15\n\x11UNKNOWN_FILE_TYPE\x10\x12\x12\x0f\n\x0bMEAREC_HDF5\x10\x13*1\n\nSignalType\x12\x07\n\x03PRI\x10\x00\x12\x07\n\x03\x41UX\x10\x01\x12\x07\n\x03\x44IN\x10\x02\x12\x08\n\x04\x44OUT\x10\x03*:\n\x0fResampleRoutine\x12\t\n\x05NAIVE\x10\x00\x12\r\n\tRETENTIVE\x10\x01\x12\r\n\tANTIALIAS\x10\x03*>\n\x04Port\x12\x05\n\x01\x41\x10\x00\x12\x05\n\x01\x42\x10\x01\x12\x05\n\x01\x43\x10\x02\x12\x05\n\x01\x44\x10\x03\x12\x05\n\x01\x45\x10\x04\x12\x05\n\x01\x46\x10\x05\x12\x05\n\x01G\x10\x06\x12\x05\n\x01H\x10\x07*2\n\x0cWorkspaceApp\x12\n\n\x06\x41llego\x10\x00\x12\n\n\x06\x43urate\x10\x01\x12\n\n\x06Videre\x10\x02*\xa0\x01\n\x11WorkspaceCommands\x12\x0f\n\x0bWSPACE_Save\x10\x00\x12\x11\n\rWSPACE_SaveAs\x10\x01\x12\x11\n\rWSPACE_Export\x10\x02\x12\x11\n\rWSPACE_Import\x10\x03\x12\x11\n\rWSPACE_Delete\x10\x04\x12\x11\n\rWSPACE_Switch\x10\x07\x12\x1b\n\x17WSPACE_SwitchToLastUsed\x10\x08*C\n\x14GetWorkspaceCommands\x12\x13\n\x0fGET_WSPACE_List\x10\x01\x12\x16\n\x12GET_WSPACE_Current\x10\x02*8\n\x11RadiensServerType\x12\x10\n\x0c\x41llegoserver\x10\x00\x12\x11\n\rRadiensserver\x10\x01*\xae\x01\n\x0fGrpcServiceType\x12\x0f\n\x0b\x41LLEGO_CORE\x10\x00\x12\x11\n\rALLEGO_PCACHE\x10\x01\x12\x0e\n\nALLEGO_KPI\x10\x02\x12\x12\n\x0e\x41LLEGO_NEURONS\x10\x03\x12\x10\n\x0cRADIENS_CORE\x10\x04\x12\x18\n\x14RADIENS_SPIKE_SORTER\x10\x05\x12\x0f\n\x0bRADIENS_DEV\x10\x06\x12\x16\n\x12RADIENS_DASHBOARDS\x10\x07*?\n\x0e\x44\x65vDatasetType\x12\x08\n\x04\x42\x41SE\x10\x00\x12\t\n\x05TRAIN\x10\x01\x12\x0e\n\nVALIDATION\x10\x02\x12\x08\n\x04TEST\x10\x03*C\n\rPSDWindowType\x12\x0f\n\x0bHAMMING_p01\x10\x00\x12\x0f\n\x0bHAMMING_p05\x10\x01\x12\x10\n\x0cPASS_THROUGH\x10\x02*\x1e\n\nPSDScaling\x12\x10\n\x0cPSD_ABSOLUTE\x10\x00*X\n\x0e\x44\x61taSourceSort\x12\x10\n\x0c\x44SOURCE_DATE\x10\x00\x12\x10\n\x0c\x44SOURCE_NAME\x10\x01\x12\x10\n\x0c\x44SOURCE_SIZE\x10\x02\x12\x10\n\x0c\x44SOURCE_TYPE\x10\x03*.\n\x0fSignalGroupType\x12\x11\n\rPRIMARY_CACHE\x10\x00\x12\x08\n\x04\x46ILE\x10\x03*\x81\x01\n\x07\x44SPType\x12\x0b\n\x07LOWPASS\x10\x00\x12\x0c\n\x08HIGHPASS\x10\x01\x12\x0c\n\x08\x42\x41NDPASS\x10\x02\x12\t\n\x05NOTCH\x10\x03\x12\x0c\n\x08\x42\x41NDSTOP\x10\x04\x12\x07\n\x03\x43\x41R\x10\x05\x12\x15\n\x11VIRTUAL_REFERENCE\x10\x06\x12\x14\n\x10PAIRED_REFERENCE\x10\x07*9\n\x0b\x46ilterStage\x12\x12\n\x0eSTAGE_HARDWARE\x10\x00\x12\n\n\x06STAGE1\x10\x01\x12\n\n\x06STAGE2\x10\x02*\xd3\x02\n\x0e\x46\x65\x61tureLicense\x12\x1a\n\x16\x46\x65\x61t_NoLicenseRequired\x10\x00\x12\x0c\n\x08\x46\x65\x61t_Any\x10\x01\x12\x0f\n\x0b\x46\x65\x61t_Power9\x10\x02\x12\x11\n\rFeat_RadixAPI\x10\x03\x12\x0e\n\nFeat_Scope\x10\x04\x12\x13\n\x0f\x46\x65\x61t_Electrodes\x10\x05\x12\x13\n\x0f\x46\x65\x61t_HDSnapshot\x10\x06\x12\x12\n\x0e\x46\x65\x61t_Impedance\x10\x07\x12\x10\n\x0c\x46\x65\x61t_Monitor\x10\x08\x12\x16\n\x12\x46\x65\x61t_SignalMetrics\x10\t\x12\x19\n\x15\x46\x65\x61t_SignalProcessing\x10\n\x12\x0f\n\x0b\x46\x65\x61t_System\x10\x0b\x12\x12\n\x0e\x46\x65\x61t_SpikeGrid\x10\x0c\x12\x14\n\x10\x46\x65\x61t_SpikeSorter\x10\r\x12\x0f\n\x0b\x46\x65\x61t_Raster\x10\x0e\x12\x14\n\x10\x46\x65\x61t_ThreeDModel\x10\x0f*\xed\x01\n\x10SummaryStatsEnum\x12\x10\n\x0cSS_STAT_MEAN\x10\x00\x12\x0e\n\nSS_STAT_SD\x10\x01\x12\x10\n\x0cSS_STAT_MODE\x10\x02\x12\x0f\n\x0bSS_STAT_MIN\x10\x03\x12\x0f\n\x0bSS_STAT_MAX\x10\x04\x12\x16\n\x12SS_STAT_MODE_COUNT\x10\x05\x12\x12\n\x0eSS_STAT_MEDIAN\x10\x06\x12\x0f\n\x0bSS_STAT_Q25\x10\x07\x12\x0f\n\x0bSS_STAT_Q75\x10\x08\x12\x10\n\x0cSS_STAT_SKEW\x10\t\x12\x14\n\x10SS_STAT_KURTOSIS\x10\n\x12\r\n\tSS_STAT_N\x10\x0b*_\n\x0eKpiMetricsMode\x12\x18\n\x14Kpi_MetricsMode_Base\x10\x00\x12\x17\n\x13Kpi_MetricsMode_Avg\x10\x01\x12\x1a\n\x16Kpi_MetricsMode_Stream\x10\x02*\xa1\x06\n\x0eKpiMetricsEnum\x12\x0f\n\x0bKPI_NUM_PTS\x10\x00\x12\x13\n\x0fKPI_NUM_PTS_ISI\x10\x01\x12\x0f\n\x0bKPI_DUR_SEC\x10\x02\x12\x0c\n\x08KPI_MEAN\x10\x03\x12\x0b\n\x07KPI_MIN\x10\x04\x12\x0f\n\x0bKPI_MIN_ISI\x10\x05\x12\x0b\n\x07KPI_MAX\x10\x06\x12\x0f\n\x0bKPI_MAX_ISI\x10\x07\x12\x0f\n\x0bKPI_MAX_ABS\x10\x08\x12\x13\n\x0fKPI_MAX_ABS_ISI\x10\t\x12\x15\n\x11KPI_TIMESTAMP_MIN\x10\n\x12\x15\n\x11KPI_TIMESTAMP_MAX\x10\x0b\x12\x18\n\x14KPI_MAX_MIN_DIFF_ABS\x10\x0c\x12\x1c\n\x18KPI_MAX_MIN_DIFF_ABS_ISI\x10\r\x12\n\n\x06KPI_SD\x10\x0e\x12\x0e\n\nKPI_SD_ISI\x10\x0f\x12\x0b\n\x07KPI_VAR\x10\x10\x12\x0f\n\x0bKPI_VAR_ISI\x10\x11\x12\x0b\n\x07KPI_RMS\x10\x12\x12\x0f\n\x0bKPI_RMS_ISI\x10\x13\x12\x10\n\x0cKPI_NOISE_UV\x10\x14\x12\x0b\n\x07KPI_SNR\x10\x15\x12\x12\n\x0eKPI_NUM_EVENTS\x10\x16\x12\x12\n\x0eKPI_EVENT_RATE\x10\x17\x12\x11\n\rKPI_EVENT_MAX\x10\x18\x12\x11\n\rKPI_EVENT_MIN\x10\x19\x12\x15\n\x11KPI_EVENT_MAX_ABS\x10\x1a\x12\x1e\n\x1aKPI_EVENT_MAX_MIN_DIFF_ABS\x10\x1b\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MIN\x10\x1c\x12\x1b\n\x17KPI_EVENT_TIMESTAMP_MAX\x10\x1d\x12\x1f\n\x1bKPI_EVENT_TIMESTAMP_MAX_ABS\x10\x1e\x12(\n$KPI_EVENT_TIMESTAMP_MAX_MIN_DIFF_ABS\x10\x1f\x12\x10\n\x0cKPI_MEAN_MAX\x10 \x12\x10\n\x0cKPI_MEAN_MIN\x10!\x12\x14\n\x10KPI_MEAN_MAX_ABS\x10\"\x12#\n\x1fKPI_EVENT_MEAN_MAX_MIN_DIFF_ABS\x10#\x12\"\n\x1eKPI_MAX_MIN_DIFF_ABS_AMPLIFIED\x10$*\x8b\x01\n\x13KpiMetricsStatsEnum\x12\x1e\n\x1aKPI_BDL_METRICS_STATS_MEAN\x10\x00\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MAX\x10\x01\x12\x1d\n\x19KPI_BDL_METRICS_STATS_MIN\x10\x02\x12\x16\n\x12KPI_BDL_METRICS_SD\x10\x03*\xc0\x02\n\x19KpiBundlePacketsStatsEnum\x12\x14\n\x10KPI_BDL_NUM_SIGS\x10\x00\x12\x13\n\x0fKPI_BDL_DUR_SEC\x10\x01\x12\x1d\n\x19KPI_BDL_NUM_SIGS_W_EVENTS\x10\x02\x12\x15\n\x11KPI_BDL_SIG_YIELD\x10\x03\x12\x13\n\x0fKPI_BDL_RMS_AVG\x10\x04\x12\x13\n\x0fKPI_BDL_SNR_AVG\x10\x05\x12\x13\n\x0fKPI_BDL_SIG_MAX\x10\x06\x12\x13\n\x0fKPI_BDL_SIG_MIN\x10\x07\x12\x18\n\x14KPI_BDL_NOISE_UV_AVG\x10\x08\x12\x1c\n\x18KPI_BDL_NUM_EVENTS_TOTAL\x10\t\x12\x1a\n\x16KPI_BDL_NUM_EVENTS_AVG\x10\n\x12\x1a\n\x16KPI_BDL_EVENT_RATE_AVG\x10\x0b*F\n\x10TimeRangeSelMode\x12\x0e\n\nTRS_SUBSET\x10\x00\x12\x0f\n\x0bTRS_TO_HEAD\x10\x01\x12\x11\n\rTRS_FROM_HEAD\x10\x02*e\n\rKpiScannerCmd\x12\x13\n\x0fKPI_SCANNER_OFF\x10\x00\x12\x1e\n\x1aKPI_SCANNER_BESPOKE_SPRINT\x10\x01\x12\x1f\n\x1bKPI_SCANNER_STANDARD_SPRINT\x10\x02*N\n\x16OutfitterComponentType\x12\x16\n\x12OUTFIT_COMP_SENSOR\x10\x00\x12\x1c\n\x18OUTFIT_COMP_SPIKE_SORTER\x10\x01*}\n\x0eWorldNodeLabel\x12\x12\n\x0eWORLD_NODE_ORG\x10\x01\x12\x12\n\x0eWORLD_NODE_LAB\x10\x02\x12\x13\n\x0fWORLD_NODE_USER\x10\x03\x12\x18\n\x14WORLD_NODE_CAT_PROBE\x10\x04\x12\x14\n\x10WORLD_NODE_PROBE\x10\x05*\'\n\x0eWorldEdgeLabel\x12\x15\n\x11WORLD_EDGE_MEMBER\x10\x01*`\n\x12WorldEdgeDirection\x12\x18\n\x14WORLD_EDGE_DIR_RIGHT\x10\x01\x12\x17\n\x13WORLD_EDGE_DIR_LEFT\x10\x02\x12\x17\n\x13WORLD_EDGE_DIR_BOTH\x10\x03*\x9f\x01\n\x0cUserRoleType\x12\x0b\n\x07USER_PI\x10\x01\x12\x12\n\x0eUSER_SCIENTIST\x10\x02\x12\x11\n\rUSER_POST_DOC\x10\x03\x12\x15\n\x11USER_GRAD_STUDENT\x10\x04\x12\x13\n\x0fUSER_UG_STUDENT\x10\x05\x12\x10\n\x0cUSER_MANAGER\x10\x06\x12\r\n\tUSER_TECH\x10\x07\x12\x0e\n\nUSER_OTHER\x10\x08*G\n\rManageNodeCmd\x12\x10\n\x0cNODE_CMD_NEW\x10\x01\x12\x12\n\x0eNODE_CMD_MERGE\x10\x02\x12\x10\n\x0cNODE_CMD_DEL\x10\x03*\xe8\x01\n\rWorldQueryCmd\x12\x15\n\x11WQ_LIST_ALL_USERS\x10\x01\x12\x14\n\x10WQ_LIST_ALL_LABS\x10\x02\x12\x14\n\x10WQ_LIST_ALL_ORGS\x10\x03\x12\x1a\n\x16WQ_LIST_ALL_CAT_PROBES\x10\x04\x12\x16\n\x12WQ_LIST_ALL_PROBES\x10\x05\x12\x18\n\x14WQ_CAT_PROBE_BY_NAME\x10\x06\x12\x11\n\rWQ_USER_BY_ID\x10\x07\x12\x19\n\x15WQ_USER_AND_LAB_BY_ID\x10\x08\x12\x18\n\x14WQ2_LIST_ALL_DEVICES\x10\x1e*\x82\x02\n\x11TransformNodeType\x12\x10\n\x0cNOTCH_FILTER\x10\x00\x12\x13\n\x0f\x42\x41NDPASS_FILTER\x10\x01\x12\x13\n\x0f\x42\x41NDSTOP_FILTER\x10\x02\x12\x13\n\x0fHIGHPASS_FILTER\x10\x03\x12\x12\n\x0eLOWPASS_FILTER\x10\x04\x12\x0e\n\nPAIRED_REF\x10\x05\x12\x0f\n\x0bVIRTUAL_REF\x10\x06\x12\x0b\n\x07\x43\x41R_REF\x10\x07\x12\x0e\n\nSLICE_TIME\x10\t\x12\x12\n\x0eSLICE_CHANNELS\x10\n\x12\n\n\x06SOURCE\x10\x0b\x12\x08\n\x04SINK\x10\x0c\x12\x0e\n\nDOWNSAMPLE\x10\r\x12\x10\n\x0cREMAP_SENSOR\x10\x0e*\xdf\x01\n\x17SpikeSorterParamCommand\x12\x14\n\x10SORTER_THR_LEVEL\x10\x01\x12\x17\n\x13SORTER_THR_LEVEL_SD\x10\x04\x12\x12\n\x0eSORTER_THR_WDW\x10\x08\x12\x19\n\x15SORTER_WEAK_THR_LEVEL\x10\n\x12\x1c\n\x18SORTER_WEAK_THR_LEVEL_SD\x10\r\x12\x11\n\rSORTER_SHADOW\x10\x11\x12\x17\n\x13SORTER_THR_ACTIVATE\x10\x13\x12\x1c\n\x18SORTER_WEAK_THR_ACTIVATE\x10\x15*\xee\x03\n\x10StatusPollFields\x12\x19\n\x15PORT_CONNECTION_STATE\x10\x00\x12\x14\n\x10RECORDING_ERRORS\x10\x01\x12\x15\n\x11STREAM_TIME_RANGE\x10\x02\x12\x11\n\rSTREAM_STATUS\x10\x03\x12\x11\n\rRECORD_STATUS\x10\x04\x12\x10\n\x0cIS_CONNECTED\x10\x06\x12\x0e\n\nRECORD_DUR\x10\x07\x12\x11\n\rBACKBONE_MODE\x10\t\x12\x10\n\x0cSIGNAL_GROUP\x10\n\x12\x14\n\x10SINAPS_REGISTERS\x10\x0b\x12\x14\n\x10RECORDING_CONFIG\x10\x0c\x12\x0b\n\x07\x46ILTERS\x10\r\x12\x17\n\x13\x45VENT_THRESH_PARAMS\x10\x0e\x12\x10\n\x0c\x44\x41\x43_REGISTER\x10\x0f\x12\x10\n\x0c\x44IO_REGISTER\x10\x10\x12\x10\n\x0cTRIGGER_MODE\x10\x11\x12\x11\n\rCABLE_LENGTHS\x10\x12\x12\x11\n\rEVENT_VIEWERS\x10\x13\x12\x0f\n\x0bSAMPLE_RATE\x10\x14\x12\x0e\n\nALL_FIELDS\x10\x15\x12\x16\n\x12SPIKE_SORTER_STATE\x10\x16\x12\x0f\n\x0bSTIM_PARAMS\x10\x17\x12\x19\n\x15SPIKE_SORTER_WARNINGS\x10\x18\x12\x12\n\x0eSTIM_STEP_SIZE\x10\x19*\x1b\n\rDashboardType\x12\n\n\x06\x44\x41SH_1\x10\x00*N\n\x10\x44\x61shboardCommand\x12\x11\n\rDASH_CMD_OPEN\x10\x00\x12\x12\n\x0e\x44\x41SH_CMD_CLOSE\x10\x01\x12\x13\n\x0f\x44\x41SH_CMD_UPDATE\x10\x02\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
@@ -28,86 +28,86 @@
   _SERVERSPEC_SERVICEENTRY._serialized_options = b'8\001'
   _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._options = None
   _GETSORTERIDMAPREPLY_SIGTOSORTMAPENTRY._serialized_options = b'8\001'
   _SIGNALGROUPUNITS_UNITSENTRY._options = None
   _SIGNALGROUPUNITS_UNITSENTRY._serialized_options = b'8\001'
   _UPDATESIGNALGROUPREQUEST.fields_by_name['ntvChanIdx']._options = None
   _UPDATESIGNALGROUPREQUEST.fields_by_name['ntvChanIdx']._serialized_options = b'\020\001'
-  _RADIXFILETYPES._serialized_start=24598
-  _RADIXFILETYPES._serialized_end=24876
-  _SIGNALTYPE._serialized_start=24878
-  _SIGNALTYPE._serialized_end=24927
-  _RESAMPLEROUTINE._serialized_start=24929
-  _RESAMPLEROUTINE._serialized_end=24987
-  _PORT._serialized_start=24989
-  _PORT._serialized_end=25051
-  _WORKSPACEAPP._serialized_start=25053
-  _WORKSPACEAPP._serialized_end=25103
-  _WORKSPACECOMMANDS._serialized_start=25106
-  _WORKSPACECOMMANDS._serialized_end=25266
-  _GETWORKSPACECOMMANDS._serialized_start=25268
-  _GETWORKSPACECOMMANDS._serialized_end=25335
-  _RADIENSSERVERTYPE._serialized_start=25337
-  _RADIENSSERVERTYPE._serialized_end=25393
-  _GRPCSERVICETYPE._serialized_start=25396
-  _GRPCSERVICETYPE._serialized_end=25570
-  _DEVDATASETTYPE._serialized_start=25572
-  _DEVDATASETTYPE._serialized_end=25635
-  _PSDWINDOWTYPE._serialized_start=25637
-  _PSDWINDOWTYPE._serialized_end=25704
-  _PSDSCALING._serialized_start=25706
-  _PSDSCALING._serialized_end=25736
-  _DATASOURCESORT._serialized_start=25738
-  _DATASOURCESORT._serialized_end=25826
-  _SIGNALGROUPTYPE._serialized_start=25828
-  _SIGNALGROUPTYPE._serialized_end=25874
-  _DSPTYPE._serialized_start=25877
-  _DSPTYPE._serialized_end=26006
-  _FILTERSTAGE._serialized_start=26008
-  _FILTERSTAGE._serialized_end=26065
-  _FEATURELICENSE._serialized_start=26068
-  _FEATURELICENSE._serialized_end=26407
-  _SUMMARYSTATSENUM._serialized_start=26410
-  _SUMMARYSTATSENUM._serialized_end=26647
-  _KPIMETRICSMODE._serialized_start=26649
-  _KPIMETRICSMODE._serialized_end=26744
-  _KPIMETRICSENUM._serialized_start=26747
-  _KPIMETRICSENUM._serialized_end=27548
-  _KPIMETRICSSTATSENUM._serialized_start=27551
-  _KPIMETRICSSTATSENUM._serialized_end=27690
-  _KPIBUNDLEPACKETSSTATSENUM._serialized_start=27693
-  _KPIBUNDLEPACKETSSTATSENUM._serialized_end=28013
-  _TIMERANGESELMODE._serialized_start=28015
-  _TIMERANGESELMODE._serialized_end=28085
-  _KPISCANNERCMD._serialized_start=28087
-  _KPISCANNERCMD._serialized_end=28188
-  _OUTFITTERCOMPONENTTYPE._serialized_start=28190
-  _OUTFITTERCOMPONENTTYPE._serialized_end=28268
-  _WORLDNODELABEL._serialized_start=28270
-  _WORLDNODELABEL._serialized_end=28395
-  _WORLDEDGELABEL._serialized_start=28397
-  _WORLDEDGELABEL._serialized_end=28436
-  _WORLDEDGEDIRECTION._serialized_start=28438
-  _WORLDEDGEDIRECTION._serialized_end=28534
-  _USERROLETYPE._serialized_start=28537
-  _USERROLETYPE._serialized_end=28696
-  _MANAGENODECMD._serialized_start=28698
-  _MANAGENODECMD._serialized_end=28769
-  _WORLDQUERYCMD._serialized_start=28772
-  _WORLDQUERYCMD._serialized_end=29004
-  _TRANSFORMNODETYPE._serialized_start=29007
-  _TRANSFORMNODETYPE._serialized_end=29265
-  _SPIKESORTERPARAMCOMMAND._serialized_start=29268
-  _SPIKESORTERPARAMCOMMAND._serialized_end=29491
-  _STATUSPOLLFIELDS._serialized_start=29494
-  _STATUSPOLLFIELDS._serialized_end=30012
-  _DASHBOARDTYPE._serialized_start=30014
-  _DASHBOARDTYPE._serialized_end=30041
-  _DASHBOARDCOMMAND._serialized_start=30043
-  _DASHBOARDCOMMAND._serialized_end=30121
+  _RADIXFILETYPES._serialized_start=24615
+  _RADIXFILETYPES._serialized_end=24893
+  _SIGNALTYPE._serialized_start=24895
+  _SIGNALTYPE._serialized_end=24944
+  _RESAMPLEROUTINE._serialized_start=24946
+  _RESAMPLEROUTINE._serialized_end=25004
+  _PORT._serialized_start=25006
+  _PORT._serialized_end=25068
+  _WORKSPACEAPP._serialized_start=25070
+  _WORKSPACEAPP._serialized_end=25120
+  _WORKSPACECOMMANDS._serialized_start=25123
+  _WORKSPACECOMMANDS._serialized_end=25283
+  _GETWORKSPACECOMMANDS._serialized_start=25285
+  _GETWORKSPACECOMMANDS._serialized_end=25352
+  _RADIENSSERVERTYPE._serialized_start=25354
+  _RADIENSSERVERTYPE._serialized_end=25410
+  _GRPCSERVICETYPE._serialized_start=25413
+  _GRPCSERVICETYPE._serialized_end=25587
+  _DEVDATASETTYPE._serialized_start=25589
+  _DEVDATASETTYPE._serialized_end=25652
+  _PSDWINDOWTYPE._serialized_start=25654
+  _PSDWINDOWTYPE._serialized_end=25721
+  _PSDSCALING._serialized_start=25723
+  _PSDSCALING._serialized_end=25753
+  _DATASOURCESORT._serialized_start=25755
+  _DATASOURCESORT._serialized_end=25843
+  _SIGNALGROUPTYPE._serialized_start=25845
+  _SIGNALGROUPTYPE._serialized_end=25891
+  _DSPTYPE._serialized_start=25894
+  _DSPTYPE._serialized_end=26023
+  _FILTERSTAGE._serialized_start=26025
+  _FILTERSTAGE._serialized_end=26082
+  _FEATURELICENSE._serialized_start=26085
+  _FEATURELICENSE._serialized_end=26424
+  _SUMMARYSTATSENUM._serialized_start=26427
+  _SUMMARYSTATSENUM._serialized_end=26664
+  _KPIMETRICSMODE._serialized_start=26666
+  _KPIMETRICSMODE._serialized_end=26761
+  _KPIMETRICSENUM._serialized_start=26764
+  _KPIMETRICSENUM._serialized_end=27565
+  _KPIMETRICSSTATSENUM._serialized_start=27568
+  _KPIMETRICSSTATSENUM._serialized_end=27707
+  _KPIBUNDLEPACKETSSTATSENUM._serialized_start=27710
+  _KPIBUNDLEPACKETSSTATSENUM._serialized_end=28030
+  _TIMERANGESELMODE._serialized_start=28032
+  _TIMERANGESELMODE._serialized_end=28102
+  _KPISCANNERCMD._serialized_start=28104
+  _KPISCANNERCMD._serialized_end=28205
+  _OUTFITTERCOMPONENTTYPE._serialized_start=28207
+  _OUTFITTERCOMPONENTTYPE._serialized_end=28285
+  _WORLDNODELABEL._serialized_start=28287
+  _WORLDNODELABEL._serialized_end=28412
+  _WORLDEDGELABEL._serialized_start=28414
+  _WORLDEDGELABEL._serialized_end=28453
+  _WORLDEDGEDIRECTION._serialized_start=28455
+  _WORLDEDGEDIRECTION._serialized_end=28551
+  _USERROLETYPE._serialized_start=28554
+  _USERROLETYPE._serialized_end=28713
+  _MANAGENODECMD._serialized_start=28715
+  _MANAGENODECMD._serialized_end=28786
+  _WORLDQUERYCMD._serialized_start=28789
+  _WORLDQUERYCMD._serialized_end=29021
+  _TRANSFORMNODETYPE._serialized_start=29024
+  _TRANSFORMNODETYPE._serialized_end=29282
+  _SPIKESORTERPARAMCOMMAND._serialized_start=29285
+  _SPIKESORTERPARAMCOMMAND._serialized_end=29508
+  _STATUSPOLLFIELDS._serialized_start=29511
+  _STATUSPOLLFIELDS._serialized_end=30005
+  _DASHBOARDTYPE._serialized_start=30007
+  _DASHBOARDTYPE._serialized_end=30034
+  _DASHBOARDCOMMAND._serialized_start=30036
+  _DASHBOARDCOMMAND._serialized_end=30114
   _OFFLINELICENSESTATUS._serialized_start=57
   _OFFLINELICENSESTATUS._serialized_end=121
   _FIRMWAREVERSION._serialized_start=123
   _FIRMWAREVERSION._serialized_end=190
   _RADIXENVIRONMENT._serialized_start=192
   _RADIXENVIRONMENT._serialized_end=299
   _STANDARDREQUEST._serialized_start=301
@@ -453,65 +453,65 @@
   _SLICETIMETRANSFORMPARAMS._serialized_start=20546
   _SLICETIMETRANSFORMPARAMS._serialized_end=20608
   _SLICECHANNELSTRANSFORMPARAMS._serialized_start=20610
   _SLICECHANNELSTRANSFORMPARAMS._serialized_end=20720
   _DOWNSAMPLETRANSFORMPARAMS._serialized_start=20722
   _DOWNSAMPLETRANSFORMPARAMS._serialized_end=20771
   _REMAPSENSORTRANSFORMPARAMS._serialized_start=20774
-  _REMAPSENSORTRANSFORMPARAMS._serialized_end=20993
-  _REMAPSENSORTRANSFORMPARAMS_SENSORSPEC._serialized_start=20868
-  _REMAPSENSORTRANSFORMPARAMS_SENSORSPEC._serialized_end=20993
-  _POSITION._serialized_start=20995
-  _POSITION._serialized_end=21027
-  _TRANSFORMNODE._serialized_start=21030
-  _TRANSFORMNODE._serialized_end=21822
-  _TRANSFORMEDGE._serialized_start=21824
-  _TRANSFORMEDGE._serialized_end=21883
-  _PROTOCOL._serialized_start=21885
-  _PROTOCOL._serialized_end=22001
-  _PROTOCOLREQUEST._serialized_start=22003
-  _PROTOCOLREQUEST._serialized_end=22040
-  _RENAMEPROTOCOLREQUEST._serialized_start=22042
-  _RENAMEPROTOCOLREQUEST._serialized_end=22108
-  _GETALLPROTOCOLSREPLY._serialized_start=22110
-  _GETALLPROTOCOLSREPLY._serialized_end=22169
-  _APPLYPROTOCOLPROGRESS._serialized_start=22171
-  _APPLYPROTOCOLPROGRESS._serialized_end=22294
-  _SPIKESORTERSETPARAMREQUEST._serialized_start=22297
-  _SPIKESORTERSETPARAMREQUEST._serialized_end=22451
-  _SPIKESORTERSETPARAMSREQUEST._serialized_start=22453
-  _SPIKESORTERSETPARAMSREQUEST._serialized_end=22534
-  _SPIKESORTERPARAMCOMMANDRECORD._serialized_start=22537
-  _SPIKESORTERPARAMCOMMANDRECORD._serialized_end=22832
-  _KPIPARAMS._serialized_start=22834
-  _KPIPARAMS._serialized_end=22897
-  _DACSTREAMREQUEST._serialized_start=22899
-  _DACSTREAMREQUEST._serialized_end=22973
-  _EVENTVIEWERCONFIG._serialized_start=22976
-  _EVENTVIEWERCONFIG._serialized_end=23198
-  _EVENTVIEWERID._serialized_start=23200
-  _EVENTVIEWERID._serialized_end=23261
-  _GETEVENTVIEWEREVENTREQUEST._serialized_start=23263
-  _GETEVENTVIEWEREVENTREQUEST._serialized_end=23331
-  _EVENTVIEWEREVENTDESC._serialized_start=23333
-  _EVENTVIEWEREVENTDESC._serialized_end=23422
-  _EVENTVIEWEREVENT._serialized_start=23425
-  _EVENTVIEWEREVENT._serialized_end=23568
-  _LISTEVENTVIEWEREVENTSREPLY._serialized_start=23570
-  _LISTEVENTVIEWEREVENTSREPLY._serialized_end=23667
-  _LISTEVENTVIEWERSREPLY._serialized_start=23669
-  _LISTEVENTVIEWERSREPLY._serialized_end=23737
-  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_start=23739
-  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_end=23790
-  _STATUSPOLLFIELDSTOUPDATE._serialized_start=23792
-  _STATUSPOLLFIELDSTOUPDATE._serialized_end=23886
-  _DASHBOARDCOMMANDREQUEST._serialized_start=23889
-  _DASHBOARDCOMMANDREQUEST._serialized_end=24054
-  _DASHBOARDCOMMANDREQUEST_ARGS._serialized_start=24009
-  _DASHBOARDCOMMANDREQUEST_ARGS._serialized_end=24054
-  _SELTABLESIGNALGROUP._serialized_start=24056
-  _SELTABLESIGNALGROUP._serialized_end=24149
-  _SELECTORTABLESREPLY._serialized_start=24151
-  _SELECTORTABLESREPLY._serialized_end=24214
-  _DATASOURCESTATUS._serialized_start=24217
-  _DATASOURCESTATUS._serialized_end=24595
+  _REMAPSENSORTRANSFORMPARAMS._serialized_end=21010
+  _REMAPSENSORTRANSFORMPARAMS_SENSORSPEC._serialized_start=20885
+  _REMAPSENSORTRANSFORMPARAMS_SENSORSPEC._serialized_end=21010
+  _POSITION._serialized_start=21012
+  _POSITION._serialized_end=21044
+  _TRANSFORMNODE._serialized_start=21047
+  _TRANSFORMNODE._serialized_end=21839
+  _TRANSFORMEDGE._serialized_start=21841
+  _TRANSFORMEDGE._serialized_end=21900
+  _PROTOCOL._serialized_start=21902
+  _PROTOCOL._serialized_end=22018
+  _PROTOCOLREQUEST._serialized_start=22020
+  _PROTOCOLREQUEST._serialized_end=22057
+  _RENAMEPROTOCOLREQUEST._serialized_start=22059
+  _RENAMEPROTOCOLREQUEST._serialized_end=22125
+  _GETALLPROTOCOLSREPLY._serialized_start=22127
+  _GETALLPROTOCOLSREPLY._serialized_end=22186
+  _APPLYPROTOCOLPROGRESS._serialized_start=22188
+  _APPLYPROTOCOLPROGRESS._serialized_end=22311
+  _SPIKESORTERSETPARAMREQUEST._serialized_start=22314
+  _SPIKESORTERSETPARAMREQUEST._serialized_end=22468
+  _SPIKESORTERSETPARAMSREQUEST._serialized_start=22470
+  _SPIKESORTERSETPARAMSREQUEST._serialized_end=22551
+  _SPIKESORTERPARAMCOMMANDRECORD._serialized_start=22554
+  _SPIKESORTERPARAMCOMMANDRECORD._serialized_end=22849
+  _KPIPARAMS._serialized_start=22851
+  _KPIPARAMS._serialized_end=22914
+  _DACSTREAMREQUEST._serialized_start=22916
+  _DACSTREAMREQUEST._serialized_end=22990
+  _EVENTVIEWERCONFIG._serialized_start=22993
+  _EVENTVIEWERCONFIG._serialized_end=23215
+  _EVENTVIEWERID._serialized_start=23217
+  _EVENTVIEWERID._serialized_end=23278
+  _GETEVENTVIEWEREVENTREQUEST._serialized_start=23280
+  _GETEVENTVIEWEREVENTREQUEST._serialized_end=23348
+  _EVENTVIEWEREVENTDESC._serialized_start=23350
+  _EVENTVIEWEREVENTDESC._serialized_end=23439
+  _EVENTVIEWEREVENT._serialized_start=23442
+  _EVENTVIEWEREVENT._serialized_end=23585
+  _LISTEVENTVIEWEREVENTSREPLY._serialized_start=23587
+  _LISTEVENTVIEWEREVENTSREPLY._serialized_end=23684
+  _LISTEVENTVIEWERSREPLY._serialized_start=23686
+  _LISTEVENTVIEWERSREPLY._serialized_end=23754
+  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_start=23756
+  _STATUSPOLLFIELDSTOUPDATEREQUEST._serialized_end=23807
+  _STATUSPOLLFIELDSTOUPDATE._serialized_start=23809
+  _STATUSPOLLFIELDSTOUPDATE._serialized_end=23903
+  _DASHBOARDCOMMANDREQUEST._serialized_start=23906
+  _DASHBOARDCOMMANDREQUEST._serialized_end=24071
+  _DASHBOARDCOMMANDREQUEST_ARGS._serialized_start=24026
+  _DASHBOARDCOMMANDREQUEST_ARGS._serialized_end=24071
+  _SELTABLESIGNALGROUP._serialized_start=24073
+  _SELTABLESIGNALGROUP._serialized_end=24166
+  _SELECTORTABLESREPLY._serialized_start=24168
+  _SELECTORTABLESREPLY._serialized_end=24231
+  _DATASOURCESTATUS._serialized_start=24234
+  _DATASOURCESTATUS._serialized_end=24612
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-3.0.0b4/radiens/grpc_radiens/datasource_pb2.py` & `radiens-3.0.0b5/radiens/grpc_radiens/datasource_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,56 +11,56 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import common_pb2 as common__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x64\x61tasource.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"<\n\x11\x44\x61taSourceRequest\x12\x11\n\tdsourceID\x18\x01 \x03(\t\x12\x14\n\x0crenameDsrcID\x18\x02 \x01(\t\"\xc7\x01\n\x18\x44\x61taSourceSetSaveRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x01(\t\x12\x11\n\tdsourceID\x18\x03 \x01(\t\x12\x0b\n\x03uID\x18\x04 \x01(\t\x12(\n\x08\x66ileType\x18\x05 \x01(\x0e\x32\x16.allego.RadixFileTypes\x12\x0f\n\x07isForce\x18\x06 \x01(\x08\x12\x17\n\x0fisBackgroundKPI\x18\x07 \x01(\x08\x12\x17\n\x0fparentDsourceID\x18\x08 \x01(\t\"%\n\x11\x44\x61taSourceIDReply\x12\x10\n\x08sortedID\x18\x01 \x03(\t\"\x95\x01\n\x16\x44\x61taSourceSetSaveReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12(\n\x06status\x18\x02 \x01(\x0b\x32\x18.allego.DataSourceStatus\x12\r\n\x05niIDs\x18\x03 \x03(\t\x12/\n\x0f\x61ssociatedDsrcs\x18\x04 \x03(\x0b\x32\x16.allego.FileDescriptor\"\xae\x01\n\x13\x44\x61taSourceStatusMap\x12\x39\n\x07\x64source\x18\x01 \x03(\x0b\x32(.allego.DataSourceStatusMap.DsourceEntry\x12\x12\n\norderedIDs\x18\x02 \x03(\t\x1aH\n\x0c\x44sourceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.allego.DataSourceStatus:\x02\x38\x01\"\xa1\x03\n\x1f\x43opyRemoveDataSourceFileRequest\x12\x45\n\x04many\x18\x01 \x01(\x0b\x32\x35.allego.CopyRemoveDataSourceFileRequest.MultipleFilesH\x00\x12>\n\x03one\x18\x02 \x01(\x0b\x32/.allego.CopyRemoveDataSourceFileRequest.OneFileH\x00\x12\x0f\n\x07isForce\x18\x03 \x01(\x08\x12\x12\n\nisValidate\x18\x04 \x01(\x08\x1at\n\rMultipleFiles\x12#\n\x03src\x18\x01 \x03(\x0b\x32\x16.allego.FileDescriptor\x12\x10\n\x08\x64\x65stPath\x18\x02 \x01(\t\x12,\n\x0c\x64\x65stFileType\x18\x03 \x01(\x0e\x32\x16.allego.RadixFileTypes\x1aT\n\x07OneFile\x12#\n\x03src\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12$\n\x04\x64\x65st\x18\x02 \x01(\x0b\x32\x16.allego.FileDescriptorB\x06\n\x04\x64\x65sc\"\xf8\x02\n\x15\x44\x61taSourceFileSetStat\x12\x10\n\x08numFiles\x18\x01 \x02(\x05\x12\x1b\n\x13numBytesPrimaryData\x18\x02 \x02(\x03\x12\x18\n\x10numBytesMetaData\x18\x03 \x02(\x03\x12\x10\n\x08numBytes\x18\x04 \x02(\x03\x12\x16\n\x0eisMetadataFile\x18\x05 \x02(\x08\x12-\n\ttimeStamp\x18\x06 \x02(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bnumChannels\x18\x07 \x02(\x05\x12\x13\n\x0b\x64urationSec\x18\x08 \x02(\x01\x12\x12\n\ndatasetUID\x18\t \x02(\t\x12\x17\n\x0f\x64\x61tasetChecksum\x18\n \x01(\t\x12\x19\n\x11\x64\x61tasetProvenance\x18\x0b \x03(\t\x12\x12\n\nsampleRate\x18\x0c \x02(\x05\x12\x37\n\x0e\x62\x61\x63kgroundProc\x18\r \x01(\x0b\x32\x1f.allego.BackgroundProcessStatus\"\x82\x02\n\rCpRmMvLsReply\x12\x10\n\x08numFiles\x18\x01 \x02(\x05\x12\x12\n\nnumDsource\x18\x02 \x02(\x05\x12\x10\n\x08numBytes\x18\x03 \x02(\x03\x12\x10\n\x08\x64\x65stPath\x18\x04 \x02(\t\x12\x35\n\x07\x64source\x18\x05 \x03(\x0b\x32$.allego.CpRmMvLsReply.DataSourceInfo\x12\x0b\n\x03msg\x18\x06 \x01(\t\x1a\x63\n\x0e\x44\x61taSourceInfo\x12$\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12+\n\x04stat\x18\x02 \x02(\x0b\x32\x1d.allego.DataSourceFileSetStat\"y\n\x17\x42\x61\x63kgroundProcessStatus\x12\x0b\n\x03uID\x18\x01 \x02(\t\x12\x14\n\x0c\x66racComplete\x18\x02 \x01(\x01\x12\x16\n\x0e\x65lapsedTimeSec\x18\x03 \x01(\x01\x12#\n\x1b\x65stimatedCompletionWallTime\x18\x04 \x01(\t\"\x8b\x01\n\x19MoveDataSourceFileRequest\x12#\n\x03src\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12$\n\x04\x64\x65st\x18\x02 \x02(\x0b\x32\x16.allego.FileDescriptor\x12\x0f\n\x07isForce\x18\x03 \x01(\x08\x12\x12\n\nisValidate\x18\x04 \x01(\x08\"\xbf\x01\n\x10\x44\x61taSourceParams\x12\x12\n\nsampleFreq\x18\x01 \x02(\x01\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x10\n\x08\x64uration\x18\x03 \x02(\x01\x12%\n\x04type\x18\x05 \x02(\x0e\x32\x17.allego.SignalGroupType\x12\x35\n\x0e\x64\x61tasourceType\x18\x06 \x01(\x0e\x32\x1d.allego.RadiensDatasourceType\x12\x14\n\x0c\x64\x61tasourceID\x18\x07 \x01(\t\".\n\x10ImpedanceRequest\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\"\x85\x01\n\tImpedance\x12\x34\n\nimpedances\x18\x01 \x03(\x0b\x32 .allego.Impedance.ImpedanceValue\x1a\x42\n\x0eImpedanceValue\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x0c\n\x04zMag\x18\x02 \x02(\x01\x12\x0e\n\x06zPhase\x18\x03 \x02(\x01*0\n\x15RadiensDatasourceType\x12\x07\n\x03\x41NY\x10\x00\x12\x0e\n\nTIMESERIES\x10\x01\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x64\x61tasource.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"<\n\x11\x44\x61taSourceRequest\x12\x11\n\tdsourceID\x18\x01 \x03(\t\x12\x14\n\x0crenameDsrcID\x18\x02 \x01(\t\"\xde\x01\n\x18\x44\x61taSourceSetSaveRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x01(\t\x12\x11\n\tdsourceID\x18\x03 \x01(\t\x12\x0b\n\x03uID\x18\x04 \x01(\t\x12(\n\x08\x66ileType\x18\x05 \x01(\x0e\x32\x16.allego.RadixFileTypes\x12\x0f\n\x07isForce\x18\x06 \x01(\x08\x12\x17\n\x0fisBackgroundKPI\x18\x07 \x01(\x08\x12\x17\n\x0fparentDsourceID\x18\x08 \x01(\t\x12\x15\n\rforceNoSorter\x18\t \x01(\x08\"%\n\x11\x44\x61taSourceIDReply\x12\x10\n\x08sortedID\x18\x01 \x03(\t\"\x95\x01\n\x16\x44\x61taSourceSetSaveReply\x12\x11\n\tdsourceID\x18\x01 \x02(\t\x12(\n\x06status\x18\x02 \x01(\x0b\x32\x18.allego.DataSourceStatus\x12\r\n\x05niIDs\x18\x03 \x03(\t\x12/\n\x0f\x61ssociatedDsrcs\x18\x04 \x03(\x0b\x32\x16.allego.FileDescriptor\"\xae\x01\n\x13\x44\x61taSourceStatusMap\x12\x39\n\x07\x64source\x18\x01 \x03(\x0b\x32(.allego.DataSourceStatusMap.DsourceEntry\x12\x12\n\norderedIDs\x18\x02 \x03(\t\x1aH\n\x0c\x44sourceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.allego.DataSourceStatus:\x02\x38\x01\"\xa1\x03\n\x1f\x43opyRemoveDataSourceFileRequest\x12\x45\n\x04many\x18\x01 \x01(\x0b\x32\x35.allego.CopyRemoveDataSourceFileRequest.MultipleFilesH\x00\x12>\n\x03one\x18\x02 \x01(\x0b\x32/.allego.CopyRemoveDataSourceFileRequest.OneFileH\x00\x12\x0f\n\x07isForce\x18\x03 \x01(\x08\x12\x12\n\nisValidate\x18\x04 \x01(\x08\x1at\n\rMultipleFiles\x12#\n\x03src\x18\x01 \x03(\x0b\x32\x16.allego.FileDescriptor\x12\x10\n\x08\x64\x65stPath\x18\x02 \x01(\t\x12,\n\x0c\x64\x65stFileType\x18\x03 \x01(\x0e\x32\x16.allego.RadixFileTypes\x1aT\n\x07OneFile\x12#\n\x03src\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12$\n\x04\x64\x65st\x18\x02 \x01(\x0b\x32\x16.allego.FileDescriptorB\x06\n\x04\x64\x65sc\"\xf8\x02\n\x15\x44\x61taSourceFileSetStat\x12\x10\n\x08numFiles\x18\x01 \x02(\x05\x12\x1b\n\x13numBytesPrimaryData\x18\x02 \x02(\x03\x12\x18\n\x10numBytesMetaData\x18\x03 \x02(\x03\x12\x10\n\x08numBytes\x18\x04 \x02(\x03\x12\x16\n\x0eisMetadataFile\x18\x05 \x02(\x08\x12-\n\ttimeStamp\x18\x06 \x02(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bnumChannels\x18\x07 \x02(\x05\x12\x13\n\x0b\x64urationSec\x18\x08 \x02(\x01\x12\x12\n\ndatasetUID\x18\t \x02(\t\x12\x17\n\x0f\x64\x61tasetChecksum\x18\n \x01(\t\x12\x19\n\x11\x64\x61tasetProvenance\x18\x0b \x03(\t\x12\x12\n\nsampleRate\x18\x0c \x02(\x05\x12\x37\n\x0e\x62\x61\x63kgroundProc\x18\r \x01(\x0b\x32\x1f.allego.BackgroundProcessStatus\"\x82\x02\n\rCpRmMvLsReply\x12\x10\n\x08numFiles\x18\x01 \x02(\x05\x12\x12\n\nnumDsource\x18\x02 \x02(\x05\x12\x10\n\x08numBytes\x18\x03 \x02(\x03\x12\x10\n\x08\x64\x65stPath\x18\x04 \x02(\t\x12\x35\n\x07\x64source\x18\x05 \x03(\x0b\x32$.allego.CpRmMvLsReply.DataSourceInfo\x12\x0b\n\x03msg\x18\x06 \x01(\t\x1a\x63\n\x0e\x44\x61taSourceInfo\x12$\n\x04\x64\x65sc\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12+\n\x04stat\x18\x02 \x02(\x0b\x32\x1d.allego.DataSourceFileSetStat\"y\n\x17\x42\x61\x63kgroundProcessStatus\x12\x0b\n\x03uID\x18\x01 \x02(\t\x12\x14\n\x0c\x66racComplete\x18\x02 \x01(\x01\x12\x16\n\x0e\x65lapsedTimeSec\x18\x03 \x01(\x01\x12#\n\x1b\x65stimatedCompletionWallTime\x18\x04 \x01(\t\"\x8b\x01\n\x19MoveDataSourceFileRequest\x12#\n\x03src\x18\x01 \x02(\x0b\x32\x16.allego.FileDescriptor\x12$\n\x04\x64\x65st\x18\x02 \x02(\x0b\x32\x16.allego.FileDescriptor\x12\x0f\n\x07isForce\x18\x03 \x01(\x08\x12\x12\n\nisValidate\x18\x04 \x01(\x08\"\xbf\x01\n\x10\x44\x61taSourceParams\x12\x12\n\nsampleFreq\x18\x01 \x02(\x01\x12\x11\n\ttimeRange\x18\x02 \x03(\x01\x12\x10\n\x08\x64uration\x18\x03 \x02(\x01\x12%\n\x04type\x18\x05 \x02(\x0e\x32\x17.allego.SignalGroupType\x12\x35\n\x0e\x64\x61tasourceType\x18\x06 \x01(\x0e\x32\x1d.allego.RadiensDatasourceType\x12\x14\n\x0c\x64\x61tasourceID\x18\x07 \x01(\t\".\n\x10ImpedanceRequest\x12\x1a\n\x04port\x18\x01 \x02(\x0e\x32\x0c.allego.Port\"\x85\x01\n\tImpedance\x12\x34\n\nimpedances\x18\x01 \x03(\x0b\x32 .allego.Impedance.ImpedanceValue\x1a\x42\n\x0eImpedanceValue\x12\x12\n\nntvChanIdx\x18\x01 \x02(\x05\x12\x0c\n\x04zMag\x18\x02 \x02(\x01\x12\x0e\n\x06zPhase\x18\x03 \x02(\x01*0\n\x15RadiensDatasourceType\x12\x07\n\x03\x41NY\x10\x00\x12\x0e\n\nTIMESERIES\x10\x01\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'datasource_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
   _DATASOURCESTATUSMAP_DSOURCEENTRY._options = None
   _DATASOURCESTATUSMAP_DSOURCEENTRY._serialized_options = b'8\001'
-  _RADIENSDATASOURCETYPE._serialized_start=2410
-  _RADIENSDATASOURCETYPE._serialized_end=2458
+  _RADIENSDATASOURCETYPE._serialized_start=2433
+  _RADIENSDATASOURCETYPE._serialized_end=2481
   _DATASOURCEREQUEST._serialized_start=75
   _DATASOURCEREQUEST._serialized_end=135
   _DATASOURCESETSAVEREQUEST._serialized_start=138
-  _DATASOURCESETSAVEREQUEST._serialized_end=337
-  _DATASOURCEIDREPLY._serialized_start=339
-  _DATASOURCEIDREPLY._serialized_end=376
-  _DATASOURCESETSAVEREPLY._serialized_start=379
-  _DATASOURCESETSAVEREPLY._serialized_end=528
-  _DATASOURCESTATUSMAP._serialized_start=531
-  _DATASOURCESTATUSMAP._serialized_end=705
-  _DATASOURCESTATUSMAP_DSOURCEENTRY._serialized_start=633
-  _DATASOURCESTATUSMAP_DSOURCEENTRY._serialized_end=705
-  _COPYREMOVEDATASOURCEFILEREQUEST._serialized_start=708
-  _COPYREMOVEDATASOURCEFILEREQUEST._serialized_end=1125
-  _COPYREMOVEDATASOURCEFILEREQUEST_MULTIPLEFILES._serialized_start=915
-  _COPYREMOVEDATASOURCEFILEREQUEST_MULTIPLEFILES._serialized_end=1031
-  _COPYREMOVEDATASOURCEFILEREQUEST_ONEFILE._serialized_start=1033
-  _COPYREMOVEDATASOURCEFILEREQUEST_ONEFILE._serialized_end=1117
-  _DATASOURCEFILESETSTAT._serialized_start=1128
-  _DATASOURCEFILESETSTAT._serialized_end=1504
-  _CPRMMVLSREPLY._serialized_start=1507
-  _CPRMMVLSREPLY._serialized_end=1765
-  _CPRMMVLSREPLY_DATASOURCEINFO._serialized_start=1666
-  _CPRMMVLSREPLY_DATASOURCEINFO._serialized_end=1765
-  _BACKGROUNDPROCESSSTATUS._serialized_start=1767
-  _BACKGROUNDPROCESSSTATUS._serialized_end=1888
-  _MOVEDATASOURCEFILEREQUEST._serialized_start=1891
-  _MOVEDATASOURCEFILEREQUEST._serialized_end=2030
-  _DATASOURCEPARAMS._serialized_start=2033
-  _DATASOURCEPARAMS._serialized_end=2224
-  _IMPEDANCEREQUEST._serialized_start=2226
-  _IMPEDANCEREQUEST._serialized_end=2272
-  _IMPEDANCE._serialized_start=2275
-  _IMPEDANCE._serialized_end=2408
-  _IMPEDANCE_IMPEDANCEVALUE._serialized_start=2342
-  _IMPEDANCE_IMPEDANCEVALUE._serialized_end=2408
+  _DATASOURCESETSAVEREQUEST._serialized_end=360
+  _DATASOURCEIDREPLY._serialized_start=362
+  _DATASOURCEIDREPLY._serialized_end=399
+  _DATASOURCESETSAVEREPLY._serialized_start=402
+  _DATASOURCESETSAVEREPLY._serialized_end=551
+  _DATASOURCESTATUSMAP._serialized_start=554
+  _DATASOURCESTATUSMAP._serialized_end=728
+  _DATASOURCESTATUSMAP_DSOURCEENTRY._serialized_start=656
+  _DATASOURCESTATUSMAP_DSOURCEENTRY._serialized_end=728
+  _COPYREMOVEDATASOURCEFILEREQUEST._serialized_start=731
+  _COPYREMOVEDATASOURCEFILEREQUEST._serialized_end=1148
+  _COPYREMOVEDATASOURCEFILEREQUEST_MULTIPLEFILES._serialized_start=938
+  _COPYREMOVEDATASOURCEFILEREQUEST_MULTIPLEFILES._serialized_end=1054
+  _COPYREMOVEDATASOURCEFILEREQUEST_ONEFILE._serialized_start=1056
+  _COPYREMOVEDATASOURCEFILEREQUEST_ONEFILE._serialized_end=1140
+  _DATASOURCEFILESETSTAT._serialized_start=1151
+  _DATASOURCEFILESETSTAT._serialized_end=1527
+  _CPRMMVLSREPLY._serialized_start=1530
+  _CPRMMVLSREPLY._serialized_end=1788
+  _CPRMMVLSREPLY_DATASOURCEINFO._serialized_start=1689
+  _CPRMMVLSREPLY_DATASOURCEINFO._serialized_end=1788
+  _BACKGROUNDPROCESSSTATUS._serialized_start=1790
+  _BACKGROUNDPROCESSSTATUS._serialized_end=1911
+  _MOVEDATASOURCEFILEREQUEST._serialized_start=1914
+  _MOVEDATASOURCEFILEREQUEST._serialized_end=2053
+  _DATASOURCEPARAMS._serialized_start=2056
+  _DATASOURCEPARAMS._serialized_end=2247
+  _IMPEDANCEREQUEST._serialized_start=2249
+  _IMPEDANCEREQUEST._serialized_end=2295
+  _IMPEDANCE._serialized_start=2298
+  _IMPEDANCE._serialized_end=2431
+  _IMPEDANCE_IMPEDANCEVALUE._serialized_start=2365
+  _IMPEDANCE_IMPEDANCEVALUE._serialized_end=2431
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-3.0.0b4/radiens/grpc_radiens/pybridge_pb2.py` & `radiens-3.0.0b5/radiens/grpc_radiens/pybridge_pb2.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/grpc_radiens/pybridge_pb2_grpc.py` & `radiens-3.0.0b5/radiens/grpc_radiens/pybridge_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/grpc_radiens/radiens_dev_pb2.py` & `radiens-3.0.0b5/radiens/grpc_radiens/radiens_dev_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,62 +9,65 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import common_pb2 as common__pb2
 from . import spikesorter_pb2 as spikesorter__pb2
+from . import datasource_pb2 as datasource__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11radiens_dev.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x11spikesorter.proto\"\xc0\x01\n\x14SpkSortTrainerNewReq\x12\x33\n\x07\x64\x61taset\x18\x01 \x02(\x0b\x32\".allego.SpkSortTrainerDatasetParam\x12=\n\x08training\x18\x02 \x02(\x0b\x32+.allego.SpkSortTrainerNetworkTrainingParams\x12\x34\n\x05store\x18\x03 \x02(\x0b\x32%.allego.SpkSortTrainerStoreDescriptor\"l\n\x1cSpkSortTrainerDeleteModelReq\x12\x35\n\x07release\x18\x01 \x01(\x0e\x32$.allego.SpkSortTrainerNetworkRelease\x12\x15\n\risDeleteNamed\x18\x02 \x01(\x08\"\xdf\x03\n\x1aSpkSortTrainerDatasetParam\x12\x13\n\x0bniPathTrain\x18\x01 \x03(\t\x12\x17\n\x0fniBaseNameTrain\x18\x02 \x03(\t\x12\x18\n\x10niPathValidation\x18\x03 \x03(\t\x12\x1c\n\x14niBaseNameValidation\x18\x04 \x03(\t\x12\x12\n\nniPathTest\x18\x05 \x03(\t\x12\x16\n\x0eniBaseNameTest\x18\x06 \x03(\t\x12\x0f\n\x07NbhdDim\x18\x07 \x02(\x05\x12\x10\n\x08radiusUm\x18\x08 \x02(\x01\x12\x19\n\x11maxNumSamplesTest\x18\t \x02(\x03\x12\x1a\n\x12networkMaskingFrac\x18\n \x02(\x01\x12 \n\x18networkInitWeightsStdDev\x18\x0b \x02(\x01\x12\x1d\n\x15networkInitBiasStdDev\x18\x0c \x02(\x01\x12\x17\n\x0fnetworkL1lambda\x18\r \x02(\x01\x12*\n\"networkHiddenLayerShapeRelInputDim\x18\x0e \x03(\x01\x12\x1b\n\x13networkNumFeatures2\x18\x0f \x02(\x05\x12\x32\n\x10\x64\x65\x63InputFeatures\x18\x10 \x01(\x0e\x32\x18.allego.DecInputFeatures\"\xbd\x01\n#SpkSortTrainerNetworkTrainingParams\x12\x11\n\tnumEpochs\x18\x01 \x02(\x05\x12\x15\n\rminibatchSize\x18\x02 \x02(\x05\x12\x15\n\rmaxNumSamples\x18\x03 \x02(\x03\x12\r\n\x05\x61lpha\x18\x04 \x02(\x01\x12\x11\n\talphaBias\x18\x05 \x02(\x01\x12\x18\n\x10\x65rrorTolPretrain\x18\x06 \x02(\x01\x12\x19\n\x11numSamplesTestMSE\x18\x07 \x02(\x05\"\xb6\x02\n\x1dSpkSortTrainerStoreDescriptor\x12\x13\n\x0b\x62rainRegion\x18\x01 \x02(\t\x12\x36\n\x0bnetworkSize\x18\x02 \x02(\x0e\x32!.allego.SpkSortTrainerNetworkSize\x12\x39\n\nnbrPattern\x18\x03 \x02(\x0e\x32%.allego.SpkSortTrainerNeighborPattern\x12\x11\n\tnetworkID\x18\x04 \x02(\t\x12\x0f\n\x07NbhdDim\x18\x05 \x02(\x05\x12\x35\n\x07release\x18\x06 \x02(\x0e\x32$.allego.SpkSortTrainerNetworkRelease\x12\x32\n\x10\x64\x65\x63InputFeatures\x18\x07 \x02(\x0e\x32\x18.allego.DecInputFeatures\"(\n\x18SpkSortTrainerSetModeReq\x12\x0c\n\x04mode\x18\x01 \x02(\x05\"\x81\x01\n\x14SpkSortTrainerCmdReq\x12;\n\x03\x63md\x18\x01 \x02(\x0e\x32..allego.SpkSortTrainerCmdReq.SpkSortTrainerCmd\",\n\x11SpkSortTrainerCmd\x12\n\n\x06\x43MD_ON\x10\x00\x12\x0b\n\x07\x43MD_OFF\x10\x01\",\n\x19SpkSortTrainerStatusReply\x12\x0f\n\x07msgJson\x18\x01 \x02(\x0c\"W\n\x0eWrangleRequest\x12!\n\x04mode\x18\x01 \x02(\x0e\x32\x13.allego.WrangleMode\x12\"\n\x04spec\x18\x02 \x02(\x0b\x32\x14.allego.WrangleMerge\"Y\n\x0bWrangleSpec\x12%\n\x06import\x18\x01 \x03(\x0b\x32\x15.allego.WrangleImport\x12#\n\x05merge\x18\x02 \x03(\x0b\x32\x14.allego.WrangleMerge\"H\n\rWrangleImport\x12\x37\n\x0cvexSpikesSim\x18\x01 \x01(\x0b\x32!.allego.WrangleImportVexSpikesSim\"g\n\x19WrangleImportVexSpikesSim\x12\'\n\x06source\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x13\n\x0bisOverwrite\x18\x02 \x01(\x08\x12\x0c\n\x04note\x18\x03 \x01(\t\"C\n\x0fWrangleFileDesc\x12\x0c\n\x04path\x18\x01 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x02(\t\x12\x10\n\x08\x66ileType\x18\x03 \x01(\t\"H\n\x0cWrangleMerge\x12\x38\n\rvexSpikesView\x18\x01 \x01(\x0b\x32!.allego.WrangleMergeVexSpikesView\"\xaf\x02\n\x19WrangleMergeVexSpikesView\x12*\n\tsourceVex\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12*\n\tsourceBio\x18\x02 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x33\n\x04view\x18\x03 \x03(\x0b\x32%.allego.WrangleMergeVexSpikesViewSpec\x12\x0c\n\x04note\x18\x04 \x01(\t\x12\x18\n\x10isBandpassFilter\x18\x05 \x01(\x08\x12\x1a\n\x12\x62\x61ndpassFilterSpec\x18\x06 \x03(\x01\x12\x13\n\x0bisOverwrite\x18\x07 \x01(\x08\x12\x15\n\rspikeWindowMs\x18\x08 \x03(\x01\x12\x15\n\rspikeShadowMs\x18\t \x01(\x01\"\xc0\x01\n\x1dWrangleMergeVexSpikesViewSpec\x12(\n\x07sinkBio\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x1c\n\x14siteNeighborRadiusUm\x18\x02 \x01(\x01\x12\x1b\n\x13reqNumSiteNeighbors\x18\x03 \x01(\x05\x12\x15\n\rspikeWindowMs\x18\x04 \x03(\x01\x12\x15\n\rspikeShadowMs\x18\x05 \x01(\x01\x12\x0c\n\x04note\x18\x06 \x01(\t\"\xa2\x01\n\x0cRecgenImport\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x01(\t\x12(\n\x08\x66ileType\x18\x05 \x01(\x0e\x32\x16.allego.RadixFileTypes\x12\x14\n\x0cnbhdRadiusUm\x18\x06 \x01(\x01\x12\x32\n\x10\x64\x65\x63InputFeatures\x18\x07 \x01(\x0e\x32\x18.allego.DecInputFeatures*\x81\x01\n\x19SpkSortTrainerNetworkSize\x12\x14\n\x10SST_SIZE_DEFAULT\x10\x00\x12\x10\n\x0cSST_SIZE_ARB\x10\x01\x12\x12\n\x0eSST_SIZE_SMALL\x10\x02\x12\x14\n\x10SST_SIZE_NOMINAL\x10\x03\x12\x12\n\x0eSST_SIZE_LARGE\x10\x04*\xa1\x01\n\x1dSpkSortTrainerNeighborPattern\x12\x17\n\x13SST_PATTERN_DEFAULT\x10\x00\x12\x13\n\x0fSST_PATTERN_ARB\x10\x01\x12\x14\n\x10SST_PATTERN_DIST\x10\x02\x12\x1d\n\x19SST_PATTERN_SPATIAL_TIGHT\x10\x03\x12\x1d\n\x19SST_PATTERN_SPATIAL_LOOSE\x10\x04*\xe3\x01\n\x1cSpkSortTrainerNetworkRelease\x12\x17\n\x13SST_NET_RELEASE_ANY\x10\x00\x12\x17\n\x13SST_NET_RELEASE_DEV\x10\x01\x12\x1b\n\x17SST_NET_RELEASE_DEV_MOD\x10\x02\x12\x18\n\x14SST_NET_RELEASE_PROD\x10\x03\x12\x1c\n\x18SST_NET_RELEASE_PROD_MOD\x10\x04\x12\x1b\n\x17SST_NET_RELEASE_SANDBOX\x10\x05\x12\x1f\n\x1bSST_NET_RELEASE_SANDBOX_MOD\x10\x06*\x83\x01\n\x0bWrangleMode\x12*\n&WRANGLE_MODE_IMPORT_NNX_VEX_SPIKES_SIM\x10\x00\x12\x1f\n\x1bWRANGLE_MODE_MERGE_FIT_VIEW\x10\x01\x12\'\n#WRANGLE_MODE_IMPORT_KILOSORT_SPIKES\x10\x02\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11radiens_dev.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x11spikesorter.proto\x1a\x10\x64\x61tasource.proto\"\xce\x01\n\x14SpkSortTrainerNewReq\x12\x33\n\x07\x64\x61taset\x18\x01 \x02(\x0b\x32\".allego.SpkSortTrainerDatasetParam\x12=\n\x08training\x18\x02 \x02(\x0b\x32+.allego.SpkSortTrainerNetworkTrainingParams\x12\x34\n\x05store\x18\x03 \x02(\x0b\x32%.allego.SpkSortTrainerStoreDescriptor\x12\x0c\n\x04seed\x18\x04 \x01(\x03\"[\n\x18SpkSortTrainerProfileReq\x12\x31\n\x07\x64srcReq\x18\x01 \x02(\x0b\x32 .allego.DataSourceSetSaveRequest\x12\x0c\n\x04path\x18\x02 \x02(\t\"l\n\x1cSpkSortTrainerDeleteModelReq\x12\x35\n\x07release\x18\x01 \x01(\x0e\x32$.allego.SpkSortTrainerNetworkRelease\x12\x15\n\risDeleteNamed\x18\x02 \x01(\x08\"\xc7\x02\n\x1aSpkSortTrainerDatasetParam\x12\x13\n\x0bniPathTrain\x18\x01 \x02(\t\x12\x17\n\x0fniBaseNameTrain\x18\x02 \x02(\t\x12\x0f\n\x07NbhdDim\x18\x07 \x02(\x05\x12\x10\n\x08radiusUm\x18\x08 \x02(\x01\x12\x19\n\x11maxNumSamplesTest\x18\t \x02(\x03\x12\x1a\n\x12networkMaskingFrac\x18\n \x02(\x01\x12 \n\x18networkInitWeightsStdDev\x18\x0b \x02(\x01\x12\x1d\n\x15networkInitBiasStdDev\x18\x0c \x02(\x01\x12\x17\n\x0fnetworkL1lambda\x18\r \x02(\x01\x12*\n\"networkHiddenLayerShapeRelInputDim\x18\x0e \x03(\x01\x12\x1b\n\x13networkNumFeatures2\x18\x0f \x02(\x05\"\xbd\x01\n#SpkSortTrainerNetworkTrainingParams\x12\x11\n\tnumEpochs\x18\x01 \x02(\x05\x12\x15\n\rminibatchSize\x18\x02 \x02(\x05\x12\x15\n\rmaxNumSamples\x18\x03 \x02(\x03\x12\r\n\x05\x61lpha\x18\x04 \x02(\x01\x12\x11\n\talphaBias\x18\x05 \x02(\x01\x12\x18\n\x10\x65rrorTolPretrain\x18\x06 \x02(\x01\x12\x19\n\x11numSamplesTestMSE\x18\x07 \x02(\x05\"\xb6\x02\n\x1dSpkSortTrainerStoreDescriptor\x12\x13\n\x0b\x62rainRegion\x18\x01 \x02(\t\x12\x36\n\x0bnetworkSize\x18\x02 \x02(\x0e\x32!.allego.SpkSortTrainerNetworkSize\x12\x39\n\nnbrPattern\x18\x03 \x02(\x0e\x32%.allego.SpkSortTrainerNeighborPattern\x12\x11\n\tnetworkID\x18\x04 \x02(\t\x12\x0f\n\x07NbhdDim\x18\x05 \x02(\x05\x12\x35\n\x07release\x18\x06 \x02(\x0e\x32$.allego.SpkSortTrainerNetworkRelease\x12\x32\n\x10\x64\x65\x63InputFeatures\x18\x07 \x02(\x0e\x32\x18.allego.DecInputFeatures\"(\n\x18SpkSortTrainerSetModeReq\x12\x0c\n\x04mode\x18\x01 \x02(\x05\"\x81\x01\n\x14SpkSortTrainerCmdReq\x12;\n\x03\x63md\x18\x01 \x02(\x0e\x32..allego.SpkSortTrainerCmdReq.SpkSortTrainerCmd\",\n\x11SpkSortTrainerCmd\x12\n\n\x06\x43MD_ON\x10\x00\x12\x0b\n\x07\x43MD_OFF\x10\x01\",\n\x19SpkSortTrainerStatusReply\x12\x0f\n\x07msgJson\x18\x01 \x02(\x0c\"W\n\x0eWrangleRequest\x12!\n\x04mode\x18\x01 \x02(\x0e\x32\x13.allego.WrangleMode\x12\"\n\x04spec\x18\x02 \x02(\x0b\x32\x14.allego.WrangleMerge\"Y\n\x0bWrangleSpec\x12%\n\x06import\x18\x01 \x03(\x0b\x32\x15.allego.WrangleImport\x12#\n\x05merge\x18\x02 \x03(\x0b\x32\x14.allego.WrangleMerge\"H\n\rWrangleImport\x12\x37\n\x0cvexSpikesSim\x18\x01 \x01(\x0b\x32!.allego.WrangleImportVexSpikesSim\"g\n\x19WrangleImportVexSpikesSim\x12\'\n\x06source\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x13\n\x0bisOverwrite\x18\x02 \x01(\x08\x12\x0c\n\x04note\x18\x03 \x01(\t\"C\n\x0fWrangleFileDesc\x12\x0c\n\x04path\x18\x01 \x02(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x02(\t\x12\x10\n\x08\x66ileType\x18\x03 \x01(\t\"H\n\x0cWrangleMerge\x12\x38\n\rvexSpikesView\x18\x01 \x01(\x0b\x32!.allego.WrangleMergeVexSpikesView\"\xaf\x02\n\x19WrangleMergeVexSpikesView\x12*\n\tsourceVex\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12*\n\tsourceBio\x18\x02 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x33\n\x04view\x18\x03 \x03(\x0b\x32%.allego.WrangleMergeVexSpikesViewSpec\x12\x0c\n\x04note\x18\x04 \x01(\t\x12\x18\n\x10isBandpassFilter\x18\x05 \x01(\x08\x12\x1a\n\x12\x62\x61ndpassFilterSpec\x18\x06 \x03(\x01\x12\x13\n\x0bisOverwrite\x18\x07 \x01(\x08\x12\x15\n\rspikeWindowMs\x18\x08 \x03(\x01\x12\x15\n\rspikeShadowMs\x18\t \x01(\x01\"\xc0\x01\n\x1dWrangleMergeVexSpikesViewSpec\x12(\n\x07sinkBio\x18\x01 \x02(\x0b\x32\x17.allego.WrangleFileDesc\x12\x1c\n\x14siteNeighborRadiusUm\x18\x02 \x01(\x01\x12\x1b\n\x13reqNumSiteNeighbors\x18\x03 \x01(\x05\x12\x15\n\rspikeWindowMs\x18\x04 \x03(\x01\x12\x15\n\rspikeShadowMs\x18\x05 \x01(\x01\x12\x0c\n\x04note\x18\x06 \x01(\t\"\xa2\x01\n\x0cRecgenImport\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x10\n\x08\x62\x61seName\x18\x02 \x01(\t\x12(\n\x08\x66ileType\x18\x05 \x01(\x0e\x32\x16.allego.RadixFileTypes\x12\x14\n\x0cnbhdRadiusUm\x18\x06 \x01(\x01\x12\x32\n\x10\x64\x65\x63InputFeatures\x18\x07 \x01(\x0e\x32\x18.allego.DecInputFeatures*\x81\x01\n\x19SpkSortTrainerNetworkSize\x12\x14\n\x10SST_SIZE_DEFAULT\x10\x00\x12\x10\n\x0cSST_SIZE_ARB\x10\x01\x12\x12\n\x0eSST_SIZE_SMALL\x10\x02\x12\x14\n\x10SST_SIZE_NOMINAL\x10\x03\x12\x12\n\x0eSST_SIZE_LARGE\x10\x04*\xa1\x01\n\x1dSpkSortTrainerNeighborPattern\x12\x17\n\x13SST_PATTERN_DEFAULT\x10\x00\x12\x13\n\x0fSST_PATTERN_ARB\x10\x01\x12\x14\n\x10SST_PATTERN_DIST\x10\x02\x12\x1d\n\x19SST_PATTERN_SPATIAL_TIGHT\x10\x03\x12\x1d\n\x19SST_PATTERN_SPATIAL_LOOSE\x10\x04*\xe3\x01\n\x1cSpkSortTrainerNetworkRelease\x12\x17\n\x13SST_NET_RELEASE_ANY\x10\x00\x12\x17\n\x13SST_NET_RELEASE_DEV\x10\x01\x12\x1b\n\x17SST_NET_RELEASE_DEV_MOD\x10\x02\x12\x18\n\x14SST_NET_RELEASE_PROD\x10\x03\x12\x1c\n\x18SST_NET_RELEASE_PROD_MOD\x10\x04\x12\x1b\n\x17SST_NET_RELEASE_SANDBOX\x10\x05\x12\x1f\n\x1bSST_NET_RELEASE_SANDBOX_MOD\x10\x06*\x83\x01\n\x0bWrangleMode\x12*\n&WRANGLE_MODE_IMPORT_NNX_VEX_SPIKES_SIM\x10\x00\x12\x1f\n\x1bWRANGLE_MODE_MERGE_FIT_VIEW\x10\x01\x12\'\n#WRANGLE_MODE_IMPORT_KILOSORT_SPIKES\x10\x02\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'radiens_dev_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
-  _SPKSORTTRAINERNETWORKSIZE._serialized_start=2743
-  _SPKSORTTRAINERNETWORKSIZE._serialized_end=2872
-  _SPKSORTTRAINERNEIGHBORPATTERN._serialized_start=2875
-  _SPKSORTTRAINERNEIGHBORPATTERN._serialized_end=3036
-  _SPKSORTTRAINERNETWORKRELEASE._serialized_start=3039
-  _SPKSORTTRAINERNETWORKRELEASE._serialized_end=3266
-  _WRANGLEMODE._serialized_start=3269
-  _WRANGLEMODE._serialized_end=3400
-  _SPKSORTTRAINERNEWREQ._serialized_start=63
-  _SPKSORTTRAINERNEWREQ._serialized_end=255
-  _SPKSORTTRAINERDELETEMODELREQ._serialized_start=257
-  _SPKSORTTRAINERDELETEMODELREQ._serialized_end=365
-  _SPKSORTTRAINERDATASETPARAM._serialized_start=368
-  _SPKSORTTRAINERDATASETPARAM._serialized_end=847
-  _SPKSORTTRAINERNETWORKTRAININGPARAMS._serialized_start=850
-  _SPKSORTTRAINERNETWORKTRAININGPARAMS._serialized_end=1039
-  _SPKSORTTRAINERSTOREDESCRIPTOR._serialized_start=1042
-  _SPKSORTTRAINERSTOREDESCRIPTOR._serialized_end=1352
-  _SPKSORTTRAINERSETMODEREQ._serialized_start=1354
-  _SPKSORTTRAINERSETMODEREQ._serialized_end=1394
-  _SPKSORTTRAINERCMDREQ._serialized_start=1397
-  _SPKSORTTRAINERCMDREQ._serialized_end=1526
-  _SPKSORTTRAINERCMDREQ_SPKSORTTRAINERCMD._serialized_start=1482
-  _SPKSORTTRAINERCMDREQ_SPKSORTTRAINERCMD._serialized_end=1526
-  _SPKSORTTRAINERSTATUSREPLY._serialized_start=1528
-  _SPKSORTTRAINERSTATUSREPLY._serialized_end=1572
-  _WRANGLEREQUEST._serialized_start=1574
-  _WRANGLEREQUEST._serialized_end=1661
-  _WRANGLESPEC._serialized_start=1663
-  _WRANGLESPEC._serialized_end=1752
-  _WRANGLEIMPORT._serialized_start=1754
-  _WRANGLEIMPORT._serialized_end=1826
-  _WRANGLEIMPORTVEXSPIKESSIM._serialized_start=1828
-  _WRANGLEIMPORTVEXSPIKESSIM._serialized_end=1931
-  _WRANGLEFILEDESC._serialized_start=1933
-  _WRANGLEFILEDESC._serialized_end=2000
-  _WRANGLEMERGE._serialized_start=2002
-  _WRANGLEMERGE._serialized_end=2074
-  _WRANGLEMERGEVEXSPIKESVIEW._serialized_start=2077
-  _WRANGLEMERGEVEXSPIKESVIEW._serialized_end=2380
-  _WRANGLEMERGEVEXSPIKESVIEWSPEC._serialized_start=2383
-  _WRANGLEMERGEVEXSPIKESVIEWSPEC._serialized_end=2575
-  _RECGENIMPORT._serialized_start=2578
-  _RECGENIMPORT._serialized_end=2740
+  _SPKSORTTRAINERNETWORKSIZE._serialized_start=2716
+  _SPKSORTTRAINERNETWORKSIZE._serialized_end=2845
+  _SPKSORTTRAINERNEIGHBORPATTERN._serialized_start=2848
+  _SPKSORTTRAINERNEIGHBORPATTERN._serialized_end=3009
+  _SPKSORTTRAINERNETWORKRELEASE._serialized_start=3012
+  _SPKSORTTRAINERNETWORKRELEASE._serialized_end=3239
+  _WRANGLEMODE._serialized_start=3242
+  _WRANGLEMODE._serialized_end=3373
+  _SPKSORTTRAINERNEWREQ._serialized_start=81
+  _SPKSORTTRAINERNEWREQ._serialized_end=287
+  _SPKSORTTRAINERPROFILEREQ._serialized_start=289
+  _SPKSORTTRAINERPROFILEREQ._serialized_end=380
+  _SPKSORTTRAINERDELETEMODELREQ._serialized_start=382
+  _SPKSORTTRAINERDELETEMODELREQ._serialized_end=490
+  _SPKSORTTRAINERDATASETPARAM._serialized_start=493
+  _SPKSORTTRAINERDATASETPARAM._serialized_end=820
+  _SPKSORTTRAINERNETWORKTRAININGPARAMS._serialized_start=823
+  _SPKSORTTRAINERNETWORKTRAININGPARAMS._serialized_end=1012
+  _SPKSORTTRAINERSTOREDESCRIPTOR._serialized_start=1015
+  _SPKSORTTRAINERSTOREDESCRIPTOR._serialized_end=1325
+  _SPKSORTTRAINERSETMODEREQ._serialized_start=1327
+  _SPKSORTTRAINERSETMODEREQ._serialized_end=1367
+  _SPKSORTTRAINERCMDREQ._serialized_start=1370
+  _SPKSORTTRAINERCMDREQ._serialized_end=1499
+  _SPKSORTTRAINERCMDREQ_SPKSORTTRAINERCMD._serialized_start=1455
+  _SPKSORTTRAINERCMDREQ_SPKSORTTRAINERCMD._serialized_end=1499
+  _SPKSORTTRAINERSTATUSREPLY._serialized_start=1501
+  _SPKSORTTRAINERSTATUSREPLY._serialized_end=1545
+  _WRANGLEREQUEST._serialized_start=1547
+  _WRANGLEREQUEST._serialized_end=1634
+  _WRANGLESPEC._serialized_start=1636
+  _WRANGLESPEC._serialized_end=1725
+  _WRANGLEIMPORT._serialized_start=1727
+  _WRANGLEIMPORT._serialized_end=1799
+  _WRANGLEIMPORTVEXSPIKESSIM._serialized_start=1801
+  _WRANGLEIMPORTVEXSPIKESSIM._serialized_end=1904
+  _WRANGLEFILEDESC._serialized_start=1906
+  _WRANGLEFILEDESC._serialized_end=1973
+  _WRANGLEMERGE._serialized_start=1975
+  _WRANGLEMERGE._serialized_end=2047
+  _WRANGLEMERGEVEXSPIKESVIEW._serialized_start=2050
+  _WRANGLEMERGEVEXSPIKESVIEW._serialized_end=2353
+  _WRANGLEMERGEVEXSPIKESVIEWSPEC._serialized_start=2356
+  _WRANGLEMERGEVEXSPIKESVIEWSPEC._serialized_end=2548
+  _RECGENIMPORT._serialized_start=2551
+  _RECGENIMPORT._serialized_end=2713
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-3.0.0b4/radiens/grpc_radiens/radiensserver_pb2.py` & `radiens-3.0.0b5/radiens/grpc_radiens/radiensserver_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from . import common_pb2 as common__pb2
 from . import datasource_pb2 as datasource__pb2
 from . import biointerface_pb2 as biointerface__pb2
 from . import spikesorter_pb2 as spikesorter__pb2
 from . import radiens_dev_pb2 as radiens__dev__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13radiensserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\x1a\x11radiens_dev.proto\"K\n\x19RadiensHealthcheckRequest\x12\x1a\n\x12isIncludeWarehouse\x18\x01 \x01(\x08\x12\x12\n\nisDetailed\x18\x02 \x01(\x08\"]\n\x16RadiensHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\x12\x33\n\toutfitter\x18\x02 \x01(\x0b\x32 .allego.WarehouseHealthcheckSpec\"\x1e\n\x0fRadiensClientId\x12\x0b\n\x03pid\x18\x01 \x02(\x05\"\x91\x01\n\x12SummaSessionsReply\x12?\n\x07session\x18\x01 \x03(\x0b\x32..allego.SummaSessionsReply.SummaCurrentSession\x1a:\n\x13SummaCurrentSession\x12\x0f\n\x07summaID\x18\x01 \x02(\t\x12\x12\n\ndsourceIDs\x18\x02 \x03(\t\"_\n\x14SummaAnalysisRequest\x12\x0f\n\x07summaID\x18\x01 \x01(\t\x12\x12\n\ndsourceIDs\x18\x02 \x03(\t\x12\x11\n\tpktDurSec\x18\x03 \x01(\x01\x12\x0f\n\x07reqPart\x18\x04 \x01(\t\"\xa1\x02\n\x12SummaAnalysisReply\x12\x0f\n\x07summaID\x18\x01 \x01(\t\x12\x15\n\rallDsourceIDs\x18\x02 \x03(\t\x12!\n\x05state\x18\x03 \x01(\x0b\x32\x12.allego.SummaState\x12\x33\n\x0e\x61llDsourceSpec\x18\x04 \x03(\x0b\x32\x1b.allego.SummaDatasourceSpec\x12-\n\x08\x61ggStats\x18\x05 \x01(\x0b\x32\x1b.allego.SummaAggregateStats\x12@\n\x14reqAvailDsourceStats\x18\x06 \x03(\x0b\x32\".allego.SummaDatasourceAnalysisPkg\x12\x1a\n\x12reqAvailDsourceIDs\x18\x07 \x03(\t\"\xd9\x01\n\nSummaState\x12\x0f\n\x07summaID\x18\x01 \x02(\t\x12\x12\n\nisComplete\x18\x02 \x02(\x08\x12\x14\n\x0c\x66racComplete\x18\x03 \x02(\x01\x12\x0b\n\x03msg\x18\x04 \x02(\t\x12\x19\n\x11\x64srcWalltimeStart\x18\x05 \x02(\t\x12\x17\n\x0f\x64srcWalltimeEnd\x18\x06 \x02(\t\x12\x1d\n\x15\x61nalysisWallTimeStart\x18\x07 \x02(\t\x12\x1a\n\x12\x61nalysisElapsedSec\x18\x08 \x02(\x01\x12\x14\n\x0cpacketDurSec\x18\t \x02(\x01\"]\n\x13SummaAggregateStats\x12%\n\x08metricID\x18\x01 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x1f\n\x04hist\x18\x02 \x03(\x0b\x32\x11.allego.Histogram\"\xbd\x01\n\x1aSummaDatasourceAnalysisPkg\x12%\n\x08metricID\x18\x01 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x1f\n\x04hist\x18\x02 \x03(\x0b\x32\x11.allego.Histogram\x12!\n\x04recs\x18\x03 \x03(\x0b\x32\x13.allego.DenseMatrix\x12#\n\x08histRecs\x18\x04 \x03(\x0b\x32\x11.allego.Histogram\x12\x0f\n\x07ntvIdxs\x18\x05 \x03(\x03\"~\n\x13SummaDatasourceSpec\x12\x1f\n\x02sG\x18\x01 \x01(\x0b\x32\x13.allego.SignalGroup\x12\x1d\n\x02tR\x18\x02 \x01(\x0b\x32\x11.allego.TimeRange\x12\'\n\x06niSpec\x18\x03 \x01(\x0b\x32\x17.allego.SpikesSpecReply2\xfc\x32\n\x0bRadiensCore\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12\x41\n\rClientConnect\x12\x17.allego.RadiensClientId\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x10\x43lientDisconnect\x12\x17.allego.RadiensClientId\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12R\n\x17GetOfflineLicenseStatus\x12\x17.allego.StandardRequest\x1a\x1c.allego.OfflineLicenseStatus\"\x00\x12H\n\rListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12V\n\x12\x43opyDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12X\n\x14RemoveDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12P\n\x12MoveDataSourceFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12N\n\x13SpikesListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12R\n\x0eSpikesCopyFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x10SpikesRemoveFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12L\n\x0eSpikesMoveFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x16ManageNodeOrganization\x12\x1c.allego.ManageNodeOrgRequest\x1a\x1a.allego.ManageNodeOrgReply\"\x00\x12K\n\rManageNodeLab\x12\x1c.allego.ManageNodeLabRequest\x1a\x1a.allego.ManageNodeLabReply\"\x00\x12N\n\x0eManageNodeUser\x12\x1d.allego.ManageNodeUserRequest\x1a\x1b.allego.ManageNodeUserReply\"\x00\x12\x45\n\x0fManageNodeProbe\x12\x18.allego.ProbeNodeRequest\x1a\x16.allego.ProbeNodeReply\"\x00\x12\x41\n\x0bManageEdges\x12\x18.allego.WorldEdgeRequest\x1a\x16.allego.WorldEdgeReply\"\x00\x12\x42\n\nQueryWorld\x12\x19.allego.QueryWorldRequest\x1a\x17.allego.QueryWorldReply\"\x00\x12V\n\x1bGetWarehouseSensorComponent\x12\x19.allego.SensorCompRequest\x1a\x1a.allego.GetSensorCompReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12H\n\x0eGetSorterIDMap\x12\x17.allego.StandardRequest\x1a\x1b.allego.GetSorterIDMapReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x0fGetHDSnapshotPy\x12\x1a.allego.HDSnapshotRequest2\x1a\x13.allego.HDSnapshot2\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12+\n\x06GetPSD\x12\x12.allego.PSDRequest\x1a\x0b.allego.PSD\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12J\n\x0eListDataSource\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12K\n\x11ListDataSourceIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12[\n\x15SetDataSourceFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12I\n\x0f\x43learDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12J\n\x10RenameDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12P\n\x1aGetDataSourceKpiFileStatus\x12\x19.allego.DataSourceRequest\x1a\x15.allego.KpiFileStatus\"\x00\x12R\n\x1bGetDataSourceKpiFileStatus2\x12\x19.allego.DataSourceRequest\x1a\x16.allego.KpiFileStatus2\"\x00\x12\x46\n\x0eGetKpiMetadata\x12\x19.allego.DataSourceRequest\x1a\x17.allego.KpiFileMetadata\"\x00\x12?\n\x08KpiClear\x12\x1a.allego.KpiStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0cKpiCalculate\x12\x1a.allego.KpiStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12\x46\n\x0fSetKpiPacketDur\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x12K\n\x0bSetKpiParam\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x0bGetKpiParam\x12\x19.allego.DataSourceRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12W\n\x11SpikesSetFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12\x46\n\x0cSpikesGetIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12H\n\x0eSpikesRenameID\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12S\n\x17SpikesGetAllSummaryInfo\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12\x45\n\rSpikesGetSpec\x12\x19.allego.DataSourceRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12\x64\n\x13SpikesGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12[\n\x14SpikesGetSpikesDense\x12\x1e.allego.SpikesGetSpikesRequest\x1a!.allego.SpikesSpikeDataDenseReply\"\x00\x12q\n\x15GetSpikeTrainAnalytic\x12+.allego.SpikesGetSpikeTrainAnalyticsRequest\x1a).allego.SpikesGetSpikeTrainAnalyticsReply\"\x00\x12I\n\x0fSpikesDeleteIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12l\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x11.allego.TimeRange\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x12[\n\x1b\x42iointerfaceListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12J\n\x15\x42iointerfaceSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12`\n BiointerfaceSetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12^\n\x1f\x42iointerfaceSetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x11\x44\x65leteSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x12K\n\x14SpikesGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12\x33\n\x0bSetProtocol\x12\x10.allego.Protocol\x1a\x10.allego.Protocol\"\x00\x12:\n\x0bGetProtocol\x12\x17.allego.ProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12\x43\n\x0eRenameProtocol\x12\x1d.allego.RenameProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12J\n\x0fGetAllProtocols\x12\x17.allego.StandardRequest\x1a\x1c.allego.GetAllProtocolsReply\"\x00\x12K\n\rApplyProtocol\x12\x17.allego.ProtocolRequest\x1a\x1d.allego.ApplyProtocolProgress\"\x00\x30\x01\x32\xc1\x07\n\x13RadiensSpikeSorter1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x63\n\x17SpikeSorterGetDashboard\x12#.allego.SpikeSorterDashboardRequest\x1a!.allego.SpikeSorterDashboardReply\"\x00\x12I\n\x16SpikeSorterWrangleData\x12\x16.allego.WrangleRequest\x1a\x15.allego.StandardReply\"\x00\x12W\n\x11SpikeSorterLaunch\x12 .allego.SpikeSorterLaunchRequest\x1a\x1e.allego.SpikeSorterLaunchReply\"\x00\x12P\n\x11SpikeSorterDelete\x12\".allego.SpikeSorterStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12H\n\x17SpikeSorterImportMearec\x12\x14.allego.RecgenImport\x1a\x15.allego.StandardReply\"\x00\x32\xe2\x03\n\nDashboards\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12L\n\x10\x43ommandDashboard\x12\x1f.allego.DashboardCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x15LaunchSessionAnalysis\x12\x1c.allego.SummaAnalysisRequest\x1a\x1a.allego.SummaAnalysisReply\"\x00\x12P\n\x12GetSessionAnalysis\x12\x1c.allego.SummaAnalysisRequest\x1a\x1a.allego.SummaAnalysisReply\"\x00\x12\x45\n\x0cListSessions\x12\x17.allego.StandardRequest\x1a\x1a.allego.SummaSessionsReply\"\x00\x12\x44\n\x10\x43learAllSessions\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x32\xb7\x04\n\x0bRadiensDev1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12S\n\x1aSpkSortTrainerMakeNewModel\x12\x1c.allego.SpkSortTrainerNewReq\x1a\x15.allego.StandardReply\"\x00\x12W\n#SpkSortTrainerMakeDefaultProdModels\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n$SpkSortTrainerListLocalNetworkModels\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x12g\n&SpkSortTrainerDeleteLocalNetworkModels\x12$.allego.SpkSortTrainerDeleteModelReq\x1a\x15.allego.StandardReply\"\x00\x12W\n\x17SpkSortTrainerGetStatus\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x42\x15Z\x13internal/radix/grpc')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13radiensserver.proto\x12\x06\x61llego\x1a\x0c\x63ommon.proto\x1a\x10\x64\x61tasource.proto\x1a\x12\x62iointerface.proto\x1a\x11spikesorter.proto\x1a\x11radiens_dev.proto\"K\n\x19RadiensHealthcheckRequest\x12\x1a\n\x12isIncludeWarehouse\x18\x01 \x01(\x08\x12\x12\n\nisDetailed\x18\x02 \x01(\x08\"]\n\x16RadiensHealthcheckSpec\x12\x0e\n\x06\x65rrMsg\x18\x01 \x01(\t\x12\x33\n\toutfitter\x18\x02 \x01(\x0b\x32 .allego.WarehouseHealthcheckSpec\"\x1e\n\x0fRadiensClientId\x12\x0b\n\x03pid\x18\x01 \x02(\x05\"\x91\x01\n\x12SummaSessionsReply\x12?\n\x07session\x18\x01 \x03(\x0b\x32..allego.SummaSessionsReply.SummaCurrentSession\x1a:\n\x13SummaCurrentSession\x12\x0f\n\x07summaID\x18\x01 \x02(\t\x12\x12\n\ndsourceIDs\x18\x02 \x03(\t\"_\n\x14SummaAnalysisRequest\x12\x0f\n\x07summaID\x18\x01 \x01(\t\x12\x12\n\ndsourceIDs\x18\x02 \x03(\t\x12\x11\n\tpktDurSec\x18\x03 \x01(\x01\x12\x0f\n\x07reqPart\x18\x04 \x01(\t\"\xa1\x02\n\x12SummaAnalysisReply\x12\x0f\n\x07summaID\x18\x01 \x01(\t\x12\x15\n\rallDsourceIDs\x18\x02 \x03(\t\x12!\n\x05state\x18\x03 \x01(\x0b\x32\x12.allego.SummaState\x12\x33\n\x0e\x61llDsourceSpec\x18\x04 \x03(\x0b\x32\x1b.allego.SummaDatasourceSpec\x12-\n\x08\x61ggStats\x18\x05 \x01(\x0b\x32\x1b.allego.SummaAggregateStats\x12@\n\x14reqAvailDsourceStats\x18\x06 \x03(\x0b\x32\".allego.SummaDatasourceAnalysisPkg\x12\x1a\n\x12reqAvailDsourceIDs\x18\x07 \x03(\t\"\xd9\x01\n\nSummaState\x12\x0f\n\x07summaID\x18\x01 \x02(\t\x12\x12\n\nisComplete\x18\x02 \x02(\x08\x12\x14\n\x0c\x66racComplete\x18\x03 \x02(\x01\x12\x0b\n\x03msg\x18\x04 \x02(\t\x12\x19\n\x11\x64srcWalltimeStart\x18\x05 \x02(\t\x12\x17\n\x0f\x64srcWalltimeEnd\x18\x06 \x02(\t\x12\x1d\n\x15\x61nalysisWallTimeStart\x18\x07 \x02(\t\x12\x1a\n\x12\x61nalysisElapsedSec\x18\x08 \x02(\x01\x12\x14\n\x0cpacketDurSec\x18\t \x02(\x01\"]\n\x13SummaAggregateStats\x12%\n\x08metricID\x18\x01 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x1f\n\x04hist\x18\x02 \x03(\x0b\x32\x11.allego.Histogram\"\xbd\x01\n\x1aSummaDatasourceAnalysisPkg\x12%\n\x08metricID\x18\x01 \x03(\x0b\x32\x13.allego.KpiMetricID\x12\x1f\n\x04hist\x18\x02 \x03(\x0b\x32\x11.allego.Histogram\x12!\n\x04recs\x18\x03 \x03(\x0b\x32\x13.allego.DenseMatrix\x12#\n\x08histRecs\x18\x04 \x03(\x0b\x32\x11.allego.Histogram\x12\x0f\n\x07ntvIdxs\x18\x05 \x03(\x03\"~\n\x13SummaDatasourceSpec\x12\x1f\n\x02sG\x18\x01 \x01(\x0b\x32\x13.allego.SignalGroup\x12\x1d\n\x02tR\x18\x02 \x01(\x0b\x32\x11.allego.TimeRange\x12\'\n\x06niSpec\x18\x03 \x01(\x0b\x32\x17.allego.SpikesSpecReply2\xfc\x32\n\x0bRadiensCore\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12\x41\n\rClientConnect\x12\x17.allego.RadiensClientId\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x10\x43lientDisconnect\x12\x17.allego.RadiensClientId\x1a\x15.allego.StandardReply\"\x00\x12\x39\n\x05\x43lose\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12L\n\x10WorkspaceControl\x12\x1f.allego.WorkspaceControlRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x11GetRadiensServers\x12 .allego.GetRadiensServersRequest\x1a\x1b.allego.RadiensServersReply\"\x00\x12H\n\x0cGetWorkspace\x12\x1b.allego.GetWorkspaceRequest\x1a\x19.allego.GetWorkspaceReply\"\x00\x12J\n\x13GetRadixEnvironment\x12\x17.allego.StandardRequest\x1a\x18.allego.RadixEnvironment\"\x00\x12R\n\x17GetOfflineLicenseStatus\x12\x17.allego.StandardRequest\x1a\x1c.allego.OfflineLicenseStatus\"\x00\x12H\n\rListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12V\n\x12\x43opyDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12X\n\x14RemoveDataSourceFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12P\n\x12MoveDataSourceFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12N\n\x13SpikesListDirectory\x12\x1e.allego.ListDataSourcesRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12R\n\x0eSpikesCopyFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x10SpikesRemoveFile\x12\'.allego.CopyRemoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12L\n\x0eSpikesMoveFile\x12!.allego.MoveDataSourceFileRequest\x1a\x15.allego.CpRmMvLsReply\"\x00\x12T\n\x16ManageNodeOrganization\x12\x1c.allego.ManageNodeOrgRequest\x1a\x1a.allego.ManageNodeOrgReply\"\x00\x12K\n\rManageNodeLab\x12\x1c.allego.ManageNodeLabRequest\x1a\x1a.allego.ManageNodeLabReply\"\x00\x12N\n\x0eManageNodeUser\x12\x1d.allego.ManageNodeUserRequest\x1a\x1b.allego.ManageNodeUserReply\"\x00\x12\x45\n\x0fManageNodeProbe\x12\x18.allego.ProbeNodeRequest\x1a\x16.allego.ProbeNodeReply\"\x00\x12\x41\n\x0bManageEdges\x12\x18.allego.WorldEdgeRequest\x1a\x16.allego.WorldEdgeReply\"\x00\x12\x42\n\nQueryWorld\x12\x19.allego.QueryWorldRequest\x1a\x17.allego.QueryWorldReply\"\x00\x12V\n\x1bGetWarehouseSensorComponent\x12\x19.allego.SensorCompRequest\x1a\x1a.allego.GetSensorCompReply\"\x00\x12O\n\x0fListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12>\n\tSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12T\n\x14SetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11UpdateSignalGroup\x12 .allego.UpdateSignalGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\x11GetSignalGroupIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSignalGroupIDsReply\"\x00\x12H\n\x0eGetSorterIDMap\x12\x17.allego.StandardRequest\x1a\x1b.allego.GetSorterIDMapReply\"\x00\x12N\n\x11GetSpikeSorterIDs\x12\x17.allego.StandardRequest\x1a\x1e.allego.GetSpikeSorterIDsReply\"\x00\x12\x45\n\x0eGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12O\n\x13GetDataSourceParams\x12\x1c.allego.SignalGroupIDRequest\x1a\x18.allego.DataSourceParams\"\x00\x12=\n\nGetSignals\x12\x19.allego.GetSignalsRequest\x1a\x12.allego.RawSignals\"\x00\x12\x41\n\x0cSetDACStream\x12\x18.allego.DACStreamRequest\x1a\x15.allego.StandardReply\"\x00\x12;\n\tSetDACOff\x12\x15.allego.DACOffRequest\x1a\x15.allego.StandardReply\"\x00\x12\x44\n\x0fGetHDSnapshotPy\x12\x1a.allego.HDSnapshotRequest2\x1a\x13.allego.HDSnapshot2\"\x00\x12@\n\rGetHDSnapshot\x12\x19.allego.HDSnapshotRequest\x1a\x12.allego.HDSnapshot\"\x00\x12+\n\x06GetPSD\x12\x12.allego.PSDRequest\x1a\x0b.allego.PSD\"\x00\x12\x42\n\x0bSetDSPGroup\x12\x1a.allego.SetDSPGroupRequest\x1a\x15.allego.StandardReply\"\x00\x12?\n\x0bGetDSPGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x10.allego.DSPGroup\"\x00\x12J\n\x0eListDataSource\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12K\n\x11ListDataSourceIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12[\n\x15SetDataSourceFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12I\n\x0f\x43learDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12J\n\x10RenameDataSource\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12P\n\x1aGetDataSourceKpiFileStatus\x12\x19.allego.DataSourceRequest\x1a\x15.allego.KpiFileStatus\"\x00\x12R\n\x1bGetDataSourceKpiFileStatus2\x12\x19.allego.DataSourceRequest\x1a\x16.allego.KpiFileStatus2\"\x00\x12\x46\n\x0eGetKpiMetadata\x12\x19.allego.DataSourceRequest\x1a\x17.allego.KpiFileMetadata\"\x00\x12?\n\x08KpiClear\x12\x1a.allego.KpiStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x43\n\x0cKpiCalculate\x12\x1a.allego.KpiStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x45\n\x0cGetKpiStatus\x12\x1b.allego.GetKpiStatusRequest\x1a\x16.allego.KpiStatusReply\"\x00\x12H\n\rKpiGetMetrics\x12\x15.allego.KpiMetricsReq\x1a\x1e.allego.KpiBundlePacketMetrics\"\x00\x12\x46\n\x0fSetKpiPacketDur\x12\x1a.allego.SetKpiParamRequest\x1a\x15.allego.StandardReply\"\x00\x12K\n\x0bSetKpiParam\x12#.allego.SpikeSorterSetParamsRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x0bGetKpiParam\x12\x19.allego.DataSourceRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12W\n\x11SpikesSetFromFile\x12 .allego.DataSourceSetSaveRequest\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x12\x46\n\x0cSpikesGetIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12H\n\x0eSpikesRenameID\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12S\n\x17SpikesGetAllSummaryInfo\x12\x19.allego.DataSourceRequest\x1a\x1b.allego.DataSourceStatusMap\"\x00\x12\x45\n\rSpikesGetSpec\x12\x19.allego.DataSourceRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12\x64\n\x13SpikesGetRasterData\x12\'.allego.SpikeSorterGetRasterDataRequest\x1a\".allego.SpikeSorterRasterDataReply\"\x00\x12[\n\x14SpikesGetSpikesDense\x12\x1e.allego.SpikesGetSpikesRequest\x1a!.allego.SpikesSpikeDataDenseReply\"\x00\x12q\n\x15GetSpikeTrainAnalytic\x12+.allego.SpikesGetSpikeTrainAnalyticsRequest\x1a).allego.SpikesGetSpikeTrainAnalyticsReply\"\x00\x12I\n\x0fSpikesDeleteIDs\x12\x19.allego.DataSourceRequest\x1a\x19.allego.DataSourceIDReply\"\x00\x12\x66\n\x16\x42iointerfaceGetNeurons\x12%.allego.BiointerfaceGetNeuronsRequest\x1a#.allego.BiointerfaceGetNeuronsReply\"\x00\x12l\n\"BiointerfaceSeekEndSpikeTimestamps\x12\x31.allego.BiointerfaceSeekEndSpikeTimestampsRequest\x1a\x11.allego.TimeRange\"\x00\x12Q\n\x0f\x42iointerfaceViz\x12\x1e.allego.BiointerfaceVizRequest\x1a\x1c.allego.BiointerfaceVizReply\"\x00\x12[\n\x1b\x42iointerfaceListSensorSpecs\x12\x1c.allego.SignalGroupIDRequest\x1a\x1c.allego.ListSensorSpecsReply\"\x00\x12J\n\x15\x42iointerfaceSetSensor\x12\x18.allego.SetSensorRequest\x1a\x15.allego.StandardReply\"\x00\x12`\n BiointerfaceSetSensorPositionTcs\x12#.allego.SetSensorPositionTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12^\n\x1f\x42iointerfaceSetSitePositionsTcs\x12\".allego.SetSitePositionsTcsRequest\x1a\x15.allego.StandardReply\"\x00\x12H\n\x0c\x46\x65\x61tureStart\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12G\n\x0b\x46\x65\x61tureStop\x12\x1f.allego.FeatureStartStopRequest\x1a\x15.allego.StandardReply\"\x00\x12=\n\nGetPrivacy\x12\x17.allego.StandardRequest\x1a\x14.allego.PrivacyReply\"\x00\x12@\n\nSetPrivacy\x12\x19.allego.SetPrivacyRequest\x1a\x15.allego.StandardReply\"\x00\x12J\n\x11\x44\x65leteSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x15.allego.StandardReply\"\x00\x12K\n\x14SpikesGetSignalGroup\x12\x1c.allego.SignalGroupIDRequest\x1a\x13.allego.SignalGroup\"\x00\x12\x33\n\x0bSetProtocol\x12\x10.allego.Protocol\x1a\x10.allego.Protocol\"\x00\x12:\n\x0bGetProtocol\x12\x17.allego.ProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12\x43\n\x0eRenameProtocol\x12\x1d.allego.RenameProtocolRequest\x1a\x10.allego.Protocol\"\x00\x12J\n\x0fGetAllProtocols\x12\x17.allego.StandardRequest\x1a\x1c.allego.GetAllProtocolsReply\"\x00\x12K\n\rApplyProtocol\x12\x17.allego.ProtocolRequest\x1a\x1d.allego.ApplyProtocolProgress\"\x00\x30\x01\x32\xca\x07\n\x13RadiensSpikeSorter1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12P\n\x12SpikeSorterCommand\x12!.allego.SpikeSorterCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12R\n\x13SpikeSorterSetParam\x12\".allego.SpikeSorterSetParamRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n\x13SpikeSorterGetParam\x12\".allego.SpikeSorterStandardRequest\x1a\'.allego.GetSpikeSorterParamCommandReply\"\x00\x12U\n\x13SpikeSorterGetState\x12\".allego.SpikeSorterStandardRequest\x1a\x18.allego.SpikeSorterState\"\x00\x12\x63\n\x17SpikeSorterGetDashboard\x12#.allego.SpikeSorterDashboardRequest\x1a!.allego.SpikeSorterDashboardReply\"\x00\x12I\n\x16SpikeSorterWrangleData\x12\x16.allego.WrangleRequest\x1a\x15.allego.StandardReply\"\x00\x12W\n\x11SpikeSorterLaunch\x12 .allego.SpikeSorterLaunchRequest\x1a\x1e.allego.SpikeSorterLaunchReply\"\x00\x12P\n\x11SpikeSorterDelete\x12\".allego.SpikeSorterStandardRequest\x1a\x15.allego.StandardReply\"\x00\x12N\n\rSpikesGetSpec\x12\".allego.SpikeSorterStandardRequest\x1a\x17.allego.SpikesSpecReply\"\x00\x12Q\n\x17SpikeSorterImportMearec\x12\x14.allego.RecgenImport\x1a\x1e.allego.DataSourceSetSaveReply\"\x00\x32\xe2\x03\n\nDashboards\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12L\n\x10\x43ommandDashboard\x12\x1f.allego.DashboardCommandRequest\x1a\x15.allego.StandardReply\"\x00\x12S\n\x15LaunchSessionAnalysis\x12\x1c.allego.SummaAnalysisRequest\x1a\x1a.allego.SummaAnalysisReply\"\x00\x12P\n\x12GetSessionAnalysis\x12\x1c.allego.SummaAnalysisRequest\x1a\x1a.allego.SummaAnalysisReply\"\x00\x12\x45\n\x0cListSessions\x12\x17.allego.StandardRequest\x1a\x1a.allego.SummaSessionsReply\"\x00\x12\x44\n\x10\x43learAllSessions\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x32\x90\x05\n\x0bRadiensDev1\x12R\n\x0bHealthcheck\x12!.allego.RadiensHealthcheckRequest\x1a\x1e.allego.RadiensHealthcheckSpec\"\x00\x12S\n\x1aSpkSortTrainerMakeNewModel\x12\x1c.allego.SpkSortTrainerNewReq\x1a\x15.allego.StandardReply\"\x00\x12W\n\x1aSpkSortTrainerProfileModel\x12 .allego.SpkSortTrainerProfileReq\x1a\x15.allego.StandardReply\"\x00\x12W\n#SpkSortTrainerMakeDefaultProdModels\x12\x17.allego.StandardRequest\x1a\x15.allego.StandardReply\"\x00\x12\x64\n$SpkSortTrainerListLocalNetworkModels\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x12g\n&SpkSortTrainerDeleteLocalNetworkModels\x12$.allego.SpkSortTrainerDeleteModelReq\x1a\x15.allego.StandardReply\"\x00\x12W\n\x17SpkSortTrainerGetStatus\x12\x17.allego.StandardRequest\x1a!.allego.SpkSortTrainerStatusReply\"\x00\x42\x15Z\x13internal/radix/grpc')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'radiensserver_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\023internal/radix/grpc'
@@ -47,13 +47,13 @@
   _SUMMADATASOURCEANALYSISPKG._serialized_start=1178
   _SUMMADATASOURCEANALYSISPKG._serialized_end=1367
   _SUMMADATASOURCESPEC._serialized_start=1369
   _SUMMADATASOURCESPEC._serialized_end=1495
   _RADIENSCORE._serialized_start=1498
   _RADIENSCORE._serialized_end=8022
   _RADIENSSPIKESORTER1._serialized_start=8025
-  _RADIENSSPIKESORTER1._serialized_end=8986
-  _DASHBOARDS._serialized_start=8989
-  _DASHBOARDS._serialized_end=9471
-  _RADIENSDEV1._serialized_start=9474
-  _RADIENSDEV1._serialized_end=10041
+  _RADIENSSPIKESORTER1._serialized_end=8995
+  _DASHBOARDS._serialized_start=8998
+  _DASHBOARDS._serialized_end=9480
+  _RADIENSDEV1._serialized_start=9483
+  _RADIENSDEV1._serialized_end=10139
 # @@protoc_insertion_point(module_scope)
```

### Comparing `radiens-3.0.0b4/radiens/grpc_radiens/radiensserver_pb2_grpc.py` & `radiens-3.0.0b5/radiens/grpc_radiens/radiensserver_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -2903,15 +2903,15 @@
                 '/allego.RadiensSpikeSorter1/SpikesGetSpec',
                 request_serializer=spikesorter__pb2.SpikeSorterStandardRequest.SerializeToString,
                 response_deserializer=biointerface__pb2.SpikesSpecReply.FromString,
                 )
         self.SpikeSorterImportMearec = channel.unary_unary(
                 '/allego.RadiensSpikeSorter1/SpikeSorterImportMearec',
                 request_serializer=radiens__dev__pb2.RecgenImport.SerializeToString,
-                response_deserializer=common__pb2.StandardReply.FromString,
+                response_deserializer=datasource__pb2.DataSourceSetSaveReply.FromString,
                 )
 
 
 class RadiensSpikeSorter1Servicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Healthcheck(self, request, context):
@@ -3035,15 +3035,15 @@
                     servicer.SpikesGetSpec,
                     request_deserializer=spikesorter__pb2.SpikeSorterStandardRequest.FromString,
                     response_serializer=biointerface__pb2.SpikesSpecReply.SerializeToString,
             ),
             'SpikeSorterImportMearec': grpc.unary_unary_rpc_method_handler(
                     servicer.SpikeSorterImportMearec,
                     request_deserializer=radiens__dev__pb2.RecgenImport.FromString,
-                    response_serializer=common__pb2.StandardReply.SerializeToString,
+                    response_serializer=datasource__pb2.DataSourceSetSaveReply.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'allego.RadiensSpikeSorter1', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -3230,15 +3230,15 @@
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/allego.RadiensSpikeSorter1/SpikeSorterImportMearec',
             radiens__dev__pb2.RecgenImport.SerializeToString,
-            common__pb2.StandardReply.FromString,
+            datasource__pb2.DataSourceSetSaveReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
 
 class DashboardsStub(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -3480,14 +3480,19 @@
                 response_deserializer=radiensserver__pb2.RadiensHealthcheckSpec.FromString,
                 )
         self.SpkSortTrainerMakeNewModel = channel.unary_unary(
                 '/allego.RadiensDev1/SpkSortTrainerMakeNewModel',
                 request_serializer=radiens__dev__pb2.SpkSortTrainerNewReq.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
+        self.SpkSortTrainerProfileModel = channel.unary_unary(
+                '/allego.RadiensDev1/SpkSortTrainerProfileModel',
+                request_serializer=radiens__dev__pb2.SpkSortTrainerProfileReq.SerializeToString,
+                response_deserializer=common__pb2.StandardReply.FromString,
+                )
         self.SpkSortTrainerMakeDefaultProdModels = channel.unary_unary(
                 '/allego.RadiensDev1/SpkSortTrainerMakeDefaultProdModels',
                 request_serializer=common__pb2.StandardRequest.SerializeToString,
                 response_deserializer=common__pb2.StandardReply.FromString,
                 )
         self.SpkSortTrainerListLocalNetworkModels = channel.unary_unary(
                 '/allego.RadiensDev1/SpkSortTrainerListLocalNetworkModels',
@@ -3517,14 +3522,20 @@
 
     def SpkSortTrainerMakeNewModel(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SpkSortTrainerProfileModel(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def SpkSortTrainerMakeDefaultProdModels(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SpkSortTrainerListLocalNetworkModels(self, request, context):
@@ -3555,14 +3566,19 @@
                     response_serializer=radiensserver__pb2.RadiensHealthcheckSpec.SerializeToString,
             ),
             'SpkSortTrainerMakeNewModel': grpc.unary_unary_rpc_method_handler(
                     servicer.SpkSortTrainerMakeNewModel,
                     request_deserializer=radiens__dev__pb2.SpkSortTrainerNewReq.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
+            'SpkSortTrainerProfileModel': grpc.unary_unary_rpc_method_handler(
+                    servicer.SpkSortTrainerProfileModel,
+                    request_deserializer=radiens__dev__pb2.SpkSortTrainerProfileReq.FromString,
+                    response_serializer=common__pb2.StandardReply.SerializeToString,
+            ),
             'SpkSortTrainerMakeDefaultProdModels': grpc.unary_unary_rpc_method_handler(
                     servicer.SpkSortTrainerMakeDefaultProdModels,
                     request_deserializer=common__pb2.StandardRequest.FromString,
                     response_serializer=common__pb2.StandardReply.SerializeToString,
             ),
             'SpkSortTrainerListLocalNetworkModels': grpc.unary_unary_rpc_method_handler(
                     servicer.SpkSortTrainerListLocalNetworkModels,
@@ -3620,14 +3636,31 @@
         return grpc.experimental.unary_unary(request, target, '/allego.RadiensDev1/SpkSortTrainerMakeNewModel',
             radiens__dev__pb2.SpkSortTrainerNewReq.SerializeToString,
             common__pb2.StandardReply.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def SpkSortTrainerProfileModel(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/allego.RadiensDev1/SpkSortTrainerProfileModel',
+            radiens__dev__pb2.SpkSortTrainerProfileReq.SerializeToString,
+            common__pb2.StandardReply.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def SpkSortTrainerMakeDefaultProdModels(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `radiens-3.0.0b4/radiens/grpc_radiens/spikesorter_pb2.py` & `radiens-3.0.0b5/radiens/grpc_radiens/spikesorter_pb2.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/lib/allego_lib.py` & `radiens-3.0.0b5/radiens/lib/allego_lib.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/lib/channel_metadata.py` & `radiens-3.0.0b5/radiens/lib/channel_metadata.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/lib/dataset_metadata.py` & `radiens-3.0.0b5/radiens/lib/dataset_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import json
 
 import pandas as pd
-from radiens.api.api_utils.util import to_file_ext
+from radiens.api.api_utils.util import ext_to_radiens_file_type, to_file_ext
 from radiens.grpc_radiens import allegoserver_pb2, common_pb2, datasource_pb2
 from radiens.lib.channel_metadata import ChannelMetadata
 from radiens.utils.constants import TimeRange
-from radiens.utils.enums import SignalType
+from radiens.utils.enums import RadiensFileType, SignalType
 from radiens.utils.util import generic_repr, make_time_range
 
 
 class FileSetDescriptor():
     '''
     Radiens data file descriptor.
     '''
@@ -236,15 +236,15 @@
 
         self._d = {'dsource_id': raw_msg.dsourceID,
                    'kpi_dsource_id': raw_msg.status.kpiDsourceID,
                    'TR': tr,
                    'channel_metadata': ChannelMetadata(raw_msg.status.signalGroup),
                    'dataset_uid': raw_msg.status.uid,
                    'source_type': raw_msg.status.dataSourceType,
-                   'file_type': raw_msg.status.fileType,
+                   'file_type': RadiensFileType.parse(ext_to_radiens_file_type(raw_msg.status.fileType)),
                    'source_mode': raw_msg.status.mode,
                    'label': raw_msg.status.label,
                    'path': raw_msg.status.path,
                    'base_name': raw_msg.status.baseFileName}
 
     @ property
     def id(self) -> str:
@@ -292,21 +292,28 @@
     def base_name(self) -> str:
         """
         File system base name of the Radiens data file set that backs this DataSource.
         """
         return self._d['base_name']
 
     @ property
+    def file_type(self) -> RadiensFileType:
+        """
+        File type of the Radiens data file set that backs this DataSource.
+        """
+        return self._d['file_type']
+
+    @ property
     def table(self) -> pd.DataFrame:
         """
         Dataset attributes as a table.
         """
         return pd.DataFrame({'path': [self.path],
                              'name': [self.base_name],
-                             'type': [self._d['file_type']],
+                             'type': [self._d['file_type'].name],
                              'time range (sec)': ['[{:.3f}, {:.3f}]'.format(*self.time_range.sec)],
                              'duration (sec)': ['{:.3f}'.format(self.time_range.dur_sec)],
                              'channels': [self.channel_metadata.num_sigs(SignalType.AMP)],
                              'gpio': [[self.channel_metadata.num_sigs(SignalType.AIN), self.channel_metadata.num_sigs(SignalType.DIN), self.channel_metadata.num_sigs(SignalType.DOUT)]],
                              'sample freq': ['{:.0f}'.format(self.time_range.fs)],
                              'dataset UID': [self._d['dataset_uid']],
                              'label': [self._d['label']],
```

### Comparing `radiens-3.0.0b4/radiens/lib/fsys.py` & `radiens-3.0.0b5/radiens/lib/fsys.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/lib/sig_metrics.py` & `radiens-3.0.0b5/radiens/lib/sig_metrics.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/lib/signals_snapshot.py` & `radiens-3.0.0b5/radiens/lib/signals_snapshot.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/lib/spike_sorter.py` & `radiens-3.0.0b5/radiens/lib/spike_sorter.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/lib/spikes.py` & `radiens-3.0.0b5/radiens/lib/spikes.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/lib/summa.py` & `radiens-3.0.0b5/radiens/lib/summa.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/metrics_client.py` & `radiens-3.0.0b5/radiens/metrics_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/signals_client.py` & `radiens-3.0.0b5/radiens/signals_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/spike_sorter_client.py` & `radiens-3.0.0b5/radiens/spike_sorter_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/spikes_client.py` & `radiens-3.0.0b5/radiens/spikes_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/utils/config.py` & `radiens-3.0.0b5/radiens/utils/config.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/utils/constants.py` & `radiens-3.0.0b5/radiens/utils/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
 from collections import namedtuple
 
+from radiens.utils.enums import RadiensFileType
+
 ### constants ##
 ##
 ##
 
 
 MAX_GRPC_MSG_BYTES = 4 * 1024 * 1024  # 4MB
 MSG_OVERHEAD_BYTES = 10 * 1024  # 10 KB for metadata seems to work
@@ -90,7 +92,15 @@
 SignalArrays = namedtuple(
     "SignalArrays", ['amp', 'gpio_ain', 'gpio_din', 'gpio_dout'])
 KeyIdxs = namedtuple("KEY_IDXS", ['ntv', 'dset', 'sys'])
 
 SigSelect = namedtuple(
     "SigSelect", ['amp', 'gpio_ain', 'gpio_din', 'gpio_dout', 'key_idx'])
 ''' SigSelect is used for selecting signals by the given key index type, `key_idx`. The elements are numpy arrays '''
+
+CONVERTIBLE_RADIENS_FILE_TYPES = [
+    RadiensFileType.CSV,
+    RadiensFileType.XDAT,
+    RadiensFileType.KILOSORT2,
+    RadiensFileType.NWB,
+    RadiensFileType.NEX5,
+]
```

### Comparing `radiens-3.0.0b4/radiens/utils/enums.py` & `radiens-3.0.0b5/radiens/utils/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -319,14 +319,30 @@
     Q25 = common_pb2.SummaryStatsEnum.SS_STAT_Q25
     Q75 = common_pb2.SummaryStatsEnum.SS_STAT_Q75
     SKEW = common_pb2.SummaryStatsEnum.SS_STAT_SKEW
     KURTOSIS = common_pb2.SummaryStatsEnum.SS_STAT_KURTOSIS
     N = common_pb2.SummaryStatsEnum.SS_STAT_N
 
 
+class RadiensFileType(GrpcEnum):
+    """
+    An enumeration of Radiens file types
+    """
+    RHD = common_pb2.RHD
+    XDAT = common_pb2.XDAT
+    CSV = common_pb2.CSV
+    HDF5 = common_pb2.HDF5
+    NEX5 = common_pb2.NEX5
+    NWB = common_pb2.NWB
+    KILOSORT2 = common_pb2.KILOSORT2
+    NSX = common_pb2.NSX
+    TDT = common_pb2.TDT
+    SPIKES = common_pb2.SPIKES
+
+
 class TrsMode(GrpcEnum):
     """
     TrsMode is the time range selector (TRS) enum used to control time range selection in calls to get signals, spikes, power spectral density, or similar data sets.  
 
     Example:
         >>> sel_mode = TrsMode.SUBSET
```

### Comparing `radiens-3.0.0b4/radiens/utils/util.py` & `radiens-3.0.0b5/radiens/utils/util.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/videre_client.py` & `radiens-3.0.0b5/radiens/videre_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens/workspace_client.py` & `radiens-3.0.0b5/radiens/workspace_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/radiens.egg-info/PKG-INFO` & `radiens-3.0.0b5/radiens.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radiens
-Version: 3.0.0b4
+Version: 3.0.0b5
 Summary: provides python API to RADIENS analytics platform
 Home-page: http://neuronexus.github.io
 Author: NeuroNexus
 Author-email: dkipke@neuronexus.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `radiens-3.0.0b4/radiens.egg-info/SOURCES.txt` & `radiens-3.0.0b5/radiens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/setup.py` & `radiens-3.0.0b5/setup.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/tests/test_allego_client.py` & `radiens-3.0.0b5/tests/test_allego_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/tests/test_base_client.py` & `radiens-3.0.0b5/tests/test_base_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/tests/test_curate_client.py` & `radiens-3.0.0b5/tests/test_curate_client.py`

 * *Files identical despite different names*

### Comparing `radiens-3.0.0b4/tests/test_videre_client.py` & `radiens-3.0.0b5/tests/test_videre_client.py`

 * *Files identical despite different names*

