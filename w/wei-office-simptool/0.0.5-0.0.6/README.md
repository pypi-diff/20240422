# Comparing `tmp/wei_office_simptool-0.0.5.tar.gz` & `tmp/wei_office_simptool-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wei_office_simptool-0.0.5.tar", last modified: Sat Apr 20 02:04:22 2024, max compression
+gzip compressed data, was "wei_office_simptool-0.0.6.tar", last modified: Mon Apr 22 06:38:11 2024, max compression
```

## Comparing `wei_office_simptool-0.0.5.tar` & `wei_office_simptool-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 02:04:22.584656 wei_office_simptool-0.0.5/
--rw-rw-rw-   0        0        0     4893 2024-04-20 02:04:22.583656 wei_office_simptool-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4092 2024-04-19 08:30:50.000000 wei_office_simptool-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 02:04:22.585828 wei_office_simptool-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2483 2024-04-20 02:04:13.000000 wei_office_simptool-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 02:04:22.564491 wei_office_simptool-0.0.5/tests/
--rw-rw-rw-   0        0        0     1359 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0     2101 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.5/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 02:04:22.568545 wei_office_simptool-0.0.5/wei_office_simptool/
--rw-rw-rw-   0        0        0     1669 2024-04-19 08:47:36.000000 wei_office_simptool-0.0.5/wei_office_simptool/__init__.py
--rw-rw-rw-   0        0        0    14313 2024-04-20 01:37:53.000000 wei_office_simptool-0.0.5/wei_office_simptool/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-20 02:04:22.578535 wei_office_simptool-0.0.5/wei_office_simptool.egg-info/
--rw-rw-rw-   0        0        0     4893 2024-04-20 02:04:22.000000 wei_office_simptool-0.0.5/wei_office_simptool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-04-20 02:04:22.000000 wei_office_simptool-0.0.5/wei_office_simptool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 02:04:22.000000 wei_office_simptool-0.0.5/wei_office_simptool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-20 02:04:22.000000 wei_office_simptool-0.0.5/wei_office_simptool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-20 02:04:22.000000 wei_office_simptool-0.0.5/wei_office_simptool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 06:38:11.539742 wei_office_simptool-0.0.6/
+-rw-rw-rw-   0        0        0     5306 2024-04-22 06:38:11.537740 wei_office_simptool-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4490 2024-04-22 05:51:50.000000 wei_office_simptool-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 06:38:11.539742 wei_office_simptool-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2498 2024-04-22 06:36:05.000000 wei_office_simptool-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:38:11.518736 wei_office_simptool-0.0.6/tests/
+-rw-rw-rw-   0        0        0     1359 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     2101 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.6/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:38:11.523738 wei_office_simptool-0.0.6/wei_office_simptool/
+-rw-rw-rw-   0        0        0     1669 2024-04-19 08:47:36.000000 wei_office_simptool-0.0.6/wei_office_simptool/__init__.py
+-rw-rw-rw-   0        0        0    15251 2024-04-22 05:51:50.000000 wei_office_simptool-0.0.6/wei_office_simptool/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:38:11.535750 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/
+-rw-rw-rw-   0        0        0     5306 2024-04-22 06:38:11.000000 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-04-22 06:38:11.000000 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 06:38:11.000000 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-22 06:38:11.000000 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-22 06:38:11.000000 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/top_level.txt
```

### Comparing `wei_office_simptool-0.0.5/PKG-INFO` & `wei_office_simptool-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wei_office_simptool
-Version: 0.0.5
-Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换等常见功能,实现1到3行代码完成相关处理的快捷操作。
+Version: 0.0.6
+Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。
 Home-page: https://github.com/phoenixlucky/wei_office_simptool
 Author: Ethan Wilkins
 Author-email: thisluckyboy@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -16,15 +16,15 @@
 Requires-Dist: datetime
 Requires-Dist: openpyxl
 Requires-Dist: toml
 Requires-Dist: mysql-connector-python
 
 # wei_office_simptool
 
-`wei_office_simptool` 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换等常见功能,实现1到3行代码完成相关处理的快捷操作。
+`wei_office_simptool` 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。
 
 ## 安装
 
 使用以下命令安装 `wei_office_simptool`：
 
 ```bash
 pip install wei_office_simptool
@@ -108,15 +108,28 @@
 用于获取最近的时间处理。
 
 ```bash
 from wei_office_simptool import eConstant
 
 # 示例代码
 #timeclass:1日期 2时间戳 3时刻
-interval_time = eConstant(interval_day,timeclass).get_timeparameter()
+#获取当日的日期字符串
+x=eConstant(interval_day=0,timeclass=1).get_timeparameter(Format="%Y-%m-%d")
+print(x)
+```
+
+## 5 FileManagement 类
+用于文件移动并且重命名。
+```bash
+#latest_folder2 当前目录
+#destination_directory 目标目录
+#target_files2 文件名
+#add_prefix 重命名去除数字
+#file_type 文件类型
+copy_files(latest_folder2, destination_directory, target_files2, rename=add_prefix,file_type="xls")
 ```
 
 ## 贡献
 #### 有任何问题或建议，请提出 issue。欢迎贡献代码！
 
 Copyright (c) 2024 The Python Packaging Authority
```

### Comparing `wei_office_simptool-0.0.5/README.md` & `wei_office_simptool-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # wei_office_simptool
 
-`wei_office_simptool` 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换等常见功能,实现1到3行代码完成相关处理的快捷操作。
+`wei_office_simptool` 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。
 
 ## 安装
 
 使用以下命令安装 `wei_office_simptool`：
 
 ```bash
 pip install wei_office_simptool
@@ -88,15 +88,28 @@
 用于获取最近的时间处理。
 
 ```bash
 from wei_office_simptool import eConstant
 
 # 示例代码
 #timeclass:1日期 2时间戳 3时刻
-interval_time = eConstant(interval_day,timeclass).get_timeparameter()
+#获取当日的日期字符串
+x=eConstant(interval_day=0,timeclass=1).get_timeparameter(Format="%Y-%m-%d")
+print(x)
+```
+
+## 5 FileManagement 类
+用于文件移动并且重命名。
+```bash
+#latest_folder2 当前目录
+#destination_directory 目标目录
+#target_files2 文件名
+#add_prefix 重命名去除数字
+#file_type 文件类型
+copy_files(latest_folder2, destination_directory, target_files2, rename=add_prefix,file_type="xls")
 ```
 
 ## 贡献
 #### 有任何问题或建议，请提出 issue。欢迎贡献代码！
 
 Copyright (c) 2024 The Python Packaging Authority
```

### Comparing `wei_office_simptool-0.0.5/setup.py` & `wei_office_simptool-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 @email:thisluckyboy@126.com
 """
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='wei_office_simptool',
-    version='0.0.5',
+    version='0.0.6',
     author="Ethan Wilkins",
     author_email="thisluckyboy@126.com",
-    description="一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换等常见功能,实现1到3行代码完成相关处理的快捷操作。",  # 包的简述
+    description="一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。",  # 包的简述
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phoenixlucky/wei_office_simptool",
     packages=find_packages(),
     install_requires=[
         'pathlib',
         'pandas',
```

### Comparing `wei_office_simptool-0.0.5/tests/__init__.py` & `wei_office_simptool-0.0.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.5/tests/test_utils.py` & `wei_office_simptool-0.0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.5/wei_office_simptool/__init__.py` & `wei_office_simptool-0.0.6/wei_office_simptool/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.5/wei_office_simptool/utils.py` & `wei_office_simptool-0.0.6/wei_office_simptool/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 @date:2023/12/3
 @time:17:33
 @month:十二月
 @email:thisluckyboy@126.com
 """
 import base64
 import datetime
+import os
 import pathlib
+import re
+import shutil
 import smtplib
 import time
 from contextlib import contextmanager
 from email.header import Header
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from functools import wraps
@@ -162,14 +165,33 @@
             elif operation_mode == "c":
                 self.callsql(sql)
             elif operation_mode == "wm":
                 self.writesqlmany(sql, purchases)
         else:
             return self.to_df(sql)
 
+class FileManagement:
+    def __init__(self):
+        pass
+
+    def add_prefix(self,filename,file_type):
+        pattern = r'[\u4e00-\u9fa5]+'
+        matches = re.findall(pattern, filename)[0]
+        return f"{matches}.{file_type}"
+    def copy_files(self,src_dir, dest_dir, target_files, rename=None,file_type="xls"):
+        for target_file in target_files:
+            source_path = os.path.join(src_dir, target_file)
+            destination_file = rename(target_file,file_type) if rename else target_file
+            destination_path = os.path.join(dest_dir, destination_file)
+            if os.path.exists(source_path):
+                shutil.copy(source_path, destination_path)
+                print(f"File {target_file} copied from {source_path} to {destination_path}")
+            else:
+                print(f"Source file {target_file} not found in the latest folder.")
+
 class MySQLDatabase:
     def __init__(self, config):
         self.config = config
         self.connection = None
         self.connect()
 
     def connect(self):
```

### Comparing `wei_office_simptool-0.0.5/wei_office_simptool.egg-info/PKG-INFO` & `wei_office_simptool-0.0.6/wei_office_simptool.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wei_office_simptool
-Version: 0.0.5
-Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换等常见功能,实现1到3行代码完成相关处理的快捷操作。
+Version: 0.0.6
+Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。
 Home-page: https://github.com/phoenixlucky/wei_office_simptool
 Author: Ethan Wilkins
 Author-email: thisluckyboy@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -16,15 +16,15 @@
 Requires-Dist: datetime
 Requires-Dist: openpyxl
 Requires-Dist: toml
 Requires-Dist: mysql-connector-python
 
 # wei_office_simptool
 
-`wei_office_simptool` 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换等常见功能,实现1到3行代码完成相关处理的快捷操作。
+`wei_office_simptool` 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。
 
 ## 安装
 
 使用以下命令安装 `wei_office_simptool`：
 
 ```bash
 pip install wei_office_simptool
@@ -108,15 +108,28 @@
 用于获取最近的时间处理。
 
 ```bash
 from wei_office_simptool import eConstant
 
 # 示例代码
 #timeclass:1日期 2时间戳 3时刻
-interval_time = eConstant(interval_day,timeclass).get_timeparameter()
+#获取当日的日期字符串
+x=eConstant(interval_day=0,timeclass=1).get_timeparameter(Format="%Y-%m-%d")
+print(x)
+```
+
+## 5 FileManagement 类
+用于文件移动并且重命名。
+```bash
+#latest_folder2 当前目录
+#destination_directory 目标目录
+#target_files2 文件名
+#add_prefix 重命名去除数字
+#file_type 文件类型
+copy_files(latest_folder2, destination_directory, target_files2, rename=add_prefix,file_type="xls")
 ```
 
 ## 贡献
 #### 有任何问题或建议，请提出 issue。欢迎贡献代码！
 
 Copyright (c) 2024 The Python Packaging Authority
```

