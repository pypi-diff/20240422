# Comparing `tmp/asyffmpeg-0.2.3.tar.gz` & `tmp/asyffmpeg-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyffmpeg-0.2.3.tar", last modified: Fri Apr 19 15:06:50 2024, max compression
+gzip compressed data, was "asyffmpeg-0.2.4.tar", last modified: Mon Apr 22 08:30:40 2024, max compression
```

## Comparing `asyffmpeg-0.2.3.tar` & `asyffmpeg-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 15:06:50.572956 asyffmpeg-0.2.3/
--rw-rw-rw-   0        0        0     2130 2024-04-19 15:06:50.567958 asyffmpeg-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1683 2024-04-19 15:06:03.000000 asyffmpeg-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 15:06:50.558411 asyffmpeg-0.2.3/asyffmpeg/
--rw-rw-rw-   0        0        0    11817 2024-04-19 15:00:50.000000 asyffmpeg-0.2.3/asyffmpeg/__init__.py
--rw-rw-rw-   0        0        0     1140 2024-04-18 17:06:39.000000 asyffmpeg-0.2.3/asyffmpeg/statistic.py
--rw-rw-rw-   0        0        0      997 2024-04-18 16:54:54.000000 asyffmpeg-0.2.3/asyffmpeg/tempf.py
--rw-rw-rw-   0        0        0     2169 2024-04-18 16:53:26.000000 asyffmpeg-0.2.3/asyffmpeg/util.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:06:50.566960 asyffmpeg-0.2.3/asyffmpeg.egg-info/
--rw-rw-rw-   0        0        0     2130 2024-04-19 15:06:50.000000 asyffmpeg-0.2.3/asyffmpeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-04-19 15:06:50.000000 asyffmpeg-0.2.3/asyffmpeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 15:06:50.000000 asyffmpeg-0.2.3/asyffmpeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-19 15:06:50.000000 asyffmpeg-0.2.3/asyffmpeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 15:06:50.000000 asyffmpeg-0.2.3/asyffmpeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 15:06:50.572956 asyffmpeg-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      654 2024-04-19 15:06:36.000000 asyffmpeg-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:30:40.250755 asyffmpeg-0.2.4/
+-rw-rw-rw-   0        0        0     2130 2024-04-22 08:30:40.245766 asyffmpeg-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1683 2024-04-19 15:06:03.000000 asyffmpeg-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 08:30:40.218838 asyffmpeg-0.2.4/asyffmpeg/
+-rw-rw-rw-   0        0        0    12224 2024-04-19 17:59:19.000000 asyffmpeg-0.2.4/asyffmpeg/__init__.py
+-rw-rw-rw-   0        0        0     1140 2024-04-18 17:06:39.000000 asyffmpeg-0.2.4/asyffmpeg/statistic.py
+-rw-rw-rw-   0        0        0      997 2024-04-18 16:54:54.000000 asyffmpeg-0.2.4/asyffmpeg/tempf.py
+-rw-rw-rw-   0        0        0     2169 2024-04-18 16:53:26.000000 asyffmpeg-0.2.4/asyffmpeg/util.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:30:40.240781 asyffmpeg-0.2.4/asyffmpeg.egg-info/
+-rw-rw-rw-   0        0        0     2130 2024-04-22 08:30:39.000000 asyffmpeg-0.2.4/asyffmpeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-04-22 08:30:39.000000 asyffmpeg-0.2.4/asyffmpeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 08:30:39.000000 asyffmpeg-0.2.4/asyffmpeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-22 08:30:39.000000 asyffmpeg-0.2.4/asyffmpeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-22 08:30:39.000000 asyffmpeg-0.2.4/asyffmpeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 08:30:40.252763 asyffmpeg-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      654 2024-04-19 18:02:00.000000 asyffmpeg-0.2.4/setup.py
```

### Comparing `asyffmpeg-0.2.3/PKG-INFO` & `asyffmpeg-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyffmpeg
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library for asynchronous operation with FFmpeg, providing the ability to track events such as start, end, and encoding progress.
 Home-page: https://github.com/drhspfn/asyffmpeg
 Author: drhspfn
 Author-email: jenya.gsta@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles
```

### Comparing `asyffmpeg-0.2.3/README.md` & `asyffmpeg-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.2.3/asyffmpeg/__init__.py` & `asyffmpeg-0.2.4/asyffmpeg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             ffmpeg.args({'vf': 'scale=1920:1080', 'codec:a': 'aac'})
             ffmpeg.on_event('progress', progress)
             await ffmpeg.run()
 
         asyncio.run(main())
         ```
     """
-    def __init__(self, debug:bool=False, logger:logging.Logger=None) -> None:
+    def __init__(self, debug:bool=False, logger:logging.Logger=None, id:str=None) -> None:
         """
         Initializes an instance of the AsyFFmpeg class.
 
         Args:
             debug (`bool, optional`): Whether debugging is enabled. Defaults to False.
             logger (`logging.Logger, optional`): The logger object for logging debug messages. Defaults to None.
         """
@@ -50,15 +50,15 @@
         self._args: Dict[str, str] = {}
 
         self.__events:Dict[str, Callable[[None], Awaitable[None]]] = {}
 
         self.__start_time:datetime = 0
 
         self.__preffix = "AsyFFmpeg"
-
+        self.__id = id
 
     def _debug(self, data:str) -> None:
         """
         Logs debug information if debugging is enabled.
 
         This method logs debug information to the specified logger (if available) or prints it to the console
         with a custom prefix. Debugging must be enabled for this method to log information. If no logger is provided,
@@ -70,42 +70,49 @@
         Returns:
             `None`
         """
         if self.__debug:
             if self.__logger:
                 self.__logger.debug(data)
             else:
-                print(f'[{self.__preffix}]: {data}')
+                if self.__id:
+                    print(f'[{self.__preffix}-{self.__id}]: {data}')
+                else:
+                    print(f'[{self.__preffix}]: {data}')
+
 
-    
     def __build_command(self) -> None:
         """
         Builds the FFmpeg command based on input parameters.
 
         This method constructs the FFmpeg command by assembling the input file, output file, 
         and additional arguments into a list of command-line arguments. If additional arguments 
         are provided, they are included in the command along with their corresponding values.
         If the value for an argument is `None`, only the key will be included in the command.
 
         Returns:
             `None`
         """
 
-        args = ['-y', '-i', self._input if self._input.strip().find(" ") == -1 else f'"{self._input}"']
+        # args = ['-y', '-i', self._input if self._input.strip().find(" ") == -1 else f'"{self._input}"']
+        args = ['-y', '-i', self._input]
 
         if self._args:
             for key, value in self._args.items():
                 if value is not None:
                     args.extend(['-' + key, value])
                 else:
                     args.append('-' + key)
 
         args.append(self._output)
         self._args = args
 
+    def set_id(self, id:str):
+        self.__id = id
+
     def add_arg(self, arg_key: str, arg_value: str = None) -> None:
         """
         Adds an argument to the FFmpeg command.
 
         This method adds an argument to the FFmpeg command with the specified key and value.
 
         Args:
@@ -196,20 +203,20 @@
                         remaining_time = timedelta(seconds=(elapsed_time.total_seconds() / _progress)) - elapsed_time
                     else:
                         remaining_time = timedelta()
                        
 
                     self._debug("Progress intercepted...")
                     await self.__events['progress'](_progress, elapsed_time, remaining_time, 
-                                            progress.frame, not progress.progress, progress.bitrate)
+                                            progress.frame, not progress.progress, progress.bitrate, self.__id)
 
                     if progress.progress is False:
                         self._debug("Encoding completed...")
                         if self.__events.get('end', None):
-                            await self.__events['end'](datetime.now() - self.__start_time)
+                            await self.__events['end'](datetime.now() - self.__start_time, self.__id)
 
                         await progress_file.close()
                         break
             await asyncio.sleep(1)
 
     async def _prepare(self) -> None:
         """
@@ -280,34 +287,38 @@
         self.__build_command()
         self.__start_time = datetime.now()
         async with TempFile() as progress_file_path:
             
             self._debug("Encoding started...")
             async def _run(args_list, f_path):
                 if self.__events.get('start', None):
-                    await self.__events['start'](self._input, self._output)
+                    await self.__events['start'](self._input, self._output, self.__id)
 
                 cmd = ["ffmpeg"] + [str(var) for var in args_list]
+                
+                
                 if self.file_duration != -1:
                     cmd +=  ["-progress", f_path]
                 
+                print(cmd)
+
                 proc = await asyncio.create_subprocess_exec(
                     *cmd,
                     stdout=asyncio.subprocess.PIPE,
                     stderr=asyncio.subprocess.PIPE
                 )
                 stdout, stderr = await proc.communicate()
                 # print(stdout.decode())
                 # stderr.decode()
                 
                 
 
                 if proc.returncode != 0:
                     self._debug(f"FFmpeg process exited with non-zero code: {proc.returncode}")
-
+                    self._debug(stderr.decode())
                 if self.__events.get('end', None):
                     await self.__events['end'](datetime.now() - self.__start_time)
                 
                 return stdout, stderr
 
             
             tasks = []
```

### Comparing `asyffmpeg-0.2.3/asyffmpeg/statistic.py` & `asyffmpeg-0.2.4/asyffmpeg/statistic.py`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.2.3/asyffmpeg/tempf.py` & `asyffmpeg-0.2.4/asyffmpeg/tempf.py`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.2.3/asyffmpeg/util.py` & `asyffmpeg-0.2.4/asyffmpeg/util.py`

 * *Files identical despite different names*

### Comparing `asyffmpeg-0.2.3/asyffmpeg.egg-info/PKG-INFO` & `asyffmpeg-0.2.4/asyffmpeg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyffmpeg
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library for asynchronous operation with FFmpeg, providing the ability to track events such as start, end, and encoding progress.
 Home-page: https://github.com/drhspfn/asyffmpeg
 Author: drhspfn
 Author-email: jenya.gsta@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: aiofiles
```

### Comparing `asyffmpeg-0.2.3/setup.py` & `asyffmpeg-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='asyffmpeg',
-    version='0.2.3',
+    version='0.2.4',
     packages=find_packages(),
     install_requires=[
         'aiofiles',
         'ffprobe-python',
     ],
     author='drhspfn',
     author_email='jenya.gsta@gmail.com',
```

