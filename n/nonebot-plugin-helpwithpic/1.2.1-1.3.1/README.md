# Comparing `tmp/nonebot-plugin-HelpWithPic-1.2.1.tar.gz` & `tmp/nonebot_plugin_helpwithpic-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-HelpWithPic-1.2.1.tar", last modified: Thu Apr  4 13:54:54 2024, max compression
+gzip compressed data, was "nonebot_plugin_helpwithpic-1.3.1.tar", last modified: Mon Apr 22 08:39:32 2024, max compression
```

## Comparing `nonebot-plugin-HelpWithPic-1.2.1.tar` & `nonebot_plugin_helpwithpic-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:54:54.091496 nonebot-plugin-HelpWithPic-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 13:54:50.000000 nonebot-plugin-HelpWithPic-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44128 2024-04-04 13:54:54.091496 nonebot-plugin-HelpWithPic-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-04 13:54:50.000000 nonebot-plugin-HelpWithPic-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:54:54.091496 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44128 2024-04-04 13:54:54.000000 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-04 13:54:54.000000 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:54:54.000000 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 13:54:54.000000 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:54:54.000000 nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-04 13:54:50.000000 nonebot-plugin-HelpWithPic-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:54:54.091496 nonebot-plugin-HelpWithPic-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:39:32.410482 nonebot_plugin_helpwithpic-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44288 2024-04-22 08:39:32.410482 nonebot_plugin_helpwithpic-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:39:32.410482 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/draw_contect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/hwp_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic/plugins_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:39:32.410482 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44288 2024-04-22 08:39:32.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-22 08:39:32.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:39:32.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-22 08:39:32.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 08:39:32.000000 nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-22 08:39:26.000000 nonebot_plugin_helpwithpic-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:39:32.410482 nonebot_plugin_helpwithpic-1.3.1/setup.cfg
```

### Comparing `nonebot-plugin-HelpWithPic-1.2.1/LICENSE` & `nonebot_plugin_helpwithpic-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-HelpWithPic-1.2.1/PKG-INFO` & `nonebot_plugin_helpwithpic-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot-plugin-HelpWithPic
-Version: 1.2.1
+Name: nonebot-plugin-helpwithpic
+Version: 1.3.1
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,23 +682,26 @@
 Project-URL: repository, https://github.com/cubstaryow/nonebot-plugin-HelpWithPic
 Keywords: egg,bacon,sausage,tomatoes,Lobster Thermidor
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nonebot-adapter-onebot
+Requires-Dist: nonebot2
 Requires-Dist: httpx
-Requires-Dist: nonebot_plugin_send_anything_anywhere
+Requires-Dist: aiohttp
+Requires-Dist: nonebot-plugin-send-anything-anywhere
 Requires-Dist: pil_utils
 Requires-Dist: pillow
 
 <div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-HelpWithPic/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+  <p><img src="https://github.com/cubstaryow/nonebot-plugin-HelpWithPic/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-HelpWithPic
 
 _✨ nonebot插件-动态帮助图片制作 ✨_
@@ -712,22 +715,20 @@
 </a>
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 </div>
 
 
 
-
-
 ## ⚠ 注意
 因为我是小白,我只能以我自己的方式写我觉得可能挺好用的插件()
 所以部分代码逻辑可能不是很好
-此插件部分代码参考 nonebot-plugin-picstatus (制图与部分资源获取)
 
-目前只支持 onebotV11 !!!!
+目前只支持 onebotV11
+暂时还未上传nonebot商店 将在正式版尝试上传.
 
 ## 📖 介绍
 
 这里是插件的详细介绍部分
 
 ## 💿 安装
 
@@ -769,20 +770,25 @@
     plugins = ["nonebot_plugin_HelpWithPic"]
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
 大小写不影响配置)
 
+### ⚠ 注意
+部分 pydantic 版本可能会导致 HWP_custom_bg 项目报错!
+
+
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | HWP_font | 否 | None | 使用的字体文件 |
-| HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png']此处使用相对路径,默认使用bing壁纸 |
+| HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如["file:///./data/draw/default_bg1.png"]此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
 | HWP_version | 否 | "HelpWithPic-Betaxxx"  | 插件版本 |
 
 ## 🎉 使用
```

### Comparing `nonebot-plugin-HelpWithPic-1.2.1/README.md` & `nonebot_plugin_helpwithpic-1.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-HelpWithPic/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+  <p><img src="https://github.com/cubstaryow/nonebot-plugin-HelpWithPic/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-HelpWithPic
 
 _✨ nonebot插件-动态帮助图片制作 ✨_
@@ -19,22 +19,20 @@
 </a>
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 </div>
 
 
 
-
-
 ## ⚠ 注意
 因为我是小白,我只能以我自己的方式写我觉得可能挺好用的插件()
 所以部分代码逻辑可能不是很好
-此插件部分代码参考 nonebot-plugin-picstatus (制图与部分资源获取)
 
-目前只支持 onebotV11 !!!!
+目前只支持 onebotV11
+暂时还未上传nonebot商店 将在正式版尝试上传.
 
 ## 📖 介绍
 
 这里是插件的详细介绍部分
 
 ## 💿 安装
 
@@ -76,20 +74,25 @@
     plugins = ["nonebot_plugin_HelpWithPic"]
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
 大小写不影响配置)
 
+### ⚠ 注意
+部分 pydantic 版本可能会导致 HWP_custom_bg 项目报错!
+
+
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | HWP_font | 否 | None | 使用的字体文件 |
-| HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png']此处使用相对路径,默认使用bing壁纸 |
+| HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如["file:///./data/draw/default_bg1.png"]此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
 | HWP_version | 否 | "HelpWithPic-Betaxxx"  | 插件版本 |
 
 ## 🎉 使用
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # nonebot-plugin-HelpWithPic _â¨ nonebotæä»¶-å¨æå¸®å©å¾çå¶ä½ â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## â  æ³¨æ
 å ä¸ºææ¯å°ç½,æåªè½ä»¥æèªå·±çæ¹å¼åæè§å¾å¯è½æºå¥½ç¨çæä»¶
-() æä»¥é¨åä»£ç é»è¾å¯è½ä¸æ¯å¾å¥½ æ­¤æä»¶é¨åä»£ç åè
-nonebot-plugin-picstatus (å¶å¾ä¸é¨åèµæºè·å) ç®ååªæ¯æ
-onebotV11 !!!! ## ð ä»ç» è¿éæ¯æä»¶çè¯¦ç»ä»ç»é¨å ## ð¿
-å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-HelpWithPic
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-HelpWithPic pdm pdm add nonebot-plugin-
-HelpWithPic poetry poetry add nonebot-plugin-HelpWithPic conda conda install
-nonebot-plugin-HelpWithPic æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot_plugin_HelpWithPic"] ## âï¸ éç½® å¨ nonebot2
+() æä»¥é¨åä»£ç é»è¾å¯è½ä¸æ¯å¾å¥½ ç®ååªæ¯æ onebotV11
+ææ¶è¿æªä¸ä¼ nonebotååº å°å¨æ­£å¼çå°è¯ä¸ä¼ . ## ð ä»ç»
+è¿éæ¯æä»¶çè¯¦ç»ä»ç»é¨å ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨
+nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
+nb plugin install nonebot-plugin-HelpWithPic ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install
+nonebot-plugin-HelpWithPic pdm pdm add nonebot-plugin-HelpWithPic poetry poetry
+add nonebot-plugin-HelpWithPic conda conda install nonebot-plugin-HelpWithPic
+æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
+[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_HelpWithPic"] ##
+âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
-å¤§å°åä¸å½±åéç½®) | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:
-|:----:|:----:|:----:| | HWP_font | å¦ | None | ä½¿ç¨çå­ä½æä»¶ | |
-HWP_custom_bg | å¦ | [] | å¾çèæ¯,éè¦ä»¥file:///å¼å¤´,æ¯å¦['file://
-/./data/draw/default_bg1.png']æ­¤å¤ä½¿ç¨ç¸å¯¹è·¯å¾,é»è®¤ä½¿ç¨bingå£çº¸ |
+å¤§å°åä¸å½±åéç½®) ### â  æ³¨æ é¨å pydantic çæ¬å¯è½ä¼å¯¼è´
+HWP_custom_bg é¡¹ç®æ¥é! | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:----
+-:|:----:|:----:|:----:| | HWP_font | å¦ | None | ä½¿ç¨çå­ä½æä»¶ | |
+HWP_custom_bg | å¦ | [] | å¾çèæ¯,éè¦ä»¥file:///å¼å¤´,æ¯å¦["file://
+/./data/draw/default_bg1.png"]æ­¤å¤ä½¿ç¨ç¸å¯¹è·¯å¾,é»è®¤ä½¿ç¨bingå£çº¸ |
 | version | å¦ | "Unknow" | å¯ä»¥å¡«ä½ çbotçæ¬ | | HWP_commandstart |
 å¦ | "#" | èªå®ä¹å½ä»¤å¤´ | | HWP_nickname | å¦ | "æ¬botçå¸®å©ææ¡£"
 | æ é¢ | | HWP_text | å¦ | "ä½ æ³è¦ç,æä»¬é½æ²¡æ
 (ä¸æ¯\nè¿æ¯æè¿°" | æè¿° | | HWP_version | å¦ | "HelpWithPic-Betaxxx" |
 æä»¶çæ¬ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ |
 èå´ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:| | #help | user | å¦ |
 ç¾¤è/ç§è | è¯·æ ¹æ®HWP_commandstartä½¿ç¨ |
```

### Comparing `nonebot-plugin-HelpWithPic-1.2.1/nonebot_plugin_HelpWithPic.egg-info/PKG-INFO` & `nonebot_plugin_helpwithpic-1.3.1/nonebot_plugin_helpwithpic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot-plugin-HelpWithPic
-Version: 1.2.1
+Name: nonebot-plugin-helpwithpic
+Version: 1.3.1
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,23 +682,26 @@
 Project-URL: repository, https://github.com/cubstaryow/nonebot-plugin-HelpWithPic
 Keywords: egg,bacon,sausage,tomatoes,Lobster Thermidor
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: nonebot-adapter-onebot
+Requires-Dist: nonebot2
 Requires-Dist: httpx
-Requires-Dist: nonebot_plugin_send_anything_anywhere
+Requires-Dist: aiohttp
+Requires-Dist: nonebot-plugin-send-anything-anywhere
 Requires-Dist: pil_utils
 Requires-Dist: pillow
 
 <div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-HelpWithPic/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+  <p><img src="https://github.com/cubstaryow/nonebot-plugin-HelpWithPic/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-HelpWithPic
 
 _✨ nonebot插件-动态帮助图片制作 ✨_
@@ -712,22 +715,20 @@
 </a>
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 </div>
 
 
 
-
-
 ## ⚠ 注意
 因为我是小白,我只能以我自己的方式写我觉得可能挺好用的插件()
 所以部分代码逻辑可能不是很好
-此插件部分代码参考 nonebot-plugin-picstatus (制图与部分资源获取)
 
-目前只支持 onebotV11 !!!!
+目前只支持 onebotV11
+暂时还未上传nonebot商店 将在正式版尝试上传.
 
 ## 📖 介绍
 
 这里是插件的详细介绍部分
 
 ## 💿 安装
 
@@ -769,20 +770,25 @@
     plugins = ["nonebot_plugin_HelpWithPic"]
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
 大小写不影响配置)
 
+### ⚠ 注意
+部分 pydantic 版本可能会导致 HWP_custom_bg 项目报错!
+
+
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | HWP_font | 否 | None | 使用的字体文件 |
-| HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如['file:///./data/draw/default_bg1.png']此处使用相对路径,默认使用bing壁纸 |
+| HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如["file:///./data/draw/default_bg1.png"]此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
 | HWP_version | 否 | "HelpWithPic-Betaxxx"  | 插件版本 |
 
 ## 🎉 使用
```

### Comparing `nonebot-plugin-HelpWithPic-1.2.1/pyproject.toml` & `nonebot_plugin_helpwithpic-1.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "nonebot-plugin-HelpWithPic"
-version = "1.2.1"
+name = "nonebot-plugin-helpwithpic"
+version = "1.3.1"
 description = "nonebot插件-动态帮助图片制作"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
@@ -12,15 +12,18 @@
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
 
 dependencies = [
+  "nonebot-adapter-onebot",
+  "nonebot2",
   "httpx",
-  "nonebot_plugin_send_anything_anywhere",
+  "aiohttp",
+  "nonebot-plugin-send-anything-anywhere",
   "pil_utils",
   "pillow"
 ]
 
 [project.urls]
 repository = "https://github.com/cubstaryow/nonebot-plugin-HelpWithPic"
```

