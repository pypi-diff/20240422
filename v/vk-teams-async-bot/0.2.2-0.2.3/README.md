# Comparing `tmp/vk_teams_async_bot-0.2.2.tar.gz` & `tmp/vk_teams_async_bot-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vk_teams_async_bot-0.2.2.tar", max compression
+gzip compressed data, was "vk_teams_async_bot-0.2.3.tar", max compression
```

## Comparing `vk_teams_async_bot-0.2.2.tar` & `vk_teams_async_bot-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1108 2023-12-28 10:42:15.574550 vk_teams_async_bot-0.2.2/LICENSE
--rw-r--r--   0        0        0     1241 2024-04-16 10:20:00.658577 vk_teams_async_bot-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     7032 2024-03-25 10:04:01.896611 vk_teams_async_bot-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-10-20 09:08:44.418623 vk_teams_async_bot-0.2.2/vk_teams_async_bot/__init__.py
--rw-r--r--   0        0        0    20547 2024-04-16 10:16:48.278783 vk_teams_async_bot-0.2.2/vk_teams_async_bot/bot.py
--rw-r--r--   0        0        0     4864 2024-04-16 10:16:38.504694 vk_teams_async_bot-0.2.2/vk_teams_async_bot/client_session.py
--rw-r--r--   0        0        0      848 2023-12-28 10:05:54.075146 vk_teams_async_bot-0.2.2/vk_teams_async_bot/constants.py
--rw-r--r--   0        0        0      700 2024-04-05 12:37:06.616281 vk_teams_async_bot-0.2.2/vk_teams_async_bot/dispatcher.py
--rw-r--r--   0        0        0       60 2024-03-25 13:41:10.135840 vk_teams_async_bot-0.2.2/vk_teams_async_bot/errors.py
--rw-r--r--   0        0        0     3200 2024-03-25 14:08:04.048523 vk_teams_async_bot-0.2.2/vk_teams_async_bot/events.py
--rw-r--r--   0        0        0     4763 2024-04-05 10:44:28.021696 vk_teams_async_bot-0.2.2/vk_teams_async_bot/filter.py
--rw-r--r--   0        0        0     2357 2024-03-25 13:41:10.159392 vk_teams_async_bot-0.2.2/vk_teams_async_bot/handler.py
--rw-r--r--   0        0        0     6086 2024-03-25 13:41:10.174905 vk_teams_async_bot-0.2.2/vk_teams_async_bot/helpers.py
--rw-r--r--   0        0        0      324 2024-03-25 14:12:50.638587 vk_teams_async_bot-0.2.2/vk_teams_async_bot/middleware.py
--rw-r--r--   0        0        0      260 2024-03-25 14:13:20.831674 vk_teams_async_bot-0.2.2/vk_teams_async_bot/schemas.py
--rw-r--r--   0        0        0     7060 2024-03-25 15:11:28.102016 vk_teams_async_bot-0.2.2/vk_teams_async_bot/state.py
--rw-r--r--   0        0        0      519 2023-12-21 14:07:29.369149 vk_teams_async_bot-0.2.2/vk_teams_async_bot/timer.py
--rw-r--r--   0        0        0     7476 1970-01-01 00:00:00.000000 vk_teams_async_bot-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-12-28 10:42:15.574550 vk_teams_async_bot-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1241 2024-04-22 09:19:44.862079 vk_teams_async_bot-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7032 2024-03-25 10:04:01.896611 vk_teams_async_bot-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-10-20 09:08:44.418623 vk_teams_async_bot-0.2.3/vk_teams_async_bot/__init__.py
+-rw-r--r--   0        0        0    20583 2024-04-22 08:23:03.004241 vk_teams_async_bot-0.2.3/vk_teams_async_bot/bot.py
+-rw-r--r--   0        0        0     4864 2024-04-16 10:16:38.504694 vk_teams_async_bot-0.2.3/vk_teams_async_bot/client_session.py
+-rw-r--r--   0        0        0      848 2023-12-28 10:05:54.075146 vk_teams_async_bot-0.2.3/vk_teams_async_bot/constants.py
+-rw-r--r--   0        0        0      700 2024-04-05 12:37:06.616281 vk_teams_async_bot-0.2.3/vk_teams_async_bot/dispatcher.py
+-rw-r--r--   0        0        0       60 2024-03-25 13:41:10.135840 vk_teams_async_bot-0.2.3/vk_teams_async_bot/errors.py
+-rw-r--r--   0        0        0     3200 2024-03-25 14:08:04.048523 vk_teams_async_bot-0.2.3/vk_teams_async_bot/events.py
+-rw-r--r--   0        0        0     4763 2024-04-05 10:44:28.021696 vk_teams_async_bot-0.2.3/vk_teams_async_bot/filter.py
+-rw-r--r--   0        0        0     2357 2024-03-25 13:41:10.159392 vk_teams_async_bot-0.2.3/vk_teams_async_bot/handler.py
+-rw-r--r--   0        0        0     6086 2024-03-25 13:41:10.174905 vk_teams_async_bot-0.2.3/vk_teams_async_bot/helpers.py
+-rw-r--r--   0        0        0      324 2024-03-25 14:12:50.638587 vk_teams_async_bot-0.2.3/vk_teams_async_bot/middleware.py
+-rw-r--r--   0        0        0      260 2024-03-25 14:13:20.831674 vk_teams_async_bot-0.2.3/vk_teams_async_bot/schemas.py
+-rw-r--r--   0        0        0     7060 2024-03-25 15:11:28.102016 vk_teams_async_bot-0.2.3/vk_teams_async_bot/state.py
+-rw-r--r--   0        0        0      519 2023-12-21 14:07:29.369149 vk_teams_async_bot-0.2.3/vk_teams_async_bot/timer.py
+-rw-r--r--   0        0        0     7476 1970-01-01 00:00:00.000000 vk_teams_async_bot-0.2.3/PKG-INFO
```

### Comparing `vk_teams_async_bot-0.2.2/LICENSE` & `vk_teams_async_bot-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.2/pyproject.toml` & `vk_teams_async_bot-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vk-teams-async-bot"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Александр Смирнов <alexsmi4444@gmail.com>"]
 readme = "README.md"
 packages = [{include = "vk_teams_async_bot"}]
 license = "MIT"
 repository = "https://github.com/Quakeer444/vk_teams_async_bot"
```

### Comparing `vk_teams_async_bot-0.2.2/README.md` & `vk_teams_async_bot-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.2/vk_teams_async_bot/bot.py` & `vk_teams_async_bot-0.2.3/vk_teams_async_bot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         :param _format: Description of text formatting.
         :param parse_mode: Mode for processing formatting from message text.
         :param count_request_retries: number of request retries in case of
                500 response from server VK Teams
 
         :return: Response 200 {"ok": true}
         """
-        data = FormData()
+        data = FormData(quote_fields=False)
 
         if file_path:
             data.add_field("file", await async_read_file(file_path), filename=filename)
         if bytes_io_object:
             data.add_field(
                 "file",
                 bytes_io_object,
@@ -446,15 +446,15 @@
         :param parse_mode: Mode for processing formatting from message text.
         :param count_request_retries: number of request retries in case of
                500 response from server VK Teams
 
         :return: Response 200 {"ok": true}
         """
 
-        data = FormData()
+        data = FormData(quote_fields=False)
         data.add_field("file", await async_read_file(file_path), filename=filename)
 
         return await self.session.post_request(
             endpoint="messages/sendVoice",
             chatId=chat_id,
             body=data,
             replyMsgId=reply_msg_id,
```

### Comparing `vk_teams_async_bot-0.2.2/vk_teams_async_bot/client_session.py` & `vk_teams_async_bot-0.2.3/vk_teams_async_bot/client_session.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.2/vk_teams_async_bot/constants.py` & `vk_teams_async_bot-0.2.3/vk_teams_async_bot/constants.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.2/vk_teams_async_bot/dispatcher.py` & `vk_teams_async_bot-0.2.3/vk_teams_async_bot/dispatcher.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.2/vk_teams_async_bot/events.py` & `vk_teams_async_bot-0.2.3/vk_teams_async_bot/events.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.2/vk_teams_async_bot/filter.py` & `vk_teams_async_bot-0.2.3/vk_teams_async_bot/filter.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.2/vk_teams_async_bot/handler.py` & `vk_teams_async_bot-0.2.3/vk_teams_async_bot/handler.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.2/vk_teams_async_bot/helpers.py` & `vk_teams_async_bot-0.2.3/vk_teams_async_bot/helpers.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.2/vk_teams_async_bot/state.py` & `vk_teams_async_bot-0.2.3/vk_teams_async_bot/state.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.2/vk_teams_async_bot/timer.py` & `vk_teams_async_bot-0.2.3/vk_teams_async_bot/timer.py`

 * *Files identical despite different names*

### Comparing `vk_teams_async_bot-0.2.2/PKG-INFO` & `vk_teams_async_bot-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vk-teams-async-bot
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Home-page: https://github.com/Quakeer444/vk_teams_async_bot
 License: MIT
 Author: Александр Смирнов
 Author-email: alexsmi4444@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

