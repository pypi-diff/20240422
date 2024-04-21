# Comparing `tmp/tendril_connector_rabbitmq-0.2.1.tar.gz` & `tmp/tendril_connector_rabbitmq-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril_connector_rabbitmq-0.2.1.tar", last modified: Thu Apr 18 22:03:36 2024, max compression
+gzip compressed data, was "tendril_connector_rabbitmq-0.2.2.tar", last modified: Sun Apr 21 22:57:15 2024, max compression
```

## Comparing `tendril_connector_rabbitmq-0.2.1.tar` & `tendril_connector_rabbitmq-0.2.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.053965 tendril_connector_rabbitmq-0.2.1/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/MANIFEST.in
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5591 2024-04-18 22:03:36.049965 tendril_connector_rabbitmq-0.2.1/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2368 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.033965 tendril_connector_rabbitmq-0.2.1/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_connector_rabbitmq-0.2.1/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13482 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1602 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-18 22:03:36.053965 tendril_connector_rabbitmq-0.2.1/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3285 2023-08-15 05:25:44.000000 tendril_connector_rabbitmq-0.2.1/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.025965 tendril_connector_rabbitmq-0.2.1/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2021-03-26 08:21:36.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4484 2023-09-06 12:05:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/config/mq.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1439 2021-06-17 11:57:47.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/config/mq_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:06:39.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.041965 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-03 06:03:50.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5773 2024-04-17 22:19:49.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/aio.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8866 2023-09-09 06:47:04.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/tx.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.041965 tendril_connector_rabbitmq-0.2.1/src/tendril/core/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:03:13.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/core/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.041965 tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-04 13:00:08.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2715 2024-04-18 22:01:58.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/aio.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      816 2024-04-16 18:25:58.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/aio_base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      163 2023-08-14 12:34:45.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/tx.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.045965 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5591 2024-04-18 22:03:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1088 2024-04-18 22:03:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-18 22:03:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      568 2024-04-18 22:03:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-18 22:03:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.045965 tendril_connector_rabbitmq-0.2.1/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.678071 tendril_connector_rabbitmq-0.2.2/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5591 2024-04-21 22:57:15.678071 tendril_connector_rabbitmq-0.2.2/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2368 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.662071 tendril_connector_rabbitmq-0.2.2/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.666071 tendril_connector_rabbitmq-0.2.2/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.666071 tendril_connector_rabbitmq-0.2.2/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_connector_rabbitmq-0.2.2/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.666071 tendril_connector_rabbitmq-0.2.2/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13482 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1602 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.670071 tendril_connector_rabbitmq-0.2.2/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-21 22:57:15.678071 tendril_connector_rabbitmq-0.2.2/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3285 2023-08-15 05:25:44.000000 tendril_connector_rabbitmq-0.2.2/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.662071 tendril_connector_rabbitmq-0.2.2/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.670071 tendril_connector_rabbitmq-0.2.2/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.670071 tendril_connector_rabbitmq-0.2.2/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2021-03-26 08:21:36.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4484 2023-09-06 12:05:35.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/config/mq.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1439 2021-06-17 11:57:47.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/config/mq_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.670071 tendril_connector_rabbitmq-0.2.2/src/tendril/connectors/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:06:39.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/connectors/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.670071 tendril_connector_rabbitmq-0.2.2/src/tendril/connectors/rabbitmq/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-03 06:03:50.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/connectors/rabbitmq/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5773 2024-04-17 22:19:49.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/connectors/rabbitmq/aio.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8866 2023-09-09 06:47:04.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/connectors/rabbitmq/tx.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.670071 tendril_connector_rabbitmq-0.2.2/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:03:13.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.670071 tendril_connector_rabbitmq-0.2.2/src/tendril/core/mq/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-04 13:00:08.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/core/mq/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2808 2024-04-21 22:56:36.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/core/mq/aio.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      816 2024-04-16 18:25:58.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/core/mq/aio_base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      163 2023-08-14 12:34:45.000000 tendril_connector_rabbitmq-0.2.2/src/tendril/core/mq/tx.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.674071 tendril_connector_rabbitmq-0.2.2/src/tendril_connector_rabbitmq.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5591 2024-04-21 22:57:15.000000 tendril_connector_rabbitmq-0.2.2/src/tendril_connector_rabbitmq.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1088 2024-04-21 22:57:15.000000 tendril_connector_rabbitmq-0.2.2/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-21 22:57:15.000000 tendril_connector_rabbitmq-0.2.2/src/tendril_connector_rabbitmq.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      568 2024-04-21 22:57:15.000000 tendril_connector_rabbitmq-0.2.2/src/tendril_connector_rabbitmq.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-21 22:57:15.000000 tendril_connector_rabbitmq-0.2.2/src/tendril_connector_rabbitmq.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-21 22:57:15.674071 tendril_connector_rabbitmq-0.2.2/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.2/tox.ini
```

### Comparing `tendril_connector_rabbitmq-0.2.1/.gitignore` & `tendril_connector_rabbitmq-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/.readthedocs.yml` & `tendril_connector_rabbitmq-0.2.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/.travis.yml` & `tendril_connector_rabbitmq-0.2.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/LICENSE` & `tendril_connector_rabbitmq-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/PKG-INFO` & `tendril_connector_rabbitmq-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-connector-rabbitmq
-Version: 0.2.1
+Version: 0.2.2
 Summary: RabbitMQ Connector for Tendril
 Home-page: https://github.com/tendril-framework/tendril-connector-rabbitmq
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-connector-rabbitmq.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-connector-rabbitmq/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-connector-rabbitmq
```

### Comparing `tendril_connector_rabbitmq-0.2.1/README.rst` & `tendril_connector_rabbitmq-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/docs/Makefile` & `tendril_connector_rabbitmq-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/docs/_static/custom.css` & `tendril_connector_rabbitmq-0.2.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/docs/_static/favicon.ico` & `tendril_connector_rabbitmq-0.2.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/docs/_static/logo.png` & `tendril_connector_rabbitmq-0.2.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/docs/_static/logo_packed.png` & `tendril_connector_rabbitmq-0.2.2/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/docs/_templates/about.html` & `tendril_connector_rabbitmq-0.2.2/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/docs/conf.py` & `tendril_connector_rabbitmq-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/docs/index.rst` & `tendril_connector_rabbitmq-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/docs/installation.rst` & `tendril_connector_rabbitmq-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/setup.py` & `tendril_connector_rabbitmq-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/src/tendril/config/__init__.py` & `tendril_connector_rabbitmq-0.2.2/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/src/tendril/config/mq.py` & `tendril_connector_rabbitmq-0.2.2/src/tendril/config/mq.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/src/tendril/config/mq_core.py` & `tendril_connector_rabbitmq-0.2.2/src/tendril/config/mq_core.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/aio.py` & `tendril_connector_rabbitmq-0.2.2/src/tendril/connectors/rabbitmq/aio.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/tx.py` & `tendril_connector_rabbitmq-0.2.2/src/tendril/connectors/rabbitmq/tx.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/aio.py` & `tendril_connector_rabbitmq-0.2.2/src/tendril/core/mq/aio.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 
 import asyncio
 import importlib
 from functools import wraps
-from contextlib import asynccontextmanager
 
 from .aio_base import GenericMQAsyncClient
 from .aio_base import MQServerNotEnabled
-from tendril.config import MQ_ENABLED
+from tendril import config
+from tendril.config import MQ_SERVER_CODES
 from tendril.config import APISERVER_ENABLED
 from tendril.utils.versions import get_namespace_package_names
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
 if True:
@@ -65,17 +65,23 @@
 
 
 async def shutdown():
     manager = await MQManager.get_instance()
     await manager.close()
 
 
-if MQ_ENABLED:
+def _enable():
     if APISERVER_ENABLED:
         # Register the startup and shutdown functions as app events
         from tendril.apiserver.core import apiserver
+
         apiserver.on_event("startup")(startup)
         apiserver.on_event("shutdown")(shutdown)
     else:
         asyncio.get_event_loop().run_until_complete(startup())
         # atexit.register(asyncio.run, shutdown())
-        pass
+
+
+for code in MQ_SERVER_CODES:
+    if getattr(config, 'MQ{}_ENABLED'.format(code)):
+        _enable()
+        break
```

### Comparing `tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/aio_base.py` & `tendril_connector_rabbitmq-0.2.2/src/tendril/core/mq/aio_base.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/PKG-INFO` & `tendril_connector_rabbitmq-0.2.2/src/tendril_connector_rabbitmq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-connector-rabbitmq
-Version: 0.2.1
+Version: 0.2.2
 Summary: RabbitMQ Connector for Tendril
 Home-page: https://github.com/tendril-framework/tendril-connector-rabbitmq
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-connector-rabbitmq.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-connector-rabbitmq/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-connector-rabbitmq
```

### Comparing `tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt` & `tendril_connector_rabbitmq-0.2.2/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/requires.txt` & `tendril_connector_rabbitmq-0.2.2/src/tendril_connector_rabbitmq.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/tests/coveralls.py` & `tendril_connector_rabbitmq-0.2.2/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.1/tox.ini` & `tendril_connector_rabbitmq-0.2.2/tox.ini`

 * *Files identical despite different names*

