# Comparing `tmp/cs.cache-20240412.tar.gz` & `tmp/cs.cache-20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.cache-20240412.tar", last modified: Fri Apr 12 05:54:46 2024, max compression
+gzip compressed data, was "cs.cache-20240422.tar", last modified: Mon Apr 22 05:30:46 2024, max compression
```

## Comparing `cs.cache-20240412.tar` & `cs.cache-20240422.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:54:46.823222 cs.cache-20240412/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:54:43.000000 cs.cache-20240412/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     4046 2024-04-12 05:54:46.822922 cs.cache-20240412/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     3264 2024-04-12 05:54:43.000000 cs.cache-20240412/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:54:46.817482 cs.cache-20240412/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:54:46.818083 cs.cache-20240412/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:54:46.819962 cs.cache-20240412/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    11563 2024-04-12 05:54:29.000000 cs.cache-20240412/lib/python/cs/cache.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:54:46.822417 cs.cache-20240412/lib/python/cs.cache.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     4046 2024-04-12 05:54:46.000000 cs.cache-20240412/lib/python/cs.cache.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      273 2024-04-12 05:54:46.000000 cs.cache-20240412/lib/python/cs.cache.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:54:46.000000 cs.cache-20240412/lib/python/cs.cache.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      118 2024-04-12 05:54:46.000000 cs.cache-20240412/lib/python/cs.cache.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:54:46.000000 cs.cache-20240412/lib/python/cs.cache.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     4525 2024-04-12 05:54:45.000000 cs.cache-20240412/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:54:46.823329 cs.cache-20240412/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 05:30:46.974415 cs.cache-20240422/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 05:30:42.000000 cs.cache-20240422/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5998 2024-04-22 05:30:46.974136 cs.cache-20240422/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5216 2024-04-22 05:30:43.000000 cs.cache-20240422/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 05:30:46.970258 cs.cache-20240422/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 05:30:46.970548 cs.cache-20240422/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 05:30:46.971902 cs.cache-20240422/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    16351 2024-04-22 05:30:25.000000 cs.cache-20240422/lib/python/cs/cache.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 05:30:46.973691 cs.cache-20240422/lib/python/cs.cache.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5998 2024-04-22 05:30:46.000000 cs.cache-20240422/lib/python/cs.cache.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      273 2024-04-22 05:30:46.000000 cs.cache-20240422/lib/python/cs.cache.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 05:30:46.000000 cs.cache-20240422/lib/python/cs.cache.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      225 2024-04-22 05:30:46.000000 cs.cache-20240422/lib/python/cs.cache.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 05:30:46.000000 cs.cache-20240422/lib/python/cs.cache.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6626 2024-04-22 05:30:45.000000 cs.cache-20240422/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 05:30:46.974518 cs.cache-20240422/setup.cfg
```

