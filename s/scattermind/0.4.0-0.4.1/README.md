# Comparing `tmp/scattermind-0.4.0.tar.gz` & `tmp/scattermind-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scattermind-0.4.0.tar", last modified: Thu Mar 28 00:08:23 2024, max compression
+gzip compressed data, was "scattermind-0.4.1.tar", last modified: Mon Apr 22 03:14:44 2024, max compression
```

## Comparing `scattermind-0.4.0.tar` & `scattermind-0.4.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.056267 scattermind-0.4.0/
--rw-r--r--   0 krause     (501) staff       (20)    11357 2024-02-29 05:22:24.000000 scattermind-0.4.0/LICENSE
--rw-r--r--   0 krause     (501) staff       (20)       33 2023-10-04 16:20:45.000000 scattermind-0.4.0/MANIFEST.in
--rw-r--r--   0 krause     (501) staff       (20)    15032 2024-03-28 00:08:23.056016 scattermind-0.4.0/PKG-INFO
--rw-r--r--   0 krause     (501) staff       (20)      700 2024-02-29 05:22:24.000000 scattermind-0.4.0/README.md
--rw-r--r--   0 krause     (501) staff       (20)     4239 2024-03-28 00:03:01.000000 scattermind-0.4.0/pyproject.toml
--rw-r--r--   0 krause     (501) staff       (20)      177 2024-03-28 00:03:01.000000 scattermind-0.4.0/requirements.dev.txt
--rw-r--r--   0 krause     (501) staff       (20)       90 2024-03-28 00:03:01.000000 scattermind-0.4.0/requirements.txt
--rw-r--r--   0 krause     (501) staff       (20)       38 2024-03-28 00:08:23.056307 scattermind-0.4.0/setup.cfg
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.038734 scattermind-0.4.0/src/
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.041019 scattermind-0.4.0/src/scattermind/
--rw-r--r--   0 krause     (501) staff       (20)     2042 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     1913 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/__main__.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.042018 scattermind-0.4.0/src/scattermind/api/
--rw-r--r--   0 krause     (501) staff       (20)      728 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/api/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     9410 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/api/api.py
--rw-r--r--   0 krause     (501) staff       (20)     1616 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/api/loader.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.042711 scattermind-0.4.0/src/scattermind/app/
--rw-r--r--   0 krause     (501) staff       (20)      644 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/app/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     4931 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/app/args.py
--rw-r--r--   0 krause     (501) staff       (20)     5460 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/app/healthcheck.py
--rw-r--r--   0 krause     (501) staff       (20)     2684 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/app/worker.py
--rw-r--r--   0 krause     (501) staff       (20)        0 2023-10-04 16:20:02.000000 scattermind-0.4.0/src/scattermind/py.typed
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.044419 scattermind-0.4.0/src/scattermind/system/
--rw-r--r--   0 krause     (501) staff       (20)      639 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)    16845 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/base.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.045146 scattermind-0.4.0/src/scattermind/system/cache/
--rw-r--r--   0 krause     (501) staff       (20)      611 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/cache/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     2850 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/cache/cache.py
--rw-r--r--   0 krause     (501) staff       (20)     2036 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/cache/loader.py
--rw-r--r--   0 krause     (501) staff       (20)     1332 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/cache/nocache.py
--rw-r--r--   0 krause     (501) staff       (20)     2016 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/cache/redis.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.046018 scattermind-0.4.0/src/scattermind/system/client/
--rw-r--r--   0 krause     (501) staff       (20)      715 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/client/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)    22095 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/client/client.py
--rw-r--r--   0 krause     (501) staff       (20)     2191 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/client/loader.py
--rw-r--r--   0 krause     (501) staff       (20)     9721 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/client/local.py
--rw-r--r--   0 krause     (501) staff       (20)    13544 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/client/redis.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.046474 scattermind-0.4.0/src/scattermind/system/config/
--rw-r--r--   0 krause     (501) staff       (20)      618 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/config/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)    15891 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/config/config.py
--rw-r--r--   0 krause     (501) staff       (20)     9048 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/config/loader.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.047433 scattermind-0.4.0/src/scattermind/system/executor/
--rw-r--r--   0 krause     (501) staff       (20)      639 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/executor/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)    18736 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/executor/executor.py
--rw-r--r--   0 krause     (501) staff       (20)     4739 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/executor/loader.py
--rw-r--r--   0 krause     (501) staff       (20)    13001 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/executor/redis.py
--rw-r--r--   0 krause     (501) staff       (20)     3210 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/executor/single.py
--rw-r--r--   0 krause     (501) staff       (20)    10904 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/executor/thread.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.048356 scattermind-0.4.0/src/scattermind/system/graph/
--rw-r--r--   0 krause     (501) staff       (20)      634 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/graph/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     8489 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/graph/args.py
--rw-r--r--   0 krause     (501) staff       (20)    11650 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/graph.py
--rw-r--r--   0 krause     (501) staff       (20)    10288 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/graphdef.py
--rw-r--r--   0 krause     (501) staff       (20)     1928 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/graph/loader.py
--rw-r--r--   0 krause     (501) staff       (20)    12636 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/node.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.049688 scattermind-0.4.0/src/scattermind/system/graph/nodes/
--rw-r--r--   0 krause     (501) staff       (20)      632 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/graph/nodes/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     1941 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/nodes/assertion_error.py
--rw-r--r--   0 krause     (501) staff       (20)     4165 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/nodes/bin_op.py
--rw-r--r--   0 krause     (501) staff       (20)     2977 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/nodes/call.py
--rw-r--r--   0 krause     (501) staff       (20)     3825 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/nodes/constant_op.py
--rw-r--r--   0 krause     (501) staff       (20)     3133 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/nodes/for_loop.py
--rw-r--r--   0 krause     (501) staff       (20)     2496 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/nodes/if_op.py
--rw-r--r--   0 krause     (501) staff       (20)     2867 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/nodes/load_constant.py
--rw-r--r--   0 krause     (501) staff       (20)     2494 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/nodes/mat_square.py
--rw-r--r--   0 krause     (501) staff       (20)     2941 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/nodes/str_concat.py
--rw-r--r--   0 krause     (501) staff       (20)     3672 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/graph/nodes/test_cache.py
--rw-r--r--   0 krause     (501) staff       (20)     2770 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/helper.py
--rw-r--r--   0 krause     (501) staff       (20)     8169 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/info.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.050431 scattermind-0.4.0/src/scattermind/system/logger/
--rw-r--r--   0 krause     (501) staff       (20)      793 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/logger/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     7247 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/logger/context.py
--rw-r--r--   0 krause     (501) staff       (20)     4576 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/logger/error.py
--rw-r--r--   0 krause     (501) staff       (20)     3489 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/logger/event.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.050732 scattermind-0.4.0/src/scattermind/system/logger/listeners/
--rw-r--r--   0 krause     (501) staff       (20)      637 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/logger/listeners/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     1895 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/logger/listeners/stdout.py
--rw-r--r--   0 krause     (501) staff       (20)     2448 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/logger/loader.py
--rw-r--r--   0 krause     (501) staff       (20)    10857 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/logger/log.py
--rw-r--r--   0 krause     (501) staff       (20)    10023 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/names.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.051468 scattermind-0.4.0/src/scattermind/system/payload/
--rw-r--r--   0 krause     (501) staff       (20)     1365 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/payload/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     5068 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/payload/data.py
--rw-r--r--   0 krause     (501) staff       (20)     2390 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/payload/loader.py
--rw-r--r--   0 krause     (501) staff       (20)     2899 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/payload/local.py
--rw-r--r--   0 krause     (501) staff       (20)     2781 2024-03-07 05:09:12.000000 scattermind-0.4.0/src/scattermind/system/payload/redis.py
--rw-r--r--   0 krause     (501) staff       (20)    33335 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/payload/values.py
--rw-r--r--   0 krause     (501) staff       (20)     2334 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/plugins.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.052141 scattermind-0.4.0/src/scattermind/system/queue/
--rw-r--r--   0 krause     (501) staff       (20)     1082 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/queue/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     2595 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/queue/loader.py
--rw-r--r--   0 krause     (501) staff       (20)     7879 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/queue/local.py
--rw-r--r--   0 krause     (501) staff       (20)    51388 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/queue/queue.py
--rw-r--r--   0 krause     (501) staff       (20)    11436 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/queue/redis.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.052564 scattermind-0.4.0/src/scattermind/system/queue/strategy/
--rw-r--r--   0 krause     (501) staff       (20)      691 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/queue/strategy/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     3352 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/queue/strategy/loader.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.052924 scattermind-0.4.0/src/scattermind/system/queue/strategy/node/
--rw-r--r--   0 krause     (501) staff       (20)      637 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/queue/strategy/node/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     3404 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/queue/strategy/node/dedicated.py
--rw-r--r--   0 krause     (501) staff       (20)     3148 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/queue/strategy/node/simple.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.053151 scattermind-0.4.0/src/scattermind/system/queue/strategy/queue/
--rw-r--r--   0 krause     (501) staff       (20)      638 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/queue/strategy/queue/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     1189 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/queue/strategy/queue/simple.py
--rw-r--r--   0 krause     (501) staff       (20)     7135 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/queue/strategy/strategy.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.053695 scattermind-0.4.0/src/scattermind/system/readonly/
--rw-r--r--   0 krause     (501) staff       (20)     1052 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/readonly/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     6837 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/readonly/access.py
--rw-r--r--   0 krause     (501) staff       (20)     1948 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/readonly/loader.py
--rw-r--r--   0 krause     (501) staff       (20)     2476 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/readonly/ram.py
--rw-r--r--   0 krause     (501) staff       (20)     5399 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/readonly/writer.py
--rw-r--r--   0 krause     (501) staff       (20)    12657 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/redis_util.py
--rw-r--r--   0 krause     (501) staff       (20)     3960 2024-02-29 05:22:24.000000 scattermind-0.4.0/src/scattermind/system/response.py
--rw-r--r--   0 krause     (501) staff       (20)    18252 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/torch_util.py
--rw-r--r--   0 krause     (501) staff       (20)    10506 2024-03-28 00:03:01.000000 scattermind-0.4.0/src/scattermind/system/util.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.055300 scattermind-0.4.0/src/scattermind.egg-info/
--rw-r--r--   0 krause     (501) staff       (20)    15032 2024-03-28 00:08:23.000000 scattermind-0.4.0/src/scattermind.egg-info/PKG-INFO
--rw-r--r--   0 krause     (501) staff       (20)     4040 2024-03-28 00:08:23.000000 scattermind-0.4.0/src/scattermind.egg-info/SOURCES.txt
--rw-r--r--   0 krause     (501) staff       (20)        1 2024-03-28 00:08:23.000000 scattermind-0.4.0/src/scattermind.egg-info/dependency_links.txt
--rw-r--r--   0 krause     (501) staff       (20)      275 2024-03-28 00:08:23.000000 scattermind-0.4.0/src/scattermind.egg-info/requires.txt
--rw-r--r--   0 krause     (501) staff       (20)       12 2024-03-28 00:08:23.000000 scattermind-0.4.0/src/scattermind.egg-info/top_level.txt
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-28 00:08:23.055110 scattermind-0.4.0/test/
--rw-r--r--   0 krause     (501) staff       (20)    10212 2024-03-28 00:03:01.000000 scattermind-0.4.0/test/test_assert.py
--rw-r--r--   0 krause     (501) staff       (20)    15325 2024-03-28 00:03:01.000000 scattermind-0.4.0/test/test_cache.py
--rw-r--r--   0 krause     (501) staff       (20)     8551 2024-03-28 00:03:01.000000 scattermind-0.4.0/test/test_call.py
--rw-r--r--   0 krause     (501) staff       (20)     7407 2024-03-28 00:03:01.000000 scattermind-0.4.0/test/test_cop.py
--rw-r--r--   0 krause     (501) staff       (20)     1970 2024-02-29 05:22:24.000000 scattermind-0.4.0/test/test_dtype.py
--rw-r--r--   0 krause     (501) staff       (20)    12496 2024-03-28 00:03:01.000000 scattermind-0.4.0/test/test_invalid.py
--rw-r--r--   0 krause     (501) staff       (20)     6021 2024-03-28 00:03:01.000000 scattermind-0.4.0/test/test_lowmem.py
--rw-r--r--   0 krause     (501) staff       (20)     5067 2024-03-28 00:03:01.000000 scattermind-0.4.0/test/test_ns.py
--rw-r--r--   0 krause     (501) staff       (20)     5512 2024-02-29 05:22:24.000000 scattermind-0.4.0/test/test_plugins.py
--rw-r--r--   0 krause     (501) staff       (20)     8324 2024-02-29 05:22:24.000000 scattermind-0.4.0/test/test_util.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.471307 scattermind-0.4.1/
+-rw-r--r--   0 krause     (501) staff       (20)    11357 2024-02-29 05:22:24.000000 scattermind-0.4.1/LICENSE
+-rw-r--r--   0 krause     (501) staff       (20)       33 2023-10-04 16:20:45.000000 scattermind-0.4.1/MANIFEST.in
+-rw-r--r--   0 krause     (501) staff       (20)    15032 2024-04-22 03:14:44.470728 scattermind-0.4.1/PKG-INFO
+-rw-r--r--   0 krause     (501) staff       (20)      700 2024-02-29 05:22:24.000000 scattermind-0.4.1/README.md
+-rw-r--r--   0 krause     (501) staff       (20)     4239 2024-04-22 03:14:31.000000 scattermind-0.4.1/pyproject.toml
+-rw-r--r--   0 krause     (501) staff       (20)      177 2024-03-28 00:03:01.000000 scattermind-0.4.1/requirements.dev.txt
+-rw-r--r--   0 krause     (501) staff       (20)       90 2024-04-22 03:14:31.000000 scattermind-0.4.1/requirements.txt
+-rw-r--r--   0 krause     (501) staff       (20)       38 2024-04-22 03:14:44.471343 scattermind-0.4.1/setup.cfg
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.439982 scattermind-0.4.1/src/
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.442618 scattermind-0.4.1/src/scattermind/
+-rw-r--r--   0 krause     (501) staff       (20)     2042 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     1913 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/__main__.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.444100 scattermind-0.4.1/src/scattermind/api/
+-rw-r--r--   0 krause     (501) staff       (20)      728 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/api/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     8376 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/api/api.py
+-rw-r--r--   0 krause     (501) staff       (20)     1616 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/api/loader.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.444985 scattermind-0.4.1/src/scattermind/app/
+-rw-r--r--   0 krause     (501) staff       (20)      644 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/app/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     4931 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/app/args.py
+-rw-r--r--   0 krause     (501) staff       (20)     5459 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/app/healthcheck.py
+-rw-r--r--   0 krause     (501) staff       (20)     2702 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/app/worker.py
+-rw-r--r--   0 krause     (501) staff       (20)        0 2023-10-04 16:20:02.000000 scattermind-0.4.1/src/scattermind/py.typed
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.447764 scattermind-0.4.1/src/scattermind/system/
+-rw-r--r--   0 krause     (501) staff       (20)      639 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)    16845 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/base.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.448887 scattermind-0.4.1/src/scattermind/system/cache/
+-rw-r--r--   0 krause     (501) staff       (20)      611 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/cache/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     4400 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/cache/cache.py
+-rw-r--r--   0 krause     (501) staff       (20)     2090 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/cache/loader.py
+-rw-r--r--   0 krause     (501) staff       (20)     1799 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/cache/nocache.py
+-rw-r--r--   0 krause     (501) staff       (20)     3900 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/cache/redis.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.450312 scattermind-0.4.1/src/scattermind/system/client/
+-rw-r--r--   0 krause     (501) staff       (20)      715 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/client/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)    24674 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/client/client.py
+-rw-r--r--   0 krause     (501) staff       (20)     2191 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/client/loader.py
+-rw-r--r--   0 krause     (501) staff       (20)    11330 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/client/local.py
+-rw-r--r--   0 krause     (501) staff       (20)    14951 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/client/redis.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.451162 scattermind-0.4.1/src/scattermind/system/config/
+-rw-r--r--   0 krause     (501) staff       (20)      618 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/config/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)    18746 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/config/config.py
+-rw-r--r--   0 krause     (501) staff       (20)     9079 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/config/loader.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.452850 scattermind-0.4.1/src/scattermind/system/executor/
+-rw-r--r--   0 krause     (501) staff       (20)      639 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/executor/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)    21500 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/executor/executor.py
+-rw-r--r--   0 krause     (501) staff       (20)     4739 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/executor/loader.py
+-rw-r--r--   0 krause     (501) staff       (20)    13828 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/executor/redis.py
+-rw-r--r--   0 krause     (501) staff       (20)     3602 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/executor/single.py
+-rw-r--r--   0 krause     (501) staff       (20)    12808 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/executor/thread.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.454349 scattermind-0.4.1/src/scattermind/system/graph/
+-rw-r--r--   0 krause     (501) staff       (20)      634 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/graph/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     9129 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/graph/args.py
+-rw-r--r--   0 krause     (501) staff       (20)    11650 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/graph.py
+-rw-r--r--   0 krause     (501) staff       (20)    10288 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/graphdef.py
+-rw-r--r--   0 krause     (501) staff       (20)     1928 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/graph/loader.py
+-rw-r--r--   0 krause     (501) staff       (20)    12636 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/node.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.456879 scattermind-0.4.1/src/scattermind/system/graph/nodes/
+-rw-r--r--   0 krause     (501) staff       (20)      632 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/graph/nodes/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     1941 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/nodes/assertion_error.py
+-rw-r--r--   0 krause     (501) staff       (20)     4165 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/nodes/bin_op.py
+-rw-r--r--   0 krause     (501) staff       (20)     2977 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/nodes/call.py
+-rw-r--r--   0 krause     (501) staff       (20)     3825 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/nodes/constant_op.py
+-rw-r--r--   0 krause     (501) staff       (20)     3133 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/nodes/for_loop.py
+-rw-r--r--   0 krause     (501) staff       (20)     2496 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/nodes/if_op.py
+-rw-r--r--   0 krause     (501) staff       (20)     2867 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/nodes/load_constant.py
+-rw-r--r--   0 krause     (501) staff       (20)     2494 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/nodes/mat_square.py
+-rw-r--r--   0 krause     (501) staff       (20)     2941 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/nodes/str_concat.py
+-rw-r--r--   0 krause     (501) staff       (20)     3672 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/graph/nodes/test_cache.py
+-rw-r--r--   0 krause     (501) staff       (20)     2770 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/helper.py
+-rw-r--r--   0 krause     (501) staff       (20)     8169 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/info.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.458128 scattermind-0.4.1/src/scattermind/system/logger/
+-rw-r--r--   0 krause     (501) staff       (20)      793 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/logger/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     7247 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/logger/context.py
+-rw-r--r--   0 krause     (501) staff       (20)     4576 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/logger/error.py
+-rw-r--r--   0 krause     (501) staff       (20)     3489 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/logger/event.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.458568 scattermind-0.4.1/src/scattermind/system/logger/listeners/
+-rw-r--r--   0 krause     (501) staff       (20)      637 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/logger/listeners/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     1895 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/logger/listeners/stdout.py
+-rw-r--r--   0 krause     (501) staff       (20)     2448 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/logger/loader.py
+-rw-r--r--   0 krause     (501) staff       (20)    10857 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/logger/log.py
+-rw-r--r--   0 krause     (501) staff       (20)    10023 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/names.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.459751 scattermind-0.4.1/src/scattermind/system/payload/
+-rw-r--r--   0 krause     (501) staff       (20)     1365 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/payload/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     5068 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/payload/data.py
+-rw-r--r--   0 krause     (501) staff       (20)     2390 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/payload/loader.py
+-rw-r--r--   0 krause     (501) staff       (20)     2899 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/payload/local.py
+-rw-r--r--   0 krause     (501) staff       (20)     2781 2024-03-07 05:09:12.000000 scattermind-0.4.1/src/scattermind/system/payload/redis.py
+-rw-r--r--   0 krause     (501) staff       (20)    33543 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/payload/values.py
+-rw-r--r--   0 krause     (501) staff       (20)     2334 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/plugins.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.463640 scattermind-0.4.1/src/scattermind/system/queue/
+-rw-r--r--   0 krause     (501) staff       (20)     1082 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/queue/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     2595 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/queue/loader.py
+-rw-r--r--   0 krause     (501) staff       (20)     7879 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/queue/local.py
+-rw-r--r--   0 krause     (501) staff       (20)    53013 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/queue/queue.py
+-rw-r--r--   0 krause     (501) staff       (20)    11436 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/queue/redis.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.464733 scattermind-0.4.1/src/scattermind/system/queue/strategy/
+-rw-r--r--   0 krause     (501) staff       (20)      691 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/queue/strategy/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     3352 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/queue/strategy/loader.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.465467 scattermind-0.4.1/src/scattermind/system/queue/strategy/node/
+-rw-r--r--   0 krause     (501) staff       (20)      637 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/queue/strategy/node/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     3404 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/queue/strategy/node/dedicated.py
+-rw-r--r--   0 krause     (501) staff       (20)     3148 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/queue/strategy/node/simple.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.465744 scattermind-0.4.1/src/scattermind/system/queue/strategy/queue/
+-rw-r--r--   0 krause     (501) staff       (20)      638 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/queue/strategy/queue/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     1189 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/queue/strategy/queue/simple.py
+-rw-r--r--   0 krause     (501) staff       (20)     7135 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/queue/strategy/strategy.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.466550 scattermind-0.4.1/src/scattermind/system/readonly/
+-rw-r--r--   0 krause     (501) staff       (20)     1052 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/readonly/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     6837 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/readonly/access.py
+-rw-r--r--   0 krause     (501) staff       (20)     1948 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/readonly/loader.py
+-rw-r--r--   0 krause     (501) staff       (20)     2476 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/readonly/ram.py
+-rw-r--r--   0 krause     (501) staff       (20)     5399 2024-02-29 05:22:24.000000 scattermind-0.4.1/src/scattermind/system/readonly/writer.py
+-rw-r--r--   0 krause     (501) staff       (20)    12657 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/redis_util.py
+-rw-r--r--   0 krause     (501) staff       (20)     4278 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/response.py
+-rw-r--r--   0 krause     (501) staff       (20)    18252 2024-03-28 00:03:01.000000 scattermind-0.4.1/src/scattermind/system/torch_util.py
+-rw-r--r--   0 krause     (501) staff       (20)    10897 2024-04-22 03:14:31.000000 scattermind-0.4.1/src/scattermind/system/util.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.470018 scattermind-0.4.1/src/scattermind.egg-info/
+-rw-r--r--   0 krause     (501) staff       (20)    15032 2024-04-22 03:14:44.000000 scattermind-0.4.1/src/scattermind.egg-info/PKG-INFO
+-rw-r--r--   0 krause     (501) staff       (20)     4040 2024-04-22 03:14:44.000000 scattermind-0.4.1/src/scattermind.egg-info/SOURCES.txt
+-rw-r--r--   0 krause     (501) staff       (20)        1 2024-04-22 03:14:44.000000 scattermind-0.4.1/src/scattermind.egg-info/dependency_links.txt
+-rw-r--r--   0 krause     (501) staff       (20)      275 2024-04-22 03:14:44.000000 scattermind-0.4.1/src/scattermind.egg-info/requires.txt
+-rw-r--r--   0 krause     (501) staff       (20)       12 2024-04-22 03:14:44.000000 scattermind-0.4.1/src/scattermind.egg-info/top_level.txt
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 03:14:44.469592 scattermind-0.4.1/test/
+-rw-r--r--   0 krause     (501) staff       (20)    10264 2024-04-22 03:14:31.000000 scattermind-0.4.1/test/test_assert.py
+-rw-r--r--   0 krause     (501) staff       (20)    15489 2024-04-22 03:14:31.000000 scattermind-0.4.1/test/test_cache.py
+-rw-r--r--   0 krause     (501) staff       (20)     8594 2024-04-22 03:14:31.000000 scattermind-0.4.1/test/test_call.py
+-rw-r--r--   0 krause     (501) staff       (20)     7433 2024-04-22 03:14:31.000000 scattermind-0.4.1/test/test_cop.py
+-rw-r--r--   0 krause     (501) staff       (20)     1970 2024-02-29 05:22:24.000000 scattermind-0.4.1/test/test_dtype.py
+-rw-r--r--   0 krause     (501) staff       (20)    12496 2024-03-28 00:03:01.000000 scattermind-0.4.1/test/test_invalid.py
+-rw-r--r--   0 krause     (501) staff       (20)     6027 2024-04-22 03:14:31.000000 scattermind-0.4.1/test/test_lowmem.py
+-rw-r--r--   0 krause     (501) staff       (20)     5067 2024-04-22 03:14:31.000000 scattermind-0.4.1/test/test_ns.py
+-rw-r--r--   0 krause     (501) staff       (20)     5512 2024-02-29 05:22:24.000000 scattermind-0.4.1/test/test_plugins.py
+-rw-r--r--   0 krause     (501) staff       (20)     8324 2024-02-29 05:22:24.000000 scattermind-0.4.1/test/test_util.py
```

### Comparing `scattermind-0.4.0/LICENSE` & `scattermind-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/PKG-INFO` & `scattermind-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scattermind
-Version: 0.4.0
+Version: 0.4.1
 Summary: A decentralized and distributed horizontally scalable model execution framework.
 Author-email: Josua Krause <josua.krause@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,15 +214,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mypy>=1.5.1
 Requires-Dist: numpy>=1.25.2
 Requires-Dist: quick-server>=0.9.0
-Requires-Dist: redipy>=0.6.0
+Requires-Dist: redipy>=0.7.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: torch>=2.0.0
 Provides-Extra: test
 Requires-Dist: flake8-commas>=2.1.0; extra == "test"
 Requires-Dist: flake8-isort>=6.1.1; extra == "test"
 Requires-Dist: flake8>=5.0.4; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
```

### Comparing `scattermind-0.4.0/README.md` & `scattermind-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/pyproject.toml` & `scattermind-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
     name = "scattermind"
     description = "A decentralized and distributed horizontally scalable model execution framework."
     readme = "README.md"
-    version = "0.4.0"
+    version = "0.4.1"
     authors = [
         {name = "Josua Krause", email = "josua.krause@gmail.com"},
     ]
     keywords = [
         "distributed",
         "model inference",
         "machine learning",
```

### Comparing `scattermind-0.4.0/src/scattermind/__init__.py` & `scattermind-0.4.1/src/scattermind/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/__main__.py` & `scattermind-0.4.1/src/scattermind/__main__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/api/__init__.py` & `scattermind-0.4.1/src/scattermind/api/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/api/api.py` & `scattermind-0.4.1/src/scattermind/api/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,32 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Provides functionality to send tasks and retrieve results."""
-import time
 from collections.abc import Iterable
 from typing import Any, TypedDict
 
 import numpy as np
 import torch
 
 from scattermind.system.base import QueueId, TaskId
 from scattermind.system.graph.graphdef import FullGraphDefJSON
 from scattermind.system.names import GNamespace, QualifiedNodeName
 from scattermind.system.payload.values import TaskValueContainer
-from scattermind.system.response import (
-    ResponseObject,
-    TASK_STATUS_DONE,
-    TASK_STATUS_ERROR,
-    TASK_STATUS_READY,
-    TaskStatus,
-)
+from scattermind.system.response import ResponseObject, TaskStatus
 from scattermind.system.torch_util import (
     create_tensor,
     DTypeName,
     str_to_tensor,
 )
 
 
@@ -85,15 +78,16 @@
             GNamespace | None: The namespace or None if the task does not
                 exist.
         """
         raise NotImplementedError()
 
     def get_status(self, task_id: TaskId) -> TaskStatus:
         """
-        Get the status of the given task.
+        Get the status of the given task. Note, calling this method is
+        required before being able to access results.
 
         Args:
             task_id (TaskId): The task id.
 
         Returns:
             TaskStatus: The status of the task.
         """
@@ -170,65 +164,33 @@
                 for key, value in obj.items()
             }))
 
     def wait_for(
             self,
             task_ids: list[TaskId],
             *,
-            timeinc: float = 1.0,
             timeout: float | None = 10.0,
             ) -> Iterable[tuple[TaskId, ResponseObject]]:
         """
         Wait for a collection of tasks to complete.
 
         Args:
             task_ids (list[TaskId]): The tasks to wait for.
-            timeinc (float, optional): The increment of internal waiting
-                between checks. Defaults to 1.0.
             timeout (float | None, optional): The maximum time to wait for any
-                task to complete. If None, no timeout is enforced. Defaults to
+                task to complete. The timeout is reset after each successfully
+                returned task. If None, no timeout is enforced. Defaults to
                 10.0.
 
         Yields:
             tuple[TaskId, ResponseObject]: Whenever the next task finishes.
                 If the wait times out all remaining tasks are returned (which
                 will have an in-progress status). A tuple of task id and its
                 response.
         """
-        assert timeinc > 0.0
-        assert timeout is None or timeout > 0.0
-        cur_ids = list(task_ids)
-        already: set[TaskId] = set()
-        start_time = time.monotonic()
-        while cur_ids:
-            task_id = cur_ids.pop(0)
-            status = self.get_status(task_id)
-            if status in (
-                    TASK_STATUS_READY,
-                    TASK_STATUS_DONE,
-                    TASK_STATUS_ERROR):
-                yield (task_id, self.get_response(task_id))
-                start_time = time.monotonic()
-                continue
-            cur_ids.append(task_id)
-            if task_id not in already:
-                already.add(task_id)
-                continue
-            already.clear()
-            elapsed = time.monotonic() - start_time
-            if timeout is not None and elapsed >= timeout:
-                break
-            if timeout is not None and elapsed + timeinc > timeout:
-                wait_time = timeout - elapsed
-            else:
-                wait_time = timeinc
-            if wait_time > 0.0:
-                time.sleep(wait_time)
-        for task_id in cur_ids:  # FIXME write timeout test?
-            yield (task_id, self.get_response(task_id))
+        raise NotImplementedError()
 
     def namespaces(self) -> set[GNamespace]:
         """
         Retrieve all registered namespaces.
 
         Returns:
             set[GNamespace]: All namespaces.
@@ -293,14 +255,23 @@
         Retrieves information about all active queues.
 
         Returns:
             Iterable[QueueCounts]: The information about each queue.
         """
         raise NotImplementedError()
 
+    def has_any_tasks(self) -> bool:
+        """
+        Checks whether any tasks are present in any queue.
+
+        Returns:
+            bool: True, if there are some tasks to be computed.
+        """
+        raise NotImplementedError()
+
     def get_healthcheck(self) -> tuple[str, str, int] | None:
         """
         Gets the address at which a healthcheck is exposed.
 
         Returns:
             tuple[str, str, int] | None: The in address, out address, port
                 tuple. If None, no healthcheck is available.
```

### Comparing `scattermind-0.4.0/src/scattermind/api/loader.py` & `scattermind-0.4.1/src/scattermind/api/loader.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/app/__init__.py` & `scattermind-0.4.1/src/scattermind/app/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/app/args.py` & `scattermind-0.4.1/src/scattermind/app/args.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/app/healthcheck.py` & `scattermind-0.4.1/src/scattermind/app/healthcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         thread_factory=threading.Thread,
         token_handler=None,
         worker_constructor=None,
         soft_worker_death=True)
 
     prefix = "/api"
 
-    server.suppress_noise = False
+    server.suppress_noise = True
 
     def report_slow_requests(
             method_str: str, path: str, duration: float) -> None:
         print(f"slow request {method_str} {path} ({duration}s)")
 
     server.report_slow_requests = report_slow_requests
```

### Comparing `scattermind-0.4.0/src/scattermind/app/worker.py` & `scattermind-0.4.1/src/scattermind/app/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,8 +67,8 @@
                 continue
             fname = os.path.join(graph_def, name)
             if not os.path.isfile(fname):
                 continue
             load_graph(fname)
     else:
         load_graph(graph_def)
-    return lambda: config.run(force_no_block=False)
+    return lambda: config.run(force_no_block=False, no_reclaim=False)
```

### Comparing `scattermind-0.4.0/src/scattermind/system/__init__.py` & `scattermind-0.4.1/src/scattermind/system/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/base.py` & `scattermind-0.4.1/src/scattermind/system/base.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/cache/__init__.py` & `scattermind-0.4.1/src/scattermind/system/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/cache/cache.py` & `scattermind-0.4.1/src/scattermind/system/cache/cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,21 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Defines the caching interface for caching graph input and outputs."""
 import hashlib
+from typing import TYPE_CHECKING
 
-from scattermind.system.base import CacheId, GraphId, Module
+from scattermind.system.base import CacheId, GraphId, Module, TaskId
 from scattermind.system.info import DataFormat
 from scattermind.system.payload.values import TaskValueContainer
 from scattermind.system.redis_util import tensor_to_redis
 
 
+if TYPE_CHECKING:
+    from scattermind.system.logger.log import EventStream
+    from scattermind.system.payload.data import DataStore
+    from scattermind.system.queue.queue import QueuePool
+
+
 class GraphCache(Module):
     """A caching layer for graph input and outputs."""
     def get_cache_id(
             self,
             graph_id: GraphId,
             input_format: DataFormat,
             tvc: TaskValueContainer) -> CacheId:
@@ -49,33 +56,67 @@
                 tvc[key], compress=False).encode("utf-8")
             blake.update(f"{len(value_bytes)}:".encode("utf-8"))
             blake.update(value_bytes)
         return CacheId(graph_id, blake.hexdigest())
 
     def put_cached_output(
             self,
+            logger: 'EventStream',
+            store: 'DataStore',
+            queue_pool: 'QueuePool',
+            *,
             cache_id: CacheId,
             output_data: TaskValueContainer) -> None:
         """
-        Caches the given result.
+        Caches the given result. It also notifies all listeners for the given
+        task.
 
         Args:
+            logger (EventStream): The logger.
+            store (DataStore): The data store for storing the payload data.
+            queue_pool (QueuePool): The queue pool.
             cache_id (CacheId): The cache id.
             output_data (TaskValueContainer): The data.
         """
         raise NotImplementedError()
 
+    def put_progress(self, cache_id: CacheId, task_id: TaskId) -> None:
+        """
+        Indicates that the given cache id is currently being computed by the
+        given task id.
+
+        Args:
+            cache_id (CacheId): The cache id.
+            task_id (TaskId): The task id.
+        """
+        raise NotImplementedError()
+
+    def add_listener(self, cache_id: CacheId, listener_id: TaskId) -> None:
+        """
+        Add a listener for the given cache id. The listener will get notified
+        when the cache gets a result. If the cache id has not an associated
+        progress task no listener will be added and all still existing
+        listeners must be removed.
+
+        Args:
+            cache_id (CacheId): The cache id.
+            listener_id (TaskId): The listening task.
+        """
+        raise NotImplementedError()
+
     def get_cached_output(
             self,
             cache_id: CacheId,
-            output_format: DataFormat) -> TaskValueContainer | None:
+            output_format: DataFormat) -> TaskValueContainer | TaskId | None:
         """
         Retrieves the cached data.
 
         Args:
             cache_id (CacheId): The cache id.
             output_format (DataFormat): The expected output format.
 
         Returns:
-            TaskValueContainer | None: The data if it is available.
+            TaskValueContainer | TaskId | None: The data if it is available.
+                It can also be the task id that is currently computing the
+                task.
         """
         raise NotImplementedError()
```

### Comparing `scattermind-0.4.0/src/scattermind/system/cache/loader.py` & `scattermind-0.4.1/src/scattermind/system/cache/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 NoCacheModule = TypedDict('NoCacheModule', {
     "name": Literal["nocache"],
 })
 """No graph caching."""
 RedisCacheModule = TypedDict('RedisCacheModule', {
     "name": Literal["redis"],
     "cfg": RedisConfig,
+    "use_defer": bool,
 })
 """Cache using redis."""
 
 
 GraphCacheModule = NoCacheModule | RedisCacheModule
 """A graph cache module configuration."""
 
@@ -55,9 +56,9 @@
         plugin = load_plugin(GraphCache, f"{kwargs.pop('name')}")
         return plugin(**kwargs)
     if module["name"] == "nocache":
         from scattermind.system.cache.nocache import NoCache
         return NoCache()
     if module["name"] == "redis":
         from scattermind.system.cache.redis import RedisCache
-        return RedisCache(module["cfg"])
+        return RedisCache(module["cfg"], use_defer=module["use_defer"])
     raise ValueError(f"unknown graph cache: {module['name']}")
```

### Comparing `scattermind-0.4.0/src/scattermind/system/cache/nocache.py` & `scattermind-0.4.1/src/scattermind/system/cache/nocache.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,30 +8,43 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A caching layer that does not do any caching."""
-from scattermind.system.base import CacheId, L_EITHER, Locality
+from scattermind.system.base import CacheId, L_EITHER, Locality, TaskId
 from scattermind.system.cache.cache import GraphCache
 from scattermind.system.info import DataFormat
+from scattermind.system.logger.log import EventStream
+from scattermind.system.payload.data import DataStore
 from scattermind.system.payload.values import TaskValueContainer
+from scattermind.system.queue.queue import QueuePool
 
 
 class NoCache(GraphCache):
     """No caching is performed with this graph cache."""
     @staticmethod
     def locality() -> Locality:
         return L_EITHER
 
     def put_cached_output(
             self,
+            logger: EventStream,
+            store: DataStore,
+            queue_pool: QueuePool,
+            *,
             cache_id: CacheId,
             output_data: TaskValueContainer) -> None:
         pass
 
+    def put_progress(self, cache_id: CacheId, task_id: TaskId) -> None:
+        pass
+
+    def add_listener(self, cache_id: CacheId, listener_id: TaskId) -> None:
+        pass
+
     def get_cached_output(
             self,
             cache_id: CacheId,
-            output_format: DataFormat) -> TaskValueContainer | None:
+            output_format: DataFormat) -> TaskValueContainer | TaskId | None:
         return None
```

### Comparing `scattermind-0.4.0/src/scattermind/system/cache/redis.py` & `scattermind-0.4.1/src/scattermind/system/graph/nodes/assertion_error.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,54 +7,52 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A caching layer implemented in redis."""
-from redipy import Redis, RedisConfig
+"""Node triggering an error."""
+from scattermind.system.base import GraphId
+from scattermind.system.graph.graph import Graph
+from scattermind.system.graph.node import Node
+from scattermind.system.info import DataFormatJSON
+from scattermind.system.payload.values import ComputeState
+from scattermind.system.queue.queue import QueuePool
+from scattermind.system.readonly.access import ReadonlyAccess
 
-from scattermind.system.base import CacheId, L_EITHER, Locality
-from scattermind.system.cache.cache import GraphCache
-from scattermind.system.info import DataFormat
-from scattermind.system.payload.values import TaskValueContainer
-from scattermind.system.redis_util import redis_to_tvc, tvc_to_redis
-
-
-class RedisCache(GraphCache):
-    """Cache using redis."""
-    def __init__(self, cfg: RedisConfig) -> None:
-        super().__init__()
-        self._redis = Redis("redis", cfg=cfg, redis_module="cache")
-
-    @staticmethod
-    def locality() -> Locality:
-        return L_EITHER
-
-    @staticmethod
-    def key(cache_id: CacheId) -> str:
-        """
-        Computes the full key.
-
-        Args:
-            cache_id (CacheId): The cache id.
-
-        Returns:
-            str: The full key.
-        """
-        return f"{cache_id.to_parseable()}"
 
-    def put_cached_output(
+class AssertionErrorNode(Node):
+    """If a task reaches this node an error is raised for the task. Put this
+    behind an `if_op` to reject faulty tasks."""
+    def do_is_pure(
             self,
-            cache_id: CacheId,
-            output_data: TaskValueContainer) -> None:
-        self._redis.set_value(self.key(cache_id), tvc_to_redis(output_data))
+            graph: Graph,
+            queue_pool: QueuePool,
+            pure_cache: dict[GraphId, bool]) -> bool:
+        return True
 
-    def get_cached_output(
-            self,
-            cache_id: CacheId,
-            output_format: DataFormat) -> TaskValueContainer | None:
-        res = self._redis.get_value(self.key(cache_id))
-        if res is None:
-            return None
-        return redis_to_tvc(res, output_format)
+    def get_input_format(self) -> DataFormatJSON:
+        return {}
+
+    def get_output_format(self) -> dict[str, DataFormatJSON]:
+        return {}
+
+    def get_weight(self) -> float:
+        return 1.0
+
+    def get_load_cost(self) -> float:
+        return 1.0
+
+    def do_load(self, roa: ReadonlyAccess) -> None:
+        pass
+
+    def do_unload(self) -> None:
+        pass
+
+    def expected_output_meta(
+            self, state: ComputeState) -> dict[str, tuple[float, int]]:
+        return {}
+
+    def execute_tasks(self, state: ComputeState) -> None:
+        msg = self.get_arg("msg").get("str")
+        raise ValueError(msg)
```

### Comparing `scattermind-0.4.0/src/scattermind/system/client/__init__.py` & `scattermind-0.4.1/src/scattermind/system/client/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/client/client.py` & `scattermind-0.4.1/src/scattermind/system/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Provides the client pool interface."""
-from collections.abc import Iterable
+from collections.abc import Callable, Iterable
 from typing import TYPE_CHECKING, TypeAlias, TypeVar
 
 from scattermind.system.base import (
     CacheId,
     DataId,
     GraphId,
     Module,
@@ -66,29 +66,30 @@
 
     def get_response(
             self,
             task_id: TaskId,
             output_format: DataFormat | None) -> ResponseObject:
         """
         Retrieves the summary of the task. If the final output are available or
-        the task caused an error, the respective fields are set.
+        the task caused an error, the respective fields are set. Make sure to
+        call `get_status` of the API first.
 
         Args:
             task_id (TaskId): The task id.
             output_format (DataFormat | None): The expected data format of the
                 final output. If the final output format is not known (e.g.,
                 if the namespace is not available) and the value is None the
                 result field will automatically be None as well.
 
         Returns:
             ResponseObject: The task summary.
         """
         return {
             "ns": self.get_namespace(task_id),
-            "status": self.get_status(task_id),
+            "status": self.get_task_status(task_id),
             "duration": self.get_duration(task_id),
             "retries": self.get_retries(task_id),
             "result":
                 None
                 if output_format is None
                 else self.get_final_output(task_id, output_format),
             "error": self.get_error(task_id),
@@ -170,47 +171,121 @@
 
         Returns:
             GNamespace | None: The namespace or None if the task does not
                 exist.
         """
         raise NotImplementedError()
 
-    def get_status(self, task_id: TaskId) -> TaskStatus:
+    def get_task_status(self, task_id: TaskId) -> TaskStatus:
         """
         Retrieves the status of the given task.
 
         Args:
             task_id (TaskId): The task id.
 
         Returns:
             TaskStatus: The status.
         """
         raise NotImplementedError()
 
+    def notify_queues(self) -> None:
+        """
+        Notifies waiting executors that new tasks are available on some queue.
+        """
+        raise NotImplementedError()
+
+    def wait_for_queues(
+            self, condition: Callable[[], bool], timeout: float) -> None:
+        """
+        Lets an executor wait until new tasks are available on some queue.
+
+        Args:
+            condition (Callable[[], bool]): If this function returns True the
+                function returns.
+            timeout (float): The timeout in seconds.
+        """
+        raise NotImplementedError()
+
+    def notify_result(self, task_id: TaskId) -> None:
+        """
+        Notifies that the results for the given task are available (or the
+        task has otherwise terminated, e.g., via error). Implementations are
+        free to interpret this as general, non task specific, notification.
+        If the task id is used, tasks must notify all deferred child tasks.
+
+        Args:
+            task_id (TaskId): The task id.
+        """
+        raise NotImplementedError()
+
+    def wait_for_task_notifications(
+            self,
+            tasks: list[TaskId],
+            *,
+            timeout: float) -> TaskId | None:
+        """
+        Waits until any of the given tasks has a final result (or has been
+        terminated for any reason; this includes the task not existing).
+
+        Args:
+            tasks (list[TaskId]): The list of tasks to wait for.
+            timeout (float): The timeout in seconds.
+
+        Returns:
+            TaskId | None: The first finished task or None if the wait timed
+                out.
+        """
+        raise NotImplementedError()
+
+    def defer_task(self, task_id: TaskId, other_task: TaskId) -> None:
+        """
+        Defers the execution of the task to the other task.
+
+        Args:
+            task_id (TaskId): The task waiting.
+            other_task (TaskId): The task executing.
+        """
+        raise NotImplementedError()
+
+    def get_deferred_task(self, task_id: TaskId) -> TaskId | None:
+        """
+        Retrieves the task that this task is deferred to if any.
+
+        Args:
+            task_id (TaskId): The task waiting.
+
+        Returns:
+            TaskId | None: The task executing or None.
+        """
+        raise NotImplementedError()
+
     def set_final_output(
             self, task_id: TaskId, final_output: 'TaskValueContainer') -> None:
         """
         Sets the final output of the task. Note, after this function completes
         successfully, the final output is stored in the client pool (instead
         of the volatile payload data storage) and is guaranteed to be
         available. However, after reading the results and returning the task
-        summary all information of the task can be freed if needed.
+        summary all information of the task can be freed if needed. Make sure
+        to notify the task completion as well.
 
         Args:
             task_id (TaskId): The task id.
             final_output (TaskValueContainer): The final output of the graph.
         """
         raise NotImplementedError()
 
     def get_final_output(
             self,
             task_id: TaskId,
             output_format: DataFormat) -> 'TaskValueContainer | None':
         """
-        Retrieves the final output of the graph.
+        Retrieves the final output of the graph. `get_status` of the API must
+        be called before this method in order to ensure that the result has
+        been properly set.
 
         Args:
             task_id (TaskId): The task id.
             output_format (DataFormat): The expected format of the final
                 output.
 
         Returns:
```

### Comparing `scattermind-0.4.0/src/scattermind/system/client/loader.py` & `scattermind-0.4.1/src/scattermind/system/client/loader.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/client/local.py` & `scattermind-0.4.1/src/scattermind/system/client/local.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A RAM-only client pool."""
 import threading
-from collections.abc import Iterable
+from collections.abc import Callable, Iterable
 from typing import TypeVar
 
 from scattermind.system.base import CacheId, DataId, L_LOCAL, Locality, TaskId
 from scattermind.system.client.client import ClientPool, TaskFrame
 from scattermind.system.info import DataFormat
 from scattermind.system.logger.context import ctx_fmt
 from scattermind.system.logger.error import ErrorInfo
 from scattermind.system.names import GNamespace, ValueMap
 from scattermind.system.payload.data import DataStore
 from scattermind.system.payload.values import DataContainer, TaskValueContainer
 from scattermind.system.response import (
+    TASK_COMPLETE,
     TASK_STATUS_DONE,
     TASK_STATUS_INIT,
     TASK_STATUS_UNKNOWN,
     TaskStatus,
 )
 from scattermind.system.util import get_time_str, seconds_since
 
@@ -51,17 +52,20 @@
         self._start_times: dict[TaskId, str] = {}
         self._duration: dict[TaskId, float] = {}
         self._weight: dict[TaskId, float] = {}
         self._byte_size: dict[TaskId, int] = {}
         self._cache_ids: dict[TaskId, list[CacheId | None]] = {}
         self._stack_data: dict[TaskId, list[DataContainer]] = {}
         self._stack_frame: dict[TaskId, list[TaskFrame]] = {}
+        self._defer_task: dict[TaskId, TaskId] = {}
         self._results: dict[TaskId, TaskValueContainer | None] = {}
         self._error: dict[TaskId, ErrorInfo] = {}
         self._lock = threading.RLock()
+        self._wait_queues = threading.Condition()
+        self._wait_results = threading.Condition()
 
     @staticmethod
     def locality() -> Locality:
         return L_LOCAL
 
     def create_task(
             self,
@@ -111,17 +115,57 @@
                 self._status[task_id] = status
                 res.append(task_id)
             return res
 
     def get_namespace(self, task_id: TaskId) -> GNamespace | None:
         return self._namespaces.get(task_id)
 
-    def get_status(self, task_id: TaskId) -> TaskStatus:
+    def get_task_status(self, task_id: TaskId) -> TaskStatus:
         return self._status.get(task_id, TASK_STATUS_UNKNOWN)
 
+    def notify_queues(self) -> None:
+        wait_queues = self._wait_queues
+        with wait_queues:
+            wait_queues.notify_all()
+
+    def wait_for_queues(
+            self, condition: Callable[[], bool], timeout: float) -> None:
+        wait_queues = self._wait_queues
+        with wait_queues:
+            wait_queues.wait_for(condition, timeout)
+
+    def notify_result(self, task_id: TaskId) -> None:
+        # FIXME: make usage of task_id work
+        wait_results = self._wait_results
+        with wait_results:
+            wait_results.notify_all()
+
+    def wait_for_task_notifications(
+            self,
+            tasks: list[TaskId],
+            *,
+            timeout: float) -> TaskId | None:
+        # FIXME: make usage of task_id work
+        wait_results = self._wait_results
+
+        def condition() -> TaskId | None:
+            for task_id in tasks:
+                if self.get_task_status(task_id) in TASK_COMPLETE:
+                    return task_id
+            return None
+
+        with wait_results:
+            return wait_results.wait_for(condition, timeout)
+
+    def defer_task(self, task_id: TaskId, other_task: TaskId) -> None:
+        self._defer_task[task_id] = other_task
+
+    def get_deferred_task(self, task_id: TaskId) -> TaskId | None:
+        return self._defer_task.get(task_id)
+
     def set_final_output(
             self, task_id: TaskId, final_output: TaskValueContainer) -> None:
         with self._lock:
             self._results[task_id] = final_output
 
     def get_final_output(
             self,
@@ -239,14 +283,15 @@
     def clear_progress(self, task_id: TaskId) -> None:
         with self._lock:
             self._weight[task_id] = 1.0
             self._byte_size[task_id] = 0
             self._cache_ids[task_id] = []
             self._stack_data[task_id] = [{}]
             self._stack_frame[task_id] = []
+            self._defer_task.pop(task_id, None)
             print(f"{ctx_fmt()} clear progress {task_id}")
 
     def clear_task(self, task_id: TaskId) -> None:
         with self._lock:
             self._namespaces.pop(task_id, None)
             self._values.pop(task_id, None)
             self._status.pop(task_id, None)
@@ -255,9 +300,10 @@
             self._start_times.pop(task_id, None)
             self._duration.pop(task_id, None)
             self._weight.pop(task_id, None)
             self._byte_size.pop(task_id, None)
             self._cache_ids.pop(task_id, None)
             self._stack_data.pop(task_id, None)
             self._stack_frame.pop(task_id, None)
+            self._defer_task.pop(task_id, None)
             self._error.pop(task_id, None)
             print(f"{ctx_fmt()} clear {task_id}")
```

### Comparing `scattermind-0.4.0/src/scattermind/system/client/redis.py` & `scattermind-0.4.1/src/scattermind/system/client/redis.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A redis client pool."""
-from collections.abc import Iterable
+from collections.abc import Callable, Iterable
 from typing import Literal, TypeVar
 
 from redipy import Redis, RedisConfig
 from redipy.api import PipelineAPI
 from redipy.graph.expr import JSONType
 
 from scattermind.system.base import (
@@ -42,14 +42,15 @@
     redis_to_robj,
     redis_to_tvc,
     robj_to_redis,
     RStack,
     tvc_to_redis,
 )
 from scattermind.system.response import (
+    TASK_COMPLETE,
     TASK_STATUS_DONE,
     TASK_STATUS_INIT,
     TASK_STATUS_UNKNOWN,
     TaskStatus,
     to_status,
 )
 from scattermind.system.util import get_time_str, seconds_since
@@ -67,14 +68,15 @@
     "start_time",  # time str
     "duration",  # float
     "weight",  # float
     "byte_size",  # int
     "cache_id",  # list cache_id str
     "stack_data",  # list obj str
     "stack_frame",  # list obj str
+    "defer",  # TaskId
     "result",  # TVC str
     "error",  # ErrorJSON str
 ]
 """Base keys for different storage categories."""
 
 
 class RedisClientPool(ClientPool):
@@ -207,20 +209,56 @@
 
     def get_namespace(self, task_id: TaskId) -> GNamespace | None:
         res = self.get_value("ns", task_id)
         if res is None:
             return None
         return GNamespace(res)
 
-    def get_status(self, task_id: TaskId) -> TaskStatus:
+    def get_task_status(self, task_id: TaskId) -> TaskStatus:
         res = self.get_value("status", task_id)
         if res is None:
             res = TASK_STATUS_UNKNOWN
         return to_status(res)
 
+    def notify_queues(self) -> None:
+        self._redis.publish("pqueues", "queues")
+
+    def wait_for_queues(
+            self, condition: Callable[[], bool], timeout: float) -> None:
+        self._redis.wait_for("pqueues", condition, timeout)
+
+    def notify_result(self, task_id: TaskId) -> None:
+        # FIXME: make usage of task_id work
+        self._redis.publish("presults", "results")
+
+    def wait_for_task_notifications(
+            self,
+            tasks: list[TaskId],
+            *,
+            timeout: float) -> TaskId | None:
+        # FIXME: make usage of task_id work
+
+        def condition() -> TaskId | None:
+            for task_id in tasks:
+                if self.get_task_status(task_id) in TASK_COMPLETE:
+                    return task_id
+            return None
+
+        return self._redis.wait_for("presults", condition, timeout)
+
+    def defer_task(self, task_id: TaskId, other_task: TaskId) -> None:
+        with self._redis.pipeline() as pipe:
+            self.set_value(pipe, "defer", task_id, other_task.to_parseable())
+
+    def get_deferred_task(self, task_id: TaskId) -> TaskId | None:
+        res = self.get_value("defer", task_id)
+        if res is None:
+            return None
+        return TaskId.parse(res)
+
     def set_final_output(
             self, task_id: TaskId, final_output: TaskValueContainer) -> None:
         with self._redis.pipeline() as pipe:
             self.set_value(pipe, "result", task_id, tvc_to_redis(final_output))
 
     def get_final_output(
             self,
@@ -368,14 +406,15 @@
     def clear_progress(self, task_id: TaskId) -> None:
         with self._redis.pipeline() as pipe:
             self.set_value(pipe, "weight", task_id, "1.0")
             self.set_value(pipe, "byte_size", task_id, "0")
             self.delete(pipe, "cache_id", task_id)
             self.delete(pipe, "stack_data", task_id)
             self.delete(pipe, "stack_frame", task_id)
+            self.delete(pipe, "defer", task_id)
 
     def clear_task(self, task_id: TaskId) -> None:
         with self._redis.pipeline() as pipe:
             self.delete(pipe, "ns", task_id)
             self.delete(pipe, "values", task_id)
             self.delete(pipe, "status", task_id)
             self.delete(pipe, "retries", task_id)
@@ -383,8 +422,9 @@
             self.delete(pipe, "start_time", task_id)
             self.delete(pipe, "duration", task_id)
             self.delete(pipe, "weight", task_id)
             self.delete(pipe, "byte_size", task_id)
             self.delete(pipe, "cache_id", task_id)
             self.delete(pipe, "stack_data", task_id)
             self.delete(pipe, "stack_frame", task_id)
+            self.delete(pipe, "defer", task_id)
             self.delete(pipe, "error", task_id)
```

### Comparing `scattermind-0.4.0/src/scattermind/system/config/__init__.py` & `scattermind-0.4.1/src/scattermind/system/config/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/config/config.py` & `scattermind-0.4.1/src/scattermind/system/config/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Configurations connect modules together to make scattermind work."""
 import threading
-from collections.abc import Iterable
+import time
+from collections.abc import Callable, Iterable
 from typing import cast, TypeVar
 
 from scattermind.api.api import QueueCounts, ScattermindAPI
 from scattermind.system.base import L_EITHER, Locality, Module, TaskId
 from scattermind.system.cache.cache import GraphCache
 from scattermind.system.client.client import ClientPool
 from scattermind.system.executor.executor import ExecutorManager
@@ -30,15 +31,20 @@
 from scattermind.system.queue.queue import (
     NodeStrategy,
     QueuePool,
     QueueStrategy,
 )
 from scattermind.system.readonly.access import ReadonlyAccess
 from scattermind.system.readonly.writer import RoAWriter
-from scattermind.system.response import ResponseObject, TaskStatus
+from scattermind.system.response import (
+    ResponseObject,
+    TASK_COMPLETE,
+    TASK_STATUS_DEFER,
+    TaskStatus,
+)
 from scattermind.system.torch_util import DTypeName
 
 
 ModuleT = TypeVar('ModuleT', bound=Module)
 """A module type."""
 
 
@@ -376,17 +382,59 @@
         queue_pool = self.get_queue_pool()
         return queue_pool.enqueue_task(ns, store, value)
 
     def get_namespace(self, task_id: TaskId) -> GNamespace | None:
         cpool = self.get_client_pool()
         return cpool.get_namespace(task_id)
 
+    def wait_for(
+            self,
+            task_ids: list[TaskId],
+            *,
+            timeout: float | None = 10.0,
+            ) -> Iterable[tuple[TaskId, ResponseObject]]:
+        assert timeout is None or timeout > 0.0
+        cpool = self.get_client_pool()
+        cur_ids: set[TaskId] = set(task_ids)
+        start_time = time.monotonic()
+        individual_timeout: float = 60.0 if timeout is None else timeout
+        while cur_ids:
+            task_id = cpool.wait_for_task_notifications(
+                list(cur_ids), timeout=individual_timeout)
+            elapsed = time.monotonic() - start_time
+            if task_id is None:
+                if timeout is not None and elapsed >= timeout:
+                    break
+                continue
+            status = self.get_status(task_id)
+            if status in TASK_COMPLETE:
+                yield (task_id, self.get_response(task_id))
+                start_time = time.monotonic()
+                cur_ids.remove(task_id)
+        for task_id in cur_ids:  # FIXME write timeout test?
+            yield (task_id, self.get_response(task_id))
+
     def get_status(self, task_id: TaskId) -> TaskStatus:
+        # FIXME: remove side-effects of this method
         cpool = self.get_client_pool()
-        return cpool.get_status(task_id)
+        res = cpool.get_task_status(task_id)
+        if res == TASK_STATUS_DEFER:
+            defer_id = cpool.get_deferred_task(task_id)
+            if defer_id is not None and defer_id != task_id:
+                defer_status = self.get_status(defer_id)
+                if defer_status not in TASK_COMPLETE:
+                    return defer_status
+            cpool.clear_task(task_id)
+            logger = self.get_logger()
+            store = self.get_data_store()
+            queue_pool = self.get_queue_pool()
+            queue_pool.maybe_requeue_task_id(
+                logger, store, task_id, error_info=None)
+            res = cpool.get_task_status(task_id)
+        return res
 
     def get_result(self, task_id: TaskId) -> TaskValueContainer | None:
         cpool = self.get_client_pool()
         ns = cpool.get_namespace(task_id)
         if ns is None:
             return None
         queue_pool = self.get_queue_pool()
@@ -404,44 +452,62 @@
         output_format = queue_pool.get_output_format(graph_id)
         return cpool.get_response(task_id, output_format)
 
     def clear_task(self, task_id: TaskId) -> None:
         cpool = self.get_client_pool()
         cpool.clear_task(task_id)
 
-    def run(self, *, force_no_block: bool) -> int | None:
+    def run(self, *, force_no_block: bool, no_reclaim: bool) -> int | None:
         """
         Run the executor given by this configuration.
 
         Args:
             force_no_block (bool): If set, forces the function to become
                 non-blocking.
+            no_reclaim (bool): If set, the reclaimer will not be executed.
+                This is only recommended for tests.
 
         Returns:
             int | None: If the call is blocking (i.e., the work is done inside
                 this function call) the exit code is returned as int. Otherwise
                 the function returns None.
         """
         executor_manager = self.get_executor_manager()
+        cpool = self.get_client_pool()
         queue_pool = self.get_queue_pool()
         store = self.get_data_store()
         roa = self.get_readonly_access()
         logger = self.get_logger()
 
         def reclaim_all_once() -> tuple[int, int]:
             return executor_manager.reclaim_inactive_tasks(
-                logger, queue_pool, store)
+                logger, cpool, queue_pool, store)
+
+        if not no_reclaim:
+            executor_manager.start_reclaimer(logger, reclaim_all_once)
 
-        executor_manager.start_reclaimer(logger, reclaim_all_once)
+        def wait_for_task(
+                is_release_requested: Callable[[], bool],
+                timeout: float) -> None:
+
+            def task_condition() -> bool:
+                if is_release_requested():
+                    return True
+                return self.has_any_tasks()
+
+            cpool.wait_for_queues(task_condition, timeout)
 
         def work(emng: ExecutorManager) -> bool:
             return emng.execute_batch(logger, queue_pool, store, roa)
 
         def do_execute() -> int | None:
-            return executor_manager.execute(logger, work)
+            return executor_manager.execute(
+                logger,
+                wait_for_task=wait_for_task,
+                work=work)
 
         if not force_no_block:
             return do_execute()
 
         th = threading.Thread(target=do_execute, daemon=False)
         th.start()
         return None
@@ -485,7 +551,16 @@
                 queue_pool)
             yield {
                 "id": qid,
                 "name": qual_name,
                 "queue_length": queue_length,
                 "listeners": listerners,
             }
+
+    def has_any_tasks(self) -> bool:
+        queue_pool = self.get_queue_pool()
+        for qid in queue_pool.get_all_queues():
+            queue = queue_pool.get_queue(qid)
+            queue_length = queue.get_queue_length()
+            if queue_length > 0:
+                return True
+        return False
```

### Comparing `scattermind-0.4.0/src/scattermind/system/config/loader.py` & `scattermind-0.4.1/src/scattermind/system/config/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,24 +180,24 @@
     queue_pool: QueuePoolModule
     graph_cache: GraphCacheModule
     if parallelism > 0:
         executor_manager = {
             "name": "thread",
             "batch_size": batch_size,
             "parallelism": parallelism,
-            "sleep_on_idle": 0.01,
+            "sleep_on_idle": 60.0,
             "reclaim_sleep": 60.0,
         }
     elif parallelism == -1:
         executor_manager = {
             "name": "redis",
             "batch_size": batch_size,
-            "sleep_on_idle": 0.01,
+            "sleep_on_idle": 60.0,
             "reclaim_sleep": 60.0,
-            "heartbeat_time": 1.0,
+            "heartbeat_time": 0.1,
             "cfg": get_test_config(),
         }
     elif parallelism == 0:
         executor_manager = {
             "name": "single",
             "batch_size": batch_size,
         }
@@ -234,14 +234,15 @@
         graph_cache = {
             "name": "nocache",
         }
     else:
         graph_cache = {
             "name": "redis",
             "cfg": get_test_config(),
+            "use_defer": True,
         }
     test_config: ConfigJSON = {
         "client_pool": client_pool,
         "data_store": data_store,
         "executor_manager": executor_manager,
         "queue_pool": queue_pool,
         "graph_cache": graph_cache,
```

### Comparing `scattermind-0.4.0/src/scattermind/system/executor/__init__.py` & `scattermind-0.4.1/src/scattermind/system/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/executor/executor.py` & `scattermind-0.4.1/src/scattermind/system/executor/executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Executor that computes the execution graph."""
 import time
 import traceback
 from collections.abc import Callable
+from typing import TYPE_CHECKING
 
 from scattermind.system.base import ExecutorId, Module, TaskId
 from scattermind.system.graph.node import Node
 from scattermind.system.logger.context import (
     add_context,
     ContextInfo,
     get_ctx,
@@ -28,14 +29,18 @@
 from scattermind.system.logger.log import EventStream
 from scattermind.system.payload.data import DataStore
 from scattermind.system.payload.values import ComputeState, NoTasksToCompute
 from scattermind.system.queue.queue import QueuePool
 from scattermind.system.readonly.access import ReadonlyAccess
 
 
+if TYPE_CHECKING:
+    from scattermind.system.client.client import ClientPool
+
+
 class Executor:
     """A wrapper to handle executor control methods more easily.
     This is used to represent (other) executors for operations."""
     def __init__(
             self, emng: 'ExecutorManager', executor_id: ExecutorId) -> None:
         """
         Create an executor object.
@@ -54,26 +59,40 @@
         Returns:
             ExecutorId: The executor id.
         """
         return self._executor_id
 
     def is_active(self) -> bool:
         """
-        Whether the exxecutor is currently active.
+        Whether the executor is currently active.
 
         Returns:
             bool: True if the executor is active.
         """
         return self._emng.is_active(self._executor_id)
 
-    def release(self) -> None:
+    def is_fully_terminated(self) -> bool:
+        """
+        Whether the executor has been completely shut down.
+
+        Returns:
+            bool: True if the executor has been completely shut down.
+        """
+        return self._emng.is_fully_terminated(self._executor_id)
+
+    def release(self, client: 'ClientPool') -> None:
         """
         Releases the executor and removes it from the pool whenever possible.
+
+        Args:
+            client (ClientPool): The configuration associated with the executor
+                to cut short waiting for tasks.
         """
-        return self._emng.release_executor(self._executor_id)
+        self._emng.release_executor(self._executor_id)
+        client.notify_queues()
 
 
 class ExecutorManager(Module):
     """
     An executor manager handles starting and stopping executors, running the
     execution loop, and various housekeeping operations (such as releasing
     unresponsive executors). In a distributed setting each executor runs an
@@ -228,14 +247,16 @@
                 )
                 r_code = "memory_purge"
                 r_tback = [
                     line.rstrip()
                     for line in traceback.format_exception(nttc)
                 ]
                 r_pctx = get_preexc_ctx()
+            except KeyboardInterrupt:  # pylint: disable=try-except-raise
+                raise
             except Exception as exc:  # pylint: disable=broad-except
                 e_msg = f"{exc}"
                 e_code = "general_exception"
                 e_tback = [
                     line.rstrip()
                     for line in traceback.format_exception(exc)
                 ]
@@ -282,63 +303,70 @@
                 for task in state.get_inputs_tasks():
                     i_task_id = task.get_task_id()
                     if i_task_id not in maybe_requeue:
                         maybe_requeue[i_task_id] = get_error(i_task_id)
             for task_id, error in maybe_requeue.items():
                 with add_context({"task": task_id}):
                     queue_pool.maybe_requeue_task_id(
-                        logger, store, task_id, error)
+                        logger, store, task_id, error_info=error)
             queue.unclaim_tasks(own_id)
             return True
 
     def reclaim_inactive_tasks(  # FIXME write test for dead executors
             self,
             logger: EventStream,
+            cpool: 'ClientPool',
             queue_pool: QueuePool,
             store: DataStore) -> tuple[int, int]:
         """
         Reclaim tasks from inactive executors. Tasks whose execution was not
         complete for their current node (results were not committed) are made
         available in their queue again.
 
         Args:
             logger (EventStream): The logger.
+            cpool (ClientPool): The client pool.
             queue_pool (QueuePool): The queue pool.
             store (DataStore): The payload data store.
 
         Returns:
             tuple[int, int]: The number of reclaimed executors. The first
                 number is the number of detected inactive executors. The second
                 number is the number of unknown / inactive listeners.
         """
         executor_count = 0
         for executor in self.get_all_executors():
             if executor.is_active():
                 continue
-            self.handle_inactive_executor(logger, queue_pool, store, executor)
+            self.handle_inactive_executor(
+                logger, cpool, queue_pool, store, executor)
             executor_count += 1
 
         def is_active(executor_id: ExecutorId) -> bool:
-            return self.is_active(executor_id)
+            return (
+                self.is_active(executor_id)
+                and not self.is_fully_terminated(executor_id))
 
         listener_count = queue_pool.clean_listeners(is_active)
         return executor_count, listener_count
 
     def handle_inactive_executor(
             self,
             logger: EventStream,
+            cpool: 'ClientPool',
             queue_pool: QueuePool,
             store: DataStore,
             executor: Executor) -> None:
         """
         Unclaims tasks from an unresponsive executor and makes them available
         in their queue again. This increases the retries count of the tasks.
 
         Args:
             logger (EventStream): The logger.
+            cpool (ClientPool): The client pool.
             queue_pool (QueuePool): The queue pool.
             store (DataStore): The payload data store.
             executor (Executor): The unresponsive executor.
         """
         executor_id = executor.get_id()
         with add_context({"executor": executor_id}):
             for qid in queue_pool.get_all_queues():
@@ -347,53 +375,66 @@
                 queue = queue_pool.get_queue(qid)
                 for reclaim_id in queue.unclaim_tasks(executor_id):
                     with add_context({"task": reclaim_id}):
                         queue_pool.maybe_requeue_task_id(
                             logger,
                             store,
                             reclaim_id,
-                            {
+                            error_info={
                                 "ctx": get_ctx(),
                                 "message": "executor is unresponsive",
                                 "code": "defunc_executor",
                                 "traceback": [],
                             })
-        executor.release()
+        executor.release(cpool)
 
-    def release_all(self, *, timeout: float | None = None) -> None:
+    def release_all(
+            self,
+            cpool: 'ClientPool',
+            *,
+            timeout: float | None = None,
+            max_sleep: float = 0.1) -> None:
         """
         Release all executors. This usually results in halting all execution.
 
         Args:
+            cpool (ClientPool): The client pool.
             timeout (float | None, optional): Wait until all executors are
                 inactive or the number of seconds runs out. If None the
                 function returns immediately in any case. Defaults to None.
+            max_sleep (float, optional): The maximal sleep allowed in seconds.
+                Defaults to 0.1 seconds.
         """
         for executor in self.get_all_executors():
-            executor.release()
+            executor.release(cpool)
         if timeout is None:
             return
         start_time = time.monotonic()
         while time.monotonic() - start_time < timeout:
             if not self.any_active():
                 return
-            sleep_time = timeout - (time.monotonic() - start_time)
+            sleep_time = min(
+                max_sleep,
+                timeout - (time.monotonic() - start_time))
             if sleep_time > 0.0:
                 time.sleep(sleep_time)
 
     def any_active(self) -> bool:
         """
         Whether there are any registered active executors.
 
         Returns:
-            bool: True if there is at least one active executor.
+            bool: True if there is at least one active executor that has not
+                been fully terminated.
         """
         for executor in self.get_all_executors():
             if executor.is_active():
                 return True
+            if not executor.is_fully_terminated():
+                return True
         return False
 
     def get_all_executors(self) -> list[Executor]:
         """
         Retrieve all registered executors.
 
         Returns:
@@ -409,19 +450,47 @@
             executor_id (ExecutorId): The executor id.
 
         Returns:
             bool: True, if the executor is active.
         """
         raise NotImplementedError()
 
+    def is_release_requested(self, executor_id: ExecutorId) -> bool:
+        """
+        Whether the executor has been requested to shut down or is not active.
+
+        Args:
+            executor_id (ExecutorId): The executor id.
+
+        Returns:
+            bool: True if the executor is requested to shut down or has already
+                shut down.
+        """
+        raise NotImplementedError()
+
+    def is_fully_terminated(self, executor_id: ExecutorId) -> bool:
+        """
+        Whether the executor has been completely shut down.
+
+        Args:
+            executor_id (ExecutorId): The executor id.
+
+        Returns:
+            bool: True if the executor has been completely shut down.
+        """
+        raise NotImplementedError()
+
     def release_executor(self, executor_id: ExecutorId) -> None:
         """
         Release an executor and let it stop processing tasks. This does not
         necessarily result in an immediate termination of the associated
-        compute resource.
+        compute resource. More specifically, this method does not shorten wait
+        for tasks or interrupt execution of tasks. If waiting for tasks should
+        be skipped in order to release the executor faster use the
+        corresponding `release` method from the `Executor` class.
 
         Args:
             executor_id (ExecutorId): The executor id to stop.
         """
         raise NotImplementedError()
 
     def start_reclaimer(
@@ -443,26 +512,32 @@
                 and the inactive listeners respectively.
         """
         raise NotImplementedError()
 
     def execute(
             self,
             logger: EventStream,
+            *,
+            wait_for_task: Callable[[Callable[[], bool], float], None],
             work: Callable[['ExecutorManager'], bool]) -> int | None:
         """
         At its core, this function calls `work` repeatedly until `work` returns
         True. The function might also do bookkeeping and setting the "active"
         status of the own executor. That said, this function might also just
         kick off executing the `work` callback. Furthermore, an executor is
-        free to continue working even after `work` return True (ideally, add
-        a small timeout before continuing to not spinwait on tasks). For
-        stopping executors use the `release_executor` function.
+        free to continue working even after `work` return True (use
+        wait_for_task to idle in this case). For stopping executors use the
+        `release_executor` function.
 
         Args:
             logger (EventStream): The logger.
+            wait_for_task (Callable[[Callable[[], bool], float], None]): Waits
+                until a task is available or timeout in seconds is reached.
+                The callback passed as argument returns whether a shutdown was
+                requested.
             work (Callable[[ExecutorManager], bool]): The work. Call this
                 function until it returns True (i.e., work is done).
 
         Returns:
             int | None: If this call is blocking (i.e., work is directly done
                 inside the function call) then the function returns an integer
                 exit code. If it is non-blocking (i.e., calling this function
```

### Comparing `scattermind-0.4.0/src/scattermind/system/executor/loader.py` & `scattermind-0.4.1/src/scattermind/system/executor/loader.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/executor/redis.py` & `scattermind-0.4.1/src/scattermind/system/executor/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,21 @@
             else Executor(self, executor_id)
             for executor_id in self._get_executors()
         ]
 
     def is_active(self, executor_id: ExecutorId) -> bool:
         return self._get_state(executor_id) is not None
 
+    def is_release_requested(self, executor_id: ExecutorId) -> bool:
+        state = self._get_state(executor_id)
+        return state is None or state == ES_EXIT
+
+    def is_fully_terminated(self, executor_id: ExecutorId) -> bool:
+        return self._get_state(executor_id) is None
+
     def release_executor(self, executor_id: ExecutorId) -> None:
         self._set_state(executor_id, ES_EXIT, if_exists=True)
 
     def get_logger(self) -> EventStream:
         """
         Retrieves the logger.
 
@@ -217,14 +224,16 @@
             logger: EventStream,
             reclaim_all_once: Callable[[], tuple[int, int]]) -> None:
         own_id = self.get_own_id()
 
         def do_reclaim() -> None:
             conn_error = 0
             general_error = 0
+            # NOTE: on startup we wait for old executors to disappear first
+            time.sleep(10.0 + max(0.0, self._heartbeat_time * 2.0))
             while reclaim is self._reclaim:
                 try:
                     executor_count, listener_count = reclaim_all_once()
                     if executor_count > 0 or listener_count > 0:
                         logger.log_event(
                             "tally.executor.reclaim",
                             {
@@ -236,14 +245,16 @@
                     conn_error = 0
                     general_error = 0
                 except (ConnectionError, redis_lib.ConnectionError):
                     conn_error += 1
                     if conn_error > 10:
                         logger.log_error("error.executor", "connection")
                     time.sleep(60)
+                except KeyboardInterrupt:  # pylint: disable=try-except-raise
+                    raise
                 except Exception:  # pylint: disable=broad-exception-caught
                     general_error += 1
                     logger.log_error(
                         "error.executor", "uncaught_executor")
                     if general_error > 10:
                         raise
                     time.sleep(10)
@@ -284,14 +295,16 @@
             daemon=True)
         self._reclaim = reclaim
         reclaim.start()
 
     def execute(
             self,
             logger: EventStream,
+            *,
+            wait_for_task: Callable[[Callable[[], bool], float], None],
             work: Callable[[ExecutorManager], bool]) -> int | None:
         self._logger = logger
         own_id = self.get_own_id()
         running = True
         error = False
         with add_context({"executor": own_id}):
             logger.log_event(
@@ -313,22 +326,26 @@
                 conn_count = 0
                 while self._get_state(own_id) == ES_RUN:
                     sleep_on_idle = self._sleep_on_idle * 0.5
                     sleep_on_idle += random.uniform(
                         0.0, max(sleep_on_idle, 0.0))
                     try:
                         if not work(self) and sleep_on_idle > 0.0:
-                            time.sleep(sleep_on_idle)
+                            wait_for_task(
+                                lambda: self.is_release_requested(own_id),
+                                sleep_on_idle)
                         conn_count = 0
                     except (ConnectionError, redis_lib.ConnectionError):
                         conn_count += 1
                         if conn_count > 10:
                             logger.log_error("error.executor", "connection")
                         time.sleep(60)
                 running = False
+            except KeyboardInterrupt:  # pylint: disable=try-except-raise
+                raise
             except Exception:  # pylint: disable=broad-except
                 logger.log_error("error.executor", "uncaught_executor")
                 error = True
                 running = False
             finally:
                 self._set_state(own_id, None, if_exists=False)
                 logger.log_event(
```

### Comparing `scattermind-0.4.0/src/scattermind/system/executor/single.py` & `scattermind-0.4.1/src/scattermind/system/executor/single.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,26 +33,34 @@
 
     def get_all_executors(self) -> list[Executor]:
         return [self.as_executor()]
 
     def is_active(self, executor_id: ExecutorId) -> bool:
         return self._is_active
 
+    def is_release_requested(self, executor_id: ExecutorId) -> bool:
+        return not self._is_active
+
+    def is_fully_terminated(self, executor_id: ExecutorId) -> bool:
+        return not self._is_active
+
     def release_executor(self, executor_id: ExecutorId) -> None:
         pass
 
     def start_reclaimer(
             self,
             logger: EventStream,
             reclaim_all_once: Callable[[], tuple[int, int]]) -> None:
         pass  # NOTE: we do not reclaim executors
 
     def execute(
             self,
             logger: EventStream,
+            *,
+            wait_for_task: Callable[[Callable[[], bool], float], None],
             work: Callable[[ExecutorManager], bool]) -> int | None:
         with add_context({"executor": self.get_own_id()}):
             running = True
             error = False
             logger.log_event(
                 "tally.executor.start",
                 {
@@ -61,14 +69,16 @@
                 })
             try:
                 self._is_active = True
                 done = False
                 while not done:
                     done = not work(self)
                 running = False
+            except KeyboardInterrupt:  # pylint: disable=try-except-raise
+                raise
             except Exception:  # pylint: disable=broad-except
                 logger.log_error("error.executor", "uncaught_executor")
                 running = False
                 error = True
             finally:
                 self._is_active = False
                 logger.log_event(
```

### Comparing `scattermind-0.4.0/src/scattermind/system/executor/thread.py` & `scattermind-0.4.1/src/scattermind/system/logger/log.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,289 +7,292 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""A thread based executor that keeps running even if no tasks are available.
-"""
-import random
+"""Provides the custom logging for scattermind. Logging can be both messages,
+as well as, statistics about the runtime. Different backends can be used to
+compile statistics and provide monitoring capabilities."""
+import contextlib
+
+# import io
 import sys
-import threading
-import time
-from collections.abc import Callable
-
-import redis as redis_lib
-
-from scattermind.system.base import ExecutorId, L_EITHER, Locality
-from scattermind.system.executor.executor import Executor, ExecutorManager
-from scattermind.system.logger.context import add_context
-from scattermind.system.logger.log import EventStream
-
-
-LOCK = threading.RLock()
-"""The main lock."""
-EXECUTORS: dict[ExecutorId, 'ThreadExecutorManager'] = {}
-"""All registered executors."""
-ACTIVE: dict[ExecutorId, bool] = {}
-"""Indicates which executors are active."""
-ALIVE: set[ExecutorId] = set()
-"""The set of executors that are alive. This number is not reliable for
-accounting for unexpectedly terminated executors. Use listener count for this.
-"""
-
-
-class ThreadExecutorManager(ExecutorManager):
-    """Manager for a thread based executor that keeps running even if no tasks
-    are available. The number of threads is specified in the configuration and
-    the corresponding number of managers will be created."""
-    def __init__(
+import traceback
+from collections.abc import Callable, Iterator
+
+from scattermind.system.logger.context import (
+    ContextInfo,
+    get_ctx,
+    get_preexc_ctx,
+)
+from scattermind.system.logger.error import ErrorCode
+from scattermind.system.logger.event import AnyEvent, EventInfo
+from scattermind.system.util import is_partial_match, now
+
+
+class EventListener:
+    """The base class for event listeners."""
+    def __init__(self, *, disable_events: list[str] | None = None) -> None:
+        """
+        Creates an event listener. Sub-classes need to expose all keyword
+        arguments as well.
+
+        Args:
+            disable_events (list[str] | None, optional): Which events to
+                ignore. Each string is a plain text pattern and must fully
+                match event name segments. By default only prefixes are
+                checked. A `.` prefix enables the rule to be applied to inner
+                matches as well. A `!` prefix negates the rule and makes it
+                inclusive instead. A value of None allows all events. Defaults
+                to None.
+
+        Raises:
+            ValueError: If an invalid filter was passed.
+        """
+        self._pos_filters = []
+        self._neg_filters = []
+        all_filters = [] if disable_events is None else disable_events
+        for cur in all_filters:
+            if not cur or cur in ["", ".", "!", "!."]:
+                raise ValueError(f"invalid filter: {cur}")
+            flipped = cur.removeprefix("!")
+            if cur == flipped:
+                self._neg_filters.append(cur)
+            else:
+                self._pos_filters.append(flipped)
+
+    def do_capture_static(
             self,
-            own_id: ExecutorId,
-            *,
-            batch_size: int,
-            sleep_on_idle: float,
-            reclaim_sleep: float) -> None:
+            name: str) -> bool:  # pylint: disable=unused-argument
         """
-        Creates an executor manager for the given executor id.
+        Whether the event listeners wants to capture a given event. By default
+        this method returns True for all events, capturing all events.
+        Sub-classes must override this method if a different behavior is
+        preferred.
 
         Args:
-            own_id (ExecutorId): The executor id.
-            batch_size (int): The batch size for processing tasks of the
-                given executor.
-            sleep_on_idle (float): The time to sleep in seconds if no task
-                is currently available for processing.
-            reclaim_sleep (float): The time to sleep in seconds between
-                two reclaim calls.
-        """
-        super().__init__(own_id, batch_size)
-        self._sleep_on_idle = sleep_on_idle
-        self._reclaim_sleep = reclaim_sleep
-        self._thread: threading.Thread | None = None
-        self._reclaim: threading.Thread | None = None
-        self._work: Callable[[ExecutorManager], bool] | None = None
-        self._logger: EventStream | None = None
-        self._done = False
-        with LOCK:
-            EXECUTORS[own_id] = self
-            ACTIVE[own_id] = True
+            name (str): The event name. Event names are hierarchical segments
+                joined by `.`.
+
+        Returns:
+            bool: True, if the event should be processed by this event
+                listener.
+        """
+        return True  # NOTE: overwrite in subclass
 
-    def is_done(self) -> bool:
+    def capture_event(self, name: str) -> bool:
         """
-        Whether the executor should terminate at its earliest convenience.
+        Whether the event listeners captures a given event. If you want to
+        change the behavior override py::method:`do_capture_static`.
+
+        Args:
+            name (str): THe event name. Event names are hierarchical segments
+                joined by `.`.
 
         Returns:
-            bool: If True, the executor should terminate when possible.
+            bool: True, if the event will be processed by this event listener.
         """
-        return self._done
+        if not self.do_capture_static(name):
+            return False
+        for filter_str in self._pos_filters:
+            if is_partial_match(name, filter_str):
+                return True
+        for filter_str in self._neg_filters:
+            if is_partial_match(name, filter_str):
+                return False
+        return True
 
-    def set_done(self, is_done: bool) -> None:
+    def log_event(self, event: EventInfo) -> None:
         """
-        Mark the executor for termination.
+        Processes a log event.
 
         Args:
-            is_done (bool): If True, the executor will terminate when possible.
+            event (EventInfo): The event to process.
         """
-        self._done = is_done
+        raise NotImplementedError()
 
-    def _maybe_start(self) -> None:
-        # FIXME: detect when all workers terminated and exit the program with
-        # the correct status code
-        assert self._logger is not None
-        logger = self._logger
-
-        def run() -> None:
-            with add_context({"executor": self.get_own_id()}):
-                running = True
-                logger.log_event(
-                    "tally.executor.start",
-                    {
-                        "name": "executor",
-                        "action": "start",
-                    })
-                try:
-                    with LOCK:
-                        ALIVE.add(self.get_own_id())
-                    conn_count = 0
-                    while not self.is_done() and thread is self._thread:
-                        work = self._work
-                        if work is None:
-                            raise ValueError("uninitialized executor")
-                        sleep_on_idle = self._sleep_on_idle * 0.5
-                        sleep_on_idle += random.uniform(
-                            0.0, max(sleep_on_idle, 0.0))
-                        try:
-                            if not work(self) and sleep_on_idle > 0.0:
-                                time.sleep(sleep_on_idle)
-                        except (ConnectionError, redis_lib.ConnectionError):
-                            conn_count += 1
-                            if conn_count > 10:
-                                logger.log_error(
-                                    "error.executor", "connection")
-                            time.sleep(60)
-                    running = False
-                finally:
-                    logger.log_event(
-                        "tally.executor.stop",
-                        {
-                            "name": "executor",
-                            "action": "stop",
-                        })
-                    with LOCK:
-                        ALIVE.discard(self.get_own_id())
-                        ACTIVE[self.get_own_id()] = False
-                        self._thread = None
-                        if running:
-                            logger.log_error(
-                                "error.executor", "uncaught_executor")
-                            sys.exit(1)
-
-        if self._thread is not None:
-            return
-        with LOCK:
-            if self._thread is not None:
-                return
-            if self.is_done() or not self.is_active(self.get_own_id()):
-                raise ValueError("attempt to start inactive executor")
-            thread = threading.Thread(
-                target=run,
-                daemon=False)
-            self._thread = thread
-            thread.start()
-
-    @staticmethod
-    def locality() -> Locality:
-        return L_EITHER  # FIXME: figure out a way to clearly define it here
-
-    def get_all_executors(self) -> list[Executor]:
-        with LOCK:
-            return [emng.as_executor() for emng in EXECUTORS.values()]
-
-    def is_active(self, executor_id: ExecutorId) -> bool:
-        with LOCK:
-            return ACTIVE.get(executor_id, False)
-
-    def release_executor(self, executor_id: ExecutorId) -> None:
-        with LOCK:
-            executor = EXECUTORS[executor_id]
-            if executor is not None:
-                executor.set_done(True)
 
-    def get_work(self) -> Callable[[ExecutorManager], bool] | None:
+class EventStream:
+    """An event stream for logging and capturing runtime statistics. `log`
+    methods can be used to add events to the stream. The
+    ::py:method:`add_listener` method is used to add event listeners, i.e.,
+    processing backends."""
+    def __init__(self) -> None:
+        """
+        Creates a new event stream.
         """
-        Retrieves the currently installed work callback.
+        self._listeners: list[EventListener] = []
+        self._reported_warnings: set[str] = set()
 
-        Returns:
-            Callable[[ExecutorManager], bool] | None: The work callback or
-                None if the executor has not been started yet.
+    def add_listener(self, listener: EventListener) -> None:
         """
-        return self._work
+        Add an event listener, i.e., processing backend.
 
-    def get_logger(self) -> EventStream | None:
+        Args:
+            listener (EventListener): The listener.
         """
-        Retrieves the logger.
+        self._listeners.append(listener)
 
-        Returns:
-            EventStream | None: The logger or None if no logger has been set.
+    @contextlib.contextmanager
+    def log_output(self, name: str, entry: str) -> Iterator[None]:
+        """
+        A contextmanager to redirect all stdout and stderr content to events
+        for the given resource block.
+
+        Args:
+            name (str): The name of the event. Hierarchical segments joined by
+                `.`. Names for this function should start with `output.`.
+            entry (str): Message to provide further context.
         """
-        return self._logger
+        # pylint: disable=unused-argument
+        # stdout = io.StringIO()
+        # stderr = io.StringIO()
+        # try:
+        #     with (
+        #             contextlib.redirect_stdout(stdout),
+        #             contextlib.redirect_stderr(stderr)):
+        #         yield
+        # finally:
+        #     if stdout.tell() > 0 or stderr.tell() > 0:
+        #         self.log_event(
+        #             name,
+        #             {
+        #                 "name": "output",
+        #                 "entry": entry,
+        #                 "stdout": stdout.getvalue(),
+        #                 "stderr": stderr.getvalue(),
+        #             })
+        yield  # FIXME: make it work with multiple threads
 
-    def start_reclaimer(
+    def log_event(
             self,
-            logger: EventStream,
-            reclaim_all_once: Callable[[], tuple[int, int]]) -> None:
-        conn_error = 0
-        general_error = 0
-
-        def reclaim() -> None:
-            nonlocal conn_error
-            nonlocal general_error
-
-            try:
-                executor_count, listener_count = reclaim_all_once()
-                if executor_count or listener_count:
-                    logger.log_event(
-                        "tally.executor.reclaim",
-                        {
-                            "name": "executor",
-                            "action": "reclaim",
-                            "executors": executor_count,
-                            "listeners": listener_count,
-                        })
-                conn_error = 0
-                general_error = 0
-            except (ConnectionError, redis_lib.ConnectionError):
-                conn_error += 1
-                if conn_error > 10:
-                    logger.log_error(
-                        "error.executor", "connection")
-                time.sleep(60)
-            except Exception:  # pylint: disable=broad-exception-caught
-                general_error += 1
-                if general_error > 10:
-                    raise
-                logger.log_error("error.executor", "uncaught_executor")
-                time.sleep(10)
-            reclaim_sleep = self._reclaim_sleep
-            if reclaim_sleep > 0.0:
-                time.sleep(reclaim_sleep)
-
-        def run() -> None:
-            with add_context({"executor": self.get_own_id()}):
-                try:
-                    logger.log_event(
-                        "tally.executor.start",
-                        {
-                            "name": "executor",
-                            "action": "reclaim_start",
-                        })
-                    while True:
-                        reclaim()
-                finally:
-                    logger.log_event(
-                        "tally.executor.stop",
-                        {
-                            "name": "executor",
-                            "action": "reclaim_stop",
-                        })
-                    with LOCK:
-                        self._reclaim = None
-                        logger.log_error("error.executor", "uncaught_executor")
-
-        if self._reclaim is not None:
-            return
-        with LOCK:
-            if self._reclaim is not None:
-                return
-            thread = threading.Thread(
-                target=run,
-                daemon=True)
-            self._reclaim = thread
-            thread.start()
+            name: str,
+            event: AnyEvent,
+            *,
+            is_error_ctx: bool = False,
+            adjust_ctx: ContextInfo | None = None) -> None:
+        """
+        Log an event. This is a convenience function for when the event is
+        quick to create (does not require costly computation to gather
+        information) or already exists anyway.
+
+        Args:
+            name (str): The name of the event. Hierarchical segments joined by
+                `.`.
+            event (AnyEvent): The event.
+            is_error_ctx (bool, optional): Whether the current error context
+                should be included with the event. Defaults to False.
+            adjust_ctx (ContextInfo | None, optional): Additional context
+                information to be included in the event. Defaults to None.
+        """
+        self.log_lazy(
+            name,
+            lambda: event,
+            is_error_ctx=is_error_ctx,
+            adjust_ctx=adjust_ctx)
 
-    def execute(  # pylint: disable=useless-return
+    def log_warning(self, name: str, message: str) -> None:
+        """
+        Log a warning. The same warning (by name) is only reported once per
+        event stream instance.
+
+        Args:
+            name (str): The name of the event. Hierarchical segments joined by
+                `.`.
+            message (str): The warning message to provide more details.
+        """
+        self.log_event(
+            name,
+            {
+                "name": "warning",
+                "message": message,
+            })
+
+    def log_error(
             self,
-            logger: EventStream,
-            work: Callable[[ExecutorManager], bool]) -> int | None:
-        if self._work is not work or self._logger is not logger:
-            self._work = work
-            self._logger = logger
-            self._maybe_start()
-            # NOTE: propagate the work to all other thread executors
-            with LOCK:
-                executors = list(EXECUTORS.values())
-            for exe in executors:
-                is_active = exe.is_active(exe.get_own_id())
-                same_work = exe.get_work() is work
-                same_logger = self.get_logger() is logger
-                if (not same_work or not same_logger) and is_active:
-                    if exe.execute(logger, work) is not None:
-                        raise RuntimeError("this should not happen!")
-        return None
+            name: str,
+            code: ErrorCode,
+            *,
+            exc: BaseException | None = None) -> None:
+        """
+        Log an error.
 
-    @staticmethod
-    def allow_parallel() -> bool:
-        return True
+        Args:
+            name (str): The name of the event. Hierarchical segments joined by
+                `.`.
+            code (ErrorCode): The error code.
+            exc (BaseException | None, optional): The exception that caused
+                the error. If set to None the exception will be inferred from
+                the context. Defaults to None.
+        """
+        tback = [
+            line.rstrip()
+            for line in (
+                traceback.format_exc().splitlines()
+                if exc is None
+                else traceback.format_exception(exc))
+        ]
+        if exc is None:
+            exc = sys.exception()
+        notes_val = None if exc is None else getattr(exc, "__notes__", None)
+        if notes_val:
+            notes = f"\n{notes_val}"
+        else:
+            notes = ""
+        message = f"{exc}{notes}"
+        self.log_event(
+            name,
+            {
+                "name": "error",
+                "code": code,
+                "message": message,
+                "traceback": tback,
+            },
+            is_error_ctx=True)
+
+    def log_lazy(
+            self,
+            name: str,
+            event_gen: Callable[[], AnyEvent],
+            *,
+            is_error_ctx: bool = False,
+            adjust_ctx: ContextInfo | None = None) -> None:
+        """
+        Lazily log an event. This is the preferred method to log an event.
+        The event will only be created if an event listener backend actually
+        wants to process the event.
 
-    def active_count(self) -> int:
-        return len(ALIVE)
+        Args:
+            name (str): The name of the event. Hierarchical segments joined by
+                `.`.
+            event_gen (Callable[[], AnyEvent]): A callback that creates the
+                event when needed. Information that is only required for the
+                event should be retrieved in this callback to avoid computation
+                when the event is not processed.
+            is_error_ctx (bool, optional): Whether the current error context
+                should be included with the event. Defaults to False.
+            adjust_ctx (ContextInfo | None, optional): Additional context
+                information to be included in the event. Defaults to None.
+        """
+        event_info: EventInfo | None = None
+        for listener in self._listeners:
+            if not listener.capture_event(name):
+                continue
+            if event_info is None:
+                when = now()
+                ctx = get_preexc_ctx() if is_error_ctx else get_ctx()
+                if adjust_ctx is not None:
+                    ctx.update(adjust_ctx)
+                event = event_gen()
+                if event["name"] == "warning":
+                    if name in self._reported_warnings:
+                        return  # report a warning only once per instance
+                    self._reported_warnings.add(name)
+                event_info = {
+                    "when": when,
+                    "ctx": ctx,
+                    "name": name,
+                    "event": event,
+                }
+            listener.log_event(event_info)
```

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/__init__.py` & `scattermind-0.4.1/src/scattermind/system/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/args.py` & `scattermind-0.4.1/src/scattermind/system/graph/args.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,23 +19,25 @@
     GName,
     GNamespace,
     NAME_SEP,
     QualifiedGraphName,
 )
 from scattermind.system.readonly.access import DataAccess
 from scattermind.system.torch_util import DTypeName, get_dtype_name
-from scattermind.system.util import as_int_list, as_shape, to_bool
+from scattermind.system.util import as_int_list, as_shape, as_str_list, to_bool
 
 
 ArgType = Literal[
     "bool",
     "str",
     "int",
     "float",
     "list_int",
+    "list_str",
+    "set_str",
     "shape",
     "ushape",
     "format",
     "info",
     "graph",
     "dtype",
     "data",
@@ -46,28 +48,31 @@
 ArgumentType = (
     bool
     | str
     | int
     | float
     | list[int]
     | list[int | None]
+    | list[str]
     | DataFormatJSON
     | DataInfoJSON
     | DTypeName
     | DataAccess
     | None
 )
 """Available argument types as python types as seen in the JSON."""
 ArgumentRetType = (
     bool
     | str
     | int
     | float
     | list[int]
     | list[int | None]
+    | list[str]
+    | set[str]
     | DataFormatJSON
     | DataInfo
     | QualifiedGraphName
     | DTypeName
     | DataAccess
 )
 """Available argument types as python types as returned from the argument
@@ -156,14 +161,28 @@
             type_name: Literal["list_int"],
             default: list[int] | None = None) -> list[int]:
         ...
 
     @overload
     def get(
             self,
+            type_name: Literal["list_str"],
+            default: list[str] | None = None) -> list[str]:
+        ...
+
+    @overload
+    def get(
+            self,
+            type_name: Literal["set_str"],
+            default: set[str] | None = None) -> set[str]:
+        ...
+
+    @overload
+    def get(
+            self,
             type_name: Literal["shape"],
             default: list[int | None] | None = None) -> list[int | None]:
         ...
 
     @overload
     def get(
             self,
@@ -243,14 +262,19 @@
         if type_name == "int":
             return int(cast(int, val))
         if type_name == "float":
             return float(cast(float, val))
         if type_name in ("list_int", "ushape"):
             res_list_int: list[int] = as_int_list(cast(list, val))
             return res_list_int
+        if type_name in ("list_str", "set_str"):
+            res_list_str: list[str] = as_str_list(cast(list, val))
+            if type_name == "set_str":
+                return set(res_list_str)
+            return res_list_str
         if type_name == "shape":
             res_shape: list[int | None] = as_shape(cast(list, val))
             return res_shape
         if type_name == "format":
             res_format: DataFormatJSON = {
                 key: (get_dtype_name(dtype), as_shape(dims))
                 for key, (dtype, dims) in cast(dict, val).items()
```

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/graph.py` & `scattermind-0.4.1/src/scattermind/system/graph/graph.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/graphdef.py` & `scattermind-0.4.1/src/scattermind/system/graph/graphdef.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/loader.py` & `scattermind-0.4.1/src/scattermind/system/graph/loader.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/node.py` & `scattermind-0.4.1/src/scattermind/system/graph/node.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/nodes/__init__.py` & `scattermind-0.4.1/src/scattermind/system/graph/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/nodes/assertion_error.py` & `scattermind-0.4.1/src/scattermind/system/graph/nodes/load_constant.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,52 +7,78 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Node triggering an error."""
-from scattermind.system.base import GraphId
+"""Load a constant tensor."""
+import torch
+
+from scattermind.system.base import GraphId, NodeId
+from scattermind.system.client.client import ComputeTask
 from scattermind.system.graph.graph import Graph
 from scattermind.system.graph.node import Node
 from scattermind.system.info import DataFormatJSON
 from scattermind.system.payload.values import ComputeState
 from scattermind.system.queue.queue import QueuePool
 from scattermind.system.readonly.access import ReadonlyAccess
 
 
-class AssertionErrorNode(Node):
-    """If a task reaches this node an error is raised for the task. Put this
-    behind an `if_op` to reject faulty tasks."""
+class LoadConstant(Node):
+    """Load a constant tensor."""
+    def __init__(self, kind: str, graph: Graph, node_id: NodeId) -> None:
+        super().__init__(kind, graph, node_id)
+        self._constant: torch.Tensor | None = None
+
     def do_is_pure(
             self,
             graph: Graph,
             queue_pool: QueuePool,
             pure_cache: dict[GraphId, bool]) -> bool:
         return True
 
     def get_input_format(self) -> DataFormatJSON:
         return {}
 
     def get_output_format(self) -> dict[str, DataFormatJSON]:
-        return {}
+        data_info = self.get_arg("ret").get("info")
+        return {
+            "out": {
+                "value": data_info.to_json(),
+            },
+        }
 
     def get_weight(self) -> float:
         return 1.0
 
     def get_load_cost(self) -> float:
-        return 1.0
+        _, _, length = self.get_arg("data").get("data")
+        return length
 
     def do_load(self, roa: ReadonlyAccess) -> None:
-        pass
+        data = self.get_arg("data").get("data")
+        data_info = self.get_arg("ret").get("info")
+        self._constant = roa.load_tensor(data, data_info)
 
     def do_unload(self) -> None:
-        pass
+        self._constant = None
 
     def expected_output_meta(
             self, state: ComputeState) -> dict[str, tuple[float, int]]:
-        return {}
+        tasks = list(state.get_inputs_tasks())
+        return {
+            "out": (len(tasks), ComputeTask.get_total_byte_size(tasks)),
+        }
 
     def execute_tasks(self, state: ComputeState) -> None:
-        msg = self.get_arg("msg").get("str")
-        raise ValueError(msg)
+        assert self._constant is not None
+        tasks = list(state.get_inputs_tasks())
+        state.push_results(
+            "out",
+            tasks,
+            {
+                "value": state.create_uniform(torch.vstack([
+                    torch.unsqueeze(self._constant, 0)
+                    for _ in tasks
+                ])),
+            })
```

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/nodes/bin_op.py` & `scattermind-0.4.1/src/scattermind/system/graph/nodes/bin_op.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/nodes/call.py` & `scattermind-0.4.1/src/scattermind/system/graph/nodes/call.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/nodes/constant_op.py` & `scattermind-0.4.1/src/scattermind/system/graph/nodes/constant_op.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/nodes/for_loop.py` & `scattermind-0.4.1/src/scattermind/system/graph/nodes/for_loop.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/nodes/if_op.py` & `scattermind-0.4.1/src/scattermind/system/graph/nodes/if_op.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/nodes/load_constant.py` & `scattermind-0.4.1/src/scattermind/system/graph/nodes/mat_square.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,78 +7,71 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Load a constant tensor."""
+"""Square a square matrix."""
 import torch
 
-from scattermind.system.base import GraphId, NodeId
+from scattermind.system.base import GraphId
 from scattermind.system.client.client import ComputeTask
 from scattermind.system.graph.graph import Graph
 from scattermind.system.graph.node import Node
 from scattermind.system.info import DataFormatJSON
 from scattermind.system.payload.values import ComputeState
 from scattermind.system.queue.queue import QueuePool
 from scattermind.system.readonly.access import ReadonlyAccess
 
 
-class LoadConstant(Node):
-    """Load a constant tensor."""
-    def __init__(self, kind: str, graph: Graph, node_id: NodeId) -> None:
-        super().__init__(kind, graph, node_id)
-        self._constant: torch.Tensor | None = None
-
+class MatSquare(Node):
+    """Multiply a square matrix with itself."""
     def do_is_pure(
             self,
             graph: Graph,
             queue_pool: QueuePool,
             pure_cache: dict[GraphId, bool]) -> bool:
         return True
 
     def get_input_format(self) -> DataFormatJSON:
-        return {}
+        size = self.get_arg("size").get("int")
+        return {
+            "value": ("float", [size, size]),
+        }
 
     def get_output_format(self) -> dict[str, DataFormatJSON]:
-        data_info = self.get_arg("ret").get("info")
+        size = self.get_arg("size").get("int")
         return {
             "out": {
-                "value": data_info.to_json(),
+                "value": ("float", [size, size]),
             },
         }
 
     def get_weight(self) -> float:
         return 1.0
 
     def get_load_cost(self) -> float:
-        _, _, length = self.get_arg("data").get("data")
-        return length
+        return 1.0
 
     def do_load(self, roa: ReadonlyAccess) -> None:
-        data = self.get_arg("data").get("data")
-        data_info = self.get_arg("ret").get("info")
-        self._constant = roa.load_tensor(data, data_info)
+        pass
 
     def do_unload(self) -> None:
-        self._constant = None
+        pass
 
     def expected_output_meta(
             self, state: ComputeState) -> dict[str, tuple[float, int]]:
         tasks = list(state.get_inputs_tasks())
         return {
             "out": (len(tasks), ComputeTask.get_total_byte_size(tasks)),
         }
 
     def execute_tasks(self, state: ComputeState) -> None:
-        assert self._constant is not None
-        tasks = list(state.get_inputs_tasks())
+        inputs = state.get_values()
+        val = inputs.get_data("value").get_uniform()
         state.push_results(
             "out",
-            tasks,
+            inputs.get_current_tasks(),
             {
-                "value": state.create_uniform(torch.vstack([
-                    torch.unsqueeze(self._constant, 0)
-                    for _ in tasks
-                ])),
+                "value": state.create_uniform(torch.bmm(val, val)),
             })
```

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/nodes/mat_square.py` & `scattermind-0.4.1/src/scattermind/system/graph/nodes/str_concat.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,47 +7,45 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Square a square matrix."""
-import torch
-
+"""Concatenate two strings."""
 from scattermind.system.base import GraphId
 from scattermind.system.client.client import ComputeTask
 from scattermind.system.graph.graph import Graph
 from scattermind.system.graph.node import Node
 from scattermind.system.info import DataFormatJSON
 from scattermind.system.payload.values import ComputeState
 from scattermind.system.queue.queue import QueuePool
 from scattermind.system.readonly.access import ReadonlyAccess
+from scattermind.system.torch_util import str_to_tensor, tensor_to_str
 
 
-class MatSquare(Node):
-    """Multiply a square matrix with itself."""
+class StrConcat(Node):
+    """Concatenate two strings."""
     def do_is_pure(
             self,
             graph: Graph,
             queue_pool: QueuePool,
             pure_cache: dict[GraphId, bool]) -> bool:
         return True
 
     def get_input_format(self) -> DataFormatJSON:
-        size = self.get_arg("size").get("int")
         return {
-            "value": ("float", [size, size]),
+            "left": ("uint8", [None]),
+            "right": ("uint8", [None]),
         }
 
     def get_output_format(self) -> dict[str, DataFormatJSON]:
-        size = self.get_arg("size").get("int")
         return {
             "out": {
-                "value": ("float", [size, size]),
+                "value": ("uint8", [None]),
             },
         }
 
     def get_weight(self) -> float:
         return 1.0
 
     def get_load_cost(self) -> float:
@@ -63,15 +61,29 @@
             self, state: ComputeState) -> dict[str, tuple[float, int]]:
         tasks = list(state.get_inputs_tasks())
         return {
             "out": (len(tasks), ComputeTask.get_total_byte_size(tasks)),
         }
 
     def execute_tasks(self, state: ComputeState) -> None:
+        delimiter = self.get_arg("delimiter").get("str")
         inputs = state.get_values()
-        val = inputs.get_data("value").get_uniform()
-        state.push_results(
-            "out",
-            inputs.get_current_tasks(),
-            {
-                "value": state.create_uniform(torch.bmm(val, val)),
-            })
+        lefts: list[str] = [
+            tensor_to_str(left)
+            for left in inputs.get_data("left").iter_values()
+        ]
+        rights: list[str] = [
+            tensor_to_str(right)
+            for right in inputs.get_data("right").iter_values()
+        ]
+
+        outs: list[str] = [
+            f"{left}{delimiter}{right}"
+            for left, right in zip(lefts, rights)
+        ]
+        for task, out in zip(inputs.get_current_tasks(), outs):
+            state.push_results(
+                "out",
+                [task],
+                {
+                    "value": state.create_single(str_to_tensor(out)),
+                })
```

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/nodes/str_concat.py` & `scattermind-0.4.1/src/scattermind/system/readonly/ram.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,83 +7,64 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Concatenate two strings."""
-from scattermind.system.base import GraphId
-from scattermind.system.client.client import ComputeTask
-from scattermind.system.graph.graph import Graph
-from scattermind.system.graph.node import Node
-from scattermind.system.info import DataFormatJSON
-from scattermind.system.payload.values import ComputeState
-from scattermind.system.queue.queue import QueuePool
-from scattermind.system.readonly.access import ReadonlyAccess
-from scattermind.system.torch_util import str_to_tensor, tensor_to_str
-
-
-class StrConcat(Node):
-    """Concatenate two strings."""
-    def do_is_pure(
-            self,
-            graph: Graph,
-            queue_pool: QueuePool,
-            pure_cache: dict[GraphId, bool]) -> bool:
-        return True
-
-    def get_input_format(self) -> DataFormatJSON:
-        return {
-            "left": ("uint8", [None]),
-            "right": ("uint8", [None]),
-        }
-
-    def get_output_format(self) -> dict[str, DataFormatJSON]:
-        return {
-            "out": {
-                "value": ("uint8", [None]),
-            },
-        }
+"""A RAM based readonly access. It has a writer interface initially fill the
+data. It is most commonly used for test cases."""
+import os
+import threading
+from io import BytesIO, SEEK_END, SEEK_SET
 
-    def get_weight(self) -> float:
-        return 1.0
+from scattermind.system.base import L_EITHER, Locality, NodeId
+from scattermind.system.readonly.access import ReadonlyAccess
+from scattermind.system.readonly.writer import RoAWriter
 
-    def get_load_cost(self) -> float:
-        return 1.0
 
-    def do_load(self, roa: ReadonlyAccess) -> None:
-        pass
+class RAMAccess(ReadonlyAccess[str], RoAWriter[str]):
+    """A RAM based readonly access. It has a writer interface initially fill
+    the data. It is most commonly used for test cases."""
+    def __init__(self, scratch: str) -> None:
+        super().__init__()
+        self._objs: dict[str, BytesIO] = {}
+        self._scratch_folder = scratch
+        self._lock = threading.RLock()
+
+    @staticmethod
+    def locality() -> Locality:
+        return L_EITHER
+
+    def open_raw(self, path: str) -> str:
+        return path
+
+    def read_raw(self, hnd: str, offset: int, length: int) -> bytes:
+        with self._lock:
+            fout = self._objs[hnd]
+            fout.seek(offset, SEEK_SET)
+            return fout.read(length)
+
+    def open_write_raw(self, path: str) -> str:
+        with self._lock:
+            buff = self._objs.get(path)
+            if buff is None:
+                self._objs[path] = BytesIO()
+            return path
+
+    def write_raw(self, hnd: str, data: bytes) -> tuple[int, int]:
+        with self._lock:
+            fin = self._objs[hnd]
+            offset = fin.seek(0, SEEK_END)
+            length = fin.write(data)
+            return offset, length
 
-    def do_unload(self) -> None:
+    def close(self, hnd: str) -> None:
         pass
 
-    def expected_output_meta(
-            self, state: ComputeState) -> dict[str, tuple[float, int]]:
-        tasks = list(state.get_inputs_tasks())
-        return {
-            "out": (len(tasks), ComputeTask.get_total_byte_size(tasks)),
-        }
-
-    def execute_tasks(self, state: ComputeState) -> None:
-        delimiter = self.get_arg("delimiter").get("str")
-        inputs = state.get_values()
-        lefts: list[str] = [
-            tensor_to_str(left)
-            for left in inputs.get_data("left").iter_values()
-        ]
-        rights: list[str] = [
-            tensor_to_str(right)
-            for right in inputs.get_data("right").iter_values()
-        ]
-
-        outs: list[str] = [
-            f"{left}{delimiter}{right}"
-            for left, right in zip(lefts, rights)
-        ]
-        for task, out in zip(inputs.get_current_tasks(), outs):
-            state.push_results(
-                "out",
-                [task],
-                {
-                    "value": state.create_single(str_to_tensor(out)),
-                })
+    def do_get_scratchspace(self, node_id: NodeId) -> str:
+        name = node_id.to_parseable()
+        prefix = name[:3]
+        postfix = name[3:]
+        path = os.path.join(self._scratch_folder, prefix, postfix)
+        os.makedirs(path, exist_ok=True)
+        return path
```

### Comparing `scattermind-0.4.0/src/scattermind/system/graph/nodes/test_cache.py` & `scattermind-0.4.1/src/scattermind/system/graph/nodes/test_cache.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/helper.py` & `scattermind-0.4.1/src/scattermind/system/helper.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/info.py` & `scattermind-0.4.1/src/scattermind/system/info.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/logger/__init__.py` & `scattermind-0.4.1/src/scattermind/system/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/logger/context.py` & `scattermind-0.4.1/src/scattermind/system/logger/context.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/logger/error.py` & `scattermind-0.4.1/src/scattermind/system/logger/error.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/logger/event.py` & `scattermind-0.4.1/src/scattermind/system/logger/event.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/logger/listeners/__init__.py` & `scattermind-0.4.1/src/scattermind/system/logger/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/logger/listeners/stdout.py` & `scattermind-0.4.1/src/scattermind/system/logger/listeners/stdout.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/logger/loader.py` & `scattermind-0.4.1/src/scattermind/system/logger/loader.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/logger/log.py` & `scattermind-0.4.1/src/scattermind/system/names.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,292 +7,341 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Provides the custom logging for scattermind. Logging can be both messages,
-as well as, statistics about the runtime. Different backends can be used to
-compile statistics and provide monitoring capabilities."""
-import contextlib
-
-# import io
-import sys
-import traceback
-from collections.abc import Callable, Iterator
-
-from scattermind.system.logger.context import (
-    ContextInfo,
-    get_ctx,
-    get_preexc_ctx,
-)
-from scattermind.system.logger.error import ErrorCode
-from scattermind.system.logger.event import AnyEvent, EventInfo
-from scattermind.system.util import is_partial_match, now
-
-
-class EventListener:
-    """The base class for event listeners."""
-    def __init__(self, *, disable_events: list[str] | None = None) -> None:
+"""This module defines name classes. The classes guarantee that no invalid
+characters are used in a name. Names are comparable for equality and can be
+used as keys in dictionaries."""
+
+
+NAME_SEP = ":"
+"""Separator for names and queue id generation."""
+INVALID_CHARACTERS = {
+    " ",
+    "\n",
+    "\r",
+    "\t",
+    "\0",
+    "\\",
+    "\'",
+    "\"",
+    "\a",
+    "\b",
+    "\f",
+    "\v",
+}
+"""Characters specifically forbidden as characters in names."""
+
+
+class NameStr:
+    """A class to define a general name."""
+    def __init__(self, name: str) -> None:
         """
-        Creates an event listener. Sub-classes need to expose all keyword
-        arguments as well.
+        Creates a name from the given string.
 
         Args:
-            disable_events (list[str] | None, optional): Which events to
-                ignore. Each string is a plain text pattern and must fully
-                match event name segments. By default only prefixes are
-                checked. A `.` prefix enables the rule to be applied to inner
-                matches as well. A `!` prefix negates the rule and makes it
-                inclusive instead. A value of None allows all events. Defaults
-                to None.
+            name (str): The raw string.
 
         Raises:
-            ValueError: If an invalid filter was passed.
+            ValueError: If the name is not valid.
         """
-        self._pos_filters = []
-        self._neg_filters = []
-        all_filters = [] if disable_events is None else disable_events
-        for cur in all_filters:
-            if not cur or cur in ["", ".", "!", "!."]:
-                raise ValueError(f"invalid filter: {cur}")
-            flipped = cur.removeprefix("!")
-            if cur == flipped:
-                self._neg_filters.append(cur)
-            else:
-                self._pos_filters.append(flipped)
-
-    def do_capture_static(
-            self,
-            name: str) -> bool:  # pylint: disable=unused-argument
-        """
-        Whether the event listeners wants to capture a given event. By default
-        this method returns True for all events, capturing all events.
-        Sub-classes must override this method if a different behavior is
-        preferred.
+        if not self.is_valid_name(name):
+            raise ValueError(f"name {name} is not valid")
+        self._name = name
 
-        Args:
-            name (str): The event name. Event names are hierarchical segments
-                joined by `.`.
+    def get(self) -> str:
+        """
+        Gets the raw name string.
 
         Returns:
-            bool: True, if the event should be processed by this event
-                listener.
+            str: The name as string.
         """
-        return True  # NOTE: overwrite in subclass
+        return self._name
 
-    def capture_event(self, name: str) -> bool:
+    @staticmethod
+    def is_valid_name(name: str) -> bool:
         """
-        Whether the event listeners captures a given event. If you want to
-        change the behavior override py::method:`do_capture_static`.
+        Verifies that the raw name string is valid.
 
         Args:
-            name (str): THe event name. Event names are hierarchical segments
-                joined by `.`.
+            name (str): The raw name string.
 
         Returns:
-            bool: True, if the event will be processed by this event listener.
+            bool: Whether the string represents a valid name.
         """
-        if not self.do_capture_static(name):
+        return (
+            len(name) > 0
+            and NAME_SEP not in name
+            and not set(name).intersection(INVALID_CHARACTERS)
+        )
+
+    def __eq__(self, other: object) -> bool:
+        if other is self:
+            return True
+        if not isinstance(other, self.__class__):
             return False
-        for filter_str in self._pos_filters:
-            if is_partial_match(name, filter_str):
-                return True
-        for filter_str in self._neg_filters:
-            if is_partial_match(name, filter_str):
-                return False
-        return True
+        return self._name == other._name
+
+    def __ne__(self, other: object) -> bool:
+        return not self.__eq__(other)
+
+    def __hash__(self) -> int:
+        return hash(self._name)
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}[{self._name}]"
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+
+class NName(NameStr):
+    """Name of a execution node. Node names are deterministically converted
+    into node ids internally."""
+
+
+class QName(NameStr):
+    """Name of a queue. Queue names are deterministically converted into queue
+    ids internally."""
 
-    def log_event(self, event: EventInfo) -> None:
+
+class GName(NameStr):
+    """Name of a graph. Graph names are deterministically converted into graph
+    ids internally."""
+
+
+class GNamespace(NameStr):
+    """Namespace of a set of graphs."""
+
+
+class QualifiedGraphName:
+    """A fully specified graph name. It consists of a namespace and graph name.
+    """
+    def __init__(self, namespace: GNamespace, name: GName) -> None:
         """
-        Processes a log event.
+        Creates a qualified graph name.
 
         Args:
-            event (EventInfo): The event to process.
+            namespace (GNamespace): The namespace.
+            name (GName): The graph name.
+        """
+        self._namespace = namespace
+        self._name = name
+
+    def get_namespace(self) -> GNamespace:
+        """
+        Gets the namespace.
+
+        Returns:
+            GNamespace: The namespace.
+        """
+        return self._namespace
+
+    def get_name(self) -> GName:
         """
-        raise NotImplementedError()
+        Gets the graph name.
 
+        Returns:
+            GName: The graph name.
+        """
+        return self._name
 
-class EventStream:
-    """An event stream for logging and capturing runtime statistics. `log`
-    methods can be used to add events to the stream. The
-    ::py:method:`add_listener` method is used to add event listeners, i.e.,
-    processing backends."""
-    def __init__(self) -> None:
+    def to_parseable(self) -> str:
         """
-        Creates a new event stream.
+        Retrieves an unambiguous string representation.
+
+        Returns:
+            str: The qualified graph name as string.
         """
-        self._listeners: list[EventListener] = []
-        self._reported_warnings: set[str] = set()
+        return f"{self._namespace.get()}{NAME_SEP}{self._name.get()}"
 
-    def add_listener(self, listener: EventListener) -> None:
+    @staticmethod
+    def parse(text: str) -> 'QualifiedGraphName':
         """
-        Add an event listener, i.e., processing backend.
+        Parses a string into a qualified graph name. The format is expected to
+        be '{namespace}:{graph name}'.
 
         Args:
-            listener (EventListener): The listener.
+            text (str): The string to parse.
+
+        Raises:
+            ValueError: If the input is invalid.
+
+        Returns:
+            QualifiedGraphName: The qualified graph name.
         """
-        self._listeners.append(listener)
+        if NAME_SEP not in text:
+            raise ValueError(
+                f"{text} is not a qualified graph name: 'ns:graph'")
+        ns, gname = text.split(NAME_SEP, 1)
+        return QualifiedGraphName(GNamespace(ns), GName(gname))
+
+    def __eq__(self, other: object) -> bool:
+        if other is self:
+            return True
+        if not isinstance(other, self.__class__):
+            return False
+        return (
+            self._namespace == other._namespace and self._name == other._name)
+
+    def __ne__(self, other: object) -> bool:
+        return not self.__eq__(other)
+
+    def __hash__(self) -> int:
+        return hash((self._namespace, self._namespace))
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}[{self.to_parseable()}]"
 
-    @contextlib.contextmanager
-    def log_output(self, name: str, entry: str) -> Iterator[None]:
+    def __repr__(self) -> str:
+        return self.__str__()
+
+
+class QualifiedNodeName:
+    """A node name representation primarily for display purposes."""
+    def __init__(self, graph: QualifiedGraphName, node: NName) -> None:
         """
-        A contextmanager to redirect all stdout and stderr content to events
-        for the given resource block.
+        Creates a node name for display purposes.
 
         Args:
-            name (str): The name of the event. Hierarchical segments joined by
-                `.`. Names for this function should start with `output.`.
-            entry (str): Message to provide further context.
-        """
-        # pylint: disable=unused-argument
-        # stdout = io.StringIO()
-        # stderr = io.StringIO()
-        # try:
-        #     with (
-        #             contextlib.redirect_stdout(stdout),
-        #             contextlib.redirect_stderr(stderr)):
-        #         yield
-        # finally:
-        #     if stdout.tell() > 0 or stderr.tell() > 0:
-        #         self.log_event(
-        #             name,
-        #             {
-        #                 "name": "output",
-        #                 "entry": entry,
-        #                 "stdout": stdout.getvalue(),
-        #                 "stderr": stderr.getvalue(),
-        #             })
-        yield  # FIXME: make it work with multiple threads
-
-    def log_event(
-            self,
-            name: str,
-            event: AnyEvent,
-            *,
-            is_error_ctx: bool = False,
-            adjust_ctx: ContextInfo | None = None) -> None:
-        """
-        Log an event. This is a convenience function for when the event is
-        quick to create (does not require costly computation to gather
-        information) or already exists anyway.
+            graph (QualifiedGraphName): The graph the node belongs to.
+            node (NName): The node name.
+        """
+        self._graph = graph
+        self._node = node
 
-        Args:
-            name (str): The name of the event. Hierarchical segments joined by
-                `.`.
-            event (AnyEvent): The event.
-            is_error_ctx (bool, optional): Whether the current error context
-                should be included with the event. Defaults to False.
-            adjust_ctx (ContextInfo | None, optional): Additional context
-                information to be included in the event. Defaults to None.
-        """
-        self.log_lazy(
-            name,
-            lambda: event,
-            is_error_ctx=is_error_ctx,
-            adjust_ctx=adjust_ctx)
+    def get(self) -> str:
+        """
+        The name as string.
+
+        Returns:
+            str: The name as readable string.
+        """
+        return f"{self._graph.to_parseable()}{NAME_SEP}{self._node.get()}"
+
+    def __str__(self) -> str:
+        return f"Node[{self.get()}]"
 
-    def log_warning(self, name: str, message: str) -> None:
+    def __repr__(self) -> str:
+        return self.__str__()
+
+
+class QualifiedName:
+    """A qualified name describes a value field and how to access it. It
+    combines a node name and a value field name. The node name can be None
+    to describe input value fields. In the execution graph json definition
+    qualified names are the node name separated by ':' from the value field
+    name as defined in the node.
+
+    Examples: 'node_2:out' addresses the output value field 'out' from the
+    node named 'node_2'. ':text' addresses the input value field 'text' of
+    the current execution graph."""
+    def __init__(self, nname: NName | None, vname: str) -> None:
         """
-        Log a warning. The same warning (by name) is only reported once per
-        event stream instance.
+        Creates a qualified name from its individual parts.
 
         Args:
-            name (str): The name of the event. Hierarchical segments joined by
-                `.`.
-            message (str): The warning message to provide more details.
-        """
-        self.log_event(
-            name,
-            {
-                "name": "warning",
-                "message": message,
-            })
-
-    def log_error(
-            self,
-            name: str,
-            code: ErrorCode,
-            *,
-            exc: BaseException | None = None) -> None:
+            nname (NName | None): The node name or None to specify the input
+                of the current execution graph.
+            vname (str): The value field name of the node or execution graph.
+
+        Raises:
+            ValueError: If the value field name is not valid.
         """
-        Log an error.
+        if not self.is_valid_name(vname):
+            raise ValueError(f"value name {vname} is not valid")
+        self._nname = nname
+        self._vname = vname
+
+    @staticmethod
+    def is_valid_name(vname: str) -> bool:
+        """
+        Whether the given value field name is valid.
 
         Args:
-            name (str): The name of the event. Hierarchical segments joined by
-                `.`.
-            code (ErrorCode): The error code.
-            exc (BaseException | None, optional): The exception that caused
-                the error. If set to None the exception will be inferred from
-                the context. Defaults to None.
-        """
-        tback = [
-            line.rstrip()
-            for line in (
-                traceback.format_exc().splitlines()
-                if exc is None
-                else traceback.format_exception(exc))
-        ]
-        if exc is None:
-            exc = sys.exception()
-        notes_val = None if exc is None else getattr(exc, "__notes__", None)
-        if notes_val:
-            notes = f"\n{notes_val}"
-        else:
-            notes = ""
-        message = f"{exc}{notes}"
-        self.log_event(
-            name,
-            {
-                "name": "error",
-                "code": code,
-                "message": message,
-                "traceback": tback,
-            },
-            is_error_ctx=True)
-
-    def log_lazy(
-            self,
-            name: str,
-            event_gen: Callable[[], AnyEvent],
-            *,
-            is_error_ctx: bool = False,
-            adjust_ctx: ContextInfo | None = None) -> None:
-        """
-        Lazily log an event. This is the preferred method to log an event.
-        The event will only be created if an event listener backend actually
-        wants to process the event.
+            vname (str): The raw value field name string.
+
+        Returns:
+            bool: Whether the name is valid.
+        """
+        return (
+            len(vname) > 0
+            and NAME_SEP not in vname
+            and not set(vname).intersection(INVALID_CHARACTERS)
+        )
+
+    def get_value_name(self) -> str:
+        """
+        Get the raw value field name string.
+
+        Returns:
+            str: The raw string.
+        """
+        return self._vname
+
+    def to_parseable(self) -> str:
+        """
+        Get a parseable representation of the qualified name as it would be
+        found in the execution graph json.
+
+        Examples: 'node_2:out' addresses the output value field 'out' from the
+        node named 'node_2'. ':text' addresses the input value field 'text' of
+        the current execution graph (the node name is None in this case).
+
+        Returns:
+            str: The qualified name.
+        """
+        if self._nname is None:
+            return f"{NAME_SEP}{self._vname}"
+        return f"{self._nname.get()}{NAME_SEP}{self._vname}"
+
+    @staticmethod
+    def parse(text: str) -> 'QualifiedName':
+        """
+        Parses a string into a qualified name. The format is expected to be
+        '{node name}:{value field name}' or ':{value field name}' for the
+        input of the current execution graph.
 
         Args:
-            name (str): The name of the event. Hierarchical segments joined by
-                `.`.
-            event_gen (Callable[[], AnyEvent]): A callback that creates the
-                event when needed. Information that is only required for the
-                event should be retrieved in this callback to avoid computation
-                when the event is not processed.
-            is_error_ctx (bool, optional): Whether the current error context
-                should be included with the event. Defaults to False.
-            adjust_ctx (ContextInfo | None, optional): Additional context
-                information to be included in the event. Defaults to None.
-        """
-        event_info: EventInfo | None = None
-        for listener in self._listeners:
-            if not listener.capture_event(name):
-                continue
-            if event_info is None:
-                when = now()
-                ctx = get_preexc_ctx() if is_error_ctx else get_ctx()
-                if adjust_ctx is not None:
-                    ctx.update(adjust_ctx)
-                event = event_gen()
-                if event["name"] == "warning":
-                    if name in self._reported_warnings:
-                        return  # report a warning only once per instance
-                    self._reported_warnings.add(name)
-                event_info = {
-                    "when": when,
-                    "ctx": ctx,
-                    "name": name,
-                    "event": event,
-                }
-            listener.log_event(event_info)
+            text (str): The string to parse.
+
+        Raises:
+            ValueError: If the input is invalid.
+
+        Returns:
+            QualifiedName: The qualified name.
+        """
+        if NAME_SEP not in text:
+            raise ValueError(
+                f"{text} is not a qualified name: 'node:value'")
+        nname_str, vname = text.split(NAME_SEP, 1)
+        if not nname_str:
+            return QualifiedName(None, vname)
+        return QualifiedName(NName(nname_str), vname)
+
+    def __eq__(self, other: object) -> bool:
+        if other is self:
+            return True
+        if not isinstance(other, self.__class__):
+            return False
+        return self._nname == other._nname and self._vname == other._vname
+
+    def __ne__(self, other: object) -> bool:
+        return not self.__eq__(other)
+
+    def __hash__(self) -> int:
+        return hash((self._nname, self._vname))
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}[{self.to_parseable()}]"
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+
+ValueMap = dict[str, QualifiedName]
+"""A map of input value field names to output qualified names. This is used
+to connect inputs of a node to the correct outputs of previous nodes or an
+input of the current execution graph."""
```

### Comparing `scattermind-0.4.0/src/scattermind/system/payload/__init__.py` & `scattermind-0.4.1/src/scattermind/system/payload/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/payload/data.py` & `scattermind-0.4.1/src/scattermind/system/payload/data.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/payload/loader.py` & `scattermind-0.4.1/src/scattermind/system/payload/loader.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/payload/local.py` & `scattermind-0.4.1/src/scattermind/system/payload/local.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/payload/redis.py` & `scattermind-0.4.1/src/scattermind/system/payload/redis.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/payload/values.py` & `scattermind-0.4.1/src/scattermind/system/payload/values.py`

 * *Files 0% similar despite different names*

```diff
@@ -759,14 +759,18 @@
             missing_key = kexc.args[0]
             raise ValueError(
                 f"unexpected output name. expected '{missing_key}' but got "
                 f"{set(values.keys())} in {self.get_node()}") from kexc
         data_ids: list[DataContainer] = [{} for _ in tasks]
         byte_sizes: list[int] = [0 for _ in tasks]
         for key, cvalues in data.items():
+            if cvalues.row_count() != len(tasks):
+                raise ValueError(
+                    f"invalid row count for {key} "
+                    f"expected={len(tasks)} got={cvalues.row_count()}")
             qual = QualifiedName(node.get_name(), key)
             for ix, value in enumerate(cvalues.iter_values()):
                 data_ids[ix][qual] = store.store_tensor(value)
                 byte_sizes[ix] += data_format[key].byte_size(list(value.shape))
         add_weight = node.get_weight()
         next_qid = node.get_output_queue(qname_obj)
         for task, dids, byte_size in zip(tasks, data_ids, byte_sizes):
```

### Comparing `scattermind-0.4.0/src/scattermind/system/plugins.py` & `scattermind-0.4.1/src/scattermind/system/plugins.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/__init__.py` & `scattermind-0.4.1/src/scattermind/system/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/loader.py` & `scattermind-0.4.1/src/scattermind/system/queue/loader.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/local.py` & `scattermind-0.4.1/src/scattermind/system/queue/local.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/queue.py` & `scattermind-0.4.1/src/scattermind/system/queue/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     NodeStrategy,
     PICK_LEFT,
     PICK_RIGHT,
     QueueStrategy,
 )
 from scattermind.system.response import (
     TASK_STATUS_BUSY,
+    TASK_STATUS_DEFER,
     TASK_STATUS_ERROR,
     TASK_STATUS_READY,
     TASK_STATUS_WAIT,
     TaskStatus,
 )
 
 
@@ -874,40 +875,47 @@
                     "node": right_node.get_id(),
                     "node_name": right_node.get_name(),
                 })
             return left_node if pick_node == PICK_LEFT else right_node
 
         good_node: 'Node | None' = None
         for node in self.get_all_nodes():
+            # pylint: disable=try-except-raise
             if node == current_node:
                 continue
             try:
                 candidate_node = process_node(candidate_node, node)
                 good_node = candidate_node
+            except KeyboardInterrupt:
+                raise
             except Exception:  # pylint: disable=broad-except
                 print(
                     f"candidate={candidate_node.get_qualified_name(self)} "
                     f"other={node.get_qualified_name(self)} "
                     f"exception in strategy {traceback.format_exc()}")
                 if good_node is not None:
                     try:
                         process_node(good_node, node)
+                    except KeyboardInterrupt:
+                        raise
                     except Exception:  # pylint: disable=broad-except
                         print(
                             "bad node "
                             f"{node.get_qualified_name(self)} "
                             f"{traceback.format_exc()}")
                         # FIXME: log exception
                         # NOTE: node is faulty
                         return (
                             node,
                             current_node is None or node == current_node,
                         )
                     try:
                         process_node(good_node, candidate_node)
+                    except KeyboardInterrupt:
+                        raise
                     except Exception:  # pylint: disable=broad-except
                         print(
                             "bad node "
                             f"{candidate_node.get_qualified_name(self)} "
                             f"{traceback.format_exc()}")
                         # FIXME: log exception
                         # NOTE: candidate_node is faulty
@@ -984,23 +992,27 @@
                 other_cost_to_load=other_cost_to_load,
                 other_claimants=other_claimants,
                 other_loaded=other_loaded)
 
         try:
             if want_to_switch_to(candidate_node):
                 return (candidate_node, candidate_node != current_node)
+        except KeyboardInterrupt:  # pylint: disable=try-except-raise
+            raise
         except Exception:  # pylint: disable=broad-except
             print(
                 f"candidate={candidate_node.get_qualified_name(self)} "
                 f"current={current_node.get_qualified_name(self)} "
                 f"error trying to switch {traceback.format_exc()}")
             # FIXME: log exception
             try:
                 want_to_switch_to(good_node)
                 return (candidate_node, candidate_node != current_node)
+            except KeyboardInterrupt:  # pylint: disable=try-except-raise
+                raise
             except Exception:  # pylint: disable=broad-except
                 print(
                     f"current={current_node.get_qualified_name(self)} "
                     "candidate is bad "
                     f"{candidate_node.get_qualified_name(self)} "
                     f"{traceback.format_exc()}")
                 # FIXME: log exception
@@ -1030,51 +1042,56 @@
         return task_id
 
     def maybe_requeue_task_id(
             self,
             logger: EventStream,
             store: DataStore,
             task_id: TaskId,
-            error_info: ErrorInfo) -> None:
+            *,
+            error_info: ErrorInfo | None) -> None:
         """
         Enqueue a previously created task again to the overall input queue.
 
         Args:
             logger (EventStream): The logger.
             store (DataStore): The data store for storing the payload data.
             task_id (TaskId): The existing task id.
-            error_info (ErrorInfo): The error that triggered the requeue.
+            error_info (ErrorInfo | None): The error that triggered the
+                requeue. This can be None for deferred tasks.
 
         Raises:
             AssertionError: If the task is already / still in a queue.
         """
         cpool = self.get_client_pool()
-        cpool.set_error(task_id, error_info)
-        new_retries = cpool.inc_retries(task_id)
-        adj_ctx, retry_event = to_retry_event(error_info, new_retries)
-        logger.log_event("error.task", retry_event, adjust_ctx=adj_ctx)
+        if error_info is not None:
+            cpool.set_error(task_id, error_info)
+            new_retries = cpool.inc_retries(task_id)
+            adj_ctx, retry_event = to_retry_event(error_info, new_retries)
+            logger.log_event("error.task", retry_event, adjust_ctx=adj_ctx)
+        else:
+            # NOTE: we don't increase retries for deferred tasks
+            new_retries = 0
         if new_retries >= ClientPool.get_max_retries():
             cpool.set_duration(task_id)
             cpool.set_bulk_status([task_id], TASK_STATUS_ERROR)
         else:
-            if cpool.get_status(task_id) == TASK_STATUS_WAIT:
+            if cpool.get_task_status(task_id) == TASK_STATUS_WAIT:
                 mqid = self.maybe_get_queue(task_id)
                 if mqid is not None:
                     raise AssertionError(
                         f"{ctx_fmt()} {task_id} already waiting at {mqid}")
             cpool.clear_progress(task_id)
             if not self._enqueue_task_id(cpool, store, task_id):
                 logger.log_event(
                     "error.task",
                     {
                         "name": "ghost",
                         "message": "Cleaned up ghost task.",
                         "task": task_id,
-                    },
-                    adjust_ctx=adj_ctx)
+                    })
 
     def handle_task_result(
             self,
             logger: EventStream,
             store: DataStore,
             task: ComputeTask) -> None:
         """
@@ -1118,25 +1135,31 @@
                     for qual, _ in ret_data.items()
                 }
                 output_format = self.get_output_format(graph_id)
                 tvc_out = TaskValueContainer.extract_data(
                     store, output_format, ret_data, final_vmap)
                 if tvc_out is not None:
                     cache_id = cpool.pop_cache_id(task_id)
-                    if cache_id is not None:
-                        graph_cache.put_cached_output(cache_id, tvc_out)
                     cpool.set_final_output(task_id, tvc_out)
                     cpool.set_duration(task_id)
                     cpool.set_bulk_status([task_id], TASK_STATUS_READY)
+                    if cache_id is not None:
+                        graph_cache.put_cached_output(
+                            logger,
+                            store,
+                            self,
+                            cache_id=cache_id,
+                            output_data=tvc_out)
+                    cpool.notify_result(task_id)
                 else:
                     self.maybe_requeue_task_id(
                         logger,
                         store,
                         task_id,
-                        {
+                        error_info={
                             "ctx": get_ctx(),
                             "message": "result got purged from memory",
                             "code": "memory_purge",
                             "traceback": [],
                         })
             else:
                 cpool.commit_task(
@@ -1144,26 +1167,27 @@
                     ret_data,
                     weight=task.get_weight_out(),
                     byte_size=task.get_byte_size_out(),
                     push_frame=None)
         if not is_final:
             out_queue = self.get_queue(qid)
             out_queue.push_task_id(task_id)
+            cpool.notify_queues()
 
     def get_task_status(self, task_id: TaskId) -> TaskStatus:
         """
         Retrieve the status of the given task.
 
         Args:
             task_id (TaskId): The task id.
 
         Returns:
             TaskStatus: The status of the task.
         """
-        return self.get_client_pool().get_status(task_id)
+        return self.get_client_pool().get_task_status(task_id)
 
     def _enqueue_task_id(
             self,
             cpool: ClientPool,
             store: DataStore,
             task_id: TaskId) -> bool:
         """
@@ -1192,26 +1216,38 @@
         cache_id: CacheId | None = None
         if self.is_cached_graph(entry_graph_id):
             cache_id = graph_cache.get_cache_id(
                 entry_graph_id, input_format, original_input)
             output_format = self.get_output_format(entry_graph_id)
             result = graph_cache.get_cached_output(cache_id, output_format)
             if result is not None:
-                print(f"CACHE HIT {cache_id}")  # TODO: add logging
-                cpool.set_final_output(task_id, result)
-                cpool.set_duration(task_id)
-                cpool.set_bulk_status([task_id], TASK_STATUS_READY)
+                if isinstance(result, TaskValueContainer):
+                    tvc: TaskValueContainer = result
+                    print(f"CACHE HIT {cache_id}")  # TODO: add logging
+                    cpool.set_final_output(task_id, tvc)
+                    cpool.set_duration(task_id)
+                    cpool.set_bulk_status([task_id], TASK_STATUS_READY)
+                    cpool.notify_result(task_id)
+                    return True
+                print(f"CACHE DEFER {cache_id}")  # TODO: add logging
+                other_task_id: TaskId = result
+                cpool.init_data(store, task_id, input_format, original_input)
+                cpool.defer_task(task_id, other_task_id)
+                cpool.set_bulk_status([task_id], TASK_STATUS_DEFER)
+                graph_cache.add_listener(cache_id, task_id)
                 return True
             print(f"CACHE MISS {cache_id}")  # TODO: add logging
+            graph_cache.put_progress(cache_id, task_id)
         cpool.push_cache_id(task_id, cache_id)
         cpool.init_data(store, task_id, input_format, original_input)
+        cpool.set_bulk_status([task_id], TASK_STATUS_WAIT)
         node = self.get_input_node(entry_graph_id)
         qid = node.get_input_queue()
-        cpool.set_bulk_status([task_id], TASK_STATUS_WAIT)
         self.push_task_id(qid, task_id)
+        cpool.notify_queues()
         return True
 
     def get_compute_task(
             self,
             cpool: ClientPool,
             qid: QueueId,
             task_id: TaskId) -> ComputeTask:
```

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/redis.py` & `scattermind-0.4.1/src/scattermind/system/queue/redis.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/strategy/__init__.py` & `scattermind-0.4.1/src/scattermind/system/queue/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/strategy/loader.py` & `scattermind-0.4.1/src/scattermind/system/queue/strategy/loader.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/strategy/node/__init__.py` & `scattermind-0.4.1/src/scattermind/system/queue/strategy/node/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/strategy/node/dedicated.py` & `scattermind-0.4.1/src/scattermind/system/queue/strategy/node/dedicated.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/strategy/node/simple.py` & `scattermind-0.4.1/src/scattermind/system/queue/strategy/node/simple.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/strategy/queue/__init__.py` & `scattermind-0.4.1/src/scattermind/system/queue/strategy/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/strategy/queue/simple.py` & `scattermind-0.4.1/src/scattermind/system/queue/strategy/queue/simple.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/queue/strategy/strategy.py` & `scattermind-0.4.1/src/scattermind/system/queue/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/readonly/__init__.py` & `scattermind-0.4.1/src/scattermind/system/readonly/__init__.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/readonly/access.py` & `scattermind-0.4.1/src/scattermind/system/readonly/access.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/readonly/loader.py` & `scattermind-0.4.1/src/scattermind/system/readonly/loader.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/readonly/writer.py` & `scattermind-0.4.1/src/scattermind/system/readonly/writer.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/redis_util.py` & `scattermind-0.4.1/src/scattermind/system/redis_util.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/response.py` & `scattermind-0.4.1/src/scattermind/system/response.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 TaskStatus = Literal[
     "init",
     "wait",
     "busy",
     "ready",
     "done",
+    "deferred",
     "error",
     "unknown",
 ]
 """The status of the task."""
 TASK_STATUS_ALL: set[TaskStatus] = set(get_args(TaskStatus))
 """All valid task status values."""
 TASK_STATUS_INIT: TaskStatus = "init"
@@ -40,20 +41,31 @@
 """The task is waiting to continue computation."""
 TASK_STATUS_BUSY: TaskStatus = "busy"
 """The task is busy computing."""
 TASK_STATUS_READY: TaskStatus = "ready"
 """The results of the task are ready to be read."""
 TASK_STATUS_DONE: TaskStatus = "done"
 """The results have been read and the task can be cleaned up."""
+TASK_STATUS_DEFER: TaskStatus = "deferred"
+"""The task is computed by a different task via caching."""
 TASK_STATUS_ERROR: TaskStatus = "error"
 """An error occured while executing the task."""
 TASK_STATUS_UNKNOWN: TaskStatus = "unknown"
 """The status of the task is unknown. The task might not exist."""
 
 
+TASK_COMPLETE: set[TaskStatus] = {
+    TASK_STATUS_READY,
+    TASK_STATUS_DONE,
+    TASK_STATUS_ERROR,
+    TASK_STATUS_UNKNOWN,
+}
+"""The task has either finished, had an error, or is not known."""
+
+
 def to_status(text: str) -> TaskStatus:
     """
     Converts a string into a task status.
 
     Args:
         text (str): The string.
```

### Comparing `scattermind-0.4.0/src/scattermind/system/torch_util.py` & `scattermind-0.4.1/src/scattermind/system/torch_util.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/src/scattermind/system/util.py` & `scattermind-0.4.1/src/scattermind/system/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,29 @@
 
     Returns:
         list[int]: The converted list.
     """
     return [int(elem) for elem in arr]
 
 
+def as_str_list(arr: list[str]) -> list[str]:
+    """
+    Converts all elements of the given list to strings. This is useful for
+    processing outside data where we cannot trust that the items in the list
+    are actually strings.
+
+    Args:
+        arr (list[str]): The list to convert.
+
+    Returns:
+        list[str]: The converted list.
+    """
+    return [f"{elem}" for elem in arr]
+
+
 def as_shape(arr: Sequence[int | None]) -> list[int | None]:
     """
     Converts a sequence into a variable shape. The shape is a list of integers
     where the first element indicates the size of the first dimension etc. The
     shape is variable meaning it can have None values leaving the general size
     of that dimension unspecified until it is used on a concrete instance.
```

### Comparing `scattermind-0.4.0/src/scattermind.egg-info/PKG-INFO` & `scattermind-0.4.1/src/scattermind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scattermind
-Version: 0.4.0
+Version: 0.4.1
 Summary: A decentralized and distributed horizontally scalable model execution framework.
 Author-email: Josua Krause <josua.krause@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,15 +214,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mypy>=1.5.1
 Requires-Dist: numpy>=1.25.2
 Requires-Dist: quick-server>=0.9.0
-Requires-Dist: redipy>=0.6.0
+Requires-Dist: redipy>=0.7.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: torch>=2.0.0
 Provides-Extra: test
 Requires-Dist: flake8-commas>=2.1.0; extra == "test"
 Requires-Dist: flake8-isort>=6.1.1; extra == "test"
 Requires-Dist: flake8>=5.0.4; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
```

### Comparing `scattermind-0.4.0/src/scattermind.egg-info/SOURCES.txt` & `scattermind-0.4.1/src/scattermind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/test/test_assert.py` & `scattermind-0.4.1/test/test_assert.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,15 @@
     set_debug_output_length(7)
     config = load_test(
         batch_size=batch_size, parallelism=parallelism, is_redis=is_redis)
     ns = config.load_graph({
         "graphs": [
             {
                 "name": "main",
-                "description":
-                    f"batch_size={batch_size};parallelism={parallelism}",
+                "description": f"{batch_size=};{parallelism=}",
                 "input": "node_0",
                 "input_format": {
                     "value": ("bool", [1]),
                 },
                 "output_format": {
                     "value": ("bool", [1]),
                 },
@@ -103,15 +102,15 @@
             tix % 3 > 0,
         )
         for tix in range(20)
     ]
     for task_id, _ in tasks:
         assert config.get_status(task_id) == TASK_STATUS_WAIT
     try:
-        config.run(force_no_block=True)
+        config.run(force_no_block=True, no_reclaim=True)
         for task_id, response, expected_result in wait_for_tasks(
                 config, tasks):
             real_duration = time.monotonic() - time_start
             status = response["status"]
             task_ns = response["ns"]
             task_duration = response["duration"]
             result = response["result"]
@@ -151,15 +150,15 @@
             config.clear_task(task_id)
             assert config.get_namespace(task_id) is None
             assert config.get_status(task_id) == TASK_STATUS_UNKNOWN
             assert config.get_result(task_id) is None
     finally:
         print("TEST TEARDOWN!")
         emng = config.get_executor_manager()
-        emng.release_all(timeout=0.1)
+        emng.release_all(config.get_client_pool(), timeout=0.5)
         if emng.any_active():
             raise ValueError("threads did not shut down in time")
 
 
 @pytest.mark.parametrize("base", [[[1.0]], [[1.0, 2.0], [3.0, 4.0]]])
 @pytest.mark.parametrize("batch_size", [1, 3, 5, 12, 30])
 @pytest.mark.parametrize("is_redis", [False, True])
@@ -233,15 +232,16 @@
     for task_id, _ in tasks[::2]:
         config.clear_task(task_id)  # NOTE: prematurely clean tasks
         assert config.get_namespace(task_id) is None
         assert config.get_status(task_id) == TASK_STATUS_UNKNOWN
         assert config.get_result(task_id) is None
         bad_tasks.add(task_id)
     try:
-        config.run(force_no_block=False)  # NOTE: we only use single here
+        # NOTE: we only use single here
+        config.run(force_no_block=False, no_reclaim=True)
         for task_id, response, expected_result in wait_for_tasks(
                 config, tasks):
             if task_id in bad_tasks:
                 assert response["status"] == TASK_STATUS_UNKNOWN
                 assert config.get_namespace(task_id) is None
                 assert config.get_status(task_id) == TASK_STATUS_UNKNOWN
                 assert config.get_result(task_id) is None
@@ -262,10 +262,10 @@
             config.clear_task(task_id)
             assert config.get_namespace(task_id) is None
             assert config.get_status(task_id) == TASK_STATUS_UNKNOWN
             assert config.get_result(task_id) is None
     finally:
         print("TEST TEARDOWN!")
         emng = config.get_executor_manager()
-        emng.release_all(timeout=0.1)
+        emng.release_all(config.get_client_pool(), timeout=0.5)
         if emng.any_active():
             raise ValueError("threads did not shut down in time")
```

### Comparing `scattermind-0.4.0/test/test_cache.py` & `scattermind-0.4.1/test/test_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,46 +28,50 @@
     TASK_STATUS_READY,
     TASK_STATUS_UNKNOWN,
 )
 from scattermind.system.torch_util import str_to_tensor, tensor_to_str
 from scattermind.system.util import get_short_hash
 
 
+@pytest.mark.parametrize("batch_size", [1, 3, 6, 7, 13, 14, 20])
 @pytest.mark.parametrize("parallelism", [1, 2, 4, -1])
 @pytest.mark.parametrize("is_redis", [False, True])
 @pytest.mark.parametrize("is_cache", [False, True])
 @pytest.mark.parametrize("cache_main", [False, True])
 @pytest.mark.parametrize("cache_mid", [False])  # FIXME: enable when ready
 @pytest.mark.parametrize("cache_top", [False])  # FIXME: enable when ready
 def test_graph_cache(
+        batch_size: int,
         parallelism: int,
         is_redis: bool,
         is_cache: bool,
         cache_main: bool,
         cache_mid: bool,
         cache_top: bool) -> None:
     """
     Test for graph caching.
 
     Args:
+        batch_size (int): The batch size.
         parallelism (int): The parallelism. Cannot use single executor since
             it terminates upon completion.
         is_redis (bool): Whether to use redis.
         is_cache (bool): Whether to cache at all.
         cache_main (bool): Whether to cache the main graph.
         cache_mid (bool): Whether to cache the mid graph.
         cache_top (bool): Whether to cache the top graph.
     """
-    # NOTE: batch_size can only be one to guarantee caching comes into effect
     set_debug_output_length(7)
     config = load_test(
+        batch_size=batch_size,
         parallelism=parallelism,
         is_redis=is_redis,
         no_cache=not is_cache)
     desc = (
+        f"batch_size={batch_size};"
         f"parallelism={parallelism};"
         f"is_redis={is_redis};"
         f"is_cache={is_cache}")
     seed = get_short_hash(desc)
     ns = config.load_graph({
         "graphs": [
             {
@@ -385,15 +389,15 @@
         val_mid = mid_expected((val_1, val_2))
         val = f"{val_0}-{val_mid}"
         if is_cache and cache_main:
             cache_main_obj[input_tup] = val
         return val
 
     try:
-        config.run(force_no_block=True)
+        config.run(force_no_block=True, no_reclaim=True)
         print(
             f"SETTING: is_cache={is_cache} cache_main={cache_main} "
             f"cache_mid={cache_mid} cache_top={cache_top}")
         for cur_input in inputs:
             expected = compute_expected(cur_input)
             print(f"EXECUTING TASK: {cur_input} with {expected}")
             task_id = config.enqueue(
@@ -426,10 +430,10 @@
             config.clear_task(task_id)
             assert config.get_namespace(task_id) is None
             assert config.get_status(task_id) == TASK_STATUS_UNKNOWN
             assert config.get_result(task_id) is None
     finally:
         print("TEST TEARDOWN!")
         emng = config.get_executor_manager()
-        emng.release_all(timeout=0.1)
+        emng.release_all(config.get_client_pool(), timeout=0.5)
         if emng.any_active():
             raise ValueError("threads did not shut down in time")
```

### Comparing `scattermind-0.4.0/test/test_call.py` & `scattermind-0.4.1/test/test_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,15 @@
             ]),
         )
         for tix in range(20)
     ]
     for task_id, _ in tasks:
         assert config.get_status(task_id) == TASK_STATUS_WAIT
     try:
-        config.run(force_no_block=True)
+        config.run(force_no_block=True, no_reclaim=True)
         for task_id, response, expected_result in wait_for_tasks(
                 config, tasks):
             response_ok(response, no_warn=True)
             real_duration = time.monotonic() - time_start
             status = response["status"]
             task_ns = response["ns"]
             result = response["result"]
@@ -241,10 +241,10 @@
             assert config.get_status(task_id) == TASK_STATUS_DONE
             config.clear_task(task_id)
             assert config.get_namespace(task_id) is None
             assert config.get_status(task_id) == TASK_STATUS_UNKNOWN
             assert config.get_result(task_id) is None
     finally:
         emng = config.get_executor_manager()
-        emng.release_all(timeout=0.1)
+        emng.release_all(config.get_client_pool(), timeout=0.5)
         if emng.any_active():
             raise ValueError("threads did not shut down in time")
```

### Comparing `scattermind-0.4.0/test/test_cop.py` & `scattermind-0.4.1/test/test_cop.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,16 @@
                 }),
             np.array(base) * tix * 2.0,
         )
         for tix in range(20)
     ]
     for task_id, _ in tasks:
         assert config.get_status(task_id) == TASK_STATUS_WAIT
-    config.run(force_no_block=False)  # NOTE: we only use single here
+    # NOTE: we only use single here
+    config.run(force_no_block=False, no_reclaim=True)
     for task_id, expected_result in tasks:
         response = config.get_response(task_id)
         response_ok(response, no_warn=True)
         assert response["status"] == TASK_STATUS_READY
         assert response["ns"] == ns
         result = response["result"]
         assert result is not None
@@ -124,15 +125,15 @@
     """
     shape = [len(base), len(base[0])]
     config = load_test(batch_size=batch_size, is_redis=is_redis)
     ns = config.load_graph({
         "graphs": [
             {
                 "name": "copchain",
-                "description": f"batch_size={batch_size},base={base}",
+                "description": f"{batch_size=},{base=}",
                 "input": "node_0",
                 "input_format": {
                     "value": ("float", shape),
                 },
                 "output_format": {
                     "value": ("float", shape),
                 },
@@ -185,15 +186,16 @@
                 }),
             np.array(base) * tix * 2.0 + 1.0,
         )
         for tix in range(20)
     ]
     for task_id, _ in tasks:
         assert config.get_status(task_id) == TASK_STATUS_WAIT
-    config.run(force_no_block=False)  # NOTE: we only use single here
+    # NOTE: we only use single here
+    config.run(force_no_block=False, no_reclaim=True)
     for task_id, expected_result in tasks:
         response = config.get_response(task_id)
         response_ok(response, no_warn=True)
         assert response["status"] == TASK_STATUS_READY
         assert response["ns"] == ns
         result = response["result"]
         assert result is not None
```

### Comparing `scattermind-0.4.0/test/test_dtype.py` & `scattermind-0.4.1/test/test_dtype.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/test/test_invalid.py` & `scattermind-0.4.1/test/test_invalid.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/test/test_lowmem.py` & `scattermind-0.4.1/test/test_lowmem.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     shape = [len(base), len(base[0])]
     config = load_test(
         batch_size=batch_size, max_store_size=200, is_redis=False)
     ns = config.load_graph({
         "graphs": [
             {
                 "name": "lowmem",
-                "description": f"batch_size={batch_size},base={base}",
+                "description": f"{batch_size=},{base=}",
                 "input": "node_0",
                 "input_format": {
                     "value": ("float", shape),
                 },
                 "output_format": {
                     "value": ("float", shape),
                 },
@@ -108,15 +108,16 @@
                 }),
             np.array(base) * tix * 2.0 + 1.0,
         )
         for tix in range(20)
     ]
     for task_id, _ in tasks:
         assert config.get_status(task_id) == TASK_STATUS_WAIT
-    config.run(force_no_block=False)  # NOTE: we only use single here
+    # NOTE: we only use single here
+    config.run(force_no_block=False, no_reclaim=True)
     has_error = batch_size >= 3 if len(base) < 2 else batch_size >= 2
     is_variable = (batch_size, len(base)) in (
         (2, 2),
         (3, 1),
         (3, 2),
         (10, 1),
         (10, 2),
```

### Comparing `scattermind-0.4.0/test/test_ns.py` & `scattermind-0.4.1/test/test_ns.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         is_redis (bool): Whether to use redis.
     """
     config = load_test(batch_size=batch_size, is_redis=is_redis)
     ns_1 = config.load_graph({
         "graphs": [
             {
                 "name": "main",
-                "description": f"batch_size={batch_size}",
+                "description": f"{batch_size=}",
                 "input": "node",
                 "input_format": {
                     "value": ("float", [1]),
                 },
                 "output_format": {
                     "value": ("float", [1]),
                 },
@@ -76,15 +76,15 @@
         "entry": "main",
         "ns": "graph_1",
     })
     ns_2 = config.load_graph({
         "graphs": [
             {
                 "name": "main",
-                "description": f"batch_size={batch_size}",
+                "description": f"{batch_size=}",
                 "input": "node",
                 "input_format": {
                     "value": ("float", [1]),
                 },
                 "output_format": {
                     "value": ("float", [1]),
                 },
@@ -126,15 +126,16 @@
             GNamespace(f"graph_{gix}"),
         )
         for gix in [1, 2]
         for tix in range(20)
     ]
     for task_id, _, _ in tasks:
         assert config.get_status(task_id) == TASK_STATUS_WAIT
-    config.run(force_no_block=False)  # NOTE: we only use single here
+    # NOTE: we only use single here
+    config.run(force_no_block=False, no_reclaim=True)
     for task_id, expected_result, ns in tasks:
         response = config.get_response(task_id)
         response_ok(response, no_warn=True)
         assert response["status"] == TASK_STATUS_READY
         assert response["ns"] == ns
         result = response["result"]
         assert result is not None
```

### Comparing `scattermind-0.4.0/test/test_plugins.py` & `scattermind-0.4.1/test/test_plugins.py`

 * *Files identical despite different names*

### Comparing `scattermind-0.4.0/test/test_util.py` & `scattermind-0.4.1/test/test_util.py`

 * *Files identical despite different names*

