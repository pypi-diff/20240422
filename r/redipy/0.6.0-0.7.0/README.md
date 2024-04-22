# Comparing `tmp/redipy-0.6.0.tar.gz` & `tmp/redipy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redipy-0.6.0.tar", last modified: Wed Mar 27 22:37:14 2024, max compression
+gzip compressed data, was "redipy-0.7.0.tar", last modified: Mon Apr 22 02:41:43 2024, max compression
```

## Comparing `redipy-0.6.0.tar` & `redipy-0.7.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 22:37:14.184934 redipy-0.6.0/
--rw-r--r--   0 krause     (501) staff       (20)     1821 2024-03-27 22:36:53.000000 redipy-0.6.0/CHANGELOG.md
--rw-r--r--   0 krause     (501) staff       (20)    11357 2023-10-15 03:56:22.000000 redipy-0.6.0/LICENSE
--rw-r--r--   0 krause     (501) staff       (20)      106 2023-11-19 05:15:48.000000 redipy-0.6.0/MANIFEST.in
--rw-r--r--   0 krause     (501) staff       (20)    33555 2024-03-27 22:37:14.184685 redipy-0.6.0/PKG-INFO
--rw-r--r--   0 krause     (501) staff       (20)    19140 2024-03-27 22:36:53.000000 redipy-0.6.0/README.md
--rw-r--r--   0 krause     (501) staff       (20)     4615 2024-03-27 22:36:53.000000 redipy-0.6.0/pyproject.toml
--rw-r--r--   0 krause     (501) staff       (20)      138 2023-10-15 03:56:22.000000 redipy-0.6.0/requirements.dev.txt
--rw-r--r--   0 krause     (501) staff       (20)       88 2023-10-15 03:56:22.000000 redipy-0.6.0/requirements.txt
--rw-r--r--   0 krause     (501) staff       (20)       38 2024-03-27 22:37:14.184976 redipy-0.6.0/setup.cfg
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 22:37:14.171321 redipy-0.6.0/src/
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 22:37:14.174014 redipy-0.6.0/src/redipy/
--rw-r--r--   0 krause     (501) staff       (20)     3127 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)    47393 2024-03-27 22:36:53.000000 redipy-0.6.0/src/redipy/api.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 22:37:14.175652 redipy-0.6.0/src/redipy/backend/
--rw-r--r--   0 krause     (501) staff       (20)      652 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/backend/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     5158 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/backend/backend.py
--rw-r--r--   0 krause     (501) staff       (20)     3681 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/backend/runtime.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 22:37:14.176706 redipy-0.6.0/src/redipy/graph/
--rw-r--r--   0 krause     (501) staff       (20)      871 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/graph/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     2555 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/graph/cmd.py
--rw-r--r--   0 krause     (501) staff       (20)     5951 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/graph/expr.py
--rw-r--r--   0 krause     (501) staff       (20)     1368 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/graph/seq.py
--rw-r--r--   0 krause     (501) staff       (20)    15243 2024-03-27 22:36:53.000000 redipy-0.6.0/src/redipy/main.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 22:37:14.178099 redipy-0.6.0/src/redipy/memory/
--rw-r--r--   0 krause     (501) staff       (20)      610 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/memory/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)     4635 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/memory/gfun.py
--rw-r--r--   0 krause     (501) staff       (20)    20949 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/memory/local.py
--rw-r--r--   0 krause     (501) staff       (20)    13855 2024-03-27 22:36:53.000000 redipy-0.6.0/src/redipy/memory/rfun.py
--rw-r--r--   0 krause     (501) staff       (20)    21959 2024-03-27 22:36:53.000000 redipy-0.6.0/src/redipy/memory/rt.py
--rw-r--r--   0 krause     (501) staff       (20)    51220 2024-03-27 22:36:53.000000 redipy-0.6.0/src/redipy/memory/state.py
--rw-r--r--   0 krause     (501) staff       (20)     8811 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/plugin.py
--rw-r--r--   0 krause     (501) staff       (20)        0 2023-10-15 03:56:22.000000 redipy-0.6.0/src/redipy/py.typed
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 22:37:14.179166 redipy-0.6.0/src/redipy/redis/
--rw-r--r--   0 krause     (501) staff       (20)      609 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/redis/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)    37758 2024-03-27 22:36:53.000000 redipy-0.6.0/src/redipy/redis/conn.py
--rw-r--r--   0 krause     (501) staff       (20)     1720 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/redis/gpatch.py
--rw-r--r--   0 krause     (501) staff       (20)     3209 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/redis/helpers.py
--rw-r--r--   0 krause     (501) staff       (20)    19329 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/redis/lua.py
--rw-r--r--   0 krause     (501) staff       (20)     6118 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/redis/rpatch.py
--rw-r--r--   0 krause     (501) staff       (20)     1796 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/script.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 22:37:14.180922 redipy-0.6.0/src/redipy/symbolic/
--rw-r--r--   0 krause     (501) staff       (20)      641 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/symbolic/__init__.py
--rw-r--r--   0 krause     (501) staff       (20)    10515 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/symbolic/core.py
--rw-r--r--   0 krause     (501) staff       (20)    12115 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/symbolic/expr.py
--rw-r--r--   0 krause     (501) staff       (20)     8814 2024-03-27 22:36:53.000000 redipy-0.6.0/src/redipy/symbolic/fun.py
--rw-r--r--   0 krause     (501) staff       (20)     2912 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/symbolic/rhash.py
--rw-r--r--   0 krause     (501) staff       (20)     3394 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/symbolic/rlist.py
--rw-r--r--   0 krause     (501) staff       (20)     1958 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/symbolic/rset.py
--rw-r--r--   0 krause     (501) staff       (20)     3106 2024-03-27 22:36:53.000000 redipy-0.6.0/src/redipy/symbolic/rvar.py
--rw-r--r--   0 krause     (501) staff       (20)     2556 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/symbolic/rzset.py
--rw-r--r--   0 krause     (501) staff       (20)    11688 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/symbolic/seq.py
--rw-r--r--   0 krause     (501) staff       (20)    28443 2024-03-07 04:28:39.000000 redipy-0.6.0/src/redipy/util.py
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 22:37:14.183963 redipy-0.6.0/src/redipy.egg-info/
--rw-r--r--   0 krause     (501) staff       (20)    33555 2024-03-27 22:37:14.000000 redipy-0.6.0/src/redipy.egg-info/PKG-INFO
--rw-r--r--   0 krause     (501) staff       (20)     1462 2024-03-27 22:37:14.000000 redipy-0.6.0/src/redipy.egg-info/SOURCES.txt
--rw-r--r--   0 krause     (501) staff       (20)        1 2024-03-27 22:37:14.000000 redipy-0.6.0/src/redipy.egg-info/dependency_links.txt
--rw-r--r--   0 krause     (501) staff       (20)      234 2024-03-27 22:37:14.000000 redipy-0.6.0/src/redipy.egg-info/requires.txt
--rw-r--r--   0 krause     (501) staff       (20)        7 2024-03-27 22:37:14.000000 redipy-0.6.0/src/redipy.egg-info/top_level.txt
-drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-03-27 22:37:14.183599 redipy-0.6.0/test/
--rw-r--r--   0 krause     (501) staff       (20)    19005 2024-03-27 22:36:53.000000 redipy-0.6.0/test/test_api.py
--rw-r--r--   0 krause     (501) staff       (20)     4571 2024-03-07 04:28:39.000000 redipy-0.6.0/test/test_err.py
--rw-r--r--   0 krause     (501) staff       (20)    14276 2024-03-27 22:36:53.000000 redipy-0.6.0/test/test_expire.py
--rw-r--r--   0 krause     (501) staff       (20)    14530 2024-03-27 22:36:53.000000 redipy-0.6.0/test/test_keys.py
--rw-r--r--   0 krause     (501) staff       (20)     6437 2024-03-27 22:36:53.000000 redipy-0.6.0/test/test_misc.py
--rw-r--r--   0 krause     (501) staff       (20)     4860 2024-03-27 22:36:53.000000 redipy-0.6.0/test/test_pipe.py
--rw-r--r--   0 krause     (501) staff       (20)     3823 2024-03-27 22:36:53.000000 redipy-0.6.0/test/test_rlist.py
--rw-r--r--   0 krause     (501) staff       (20)     6732 2024-03-07 04:28:39.000000 redipy-0.6.0/test/test_rset.py
--rw-r--r--   0 krause     (501) staff       (20)     8672 2024-03-27 22:36:53.000000 redipy-0.6.0/test/test_rvar.py
--rw-r--r--   0 krause     (501) staff       (20)     4517 2024-03-07 04:28:39.000000 redipy-0.6.0/test/test_rzset.py
--rw-r--r--   0 krause     (501) staff       (20)     8028 2024-03-27 22:36:53.000000 redipy-0.6.0/test/test_sanity.py
--rw-r--r--   0 krause     (501) staff       (20)     2480 2024-03-07 04:28:39.000000 redipy-0.6.0/test/test_simple.py
--rw-r--r--   0 krause     (501) staff       (20)    16010 2024-03-27 22:36:53.000000 redipy-0.6.0/test/test_stack.py
--rw-r--r--   0 krause     (501) staff       (20)     8097 2024-03-07 04:28:39.000000 redipy-0.6.0/test/test_util.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 02:41:43.988173 redipy-0.7.0/
+-rw-r--r--   0 krause     (501) staff       (20)     1957 2024-04-22 02:38:47.000000 redipy-0.7.0/CHANGELOG.md
+-rw-r--r--   0 krause     (501) staff       (20)    11357 2023-10-15 03:56:22.000000 redipy-0.7.0/LICENSE
+-rw-r--r--   0 krause     (501) staff       (20)      106 2023-11-19 05:15:48.000000 redipy-0.7.0/MANIFEST.in
+-rw-r--r--   0 krause     (501) staff       (20)    33478 2024-04-22 02:41:43.987946 redipy-0.7.0/PKG-INFO
+-rw-r--r--   0 krause     (501) staff       (20)    19063 2024-04-22 02:38:47.000000 redipy-0.7.0/README.md
+-rw-r--r--   0 krause     (501) staff       (20)     4615 2024-04-22 02:38:47.000000 redipy-0.7.0/pyproject.toml
+-rw-r--r--   0 krause     (501) staff       (20)      138 2023-10-15 03:56:22.000000 redipy-0.7.0/requirements.dev.txt
+-rw-r--r--   0 krause     (501) staff       (20)       88 2023-10-15 03:56:22.000000 redipy-0.7.0/requirements.txt
+-rw-r--r--   0 krause     (501) staff       (20)       38 2024-04-22 02:41:43.988210 redipy-0.7.0/setup.cfg
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 02:41:43.968537 redipy-0.7.0/src/
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 02:41:43.973314 redipy-0.7.0/src/redipy/
+-rw-r--r--   0 krause     (501) staff       (20)     3127 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)    48887 2024-04-22 02:38:47.000000 redipy-0.7.0/src/redipy/api.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 02:41:43.975457 redipy-0.7.0/src/redipy/backend/
+-rw-r--r--   0 krause     (501) staff       (20)      652 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/backend/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     5158 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/backend/backend.py
+-rw-r--r--   0 krause     (501) staff       (20)     3681 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/backend/runtime.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 02:41:43.976562 redipy-0.7.0/src/redipy/graph/
+-rw-r--r--   0 krause     (501) staff       (20)      871 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/graph/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     2555 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/graph/cmd.py
+-rw-r--r--   0 krause     (501) staff       (20)     5951 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/graph/expr.py
+-rw-r--r--   0 krause     (501) staff       (20)     1368 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/graph/seq.py
+-rw-r--r--   0 krause     (501) staff       (20)    15570 2024-04-22 02:38:47.000000 redipy-0.7.0/src/redipy/main.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 02:41:43.978272 redipy-0.7.0/src/redipy/memory/
+-rw-r--r--   0 krause     (501) staff       (20)      610 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/memory/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)     4635 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/memory/gfun.py
+-rw-r--r--   0 krause     (501) staff       (20)    20949 2024-04-22 02:17:57.000000 redipy-0.7.0/src/redipy/memory/local.py
+-rw-r--r--   0 krause     (501) staff       (20)    13855 2024-04-22 02:18:00.000000 redipy-0.7.0/src/redipy/memory/rfun.py
+-rw-r--r--   0 krause     (501) staff       (20)    22318 2024-04-22 02:38:47.000000 redipy-0.7.0/src/redipy/memory/rt.py
+-rw-r--r--   0 krause     (501) staff       (20)    52183 2024-04-22 02:38:47.000000 redipy-0.7.0/src/redipy/memory/state.py
+-rw-r--r--   0 krause     (501) staff       (20)     8811 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/plugin.py
+-rw-r--r--   0 krause     (501) staff       (20)        0 2023-10-15 03:56:22.000000 redipy-0.7.0/src/redipy/py.typed
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 02:41:43.980100 redipy-0.7.0/src/redipy/redis/
+-rw-r--r--   0 krause     (501) staff       (20)      609 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/redis/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)    38110 2024-04-22 02:38:47.000000 redipy-0.7.0/src/redipy/redis/conn.py
+-rw-r--r--   0 krause     (501) staff       (20)     1720 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/redis/gpatch.py
+-rw-r--r--   0 krause     (501) staff       (20)     3209 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/redis/helpers.py
+-rw-r--r--   0 krause     (501) staff       (20)    19329 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/redis/lua.py
+-rw-r--r--   0 krause     (501) staff       (20)     6118 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/redis/rpatch.py
+-rw-r--r--   0 krause     (501) staff       (20)     1796 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/script.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 02:41:43.982720 redipy-0.7.0/src/redipy/symbolic/
+-rw-r--r--   0 krause     (501) staff       (20)      641 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/symbolic/__init__.py
+-rw-r--r--   0 krause     (501) staff       (20)    10515 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/symbolic/core.py
+-rw-r--r--   0 krause     (501) staff       (20)    12115 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/symbolic/expr.py
+-rw-r--r--   0 krause     (501) staff       (20)     8814 2024-03-27 22:36:53.000000 redipy-0.7.0/src/redipy/symbolic/fun.py
+-rw-r--r--   0 krause     (501) staff       (20)     2912 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/symbolic/rhash.py
+-rw-r--r--   0 krause     (501) staff       (20)     3394 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/symbolic/rlist.py
+-rw-r--r--   0 krause     (501) staff       (20)     1958 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/symbolic/rset.py
+-rw-r--r--   0 krause     (501) staff       (20)     3106 2024-03-27 22:36:53.000000 redipy-0.7.0/src/redipy/symbolic/rvar.py
+-rw-r--r--   0 krause     (501) staff       (20)     2556 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/symbolic/rzset.py
+-rw-r--r--   0 krause     (501) staff       (20)    11688 2024-03-07 04:28:39.000000 redipy-0.7.0/src/redipy/symbolic/seq.py
+-rw-r--r--   0 krause     (501) staff       (20)    28872 2024-04-22 02:38:47.000000 redipy-0.7.0/src/redipy/util.py
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 02:41:43.987309 redipy-0.7.0/src/redipy.egg-info/
+-rw-r--r--   0 krause     (501) staff       (20)    33478 2024-04-22 02:41:43.000000 redipy-0.7.0/src/redipy.egg-info/PKG-INFO
+-rw-r--r--   0 krause     (501) staff       (20)     1462 2024-04-22 02:41:43.000000 redipy-0.7.0/src/redipy.egg-info/SOURCES.txt
+-rw-r--r--   0 krause     (501) staff       (20)        1 2024-04-22 02:41:43.000000 redipy-0.7.0/src/redipy.egg-info/dependency_links.txt
+-rw-r--r--   0 krause     (501) staff       (20)      234 2024-04-22 02:41:43.000000 redipy-0.7.0/src/redipy.egg-info/requires.txt
+-rw-r--r--   0 krause     (501) staff       (20)        7 2024-04-22 02:41:43.000000 redipy-0.7.0/src/redipy.egg-info/top_level.txt
+drwxr-xr-x   0 krause     (501) staff       (20)        0 2024-04-22 02:41:43.986978 redipy-0.7.0/test/
+-rw-r--r--   0 krause     (501) staff       (20)    19005 2024-03-27 22:36:53.000000 redipy-0.7.0/test/test_api.py
+-rw-r--r--   0 krause     (501) staff       (20)     4571 2024-03-07 04:28:39.000000 redipy-0.7.0/test/test_err.py
+-rw-r--r--   0 krause     (501) staff       (20)    14276 2024-03-27 22:36:53.000000 redipy-0.7.0/test/test_expire.py
+-rw-r--r--   0 krause     (501) staff       (20)    14530 2024-03-27 22:36:53.000000 redipy-0.7.0/test/test_keys.py
+-rw-r--r--   0 krause     (501) staff       (20)     6437 2024-03-27 22:36:53.000000 redipy-0.7.0/test/test_misc.py
+-rw-r--r--   0 krause     (501) staff       (20)     4860 2024-03-27 22:36:53.000000 redipy-0.7.0/test/test_pipe.py
+-rw-r--r--   0 krause     (501) staff       (20)     3823 2024-03-27 22:36:53.000000 redipy-0.7.0/test/test_rlist.py
+-rw-r--r--   0 krause     (501) staff       (20)     6732 2024-03-07 04:28:39.000000 redipy-0.7.0/test/test_rset.py
+-rw-r--r--   0 krause     (501) staff       (20)     8672 2024-03-27 22:36:53.000000 redipy-0.7.0/test/test_rvar.py
+-rw-r--r--   0 krause     (501) staff       (20)     4517 2024-03-07 04:28:39.000000 redipy-0.7.0/test/test_rzset.py
+-rw-r--r--   0 krause     (501) staff       (20)     8028 2024-03-27 22:36:53.000000 redipy-0.7.0/test/test_sanity.py
+-rw-r--r--   0 krause     (501) staff       (20)     2480 2024-03-07 04:28:39.000000 redipy-0.7.0/test/test_simple.py
+-rw-r--r--   0 krause     (501) staff       (20)    16010 2024-03-27 22:36:53.000000 redipy-0.7.0/test/test_stack.py
+-rw-r--r--   0 krause     (501) staff       (20)     8097 2024-03-07 04:28:39.000000 redipy-0.7.0/test/test_util.py
```

### Comparing `redipy-0.6.0/CHANGELOG.md` & `redipy-0.7.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## [0.7.0] - 2024-04-21
+
+### Added
+
+- Partial support for pubsub channels ([#18])
+
 ## [0.6.0] - 2024-03-27
 
 ### Breaking
 
 - Removed `set` and `get` ([#17])
 
 ### Added
@@ -68,7 +74,8 @@
 
 - Removed some usage of `nil` in lua scripts (in favor of `cjson.null`). ([#3])
 
 [#3]: https://github.com/JosuaKrause/redipy/pull/3
 [#7]: https://github.com/JosuaKrause/redipy/pull/7
 [#15]: https://github.com/JosuaKrause/redipy/pull/15
 [#17]: https://github.com/JosuaKrause/redipy/pull/17
+[#18]: https://github.com/JosuaKrause/redipy/pull/18
```

### Comparing `redipy-0.6.0/LICENSE` & `redipy-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/PKG-INFO` & `redipy-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redipy
-Version: 0.6.0
+Version: 0.7.0
 Summary: redipy is a uniform interface to Redis-like storage systems. It allows you to use the same Redis API with different backends that implement the same functionality.
 Author-email: Josua Krause <josua.krause@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -264,21 +264,16 @@
 8. [License](#license)
 9. [Feedback](#feedback)
 
 </details>
 
 This [medium article][medium] explores some of the rationale behind the library.
 
-### Warning
-
-This library is still early in development and [not all Redis functions are
-available yet][implemented]!
 If you need certain functionality or found a bug, have a look at the
 [contributing](#contributing) section.
-It is easy to add Redis functions to the API.
 
 ## Installation<a id="installation"></a>
 You can install `redipy` using pip:
 
 ```sh
 pip install redipy
 ```
@@ -631,16 +626,17 @@
 ```
 
 [🔝](#toc)
 
 ## Limitations<a id="limitations"></a>
 The current limitations of `redipy` are:
 
-- Not all Redis commands are supported yet: This will eventually be resolved.
-  See [this issue to see the progress][implemented].
+- Some Redis commands are not supported yet: This is likely due to redundant
+  functionality. For all other cases it will eventually be resolved.
+  Check [this issue to see the status of redis functions][implemented].
 - The API differs slightly: Most notably stored values are always strings
   (i.e., the bytes returned by Redis are decoded as utf-8).
 - The semantic of Redis functions inside scripts has been altered to feel more
   natural coming from python: Redis functions inside Lua scripts often differ
   greatly from the documented behavior. For example, `LPOP` returns `false` for
   an empty list inside Lua (instead of `nil` or `cjson.null`). While `LPOP`
   returns `None` in the python API. The script API of `redipy` has been altered
```

### Comparing `redipy-0.6.0/README.md` & `redipy-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,21 +30,16 @@
 8. [License](#license)
 9. [Feedback](#feedback)
 
 </details>
 
 This [medium article][medium] explores some of the rationale behind the library.
 
-### Warning
-
-This library is still early in development and [not all Redis functions are
-available yet][implemented]!
 If you need certain functionality or found a bug, have a look at the
 [contributing](#contributing) section.
-It is easy to add Redis functions to the API.
 
 ## Installation<a id="installation"></a>
 You can install `redipy` using pip:
 
 ```sh
 pip install redipy
 ```
@@ -397,16 +392,17 @@
 ```
 
 [🔝](#toc)
 
 ## Limitations<a id="limitations"></a>
 The current limitations of `redipy` are:
 
-- Not all Redis commands are supported yet: This will eventually be resolved.
-  See [this issue to see the progress][implemented].
+- Some Redis commands are not supported yet: This is likely due to redundant
+  functionality. For all other cases it will eventually be resolved.
+  Check [this issue to see the status of redis functions][implemented].
 - The API differs slightly: Most notably stored values are always strings
   (i.e., the bytes returned by Redis are decoded as utf-8).
 - The semantic of Redis functions inside scripts has been altered to feel more
   natural coming from python: Redis functions inside Lua scripts often differ
   greatly from the documented behavior. For example, `LPOP` returns `false` for
   an empty list inside Lua (instead of `nil` or `cjson.null`). While `LPOP`
   returns `None` in the python API. The script API of `redipy` has been altered
```

### Comparing `redipy-0.6.0/pyproject.toml` & `redipy-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
     name = "redipy"
     description = "redipy is a uniform interface to Redis-like storage systems. It allows you to use the same Redis API with different backends that implement the same functionality."
     readme = "README.md"
-    version = "0.6.0"
+    version = "0.7.0"
     authors = [
         {name = "Josua Krause", email = "josua.krause@gmail.com"},
     ]
     keywords = [
         "redis",
         "in-memory",
         "uniform api",
```

### Comparing `redipy-0.6.0/src/redipy/__init__.py` & `redipy-0.7.0/src/redipy/__init__.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/api.py` & `redipy-0.7.0/src/redipy/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module defines the basic redis API. All redis functions appear once
 in RedisAPI and once in PipelineAPI. Additional functionality is added via
 RedisClientAPI."""
 import contextlib
 import datetime
-from collections.abc import Iterable, Iterator
-from typing import cast, get_args, Literal, overload
+from collections.abc import Callable, Iterable, Iterator
+from typing import cast, get_args, Literal, overload, TypeVar
 
 from redipy.backend.backend import ExecFunction
 from redipy.symbolic.seq import FnContext
 
 
+T = TypeVar('T')
+
+
 RSetMode = Literal[
     "always",
     "if_missing",  # NX
     "if_exists",  # XX
 ]
 """The conditions on when to set a value for the set command."""
 RSM_ALWAYS: RSetMode = "always"
@@ -1523,14 +1526,53 @@
             key (str): The key.
 
         Returns:
             set[str]: All elements of the set.
         """
         raise NotImplementedError()
 
+    def publish(self, key: str, msg: str) -> None:
+        """
+        Publishes a message on a pubsub channel.
+
+        See also the redis documentation: https://redis.io/commands/publish/
+
+        Args:
+            key (str): The pubsub key.
+            msg (str): The message.
+        """
+        raise NotImplementedError()
+
+    def wait_for(
+            self,
+            key: str,
+            predicate: Callable[[], T],
+            timeout: float | None) -> T | None:
+        """
+        Waits on a pubsub channel until a certain condition is met. This
+        ignores messages sent on the channel but instead checks the provided
+        condition once a message has been received. If the condition is
+        satisfied, its result is returned.
+
+        Args:
+            key (str): The pubsub key.
+            predicate (Callable[[], T]): If the result of this condition can
+                be converted to `True` via `bool` the condition is considered
+                satisfied and its result is returned.
+            timeout (float | None): If the predicate has not been fullfilled
+                within the time set by the timeout in seconds the function
+                returns None. If timeout is set to None the function will wait
+                indefinitely.
+
+        Returns:
+            T | None: The result of the condition is returned or None if the
+                function timed out.
+        """
+        raise NotImplementedError()
+
 
 class RedisClientAPI(RedisAPI):
     """This class enriches the redis API with pipeline and script
     functionality."""
     @contextlib.contextmanager
     def pipeline(self) -> Iterator[PipelineAPI]:
         """
```

### Comparing `redipy-0.6.0/src/redipy/backend/__init__.py` & `redipy-0.7.0/src/redipy/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/backend/backend.py` & `redipy-0.7.0/src/redipy/backend/backend.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/backend/runtime.py` & `redipy-0.7.0/src/redipy/backend/runtime.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/graph/__init__.py` & `redipy-0.7.0/src/redipy/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/graph/cmd.py` & `redipy-0.7.0/src/redipy/graph/cmd.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/graph/expr.py` & `redipy-0.7.0/src/redipy/graph/expr.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/graph/seq.py` & `redipy-0.7.0/src/redipy/graph/seq.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/main.py` & `redipy-0.7.0/src/redipy/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module contains the main class for accessing redis. The Redis class
 can be instantiated with different backends."""
 import contextlib
 import datetime
 from collections.abc import Callable, Iterator
-from typing import Literal, overload
+from typing import Literal, overload, TypeVar
 
 from redipy.api import (
     KeyType,
     PipelineAPI,
     RedisClientAPI,
     REX_ALWAYS,
     RExpireMode,
@@ -31,14 +31,17 @@
 from redipy.backend.runtime import Runtime
 from redipy.graph.seq import SequenceObj
 from redipy.memory.rt import LocalRuntime
 from redipy.redis.conn import RedisConfig, RedisConnection, RedisFactory
 from redipy.symbolic.seq import FnContext
 
 
+T = TypeVar('T')
+
+
 class Redis(RedisClientAPI):
     """
     This class is a wrapper around different runtime backends. Use this class
     to instantiate a redipy runtime.
     """
     def __init__(
             self,
@@ -451,7 +454,17 @@
         return self._rt.sismember(key, value)
 
     def scard(self, key: str) -> int:
         return self._rt.scard(key)
 
     def smembers(self, key: str) -> set[str]:
         return self._rt.smembers(key)
+
+    def publish(self, key: str, msg: str) -> None:
+        return self._rt.publish(key, msg)
+
+    def wait_for(
+            self,
+            key: str,
+            predicate: Callable[[], T],
+            timeout: float | None) -> T | None:
+        return self._rt.wait_for(key, predicate, timeout)
```

### Comparing `redipy-0.6.0/src/redipy/memory/__init__.py` & `redipy-0.7.0/src/redipy/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/memory/gfun.py` & `redipy-0.7.0/src/redipy/memory/gfun.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/memory/local.py` & `redipy-0.7.0/src/redipy/memory/local.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/memory/rfun.py` & `redipy-0.7.0/src/redipy/memory/rfun.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/memory/rt.py` & `redipy-0.7.0/src/redipy/memory/rt.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,14 +484,26 @@
         with self.lock():
             return self._sm.scard(key)
 
     def smembers(self, key: str) -> set[str]:
         with self.lock():
             return self._sm.smembers(key)
 
+    def publish(self, key: str, msg: str) -> None:
+        with self.lock():
+            return self._sm.publish(key, msg)
+
+    def wait_for(
+            self,
+            key: str,
+            predicate: Callable[[], T],
+            timeout: float | None) -> T | None:
+        with self.lock():
+            return self._sm.wait_for(key, predicate, timeout)
+
     def __str__(self) -> str:
         return f"{self.__class__.__name__}[{self._sm.get_state()}]"
 
     def __repr__(self) -> str:
         return self.__str__()
```

### Comparing `redipy-0.6.0/src/redipy/memory/state.py` & `redipy-0.7.0/src/redipy/memory/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module handles the internal state of the memory runtime."""
 import bisect
 import collections
 import itertools
+import threading
 import time
 from collections.abc import Callable, Iterable
 from datetime import datetime
 from typing import Literal, overload, TypeVar
 
 from redipy.api import (
     KeyType,
@@ -30,15 +31,21 @@
     REX_PERSIST,
     RExpireMode,
     RSetMode,
     RSM_ALWAYS,
     RSM_EXISTS,
     RSM_MISSING,
 )
-from redipy.util import convert_pattern, now, time_diff, to_number_str
+from redipy.util import (
+    convert_pattern,
+    now,
+    reject_patterns,
+    time_diff,
+    to_number_str,
+)
 
 
 T = TypeVar('T')
 
 
 def compute_expire(
         now_mono: float,
@@ -1083,14 +1090,16 @@
 
         Args:
             state (State): The associated state.
         """
         super().__init__()
         self._state = state
         self._now_mono: tuple[float, datetime] | None = None
+        # FIXME: for now we implement pubsub in the machine
+        self._pubsub: dict[str, threading.Condition] = {}
 
     def set_mono(self, now_mono: tuple[float, datetime] | None) -> None:
         """
         Sets the current time.
 
         Args:
             now_mono (tuple[float, datetime] | None): The current time for
@@ -1575,13 +1584,36 @@
     def smembers(self, key: str) -> set[str]:
         now_mono = self.get_mono()
         obj = self._state.readonly_set(key, now_mono)
         if obj is None:
             return set()
         return set(obj)
 
+    def publish(self, key: str, msg: str) -> None:
+        # FIXME: we do not support patterns or messages yet
+        pubsub_key = reject_patterns(key)
+        listen = self._pubsub.get(pubsub_key)
+        if listen is None:
+            return
+        with listen:
+            listen.notify_all()
+
+    def wait_for(
+            self,
+            key: str,
+            predicate: Callable[[], T],
+            timeout: float | None) -> T | None:
+        # FIXME: we do not support patterns or messages yet
+        pubsub_key = reject_patterns(key)
+        listen = self._pubsub.get(pubsub_key)
+        if listen is None:
+            listen = threading.Condition()
+            self._pubsub[pubsub_key] = listen
+        with listen:
+            return listen.wait_for(predicate, timeout)
+
     def __str__(self) -> str:
         return (
             f"{self.__class__.__name__}[state={self._state}]")
 
     def __repr__(self) -> str:
         return self.__str__()
```

### Comparing `redipy-0.6.0/src/redipy/plugin.py` & `redipy-0.7.0/src/redipy/plugin.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/redis/__init__.py` & `redipy-0.7.0/src/redipy/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/redis/conn.py` & `redipy-0.7.0/src/redipy/redis/conn.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """The runtime for the redis backend."""
 import contextlib
 import datetime
 import threading
+import time
 import uuid
 from collections.abc import Callable, Iterable, Iterator
 from typing import (
     Any,
     cast,
     Literal,
     NoReturn,
     NotRequired,
     overload,
     Protocol,
     TypedDict,
+    TypeVar,
 )
 
 from redis import Redis
 from redis.client import Pipeline
 from redis.commands.core import Script
 from redis.exceptions import ResponseError
 
@@ -56,14 +58,17 @@
     now,
     time_diff,
     to_list_str,
     to_maybe_str,
 )
 
 
+T = TypeVar('T')
+
+
 RedisConfig = TypedDict('RedisConfig', {
     "host": str,
     "port": int,
     "passwd": str,
     "prefix": NotRequired[str],
     "path": NotRequired[str],
 })
@@ -719,51 +724,55 @@
             str: The actual pubsub key.
         """
         return f"{self.get_prefix()}ps:{key}"
 
     def wait_for(
             self,
             key: str,
-            predicate: Callable[[], bool],
-            granularity: float = 30.0) -> None:
-        """
-        Waits until the condition is met.
-
-        Args:
-            key (str): The key used for the pubsub channel.
-
-            predicate (Callable[[], bool]): The condition.
-
-            granularity (float, optional): Maximum wait between predicate
-            checks in seconds. Defaults to 30.0.
-        """
-        if predicate():
-            return
+            predicate: Callable[[], T],
+            timeout: float | None) -> T | None:
+        res = predicate()
+        if bool(res):
+            return res
         with self.get_connection() as conn:
             with conn.pubsub() as psub:
                 psub.subscribe(self.get_pubsub_key(key))
                 try:
-                    while not predicate():
+                    start_time = time.monotonic()
+                    while True:
+                        res = predicate()
+                        if bool(res):
+                            return res
+                        so_far = time.monotonic() - start_time
+                        if timeout is not None and so_far > timeout:
+                            return None
+                        if timeout is None:
+                            wait_time = None
+                        else:
+                            wait_time = max(0, timeout - so_far)
                         psub.get_message(
                             ignore_subscribe_messages=True,
-                            timeout=granularity)
+                            timeout=cast(float, wait_time))
                         while psub.get_message() is not None:  # flushing queue
                             pass
                 finally:
                     psub.unsubscribe()
 
+    def publish(self, key: str, msg: str) -> None:
+        with self.get_connection() as conn:
+            conn.publish(self.get_pubsub_key(key), msg)
+
     def notify_all(self, key: str) -> None:
         """
         Notifies a pubsub channel.
 
         Args:
             key (str): The key used for the pubsub channel.
         """
-        with self.get_connection() as conn:
-            conn.publish(self.get_pubsub_key(key), "notify")
+        self.publish(key, "notify")
 
     def ping(self) -> None:
         """
         Pings the redis server (and checks whether the connection is live).
         """
         with self.get_connection() as conn:
             conn.ping()
```

### Comparing `redipy-0.6.0/src/redipy/redis/gpatch.py` & `redipy-0.7.0/src/redipy/redis/gpatch.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/redis/helpers.py` & `redipy-0.7.0/src/redipy/redis/helpers.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/redis/lua.py` & `redipy-0.7.0/src/redipy/redis/lua.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/redis/rpatch.py` & `redipy-0.7.0/src/redipy/redis/rpatch.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/script.py` & `redipy-0.7.0/src/redipy/script.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/symbolic/__init__.py` & `redipy-0.7.0/src/redipy/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/symbolic/core.py` & `redipy-0.7.0/src/redipy/symbolic/core.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/symbolic/expr.py` & `redipy-0.7.0/src/redipy/symbolic/expr.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/symbolic/fun.py` & `redipy-0.7.0/src/redipy/symbolic/fun.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/symbolic/rhash.py` & `redipy-0.7.0/src/redipy/symbolic/rhash.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/symbolic/rlist.py` & `redipy-0.7.0/src/redipy/symbolic/rlist.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/symbolic/rset.py` & `redipy-0.7.0/src/redipy/symbolic/rset.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/symbolic/rvar.py` & `redipy-0.7.0/src/redipy/symbolic/rvar.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/symbolic/rzset.py` & `redipy-0.7.0/src/redipy/symbolic/rzset.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/symbolic/seq.py` & `redipy-0.7.0/src/redipy/symbolic/seq.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/src/redipy/util.py` & `redipy-0.7.0/src/redipy/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1072,14 +1072,31 @@
         return {
             normalize_values(key): normalize_values(value)
             for key, value in res.items()
         }
     return res
 
 
+def reject_patterns(key: str) -> str:
+    """
+    Rejects a key if it is a pattern. This method should only be used for
+    partially implemented functions that would break if a user attempted to
+    use a pattern as input.
+
+    Args:
+        key (str): The key.
+
+    Returns:
+        str: The key.
+    """
+    if "*" in key or "?" in key or "[" in key:
+        raise ValueError(f"{key=} must not be a pattern")
+    return key
+
+
 def convert_pattern(pattern: str) -> tuple[str, re.Pattern]:
     """
     Convert a redis pattern into a prefix and a regular expression.
 
     Args:
         pattern (str): The redis pattern. A redis pattern can contain the
             wildcards `*` (variable match) and `?` (single character match) and
```

### Comparing `redipy-0.6.0/src/redipy.egg-info/PKG-INFO` & `redipy-0.7.0/src/redipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redipy
-Version: 0.6.0
+Version: 0.7.0
 Summary: redipy is a uniform interface to Redis-like storage systems. It allows you to use the same Redis API with different backends that implement the same functionality.
 Author-email: Josua Krause <josua.krause@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -264,21 +264,16 @@
 8. [License](#license)
 9. [Feedback](#feedback)
 
 </details>
 
 This [medium article][medium] explores some of the rationale behind the library.
 
-### Warning
-
-This library is still early in development and [not all Redis functions are
-available yet][implemented]!
 If you need certain functionality or found a bug, have a look at the
 [contributing](#contributing) section.
-It is easy to add Redis functions to the API.
 
 ## Installation<a id="installation"></a>
 You can install `redipy` using pip:
 
 ```sh
 pip install redipy
 ```
@@ -631,16 +626,17 @@
 ```
 
 [🔝](#toc)
 
 ## Limitations<a id="limitations"></a>
 The current limitations of `redipy` are:
 
-- Not all Redis commands are supported yet: This will eventually be resolved.
-  See [this issue to see the progress][implemented].
+- Some Redis commands are not supported yet: This is likely due to redundant
+  functionality. For all other cases it will eventually be resolved.
+  Check [this issue to see the status of redis functions][implemented].
 - The API differs slightly: Most notably stored values are always strings
   (i.e., the bytes returned by Redis are decoded as utf-8).
 - The semantic of Redis functions inside scripts has been altered to feel more
   natural coming from python: Redis functions inside Lua scripts often differ
   greatly from the documented behavior. For example, `LPOP` returns `false` for
   an empty list inside Lua (instead of `nil` or `cjson.null`). While `LPOP`
   returns `None` in the python API. The script API of `redipy` has been altered
```

### Comparing `redipy-0.6.0/src/redipy.egg-info/SOURCES.txt` & `redipy-0.7.0/src/redipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_api.py` & `redipy-0.7.0/test/test_api.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_err.py` & `redipy-0.7.0/test/test_err.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_expire.py` & `redipy-0.7.0/test/test_expire.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_keys.py` & `redipy-0.7.0/test/test_keys.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_misc.py` & `redipy-0.7.0/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_pipe.py` & `redipy-0.7.0/test/test_pipe.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_rlist.py` & `redipy-0.7.0/test/test_rlist.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_rset.py` & `redipy-0.7.0/test/test_rset.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_rvar.py` & `redipy-0.7.0/test/test_rvar.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_rzset.py` & `redipy-0.7.0/test/test_rzset.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_sanity.py` & `redipy-0.7.0/test/test_sanity.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_simple.py` & `redipy-0.7.0/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_stack.py` & `redipy-0.7.0/test/test_stack.py`

 * *Files identical despite different names*

### Comparing `redipy-0.6.0/test/test_util.py` & `redipy-0.7.0/test/test_util.py`

 * *Files identical despite different names*

