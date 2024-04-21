# Comparing `tmp/nonebot-plugin-hx-yinying-0.0.7.tar.gz` & `tmp/nonebot-plugin-hx-yinying-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.7.tar", last modified: Fri Apr 19 20:07:33 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.8.tar", last modified: Sun Apr 21 21:59:24 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-0.0.7.tar` & `nonebot-plugin-hx-yinying-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 20:07:33.716940 nonebot-plugin-hx-yinying-0.0.7/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3889 2024-04-19 20:07:33.716940 nonebot-plugin-hx-yinying-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3449 2024-04-19 20:07:15.000000 nonebot-plugin-hx-yinying-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 20:07:33.585275 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0     1968 2024-04-19 20:05:40.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    13088 2024-04-19 20:01:47.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      749 2024-04-18 04:08:44.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-19 20:07:33.716940 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     3889 2024-04-19 20:07:33.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-19 20:07:33.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 20:07:33.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2024-04-19 20:07:33.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-19 20:07:33.000000 nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-19 20:07:33.740244 nonebot-plugin-hx-yinying-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      840 2024-04-19 20:07:25.000000 nonebot-plugin-hx-yinying-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:59:23.987544 nonebot-plugin-hx-yinying-0.0.8/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3924 2024-04-21 21:59:23.988553 nonebot-plugin-hx-yinying-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3484 2024-04-21 21:01:59.000000 nonebot-plugin-hx-yinying-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 21:59:23.816561 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0     7340 2024-04-21 21:59:02.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    29062 2024-04-21 21:56:18.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      764 2024-04-21 21:59:08.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-21 21:59:23.980562 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     3924 2024-04-21 21:59:23.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-21 21:59:23.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 21:59:23.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2024-04-21 21:59:23.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-21 21:59:23.000000 nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-21 21:59:23.996739 nonebot-plugin-hx-yinying-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      840 2024-04-21 21:59:16.000000 nonebot-plugin-hx-yinying-0.0.8/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-0.0.7/LICENSE` & `nonebot-plugin-hx-yinying-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.7/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-hx-yinying
-Version: 0.0.7
-Summary: chat with yinying
-Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
-Author: Huan Xin
-Author-email: mc.xiaolang@foxmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!--
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
  * @Author         : huanxin996
  * @Date           : 2024-4-17
  * @LastEditors    : huanxin996
- * @LastEditTime   : 2024-4-19
+ * @LastEditTime   : 2024-4-22
  * @Description    : None
  * @GitHub         : https://github.com/huanxin996
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
@@ -83,59 +70,55 @@
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：这里写你找秩乱获取到的api_key
 - 重要：必填
 
 
-### hx_api_yinying
+### hx_api_yinying(已于0.0.7版本移除)
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：yinying的api地址
 - 重要：必填
 
-### yinying_model
+### yinying_model(已于0.0.7版本移除)
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：选择使用银影的模型
 - 注意 该配置项即将移除（转为插件内配置！）
 
 ## hx_path
 - 类型：`str`
 - 默认值：`None`
 - 说明：银影对话的用户数据存储路径(不写将使用默认配置)
 
-## hx_reply
+## hx_reply(已于0.0.7版本移除)
 - 类型：`bool`
 - 默认值：`False`
 - 说明：bot发送chat消息时是否回复
 - 注意：该项启用时hx_reply_at将被忽略
 
-## hx_reply_at
+## hx_reply_at(已于0.0.7版本移除)
 - 类型：`bool`
 - 默认值：`False`
 - 说明：bot发送chat消息时不回复时是否艾特
 
-## yinying_limit
+## yinying_limit(已于0.0.7版本移除)
 - 类型：`int`
 - 默认值：`12`
 - 说明：对于银影对话限制的次数
 
 
 配置文件示例（默认模板）
 
 ```dotenv
-hx_api_yinying=https://地址
 yinying_appid=你的appid
 yinying_token=你的token(不带bearer)
-yinying_model=模型
-hx_reply_at=False
-yinying_limit=12
 ```
 
 
 ## Contributors ✨
 
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
```

#### html2text {}

```diff
@@ -1,17 +1,11 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.7 Summary:
-chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
-yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown License-File: LICENSE [![All Contributors](https://
-img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
-(#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
-huanxin996 * @LastEditTime : 2024-4-19 * @Description : None * @GitHub : https:
-//github.com/huanxin996 -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-
+orange.svg?style=flat-square)](#contributors-) * @Author : huanxin996 * @Date :
+2024-4-17 * @LastEditors : huanxin996 * @LastEditTime : 2024-4-22 *
+@Description : None * @GitHub : https://github.com/huanxin996 -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
 éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
 çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.python.org/pypi/nonebot-
@@ -21,22 +15,23 @@
 è¯·æ³¨æï¼è¯¥é¡¹ç®æ¯æ¥å¥äºä¹±ä¹±çé¡¹ç®ï¼ä½ éè¦éµå®apiä½¿ç¨ç
 [è§è](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)ã
 éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_appid -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid - éè¦ï¼å¿å¡«
 ### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ###
-hx_api_yinying - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model -
-ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å -
-æ³¨æ è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
+hx_api_yinying(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model
+(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å - æ³¨æ
+è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
-## hx_reply - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+## hx_reply(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
 è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
-æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at -
-ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit -
-ç±»åï¼`int` - é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
-éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv hx_api_yinying=https://å°å
-yinying_appid=ä½ çappid yinying_token=ä½ çtoken(ä¸å¸¦bearer)
-yinying_model=æ¨¡å hx_reply_at=False yinying_limit=12 ``` ## Contributors â¨
+æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at
+(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit
+(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`int` - é»è®¤å¼ï¼`12` -
+è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ° éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼
+```dotenv yinying_appid=ä½ çappid yinying_token=ä½ çtoken(ä¸å¸¦bearer) ```
+## Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-0.0.7/README.md` & `nonebot-plugin-hx-yinying-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,29 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-hx-yinying
+Version: 0.0.8
+Summary: chat with yinying
+Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
+Author: Huan Xin
+Author-email: mc.xiaolang@foxmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!--
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
  * @Author         : huanxin996
  * @Date           : 2024-4-17
  * @LastEditors    : huanxin996
- * @LastEditTime   : 2024-4-19
+ * @LastEditTime   : 2024-4-22
  * @Description    : None
  * @GitHub         : https://github.com/huanxin996
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
@@ -70,59 +83,55 @@
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：这里写你找秩乱获取到的api_key
 - 重要：必填
 
 
-### hx_api_yinying
+### hx_api_yinying(已于0.0.7版本移除)
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：yinying的api地址
 - 重要：必填
 
-### yinying_model
+### yinying_model(已于0.0.7版本移除)
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：选择使用银影的模型
 - 注意 该配置项即将移除（转为插件内配置！）
 
 ## hx_path
 - 类型：`str`
 - 默认值：`None`
 - 说明：银影对话的用户数据存储路径(不写将使用默认配置)
 
-## hx_reply
+## hx_reply(已于0.0.7版本移除)
 - 类型：`bool`
 - 默认值：`False`
 - 说明：bot发送chat消息时是否回复
 - 注意：该项启用时hx_reply_at将被忽略
 
-## hx_reply_at
+## hx_reply_at(已于0.0.7版本移除)
 - 类型：`bool`
 - 默认值：`False`
 - 说明：bot发送chat消息时不回复时是否艾特
 
-## yinying_limit
+## yinying_limit(已于0.0.7版本移除)
 - 类型：`int`
 - 默认值：`12`
 - 说明：对于银影对话限制的次数
 
 
 配置文件示例（默认模板）
 
 ```dotenv
-hx_api_yinying=https://地址
 yinying_appid=你的appid
 yinying_token=你的token(不带bearer)
-yinying_model=模型
-hx_reply_at=False
-yinying_limit=12
 ```
 
 
 ## Contributors ✨
 
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
```

#### html2text {}

```diff
@@ -1,11 +1,17 @@
-[![All Contributors](https://img.shields.io/badge/all_contributors-2-
-orange.svg?style=flat-square)](#contributors-) * @Author : huanxin996 * @Date :
-2024-4-17 * @LastEditors : huanxin996 * @LastEditTime : 2024-4-19 *
-@Description : None * @GitHub : https://github.com/huanxin996 -->
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.8 Summary:
+chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
+yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Description-Content-
+Type: text/markdown License-File: LICENSE [![All Contributors](https://
+img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
+(#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
+huanxin996 * @LastEditTime : 2024-4-22 * @Description : None * @GitHub : https:
+//github.com/huanxin996 -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
 éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
 çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.python.org/pypi/nonebot-
@@ -15,22 +21,23 @@
 è¯·æ³¨æï¼è¯¥é¡¹ç®æ¯æ¥å¥äºä¹±ä¹±çé¡¹ç®ï¼ä½ éè¦éµå®apiä½¿ç¨ç
 [è§è](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)ã
 éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_appid -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid - éè¦ï¼å¿å¡«
 ### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ###
-hx_api_yinying - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model -
-ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å -
-æ³¨æ è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
+hx_api_yinying(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model
+(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å - æ³¨æ
+è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
-## hx_reply - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+## hx_reply(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
 è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
-æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at -
-ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit -
-ç±»åï¼`int` - é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
-éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv hx_api_yinying=https://å°å
-yinying_appid=ä½ çappid yinying_token=ä½ çtoken(ä¸å¸¦bearer)
-yinying_model=æ¨¡å hx_reply_at=False yinying_limit=12 ``` ## Contributors â¨
+æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at
+(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit
+(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`int` - é»è®¤å¼ï¼`12` -
+è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ° éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼
+```dotenv yinying_appid=ä½ çappid yinying_token=ä½ çtoken(ä¸å¸¦bearer) ```
+## Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import Optional
 
 import nonebot
 from pydantic import BaseModel
 
 
 class Config(BaseModel):
-    # 配置文件版本号
-    hx_version: Optional[str] = None
+    # 插件版本号勿动！！！！
+    hx_version: Optional[str] = "0.0.8"
     # 你的appid
     yinying_appid: Optional[str] = None
     # model，如 yinying-v3
     yinying_model: Optional[str] = None
     furbar_model: Optional[str] = None
 
     yinying_token: Optional[str] = None
```

### Comparing `nonebot-plugin-hx-yinying-0.0.7/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.8/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.0.7
+Version: 0.0.8
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
  * @Author         : huanxin996
  * @Date           : 2024-4-17
  * @LastEditors    : huanxin996
- * @LastEditTime   : 2024-4-19
+ * @LastEditTime   : 2024-4-22
  * @Description    : None
  * @GitHub         : https://github.com/huanxin996
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
@@ -83,59 +83,55 @@
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：这里写你找秩乱获取到的api_key
 - 重要：必填
 
 
-### hx_api_yinying
+### hx_api_yinying(已于0.0.7版本移除)
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：yinying的api地址
 - 重要：必填
 
-### yinying_model
+### yinying_model(已于0.0.7版本移除)
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：选择使用银影的模型
 - 注意 该配置项即将移除（转为插件内配置！）
 
 ## hx_path
 - 类型：`str`
 - 默认值：`None`
 - 说明：银影对话的用户数据存储路径(不写将使用默认配置)
 
-## hx_reply
+## hx_reply(已于0.0.7版本移除)
 - 类型：`bool`
 - 默认值：`False`
 - 说明：bot发送chat消息时是否回复
 - 注意：该项启用时hx_reply_at将被忽略
 
-## hx_reply_at
+## hx_reply_at(已于0.0.7版本移除)
 - 类型：`bool`
 - 默认值：`False`
 - 说明：bot发送chat消息时不回复时是否艾特
 
-## yinying_limit
+## yinying_limit(已于0.0.7版本移除)
 - 类型：`int`
 - 默认值：`12`
 - 说明：对于银影对话限制的次数
 
 
 配置文件示例（默认模板）
 
 ```dotenv
-hx_api_yinying=https://地址
 yinying_appid=你的appid
 yinying_token=你的token(不带bearer)
-yinying_model=模型
-hx_reply_at=False
-yinying_limit=12
 ```
 
 
 ## Contributors ✨
 
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.8 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
-huanxin996 * @LastEditTime : 2024-4-19 * @Description : None * @GitHub : https:
+huanxin996 * @LastEditTime : 2024-4-22 * @Description : None * @GitHub : https:
 //github.com/huanxin996 -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
 éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
@@ -21,22 +21,23 @@
 è¯·æ³¨æï¼è¯¥é¡¹ç®æ¯æ¥å¥äºä¹±ä¹±çé¡¹ç®ï¼ä½ éè¦éµå®apiä½¿ç¨ç
 [è§è](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)ã
 éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_appid -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid - éè¦ï¼å¿å¡«
 ### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ###
-hx_api_yinying - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
-è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model -
-ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å -
-æ³¨æ è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
+hx_api_yinying(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+è¯´æï¼yinyingçapiå°å - éè¦ï¼å¿å¡« ### yinying_model
+(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å - æ³¨æ
+è¯¥éç½®é¡¹å³å°ç§»é¤ï¼è½¬ä¸ºæä»¶åéç½®ï¼ï¼ ## hx_path -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
-## hx_reply - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+## hx_reply(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
 è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
-æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at -
-ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit -
-ç±»åï¼`int` - é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
-éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv hx_api_yinying=https://å°å
-yinying_appid=ä½ çappid yinying_token=ä½ çtoken(ä¸å¸¦bearer)
-yinying_model=æ¨¡å hx_reply_at=False yinying_limit=12 ``` ## Contributors â¨
+æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at
+(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit
+(å·²äº0.0.7çæ¬ç§»é¤) - ç±»åï¼`int` - é»è®¤å¼ï¼`12` -
+è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ° éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼
+```dotenv yinying_appid=ä½ çappid yinying_token=ä½ çtoken(ä¸å¸¦bearer) ```
+## Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-0.0.7/setup.py` & `nonebot-plugin-hx-yinying-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="0.0.7",
+    version="0.0.8",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

