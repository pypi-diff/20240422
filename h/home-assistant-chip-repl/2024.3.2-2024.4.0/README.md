# Comparing `tmp/home_assistant_chip_repl-2024.3.2-py3-none-any.whl.zip` & `tmp/home_assistant_chip_repl-2024.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 30034 bytes, number of entries: 10
--rw-r--r--  2.0 unx    36704 b- defN 24-Mar-28 16:27 chip/ChipBluezMgr.py
--rw-r--r--  2.0 unx    21470 b- defN 24-Mar-28 16:27 chip/ChipCoreBluetoothMgr.py
--rw-r--r--  2.0 unx     3958 b- defN 24-Mar-28 16:27 chip/ChipReplStartup.py
--rwxr-xr-x  2.0 unx    44047 b- defN 24-Mar-28 16:27 home_assistant_chip_repl-2024.3.2.data/scripts/chip-device-ctrl
--rwxr-xr-x  2.0 unx     1051 b- defN 24-Mar-28 16:27 home_assistant_chip_repl-2024.3.2.data/scripts/chip-repl
--rw-r--r--  2.0 unx    11357 b- defN 24-Mar-28 16:27 home_assistant_chip_repl-2024.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      663 b- defN 24-Mar-28 16:27 home_assistant_chip_repl-2024.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-28 16:27 home_assistant_chip_repl-2024.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Mar-28 16:27 home_assistant_chip_repl-2024.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      963 b- defN 24-Mar-28 16:27 home_assistant_chip_repl-2024.3.2.dist-info/RECORD
-10 files, 120310 bytes uncompressed, 28354 bytes compressed:  76.4%
+Zip file size: 30581 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    36704 b- defN 24-Apr-21 22:22 chip/ChipBluezMgr.py
+-rw-r--r--  2.0 unx    21470 b- defN 24-Apr-21 22:22 chip/ChipCoreBluetoothMgr.py
+-rw-r--r--  2.0 unx     5618 b- defN 24-Apr-21 22:22 chip/ChipReplStartup.py
+-rwxr-xr-x  2.0 unx    44047 b- defN 24-Apr-21 22:22 home_assistant_chip_repl-2024.4.0.data/scripts/chip-device-ctrl
+-rwxr-xr-x  2.0 unx     1051 b- defN 24-Apr-21 22:22 home_assistant_chip_repl-2024.4.0.data/scripts/chip-repl
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-21 22:22 home_assistant_chip_repl-2024.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      663 b- defN 24-Apr-21 22:22 home_assistant_chip_repl-2024.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 22:22 home_assistant_chip_repl-2024.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-21 22:22 home_assistant_chip_repl-2024.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      963 b- defN 24-Apr-21 22:22 home_assistant_chip_repl-2024.4.0.dist-info/RECORD
+10 files, 121970 bytes uncompressed, 28901 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: chip/ChipCoreBluetoothMgr.py
 Comment: 
 
 Filename: chip/ChipReplStartup.py
 Comment: 
 
-Filename: home_assistant_chip_repl-2024.3.2.data/scripts/chip-device-ctrl
+Filename: home_assistant_chip_repl-2024.4.0.data/scripts/chip-device-ctrl
 Comment: 
 
-Filename: home_assistant_chip_repl-2024.3.2.data/scripts/chip-repl
+Filename: home_assistant_chip_repl-2024.4.0.data/scripts/chip-repl
 Comment: 
 
-Filename: home_assistant_chip_repl-2024.3.2.dist-info/LICENSE
+Filename: home_assistant_chip_repl-2024.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: home_assistant_chip_repl-2024.3.2.dist-info/METADATA
+Filename: home_assistant_chip_repl-2024.4.0.dist-info/METADATA
 Comment: 
 
-Filename: home_assistant_chip_repl-2024.3.2.dist-info/WHEEL
+Filename: home_assistant_chip_repl-2024.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: home_assistant_chip_repl-2024.3.2.dist-info/top_level.txt
+Filename: home_assistant_chip_repl-2024.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: home_assistant_chip_repl-2024.3.2.dist-info/RECORD
+Filename: home_assistant_chip_repl-2024.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chip/ChipReplStartup.py

```diff
@@ -1,14 +1,15 @@
 import argparse
 import atexit
 import builtins
 import logging
+import os
+import pathlib
 
 import chip.CertificateAuthority
-import chip.discovery
 import chip.FabricAdmin
 import chip.logging
 import chip.native
 import coloredlogs
 from chip.ChipStack import ChipStack
 from rich import inspect, pretty
 from rich.console import Console
@@ -47,15 +48,18 @@
     else:
         logging.getLogger().setLevel(logging.WARN)
 
 
 certificateAuthorityManager = None
 
 
+@atexit.register
 def StackShutdown():
+    if not certificateAuthorityManager:
+        return
     certificateAuthorityManager.Shutdown()
     builtins.chipStack.Shutdown()
 
 
 def matterhelp(classOrObj=None):
     if (classOrObj is None):
         inspect(builtins.devCtrl, methods=True, help=True, private=False)
@@ -73,54 +77,95 @@
     ''' Enables debug mode that is utilized by some Matter modules
         to better facilitate debugging of failures (e.g throwing exceptions instead
         of returning well-formatted results).
     '''
     builtins.enableDebugMode = enableDebugMode
 
 
-console = Console()
+def main():
+    console = Console()
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-p", "--storagepath",
+        help="Path to persistent storage configuration file (default: /tmp/repl-storage.json)",
+        action="store",
+        default="/tmp/repl-storage.json")
+    parser.add_argument(
+        "-d", "--debug", help="Set default logging level to debug.", action="store_true")
+    parser.add_argument(
+        "-t", "--trust-store", help="Path to the PAA trust store.", action="store", default="./credentials/development/paa-root-certs")
+    args = parser.parse_args()
+
+    if not os.path.exists(args.trust_store):
+        # there is a chance that the script is being run from a sub-path of a checkout.
+        # try to adjust for convenience
+        store_path = pathlib.Path(args.trust_store)
+        if not store_path.is_absolute():
+            prefix = pathlib.Path().absolute()
+            while prefix != prefix.parent:
+                if prefix.joinpath(store_path).exists():
+                    oldpath = args.trust_store
+                    args.trust_store = prefix.joinpath(store_path).as_posix()
+                    console.print(f'''
+[bold] Replacing [/] store path {oldpath} with {args.trust_store}
+Note that you are still running from {os.getcwd()} so other relative paths may be off.
+                    ''')
+                    break
+                prefix = prefix.parent
+
+    if not os.path.exists(args.trust_store):
+        console.print(f'''
+[bold red] Missing directory:     [/]{args.trust_store}
+[bold] Your current directory: [/]{os.getcwd()}
+
+Please add a valid `--trust-store` argument to your script. If using jupyterlab,
+the command should look like:
+
+%run {{module.path}} --trust-store /chip/root/credentials/development/paa-root-certs
+
+or run `os.chdir` to the root of your CHIP repository checkout.
+        ''')
+        # nothing we can do ... things will NOT work
+        return
+
+    chip.native.Init()
+
+    global certificateAuthorityManager
+    global chipStack
+    global caList
+    global devCtrl
+
+    ReplInit(args.debug)
+
+    chipStack = ChipStack(persistentStoragePath=args.storagepath, enableServerInteractions=False)
+    certificateAuthorityManager = chip.CertificateAuthority.CertificateAuthorityManager(chipStack, chipStack.GetStorageManager())
+
+    certificateAuthorityManager.LoadAuthoritiesFromStorage()
+
+    if not certificateAuthorityManager.activeCaList:
+        ca = certificateAuthorityManager.NewCertificateAuthority()
+        ca.NewFabricAdmin(vendorId=0xFFF1, fabricId=1)
+    elif not certificateAuthorityManager.activeCaList[0].adminList:
+        certificateAuthorityManager.activeCaList[0].NewFabricAdmin(vendorId=0xFFF1, fabricId=1)
+
+    caList = certificateAuthorityManager.activeCaList
+
+    devCtrl = caList[0].adminList[0].NewController(paaTrustStorePath=args.trust_store)
+    builtins.devCtrl = devCtrl
+
+    console.print(
+        '\n\n[blue]The following objects have been created:')
+
+    console.print(
+        '''\t[red]certificateAuthorityManager[blue]:\tManages a list of CertificateAuthority instances.
+    \t[red]caList[blue]:\t\t\t\tThe list of CertificateAuthority instances.
+    \t[red]caList[n][m][blue]:\t\t\tA specific FabricAdmin object at index m for the nth CertificateAuthority instance.''')
+
+    console.print(
+        f'\n\n[blue]Default CHIP Device Controller (NodeId: {devCtrl.nodeId}): '
+        f'has been initialized to manage [bold red]caList[0].adminList[0][blue] (FabricId = {caList[0].adminList[0].fabricId}), '
+        'and is available as [bold red]devCtrl')
+
 
-parser = argparse.ArgumentParser()
-parser.add_argument(
-    "-p", "--storagepath",
-    help="Path to persistent storage configuration file (default: /tmp/repl-storage.json)",
-    action="store",
-    default="/tmp/repl-storage.json")
-parser.add_argument(
-    "-d", "--debug", help="Set default logging level to debug.", action="store_true")
-parser.add_argument(
-    "-t", "--trust-store", help="Path to the PAA trust store.", action="store", default="./credentials/development/paa-root-certs")
-args = parser.parse_args()
-
-chip.native.Init()
-
-ReplInit(args.debug)
-chipStack = ChipStack(persistentStoragePath=args.storagepath, enableServerInteractions=False)
-certificateAuthorityManager = chip.CertificateAuthority.CertificateAuthorityManager(chipStack, chipStack.GetStorageManager())
-
-certificateAuthorityManager.LoadAuthoritiesFromStorage()
-
-if (len(certificateAuthorityManager.activeCaList) == 0):
-    ca = certificateAuthorityManager.NewCertificateAuthority()
-    ca.NewFabricAdmin(vendorId=0xFFF1, fabricId=1)
-elif (len(certificateAuthorityManager.activeCaList[0].adminList) == 0):
-    certificateAuthorityManager.activeCaList[0].NewFabricAdmin(vendorId=0xFFF1, fabricId=1)
-
-caList = certificateAuthorityManager.activeCaList
-
-devCtrl = caList[0].adminList[0].NewController(paaTrustStorePath=args.trust_store)
-builtins.devCtrl = devCtrl
-
-atexit.register(StackShutdown)
-
-console.print(
-    '\n\n[blue]The following objects have been created:')
-
-console.print(
-    '''\t[red]certificateAuthorityManager[blue]:\tManages a list of CertificateAuthority instances.
-\t[red]caList[blue]:\t\t\t\tThe list of CertificateAuthority instances.
-\t[red]caList[n][m][blue]:\t\t\tA specific FabricAdmin object at index m for the nth CertificateAuthority instance.''')
-
-console.print(
-    f'\n\n[blue]Default CHIP Device Controller (NodeId: {devCtrl.nodeId}): '
-    f'has been initialized to manage [bold red]caList[0].adminList[0][blue] (FabricId = {caList[0].adminList[0].fabricId}), '
-    'and is available as [bold red]devCtrl')
+if __name__ == "__main__":
+    main()
```

## Comparing `home_assistant_chip_repl-2024.3.2.data/scripts/chip-device-ctrl` & `home_assistant_chip_repl-2024.4.0.data/scripts/chip-device-ctrl`

 * *Files identical despite different names*

## Comparing `home_assistant_chip_repl-2024.3.2.data/scripts/chip-repl` & `home_assistant_chip_repl-2024.4.0.data/scripts/chip-repl`

 * *Files identical despite different names*

## Comparing `home_assistant_chip_repl-2024.3.2.dist-info/LICENSE` & `home_assistant_chip_repl-2024.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `home_assistant_chip_repl-2024.3.2.dist-info/METADATA` & `home_assistant_chip_repl-2024.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-chip-repl
-Version: 2024.3.2
+Version: 2024.4.0
 Summary: Python-base APIs and tools for CHIP.
 Home-page: https://github.com/project-chip/connectedhomeip
 License: Apache
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

