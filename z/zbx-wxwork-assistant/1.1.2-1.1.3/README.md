# Comparing `tmp/zbx_wxwork_assistant-1.1.2-py3-none-any.whl.zip` & `tmp/zbx_wxwork_assistant-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 7737 bytes, number of entries: 9
+Zip file size: 8852 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     7191 b- defN 24-Apr-18 03:01 ZbxAssistant/ZbxApis.py
--rw-r--r--  2.0 unx      605 b- defN 24-Apr-17 10:35 ZbxAssistant/ZbxConfigs.py
--rw-r--r--  2.0 unx     1078 b- defN 24-Apr-17 09:59 ZbxAssistant/ZbxWxworkHots.py
+-rw-r--r--  2.0 unx      595 b- defN 24-Apr-22 09:09 ZbxAssistant/ZbxConfigs.py
+-rw-r--r--  2.0 unx     1754 b- defN 24-Apr-22 09:09 ZbxAssistant/ZbxWxworkHosts.py
 -rw-r--r--  2.0 unx     6149 b- defN 24-Apr-17 10:45 ZbxAssistant/ZbxWxworkProblems.py
+-rw-r--r--  2.0 unx     1981 b- defN 24-Apr-22 09:09 ZbxAssistant/ZbxWxworkProblemsBySeverity.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 09:59 ZbxAssistant/__init__.py
--rw-r--r--  2.0 unx     1337 b- defN 24-Apr-18 03:04 zbx_wxwork_assistant-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 03:04 zbx_wxwork_assistant-1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-18 03:04 zbx_wxwork_assistant-1.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      766 b- defN 24-Apr-18 03:04 zbx_wxwork_assistant-1.1.2.dist-info/RECORD
-9 files, 17231 bytes uncompressed, 6401 bytes compressed:  62.9%
+-rw-r--r--  2.0 unx     1337 b- defN 24-Apr-22 09:09 zbx_wxwork_assistant-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 09:09 zbx_wxwork_assistant-1.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-22 09:09 zbx_wxwork_assistant-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      867 b- defN 24-Apr-22 09:09 zbx_wxwork_assistant-1.1.3.dist-info/RECORD
+10 files, 19979 bytes uncompressed, 7352 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: ZbxAssistant/ZbxApis.py
 Comment: 
 
 Filename: ZbxAssistant/ZbxConfigs.py
 Comment: 
 
-Filename: ZbxAssistant/ZbxWxworkHots.py
+Filename: ZbxAssistant/ZbxWxworkHosts.py
 Comment: 
 
 Filename: ZbxAssistant/ZbxWxworkProblems.py
 Comment: 
 
+Filename: ZbxAssistant/ZbxWxworkProblemsBySeverity.py
+Comment: 
+
 Filename: ZbxAssistant/__init__.py
 Comment: 
 
-Filename: zbx_wxwork_assistant-1.1.2.dist-info/METADATA
+Filename: zbx_wxwork_assistant-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: zbx_wxwork_assistant-1.1.2.dist-info/WHEEL
+Filename: zbx_wxwork_assistant-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: zbx_wxwork_assistant-1.1.2.dist-info/top_level.txt
+Filename: zbx_wxwork_assistant-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: zbx_wxwork_assistant-1.1.2.dist-info/RECORD
+Filename: zbx_wxwork_assistant-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ZbxAssistant/ZbxConfigs.py

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-import os
 
 # 代表 Zabbix Problem 【是否被确认】的参数表示
 ACKNOWLEDGED = {
     "0": "unacknowledged/未确认",
     "1": "acknowledged/确认"
 }
 # 代表 Zabbix Problem 【是否处于维护状态】的参数表示
```

## Comparing `zbx_wxwork_assistant-1.1.2.dist-info/METADATA` & `zbx_wxwork_assistant-1.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zbx-wxwork-assistant
-Version: 1.1.2
+Version: 1.1.3
 Summary: A simple package for zabbix-wxwork assistant tool.
 Author: gary
 Author-email: mepmb@sina.com
 Requires-Dist: zabbix-api >=0.5.4
 Requires-Dist: diskcache ~=5.4.0
 
 zbx-wxwork-assistant
```

## Comparing `zbx_wxwork_assistant-1.1.2.dist-info/RECORD` & `zbx_wxwork_assistant-1.1.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ZbxAssistant/ZbxApis.py,sha256=yH3hjx7IkiukvXQz6O1v7wEVAQQZFHwkB1zmwc9x-x0,7191
-ZbxAssistant/ZbxConfigs.py,sha256=dpWIL0xEU8qLpCYQu5MN4H-q06jtXOQCEmdN_dupLQQ,605
-ZbxAssistant/ZbxWxworkHots.py,sha256=EVjwQTKregAi4kYV9eLzyUykwYK0sBog7aB4xI3WDyk,1078
+ZbxAssistant/ZbxConfigs.py,sha256=IvijR602v8kGyuLxIKvzxVA8HVYk30MyIwCaK_pTFTE,595
+ZbxAssistant/ZbxWxworkHosts.py,sha256=iQOinb1RErWyLLXeFteMhUI1_5jNCVCx1je9XgK8pnM,1754
 ZbxAssistant/ZbxWxworkProblems.py,sha256=DUU1UBpkEPXMAVVFTSaadDWOG1OFL_UJQWEYfW44JcY,6149
+ZbxAssistant/ZbxWxworkProblemsBySeverity.py,sha256=_291HpgJRcWm9hRs3VTEDxxQaGVaELxILpmRZKzEpeM,1981
 ZbxAssistant/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-zbx_wxwork_assistant-1.1.2.dist-info/METADATA,sha256=98ouPHS4oOTJOQqX7HB9EuFYEYVkF9exuLfPDvy8k7A,1337
-zbx_wxwork_assistant-1.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zbx_wxwork_assistant-1.1.2.dist-info/top_level.txt,sha256=wrjpqZuMDLcVJwJGkQiG-PPsasnELlI0eOxfUzGseu0,13
-zbx_wxwork_assistant-1.1.2.dist-info/RECORD,,
+zbx_wxwork_assistant-1.1.3.dist-info/METADATA,sha256=R0VHqX6dZus1fl7_gQy_lsaP5OpP823fWnRggxRa_sw,1337
+zbx_wxwork_assistant-1.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zbx_wxwork_assistant-1.1.3.dist-info/top_level.txt,sha256=wrjpqZuMDLcVJwJGkQiG-PPsasnELlI0eOxfUzGseu0,13
+zbx_wxwork_assistant-1.1.3.dist-info/RECORD,,
```

