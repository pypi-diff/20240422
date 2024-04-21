# Comparing `tmp/botl-110.tar.gz` & `tmp/botl-111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botl-110.tar", last modified: Fri Apr 19 12:06:46 2024, max compression
+gzip compressed data, was "botl-111.tar", last modified: Sun Apr 21 22:04:11 2024, max compression
```

## Comparing `botl-110.tar` & `botl-111.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-19 12:06:46.154775 botl-110/
--rw-r--r--   0 bart      (1000) bart      (1000)     3961 2024-04-19 12:06:46.154775 botl-110/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     3438 2024-04-19 11:31:35.000000 botl-110/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-19 12:06:46.150776 botl-110/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1000)     2261 2024-04-19 12:00:28.000000 botl-110/bin/botl
--rwxr-xr-x   0 bart      (1000) bart      (1000)     4474 2024-04-19 11:54:20.000000 botl-110/bin/botlbot
--rwxr-xr-x   0 bart      (1000) bart      (1000)     2384 2024-04-19 11:31:26.000000 botl-110/bin/botld
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-19 12:06:46.150776 botl-110/botl/
--rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-04-19 11:09:23.000000 botl-110/botl/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1364 2024-04-19 11:09:23.000000 botl-110/botl/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3873 2024-04-19 11:09:23.000000 botl-110/botl/client.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1922 2024-04-19 11:09:23.000000 botl-110/botl/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)      230 2024-04-19 11:09:23.000000 botl-110/botl/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1089 2024-04-19 11:09:23.000000 botl-110/botl/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)      766 2024-04-19 11:09:23.000000 botl-110/botl/event.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1930 2024-04-19 11:09:23.000000 botl-110/botl/find.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1362 2024-04-19 11:09:23.000000 botl-110/botl/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-19 12:06:46.154775 botl-110/botl/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      500 2024-04-19 11:35:02.000000 botl-110/botl/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      211 2024-04-19 11:11:55.000000 botl-110/botl/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      403 2024-04-19 11:13:15.000000 botl-110/botl/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      425 2024-04-19 11:13:31.000000 botl-110/botl/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      834 2024-04-19 11:13:58.000000 botl-110/botl/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17621 2024-04-19 11:25:12.000000 botl-110/botl/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      776 2024-04-19 11:15:36.000000 botl-110/botl/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)      371 2024-04-19 11:36:24.000000 botl-110/botl/modules/man.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3552 2024-04-19 11:16:02.000000 botl-110/botl/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17081 2024-04-19 11:16:31.000000 botl-110/botl/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)      240 2024-04-19 11:16:41.000000 botl-110/botl/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2400 2024-04-19 11:16:52.000000 botl-110/botl/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)    11001 2024-04-19 11:12:04.000000 botl-110/botl/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2761 2024-04-19 11:19:37.000000 botl-110/botl/modules/rst.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1184 2024-04-19 11:17:55.000000 botl-110/botl/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1038 2024-04-19 11:18:07.000000 botl-110/botl/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5130 2024-04-19 11:18:37.000000 botl-110/botl/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2933 2024-04-19 11:18:56.000000 botl-110/botl/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5799 2024-04-19 11:19:09.000000 botl-110/botl/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6155 2024-04-19 11:09:23.000000 botl-110/botl/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1814 2024-04-19 11:07:31.000000 botl-110/botl/parser.py
--rw-r--r--   0 bart      (1000) bart      (1000)      752 2024-04-19 11:09:23.000000 botl-110/botl/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)      275 2024-04-19 11:09:23.000000 botl-110/botl/repeater.py
--rw-r--r--   0 bart      (1000) bart      (1000)      109 2024-04-19 11:09:23.000000 botl-110/botl/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1900 2024-04-19 11:09:23.000000 botl-110/botl/thread.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1091 2024-04-19 11:09:23.000000 botl-110/botl/timer.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-19 11:07:31.000000 botl-110/botl/utils.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1101 2024-04-19 11:09:23.000000 botl-110/botl/workdir.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-19 12:06:46.154775 botl-110/botl.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     3961 2024-04-19 12:06:46.000000 botl-110/botl.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      860 2024-04-19 12:06:46.000000 botl-110/botl.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-19 12:06:46.000000 botl-110/botl.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-19 12:06:46.000000 botl-110/botl.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-19 12:06:46.000000 botl-110/botl.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      857 2024-04-19 12:03:01.000000 botl-110/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-19 12:06:46.154775 botl-110/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      196 2024-04-19 12:01:22.000000 botl-110/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-21 22:04:11.201950 botl-111/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3961 2024-04-21 22:04:11.201950 botl-111/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     3438 2024-04-19 17:56:29.000000 botl-111/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-21 22:04:11.193950 botl-111/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     2261 2024-04-21 22:02:36.000000 botl-111/bin/botl
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     4654 2024-04-21 22:02:58.000000 botl-111/bin/botlbot
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     2385 2024-04-21 22:02:22.000000 botl-111/bin/botld
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-21 22:04:11.197950 botl-111/botl/
+-rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-04-19 17:56:29.000000 botl-111/botl/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1364 2024-04-19 17:56:29.000000 botl-111/botl/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3873 2024-04-20 23:22:28.000000 botl-111/botl/client.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1922 2024-04-19 17:56:29.000000 botl-111/botl/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      230 2024-04-19 17:56:29.000000 botl-111/botl/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1089 2024-04-19 17:56:29.000000 botl-111/botl/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      766 2024-04-19 17:56:29.000000 botl-111/botl/event.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1930 2024-04-19 17:56:29.000000 botl-111/botl/find.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1362 2024-04-19 17:56:29.000000 botl-111/botl/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-21 22:04:11.201950 botl-111/botl/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      493 2024-04-20 21:28:02.000000 botl-111/botl/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      211 2024-04-19 17:56:29.000000 botl-111/botl/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      403 2024-04-19 17:56:29.000000 botl-111/botl/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      425 2024-04-19 17:56:29.000000 botl-111/botl/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      819 2024-04-20 23:21:57.000000 botl-111/botl/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17621 2024-04-19 17:56:29.000000 botl-111/botl/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      776 2024-04-19 17:56:29.000000 botl-111/botl/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3552 2024-04-19 17:56:29.000000 botl-111/botl/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17081 2024-04-19 17:56:29.000000 botl-111/botl/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      240 2024-04-19 17:56:29.000000 botl-111/botl/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2400 2024-04-19 17:56:29.000000 botl-111/botl/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    11001 2024-04-19 17:56:29.000000 botl-111/botl/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2761 2024-04-19 17:56:29.000000 botl-111/botl/modules/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1184 2024-04-19 17:56:29.000000 botl-111/botl/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1038 2024-04-19 17:56:29.000000 botl-111/botl/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5130 2024-04-19 17:56:29.000000 botl-111/botl/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2933 2024-04-19 17:56:29.000000 botl-111/botl/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5799 2024-04-19 17:56:29.000000 botl-111/botl/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6155 2024-04-19 17:56:29.000000 botl-111/botl/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1814 2024-04-19 17:56:29.000000 botl-111/botl/parser.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      752 2024-04-19 17:56:29.000000 botl-111/botl/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      275 2024-04-19 17:56:29.000000 botl-111/botl/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      109 2024-04-20 21:23:50.000000 botl-111/botl/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1900 2024-04-19 17:56:29.000000 botl-111/botl/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1091 2024-04-19 17:56:29.000000 botl-111/botl/timer.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-19 17:56:29.000000 botl-111/botl/utils.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1101 2024-04-19 17:56:29.000000 botl-111/botl/workdir.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-21 22:04:11.197950 botl-111/botl.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3961 2024-04-21 22:04:11.000000 botl-111/botl.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      840 2024-04-21 22:04:11.000000 botl-111/botl.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-21 22:04:11.000000 botl-111/botl.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-21 22:04:11.000000 botl-111/botl.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-21 22:04:11.000000 botl-111/botl.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      857 2024-04-21 22:03:04.000000 botl-111/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-21 22:04:11.201950 botl-111/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      196 2024-04-19 17:56:29.000000 botl-111/setup.py
```

### Comparing `botl-110/PKG-INFO` & `botl-111/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botl
-Version: 110
+Version: 111
 Summary: bot library
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/botl
 Project-URL: bugs, https://github.com/xobjectz/botl/issues
 Project-URL: source, https://github.com/xobjectz/botl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `botl-110/README.rst` & `botl-111/README.rst`

 * *Files identical despite different names*

### Comparing `botl-110/bin/botl` & `botl-111/bin/botl`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     mods = None
 
 
 Cfg             = Default()
 Cfg.mod         = "cmd,mod"
 Cfg.opts        = ""
 Cfg.name        = "botl"
-Cfg.version     = "552"
+Cfg.version     = "111"
 Cfg.user        = getpass.getuser()
 Cfg.wd          = os.path.expanduser(f"~/.{Cfg.name}")
 Cfg.pidfile     = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
 Workdir.workdir = Cfg.wd
 
 
 dte = time.ctime(time.time()).replace("  ", " ")
```

### Comparing `botl-110/bin/botlbot` & `botl-111/bin/botlbot`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0201,W0212,W0613,E0401,E0402,E0611
+# pylint: disable=C,R,W0105,W0201,W0212,W0613,E0401,E0402,W0611
 # ruff: noqa: E402
 
 
 """NAME
 
     BOTL - bot library
 
@@ -32,30 +32,30 @@
 
 "main"
 
 
 import getpass
 import os
 import pwd
-import readline # pylint: disable=W0611
+import readline
 import sys
 import termios
 import time
 
 
 sys.path.insert(0, os.getcwd())
 
 
 from botl.client  import Client, cmnd, parse_cmd, spl
 from botl.command import Command
 from botl.default import Default
 from botl.errors  import debug, enable, errors
 from botl.event   import Event
 from botl.object  import cdir
-from botl.runtime  import broker
+from botl.runtime import broker
 from botl.workdir import Workdir, skel
 
 
 from botl import modules
 
 
 if os.path.exists("mods"):
@@ -64,15 +64,15 @@
     mods = None
 
 
 Cfg             = Default()
 Cfg.mod         = "cmd,mod"
 Cfg.opts        = ""
 Cfg.name        = "botl"
-Cfg.version     = "552"
+Cfg.version     = "111"
 Cfg.wd          = os.path.expanduser(f"~/.{Cfg.name}")
 Cfg.pidfile     = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
 Workdir.workdir = Cfg.wd
 
 
 dte = time.ctime(time.time()).replace("  ", " ")
 
@@ -122,17 +122,19 @@
     if os.path.exists(pidfile):
         os.unlink(pidfile)
     cdir(os.path.dirname(pidfile))
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
-def init(pkg, modstr):
+def init(pkg, modstr, disable=""):
     mds = []
     for modname in spl(modstr):
+        if skip(modname, disable):
+            continue
         module = getattr(pkg, modname, None)
         if not module:
             continue
         if "init" in dir(module):
             module.init()
             mds.append(module)
     return mds
@@ -140,14 +142,21 @@
 
 def privileges(username):
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
+def skip(name, skipped):
+    for skip in spl(skipped):
+        if skip in name:
+            return True
+    return False
+
+
 def wrap(func):
     old2 = None
     try:
         old2 = termios.tcgetattr(sys.stdin.fileno())
     except termios.error:
         pass
     try:
@@ -183,15 +192,15 @@
         daemon(Cfg.pidfile, "v" in Cfg.opts)
         privileges(Cfg.user)
         init(modules, Cfg.mod)
         while 1:
             time.sleep(1.0)
         return
     if "c" in Cfg.opts:
-        init(modules, Cfg.mod)
+        init(modules, Cfg.mod, Cfg.sets.dis)
         if mods:
             Cfg.mod += "," + ",".join(mods.__dir__())
             init(mods, Cfg.mod)
         csl = Console()
         csl.start()
         while 1:
             time.sleep(1.0)
```

### Comparing `botl-110/bin/botld` & `botl-111/bin/botld`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from botl.workdir import Workdir, skel
 
 
 Cfg             = Default()
 Cfg.mod         = "cmd,irc,mod,rss"
 Cfg.opts        = ""
 Cfg.name        = "botld"
-Cfg.version     = "107
+Cfg.version     = "111"
 Cfg.wd          = os.path.expanduser(f"~/.{Cfg.name}")
 Cfg.pidfile     = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
 Workdir.workdir = Cfg.wd
 
 
 from botl import modules
```

### Comparing `botl-110/botl/__init__.py` & `botl-111/botl/__init__.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/broker.py` & `botl-111/botl/broker.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/client.py` & `botl-111/botl/client.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/command.py` & `botl-111/botl/command.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/errors.py` & `botl-111/botl/errors.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/event.py` & `botl-111/botl/event.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/find.py` & `botl-111/botl/find.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/handler.py` & `botl-111/botl/handler.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/fnd.py` & `botl-111/botl/modules/fnd.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 #
 # pylint: disable=C,R,W0611,E0402
 
 
 "locate"
 
 
-from botl.command import Command
-from botl.find    import find
-from botl.object  import fmt
-from botl.persist import long
-from botl.workdir import liststore, skel
+from ..command import Command
+from ..find    import find
+from ..object  import fmt
+from ..persist import long
+from ..workdir import liststore, skel
 
 
 def fnd(event):
     skel()
     if not event.rest:
         res = sorted([x.split('.')[-1].lower() for x in liststore()])
         if res:
```

### Comparing `botl-110/botl/modules/irc.py` & `botl-111/botl/modules/irc.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/log.py` & `botl-111/botl/modules/log.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/mbx.py` & `botl-111/botl/modules/mbx.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/mdl.py` & `botl-111/botl/modules/mdl.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/req.py` & `botl-111/botl/modules/req.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/rss.py` & `botl-111/botl/modules/rss.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/rst.py` & `botl-111/botl/modules/rst.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/tdo.py` & `botl-111/botl/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/thr.py` & `botl-111/botl/modules/thr.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/tmr.py` & `botl-111/botl/modules/tmr.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/udp.py` & `botl-111/botl/modules/udp.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/modules/wsd.py` & `botl-111/botl/modules/wsd.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/object.py` & `botl-111/botl/object.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/parser.py` & `botl-111/botl/parser.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/persist.py` & `botl-111/botl/persist.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/thread.py` & `botl-111/botl/thread.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/timer.py` & `botl-111/botl/timer.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/utils.py` & `botl-111/botl/utils.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl/workdir.py` & `botl-111/botl/workdir.py`

 * *Files identical despite different names*

### Comparing `botl-110/botl.egg-info/PKG-INFO` & `botl-111/botl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botl
-Version: 110
+Version: 111
 Summary: bot library
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/botl
 Project-URL: bugs, https://github.com/xobjectz/botl/issues
 Project-URL: source, https://github.com/xobjectz/botl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `botl-110/botl.egg-info/SOURCES.txt` & `botl-111/botl.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 botl/modules/__init__.py
 botl/modules/cmd.py
 botl/modules/err.py
 botl/modules/flt.py
 botl/modules/fnd.py
 botl/modules/irc.py
 botl/modules/log.py
-botl/modules/man.py
 botl/modules/mbx.py
 botl/modules/mdl.py
 botl/modules/mod.py
 botl/modules/req.py
 botl/modules/rss.py
 botl/modules/rst.py
 botl/modules/tdo.py
```

### Comparing `botl-110/pyproject.toml` & `botl-111/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "botl"
 description = "bot library"
-version = "110"
+version = "111"
 authors = [
     {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
```

