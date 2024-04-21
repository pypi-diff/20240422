# Comparing `tmp/foamlib-0.3.4.tar.gz` & `tmp/foamlib-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.3.4.tar", last modified: Sun Apr 21 19:24:40 2024, max compression
+gzip compressed data, was "foamlib-0.3.5.tar", last modified: Sun Apr 21 23:11:29 2024, max compression
```

## Comparing `foamlib-0.3.4.tar` & `foamlib-0.3.5.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:24:40.089274 foamlib-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-21 19:24:35.000000 foamlib-0.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-21 19:24:40.085273 foamlib-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-21 19:24:35.000000 foamlib-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:24:40.081273 foamlib-0.3.4/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20567 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:24:40.085273 foamlib-0.3.4/foamlib/_files/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_files/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:24:35.000000 foamlib-0.3.4/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:24:40.085273 foamlib-0.3.4/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-21 19:24:40.000000 foamlib-0.3.4/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-21 19:24:40.000000 foamlib-0.3.4/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:24:40.000000 foamlib-0.3.4/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-21 19:24:40.000000 foamlib-0.3.4/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 19:24:40.000000 foamlib-0.3.4/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-21 19:24:35.000000 foamlib-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:24:40.089274 foamlib-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:11:29.282135 foamlib-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-21 23:11:24.000000 foamlib-0.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-21 23:11:29.282135 foamlib-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-21 23:11:24.000000 foamlib-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:11:29.278135 foamlib-0.3.5/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-21 23:11:24.000000 foamlib-0.3.5/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-04-21 23:11:24.000000 foamlib-0.3.5/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:11:29.282135 foamlib-0.3.5/foamlib/_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-21 23:11:24.000000 foamlib-0.3.5/foamlib/_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-21 23:11:24.000000 foamlib-0.3.5/foamlib/_files/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-21 23:11:24.000000 foamlib-0.3.5/foamlib/_files/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-21 23:11:24.000000 foamlib-0.3.5/foamlib/_files/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-21 23:11:24.000000 foamlib-0.3.5/foamlib/_files/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-21 23:11:24.000000 foamlib-0.3.5/foamlib/_files/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-21 23:11:24.000000 foamlib-0.3.5/foamlib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 23:11:24.000000 foamlib-0.3.5/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 23:11:29.282135 foamlib-0.3.5/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-21 23:11:29.000000 foamlib-0.3.5/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-21 23:11:29.000000 foamlib-0.3.5/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 23:11:29.000000 foamlib-0.3.5/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-21 23:11:29.000000 foamlib-0.3.5/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 23:11:29.000000 foamlib-0.3.5/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-21 23:11:24.000000 foamlib-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 23:11:29.282135 foamlib-0.3.5/setup.cfg
```

### Comparing `foamlib-0.3.4/LICENSE.txt` & `foamlib-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.4/PKG-INFO` & `foamlib-0.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -54,19 +54,19 @@
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/foamlib)](https://pypi.org/project/foamlib/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/foamlib)](https://pypi.org/project/foamlib/)
 [![Docker image](https://img.shields.io/badge/docker%20image-gerlero%2Ffoamlib-informational)](https://hub.docker.com/r/gerlero/foamlib/)
 
 **foamlib** provides a simple, modern and ergonomic Python interface for interacting with [OpenFOAM](https://www.openfoam.com).
 
-It offers the following classes (among a few others):
+It offers the following classes:
 
+* [`FoamFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFile) (and [`FoamFieldFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFieldFile)): read-write access to OpenFOAM configuration and field files as if they were Python `dict`s, using `foamlib`'s own parser. Supports both ASCII and binary field formats.
 * [`FoamCase`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamCase): a class for manipulating, executing and accessing the results of OpenFOAM cases.
 * [`AsyncFoamCase`](https://foamlib.readthedocs.io/en/stable/#foamlib.AsyncFoamCase): variant of `FoamCase` with asynchronous methods for running multiple cases at once.
-* [`FoamFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFile): read-write access to OpenFOAM configuration and field files as if they were Python `dict`s.
 
 ## Get started
 
 ### Install
 
 Install with [pip](https://pypi.org/project/pip/):
 
@@ -126,10 +126,20 @@
     my_pitz_async = AsyncFoamCase(my_pitz)
 
     await my_pitz_async.run()
 
 asyncio.run(run_case())
 ```
 
+### Parse a field using the [`FoamFieldFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFieldFile) class directly
+
+```python
+from foamlib import FoamFieldFile
+
+U = FoamFieldFile(Path(my_pitz) / "0/U")
+
+print(U.internal_field)
+```
+
 ## Documentation
 
 For more information, check out the [documentation](https://foamlib.readthedocs.io/).
```

### Comparing `foamlib-0.3.4/README.md` & `foamlib-0.3.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/foamlib)](https://pypi.org/project/foamlib/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/foamlib)](https://pypi.org/project/foamlib/)
 [![Docker image](https://img.shields.io/badge/docker%20image-gerlero%2Ffoamlib-informational)](https://hub.docker.com/r/gerlero/foamlib/)
 
 **foamlib** provides a simple, modern and ergonomic Python interface for interacting with [OpenFOAM](https://www.openfoam.com).
 
-It offers the following classes (among a few others):
+It offers the following classes:
 
+* [`FoamFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFile) (and [`FoamFieldFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFieldFile)): read-write access to OpenFOAM configuration and field files as if they were Python `dict`s, using `foamlib`'s own parser. Supports both ASCII and binary field formats.
 * [`FoamCase`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamCase): a class for manipulating, executing and accessing the results of OpenFOAM cases.
 * [`AsyncFoamCase`](https://foamlib.readthedocs.io/en/stable/#foamlib.AsyncFoamCase): variant of `FoamCase` with asynchronous methods for running multiple cases at once.
-* [`FoamFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFile): read-write access to OpenFOAM configuration and field files as if they were Python `dict`s.
 
 ## Get started
 
 ### Install
 
 Install with [pip](https://pypi.org/project/pip/):
 
@@ -79,10 +79,20 @@
     my_pitz_async = AsyncFoamCase(my_pitz)
 
     await my_pitz_async.run()
 
 asyncio.run(run_case())
 ```
 
+### Parse a field using the [`FoamFieldFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFieldFile) class directly
+
+```python
+from foamlib import FoamFieldFile
+
+U = FoamFieldFile(Path(my_pitz) / "0/U")
+
+print(U.internal_field)
+```
+
 ## Documentation
 
 For more information, check out the [documentation](https://foamlib.readthedocs.io/).
```

### Comparing `foamlib-0.3.4/foamlib/_cases.py` & `foamlib-0.3.5/foamlib/_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 import multiprocessing
-import os
 import shutil
 import sys
 from contextlib import asynccontextmanager
 from pathlib import Path
 from typing import (
     Optional,
     Union,
@@ -13,21 +12,20 @@
 
 if sys.version_info >= (3, 9):
     from collections.abc import (
         AsyncGenerator,
         Callable,
         Collection,
         Iterator,
-        Mapping,
         Sequence,
         Set,
     )
 else:
     from typing import AbstractSet as Set
-    from typing import AsyncGenerator, Callable, Collection, Iterator, Mapping, Sequence
+    from typing import AsyncGenerator, Callable, Collection, Iterator, Sequence
 
 import aioshutil
 
 from ._files import FoamFieldFile, FoamFile
 from ._util import is_sequence, run_process, run_process_async
 
 
@@ -83,15 +81,15 @@
         def __len__(self) -> int:
             return len(list(iter(self)))
 
         def __fspath__(self) -> str:
             return str(self.path)
 
         def __repr__(self) -> str:
-            return f"{type(self).__name__}('{self.path}')"
+            return f"{type(self).__qualname__}('{self.path}')"
 
         def __str__(self) -> str:
             return str(self.path)
 
     @property
     def _times(self) -> Sequence["FoamCaseBase.TimeDirectory"]:
         times = []
@@ -199,20 +197,14 @@
         elif parallel is not False and (
             run_parallel.is_file() or all_run_parallel.is_file()
         ):
             return run_parallel if run_parallel.is_file() else all_run_parallel
         else:
             return None
 
-    def _env(self) -> Mapping[str, str]:
-        """Return the environment variables for this case."""
-        env = os.environ.copy()
-        env["PWD"] = str(self.path)
-        return env
-
     def _parallel_cmd(
         self, cmd: Union[Sequence[Union[str, Path]], str, Path]
     ) -> Union[Sequence[Union[str, Path]], str]:
         if not is_sequence(cmd):
             return f"mpiexec -np {self._nprocessors} {cmd} -parallel"
         else:
             return [
@@ -294,15 +286,15 @@
         """The turbulenceProperties file."""
         return self.file("constant/turbulenceProperties")
 
     def __fspath__(self) -> str:
         return str(self.path)
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}('{self.path}')"
+        return f"{type(self).__qualname__}('{self.path}')"
 
     def __str__(self) -> str:
         return str(self.path)
 
 
 class FoamCase(FoamCaseBase):
     """
@@ -355,15 +347,14 @@
             if parallel:
                 cmd = self._parallel_cmd(cmd)
 
             run_process(
                 cmd,
                 check=check,
                 cwd=self.path,
-                env=self._env(),
             )
         else:
             script_path = self._run_script(parallel=parallel) if script else None
 
             if script_path is not None:
                 return self.run([script_path], check=check)
 
@@ -518,15 +509,14 @@
                 cmd = self._parallel_cmd(cmd)
 
             async with self._cpus(cpus):
                 await run_process_async(
                     cmd,
                     check=check,
                     cwd=self.path,
-                    env=self._env(),
                 )
         else:
             script_path = self._run_script(parallel=parallel) if script else None
 
             if script_path is not None:
                 if cpus is None:
                     if self._nprocessors > 0:
```

### Comparing `foamlib-0.3.4/foamlib/_files/_base.py` & `foamlib-0.3.5/foamlib/_files/_base.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.4/foamlib/_files/_io.py` & `foamlib-0.3.5/foamlib/_files/_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,8 +69,8 @@
         if not self.__defer_io:
             self.path.write_bytes(contents)
             self.__dirty = False
         else:
             self.__dirty = True
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}('{self.path}')"
+        return f"{type(self).__qualname__}('{self.path}')"
```

### Comparing `foamlib-0.3.4/foamlib/_files/_parsing.py` & `foamlib-0.3.5/foamlib/_files/_parsing.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.3.4/foamlib/_util.py` & `foamlib-0.3.5/foamlib/_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import os
 import subprocess
 import sys
 from pathlib import Path
 from typing import Any, Optional, Union
 from warnings import warn
 
 if sys.version_info >= (3, 9):
@@ -43,66 +44,73 @@
 ) -> None:
     if retcode != 0:
         raise CalledProcessError(retcode, cmd, None, stderr)
     elif stderr:
         warn(f"Command {cmd} printed to stderr.\n{stderr}", CalledProcessWarning)
 
 
+def _env(cwd: Optional[Union[str, Path]] = None) -> Optional[Mapping[str, str]]:
+    if cwd is not None:
+        env = os.environ.copy()
+        env["PWD"] = str(cwd)
+        return env
+    else:
+        return None
+
+
 def run_process(
     cmd: Union[Sequence[Union[str, Path]], str, Path],
     *,
     check: bool = True,
     cwd: Union[None, str, Path] = None,
-    env: Union[None, Mapping[str, str]] = None,
 ) -> None:
     shell = not is_sequence(cmd)
 
     if sys.version_info < (3, 8):
         if shell:
             cmd = str(cmd)
         else:
             cmd = (str(arg) for arg in cmd)
 
     proc = subprocess.run(
         cmd,
         cwd=cwd,
-        env=env,
-        stdout=subprocess.DEVNULL,
+        env=_env(cwd),
+        stdout=None,
         stderr=subprocess.PIPE if check else subprocess.DEVNULL,
         text=True,
         shell=shell,
     )
 
     if check:
         _check(proc.returncode, cmd, proc.stderr)
 
 
 async def run_process_async(
     cmd: Union[Sequence[Union[str, Path]], str, Path],
     *,
     check: bool = True,
     cwd: Union[None, str, Path] = None,
-    env: Union[None, Mapping[str, str]] = None,
 ) -> None:
     if not is_sequence(cmd):
         proc = await asyncio.create_subprocess_shell(
             str(cmd),
             cwd=cwd,
-            env=env,
+            env=_env(cwd),
             stdout=asyncio.subprocess.DEVNULL,
             stderr=asyncio.subprocess.PIPE if check else asyncio.subprocess.DEVNULL,
         )
 
     else:
         if sys.version_info < (3, 8):
             cmd = (str(arg) for arg in cmd)
         proc = await asyncio.create_subprocess_exec(
             *cmd,
             cwd=cwd,
-            env=env,
+            env=_env(cwd),
             stdout=asyncio.subprocess.DEVNULL,
             stderr=asyncio.subprocess.PIPE if check else asyncio.subprocess.DEVNULL,
         )
 
     stdout, stderr = await proc.communicate()
 
     assert stdout is None
```

### Comparing `foamlib-0.3.4/foamlib.egg-info/PKG-INFO` & `foamlib-0.3.5/foamlib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -54,19 +54,19 @@
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI](https://img.shields.io/pypi/v/foamlib)](https://pypi.org/project/foamlib/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/foamlib)](https://pypi.org/project/foamlib/)
 [![Docker image](https://img.shields.io/badge/docker%20image-gerlero%2Ffoamlib-informational)](https://hub.docker.com/r/gerlero/foamlib/)
 
 **foamlib** provides a simple, modern and ergonomic Python interface for interacting with [OpenFOAM](https://www.openfoam.com).
 
-It offers the following classes (among a few others):
+It offers the following classes:
 
+* [`FoamFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFile) (and [`FoamFieldFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFieldFile)): read-write access to OpenFOAM configuration and field files as if they were Python `dict`s, using `foamlib`'s own parser. Supports both ASCII and binary field formats.
 * [`FoamCase`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamCase): a class for manipulating, executing and accessing the results of OpenFOAM cases.
 * [`AsyncFoamCase`](https://foamlib.readthedocs.io/en/stable/#foamlib.AsyncFoamCase): variant of `FoamCase` with asynchronous methods for running multiple cases at once.
-* [`FoamFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFile): read-write access to OpenFOAM configuration and field files as if they were Python `dict`s.
 
 ## Get started
 
 ### Install
 
 Install with [pip](https://pypi.org/project/pip/):
 
@@ -126,10 +126,20 @@
     my_pitz_async = AsyncFoamCase(my_pitz)
 
     await my_pitz_async.run()
 
 asyncio.run(run_case())
 ```
 
+### Parse a field using the [`FoamFieldFile`](https://foamlib.readthedocs.io/en/stable/#foamlib.FoamFieldFile) class directly
+
+```python
+from foamlib import FoamFieldFile
+
+U = FoamFieldFile(Path(my_pitz) / "0/U")
+
+print(U.internal_field)
+```
+
 ## Documentation
 
 For more information, check out the [documentation](https://foamlib.readthedocs.io/).
```

### Comparing `foamlib-0.3.4/pyproject.toml` & `foamlib-0.3.5/pyproject.toml`

 * *Files identical despite different names*

