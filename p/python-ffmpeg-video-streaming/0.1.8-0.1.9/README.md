# Comparing `tmp/python-ffmpeg-video-streaming-0.1.8.tar.gz` & `tmp/python-ffmpeg-video-streaming-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\python-ffmpeg-video-streaming-0.1.8.tar", last modified: Thu Jun 11 00:01:41 2020, max compression
+gzip compressed data, was "dist\python-ffmpeg-video-streaming-0.1.9.tar", last modified: Sun Jun 21 19:23:23 2020, max compression
```

## Comparing `python-ffmpeg-video-streaming-0.1.8.tar` & `python-ffmpeg-video-streaming-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2020-06-11 00:01:41.143299 python-ffmpeg-video-streaming-0.1.8/
--rw-rw-rw-   0        0        0    22749 2020-06-11 00:01:41.141301 python-ffmpeg-video-streaming-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    19006 2020-06-10 23:38:09.000000 python-ffmpeg-video-streaming-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2020-06-11 00:01:41.095298 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/
--rw-rw-rw-   0        0        0      295 2020-04-20 00:29:55.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/__init__.py
--rw-rw-rw-   0        0        0     6655 2020-05-04 22:24:22.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_clouds.py
--rw-rw-rw-   0        0        0     3845 2020-06-10 23:14:38.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_command_builder.py
--rw-rw-rw-   0        0        0     4912 2020-06-10 23:38:09.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_format.py
--rw-rw-rw-   0        0        0     3258 2020-06-10 17:26:49.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_hls_helper.py
--rw-rw-rw-   0        0        0     4503 2020-06-10 22:11:31.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_input.py
--rw-rw-rw-   0        0        0     7291 2020-06-10 23:56:00.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_media.py
--rw-rw-rw-   0        0        0     4400 2020-06-10 16:58:37.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_media_property.py
--rw-rw-rw-   0        0        0     3665 2020-06-08 23:50:35.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_process.py
--rw-rw-rw-   0        0        0     3274 2020-06-10 23:04:15.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_reperesentation.py
--rw-rw-rw-   0        0        0     2541 2020-06-10 19:02:29.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_utiles.py
--rw-rw-rw-   0        0        0     4038 2020-06-08 23:56:25.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/ffprobe.py
-drwxrwxrwx   0        0        0        0 2020-06-11 00:01:41.105301 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/tests/
--rw-rw-rw-   0        0        0        0 2020-04-12 16:33:24.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/tests/__init__.py
--rw-rw-rw-   0        0        0     4870 2020-06-10 23:55:09.000000 python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/tests/test_ffmpeg_video_streaming.py
-drwxrwxrwx   0        0        0        0 2020-06-11 00:01:41.134298 python-ffmpeg-video-streaming-0.1.8/python_ffmpeg_video_streaming.egg-info/
--rw-rw-rw-   0        0        0    22749 2020-06-11 00:01:40.000000 python-ffmpeg-video-streaming-0.1.8/python_ffmpeg_video_streaming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      685 2020-06-11 00:01:40.000000 python-ffmpeg-video-streaming-0.1.8/python_ffmpeg_video_streaming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-06-11 00:01:40.000000 python-ffmpeg-video-streaming-0.1.8/python_ffmpeg_video_streaming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2020-06-11 00:01:40.000000 python-ffmpeg-video-streaming-0.1.8/python_ffmpeg_video_streaming.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-06-11 00:01:41.144299 python-ffmpeg-video-streaming-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1104 2020-06-11 00:00:53.000000 python-ffmpeg-video-streaming-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-06-21 19:23:23.936738 python-ffmpeg-video-streaming-0.1.9/
+-rw-rw-rw-   0        0        0    22749 2020-06-21 19:23:23.935739 python-ffmpeg-video-streaming-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    19006 2020-06-10 23:38:09.000000 python-ffmpeg-video-streaming-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2020-06-21 19:23:23.901346 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/
+-rw-rw-rw-   0        0        0      295 2020-04-20 00:29:55.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/__init__.py
+-rw-rw-rw-   0        0        0     6655 2020-05-04 22:24:22.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_clouds.py
+-rw-rw-rw-   0        0        0     3885 2020-06-21 18:56:02.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_command_builder.py
+-rw-rw-rw-   0        0        0     4912 2020-06-21 17:55:25.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_format.py
+-rw-rw-rw-   0        0        0     3730 2020-06-21 17:13:08.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_hls_helper.py
+-rw-rw-rw-   0        0        0     4503 2020-06-21 18:14:34.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_input.py
+-rw-rw-rw-   0        0        0     7313 2020-06-21 18:44:17.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_media.py
+-rw-rw-rw-   0        0        0     4197 2020-06-21 17:11:14.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_media_property.py
+-rw-rw-rw-   0        0        0     3665 2020-06-08 23:50:35.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_process.py
+-rw-rw-rw-   0        0        0     3317 2020-06-21 16:41:00.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_reperesentation.py
+-rw-rw-rw-   0        0        0     2544 2020-06-16 11:31:26.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_utiles.py
+-rw-rw-rw-   0        0        0     4038 2020-06-08 23:56:25.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/ffprobe.py
+drwxrwxrwx   0        0        0        0 2020-06-21 19:23:23.910347 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/tests/
+-rw-rw-rw-   0        0        0        0 2020-04-12 16:33:24.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/tests/__init__.py
+-rw-rw-rw-   0        0        0     4870 2020-06-10 23:55:09.000000 python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/tests/test_ffmpeg_video_streaming.py
+drwxrwxrwx   0        0        0        0 2020-06-21 19:23:23.931342 python-ffmpeg-video-streaming-0.1.9/python_ffmpeg_video_streaming.egg-info/
+-rw-rw-rw-   0        0        0    22749 2020-06-21 19:23:23.000000 python-ffmpeg-video-streaming-0.1.9/python_ffmpeg_video_streaming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2020-06-21 19:23:23.000000 python-ffmpeg-video-streaming-0.1.9/python_ffmpeg_video_streaming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-06-21 19:23:23.000000 python-ffmpeg-video-streaming-0.1.9/python_ffmpeg_video_streaming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2020-06-21 19:23:23.000000 python-ffmpeg-video-streaming-0.1.9/python_ffmpeg_video_streaming.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-06-21 19:23:23.937738 python-ffmpeg-video-streaming-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1104 2020-06-21 19:02:29.000000 python-ffmpeg-video-streaming-0.1.9/setup.py
```

### Comparing `python-ffmpeg-video-streaming-0.1.8/PKG-INFO` & `python-ffmpeg-video-streaming-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ffmpeg-video-streaming
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package media content for online streaming(DASH and HLS) using ffmpeg
 Home-page: https://github.com/aminyazdanpanah/python-ffmpeg-video-streaming
 Author: Amin Yazdanpanah
 Author-email: contact@aminyazdanpanah.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aminyazdanpanah/python-ffmpeg-video-streaming/issues
 Project-URL: Documentation, https://video.aminyazdanpanah.com/python
```

### Comparing `python-ffmpeg-video-streaming-0.1.8/README.md` & `python-ffmpeg-video-streaming-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_clouds.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_clouds.py`

 * *Files identical despite different names*

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_command_builder.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_command_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,17 +40,18 @@
 def _get_dash_stream(key, rep):
     """
     @TODO: add documentation
     """
     args = {
         'map':               0,
         's:v:' + str(key):   rep.size.normalize,
-        'b:v:' + str(key):   rep.bitrate.normalize_video()
+        'b:v:' + str(key):   rep.bitrate.calc_video()
     }
     args.update(_get_audio_bitrate(rep, key))
+    args.update(rep.options)
     return cnv_options_to_args(args)
 
 
 def _dash(dash):
     """
     @TODO: add documentation
     """
@@ -84,20 +85,21 @@
     @TODO: add documentation
     """
     args = hls.format.all
     args.update({
         'hls_list_size':            0,
         'hls_time':                 10,
         'hls_allow_cache':          1,
-        'hls_segment_filename':     "{}/{}_{}p_%04d.{}".format(dirname, name, str(rep.size.height), _hls_seg_ext(hls)),
-        'hls_fmp4_init_filename':   "{}_{}p_init.mp4".format(name, str(rep.size.height)),
+        'hls_segment_filename':     "{}/{}_{}p_%04d.{}".format(dirname, name, rep.size.height, _hls_seg_ext(hls)),
+        'hls_fmp4_init_filename':   "{}_{}p_init.mp4".format(name, rep.size.height),
         's:v':                      rep.size.normalize,
-        'b:v':                      rep.bitrate.normalize_video()
+        'b:v':                      rep.bitrate.calc_video()
     })
     args.update(_get_audio_bitrate(rep))
+    args.update(rep.options)
     args.update({'strict': '-2'})
     args.update(hls.options)
 
     return cnv_options_to_args(args) + ["{}/{}_{}p.m3u8".format(dirname, name, str(rep.size.height))]
 
 
 def _hls(hls):
```

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_format.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 
 class H264(Format):
     def __init__(self, video: str = "libx264", audio: str = 'aac', **codec_options):
         """
         @TODO: add documentation
         """
-        videos = ['libx264', 'h264', 'h264_afm', 'h264_cuvid']
+        videos = ['libx264', 'h264', 'h264_afm', 'h264_nvenc']
         audios = ['copy', 'aac', 'libvo_aacenc', 'libfaac', 'libmp3lame', 'libfdk_aac']
 
         super(H264, self).__init__(_verify_codecs(video, videos), _verify_codecs(audio, audios), **codec_options)
 
     def multiply(self) -> int:
         return MULTIPLY_BY_TWO
```

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_hls_helper.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_hls_helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 :email: contact@aminyazdanpanah.com
 :license: MIT, see LICENSE for more details.
 """
 import os
 import uuid
 from secrets import token_bytes, token_hex
 
-from ffmpeg_streaming._utiles import mkdir
+from ffmpeg_streaming._utiles import mkdir, get_path_info
 
 
 class HLSKeyInfoFile:
     def __init__(self, key_info_file_path: str, path: str, url: str, period: int = 0, needle: str = '', length: int = 16):
         """
         @TODO: add documentation
         """
@@ -28,67 +28,86 @@
         self.length = length
         self.url = self.c_url = url
         self.path = self.c_path = path
         mkdir(os.path.dirname(path))
         self.key_info_file_path = key_info_file_path
 
     def __str__(self):
+        """
+        @TODO: add documentation
+        """
         self.generate()
         return self.key_info_file_path
 
     def generate(self):
+        """
+        @TODO: add documentation
+        """
         self.generate_key()
         self.update_key_info_file()
 
     def generate_key(self):
+        """
+        @TODO: add documentation
+        """
         with open(self.path, 'wb') as key:
             key.write(token_bytes(self.length))
 
     def update_key_info_file(self):
+        """
+        @TODO: add documentation
+        """
         with open(self.key_info_file_path, 'w') as key_info_file:
             key_info_file.write("\n".join([self.url, self.path, token_hex(self.length)]))
 
     def update_suffix(self):
+        """
+        @TODO: add documentation
+        """
         unique = uuid.uuid4()
         self.path = self.c_path + "-" + str(unique)
         self.url = self.c_url + "-" + str(unique)
 
     def rotate_key(self, line: str):
+        """
+        @TODO: add documentation
+        """
         if self.needle in line and line not in self.segments:
             self.segments.append(line)
             if len(self.segments) % self.period == 0:
                 self.update_suffix()
                 self.generate()
 
 
 def stream_info(rep) -> list:
-    # @TODO: add custom stream info
+    """
+    @TODO: add documentation
+    """
     tag = '#EXT-X-STREAM-INF:'
     info = [
-        'BANDWIDTH=' + str(rep.bitrate.normalize_video(False)),
-        'RESOLUTION=' + rep.size.normalize,
-        'NAME="' + str(rep.size.height) + '"'
+        f'BANDWIDTH={rep.bitrate.calc_overall}',
+        f'RESOLUTION={rep.size.normalize}',
+        f'NAME="{rep.size.height}"'
     ]
-    
-    return [tag + ",".join(info)]
+    custom = rep.options.pop('stream_info', [])
+
+    return [tag + ",".join(info + custom)]
 
 
 class HLSMasterPlaylist:
     def __init__(self, media):
         """
         @TODO: add documentation
         """
         self.media = media
-        self.path = media.output
 
     @classmethod
     def generate(cls, media, path=None):
         if path is None:
-            path = os.path.join(os.path.dirname(media.output_), os.path.basename(media.output_).split('.')[0] + '.m3u8')
-
+            path = "{}.m3u8".format(os.path.join(*get_path_info(media.output_)))
         with open(path, 'w', encoding='utf-8') as playlist:
             playlist.write(cls(media)._content())
 
     def _content(self) -> str:
         """
         @TODO: add documentation
         """
@@ -96,12 +115,18 @@
 
         for rep in self.media.reps:
             content += stream_info(rep) + self.stream_path(rep)
 
         return "\n".join(content)
 
     def _get_version(self) -> list:
-        version = "7" if hasattr(self.media, 'fragmented_mp4') else "3"
+        """
+        @TODO: add documentation
+        """
+        version = "7" if self.media.options.get('hls_segment_type', '') == 'fmp4' else "3"
         return ['#EXT-X-VERSION:' + version]
 
     def stream_path(self, rep):
-        return [str(os.path.basename(self.media.output_).split('.')[0]) + "_" + str(rep.size.height) + "p.m3u8"]
+        """
+        @TODO: add documentation
+        """
+        return ["{}_{}p.m3u8".format(os.path.basename(self.media.output_).split('.')[0], rep.size.height)]
```

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_input.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_input.py`

 * *Files identical despite different names*

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_media.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_media.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 """
 import abc
 import os
 import shutil
 import tempfile
 import atexit
 import asyncio
+import copy
 
 from ._clouds import CloudManager
 from ._command_builder import command_builder
 from ._format import Format
 from ._hls_helper import HLSKeyInfoFile, HLSMasterPlaylist
 from ._process import Process
 from ._reperesentation import Representation, AutoRep
@@ -209,17 +210,17 @@
 class Media(object):
     def __init__(self, _inputs):
         """
         @TODO: add documentation
         """
         self.inputs = _inputs
 
-        first_options = dict(_inputs.inputs[0])
-        self.input = first_options.get('i', None)
-        self.input_temp = first_options.get('is_tmp', False)
+        first_input = dict(copy.deepcopy(_inputs.inputs[0]))
+        self.input = first_input.get('i', None)
+        self.input_temp = first_input.get('is_tmp', False)
 
     def hls(self, _format: Format, **hls_options):
         """
         @TODO: add documentation
         """
         return HLS(self, _format, **hls_options)
```

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_media_property.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_media_property.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,39 +58,31 @@
     @property
     def audio(self):
         """
         @TODO: add documentation
         """
         return cnv_bitrate(self.audio_, self.type) if self.audio_ is not None else 'copy'
 
-    def normalize_video(self, convert: bool = True):
+    def calc_video(self, convert: bool = True):
         """
         @TODO: add documentation
         """
         if self.video_ is not None and self.video_ != 0:
             val = self.video_
         else:
             val = int(self.overall_ * OVERALL_TO_VIDEO_COEFFICIENT)
 
         return cnv_bitrate(val, self.type) if convert else val
 
     @property
-    def max_rate(self):
+    def calc_overall(self):
         """
         @TODO: add documentation
         """
-        return cnv_bitrate(int(self.normalize_video(False) * MAX_RATE_COEFFICIENT), self.type)
-
-    @property
-    def buffer_size(self):
-        """
-        @TODO: add documentation
-        """
-
-        return cnv_bitrate(int(self.kwargs.get('buffer_size', BUFFER_SIZE)), self.type)
+        return self.overall_ if self.overall_ is not None else self.video_ + self.audio_
 
 
 def multiple_up(value, multiple):
     while 0 != value % multiple:
         value += 1
 
     return value
```

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_process.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_process.py`

 * *Files identical despite different names*

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_reperesentation.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_reperesentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 from ._format import Format
 from ._media_property import Size, Bitrate
 
 MINIMUM_BITRATE = 65536
 
 
 class Representation:
-    def __init__(self, size: Size, bitrate: Bitrate):
+    def __init__(self, size: Size, bitrate: Bitrate, **options):
         """
         @TODO: add documentation
         """
         self.size = size
         self.bitrate = bitrate
+        self.options = options
 
 
 def min_bitrate(bitrate: int) -> int:
     """
     @TODO: add documentation
     """
     if bitrate < MINIMUM_BITRATE:
```

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/_utiles.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/_utiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     return int(h) * 3600 + int(m) * 60 + int(s)
 
 
 def get_time(key, string, default):
     """
     @TODO: add documentation
     """
-    time = re.search('(?<=' + key + ')\w+:\w+:\w+', string)
+    time = re.search('(?<={})\w+:\w+:\w+'.format(key), string)
     return convert_to_sec(time.group(0)) if time else default
 
 
 def deprecated(func):
     """
     @TODO: add documentation
     """
```

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/ffprobe.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/ffprobe.py`

 * *Files identical despite different names*

### Comparing `python-ffmpeg-video-streaming-0.1.8/ffmpeg_streaming/tests/test_ffmpeg_video_streaming.py` & `python-ffmpeg-video-streaming-0.1.9/ffmpeg_streaming/tests/test_ffmpeg_video_streaming.py`

 * *Files identical despite different names*

### Comparing `python-ffmpeg-video-streaming-0.1.8/python_ffmpeg_video_streaming.egg-info/PKG-INFO` & `python-ffmpeg-video-streaming-0.1.9/python_ffmpeg_video_streaming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ffmpeg-video-streaming
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package media content for online streaming(DASH and HLS) using ffmpeg
 Home-page: https://github.com/aminyazdanpanah/python-ffmpeg-video-streaming
 Author: Amin Yazdanpanah
 Author-email: contact@aminyazdanpanah.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aminyazdanpanah/python-ffmpeg-video-streaming/issues
 Project-URL: Documentation, https://video.aminyazdanpanah.com/python
```

### Comparing `python-ffmpeg-video-streaming-0.1.8/python_ffmpeg_video_streaming.egg-info/SOURCES.txt` & `python-ffmpeg-video-streaming-0.1.9/python_ffmpeg_video_streaming.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-ffmpeg-video-streaming-0.1.8/setup.py` & `python-ffmpeg-video-streaming-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="python-ffmpeg-video-streaming",
-    version="0.1.8",
+    version="0.1.9",
     author="Amin Yazdanpanah",
     author_email="contact@aminyazdanpanah.com",
     description="Package media content for online streaming(DASH and HLS) using ffmpeg",
     long_description=long_description,
     project_urls={
         "Bug Tracker": "https://github.com/aminyazdanpanah/python-ffmpeg-video-streaming/issues",
         "Documentation": "https://video.aminyazdanpanah.com/python",
```

