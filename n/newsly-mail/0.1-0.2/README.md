# Comparing `tmp/newsly_mail-0.1.tar.gz` & `tmp/newsly_mail-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newsly_mail-0.1.tar", last modified: Wed Apr  3 11:05:43 2024, max compression
+gzip compressed data, was "newsly_mail-0.2.tar", last modified: Mon Apr 22 01:03:30 2024, max compression
```

## Comparing `newsly_mail-0.1.tar` & `newsly_mail-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 11:05:43.638100 newsly_mail-0.1/
--rw-rw-rw-   0        0        0      202 2024-04-03 11:05:43.638100 newsly_mail-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-03 10:59:19.000000 newsly_mail-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 11:05:43.606849 newsly_mail-0.1/newsly_mail/
--rw-rw-rw-   0        0        0       39 2024-04-03 11:04:34.000000 newsly_mail-0.1/newsly_mail/__init__.py
--rw-rw-rw-   0        0        0      615 2024-04-03 10:59:36.000000 newsly_mail-0.1/newsly_mail/newsletter_mail.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:05:43.638100 newsly_mail-0.1/newsly_mail.egg-info/
--rw-rw-rw-   0        0        0      202 2024-04-03 11:05:43.000000 newsly_mail-0.1/newsly_mail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-04-03 11:05:43.000000 newsly_mail-0.1/newsly_mail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 11:05:43.000000 newsly_mail-0.1/newsly_mail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 11:05:43.000000 newsly_mail-0.1/newsly_mail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 11:05:43.638100 newsly_mail-0.1/setup.cfg
--rw-rw-rw-   0        0        0      359 2024-04-03 11:00:57.000000 newsly_mail-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 01:03:30.279448 newsly_mail-0.2/
+-rw-rw-rw-   0        0        0      895 2024-04-22 01:03:30.279448 newsly_mail-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      691 2024-04-22 01:01:07.000000 newsly_mail-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 01:03:30.271171 newsly_mail-0.2/newsly_mail/
+-rw-rw-rw-   0        0        0       39 2024-04-03 11:04:34.000000 newsly_mail-0.2/newsly_mail/__init__.py
+-rw-rw-rw-   0        0        0      615 2024-04-03 10:59:36.000000 newsly_mail-0.2/newsly_mail/newsletter_mail.py
+drwxrwxrwx   0        0        0        0 2024-04-22 01:03:30.279448 newsly_mail-0.2/newsly_mail.egg-info/
+-rw-rw-rw-   0        0        0      895 2024-04-22 01:03:29.000000 newsly_mail-0.2/newsly_mail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-04-22 01:03:30.000000 newsly_mail-0.2/newsly_mail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 01:03:29.000000 newsly_mail-0.2/newsly_mail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-22 01:03:29.000000 newsly_mail-0.2/newsly_mail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 01:03:30.279448 newsly_mail-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      359 2024-04-22 01:01:33.000000 newsly_mail-0.2/setup.py
```

### Comparing `newsly_mail-0.1/newsly_mail/newsletter_mail.py` & `newsly_mail-0.2/newsly_mail/newsletter_mail.py`

 * *Files identical despite different names*

