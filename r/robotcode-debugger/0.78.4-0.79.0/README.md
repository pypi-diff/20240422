# Comparing `tmp/robotcode_debugger-0.78.4.tar.gz` & `tmp/robotcode_debugger-0.79.0.tar.gz`

## Comparing `robotcode_debugger-0.78.4.tar` & `robotcode_debugger-0.79.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0    25783 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    69967 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/hooks.py
--rw-r--r--   0        0        0    12616 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12765 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/run.py
--rw-r--r--   0        0        0    15859 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/launcher/client.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/launcher/run.py
--rw-r--r--   0        0        0    13913 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/LICENSE.txt
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/README.md
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/pyproject.toml
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 robotcode_debugger-0.78.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0    25783 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    69967 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/hooks.py
+-rw-r--r--   0        0        0    12904 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/run.py
+-rw-r--r--   0        0        0    15859 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/client.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/run.py
+-rw-r--r--   0        0        0    13913 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/LICENSE.txt
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/README.md
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/pyproject.toml
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/PKG-INFO
```

### Comparing `robotcode_debugger-0.78.4/src/robotcode/debugger/cli.py` & `robotcode_debugger-0.79.0/src/robotcode/debugger/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.78.4/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.79.0/src/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.78.4/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.79.0/src/robotcode/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.78.4/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.79.0/src/robotcode/debugger/listeners.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,41 +2,51 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, Union, cast
 
 from robot import result, running
 from robot.model import Message
 
+from robotcode.core.utils.path import normalized_path
+
 from .dap_types import Event, Model
 from .debugger import Debugger
 
 
 @dataclass
 class RobotExecutionEventBody(Model):
     type: str
     id: str
     attributes: Optional[Dict[str, Any]] = None
     failed_keywords: Optional[List[Dict[str, Any]]] = None
 
 
+def source_from_attributes(attributes: Dict[str, Any]) -> str:
+    s = attributes.get("source", "")
+    if s:
+        return str(normalized_path(Path(s)))
+
+    return s or ""
+
+
 class ListenerV2:
     ROBOT_LISTENER_API_VERSION = "2"
 
     def __init__(self) -> None:
         self.failed_keywords: Optional[List[Dict[str, Any]]] = None
         self.last_fail_message: Optional[str] = None
 
     def start_suite(self, name: str, attributes: Dict[str, Any]) -> None:
         Debugger.instance().send_event(
             self,
             Event(
                 event="robotStarted",
                 body=RobotExecutionEventBody(
                     type="suite",
-                    id=f"{attributes.get('source', '')};{attributes.get('longname', '')}",
+                    id=f"{source_from_attributes(attributes)};{attributes.get('longname', '')}",
                     attributes=dict(attributes),
                 ),
             ),
         )
 
         Debugger.instance().start_output_group(name, attributes, "SUITE")
 
@@ -50,15 +60,15 @@
         Debugger.instance().send_event(
             self,
             Event(
                 event="robotEnded",
                 body=RobotExecutionEventBody(
                     type="suite",
                     attributes=dict(attributes),
-                    id=f"{attributes.get('source', '')};{attributes.get('longname', '')}",
+                    id=f"{source_from_attributes(attributes)};{attributes.get('longname', '')}",
                     failed_keywords=self.failed_keywords,
                 ),
             ),
         )
 
         self.failed_keywords = None
 
@@ -67,15 +77,15 @@
 
         Debugger.instance().send_event(
             self,
             Event(
                 event="robotStarted",
                 body=RobotExecutionEventBody(
                     type="test",
-                    id=f"{attributes.get('source', '')};{attributes.get('longname', '')};"
+                    id=f"{source_from_attributes(attributes)};{attributes.get('longname', '')};"
                     f"{attributes.get('lineno', 0)}",
                     attributes=dict(attributes),
                 ),
             ),
         )
 
         Debugger.instance().start_output_group(name, attributes, "TEST")
@@ -89,15 +99,15 @@
 
         Debugger.instance().send_event(
             self,
             Event(
                 event="robotEnded",
                 body=RobotExecutionEventBody(
                     type="test",
-                    id=f"{attributes.get('source', '')};{attributes.get('longname', '')};"
+                    id=f"{source_from_attributes(attributes)};{attributes.get('longname', '')};"
                     f"{attributes.get('lineno', 0)}",
                     attributes=dict(attributes),
                     failed_keywords=self.failed_keywords,
                 ),
             ),
         )
 
@@ -138,17 +148,17 @@
             source = current_frame.source if current_frame else None
             line = current_frame.line if current_frame else None
             column = current_frame.column if current_frame else None
 
             item_id = next(
                 (
                     (
-                        f"{Path(item.source).resolve() if item.source is not None else ''};{item.longname}"
+                        f"{normalized_path(Path(item.source)) if item.source is not None else ''};{item.longname}"
                         if item.type == "SUITE"
-                        else f"{Path(item.source).resolve() if item.source is not None else ''};"
+                        else f"{normalized_path(Path(item.source)) if item.source is not None else ''};"
                         f"{item.longname};{item.line}"
                     )
                     for item in Debugger.instance().full_stack_frames
                     if item.type in ["SUITE", "TEST"]
                 ),
                 None,
             )
@@ -185,17 +195,17 @@
             source = current_frame.source if current_frame else None
             line = current_frame.line if current_frame else None
             column = current_frame.column if current_frame else None
 
             item_id = next(
                 (
                     (
-                        f"{Path(item.source).resolve() if item.source is not None else ''};{item.longname}"
+                        f"{normalized_path(Path(item.source)) if item.source is not None else ''};{item.longname}"
                         if item.type == "SUITE"
-                        else f"{Path(item.source).resolve() if item.source is not None else ''};"
+                        else f"{normalized_path(Path(item.source)) if item.source is not None else ''};"
                         f"{item.longname};{item.line}"
                     )
                     for item in Debugger.instance().full_stack_frames
                     if item.type in ["SUITE", "TEST"]
                 ),
                 None,
             )
@@ -262,23 +272,23 @@
     def start_suite(self, data: running.TestSuite, result: result.TestSuite) -> None:
         """Called when a suite starts."""
 
         def enqueue(
             item: Union[running.TestSuite, running.TestCase],
         ) -> Iterator[str]:
             if isinstance(item, running.TestSuite):
-                yield f"{Path(item.source).resolve() if item.source is not None else ''};{item.longname}"
+                yield f"{normalized_path(item.source) if item.source is not None else ''};{item.longname}"
 
                 for s in item.suites:
                     yield from enqueue(s)
                 for s in item.tests:
                     yield from enqueue(s)
                 return
 
-            yield f"{Path(item.source).resolve() if item.source is not None else ''};{item.longname};{item.lineno}"
+            yield (f"{normalized_path(item.source) if item.source is not None else ''};{item.longname};{item.lineno}")
 
         if self._event_sended:
             return
 
         items = list(reversed(list(enqueue(cast(running.model.TestSuite, data)))))
 
         Debugger.instance().send_event(self, Event(event="robotEnqueued", body={"items": items}))
```

### Comparing `robotcode_debugger-0.78.4/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.79.0/src/robotcode/debugger/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,17 +219,17 @@
                 kw_args["arguments"] = converted_params
         return args, kw_args
 
     async def handle_unknown_command(self, message: Request) -> Any:
         raise DebugAdapterRPCErrorException(
             f"Unknown Command '{message.command}'",
             error_message=Message(
-                format='Unknown command "{command}"',
-                variables={"command": str(message.command)},
-                show_user=True,
+                format='Unknown command "{command}": {request}',
+                variables={"command": str(message.command), "request": str(message)},
+                show_user=False,
             ),
         )
 
     @_logger.call
     def handle_request(self, message: Request) -> None:
         e = self.registry.get_entry(message.command)
```

### Comparing `robotcode_debugger-0.78.4/src/robotcode/debugger/run.py` & `robotcode_debugger-0.79.0/src/robotcode/debugger/run.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -205,17 +205,17 @@
 
         if debugpy and debugpy_wait_for_client:
             app.verbose("Wait for debugpy incomming connections.")
             wait_for_debugpy_connected()
 
         args = [
             "--listener",
-            "robotcode.debugger.listeners.ListenerV2",
-            "--listener",
             "robotcode.debugger.listeners.ListenerV3",
+            "--listener",
+            "robotcode.debugger.listeners.ListenerV2",
             *args,
         ]
 
         Debugger.instance().stop_on_entry = stop_on_entry
         Debugger.instance().output_messages = output_messages
         Debugger.instance().output_log = output_log
         Debugger.instance().group_output = group_output
```

### Comparing `robotcode_debugger-0.78.4/src/robotcode/debugger/server.py` & `robotcode_debugger-0.79.0/src/robotcode/debugger/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.78.4/src/robotcode/debugger/launcher/cli.py` & `robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.78.4/src/robotcode/debugger/launcher/client.py` & `robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/client.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.78.4/src/robotcode/debugger/launcher/run.py` & `robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.78.4/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.78.4/.gitignore` & `robotcode_debugger-0.79.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.78.4/LICENSE.txt` & `robotcode_debugger-0.79.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.78.4/README.md` & `robotcode_debugger-0.79.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.78.4/pyproject.toml` & `robotcode_debugger-0.79.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.78.4",
-  "robotcode-runner==0.78.4",
+  "robotcode-jsonrpc2==0.79.0",
+  "robotcode-runner==0.79.0",
 ]
 
 [project.optional-dependencies]
 debugpy = ["debugpy"]
 
 [project.entry-points.robotcode]
 debugger = "robotcode.debugger.hooks"
```

### Comparing `robotcode_debugger-0.78.4/PKG-INFO` & `robotcode_debugger-0.79.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-debugger
-Version: 0.78.4
+Version: 0.79.0
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.78.4
-Requires-Dist: robotcode-runner==0.78.4
+Requires-Dist: robotcode-jsonrpc2==0.79.0
+Requires-Dist: robotcode-runner==0.79.0
 Requires-Dist: robotframework>=4.1.0
 Provides-Extra: debugpy
 Requires-Dist: debugpy; extra == 'debugpy'
 Description-Content-Type: text/markdown
 
 # robotcode-debugger
```

