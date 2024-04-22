# Comparing `tmp/PySqlModel-1.1.3.tar.gz` & `tmp/PySqlModel-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySqlModel-1.1.3.tar", last modified: Fri Apr 19 15:44:15 2024, max compression
+gzip compressed data, was "dist\PySqlModel-1.1.4.tar", last modified: Mon Apr 22 01:39:10 2024, max compression
```

## Comparing `PySqlModel-1.1.3.tar` & `PySqlModel-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 15:44:15.000000 PySqlModel-1.1.3/
--rw-rw-rw-   0        0        0     1524 2024-04-19 14:25:02.000000 PySqlModel-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      388 2024-04-19 15:44:15.000000 PySqlModel-1.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 15:44:15.000000 PySqlModel-1.1.3/PySqlModel/
--rw-rw-rw-   0        0        0      123 2024-04-19 13:01:04.000000 PySqlModel-1.1.3/PySqlModel/__init__.py
--rw-rw-rw-   0        0        0       94 2023-05-09 17:36:37.000000 PySqlModel-1.1.3/PySqlModel/base.py
--rw-rw-rw-   0        0        0    11457 2024-04-19 15:43:49.000000 PySqlModel-1.1.3/PySqlModel/mysql.py
--rw-rw-rw-   0        0        0    10832 2024-04-19 15:43:49.000000 PySqlModel-1.1.3/PySqlModel/sqlite.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:44:15.000000 PySqlModel-1.1.3/PySqlModel.egg-info/
--rw-rw-rw-   0        0        0      388 2024-04-19 15:44:15.000000 PySqlModel-1.1.3/PySqlModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-04-19 15:44:15.000000 PySqlModel-1.1.3/PySqlModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 15:44:15.000000 PySqlModel-1.1.3/PySqlModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-19 15:44:15.000000 PySqlModel-1.1.3/PySqlModel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-19 15:44:15.000000 PySqlModel-1.1.3/PySqlModel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6974 2024-04-19 14:15:02.000000 PySqlModel-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 15:44:15.000000 PySqlModel-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      805 2024-04-19 15:43:59.000000 PySqlModel-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 01:39:10.000000 PySqlModel-1.1.4/
+-rw-rw-rw-   0        0        0     1524 2024-04-22 01:10:19.000000 PySqlModel-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      433 2024-04-22 01:39:10.000000 PySqlModel-1.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-22 01:39:10.000000 PySqlModel-1.1.4/PySqlModel/
+-rw-rw-rw-   0        0        0      123 2024-04-22 01:10:19.000000 PySqlModel-1.1.4/PySqlModel/__init__.py
+-rw-rw-rw-   0        0        0       94 2024-04-22 01:10:19.000000 PySqlModel-1.1.4/PySqlModel/base.py
+-rw-rw-rw-   0        0        0    11457 2024-04-22 01:10:19.000000 PySqlModel-1.1.4/PySqlModel/mysql.py
+-rw-rw-rw-   0        0        0    10832 2024-04-22 01:10:19.000000 PySqlModel-1.1.4/PySqlModel/sqlite.py
+drwxrwxrwx   0        0        0        0 2024-04-22 01:39:10.000000 PySqlModel-1.1.4/PySqlModel.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-04-22 01:39:10.000000 PySqlModel-1.1.4/PySqlModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-22 01:39:10.000000 PySqlModel-1.1.4/PySqlModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 01:39:10.000000 PySqlModel-1.1.4/PySqlModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-22 01:39:10.000000 PySqlModel-1.1.4/PySqlModel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6974 2024-04-22 01:10:19.000000 PySqlModel-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 01:39:10.000000 PySqlModel-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      842 2024-04-22 01:24:57.000000 PySqlModel-1.1.4/setup.py
```

### Comparing `PySqlModel-1.1.3/LICENSE` & `PySqlModel-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PySqlModel-1.1.3/PySqlModel/mysql.py` & `PySqlModel-1.1.4/PySqlModel/mysql.py`

 * *Files identical despite different names*

### Comparing `PySqlModel-1.1.3/PySqlModel/sqlite.py` & `PySqlModel-1.1.4/PySqlModel/sqlite.py`

 * *Files identical despite different names*

### Comparing `PySqlModel-1.1.3/README.md` & `PySqlModel-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `PySqlModel-1.1.3/setup.py` & `PySqlModel-1.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 @Author:函封封
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="PySqlModel",
-    version="1.1.3",
+    version="1.1.4",
     author="HanFengFeng",
     author_email="mr_jia_han@qq.com",
     description="简单方便的数据库查询包",
     # 项目主页
     url="https://github.com/NeverStopDreamingWang/pysqlmodel",
     # 你要安装的包，通过 setuptools.find_packages 找到当前目录下有哪些包
     packages=find_packages(),
-    install_requires=[
-        "pymysql",
-        "sqlite3"
-    ],
+    python_requires='>=3',
+    install_requires=[],
+    license="BSD 3-Clause",
     project_urls={
         "github": "https://github.com/NeverStopDreamingWang/pysqlmodel",
         "gitee": "https://gitee.com/NeverStopDreamingWang/pysqlmodel",
     }
 )
 
+# python setup.py check
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
```

