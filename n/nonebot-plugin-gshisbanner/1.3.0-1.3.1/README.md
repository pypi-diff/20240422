# Comparing `tmp/nonebot_plugin_gshisbanner-1.3.0.tar.gz` & `tmp/nonebot_plugin_gshisbanner-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gshisbanner-1.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_gshisbanner-1.3.1.tar", max compression
```

## Comparing `nonebot_plugin_gshisbanner-1.3.0.tar` & `nonebot_plugin_gshisbanner-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1067 2024-04-22 06:48:19.556158 nonebot_plugin_gshisbanner-1.3.0/LICENSE
--rw-r--r--   0        0        0     5920 2024-04-22 06:48:19.556158 nonebot_plugin_gshisbanner-1.3.0/README.md
--rw-r--r--   0        0        0     1320 2024-04-22 06:48:19.556158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/__init__.py
--rw-r--r--   0        0        0      426 2024-04-22 06:48:19.556158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/adapters/__init__.py
--rw-r--r--   0        0        0     4816 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/adapters/ob11.py
--rw-r--r--   0        0        0     4806 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/adapters/red.py
--rw-r--r--   0        0        0      990 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/alias.py
--rw-r--r--   0        0        0      428 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/api.py
--rw-r--r--   0        0        0      577 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/config.py
--rw-r--r--   0        0        0      458 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/constant.py
--rw-r--r--   0        0        0     3876 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/deal.py
--rw-r--r--   0        0        0     1192 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/deal_json.py
--rw-r--r--   0        0        0     3765 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/draw.py
--rw-r--r--   0        0        0     1515 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/model.py
--rw-r--r--   0        0        0     2580 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/send.py
--rw-r--r--   0        0        0     1279 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/start.py
--rw-r--r--   0        0        0      893 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6713 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-22 07:00:11.386129 nonebot_plugin_gshisbanner-1.3.1/LICENSE
+-rw-r--r--   0        0        0     5907 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/README.md
+-rw-r--r--   0        0        0     1320 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/adapters/__init__.py
+-rw-r--r--   0        0        0     4816 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/adapters/ob11.py
+-rw-r--r--   0        0        0     4806 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/adapters/red.py
+-rw-r--r--   0        0        0      990 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/alias.py
+-rw-r--r--   0        0        0      428 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/api.py
+-rw-r--r--   0        0        0      651 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/config.py
+-rw-r--r--   0        0        0      458 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/constant.py
+-rw-r--r--   0        0        0     3876 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/deal.py
+-rw-r--r--   0        0        0     1192 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/deal_json.py
+-rw-r--r--   0        0        0     3765 2024-04-22 07:00:11.390129 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/draw.py
+-rw-r--r--   0        0        0  8052924 2024-04-22 07:00:11.442130 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/fonts/misans.ttf
+-rw-r--r--   0        0        0     1515 2024-04-22 07:00:11.442130 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/model.py
+-rw-r--r--   0        0        0     2580 2024-04-22 07:00:11.442130 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/send.py
+-rw-r--r--   0        0        0     1279 2024-04-22 07:00:11.442130 nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/start.py
+-rw-r--r--   0        0        0      893 2024-04-22 07:00:11.442130 nonebot_plugin_gshisbanner-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6700 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-1.3.1/PKG-INFO
```

### Comparing `nonebot_plugin_gshisbanner-1.3.0/LICENSE` & `nonebot_plugin_gshisbanner-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.3.0/README.md` & `nonebot_plugin_gshisbanner-1.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 send_type: Literal["forward", "pic"]
 # 结果发送方式
 forward: 使用合并转发的方式发送
 pic: 使用图片发送
 
 pic_font_path: str
 # 图片发送所需要的字体
-# windows上无需配置，有默认的msyh字体，linux需自行配置
+# 默认配置了MiSans字体，不满意可以自己更改
 ```
 **也可以自己尝试复制json文件到数据目录`{bot_dir}/data/genshin_history`**
 
 ## 🎉 使用
 ### 指令表
 #### 用前提示，本插件采用on_keyword，不需要带你设置的command_start，当然，如果你非要带，本插件做了一定的处理
 |        指令        |  权限   | 需要@ | 范围  |                                说明                                |
```

#### html2text {}

```diff
@@ -27,15 +27,15 @@
 ##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
 (å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
 (éè¦æ¯æhttps) Â·Â· 5."jsd.cdn.zzko.cn/gh/KeyPJ/FetchData@main/data/gacha"
 ##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ``` ``` send_type:
 Literal["forward", "pic"] # ç»æåéæ¹å¼ forward:
 ä½¿ç¨åå¹¶è½¬åçæ¹å¼åé pic: ä½¿ç¨å¾çåé pic_font_path: str #
 å¾çåéæéè¦çå­ä½ #
-windowsä¸æ ééç½®ï¼æé»è®¤çmsyhå­ä½ï¼linuxéèªè¡éç½® ```
+é»è®¤éç½®äºMiSanså­ä½ï¼ä¸æ»¡æå¯ä»¥èªå·±æ´æ¹ ```
 **ä¹å¯ä»¥èªå·±å°è¯å¤å¶jsonæä»¶å°æ°æ®ç®å½`{bot_dir}/data/
 genshin_history`** ## ð ä½¿ç¨ ### æä»¤è¡¨ ####
 ç¨åæç¤ºï¼æ¬æä»¶éç¨on_keywordï¼ä¸éè¦å¸¦ä½ è®¾ç½®çcommand_startï¼å½ç¶ï¼å¦æä½ éè¦å¸¦ï¼æ¬æä»¶åäºä¸å®çå¤ç
 | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:----------------:|:-----:|:--
 -:|:---:|:----------------------------------------------------------------:| |
 [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
```

### Comparing `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/__init__.py` & `nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .constant import DRIVER
 from .adapters import *  # noqa: F401, F403
 from .start import init_group_card  # noqa: F401
 
 enable_auto_select_bot()
 DRIVER.on_startup(init_group_card)
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 __plugin_meta__ = PluginMetadata(
     name="gshisbanner",
     description="这是一个在机器人上获取原神历史卡池的插件",
     usage="""
     (
         usage1: [角色/武器名]历史卡池/历史up[长度],
         explain1: 获取该角色/武器的历史卡池信息,
```

### Comparing `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/adapters/ob11.py` & `nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/adapters/ob11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/adapters/red.py` & `nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/adapters/red.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/alias.py` & `nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/alias.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/config.py` & `nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # 插件的配置文件
+from pathlib import Path
 from typing import Literal
 
 from nonebot import get_driver
 from pydantic import Extra, BaseModel
 
 
 class Config(BaseModel, extra=Extra.ignore):
     gshisbanner_forward_length: int = 10
     """单次合并转发条数"""
     gshisbanner_json_url: str = "banners.52v6.com/data"
     """卡池信息来源网站"""
     send_type: Literal["forward", "pic"] = "forward"
     """发送方式：[“合并转发”，“图片”]"""
-    pic_font_path: str = "msyh.ttc"
+    pic_font_path: str = (Path(__file__).parent / "fonts" / "misans.ttf").as_posix()
     """图片字体路径"""
 
 
 plugin_config = Config.parse_obj(get_driver().config.dict())
```

### Comparing `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/deal.py` & `nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/deal.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/deal_json.py` & `nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/deal_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/draw.py` & `nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/model.py` & `nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/send.py` & `nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/send.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/start.py` & `nonebot_plugin_gshisbanner-1.3.1/nonebot_plugin_gshisbanner/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.3.0/pyproject.toml` & `nonebot_plugin_gshisbanner-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gshisbanner"
-version = "1.3.0"
+version = "1.3.1"
 description = "Nonebot2查询原神历史卡池小插件"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_gshisbanner"}]
```

### Comparing `nonebot_plugin_gshisbanner-1.3.0/PKG-INFO` & `nonebot_plugin_gshisbanner-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gshisbanner
-Version: 1.3.0
+Version: 1.3.1
 Summary: Nonebot2查询原神历史卡池小插件
 License: MIT
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -96,15 +96,15 @@
 send_type: Literal["forward", "pic"]
 # 结果发送方式
 forward: 使用合并转发的方式发送
 pic: 使用图片发送
 
 pic_font_path: str
 # 图片发送所需要的字体
-# windows上无需配置，有默认的msyh字体，linux需自行配置
+# 默认配置了MiSans字体，不满意可以自己更改
 ```
 **也可以自己尝试复制json文件到数据目录`{bot_dir}/data/genshin_history`**
 
 ## 🎉 使用
 ### 指令表
 #### 用前提示，本插件采用on_keyword，不需要带你设置的command_start，当然，如果你非要带，本插件做了一定的处理
 |        指令        |  权限   | 需要@ | 范围  |                                说明                                |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 1.3.1 Summary:
 Nonebot2æ¥è¯¢åç¥åå²å¡æ± å°æä»¶ License: MIT Author: forchannot
 Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: httpx (>=0.20.0,<1.0.0)
@@ -38,15 +38,15 @@
 ##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
 (å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
 (éè¦æ¯æhttps) Â·Â· 5."jsd.cdn.zzko.cn/gh/KeyPJ/FetchData@main/data/gacha"
 ##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ``` ``` send_type:
 Literal["forward", "pic"] # ç»æåéæ¹å¼ forward:
 ä½¿ç¨åå¹¶è½¬åçæ¹å¼åé pic: ä½¿ç¨å¾çåé pic_font_path: str #
 å¾çåéæéè¦çå­ä½ #
-windowsä¸æ ééç½®ï¼æé»è®¤çmsyhå­ä½ï¼linuxéèªè¡éç½® ```
+é»è®¤éç½®äºMiSanså­ä½ï¼ä¸æ»¡æå¯ä»¥èªå·±æ´æ¹ ```
 **ä¹å¯ä»¥èªå·±å°è¯å¤å¶jsonæä»¶å°æ°æ®ç®å½`{bot_dir}/data/
 genshin_history`** ## ð ä½¿ç¨ ### æä»¤è¡¨ ####
 ç¨åæç¤ºï¼æ¬æä»¶éç¨on_keywordï¼ä¸éè¦å¸¦ä½ è®¾ç½®çcommand_startï¼å½ç¶ï¼å¦æä½ éè¦å¸¦ï¼æ¬æä»¶åäºä¸å®çå¤ç
 | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:----------------:|:-----:|:--
 -:|:---:|:----------------------------------------------------------------:| |
 [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
```

