# Comparing `tmp/nonebot-plugin-hx-yinying-0.0.8.tar.gz` & `tmp/nonebot-plugin-hx-yinying-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.8.tar", last modified: Sun Apr 21 21:59:24 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.9.tar", last modified: Sun Apr 21 22:06:55 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-0.0.8.tar` & `nonebot-plugin-hx-yinying-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 21:59:23.987544 nonebot-plugin-hx-yinying-0.0.8/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3924 2024-04-21 21:59:23.988553 nonebot-plugin-hx-yinying-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3484 2024-04-21 21:01:59.000000 nonebot-plugin-hx-yinying-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 21:59:23.816561 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0     7340 2024-04-21 21:59:02.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    29062 2024-04-21 21:56:18.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      764 2024-04-21 21:59:08.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-21 21:59:23.980562 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     3924 2024-04-21 21:59:23.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-21 21:59:23.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 21:59:23.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2024-04-21 21:59:23.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-21 21:59:23.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-21 21:59:23.996739 nonebot-plugin-hx-yinying-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      840 2024-04-21 21:59:16.000000 nonebot-plugin-hx-yinying-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:06:55.329979 nonebot-plugin-hx-yinying-0.0.9/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3924 2024-04-21 22:06:55.633849 nonebot-plugin-hx-yinying-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3484 2024-04-21 21:01:59.000000 nonebot-plugin-hx-yinying-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 22:06:54.936848 nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0     7469 2024-04-21 22:06:03.000000 nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    29062 2024-04-21 21:56:18.000000 nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      764 2024-04-21 22:06:40.000000 nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-21 22:06:55.300214 nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     3924 2024-04-21 22:06:53.000000 nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-21 22:06:53.000000 nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 22:06:53.000000 nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2024-04-21 22:06:53.000000 nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-21 22:06:53.000000 nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-21 22:06:55.841719 nonebot-plugin-hx-yinying-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      840 2024-04-21 22:06:43.000000 nonebot-plugin-hx-yinying-0.0.9/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-0.0.8/LICENSE` & `nonebot-plugin-hx-yinying-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.8/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.0.8
+Version: 0.0.9
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.9 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-0.0.8/README.md` & `nonebot-plugin-hx-yinying-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Message,
     PrivateMessageEvent,
     Event,
 )
 from nonebot.log import default_filter, logger, logger_id, sys
 from nonebot.matcher import Matcher
 from nonebot.rule import to_me
-import json,datetime
+import json,datetime,os
 from nonebot.adapters.onebot.v11.event import PrivateMessageEvent, GroupMessageEvent
 from .chat import (
     get_id,
     get_answer_at,
     get_answer_ml,
     get_nick,
     send_msg,
@@ -33,20 +33,22 @@
     path_in,
     update_hx,
 )
 
 hx_config = get_plugin_config(Config)
 log_dir = path_in()
    
-if update_hx() <= hx_config.hx_version:
+new_verision = update_hx()
+if new_verision <= hx_config.hx_version:
     logger.success("你的Hx_YinYing已经是最新版本了！")
 else:
     logger.success("检查到Hx_YinYing有新版本！")
     logger.warning("【Hx】正在自动更新中")
-    main.main(['install', 'nonebot-plugin-hx-yinying'])
+    os.system(f'pip install nonebot-plugin-hx-yinying=={new_verision}')
+    logger.success(f"[Hx_YinYing]更新完成！当前版本为{new_verision}")
 
 __plugin_meta__ = PluginMetadata(
     name="Hx_YinYing",
     description="快来和可爱的赛博狼狼聊天！",
     usage=(
         "通过QQ艾特机器人来进行对话"
     ),
```

### Comparing `nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying/chat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import nonebot
 from pydantic import BaseModel
 
 
 class Config(BaseModel):
     # 插件版本号勿动！！！！
-    hx_version: Optional[str] = "0.0.8"
+    hx_version: Optional[str] = "0.0.9"
     # 你的appid
     yinying_appid: Optional[str] = None
     # model，如 yinying-v3
     yinying_model: Optional[str] = None
     furbar_model: Optional[str] = None
 
     yinying_token: Optional[str] = None
```

### Comparing `nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.9/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.0.8
+Version: 0.0.9
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.9 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-0.0.8/setup.py` & `nonebot-plugin-hx-yinying-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="0.0.8",
+    version="0.0.9",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

