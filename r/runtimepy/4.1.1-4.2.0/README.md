# Comparing `tmp/runtimepy-4.1.1.tar.gz` & `tmp/runtimepy-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-4.1.1.tar", last modified: Tue Apr 16 03:04:51 2024, max compression
+gzip compressed data, was "runtimepy-4.2.0.tar", last modified: Mon Apr 22 04:32:19 2024, max compression
```

## Comparing `runtimepy-4.1.1.tar` & `runtimepy-4.2.0.tar`

### file list

```diff
@@ -1,292 +1,304 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.773031 runtimepy-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 03:02:39.000000 runtimepy-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-16 03:04:51.773031 runtimepy-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-16 03:02:39.000000 runtimepy-4.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-16 03:02:39.000000 runtimepy-4.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.733031 runtimepy-4.1.1/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/channel/environment/command/
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/command/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/command/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/command/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/channel/event/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/event/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/codec/system/
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/codec/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.741031 runtimepy-4.1.1/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.741031 runtimepy-4.1.1/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.741031 runtimepy-4.1.1/runtimepy/data/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/css/bootstrap_extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/dummy_load.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/factories.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.741031 runtimepy-4.1.1/runtimepy/data/js/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/audio.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.745031 runtimepy-4.1.1/runtimepy/data/js/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/App.js
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/ChannelTable.js
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/Plot.js
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/PlotManager.js
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/PlotModalManager.js
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/TabFilter.js
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/TabInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/WindowHashManager.js
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/WorkerInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/init.js
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/main.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.745031 runtimepy-4.1.1/runtimepy/data/js/tab/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/tab/env.js
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/tab/sound.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.745031 runtimepy-4.1.1/runtimepy/data/js/unused/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/unused/pyodide.js
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/util.js
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.749031 runtimepy-4.1.1/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/ChannelCommand.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/FindFile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/StructConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/TaskConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/has_factory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/has_name.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/has_request_flag.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/server_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/server_dev.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.749031 runtimepy-4.1.1/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/enum/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.749031 runtimepy-4.1.1/runtimepy/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/metrics/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/metrics/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/metrics/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.749031 runtimepy-4.1.1/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/async_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/config/
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/config/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/config/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/factory/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/factory/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/housekeeping/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/housekeeping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/imports/
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/imports/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/tcp/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.757031 runtimepy-4.1.1/runtimepy/net/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/request_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.757031 runtimepy-4.1.1/runtimepy/net/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.757031 runtimepy-4.1.1/runtimepy/net/server/app/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.757031 runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.757031 runtimepy-4.1.1/runtimepy/net/server/app/env/
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/modal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/pyodide.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/server/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/server/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/websocket/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/stream/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/stream/json/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/json/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/json/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/json/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/tcp/http/
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/udp/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/udp/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/primitives/array/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/primitives/serializable/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/serializable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/serializable/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/serializable/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/serializable/prefixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/primitives/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/int.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/basic/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/basic/periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/task/trig/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/trig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 03:04:51.773031 runtimepy-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-16 03:02:39.000000 runtimepy-4.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-16 03:02:39.000000 runtimepy-4.1.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-16 03:02:39.000000 runtimepy-4.1.1/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 03:02:39.000000 runtimepy-4.1.1/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.640229 runtimepy-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 04:29:49.000000 runtimepy-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-22 04:32:19.636229 runtimepy-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-22 04:29:49.000000 runtimepy-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-22 04:29:49.000000 runtimepy-4.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.600229 runtimepy-4.2.0/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9270 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/channel/environment/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/command/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/command/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/command/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/channel/event/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/event/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/codec/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/codec/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.608229 runtimepy-4.2.0/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.608229 runtimepy-4.2.0/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.608229 runtimepy-4.2.0/runtimepy/data/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/css/bootstrap_extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/dummy_load.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/factories.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.608229 runtimepy-4.2.0/runtimepy/data/js/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/audio.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.612229 runtimepy-4.2.0/runtimepy/data/js/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/App.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/ChannelTable.js
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/Plot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/PlotManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/PlotModalManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/TabFilter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/TabInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/WindowHashManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/WorkerInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/init.js
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/main.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.612229 runtimepy-4.2.0/runtimepy/data/js/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/tab/env.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/tab/sound.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.612229 runtimepy-4.2.0/runtimepy/data/js/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/unused/pyodide.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.616229 runtimepy-4.2.0/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/ChannelCommand.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/FindFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/PeerProcessConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/StructConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/has_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/has_request_flag.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/server_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/server_dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.616229 runtimepy-4.2.0/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/enum/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.616229 runtimepy-4.2.0/runtimepy/message/
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/message/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/message/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/message/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.616229 runtimepy-4.2.0/runtimepy/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/metrics/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/metrics/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/metrics/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.616229 runtimepy-4.2.0/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/async_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/config/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/factory/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/housekeeping/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/housekeeping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/imports/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/tcp/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/request_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/app/env/
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/app/env/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/tab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/tab/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/tab/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/tab/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/websocket/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/stream/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/stream/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/stream/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/stream/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/tcp/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/udp/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/udp/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/primitives/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/primitives/serializable/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/serializable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/serializable/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/serializable/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/serializable/prefixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/primitives/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/sample/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/sample/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/subprocess/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/subprocess/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/subprocess/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/subprocess/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/basic/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/task/trig/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/trig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 04:32:19.640229 runtimepy-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-22 04:29:49.000000 runtimepy-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-22 04:29:49.000000 runtimepy-4.2.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-22 04:29:49.000000 runtimepy-4.2.0/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-22 04:29:49.000000 runtimepy-4.2.0/tests/test_resources.py
```

### Comparing `runtimepy-4.1.1/LICENSE` & `runtimepy-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/PKG-INFO` & `runtimepy-4.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.1.1
+Version: 4.2.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,18 +13,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vcorelib>=3.2.3
+Requires-Dist: websockets
+Requires-Dist: vcorelib>=3.2.4
 Requires-Dist: svgen>=0.6.6
 Requires-Dist: psutil
-Requires-Dist: websockets
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=36872ce673f57f77e5b632b95169543d
+    hash=e23f54e60d0c62ebc1be3cae63bc7678
     =====================================
 -->
 
-# runtimepy ([4.1.1](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.2.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.1.1/README.md` & `runtimepy-4.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=36872ce673f57f77e5b632b95169543d
+    hash=e23f54e60d0c62ebc1be3cae63bc7678
     =====================================
 -->
 
-# runtimepy ([4.1.1](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.2.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.1.1/pyproject.toml` & `runtimepy-4.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "4.1.1"
+version = "4.2.0"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-4.1.1/runtimepy/app.py` & `runtimepy-4.2.0/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/channel/__init__.py` & `runtimepy-4.2.0/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/channel/environment/array.py` & `runtimepy-4.2.0/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/channel/environment/base.py` & `runtimepy-4.2.0/runtimepy/channel/environment/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,17 +62,20 @@
         if channels is None:
             channels = _ChannelRegistry()
         if enums is None:
             enums = _EnumRegistry()
 
         self.channels = channels
         self.enums = enums
-        self.fields = _BitFieldsManager(
-            channels.names, self.enums, fields=fields
-        )
+
+        # Register fields.
+        self.fields = _BitFieldsManager(channels.names, self.enums)
+        if fields:
+            for field in fields:
+                self.fields.add(field)
 
         # Keep a mapping of each channel's name and integer identifier to the
         # underlying enumeration.
         self.channel_enums: dict[_AnyChannel, _RuntimeEnum] = {
             chan: self.enums[chan.enum]
             for chan in self.channels.items.values()
             if chan.is_enum
```

### Comparing `runtimepy-4.1.1/runtimepy/channel/environment/command/__init__.py` & `runtimepy-4.2.0/runtimepy/channel/environment/command/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/channel/environment/command/parser.py` & `runtimepy-4.2.0/runtimepy/channel/environment/command/parser.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/channel/environment/command/processor.py` & `runtimepy-4.2.0/runtimepy/channel/environment/command/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,7 +179,17 @@
             assert args is not None
             result = self.handle_command(args)
 
         return result
 
 
 EnvironmentMap = dict[str, ChannelCommandProcessor]
+
+
+class RemoteCommandProcessor(ChannelCommandProcessor):
+    """A command processing interface for channel environments."""
+
+    def handle_command(self, args: Namespace) -> CommandResult:
+        """Handle a command from parsed arguments."""
+
+        args.remote = True
+        return super().handle_command(args)
```

### Comparing `runtimepy-4.1.1/runtimepy/channel/environment/command/result.py` & `runtimepy-4.2.0/runtimepy/channel/environment/command/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/channel/environment/create.py` & `runtimepy-4.2.0/runtimepy/channel/environment/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         self,
         name: str,
         kind: _Union[Primitive[_Any], _Primitivelike],
         commandable: bool = False,
         enum: _Union[_RegistryKey, _RuntimeEnum] = None,
         namespace: _Namespace = None,
         scaling: ChannelScaling = None,
+        min_period_s: float = None,
         **kwargs,
     ) -> _ChannelResult:
         """Create a new channel from the environment."""
 
         assert not self.finalized, "Environment already finalized!"
 
         # Apply the current (or provided) namespace.
@@ -62,16 +63,21 @@
             name,
             kind,
             commandable=commandable,
             enum=enum,
             scaling=scaling,
             **kwargs,
         )
+
         assert result is not None, f"Can't create channel '{name}'!"
 
+        # Set a minimum period if one was specified.
+        if min_period_s is not None:
+            result.event.set_min_period(min_period_s)
+
         # Keep track of any new enum channels.
         if enum is not None:
             self.channel_enums[result] = self.enums[enum]
 
         return self[name]
 
     def int_channel(
@@ -179,12 +185,14 @@
         assert result is not None, f"Can't create enum '{name}'!"
         return result
 
     def add_field(self, field: BitField, namespace: _Namespace = None) -> str:
         """Add a bit field to the environment."""
 
         fields = BitFields.new()
+        fields.claim_field(field)
+
         name = self.namespace(name=field.name, namespace=namespace)
-        fields.fields[name] = field
+
         self.fields.add(fields)
 
         return name
```

### Comparing `runtimepy-4.1.1/runtimepy/channel/environment/file.py` & `runtimepy-4.2.0/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/channel/environment/sample.py` & `runtimepy-4.2.0/runtimepy/channel/environment/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 
 # internal
 from runtimepy.channel.environment import ChannelEnvironment
 from runtimepy.primitives import Uint8
 from runtimepy.primitives.field import BitField, BitFlag
 
 
-def sample_env(env: ChannelEnvironment) -> None:
+def sample_env(env: ChannelEnvironment = None) -> ChannelEnvironment:
     """Register sample enumerations and channels to an environment."""
 
+    if env is None:
+        env = ChannelEnvironment()
+
     # Register an enum.
     sample_enum = env.enum(
         "SampleEnum",
         "int",
         items={
             "zero": 0,
             "one": 1,
@@ -90,14 +93,16 @@
                     )
                     env.int_channel(
                         "scaled_float",
                         commandable=True,
                         scaling=[2.0, 3.0],
                     )
 
+    return env
+
 
 def poll_sample_env(env: ChannelEnvironment) -> None:
     """Register sample enumerations and channels to an environment."""
 
     # Update local channels.
     for name in ["a", "b", "c"]:
         for i in range(10):
```

### Comparing `runtimepy-4.1.1/runtimepy/channel/event/__init__.py` & `runtimepy-4.2.0/runtimepy/channel/event/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,67 +2,99 @@
 A module implementing a channel-event protocol.
 """
 
 # built-in
 from contextlib import contextmanager
 from typing import BinaryIO, Iterator
 
+# third-party
+from vcorelib.math import to_nanos
+
 # internal
 from runtimepy.channel.event.header import PrimitiveEventHeader
+from runtimepy.metrics.channel import ChannelMetrics
 from runtimepy.primitives import AnyPrimitive
 
 
 class PrimitiveEvent:
     """A class implementing a simple channel-even interface."""
 
-    def __init__(self, primitive: AnyPrimitive, identifier: int) -> None:
+    def __init__(
+        self,
+        primitive: AnyPrimitive,
+        identifier: int,
+    ) -> None:
         """Initialize this instance."""
 
         self.primitive = primitive
         self.header = PrimitiveEventHeader.instance()
         PrimitiveEventHeader.init_header(self.header, identifier)
         self.prev_ns: int = 0
+        self.min_period_ns: int = 0
         self.streaming = False
 
+    def set_min_period(self, min_period_s: float) -> None:
+        """Set a minimum period."""
+
+        assert min_period_s > 0, min_period_s
+        self.min_period_ns = to_nanos(min_period_s)
+
     @contextmanager
-    def registered(self, stream: BinaryIO) -> Iterator[None]:
+    def registered(
+        self,
+        stream: BinaryIO,
+        flush: bool = False,
+        channel: ChannelMetrics = None,
+    ) -> Iterator[None]:
         """Register a stream as a managed context."""
 
         assert not self.streaming, "Already streaming!"
 
         def callback(_, __) -> None:
             """Emit a change event to the stream."""
-            self._poll(stream, force=True)
+            self._poll(stream, flush=flush, channel=channel)
 
         # Poll immediately.
         self.prev_ns = 0
-        self._poll(stream)
+
+        self._poll(stream, flush=flush, channel=channel)
 
         raw = self.primitive
         ident = raw.register_callback(callback)
 
         self.streaming = True
         yield
         assert raw.remove_callback(ident)
         self.streaming = False
 
-    def _poll(self, stream: BinaryIO, force: bool = False) -> int:
+    def _poll(
+        self,
+        stream: BinaryIO,
+        flush: bool = False,
+        channel: ChannelMetrics = None,
+    ) -> int:
         """
         Poll this event so that if the underlying channel has changed since the
         last write, we write another event.
         """
 
         written = 0
 
         # Check timestamp and update header if necessary.
         raw = self.primitive
         curr_ns = raw.last_updated_ns
-        if force or curr_ns >= self.prev_ns:
+
+        if curr_ns - self.prev_ns >= self.min_period_ns:
             self.prev_ns = curr_ns
             self.header["timestamp"] = curr_ns
 
             # Write header then value.
             array = self.header.array
             written += array.to_stream(stream)
             written += raw.to_stream(stream, byte_order=array.byte_order)
+            if flush:
+                stream.flush()
+
+        if channel is not None:
+            channel.increment(written)
 
         return written
```

### Comparing `runtimepy-4.1.1/runtimepy/channel/event/header.py` & `runtimepy-4.2.0/runtimepy/channel/event/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/channel/registry.py` & `runtimepy-4.2.0/runtimepy/channel/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 # internal
 from runtimepy.channel import AnyChannel as _AnyChannel
 from runtimepy.channel import Channel as _Channel
 from runtimepy.channel.event.header import PrimitiveEventHeader
 from runtimepy.codec.protocol import Protocol
 from runtimepy.mapping import DEFAULT_PATTERN
+from runtimepy.metrics.channel import ChannelMetrics
 from runtimepy.mixins.regex import CHANNEL_PATTERN as _CHANNEL_PATTERN
 from runtimepy.primitives import ChannelScaling, Primitive
 from runtimepy.primitives import Primitivelike as _Primitivelike
 from runtimepy.primitives import normalize
 from runtimepy.primitives.types.base import PythonPrimitive
 from runtimepy.registry import Registry as _Registry
 from runtimepy.registry.name import NameRegistry as _NameRegistry
@@ -128,24 +129,28 @@
 
     @contextmanager
     def registered(
         self,
         stream: BinaryIO,
         pattern: str = DEFAULT_PATTERN,
         exact: bool = False,
+        flush: bool = False,
+        channel: ChannelMetrics = None,
     ) -> Iterator[list[str]]:
         """
         Register a stream as a managed context. Returns a list of all channels
         registered.
         """
 
         with ExitStack() as stack:
             names = []
-            for name, channel in self.search(pattern, exact=exact):
-                stack.enter_context(channel.event.registered(stream))
+            for name, chan in self.search(pattern, exact=exact):
+                stack.enter_context(
+                    chan.event.registered(stream, flush=flush, channel=channel)
+                )
                 names.append(name)
 
             yield names
 
     def parse_event_stream(self, stream: BinaryIO) -> Iterator[ParsedEvent]:
         """Parse individual events from a stream."""
```

### Comparing `runtimepy-4.1.1/runtimepy/codec/protocol/__init__.py` & `runtimepy-4.2.0/runtimepy/codec/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/codec/protocol/base.py` & `runtimepy-4.2.0/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/codec/protocol/json.py` & `runtimepy-4.2.0/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/codec/system/__init__.py` & `runtimepy-4.2.0/runtimepy/codec/system/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/commands/all.py` & `runtimepy-4.2.0/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/commands/arbiter.py` & `runtimepy-4.2.0/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/commands/common.py` & `runtimepy-4.2.0/runtimepy/commands/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/commands/server.py` & `runtimepy-4.2.0/runtimepy/commands/server.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/commands/task.py` & `runtimepy-4.2.0/runtimepy/commands/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/commands/tui.py` & `runtimepy-4.2.0/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/css/bootstrap_extra.css` & `runtimepy-4.2.0/runtimepy/data/css/bootstrap_extra.css`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/dummy_load.yaml` & `runtimepy-4.2.0/runtimepy/data/dummy_load.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -12,16 +12,23 @@
   - {name: wave3, factory: sinusoid, period_s: 0.03}
 
 # Add some sample structs.
 structs:
   - name: example.struct1
     factory: sample_struct
     # Not actually used.
-    config:
+    config: &cfg
       a: 1
       b: 2
       c: 3
 
   - name: struct2
     factory: sample_struct
   - name: struct3
     factory: sample_struct
+
+# Sample peer processes.
+processes:
+  - name: proc1
+    factory: sample_peer
+    config: *cfg
+    program: runtimepy.sample.program.SampleProgram
```

### Comparing `runtimepy-4.1.1/runtimepy/data/factories.yaml` & `runtimepy-4.2.0/runtimepy/data/factories.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,18 @@
   - {name: runtimepy.net.factories.RuntimepyWebsocketData}
 
   # Useful tasks.
   - {name: runtimepy.task.trig.Sinusoid}
   - {name: runtimepy.task.sample.Sample}
 
   # Useful structs.
-  - {name: runtimepy.net.arbiter.struct.SampleStruct}
+  - {name: runtimepy.net.arbiter.info.SampleStruct}
   - {name: runtimepy.net.server.struct.UiState}
 
+  # Useful subprocess peer interfaces.
+  - {name: runtimepy.sample.peer.SamplePeer}
+
 ports:
   # Reserve ports for JSON listeners.
   - {name: udp_json, type: udp}
   - {name: tcp_json, type: tcp}
   - {name: websocket_json, type: tcp}
```

### Comparing `runtimepy-4.1.1/runtimepy/data/favicon.ico` & `runtimepy-4.2.0/runtimepy/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/JsonConnection.js` & `runtimepy-4.2.0/runtimepy/data/js/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/audio.js` & `runtimepy-4.2.0/runtimepy/data/js/audio.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/classes/App.js` & `runtimepy-4.2.0/runtimepy/data/js/classes/App.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/classes/ChannelTable.js` & `runtimepy-4.2.0/runtimepy/data/js/classes/ChannelTable.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/classes/JsonConnection.js` & `runtimepy-4.2.0/runtimepy/data/js/classes/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/classes/Plot.js` & `runtimepy-4.2.0/runtimepy/data/js/classes/Plot.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/classes/PlotManager.js` & `runtimepy-4.2.0/runtimepy/data/js/classes/PlotManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/classes/PlotModalManager.js` & `runtimepy-4.2.0/runtimepy/data/js/classes/PlotModalManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/classes/TabFilter.js` & `runtimepy-4.2.0/runtimepy/data/js/classes/TabFilter.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/classes/TabInterface.js` & `runtimepy-4.2.0/runtimepy/data/js/classes/TabInterface.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/classes/WindowHashManager.js` & `runtimepy-4.2.0/runtimepy/data/js/classes/WindowHashManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/tab/sound.js` & `runtimepy-4.2.0/runtimepy/data/js/tab/sound.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/unused/pyodide.js` & `runtimepy-4.2.0/runtimepy/data/js/unused/pyodide.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/util.js` & `runtimepy-4.2.0/runtimepy/data/js/util.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/js/worker.js` & `runtimepy-4.2.0/runtimepy/data/js/worker.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-4.2.0/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-4.2.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 ---
+includes:
+  - has_config.yaml
+
 type: object
 additionalProperties: false
 
 properties:
   clients:
     type: array
     items:
       $ref: package://runtimepy/schemas/ClientConnectionConfig.yaml
 
+  processes:
+    type: array
+    items:
+      $ref: package://runtimepy/schemas/PeerProcessConfig.yaml
+
   servers:
     type: array
     items:
       $ref: package://runtimepy/schemas/ServerConnectionConfig.yaml
 
   structs:
     type: array
@@ -40,18 +48,14 @@
   init: *applike
 
   config_builders:
     type: array
     items:
       type: string
 
-  # Application configuration data.
-  config:
-    type: object
-
   # A 'site' directory to add for discovering modules that may appear in other
   # parts of the configuration. If this isn't specified, the current directory
   # is used.
   directory:
     type: string
 
   factories:
```

### Comparing `runtimepy-4.1.1/runtimepy/data/schemas/FindFile.yaml` & `runtimepy-4.2.0/runtimepy/data/schemas/FindFile.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/data/server_base.yaml` & `runtimepy-4.2.0/runtimepy/data/server_base.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/entry.py` & `runtimepy-4.2.0/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/enum/__init__.py` & `runtimepy-4.2.0/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/enum/registry.py` & `runtimepy-4.2.0/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/enum/types.py` & `runtimepy-4.2.0/runtimepy/enum/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/mapping.py` & `runtimepy-4.2.0/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/metrics/channel.py` & `runtimepy-4.2.0/runtimepy/metrics/channel.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/metrics/connection.py` & `runtimepy-4.2.0/runtimepy/metrics/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/metrics/task.py` & `runtimepy-4.2.0/runtimepy/metrics/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/mixins/async_command.py` & `runtimepy-4.2.0/runtimepy/mixins/async_command.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/mixins/enum.py` & `runtimepy-4.2.0/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/mixins/environment.py` & `runtimepy-4.2.0/runtimepy/mixins/environment.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 A module implementing a channel-environment class mixin.
 """
 
 # internal
 from runtimepy import METRICS_NAME
 from runtimepy.channel.environment import ChannelEnvironment
 from runtimepy.metrics import ConnectionMetrics, PeriodicTaskMetrics
+from runtimepy.metrics.channel import ChannelMetrics
+
+# 10 Hz metrics.
+METRICS_MIN_PERIOD_S = 0.1
 
 
 class ChannelEnvironmentMixin:
     """A simple channel-environment mixin."""
 
     env: ChannelEnvironment
 
@@ -27,65 +31,82 @@
         """Register periodic task metrics."""
 
         with self.env.names_pushed(namespace):
             self.env.channel(
                 "dispatches",
                 metrics.dispatches,
                 description="Dispatch call counter for this task.",
+                min_period_s=METRICS_MIN_PERIOD_S,
             )
             self.env.channel(
                 "rate_hz",
                 metrics.rate_hz,
                 description="Measured dispatch rate in Hertz.",
+                min_period_s=METRICS_MIN_PERIOD_S,
             )
             self.env.channel(
                 "average_s",
                 metrics.average_s,
                 description="An averaged dispatch time measurement.",
+                min_period_s=METRICS_MIN_PERIOD_S,
             )
             self.env.channel(
                 "max_s",
                 metrics.max_s,
                 description="Maximum dispatch time measured.",
+                min_period_s=METRICS_MIN_PERIOD_S,
             )
             self.env.channel(
                 "min_s",
                 metrics.min_s,
                 description="Minimum dispatch time measured.",
+                min_period_s=METRICS_MIN_PERIOD_S,
             )
             self.env.channel(
                 "overruns",
                 metrics.overruns,
                 description="Dispatch time exceeding period counter.",
+                min_period_s=METRICS_MIN_PERIOD_S,
+            )
+
+    def register_channel_metrics(
+        self, name: str, channel: ChannelMetrics, verb: str
+    ) -> None:
+        """Register individual channel metrics."""
+
+        with self.env.names_pushed(name):
+            self.env.channel(
+                "messages",
+                channel.messages,
+                description=f"Number of messages {verb}.",
+                min_period_s=METRICS_MIN_PERIOD_S,
+            )
+            self.env.channel(
+                "messages_rate",
+                channel.message_rate,
+                description=f"Messages per second {verb}.",
+                min_period_s=METRICS_MIN_PERIOD_S,
+            )
+            self.env.channel(
+                "bytes",
+                channel.bytes,
+                description=f"Number of bytes {verb}.",
+                min_period_s=METRICS_MIN_PERIOD_S,
+            )
+            self.env.channel(
+                "kbps",
+                channel.kbps,
+                description=f"Kilobits per second {verb}.",
+                min_period_s=METRICS_MIN_PERIOD_S,
             )
 
     def register_connection_metrics(
         self, metrics: ConnectionMetrics, namespace: str = METRICS_NAME
     ) -> None:
         """Register connection metrics."""
 
         with self.env.names_pushed(namespace):
             for name, direction, verb in [
                 ("tx", metrics.tx, "transmitted"),
                 ("rx", metrics.rx, "received"),
             ]:
-                with self.env.names_pushed(name):
-                    self.env.channel(
-                        "messages",
-                        direction.messages,
-                        description=f"Number of messages {verb}.",
-                    )
-                    self.env.channel(
-                        "messages_rate",
-                        direction.message_rate,
-                        description=f"Messages per second {verb}.",
-                    )
-                    self.env.channel(
-                        "bytes",
-                        direction.bytes,
-                        description=f"Number of bytes {verb}.",
-                    )
-                    self.env.channel(
-                        "kbps",
-                        direction.kbps,
-                        description=f"Kilobits per second {verb}.",
-                    )
+                self.register_channel_metrics(name, direction, verb)
```

### Comparing `runtimepy-4.1.1/runtimepy/mixins/finalize.py` & `runtimepy-4.2.0/runtimepy/mixins/finalize.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/mixins/logging.py` & `runtimepy-4.2.0/runtimepy/mixins/logging.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/mixins/regex.py` & `runtimepy-4.2.0/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/__init__.py` & `runtimepy-4.2.0/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/apps/__init__.py` & `runtimepy-4.2.0/runtimepy/net/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/__init__.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/base.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,26 +31,28 @@
 from runtimepy.net.arbiter.housekeeping import metrics_poller
 from runtimepy.net.arbiter.info import (
     AppInfo,
     ArbiterApps,
     ConnectionMap,
     NetworkApplication,
     NetworkApplicationlike,
+    RuntimeStruct,
 )
 from runtimepy.net.arbiter.result import AppResult, ResultState
-from runtimepy.net.arbiter.struct import RuntimeStruct
 from runtimepy.net.arbiter.task import (
     ArbiterTaskManager as _ArbiterTaskManager,
 )
 from runtimepy.net.connection import Connection as _Connection
 from runtimepy.net.manager import ConnectionManager as _ConnectionManager
 from runtimepy.net.server import RuntimepyServerConnection
+from runtimepy.subprocess.peer import RuntimepyPeer as _RuntimepyPeer
 from runtimepy.tui.mixin import CursesWindow, TuiMixin
 
 ServerTask = _Awaitable[None]
+RuntimeProcessTask = tuple[type[_RuntimepyPeer], str, _JsonObject, str]
 
 
 async def init_only(app: AppInfo) -> int:
     """A network application that doesn't do anything."""
 
     await app.all_finalized()
     return 0
@@ -122,14 +124,18 @@
         self._deferred_connections: _MutableMapping[
             str, _Awaitable[_Connection]
         ] = {}
 
         # Runtime structures.
         self._structs: dict[str, RuntimeStruct] = {}
 
+        # Runtime procesess.
+        self._peers: dict[str, RuntimeProcessTask] = {}
+        self._runtime_peers: dict[str, _RuntimepyPeer] = {}
+
         self._servers: list[_asyncio.Task[None]] = []
         self._servers_started = _asyncio.Semaphore(0)
 
         self._init()
 
     def _init(self) -> None:
         """Additional initialization tasks."""
@@ -178,27 +184,22 @@
 
         # Connect environment data.
         cls.json_data["environments"] = env_json_data()
 
     def _register_envs(self) -> None:
         """Register environments."""
 
-        clear_env()
         for name, conn in self._connections.items():
             register_env(name, conn.command)
         for struct in self._structs.values():
             register_env(struct.name, struct.command)
 
     async def _init_connections(self) -> None:
         """Initialize network connections."""
 
-        # Wait for servers to start.
-        for _ in range(len(self._servers)):
-            await self._servers_started.acquire()
-
         # Start deferred connections.
         for key, value in zip(
             self._deferred_connections,
             await _asyncio.gather(*self._deferred_connections.values()),
         ):
             self._register_connection(value, key)
 
@@ -213,14 +214,106 @@
         with info.log_time("Building structs", reminder=True):
             await _asyncio.gather(
                 *(x.build(info) for x in self._structs.values())
             )
             for struct in self._structs.values():
                 struct.env.finalize(strict=False)
 
+    async def _start_processes(self, stack: _AsyncExitStack) -> None:
+        """Start processes."""
+
+        for name, (peer, name, config, import_str) in self._peers.items():
+            self._runtime_peers[name] = await stack.enter_async_context(
+                peer.running_program(name, config, import_str)
+            )
+            self.logger.info("Started process '%s'.", name)
+
+    async def _main(
+        self,
+        stack: _AsyncExitStack,
+        app: NetworkApplicationlike = None,
+        check_connections: bool = True,
+        config: _JsonObject = None,
+    ) -> tuple[int, Optional[AppInfo]]:
+        """Main application entry."""
+
+        result = -1
+        info: Optional[AppInfo] = None
+
+        clear_env()
+
+        # Wait for servers to start.
+        for _ in range(len(self._servers)):
+            await self._servers_started.acquire()
+
+        # Start processes.
+        await self._start_processes(stack)
+
+        with self.log_time("Connection initialization", reminder=True):
+            await self._init_connections()
+
+        # Register environments.
+        self._register_envs()
+        tasks = {x.name: x for x in self.task_manager.tasks}
+        for task in tasks.values():
+            register_env(task.name, task.command)
+
+        # Run application, but only if all the registered connections
+        # are still alive after initialization.
+        if not check_connections or not any(
+            x.disabled for x in self._connections.values()
+        ):
+            info = AppInfo(
+                self.logger,
+                stack,
+                self._connections,
+                self.manager,
+                self._namespace,
+                self.stop_sig,
+                config if config is not None else self._config,
+                self,
+                tasks,  # type: ignore
+                self.task_manager,
+                [],
+                self._structs,  # type: ignore
+                self._runtime_peers,
+            )
+
+            # Build structs.
+            await self._build_structs(info)
+
+            # Initialize tasks.
+            with info.log_time("Initializing periodic tasks", reminder=True):
+                await _asyncio.gather(
+                    *(x.init(info) for x in self.task_manager.tasks)
+                )
+                for task in self.task_manager.tasks:
+                    task.env.finalize(strict=False)
+
+            # Wire runtime data to server JSON.
+            self._setup_server_json(info)
+
+            # Start tasks.
+            await stack.enter_async_context(
+                self.task_manager.running(stop_sig=self.stop_sig)
+            )
+
+            # Run initialization methods.
+            result = await self._run_apps_list(self._inits, info)
+            if result == 0:
+                # Get application methods.
+                apps = self._apps
+                if app is not None:
+                    apps = normalize_app(app)
+
+                # Run applications in order.
+                result = await self._run_apps_list(apps, info)
+
+        return result, info
+
     async def _entry(
         self,
         app: NetworkApplicationlike = None,
         check_connections: bool = True,
         config: _JsonObject = None,
     ) -> int:
         """
@@ -228,75 +321,21 @@
         application, clean up connections and return the application's result.
         """
 
         result = -1
         info: Optional[AppInfo] = None
 
         try:
-            with self.log_time("Connection initialization", reminder=True):
-                await self._init_connections()
-
-            # Register environments.
-            self._register_envs()
-            tasks = {x.name: x for x in self.task_manager.tasks}
-            for task in tasks.values():
-                register_env(task.name, task.command)
-
-            # Run application, but only if all the registered connections are
-            # still alive after initialization.
-            if not check_connections or not any(
-                x.disabled for x in self._connections.values()
-            ):
-                async with _AsyncExitStack() as stack:
-                    info = AppInfo(
-                        self.logger,
-                        stack,
-                        self._connections,
-                        self.manager,
-                        self._namespace,
-                        self.stop_sig,
-                        config if config is not None else self._config,
-                        self,
-                        tasks,  # type: ignore
-                        self.task_manager,
-                        [],
-                        self._structs,  # type: ignore
-                    )
-
-                    # Build structs.
-                    await self._build_structs(info)
-
-                    # Initialize tasks.
-                    with info.log_time(
-                        "Initializing periodic tasks", reminder=True
-                    ):
-                        await _asyncio.gather(
-                            *(x.init(info) for x in self.task_manager.tasks)
-                        )
-                        for task in self.task_manager.tasks:
-                            task.env.finalize(strict=False)
-
-                    # Wire runtime data to server JSON.
-                    self._setup_server_json(info)
-
-                    # Start tasks.
-                    await stack.enter_async_context(
-                        self.task_manager.running(stop_sig=self.stop_sig)
-                    )
-
-                    # Run initialization methods.
-                    result = await self._run_apps_list(self._inits, info)
-                    if result == 0:
-                        # Get application methods.
-                        apps = self._apps
-                        if app is not None:
-                            apps = normalize_app(app)
-
-                        # Run applications in order.
-                        result = await self._run_apps_list(apps, info)
+            async with _AsyncExitStack() as stack:
+                result, info = await self._main(
+                    stack,
+                    app=app,
+                    check_connections=check_connections,
+                    config=config,
+                )
         finally:
             for conn in self._connections.values():
                 conn.disable(f"app exit {result}")
 
             # Stop runtime entities.
             self.stop_sig.set()
             await _asyncio.sleep(0)
```

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/config/__init__.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 # internal
 from runtimepy import DEFAULT_EXT, PKG_NAME
 from runtimepy.net.arbiter.config.codec import ConnectionArbiterConfig
 from runtimepy.net.arbiter.config.util import fix_args, fix_kwargs, list_adder
 from runtimepy.net.arbiter.imports import (
     ImportConnectionArbiter as _ImportConnectionArbiter,
 )
-from runtimepy.net.arbiter.imports.util import get_apps, import_str_and_item
+from runtimepy.net.arbiter.imports.util import get_apps
+from runtimepy.util import import_str_and_item
 
 ConfigObject = dict[str, _Any]
 ConfigBuilder = _Callable[[ConfigObject], None]
 
 
 def handle_config_builders(data: ConfigObject, logger: _LoggerMixin) -> None:
     """Run any configured configuration-data building methods."""
@@ -192,14 +193,22 @@
         for struct in config.structs:
             name = struct["name"]
             factory = struct["factory"]
             assert self.factory_struct(
                 struct["factory"], struct["name"], struct.get("config", {})
             ), f"Couldn't register struct '{name}' ({factory})!"
 
+        # Register processes.
+        for process in config.processes:
+            name = process["name"]
+            factory = process["factory"]
+            assert self.factory_process(
+                factory, name, process.get("config", {}), process["program"]
+            ), f"Couldn't register process '{name}' ({factory})!"
+
         # Load initialization methods.
         self._inits = get_apps(config.inits)
 
         # Set the new application entry if it's set.
         apps = get_apps(config.app, wait_for_stop=wait_for_stop)
         if apps:
             self._apps = apps
```

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/config/codec.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/config/codec.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         )
 
         self.factories: list[_Any] = data.get("factories", [])  # type: ignore
         self.clients: list[_Any] = data.get("clients", [])  # type: ignore
         self.servers: list[_Any] = data.get("servers", [])  # type: ignore
         self.tasks: list[_Any] = data.get("tasks", [])  # type: ignore
         self.structs: list[_Any] = data.get("structs", [])  # type: ignore
+        self.processes: list[_Any] = data.get("processes", [])  # type: ignore
 
         directory_str = str(data.get("directory", "."))
         self.directory = _Path(directory_str)
 
         # Add directory to Python path.
         if directory_str not in sys.path:
             sys.path.append(directory_str)
```

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/config/util.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/config/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/factory/connection.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/factory/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/factory/task.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/factory/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/housekeeping/__init__.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/housekeeping/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/imports/__init__.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/imports/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,38 +16,70 @@
 )
 from runtimepy.net.arbiter.factory import (
     FactoryConnectionArbiter as _FactoryConnectionArbiter,
 )
 from runtimepy.net.arbiter.factory.task import (
     TaskConnectionArbiter as _TaskConnectionArbiter,
 )
-from runtimepy.net.arbiter.imports.util import import_str_and_item
-from runtimepy.net.arbiter.struct import RuntimeStruct as _RuntimeStruct
+from runtimepy.net.arbiter.info import RuntimeStruct as _RuntimeStruct
 from runtimepy.net.arbiter.task import TaskFactory as _TaskFactory
+from runtimepy.subprocess.peer import RuntimepyPeer as _RuntimepyPeer
+from runtimepy.util import import_str_and_item
 
 
 class ImportConnectionArbiter(
     _FactoryConnectionArbiter, _TaskConnectionArbiter
 ):
     """
     A class implementing extensions to the connection arbiter for working with
     arbitrary Python modules.
     """
 
     def _init(self) -> None:
         """Additional initialization tasks."""
 
         super()._init()
+
         self._struct_factories: dict[str, type[_RuntimeStruct]] = {}
         self._struct_names: dict[type[_RuntimeStruct], list[str]] = {}
 
+        self._peer_factories: dict[str, type[_RuntimepyPeer]] = {}
+        self._peer_names: dict[type[_RuntimepyPeer], list[str]] = {}
+
+    def register_peer_factory(
+        self, factory: type[_RuntimepyPeer], *namespaces: str
+    ) -> bool:
+        """Attempt to register a subprocess peer factory."""
+
+        result = False
+
+        name = factory.__name__
+        snake_name = to_snake(name)
+
+        if (
+            name not in self._peer_factories
+            and snake_name not in self._peer_factories
+        ):
+            self._peer_factories[name] = factory
+            self._peer_factories[snake_name] = factory
+            self._peer_names[factory] = [*namespaces]
+
+            result = True
+            self.logger.debug(
+                "Registered '%s' (%s) subprocess peer factory.",
+                name,
+                snake_name,
+            )
+
+        return result
+
     def register_struct_factory(
         self, factory: type[_RuntimeStruct], *namespaces: str
     ) -> bool:
-        """Attempt to register a periodic task factory."""
+        """Attempt to register a struct factory."""
 
         result = False
 
         name = factory.__name__
         snake_name = to_snake(name)
 
         if (
@@ -74,31 +106,51 @@
 
         if factory in self._struct_factories and name not in self._structs:
             self._structs[name] = self._struct_factories[factory](name, config)
             result = True
 
         return result
 
+    def factory_process(
+        self, factory: str, name: str, config: _JsonObject, program: str
+    ) -> bool:
+        """Register a runtime process."""
+
+        result = False
+
+        if factory in self._peer_factories and name not in self._peers:
+            self._peers[name] = (
+                self._peer_factories[factory],
+                name,
+                config,
+                program,
+            )
+            result = True
+
+        return result
+
     def register_module_factory(
         self, module_path: str, *namespaces: str, **kwargs
     ) -> bool:
         """Attempt to register a factory class based on its module path."""
 
         module, factory_class = import_str_and_item(module_path)
 
         raw_import = getattr(_import_module(module), factory_class)
 
+        result = False
+
         # Handle factories that don't need factory-class proxying.
-        if (
-            isinstance(raw_import, type)
-            and _RuntimeStruct in raw_import.__bases__
-        ):
-            result = self.register_struct_factory(raw_import, *namespaces)
+        if isinstance(raw_import, type):
+            if _RuntimeStruct in raw_import.__bases__:
+                result = self.register_struct_factory(raw_import, *namespaces)
+            elif _RuntimepyPeer in raw_import.__bases__:
+                result = self.register_peer_factory(raw_import, *namespaces)
 
-        else:
+        if not result:
             # We need to call the factory class to create an instance.
             inst = raw_import(**kwargs)
 
             # Determine what kind of factory to register.
             result = False
             if isinstance(inst, _ConnectionFactory):
                 result = self.register_connection_factory(inst, *namespaces)
```

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/imports/util.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/imports/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,15 @@
 
 # built-in
 from importlib import import_module as _import_module
 
 # internal
 from runtimepy.net.arbiter.config.codec import ConfigApps
 from runtimepy.net.arbiter.info import ArbiterApps
-
-
-def import_str_and_item(module_path: str) -> tuple[str, str]:
-    """
-    Treat the last entry in a '.' delimited string as the item to import from
-    the module in the string preceding it.
-    """
-
-    parts = module_path.split(".")
-    assert len(parts) > 1, module_path
-
-    item = parts.pop()
-    return ".".join(parts), item
+from runtimepy.util import import_str_and_item
 
 
 def get_apps(
     module_path: ConfigApps, wait_for_stop: bool = False
 ) -> ArbiterApps:
     """
     Attempt to update the application method from the provided string.
```

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/info.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,82 @@
 """
 A module implementing an application information interface.
 """
 
 # built-in
+from abc import ABC as _ABC
 import asyncio as _asyncio
 from contextlib import AsyncExitStack as _AsyncExitStack
 from dataclasses import dataclass
 from logging import getLogger as _getLogger
 from re import compile as _compile
-from typing import Any
 from typing import Awaitable as _Awaitable
 from typing import Callable as _Callable
 from typing import Iterator as _Iterator
 from typing import MutableMapping as _MutableMapping
+from typing import TYPE_CHECKING, Any
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.logging import LoggerMixin as _LoggerMixin
 from vcorelib.logging import LoggerType as _LoggerType
 from vcorelib.namespace import Namespace as _Namespace
 
 # internal
+from runtimepy.channel.environment.sample import poll_sample_env, sample_env
 from runtimepy.mapping import DEFAULT_PATTERN
 from runtimepy.net.arbiter.result import OverallResult, results
 from runtimepy.net.connection import Connection as _Connection
 from runtimepy.net.manager import ConnectionManager
+from runtimepy.struct import RuntimeStructBase
 from runtimepy.struct import StructMap as _StructMap
 from runtimepy.task import PeriodicTask, PeriodicTaskManager
 from runtimepy.tui.mixin import TuiMixin
 
+if TYPE_CHECKING:
+    from runtimepy.subprocess.peer import (
+        RuntimepyPeer as _RuntimepyPeer,  # pragma: nocover
+    )
+
 ConnectionMap = _MutableMapping[str, _Connection]
 T = _TypeVar("T", bound=_Connection)
 V = _TypeVar("V", bound=PeriodicTask)
 Z = _TypeVar("Z")
 
 
+class RuntimeStruct(RuntimeStructBase, _ABC):
+    """A class implementing a base runtime structure."""
+
+    def init_env(self) -> None:
+        """Initialize this sample environment."""
+
+    async def build(self, app: "AppInfo") -> None:
+        """Build a struct instance's channel environment."""
+
+        del app
+        self.init_env()
+
+
+class SampleStruct(RuntimeStruct):
+    """A sample runtime structure."""
+
+    def init_env(self) -> None:
+        """Initialize this sample environment."""
+        sample_env(self.env)
+
+    def poll(self) -> None:
+        """
+        A method that other runtime entities can call to perform canonical
+        updates to this struct's environment.
+        """
+        poll_sample_env(self.env)
+
+
 @dataclass
 class AppInfo(_LoggerMixin):
     """References provided to network applications."""
 
     # A logger for applications to use.
     logger: _LoggerType
 
@@ -69,14 +105,17 @@
 
     # Keep track of application state.
     results: OverallResult
 
     # A name-to-struct mapping.
     structs: _StructMap
 
+    # A name-to-peer mapping.
+    peers: dict[str, "_RuntimepyPeer"]
+
     def with_new_logger(self, name: str) -> "AppInfo":
         """Get a copy of this AppInfo instance, but with a new logger."""
 
         return AppInfo(
             _getLogger(name),
             self.stack,
             self.connections,
@@ -85,14 +124,15 @@
             self.stop,
             self.config,
             self.tui,
             self.tasks,
             self.task_manager,
             self.results,
             self.structs,
+            self.peers,
         )
 
     def search(
         self,
         *names: str,
         pattern: str = DEFAULT_PATTERN,
         kind: type[T] = _Connection,  # type: ignore
```

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/result.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/struct/__init__.py` & `runtimepy-4.2.0/runtimepy/net/server/app/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 """
-A module implementing a runtime data structure interface.
+A module implementing application methods for this package's server interface.
 """
 
 # built-in
-from abc import ABC as _ABC
-from abc import abstractmethod as _abstractmethod
+from importlib import import_module as _import_module
 
 # internal
-from runtimepy.channel.environment.sample import poll_sample_env, sample_env
 from runtimepy.net.arbiter.info import AppInfo
-from runtimepy.struct import RuntimeStructBase
+from runtimepy.net.server import RuntimepyServerConnection
+from runtimepy.net.server.app.create import config_param, create_app
+from runtimepy.util import import_str_and_item
+
+
+async def setup(app: AppInfo) -> int:
+    """Perform server application setup steps."""
+
+    # Set default application.
+    module, method = import_str_and_item(
+        config_param(
+            app,
+            "html_method",
+            "runtimepy.net.server.app.env.channel_environments",
+        )
+    )
+    RuntimepyServerConnection.default_app = create_app(
+        app, getattr(_import_module(module), method)
+    )
 
-
-class RuntimeStruct(RuntimeStructBase, _ABC):
-    """A class implementing a base runtime structure."""
-
-    @_abstractmethod
-    async def build(self, app: AppInfo) -> None:
-        """Build a struct instance's channel environment."""
-
-
-class SampleStruct(RuntimeStruct):
-    """A sample runtime structure."""
-
-    async def build(self, app: AppInfo) -> None:
-        """Build a struct instance's channel environment."""
-
-        del app
-        sample_env(self.env)
-
-    def poll(self) -> None:
-        """
-        A method that other runtime entities can call to perform canonical
-        updates to this struct's environment.
-        """
-        poll_sample_env(self.env)
+    return 0
```

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/task.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/tcp/__init__.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/tcp/json.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/tcp/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/udp.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/arbiter/websocket.py` & `runtimepy-4.2.0/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/backoff.py` & `runtimepy-4.2.0/runtimepy/net/backoff.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/connection.py` & `runtimepy-4.2.0/runtimepy/net/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/factories/__init__.py` & `runtimepy-4.2.0/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/http/__init__.py` & `runtimepy-4.2.0/runtimepy/net/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/http/common.py` & `runtimepy-4.2.0/runtimepy/net/http/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/http/header.py` & `runtimepy-4.2.0/runtimepy/net/http/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/http/request_target.py` & `runtimepy-4.2.0/runtimepy/net/http/request_target.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/http/response.py` & `runtimepy-4.2.0/runtimepy/net/http/response.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/http/state.py` & `runtimepy-4.2.0/runtimepy/net/http/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/http/version.py` & `runtimepy-4.2.0/runtimepy/net/http/version.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/manager.py` & `runtimepy-4.2.0/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/mixin.py` & `runtimepy-4.2.0/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/__init__.py` & `runtimepy-4.2.0/runtimepy/net/server/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/base.py` & `runtimepy-4.2.0/runtimepy/net/server/app/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/__init__.py` & `runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/elements.py` & `runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/elements.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/tabs.py` & `runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/tabs.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/create.py` & `runtimepy-4.2.0/runtimepy/net/server/app/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/env/__init__.py` & `runtimepy-4.2.0/runtimepy/net/server/app/env/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,27 @@
 
     # Struct tabs.
     for struct in app.structs.values():
         ChannelEnvironmentTab(
             struct.name, struct.command, app, tabs, icon="bucket"
         ).entry()
 
+    # Subprocess tabs.
+    for name, peer in app.peers.items():
+        # Host side.
+        ChannelEnvironmentTab(
+            peer.struct.name, peer.struct.command, app, tabs, icon="cpu-fill"
+        ).entry()
+
+        # Remote side.
+        assert peer.peer is not None
+        ChannelEnvironmentTab(
+            peer.peer_name, peer.peer, app, tabs, icon="cpu"
+        ).entry()
+
     # Toggle channel-table button.
     tabs.add_button(
         "Toggle channel table",
         ".channel-column",
         icon="table",
         id="channels-button",
     )
```

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/env/modal.py` & `runtimepy-4.2.0/runtimepy/net/server/app/env/modal.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/env/tab/__init__.py` & `runtimepy-4.2.0/runtimepy/net/server/app/env/tab/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/env/tab/base.py` & `runtimepy-4.2.0/runtimepy/net/server/app/env/tab/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/env/tab/html.py` & `runtimepy-4.2.0/runtimepy/net/server/app/env/tab/html.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/env/tab/message.py` & `runtimepy-4.2.0/runtimepy/net/server/app/env/tab/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 A module implementing a channel-environment tab message-handling interface.
 """
 
 # built-in
 import logging
-from typing import Any, cast
+from typing import Any, Callable, cast
 
 # internal
 from runtimepy.channel import Channel
+from runtimepy.message import JsonMessage
 from runtimepy.net.server.app.env.tab.base import ChannelEnvironmentTabBase
-from runtimepy.net.server.app.env.tab.logger import TabMessageSender
 from runtimepy.net.server.websocket.state import TabState
-from runtimepy.net.stream.json.types import JsonMessage
+
+TabMessageSender = Callable[[JsonMessage], None]
 
 
 class ChannelEnvironmentTabMessaging(ChannelEnvironmentTabBase):
     """A channel-environment tab interface."""
 
     def _setup_callback(self, name: str, state: TabState) -> None:
         """Register a channel's value-change callback."""
```

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/env/widgets.py` & `runtimepy-4.2.0/runtimepy/net/server/app/env/widgets.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/files.py` & `runtimepy-4.2.0/runtimepy/net/server/app/files.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/placeholder.py` & `runtimepy-4.2.0/runtimepy/net/server/app/placeholder.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/sound.py` & `runtimepy-4.2.0/runtimepy/net/server/app/sound.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/app/tab.py` & `runtimepy-4.2.0/runtimepy/net/server/app/tab.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/html.py` & `runtimepy-4.2.0/runtimepy/net/server/html.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/json.py` & `runtimepy-4.2.0/runtimepy/net/server/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/server/struct/__init__.py` & `runtimepy-4.2.0/runtimepy/net/server/struct/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,38 @@
 """
 A module implementing a structure for tracking UI state and metrics.
 """
 
 # built-in
 from typing import Optional
 
-# third-party
-import psutil
-from vcorelib.math import WeightedAverage
-
 # internal
 from runtimepy.metrics.connection import ConnectionMetrics
-from runtimepy.net.arbiter.info import AppInfo
-from runtimepy.net.arbiter.struct import RuntimeStruct
+from runtimepy.mixins.psutil import PsutilMixin
+from runtimepy.net.arbiter.info import RuntimeStruct
 from runtimepy.primitives import Float
 
 UI: Optional["UiState"] = None
 
 
-class UiState(RuntimeStruct):
+class UiState(RuntimeStruct, PsutilMixin):
     """A sample runtime structure."""
 
     json_metrics: ConnectionMetrics
-    process: psutil.Process
-    cpu_average: WeightedAverage
 
     time_ms: Float
     frame_period_ms: Float
-    memory_percent: Float
-    cpu_percent: Float
 
     @staticmethod
     def singleton() -> Optional["UiState"]:
         """Attempt to get the singleton UI struct instance."""
         return UI
 
-    async def build(self, app: AppInfo) -> None:
-        """Build a struct instance's channel environment."""
-
-        del app
+    def init_env(self) -> None:
+        """Initialize this sample environment."""
 
         # Animation-frame time.
         self.time_ms = Float()
         self.env.float_channel("time_ms", self.time_ms)
         self.frame_period_ms = Float()
         self.env.float_channel("frame_period_ms", self.frame_period_ms)
 
@@ -51,32 +41,19 @@
 
         # JSON-messaging interface metrics.
         self.json_metrics = ConnectionMetrics()
         with self.env.names_pushed("json"):
             self.register_connection_metrics(self.json_metrics)
 
         # System metrics.
-        self.process = psutil.Process()
-        self.cpu_average = WeightedAverage(depth=60)
-        self.memory_percent = Float()
-        self.env.float_channel("memory_percent", self.memory_percent)
-        self.cpu_percent = Float()
-        self.env.float_channel("cpu_percent", self.cpu_percent)
+        self.init_psutil(self.env)
 
         # Update singleton.
         global UI  # pylint: disable=global-statement
         UI = self
 
     def poll(self) -> None:
         """
         A method that other runtime entities can call to perform canonical
         updates to this struct's environment.
         """
-
-        self.memory_percent.value = psutil.virtual_memory().percent
-
-        with self.process.oneshot():
-            self.cpu_average(
-                self.process.cpu_percent(),
-                weight=self.frame_period_ms.value,
-            )
-            self.cpu_percent.value = self.cpu_average.average()
+        self.poll_psutil(self.frame_period_ms.value)
```

### Comparing `runtimepy-4.1.1/runtimepy/net/server/websocket/__init__.py` & `runtimepy-4.2.0/runtimepy/net/server/websocket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 A module implementing a simple WebSocket server for the package.
 """
 
 # built-in
 from collections import defaultdict
 
 # internal
+from runtimepy.message import JsonMessage
 from runtimepy.net.arbiter.tcp.json import WebsocketJsonMessageConnection
 from runtimepy.net.server.app.env.tab import ChannelEnvironmentTab
-from runtimepy.net.server.app.env.tab.logger import TabMessageSender
+from runtimepy.net.server.app.env.tab.message import TabMessageSender
 from runtimepy.net.server.struct import UiState
 from runtimepy.net.server.websocket.state import TabState
-from runtimepy.net.stream.json.types import JsonMessage
 from runtimepy.net.websocket import WebsocketConnection
 
 
 class RuntimepyWebsocketConnection(WebsocketJsonMessageConnection):
     """A class implementing a package-specific WebSocket connection."""
 
     send_interfaces: dict[str, TabMessageSender]
```

### Comparing `runtimepy-4.1.1/runtimepy/net/server/websocket/state.py` & `runtimepy-4.2.0/runtimepy/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 """
-A module implementing a stateful data interface for per-connection tabs.
+A module implementing package utilities.
 """
 
 # built-in
-from collections import defaultdict
-from dataclasses import dataclass
 import logging
+from typing import NamedTuple
 
 # third-party
 from vcorelib.logging import DEFAULT_TIME_FORMAT
 
-# internal
-from runtimepy.net.server.app.env.tab.logger import ListLogger
-from runtimepy.net.stream.json.types import JsonMessage
-from runtimepy.primitives import AnyPrimitive
 
-# (value, nanosecond timestamp)
-Point = tuple[str | int | float | bool, int]
+class StrToBool(NamedTuple):
+    """A container for results when converting strings to boolean."""
 
+    result: bool
+    valid: bool
 
-@dataclass
-class TabState:
-    """Stateful information relevant to individual tabs."""
-
-    shown: bool
-    shown_ever: bool
-    tab_logger: ListLogger
-
-    points: dict[str, list[Point]]
-    primitives: dict[str, AnyPrimitive]
-    callbacks: dict[str, int]
-
-    _loggers: list[logging.Logger]
+    @staticmethod
+    def parse(data: str) -> "StrToBool":
+        """Parse a string to boolean."""
 
-    def frame(self, time: float) -> JsonMessage:
-        """Handle a new UI frame."""
+        data = data.lower()
+        is_true = data == "true"
+        resolved = is_true or data == "false"
+        return StrToBool(is_true, resolved)
 
-        # Not used yet.
-        del time
 
-        result: JsonMessage = {}
+class ListLogger(logging.Handler):
+    """An interface facilitating sending log messages to browser tabs."""
 
-        # Handle log messages.
-        if self.tab_logger.log_messages:
-            result["log_messages"] = self.tab_logger.log_messages
-            self.tab_logger.log_messages = []
+    log_messages: list[logging.LogRecord]
 
-        # Handle channel updates.
-        if self.points:
-            result["points"] = self.points
-            self.points = defaultdict(list)
+    def drain(self) -> list[logging.LogRecord]:
+        """Drain messages."""
 
+        result = self.log_messages
+        self.log_messages = []
         return result
 
-    def clear_loggers(self) -> None:
-        """Clear all logging handlers."""
+    def drain_str(self) -> list[str]:
+        """Drain formatted messages."""
+
+        return [self.format(x) for x in self.drain()]
 
-        for logger in self._loggers:
-            logger.removeHandler(self.tab_logger)
-        self._loggers = []
+    def __bool__(self) -> bool:
+        """Evaluate this instance as boolean."""
+        return bool(self.log_messages)
 
-    def add_logger(self, logger: logging.Logger) -> None:
-        """Add a logger."""
+    def emit(self, record: logging.LogRecord) -> None:
+        """Send the log message."""
 
-        logger.addHandler(self.tab_logger)
-        self._loggers.append(logger)
+        self.log_messages.append(record)
 
     @staticmethod
-    def create() -> "TabState":
-        """Create a new instance."""
+    def create() -> "ListLogger":
+        """Create an instance of this handler."""
 
         logger = ListLogger()
         logger.log_messages = []
         logger.setFormatter(logging.Formatter(DEFAULT_TIME_FORMAT))
 
-        return TabState(False, False, logger, defaultdict(list), {}, {}, [])
+        return logger
+
+
+def import_str_and_item(module_path: str) -> tuple[str, str]:
+    """
+    Treat the last entry in a '.' delimited string as the item to import from
+    the module in the string preceding it.
+    """
+
+    parts = module_path.split(".")
+    assert len(parts) > 1, module_path
+
+    item = parts.pop()
+    return ".".join(parts), item
```

### Comparing `runtimepy-4.1.1/runtimepy/net/stream/__init__.py` & `runtimepy-4.2.0/runtimepy/net/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/stream/base.py` & `runtimepy-4.2.0/runtimepy/message/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,67 @@
 """
-A module implementing a base, stream-oriented connection interface.
+A module implementing a message-stream processing interface.
 """
 
 # built-in
 from io import BytesIO as _BytesIO
-from typing import BinaryIO as _BinaryIO
+from json import dumps, loads
+from typing import Any
+from typing import Iterator as _Iterator
 
 # third-party
 from vcorelib.io import ByteFifo
 
 # internal
-from runtimepy.net.connection import BinaryMessage
-from runtimepy.net.connection import Connection as _Connection
 from runtimepy.primitives import Uint32, UnsignedInt
+from runtimepy.primitives.byte_order import DEFAULT_BYTE_ORDER, ByteOrder
 
+JsonMessage = dict[str, Any]
 
-class PrefixedMessageConnection(_Connection):
-    """
-    A connection for handling inter-frame message size prefixes for some
-    stream-oriented protocols.
-    """
+
+class MessageProcessor:
+    """A class for parsing size-delimited messages."""
 
     message_length_kind: type[UnsignedInt] = Uint32
-    reading_header: bool
 
-    def init(self) -> None:
+    def __init__(self, byte_order: ByteOrder = DEFAULT_BYTE_ORDER) -> None:
         """Initialize this instance."""
 
+        self.byte_order = byte_order
+
         # Header parsing.
         self.buffer = ByteFifo()
         self.reading_header = True
         self.message_length_in = self.message_length_kind()
         self.prefix_size = self.message_length_in.size
 
         self.message_length_out = self.message_length_kind()
 
-    def _send_message(
-        self, data: BinaryMessage, addr: tuple[str, int] = None
-    ) -> None:
-        """Underlying data send."""
-
-        del addr
-        self.send_binary(data)
-
-    def send_message(
-        self, data: BinaryMessage, addr: tuple[str, int] = None
-    ) -> None:
-        """Handle inter-message prefixes for outgoing messages."""
+    def encode(self, stream: _BytesIO, data: bytes | str) -> None:
+        """Encode a message to a stream."""
+
+        if isinstance(data, str):
+            data = data.encode()
 
         self.message_length_out.value = len(data)
+        self.message_length_out.to_stream(stream, byte_order=self.byte_order)
+        stream.write(data)
 
-        with _BytesIO() as stream:
-            self.message_length_out.to_stream(
-                stream, byte_order=self.byte_order
-            )
-            stream.write(data)
-            self._send_message(stream.getvalue(), addr=addr)
-
-    def send_message_str(
-        self, data: str, addr: tuple[str, int] = None
-    ) -> None:
-        """Convert a message to bytes before sending."""
-        self.send_message(data.encode(), addr=addr)
-
-    async def process_single(
-        self, stream: _BinaryIO, addr: tuple[str, int] = None
-    ) -> bool:
-        """Process a single message."""
-        del stream
-        del addr
-        return True
-
-    async def process_binary(
-        self, data: bytes, addr: tuple[str, int] = None
-    ) -> bool:
-        """Process an incoming message."""
+    def encode_json(self, stream: _BytesIO, data: JsonMessage) -> None:
+        """Encode a message as JSON."""
+        self.encode(stream, dumps(data, separators=(",", ":")))
 
-        result = True
+    def messages(self, data: bytes) -> _Iterator[JsonMessage]:
+        """Iterate over incoming messages."""
+
+        for message in self.process(data):
+            yield loads(message.decode())
+
+    def process(self, data: bytes) -> _Iterator[bytes]:
+        """Process an incoming message."""
 
         self.buffer.ingest(data)
 
         can_continue = True
         while can_continue:
             # Read the message size.
             if self.reading_header:
@@ -94,15 +75,11 @@
                 else:
                     can_continue = False
 
             # Read the message payload.
             else:
                 message = self.buffer.pop(self.message_length_in.value)
                 if message is not None:
-                    # process message
-                    with _BytesIO(message) as stream:
-                        result &= await self.process_single(stream, addr=addr)
+                    yield message
                     self.reading_header = True
                 else:
                     can_continue = False
-
-        return result
```

### Comparing `runtimepy-4.1.1/runtimepy/net/stream/json/base.py` & `runtimepy-4.2.0/runtimepy/message/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,89 +1,98 @@
 """
-A module implementing a base JSON messaging connection interface.
+A module implementing a JSON messaging interface.
 """
 
 # built-in
-from argparse import Namespace
 import asyncio
 from copy import copy
-from json import JSONDecodeError, dumps, loads
+from io import BytesIO
 import logging
 from typing import Any, Optional, Union
 
 # third-party
 from vcorelib.dict.codec import JsonCodec
+from vcorelib.logging import LoggerType
 from vcorelib.target.resolver import TargetResolver
 
 # internal
 from runtimepy import PKG_NAME, VERSION
-from runtimepy.channel.environment.command import ENVIRONMENTS, FieldOrChannel
+from runtimepy.channel.environment import ChannelEnvironment
+from runtimepy.channel.environment.command import ENVIRONMENTS
+from runtimepy.channel.environment.command.processor import (
+    ChannelCommandProcessor,
+)
 from runtimepy.channel.environment.command.result import CommandResult
-from runtimepy.mixins.async_command import AsyncCommandProcessingMixin
-from runtimepy.net.stream.json.handlers import (
+from runtimepy.message import JsonMessage, MessageProcessor
+from runtimepy.message.handlers import (
     ChannelCommand,
     FindFile,
     channel_env_handler,
     event_wait,
     find_file_request_handler,
     loopback_handler,
 )
-from runtimepy.net.stream.json.types import (
+from runtimepy.message.types import (
     DEFAULT_LOOPBACK,
     DEFAULT_TIMEOUT,
     RESERVED_KEYS,
-    JsonMessage,
     MessageHandler,
     T,
     TypedHandler,
 )
-from runtimepy.net.stream.string import StringMessageConnection
+from runtimepy.util import ListLogger
 
 
-class JsonMessageConnection(
-    StringMessageConnection, AsyncCommandProcessingMixin
-):
-    """A connection interface for JSON messaging."""
+class Identifier:
+    """A simple message indentifier interface."""
 
-    _log_messages: list[dict[str, Any]]
-    remote_meta: Optional[JsonMessage]
+    def __init__(self) -> None:
+        """Initialize this instance."""
+        self.curr_id: int = 1
 
-    def _register_handlers(self) -> None:
-        """Register connection-specific command handlers."""
+    def __call__(self) -> int:
+        """Get the next identifier."""
+        curr = self.curr_id
+        self.curr_id += 2
+        return curr
 
-        # Extra handlers.
-        self.typed_handler("find_file", FindFile, find_file_request_handler)
-        self.typed_handler(
-            "channel_command",
-            ChannelCommand,
-            channel_env_handler(ENVIRONMENTS.data, self.command),
-        )
 
-    def init(self) -> None:
-        """Initialize this instance."""
+class JsonMessageInterface:
+    """A JSON messaging interface class."""
+
+    logger: LoggerType
+    processor: MessageProcessor
+    command: ChannelCommandProcessor
 
-        super().init()
-        self._setup_async_commands()
+    list_handler: ListLogger
+
+    remote_environments: dict[str, ChannelEnvironment]
+
+    def __init__(self) -> None:
+        """Initialize this instance"""
 
         self.targets = TargetResolver()
+        self.remote_meta: Optional[JsonMessage] = None
+        self._log_messages: list[dict[str, Any]] = []
+
+        self.list_handler = ListLogger.create()
+
+        self.remote_environments = {}
 
         self.meta = {
             "package": PKG_NAME,
             "version": VERSION,
             "kind": type(self).__name__,
         }
 
-        self.curr_id: int = 1
+        self.curr_id = Identifier()
 
         self.ids_waiting: dict[int, asyncio.Event] = {}
         self.id_responses: dict[int, JsonMessage] = {}
 
-        self._log_messages: list[dict[str, Any]] = []
-        self.remote_meta = None
-
         # Standard handlers.
         self.basic_handler("loopback")
         self.basic_handler("meta", self._meta_handler)
 
         self._register_handlers()
 
         self.meta["handlers"] = list(self.targets.literals) + [  # type: ignore
@@ -94,116 +103,153 @@
             "metadata: package=%s, version=%s, kind=%s, handlers=%s",
             self.meta["package"],
             self.meta["version"],
             self.meta["kind"],
             self.meta["handlers"],
         )
 
+    def _register_handlers(self) -> None:
+        """Register connection-specific command handlers."""
+
+        # Extra handlers.
+        self.typed_handler("find_file", FindFile, find_file_request_handler)
+        self.typed_handler(
+            "channel_command",
+            ChannelCommand,
+            channel_env_handler(ENVIRONMENTS.data, self.command),
+        )
+
+    def typed_handler(
+        self, key: str, kind: type[T], handler: TypedHandler[T]
+    ) -> None:
+        """Register a typed handler."""
+
+        assert self.targets.register(key, (key, handler, kind))
+
     def basic_handler(
         self, key: str, handler: MessageHandler = loopback_handler
     ) -> None:
         """Register a basic handler."""
 
         assert self.targets.register(key, (key, handler, None))
 
-    def typed_handler(
-        self, key: str, kind: type[T], handler: TypedHandler[T]
+    async def _meta_handler(
+        self, outbox: JsonMessage, inbox: JsonMessage
     ) -> None:
-        """Register a typed handler."""
+        """Handle the peer's metadata."""
 
-        assert self.targets.register(key, (key, handler, kind))
+        if self.remote_meta is None:
+            self.remote_meta = inbox
+            outbox.update(self.meta)
+
+            # Log peer's metadata.
+            self.logger.info(
+                (
+                    "remote metadata: package=%s, "
+                    "version=%s, kind=%s, handlers=%s"
+                ),
+                self.remote_meta["package"],
+                self.remote_meta["version"],
+                self.remote_meta["kind"],
+                self.remote_meta["handlers"],
+            )
+
+    def stage_remote_log(
+        self, msg: str, *args, level: int = logging.INFO
+    ) -> None:
+        """Log a message on the remote."""
+
+        data = {"msg": msg, "level": level}
+        if args:
+            data["args"] = [*args]
+        self._log_messages.append(data)
+
+    def write(self, data: bytes, addr: tuple[str, int] = None) -> None:
+        """Write data."""
 
     def send_json(
         self, data: Union[JsonMessage, JsonCodec], addr: tuple[str, int] = None
     ) -> None:
         """Send a JSON message."""
 
         if isinstance(data, JsonCodec):
             data = data.asdict()
 
+        # Stage any pending log messages.
+        if self.list_handler:
+            for record in self.list_handler.drain():
+                self.stage_remote_log(  # type: ignore
+                    record.msg, *record.args, level=record.levelno
+                )
+
         # Add any pending log messages to this message.
         if self._log_messages:
             assert "__log_messages__" not in data
             data["__log_messages__"] = self._log_messages  # type: ignore
             self._log_messages = []
 
-        self.send_message_str(dumps(data, separators=(",", ":")), addr=addr)
-
-    def stage_remote_log(
-        self, msg: str, *args, level: int = logging.INFO
-    ) -> None:
-        """Log a message on the remote."""
+        with BytesIO() as stream:
+            self.processor.encode_json(stream, data)
+            self.write(stream.getvalue(), addr=addr)
 
-        data = {"msg": msg, "level": level}
-        if args:
-            data["args"] = [*args]
-        self._log_messages.append(data)
+    def _handle_reserved(
+        self, data: JsonMessage, response: JsonMessage
+    ) -> bool:
+        """Handle special keys in an incoming message."""
 
-    async def handle_command(
-        self, args: Namespace, channel: Optional[FieldOrChannel]
-    ) -> None:
-        """Handle a remote command asynchronously."""
+        should_respond = True
 
-        if args.remote and self.connected:
-            cli_args = [args.command]
-            if args.force:
-                cli_args.append("-f")
-            cli_args.append(args.channel)
+        # If a message identifier is present, send one in the response.
+        if "__id__" in data:
+            ident = data["__id__"]
+            if ident in self.ids_waiting:
+                del data["__id__"]
+                self.id_responses[ident] = data
+                event = self.ids_waiting[ident]
+                del self.ids_waiting[ident]
+                event.set()
 
-            self.logger.info(
-                "Remote command: %s",
-                await self.channel_command(
-                    " ".join(cli_args + args.extra), environment=args.env
-                ),
-            )
+                # Don't respond if we're receiving a reply.
+                should_respond = False
 
-    async def channel_command(
-        self,
-        command: str,
-        environment: str = "default",
-        addr: tuple[str, int] = None,
-    ) -> CommandResult:
-        """Send a channel command to an endpoint."""
+            response["__id__"] = ident
 
-        result = await self.wait_json(
-            {
-                "channel_command": {
-                    "environment": environment,
-                    "command": command,
-                    "is_request": True,
-                }
-            },
-            addr=addr,
-        )
+        # Log messages sent by the peer.
+        if "__log_messages__" in data:
+            for message in data["__log_messages__"]:
+                if "msg" in message and message["msg"]:
+                    self.logger.log(
+                        message.get("level", logging.INFO),
+                        "remote: " + message["msg"],
+                        *message.get("args", []),
+                    )
+            del data["__log_messages__"]
 
-        return CommandResult(
-            result["channel_command"]["success"],
-            result["channel_command"].get("reason"),
-        )
+        return should_respond
 
     async def wait_json(
         self,
-        data: Union[JsonMessage, JsonCodec],
+        data: Union[JsonMessage, JsonCodec] = None,
         addr: tuple[str, int] = None,
         timeout: float = DEFAULT_TIMEOUT,
     ) -> JsonMessage:
         """Send a JSON message and wait for a response."""
 
+        if data is None:
+            data = {}
         if isinstance(data, JsonCodec):
             data = data.asdict()
 
         data = copy(data)
         assert "__id__" not in data, data
-        data["__id__"] = self.curr_id
+        ident = self.curr_id()
+        data["__id__"] = ident
 
         got_response = asyncio.Event()
 
-        ident = self.curr_id
-        self.curr_id += 1
-
         assert ident not in self.ids_waiting
         self.ids_waiting[ident] = got_response
 
         # Send message and await response.
         self.send_json(data, addr=addr)
 
         assert await event_wait(
@@ -235,83 +281,37 @@
             "Loopback result: '%s' (%s).",
             response,
             "success" if status else "fail",
         )
 
         return status
 
-    async def async_init(self) -> bool:
-        """A runtime initialization routine (executes during 'process')."""
-
-        # Check loopback if it makes sense to.
-        result = await super().async_init()
-
-        # Only not-connected UDP connections can't do this.
-        if self.connected:
-            result = await self.loopback()
-
-            if result:
-                await self.wait_json({"meta": self.meta})
-
-        return result
-
-    async def _meta_handler(
-        self, outbox: JsonMessage, inbox: JsonMessage
-    ) -> None:
-        """Handle the peer's metadata."""
-
-        if self.remote_meta is None:
-            self.remote_meta = inbox
-            outbox.update(self.meta)
-
-            # Log peer's metadata.
-            self.logger.info(
-                (
-                    "remote metadata: package=%s, "
-                    "version=%s, kind=%s, handlers=%s"
-                ),
-                self.remote_meta["package"],
-                self.remote_meta["version"],
-                self.remote_meta["kind"],
-                self.remote_meta["handlers"],
-            )
-
-    def _handle_reserved(
-        self, data: JsonMessage, response: JsonMessage
-    ) -> bool:
-        """Handle special keys in an incoming message."""
-
-        should_respond = True
-
-        # If a message identifier is present, send one in the response.
-        if "__id__" in data:
-            ident = data["__id__"]
-            if ident in self.ids_waiting:
-                del data["__id__"]
-                self.id_responses[ident] = data
-                event = self.ids_waiting[ident]
-                del self.ids_waiting[ident]
-                event.set()
-
-                # Don't respond if we're receiving a reply.
-                should_respond = False
-
-            response["__id__"] = ident
+    async def channel_command(
+        self,
+        command: str,
+        environment: str = "default",
+        addr: tuple[str, int] = None,
+    ) -> CommandResult:
+        """Send a channel command to an endpoint."""
 
-        # Log messages sent by the peer.
-        if "__log_messages__" in data:
-            for message in data["__log_messages__"]:
-                if "msg" in message and message["msg"]:
-                    self.logger.log(
-                        message.get("level", logging.INFO),
-                        "remote: " + message["msg"],
-                        *message.get("args", []),
-                    )
+        result = await self.wait_json(
+            {
+                "channel_command": {
+                    "environment": environment,
+                    "command": command,
+                    "is_request": True,
+                }
+            },
+            addr=addr,
+        )
 
-        return should_respond
+        return CommandResult(
+            result["channel_command"]["success"],
+            result["channel_command"].get("reason"),
+        )
 
     async def process_json(
         self, data: JsonMessage, addr: tuple[str, int] = None
     ) -> bool:
         """Process a JSON message."""
 
         response: JsonMessage = {}
@@ -367,26 +367,7 @@
                 "Ignored incoming message keys: %s.", ", ".join(keys_ignored)
             )
 
         if self._handle_reserved(data, response) and response:
             self.send_json(response, addr=addr)
 
         return True
-
-    async def process_message(
-        self, data: str, addr: tuple[str, int] = None
-    ) -> bool:
-        """Process a string message."""
-
-        result = True
-
-        try:
-            decoded = loads(data)
-
-            if decoded and isinstance(decoded, dict):
-                result = await self.process_json(decoded, addr=addr)
-            else:
-                self.logger.error("Ignoring message '%s'.", data)
-        except JSONDecodeError as exc:
-            self.logger.exception("Couldn't decode '%s': %s", data, exc)
-
-        return result
```

### Comparing `runtimepy-4.1.1/runtimepy/net/stream/json/handlers.py` & `runtimepy-4.2.0/runtimepy/message/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from vcorelib.io import ARBITER
 from vcorelib.paths import find_file
 
 # internal
 from runtimepy.channel.environment.command.processor import (
     ChannelCommandProcessor,
 )
-from runtimepy.net.stream.json.types import JsonMessage, TypedHandler
+from runtimepy.message import JsonMessage
+from runtimepy.message.types import TypedHandler
 from runtimepy.schemas import RuntimepyDictCodec
 
 
 class ChannelCommand(RuntimepyDictCodec, BasicDictCodec):
     """A schema-validated find-file request."""
 
     data: JsonMessage
```

### Comparing `runtimepy-4.1.1/runtimepy/net/stream/json/types.py` & `runtimepy-4.2.0/runtimepy/message/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 A module containing useful type definitions for JSON messaging.
 """
 
 # built-in
-from typing import Any, Awaitable, Callable, TypeVar
+from typing import Awaitable, Callable, TypeVar
 
 # third-party
 from vcorelib.dict.codec import JsonCodec
 
-JsonMessage = dict[str, Any]
+# internal
+from runtimepy.message import JsonMessage
 
 #
 # async def message_handler(response: JsonMessage, data: JsonMessage) -> None:
 #     """A sample message handler."""
 #
 MessageHandler = Callable[[JsonMessage, JsonMessage], Awaitable[None]]
 MessageHandlers = dict[str, MessageHandler]
```

### Comparing `runtimepy-4.1.1/runtimepy/net/stream/string.py` & `runtimepy-4.2.0/runtimepy/net/stream/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/tcp/connection.py` & `runtimepy-4.2.0/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/tcp/create.py` & `runtimepy-4.2.0/runtimepy/net/tcp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/tcp/http/__init__.py` & `runtimepy-4.2.0/runtimepy/net/tcp/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/tcp/protocol.py` & `runtimepy-4.2.0/runtimepy/net/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-4.2.0/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-4.2.0/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/udp/connection.py` & `runtimepy-4.2.0/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/udp/create.py` & `runtimepy-4.2.0/runtimepy/net/udp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/udp/protocol.py` & `runtimepy-4.2.0/runtimepy/net/udp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/util.py` & `runtimepy-4.2.0/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/net/websocket/connection.py` & `runtimepy-4.2.0/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/__init__.py` & `runtimepy-4.2.0/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/array/__init__.py` & `runtimepy-4.2.0/runtimepy/primitives/array/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/base.py` & `runtimepy-4.2.0/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/bool.py` & `runtimepy-4.2.0/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/byte_order.py` & `runtimepy-4.2.0/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/field/__init__.py` & `runtimepy-4.2.0/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/field/fields.py` & `runtimepy-4.2.0/runtimepy/primitives/field/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,36 +176,45 @@
 
         # Ensure the padded field is still set to the correct value.
         _BitFieldBase(self.raw, result, width)(val=val)
 
         self.by_index[result] = (width, val)
         return result
 
+    def claim_field(self, field: _BitField) -> _BitField:
+        """Claim a bit field."""
+
+        assert field.name not in self.fields, field.name
+        self.fields[field.name] = field
+        self.by_index[field.index] = field
+        return field
+
     def field(
         self,
         name: str,
         width: int,
         index: int = None,
         enum: _RegistryKey = None,
         description: str = None,
     ) -> _BitField:
         """Create a new bit field."""
 
         assert width != 1, "Use bit-flags for single-width fields!"
 
-        index = self._claim_bits(width, index=index)
-
-        result = _BitField(
-            name, self.raw, index, width, enum=enum, description=description
+        return self.claim_field(
+            _BitField(
+                name,
+                self.raw,
+                self._claim_bits(width, index=index),
+                width,
+                enum=enum,
+                description=description,
+            )
         )
 
-        self.fields[name] = result
-        self.by_index[index] = result
-        return result
-
     @classmethod
     def new(cls: type[T], value: _Primitivelike = "uint8") -> T:
         """Create a new bit-field storage entity."""
 
         return cls.create(
             {"type": _cast(str, value), "fields": [], "finalized": False}
         )
```

### Comparing `runtimepy-4.1.1/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-4.2.0/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/field/manager/base.py` & `runtimepy-4.2.0/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/float.py` & `runtimepy-4.2.0/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/int.py` & `runtimepy-4.2.0/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/scaling.py` & `runtimepy-4.2.0/runtimepy/primitives/scaling.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/serializable/base.py` & `runtimepy-4.2.0/runtimepy/primitives/serializable/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/serializable/fixed.py` & `runtimepy-4.2.0/runtimepy/primitives/serializable/fixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/serializable/prefixed.py` & `runtimepy-4.2.0/runtimepy/primitives/serializable/prefixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/string.py` & `runtimepy-4.2.0/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/types/__init__.py` & `runtimepy-4.2.0/runtimepy/primitives/types/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/types/base.py` & `runtimepy-4.2.0/runtimepy/primitives/types/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/types/bool.py` & `runtimepy-4.2.0/runtimepy/primitives/types/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/types/bounds.py` & `runtimepy-4.2.0/runtimepy/primitives/types/bounds.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/types/float.py` & `runtimepy-4.2.0/runtimepy/primitives/types/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/primitives/types/int.py` & `runtimepy-4.2.0/runtimepy/primitives/types/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/registry/__init__.py` & `runtimepy-4.2.0/runtimepy/registry/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 A generic registry interface for keeping track of objects by either string or
 integer identifier.
 """
 
 # built-in
 from abc import abstractmethod as _abstractmethod
+from contextlib import suppress
 from typing import Generic as _Generic
 from typing import Iterator
 from typing import Optional as _Optional
 from typing import TypeVar as _TypeVar
 from typing import cast as _cast
 
 # third-party
@@ -50,15 +51,16 @@
 
     def search(
         self, pattern: str, exact: bool = False
     ) -> Iterator[tuple[str, T]]:
         """Search for items in the registry by name."""
 
         for name in self.names.search(pattern, exact=exact):
-            yield name, self.items[name]
+            with suppress(KeyError):
+                yield name, self.items[name]
 
     def asdict(self) -> _JsonObject:
         """Get this registry as a dictionary."""
 
         return {
             name: _cast(_JsonValue, item.asdict())
             for name, item in self.items.items()
```

### Comparing `runtimepy-4.1.1/runtimepy/registry/bool.py` & `runtimepy-4.2.0/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/registry/item.py` & `runtimepy-4.2.0/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/registry/name.py` & `runtimepy-4.2.0/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/schemas.py` & `runtimepy-4.2.0/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/struct/__init__.py` & `runtimepy-4.2.0/runtimepy/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/task/asynchronous.py` & `runtimepy-4.2.0/runtimepy/task/asynchronous.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/task/basic/manager.py` & `runtimepy-4.2.0/runtimepy/task/basic/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/task/basic/periodic.py` & `runtimepy-4.2.0/runtimepy/task/basic/periodic.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/task/sample.py` & `runtimepy-4.2.0/runtimepy/task/sample.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/task/trig/__init__.py` & `runtimepy-4.2.0/runtimepy/task/trig/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/tui/channels/__init__.py` & `runtimepy-4.2.0/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/tui/cursor.py` & `runtimepy-4.2.0/runtimepy/tui/cursor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/tui/mixin.py` & `runtimepy-4.2.0/runtimepy/tui/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/tui/mock.py` & `runtimepy-4.2.0/runtimepy/tui/mock.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy/tui/task.py` & `runtimepy-4.2.0/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/runtimepy.egg-info/PKG-INFO` & `runtimepy-4.2.0/runtimepy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.1.1
+Version: 4.2.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,18 +13,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vcorelib>=3.2.3
+Requires-Dist: websockets
+Requires-Dist: vcorelib>=3.2.4
 Requires-Dist: svgen>=0.6.6
 Requires-Dist: psutil
-Requires-Dist: websockets
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=36872ce673f57f77e5b632b95169543d
+    hash=e23f54e60d0c62ebc1be3cae63bc7678
     =====================================
 -->
 
-# runtimepy ([4.1.1](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.2.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.1.1/runtimepy.egg-info/SOURCES.txt` & `runtimepy-4.2.0/runtimepy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -77,34 +77,41 @@
 runtimepy/data/schemas/Channel.yaml
 runtimepy/data/schemas/ChannelCommand.yaml
 runtimepy/data/schemas/ChannelRegistry.yaml
 runtimepy/data/schemas/ClientConnectionConfig.yaml
 runtimepy/data/schemas/ConnectionArbiterConfig.yaml
 runtimepy/data/schemas/EnumRegistry.yaml
 runtimepy/data/schemas/FindFile.yaml
+runtimepy/data/schemas/PeerProcessConfig.yaml
 runtimepy/data/schemas/RuntimeEnum.yaml
 runtimepy/data/schemas/ServerConnectionConfig.yaml
 runtimepy/data/schemas/StructConfig.yaml
 runtimepy/data/schemas/TaskConfig.yaml
+runtimepy/data/schemas/has_config.yaml
 runtimepy/data/schemas/has_factory.yaml
 runtimepy/data/schemas/has_name.yaml
 runtimepy/data/schemas/has_request_flag.yaml
 runtimepy/enum/__init__.py
 runtimepy/enum/registry.py
 runtimepy/enum/types.py
+runtimepy/message/__init__.py
+runtimepy/message/handlers.py
+runtimepy/message/interface.py
+runtimepy/message/types.py
 runtimepy/metrics/__init__.py
 runtimepy/metrics/channel.py
 runtimepy/metrics/connection.py
 runtimepy/metrics/task.py
 runtimepy/mixins/__init__.py
 runtimepy/mixins/async_command.py
 runtimepy/mixins/enum.py
 runtimepy/mixins/environment.py
 runtimepy/mixins/finalize.py
 runtimepy/mixins/logging.py
+runtimepy/mixins/psutil.py
 runtimepy/mixins/regex.py
 runtimepy/net/__init__.py
 runtimepy/net/backoff.py
 runtimepy/net/connection.py
 runtimepy/net/manager.py
 runtimepy/net/mixin.py
 runtimepy/net/util.py
@@ -121,15 +128,14 @@
 runtimepy/net/arbiter/config/util.py
 runtimepy/net/arbiter/factory/__init__.py
 runtimepy/net/arbiter/factory/connection.py
 runtimepy/net/arbiter/factory/task.py
 runtimepy/net/arbiter/housekeeping/__init__.py
 runtimepy/net/arbiter/imports/__init__.py
 runtimepy/net/arbiter/imports/util.py
-runtimepy/net/arbiter/struct/__init__.py
 runtimepy/net/arbiter/tcp/__init__.py
 runtimepy/net/arbiter/tcp/json.py
 runtimepy/net/factories/__init__.py
 runtimepy/net/http/__init__.py
 runtimepy/net/http/common.py
 runtimepy/net/http/header.py
 runtimepy/net/http/request_target.py
@@ -153,26 +159,22 @@
 runtimepy/net/server/app/bootstrap/tabs.py
 runtimepy/net/server/app/env/__init__.py
 runtimepy/net/server/app/env/modal.py
 runtimepy/net/server/app/env/widgets.py
 runtimepy/net/server/app/env/tab/__init__.py
 runtimepy/net/server/app/env/tab/base.py
 runtimepy/net/server/app/env/tab/html.py
-runtimepy/net/server/app/env/tab/logger.py
 runtimepy/net/server/app/env/tab/message.py
 runtimepy/net/server/struct/__init__.py
 runtimepy/net/server/websocket/__init__.py
 runtimepy/net/server/websocket/state.py
 runtimepy/net/stream/__init__.py
 runtimepy/net/stream/base.py
 runtimepy/net/stream/string.py
 runtimepy/net/stream/json/__init__.py
-runtimepy/net/stream/json/base.py
-runtimepy/net/stream/json/handlers.py
-runtimepy/net/stream/json/types.py
 runtimepy/net/tcp/__init__.py
 runtimepy/net/tcp/connection.py
 runtimepy/net/tcp/create.py
 runtimepy/net/tcp/protocol.py
 runtimepy/net/tcp/http/__init__.py
 runtimepy/net/tcp/telnet/__init__.py
 runtimepy/net/tcp/telnet/codes.py
@@ -205,15 +207,23 @@
 runtimepy/primitives/types/bounds.py
 runtimepy/primitives/types/float.py
 runtimepy/primitives/types/int.py
 runtimepy/registry/__init__.py
 runtimepy/registry/bool.py
 runtimepy/registry/item.py
 runtimepy/registry/name.py
+runtimepy/sample/__init__.py
+runtimepy/sample/peer.py
+runtimepy/sample/program.py
 runtimepy/struct/__init__.py
+runtimepy/subprocess/__init__.py
+runtimepy/subprocess/interface.py
+runtimepy/subprocess/peer.py
+runtimepy/subprocess/program.py
+runtimepy/subprocess/protocol.py
 runtimepy/task/__init__.py
 runtimepy/task/asynchronous.py
 runtimepy/task/sample.py
 runtimepy/task/basic/__init__.py
 runtimepy/task/basic/manager.py
 runtimepy/task/basic/periodic.py
 runtimepy/task/trig/__init__.py
```

### Comparing `runtimepy-4.1.1/setup.py` & `runtimepy-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/tests/test_entry.py` & `runtimepy-4.2.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.1/tests/test_mapping.py` & `runtimepy-4.2.0/tests/test_mapping.py`

 * *Files identical despite different names*

