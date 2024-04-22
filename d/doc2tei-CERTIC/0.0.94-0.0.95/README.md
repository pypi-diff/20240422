# Comparing `tmp/doc2tei-CERTIC-0.0.94.tar.gz` & `tmp/doc2tei-CERTIC-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc2tei-CERTIC-0.0.94.tar", last modified: Mon Apr  8 16:23:04 2024, max compression
+gzip compressed data, was "doc2tei-CERTIC-0.0.95.tar", last modified: Mon Apr 22 08:03:03 2024, max compression
```

## Comparing `doc2tei-CERTIC-0.0.94.tar` & `doc2tei-CERTIC-0.0.95.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.179332 doc2tei-CERTIC-0.0.94/
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      537 2024-04-08 16:23:04.175331 doc2tei-CERTIC-0.0.94/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1710 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.155330 doc2tei-CERTIC-0.0.94/doc2tei/
--rw-rw-rw-   0 root         (0) root         (0)    21029 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1518 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.155330 doc2tei-CERTIC-0.0.94/doc2tei/resources/
--rwxrwxrwx   0 root         (0) root         (0)  5046534 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/saxon9.jar
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.167331 doc2tei-CERTIC-0.0.94/doc2tei/resources/schema/
--rw-rw-rw-   0 root         (0) root         (0)   355944 2024-03-28 17:16:57.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/schema/metopes.rng
--rw-rw-rw-   0 root         (0) root         (0)   176870 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/schema/openedition.rng
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.171331 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-01-cleanup/
--rw-rw-rw-   0 root         (0) root         (0)     4312 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl
--rw-rw-rw-   0 root         (0) root         (0)     8141 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4404 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl
--rw-rw-rw-   0 root         (0) root         (0)    33450 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3098 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-01-cleanup/cleanup.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.171331 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-02-normalisation/
--rw-rw-rw-   0 root         (0) root         (0)     3431 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl
--rw-rw-rw-   0 root         (0) root         (0)     8617 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl
--rw-rw-rw-   0 root         (0) root         (0)     7762 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4904 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4086 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.171331 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-03-enrich/
--rw-rw-rw-   0 root         (0) root         (0)     3552 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-03-enrich/enrich.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.171331 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/
--rw-rw-rw-   0 root         (0) root         (0)     4975 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-cit.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3685 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-figure-grp.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4512 2024-04-08 16:08:32.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-figure.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4093 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-floatingText.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3746 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-review.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4045 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-sp.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4248 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl
--rw-rw-rw-   0 root         (0) root         (0)     5996 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/hierarchize-review.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.171331 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-05-control/
--rw-rw-rw-   0 root         (0) root         (0)     2648 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-05-control/control-errors.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4036 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-05-control/control-hierarchy.xsl
--rw-rw-rw-   0 root         (0) root         (0)    10640 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-05-control/control-styles-id.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.171331 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-06-hierarchize/
--rw-rw-rw-   0 root         (0) root         (0)     5073 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.171331 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-07-organise/
--rw-rw-rw-   0 root         (0) root         (0)     8786 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-07-organise/organise.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.175331 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/
--rw-rw-rw-   0 root         (0) root         (0)     4102 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/back.xsl
--rw-rw-rw-   0 root         (0) root         (0)    14220 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_cit.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4026 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_code.xsl
--rw-rw-rw-   0 root         (0) root         (0)     8280 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_div-para.xsl
--rw-rw-rw-   0 root         (0) root         (0)    12366 2024-04-08 16:08:32.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_figure.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3771 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_linking.xsl
--rw-rw-rw-   0 root         (0) root         (0)     4335 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_list.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3468 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_note.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3592 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_typo.xsl
--rw-rw-rw-   0 root         (0) root         (0)    12206 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/front.xsl
--rw-rw-rw-   0 root         (0) root         (0)    33916 2024-04-08 16:22:45.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/teiHeader.xsl
--rw-rw-rw-   0 root         (0) root         (0)     3499 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/totei.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.175331 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-09-toOpenedition/
--rwxrwxrwx   0 root         (0) root         (0)     8845 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 16:23:04.175331 doc2tei-CERTIC-0.0.94/doc2tei_CERTIC.egg-info/
--rw-r--r--   0 root         (0) root         (0)      537 2024-04-08 16:23:04.000000 doc2tei-CERTIC-0.0.94/doc2tei_CERTIC.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2286 2024-04-08 16:23:04.000000 doc2tei-CERTIC-0.0.94/doc2tei_CERTIC.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 16:23:04.000000 doc2tei-CERTIC-0.0.94/doc2tei_CERTIC.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-04-08 16:23:04.000000 doc2tei-CERTIC-0.0.94/doc2tei_CERTIC.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-08 16:23:04.000000 doc2tei-CERTIC-0.0.94/doc2tei_CERTIC.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 16:23:04.000000 doc2tei-CERTIC-0.0.94/doc2tei_CERTIC.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 16:23:04.179332 doc2tei-CERTIC-0.0.94/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-08 16:22:45.000000 doc2tei-CERTIC-0.0.94/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.197390 doc2tei-CERTIC-0.0.95/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      537 2024-04-22 08:03:03.197390 doc2tei-CERTIC-0.0.95/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.005378 doc2tei-CERTIC-0.0.95/doc2tei/
+-rw-rw-rw-   0 root         (0) root         (0)    21029 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.005378 doc2tei-CERTIC-0.0.95/doc2tei/resources/
+-rwxrwxrwx   0 root         (0) root         (0)  5046534 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/saxon9.jar
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.097384 doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/
+-rw-rw-rw-   0 root         (0) root         (0)   357736 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/metopes.rng
+-rw-rw-rw-   0 root         (0) root         (0)   176870 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/openedition.rng
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.117385 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/
+-rw-rw-rw-   0 root         (0) root         (0)     4312 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     8141 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    33450 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.121385 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/
+-rw-rw-rw-   0 root         (0) root         (0)     3431 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     8617 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4904 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4086 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.121385 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-03-enrich/
+-rw-rw-rw-   0 root         (0) root         (0)     3552 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-03-enrich/enrich.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.125386 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-cit.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3685 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-figure-grp.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4512 2024-04-08 16:08:32.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-figure.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4093 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-floatingText.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3746 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-review.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-sp.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4248 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     5996 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/hierarchize-review.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.153387 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-errors.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4036 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-hierarchy.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    12240 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-styles-id.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.157388 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-06-hierarchize/
+-rw-rw-rw-   0 root         (0) root         (0)     5073 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.165388 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-07-organise/
+-rw-rw-rw-   0 root         (0) root         (0)     8786 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-07-organise/organise.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.181389 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/
+-rw-rw-rw-   0 root         (0) root         (0)     4102 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/back.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    14220 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_cit.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4026 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_code.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     9140 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_div-para.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    12822 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_figure.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_linking.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     4335 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_list.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3468 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_note.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3592 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_typo.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    12206 2024-04-08 15:44:42.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/front.xsl
+-rw-rw-rw-   0 root         (0) root         (0)    37403 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/teiHeader.xsl
+-rw-rw-rw-   0 root         (0) root         (0)     3499 2024-03-28 17:14:35.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/totei.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.193390 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-09-toOpenedition/
+-rwxrwxrwx   0 root         (0) root         (0)     9839 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:03:03.197390 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      537 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-22 08:03:02.000000 doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 08:03:03.197390 doc2tei-CERTIC-0.0.95/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-22 08:02:44.000000 doc2tei-CERTIC-0.0.95/setup.py
```

### Comparing `doc2tei-CERTIC-0.0.94/PKG-INFO` & `doc2tei-CERTIC-0.0.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc2tei-CERTIC
-Version: 0.0.94
+Version: 0.0.95
 Summary: Convert ODT and DOCX files to TEI
 Home-page: https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doc2tei-CERTIC-0.0.94/README.md` & `doc2tei-CERTIC-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/__init__.py` & `doc2tei-CERTIC-0.0.95/doc2tei/__init__.py`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/__main__.py` & `doc2tei-CERTIC-0.0.95/doc2tei/__main__.py`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/saxon9.jar` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/saxon9.jar`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/schema/metopes.rng` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/metopes.rng`

 * *Files 0% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/schema/metopes.rng` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/metopes.rng`

```diff
@@ -5793,14 +5793,41 @@
       <ref name="att.datable.attributes"/>
       <optional>
         <attribute name="type">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">Sample values include: 1] speaker</a:documentation>
           <text/>
         </attribute>
       </optional>
+      <optional>
+        <attribute name="role">
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+          <choice>
+            <value>aut</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>aut fld</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>edt</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>fld</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>trl</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>ill</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>pht</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>drm</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>pbd</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+            <value>rcp</value>
+            <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+          </choice>
+        </attribute>
+      </optional>
       <empty/>
     </element>
   </define>
   <define name="email">
     <element name="email">
       <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(electronic mail address) contains an email address identifying a location to which email messages can be delivered. [3.6.2. Addresses]</a:documentation>
       <ref name="macro.phraseSeq"/>
@@ -6781,27 +6808,20 @@
       </optional>
       <empty/>
     </element>
   </define>
   <define name="publicationStmt">
     <element name="publicationStmt">
       <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(publication statement) Information about electronic publishing [2.2.4. Publication, Distribution, Licensing, etc. 2.2. The File Description]</a:documentation>
-      <choice>
-        <oneOrMore>
-          <group>
-            <ref name="model.publicationStmtPart.agency"/>
-            <zeroOrMore>
-              <ref name="model.publicationStmtPart.detail"/>
-            </zeroOrMore>
-          </group>
-        </oneOrMore>
-        <oneOrMore>
-          <ref name="model.pLike"/>
-        </oneOrMore>
-      </choice>
+      <zeroOrMore>
+        <choice>
+          <ref name="ref"/>
+          <ref name="ab"/>
+        </choice>
+      </zeroOrMore>
     </element>
   </define>
   <define name="distributor">
     <element name="distributor">
       <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(distributor) supplies the name of a person or other agency responsible for the distribution of a text. [2.2.4. Publication, Distribution, Licensing, etc.]</a:documentation>
       <text/>
     </element>
@@ -7990,14 +8010,20 @@
         <attribute name="type">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
           <data type="token">
             <param name="pattern">[a-zA-Z_\d]*</param>
           </data>
         </attribute>
       </optional>
+      <optional>
+        <attribute name="subtype">
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+          <text/>
+        </attribute>
+      </optional>
       <empty/>
     </element>
   </define>
   <define name="argument">
     <element name="argument">
       <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(argument) contains a formal list or prose description of the topics addressed by a subdivision of a text. [4.2. Elements Common to All Divisions 4.6. Title Pages]</a:documentation>
       <group>
@@ -8559,14 +8585,20 @@
       </optional>
       <optional>
         <attribute name="unit">
           <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
           <text/>
         </attribute>
       </optional>
+      <optional>
+        <attribute name="extent">
+          <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0"/>
+          <text/>
+        </attribute>
+      </optional>
       <empty/>
     </element>
   </define>
   <define name="normalization">
     <element name="normalization">
       <a:documentation xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0">(normalization) [Métopes] indique l'extension de la normalisation ou de la régularisation effectuée sur le texte source dans sa conversion vers sa forme électronique. [ ]</a:documentation>
       <oneOrMore>
```

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/schema/openedition.rng` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/schema/openedition.rng`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-delete.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-nodes.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-preserve.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup-styles.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-01-cleanup/cleanup.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-01-cleanup/cleanup.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/a-normalize-stylename.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-cit.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes-index.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/b-normalize-nodes.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-02-normalisation/c-normalize-groupspan.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-03-enrich/enrich.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-03-enrich/enrich.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-cit.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-cit.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-figure-grp.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-figure-grp.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-figure.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-figure.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-floatingText.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-floatingText.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-review.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-review.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/group-sp.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/group-sp.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/hierarchize-floatingText.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/hierarchize-review.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/hierarchize-review.xsl`

 * *Files 1% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-04-group/hierarchize-review.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-04-group/hierarchize-review.xsl`

```diff
@@ -35,15 +35,15 @@
               </xsl:call-template>
             </xsl:when>
             <xsl:otherwise>
               <div>
                 <xsl:attribute name="type">
                   <xsl:choose>
                     <xsl:when test="@subtype='biblio'">
-                      <xsl:text>review-bibliography</xsl:text>
+                      <xsl:text>review_bibliography</xsl:text>
                     </xsl:when>
                     <xsl:otherwise>
                       <xsl:value-of select="concat('section',$level)"/>
                     </xsl:otherwise>
                   </xsl:choose>
                 </xsl:attribute>
                 <xsl:attribute name="xml:id">
```

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-05-control/control-errors.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-errors.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-05-control/control-hierarchy.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-hierarchy.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-05-control/control-styles-id.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-styles-id.xsl`

 * *Files 10% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-05-control/control-styles-id.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-05-control/control-styles-id.xsl`

```diff
@@ -94,14 +94,34 @@
                     <xsl:text>aff</xsl:text>
                     <xsl:number count="*[local-name()=$currentElementName]" from="*:front" level="any" format="01"/>
                   </xsl:when>
                   <xsl:when test="$currentElementName='email'">
                     <xsl:text>email</xsl:text>
                     <xsl:number count="*[local-name()=$currentElementName]" from="*:front" level="any" format="01"/>
                   </xsl:when>
+                  <xsl:when test="$currentElementName='figure'">
+                    <xsl:choose>
+                      <xsl:when test="parent::*:figure">
+                        <xsl:value-of select="$currentElementName"/>
+                        <xsl:number count="*[local-name()=$currentElementName and not(parent::*:figure or parent::*:cell)]" from="*:text" level="any" format="01"/>
+                        <xsl:text>_</xsl:text>
+                        <xsl:number count="*[local-name()=$currentElementName]" from="*:figure" level="single" format="1"/>
+                      </xsl:when>
+                      <xsl:when test="parent::*:cell">
+                        <xsl:value-of select="$currentElementName"/>
+                        <xsl:number count="*[local-name()=$currentElementName and not(parent::*:figure or parent::*:cell)]" from="*:text" level="any" format="01"/>
+                        <xsl:text>_</xsl:text>
+                        <xsl:number count="*:figure[parent::*:cell]" from="*:table" level="any" format="1"/>
+                      </xsl:when>
+                      <xsl:otherwise>
+                        <xsl:value-of select="$currentElementName"/>
+                        <xsl:number count="*[local-name()=$currentElementName and not(parent::*:figure or parent::*:cell)]" from="*:text" level="any" format="01"/>
+                      </xsl:otherwise>
+                    </xsl:choose>
+                  </xsl:when>
                   <xsl:when test="$currentElementName='bibl'">
                     <xsl:value-of select="$currentElementName"/>
                     <xsl:number count="*[local-name()=$currentElementName]" from="*:back" level="any" format="001"/>
                   </xsl:when>
                   <xsl:when test="($currentElementName='div' and ./@type='bibliography') or ($currentElementName='div' and ./@type='appendix')">
                     <xsl:value-of select="@type"/>
                   </xsl:when>
@@ -121,15 +141,15 @@
                   </xsl:when>
                   <xsl:when test="$currentElementName='p'">
                     <xsl:value-of select="$currentElementName"/>
                     <xsl:number count="*[local-name()='p' and ancestor::*:body and not(parent::*:note) and not(parent::*:figure)]" from="*:body[not(parent::*:floatingText)]" level="any"/>
                   </xsl:when>
                   <xsl:otherwise>
                     <xsl:value-of select="$currentElementName"/>
-                    <xsl:number count="*[local-name()=$currentElementName]" from="*:body[not(parent::*:floatingText)]" level="any"/>
+                    <xsl:number count="*[local-name()=$currentElementName]" from="*:body[not(parent::*:floatingText)]" level="any" format="01"/>
                     <!-- [not(parent::*:note)] -->
                   </xsl:otherwise>
                 </xsl:choose>
               </xsl:attribute>
               <xsl:apply-templates/>
             </xsl:element>
           </xsl:when>
```

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-06-hierarchize/hierarchize.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-07-organise/organise.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-07-organise/organise.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/back.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/back.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_cit.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_cit.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_code.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_code.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_div-para.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_div-para.xsl`

 * *Files 3% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_div-para.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_div-para.xsl`

```diff
@@ -159,20 +159,40 @@
             </bibl>
           </body>
         </xsl:otherwise>
       </xsl:choose>
     </floatingText>
   </xsl:template>
   <!-- ### archeo CHR ### -->
-  <xsl:template match="text:p[@text:style-name='TEI_archeoCHR_fieldwork-method']|text:p[@text:style-name='TEI_archeoCHR_fieldwork-year']|text:p[@text:style-name='TEI_archeoCHR_type']|text:p[starts-with(@text:style-name,'TEI_archeoCHR_keywords')]">
+  <xsl:template match="text:p[@text:style-name='TEI_archeoCHR_fieldwork-method']|text:p[@text:style-name='TEI_archeoCHR_type']|text:p[starts-with(@text:style-name,'TEI_archeoCHR_keywords')]|text:p[@text:style-name='TEI_archeoCHR_authority']">
     <p rend="{concat('archeo_',substring-after(@text:style-name,'TEI_archeoCHR_'))}">
       <xsl:copy-of select="@rendition"/>
       <xsl:apply-templates/>
     </p>
   </xsl:template>
+  <xsl:template match="text:p[@text:style-name='TEI_archeoCHR_fieldwork-year']">
+    <p rend="{concat('archeo_',substring-after(@text:style-name,'TEI_archeoCHR_'))}">
+      <xsl:copy-of select="@rendition"/>
+      <xsl:analyze-string select="." regex="\d{{4}}">
+        <xsl:matching-substring>
+          <date>
+            <xsl:value-of select="."/>
+          </date>
+        </xsl:matching-substring>
+        <xsl:non-matching-substring>
+          <xsl:value-of select="."/>
+        </xsl:non-matching-substring>
+      </xsl:analyze-string>
+    </p>
+  </xsl:template>
+  <xsl:template match="text:span[starts-with(@text:style-name,'TEI_archeoCHR_name')]">
+    <name role="{replace(substring-after(@text:style-name,'TEI_archeoCHR_name:'),'_20_',' ')}">
+      <xsl:apply-templates/>
+    </name>
+  </xsl:template>
   <!-- ### bibl ### -->
   <xsl:template match="text:p[@text:style-name='TEI_bibl_reference']">
     <!--    <xsl:comment>traitement générique des bibl</xsl:comment>-->
     <bibl>
       <xsl:copy-of select="@* except(@text:style-name)"/>
       <xsl:apply-templates/>
     </bibl>
```

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_figure.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_figure.xsl`

 * *Files 2% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_figure.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_figure.xsl`

```diff
@@ -157,21 +157,29 @@
   <xsl:template match="draw:frame">
     <xsl:choose>
       <xsl:when test="preceding-sibling::text() or following-sibling::text()">
         <figure rend="inline">
           <xsl:apply-templates/>
         </figure>
       </xsl:when>
-      <xsl:when test="ancestor::*:figure">
+      <xsl:when test="ancestor::*:figure and not(ancestor::table:table-cell)">
         <xsl:apply-templates/>
       </xsl:when>
+      <!-- dans une cellule de tableau : sans texte avant ou après donc block mais peut déjà être dans une section figure (avec titre, légende…) -->
       <xsl:when test="not(preceding-sibling::text() or following-sibling::text()) and ancestor::table:table-cell">
-        <figure>
-          <xsl:apply-templates/>
-        </figure>
+        <xsl:choose>
+          <xsl:when test="parent::text:p[parent::*:figure]">
+            <xsl:apply-templates/>
+          </xsl:when>
+          <xsl:otherwise>
+            <figure>
+              <xsl:apply-templates/>
+            </figure>
+          </xsl:otherwise>
+        </xsl:choose>
       </xsl:when>
       <xsl:when test="not(preceding-sibling::text() or following-sibling::text()) and parent::text:p[parent::text:note]">
         <figure>
           <xsl:apply-templates/>
         </figure>
       </xsl:when>
       <xsl:otherwise>
```

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_linking.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_linking.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_list.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_list.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_note.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_note.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/core_typo.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/core_typo.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/front.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/front.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/teiHeader.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/teiHeader.xsl`

 * *Files 2% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/teiHeader.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/teiHeader.xsl`

```diff
@@ -44,19 +44,20 @@
                 <xsl:otherwise>undefined</xsl:otherwise>
               </xsl:choose>
             </xsl:variable>
             <xsl:choose>
               <!-- cas d'utilisation de TEI_section_auteur avec affiliation (coll. de cr ou encadrés) -->
               <xsl:when test="@text:style-name='TEI_authority_affiliation'"/>
               <xsl:when test="$context='authorities'">
-                <!--                        <xsl:comment>authorities</xsl:comment>-->
                 <xsl:apply-templates select="./text:span[starts-with(@text:style-name,'TEI_author-inline:')]|./text:span[starts-with(@text:style-name,'TEI_editor-inline:')]" mode="teiHeader"/>
+                <xsl:if test="following-sibling::*[1][local-name()='p' and @text:style-name='TEI_authorities']">
+                  <xsl:apply-templates select="following-sibling::*[1][local-name()='p' and @text:style-name='TEI_authorities']/text:span[starts-with(@text:style-name,'TEI_author-inline:')]|following-sibling::*[1][local-name()='p' and @text:style-name='TEI_authorities']/text:span[starts-with(@text:style-name,'TEI_editor-inline:')]" mode="teiHeader"/>
+                </xsl:if>
               </xsl:when>
               <xsl:otherwise>
-                <!--                        <xsl:comment>author|editor</xsl:comment>-->
                 <xsl:element name="{$context}">
                   <xsl:attribute name="role" select="substring-after(./@text:style-name,':')"/>
                   <xsl:apply-templates select="current-group()[not(contains(@text:style-name,'_biography'))]" mode="teiHeader"/>
                   <xsl:if test="current-group()/.[@text:style-name='TEI_authority_biography']">
                     <ref type="biography" target="{concat('#bio',format-number(position(),'00'))}"/>
                   </xsl:if>
                   <!--
@@ -122,26 +123,24 @@
               <idno>
                 <xsl:value-of select="text:span[@text:style-name='TEI_funderref_inline']"/>
               </idno>
             </funder>
           </xsl:for-each>
         </titleStmt>
         <publicationStmt>
-          <!--          <publisher></publisher>-->
           <!-- ## editorial_workflow ## -->
+          <ref type="volume_xml"/>
           <ab type="expression">
             <bibl>
               <publisher/>
               <!-- Droits : expression de l'auteur (dispositifs légaux généraux)  -->
               <availability>
                 <licence target="#"/>
                 <p/>
               </availability>
-              <!-- volume (fichier XML) auquel est rattaché l'UE  -->
-              <ref type="book" target="#"/>
             </bibl>
           </ab>
           <xsl:if test="//text:p[@text:style-name='TEI_date_reception'] or //text:p[@text:style-name='TEI_date_acceptance']">
             <ab type="editorial_workflow">
               <xsl:if test="//text:p[@text:style-name='TEI_date_reception']">
                 <date type="received">
                   <xsl:variable name="rDate" select="substring(//text:p[@text:style-name='TEI_date_reception']/text:span[@text:style-name='TEI_date_normalised'],2,10)"/>
@@ -160,90 +159,141 @@
                   <xsl:variable name="aDateY" select="substring($aDate,7,4)"/>
                   <xsl:attribute name="when" select="concat($aDateY,'-',$aDateM,'-',$aDateD)"/>
                   <xsl:value-of select="//text:p[@text:style-name='TEI_date_acceptance']"/>
                 </date>
               </xsl:if>
             </ab>
           </xsl:if>
-          <!-- blocs <ab> Métopes [todo] -->
+          <!-- blocs <ab> Métopes -->
           <ab type="book">
             <bibl>
-              <publisher/>
-              <distributor/>
               <date type="publishing"/>
               <biblScope unit="page">
                 <xsl:attribute name="from" select="substring-before(//text:p[@text:style-name='TEI_pagination'],'-')"/>
                 <xsl:attribute name="to" select="substring-after(//text:p[@text:style-name='TEI_pagination'],'-')"/>
                 <xsl:value-of select="//text:p[@text:style-name='TEI_pagination']"/>
               </biblScope>
               <availability>
                 <licence/>
                 <p/>
               </availability>
             </bibl>
           </ab>
           <ab type="digital_download" subtype="PDF">
             <bibl>
+              <idno type="DOI" subtype="-"/>
+              <ref type="DOI"/>
+              <ref type="site"/>
               <distributor/>
               <date type="publishing"/>
-              <dim type="pagination" unit="page" extent="xx-yy">pages xx à yy</dim>
-              <dim type="weight" unit="Ko|Mo" extent="">poids :</dim>
-              <idno type="DOI" subtype="crossref|datacite|lsid"/>
-              <!-- Si contraire à ce qui est défini supra -->
-              <publisher/>
+              <dim type="weight" unit="Mo" extent=""/>
+              <!-- Si contraire à ce qui est défini supra
+                    <publisher></publisher> -->
               <availability>
                 <licence/>
                 <p/>
               </availability>
             </bibl>
-            <!-- Ajouter des métadonnées d'accessibilité -->
-            <desc type="??"/>
+            <!-- Ajouter des métadonnées d'accessibilité 
+                <desc type="??"></desc>-->
           </ab>
           <ab type="digital_download" subtype="EPUB">
             <bibl>
+              <idno type="ISBN-13"/>
+              <idno type="DOI" subtype="-"/>
+              <ref type="DOI"/>
+              <ref type="site"/>
               <distributor/>
               <date type="publishing"/>
-              <idno type="ISBN-13"/>
-              <idno type="EAN"/>
-              <idno type="DOI"/>
               <availability>
                 <licence/>
                 <p/>
               </availability>
-              <dim type="weight" unit="Ko|Mo" extent=""/>
+              <dim type="weight" unit="Ko" extent=""/>
             </bibl>
-            <!-- XG : ajout des valeurs par défaut -->
+            <!-- Mode d'accès par défaut : textual -->
             <desc type="accessMode">textual</desc>
-            <desc type="accessibilityFeature">none</desc>
+            <!-- Mode d'accès 'visual' ajouté s'il y a des images. -->
+            <xsl:if test="ancestor::*:TEI//draw:image">
+              <desc type="accessMode">visual</desc>
+            </xsl:if>
+            <!-- Caractéristiques d'accessibilité présentes par défaut dans tous les ePubs Métopes : -->
+            <desc type="accessibilityFeature">ARIA</desc>
+            <desc type="accessibilityFeature">highContrastDisplay</desc>
+            <desc type="accessibilityFeature">readingOrder</desc>
+            <desc type="accessibilityFeature">structuralNavigation</desc>
+            <desc type="accessibilityFeature">tableOfContents</desc>
+            <desc type="accessibilityFeature">unlocked</desc>
+            <xsl:if test="count(ancestor::*:TEI//draw:image) = count(ancestor::*:TEI//draw:frame/svg:desc)">
+              <desc type="accessibilityFeature">alternativeText</desc>
+            </xsl:if>
+            <!-- Risques d'accessibilité (à vérifier par l'utilisateur) : -->
             <desc subtype="soundHazard" type="accessibilityHazard">noSoundHazard</desc>
             <desc subtype="flashingHazard" type="accessibilityHazard">noFlashingHazard</desc>
             <desc subtype="motionSimulationHazard" type="accessibilityHazard">noMotionSimulationHazard</desc>
-            <desc type="accessModeSufficient">textual</desc>
-            <desc type="accessibilitySummary"/>
-            <!-- Fin ajout XG -->
+            <!-- Mode d'accès suffisant (à vérifier par l'utilisateur) : "textual" par défaut, "textual,visual" lorsque toutes les images ne sont pas pourvues de texte alternatif. -->
+            <xsl:choose>
+              <xsl:when test="not(count(ancestor::*:TEI//draw:image) = count(ancestor::*:TEI//draw:frame/svg:desc))">
+                <desc type="accessModeSufficient">textual,visual</desc>
+              </xsl:when>
+              <xsl:otherwise>
+                <desc type="accessModeSufficient">textual</desc>
+              </xsl:otherwise>
+            </xsl:choose>
+            <!-- Résumé d'accessibilité : -->
+            <desc type="accessibilitySummary">
+              <xsl:variable name="mainLangTwoCars" select="substring-before($mainLang, '-')"/>
+              <!-- commenté car la ressource n'est pas sur le serveur : 
+<xsl:apply-templates select="document('../../../xxe/common/i18n.xml')//*:entry[*:key='accessibilitySummaryContent']/*:text[@xml:lang = $mainLangTwoCars]/node()"/>-->
+            </desc>
           </ab>
           <ab type="digital_online" subtype="HTML">
             <bibl>
               <distributor>
-                <!--OpenEdition|Cairn.info|OJS|alt-->
+                <!--OpenEdition|Cairn.info|Érudit|Redalyc|Other-->
               </distributor>
+              <name type="CMS"/>
+              <idno type="DOI" subtype="-"/>
+              <ref type="DOI"/>
+              <ref type="site"/>
               <date type="publishing"/>
               <date type="embargoend"/>
               <idno type="documentnumber">
                 <xsl:value-of select="//text:p[@text:style-name='TEI_document_number']"/>
               </idno>
               <!--num ?-->
-              <idno type="DOI"/>
-              <ref target="URL"/>
               <availability>
                 <licence/>
                 <p/>
               </availability>
             </bibl>
           </ab>
+          <!-- archeo…-->
+          <xsl:if test="following::text:p[starts-with(@text:style-name,'TEI_archeoART')]">
+            <ab subtype="archeo">
+              <idno>
+                <xsl:attribute name="type" select="substring-after(following::text:p[starts-with(@text:style-name,'TEI_archeoART_IDmission:EFA')]/@text:style-name,':')"/>
+                <xsl:value-of select="substring-after(following::text:p[starts-with(@text:style-name,'TEI_archeoART_IDmission:EFA')]/text(),': ')"/>
+              </idno>
+              <xsl:variable name="dateOP" select="substring-after(following::text:p[@text:style-name='TEI_archeoART_date'],': ')"/>
+              <xsl:analyze-string select="$dateOP" regex="\d{{4}}">
+                <xsl:matching-substring>
+                  <date>
+                    <xsl:value-of select="."/>
+                  </date>
+                </xsl:matching-substring>
+                <xsl:non-matching-substring/>
+              </xsl:analyze-string>
+              <name type="nature_op">
+                <term>
+                  <xsl:value-of select="substring-after(following::text:p[starts-with(@text:style-name,'TEI_archeoCHR_fieldwork_method')]/text(),': ')"/>
+                </term>
+              </name>
+            </ab>
+          </xsl:if>
         </publicationStmt>
         <sourceDesc>
           <p>COMMONS/Métopes : 1.0</p>
         </sourceDesc>
       </fileDesc>
       <encodingDesc>
         <xsl:if test="not(//meta:user-defined[@meta:name='tplVersion'])">
@@ -257,15 +307,15 @@
               <xsl:value-of select="//meta:user-defined[@meta:name='tplVersion']"/>
             </xsl:attribute>
             <label>Word template</label>
             <desc>Version of MS Word template used</desc>
             <!-- todo : lien vers le code publié -->
             <ref target="#"/>
           </application>
-          <application version="0.0.94">
+          <application version="0.0.95">
             <xsl:attribute name="ident" select="concat('circe-',$source)"/>
             <label>Circé</label>
             <desc>Document converted into TEI using Circé application (doc2tei pipeline)</desc>
             <!-- todo : lien vers le code publié -->
             <ref target="#"/>
           </application>
         </appInfo>
```

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-08-totei/totei.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-08-totei/totei.xsl`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl`

 * *Files 4% similar despite different names*

#### Comparing `doc2tei-CERTIC-0.0.94/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl` & `doc2tei-CERTIC-0.0.95/doc2tei/resources/xsl-09-toOpenedition/toOpenedition.xsl`

```diff
@@ -85,14 +85,28 @@
         </xsl:when>
         <xsl:otherwise>
           <p>Circé</p>
         </xsl:otherwise>
       </xsl:choose>
     </sourceDesc>
   </xsl:template>
+  <xsl:template match="tei:tagsDecl">
+    <tagsDecl>
+      <xsl:if test="child::tei:rendition[@xml:id='list-ndash'] and not(child::tei:rendition[@xml:id='list-ndash'])">
+        <rendition scheme="css" xml:id="list-disc">list-style-type:disc;</rendition>
+      </xsl:if>
+      <xsl:if test="following::tei:bibl[@type='sec_authority']">
+        <rendition scheme="css" xml:id="end">text-align:end;</rendition>
+      </xsl:if>
+      <xsl:apply-templates/>
+    </tagsDecl>
+  </xsl:template>
+  <xsl:template match="tei:language">
+    <language ident="{substring-before(@ident,'-')}"/>
+  </xsl:template>
   <xsl:template match="@change"/>
   <xsl:template match="tei:editorialDecl"/>
   <xsl:template match="tei:ab"/>
   <xsl:template match="tei:sourceDesc"/>
   <xsl:template match="tei:funder[not(@type='funder_registry')]"/>
   <!-- ## TEXT ## -->
   <xsl:template match="tei:text">
@@ -128,27 +142,40 @@
   </xsl:template>
   <xsl:template match="tei:p[starts-with(@rend,'unknownstyle:')]">
     <xsl:copy>
       <xsl:apply-templates select="@*[name() != 'rend']"/>
       <xsl:apply-templates select="node()"/>
     </xsl:copy>
   </xsl:template>
+  <xsl:template match="tei:p[starts-with(@rend,'TEI_local')]">
+    <xsl:copy>
+      <xsl:apply-templates select="@*[name() != 'rend']"/>
+      <xsl:apply-templates select="node()"/>
+    </xsl:copy>
+  </xsl:template>
   <xsl:template match="tei:index"/>
-  <xsl:template match="tei:tagsDecl">
-    <tagsDecl>
-      <xsl:if test="child::tei:rendition[@xml:id='list-ndash'] and not(child::tei:rendition[@xml:id='list-ndash'])">
-        <rendition scheme="css" xml:id="list-disc">list-style-type:disc;</rendition>
-      </xsl:if>
+  <xsl:template match="tei:floatingText">
+    <floatingText>
+      <xsl:copy-of select="@* except(@type)"/>
       <xsl:apply-templates/>
-    </tagsDecl>
+    </floatingText>
   </xsl:template>
   <xsl:template match="tei:list[@rendition='#list-ndash']">
     <list>
       <xsl:copy-of select="@*"/>
       <xsl:attribute name="rendition">#list-disc</xsl:attribute>
       <xsl:apply-templates/>
     </list>
   </xsl:template>
+  <xsl:template match="tei:bibl[@type='sec_authority']">
+    <p rendition="#end">
+      <xsl:apply-templates select="descendant::text()|descendant::tei:hi"/>
+    </p>
+  </xsl:template>
+  <!-- ## TYPO ## -->
+  <xsl:template match="tei:hi[starts-with(@rend,'TEI_local')]">
+    <xsl:apply-templates select="node()"/>
+  </xsl:template>
   <!-- ## BACK ## -->
   <xsl:template match="tei:head[parent::tei:div[@type='bibliography']]|tei:head[parent::tei:div[@type='appendix']]"/>
   <xsl:template match="tei:div[@type='biographies']"/>
 </xsl:stylesheet>
```

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei_CERTIC.egg-info/PKG-INFO` & `doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc2tei-CERTIC
-Version: 0.0.94
+Version: 0.0.95
 Summary: Convert ODT and DOCX files to TEI
 Home-page: https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doc2tei-CERTIC-0.0.94/doc2tei_CERTIC.egg-info/SOURCES.txt` & `doc2tei-CERTIC-0.0.95/doc2tei_CERTIC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doc2tei-CERTIC-0.0.94/setup.py` & `doc2tei-CERTIC-0.0.95/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="doc2tei-CERTIC",
-    version="0.0.94",
+    version="0.0.95",
     author="Mickaël Desfrênes",
     author_email="mickael.desfrenes@unicaen.fr",
     description="Convert ODT and DOCX files to TEI",
     long_description="Convert ODT and DOCX files to TEI",
     long_description_content_type="text/plain",
     url="https://git.unicaen.fr/fnso/i-fair-ir/xsl-tei-circe",
     packages=setuptools.find_packages(),
```

