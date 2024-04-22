# Comparing `tmp/oterm-0.2.6.tar.gz` & `tmp/oterm-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oterm-0.2.6.tar", max compression
+gzip compressed data, was "oterm-0.2.7.tar", max compression
```

## Comparing `oterm-0.2.6.tar` & `oterm-0.2.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1064 2024-04-20 06:48:32.686512 oterm-0.2.6/LICENSE
--rw-r--r--   0        0        0     3798 2024-04-20 06:48:32.686512 oterm-0.2.6/README.md
--rw-r--r--   0        0        0        0 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/__init__.py
--rw-r--r--   0        0        0     7129 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/chat_edit.py
--rw-r--r--   0        0        0     1593 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/chat_export.py
--rw-r--r--   0        0        0      734 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/chat_rename.py
--rw-r--r--   0        0        0     2313 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/image_browser.py
--rw-r--r--   0        0        0     3244 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/oterm.py
--rw-r--r--   0        0        0     3239 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/oterm.tcss
--rw-r--r--   0        0        0     1058 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/prompt_history.py
--rw-r--r--   0        0        0     1947 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/splash.py
--rw-r--r--   0        0        0       46 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/__init__.py
--rw-r--r--   0        0        0     9680 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/chat.py
--rw-r--r--   0        0        0     1823 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/image.py
--rw-r--r--   0        0        0      627 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/monkey.py
--rw-r--r--   0        0        0     5569 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/prompt.py
--rw-r--r--   0        0        0      879 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/app/widgets/text_area.py
--rw-r--r--   0        0        0        0 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/cli/__init__.py
--rw-r--r--   0        0        0      724 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/cli/oterm.py
--rw-r--r--   0        0        0     3131 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/config.py
--rw-r--r--   0        0        0     1763 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/ollama.py
--rw-r--r--   0        0        0        0 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/__init__.py
--rw-r--r--   0        0        0      892 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/chat.py
--rw-r--r--   0        0        0      572 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/setup.py
--rw-r--r--   0        0        0     5769 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/store.py
--rw-r--r--   0        0        0      359 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/upgrades/__init__.py
--rw-r--r--   0        0        0      574 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/upgrades/v0_1_11.py
--rw-r--r--   0        0        0      514 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/upgrades/v0_1_6.py
--rw-r--r--   0        0        0      522 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/upgrades/v0_2_0.py
--rw-r--r--   0        0        0      533 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/store/upgrades/v0_2_4.py
--rw-r--r--   0        0        0     1408 2024-04-20 06:48:32.686512 oterm-0.2.6/oterm/utils.py
--rw-r--r--   0        0        0     2040 2024-04-20 06:48:32.690512 oterm-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 oterm-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 06:47:10.868047 oterm-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3798 2024-04-22 06:47:10.868047 oterm-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/__init__.py
+-rw-r--r--   0        0        0     7156 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/chat_edit.py
+-rw-r--r--   0        0        0     1593 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/chat_export.py
+-rw-r--r--   0        0        0      734 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/chat_rename.py
+-rw-r--r--   0        0        0     2313 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/image_browser.py
+-rw-r--r--   0        0        0     3244 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/oterm.py
+-rw-r--r--   0        0        0     3239 2024-04-22 06:47:10.868047 oterm-0.2.7/oterm/app/oterm.tcss
+-rw-r--r--   0        0        0     1058 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/prompt_history.py
+-rw-r--r--   0        0        0     1947 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/splash.py
+-rw-r--r--   0        0        0       46 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/__init__.py
+-rw-r--r--   0        0        0     9680 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/chat.py
+-rw-r--r--   0        0        0     1823 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/image.py
+-rw-r--r--   0        0        0      627 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/monkey.py
+-rw-r--r--   0        0        0     5569 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/prompt.py
+-rw-r--r--   0        0        0      879 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/app/widgets/text_area.py
+-rw-r--r--   0        0        0        0 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/cli/__init__.py
+-rw-r--r--   0        0        0      724 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/cli/oterm.py
+-rw-r--r--   0        0        0     3131 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/config.py
+-rw-r--r--   0        0        0     2181 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/ollama.py
+-rw-r--r--   0        0        0        0 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/__init__.py
+-rw-r--r--   0        0        0      892 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/chat.py
+-rw-r--r--   0        0        0      572 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/setup.py
+-rw-r--r--   0        0        0     5769 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/store.py
+-rw-r--r--   0        0        0      359 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/upgrades/__init__.py
+-rw-r--r--   0        0        0      574 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/upgrades/v0_1_11.py
+-rw-r--r--   0        0        0      514 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/upgrades/v0_1_6.py
+-rw-r--r--   0        0        0      522 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/upgrades/v0_2_0.py
+-rw-r--r--   0        0        0      533 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/store/upgrades/v0_2_4.py
+-rw-r--r--   0        0        0     1408 2024-04-22 06:47:10.872047 oterm-0.2.7/oterm/utils.py
+-rw-r--r--   0        0        0     2040 2024-04-22 06:47:10.872047 oterm-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 oterm-0.2.7/PKG-INFO
```

### Comparing `oterm-0.2.6/LICENSE` & `oterm-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/README.md` & `oterm-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/chat_edit.py` & `oterm-0.2.7/oterm/app/chat_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 from ast import literal_eval
 from typing import Any
 
-import ollama
 from rich.text import Text
 from textual.app import ComposeResult
 from textual.containers import Container, Horizontal, Vertical
 from textual.css.query import NoMatches
 from textual.reactive import reactive
 from textual.screen import ModalScreen
 from textual.widgets import Button, Checkbox, Label, OptionList, Pretty
 
 from oterm.app.widgets.text_area import TextArea
+from oterm.ollama import OllamaLLM
 
 
 class ChatEdit(ModalScreen[str]):
     models = []
     models_info: dict[str, dict] = {}
 
     model_name: reactive[str] = reactive("")
@@ -70,18 +70,18 @@
         select = self.query_one("#model-select", OptionList)
         for index, option in enumerate(select._options):
             if str(option.prompt) == model:
                 select.highlighted = index
                 break
 
     async def on_mount(self) -> None:
-        self.models = ollama.list()["models"]
+        self.models = OllamaLLM.list()["models"]
         models = [model["name"] for model in self.models]
         for model in models:
-            info = dict(ollama.show(model))
+            info = dict(OllamaLLM.show(model))
             for key in ["modelfile", "license"]:
                 if key in info.keys():
                     del info[key]
             self.models_info[model] = info
         option_list = self.query_one("#model-select", OptionList)
         option_list.clear_options()
         for model in models:
```

### Comparing `oterm-0.2.6/oterm/app/chat_export.py` & `oterm-0.2.7/oterm/app/chat_export.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/chat_rename.py` & `oterm-0.2.7/oterm/app/chat_rename.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/image_browser.py` & `oterm-0.2.7/oterm/app/image_browser.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/oterm.py` & `oterm-0.2.7/oterm/app/oterm.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/oterm.tcss` & `oterm-0.2.7/oterm/app/oterm.tcss`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/prompt_history.py` & `oterm-0.2.7/oterm/app/prompt_history.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/splash.py` & `oterm-0.2.7/oterm/app/splash.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/widgets/chat.py` & `oterm-0.2.7/oterm/app/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/widgets/image.py` & `oterm-0.2.7/oterm/app/widgets/image.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/widgets/monkey.py` & `oterm-0.2.7/oterm/app/widgets/monkey.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/widgets/prompt.py` & `oterm-0.2.7/oterm/app/widgets/prompt.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/app/widgets/text_area.py` & `oterm-0.2.7/oterm/app/widgets/text_area.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/cli/oterm.py` & `oterm-0.2.7/oterm/cli/oterm.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/config.py` & `oterm-0.2.7/oterm/config.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/ollama.py` & `oterm-0.2.7/oterm/ollama.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Any, AsyncGenerator, AsyncIterator, Literal
+from typing import Any, AsyncGenerator, AsyncIterator, Literal, Mapping
 
-from ollama import AsyncClient
+from ollama import AsyncClient, Client
 
 from oterm.config import envConfig
 
 
 class OllamaLLM:
     def __init__(
         self,
@@ -50,7 +50,21 @@
         )
         text = ""
         async for response in stream:
             text = text + response.get("response", "")
             if "context" in response:
                 self.context = response.get("context")
             yield text
+
+    @staticmethod
+    def list() -> Mapping[str, Any]:
+        client = Client(
+            host=envConfig.OLLAMA_URL, verify=envConfig.OTERM_VERIFY_SSL
+        )
+        return client.list()
+
+    @staticmethod
+    def show(model: str) -> Mapping[str, Any]:
+        client = Client(
+            host=envConfig.OLLAMA_URL, verify=envConfig.OTERM_VERIFY_SSL
+        )
+        return client.show(model)
```

### Comparing `oterm-0.2.6/oterm/store/chat.py` & `oterm-0.2.7/oterm/store/chat.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/store/setup.py` & `oterm-0.2.7/oterm/store/setup.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/store/store.py` & `oterm-0.2.7/oterm/store/store.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/store/upgrades/v0_1_11.py` & `oterm-0.2.7/oterm/store/upgrades/v0_1_11.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/store/upgrades/v0_1_6.py` & `oterm-0.2.7/oterm/store/upgrades/v0_1_6.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/store/upgrades/v0_2_0.py` & `oterm-0.2.7/oterm/store/upgrades/v0_2_0.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/store/upgrades/v0_2_4.py` & `oterm-0.2.7/oterm/store/upgrades/v0_2_4.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/oterm/utils.py` & `oterm-0.2.7/oterm/utils.py`

 * *Files identical despite different names*

### Comparing `oterm-0.2.6/pyproject.toml` & `oterm-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oterm"
-version = "0.2.6"
+version = "0.2.7"
 description = "A text-based terminal client for Ollama."
 authors = ["Yiorgis Gozadinos <ggozadinos@gmail.com>"]
 homepage = "https://github.com/ggozad/oterm"
 repository = "https://github.com/ggozad/oterm"
 license = "MIT"
 readme = "README.md"
 classifiers = [
```

### Comparing `oterm-0.2.6/PKG-INFO` & `oterm-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oterm
-Version: 0.2.6
+Version: 0.2.7
 Summary: A text-based terminal client for Ollama.
 Home-page: https://github.com/ggozad/oterm
 License: MIT
 Author: Yiorgis Gozadinos
 Author-email: ggozadinos@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

