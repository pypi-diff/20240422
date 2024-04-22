# Comparing `tmp/moobius-1.1.8.tar.gz` & `tmp/moobius-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moobius-1.1.8.tar", last modified: Tue Apr 16 23:48:10 2024, max compression
+gzip compressed data, was "moobius-1.1.9.tar", last modified: Mon Apr 22 05:00:33 2024, max compression
```

## Comparing `moobius-1.1.8.tar` & `moobius-1.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.332909 moobius-1.1.8/
--rw-rw-rw-   0        0        0     8910 2024-04-16 23:48:10.331911 moobius-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2024-03-24 16:36:44.000000 moobius-1.1.8/license.md
--rw-rw-rw-   0        0        0      647 2024-04-16 23:28:47.000000 moobius-1.1.8/pyproject.toml
--rw-rw-rw-   0        0        0     8055 2024-03-17 18:58:55.000000 moobius-1.1.8/readme.md
--rw-rw-rw-   0        0        0       42 2024-04-16 23:48:10.332909 moobius-1.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.312366 moobius-1.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.314358 moobius-1.1.8/src/moobius/
--rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.1.8/src/moobius/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.323938 moobius-1.1.8/src/moobius/core/
--rw-rw-rw-   0        0        0    57439 2024-04-16 23:42:53.000000 moobius-1.1.8/src/moobius/core/sdk.py
--rw-rw-rw-   0        0        0     4170 2024-04-01 21:02:47.000000 moobius-1.1.8/src/moobius/core/wand.py
-drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.327926 moobius-1.1.8/src/moobius/database/
--rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.1.8/src/moobius/database/database_interface.py
--rw-rw-rw-   0        0        0     4098 2024-04-16 23:43:03.000000 moobius-1.1.8/src/moobius/database/json_database.py
--rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.1.8/src/moobius/database/null_database.py
--rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.1.8/src/moobius/database/redis_database.py
--rw-rw-rw-   0        0        0     9559 2024-03-26 23:06:54.000000 moobius-1.1.8/src/moobius/database/storage.py
-drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.329919 moobius-1.1.8/src/moobius/network/
--rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.1.8/src/moobius/network/asserts.py
--rw-rw-rw-   0        0        0    44002 2024-04-16 23:40:27.000000 moobius-1.1.8/src/moobius/network/http_api_wrapper.py
--rw-rw-rw-   0        0        0    25652 2024-04-10 03:05:43.000000 moobius-1.1.8/src/moobius/network/ws_client.py
--rw-rw-rw-   0        0        0     7154 2024-04-08 21:51:19.000000 moobius-1.1.8/src/moobius/types.py
--rw-rw-rw-   0        0        0     7399 2024-03-29 15:46:12.000000 moobius-1.1.8/src/moobius/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-16 23:48:10.330915 moobius-1.1.8/src/moobius.egg-info/
--rw-rw-rw-   0        0        0     8910 2024-04-16 23:48:10.000000 moobius-1.1.8/src/moobius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2024-04-16 23:48:10.000000 moobius-1.1.8/src/moobius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 23:48:10.000000 moobius-1.1.8/src/moobius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-04-16 23:48:10.000000 moobius-1.1.8/src/moobius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 23:48:10.000000 moobius-1.1.8/src/moobius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      329 2024-04-08 18:24:26.000000 moobius-1.1.8/src/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.307537 moobius-1.1.9/
+-rw-rw-rw-   0        0        0     8910 2024-04-22 05:00:33.307537 moobius-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2024-03-24 16:36:44.000000 moobius-1.1.9/license.md
+-rw-rw-rw-   0        0        0      647 2024-04-22 02:34:33.000000 moobius-1.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0     8055 2024-03-17 18:58:55.000000 moobius-1.1.9/readme.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 05:00:33.307537 moobius-1.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.287603 moobius-1.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.289596 moobius-1.1.9/src/moobius/
+-rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.1.9/src/moobius/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.297570 moobius-1.1.9/src/moobius/core/
+-rw-rw-rw-   0        0        0    57654 2024-04-22 00:12:14.000000 moobius-1.1.9/src/moobius/core/sdk.py
+-rw-rw-rw-   0        0        0     4170 2024-04-01 21:02:47.000000 moobius-1.1.9/src/moobius/core/wand.py
+drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.302554 moobius-1.1.9/src/moobius/database/
+-rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.1.9/src/moobius/database/database_interface.py
+-rw-rw-rw-   0        0        0     4098 2024-04-16 23:52:13.000000 moobius-1.1.9/src/moobius/database/json_database.py
+-rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.1.9/src/moobius/database/null_database.py
+-rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.1.9/src/moobius/database/redis_database.py
+-rw-rw-rw-   0        0        0     9559 2024-03-26 23:06:54.000000 moobius-1.1.9/src/moobius/database/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.305543 moobius-1.1.9/src/moobius/network/
+-rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.1.9/src/moobius/network/asserts.py
+-rw-rw-rw-   0        0        0    45076 2024-04-22 00:04:45.000000 moobius-1.1.9/src/moobius/network/http_api_wrapper.py
+-rw-rw-rw-   0        0        0    25652 2024-04-10 03:05:43.000000 moobius-1.1.9/src/moobius/network/ws_client.py
+-rw-rw-rw-   0        0        0     7154 2024-04-08 21:51:19.000000 moobius-1.1.9/src/moobius/types.py
+-rw-rw-rw-   0        0        0     7399 2024-03-29 15:46:12.000000 moobius-1.1.9/src/moobius/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 05:00:33.306539 moobius-1.1.9/src/moobius.egg-info/
+-rw-rw-rw-   0        0        0     8910 2024-04-22 05:00:33.000000 moobius-1.1.9/src/moobius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2024-04-22 05:00:33.000000 moobius-1.1.9/src/moobius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 05:00:33.000000 moobius-1.1.9/src/moobius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-04-22 05:00:33.000000 moobius-1.1.9/src/moobius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-22 05:00:33.000000 moobius-1.1.9/src/moobius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      329 2024-04-08 18:24:26.000000 moobius-1.1.9/src/setup.py
```

### Comparing `moobius-1.1.8/PKG-INFO` & `moobius-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.1.8
+Version: 1.1.9
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.1.8/license.md` & `moobius-1.1.9/license.md`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/pyproject.toml` & `moobius-1.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "moobius"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   { name="Kevin Kostlan", email="sdk@moobius.app"},
 ]
 description = "Moobius Platform SDK"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `moobius-1.1.8/readme.md` & `moobius-1.1.9/readme.md`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/src/moobius/core/sdk.py` & `moobius-1.1.9/src/moobius/core/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -605,14 +605,15 @@
     async def fetch_popular_channels(self): """Calls self.http_api.fetch_popular_channels."""; return await self.http_api.fetch_popular_channels()
     async def fetch_channel_list(self): """Calls self.http_api.fetch_channel_list."""; return await self.http_api.fetch_channel_list()
     async def fetch_real_character_ids(self, channel_id, raise_empty_list_err=True): """Calls self.http_api.fetch_real_character_ids using self.client_id."""; return await self.http_api.fetch_real_character_ids(channel_id, self.client_id, raise_empty_list_err=raise_empty_list_err)
     async def fetch_character_profile(self, character_id): """Calls self.http_api.fetch_character_profile"""; return await self.http_api.fetch_character_profile(character_id)
     async def fetch_service_id_list(self): """Calls self.http_api.fetch_service_id_list"""; return await self.http_api.fetch_service_id_list()
     async def fetch_service_characters(self): """Calls self.http_api.fetch_service_characters using self.client_id."""; return await self.http_api.fetch_service_characters(self.client_id)
     async def upload_file(self, filepath): """Calls self.http_api.upload_file."""; return await self.http_api.upload_file(filepath)
+    async def download_file(self, url, filepath, assert_no_overwrite=False): """Calls self.http_api.download_file"""; return await self.http_api.download_file(url, filepath, assert_no_overwrite=assert_no_overwrite)
     async def fetch_message_history(self, channel_id, limit=1024, before="null"): """Calls self.http_api.fetch_message_history."""; return await self.http_api.fetch_message_history(channel_id, limit, before)
     async def create_channel_group(self, channel_id, group_name, members): """Calls self.http_api.create_channel_group."""; return await self.http_api.create_channel_group(channel_id, group_name, members)
     async def create_service_group(self, group_id, members): """Calls self.http_api.create_service_group."""; return await self.http_api.create_service_group(group_id, members)
     async def character_ids_of_channel_group(self, sender_id, channel_id, group_id): """Calls self.http_api.character_ids_of_channel_group"""; return await self.http_api.character_ids_of_channel_group(sender_id, channel_id, group_id)
     async def character_ids_of_service_group(self, group_id): """Calls self.http_api.character_ids_of_service_group"""; return await self.http_api.character_ids_of_service_group(group_id)
     async def update_channel_group(self, channel_id, group_id, members): """Calls self.http_api.update_channel_group."""; return await self.http_api.update_channel_group(channel_id, group_id, members)
     async def update_temp_channel_group(self, channel_id, members): """Calls self.http_api.update_temp_channel_group."""; return await self.http_api.update_temp_channel_group(channel_id, members)
```

### Comparing `moobius-1.1.8/src/moobius/core/wand.py` & `moobius-1.1.9/src/moobius/core/wand.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/src/moobius/database/database_interface.py` & `moobius-1.1.9/src/moobius/database/database_interface.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/src/moobius/database/json_database.py` & `moobius-1.1.9/src/moobius/database/json_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/src/moobius/database/null_database.py` & `moobius-1.1.9/src/moobius/database/null_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/src/moobius/database/redis_database.py` & `moobius-1.1.9/src/moobius/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/src/moobius/database/storage.py` & `moobius-1.1.9/src/moobius/database/storage.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/src/moobius/network/asserts.py` & `moobius-1.1.9/src/moobius/network/asserts.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/src/moobius/network/http_api_wrapper.py` & `moobius-1.1.9/src/moobius/network/http_api_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,15 +472,14 @@
         requests_kwargs = {'params':{"extension": extension}, 'headers':self.headers}
         response_dict = await self.checked_get(url=self.http_server_uri + "/file/upload", the_request=None, requests_kwargs=requests_kwargs, good_message="Successfully fetched upload url!", bad_message="Error fetching upload url", raise_errors=True)
 
         upload_url = response_dict.get('data').get('url')
         upload_fields = response_dict.get('data').get('fields')
         return upload_url, upload_fields
 
-
     async def _do_upload_file(self, upload_url, upload_fields, file_path):
         """
         Upload a file to the given upload URL with the given upload fields.
 
         Parameters:
           upload_url (str): obtained with _upload_extension.
           upload_fields (dict): obtained with _upload_extension.
@@ -517,14 +516,30 @@
             # Exception will be raised in _do_upload_file(), no need to raise here
             full_url = await self._do_upload_file(upload_url, upload_fields, file_path)
             return full_url
         else:
             logger.error(f"Error getting upload url and upload fields! file_path: {file_path}")
             raise Exception(f"Error getting upload url and upload fields! file_path: {file_path}")
 
+    async def download_file(self, url, filename, assert_no_overwrite=False):
+        """Downloads a file from url to filename, automatically creating dirs and overwriting pre-existing files."""
+        requests_kwargs={'headers':self.headers} # Auth allows downloading form buckets we authed for.
+        # https://stackoverflow.com/questions/35388332/how-to-download-images-with-aiohttp
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url, **requests_kwargs) as resp:
+                if resp.status == 200:
+                    if os.path.exists(filename) and assert_no_overwrite:
+                        raise Exception(f'Assert no overwrite to pre-existing file: {os.path.realpath(filename)}')
+                    os.makedirs(os.path.dirname(filename), exist_ok=True)
+                    with open(filename, 'wb') as fd:
+                        async for chunk in resp.content.iter_chunked(10):
+                            fd.write(chunk)
+                else:
+                    raise Exception(f'Cannot download file: {resp}')
+
     ############################# Groups ############################
 
     async def fetch_channel_group_dict(self, channel_id, service_id):
         """Like fetch_real_character_ids but returns a dict from group_id to all characters."""
         asserts.types_assert(str, channel_id=channel_id, service_id=service_id)
         params = {"channel_id": channel_id, "service_id": service_id}
         rkwargs = {'params':params, 'headers':self.headers}
```

### Comparing `moobius-1.1.8/src/moobius/network/ws_client.py` & `moobius-1.1.9/src/moobius/network/ws_client.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/src/moobius/types.py` & `moobius-1.1.9/src/moobius/types.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/src/moobius/utils.py` & `moobius-1.1.9/src/moobius/utils.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.8/src/moobius.egg-info/PKG-INFO` & `moobius-1.1.9/src/moobius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.1.8
+Version: 1.1.9
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.1.8/src/moobius.egg-info/SOURCES.txt` & `moobius-1.1.9/src/moobius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

