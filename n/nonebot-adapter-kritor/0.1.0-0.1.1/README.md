# Comparing `tmp/nonebot_adapter_kritor-0.1.0.tar.gz` & `tmp/nonebot_adapter_kritor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_kritor-0.1.0.tar", last modified: Thu Apr 18 11:03:46 2024, max compression
+gzip compressed data, was "nonebot_adapter_kritor-0.1.1.tar", last modified: Mon Apr 22 09:08:15 2024, max compression
```

## Comparing `nonebot_adapter_kritor-0.1.0.tar` & `nonebot_adapter_kritor-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1064 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/LICENSE
--rw-r--r--   0        0        0     1042 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/README.md
--rw-r--r--   0        0        0     2262 2024-04-18 11:03:46.214179 nonebot_adapter_kritor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      244 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/__init__.py
--rw-r--r--   0        0        0     7191 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/adapter.py
--rw-r--r--   0        0        0    55211 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/bot.py
--rw-r--r--   0        0        0      618 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/compat.py
--rw-r--r--   0        0        0      451 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/config.py
--rw-r--r--   0        0        0    21042 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/event.py
--rw-r--r--   0        0        0     2482 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/exception.py
--rw-r--r--   0        0        0    15139 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/message.py
--rw-r--r--   0        0        0     1665 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/model.py
--rw-r--r--   0        0        0        0 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/__init__.py
--rw-r--r--   0        0        0     9573 2024-04-18 11:03:16.410174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/authentication/__init__.py
--rw-r--r--   0        0        0    13153 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/common/__init__.py
--rw-r--r--   0        0        0     7604 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/core/__init__.py
--rw-r--r--   0        0        0     1965 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/customization/__init__.py
--rw-r--r--   0        0        0    15256 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/developer/__init__.py
--rw-r--r--   0        0        0    14777 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/event/__init__.py
--rw-r--r--   0        0        0    13287 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/file/__init__.py
--rw-r--r--   0        0        0    16773 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/friend/__init__.py
--rw-r--r--   0        0        0    34177 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/group/__init__.py
--rw-r--r--   0        0        0    28678 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/guild/__init__.py
--rw-r--r--   0        0        0    26122 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/message/__init__.py
--rw-r--r--   0        0        0     6218 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/process/__init__.py
--rw-r--r--   0        0        0     2267 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/reverse/__init__.py
--rw-r--r--   0        0        0     7047 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/web/__init__.py
--rw-r--r--   0        0        0     1188 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/utils.py
--rw-r--r--   0        0        0        0 2024-04-18 11:03:16.414174 nonebot_adapter_kritor-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 nonebot_adapter_kritor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 09:07:47.013935 nonebot_adapter_kritor-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1042 2024-04-22 09:07:47.013935 nonebot_adapter_kritor-0.1.1/README.md
+-rw-r--r--   0        0        0     2262 2024-04-22 09:08:15.218109 nonebot_adapter_kritor-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      244 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/__init__.py
+-rw-r--r--   0        0        0     7191 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/adapter.py
+-rw-r--r--   0        0        0    55211 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/bot.py
+-rw-r--r--   0        0        0      618 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/compat.py
+-rw-r--r--   0        0        0      451 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/config.py
+-rw-r--r--   0        0        0    21042 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/event.py
+-rw-r--r--   0        0        0     2482 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/exception.py
+-rw-r--r--   0        0        0    15038 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/message.py
+-rw-r--r--   0        0        0     1665 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/model.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/__init__.py
+-rw-r--r--   0        0        0     9573 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/authentication/__init__.py
+-rw-r--r--   0        0        0    13153 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/common/__init__.py
+-rw-r--r--   0        0        0     7604 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/core/__init__.py
+-rw-r--r--   0        0        0     1965 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/customization/__init__.py
+-rw-r--r--   0        0        0    15256 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/developer/__init__.py
+-rw-r--r--   0        0        0    14777 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/event/__init__.py
+-rw-r--r--   0        0        0    13287 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/file/__init__.py
+-rw-r--r--   0        0        0    16773 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/friend/__init__.py
+-rw-r--r--   0        0        0    34177 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/group/__init__.py
+-rw-r--r--   0        0        0    28678 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/guild/__init__.py
+-rw-r--r--   0        0        0    26122 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/message/__init__.py
+-rw-r--r--   0        0        0     6218 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/process/__init__.py
+-rw-r--r--   0        0        0     2267 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/reverse/__init__.py
+-rw-r--r--   0        0        0     7047 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/web/__init__.py
+-rw-r--r--   0        0        0     1188 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/utils.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:07:47.017935 nonebot_adapter_kritor-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 nonebot_adapter_kritor-0.1.1/PKG-INFO
```

### Comparing `nonebot_adapter_kritor-0.1.0/LICENSE` & `nonebot_adapter_kritor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/README.md` & `nonebot_adapter_kritor-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/pyproject.toml` & `nonebot_adapter_kritor-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-adapter-kritor"
-version = "0.1.0"
+version = "0.1.1"
 description = "Nonebot Adapter for Kritor Protocol"
 authors = [
     { name = "rf_tar_railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "betterproto>=2.0.0b6",
     "nonebot2>=2.2.1",
```

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/adapter.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/bot.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/compat.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/event.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/exception.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/message.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 
 from nonebot.adapters import Message as BaseMessage
 from nonebot.adapters import MessageSegment as BaseMessageSegment
 
 from .model import SceneType
 from .protos.kritor.common import Scene as KritorScene
 from .protos.kritor.common import (
+    Button,
     Element,
+    KeyboardRow,
     ContactElement,
+    KeyboardElement,
     ElementElementType,
     ImageElementImageType,
     MusicElementMusicPlatform,
 )
 
 
 class MessageSegment(BaseMessageSegment["Message"]):
@@ -200,16 +203,16 @@
         return Xml("xml", {"xml": xml})
 
     @staticmethod
     def markdown(markdown: str) -> "Markdown":
         return Markdown("markdown", {"markdown": markdown})
 
     @staticmethod
-    def button(bot_appid: int, rows: list[list["ButtonData"]]) -> "Keyboard":
-        return Keyboard("button", {"bot_appid": bot_appid, "rows": [{"buttons": row} for row in rows]})
+    def keyboard(bot_appid: int, buttons: list[list[Button]]) -> "Keyboard":
+        return Keyboard("keyboard", {"bot_appid": bot_appid, "rows": [{"buttons": row} for row in buttons]})
 
 
 class TextData(TypedDict):
     text: str
 
 
 @dataclass
@@ -476,54 +479,37 @@
 
 
 @dataclass
 class Markdown(MessageSegment, element_type=ElementElementType.MARKDOWN):
     data: MarkdownData = field(default_factory=dict)  # type: ignore
 
 
-class ButtonActionPermissionData(TypedDict):
-    type: int
-    role_ids: list[int]
-    user_ids: list[int]
-
-
-class ButtonActionData(TypedDict):
-    type: int
-    permission: ButtonActionPermissionData
-    unsupported_tips: str
-    data: str
-    reply: bool
-    enter: bool
-
-
-class ButtonRenderData(TypedDict):
-    label: str
-    visited_label: str
-    style: int
-
-
-class ButtonData(TypedDict):
-    id: str
-    render_data: ButtonRenderData
-    action: ButtonActionData
-
-
 class KeyboardRowData(TypedDict):
-    buttons: list[ButtonData]
+    buttons: list[Button]
 
 
 class KeyboardData(TypedDict):
     rows: list[KeyboardRowData]
     bot_appid: int
 
 
 @dataclass
 class Keyboard(MessageSegment, element_type=ElementElementType.KEYBOARD):
     data: KeyboardData = field(default_factory=dict)  # type: ignore
 
+    @override
+    def dump(self) -> "Element":
+        return Element(
+            type=ElementElementType.KEYBOARD,
+            keyboard=KeyboardElement(
+                rows=[KeyboardRow(buttons=row["buttons"]) for row in self.data["rows"]],
+                bot_appid=self.data["bot_appid"],
+            ),
+        )
+
 
 TYPE_MAPPING = {cls.__element_type__: cls for cls in MessageSegment.__subclasses__()}  # type: ignore
 
 
 class Message(BaseMessage[MessageSegment]):
     @classmethod
     @override
```

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/model.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/authentication/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/common/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/core/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/customization/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/customization/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/developer/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/developer/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/event/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/event/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/file/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/friend/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/friend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/group/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/group/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/guild/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/guild/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/message/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/message/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/process/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/reverse/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/reverse/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/protos/kritor/web/__init__.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/protos/kritor/web/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/src/nonebot/adapters/kritor/utils.py` & `nonebot_adapter_kritor-0.1.1/src/nonebot/adapters/kritor/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kritor-0.1.0/PKG-INFO` & `nonebot_adapter_kritor-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-kritor
-Version: 0.1.0
+Version: 0.1.1
 Summary: Nonebot Adapter for Kritor Protocol
 Author-Email: rf_tar_railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: betterproto>=2.0.0b6
 Requires-Dist: nonebot2>=2.2.1
 Description-Content-Type: text/markdown
```

