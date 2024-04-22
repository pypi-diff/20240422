# Comparing `tmp/era_5g_interface-0.8.0.tar.gz` & `tmp/era_5g_interface-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_interface-0.8.0.tar", last modified: Fri Dec 15 13:19:57 2023, max compression
+gzip compressed data, was "era_5g_interface-0.9.0.tar", last modified: Thu Jan 18 08:14:57 2024, max compression
```

## Comparing `era_5g_interface-0.8.0.tar` & `era_5g_interface-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-15 13:19:57.721716 era_5g_interface-0.8.0/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/MANIFEST.in
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      434 2023-12-15 13:19:57.721716 era_5g_interface-0.8.0/PKG-INFO
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/backend_shim.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-15 13:19:57.721716 era_5g_interface-0.8.0/era_5g_interface/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    17288 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/channels.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4223 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/client_channels.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-15 13:19:57.721716 era_5g_interface-0.8.0/era_5g_interface/dataclasses/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/dataclasses/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1467 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/dataclasses/control_command.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      489 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/exceptions.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4031 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/h264_decoder.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4477 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/h264_encoder.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6030 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/interface_helpers.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/py.typed
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4458 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/server_channels.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6559 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/task_handler_internal_q.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-15 13:19:57.721716 era_5g_interface-0.8.0/era_5g_interface/utils/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/utils/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1097 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/utils/locked_set.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5978 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface/utils/rate_timer.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-15 13:19:57.721716 era_5g_interface-0.8.0/era_5g_interface.egg-info/
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      434 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface.egg-info/PKG-INFO
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      817 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      147 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface.egg-info/requires.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       17 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/era_5g_interface.egg-info/top_level.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2023-12-15 13:19:57.721716 era_5g_interface-0.8.0/setup.cfg
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1154 2023-12-15 13:19:57.000000 era_5g_interface-0.8.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-18 08:14:57.394314 era_5g_interface-0.9.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      434 2024-01-18 08:14:57.394314 era_5g_interface-0.9.0/PKG-INFO
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/backend_shim.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-18 08:14:57.382315 era_5g_interface-0.9.0/era_5g_interface/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    19374 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/channels.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4280 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/client_channels.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-18 08:14:57.390314 era_5g_interface-0.9.0/era_5g_interface/dataclasses/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/dataclasses/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1467 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/dataclasses/control_command.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      489 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/exceptions.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4199 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/frame_decoder.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5250 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/frame_encoder.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     8558 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/interface_helpers.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/py.typed
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4509 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/server_channels.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6559 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/task_handler_internal_q.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-18 08:14:57.394314 era_5g_interface-0.9.0/era_5g_interface/utils/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/utils/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1097 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/utils/locked_set.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5978 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/era_5g_interface/utils/rate_timer.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-01-18 08:14:57.386315 era_5g_interface-0.9.0/era_5g_interface.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      434 2024-01-18 08:14:57.000000 era_5g_interface-0.9.0/era_5g_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      819 2024-01-18 08:14:57.000000 era_5g_interface-0.9.0/era_5g_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-01-18 08:14:57.000000 era_5g_interface-0.9.0/era_5g_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-01-18 08:14:57.000000 era_5g_interface-0.9.0/era_5g_interface.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      147 2024-01-18 08:14:57.000000 era_5g_interface-0.9.0/era_5g_interface.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       17 2024-01-18 08:14:57.000000 era_5g_interface-0.9.0/era_5g_interface.egg-info/top_level.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-01-18 08:14:57.394314 era_5g_interface-0.9.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1154 2024-01-18 08:14:54.000000 era_5g_interface-0.9.0/setup.py
```

### Comparing `era_5g_interface-0.8.0/backend_shim.py` & `era_5g_interface-0.9.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.8.0/era_5g_interface/channels.py` & `era_5g_interface-0.9.0/era_5g_interface/channels.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import cv2
 import numpy as np
 import socketio
 import ujson
 from lz4.frame import compress, decompress
 
 from era_5g_interface.exceptions import BackPressureException, UnknownChannelTypeUsed
-from era_5g_interface.h264_decoder import H264Decoder, H264DecoderError
-from era_5g_interface.h264_encoder import H264Encoder, H264EncoderError
+from era_5g_interface.frame_decoder import FrameDecoder, FrameDecoderError
+from era_5g_interface.frame_encoder import FrameEncoder, FrameEncoderError
 
 logger = logging.getLogger(__name__)
 
 # TODO: use enums?
 DATA_NAMESPACE = str("/data")
 DATA_ERROR_EVENT = str("data_error")
 
@@ -33,78 +33,79 @@
 class ChannelType(Enum):
     """Channel type dataclass."""
 
     JSON = 1
     JPEG = 2
     H264 = 3
     JSON_LZ4 = 4
+    HEVC = 5
 
 
 @dataclass
 class CallbackInfoClient:
     """Callback info dataclass used on client side."""
 
     type: ChannelType
-    callback: Callable[[Dict], None]  # Custom callback with dict.
+    callback: Callable[[Dict], Any]  # Custom callback with dict.
     error_event: str = DATA_ERROR_EVENT  # Custom error event name.
 
 
 @dataclass
 class CallbackInfoServer:
     """Callback info dataclass used on server side - callback has namespace sid parameter."""
 
     type: ChannelType
-    callback: Callable[[str, Dict], None]  # Custom callback with sid and dict.
+    callback: Callable[[str, Dict], Any]  # Custom callback with sid and dict.
     error_event: str = DATA_ERROR_EVENT  # Custom error event name.
 
 
 class Channels(ABC):
     """Channels class is used to define channel data callbacks and contains send functions.
 
-    It handles image frames JPEG and H.264 encoding/decoding. Data is sent via the DATA_NAMESPACE. The class cannot be
-    used alone. The ServerChannels and ClientChannels classes create callbacks and encoders/decoders.
+    It handles image frames JPEG, H.264 and HEVC encoding/decoding. Data is sent via the DATA_NAMESPACE. The class
+    cannot be used alone. The ServerChannels and ClientChannels classes create callbacks and encoders/decoders.
     """
 
     # This should work roughly like an abstract member.
     _callbacks_info: Union[Dict[str, CallbackInfoClient], Dict[str, CallbackInfoServer]]
 
     def __init__(
         self,
         sio: Union[socketio.Client, socketio.Server],
         callbacks_info: Union[Dict[str, CallbackInfoClient], Dict[str, CallbackInfoServer]],
         back_pressure_size: Optional[int] = 5,
-        recreate_h264_attempts_count: int = 5,
+        recreate_coder_attempts_count: int = 5,
         stats: bool = False,
     ):
         """Constructor.
 
         Args:
             sio (Union[socketio.Client, socketio.Server]): Socketio Client or Server object.
             callbacks_info (Union[Dict[str, CallbackInfoClient], Dict[str, CallbackInfoServer]]): Callbacks Info
                 dictionary, key is custom event name.
             back_pressure_size (int, optional): Back pressure size - max size of eio.queue.qsize().
-            recreate_h264_attempts_count (int): How many times try to recreate the H.264 encoder/decoder.
+            recreate_coder_attempts_count (int): How many times try to recreate the frame encoder/decoder.
             stats (bool): Store output data sizes.
         """
 
         self._sio = sio
 
         if back_pressure_size is not None and back_pressure_size < 1:
             raise ValueError("Invalid value for back_pressure_size.")
 
         self._back_pressure_size = back_pressure_size
-        self._recreate_h264_attempts_count = recreate_h264_attempts_count
+        self._recreate_coder_attempts_count = recreate_coder_attempts_count
         self._stats = stats
         if self._stats:
             self._sizes: List[int] = []
 
         self._callbacks_info = callbacks_info
-        # For multiple H.264 streams, the encoders and the decoders are indexed by Tuple(eio_sid, event).
-        self._decoders: Dict[Tuple[str, str], H264Decoder] = dict()
-        self._encoders: Dict[Tuple[str, str], H264Encoder] = dict()
+        # For multiple frame streams, the encoders and the decoders are indexed by Tuple(eio_sid, event).
+        self._decoders: Dict[Tuple[str, str], FrameDecoder] = dict()
+        self._encoders: Dict[Tuple[str, str], FrameEncoder] = dict()
 
     @staticmethod
     def _shutdown(cb_type: str, event: str) -> None:
         logger.error(f"Unhandled exception in {cb_type} callback (event: {event}).", exc_info=sys.exc_info())
         logging.shutdown()  # should flush the logger
         os._exit(1)  # standard sys.exit() is not enough
 
@@ -128,107 +129,126 @@
         event: str,
         channel_type: ChannelType,
         timestamp: Optional[int] = None,
         metadata: Optional[Dict[str, Any]] = None,
         sid: Optional[str] = None,
         can_be_dropped: bool = True,
         wait_for_reconnection: bool = True,
+        blocking: bool = False,
         encoding_options: Optional[Dict[str, str]] = None,
-    ) -> None:
-        """Send general image data with JPEG or H.264 encoding via DATA_NAMESPACE.
+    ) -> Any:
+        """Send general image data with JPEG or H.264 or HEVC encoding via DATA_NAMESPACE.
 
         NOTE: DATA_NAMESPACE is assumed to be a connected namespace.
 
         Args:
             frame (np.ndarray): Video frame / image.
             event (str): Event name.
-            channel_type (ChannelType): Encoding type - ChannelType.JPEG or ChannelType.H264.
+            channel_type (ChannelType): Encoding type - ChannelType.JPEG or ChannelType.H264 or ChannelType.HEVC.
             timestamp (int): Frame timestamp.
             metadata (Dict[str, Any], optional): Optional metadata to send.
             sid (str, optional): Namespace sid - mandatory when sending from the server side to the client.
             can_be_dropped (bool): If data can be lost due to back pressure.
             wait_for_reconnection (bool): Wait for reconnection to server side? Wait is blocking.
-            encoding_options (Dict[str, str], optional): ChannelType.H264 options, e.g. {"crf": "0", "preset":
+            blocking (bool): If True, wait for the response. Defaults to False.
+            encoding_options (Dict[str, str], optional): Video codec options, e.g. {"crf": "0", "preset":
                 "ultrafast", "tune": "zerolatency", "x264-params": "keyint=5"}, default: {"preset": "ultrafast",
                 "tune": "zerolatency"}.
 
         Parameter frame.shape should not be changed after first send_image function call.
         Parameters encoding_options and frame.shape are only used in the first send_image call to create the encoder.
         """
 
-        if channel_type is not ChannelType.JPEG and channel_type is not ChannelType.H264:
+        if channel_type not in (ChannelType.JPEG, ChannelType.H264, ChannelType.HEVC):
             raise UnknownChannelTypeUsed()
 
         if timestamp is None:
             timestamp = time.perf_counter_ns()
         data: Dict[str, Any] = {"timestamp": timestamp}
         if metadata:
             data["metadata"] = metadata
         eio_sid = self.get_client_eio_sid(sid, DATA_NAMESPACE)
         encoder_id = (eio_sid, event)
-        if channel_type is ChannelType.H264:
+        if channel_type in (ChannelType.H264, ChannelType.HEVC):
             if encoder_id not in self._encoders:
                 try:
-                    logger.info(f"Creating H.264 encoder for image size {frame.shape[1]}x{frame.shape[0]}")
-                    self._encoders[encoder_id] = H264Encoder(frame.shape[1], frame.shape[0], options=encoding_options)
+                    if channel_type is ChannelType.H264:
+                        logger.info(f"Creating H.264 encoder for image size {frame.shape[1]}x{frame.shape[0]}")
+                        self._encoders[encoder_id] = FrameEncoder(
+                            frame.shape[1], frame.shape[0], codec="h264", options=encoding_options
+                        )
+                    elif channel_type is ChannelType.HEVC:
+                        logger.info(f"Creating HEVC encoder for image size {frame.shape[1]}x{frame.shape[0]}")
+                        self._encoders[encoder_id] = FrameEncoder(
+                            frame.shape[1], frame.shape[0], codec="hevc", options=encoding_options
+                        )
                 except Exception as e:
-                    logger.error(f"Cannot create H.264 encoder: {repr(e)}")
+                    logger.error(f"Cannot create video frame encoder: {repr(e)}")
                     raise e
         try:
             is_key_frame = False
-            if channel_type is ChannelType.H264:
+            if channel_type in (ChannelType.H264, ChannelType.HEVC):
                 frame_encoded = self._encoders[encoder_id].encode_ndarray(frame)
                 # TODO: dataclass for this data
-                data["h264"] = True
                 data["width"] = self._encoders[encoder_id].width()
                 data["height"] = self._encoders[encoder_id].height()
                 is_key_frame = self._encoders[encoder_id].last_frame_is_keyframe()
             else:
                 _, frame_jpeg = cv2.imencode(".jpg", frame)
                 frame_encoded = frame_jpeg.tobytes()
             data["frame"] = frame_encoded
             if self._stats:
                 # TODO: include all data size
                 self._sizes.append(len(frame_encoded))
                 logger.debug(f"Frame data size: {self._sizes[-1]}")
-            self.send_data(
-                data,
-                event,
-                sid=sid,
-                can_be_dropped=(can_be_dropped and not is_key_frame),
-            )
-        except H264EncoderError as e:
-            logger.error(f"H.264 encoder error: {e}")
+            if len(frame_encoded):
+                self.send_data(
+                    data,
+                    event,
+                    sid=sid,
+                    can_be_dropped=(can_be_dropped and not is_key_frame),
+                    wait_for_reconnection=wait_for_reconnection,
+                )
+            else:
+                logger.warning(
+                    "Encoded frame size is zero. It is possible that the encoder settings allow a delay "
+                    "of several frames at the beginning of the stream. This means that the timestamps "
+                    "will be shifted and will not match the original frames."
+                )
+        except FrameEncoderError as e:
+            logger.error(f"Video frame encoder error: {e}")
             # Try to recreate encoder
-            if self._encoders[encoder_id].get_init_count() < self._recreate_h264_attempts_count:
+            if self._encoders[encoder_id].get_init_count() < self._recreate_coder_attempts_count:
                 logger.info(f"Try to recreate encoder ... attempt {self._encoders[encoder_id].get_init_count()}")
                 self._encoders[encoder_id].encoder_init()
             else:
                 raise e
 
     def send_data(
         self,
         data: Dict[str, Any],
         event: str,
         channel_type: ChannelType = ChannelType.JSON,
         sid: Optional[str] = None,
         can_be_dropped: bool = False,
         wait_for_reconnection: bool = True,
-    ) -> None:
+        blocking: bool = False,
+    ) -> Any:
         """Send general JSON data via DATA_NAMESPACE.
 
         NOTE: DATA_NAMESPACE is assumed to be a connected namespace.
 
         Args:
             data (Dict[str, Any]): JSON data.
             event (str): Event name.
             channel_type (ChannelType): ChannelType.JSON for raw JSON or ChannelType.JSON_LZ4 for LZ4 compressed JSON.
             sid (str, optional): Namespace sid - mandatory when sending from the server side to the client.
             can_be_dropped (bool): If data can be lost due to back pressure.
             wait_for_reconnection (bool): Wait for reconnection to server side? Wait is blocking.
+            blocking (bool): If True, wait for the response. Defaults to False.
         """
 
         if channel_type is not ChannelType.JSON and channel_type is not ChannelType.JSON_LZ4:
             raise UnknownChannelTypeUsed()
 
         if can_be_dropped:
             self._apply_back_pressure(sid)
@@ -240,21 +260,27 @@
         if isinstance(self._sio, socketio.Client):
             if wait_for_reconnection:
                 while not self._sio.connected or not self._sio.eio.state:
                     logger.info("Waiting for reconnection ...")
                     if not self._sio._reconnect_task or not self._sio._reconnect_task.is_alive():
                         break
                     time.sleep(1)
-            self._sio.emit(event, new_data, namespace=DATA_NAMESPACE)
+            if blocking:
+                return self._sio.call(event, new_data, namespace=DATA_NAMESPACE)
+            else:
+                self._sio.emit(event, new_data, namespace=DATA_NAMESPACE)
         else:
             if sid is None:
                 raise ValueError("'sid' has to be set for server.")
             if not self._sio.manager.is_connected(sid, DATA_NAMESPACE):
                 raise ConnectionError(f"Client with {DATA_NAMESPACE} sid {sid} is not connected to server.")
-            self._sio.emit(event, new_data, namespace=DATA_NAMESPACE, to=sid)
+            if blocking:
+                self._sio.call(event, new_data, namespace=DATA_NAMESPACE, to=sid)
+            else:
+                self._sio.emit(event, new_data, namespace=DATA_NAMESPACE, to=sid)
 
     def get_client_eio_sid(self, sid: Optional[str] = None, namespace: Optional[str] = None) -> str:
         """Get client eio sid.
 
         Args:
             sid (str, optional): Namespace sid - mandatory for using on the server side.
             namespace (str, optional): Namespace - mandatory for using on the server side.
@@ -277,15 +303,15 @@
             data (Dict[str, Any]): JSON data.
             sid (str, optional): Namespace sid - only on the server side.
         """
 
         logger.error(f"Data error, eio_sid {self.get_client_eio_sid(sid, DATA_NAMESPACE)}, sid {sid}, data {data}")
 
     def image_decode(self, data: Dict[str, Any], event: str, sid: Optional[str] = None) -> Optional[Dict]:
-        """Decode JPEG or H.264 encoded image received on DATA_NAMESPACE.
+        """Decode JPEG or H.264 or HEVC encoded image received on DATA_NAMESPACE.
 
         Args:
             data (Dict[str, Any]): Received dictionary with frame data.
             event (str): Event name.
             sid (str, optional): Namespace sid - only on the server side.
         """
 
@@ -302,33 +328,40 @@
                 self._callbacks_info[event].error_event,
                 sid=sid,
             )
             return None
 
         eio_sid = self.get_client_eio_sid(sid, DATA_NAMESPACE)
         decoder_id = (eio_sid, event)
-        if self._callbacks_info[event].type is ChannelType.H264 and decoder_id not in self._decoders:
+        if (
+            self._callbacks_info[event].type in (ChannelType.H264, ChannelType.HEVC)
+            and decoder_id not in self._decoders
+        ):
             if "width" not in data or "height" not in data:
-                logger.error("Data does not contain width or height, it is mandatory for H.264.")
+                logger.error("Data does not contain width or height, it is mandatory for video frame decoder.")
                 self.send_data(
                     {
                         "timestamp": timestamp,
-                        "error": "Data does not contain width or height, it is mandatory for H.264.",
+                        "error": "Data does not contain width or height, it is mandatory for video frame decoder.",
                     },
                     self._callbacks_info[event].error_event,
                     sid=sid,
                 )
                 return None
             try:
-                logger.info(f"Creating H.264 decoder for image size {data['width']}x{data['height']}")
-                self._decoders[decoder_id] = H264Decoder(data["width"], data["height"])
+                if self._callbacks_info[event].type is ChannelType.H264:
+                    logger.info(f"Creating H.264 decoder for image size {data['width']}x{data['height']}")
+                    self._decoders[decoder_id] = FrameDecoder(data["width"], data["height"], codec="h264")
+                elif self._callbacks_info[event].type is ChannelType.HEVC:
+                    logger.info(f"Creating HEVC decoder for image size {data['width']}x{data['height']}")
+                    self._decoders[decoder_id] = FrameDecoder(data["width"], data["height"], codec="hevc")
             except Exception as e:
-                logger.error(f"Cannot create H.264 decoder: {repr(e)}")
+                logger.error(f"Cannot create video frame decoder: {repr(e)}")
                 self.send_data(
-                    {"timestamp": timestamp, "error": f"Cannot create H.264 decoder: {repr(e)}"},
+                    {"timestamp": timestamp, "error": f"Cannot create video frame decoder: {repr(e)}"},
                     self._callbacks_info[event].error_event,
                     sid=sid,
                 )
                 return None
 
         if decoder_id in self._decoders:
             last_timestamp = self._decoders[decoder_id].last_timestamp
@@ -336,34 +369,36 @@
                 logger.error(
                     f"Received frame with older timestamp: {timestamp}, "
                     f"last_timestamp: {last_timestamp}, diff: {timestamp - last_timestamp}"
                 )
                 self.send_data(
                     {
                         "timestamp": timestamp,
-                        "error": f"Received frame with older timestamp: {timestamp}, "
-                        f"last_timestamp: {last_timestamp}, diff: {timestamp - last_timestamp}",
+                        "error": (
+                            f"Received frame with older timestamp: {timestamp}, "
+                            f"last_timestamp: {last_timestamp}, diff: {timestamp - last_timestamp}"
+                        ),
                     },
                     self._callbacks_info[event].error_event,
                     sid=sid,
                 )
                 return None
             self._decoders[decoder_id].last_timestamp = timestamp
 
         if decoder_id in self._decoders:
             try:
                 frame_decoded = self._decoders[decoder_id].decode_packet_data(data["frame"])
-            except H264DecoderError as e:
-                logger.error(f"H.264 decoder error: {e}")
+            except FrameDecoderError as e:
+                logger.error(f"Video frame decoder error: {e}")
                 # Try to recreate decoder
-                if self._decoders[decoder_id].get_init_count() < self._recreate_h264_attempts_count:
+                if self._decoders[decoder_id].get_init_count() < self._recreate_coder_attempts_count:
                     logger.info(f"Try to recreate decoder ... attempt {self._decoders[decoder_id].get_init_count()}")
-                    self._decoders[decoder_id].decoder_init()
+                    # self._decoders[decoder_id].decoder_init()
                 self.send_data(
-                    {"timestamp": timestamp, "error": f"H.264 decoder error: {e}"},
+                    {"timestamp": timestamp, "error": f"Video frame decoder error: {e}"},
                     self._callbacks_info[event].error_event,
                     sid=sid,
                 )
                 return None
         else:
             try:
                 frame_decoded = cv2.imdecode(np.frombuffer(data["frame"], dtype=np.uint8), cv2.IMREAD_COLOR)
```

### Comparing `era_5g_interface-0.8.0/era_5g_interface/client_channels.py` & `era_5g_interface-0.9.0/era_5g_interface/client_channels.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class ClientChannels(Channels):
     """Channels class is used to define channel data callbacks and contains send functions.
 
-    It handles image frames JPEG and H.264, and JSON LZ4 encoding/decoding. Data is sent via the DATA_NAMESPACE.
+    It handles image frames JPEG, H.264 and HEVC, and JSON LZ4 encoding/decoding. Data is sent via the DATA_NAMESPACE.
     """
 
     _callbacks_info: Dict[str, CallbackInfoClient]
 
     def __init__(
         self,
         sio: socketio.Client,
@@ -26,15 +26,15 @@
         """Constructor.
 
         Args:
             sio (socketio.Client): Socketio Client object.
             callbacks_info (Dict[str, CallbackInfoClient]): Callbacks Info dictionary, key is custom event name.
             disconnect_callback (Callable, optional): Triggered on client side before _shutdown on unhandled exception.
             back_pressure_size (int, optional): Back pressure size - max size of eio.queue.qsize().
-            recreate_h264_attempts_count (int): How many times try to recreate the H.264 encoder/decoder.
+            recreate_coder_attempts_count (int): How many times try to recreate the video frame encoder/decoder.
             stats (bool): Store output data sizes.
         """
 
         super().__init__(sio, callbacks_info, **kwargs)
 
         self._disconnect_callback = disconnect_callback
 
@@ -50,63 +50,63 @@
                 )
             elif callback_info.type is ChannelType.JSON_LZ4:
                 self._sio.on(
                     event,
                     lambda data, local_event=event: self.json_lz4_callback(data, local_event),
                     namespace=DATA_NAMESPACE,
                 )
-            elif callback_info.type in (ChannelType.JPEG, ChannelType.H264):
+            elif callback_info.type in (ChannelType.JPEG, ChannelType.H264, ChannelType.HEVC):
                 self._sio.on(
                     event,
                     lambda data, local_event=event: self.image_callback(data, local_event),
                     namespace=DATA_NAMESPACE,
                 )
             else:
                 raise ValueError(f"Unknown channel type: {callback_info.type}")
 
-    def json_callback(self, data: Dict[str, Any], event: str) -> None:
+    def json_callback(self, data: Dict[str, Any], event: str) -> Any:
         """Allows to receive general JSON data on DATA_NAMESPACE.
 
         Args:
             data (Dict[str, Any]): JSON data.
             event (str): Event name.
         """
 
         cb_info = self._callbacks_info[event]
 
         try:
-            cb_info.callback(data)
+            return cb_info.callback(data)
         except Exception:
             if self._disconnect_callback:
                 self._disconnect_callback()
             Channels._shutdown("JSON", event)
 
-    def json_lz4_callback(self, data: bytes, event: str) -> None:
+    def json_lz4_callback(self, data: bytes, event: str) -> Any:
         """Allows to receive LZ4 compressed general JSON data on DATA_NAMESPACE.
 
         Args:
             data (bytes): LZ4 compressed JSON data.
             event (str): Event name.
         """
 
         decoded_data = super().data_lz4_decode(data, event)
         if decoded_data:
-            self.json_callback(decoded_data, event)
+            return self.json_callback(decoded_data, event)
 
-    def image_callback(self, data: Dict[str, Any], event: str) -> None:
-        """Allows to receive JPEG or H.264 encoded image on DATA_NAMESPACE.
+    def image_callback(self, data: Dict[str, Any], event: str) -> Any:
+        """Allows to receive JPEG or H.264 or HEVC encoded image on DATA_NAMESPACE.
 
         Args:
             data (Dict[str, Any]): Received dictionary with frame data.
             event (str): Event name.
         """
 
         cb_info = self._callbacks_info[event]
 
         decoded_data = super().image_decode(data, event)
         if decoded_data:
             try:
-                cb_info.callback(decoded_data)
+                return cb_info.callback(decoded_data)
             except Exception:
                 if self._disconnect_callback:
                     self._disconnect_callback()
                 Channels._shutdown("image", event)
```

### Comparing `era_5g_interface-0.8.0/era_5g_interface/dataclasses/control_command.py` & `era_5g_interface-0.9.0/era_5g_interface/dataclasses/control_command.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.8.0/era_5g_interface/h264_decoder.py` & `era_5g_interface-0.9.0/era_5g_interface/frame_decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,42 +4,44 @@
 from av.codec import CodecContext
 from av.error import FFmpegError, tag_to_code
 from av.packet import Packet
 from av.video.codeccontext import VideoCodecContext
 from av.video.frame import VideoFrame
 
 
-class H264DecoderError(Exception):
-    """H264DecoderError Exception."""
+class FrameDecoderError(Exception):
+    """FrameDecoderError Exception."""
 
     pass
 
 
 # TODO: only for testing purpose
+# from pathlib import Path
 # Path("output").mkdir(parents=True, exist_ok=True)
 
-logger = logging.getLogger("H.264 decoder")
+logger = logging.getLogger("Video frame decoder")
 
 
-class H264Decoder:
-    """H.264 Decoder."""
+class FrameDecoder:
+    """Video frame Decoder."""
 
-    def __init__(self, width: int, height: int, fps: float = 30) -> None:
+    def __init__(self, width: int, height: int, fps: float = 30, codec: str = "h264") -> None:
         """Constructor.
 
         Args:
             width (int): Video frame width.
             height (int): Video frame height.
             fps (float): Video framerate (FPS), default: 30.
+            codec (str): Video codec name, e.g. h264, hevc, or vp9, default: h264.
         """
         self._fps = fps
         self._width = width
         self._height = height
         self._pix_fmt = "yuv420p"
-        self._decoder: VideoCodecContext = CodecContext.create("h264", "r")
+        self._decoder: VideoCodecContext = CodecContext.create(codec, "r")
         self._init_count = 0
         self.last_timestamp: int = 0
         self._last_frame_is_keyframe = False
         self.decoder_init()
 
     def width(self) -> int:
         """Get video frame width.
@@ -65,22 +67,24 @@
         Returns:
             Video framerate.
         """
 
         return self._fps
 
     def decoder_init(self) -> None:
-        """Init H.264 decoder."""
+        """Init video decoder."""
 
         self._init_count += 1
-        self._decoder = CodecContext.create("h264", "r")
+        if self._decoder.is_open:
+            self._decoder.close()
         self._decoder.width = self._width
         self._decoder.height = self._height
         self._decoder.framerate = self._fps
         self._decoder.pix_fmt = self._pix_fmt
+        self._decoder.open()
 
     def get_init_count(self) -> int:
         """Get decoder init attempts count.
 
         Returns:
             Decoder init attempts count.
         """
@@ -93,15 +97,15 @@
         Returns:
             True if last frame is keyframe.
         """
 
         return self._last_frame_is_keyframe
 
     def decode_packet_data(self, packet_data: bytes, format: str = "bgr24") -> np.ndarray:
-        """Decode H.264 packets bytes to ndarray.
+        """Decode packets bytes to ndarray.
 
         Args:
             packet_data (bytes): Packet data.
             format (str): Image format.
 
         Returns:
             Video frame / image.
@@ -110,27 +114,27 @@
         try:
             packet = Packet(packet_data)
 
             # Multiple frames? - This should not happen because on the encoders side one frame is always encoded and sent
             frame: VideoFrame
             for frame in self._decoder.decode(packet):
                 # TODO: only for testing purpose
-                # logger.debug(f"Frame {frame} with id {frame.index} decoded from packet: {packet}")
-                # logger.debug(
-                #    f"frame.pts: {frame.pts}, "
-                #    f"frame.dts: {frame.dts}, "
-                #    f"frame.index: {frame.index}, "
-                #    f"frame.key_frame: {frame.key_frame}, "
-                #    f"frame.is_corrupt: {frame.is_corrupt}, "
-                #    f"frame.time: {frame.time}"
-                # )
+                logger.debug(f"Frame {frame} with id {frame.index} decoded from packet: {packet}")
+                logger.debug(
+                    f"frame.pts: {frame.pts}, "
+                    f"frame.dts: {frame.dts}, "
+                    f"frame.index: {frame.index}, "
+                    f"frame.key_frame: {frame.key_frame}, "
+                    f"frame.is_corrupt: {frame.is_corrupt}, "
+                    f"frame.time: {frame.time}"
+                )
                 # TODO: only for testing purpose
-                # frame.to_image().save('output/frame-%04d.jpg' % frame.index)
+                # frame.to_image().save("output/frame-%04d.jpg" % frame.index)
 
                 self._last_frame_is_keyframe = frame.key_frame
                 frame_ndarray: np.ndarray = frame.to_ndarray(format=format)
                 return frame_ndarray
             # Sometimes, with dropping some TCP packets, no frame is decoded from av.Packet while no FFmpegError is
             # raised. This is resolved by throwing this exception.
             raise FFmpegError(tag_to_code(b"INDA"), f"No frame decoded from packet {packet}")
         except FFmpegError as e:
-            raise H264DecoderError(e)
+            raise FrameDecoderError(e)
```

### Comparing `era_5g_interface-0.8.0/era_5g_interface/h264_encoder.py` & `era_5g_interface-0.9.0/era_5g_interface/frame_encoder.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,55 +5,66 @@
 from av.codec import CodecContext
 from av.error import FFmpegError
 from av.packet import Packet
 from av.video.codeccontext import VideoCodecContext
 from av.video.frame import VideoFrame
 
 
-class H264EncoderError(Exception):
-    """FFmpegError Exception."""
+class FrameEncoderError(Exception):
+    """FrameEncoderError Exception."""
 
     pass
 
 
 # TODO: only for testing purpose
+# from pathlib import Path
 # Path("input").mkdir(parents=True, exist_ok=True)
 
-logger = logging.getLogger("H.264 encoder")
+logger = logging.getLogger("Video frame encoder")
 
 
-class H264Encoder:
-    """H.264 Encoder."""
+class FrameEncoder:
+    """Video frame Encoder."""
 
-    def __init__(self, width: int, height: int, fps: float = 30, options: Optional[Dict[str, str]] = None) -> None:
+    def __init__(
+        self, width: int, height: int, fps: float = 30, codec: str = "h264", options: Optional[Dict[str, str]] = None
+    ) -> None:
         """Constructor.
 
         Args:
             width (int): Video frame width.
             height (int): Video frame height.
             fps (float): Video framerate (FPS), default: 30.
-            options (Dict[str, str], optional): H264 options, e.g. {"crf": "0", "preset": "ultrafast",
+            codec (str): Video codec name, e.g. h264, hevc, or vp9, default: h264.
+            options (Dict[str, str], optional): Codec options, e.g. {"crf": "0", "preset": "ultrafast",
                 "tune": "zerolatency", "x264-params": "keyint=5"}, default: {"preset": "ultrafast",
                 "tune": "zerolatency"}.
         """
 
+        # Some default options.
         if options is None:
-            options = {"preset": "ultrafast", "tune": "zerolatency"}
+            if codec == "h264":
+                options = {"preset": "ultrafast", "tune": "zerolatency"}
+            elif codec == "hevc":
+                options = {"crf": "10", "preset": "ultrafast", "tune": "zerolatency", "x265-params": "frame-threads=1"}
+            elif codec == "vp9":
+                options = {"quality": "realtime", "speed": "8", "lag-in-frames": "0"}
+        logger.debug(f"Encoder ({codec}) options: {options}")
 
         # TODO: only for testing purpose
         # options = {"crf": "0", "preset": "ultrafast", "tune": "zerolatency"}
         # options = {"preset": "ultrafast", "tune": "zerolatency", "x264-params": "keyint=5"}
         # self.frame_id = 0
 
         self._fps = fps
         self._width = width
         self._height = height
         self._options = options
         self._pix_fmt = "yuv420p"
-        self._encoder: VideoCodecContext = CodecContext.create("h264", "w")
+        self._encoder: VideoCodecContext = CodecContext.create(codec, "w")
         self._init_count = 0
         self.last_timestamp: int = 0
         self._last_frame_is_keyframe = False
         self.encoder_init()
 
     def width(self) -> int:
         """Get video frame width.
@@ -79,23 +90,25 @@
         Returns:
             Video framerate.
         """
 
         return self._fps
 
     def encoder_init(self) -> None:
-        """Init H.264 encoder."""
+        """Init video encoder."""
 
         self._init_count += 1
-        self._encoder = CodecContext.create("h264", "w")
+        if self._encoder.is_open:
+            self._encoder.close()
         self._encoder.width = self._width
         self._encoder.height = self._height
         self._encoder.framerate = self._fps
         self._encoder.pix_fmt = self._pix_fmt
         self._encoder.options = self._options
+        self._encoder.open()
 
     def get_init_count(self) -> int:
         """Get encoder init attempts count.
 
         Returns:
             Encoder init attempts count.
         """
@@ -108,44 +121,48 @@
         Returns:
             True if last frame is keyframe.
         """
 
         return self._last_frame_is_keyframe
 
     def encode_ndarray(self, frame_data: np.ndarray, format: str = "bgr24") -> bytes:
-        """Encode ndarray to H.264 packets bytes.
+        """Encode ndarray to packets bytes.
 
         Args:
             frame_data (ndarray): Video frame / image.
             format (str): Image format.
 
         Returns:
             Packet data.
         """
 
         try:
             frame = VideoFrame.from_ndarray(frame_data, format=format)
             # TODO: only for testing purpose
-            # frame.to_image().save('input/frame-%04d.jpg' % self.frame_id)
+            # frame.to_image().save("input/frame-%04d.jpg" % self.frame_id)
             # self.frame_id += 1
 
             self._last_frame_is_keyframe = False
             packets = []
             packet: Packet
             for packet in self._encoder.encode(frame):
                 # TODO: only for testing purpose
-                # logger.debug(f"Frame {frame} encoded to packet: {packet}")
-                # logger.debug(
-                #    f"packet.pts: {packet.pts}, "
-                #    f"packet.dts: {packet.dts}, "
-                #    f"packet.key_frame: {packet.is_keyframe}, "
-                #    f"packet.is_corrupt: {packet.is_corrupt}"
-                # )
+                logger.debug(f"Frame {frame} encoded to packet: {packet}")
+                logger.debug(
+                    f"packet.pts: {packet.pts}, "
+                    f"packet.dts: {packet.dts}, "
+                    f"packet.key_frame: {packet.is_keyframe}, "
+                    f"packet.is_corrupt: {packet.is_corrupt}"
+                )
                 if packet.is_keyframe:
                     self._last_frame_is_keyframe = True
                 packets.append(bytes(packet))
 
+            # TODO: only for testing purpose
+            # if len(packets) == 0:
+            #    raise FFmpegError(tag_to_code(b"INDA"), f"No packet encoded from frame {frame}")
+
             if len(packets) > 1:
                 logger.info(f"Frame {frame} encoded to multiple packets: {packets}")
             return b"".join(packets)
         except FFmpegError as e:
-            raise H264EncoderError(e)
+            raise FrameEncoderError(e)
```

### Comparing `era_5g_interface-0.8.0/era_5g_interface/interface_helpers.py` & `era_5g_interface-0.9.0/era_5g_interface/interface_helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,20 +6,32 @@
 
 import numpy as np
 import requests
 from requests.adapters import HTTPAdapter, Retry
 
 logger = logging.getLogger(__name__)
 
-NETAPP_ID = str(os.getenv("NETAPP_ID", "00000000-0000-0000-0000-000000000000"))
+# Middleware Network Application ID (task ID, NETAPP_ID).
+MIDDLEWARE_TASK_ID = str(
+    os.getenv("MIDDLEWARE_TASK_ID", os.getenv("NETAPP_ID", "00000000-0000-0000-0000-000000000000"))
+)
+# NETAPP_ID used for compatibility.
+NETAPP_ID = MIDDLEWARE_TASK_ID
 NETAPP_ID_ROS = NETAPP_ID.replace("-", "_")
+# Middleware robot ID (robot ID).
+MIDDLEWARE_ROBOT_ID = str(os.getenv("MIDDLEWARE_ROBOT_ID", "00000000-0000-0000-0000-000000000000"))
+# Middleware address.
 MIDDLEWARE_ADDRESS = str(os.getenv("MIDDLEWARE_ADDRESS", "http://localhost"))
 MIDDLEWARE_REPORT_INTERVAL = float(os.getenv("MIDDLEWARE_REPORT_INTERVAL", 1))
+# Used for Network Application heart beat.
 MAX_LATENCY = float(os.getenv("NETAPP_MAX_LATENCY", 100))
 
+# Event name used for communication between clients and heartbeat module.
+HEARTBEAT_CLIENT_EVENT = "heartbeat_client_event"
+
 
 class LatencyMeasurements:
     """Class for holding data about processing times (latency)."""
 
     def __init__(self, num_latencies_to_keep: int = 10) -> None:
         self.num_latencies_to_keep = num_latencies_to_keep
         self.processing_latencies = np.zeros(num_latencies_to_keep)
@@ -96,45 +108,95 @@
 
         self.retries = Retry(total=0, read=0, connect=0, backoff_factor=0, status_forcelist=[429, 500, 502, 503, 504])
         self.session: requests.Session = requests.Session()
         self.adapter: HTTPAdapter = HTTPAdapter(max_retries=self.retries)
         self.session.mount(MIDDLEWARE_ADDRESS, self.adapter)
         self.connection_error = False
 
-    def _send_middleware_heart_beat_request(self, headers: Dict, json: Dict) -> None:
+    def _send_heart_beat_request(self, headers: Dict, json: Dict, repeat_on_error: bool = False) -> None:
         """Send heart beat request to Middleware.
 
         Args:
             headers (Dict): Request headers.
             json (Dict): Request JSON.
+            repeat_on_error (bool): If set, repeat requests further. Defaults to False.
         """
 
-        if not self.connection_error:
+        if not self.connection_error or repeat_on_error:
             logger.debug(f"Sending heart beat to middleware: {json}")
             try:
                 response = self.session.post(MIDDLEWARE_ADDRESS, headers=headers, json=json, timeout=(0.2, 0.2))
                 if response.ok:
                     logger.debug(f"Middleware heart beat response: {response.text}")
                 else:
-                    logger.warning(f"Middleware heart beat response: {response}")
+                    logger.warning(
+                        f"Middleware heart beat response: {response}, middleware address: {MIDDLEWARE_ADDRESS}"
+                    )
                     self.connection_error = True
             except requests.RequestException as ex:
                 logger.warning(f"Failed to connect to the middleware address: {MIDDLEWARE_ADDRESS}, {repr(ex)}")
                 self.connection_error = True
 
+    def send_robot_heart_beat(
+        self,
+        battery_level: float,
+        cpu_utilization: List[float],
+        ram_utilization: float,
+        quality_map_status=None,
+        repeat_on_error: bool = False,
+    ) -> None:
+        """Send robot heart beat to Middleware.
+
+        Args:
+            battery_level (float): Robot battery level.
+            cpu_utilization (float): Robot CPU utilization.
+            ram_utilization (float):  Robot RAM utilization.
+            quality_map_status (None): Unused, will be updated.
+            repeat_on_error (bool): If set, repeat requests further. Defaults to False.
+        """
+
+        data = {
+            "RobotId": MIDDLEWARE_ROBOT_ID,
+            "BatteryLevel": battery_level,
+            "CPUUtilization": cpu_utilization,
+            "RAMUtilization": ram_utilization,
+            "QualityMapStatus": quality_map_status,
+        }
+        headers = {"Content-type": "application/json"}
+        self._send_heart_beat_request(headers=headers, json=data, repeat_on_error=repeat_on_error)
+
     def send_middleware_heart_beat(
         self, avg_latency: float, queue_size: int, queue_occupancy: float, current_robot_count: int
     ) -> None:
-        """Send heart beat to Middleware.
+        """Obsolete function, use send_application_heart_beat instead.
+
+        Args:
+            avg_latency (float): Average latency.
+            queue_size (int): Queue size.
+            queue_occupancy (float): Queue occupancy.
+            current_robot_count (int): Current robot count.
+        """
+        self.send_application_heart_beat(avg_latency, queue_size, queue_occupancy, current_robot_count)
+
+    def send_application_heart_beat(
+        self,
+        avg_latency: float,
+        queue_size: int,
+        queue_occupancy: float,
+        current_robot_count: int,
+        repeat_on_error: bool = False,
+    ) -> None:
+        """Send application heart beat to Middleware.
 
         Args:
             avg_latency (float): Average latency.
             queue_size (int): Queue size.
             queue_occupancy (float): Queue occupancy.
             current_robot_count (int): Current robot count.
+            repeat_on_error (bool): If set, repeat requests further. Defaults to False.
         """
 
         # Latency can change over time, so reporting just the simple que occupancy can be misleading.
         # Instead, it is better to report occupancy in terms of:
         #  'total time estimated to be needed to process everything in the queue' / 'required max latency'
         processing_time_occupancy = queue_size * avg_latency / MAX_LATENCY
 
@@ -149,14 +211,14 @@
             hard_robot_count_limit = math.floor(current_robot_count / queue_occupancy)
             optimal_robot_count_limit = math.floor(hard_robot_count_limit * 0.8)
         else:
             hard_robot_count_limit = math.floor(current_robot_count / processing_time_occupancy)
             optimal_robot_count_limit = math.floor(hard_robot_count_limit * 0.8)
 
         data = {
-            "Id": NETAPP_ID,
+            "Id": MIDDLEWARE_TASK_ID,
             "CurrentRobotsCount": current_robot_count,
             "OptimalLimit": optimal_robot_count_limit,
             "HardLimit": hard_robot_count_limit,
         }
         headers = {"Content-type": "application/json"}
-        self._send_middleware_heart_beat_request(headers=headers, json=data)
+        self._send_heart_beat_request(headers=headers, json=data, repeat_on_error=repeat_on_error)
```

### Comparing `era_5g_interface-0.8.0/era_5g_interface/server_channels.py` & `era_5g_interface-0.9.0/era_5g_interface/server_channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class ServerChannels(Channels):
     """Channels class is used to define channel data callbacks and contains send functions.
 
-    It handles image frames JPEG and H.264, and JSON LZ4 encoding/decoding. Data is sent via the DATA_NAMESPACE.
+    It handles image frames JPEG, H.264 and HEVC, and JSON LZ4 encoding/decoding. Data is sent via the DATA_NAMESPACE.
     """
 
     _callbacks_info: Dict[str, CallbackInfoServer]
 
     def __init__(
         self,
         sio: socketio.Server,
@@ -25,15 +25,15 @@
     ):
         """Constructor.
 
         Args:
             sio (socketio.Server): Socketio Server object.
             callbacks_info (Dict[str, CallbackInfoServer]): Callbacks Info dictionary, key is custom event name.
             back_pressure_size (int, optional): Back pressure size - max size of eio.queue.qsize().
-            recreate_h264_attempts_count (int): How many times try to recreate the H.264 encoder/decoder.
+            recreate_coder_attempts_count (int): How many times try to recreate the frame encoder/decoder.
             stats (bool): Store output data sizes.
         """
 
         super().__init__(sio, callbacks_info, **kwargs)
 
         self._disconnect_callback = disconnect_callback
 
@@ -49,66 +49,66 @@
                 )
             elif callback_info.type is ChannelType.JSON_LZ4:
                 self._sio.on(
                     event,
                     lambda sid, data, local_event=event: self.json_lz4_callback(data, local_event, sid),
                     namespace=DATA_NAMESPACE,
                 )
-            elif callback_info.type in (ChannelType.JPEG, ChannelType.H264):
+            elif callback_info.type in (ChannelType.JPEG, ChannelType.H264, ChannelType.HEVC):
                 self._sio.on(
                     event,
                     lambda sid, data, local_event=event: self.image_callback(data, local_event, sid),
                     namespace=DATA_NAMESPACE,
                 )
             else:
                 raise ValueError(f"Unknown channel type: {callback_info.type}")
 
-    def json_callback(self, data: Dict[str, Any], event: str, sid: str) -> None:
+    def json_callback(self, data: Dict[str, Any], event: str, sid: str) -> Any:
         """Allows to receive general JSON data on DATA_NAMESPACE.
 
         Args:
             data (Dict[str, Any]): JSON data.
             event (str): Event name.
             sid (str, optional): Namespace sid - only on the server side.
         """
 
         cb_info = self._callbacks_info[event]
 
         try:
-            cb_info.callback(sid, data)
+            return cb_info.callback(sid, data)
         except Exception:
             if self._disconnect_callback:
                 self._disconnect_callback(sid, DATA_NAMESPACE)
             Channels._shutdown("JSON", event)
 
-    def json_lz4_callback(self, data: bytes, event: str, sid: str) -> None:
+    def json_lz4_callback(self, data: bytes, event: str, sid: str) -> Any:
         """Allows to receive LZ4 compressed general JSON data on DATA_NAMESPACE.
 
         Args:
             data (bytes): LZ4 compressed JSON data.
             event (str): Event name.
             sid (str, optional): Namespace sid - only on the server side.
         """
 
         decoded_data = super().data_lz4_decode(data, event, sid)
         if decoded_data:
-            self.json_callback(decoded_data, event, sid)
+            return self.json_callback(decoded_data, event, sid)
 
-    def image_callback(self, data: Dict[str, Any], event: str, sid: str) -> None:
-        """Allows to receive JPEG or H.264 encoded image on DATA_NAMESPACE.
+    def image_callback(self, data: Dict[str, Any], event: str, sid: str) -> Any:
+        """Allows to receive JPEG or H.264 or HEVC encoded image on DATA_NAMESPACE.
 
         Args:
             data (Dict[str, Any]): Received dictionary with frame data.
             event (str): Event name.
             sid (str, optional): Namespace sid - only on the server side.
         """
 
         cb_info = self._callbacks_info[event]
 
         decoded_data = super().image_decode(data, event, sid)
         if decoded_data:
             try:
-                cb_info.callback(sid, decoded_data)
+                return cb_info.callback(sid, decoded_data)
             except Exception:
                 if self._disconnect_callback:
                     self._disconnect_callback(sid, DATA_NAMESPACE)
                 Channels._shutdown("image", event)
```

### Comparing `era_5g_interface-0.8.0/era_5g_interface/task_handler_internal_q.py` & `era_5g_interface-0.9.0/era_5g_interface/task_handler_internal_q.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.8.0/era_5g_interface/utils/locked_set.py` & `era_5g_interface-0.9.0/era_5g_interface/utils/locked_set.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.8.0/era_5g_interface/utils/rate_timer.py` & `era_5g_interface-0.9.0/era_5g_interface/utils/rate_timer.py`

 * *Files identical despite different names*

### Comparing `era_5g_interface-0.8.0/era_5g_interface.egg-info/SOURCES.txt` & `era_5g_interface-0.9.0/era_5g_interface.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 MANIFEST.in
 backend_shim.py
 setup.py
 era_5g_interface/__init__.py
 era_5g_interface/channels.py
 era_5g_interface/client_channels.py
 era_5g_interface/exceptions.py
-era_5g_interface/h264_decoder.py
-era_5g_interface/h264_encoder.py
+era_5g_interface/frame_decoder.py
+era_5g_interface/frame_encoder.py
 era_5g_interface/interface_helpers.py
 era_5g_interface/py.typed
 era_5g_interface/server_channels.py
 era_5g_interface/task_handler_internal_q.py
 era_5g_interface.egg-info/PKG-INFO
 era_5g_interface.egg-info/SOURCES.txt
 era_5g_interface.egg-info/dependency_links.txt
```

### Comparing `era_5g_interface-0.8.0/setup.py` & `era_5g_interface-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,9 +35,9 @@
     },
     'packages': (
         'era_5g_interface',
         'era_5g_interface.dataclasses',
         'era_5g_interface.utils',
     ),
     'python_requires': '>=3.8',
-    'version': '0.8.0',
+    'version': '0.9.0',
 })
```

