# Comparing `tmp/meta_ai_api-1.1.2.tar.gz` & `tmp/meta_ai_api-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.1.2.tar", last modified: Fri Apr 19 21:56:10 2024, max compression
+gzip compressed data, was "meta_ai_api-1.1.3.tar", last modified: Sun Apr 21 21:23:26 2024, max compression
```

## Comparing `meta_ai_api-1.1.2.tar` & `meta_ai_api-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:56:10.351173 meta_ai_api-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-04-19 21:56:10.351173 meta_ai_api-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-19 21:56:05.000000 meta_ai_api-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 21:56:05.000000 meta_ai_api-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 21:56:10.351173 meta_ai_api-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-19 21:56:05.000000 meta_ai_api-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:56:10.347174 meta_ai_api-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:56:10.347174 meta_ai_api-1.1.2/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 21:56:05.000000 meta_ai_api-1.1.2/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10512 2024-04-19 21:56:05.000000 meta_ai_api-1.1.2/src/meta_ai_api/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-19 21:56:05.000000 meta_ai_api-1.1.2/src/meta_ai_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:56:10.351173 meta_ai_api-1.1.2/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-04-19 21:56:10.000000 meta_ai_api-1.1.2/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 21:56:10.000000 meta_ai_api-1.1.2/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:56:10.000000 meta_ai_api-1.1.2/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 21:56:10.000000 meta_ai_api-1.1.2/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 21:56:10.000000 meta_ai_api-1.1.2/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:23:26.372031 meta_ai_api-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-04-21 21:23:26.372031 meta_ai_api-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-21 21:23:22.000000 meta_ai_api-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-21 21:23:22.000000 meta_ai_api-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-21 21:23:26.372031 meta_ai_api-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-21 21:23:22.000000 meta_ai_api-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:23:26.368031 meta_ai_api-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:23:26.372031 meta_ai_api-1.1.3/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-21 21:23:22.000000 meta_ai_api-1.1.3/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 21:23:22.000000 meta_ai_api-1.1.3/src/meta_ai_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-04-21 21:23:22.000000 meta_ai_api-1.1.3/src/meta_ai_api/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-04-21 21:23:22.000000 meta_ai_api-1.1.3/src/meta_ai_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:23:26.372031 meta_ai_api-1.1.3/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-04-21 21:23:26.000000 meta_ai_api-1.1.3/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-21 21:23:26.000000 meta_ai_api-1.1.3/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 21:23:26.000000 meta_ai_api-1.1.3/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-21 21:23:26.000000 meta_ai_api-1.1.3/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 21:23:26.000000 meta_ai_api-1.1.3/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.1.2/PKG-INFO` & `meta_ai_api-1.1.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,20 @@
-Metadata-Version: 2.1
-Name: meta_ai_api
-Version: 1.1.2
-Summary: Meta AI API Wrapper to interact with the Meta AI API
-Home-page: https://github.com/tomchen/example_pypi_package
-Author: Roméo Phillips
-Author-email: phillipsromeo@gmail.com
-Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
-Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
-Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
-Keywords: llm,ai,meta_ai_api
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: requests-html
-Requires-Dist: lxml_html_clean
-Provides-Extra: dev
-Requires-Dist: check-manifest; extra == "dev"
-
 # MetaAI API Wrapper
 
 MetaAI is a Python library designed to interact with Meta's AI APIs that run in the backend of https://www.meta.ai/. It encapsulates the complexities of authentication and communication with the APIs, providing a straightforward interface for sending queries and receiving responses.
 
 With this you can easily prompt the AI with a message and get a response, directly from your Python code. **NO API KEY REQUIRED**
 
 **Meta AI is connected to the internet, so you will be able to get the latest real-time responses from the AI.** (powered by Bing)
 
 Meta AI is running Llama 3 LLM.
 
 ## Features
 - **Prompt AI**: Send a message to the AI and get a response from Llama 3.
+- **Image Generation**: Generate images using the AI. (Only for FB authenticated users)
 - **Get Up To Date Information**: Get the latest information from the AI thanks to its connection to the internet.
 - **Get Sources**: Get the sources of the information provided by the AI.
 - **Streaming**: Stream the AI's response in real-time or get the final response.
 
 ## Usage
 **Download**:
 
@@ -150,7 +121,53 @@
 {'message': "The Golden State Warriors' last game was against the Sacramento\n", 'sources': []}
 {'message': "The Golden State Warriors' last game was against the Sacramento Kings\n", 'sources': []}
 {'message': "The Golden State Warriors' last game was against the Sacramento Kings on\n", 'sources': []}
 {'message': "The Golden State Warriors' last game was against the Sacramento Kings on April\n", 'sources': []}
 ...
 {'message': "The Golden State Warriors' last game was against the Sacramento Kings on April 16, 2024, at the Golden 1 Center in Sacramento, California. The Kings won the game with a score of 118-94, with the Warriors scoring 22 points in the first quarter, 28 in the second, 26 in the third and 18 in the fourth quarter ¹.\n", 'sources': [{'link': 'https://sportradar.com/', 'title': 'Game Info of NBA from sportradar.com'}]}
 ```
+
+**Generate Image**:
+
+By default image generation is only available for FB authenticated users. If you go on https://www.meta.ai/ , and ask the AI to generate an image, you will be prompted to authenticate with Facebook.
+So if you want to generate images using this library, you need to authenticate using your FB credentials.
+
+**Note**: There seems to be higher rate limits for authenticated users. So only authenticate to generate images.
+
+```python
+from meta_ai_api import MetaAI
+ai = MetaAI(fb_email="your_fb_email", fb_password="your_fb_password")
+resp = ai.prompt(message="Generate an image of a tech CEO")
+print(resp)
+```
+
+```json
+{
+   "message":"\n",
+   "sources":[
+      
+   ],
+   "media":[
+      {
+         "url":"https://scontent-lax3-1.xx.fbcdn.net/o1/v/t0/f1/m247/4282108942387920518_1946149595_21-04-2024-14-17-48.jpeg?_nc_ht=scontent-lax3-1.xx.fbcdn.net&_nc_cat=103&ccb=9-4&oh=00_AfCnbCX7nl_J5kF6mahnams4d99Rs5WZA780HGS_scfc6A&oe=662771EE&_nc_sid=5b3566",
+         "type":"IMAGE",
+         "prompt":"a tech CEO"
+      },
+      {
+         "url":"https://scontent-lax3-1.xx.fbcdn.net/o1/v/t0/f1/m247/3356467762794691754_1025991308_21-04-2024-14-17-48.jpeg?_nc_ht=scontent-lax3-1.xx.fbcdn.net&_nc_cat=108&ccb=9-4&oh=00_AfBLmSbTSqshNAL82KIFk8hGXyL8iK_CZLGcMmmddPrxuA&oe=66276EDD&_nc_sid=5b3566",
+         "type":"IMAGE",
+         "prompt":"a tech CEO"
+      },
+      {
+         "url":"https://scontent-lax3-1.xx.fbcdn.net/o1/v/t0/f1/m247/127487551948523111_2181921077_21-04-2024-14-17-48.jpeg?_nc_ht=scontent-lax3-1.xx.fbcdn.net&_nc_cat=104&ccb=9-4&oh=00_AfAejXKeKPA4vyKXoc6UR0rEirvZwi41P3KiCSQmHRHsEw&oe=66276E45&_nc_sid=5b3566",
+         "type":"IMAGE",
+         "prompt":"a tech CEO"
+      },
+      {
+         "url":"https://scontent-lax3-1.xx.fbcdn.net/o1/v/t0/f1/m247/3497663176351797954_3954783377_21-04-2024-14-17-47.jpeg?_nc_ht=scontent-lax3-1.xx.fbcdn.net&_nc_cat=110&ccb=9-4&oh=00_AfBp3bAfcuofqtI-z9D4bHw-GuGgCNPH_xhMM0PG_95S9Q&oe=66277AE9&_nc_sid=5b3566",
+         "type":"IMAGE",
+         "prompt":"a tech CEO"
+      }
+   ]
+}
+```
+![Tech CEO](https://scontent-lax3-1.xx.fbcdn.net/o1/v/t0/f1/m247/3497663176351797954_3954783377_21-04-2024-14-17-47.jpeg?_nc_ht=scontent-lax3-1.xx.fbcdn.net&_nc_cat=110&ccb=9-4&oh=00_AfBp3bAfcuofqtI-z9D4bHw-GuGgCNPH_xhMM0PG_95S9Q&oe=66277AE9&_nc_sid=5b3566)
```

### Comparing `meta_ai_api-1.1.2/setup.py` & `meta_ai_api-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.1.2/src/meta_ai_api/main.py` & `meta_ai_api-1.1.3/src/meta_ai_api/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,45 +10,47 @@
 
 from meta_ai_api.utils import (
     generate_offline_threading_id,
     extract_value,
     format_response,
 )
 
+from meta_ai_api.utils import get_fb_session
 
 MAX_RETRIES = 3
 
 
 class MetaAI:
     """
     A class to interact with the Meta AI API to obtain and use access tokens for sending
     and receiving messages from the Meta AI Chat API.
     """
 
-    def __init__(self):
+    def __init__(self, fb_email: str = None, fb_password: str = None):
         self.session = requests.Session()
         self.session.headers.update(
             {
                 "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 "
                 "(KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36",
             }
         )
         self.access_token = None
-        self.cookies = None
+        self.fb_email = fb_email
+        self.fb_password = fb_password
+        self.is_authed = fb_password is not None and fb_email is not None
+        self.cookies = self.get_cookies()
 
     def get_access_token(self) -> str:
         """
         Retrieves an access token using Meta's authentication API.
 
         Returns:
             str: A valid access token.
         """
-        self.cookies = self.get_cookies()
         url = "https://www.meta.ai/api/graphql/"
-
         payload = {
             "lsd": self.cookies["lsd"],
             "fb_api_caller_class": "RelayModern",
             "fb_api_req_friendly_name": "useAbraAcceptTOSForTempUserMutation",
             "variables": {
                 "dob": "1999-01-01",
                 "icebreaker_type": "TEXT",
@@ -85,23 +87,28 @@
 
         Returns:
             dict: A dictionary containing the response message and sources.
 
         Raises:
             Exception: If unable to obtain a valid response after several attempts.
         """
-        if not self.access_token:
+        if not self.access_token and not self.is_authed:
             self.access_token = self.get_access_token()
+            auth_payload = {"access_token": self.access_token}
+            url = "https://graph.meta.ai/graphql?locale=user"
+
+        else:
+            auth_payload = {"fb_dtsg": self.cookies["fb_dtsg"]}
+            url = "https://www.meta.ai/api/graphql/"
 
         # Need to sleep for a bit, for some reason the API doesn't like it when we send request too quickly
         # (maybe Meta needs to register Cookies on their side?)
         time.sleep(1)
-        url = "https://graph.meta.ai/graphql?locale=user"
         payload = {
-            "access_token": self.access_token,
+            **auth_payload,
             "fb_api_caller_class": "RelayModern",
             "fb_api_req_friendly_name": "useAbraSendMessageMutation",
             "variables": json.dumps(
                 {
                     "message": {"sensitive_string_value": message},
                     "externalConversationId": str(uuid.uuid4()),
                     "offlineThreadingId": generate_offline_threading_id(),
@@ -119,14 +126,18 @@
             "doc_id": "7783822248314888",
         }
         payload = urllib.parse.urlencode(payload)  # noqa
         headers = {
             "content-type": "application/x-www-form-urlencoded",
             "x-fb-friendly-name": "useAbraSendMessageMutation",
         }
+        if self.is_authed:
+            headers["cookie"] = f'abra_sess={self.cookies["abra_sess"]}'
+            # Recreate the session to avoid cookie leakage when user is authenticated
+            self.session = requests.Session()
 
         response = self.session.post(url, headers=headers, data=payload, stream=stream)
         if not stream:
             raw_response = response.text
             last_streamed_response = self.extract_last_response(raw_response)
             if not last_streamed_response:
                 return self.retry(message, stream=stream, attempts=attempts)
@@ -216,41 +227,86 @@
         """
         bot_response_message = (
             json_line.get("data", {}).get("node", {}).get("bot_response_message", {})
         )
         response = format_response(response=json_line)
         fetch_id = bot_response_message.get("fetch_id")
         sources = self.fetch_sources(fetch_id) if fetch_id else []
-        return {"message": response, "sources": sources}
+        medias = self.extract_media(bot_response_message)
+        return {"message": response, "sources": sources, "media": medias}
 
-    @staticmethod
-    def get_cookies() -> dict:
+    def extract_media(self, json_line: dict) -> List[Dict]:
+        """
+        Extract media from a parsed JSON line.
+
+        Args:
+            json_line (dict): Parsed JSON line.
+
+        Returns:
+            list: A list of dictionaries containing the extracted media.
+        """
+        medias = []
+        imagine_card = json_line.get("imagine_card", {})
+        session = imagine_card.get("session", {}) if imagine_card else {}
+        media_sets = (
+            (json_line.get("imagine_card", {}).get("session", {}).get("media_sets", []))
+            if imagine_card and session
+            else []
+        )
+        for media_set in media_sets:
+            imagine_media = media_set.get("imagine_media", [])
+            for media in imagine_media:
+                medias.append(
+                    {
+                        "url": media.get("uri"),
+                        "type": media.get("media_type"),
+                        "prompt": media.get("prompt"),
+                    }
+                )
+        return medias
+
+    def get_cookies(self) -> dict:
         """
         Extracts necessary cookies from the Meta AI main page.
 
         Returns:
             dict: A dictionary containing essential cookies.
         """
         session = HTMLSession()
-        response = session.get("https://www.meta.ai/")
-        return {
+        headers = {}
+        if self.fb_email is not None and self.fb_password is not None:
+            fb_session = get_fb_session(self.fb_email, self.fb_password)
+            headers = {"cookie": f"abra_sess={fb_session['abra_sess']}"}
+        response = session.get(
+            "https://www.meta.ai/",
+            headers=headers,
+        )
+        cookies = {
             "_js_datr": extract_value(
                 response.text, start_str='_js_datr":{"value":"', end_str='",'
             ),
-            "abra_csrf": extract_value(
-                response.text, start_str='abra_csrf":{"value":"', end_str='",'
-            ),
             "datr": extract_value(
                 response.text, start_str='datr":{"value":"', end_str='",'
             ),
             "lsd": extract_value(
                 response.text, start_str='"LSD",[],{"token":"', end_str='"}'
             ),
+            "fb_dtsg": extract_value(
+                response.text, start_str='DTSGInitData",[],{"token":"', end_str='"'
+            ),
         }
 
+        if len(headers) > 0:
+            cookies["abra_sess"] = fb_session["abra_sess"]
+        else:
+            cookies["abra_csrf"] = extract_value(
+                response.text, start_str='abra_csrf":{"value":"', end_str='",'
+            )
+        return cookies
+
     def fetch_sources(self, fetch_id: str) -> List[Dict]:
         """
         Fetches sources from the Meta AI API based on the given query.
 
         Args:
             fetch_id (str): The fetch ID to use for the query.
 
@@ -270,28 +326,30 @@
 
         payload = urllib.parse.urlencode(payload)  # noqa
 
         headers = {
             "authority": "graph.meta.ai",
             "accept-language": "en-US,en;q=0.9,fr-FR;q=0.8,fr;q=0.7",
             "content-type": "application/x-www-form-urlencoded",
-            "cookie": f'dpr=2; abra_csrf={self.cookies["abra_csrf"]}; datr={self.cookies["datr"]}; ps_n=1; ps_l=1',
+            "cookie": f'dpr=2; abra_csrf={self.cookies.get("abra_csrf")}; datr={self.cookies.get("datr")}; ps_n=1; ps_l=1',
             "x-fb-friendly-name": "AbraSearchPluginDialogQuery",
         }
 
         response = self.session.post(url, headers=headers, data=payload)
         response_json = response.json()
-        search_results = response_json["data"]["message"]["searchResults"]
+        message = response_json.get("data", {}).get("message", {})
+        search_results = (
+            (response_json.get("data", {}).get("message", {}).get("searchResults"))
+            if message
+            else None
+        )
         if search_results is None:
             return []
 
         references = search_results["references"]
         return references
 
 
 if __name__ == "__main__":
     meta = MetaAI()
     resp = meta.prompt("What was the Warriors score last game?", stream=False)
-    # for r in resp:
-    #     print(r)
-
     print(resp)
```

