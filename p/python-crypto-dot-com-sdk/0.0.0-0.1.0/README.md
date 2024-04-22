# Comparing `tmp/python-crypto-dot-com-sdk-0.0.0.tar.gz` & `tmp/python-crypto-dot-com-sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-crypto-dot-com-sdk-0.0.0.tar", last modified: Sun Apr 21 05:55:14 2024, max compression
+gzip compressed data, was "python-crypto-dot-com-sdk-0.1.0.tar", last modified: Sun Apr 21 22:49:42 2024, max compression
```

## Comparing `python-crypto-dot-com-sdk-0.0.0.tar` & `python-crypto-dot-com-sdk-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-04-21 05:55:14.994049 python-crypto-dot-com-sdk-0.0.0/
--rw-r--r--   0 javad      (501) staff       (20)    11345 2024-04-21 05:27:36.000000 python-crypto-dot-com-sdk-0.0.0/LICENSE
--rw-r--r--   0 javad      (501) staff       (20)      399 2024-04-21 05:55:14.993960 python-crypto-dot-com-sdk-0.0.0/PKG-INFO
--rw-r--r--   0 javad      (501) staff       (20)       25 2024-04-21 05:27:36.000000 python-crypto-dot-com-sdk-0.0.0/README.md
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-04-21 05:55:14.993079 python-crypto-dot-com-sdk-0.0.0/crypto_dot_com/
--rw-r--r--   0 javad      (501) staff       (20)       22 2024-04-21 05:48:54.000000 python-crypto-dot-com-sdk-0.0.0/crypto_dot_com/__init__.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-04-21 05:55:14.993716 python-crypto-dot-com-sdk-0.0.0/python_crypto_dot_com_sdk.egg-info/
--rw-r--r--   0 javad      (501) staff       (20)      399 2024-04-21 05:55:14.000000 python-crypto-dot-com-sdk-0.0.0/python_crypto_dot_com_sdk.egg-info/PKG-INFO
--rw-r--r--   0 javad      (501) staff       (20)      307 2024-04-21 05:55:14.000000 python-crypto-dot-com-sdk-0.0.0/python_crypto_dot_com_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 javad      (501) staff       (20)        1 2024-04-21 05:55:14.000000 python-crypto-dot-com-sdk-0.0.0/python_crypto_dot_com_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 javad      (501) staff       (20)        9 2024-04-21 05:55:14.000000 python-crypto-dot-com-sdk-0.0.0/python_crypto_dot_com_sdk.egg-info/requires.txt
--rw-r--r--   0 javad      (501) staff       (20)       15 2024-04-21 05:55:14.000000 python-crypto-dot-com-sdk-0.0.0/python_crypto_dot_com_sdk.egg-info/top_level.txt
--rw-r--r--   0 javad      (501) staff       (20)      223 2024-04-21 05:55:14.994278 python-crypto-dot-com-sdk-0.0.0/setup.cfg
--rw-r--r--   0 javad      (501) staff       (20)      827 2024-04-21 05:48:41.000000 python-crypto-dot-com-sdk-0.0.0/setup.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-04-21 22:49:42.226941 python-crypto-dot-com-sdk-0.1.0/
+-rw-r--r--   0 javad      (501) staff       (20)    11345 2024-04-21 05:27:36.000000 python-crypto-dot-com-sdk-0.1.0/LICENSE
+-rw-r--r--   0 javad      (501) staff       (20)      399 2024-04-21 22:49:42.226872 python-crypto-dot-com-sdk-0.1.0/PKG-INFO
+-rw-r--r--   0 javad      (501) staff       (20)       25 2024-04-21 05:27:36.000000 python-crypto-dot-com-sdk-0.1.0/README.md
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-04-21 22:49:42.226073 python-crypto-dot-com-sdk-0.1.0/crypto_dot_com/
+-rw-r--r--   0 javad      (501) staff       (20)       22 2024-04-21 22:47:21.000000 python-crypto-dot-com-sdk-0.1.0/crypto_dot_com/__init__.py
+-rw-r--r--   0 javad      (501) staff       (20)     6214 2024-04-21 22:48:59.000000 python-crypto-dot-com-sdk-0.1.0/crypto_dot_com/client.py
+-rw-r--r--   0 javad      (501) staff       (20)      155 2024-04-21 22:28:57.000000 python-crypto-dot-com-sdk-0.1.0/crypto_dot_com/data_models.py
+-rw-r--r--   0 javad      (501) staff       (20)      140 2024-04-21 07:10:39.000000 python-crypto-dot-com-sdk-0.1.0/crypto_dot_com/settings.py
+-rw-r--r--   0 javad      (501) staff       (20)      368 2024-04-21 07:04:26.000000 python-crypto-dot-com-sdk-0.1.0/crypto_dot_com/utils.py
+-rw-r--r--   0 javad      (501) staff       (20)       30 2024-04-21 22:39:01.000000 python-crypto-dot-com-sdk-0.1.0/pyproject.toml
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-04-21 22:49:42.226644 python-crypto-dot-com-sdk-0.1.0/python_crypto_dot_com_sdk.egg-info/
+-rw-r--r--   0 javad      (501) staff       (20)      399 2024-04-21 22:49:42.000000 python-crypto-dot-com-sdk-0.1.0/python_crypto_dot_com_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 javad      (501) staff       (20)      428 2024-04-21 22:49:42.000000 python-crypto-dot-com-sdk-0.1.0/python_crypto_dot_com_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 javad      (501) staff       (20)        1 2024-04-21 22:49:42.000000 python-crypto-dot-com-sdk-0.1.0/python_crypto_dot_com_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 javad      (501) staff       (20)        9 2024-04-21 22:49:42.000000 python-crypto-dot-com-sdk-0.1.0/python_crypto_dot_com_sdk.egg-info/requires.txt
+-rw-r--r--   0 javad      (501) staff       (20)       15 2024-04-21 22:49:42.000000 python-crypto-dot-com-sdk-0.1.0/python_crypto_dot_com_sdk.egg-info/top_level.txt
+-rw-r--r--   0 javad      (501) staff       (20)      254 2024-04-21 22:49:42.227173 python-crypto-dot-com-sdk-0.1.0/setup.cfg
+-rw-r--r--   0 javad      (501) staff       (20)      827 2024-04-21 05:48:41.000000 python-crypto-dot-com-sdk-0.1.0/setup.py
```

### Comparing `python-crypto-dot-com-sdk-0.0.0/LICENSE` & `python-crypto-dot-com-sdk-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-crypto-dot-com-sdk-0.0.0/setup.py` & `python-crypto-dot-com-sdk-0.1.0/setup.py`

 * *Files identical despite different names*

