# Comparing `tmp/bioomics-0.2.1.tar.gz` & `tmp/bioomics-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioomics-0.2.1.tar", last modified: Sat Apr 20 16:14:25 2024, max compression
+gzip compressed data, was "bioomics-0.2.2.tar", last modified: Mon Apr 22 00:54:50 2024, max compression
```

## Comparing `bioomics-0.2.1.tar` & `bioomics-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:14:25.689643 bioomics-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-20 16:14:21.000000 bioomics-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-20 16:14:25.689643 bioomics-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-20 16:14:21.000000 bioomics-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 16:14:25.689643 bioomics-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-20 16:14:21.000000 bioomics-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:14:25.681643 bioomics-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:14:25.685643 bioomics-0.2.1/src/bioomics/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:14:25.689643 bioomics-0.2.1/src/bioomics/connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/connector/conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/connector/conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/connector/conn_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/connector/conn_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/iedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/iedb_antigen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/iedb_epitope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/integrate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-20 16:14:21.000000 bioomics-0.2.1/src/bioomics/rnacentral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:14:25.689643 bioomics-0.2.1/src/bioomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-20 16:14:25.000000 bioomics-0.2.1/src/bioomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-20 16:14:25.000000 bioomics-0.2.1/src/bioomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 16:14:25.000000 bioomics-0.2.1/src/bioomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-20 16:14:25.000000 bioomics-0.2.1/src/bioomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 16:14:25.000000 bioomics-0.2.1/src/bioomics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:14:25.689643 bioomics-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-20 16:14:21.000000 bioomics-0.2.1/tests/test_conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-20 16:14:21.000000 bioomics-0.2.1/tests/test_conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-20 16:14:21.000000 bioomics-0.2.1/tests/test_conn_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-20 16:14:21.000000 bioomics-0.2.1/tests/test_conn_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-20 16:14:21.000000 bioomics-0.2.1/tests/test_expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 16:14:21.000000 bioomics-0.2.1/tests/test_iedb.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-20 16:14:21.000000 bioomics-0.2.1/tests/test_iedb_antigen.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-20 16:14:21.000000 bioomics-0.2.1/tests/test_iedb_epitope.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-20 16:14:21.000000 bioomics-0.2.1/tests/test_mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-20 16:14:21.000000 bioomics-0.2.1/tests/test_ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-20 16:14:21.000000 bioomics-0.2.1/tests/test_rnacentral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:54:50.246094 bioomics-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 00:54:46.000000 bioomics-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-22 00:54:50.246094 bioomics-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-22 00:54:46.000000 bioomics-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 00:54:50.246094 bioomics-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-22 00:54:46.000000 bioomics-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:54:50.238094 bioomics-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:54:50.242094 bioomics-0.2.2/src/bioomics/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:54:50.242094 bioomics-0.2.2/src/bioomics/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/connector/conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/connector/conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/connector/conn_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/connector/conn_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:54:50.242094 bioomics-0.2.2/src/bioomics/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/constants/IEDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/iedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/iedb_antigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/iedb_epitope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/integrate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-22 00:54:46.000000 bioomics-0.2.2/src/bioomics/rnacentral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:54:50.246094 bioomics-0.2.2/src/bioomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-22 00:54:50.000000 bioomics-0.2.2/src/bioomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-22 00:54:50.000000 bioomics-0.2.2/src/bioomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 00:54:50.000000 bioomics-0.2.2/src/bioomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 00:54:50.000000 bioomics-0.2.2/src/bioomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 00:54:50.000000 bioomics-0.2.2/src/bioomics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:54:50.246094 bioomics-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-22 00:54:46.000000 bioomics-0.2.2/tests/test_conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-22 00:54:46.000000 bioomics-0.2.2/tests/test_conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-22 00:54:46.000000 bioomics-0.2.2/tests/test_conn_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-22 00:54:46.000000 bioomics-0.2.2/tests/test_conn_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-22 00:54:46.000000 bioomics-0.2.2/tests/test_expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-22 00:54:46.000000 bioomics-0.2.2/tests/test_iedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-22 00:54:46.000000 bioomics-0.2.2/tests/test_iedb_antigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-22 00:54:46.000000 bioomics-0.2.2/tests/test_iedb_epitope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 00:54:46.000000 bioomics-0.2.2/tests/test_mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-22 00:54:46.000000 bioomics-0.2.2/tests/test_ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-22 00:54:46.000000 bioomics-0.2.2/tests/test_rnacentral.py
```

### Comparing `bioomics-0.2.1/LICENSE` & `bioomics-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/PKG-INFO` & `bioomics-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.2.1
+Version: 0.2.2
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `bioomics-0.2.1/README.md` & `bioomics-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/setup.py` & `bioomics-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="bioomics",
-    version='0.2.1',
+    version='0.2.2',
     author="Tiezheng Yuan",
     author_email="tiezhengyuan@hotmail.com",
     description="Download, retrieve and process omics data for further bioinformatics",
     url = "https://github.com/Tiezhengyuan/bio_omics",
     long_description_content_type="text/markdown",
     long_description=long_description,
     package_dir={"": "src"},
```

### Comparing `bioomics-0.2.1/src/bioomics/__init__.py` & `bioomics-0.2.2/src/bioomics/__init__.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/src/bioomics/connector/conn_ftp.py` & `bioomics-0.2.2/src/bioomics/connector/conn_ftp.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/src/bioomics/connector/conn_ftplib.py` & `bioomics-0.2.2/src/bioomics/connector/conn_ftplib.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/src/bioomics/connector/conn_http.py` & `bioomics-0.2.2/src/bioomics/connector/conn_http.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/src/bioomics/connector/conn_redis.py` & `bioomics-0.2.2/src/bioomics/connector/conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/src/bioomics/expasy.py` & `bioomics-0.2.2/src/bioomics/expasy.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/src/bioomics/integrate_data.py` & `bioomics-0.2.2/src/bioomics/integrate_data.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/src/bioomics/mirbase.py` & `bioomics-0.2.2/src/bioomics/mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/src/bioomics/ncbi.py` & `bioomics-0.2.2/src/bioomics/ncbi.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/src/bioomics/rnacentral.py` & `bioomics-0.2.2/src/bioomics/rnacentral.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/src/bioomics.egg-info/PKG-INFO` & `bioomics-0.2.2/src/bioomics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.2.1
+Version: 0.2.2
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `bioomics-0.2.1/src/bioomics.egg-info/SOURCES.txt` & `bioomics-0.2.2/src/bioomics.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/bioomics.egg-info/requires.txt
 src/bioomics.egg-info/top_level.txt
 src/bioomics/connector/__init__.py
 src/bioomics/connector/conn_ftp.py
 src/bioomics/connector/conn_ftplib.py
 src/bioomics/connector/conn_http.py
 src/bioomics/connector/conn_redis.py
+src/bioomics/constants/IEDB.py
 tests/test_conn_ftp.py
 tests/test_conn_ftplib.py
 tests/test_conn_http.py
 tests/test_conn_redis.py
 tests/test_expasy.py
 tests/test_iedb.py
 tests/test_iedb_antigen.py
```

### Comparing `bioomics-0.2.1/tests/test_conn_ftp.py` & `bioomics-0.2.2/tests/test_conn_ftp.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/tests/test_conn_ftplib.py` & `bioomics-0.2.2/tests/test_conn_ftplib.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/tests/test_conn_http.py` & `bioomics-0.2.2/tests/test_conn_http.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/tests/test_conn_redis.py` & `bioomics-0.2.2/tests/test_conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/tests/test_mirbase.py` & `bioomics-0.2.2/tests/test_mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/tests/test_ncbi.py` & `bioomics-0.2.2/tests/test_ncbi.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.1/tests/test_rnacentral.py` & `bioomics-0.2.2/tests/test_rnacentral.py`

 * *Files identical despite different names*

