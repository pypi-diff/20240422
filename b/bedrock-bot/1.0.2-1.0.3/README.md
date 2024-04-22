# Comparing `tmp/bedrock_bot-1.0.2.tar.gz` & `tmp/bedrock_bot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrock_bot-1.0.2.tar", max compression
+gzip compressed data, was "bedrock_bot-1.0.3.tar", max compression
```

## Comparing `bedrock_bot-1.0.2.tar` & `bedrock_bot-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/LICENSE
--rw-r--r--   0        0        0     2598 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/README.md
--rw-r--r--   0        0        0       91 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/bedrock_bot/__init__.py
--rw-r--r--   0        0        0     2290 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/bedrock_bot/cli.py
--rw-r--r--   0        0        0     3209 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/bedrock_bot/model.py
--rw-r--r--   0        0        0      152 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/bedrock_bot/util.py
--rw-r--r--   0        0        0      448 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2598 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/README.md
+-rw-r--r--   0        0        0       91 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/bedrock_bot/__init__.py
+-rw-r--r--   0        0        0     2290 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/bedrock_bot/cli.py
+-rw-r--r--   0        0        0     3173 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/bedrock_bot/model.py
+-rw-r--r--   0        0        0      152 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/bedrock_bot/util.py
+-rw-r--r--   0        0        0      448 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.0.3/PKG-INFO
```

### Comparing `bedrock_bot-1.0.2/LICENSE` & `bedrock_bot-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.2/README.md` & `bedrock_bot-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.2/bedrock_bot/cli.py` & `bedrock_bot-1.0.3/bedrock_bot/cli.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.2/bedrock_bot/model.py` & `bedrock_bot-1.0.3/bedrock_bot/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,56 +4,57 @@
 import boto3
 from botocore.config import Config
 from rich.console import Console
 
 console = Console()
 
 
+class ConversationRole(Enum):
+    USER = "user"
+    ASSISTANT = "assistant"
+
+    def __str__(self):
+        return self.value
+
+
 class _BedrockModel:
     """
     Base class for all models. Usage:
     Add a message to the conversation and invoke the model with `model.invoke(message)`.
 
     Creating new implementations of this base model:
     - Define extra params to inject to the invoke call on self._model_params
     - Provide a model_id to `super().__init__()`
     - If your model needs a different body than the default, overwrite `self._create_invoke_body()`
     """
 
     _model_params = {}
     name = "Base Model"
 
-    class _ConversationRole(Enum):
-        USER = "user"
-        ASSISTANT = "assistant"
-
-        def __str__(self):
-            return self.value
-
     def __init__(
         self,
         model_id: str,
         boto_config=None,
     ):
         self._model_id = model_id
         if not boto_config:
             boto_config = Config()
         self._bedrock = boto3.client("bedrock-runtime", config=boto_config)
         self.messages = []
 
     def reset(self):
         self.messages = []
 
-    def _append_message(self, role: _ConversationRole, message: str):
+    def append_message(self, role: ConversationRole, message: str):
         self.messages.append({"role": role.value, "content": message})
 
     def invoke(self, message: str):
-        self._append_message(self._ConversationRole.USER, message)
+        self.append_message(ConversationRole.USER, message)
         response = self._invoke()
-        self._append_message(self._ConversationRole.ASSISTANT, response)
+        self.append_message(ConversationRole.ASSISTANT, response)
         return response
 
     def _create_invoke_body(self) -> dict:
         body = {
             "messages": self.messages,
         }
```

### Comparing `bedrock_bot-1.0.2/PKG-INFO` & `bedrock_bot-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bedrock-bot
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

