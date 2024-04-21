# Comparing `tmp/miniagents-0.0.5.tar.gz` & `tmp/miniagents-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniagents-0.0.5.tar", max compression
+gzip compressed data, was "miniagents-0.0.6.tar", max compression
```

## Comparing `miniagents-0.0.5.tar` & `miniagents-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.5/LICENSE
--rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.5/README.md
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.5/miniagents/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.5/miniagents/ext/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.5/miniagents/ext/llms/__init__.py
--rw-r--r--   0        0        0     4364 2024-04-18 21:45:37.115573 miniagents-0.0.5/miniagents/ext/llms/anthropic.py
--rw-r--r--   0        0        0    19743 2024-04-18 21:45:37.116519 miniagents-0.0.5/miniagents/miniagents.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.726367 miniagents-0.0.5/miniagents/promisegraph/__init__.py
--rw-r--r--   0        0        0      563 2024-04-02 17:38:48.000619 miniagents-0.0.5/miniagents/promisegraph/errors.py
--rw-r--r--   0        0        0     3603 2024-04-18 21:45:37.116977 miniagents-0.0.5/miniagents/promisegraph/node.py
--rw-r--r--   0        0        0    18727 2024-04-18 21:45:37.117862 miniagents-0.0.5/miniagents/promisegraph/promise.py
--rw-r--r--   0        0        0      453 2024-04-18 21:45:37.118627 miniagents-0.0.5/miniagents/promisegraph/sentinels.py
--rw-r--r--   0        0        0     1888 2024-04-16 00:22:57.814833 miniagents-0.0.5/miniagents/promisegraph/sequence.py
--rw-r--r--   0        0        0     2219 2024-04-16 00:22:57.815527 miniagents-0.0.5/miniagents/promisegraph/typing.py
--rw-r--r--   0        0        0      694 2024-04-10 07:26:59.741695 miniagents-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.6/LICENSE
+-rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.6/miniagents/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.6/miniagents/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.6/miniagents/ext/llms/__init__.py
+-rw-r--r--   0        0        0     4364 2024-04-18 21:45:37.115573 miniagents-0.0.6/miniagents/ext/llms/anthropic.py
+-rw-r--r--   0        0        0    20146 2024-04-21 22:07:14.263095 miniagents-0.0.6/miniagents/miniagents.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.726367 miniagents-0.0.6/miniagents/promisegraph/__init__.py
+-rw-r--r--   0        0        0      563 2024-04-02 17:38:48.000619 miniagents-0.0.6/miniagents/promisegraph/errors.py
+-rw-r--r--   0        0        0     3795 2024-04-21 22:07:14.264198 miniagents-0.0.6/miniagents/promisegraph/node.py
+-rw-r--r--   0        0        0    18881 2024-04-21 22:07:14.265115 miniagents-0.0.6/miniagents/promisegraph/promise.py
+-rw-r--r--   0        0        0      453 2024-04-18 21:45:37.118627 miniagents-0.0.6/miniagents/promisegraph/sentinels.py
+-rw-r--r--   0        0        0     1888 2024-04-16 00:22:57.814833 miniagents-0.0.6/miniagents/promisegraph/sequence.py
+-rw-r--r--   0        0        0     2219 2024-04-16 00:22:57.815527 miniagents-0.0.6/miniagents/promisegraph/typing.py
+-rw-r--r--   0        0        0     2356 2024-04-21 22:07:14.265779 miniagents-0.0.6/miniagents/utils.py
+-rw-r--r--   0        0        0      694 2024-04-18 21:52:04.909851 miniagents-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.6/PKG-INFO
```

### Comparing `miniagents-0.0.5/LICENSE` & `miniagents-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.5/miniagents/ext/llms/anthropic.py` & `miniagents-0.0.6/miniagents/ext/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.5/miniagents/miniagents.py` & `miniagents-0.0.6/miniagents/miniagents.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     """
 
     def __init__(
         self,
         schedule_immediately: Union[bool, Sentinel] = DEFAULT,
         message_token_producer: MessageTokenProducer = None,
         prefill_message: Optional[Message] = None,
-        metadata_so_far: Optional[Node] = None,
+        metadata_so_far: Optional[dict[str, Any]] = None,
         message_class: type[Message] = Message,
     ) -> None:
         # TODO Oleksandr: raise an error if both ready_message and message_token_producer/metadata_so_far are not None
         #  (or both are None)
         if prefill_message:
             super().__init__(
                 schedule_immediately=schedule_immediately,
@@ -136,15 +136,15 @@
         else:
             super().__init__(
                 schedule_immediately=schedule_immediately,
                 producer=self._producer,
                 packager=self._packager,
             )
             self._message_token_producer = message_token_producer
-            self._metadata_so_far: dict[str, Any] = metadata_so_far.model_dump() if metadata_so_far else {}
+            self._metadata_so_far = metadata_so_far or {}
             self._message_class = message_class
 
     def _producer(self, _) -> AsyncIterator[str]:
         return self._message_token_producer(self._metadata_so_far)
 
     async def _packager(self, _) -> Message:
         return self._message_class(
@@ -206,27 +206,36 @@
             incoming_producer=incoming_producer,
             flattener=self._flattener,
             schedule_immediately=schedule_immediately,
             sequence_promise_class=MessageSequencePromise,
         )
 
     @classmethod
-    async def acollect_messages(cls, messages: MessageType) -> tuple[Message, ...]:
+    def turn_into_sequence_promise(cls, messages: MessageType) -> MessageSequencePromise:
         """
         Convert an arbitrarily nested collection of messages of various types (strings, dicts, Message objects,
-        MessagePromise objects etc. - see `MessageType` definition for details) into a flat and uniform tuple of
-        Message objects.
+        MessagePromise objects etc. - see `MessageType` definition for details) into a flat and uniform
+        MessageSequencePromise object.
         """
         message_sequence = cls(
             producer_capture_errors=True,
             schedule_immediately=False,
         )
         with message_sequence.append_producer:
             message_sequence.append_producer.append(messages)
-        return await message_sequence.sequence_promise.acollect_messages()
+        return message_sequence.sequence_promise
+
+    @classmethod
+    async def acollect_messages(cls, messages: MessageType) -> tuple[Message, ...]:
+        """
+        Convert an arbitrarily nested collection of messages of various types (strings, dicts, Message objects,
+        MessagePromise objects etc. - see `MessageType` definition for details) into a flat and uniform tuple of
+        Message objects.
+        """
+        return await cls.turn_into_sequence_promise(messages).acollect_messages()
 
     @staticmethod
     async def _flattener(_, zero_or_more_items: MessageType) -> AsyncIterator[MessagePromise]:
         if isinstance(zero_or_more_items, MessagePromise):
             yield zero_or_more_items
         elif isinstance(zero_or_more_items, Message):
             yield MessagePromise(prefill_message=zero_or_more_items)
```

### Comparing `miniagents-0.0.5/miniagents/promisegraph/errors.py` & `miniagents-0.0.6/miniagents/promisegraph/errors.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.5/miniagents/promisegraph/node.py` & `miniagents-0.0.6/miniagents/promisegraph/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import hashlib
 import json
 from functools import cached_property
 from typing import Any
 
 from pydantic import BaseModel, ConfigDict, model_validator
 
+from miniagents.promisegraph.promise import PromiseContext
+
 
 class Node(BaseModel):
     """
     A frozen pydantic model that allows arbitrary fields, has a git-style hash key that is calculated from the
     JSON representation of its data. The data is recursively validated to be immutable. Dicts are converted to
     `Node` instances, lists and tuples are converted to tuples of immutable values, sets are prohibited.
     """
@@ -40,15 +42,18 @@
         return json.dumps(self.model_dump(), ensure_ascii=False, sort_keys=True)
 
     @cached_property
     def hash_key(self) -> str:
         """
         Get the hash key for this object. It is a hash of the JSON representation of the object.
         """
-        return hashlib.sha256(self.as_json.encode("utf-8")).hexdigest()
+        hash_key = hashlib.sha256(self.as_json.encode("utf-8")).hexdigest()
+        if not PromiseContext.get_current().longer_node_hash_keys:
+            hash_key = hash_key[:32]
+        return hash_key
 
     def serialize_node(self, **model_dump_kwargs) -> dict[str, Any]:
         """
         TODO Oleksandr
         """
         return self.model_dump(**model_dump_kwargs)
```

### Comparing `miniagents-0.0.5/miniagents/promisegraph/promise.py` & `miniagents-0.0.6/miniagents/promisegraph/promise.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,24 +31,26 @@
 
     _current: ContextVar[Optional["PromiseContext"]] = ContextVar("PromiseContext._current", default=None)
 
     def __init__(
         self,
         schedule_immediately_by_default: bool = True,
         producer_capture_errors_by_default: bool = False,
+        longer_node_hash_keys: bool = False,  # TODO Oleksandr: does it belong in this class ?
         on_promise_collected: Union[PromiseCollectedEventHandler, Iterable[PromiseCollectedEventHandler]] = (),
     ) -> None:
         self.parent = self._current.get()
         self.on_promise_collected_handlers: list[PromiseCollectedEventHandler] = (
             [on_promise_collected] if callable(on_promise_collected) else list(on_promise_collected)
         )
         self.child_tasks: set[Task] = set()
 
         self.schedule_immediately_by_default = schedule_immediately_by_default
         self.producer_capture_errors_by_default = producer_capture_errors_by_default
+        self.longer_node_hash_keys = longer_node_hash_keys
 
         self._previous_ctx_token: Optional[contextvars.Token] = None
 
     @classmethod
     def get_current(cls) -> "PromiseContext":
         """
         Get the current context. If no context is currently active, raise an error.
```

### Comparing `miniagents-0.0.5/miniagents/promisegraph/sequence.py` & `miniagents-0.0.6/miniagents/promisegraph/sequence.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.5/miniagents/promisegraph/typing.py` & `miniagents-0.0.6/miniagents/promisegraph/typing.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.5/pyproject.toml` & `miniagents-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 119
 
 [tool.coverage.run]
 branch = true
 
 [tool.poetry]
 name = "miniagents"
-version = "0.0.5"
+version = "0.0.6"
 description = """\
 TODO Oleksandr\
 """
 authors = ["Oleksandr Tereshchenko <toporok@gmail.com>"]
 homepage = "https://github.com/teremterem/MiniAgents"
 readme = "README.md"
 license = "MIT"
```

### Comparing `miniagents-0.0.5/PKG-INFO` & `miniagents-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniagents
-Version: 0.0.5
+Version: 0.0.6
 Summary: TODO Oleksandr
 Home-page: https://github.com/teremterem/MiniAgents
 License: MIT
 Author: Oleksandr Tereshchenko
 Author-email: toporok@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

