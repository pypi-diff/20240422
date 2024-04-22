# Comparing `tmp/mcfetch-1.1.0.tar.gz` & `tmp/mcfetch-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcfetch-1.1.0.tar", last modified: Sat Aug 26 23:04:02 2023, max compression
+gzip compressed data, was "mcfetch-2.0.0.tar", last modified: Mon Apr 22 00:40:41 2024, max compression
```

## Comparing `mcfetch-1.1.0.tar` & `mcfetch-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 23:04:02.179304 mcfetch-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (999)     1108 2023-08-26 23:03:50.000000 mcfetch-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     3177 2023-08-26 23:04:02.179304 mcfetch-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2719 2023-08-26 23:03:50.000000 mcfetch-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 23:04:02.175304 mcfetch-1.1.0/mcfetch/
--rw-r--r--   0 runner    (1001) docker     (999)      692 2023-08-26 23:03:50.000000 mcfetch-1.1.0/mcfetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4784 2023-08-26 23:03:50.000000 mcfetch-1.1.0/mcfetch/asyncmcfetch.py
--rw-r--r--   0 runner    (1001) docker     (999)     4147 2023-08-26 23:03:50.000000 mcfetch-1.1.0/mcfetch/mcfetch.py
--rw-r--r--   0 runner    (1001) docker     (999)     1776 2023-08-26 23:03:50.000000 mcfetch-1.1.0/mcfetch/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 23:04:02.179304 mcfetch-1.1.0/mcfetch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3177 2023-08-26 23:04:02.000000 mcfetch-1.1.0/mcfetch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      358 2023-08-26 23:04:02.000000 mcfetch-1.1.0/mcfetch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-26 23:04:02.000000 mcfetch-1.1.0/mcfetch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       59 2023-08-26 23:04:02.000000 mcfetch-1.1.0/mcfetch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       14 2023-08-26 23:04:02.000000 mcfetch-1.1.0/mcfetch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-26 23:04:02.179304 mcfetch-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      812 2023-08-26 23:03:50.000000 mcfetch-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-26 23:04:02.179304 mcfetch-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-26 23:03:50.000000 mcfetch-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3366 2023-08-26 23:03:50.000000 mcfetch-1.1.0/tests/test_async_fetch_player.py
--rw-r--r--   0 runner    (1001) docker     (999)     3078 2023-08-26 23:03:50.000000 mcfetch-1.1.0/tests/test_fetch_player.py
--rw-r--r--   0 runner    (1001) docker     (999)      593 2023-08-26 23:03:50.000000 mcfetch-1.1.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:40:41.113416 mcfetch-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 00:40:32.000000 mcfetch-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-22 00:40:41.109416 mcfetch-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-22 00:40:32.000000 mcfetch-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:40:41.109416 mcfetch-2.0.0/mcfetch/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-22 00:40:32.000000 mcfetch-2.0.0/mcfetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-22 00:40:32.000000 mcfetch-2.0.0/mcfetch/asyncmcfetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-22 00:40:32.000000 mcfetch-2.0.0/mcfetch/mcfetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-22 00:40:32.000000 mcfetch-2.0.0/mcfetch/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:40:41.109416 mcfetch-2.0.0/mcfetch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-22 00:40:41.000000 mcfetch-2.0.0/mcfetch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 00:40:41.000000 mcfetch-2.0.0/mcfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 00:40:41.000000 mcfetch-2.0.0/mcfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 00:40:41.000000 mcfetch-2.0.0/mcfetch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 00:40:41.000000 mcfetch-2.0.0/mcfetch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 00:40:41.113416 mcfetch-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-22 00:40:32.000000 mcfetch-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 00:40:41.109416 mcfetch-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 00:40:32.000000 mcfetch-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-22 00:40:32.000000 mcfetch-2.0.0/tests/test_async_fetch_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-22 00:40:32.000000 mcfetch-2.0.0/tests/test_fetch_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-22 00:40:32.000000 mcfetch-2.0.0/tests/test_tools.py
```

### Comparing `mcfetch-1.1.0/LICENSE` & `mcfetch-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcfetch-1.1.0/PKG-INFO` & `mcfetch-2.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,92 @@
-Metadata-Version: 2.1
-Name: mcfetch
-Version: 1.1.0
-Summary: Modified version of mcuuid - fetches Minecraftplayer information from the Mojang API
-Home-page: https://github.com/oDepleted/mcfetch
-Author: oDepleted
-Author-email: contact@statalytics.net
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MCFETCH
+
 Fetches Minecraft player information from the Mojang API
 
 ## Installation
+
 Run the following:
+
 ```bash
 pip install mcfetch
 ```
+
 ## How to use
 
 ### Non asynchronous
+
 Fetch a player using their username:
+
 ```python
->>> from mcfetch import FetchPlayer
->>> player = FetchPlayer(name="gronkh")
+>>> from mcfetch import Player
+>>> player = Player(player="gronkh")
 >>> player.name
 'Gronkh'
 >>> player.uuid
 'a2080281c2784181b961d99ed2f3347c'
 ```
 
 Fetch a player using their uuid:
 
 ```python
->>> from mcfetch import FetchPlayer
->>> player = FetchPlayer(uuid="a2080281c2784181b961d99ed2f3347c")
+>>> from mcfetch import Player
+>>> player = Player(player="a2080281c2784181b961d99ed2f3347c")
 >>> player.name
 'Gronkh'
 ```
 
 If a player doesn't exist:
 
 ```python
->>> from mcfetch import FetchPlayer
->>> player = FetchPlayer(name="ThisUsernameIsNotValid")
+>>> from mcfetch import Player
+>>> player = Player(player="ThisUsernameIsNotValid")
 >>> player.name
 None
 >>> player.uuid
 None
 ```
 
 It is also possible to use a custom requests object:
 
 ```python
->>> from mcfetch import FetchPlayer
+>>> from mcfetch import Player
 >>> from requests_cache import CachedSession
 >>> my_cache = CachedSession(cache_name='./my_cache', expire_after=60)
->>> player = FetchPlayer(name="gronkh", requests_obj=my_cache)
+>>> player = Player(player="gronkh", requests_obj=my_cache)
 ```
 
 You can fetch a player's skin URL and skin texture
+
 ```python
->>> from mcfetch import FetchPlayer
->>> player = FetchPlayer(name="Notch")
+>>> from mcfetch import Player
+>>> player = Player(player="Notch")
 >>> player.skin_url
 'http://textures.minecraft.net/texture/292009a4925b58f02c77dadc3ecef07ea4c7472f64e0fdc32ce5522489362680'
 >>> player.skin_texture
 b'\x89PNG\r\n\x1a\n\x00\x00\x00\...'
 ```
 
-Fetch a player without specifying whether you are using a Username or UUID
-```python
->>> from mcfetch import FetchPlayer2
->>> player = FetchPlayer2("a2080281c2784181b961d99ed2f3347c")
->>> player.name
-'Gronkh'
->>> player = FetchPlayer2("Gronkh")
->>> player.uuid
-'a2080281c2784181b961d99ed2f3347c'
-```
-
-
 ### Asynchronous
+
 Fetching a player (same functionality as the above examples)
+
 ```python
 >>> import asyncio
->>> from mcfetch import AsyncFetchPlayer2
+>>> from mcfetch import AsyncPlayer
 >>> async def main():
-...     player = AsyncFetchPlayer2("Gronkh")
+...     player = AsyncPlayer(player="Gronkh")
 ...     print(await player.name)
 ...     print(await player.uuid)
 >>> asyncio.run(main())
 'Gronkh'
 'a2080281c2784181b961d99ed2f3347c'
 ```
 
-
 ## Tools
+
 Check syntax of a username:
 
 ```python
 >>> from mcfetch import is_valid_username
 >>> is_valid_username('gronkh')
 True
 >>> is_valid_username('gronkh-is cool')
@@ -120,12 +104,21 @@
 ```
 
 Remove dashes from a UUID:
 
 ```python
 >>> from mcfetch import undash_uuid
 >>> undash_uuid('a2080281-c278-4181-b961-d99ed2f3347c')
-a2080281c2784181b961d99ed2f3347c
+'a2080281c2784181b961d99ed2f3347c'
+```
+
+Added dashes to a UUID:
+
+```python
+>>> from mcfetch import dash_uuid
+>>> dash_uuid('a2080281c2784181b961d99ed2f3347c')
+'a2080281-c278-4181-b961-d99ed2f3347c'
 ```
 
 ## License
+
 This software is licensed under the MIT license. Feel free to use it however you like. For more infomation see [LICENSE](https://github.com/oDepleted/mcfetch/blob/master/LICENSE).
```

### Comparing `mcfetch-1.1.0/mcfetch/__init__.py` & `mcfetch-2.0.0/mcfetch/__init__.py`

 * *Files identical despite different names*

### Comparing `mcfetch-1.1.0/mcfetch/asyncmcfetch.py` & `mcfetch-2.0.0/mcfetch/asyncmcfetch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import json
 from base64 import b64decode
 
 from aiohttp import ClientSession
 from aiohttp_client_cache import CacheBackend, CachedSession
 
 
-class AsyncFetchPlayer:
+class AsyncPlayer:
     def __init__(
         self,
-        name: str=None,
-        uuid: str=None,
+        player: str,
         cache_backend: CacheBackend=None
     ):
         """
-        Initializes a FetchPlayer object with a name and/or uuid.
+        Initializes an AsyncPlayer object with a name or uuid.
 
         Args:
-            name (str, optional): The player's name. Defaults to None.
-            uuid (str, optional): The player's uuid. Defaults to None.
+            player (str): The player's username or uuid.
             cache_backend (class, optional): The backend used for caching
             responses, if `None`, caching won't be used.
 
         Raises:
             AssertionError: If both name and uuid are None or if both are not None.
         """
-        assert (name, uuid).count(None) == 1
-        self._name = name
-        self._uuid = uuid
+        self._uuid = None
+        self._name = None
+
+        if len(player) > 16:
+            self._uuid = player
+        else:
+            self._name = player
 
         self._pretty_name = None
 
         self._skin_url = None
         self._skin_texture = None
 
         self._player_exists = True
@@ -124,29 +126,7 @@
                     encoded_str = item.get('value', '')
                     textures: dict = json.loads(b64decode(encoded_str) or '{}')
 
                     self._skin_url = textures.get('textures', {}).get('SKIN', {}).get('url')
                     break
 
             self._has_loaded_by_uuid == True
-
-
-class AsyncFetchPlayer2(AsyncFetchPlayer):
-    def __init__(
-        self,
-        identifier: str,
-        cache_backend: CacheBackend=None
-    ):
-        """
-        Wrapper for the `FetchPlayer` class that allows either a username or uuid to
-        be passed as the `identifier` parameter. Whether the identifier is a username
-        or uuid will be determined by its length.
-
-        Args:
-            identifier (str, optional): The player's username or uuid.
-            cache_backend (class, optional): The backend used for caching
-            responses, if `None`, caching won't be used.
-        """
-        if len(identifier) > 16:
-            super().__init__(uuid=identifier, cache_backend=cache_backend)
-        else:
-            super().__init__(name=identifier, cache_backend=cache_backend)
```

### Comparing `mcfetch-1.1.0/mcfetch/mcfetch.py` & `mcfetch-2.0.0/mcfetch/mcfetch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import json
 from base64 import b64decode
 
 import requests
 
 
-class FetchPlayer:
+class Player:
     def __init__(
         self,
-        name: str=None,
-        uuid: str=None,
+        player: str,
         requests_obj=requests
     ):
         """
-        Initializes a FetchPlayer object with a name and/or uuid.
+        Initializes a Player object with a name or uuid.
 
         Args:
-            name (str, optional): The player's name. Defaults to None.
-            uuid (str, optional): The player's uuid. Defaults to None.
+            player (str): The player's username or uuid.
             requests_obj (module, optional): The requests module or a compatible
             object to use for making HTTP requests. Defaults to the requests module.
 
         Raises:
             AssertionError: If both name and uuid are None or if both are not None.
         """
-        assert (name, uuid).count(None) == 1
-        self._name = name
-        self._uuid = uuid
+        self._uuid = None
+        self._name = None
+
+        if len(player) > 16:
+            self._uuid = player
+        else:
+            self._name = player
 
         self._pretty_name = None
 
         self._skin_url = None
         self._skin_texture = None
 
         self._player_exists = True
@@ -106,25 +108,7 @@
             for item in data.get('properties', []):
                 if item.get('name') == 'textures':
                     encoded_str = item.get('value', '')
                     textures: dict = json.loads(b64decode(encoded_str) or '{}')
 
                     self._skin_url = textures.get('textures', {}).get('SKIN', {}).get('url')
                     break
-
-
-class FetchPlayer2(FetchPlayer):
-    def __init__(self, identifier: str, requests_obj=requests):
-        """
-        Wrapper for the `FetchPlayer` class that allows either a username or uuid to
-        be passed as the `identifier` parameter. Whether the identifier is a username
-        or uuid will be determined by its length.
-
-        Args:
-            identifier (str, optional): The player's username or uuid.
-            requests_obj (module | class, optional): The requests module or a compatible
-            object to use for making HTTP requests. Defaults to the requests module.
-        """
-        if len(identifier) > 16:
-            super().__init__(uuid=identifier, requests_obj=requests_obj)
-        else:
-            super().__init__(name=identifier, requests_obj=requests_obj)
```

### Comparing `mcfetch-1.1.0/mcfetch/tools.py` & `mcfetch-2.0.0/mcfetch/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,7 +70,23 @@
 
     Returns:
         str: The UUID string with dashes removed.
     """
     uuid = uuid.lower()
     uuid = uuid.replace('-', '')
     return uuid
+
+
+def dash_uuid(uuid: str):
+    """
+    Inserts dashes (-) at the standard positions in a UUID string.
+
+    Args:
+        uuid: A string representation of a UUID without dashes.
+
+    Returns:
+        A string representation of the UUID with dashes inserted.
+    """
+    if len(uuid) != 32:
+        raise ValueError("Invalid UUID string length. Must be 32 characters.")
+
+    return f"{uuid[0:8]}-{uuid[8:12]}-{uuid[12:16]}-{uuid[16:20]}-{uuid[20:]}"
```

### Comparing `mcfetch-1.1.0/setup.py` & `mcfetch-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mcfetch",
-    version="1.1.0",
+    version="2.0.0",
     author="oDepleted",
     author_email="contact@statalytics.net",
     description="Modified version of mcuuid - fetches Minecraft"
                 "player information from the Mojang API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/oDepleted/mcfetch",
```

### Comparing `mcfetch-1.1.0/tests/test_fetch_player.py` & `mcfetch-2.0.0/tests/test_async_fetch_player.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,84 @@
-from mcfetch import FetchPlayer, FetchPlayer2
+import pytest
+
+from aiohttp_client_cache import SQLiteBackend
+from mcfetch import AsyncPlayer
 from requests_cache import CachedSession
 
 
-class BaseTestFetchPlayer:
+class _TestAsyncPlayerBase:
     def setup_method(self):
-        self.existing_player = self.get_existing_player_instance()
-        self.non_existing_player = self.get_non_existing_player_instance()
+        self.existing_player: AsyncPlayer = \
+            self.get_existing_player_instance()
+
+        self.non_existing_player: AsyncPlayer = \
+            self.get_non_existing_player_instance()
+
 
     def test_fetch_player_init(self):
         assert self.existing_player
 
-    def test_fetch_player_uuid_by_existing_player(self):
-        assert self.existing_player.uuid is not None
+    @pytest.mark.asyncio
+    async def test_fetch_player_uuid_by_existing_player(self):
+        assert await self.existing_player.uuid is not None
 
-    def test_fetch_player_name_by_existing_player(self):
-        assert self.existing_player.name is not None
+    @pytest.mark.asyncio
+    async def test_fetch_player_name_by_existing_player(self):
+        assert await self.existing_player.name is not None
 
-    def test_fetch_player_name_by_non_existing_player(self):
-        assert self.non_existing_player.name is None
+    @pytest.mark.asyncio
+    async def test_fetch_player_name_by_non_existing_player(self):
+        assert await self.non_existing_player.name is None
 
-    def test_fetch_player_skin_url_by_existing_player(self):
-        assert self.existing_player.skin_url is not None
+    @pytest.mark.asyncio
+    async def test_fetch_player_skin_url_by_existing_player(self):
+        assert await self.existing_player.skin_url is not None
 
-    def test_fetch_player_skin_url_by_non_existing_player(self):
-        assert self.non_existing_player.skin_url is None
+    @pytest.mark.asyncio
+    async def test_fetch_player_skin_url_by_non_existing_player(self):
+        assert await self.non_existing_player.skin_url is None
 
-    def test_fetch_player_skin_texture_by_existing_player(self):
-        assert self.existing_player.skin_texture is not None
+    @pytest.mark.asyncio
+    async def test_fetch_player_skin_texture_by_existing_player(self):
+        assert await self.existing_player.skin_texture is not None
 
-    def test_fetch_player_skin_texture_by_non_existing_player(self):
-        assert self.non_existing_player.skin_texture is None
+    @pytest.mark.asyncio
+    async def test_fetch_player_skin_texture_by_non_existing_player(self):
+        assert await self.non_existing_player.skin_texture is None
 
 
 
-class TestFetchPlayerByName(BaseTestFetchPlayer):
+class TestAsyncPlayerByName(_TestAsyncPlayerBase):
     def get_existing_player_instance(self):
-        return FetchPlayer(name='Notch')
+        return AsyncPlayer(player='Notch')
 
     def get_non_existing_player_instance(self):
-        return FetchPlayer(name='Bitch')
+        return AsyncPlayer(player='Bitch')
 
 
-class TestFetchPlayerByUUID(BaseTestFetchPlayer):
+class TestAsyncPlayerByUUID(_TestAsyncPlayerBase):
     def get_existing_player_instance(self):
-        return FetchPlayer(uuid='069a79f444e94726a5befca90e38aaf5')
+        return AsyncPlayer(player='069a79f444e94726a5befca90e38aaf5')
 
     def get_non_existing_player_instance(self):
-        return FetchPlayer(uuid='abcdefghijklmnopqrstuvwxyz')
-
+        return AsyncPlayer(player='abcdefghijklmnopqrstuvwxyz')
 
 
-session = CachedSession(cache_name='.cache/test', expire_after=60)
-
-class TestFetchPlayerByNameWithCaching(BaseTestFetchPlayer):
-    def get_existing_player_instance(self):
-        return FetchPlayer(name='Notch', requests_obj=session)
-
-    def get_non_existing_player_instance(self):
-        return FetchPlayer(name='Bitch', requests_obj=session)
-
-
-class TestFetchPlayerByUUIDWithCaching(BaseTestFetchPlayer):
-    def get_existing_player_instance(self):
-        return FetchPlayer(
-            uuid='069a79f444e94726a5befca90e38aaf5', requests_obj=session)
-
-    def get_non_existing_player_instance(self):
-        return FetchPlayer(
-            uuid='abcdefghijklmnopqrstuvwxyz', requests_obj=session)
 
+session = SQLiteBackend(cache_name='.cache/test', expire_after=60)
 
-class TestFetchPlayerDynamicallyByNameWithCaching(BaseTestFetchPlayer):
+class TestAsyncPlayerByNameWithCaching(_TestAsyncPlayerBase):
     def get_existing_player_instance(self):
-        return FetchPlayer2(
-            'Notch', requests_obj=session)
+        return AsyncPlayer(player='Notch', cache_backend=session)
 
     def get_non_existing_player_instance(self):
-        return FetchPlayer2(
-            'Bitch', requests_obj=session)
+        return AsyncPlayer(player='Bitch', cache_backend=session)
 
 
-class TestFetchPlayerDynamicallyByUUIDWithCaching(BaseTestFetchPlayer):
+class TestAsyncPlayerByUUIDWithCaching(_TestAsyncPlayerBase):
     def get_existing_player_instance(self):
-        return FetchPlayer2(
-            '069a79f444e94726a5befca90e38aaf5', requests_obj=session)
+        return AsyncPlayer(
+            player='069a79f444e94726a5befca90e38aaf5', cache_backend=session)
 
     def get_non_existing_player_instance(self):
-        return FetchPlayer2(
-            'abcdefghijklmnopqrstuvwxyz', requests_obj=session)
+        return AsyncPlayer(
+            player='abcdefghijklmnopqrstuvwxyz', cache_backend=session)
```

### Comparing `mcfetch-1.1.0/tests/test_tools.py` & `mcfetch-2.0.0/tests/test_tools.py`

 * *Files identical despite different names*

