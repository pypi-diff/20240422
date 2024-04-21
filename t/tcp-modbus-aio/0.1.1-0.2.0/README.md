# Comparing `tmp/tcp_modbus_aio-0.1.1.tar.gz` & `tmp/tcp_modbus_aio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcp_modbus_aio-0.1.1.tar", max compression
+gzip compressed data, was "tcp_modbus_aio-0.2.0.tar", max compression
```

## Comparing `tcp_modbus_aio-0.1.1.tar` & `tcp_modbus_aio-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/LICENSE
--rw-r--r--   0        0        0     1649 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/README.md
--rw-r--r--   0        0        0      825 2024-04-16 19:16:29.307997 tcp_modbus_aio-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-16 19:16:29.311997 tcp_modbus_aio-0.1.1/tcp_modbus_aio/__init__.py
--rw-r--r--   0        0        0    18586 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/tcp_modbus_aio/connection.py
--rw-r--r--   0        0        0      267 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/tcp_modbus_aio/exceptions.py
--rw-r--r--   0        0        0     1140 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/tcp_modbus_aio/ping.py
--rw-r--r--   0        0        0        0 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/tcp_modbus_aio/py.typed
--rw-r--r--   0        0        0     2889 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/tcp_modbus_aio/typed_functions.py
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1649 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/README.md
+-rw-r--r--   0        0        0      857 2024-04-21 22:14:56.874465 tcp_modbus_aio-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-21 22:14:56.882465 tcp_modbus_aio-0.2.0/tcp_modbus_aio/__init__.py
+-rw-r--r--   0        0        0    20152 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/tcp_modbus_aio/client.py
+-rw-r--r--   0        0        0      267 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/tcp_modbus_aio/exceptions.py
+-rw-r--r--   0        0        0     1140 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/tcp_modbus_aio/ping.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/tcp_modbus_aio/py.typed
+-rw-r--r--   0        0        0     2889 2024-04-21 22:14:55.502451 tcp_modbus_aio-0.2.0/tcp_modbus_aio/typed_functions.py
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.2.0/PKG-INFO
```

### Comparing `tcp_modbus_aio-0.1.1/LICENSE` & `tcp_modbus_aio-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.1.1/README.md` & `tcp_modbus_aio-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.1.1/pyproject.toml` & `tcp_modbus_aio-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tcp-modbus-aio"
-version = "0.1.1"
+version = "0.2.0"
 description = "asyncio client library for tcp modbus devices"
 authors = ["Josh Gruenstein <josh@tutorintelligence.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -26,8 +26,11 @@
 
 [tool.poetry.scripts]
 style = "poetry_scripts:style"
 
 [tool.semantic_release]
 version_variables = ["tcp_modbus_aio/__init__.py:__version__"]
 version_toml = ["pyproject.toml:tool.poetry.version"]
-build_command = "pip install poetry && poetry build"
+build_command = "pip install poetry && poetry build"
+
+[tool.isort]
+profile = "black"
```

### Comparing `tcp_modbus_aio-0.1.1/tcp_modbus_aio/connection.py` & `tcp_modbus_aio-0.2.0/tcp_modbus_aio/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,14 +77,17 @@
 
         # Task that pings the device every second
         self._ping_loop: asyncio.Task | None = asyncio.create_task(
             self._ping_loop_task(),
             name=f"TCPModbusClient._ping_loop_task[{self.host}:{self.port}]",
         )
 
+        # Event that is set when the first ping is received
+        self._first_ping_event: asyncio.Event = asyncio.Event()
+
         # List of CoilWatchStatus objects that are being logged
         self._log_watches = list[CoilWatchStatus]()
 
         # We cache anly active awaitable testing TCP connectivity to prevent spamming the connection
         self._active_connection_probe: asyncio.Task | None = None
 
         # We track this number because the ADAM module has a firmware bug where it will stop responding
@@ -116,17 +119,19 @@
             f"{self.__class__.__name__}({str(self._id)[:4]})[{self.host}:{self.port}]"
             f"[{last_ping_msg}, conn #{self._lifetime_tcp_connection_num}]"
         )
 
     async def _ping_loop_task(self) -> None:
         while True:
             self._last_ping = await ping_ip(self.host)
+
             if self.logger is not None:
                 self.logger.debug(f"[{self}][_ping_loop_task] ping ping ping")
 
+            self._first_ping_event.set()
             await asyncio.sleep(self.PING_LOOP_PERIOD)
 
     async def _get_tcp_connection(
         self, timeout: float | None = DEFAULT_MODBUS_TIMEOUT_SEC
     ) -> tuple[asyncio.StreamReader, asyncio.StreamWriter]:
         if self._reader is None or self._writer is None:
             self._lifetime_tcp_connection_num += 1
@@ -200,14 +205,21 @@
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         await self.close()
 
     async def close(self) -> None:
+        """
+        Permanent close of the TCP connection and ping loop.  Only call this on final destruction of the object.
+        """
+
+        if self._ping_loop is None:
+            return
+
         await self.clear_tcp_connection()
 
         if self._ping_loop is not None:
             if self.logger is not None:
                 self.logger.debug(f"[{self}][close] Cancelling ping loop")
             self._ping_loop.cancel()
             self._ping_loop = None
@@ -219,14 +231,17 @@
         Triggers a loop that reads the coil(s) at the given index at the given frequency and
         writes the current values to logs for debugging purposes.
 
         This debug loop expires after the given period, but is refreshed every time this request_function
         is called.
         """
 
+        if self._ping_loop is None:
+            raise RuntimeError("Cannot log watch on closed TCPModbusClient")
+
         for watch in self._log_watches:
             if watch.memo_key == memo_key:
                 watch.expiry = time.perf_counter() + period
                 watch.hz = hz
                 watch.msg = msg
 
                 break
@@ -274,14 +289,22 @@
                 await asyncio.sleep(1 / watch.hz)
 
         watch.task = asyncio.create_task(
             _watch_loop(), name=f"TCPModbusClient{log_prefix}"
         )
 
     async def clear_tcp_connection(self) -> None:
+        """
+        Closes the current TCP connection and clears the reader and writer objects.
+        On the next send_modbus_message call, a new connection will be created.
+        """
+
+        if self._ping_loop is None:
+            raise RuntimeError("Cannot clear TCP connection on closed TCPModbusClient")
+
         if self._writer is not None:
             if self.logger is not None:
                 self.logger.warning(
                     f"[{self}][clear_tcp_connection] closing TCP connection #{self._lifetime_tcp_connection_num}"
                 )
 
             self._writer.close()
@@ -290,41 +313,60 @@
         self._reader = None
         self._writer = None
 
     async def test_connection(
         self, timeout: float | None = DEFAULT_MODBUS_TIMEOUT_SEC
     ) -> None:
         """
+        Tests the connection to the device by sending a ReadCoil message (see TEST_CONNECTION_MESSAGE)
         Uses a cached awaitable to prevent spamming the connection on this call
         """
 
+        if self._ping_loop is None:
+            raise RuntimeError("Cannot test connection on closed TCPModbusClient")
+
         try:
             if self._active_connection_probe is None:
                 self._active_connection_probe = asyncio.create_task(
                     self.send_modbus_message(TEST_CONNECTION_MESSAGE, timeout=timeout),
                     name=f"TCPModbusClient.test_connection({self.host}:{self.port})",
                 )
 
             await self._active_connection_probe
         finally:
             self._active_connection_probe = None
 
+    async def is_pingable(self) -> bool:
+        """
+        Returns True if the device is pingable, False if not.
+        Will wait for the first ping to be received (or timeout) before returning.
+        """
+
+        if self._ping_loop is None:
+            raise RuntimeError("Cannot check pingability on closed TCPModbusClient")
+
+        if not self._first_ping_event.is_set():
+            await self._first_ping_event.wait()
+
+        return self._last_ping is not None
+
     async def send_modbus_message(
         self,
         request_function: ModbusFunctionT,
         timeout: float | None = DEFAULT_MODBUS_TIMEOUT_SEC,
         retries: int = 1,
         error_on_no_response: bool = True,
     ) -> ModbusFunctionT | None:
-        """Send ADU over socket to to server and return parsed response.
-
-        :param adu: Request ADU.
-        :param sock: Socket instance.
-        :return: Parsed response from server.
         """
+        Sends a modbus message to the device and returns the response.
+        Will create a new TCP connection if one does not exist.
+        """
+
+        if self._ping_loop is None:
+            raise RuntimeError("Cannot send modbus message on closed TCPModbusClient")
 
         request_transaction_id = self._next_transaction_id
         self._next_transaction_id = (self._next_transaction_id + 1) % MAX_TRANSACTION_ID
 
         msg_str = f"{request_function.__class__.__name__}[{request_transaction_id}]"
 
         request_mbap_header = struct.pack(
```

### Comparing `tcp_modbus_aio-0.1.1/tcp_modbus_aio/ping.py` & `tcp_modbus_aio-0.2.0/tcp_modbus_aio/ping.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.1.1/tcp_modbus_aio/typed_functions.py` & `tcp_modbus_aio-0.2.0/tcp_modbus_aio/typed_functions.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.1.1/PKG-INFO` & `tcp_modbus_aio-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcp-modbus-aio
-Version: 0.1.1
+Version: 0.2.0
 Summary: asyncio client library for tcp modbus devices
 License: MIT
 Author: Josh Gruenstein
 Author-email: josh@tutorintelligence.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

