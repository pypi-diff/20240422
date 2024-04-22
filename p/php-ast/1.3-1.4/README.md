# Comparing `tmp/php_ast-1.3.tar.gz` & `tmp/php_ast-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/php_ast-1.3.tar", last modified: Sat Apr 20 09:44:50 2024, max compression
+gzip compressed data, was "dist/php_ast-1.4.tar", last modified: Mon Apr 22 02:28:46 2024, max compression
```

## Comparing `php_ast-1.3.tar` & `php_ast-1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:44:50.000000 php_ast-1.3/
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-20 09:43:08.000000 php_ast-1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1339 2024-04-20 09:44:50.000000 php_ast-1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1019 2024-04-20 09:43:08.000000 php_ast-1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:44:50.000000 php_ast-1.3/php_ast/
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-20 09:43:08.000000 php_ast-1.3/php_ast/__init__.py
--rw-r--r--   0 root         (0) root         (0) 12946080 2024-04-20 09:43:08.000000 php_ast-1.3/php_ast/libphp7.so
--rw-r--r--   0 root         (0) root         (0)     3003 2024-04-20 09:43:08.000000 php_ast-1.3/php_ast/php_ast.py
--rw-r--r--   0 root         (0) root         (0)      166 2024-04-20 09:43:08.000000 php_ast-1.3/php_ast/php_ast_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:44:50.000000 php_ast-1.3/php_ast.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1339 2024-04-20 09:44:50.000000 php_ast-1.3/php_ast.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      249 2024-04-20 09:44:50.000000 php_ast-1.3/php_ast.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 09:44:50.000000 php_ast-1.3/php_ast.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-20 09:44:50.000000 php_ast-1.3/php_ast.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 09:44:50.000000 php_ast-1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      591 2024-04-20 09:43:48.000000 php_ast-1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 09:44:50.000000 php_ast-1.3/test/
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-20 09:43:08.000000 php_ast-1.3/test/test_ast.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:28:46.000000 php_ast-1.4/
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-20 07:29:24.000000 php_ast-1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-04-22 02:28:46.000000 php_ast-1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1684 2024-04-20 14:36:35.000000 php_ast-1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:28:46.000000 php_ast-1.4/php_ast/
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-20 08:35:57.000000 php_ast-1.4/php_ast/__init__.py
+-rw-r--r--   0 root         (0) root         (0) 12946080 2024-04-19 02:22:47.000000 php_ast-1.4/php_ast/libphp7.so
+-rw-r--r--   0 root         (0) root         (0)     3110 2024-04-22 02:26:28.000000 php_ast-1.4/php_ast/php_ast.py
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-22 02:28:03.000000 php_ast-1.4/php_ast/php_ast_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:28:46.000000 php_ast-1.4/php_ast.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-04-22 02:28:46.000000 php_ast-1.4/php_ast.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      249 2024-04-22 02:28:46.000000 php_ast-1.4/php_ast.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 02:28:46.000000 php_ast-1.4/php_ast.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-22 02:28:46.000000 php_ast-1.4/php_ast.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 02:28:46.000000 php_ast-1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      591 2024-04-22 02:28:28.000000 php_ast-1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:28:46.000000 php_ast-1.4/test/
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-20 08:01:47.000000 php_ast-1.4/test/test_ast.py
```

### Comparing `php_ast-1.3/LICENSE` & `php_ast-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `php_ast-1.3/PKG-INFO` & `php_ast-1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,47 @@
-Metadata-Version: 2.1
-Name: php_ast
-Version: 1.3
-Summary: A Python package for php_ast
-Home-page: https://github.com/php-ast/php_ast
-Author: php_ast
-Author-email: 20200120614@nxmu.edu.cn
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-#A Python Get PHP AST 
-
-
-#install 
-```bash
-    btpip install -i https://pypi.tuna.tsinghua.edu.cn/simple php-ast
-```
-
-
-#exapme 
-```Python
-# get phpinfo ast
-from php_ast import php_ast
-php_ast=php_ast()
-php_ast.get_ast(b"<?php phpinfo();?>")
-{'status': 'successed', 'ast': {'kind': 'AST_STMT_LIST', 'flags': 0, 'lineno': 1, 'children': [{'kind': 'AST_CALL', 'flags': 0, 'lineno': 1, 'children': {'expr': {'kind': 'AST_NAME', 'flags': 1, 'lineno': 1, 'children': {'name': 'phpinfo'}}, 'args': {'kind': 'AST_ARG_LIST', 'flags': 0, 'lineno': 1, 'children': []}}}]}}
-
-```
-
-```Python
-from php_ast import php_ast
-php_ast=php_ast()
-php_ast.get_file_ast("/home/11.php")
-{'status': 'successed', 'ast': {'kind': 'AST_STMT_LIST', 'flags': 0, 'lineno': 1, 'children': [{'kind': 'AST_CALL', 'flags': 0, 'lineno': 1, 'children': {'expr': {'kind': 'AST_NAME', 'flags': 1, 'lineno': 1, 'children': {'name': 'phpinfo'}}, 'args': {'kind': 'AST_ARG_LIST', 'flags': 0, 'lineno': 1, 'children': []}}}]}}
-
-```
-
-
-
+<h1 align="center">Python Get PHP-AST </h1>
+
+<div align="center">
+
+[![PHP-AST](https://img.shields.io/badge/php-ast-blue)](https://github.com/php-ast/php_ast)
+[![PHP](https://img.shields.io/badge/python_module-blue)](https://github.com/php-ast/php_ast)
+[![version](https://img.shields.io/github/v/release/php-ast/php_ast.svg?color=blue)](https://github.com/php-ast/php_ast)
+[![social](https://img.shields.io/github/stars/php-ast/php_ast?style=social)](https://github.com/php-ast/php_ast)
+</div>
+<p align="center">
+</p>
+
+## Install 
+```bash
+pip install  php-ast
+```
+
+
+## exapme 
+```Python
+# get bytes php code ast
+from php_ast import php_ast
+php_ast=php_ast()
+php_ast.get_ast(b"<?php phpinfo();?>")
+{'status': 'successed', 'ast': {'kind': 'AST_STMT_LIST', 'flags': 0, 'lineno': 1, 'children': [{'kind': 'AST_CALL', 'flags': 0, 'lineno': 1, 'children': {'expr': {'kind': 'AST_NAME', 'flags': 1, 'lineno': 1, 'children': {'name': 'phpinfo'}}, 'args': {'kind': 'AST_ARG_LIST', 'flags': 0, 'lineno': 1, 'children': []}}}]}}
+
+
+
+# get php file ast
+from php_ast import php_ast
+php_ast=php_ast()
+php_ast.get_file_ast("/home/11.php")
+{'status': 'successed', 'ast': {'kind': 'AST_STMT_LIST', 'flags': 0, 'lineno': 1, 'children': [{'kind': 'AST_CALL', 'flags': 0, 'lineno': 1, 'children': {'expr': {'kind': 'AST_NAME', 'flags': 1, 'lineno': 1, 'children': {'name': 'phpinfo'}}, 'args': {'kind': 'AST_ARG_LIST', 'flags': 0, 'lineno': 1, 'children': []}}}]}}
+
+```
+
+## 说明
+- 本项目是基于php-ast扩展的python模块，用于获取php代码的ast树
+- 暂时只支持Linux 系统 
+
+
+## 参考:
+- [php-ast](https://github.com/nikic/php-ast)
+
+
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `php_ast-1.3/php_ast/libphp7.so` & `php_ast-1.4/php_ast/libphp7.so`

 * *Files identical despite different names*

### Comparing `php_ast-1.3/php_ast/php_ast.py` & `php_ast-1.4/php_ast/php_ast.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,16 +60,19 @@
             data = json.loads(data_str)
         except:
             data = {"status": "success", "ast": {}}
         return data
 
     def get_file_ast(self, file_path):
         '''通过文件获取AST'''
-        with open(file_path, 'rb') as f:
-            src = f.read()
+        if os.path.exists(file_path) == False:
+            return {"status": "success", "ast": {}}
+        f=open(file_path, "rb")
+        src = f.read()
+        f.close()
         return self.get_ast(src)
 
     # 追踪AST
     def trace_ast(self, ast):
         '''追踪AST'''
         if ast is None:
             return
```

### Comparing `php_ast-1.3/setup.py` & `php_ast-1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="php_ast",
-    version="1.3",
+    version="1.4",
     packages=find_packages(),
     package_data={
         'php_ast': ['*.so'],
     },
     author="php_ast",
     author_email="20200120614@nxmu.edu.cn",
     description="A Python package for php_ast",
```

