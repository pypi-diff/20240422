# Comparing `tmp/nonebot_plugin_gshisbanner-1.2.5.tar.gz` & `tmp/nonebot_plugin_gshisbanner-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gshisbanner-1.2.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_gshisbanner-1.3.0.tar", max compression
```

## Comparing `nonebot_plugin_gshisbanner-1.2.5.tar` & `nonebot_plugin_gshisbanner-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1067 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/LICENSE
--rw-r--r--   0        0        0     5726 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/README.md
--rw-r--r--   0        0        0     1320 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/__init__.py
--rw-r--r--   0        0        0      426 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/adapters/__init__.py
--rw-r--r--   0        0        0     4184 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/adapters/ob11.py
--rw-r--r--   0        0        0     4174 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/adapters/red.py
--rw-r--r--   0        0        0      990 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/alias.py
--rw-r--r--   0        0        0      428 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/api.py
--rw-r--r--   0        0        0      370 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/config.py
--rw-r--r--   0        0        0      458 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/constant.py
--rw-r--r--   0        0        0     3876 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/deal.py
--rw-r--r--   0        0        0     1192 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/deal_json.py
--rw-r--r--   0        0        0      410 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/model.py
--rw-r--r--   0        0        0     2471 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/send.py
--rw-r--r--   0        0        0     1279 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/start.py
--rw-r--r--   0        0        0      893 2024-03-08 09:11:54.674160 nonebot_plugin_gshisbanner-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     6519 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-22 06:48:19.556158 nonebot_plugin_gshisbanner-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5920 2024-04-22 06:48:19.556158 nonebot_plugin_gshisbanner-1.3.0/README.md
+-rw-r--r--   0        0        0     1320 2024-04-22 06:48:19.556158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-22 06:48:19.556158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/adapters/__init__.py
+-rw-r--r--   0        0        0     4816 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/adapters/ob11.py
+-rw-r--r--   0        0        0     4806 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/adapters/red.py
+-rw-r--r--   0        0        0      990 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/alias.py
+-rw-r--r--   0        0        0      428 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/api.py
+-rw-r--r--   0        0        0      577 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/config.py
+-rw-r--r--   0        0        0      458 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/constant.py
+-rw-r--r--   0        0        0     3876 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/deal.py
+-rw-r--r--   0        0        0     1192 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/deal_json.py
+-rw-r--r--   0        0        0     3765 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/draw.py
+-rw-r--r--   0        0        0     1515 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/model.py
+-rw-r--r--   0        0        0     2580 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/send.py
+-rw-r--r--   0        0        0     1279 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/start.py
+-rw-r--r--   0        0        0      893 2024-04-22 06:48:19.560158 nonebot_plugin_gshisbanner-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6713 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-1.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_gshisbanner-1.2.5/LICENSE` & `nonebot_plugin_gshisbanner-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.2.5/README.md` & `nonebot_plugin_gshisbanner-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 ## ⚙️ 配置
 ```
 gshisbanner_forward_length: int
 # 单次合并转发消息长度（int）,默认为10
 # 仅为角色/武器卡池转发内容长度，不包括版本卡池
 # 越大单次转发内容更多，合并转发的次数更少，越小单单次转发内容更少，但合并转发的次数更多
 # 不要设置为>99或者<0的数字或者任意字符串
-
+```
+```
 gshisbanner_json_url: str
 # 历史卡池json列表下载位置
 # 可选值
 ·· 1."banners.52v6.com/data" 
      #默认，推荐
 ·· 2."genshin-gacha-banners.vercel.app/data" 
      #vercel代理，国内可能无法直连
@@ -66,15 +67,25 @@
      #cloudfare代理，可能会被墙
 ·· 4."mirror.ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha" 
      ##ghproxy代理的raw文件，大多数情况可用，不过不稳定
      ##前面的"ghproxy.com/"可以不写(如果你是国外机),或者换成你自建的github加速服务均可(需要支持https)
 ·· 5."jsd.cdn.zzko.cn/gh/KeyPJ/FetchData@main/data/gacha"
      ##jsdelivr代理的文件，大多数情况可用，推荐
 ```
-**也可以将上述4和5中的`KeyPJ`更改为`forchannot`，或者自己尝试复制json文件到数据目录`{bot_dir}/data/genshin_history`**
+```
+send_type: Literal["forward", "pic"]
+# 结果发送方式
+forward: 使用合并转发的方式发送
+pic: 使用图片发送
+
+pic_font_path: str
+# 图片发送所需要的字体
+# windows上无需配置，有默认的msyh字体，linux需自行配置
+```
+**也可以自己尝试复制json文件到数据目录`{bot_dir}/data/genshin_history`**
 
 ## 🎉 使用
 ### 指令表
 #### 用前提示，本插件采用on_keyword，不需要带你设置的command_start，当然，如果你非要带，本插件做了一定的处理
 |        指令        |  权限   | 需要@ | 范围  |                                说明                                |
 |:----------------:|:-----:|:---:|:---:|:----------------------------------------------------------------:|
 | [name]历史卡池(num)  |  ALL  |  否  | ALL | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
@@ -117,8 +128,8 @@
 <summary>刷新卡池/别名效果图</summary>
 <img src="https://jsd.cdn.zzko.cn/gh/forchannot/mypicgo@main/20230324/image.5zl59kpx8b00.jpg" alt="help">
 </details>
 
 
 ### 鸣谢
 
-[genshin-gacha-banners](https://github.com/KeyPJ/genshin-gacha-banners) #历史up卡池来源
+[FetchData](https://github.com/KeyPJ/FetchData) #历史up卡池来源，感谢
```

#### html2text {}

```diff
@@ -12,34 +12,38 @@
 install nonebot-plugin-gshisbanner pip pip install nonebot-plugin-gshisbanner
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_gshisbanner"] ##
 âï¸ éç½® ``` gshisbanner_forward_length: int #
 åæ¬¡åå¹¶è½¬åæ¶æ¯é¿åº¦ï¼intï¼,é»è®¤ä¸º10 # ä»ä¸ºè§è²/
 æ­¦å¨å¡æ± è½¬ååå®¹é¿åº¦ï¼ä¸åæ¬çæ¬å¡æ±  #
 è¶å¤§åæ¬¡è½¬ååå®¹æ´å¤ï¼åå¹¶è½¬åçæ¬¡æ°æ´å°ï¼è¶å°ååæ¬¡è½¬ååå®¹æ´å°ï¼ä½åå¹¶è½¬åçæ¬¡æ°æ´å¤
-# ä¸è¦è®¾ç½®ä¸º>99æè<0çæ°å­æèä»»æå­ç¬¦ä¸²
+# ä¸è¦è®¾ç½®ä¸º>99æè<0çæ°å­æèä»»æå­ç¬¦ä¸² ``` ```
 gshisbanner_json_url: str # åå²å¡æ± jsonåè¡¨ä¸è½½ä½ç½® # å¯éå¼ Â·Â·
 1."banners.52v6.com/data" #é»è®¤ï¼æ¨è Â·Â· 2."genshin-gacha-
 banners.vercel.app/data" #vercelä»£çï¼å½åå¯è½æ æ³ç´è¿ Â·Â·
 3."genshin-gacha-banners.52v6.com/data" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â·
 4."mirror.ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/
 data/gacha"
 ##ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼ä¸è¿ä¸ç¨³å®
 ##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
 (å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
 (éè¦æ¯æhttps) Â·Â· 5."jsd.cdn.zzko.cn/gh/KeyPJ/FetchData@main/data/gacha"
-##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ```
-**ä¹å¯ä»¥å°ä¸è¿°4å5ä¸­ç`KeyPJ`æ´æ¹ä¸º`forchannot`ï¼æèèªå·±å°è¯å¤å¶jsonæä»¶å°æ°æ®ç®å½`
-{bot_dir}/data/genshin_history`** ## ð ä½¿ç¨ ### æä»¤è¡¨ ####
+##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ``` ``` send_type:
+Literal["forward", "pic"] # ç»æåéæ¹å¼ forward:
+ä½¿ç¨åå¹¶è½¬åçæ¹å¼åé pic: ä½¿ç¨å¾çåé pic_font_path: str #
+å¾çåéæéè¦çå­ä½ #
+windowsä¸æ ééç½®ï¼æé»è®¤çmsyhå­ä½ï¼linuxéèªè¡éç½® ```
+**ä¹å¯ä»¥èªå·±å°è¯å¤å¶jsonæä»¶å°æ°æ®ç®å½`{bot_dir}/data/
+genshin_history`** ## ð ä½¿ç¨ ### æä»¤è¡¨ ####
 ç¨åæç¤ºï¼æ¬æä»¶éç¨on_keywordï¼ä¸éè¦å¸¦ä½ è®¾ç½®çcommand_startï¼å½ç¶ï¼å¦æä½ éè¦å¸¦ï¼æ¬æä»¶åäºä¸å®çå¤ç
 | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:----------------:|:-----:|:--
 -:|:---:|:----------------------------------------------------------------:| |
 [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
 | | [version]å¡æ± [num] | ALL | å¦ | ALL |
 versionä¸ºçæ¬å·ï¼å¦1.3ï¼2.6ç­ï¼numä¸º1-
 3ï¼å¯¹åºä¸åï¼ä¸­ï¼ä¸åï¼å¯ä¸å¡«ï¼å¦ä¸å¡«ååéè¯¥çæ¬å¨é¨å¡æ± 
 | | å·æ°(æ´æ°)åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
 å·æ°åå²å¡æ± æå«å | ### ææå¾ åå²å¡æ± ææå¾ å¾1
 [help]å¾2 [help]å¾3 [help]çæ¬å¡æ± ææå¾ å¾1 [help]å¾2 [help]å¾3
-[help]å·æ°å¡æ± /å«åææå¾ [help]### é¸£è°¢ [genshin-gacha-banners]
-(https://github.com/KeyPJ/genshin-gacha-banners) #åå²upå¡æ± æ¥æº
+[help]å·æ°å¡æ± /å«åææå¾ [help]### é¸£è°¢ [FetchData](https://
+github.com/KeyPJ/FetchData) #åå²upå¡æ± æ¥æºï¼æè°¢
```

### Comparing `nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/__init__.py` & `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .constant import DRIVER
 from .adapters import *  # noqa: F401, F403
 from .start import init_group_card  # noqa: F401
 
 enable_auto_select_bot()
 DRIVER.on_startup(init_group_card)
 
-__version__ = "1.2.5"
+__version__ = "1.3.0"
 __plugin_meta__ = PluginMetadata(
     name="gshisbanner",
     description="这是一个在机器人上获取原神历史卡池的插件",
     usage="""
     (
         usage1: [角色/武器名]历史卡池/历史up[长度],
         explain1: 获取该角色/武器的历史卡池信息,
```

### Comparing `nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/adapters/ob11.py` & `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/adapters/red.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from nonebot.params import Keyword
 from nonebot import logger, require
 from nonebot.permission import SUPERUSER
 from nonebot.plugin.on import on_keyword
 
 require("nonebot_plugin_saa")
-from nonebot_plugin_saa import SaaTarget
+from nonebot_plugin_saa import Image, SaaTarget
 
 from ..alias import find_name
 from ..config import plugin_config
+from ..draw import GameGachaBanner
 from ..start import init_group_card
+from ..model import GachaDraw as GachaDrawModel
 from ..deal_json import save_json, load_json_from_url
 from ..constant import gacha_info_path, special_version
-from ..send import word_send_from_name, word_send_from_version
+from ..send import send_pic, word_send_from_name, word_send_from_version
 from ..deal import deal_info_from_name, delete_command_start, deal_info_from_version
 
 old_gacha = on_keyword(
     {"历史卡池", "历史up"},
     priority=45,
     block=True,
 )
@@ -29,19 +31,19 @@
     permission=SUPERUSER,
     priority=40,
     block=True,
 )
 
 
 try:
-    from nonebot.adapters.onebot.v11 import MessageEvent as Ob11MessageEvent
+    from nonebot.adapters.red.event import MessageEvent as RedMessageEvent
 
     @old_gacha.handle()
     async def _(
-        event: Ob11MessageEvent,
+        event: RedMessageEvent,
         target: SaaTarget,
         key: str = Keyword(),  # noqa: B008
     ):
         name, length = event.get_plaintext().split(key, 1)
         name = delete_command_start(name)
         if name in ["刷新", "更新"]:
             return
@@ -52,24 +54,29 @@
             await old_gacha.finish("该角色/武器不存在或是从未up过")
         # 获取up信息
         info = await deal_info_from_name(
             real_name, "cha" if real_type == "角色" else "wep"
         )
         if not info:
             await old_gacha.finish("获取历史卡池信息失败，请联系超管")
-        if (
-            length := int(length)
-            if length
-            else plugin_config.gshisbanner_forward_length
-        ):
-            await word_send_from_name(target, real_name, info, length)
+        if plugin_config.send_type == "forward":
+            await word_send_from_name(
+                target,
+                real_name,
+                info,
+                int(length) if length else plugin_config.gshisbanner_forward_length,
+            )
+        else:
+            info = [GachaDrawModel.parse_obj(i) for i in info[::-1]]
+            img = GameGachaBanner(info, real_name, real_type).generate_table()
+            await send_pic(target, Image(img))
 
     @version_gacha.handle()
     async def _(
-        event: Ob11MessageEvent,
+        event: RedMessageEvent,
         target: SaaTarget,
         key: str = Keyword(),  # noqa: B008
     ):
         version, upordown = event.get_plaintext().split(key, 1)
         version = delete_command_start(version)
         if version in ["刷新", "更新"]:
             return
@@ -79,19 +86,24 @@
             return
         if upordown == "3" and version not in special_version:
             return
         real_version = f"{version}.{upordown}" if upordown else version
         if info := await deal_info_from_version(real_version, not upordown):
             if not info:
                 await version_gacha.finish("获取历史卡池信息失败，请联系超管")
-            await word_send_from_version(target, real_version, info)
+            if plugin_config.send_type == "forward":
+                await word_send_from_version(target, real_version, info)
+            else:
+                info = [GachaDrawModel.parse_obj(i) for i in info]
+                img = GameGachaBanner(info, real_version, "").generate_table()
+                await send_pic(target, Image(img))
 
     @refresh.handle()
     async def _(
-        event: Ob11MessageEvent,
+        event: RedMessageEvent,
         key: str = Keyword(),  # noqa: B008
     ):
         args = event.get_plaintext().split(key, 1)
         if delete_command_start(args[0]):
             # 去除掉命令开头如果仍然有内容则不处理
             return
         if (choose := args[1]) in ["历史卡池", "历史up", "卡池", "up"]:
@@ -107,10 +119,9 @@
         elif choose == "别名":
             if (await init_group_card(True)) is False:
                 await refresh.finish(f"刷新{choose}失败,可能是网络问题或api失效")
         else:
             await refresh.finish()
         await refresh.finish(f"刷新{choose}成功")
 
-
 except (ImportError, ModuleNotFoundError):
-    logger.warning("nonebot_adapter_onebot未安装,跳过ob11适配器")
+    logger.warning("nonebot_adapter_red未安装,跳过red适配器")
```

### Comparing `nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/adapters/red.py` & `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/adapters/ob11.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from nonebot.params import Keyword
 from nonebot import logger, require
 from nonebot.permission import SUPERUSER
 from nonebot.plugin.on import on_keyword
 
 require("nonebot_plugin_saa")
-from nonebot_plugin_saa import SaaTarget
+from nonebot_plugin_saa import Image, SaaTarget
 
 from ..alias import find_name
 from ..config import plugin_config
+from ..draw import GameGachaBanner
 from ..start import init_group_card
+from ..model import GachaDraw as GachaDrawModel
 from ..deal_json import save_json, load_json_from_url
 from ..constant import gacha_info_path, special_version
-from ..send import word_send_from_name, word_send_from_version
+from ..send import send_pic, word_send_from_name, word_send_from_version
 from ..deal import deal_info_from_name, delete_command_start, deal_info_from_version
 
 old_gacha = on_keyword(
     {"历史卡池", "历史up"},
     priority=45,
     block=True,
 )
@@ -29,19 +31,19 @@
     permission=SUPERUSER,
     priority=40,
     block=True,
 )
 
 
 try:
-    from nonebot.adapters.red.event import MessageEvent as RedMessageEvent
+    from nonebot.adapters.onebot.v11 import MessageEvent as Ob11MessageEvent
 
     @old_gacha.handle()
     async def _(
-        event: RedMessageEvent,
+        event: Ob11MessageEvent,
         target: SaaTarget,
         key: str = Keyword(),  # noqa: B008
     ):
         name, length = event.get_plaintext().split(key, 1)
         name = delete_command_start(name)
         if name in ["刷新", "更新"]:
             return
@@ -52,24 +54,29 @@
             await old_gacha.finish("该角色/武器不存在或是从未up过")
         # 获取up信息
         info = await deal_info_from_name(
             real_name, "cha" if real_type == "角色" else "wep"
         )
         if not info:
             await old_gacha.finish("获取历史卡池信息失败，请联系超管")
-        if (
-            length := int(length)
-            if length
-            else plugin_config.gshisbanner_forward_length
-        ):
-            await word_send_from_name(target, real_name, info, length)
+        if plugin_config.send_type == "forward":
+            await word_send_from_name(
+                target,
+                real_name,
+                info,
+                int(length) if length else plugin_config.gshisbanner_forward_length,
+            )
+        else:
+            info = [GachaDrawModel.parse_obj(i) for i in info[::-1]]
+            img = GameGachaBanner(info, real_name, real_type).generate_table()
+            await send_pic(target, Image(img))
 
     @version_gacha.handle()
     async def _(
-        event: RedMessageEvent,
+        event: Ob11MessageEvent,
         target: SaaTarget,
         key: str = Keyword(),  # noqa: B008
     ):
         version, upordown = event.get_plaintext().split(key, 1)
         version = delete_command_start(version)
         if version in ["刷新", "更新"]:
             return
@@ -79,19 +86,24 @@
             return
         if upordown == "3" and version not in special_version:
             return
         real_version = f"{version}.{upordown}" if upordown else version
         if info := await deal_info_from_version(real_version, not upordown):
             if not info:
                 await version_gacha.finish("获取历史卡池信息失败，请联系超管")
-            await word_send_from_version(target, real_version, info)
+            if plugin_config.send_type == "forward":
+                await word_send_from_version(target, real_version, info)
+            else:
+                info = [GachaDrawModel.parse_obj(i) for i in info]
+                img = GameGachaBanner(info, real_version, "").generate_table()
+                await send_pic(target, Image(img))
 
     @refresh.handle()
     async def _(
-        event: RedMessageEvent,
+        event: Ob11MessageEvent,
         key: str = Keyword(),  # noqa: B008
     ):
         args = event.get_plaintext().split(key, 1)
         if delete_command_start(args[0]):
             # 去除掉命令开头如果仍然有内容则不处理
             return
         if (choose := args[1]) in ["历史卡池", "历史up", "卡池", "up"]:
@@ -107,9 +119,10 @@
         elif choose == "别名":
             if (await init_group_card(True)) is False:
                 await refresh.finish(f"刷新{choose}失败,可能是网络问题或api失效")
         else:
             await refresh.finish()
         await refresh.finish(f"刷新{choose}成功")
 
+
 except (ImportError, ModuleNotFoundError):
-    logger.warning("nonebot_adapter_red未安装,跳过red适配器")
+    logger.warning("nonebot_adapter_onebot未安装,跳过ob11适配器")
```

### Comparing `nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/alias.py` & `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/alias.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/deal.py` & `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/deal.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/deal_json.py` & `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/deal_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/send.py` & `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/send.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime
 
 from nonebot import require
 
 require("nonebot_plugin_saa")
 from nonebot_plugin_saa import (
     Text,
+    Image,
     MessageFactory,
     PlatformTarget,
     AggregatedMessageFactory,
 )
 
 Sendable = Union[MessageFactory, AggregatedMessageFactory]
 
@@ -60,7 +61,11 @@
         banner_four = " ".join(info.get("four_character", info.get("four_weapon", [])))
         msgs.append(
             f"版本：{version}\n五星：{banner_five}"
             f"\n四星：{banner_four}\nup时间：\n{start}~~{end}"
         )
     forward_msg = AggregatedMessageFactory(list(msgs))
     await send_forward_msg(send_target, forward_msg)
+
+
+async def send_pic(send_target: PlatformTarget, pic: Image):
+    await pic.send_to(send_target)
```

### Comparing `nonebot_plugin_gshisbanner-1.2.5/nonebot_plugin_gshisbanner/start.py` & `nonebot_plugin_gshisbanner-1.3.0/nonebot_plugin_gshisbanner/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-1.2.5/pyproject.toml` & `nonebot_plugin_gshisbanner-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gshisbanner"
-version = "1.2.5"
+version = "1.3.0"
 description = "Nonebot2查询原神历史卡池小插件"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_gshisbanner"}]
```

### Comparing `nonebot_plugin_gshisbanner-1.2.5/PKG-INFO` & `nonebot_plugin_gshisbanner-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gshisbanner
-Version: 1.2.5
+Version: 1.3.0
 Summary: Nonebot2查询原神历史卡池小插件
 License: MIT
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,16 @@
 ## ⚙️ 配置
 ```
 gshisbanner_forward_length: int
 # 单次合并转发消息长度（int）,默认为10
 # 仅为角色/武器卡池转发内容长度，不包括版本卡池
 # 越大单次转发内容更多，合并转发的次数更少，越小单单次转发内容更少，但合并转发的次数更多
 # 不要设置为>99或者<0的数字或者任意字符串
-
+```
+```
 gshisbanner_json_url: str
 # 历史卡池json列表下载位置
 # 可选值
 ·· 1."banners.52v6.com/data" 
      #默认，推荐
 ·· 2."genshin-gacha-banners.vercel.app/data" 
      #vercel代理，国内可能无法直连
@@ -87,15 +88,25 @@
      #cloudfare代理，可能会被墙
 ·· 4."mirror.ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha" 
      ##ghproxy代理的raw文件，大多数情况可用，不过不稳定
      ##前面的"ghproxy.com/"可以不写(如果你是国外机),或者换成你自建的github加速服务均可(需要支持https)
 ·· 5."jsd.cdn.zzko.cn/gh/KeyPJ/FetchData@main/data/gacha"
      ##jsdelivr代理的文件，大多数情况可用，推荐
 ```
-**也可以将上述4和5中的`KeyPJ`更改为`forchannot`，或者自己尝试复制json文件到数据目录`{bot_dir}/data/genshin_history`**
+```
+send_type: Literal["forward", "pic"]
+# 结果发送方式
+forward: 使用合并转发的方式发送
+pic: 使用图片发送
+
+pic_font_path: str
+# 图片发送所需要的字体
+# windows上无需配置，有默认的msyh字体，linux需自行配置
+```
+**也可以自己尝试复制json文件到数据目录`{bot_dir}/data/genshin_history`**
 
 ## 🎉 使用
 ### 指令表
 #### 用前提示，本插件采用on_keyword，不需要带你设置的command_start，当然，如果你非要带，本插件做了一定的处理
 |        指令        |  权限   | 需要@ | 范围  |                                说明                                |
 |:----------------:|:-----:|:---:|:---:|:----------------------------------------------------------------:|
 | [name]历史卡池(num)  |  ALL  |  否  | ALL | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
@@ -138,9 +149,9 @@
 <summary>刷新卡池/别名效果图</summary>
 <img src="https://jsd.cdn.zzko.cn/gh/forchannot/mypicgo@main/20230324/image.5zl59kpx8b00.jpg" alt="help">
 </details>
 
 
 ### 鸣谢
 
-[genshin-gacha-banners](https://github.com/KeyPJ/genshin-gacha-banners) #历史up卡池来源
+[FetchData](https://github.com/KeyPJ/FetchData) #历史up卡池来源，感谢
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 1.2.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 1.3.0 Summary:
 Nonebot2æ¥è¯¢åç¥åå²å¡æ± å°æä»¶ License: MIT Author: forchannot
 Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: httpx (>=0.20.0,<1.0.0)
@@ -23,34 +23,38 @@
 install nonebot-plugin-gshisbanner pip pip install nonebot-plugin-gshisbanner
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_gshisbanner"] ##
 âï¸ éç½® ``` gshisbanner_forward_length: int #
 åæ¬¡åå¹¶è½¬åæ¶æ¯é¿åº¦ï¼intï¼,é»è®¤ä¸º10 # ä»ä¸ºè§è²/
 æ­¦å¨å¡æ± è½¬ååå®¹é¿åº¦ï¼ä¸åæ¬çæ¬å¡æ±  #
 è¶å¤§åæ¬¡è½¬ååå®¹æ´å¤ï¼åå¹¶è½¬åçæ¬¡æ°æ´å°ï¼è¶å°ååæ¬¡è½¬ååå®¹æ´å°ï¼ä½åå¹¶è½¬åçæ¬¡æ°æ´å¤
-# ä¸è¦è®¾ç½®ä¸º>99æè<0çæ°å­æèä»»æå­ç¬¦ä¸²
+# ä¸è¦è®¾ç½®ä¸º>99æè<0çæ°å­æèä»»æå­ç¬¦ä¸² ``` ```
 gshisbanner_json_url: str # åå²å¡æ± jsonåè¡¨ä¸è½½ä½ç½® # å¯éå¼ Â·Â·
 1."banners.52v6.com/data" #é»è®¤ï¼æ¨è Â·Â· 2."genshin-gacha-
 banners.vercel.app/data" #vercelä»£çï¼å½åå¯è½æ æ³ç´è¿ Â·Â·
 3."genshin-gacha-banners.52v6.com/data" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â·
 4."mirror.ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/
 data/gacha"
 ##ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼ä¸è¿ä¸ç¨³å®
 ##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
 (å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
 (éè¦æ¯æhttps) Â·Â· 5."jsd.cdn.zzko.cn/gh/KeyPJ/FetchData@main/data/gacha"
-##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ```
-**ä¹å¯ä»¥å°ä¸è¿°4å5ä¸­ç`KeyPJ`æ´æ¹ä¸º`forchannot`ï¼æèèªå·±å°è¯å¤å¶jsonæä»¶å°æ°æ®ç®å½`
-{bot_dir}/data/genshin_history`** ## ð ä½¿ç¨ ### æä»¤è¡¨ ####
+##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ``` ``` send_type:
+Literal["forward", "pic"] # ç»æåéæ¹å¼ forward:
+ä½¿ç¨åå¹¶è½¬åçæ¹å¼åé pic: ä½¿ç¨å¾çåé pic_font_path: str #
+å¾çåéæéè¦çå­ä½ #
+windowsä¸æ ééç½®ï¼æé»è®¤çmsyhå­ä½ï¼linuxéèªè¡éç½® ```
+**ä¹å¯ä»¥èªå·±å°è¯å¤å¶jsonæä»¶å°æ°æ®ç®å½`{bot_dir}/data/
+genshin_history`** ## ð ä½¿ç¨ ### æä»¤è¡¨ ####
 ç¨åæç¤ºï¼æ¬æä»¶éç¨on_keywordï¼ä¸éè¦å¸¦ä½ è®¾ç½®çcommand_startï¼å½ç¶ï¼å¦æä½ éè¦å¸¦ï¼æ¬æä»¶åäºä¸å®çå¤ç
 | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:----------------:|:-----:|:--
 -:|:---:|:----------------------------------------------------------------:| |
 [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
 | | [version]å¡æ± [num] | ALL | å¦ | ALL |
 versionä¸ºçæ¬å·ï¼å¦1.3ï¼2.6ç­ï¼numä¸º1-
 3ï¼å¯¹åºä¸åï¼ä¸­ï¼ä¸åï¼å¯ä¸å¡«ï¼å¦ä¸å¡«ååéè¯¥çæ¬å¨é¨å¡æ± 
 | | å·æ°(æ´æ°)åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
 å·æ°åå²å¡æ± æå«å | ### ææå¾ åå²å¡æ± ææå¾ å¾1
 [help]å¾2 [help]å¾3 [help]çæ¬å¡æ± ææå¾ å¾1 [help]å¾2 [help]å¾3
-[help]å·æ°å¡æ± /å«åææå¾ [help]### é¸£è°¢ [genshin-gacha-banners]
-(https://github.com/KeyPJ/genshin-gacha-banners) #åå²upå¡æ± æ¥æº
+[help]å·æ°å¡æ± /å«åææå¾ [help]### é¸£è°¢ [FetchData](https://
+github.com/KeyPJ/FetchData) #åå²upå¡æ± æ¥æºï¼æè°¢
```

