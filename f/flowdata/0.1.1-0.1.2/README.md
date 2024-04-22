# Comparing `tmp/flowdata-0.1.1.tar.gz` & `tmp/flowdata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flowdata-0.1.1.tar", last modified: Sat Apr 20 13:56:18 2024, max compression
+gzip compressed data, was "dist/flowdata-0.1.2.tar", last modified: Sun Apr 21 03:44:55 2024, max compression
```

## Comparing `flowdata-0.1.1.tar` & `flowdata-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:56:18.000000 flowdata-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     2267 2024-04-20 13:56:18.000000 flowdata-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1398 2024-04-20 13:24:52.000000 flowdata-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata/
--rw-r--r--   0 root         (0) root         (0)      107 2024-04-20 13:02:13.000000 flowdata-0.1.1/flowdata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4184 2024-04-20 06:57:27.000000 flowdata-0.1.1/flowdata/_io.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-19 12:06:46.000000 flowdata-0.1.1/flowdata/_logger.py
--rw-r--r--   0 root         (0) root         (0)     3365 2024-04-20 12:48:40.000000 flowdata-0.1.1/flowdata/data_flow.py
--rw-r--r--   0 root         (0) root         (0)     2932 2024-04-20 12:49:07.000000 flowdata-0.1.1/flowdata/data_parallel.py
--rw-r--r--   0 root         (0) root         (0)     6187 2024-04-20 12:40:02.000000 flowdata-0.1.1/flowdata/decorator.py
--rw-r--r--   0 root         (0) root         (0)      651 2024-04-20 13:12:14.000000 flowdata-0.1.1/flowdata/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2267 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      379 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-20 13:56:18.000000 flowdata-0.1.1/flowdata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 13:56:18.000000 flowdata-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      684 2024-04-20 13:56:15.000000 flowdata-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 13:56:18.000000 flowdata-0.1.1/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 03:35:00.000000 flowdata-0.1.1/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-20 13:02:35.000000 flowdata-0.1.1/test/test_flow.py
--rw-r--r--   0 root         (0) root         (0)      884 2024-04-20 13:11:06.000000 flowdata-0.1.1/test/test_multitask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 03:44:55.000000 flowdata-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     2335 2024-04-21 03:44:55.000000 flowdata-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1466 2024-04-21 02:54:19.000000 flowdata-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 03:44:55.000000 flowdata-0.1.2/flowdata/
+-rw-r--r--   0 root         (0) root         (0)      107 2024-04-20 13:02:13.000000 flowdata-0.1.2/flowdata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4184 2024-04-20 06:57:27.000000 flowdata-0.1.2/flowdata/_io.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-19 12:06:46.000000 flowdata-0.1.2/flowdata/_logger.py
+-rw-r--r--   0 root         (0) root         (0)     3501 2024-04-21 03:41:45.000000 flowdata-0.1.2/flowdata/data_flow.py
+-rw-r--r--   0 root         (0) root         (0)     2931 2024-04-21 03:02:04.000000 flowdata-0.1.2/flowdata/data_parallel.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2024-04-20 12:40:02.000000 flowdata-0.1.2/flowdata/decorator.py
+-rw-r--r--   0 root         (0) root         (0)      809 2024-04-21 03:33:07.000000 flowdata-0.1.2/flowdata/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 03:44:55.000000 flowdata-0.1.2/flowdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2335 2024-04-21 03:44:55.000000 flowdata-0.1.2/flowdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2024-04-21 03:44:55.000000 flowdata-0.1.2/flowdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 03:44:55.000000 flowdata-0.1.2/flowdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-21 03:44:55.000000 flowdata-0.1.2/flowdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-21 03:44:55.000000 flowdata-0.1.2/flowdata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-21 03:44:55.000000 flowdata-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      685 2024-04-21 03:41:49.000000 flowdata-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 03:44:55.000000 flowdata-0.1.2/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-20 03:35:00.000000 flowdata-0.1.2/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-21 03:41:25.000000 flowdata-0.1.2/test/test_flow.py
+-rw-r--r--   0 root         (0) root         (0)      884 2024-04-21 02:48:07.000000 flowdata-0.1.2/test/test_multitask.py
```

### Comparing `flowdata-0.1.1/PKG-INFO` & `flowdata-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: 流式数据简易处理包
 Home-page: https://github.com/zouweidong91/flowdata
 Author: zouweidong
 Author-email: zouweidong72@gmail.com
 License: UNKNOWN
 Description: # flowdata
         流式数据简易处理工具
@@ -21,15 +21,15 @@
         
         # Quick Start
         
         ## 1、单任务
         代码中通过add_task将任务加载到任务流中，且可以根据需要指定不同进程数量
         
         ```python
-        
+        import time
         from flowdata import FlowBase
         from flowdata import add_task
         
         class TaskFlow(FlowBase):
             @add_task(work_num=1)
             def task(self, item: dict, *args, **kwargs) -> dict:
                 time.sleep(.2)
@@ -43,18 +43,18 @@
             def save_data(self, item_iter):
                 list(item_iter)
         
         TaskFlow().main()
         ```
         
         ## 2、多任务
-        假设一个处理数据的任务可以细分为多个子任务，例如，task_a, task_b。
+        假设一个处理数据的任务可以细分为多个子任务，例如，task_a, task_b。任务执行按照task的添加顺序执行。
         
         ```python
-        
+        import time
         from flowdata import FlowBase
         from flowdata import add_task
         
         # 多个任务
         class TaskFlow(FlowBase):
             @add_task(work_num=2)
             def task_a(self, item: dict, *args, **kwargs) -> dict:
```

### Comparing `flowdata-0.1.1/README.md` & `flowdata-0.1.2/test/test_multitask.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,44 @@
-# flowdata
-流式数据简易处理工具
-
-本项目支持对流式数据的处理进行多进程加速
-
-
-# 安装 flowdata
-
-```
-pip install flowdata
-```
-
-
-# Quick Start
-
-## 1、单任务
-代码中通过add_task将任务加载到任务流中，且可以根据需要指定不同进程数量
-
-```python
-
-from flowdata import FlowBase
-from flowdata import add_task
-
-class TaskFlow(FlowBase):
-    @add_task(work_num=1)
-    def task(self, item: dict, *args, **kwargs) -> dict:
-        time.sleep(.2)
-        item['id'] += 1
-        return item
-
-    def get_data(self):
-        for i in range(20):
-            yield {"id": i}
-
-    def save_data(self, item_iter):
-        list(item_iter)
-
-TaskFlow().main()
-```
-
-## 2、多任务
-假设一个处理数据的任务可以细分为多个子任务，例如，task_a, task_b。
-
-```python
+import time
+import unittest
 
 from flowdata import FlowBase
+from flowdata.decorator import err_catch
 from flowdata import add_task
 
 # 多个任务
 class TaskFlow(FlowBase):
+    
+    @err_catch()
     @add_task(work_num=2)
-    def task_a(self, item: dict, *args, **kwargs) -> dict:
+    def task_1(self, item: dict, *args, **kwargs) -> dict:
         time.sleep(.2)
         item['id'] += 1
+        if item['id'] == 5:
+            raise Exception("ha")
         return item
 
+    
+    @err_catch()
     @add_task(work_num=2)
-    def task_b(self, item: dict, *args, **kwargs) -> dict:
+    def task_2(self, item: dict, *args, **kwargs) -> dict:
         time.sleep(.2)
         item['id'] += 1
         return item
 
+
     def get_data(self):
         for i in range(20):
             yield {"id": i}
 
+
     def save_data(self, item_iter):
         list(item_iter)
+        
+
+class FlowTest(unittest.TestCase):
+    def test_flow(self):
+        TaskFlow(verbose=True).main()
+
 
-TaskFlow().main()
-```
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `flowdata-0.1.1/flowdata/_io.py` & `flowdata-0.1.2/flowdata/_io.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.1/flowdata/_logger.py` & `flowdata-0.1.2/flowdata/_logger.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.1/flowdata/data_flow.py` & `flowdata-0.1.2/flowdata/data_flow.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 """
 通用跑数任务流
 """
 
 from collections import Counter
 from typing import Generator
 
-from flowdata.task import Task, add_task, TASK_LIST
-
 from ._logger import logger
 from .data_parallel import DataParallel
-from .decorator import err_catch, timer, tps, interrupt_catch
-
+from .decorator import err_catch, interrupt_catch, timer, tps
+from .task import TASK_LIST, Task
 
 
 class FlowBase:
     def __init__(self, verbose=True):
         self.verbose = verbose
         self.counter = Counter()
 
@@ -75,20 +73,14 @@
         task_func = getattr(self, task.func_name)
         item_iter_fn = lambda: item_iter
         with DataParallel(item_iter_fn=item_iter_fn, work_num=task.work_num, process_fn=task_func) as t:
             for index, item in enumerate(t.send_data()):
                 yield item
 
 
-    @add_task(work_num=1)
-    @err_catch()
-    def process_fn(self, item: dict, *args, **kwargs) -> dict:
-        return item
-
-    
     def exec_task(self, item_iter, task:Task):
         """执行单task
         """
         if task.work_num > 1:
             item_iter = self._exec_mp(item_iter, task)
         else:
             item_iter = self._exec(item_iter, task)
@@ -96,30 +88,39 @@
         return item_iter
 
 
     def exec_tasks(self, item_iter):
         """执行多task， TASK_LIST中上一个task的输出是下一个task的输入
         """
         for task in TASK_LIST:
-            if not hasattr(self, task.func_name):
-                continue
+            if task.class_name!=self.__class__.__name__: continue
+            if not hasattr(self, task.func_name): continue
             item_iter = self.exec_task(item_iter, task)
 
         return item_iter
 
 
+    def print_task(self):
+        num = 0
+        for task in TASK_LIST:
+            if task.class_name!=self.__class__.__name__: continue
+            num += 1
+            logger.info("task_%s: %s", num, task)
+
+
     @timer("main")
     @interrupt_catch
     def main(self, offset:int=0, head_num:int=None):
         """主函数
 
         Args:
             offset (int, optional): 偏移量. Defaults to 0.
             head_num (int, optional): 要跑的数据总量. Defaults to None.
         """
+        self.print_task()
         item_iter = self.get_data()
         item_iter = self.clip_data(item_iter, offset, head_num)
         item_iter = self.exec_tasks(item_iter)
         item_iter = self.count_data(item_iter)
         self.save_data(item_iter)
         
         print()
```

### Comparing `flowdata-0.1.1/flowdata/data_parallel.py` & `flowdata-0.1.2/flowdata/data_parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         while True:
             data = self.pip_out.get(block=True, timeout=None)
             if data == FLAG.END:
                 break
             yield data
       
 
-
     @interrupt_catch
     def work(self, work_done_value, work_i:int):
         """[summary]
 
         Args:
             work_done_value ([type]): [跟踪子进程是否结束]
             work_i ([int]): [进程索引id，外部任务可能用到]
```

### Comparing `flowdata-0.1.1/flowdata/decorator.py` & `flowdata-0.1.2/flowdata/decorator.py`

 * *Files identical despite different names*

### Comparing `flowdata-0.1.1/flowdata.egg-info/PKG-INFO` & `flowdata-0.1.2/flowdata.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: 流式数据简易处理包
 Home-page: https://github.com/zouweidong91/flowdata
 Author: zouweidong
 Author-email: zouweidong72@gmail.com
 License: UNKNOWN
 Description: # flowdata
         流式数据简易处理工具
@@ -21,15 +21,15 @@
         
         # Quick Start
         
         ## 1、单任务
         代码中通过add_task将任务加载到任务流中，且可以根据需要指定不同进程数量
         
         ```python
-        
+        import time
         from flowdata import FlowBase
         from flowdata import add_task
         
         class TaskFlow(FlowBase):
             @add_task(work_num=1)
             def task(self, item: dict, *args, **kwargs) -> dict:
                 time.sleep(.2)
@@ -43,18 +43,18 @@
             def save_data(self, item_iter):
                 list(item_iter)
         
         TaskFlow().main()
         ```
         
         ## 2、多任务
-        假设一个处理数据的任务可以细分为多个子任务，例如，task_a, task_b。
+        假设一个处理数据的任务可以细分为多个子任务，例如，task_a, task_b。任务执行按照task的添加顺序执行。
         
         ```python
-        
+        import time
         from flowdata import FlowBase
         from flowdata import add_task
         
         # 多个任务
         class TaskFlow(FlowBase):
             @add_task(work_num=2)
             def task_a(self, item: dict, *args, **kwargs) -> dict:
```

### Comparing `flowdata-0.1.1/setup.py` & `flowdata-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 NAME = 'flowdata'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = '流式数据简易处理包'
 EMAIL = 'zouweidong72@gmail.com'
 AUTHOR = 'zouweidong'
 
 
 setup(
     name=NAME,
@@ -22,8 +22,8 @@
     long_description=long_description, 
     long_description_content_type='text/markdown',
     url='https://github.com/zouweidong91/flowdata',
     python_requires='>=3.6',
     install_requires=[
     'pandas'
 ],
-)
+)
```

### Comparing `flowdata-0.1.1/test/test_flow.py` & `flowdata-0.1.2/test/test_flow.py`

 * *Files identical despite different names*

