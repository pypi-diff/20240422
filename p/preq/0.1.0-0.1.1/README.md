# Comparing `tmp/preq-0.1.0.tar.gz` & `tmp/preq-0.1.1.tar.gz`

## Comparing `preq-0.1.0.tar` & `preq-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,19 @@
--rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 preq-0.1.0/Cargo.toml
--rw-r--r--   0     1000     1000     3106 2024-04-14 18:23:40.000000 preq-0.1.0/.gitignore
--rw-r--r--   0     1000     1000     8315 2024-04-17 23:23:49.000000 preq-0.1.0/Cargo.lock
--rw-r--r--   0     1000     1000      101 2024-04-14 18:02:15.000000 preq-0.1.0/README.md
--rw-r--r--   0     1000     1000     2505 2024-04-14 19:55:31.000000 preq-0.1.0/assets/stdlib
--rw-r--r--   0     1000     1000     5530 2024-04-17 23:52:21.000000 preq-0.1.0/src/main.rs
--rw-r--r--   0     1000     1000    20572 2024-04-14 18:43:49.000000 preq-0.1.0/tests/pipreqs
--rw-r--r--   0     1000     1000      243 2024-04-17 23:30:31.000000 preq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 preq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 preq-0.1.1/Cargo.toml
+-rw-r--r--   0     1000     1000     3106 2024-04-14 18:23:40.000000 preq-0.1.1/.gitignore
+-rw-r--r--   0     1000     1000    20262 2024-04-22 01:07:12.000000 preq-0.1.1/Cargo.lock
+-rw-r--r--   0     1000     1000        0 2024-04-20 22:49:41.000000 preq-0.1.1/Config.toml
+-rw-r--r--   0     1000     1000      101 2024-04-14 18:02:15.000000 preq-0.1.1/README.md
+-rw-r--r--   0     1000     1000     2505 2024-04-14 19:55:31.000000 preq-0.1.1/assets/stdlib
+-rw-r--r--   0     1000     1000     1688 2024-04-22 01:07:51.000000 preq-0.1.1/src/cli.rs
+-rw-r--r--   0     1000     1000      681 2024-04-20 22:54:39.000000 preq-0.1.1/src/config.rs
+-rw-r--r--   0     1000     1000      964 2024-04-22 00:47:58.000000 preq-0.1.1/src/input.rs
+-rw-r--r--   0     1000     1000      534 2024-04-22 01:07:49.000000 preq-0.1.1/src/main.rs
+-rw-r--r--   0     1000     1000      973 2024-04-21 23:41:48.000000 preq-0.1.1/src/map.rs
+-rw-r--r--   0     1000     1000     1397 2024-04-22 00:42:01.000000 preq-0.1.1/src/parse.rs
+-rw-r--r--   0     1000     1000      564 2024-04-21 23:08:11.000000 preq-0.1.1/src/utils/fallback.rs
+-rw-r--r--   0     1000     1000       31 2024-04-21 23:09:02.000000 preq-0.1.1/src/utils/mod.rs
+-rw-r--r--   0     1000     1000     3078 2024-04-21 23:26:20.000000 preq-0.1.1/src/utils/pyfuncs.rs
+-rw-r--r--   0     1000     1000      458 2024-04-21 23:49:17.000000 preq-0.1.1/src/write.rs
+-rw-r--r--   0     1000     1000    20572 2024-04-14 18:43:49.000000 preq-0.1.1/tests/pipreqs
+-rw-r--r--   0     1000     1000      444 2024-04-22 01:09:57.000000 preq-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      351 1970-01-01 00:00:00.000000 preq-0.1.1/PKG-INFO
```

### Comparing `preq-0.1.0/.gitignore` & `preq-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `preq-0.1.0/assets/stdlib` & `preq-0.1.1/assets/stdlib`

 * *Files identical despite different names*

### Comparing `preq-0.1.0/tests/pipreqs` & `preq-0.1.1/tests/pipreqs`

 * *Files identical despite different names*

