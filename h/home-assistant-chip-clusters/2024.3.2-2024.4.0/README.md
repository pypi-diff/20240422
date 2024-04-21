# Comparing `tmp/home_assistant_chip_clusters-2024.3.2-py3-none-any.whl.zip` & `tmp/home_assistant_chip_clusters-2024.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 122172 bytes, number of entries: 14
--rw-r--r--  2.0 unx     2188 b- defN 24-Mar-28 16:27 chip/ChipUtility.py
--rw-r--r--  2.0 unx   415821 b- defN 24-Mar-28 16:27 chip/clusters/CHIPClusters.py
--rw-r--r--  2.0 unx    13387 b- defN 24-Mar-28 16:27 chip/clusters/ClusterObjects.py
--rw-r--r--  2.0 unx  1666474 b- defN 24-Mar-28 16:27 chip/clusters/Objects.py
--rw-r--r--  2.0 unx     1874 b- defN 24-Mar-28 16:27 chip/clusters/TestObjects.py
--rw-r--r--  2.0 unx     1226 b- defN 24-Mar-28 16:27 chip/clusters/Types.py
--rw-r--r--  2.0 unx     2404 b- defN 24-Mar-28 16:27 chip/clusters/enum.py
--rw-r--r--  2.0 unx    29245 b- defN 24-Mar-28 16:27 chip/tlv/__init__.py
--rw-r--r--  2.0 unx     5166 b- defN 24-Mar-28 16:27 chip/tlv/tlvlist.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Mar-28 16:27 home_assistant_chip_clusters-2024.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      542 b- defN 24-Mar-28 16:27 home_assistant_chip_clusters-2024.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-28 16:27 home_assistant_chip_clusters-2024.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Mar-28 16:27 home_assistant_chip_clusters-2024.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1238 b- defN 24-Mar-28 16:27 home_assistant_chip_clusters-2024.3.2.dist-info/RECORD
-14 files, 2151019 bytes uncompressed, 120102 bytes compressed:  94.4%
+Zip file size: 149965 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     2188 b- defN 24-Apr-21 22:22 chip/ChipUtility.py
+-rw-r--r--  2.0 unx   495958 b- defN 24-Apr-21 22:22 chip/clusters/CHIPClusters.py
+-rw-r--r--  2.0 unx    14516 b- defN 24-Apr-21 22:22 chip/clusters/ClusterObjects.py
+-rw-r--r--  2.0 unx  2060491 b- defN 24-Apr-21 22:22 chip/clusters/Objects.py
+-rw-r--r--  2.0 unx     1874 b- defN 24-Apr-21 22:22 chip/clusters/TestObjects.py
+-rw-r--r--  2.0 unx     1226 b- defN 24-Apr-21 22:22 chip/clusters/Types.py
+-rw-r--r--  2.0 unx     2404 b- defN 24-Apr-21 22:22 chip/clusters/enum.py
+-rw-r--r--  2.0 unx    29245 b- defN 24-Apr-21 22:22 chip/tlv/__init__.py
+-rw-r--r--  2.0 unx     5166 b- defN 24-Apr-21 22:22 chip/tlv/tlvlist.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-21 22:22 home_assistant_chip_clusters-2024.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      542 b- defN 24-Apr-21 22:22 home_assistant_chip_clusters-2024.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 22:22 home_assistant_chip_clusters-2024.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-21 22:22 home_assistant_chip_clusters-2024.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1238 b- defN 24-Apr-21 22:22 home_assistant_chip_clusters-2024.4.0.dist-info/RECORD
+14 files, 2626302 bytes uncompressed, 147895 bytes compressed:  94.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: chip/tlv/__init__.py
 Comment: 
 
 Filename: chip/tlv/tlvlist.py
 Comment: 
 
-Filename: home_assistant_chip_clusters-2024.3.2.dist-info/LICENSE
+Filename: home_assistant_chip_clusters-2024.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: home_assistant_chip_clusters-2024.3.2.dist-info/METADATA
+Filename: home_assistant_chip_clusters-2024.4.0.dist-info/METADATA
 Comment: 
 
-Filename: home_assistant_chip_clusters-2024.3.2.dist-info/WHEEL
+Filename: home_assistant_chip_clusters-2024.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: home_assistant_chip_clusters-2024.3.2.dist-info/top_level.txt
+Filename: home_assistant_chip_clusters-2024.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: home_assistant_chip_clusters-2024.3.2.dist-info/RECORD
+Filename: home_assistant_chip_clusters-2024.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chip/clusters/CHIPClusters.py

```diff
@@ -191,194 +191,14 @@
                 "attributeName": "ClusterRevision",
                 "attributeId": 0x0000FFFD,
                 "type": "int",
                 "reportable": True,
             },
         },
     }
-    _SCENES_CLUSTER_INFO = {
-        "clusterName": "Scenes",
-        "clusterId": 0x00000005,
-        "commands": {
-            0x00000000: {
-                "commandId": 0x00000000,
-                "commandName": "AddScene",
-                "args": {
-                    "groupID": "int",
-                    "sceneID": "int",
-                    "transitionTime": "int",
-                    "sceneName": "str",
-                    "extensionFieldSets": "ExtensionFieldSet",
-                },
-            },
-            0x00000001: {
-                "commandId": 0x00000001,
-                "commandName": "ViewScene",
-                "args": {
-                    "groupID": "int",
-                    "sceneID": "int",
-                },
-            },
-            0x00000002: {
-                "commandId": 0x00000002,
-                "commandName": "RemoveScene",
-                "args": {
-                    "groupID": "int",
-                    "sceneID": "int",
-                },
-            },
-            0x00000003: {
-                "commandId": 0x00000003,
-                "commandName": "RemoveAllScenes",
-                "args": {
-                    "groupID": "int",
-                },
-            },
-            0x00000004: {
-                "commandId": 0x00000004,
-                "commandName": "StoreScene",
-                "args": {
-                    "groupID": "int",
-                    "sceneID": "int",
-                },
-            },
-            0x00000005: {
-                "commandId": 0x00000005,
-                "commandName": "RecallScene",
-                "args": {
-                    "groupID": "int",
-                    "sceneID": "int",
-                    "transitionTime": "int",
-                },
-            },
-            0x00000006: {
-                "commandId": 0x00000006,
-                "commandName": "GetSceneMembership",
-                "args": {
-                    "groupID": "int",
-                },
-            },
-            0x00000040: {
-                "commandId": 0x00000040,
-                "commandName": "EnhancedAddScene",
-                "args": {
-                    "groupID": "int",
-                    "sceneID": "int",
-                    "transitionTime": "int",
-                    "sceneName": "str",
-                    "extensionFieldSets": "ExtensionFieldSet",
-                },
-            },
-            0x00000041: {
-                "commandId": 0x00000041,
-                "commandName": "EnhancedViewScene",
-                "args": {
-                    "groupID": "int",
-                    "sceneID": "int",
-                },
-            },
-            0x00000042: {
-                "commandId": 0x00000042,
-                "commandName": "CopyScene",
-                "args": {
-                    "mode": "int",
-                    "groupIdentifierFrom": "int",
-                    "sceneIdentifierFrom": "int",
-                    "groupIdentifierTo": "int",
-                    "sceneIdentifierTo": "int",
-                },
-            },
-        },
-        "attributes": {
-            0x00000000: {
-                "attributeName": "SceneCount",
-                "attributeId": 0x00000000,
-                "type": "int",
-                "reportable": True,
-            },
-            0x00000001: {
-                "attributeName": "CurrentScene",
-                "attributeId": 0x00000001,
-                "type": "int",
-                "reportable": True,
-            },
-            0x00000002: {
-                "attributeName": "CurrentGroup",
-                "attributeId": 0x00000002,
-                "type": "int",
-                "reportable": True,
-            },
-            0x00000003: {
-                "attributeName": "SceneValid",
-                "attributeId": 0x00000003,
-                "type": "bool",
-                "reportable": True,
-            },
-            0x00000004: {
-                "attributeName": "NameSupport",
-                "attributeId": 0x00000004,
-                "type": "int",
-                "reportable": True,
-            },
-            0x00000005: {
-                "attributeName": "LastConfiguredBy",
-                "attributeId": 0x00000005,
-                "type": "int",
-                "reportable": True,
-            },
-            0x00000006: {
-                "attributeName": "SceneTableSize",
-                "attributeId": 0x00000006,
-                "type": "int",
-                "reportable": True,
-            },
-            0x00000007: {
-                "attributeName": "RemainingCapacity",
-                "attributeId": 0x00000007,
-                "type": "int",
-                "reportable": True,
-            },
-            0x0000FFF8: {
-                "attributeName": "GeneratedCommandList",
-                "attributeId": 0x0000FFF8,
-                "type": "int",
-                "reportable": True,
-            },
-            0x0000FFF9: {
-                "attributeName": "AcceptedCommandList",
-                "attributeId": 0x0000FFF9,
-                "type": "int",
-                "reportable": True,
-            },
-            0x0000FFFA: {
-                "attributeName": "EventList",
-                "attributeId": 0x0000FFFA,
-                "type": "int",
-                "reportable": True,
-            },
-            0x0000FFFB: {
-                "attributeName": "AttributeList",
-                "attributeId": 0x0000FFFB,
-                "type": "int",
-                "reportable": True,
-            },
-            0x0000FFFC: {
-                "attributeName": "FeatureMap",
-                "attributeId": 0x0000FFFC,
-                "type": "int",
-                "reportable": True,
-            },
-            0x0000FFFD: {
-                "attributeName": "ClusterRevision",
-                "attributeId": 0x0000FFFD,
-                "type": "int",
-                "reportable": True,
-            },
-        },
-    }
     _ON_OFF_CLUSTER_INFO = {
         "clusterName": "OnOff",
         "clusterId": 0x00000006,
         "commands": {
             0x00000000: {
                 "commandId": 0x00000000,
                 "commandName": "Off",
@@ -1419,14 +1239,26 @@
             },
             0x00000014: {
                 "attributeName": "ProductAppearance",
                 "attributeId": 0x00000014,
                 "type": "",
                 "reportable": True,
             },
+            0x00000015: {
+                "attributeName": "SpecificationVersion",
+                "attributeId": 0x00000015,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000016: {
+                "attributeName": "MaxPathsPerInvoke",
+                "attributeId": 0x00000016,
+                "type": "int",
+                "reportable": True,
+            },
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
                 "type": "int",
                 "reportable": True,
             },
             0x0000FFF9: {
@@ -2186,14 +2018,17 @@
             0x00000002: {
                 "commandId": 0x00000002,
                 "commandName": "AddOrUpdateWiFiNetwork",
                 "args": {
                     "ssid": "bytes",
                     "credentials": "bytes",
                     "breadcrumb": "int",
+                    "networkIdentity": "bytes",
+                    "clientIdentifier": "bytes",
+                    "possessionNonce": "bytes",
                 },
             },
             0x00000003: {
                 "commandId": 0x00000003,
                 "commandName": "AddOrUpdateThreadNetwork",
                 "args": {
                     "operationalDataset": "bytes",
@@ -2221,14 +2056,22 @@
                 "commandName": "ReorderNetwork",
                 "args": {
                     "networkID": "bytes",
                     "networkIndex": "int",
                     "breadcrumb": "int",
                 },
             },
+            0x00000009: {
+                "commandId": 0x00000009,
+                "commandName": "QueryIdentity",
+                "args": {
+                    "keyIdentifier": "bytes",
+                    "possessionNonce": "bytes",
+                },
+            },
         },
         "attributes": {
             0x00000000: {
                 "attributeName": "MaxNetworks",
                 "attributeId": 0x00000000,
                 "type": "int",
                 "reportable": True,
@@ -2393,14 +2236,29 @@
                 "commandId": 0x00000000,
                 "commandName": "TestEventTrigger",
                 "args": {
                     "enableKey": "bytes",
                     "eventTrigger": "int",
                 },
             },
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "TimeSnapshot",
+                "args": {
+                },
+            },
+            0x00000003: {
+                "commandId": 0x00000003,
+                "commandName": "PayloadTestRequest",
+                "args": {
+                    "enableKey": "bytes",
+                    "value": "int",
+                    "count": "int",
+                },
+            },
         },
         "attributes": {
             0x00000000: {
                 "attributeName": "NetworkInterfaces",
                 "attributeId": 0x00000000,
                 "type": "",
                 "reportable": True,
@@ -2449,20 +2307,14 @@
             },
             0x00000008: {
                 "attributeName": "TestEventTriggersEnabled",
                 "attributeId": 0x00000008,
                 "type": "bool",
                 "reportable": True,
             },
-            0x00000009: {
-                "attributeName": "AverageWearCount",
-                "attributeId": 0x00000009,
-                "type": "int",
-                "reportable": True,
-            },
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
                 "type": "int",
                 "reportable": True,
             },
             0x0000FFF9: {
@@ -4222,14 +4074,15 @@
                     "verificationKey": "bytes",
                 },
             },
             0x00000003: {
                 "commandId": 0x00000003,
                 "commandName": "StayActiveRequest",
                 "args": {
+                    "stayActiveDuration": "int",
                 },
             },
         },
         "attributes": {
             0x00000000: {
                 "attributeName": "IdleModeDuration",
                 "attributeId": 0x00000000,
@@ -4274,14 +4127,347 @@
             },
             0x00000007: {
                 "attributeName": "UserActiveModeTriggerInstruction",
                 "attributeId": 0x00000007,
                 "type": "str",
                 "reportable": True,
             },
+            0x00000008: {
+                "attributeName": "OperatingMode",
+                "attributeId": 0x00000008,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _TIMER_CLUSTER_INFO = {
+        "clusterName": "Timer",
+        "clusterId": 0x00000047,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "SetTimer",
+                "args": {
+                    "newTime": "int",
+                },
+            },
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "ResetTimer",
+                "args": {
+                },
+            },
+            0x00000002: {
+                "commandId": 0x00000002,
+                "commandName": "AddTime",
+                "args": {
+                    "additionalTime": "int",
+                },
+            },
+            0x00000003: {
+                "commandId": 0x00000003,
+                "commandName": "ReduceTime",
+                "args": {
+                    "timeReduction": "int",
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "SetTime",
+                "attributeId": 0x00000000,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "TimeRemaining",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "TimerState",
+                "attributeId": 0x00000002,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _OVEN_CAVITY_OPERATIONAL_STATE_CLUSTER_INFO = {
+        "clusterName": "OvenCavityOperationalState",
+        "clusterId": 0x00000048,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "Pause",
+                "args": {
+                },
+            },
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "Stop",
+                "args": {
+                },
+            },
+            0x00000002: {
+                "commandId": 0x00000002,
+                "commandName": "Start",
+                "args": {
+                },
+            },
+            0x00000003: {
+                "commandId": 0x00000003,
+                "commandName": "Resume",
+                "args": {
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "PhaseList",
+                "attributeId": 0x00000000,
+                "type": "str",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "CurrentPhase",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "CountdownTime",
+                "attributeId": 0x00000002,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000003: {
+                "attributeName": "OperationalStateList",
+                "attributeId": 0x00000003,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000004: {
+                "attributeName": "OperationalState",
+                "attributeId": 0x00000004,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000005: {
+                "attributeName": "OperationalError",
+                "attributeId": 0x00000005,
+                "type": "",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _OVEN_MODE_CLUSTER_INFO = {
+        "clusterName": "OvenMode",
+        "clusterId": 0x00000049,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "ChangeToMode",
+                "args": {
+                    "newMode": "int",
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "SupportedModes",
+                "attributeId": 0x00000000,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "CurrentMode",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "StartUpMode",
+                "attributeId": 0x00000002,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000003: {
+                "attributeName": "OnMode",
+                "attributeId": 0x00000003,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _LAUNDRY_DRYER_CONTROLS_CLUSTER_INFO = {
+        "clusterName": "LaundryDryerControls",
+        "clusterId": 0x0000004A,
+        "commands": {
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "SupportedDrynessLevels",
+                "attributeId": 0x00000000,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "SelectedDrynessLevel",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
                 "type": "int",
                 "reportable": True,
             },
             0x0000FFF9: {
@@ -4650,21 +4836,14 @@
             },
             0x00000001: {
                 "attributeName": "CurrentMode",
                 "attributeId": 0x00000001,
                 "type": "int",
                 "reportable": True,
             },
-            0x00000003: {
-                "attributeName": "OnMode",
-                "attributeId": 0x00000003,
-                "type": "int",
-                "reportable": True,
-                "writable": True,
-            },
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
                 "type": "int",
                 "reportable": True,
             },
             0x0000FFF9: {
@@ -4720,21 +4899,14 @@
             },
             0x00000001: {
                 "attributeName": "CurrentMode",
                 "attributeId": 0x00000001,
                 "type": "int",
                 "reportable": True,
             },
-            0x00000003: {
-                "attributeName": "OnMode",
-                "attributeId": 0x00000003,
-                "type": "int",
-                "reportable": True,
-                "writable": True,
-            },
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
                 "type": "int",
                 "reportable": True,
             },
             0x0000FFF9: {
@@ -5253,14 +5425,186 @@
                 "attributeName": "ClusterRevision",
                 "attributeId": 0x0000FFFD,
                 "type": "int",
                 "reportable": True,
             },
         },
     }
+    _MICROWAVE_OVEN_MODE_CLUSTER_INFO = {
+        "clusterName": "MicrowaveOvenMode",
+        "clusterId": 0x0000005E,
+        "commands": {
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "SupportedModes",
+                "attributeId": 0x00000000,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "CurrentMode",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _MICROWAVE_OVEN_CONTROL_CLUSTER_INFO = {
+        "clusterName": "MicrowaveOvenControl",
+        "clusterId": 0x0000005F,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "SetCookingParameters",
+                "args": {
+                    "cookMode": "int",
+                    "cookTime": "int",
+                    "powerSetting": "int",
+                    "wattSettingIndex": "int",
+                    "startAfterSetting": "bool",
+                },
+            },
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "AddMoreTime",
+                "args": {
+                    "timeToAdd": "int",
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "CookTime",
+                "attributeId": 0x00000000,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "MaxCookTime",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "PowerSetting",
+                "attributeId": 0x00000002,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000003: {
+                "attributeName": "MinPower",
+                "attributeId": 0x00000003,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000004: {
+                "attributeName": "MaxPower",
+                "attributeId": 0x00000004,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000005: {
+                "attributeName": "PowerStep",
+                "attributeId": 0x00000005,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000006: {
+                "attributeName": "SupportedWatts",
+                "attributeId": 0x00000006,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000007: {
+                "attributeName": "SelectedWattIndex",
+                "attributeId": 0x00000007,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000008: {
+                "attributeName": "WattRating",
+                "attributeId": 0x00000008,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
     _OPERATIONAL_STATE_CLUSTER_INFO = {
         "clusterName": "OperationalState",
         "clusterId": 0x00000060,
         "commands": {
             0x00000000: {
                 "commandId": 0x00000000,
                 "commandName": "Pause",
@@ -5367,32 +5711,26 @@
         "commands": {
             0x00000000: {
                 "commandId": 0x00000000,
                 "commandName": "Pause",
                 "args": {
                 },
             },
-            0x00000001: {
-                "commandId": 0x00000001,
-                "commandName": "Stop",
-                "args": {
-                },
-            },
-            0x00000002: {
-                "commandId": 0x00000002,
-                "commandName": "Start",
-                "args": {
-                },
-            },
             0x00000003: {
                 "commandId": 0x00000003,
                 "commandName": "Resume",
                 "args": {
                 },
             },
+            0x00000080: {
+                "commandId": 0x00000080,
+                "commandName": "GoHome",
+                "args": {
+                },
+            },
         },
         "attributes": {
             0x00000000: {
                 "attributeName": "PhaseList",
                 "attributeId": 0x00000000,
                 "type": "str",
                 "reportable": True,
@@ -5461,14 +5799,145 @@
                 "attributeName": "ClusterRevision",
                 "attributeId": 0x0000FFFD,
                 "type": "int",
                 "reportable": True,
             },
         },
     }
+    _SCENES_MANAGEMENT_CLUSTER_INFO = {
+        "clusterName": "ScenesManagement",
+        "clusterId": 0x00000062,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "AddScene",
+                "args": {
+                    "groupID": "int",
+                    "sceneID": "int",
+                    "transitionTime": "int",
+                    "sceneName": "str",
+                    "extensionFieldSets": "ExtensionFieldSet",
+                },
+            },
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "ViewScene",
+                "args": {
+                    "groupID": "int",
+                    "sceneID": "int",
+                },
+            },
+            0x00000002: {
+                "commandId": 0x00000002,
+                "commandName": "RemoveScene",
+                "args": {
+                    "groupID": "int",
+                    "sceneID": "int",
+                },
+            },
+            0x00000003: {
+                "commandId": 0x00000003,
+                "commandName": "RemoveAllScenes",
+                "args": {
+                    "groupID": "int",
+                },
+            },
+            0x00000004: {
+                "commandId": 0x00000004,
+                "commandName": "StoreScene",
+                "args": {
+                    "groupID": "int",
+                    "sceneID": "int",
+                },
+            },
+            0x00000005: {
+                "commandId": 0x00000005,
+                "commandName": "RecallScene",
+                "args": {
+                    "groupID": "int",
+                    "sceneID": "int",
+                    "transitionTime": "int",
+                },
+            },
+            0x00000006: {
+                "commandId": 0x00000006,
+                "commandName": "GetSceneMembership",
+                "args": {
+                    "groupID": "int",
+                },
+            },
+            0x00000040: {
+                "commandId": 0x00000040,
+                "commandName": "CopyScene",
+                "args": {
+                    "mode": "int",
+                    "groupIdentifierFrom": "int",
+                    "sceneIdentifierFrom": "int",
+                    "groupIdentifierTo": "int",
+                    "sceneIdentifierTo": "int",
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "LastConfiguredBy",
+                "attributeId": 0x00000000,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "SceneTableSize",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "FabricSceneInfo",
+                "attributeId": 0x00000002,
+                "type": "",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
     _HEPA_FILTER_MONITORING_CLUSTER_INFO = {
         "clusterName": "HepaFilterMonitoring",
         "clusterId": 0x00000071,
         "commands": {
             0x00000000: {
                 "commandId": 0x00000000,
                 "commandName": "ResetCondition",
@@ -5635,14 +6104,1361 @@
                 "attributeName": "ClusterRevision",
                 "attributeId": 0x0000FFFD,
                 "type": "int",
                 "reportable": True,
             },
         },
     }
+    _BOOLEAN_STATE_CONFIGURATION_CLUSTER_INFO = {
+        "clusterName": "BooleanStateConfiguration",
+        "clusterId": 0x00000080,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "SuppressAlarm",
+                "args": {
+                    "alarmsToSuppress": "int",
+                },
+            },
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "EnableDisableAlarm",
+                "args": {
+                    "alarmsToEnableDisable": "int",
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "CurrentSensitivityLevel",
+                "attributeId": 0x00000000,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000001: {
+                "attributeName": "SupportedSensitivityLevels",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "DefaultSensitivityLevel",
+                "attributeId": 0x00000002,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000003: {
+                "attributeName": "AlarmsActive",
+                "attributeId": 0x00000003,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000004: {
+                "attributeName": "AlarmsSuppressed",
+                "attributeId": 0x00000004,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000005: {
+                "attributeName": "AlarmsEnabled",
+                "attributeId": 0x00000005,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000006: {
+                "attributeName": "AlarmsSupported",
+                "attributeId": 0x00000006,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000007: {
+                "attributeName": "SensorFault",
+                "attributeId": 0x00000007,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _VALVE_CONFIGURATION_AND_CONTROL_CLUSTER_INFO = {
+        "clusterName": "ValveConfigurationAndControl",
+        "clusterId": 0x00000081,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "Open",
+                "args": {
+                    "openDuration": "int",
+                    "targetLevel": "int",
+                },
+            },
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "Close",
+                "args": {
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "OpenDuration",
+                "attributeId": 0x00000000,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "DefaultOpenDuration",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000002: {
+                "attributeName": "AutoCloseTime",
+                "attributeId": 0x00000002,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000003: {
+                "attributeName": "RemainingDuration",
+                "attributeId": 0x00000003,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000004: {
+                "attributeName": "CurrentState",
+                "attributeId": 0x00000004,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000005: {
+                "attributeName": "TargetState",
+                "attributeId": 0x00000005,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000006: {
+                "attributeName": "CurrentLevel",
+                "attributeId": 0x00000006,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000007: {
+                "attributeName": "TargetLevel",
+                "attributeId": 0x00000007,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000008: {
+                "attributeName": "DefaultOpenLevel",
+                "attributeId": 0x00000008,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000009: {
+                "attributeName": "ValveFault",
+                "attributeId": 0x00000009,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000000A: {
+                "attributeName": "LevelStep",
+                "attributeId": 0x0000000A,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _ELECTRICAL_POWER_MEASUREMENT_CLUSTER_INFO = {
+        "clusterName": "ElectricalPowerMeasurement",
+        "clusterId": 0x00000090,
+        "commands": {
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "PowerMode",
+                "attributeId": 0x00000000,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "NumberOfMeasurementTypes",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "Accuracy",
+                "attributeId": 0x00000002,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000003: {
+                "attributeName": "Ranges",
+                "attributeId": 0x00000003,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000004: {
+                "attributeName": "Voltage",
+                "attributeId": 0x00000004,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000005: {
+                "attributeName": "ActiveCurrent",
+                "attributeId": 0x00000005,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000006: {
+                "attributeName": "ReactiveCurrent",
+                "attributeId": 0x00000006,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000007: {
+                "attributeName": "ApparentCurrent",
+                "attributeId": 0x00000007,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000008: {
+                "attributeName": "ActivePower",
+                "attributeId": 0x00000008,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000009: {
+                "attributeName": "ReactivePower",
+                "attributeId": 0x00000009,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000000A: {
+                "attributeName": "ApparentPower",
+                "attributeId": 0x0000000A,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000000B: {
+                "attributeName": "RMSVoltage",
+                "attributeId": 0x0000000B,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000000C: {
+                "attributeName": "RMSCurrent",
+                "attributeId": 0x0000000C,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000000D: {
+                "attributeName": "RMSPower",
+                "attributeId": 0x0000000D,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000000E: {
+                "attributeName": "Frequency",
+                "attributeId": 0x0000000E,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000000F: {
+                "attributeName": "HarmonicCurrents",
+                "attributeId": 0x0000000F,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000010: {
+                "attributeName": "HarmonicPhases",
+                "attributeId": 0x00000010,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000011: {
+                "attributeName": "PowerFactor",
+                "attributeId": 0x00000011,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000012: {
+                "attributeName": "NeutralCurrent",
+                "attributeId": 0x00000012,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _ELECTRICAL_ENERGY_MEASUREMENT_CLUSTER_INFO = {
+        "clusterName": "ElectricalEnergyMeasurement",
+        "clusterId": 0x00000091,
+        "commands": {
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "Accuracy",
+                "attributeId": 0x00000000,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "CumulativeEnergyImported",
+                "attributeId": 0x00000001,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "CumulativeEnergyExported",
+                "attributeId": 0x00000002,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000003: {
+                "attributeName": "PeriodicEnergyImported",
+                "attributeId": 0x00000003,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000004: {
+                "attributeName": "PeriodicEnergyExported",
+                "attributeId": 0x00000004,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000005: {
+                "attributeName": "CumulativeEnergyReset",
+                "attributeId": 0x00000005,
+                "type": "",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _DEMAND_RESPONSE_LOAD_CONTROL_CLUSTER_INFO = {
+        "clusterName": "DemandResponseLoadControl",
+        "clusterId": 0x00000096,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "RegisterLoadControlProgramRequest",
+                "args": {
+                    "loadControlProgram": "LoadControlProgramStruct",
+                },
+            },
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "UnregisterLoadControlProgramRequest",
+                "args": {
+                    "loadControlProgramID": "bytes",
+                },
+            },
+            0x00000002: {
+                "commandId": 0x00000002,
+                "commandName": "AddLoadControlEventRequest",
+                "args": {
+                    "event": "LoadControlEventStruct",
+                },
+            },
+            0x00000003: {
+                "commandId": 0x00000003,
+                "commandName": "RemoveLoadControlEventRequest",
+                "args": {
+                    "eventID": "bytes",
+                    "cancelControl": "int",
+                },
+            },
+            0x00000004: {
+                "commandId": 0x00000004,
+                "commandName": "ClearLoadControlEventsRequest",
+                "args": {
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "LoadControlPrograms",
+                "attributeId": 0x00000000,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "NumberOfLoadControlPrograms",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "Events",
+                "attributeId": 0x00000002,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000003: {
+                "attributeName": "ActiveEvents",
+                "attributeId": 0x00000003,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000004: {
+                "attributeName": "NumberOfEventsPerProgram",
+                "attributeId": 0x00000004,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000005: {
+                "attributeName": "NumberOfTransitions",
+                "attributeId": 0x00000005,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000006: {
+                "attributeName": "DefaultRandomStart",
+                "attributeId": 0x00000006,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000007: {
+                "attributeName": "DefaultRandomDuration",
+                "attributeId": 0x00000007,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _MESSAGES_CLUSTER_INFO = {
+        "clusterName": "Messages",
+        "clusterId": 0x00000097,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "PresentMessagesRequest",
+                "args": {
+                    "messageID": "bytes",
+                    "priority": "int",
+                    "messageControl": "int",
+                    "startTime": "int",
+                    "duration": "int",
+                    "messageText": "str",
+                    "responses": "MessageResponseOptionStruct",
+                },
+            },
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "CancelMessagesRequest",
+                "args": {
+                    "messageIDs": "bytes",
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "Messages",
+                "attributeId": 0x00000000,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "ActiveMessageIDs",
+                "attributeId": 0x00000001,
+                "type": "bytes",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _DEVICE_ENERGY_MANAGEMENT_CLUSTER_INFO = {
+        "clusterName": "DeviceEnergyManagement",
+        "clusterId": 0x00000098,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "PowerAdjustRequest",
+                "args": {
+                    "power": "int",
+                    "duration": "int",
+                    "cause": "int",
+                },
+            },
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "CancelPowerAdjustRequest",
+                "args": {
+                },
+            },
+            0x00000002: {
+                "commandId": 0x00000002,
+                "commandName": "StartTimeAdjustRequest",
+                "args": {
+                    "requestedStartTime": "int",
+                    "cause": "int",
+                },
+            },
+            0x00000003: {
+                "commandId": 0x00000003,
+                "commandName": "PauseRequest",
+                "args": {
+                    "duration": "int",
+                    "cause": "int",
+                },
+            },
+            0x00000004: {
+                "commandId": 0x00000004,
+                "commandName": "ResumeRequest",
+                "args": {
+                },
+            },
+            0x00000005: {
+                "commandId": 0x00000005,
+                "commandName": "ModifyForecastRequest",
+                "args": {
+                    "forecastId": "int",
+                    "slotAdjustments": "SlotAdjustmentStruct",
+                    "cause": "int",
+                },
+            },
+            0x00000006: {
+                "commandId": 0x00000006,
+                "commandName": "RequestConstraintBasedForecast",
+                "args": {
+                    "constraints": "ConstraintsStruct",
+                    "cause": "int",
+                },
+            },
+            0x00000007: {
+                "commandId": 0x00000007,
+                "commandName": "CancelRequest",
+                "args": {
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "ESAType",
+                "attributeId": 0x00000000,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "ESACanGenerate",
+                "attributeId": 0x00000001,
+                "type": "bool",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "ESAState",
+                "attributeId": 0x00000002,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000003: {
+                "attributeName": "AbsMinPower",
+                "attributeId": 0x00000003,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000004: {
+                "attributeName": "AbsMaxPower",
+                "attributeId": 0x00000004,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000005: {
+                "attributeName": "PowerAdjustmentCapability",
+                "attributeId": 0x00000005,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000006: {
+                "attributeName": "Forecast",
+                "attributeId": 0x00000006,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000007: {
+                "attributeName": "OptOutState",
+                "attributeId": 0x00000007,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _ENERGY_EVSE_CLUSTER_INFO = {
+        "clusterName": "EnergyEvse",
+        "clusterId": 0x00000099,
+        "commands": {
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "Disable",
+                "args": {
+                },
+            },
+            0x00000002: {
+                "commandId": 0x00000002,
+                "commandName": "EnableCharging",
+                "args": {
+                    "chargingEnabledUntil": "int",
+                    "minimumChargeCurrent": "int",
+                    "maximumChargeCurrent": "int",
+                },
+            },
+            0x00000003: {
+                "commandId": 0x00000003,
+                "commandName": "EnableDischarging",
+                "args": {
+                    "dischargingEnabledUntil": "int",
+                    "maximumDischargeCurrent": "int",
+                },
+            },
+            0x00000004: {
+                "commandId": 0x00000004,
+                "commandName": "StartDiagnostics",
+                "args": {
+                },
+            },
+            0x00000005: {
+                "commandId": 0x00000005,
+                "commandName": "SetTargets",
+                "args": {
+                    "chargingTargetSchedules": "ChargingTargetScheduleStruct",
+                },
+            },
+            0x00000006: {
+                "commandId": 0x00000006,
+                "commandName": "GetTargets",
+                "args": {
+                },
+            },
+            0x00000007: {
+                "commandId": 0x00000007,
+                "commandName": "ClearTargets",
+                "args": {
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "State",
+                "attributeId": 0x00000000,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "SupplyState",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "FaultState",
+                "attributeId": 0x00000002,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000003: {
+                "attributeName": "ChargingEnabledUntil",
+                "attributeId": 0x00000003,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000004: {
+                "attributeName": "DischargingEnabledUntil",
+                "attributeId": 0x00000004,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000005: {
+                "attributeName": "CircuitCapacity",
+                "attributeId": 0x00000005,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000006: {
+                "attributeName": "MinimumChargeCurrent",
+                "attributeId": 0x00000006,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000007: {
+                "attributeName": "MaximumChargeCurrent",
+                "attributeId": 0x00000007,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000008: {
+                "attributeName": "MaximumDischargeCurrent",
+                "attributeId": 0x00000008,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000009: {
+                "attributeName": "UserMaximumChargeCurrent",
+                "attributeId": 0x00000009,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x0000000A: {
+                "attributeName": "RandomizationDelayWindow",
+                "attributeId": 0x0000000A,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000023: {
+                "attributeName": "NextChargeStartTime",
+                "attributeId": 0x00000023,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000024: {
+                "attributeName": "NextChargeTargetTime",
+                "attributeId": 0x00000024,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000025: {
+                "attributeName": "NextChargeRequiredEnergy",
+                "attributeId": 0x00000025,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000026: {
+                "attributeName": "NextChargeTargetSoC",
+                "attributeId": 0x00000026,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000027: {
+                "attributeName": "ApproximateEVEfficiency",
+                "attributeId": 0x00000027,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000030: {
+                "attributeName": "StateOfCharge",
+                "attributeId": 0x00000030,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000031: {
+                "attributeName": "BatteryCapacity",
+                "attributeId": 0x00000031,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000032: {
+                "attributeName": "VehicleID",
+                "attributeId": 0x00000032,
+                "type": "str",
+                "reportable": True,
+            },
+            0x00000040: {
+                "attributeName": "SessionID",
+                "attributeId": 0x00000040,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000041: {
+                "attributeName": "SessionDuration",
+                "attributeId": 0x00000041,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000042: {
+                "attributeName": "SessionEnergyCharged",
+                "attributeId": 0x00000042,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000043: {
+                "attributeName": "SessionEnergyDischarged",
+                "attributeId": 0x00000043,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _ENERGY_PREFERENCE_CLUSTER_INFO = {
+        "clusterName": "EnergyPreference",
+        "clusterId": 0x0000009B,
+        "commands": {
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "EnergyBalances",
+                "attributeId": 0x00000000,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "CurrentEnergyBalance",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000002: {
+                "attributeName": "EnergyPriorities",
+                "attributeId": 0x00000002,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000003: {
+                "attributeName": "LowPowerModeSensitivities",
+                "attributeId": 0x00000003,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000004: {
+                "attributeName": "CurrentLowPowerModeSensitivity",
+                "attributeId": 0x00000004,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _POWER_TOPOLOGY_CLUSTER_INFO = {
+        "clusterName": "PowerTopology",
+        "clusterId": 0x0000009C,
+        "commands": {
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "AvailableEndpoints",
+                "attributeId": 0x00000000,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "ActiveEndpoints",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _ENERGY_EVSE_MODE_CLUSTER_INFO = {
+        "clusterName": "EnergyEvseMode",
+        "clusterId": 0x0000009D,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "ChangeToMode",
+                "args": {
+                    "newMode": "int",
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "SupportedModes",
+                "attributeId": 0x00000000,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "CurrentMode",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "StartUpMode",
+                "attributeId": 0x00000002,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000003: {
+                "attributeName": "OnMode",
+                "attributeId": 0x00000003,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _DEVICE_ENERGY_MANAGEMENT_MODE_CLUSTER_INFO = {
+        "clusterName": "DeviceEnergyManagementMode",
+        "clusterId": 0x0000009F,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "ChangeToMode",
+                "args": {
+                    "newMode": "int",
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "SupportedModes",
+                "attributeId": 0x00000000,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "CurrentMode",
+                "attributeId": 0x00000001,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "StartUpMode",
+                "attributeId": 0x00000002,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000003: {
+                "attributeName": "OnMode",
+                "attributeId": 0x00000003,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
     _DOOR_LOCK_CLUSTER_INFO = {
         "clusterName": "DoorLock",
         "clusterId": 0x00000101,
         "commands": {
             0x00000000: {
                 "commandId": 0x00000000,
                 "commandName": "LockDoor",
@@ -5800,14 +7616,30 @@
             0x00000027: {
                 "commandId": 0x00000027,
                 "commandName": "UnboltDoor",
                 "args": {
                     "PINCode": "bytes",
                 },
             },
+            0x00000028: {
+                "commandId": 0x00000028,
+                "commandName": "SetAliroReaderConfig",
+                "args": {
+                    "signingKey": "bytes",
+                    "verificationKey": "bytes",
+                    "groupIdentifier": "bytes",
+                    "groupResolvingKey": "bytes",
+                },
+            },
+            0x00000029: {
+                "commandId": 0x00000029,
+                "commandName": "ClearAliroReaderConfig",
+                "args": {
+                },
+            },
         },
         "attributes": {
             0x00000000: {
                 "attributeName": "LockState",
                 "attributeId": 0x00000000,
                 "type": "int",
                 "reportable": True,
@@ -6036,14 +7868,68 @@
             0x00000035: {
                 "attributeName": "ExpiringUserTimeout",
                 "attributeId": 0x00000035,
                 "type": "int",
                 "reportable": True,
                 "writable": True,
             },
+            0x00000080: {
+                "attributeName": "AliroReaderVerificationKey",
+                "attributeId": 0x00000080,
+                "type": "bytes",
+                "reportable": True,
+            },
+            0x00000081: {
+                "attributeName": "AliroReaderGroupIdentifier",
+                "attributeId": 0x00000081,
+                "type": "bytes",
+                "reportable": True,
+            },
+            0x00000082: {
+                "attributeName": "AliroReaderGroupSubIdentifier",
+                "attributeId": 0x00000082,
+                "type": "bytes",
+                "reportable": True,
+            },
+            0x00000083: {
+                "attributeName": "AliroExpeditedTransactionSupportedProtocolVersions",
+                "attributeId": 0x00000083,
+                "type": "bytes",
+                "reportable": True,
+            },
+            0x00000084: {
+                "attributeName": "AliroGroupResolvingKey",
+                "attributeId": 0x00000084,
+                "type": "bytes",
+                "reportable": True,
+            },
+            0x00000085: {
+                "attributeName": "AliroSupportedBLEUWBProtocolVersions",
+                "attributeId": 0x00000085,
+                "type": "bytes",
+                "reportable": True,
+            },
+            0x00000086: {
+                "attributeName": "AliroBLEAdvertisingVersion",
+                "attributeId": 0x00000086,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000087: {
+                "attributeName": "NumberOfAliroCredentialIssuerKeysSupported",
+                "attributeId": 0x00000087,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000088: {
+                "attributeName": "NumberOfAliroEndpointKeysSupported",
+                "attributeId": 0x00000088,
+                "type": "int",
+                "reportable": True,
+            },
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
                 "type": "int",
                 "reportable": True,
             },
             0x0000FFF9: {
@@ -6625,15 +8511,15 @@
             0x00000001: {
                 "commandId": 0x00000001,
                 "commandName": "SetWeeklySchedule",
                 "args": {
                     "numberOfTransitionsForSequence": "int",
                     "dayOfWeekForSequence": "int",
                     "modeForSequence": "int",
-                    "transitions": "ThermostatScheduleTransition",
+                    "transitions": "WeeklyScheduleTransitionStruct",
                 },
             },
             0x00000002: {
                 "commandId": 0x00000002,
                 "commandName": "GetWeeklySchedule",
                 "args": {
                     "daysToReturn": "int",
@@ -6642,14 +8528,61 @@
             },
             0x00000003: {
                 "commandId": 0x00000003,
                 "commandName": "ClearWeeklySchedule",
                 "args": {
                 },
             },
+            0x00000005: {
+                "commandId": 0x00000005,
+                "commandName": "SetActiveScheduleRequest",
+                "args": {
+                    "scheduleHandle": "bytes",
+                },
+            },
+            0x00000006: {
+                "commandId": 0x00000006,
+                "commandName": "SetActivePresetRequest",
+                "args": {
+                    "presetHandle": "bytes",
+                    "delayMinutes": "int",
+                },
+            },
+            0x00000007: {
+                "commandId": 0x00000007,
+                "commandName": "StartPresetsSchedulesEditRequest",
+                "args": {
+                    "timeoutSeconds": "int",
+                },
+            },
+            0x00000008: {
+                "commandId": 0x00000008,
+                "commandName": "CancelPresetsSchedulesEditRequest",
+                "args": {
+                },
+            },
+            0x00000009: {
+                "commandId": 0x00000009,
+                "commandName": "CommitPresetsSchedulesRequest",
+                "args": {
+                },
+            },
+            0x0000000A: {
+                "commandId": 0x0000000A,
+                "commandName": "CancelSetActivePresetRequest",
+                "args": {
+                },
+            },
+            0x0000000B: {
+                "commandId": 0x0000000B,
+                "commandName": "SetTemperatureSetpointHoldPolicy",
+                "args": {
+                    "temperatureSetpointHoldPolicy": "int",
+                },
+            },
         },
         "attributes": {
             0x00000000: {
                 "attributeName": "LocalTemperature",
                 "attributeId": 0x00000000,
                 "type": "int",
                 "reportable": True,
@@ -6965,14 +8898,100 @@
             0x00000047: {
                 "attributeName": "ACCapacityformat",
                 "attributeId": 0x00000047,
                 "type": "int",
                 "reportable": True,
                 "writable": True,
             },
+            0x00000048: {
+                "attributeName": "PresetTypes",
+                "attributeId": 0x00000048,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000049: {
+                "attributeName": "ScheduleTypes",
+                "attributeId": 0x00000049,
+                "type": "",
+                "reportable": True,
+            },
+            0x0000004A: {
+                "attributeName": "NumberOfPresets",
+                "attributeId": 0x0000004A,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000004B: {
+                "attributeName": "NumberOfSchedules",
+                "attributeId": 0x0000004B,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000004C: {
+                "attributeName": "NumberOfScheduleTransitions",
+                "attributeId": 0x0000004C,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000004D: {
+                "attributeName": "NumberOfScheduleTransitionPerDay",
+                "attributeId": 0x0000004D,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000004E: {
+                "attributeName": "ActivePresetHandle",
+                "attributeId": 0x0000004E,
+                "type": "bytes",
+                "reportable": True,
+            },
+            0x0000004F: {
+                "attributeName": "ActiveScheduleHandle",
+                "attributeId": 0x0000004F,
+                "type": "bytes",
+                "reportable": True,
+            },
+            0x00000050: {
+                "attributeName": "Presets",
+                "attributeId": 0x00000050,
+                "type": "",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000051: {
+                "attributeName": "Schedules",
+                "attributeId": 0x00000051,
+                "type": "",
+                "reportable": True,
+                "writable": True,
+            },
+            0x00000052: {
+                "attributeName": "PresetsSchedulesEditable",
+                "attributeId": 0x00000052,
+                "type": "bool",
+                "reportable": True,
+            },
+            0x00000053: {
+                "attributeName": "TemperatureSetpointHoldPolicy",
+                "attributeId": 0x00000053,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000054: {
+                "attributeName": "SetpointHoldExpiryTimestamp",
+                "attributeId": 0x00000054,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000055: {
+                "attributeName": "QueuedPreset",
+                "attributeId": 0x00000055,
+                "type": "",
+                "reportable": True,
+            },
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
                 "type": "int",
                 "reportable": True,
             },
             0x0000FFF9: {
@@ -7030,15 +9049,14 @@
                 "writable": True,
             },
             0x00000001: {
                 "attributeName": "FanModeSequence",
                 "attributeId": 0x00000001,
                 "type": "int",
                 "reportable": True,
-                "writable": True,
             },
             0x00000002: {
                 "attributeName": "PercentSetting",
                 "attributeId": 0x00000002,
                 "type": "int",
                 "reportable": True,
                 "writable": True,
@@ -9525,14 +11543,20 @@
         "attributes": {
             0x00000000: {
                 "attributeName": "MACAddress",
                 "attributeId": 0x00000000,
                 "type": "str",
                 "reportable": True,
             },
+            0x00000001: {
+                "attributeName": "LinkLocalAddress",
+                "attributeId": 0x00000001,
+                "type": "bytes",
+                "reportable": True,
+            },
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
                 "type": "int",
                 "reportable": True,
             },
             0x0000FFF9: {
@@ -9589,14 +11613,47 @@
             0x00000003: {
                 "commandId": 0x00000003,
                 "commandName": "SkipChannel",
                 "args": {
                     "count": "int",
                 },
             },
+            0x00000004: {
+                "commandId": 0x00000004,
+                "commandName": "GetProgramGuide",
+                "args": {
+                    "startTime": "int",
+                    "endTime": "int",
+                    "channelList": "ChannelInfoStruct",
+                    "pageToken": "PageTokenStruct",
+                    "recordingFlag": "int",
+                    "externalIDList": "AdditionalInfoStruct",
+                    "data": "bytes",
+                },
+            },
+            0x00000006: {
+                "commandId": 0x00000006,
+                "commandName": "RecordProgram",
+                "args": {
+                    "programIdentifier": "str",
+                    "shouldRecordSeries": "bool",
+                    "externalIDList": "AdditionalInfoStruct",
+                    "data": "bytes",
+                },
+            },
+            0x00000007: {
+                "commandId": 0x00000007,
+                "commandName": "CancelRecordProgram",
+                "args": {
+                    "programIdentifier": "str",
+                    "shouldRecordSeries": "bool",
+                    "externalIDList": "AdditionalInfoStruct",
+                    "data": "bytes",
+                },
+            },
         },
         "attributes": {
             0x00000000: {
                 "attributeName": "ChannelList",
                 "attributeId": 0x00000000,
                 "type": "",
                 "reportable": True,
@@ -9755,20 +11812,22 @@
                 "args": {
                 },
             },
             0x00000006: {
                 "commandId": 0x00000006,
                 "commandName": "Rewind",
                 "args": {
+                    "audioAdvanceUnmuted": "bool",
                 },
             },
             0x00000007: {
                 "commandId": 0x00000007,
                 "commandName": "FastForward",
                 "args": {
+                    "audioAdvanceUnmuted": "bool",
                 },
             },
             0x00000008: {
                 "commandId": 0x00000008,
                 "commandName": "SkipForward",
                 "args": {
                     "deltaPositionMilliseconds": "int",
@@ -9784,14 +11843,35 @@
             0x0000000B: {
                 "commandId": 0x0000000B,
                 "commandName": "Seek",
                 "args": {
                     "position": "int",
                 },
             },
+            0x0000000C: {
+                "commandId": 0x0000000C,
+                "commandName": "ActivateAudioTrack",
+                "args": {
+                    "trackID": "str",
+                    "audioOutputIndex": "int",
+                },
+            },
+            0x0000000D: {
+                "commandId": 0x0000000D,
+                "commandName": "ActivateTextTrack",
+                "args": {
+                    "trackID": "str",
+                },
+            },
+            0x0000000E: {
+                "commandId": 0x0000000E,
+                "commandName": "DeactivateTextTrack",
+                "args": {
+                },
+            },
         },
         "attributes": {
             0x00000000: {
                 "attributeName": "CurrentState",
                 "attributeId": 0x00000000,
                 "type": "int",
                 "reportable": True,
@@ -9828,14 +11908,38 @@
             },
             0x00000006: {
                 "attributeName": "SeekRangeStart",
                 "attributeId": 0x00000006,
                 "type": "int",
                 "reportable": True,
             },
+            0x00000007: {
+                "attributeName": "ActiveAudioTrack",
+                "attributeId": 0x00000007,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000008: {
+                "attributeName": "AvailableAudioTracks",
+                "attributeId": 0x00000008,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000009: {
+                "attributeName": "ActiveTextTrack",
+                "attributeId": 0x00000009,
+                "type": "",
+                "reportable": True,
+            },
+            0x0000000A: {
+                "attributeName": "AvailableTextTracks",
+                "attributeId": 0x0000000A,
+                "type": "",
+                "reportable": True,
+            },
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
                 "type": "int",
                 "reportable": True,
             },
             0x0000FFF9: {
@@ -10061,14 +12165,16 @@
             0x00000000: {
                 "commandId": 0x00000000,
                 "commandName": "LaunchContent",
                 "args": {
                     "search": "ContentSearchStruct",
                     "autoPlay": "bool",
                     "data": "str",
+                    "playbackPreferences": "PlaybackPreferencesStruct",
+                    "useCurrentContext": "bool",
                 },
             },
             0x00000001: {
                 "commandId": 0x00000001,
                 "commandName": "LaunchURL",
                 "args": {
                     "contentURL": "str",
@@ -10085,15 +12191,14 @@
                 "reportable": True,
             },
             0x00000001: {
                 "attributeName": "SupportedStreamingProtocols",
                 "attributeId": 0x00000001,
                 "type": "int",
                 "reportable": True,
-                "writable": True,
             },
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
                 "type": "int",
                 "reportable": True,
             },
@@ -10235,15 +12340,14 @@
                 "reportable": True,
             },
             0x00000001: {
                 "attributeName": "CurrentApp",
                 "attributeId": 0x00000001,
                 "type": "",
                 "reportable": True,
-                "writable": True,
             },
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
                 "type": "int",
                 "reportable": True,
             },
@@ -10384,20 +12488,233 @@
             },
             0x00000002: {
                 "commandId": 0x00000002,
                 "commandName": "Login",
                 "args": {
                     "tempAccountIdentifier": "str",
                     "setupPIN": "str",
+                    "node": "int",
                 },
             },
             0x00000003: {
                 "commandId": 0x00000003,
                 "commandName": "Logout",
                 "args": {
+                    "node": "int",
+                },
+            },
+        },
+        "attributes": {
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _CONTENT_CONTROL_CLUSTER_INFO = {
+        "clusterName": "ContentControl",
+        "clusterId": 0x0000050F,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "UpdatePIN",
+                "args": {
+                    "oldPIN": "str",
+                    "newPIN": "str",
+                },
+            },
+            0x00000001: {
+                "commandId": 0x00000001,
+                "commandName": "ResetPIN",
+                "args": {
+                },
+            },
+            0x00000003: {
+                "commandId": 0x00000003,
+                "commandName": "Enable",
+                "args": {
+                },
+            },
+            0x00000004: {
+                "commandId": 0x00000004,
+                "commandName": "Disable",
+                "args": {
+                },
+            },
+            0x00000005: {
+                "commandId": 0x00000005,
+                "commandName": "AddBonusTime",
+                "args": {
+                    "PINCode": "str",
+                    "bonusTime": "int",
+                },
+            },
+            0x00000006: {
+                "commandId": 0x00000006,
+                "commandName": "SetScreenDailyTime",
+                "args": {
+                    "screenTime": "int",
+                },
+            },
+            0x00000007: {
+                "commandId": 0x00000007,
+                "commandName": "BlockUnratedContent",
+                "args": {
+                },
+            },
+            0x00000008: {
+                "commandId": 0x00000008,
+                "commandName": "UnblockUnratedContent",
+                "args": {
+                },
+            },
+            0x00000009: {
+                "commandId": 0x00000009,
+                "commandName": "SetOnDemandRatingThreshold",
+                "args": {
+                    "rating": "str",
+                },
+            },
+            0x0000000A: {
+                "commandId": 0x0000000A,
+                "commandName": "SetScheduledContentRatingThreshold",
+                "args": {
+                    "rating": "str",
+                },
+            },
+        },
+        "attributes": {
+            0x00000000: {
+                "attributeName": "Enabled",
+                "attributeId": 0x00000000,
+                "type": "bool",
+                "reportable": True,
+            },
+            0x00000001: {
+                "attributeName": "OnDemandRatings",
+                "attributeId": 0x00000001,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000002: {
+                "attributeName": "OnDemandRatingThreshold",
+                "attributeId": 0x00000002,
+                "type": "str",
+                "reportable": True,
+            },
+            0x00000003: {
+                "attributeName": "ScheduledContentRatings",
+                "attributeId": 0x00000003,
+                "type": "",
+                "reportable": True,
+            },
+            0x00000004: {
+                "attributeName": "ScheduledContentRatingThreshold",
+                "attributeId": 0x00000004,
+                "type": "str",
+                "reportable": True,
+            },
+            0x00000005: {
+                "attributeName": "ScreenDailyTime",
+                "attributeId": 0x00000005,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000006: {
+                "attributeName": "RemainingScreenTime",
+                "attributeId": 0x00000006,
+                "type": "int",
+                "reportable": True,
+            },
+            0x00000007: {
+                "attributeName": "BlockUnrated",
+                "attributeId": 0x00000007,
+                "type": "bool",
+                "reportable": True,
+            },
+            0x0000FFF8: {
+                "attributeName": "GeneratedCommandList",
+                "attributeId": 0x0000FFF8,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFF9: {
+                "attributeName": "AcceptedCommandList",
+                "attributeId": 0x0000FFF9,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFA: {
+                "attributeName": "EventList",
+                "attributeId": 0x0000FFFA,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFB: {
+                "attributeName": "AttributeList",
+                "attributeId": 0x0000FFFB,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFC: {
+                "attributeName": "FeatureMap",
+                "attributeId": 0x0000FFFC,
+                "type": "int",
+                "reportable": True,
+            },
+            0x0000FFFD: {
+                "attributeName": "ClusterRevision",
+                "attributeId": 0x0000FFFD,
+                "type": "int",
+                "reportable": True,
+            },
+        },
+    }
+    _CONTENT_APP_OBSERVER_CLUSTER_INFO = {
+        "clusterName": "ContentAppObserver",
+        "clusterId": 0x00000510,
+        "commands": {
+            0x00000000: {
+                "commandId": 0x00000000,
+                "commandName": "ContentAppMessage",
+                "args": {
+                    "data": "str",
+                    "encodingHint": "str",
                 },
             },
         },
         "attributes": {
             0x0000FFF8: {
                 "attributeName": "GeneratedCommandList",
                 "attributeId": 0x0000FFF8,
@@ -11440,14 +13757,39 @@
             0x00000015: {
                 "commandId": 0x00000015,
                 "commandName": "TestEmitTestFabricScopedEventRequest",
                 "args": {
                     "arg1": "int",
                 },
             },
+            0x00000016: {
+                "commandId": 0x00000016,
+                "commandName": "TestBatchHelperRequest",
+                "args": {
+                    "sleepBeforeResponseTimeMs": "int",
+                    "sizeOfResponseBuffer": "int",
+                    "fillCharacter": "int",
+                },
+            },
+            0x00000017: {
+                "commandId": 0x00000017,
+                "commandName": "TestSecondBatchHelperRequest",
+                "args": {
+                    "sleepBeforeResponseTimeMs": "int",
+                    "sizeOfResponseBuffer": "int",
+                    "fillCharacter": "int",
+                },
+            },
+            0xFFF200AA: {
+                "commandId": 0xFFF200AA,
+                "commandName": "TestDifferentVendorMeiRequest",
+                "args": {
+                    "arg1": "int",
+                },
+            },
         },
         "attributes": {
             0x00000000: {
                 "attributeName": "Boolean",
                 "attributeId": 0x00000000,
                 "type": "bool",
                 "reportable": True,
@@ -12052,14 +14394,21 @@
             },
             0x0000FFFD: {
                 "attributeName": "ClusterRevision",
                 "attributeId": 0x0000FFFD,
                 "type": "int",
                 "reportable": True,
             },
+            0xFFF24F01: {
+                "attributeName": "MeiInt8u",
+                "attributeId": 0xFFF24F01,
+                "type": "int",
+                "reportable": True,
+                "writable": True,
+            },
         },
     }
     _FAULT_INJECTION_CLUSTER_INFO = {
         "clusterName": "FaultInjection",
         "clusterId": 0xFFF1FC06,
         "commands": {
             0x00000000: {
@@ -12187,15 +14536,14 @@
             },
         },
     }
 
     _CLUSTER_ID_DICT = {
         0x00000003: _IDENTIFY_CLUSTER_INFO,
         0x00000004: _GROUPS_CLUSTER_INFO,
-        0x00000005: _SCENES_CLUSTER_INFO,
         0x00000006: _ON_OFF_CLUSTER_INFO,
         0x00000007: _ON_OFF_SWITCH_CONFIGURATION_CLUSTER_INFO,
         0x00000008: _LEVEL_CONTROL_CLUSTER_INFO,
         0x0000000F: _BINARY_INPUT_BASIC_CLUSTER_INFO,
         0x0000001C: _PULSE_WIDTH_MODULATION_CLUSTER_INFO,
         0x0000001D: _DESCRIPTOR_CLUSTER_INFO,
         0x0000001E: _BINDING_CLUSTER_INFO,
@@ -12226,30 +14574,49 @@
         0x00000040: _FIXED_LABEL_CLUSTER_INFO,
         0x00000041: _USER_LABEL_CLUSTER_INFO,
         0x00000042: _PROXY_CONFIGURATION_CLUSTER_INFO,
         0x00000043: _PROXY_DISCOVERY_CLUSTER_INFO,
         0x00000044: _PROXY_VALID_CLUSTER_INFO,
         0x00000045: _BOOLEAN_STATE_CLUSTER_INFO,
         0x00000046: _ICD_MANAGEMENT_CLUSTER_INFO,
+        0x00000047: _TIMER_CLUSTER_INFO,
+        0x00000048: _OVEN_CAVITY_OPERATIONAL_STATE_CLUSTER_INFO,
+        0x00000049: _OVEN_MODE_CLUSTER_INFO,
+        0x0000004A: _LAUNDRY_DRYER_CONTROLS_CLUSTER_INFO,
         0x00000050: _MODE_SELECT_CLUSTER_INFO,
         0x00000051: _LAUNDRY_WASHER_MODE_CLUSTER_INFO,
         0x00000052: _REFRIGERATOR_AND_TEMPERATURE_CONTROLLED_CABINET_MODE_CLUSTER_INFO,
         0x00000053: _LAUNDRY_WASHER_CONTROLS_CLUSTER_INFO,
         0x00000054: _RVC_RUN_MODE_CLUSTER_INFO,
         0x00000055: _RVC_CLEAN_MODE_CLUSTER_INFO,
         0x00000056: _TEMPERATURE_CONTROL_CLUSTER_INFO,
         0x00000057: _REFRIGERATOR_ALARM_CLUSTER_INFO,
         0x00000059: _DISHWASHER_MODE_CLUSTER_INFO,
         0x0000005B: _AIR_QUALITY_CLUSTER_INFO,
         0x0000005C: _SMOKE_CO_ALARM_CLUSTER_INFO,
         0x0000005D: _DISHWASHER_ALARM_CLUSTER_INFO,
+        0x0000005E: _MICROWAVE_OVEN_MODE_CLUSTER_INFO,
+        0x0000005F: _MICROWAVE_OVEN_CONTROL_CLUSTER_INFO,
         0x00000060: _OPERATIONAL_STATE_CLUSTER_INFO,
         0x00000061: _RVC_OPERATIONAL_STATE_CLUSTER_INFO,
+        0x00000062: _SCENES_MANAGEMENT_CLUSTER_INFO,
         0x00000071: _HEPA_FILTER_MONITORING_CLUSTER_INFO,
         0x00000072: _ACTIVATED_CARBON_FILTER_MONITORING_CLUSTER_INFO,
+        0x00000080: _BOOLEAN_STATE_CONFIGURATION_CLUSTER_INFO,
+        0x00000081: _VALVE_CONFIGURATION_AND_CONTROL_CLUSTER_INFO,
+        0x00000090: _ELECTRICAL_POWER_MEASUREMENT_CLUSTER_INFO,
+        0x00000091: _ELECTRICAL_ENERGY_MEASUREMENT_CLUSTER_INFO,
+        0x00000096: _DEMAND_RESPONSE_LOAD_CONTROL_CLUSTER_INFO,
+        0x00000097: _MESSAGES_CLUSTER_INFO,
+        0x00000098: _DEVICE_ENERGY_MANAGEMENT_CLUSTER_INFO,
+        0x00000099: _ENERGY_EVSE_CLUSTER_INFO,
+        0x0000009B: _ENERGY_PREFERENCE_CLUSTER_INFO,
+        0x0000009C: _POWER_TOPOLOGY_CLUSTER_INFO,
+        0x0000009D: _ENERGY_EVSE_MODE_CLUSTER_INFO,
+        0x0000009F: _DEVICE_ENERGY_MANAGEMENT_MODE_CLUSTER_INFO,
         0x00000101: _DOOR_LOCK_CLUSTER_INFO,
         0x00000102: _WINDOW_COVERING_CLUSTER_INFO,
         0x00000103: _BARRIER_CONTROL_CLUSTER_INFO,
         0x00000200: _PUMP_CONFIGURATION_AND_CONTROL_CLUSTER_INFO,
         0x00000201: _THERMOSTAT_CLUSTER_INFO,
         0x00000202: _FAN_CONTROL_CLUSTER_INFO,
         0x00000204: _THERMOSTAT_USER_INTERFACE_CONFIGURATION_CLUSTER_INFO,
@@ -12279,24 +14646,25 @@
         0x00000508: _LOW_POWER_CLUSTER_INFO,
         0x00000509: _KEYPAD_INPUT_CLUSTER_INFO,
         0x0000050A: _CONTENT_LAUNCHER_CLUSTER_INFO,
         0x0000050B: _AUDIO_OUTPUT_CLUSTER_INFO,
         0x0000050C: _APPLICATION_LAUNCHER_CLUSTER_INFO,
         0x0000050D: _APPLICATION_BASIC_CLUSTER_INFO,
         0x0000050E: _ACCOUNT_LOGIN_CLUSTER_INFO,
+        0x0000050F: _CONTENT_CONTROL_CLUSTER_INFO,
+        0x00000510: _CONTENT_APP_OBSERVER_CLUSTER_INFO,
         0x00000B04: _ELECTRICAL_MEASUREMENT_CLUSTER_INFO,
         0xFFF1FC05: _UNIT_TESTING_CLUSTER_INFO,
         0xFFF1FC06: _FAULT_INJECTION_CLUSTER_INFO,
         0xFFF1FC20: _SAMPLE_MEI_CLUSTER_INFO,
     }
 
     _CLUSTER_NAME_DICT = {
         "Identify": _IDENTIFY_CLUSTER_INFO,
         "Groups": _GROUPS_CLUSTER_INFO,
-        "Scenes": _SCENES_CLUSTER_INFO,
         "OnOff": _ON_OFF_CLUSTER_INFO,
         "OnOffSwitchConfiguration": _ON_OFF_SWITCH_CONFIGURATION_CLUSTER_INFO,
         "LevelControl": _LEVEL_CONTROL_CLUSTER_INFO,
         "BinaryInputBasic": _BINARY_INPUT_BASIC_CLUSTER_INFO,
         "PulseWidthModulation": _PULSE_WIDTH_MODULATION_CLUSTER_INFO,
         "Descriptor": _DESCRIPTOR_CLUSTER_INFO,
         "Binding": _BINDING_CLUSTER_INFO,
@@ -12327,30 +14695,49 @@
         "FixedLabel": _FIXED_LABEL_CLUSTER_INFO,
         "UserLabel": _USER_LABEL_CLUSTER_INFO,
         "ProxyConfiguration": _PROXY_CONFIGURATION_CLUSTER_INFO,
         "ProxyDiscovery": _PROXY_DISCOVERY_CLUSTER_INFO,
         "ProxyValid": _PROXY_VALID_CLUSTER_INFO,
         "BooleanState": _BOOLEAN_STATE_CLUSTER_INFO,
         "IcdManagement": _ICD_MANAGEMENT_CLUSTER_INFO,
+        "Timer": _TIMER_CLUSTER_INFO,
+        "OvenCavityOperationalState": _OVEN_CAVITY_OPERATIONAL_STATE_CLUSTER_INFO,
+        "OvenMode": _OVEN_MODE_CLUSTER_INFO,
+        "LaundryDryerControls": _LAUNDRY_DRYER_CONTROLS_CLUSTER_INFO,
         "ModeSelect": _MODE_SELECT_CLUSTER_INFO,
         "LaundryWasherMode": _LAUNDRY_WASHER_MODE_CLUSTER_INFO,
         "RefrigeratorAndTemperatureControlledCabinetMode": _REFRIGERATOR_AND_TEMPERATURE_CONTROLLED_CABINET_MODE_CLUSTER_INFO,
         "LaundryWasherControls": _LAUNDRY_WASHER_CONTROLS_CLUSTER_INFO,
         "RvcRunMode": _RVC_RUN_MODE_CLUSTER_INFO,
         "RvcCleanMode": _RVC_CLEAN_MODE_CLUSTER_INFO,
         "TemperatureControl": _TEMPERATURE_CONTROL_CLUSTER_INFO,
         "RefrigeratorAlarm": _REFRIGERATOR_ALARM_CLUSTER_INFO,
         "DishwasherMode": _DISHWASHER_MODE_CLUSTER_INFO,
         "AirQuality": _AIR_QUALITY_CLUSTER_INFO,
         "SmokeCoAlarm": _SMOKE_CO_ALARM_CLUSTER_INFO,
         "DishwasherAlarm": _DISHWASHER_ALARM_CLUSTER_INFO,
+        "MicrowaveOvenMode": _MICROWAVE_OVEN_MODE_CLUSTER_INFO,
+        "MicrowaveOvenControl": _MICROWAVE_OVEN_CONTROL_CLUSTER_INFO,
         "OperationalState": _OPERATIONAL_STATE_CLUSTER_INFO,
         "RvcOperationalState": _RVC_OPERATIONAL_STATE_CLUSTER_INFO,
+        "ScenesManagement": _SCENES_MANAGEMENT_CLUSTER_INFO,
         "HepaFilterMonitoring": _HEPA_FILTER_MONITORING_CLUSTER_INFO,
         "ActivatedCarbonFilterMonitoring": _ACTIVATED_CARBON_FILTER_MONITORING_CLUSTER_INFO,
+        "BooleanStateConfiguration": _BOOLEAN_STATE_CONFIGURATION_CLUSTER_INFO,
+        "ValveConfigurationAndControl": _VALVE_CONFIGURATION_AND_CONTROL_CLUSTER_INFO,
+        "ElectricalPowerMeasurement": _ELECTRICAL_POWER_MEASUREMENT_CLUSTER_INFO,
+        "ElectricalEnergyMeasurement": _ELECTRICAL_ENERGY_MEASUREMENT_CLUSTER_INFO,
+        "DemandResponseLoadControl": _DEMAND_RESPONSE_LOAD_CONTROL_CLUSTER_INFO,
+        "Messages": _MESSAGES_CLUSTER_INFO,
+        "DeviceEnergyManagement": _DEVICE_ENERGY_MANAGEMENT_CLUSTER_INFO,
+        "EnergyEvse": _ENERGY_EVSE_CLUSTER_INFO,
+        "EnergyPreference": _ENERGY_PREFERENCE_CLUSTER_INFO,
+        "PowerTopology": _POWER_TOPOLOGY_CLUSTER_INFO,
+        "EnergyEvseMode": _ENERGY_EVSE_MODE_CLUSTER_INFO,
+        "DeviceEnergyManagementMode": _DEVICE_ENERGY_MANAGEMENT_MODE_CLUSTER_INFO,
         "DoorLock": _DOOR_LOCK_CLUSTER_INFO,
         "WindowCovering": _WINDOW_COVERING_CLUSTER_INFO,
         "BarrierControl": _BARRIER_CONTROL_CLUSTER_INFO,
         "PumpConfigurationAndControl": _PUMP_CONFIGURATION_AND_CONTROL_CLUSTER_INFO,
         "Thermostat": _THERMOSTAT_CLUSTER_INFO,
         "FanControl": _FAN_CONTROL_CLUSTER_INFO,
         "ThermostatUserInterfaceConfiguration": _THERMOSTAT_USER_INTERFACE_CONFIGURATION_CLUSTER_INFO,
@@ -12380,14 +14767,16 @@
         "LowPower": _LOW_POWER_CLUSTER_INFO,
         "KeypadInput": _KEYPAD_INPUT_CLUSTER_INFO,
         "ContentLauncher": _CONTENT_LAUNCHER_CLUSTER_INFO,
         "AudioOutput": _AUDIO_OUTPUT_CLUSTER_INFO,
         "ApplicationLauncher": _APPLICATION_LAUNCHER_CLUSTER_INFO,
         "ApplicationBasic": _APPLICATION_BASIC_CLUSTER_INFO,
         "AccountLogin": _ACCOUNT_LOGIN_CLUSTER_INFO,
+        "ContentControl": _CONTENT_CONTROL_CLUSTER_INFO,
+        "ContentAppObserver": _CONTENT_APP_OBSERVER_CLUSTER_INFO,
         "ElectricalMeasurement": _ELECTRICAL_MEASUREMENT_CLUSTER_INFO,
         "UnitTesting": _UNIT_TESTING_CLUSTER_INFO,
         "FaultInjection": _FAULT_INJECTION_CLUSTER_INFO,
         "SampleMei": _SAMPLE_MEI_CLUSTER_INFO,
     }
 
     def __init__(self, chipstack):
```

## chip/clusters/ClusterObjects.py

```diff
@@ -203,34 +203,54 @@
         return cls.FromDict(data=cls.descriptor.TLVToDict(data))
 
     @ChipUtility.classproperty
     def descriptor(cls):
         raise NotImplementedError()
 
 
+# The below dictionaries will be filled dynamically
+# and are used for quick lookup/mapping from cluster/attribute id to the correct class
+ALL_CLUSTERS = {}
+ALL_ATTRIBUTES = {}
+# These need to be separate because there can be overlap in command ids for commands and responses.
+ALL_ACCEPTED_COMMANDS = {}
+ALL_GENERATED_COMMANDS = {}
+
+
 class ClusterCommand(ClusterObject):
+    def __init_subclass__(cls, *args, **kwargs) -> None:
+        """Register a subclass."""
+        super().__init_subclass__(*args, **kwargs)
+        try:
+            if cls.is_client:
+                if cls.cluster_id not in ALL_ACCEPTED_COMMANDS:
+                    ALL_ACCEPTED_COMMANDS[cls.cluster_id] = {}
+                ALL_ACCEPTED_COMMANDS[cls.cluster_id][cls.command_id] = cls
+            else:
+                if cls.cluster_id not in ALL_GENERATED_COMMANDS:
+                    ALL_GENERATED_COMMANDS[cls.cluster_id] = {}
+                ALL_GENERATED_COMMANDS[cls.cluster_id][cls.command_id] = cls
+        except NotImplementedError:
+            # handle case where the ClusterAttribute class is not (fully) subclassed
+            # and accessing the id property throws a NotImplementedError.
+            pass
+
     @ChipUtility.classproperty
     def cluster_id(self) -> int:
         raise NotImplementedError()
 
     @ChipUtility.classproperty
     def command_id(self) -> int:
         raise NotImplementedError()
 
     @ChipUtility.classproperty
     def must_use_timed_invoke(cls) -> bool:
         return False
 
 
-# The below dictionaries will be filled dynamically
-# and are used for quick lookup/mapping from cluster/attribute id to the correct class
-ALL_CLUSTERS = {}
-ALL_ATTRIBUTES = {}
-
-
 class Cluster(ClusterObject):
     '''
     When send read requests with returnClusterObject=True, we will set the data_version property of the object.
     Otherwise the [endpoint][cluster][Clusters.DataVersion] will be set to the DataVersion of the cluster.
 
     For data_version, we do not make it a real property so we can distinguish it with real attributes internally,
     especially the TLV decoding logic. Also ThreadNetworkDiagnostics has an attribute with the same name so we
@@ -277,18 +297,19 @@
     and use it for actual encode / decode routine to save lines of code.
     '''
 
     def __init_subclass__(cls, *args, **kwargs) -> None:
         """Register a subclass."""
         super().__init_subclass__(*args, **kwargs)
         try:
-            if cls.cluster_id not in ALL_ATTRIBUTES:
-                ALL_ATTRIBUTES[cls.cluster_id] = {}
-            # register this clusterattribute in the ALL_ATTRIBUTES dict for quick lookups
-            ALL_ATTRIBUTES[cls.cluster_id][cls.attribute_id] = cls
+            if cls.standard_attribute:
+                if cls.cluster_id not in ALL_ATTRIBUTES:
+                    ALL_ATTRIBUTES[cls.cluster_id] = {}
+                # register this clusterattribute in the ALL_ATTRIBUTES dict for quick lookups
+                ALL_ATTRIBUTES[cls.cluster_id][cls.attribute_id] = cls
         except NotImplementedError:
             # handle case where the ClusterAttribute class is not (fully) subclassed
             # and accessing the id property throws a NotImplementedError.
             pass
 
     @classmethod
     def ToTLV(cls, tag: Union[int, None], value):
@@ -322,14 +343,18 @@
         raise NotImplementedError()
 
     @ChipUtility.classproperty
     def must_use_timed_write(cls) -> bool:
         return False
 
     @ChipUtility.classproperty
+    def standard_attribute(cls) -> bool:
+        return True
+
+    @ChipUtility.classproperty
     def _cluster_object(cls) -> ClusterObject:
         return make_dataclass('InternalClass',
                               [
                                   ('Value', cls.attribute_type.Type,
                                    field(default=None)),
                                   ('descriptor', ClassVar[ClusterObjectDescriptor],
                                    field(
```

## chip/clusters/Objects.py

```diff
@@ -579,705 +579,14 @@
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
 
 @dataclass
-class Scenes(Cluster):
-    id: typing.ClassVar[int] = 0x00000005
-
-    @ChipUtility.classproperty
-    def descriptor(cls) -> ClusterObjectDescriptor:
-        return ClusterObjectDescriptor(
-            Fields=[
-                ClusterObjectFieldDescriptor(Label="sceneCount", Tag=0x00000000, Type=uint),
-                ClusterObjectFieldDescriptor(Label="currentScene", Tag=0x00000001, Type=uint),
-                ClusterObjectFieldDescriptor(Label="currentGroup", Tag=0x00000002, Type=uint),
-                ClusterObjectFieldDescriptor(Label="sceneValid", Tag=0x00000003, Type=bool),
-                ClusterObjectFieldDescriptor(Label="nameSupport", Tag=0x00000004, Type=uint),
-                ClusterObjectFieldDescriptor(Label="lastConfiguredBy", Tag=0x00000005, Type=typing.Union[None, Nullable, uint]),
-                ClusterObjectFieldDescriptor(Label="sceneTableSize", Tag=0x00000006, Type=uint),
-                ClusterObjectFieldDescriptor(Label="remainingCapacity", Tag=0x00000007, Type=uint),
-                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
-                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
-            ])
-
-    sceneCount: 'uint' = None
-    currentScene: 'uint' = None
-    currentGroup: 'uint' = None
-    sceneValid: 'bool' = None
-    nameSupport: 'uint' = None
-    lastConfiguredBy: 'typing.Union[None, Nullable, uint]' = None
-    sceneTableSize: 'uint' = None
-    remainingCapacity: 'uint' = None
-    generatedCommandList: 'typing.List[uint]' = None
-    acceptedCommandList: 'typing.List[uint]' = None
-    eventList: 'typing.List[uint]' = None
-    attributeList: 'typing.List[uint]' = None
-    featureMap: 'uint' = None
-    clusterRevision: 'uint' = None
-
-    class Bitmaps:
-        class Feature(IntFlag):
-            kSceneNames = 0x1
-            kExplicit = 0x2
-            kTableSize = 0x4
-            kFabricScenes = 0x8
-
-        class ScenesCopyMode(IntFlag):
-            kCopyAllScenes = 0x1
-
-    class Structs:
-        @dataclass
-        class AttributeValuePair(ClusterObject):
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="attributeID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="attributeValue", Tag=1, Type=uint),
-                    ])
-
-            attributeID: 'uint' = 0
-            attributeValue: 'uint' = 0
-
-        @dataclass
-        class ExtensionFieldSet(ClusterObject):
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="clusterID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="attributeValueList", Tag=1, Type=typing.List[Scenes.Structs.AttributeValuePair]),
-                    ])
-
-            clusterID: 'uint' = 0
-            attributeValueList: 'typing.List[Scenes.Structs.AttributeValuePair]' = field(default_factory=lambda: [])
-
-    class Commands:
-        @dataclass
-        class AddScene(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000000
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'AddSceneResponse'
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="transitionTime", Tag=2, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneName", Tag=3, Type=str),
-                        ClusterObjectFieldDescriptor(Label="extensionFieldSets", Tag=4, Type=typing.List[Scenes.Structs.ExtensionFieldSet]),
-                    ])
-
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-            transitionTime: 'uint' = 0
-            sceneName: 'str' = ""
-            extensionFieldSets: 'typing.List[Scenes.Structs.ExtensionFieldSet]' = field(default_factory=lambda: [])
-
-        @dataclass
-        class AddSceneResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000000
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=2, Type=uint),
-                    ])
-
-            status: 'uint' = 0
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-
-        @dataclass
-        class ViewScene(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000001
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'ViewSceneResponse'
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
-                    ])
-
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-
-        @dataclass
-        class ViewSceneResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000001
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=2, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="transitionTime", Tag=3, Type=typing.Optional[uint]),
-                        ClusterObjectFieldDescriptor(Label="sceneName", Tag=4, Type=typing.Optional[str]),
-                        ClusterObjectFieldDescriptor(Label="extensionFieldSets", Tag=5, Type=typing.Optional[typing.List[Scenes.Structs.ExtensionFieldSet]]),
-                    ])
-
-            status: 'uint' = 0
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-            transitionTime: 'typing.Optional[uint]' = None
-            sceneName: 'typing.Optional[str]' = None
-            extensionFieldSets: 'typing.Optional[typing.List[Scenes.Structs.ExtensionFieldSet]]' = None
-
-        @dataclass
-        class RemoveScene(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000002
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'RemoveSceneResponse'
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
-                    ])
-
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-
-        @dataclass
-        class RemoveSceneResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000002
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=2, Type=uint),
-                    ])
-
-            status: 'uint' = 0
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-
-        @dataclass
-        class RemoveAllScenes(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000003
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'RemoveAllScenesResponse'
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
-                    ])
-
-            groupID: 'uint' = 0
-
-        @dataclass
-        class RemoveAllScenesResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000003
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
-                    ])
-
-            status: 'uint' = 0
-            groupID: 'uint' = 0
-
-        @dataclass
-        class StoreScene(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000004
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'StoreSceneResponse'
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
-                    ])
-
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-
-        @dataclass
-        class StoreSceneResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000004
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=2, Type=uint),
-                    ])
-
-            status: 'uint' = 0
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-
-        @dataclass
-        class RecallScene(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000005
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = None
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="transitionTime", Tag=2, Type=typing.Union[None, Nullable, uint]),
-                    ])
-
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-            transitionTime: 'typing.Union[None, Nullable, uint]' = None
-
-        @dataclass
-        class GetSceneMembership(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000006
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'GetSceneMembershipResponse'
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
-                    ])
-
-            groupID: 'uint' = 0
-
-        @dataclass
-        class GetSceneMembershipResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000006
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="capacity", Tag=1, Type=typing.Union[Nullable, uint]),
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=2, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneList", Tag=3, Type=typing.Optional[typing.List[uint]]),
-                    ])
-
-            status: 'uint' = 0
-            capacity: 'typing.Union[Nullable, uint]' = NullValue
-            groupID: 'uint' = 0
-            sceneList: 'typing.Optional[typing.List[uint]]' = None
-
-        @dataclass
-        class EnhancedAddScene(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000040
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'EnhancedAddSceneResponse'
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="transitionTime", Tag=2, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneName", Tag=3, Type=str),
-                        ClusterObjectFieldDescriptor(Label="extensionFieldSets", Tag=4, Type=typing.List[Scenes.Structs.ExtensionFieldSet]),
-                    ])
-
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-            transitionTime: 'uint' = 0
-            sceneName: 'str' = ""
-            extensionFieldSets: 'typing.List[Scenes.Structs.ExtensionFieldSet]' = field(default_factory=lambda: [])
-
-        @dataclass
-        class EnhancedAddSceneResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000040
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=2, Type=uint),
-                    ])
-
-            status: 'uint' = 0
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-
-        @dataclass
-        class EnhancedViewScene(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000041
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'EnhancedViewSceneResponse'
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
-                    ])
-
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-
-        @dataclass
-        class EnhancedViewSceneResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000041
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=2, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="transitionTime", Tag=3, Type=typing.Optional[uint]),
-                        ClusterObjectFieldDescriptor(Label="sceneName", Tag=4, Type=typing.Optional[str]),
-                        ClusterObjectFieldDescriptor(Label="extensionFieldSets", Tag=5, Type=typing.Optional[typing.List[Scenes.Structs.ExtensionFieldSet]]),
-                    ])
-
-            status: 'uint' = 0
-            groupID: 'uint' = 0
-            sceneID: 'uint' = 0
-            transitionTime: 'typing.Optional[uint]' = None
-            sceneName: 'typing.Optional[str]' = None
-            extensionFieldSets: 'typing.Optional[typing.List[Scenes.Structs.ExtensionFieldSet]]' = None
-
-        @dataclass
-        class CopyScene(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000042
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'CopySceneResponse'
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="mode", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="groupIdentifierFrom", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneIdentifierFrom", Tag=2, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="groupIdentifierTo", Tag=3, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneIdentifierTo", Tag=4, Type=uint),
-                    ])
-
-            mode: 'uint' = 0
-            groupIdentifierFrom: 'uint' = 0
-            sceneIdentifierFrom: 'uint' = 0
-            groupIdentifierTo: 'uint' = 0
-            sceneIdentifierTo: 'uint' = 0
-
-        @dataclass
-        class CopySceneResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000005
-            command_id: typing.ClassVar[int] = 0x00000042
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="groupIdentifierFrom", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="sceneIdentifierFrom", Tag=2, Type=uint),
-                    ])
-
-            status: 'uint' = 0
-            groupIdentifierFrom: 'uint' = 0
-            sceneIdentifierFrom: 'uint' = 0
-
-    class Attributes:
-        @dataclass
-        class SceneCount(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000000
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
-
-            value: 'uint' = 0
-
-        @dataclass
-        class CurrentScene(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000001
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
-
-            value: 'uint' = 0
-
-        @dataclass
-        class CurrentGroup(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000002
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
-
-            value: 'uint' = 0
-
-        @dataclass
-        class SceneValid(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000003
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=bool)
-
-            value: 'bool' = False
-
-        @dataclass
-        class NameSupport(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000004
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
-
-            value: 'uint' = 0
-
-        @dataclass
-        class LastConfiguredBy(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
-
-            value: 'typing.Union[None, Nullable, uint]' = None
-
-        @dataclass
-        class SceneTableSize(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000006
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
-
-            value: 'uint' = 0
-
-        @dataclass
-        class RemainingCapacity(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000007
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
-
-            value: 'uint' = 0
-
-        @dataclass
-        class GeneratedCommandList(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x0000FFF8
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
-
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
-
-        @dataclass
-        class AcceptedCommandList(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x0000FFF9
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
-
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
-
-        @dataclass
-        class EventList(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x0000FFFA
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
-
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
-
-        @dataclass
-        class AttributeList(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x0000FFFB
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
-
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
-
-        @dataclass
-        class FeatureMap(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x0000FFFC
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
-
-            value: 'uint' = 0
-
-        @dataclass
-        class ClusterRevision(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000005
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x0000FFFD
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
-
-            value: 'uint' = 0
-
-
-@dataclass
 class OnOff(Cluster):
     id: typing.ClassVar[int] = 0x00000006
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
@@ -1344,14 +653,15 @@
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 3,
 
     class Bitmaps:
         class Feature(IntFlag):
             kLighting = 0x1
             kDeadFrontBehavior = 0x2
+            kOffOnly = 0x4
 
         class OnOffControlBitmap(IntFlag):
             kAcceptOnlyWhenOn = 0x1
 
     class Commands:
         @dataclass
         class Off(ClusterCommand):
@@ -1826,39 +1136,39 @@
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class MoveMode(MatterIntEnum):
+        class MoveModeEnum(MatterIntEnum):
             kUp = 0x00
             kDown = 0x01
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 2,
 
-        class StepMode(MatterIntEnum):
+        class StepModeEnum(MatterIntEnum):
             kUp = 0x00
             kDown = 0x01
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 2,
 
     class Bitmaps:
         class Feature(IntFlag):
             kOnOff = 0x1
             kLighting = 0x2
             kFrequency = 0x4
 
-        class LevelControlOptions(IntFlag):
+        class OptionsBitmap(IntFlag):
             kExecuteIfOff = 0x1
             kCoupleColorTempToLevel = 0x2
 
     class Commands:
         @dataclass
         class MoveToLevel(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000008
@@ -1888,21 +1198,21 @@
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="moveMode", Tag=0, Type=LevelControl.Enums.MoveMode),
+                        ClusterObjectFieldDescriptor(Label="moveMode", Tag=0, Type=LevelControl.Enums.MoveModeEnum),
                         ClusterObjectFieldDescriptor(Label="rate", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="optionsMask", Tag=2, Type=uint),
                         ClusterObjectFieldDescriptor(Label="optionsOverride", Tag=3, Type=uint),
                     ])
 
-            moveMode: 'LevelControl.Enums.MoveMode' = 0
+            moveMode: 'LevelControl.Enums.MoveModeEnum' = 0
             rate: 'typing.Union[Nullable, uint]' = NullValue
             optionsMask: 'uint' = 0
             optionsOverride: 'uint' = 0
 
         @dataclass
         class Step(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000008
@@ -1910,22 +1220,22 @@
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="stepMode", Tag=0, Type=LevelControl.Enums.StepMode),
+                        ClusterObjectFieldDescriptor(Label="stepMode", Tag=0, Type=LevelControl.Enums.StepModeEnum),
                         ClusterObjectFieldDescriptor(Label="stepSize", Tag=1, Type=uint),
                         ClusterObjectFieldDescriptor(Label="transitionTime", Tag=2, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="optionsMask", Tag=3, Type=uint),
                         ClusterObjectFieldDescriptor(Label="optionsOverride", Tag=4, Type=uint),
                     ])
 
-            stepMode: 'LevelControl.Enums.StepMode' = 0
+            stepMode: 'LevelControl.Enums.StepModeEnum' = 0
             stepSize: 'uint' = 0
             transitionTime: 'typing.Union[Nullable, uint]' = NullValue
             optionsMask: 'uint' = 0
             optionsOverride: 'uint' = 0
 
         @dataclass
         class Stop(ClusterCommand):
@@ -1974,21 +1284,21 @@
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="moveMode", Tag=0, Type=LevelControl.Enums.MoveMode),
+                        ClusterObjectFieldDescriptor(Label="moveMode", Tag=0, Type=LevelControl.Enums.MoveModeEnum),
                         ClusterObjectFieldDescriptor(Label="rate", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="optionsMask", Tag=2, Type=uint),
                         ClusterObjectFieldDescriptor(Label="optionsOverride", Tag=3, Type=uint),
                     ])
 
-            moveMode: 'LevelControl.Enums.MoveMode' = 0
+            moveMode: 'LevelControl.Enums.MoveModeEnum' = 0
             rate: 'typing.Union[Nullable, uint]' = NullValue
             optionsMask: 'uint' = 0
             optionsOverride: 'uint' = 0
 
         @dataclass
         class StepWithOnOff(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000008
@@ -1996,22 +1306,22 @@
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="stepMode", Tag=0, Type=LevelControl.Enums.StepMode),
+                        ClusterObjectFieldDescriptor(Label="stepMode", Tag=0, Type=LevelControl.Enums.StepModeEnum),
                         ClusterObjectFieldDescriptor(Label="stepSize", Tag=1, Type=uint),
                         ClusterObjectFieldDescriptor(Label="transitionTime", Tag=2, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="optionsMask", Tag=3, Type=uint),
                         ClusterObjectFieldDescriptor(Label="optionsOverride", Tag=4, Type=uint),
                     ])
 
-            stepMode: 'LevelControl.Enums.StepMode' = 0
+            stepMode: 'LevelControl.Enums.StepModeEnum' = 0
             stepSize: 'uint' = 0
             transitionTime: 'typing.Union[Nullable, uint]' = NullValue
             optionsMask: 'uint' = 0
             optionsOverride: 'uint' = 0
 
         @dataclass
         class StopWithOnOff(ClusterCommand):
@@ -4100,14 +3410,16 @@
                 ClusterObjectFieldDescriptor(Label="productLabel", Tag=0x0000000E, Type=typing.Optional[str]),
                 ClusterObjectFieldDescriptor(Label="serialNumber", Tag=0x0000000F, Type=typing.Optional[str]),
                 ClusterObjectFieldDescriptor(Label="localConfigDisabled", Tag=0x00000010, Type=typing.Optional[bool]),
                 ClusterObjectFieldDescriptor(Label="reachable", Tag=0x00000011, Type=typing.Optional[bool]),
                 ClusterObjectFieldDescriptor(Label="uniqueID", Tag=0x00000012, Type=typing.Optional[str]),
                 ClusterObjectFieldDescriptor(Label="capabilityMinima", Tag=0x00000013, Type=BasicInformation.Structs.CapabilityMinimaStruct),
                 ClusterObjectFieldDescriptor(Label="productAppearance", Tag=0x00000014, Type=typing.Optional[BasicInformation.Structs.ProductAppearanceStruct]),
+                ClusterObjectFieldDescriptor(Label="specificationVersion", Tag=0x00000015, Type=uint),
+                ClusterObjectFieldDescriptor(Label="maxPathsPerInvoke", Tag=0x00000016, Type=uint),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
@@ -4129,14 +3441,16 @@
     productLabel: 'typing.Optional[str]' = None
     serialNumber: 'typing.Optional[str]' = None
     localConfigDisabled: 'typing.Optional[bool]' = None
     reachable: 'typing.Optional[bool]' = None
     uniqueID: 'typing.Optional[str]' = None
     capabilityMinima: 'BasicInformation.Structs.CapabilityMinimaStruct' = None
     productAppearance: 'typing.Optional[BasicInformation.Structs.ProductAppearanceStruct]' = None
+    specificationVersion: 'uint' = None
+    maxPathsPerInvoke: 'uint' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
@@ -4557,14 +3871,46 @@
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Optional[BasicInformation.Structs.ProductAppearanceStruct])
 
             value: 'typing.Optional[BasicInformation.Structs.ProductAppearanceStruct]' = None
 
         @dataclass
+        class SpecificationVersion(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000028
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000015
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class MaxPathsPerInvoke(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000028
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000016
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000028
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
@@ -5541,23 +4887,25 @@
             kHebrew = 0x05
             kIndian = 0x06
             kIslamic = 0x07
             kJapanese = 0x08
             kKorean = 0x09
             kPersian = 0x0A
             kTaiwanese = 0x0B
+            kUseActiveLocale = 0xFF
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 12,
 
         class HourFormatEnum(MatterIntEnum):
             k12hr = 0x00
             k24hr = 0x01
+            kUseActiveLocale = 0xFF
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 2,
 
     class Bitmaps:
@@ -7464,42 +6812,48 @@
             kUnknownEnumValue = 6,
 
     class Bitmaps:
         class Feature(IntFlag):
             kWiFiNetworkInterface = 0x1
             kThreadNetworkInterface = 0x2
             kEthernetNetworkInterface = 0x4
+            kPerDeviceCredentials = 0x8
 
         class ThreadCapabilitiesBitmap(IntFlag):
             kIsBorderRouterCapable = 0x1
             kIsRouterCapable = 0x2
             kIsSleepyEndDeviceCapable = 0x4
             kIsFullThreadDevice = 0x8
             kIsSynchronizedSleepyEndDeviceCapable = 0x10
 
         class WiFiSecurityBitmap(IntFlag):
             kUnencrypted = 0x1
             kWep = 0x2
             kWpaPersonal = 0x4
             kWpa2Personal = 0x8
             kWpa3Personal = 0x10
+            kWpa3MatterPdc = 0x20
 
     class Structs:
         @dataclass
         class NetworkInfoStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="networkID", Tag=0, Type=bytes),
                         ClusterObjectFieldDescriptor(Label="connected", Tag=1, Type=bool),
+                        ClusterObjectFieldDescriptor(Label="networkIdentifier", Tag=2, Type=typing.Union[None, Nullable, bytes]),
+                        ClusterObjectFieldDescriptor(Label="clientIdentifier", Tag=3, Type=typing.Union[None, Nullable, bytes]),
                     ])
 
             networkID: 'bytes' = b""
             connected: 'bool' = False
+            networkIdentifier: 'typing.Union[None, Nullable, bytes]' = None
+            clientIdentifier: 'typing.Union[None, Nullable, bytes]' = None
 
         @dataclass
         class ThreadInterfaceScanResultStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
@@ -7594,19 +6948,25 @@
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="ssid", Tag=0, Type=bytes),
                         ClusterObjectFieldDescriptor(Label="credentials", Tag=1, Type=bytes),
                         ClusterObjectFieldDescriptor(Label="breadcrumb", Tag=2, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="networkIdentity", Tag=3, Type=typing.Optional[bytes]),
+                        ClusterObjectFieldDescriptor(Label="clientIdentifier", Tag=4, Type=typing.Optional[bytes]),
+                        ClusterObjectFieldDescriptor(Label="possessionNonce", Tag=5, Type=typing.Optional[bytes]),
                     ])
 
             ssid: 'bytes' = b""
             credentials: 'bytes' = b""
             breadcrumb: 'typing.Optional[uint]' = None
+            networkIdentity: 'typing.Optional[bytes]' = None
+            clientIdentifier: 'typing.Optional[bytes]' = None
+            possessionNonce: 'typing.Optional[bytes]' = None
 
         @dataclass
         class AddOrUpdateThreadNetwork(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000031
             command_id: typing.ClassVar[int] = 0x00000003
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'NetworkConfigResponse'
@@ -7650,19 +7010,23 @@
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="networkingStatus", Tag=0, Type=NetworkCommissioning.Enums.NetworkCommissioningStatusEnum),
                         ClusterObjectFieldDescriptor(Label="debugText", Tag=1, Type=typing.Optional[str]),
                         ClusterObjectFieldDescriptor(Label="networkIndex", Tag=2, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="clientIdentity", Tag=3, Type=typing.Optional[bytes]),
+                        ClusterObjectFieldDescriptor(Label="possessionSignature", Tag=4, Type=typing.Optional[bytes]),
                     ])
 
             networkingStatus: 'NetworkCommissioning.Enums.NetworkCommissioningStatusEnum' = 0
             debugText: 'typing.Optional[str]' = None
             networkIndex: 'typing.Optional[uint]' = None
+            clientIdentity: 'typing.Optional[bytes]' = None
+            possessionSignature: 'typing.Optional[bytes]' = None
 
         @dataclass
         class ConnectNetwork(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000031
             command_id: typing.ClassVar[int] = 0x00000006
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'ConnectNetworkResponse'
@@ -7714,14 +7078,50 @@
                         ClusterObjectFieldDescriptor(Label="breadcrumb", Tag=2, Type=typing.Optional[uint]),
                     ])
 
             networkID: 'bytes' = b""
             networkIndex: 'uint' = 0
             breadcrumb: 'typing.Optional[uint]' = None
 
+        @dataclass
+        class QueryIdentity(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000031
+            command_id: typing.ClassVar[int] = 0x00000009
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'QueryIdentityResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="keyIdentifier", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="possessionNonce", Tag=1, Type=typing.Optional[bytes]),
+                    ])
+
+            keyIdentifier: 'bytes' = b""
+            possessionNonce: 'typing.Optional[bytes]' = None
+
+        @dataclass
+        class QueryIdentityResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000031
+            command_id: typing.ClassVar[int] = 0x0000000A
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="identity", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="possessionSignature", Tag=1, Type=typing.Optional[bytes]),
+                    ])
+
+            identity: 'bytes' = b""
+            possessionSignature: 'typing.Optional[bytes]' = None
+
     class Attributes:
         @dataclass
         class MaxNetworks(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000031
 
@@ -8201,15 +7601,14 @@
                 ClusterObjectFieldDescriptor(Label="upTime", Tag=0x00000002, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="totalOperationalHours", Tag=0x00000003, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="bootReason", Tag=0x00000004, Type=typing.Optional[GeneralDiagnostics.Enums.BootReasonEnum]),
                 ClusterObjectFieldDescriptor(Label="activeHardwareFaults", Tag=0x00000005, Type=typing.Optional[typing.List[GeneralDiagnostics.Enums.HardwareFaultEnum]]),
                 ClusterObjectFieldDescriptor(Label="activeRadioFaults", Tag=0x00000006, Type=typing.Optional[typing.List[GeneralDiagnostics.Enums.RadioFaultEnum]]),
                 ClusterObjectFieldDescriptor(Label="activeNetworkFaults", Tag=0x00000007, Type=typing.Optional[typing.List[GeneralDiagnostics.Enums.NetworkFaultEnum]]),
                 ClusterObjectFieldDescriptor(Label="testEventTriggersEnabled", Tag=0x00000008, Type=bool),
-                ClusterObjectFieldDescriptor(Label="averageWearCount", Tag=0x00000009, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
@@ -8219,15 +7618,14 @@
     upTime: 'typing.Optional[uint]' = None
     totalOperationalHours: 'typing.Optional[uint]' = None
     bootReason: 'typing.Optional[GeneralDiagnostics.Enums.BootReasonEnum]' = None
     activeHardwareFaults: 'typing.Optional[typing.List[GeneralDiagnostics.Enums.HardwareFaultEnum]]' = None
     activeRadioFaults: 'typing.Optional[typing.List[GeneralDiagnostics.Enums.RadioFaultEnum]]' = None
     activeNetworkFaults: 'typing.Optional[typing.List[GeneralDiagnostics.Enums.NetworkFaultEnum]]' = None
     testEventTriggersEnabled: 'bool' = None
-    averageWearCount: 'typing.Optional[uint]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
@@ -8297,14 +7695,18 @@
             kEthernetFault = 0x06
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 7,
 
+    class Bitmaps:
+        class Feature(IntFlag):
+            kDataModelTest = 0x1
+
     class Structs:
         @dataclass
         class NetworkInterface(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
@@ -8342,14 +7744,81 @@
                         ClusterObjectFieldDescriptor(Label="enableKey", Tag=0, Type=bytes),
                         ClusterObjectFieldDescriptor(Label="eventTrigger", Tag=1, Type=uint),
                     ])
 
             enableKey: 'bytes' = b""
             eventTrigger: 'uint' = 0
 
+        @dataclass
+        class TimeSnapshot(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000033
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'TimeSnapshotResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class TimeSnapshotResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000033
+            command_id: typing.ClassVar[int] = 0x00000002
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="systemTimeMs", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="posixTimeMs", Tag=1, Type=typing.Union[Nullable, uint]),
+                    ])
+
+            systemTimeMs: 'uint' = 0
+            posixTimeMs: 'typing.Union[Nullable, uint]' = NullValue
+
+        @dataclass
+        class PayloadTestRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000033
+            command_id: typing.ClassVar[int] = 0x00000003
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'PayloadTestResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="enableKey", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="count", Tag=2, Type=uint),
+                    ])
+
+            enableKey: 'bytes' = b""
+            value: 'uint' = 0
+            count: 'uint' = 0
+
+        @dataclass
+        class PayloadTestResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000033
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="payload", Tag=0, Type=bytes),
+                    ])
+
+            payload: 'bytes' = b""
+
     class Attributes:
         @dataclass
         class NetworkInterfaces(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000033
 
@@ -8488,30 +7957,14 @@
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=bool)
 
             value: 'bool' = False
 
         @dataclass
-        class AverageWearCount(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000033
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000009
-
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
-
-            value: 'typing.Optional[uint]' = None
-
-        @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000033
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
@@ -8716,15 +8169,15 @@
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Bitmaps:
         class Feature(IntFlag):
-            kWaterMarks = 0x1
+            kWatermarks = 0x1
 
     class Structs:
         @dataclass
         class ThreadMetricsStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
@@ -10858,19 +10311,19 @@
             def event_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="associationFailure", Tag=0, Type=WiFiNetworkDiagnostics.Enums.AssociationFailureCauseEnum),
+                        ClusterObjectFieldDescriptor(Label="associationFailureCause", Tag=0, Type=WiFiNetworkDiagnostics.Enums.AssociationFailureCauseEnum),
                         ClusterObjectFieldDescriptor(Label="status", Tag=1, Type=uint),
                     ])
 
-            associationFailure: 'WiFiNetworkDiagnostics.Enums.AssociationFailureCauseEnum' = 0
+            associationFailureCause: 'WiFiNetworkDiagnostics.Enums.AssociationFailureCauseEnum' = 0
             status: 'uint' = 0
 
         @dataclass
         class ConnectionStatus(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000036
@@ -14703,14 +14156,15 @@
                 ClusterObjectFieldDescriptor(Label="activeModeDuration", Tag=0x00000001, Type=uint),
                 ClusterObjectFieldDescriptor(Label="activeModeThreshold", Tag=0x00000002, Type=uint),
                 ClusterObjectFieldDescriptor(Label="registeredClients", Tag=0x00000003, Type=typing.Optional[typing.List[IcdManagement.Structs.MonitoringRegistrationStruct]]),
                 ClusterObjectFieldDescriptor(Label="ICDCounter", Tag=0x00000004, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="clientsSupportedPerFabric", Tag=0x00000005, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="userActiveModeTriggerHint", Tag=0x00000006, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="userActiveModeTriggerInstruction", Tag=0x00000007, Type=typing.Optional[str]),
+                ClusterObjectFieldDescriptor(Label="operatingMode", Tag=0x00000008, Type=typing.Optional[IcdManagement.Enums.OperatingModeEnum]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
@@ -14719,21 +14173,32 @@
     activeModeDuration: 'uint' = None
     activeModeThreshold: 'uint' = None
     registeredClients: 'typing.Optional[typing.List[IcdManagement.Structs.MonitoringRegistrationStruct]]' = None
     ICDCounter: 'typing.Optional[uint]' = None
     clientsSupportedPerFabric: 'typing.Optional[uint]' = None
     userActiveModeTriggerHint: 'typing.Optional[uint]' = None
     userActiveModeTriggerInstruction: 'typing.Optional[str]' = None
+    operatingMode: 'typing.Optional[IcdManagement.Enums.OperatingModeEnum]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
+    class Enums:
+        class OperatingModeEnum(MatterIntEnum):
+            kSit = 0x00
+            kLit = 0x01
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 2,
+
     class Bitmaps:
         class Feature(IntFlag):
             kCheckInProtocolSupport = 0x1
             kUserActiveModeTrigger = 0x2
             kLongIdleTimeSupport = 0x4
 
         class UserActiveModeTriggerBitmap(IntFlag):
@@ -14829,22 +14294,41 @@
             verificationKey: 'typing.Optional[bytes]' = None
 
         @dataclass
         class StayActiveRequest(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000046
             command_id: typing.ClassVar[int] = 0x00000003
             is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'StayActiveResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="stayActiveDuration", Tag=0, Type=uint),
+                    ])
+
+            stayActiveDuration: 'uint' = 0
+
+        @dataclass
+        class StayActiveResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000046
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = False
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="promisedActiveDuration", Tag=0, Type=uint),
                     ])
 
+            promisedActiveDuration: 'uint' = 0
+
     class Attributes:
         @dataclass
         class IdleModeDuration(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000046
 
@@ -14967,14 +14451,30 @@
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Optional[str])
 
             value: 'typing.Optional[str]' = None
 
         @dataclass
+        class OperatingMode(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000046
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000008
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[IcdManagement.Enums.OperatingModeEnum])
+
+            value: 'typing.Optional[IcdManagement.Enums.OperatingModeEnum]' = None
+
+        @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000046
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
@@ -15064,14 +14564,1107 @@
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
 
 @dataclass
+class Timer(Cluster):
+    id: typing.ClassVar[int] = 0x00000047
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="setTime", Tag=0x00000000, Type=uint),
+                ClusterObjectFieldDescriptor(Label="timeRemaining", Tag=0x00000001, Type=uint),
+                ClusterObjectFieldDescriptor(Label="timerState", Tag=0x00000002, Type=Timer.Enums.TimerStatusEnum),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    setTime: 'uint' = None
+    timeRemaining: 'uint' = None
+    timerState: 'Timer.Enums.TimerStatusEnum' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class TimerStatusEnum(MatterIntEnum):
+            kRunning = 0x00
+            kPaused = 0x01
+            kExpired = 0x02
+            kReady = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kReset = 0x1
+
+    class Commands:
+        @dataclass
+        class SetTimer(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000047
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="newTime", Tag=0, Type=uint),
+                    ])
+
+            newTime: 'uint' = 0
+
+        @dataclass
+        class ResetTimer(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000047
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class AddTime(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000047
+            command_id: typing.ClassVar[int] = 0x00000002
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="additionalTime", Tag=0, Type=uint),
+                    ])
+
+            additionalTime: 'uint' = 0
+
+        @dataclass
+        class ReduceTime(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000047
+            command_id: typing.ClassVar[int] = 0x00000003
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="timeReduction", Tag=0, Type=uint),
+                    ])
+
+            timeReduction: 'uint' = 0
+
+    class Attributes:
+        @dataclass
+        class SetTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000047
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class TimeRemaining(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000047
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class TimerState(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000047
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=Timer.Enums.TimerStatusEnum)
+
+            value: 'Timer.Enums.TimerStatusEnum' = 0
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000047
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000047
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000047
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000047
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000047
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000047
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class OvenCavityOperationalState(Cluster):
+    id: typing.ClassVar[int] = 0x00000048
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="phaseList", Tag=0x00000000, Type=typing.Union[Nullable, typing.List[str]]),
+                ClusterObjectFieldDescriptor(Label="currentPhase", Tag=0x00000001, Type=typing.Union[Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="countdownTime", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="operationalStateList", Tag=0x00000003, Type=typing.List[OvenCavityOperationalState.Structs.OperationalStateStruct]),
+                ClusterObjectFieldDescriptor(Label="operationalState", Tag=0x00000004, Type=OvenCavityOperationalState.Enums.OperationalStateEnum),
+                ClusterObjectFieldDescriptor(Label="operationalError", Tag=0x00000005, Type=OvenCavityOperationalState.Structs.ErrorStateStruct),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    phaseList: 'typing.Union[Nullable, typing.List[str]]' = None
+    currentPhase: 'typing.Union[Nullable, uint]' = None
+    countdownTime: 'typing.Union[None, Nullable, uint]' = None
+    operationalStateList: 'typing.List[OvenCavityOperationalState.Structs.OperationalStateStruct]' = None
+    operationalState: 'OvenCavityOperationalState.Enums.OperationalStateEnum' = None
+    operationalError: 'OvenCavityOperationalState.Structs.ErrorStateStruct' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class ErrorStateEnum(MatterIntEnum):
+            kNoError = 0x00
+            kUnableToStartOrResume = 0x01
+            kUnableToCompleteOperation = 0x02
+            kCommandInvalidInState = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
+
+        class OperationalStateEnum(MatterIntEnum):
+            kStopped = 0x00
+            kRunning = 0x01
+            kPaused = 0x02
+            kError = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
+
+    class Structs:
+        @dataclass
+        class ErrorStateStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="errorStateID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="errorStateLabel", Tag=1, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="errorStateDetails", Tag=2, Type=typing.Optional[str]),
+                    ])
+
+            errorStateID: 'uint' = 0
+            errorStateLabel: 'typing.Optional[str]' = None
+            errorStateDetails: 'typing.Optional[str]' = None
+
+        @dataclass
+        class OperationalStateStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="operationalStateID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="operationalStateLabel", Tag=1, Type=typing.Optional[str]),
+                    ])
+
+            operationalStateID: 'uint' = 0
+            operationalStateLabel: 'typing.Optional[str]' = None
+
+    class Commands:
+        @dataclass
+        class Pause(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000048
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class Stop(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000048
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class Start(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000048
+            command_id: typing.ClassVar[int] = 0x00000002
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class Resume(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000048
+            command_id: typing.ClassVar[int] = 0x00000003
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class OperationalCommandResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000048
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="commandResponseState", Tag=0, Type=OvenCavityOperationalState.Structs.ErrorStateStruct),
+                    ])
+
+            commandResponseState: 'OvenCavityOperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: OvenCavityOperationalState.Structs.ErrorStateStruct())
+
+    class Attributes:
+        @dataclass
+        class PhaseList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, typing.List[str]])
+
+            value: 'typing.Union[Nullable, typing.List[str]]' = NullValue
+
+        @dataclass
+        class CurrentPhase(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
+
+            value: 'typing.Union[Nullable, uint]' = NullValue
+
+        @dataclass
+        class CountdownTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class OperationalStateList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[OvenCavityOperationalState.Structs.OperationalStateStruct])
+
+            value: 'typing.List[OvenCavityOperationalState.Structs.OperationalStateStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class OperationalState(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=OvenCavityOperationalState.Enums.OperationalStateEnum)
+
+            value: 'OvenCavityOperationalState.Enums.OperationalStateEnum' = 0
+
+        @dataclass
+        class OperationalError(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=OvenCavityOperationalState.Structs.ErrorStateStruct)
+
+            value: 'OvenCavityOperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: OvenCavityOperationalState.Structs.ErrorStateStruct())
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+    class Events:
+        @dataclass
+        class OperationalError(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="errorState", Tag=0, Type=OvenCavityOperationalState.Structs.ErrorStateStruct),
+                    ])
+
+            errorState: 'OvenCavityOperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: OvenCavityOperationalState.Structs.ErrorStateStruct())
+
+        @dataclass
+        class OperationCompletion(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="completionErrorCode", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="totalOperationalTime", Tag=1, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="pausedTime", Tag=2, Type=typing.Union[None, Nullable, uint]),
+                    ])
+
+            completionErrorCode: 'uint' = 0
+            totalOperationalTime: 'typing.Union[None, Nullable, uint]' = None
+            pausedTime: 'typing.Union[None, Nullable, uint]' = None
+
+
+@dataclass
+class OvenMode(Cluster):
+    id: typing.ClassVar[int] = 0x00000049
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="supportedModes", Tag=0x00000000, Type=typing.List[OvenMode.Structs.ModeOptionStruct]),
+                ClusterObjectFieldDescriptor(Label="currentMode", Tag=0x00000001, Type=uint),
+                ClusterObjectFieldDescriptor(Label="startUpMode", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="onMode", Tag=0x00000003, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    supportedModes: 'typing.List[OvenMode.Structs.ModeOptionStruct]' = None
+    currentMode: 'uint' = None
+    startUpMode: 'typing.Union[None, Nullable, uint]' = None
+    onMode: 'typing.Union[None, Nullable, uint]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class ModeTag(MatterIntEnum):
+            kBake = 0x4000
+            kConvection = 0x4001
+            kGrill = 0x4002
+            kRoast = 0x4003
+            kClean = 0x4004
+            kConvectionBake = 0x4005
+            kConvectionRoast = 0x4006
+            kWarming = 0x4007
+            kProofing = 0x4008
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 0,
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kOnOff = 0x1
+
+    class Structs:
+        @dataclass
+        class ModeTagStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="mfgCode", Tag=0, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=uint),
+                    ])
+
+            mfgCode: 'typing.Optional[uint]' = None
+            value: 'uint' = 0
+
+        @dataclass
+        class ModeOptionStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="label", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="mode", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="modeTags", Tag=2, Type=typing.List[OvenMode.Structs.ModeTagStruct]),
+                    ])
+
+            label: 'str' = ""
+            mode: 'uint' = 0
+            modeTags: 'typing.List[OvenMode.Structs.ModeTagStruct]' = field(default_factory=lambda: [])
+
+    class Commands:
+        @dataclass
+        class ChangeToMode(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000049
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'ChangeToModeResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="newMode", Tag=0, Type=uint),
+                    ])
+
+            newMode: 'uint' = 0
+
+        @dataclass
+        class ChangeToModeResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000049
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="statusText", Tag=1, Type=typing.Optional[str]),
+                    ])
+
+            status: 'uint' = 0
+            statusText: 'typing.Optional[str]' = None
+
+    class Attributes:
+        @dataclass
+        class SupportedModes(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000049
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[OvenMode.Structs.ModeOptionStruct])
+
+            value: 'typing.List[OvenMode.Structs.ModeOptionStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class CurrentMode(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000049
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class StartUpMode(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000049
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class OnMode(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000049
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000049
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000049
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000049
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000049
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000049
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000049
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class LaundryDryerControls(Cluster):
+    id: typing.ClassVar[int] = 0x0000004A
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="supportedDrynessLevels", Tag=0x00000000, Type=typing.List[LaundryDryerControls.Enums.DrynessLevelEnum]),
+                ClusterObjectFieldDescriptor(Label="selectedDrynessLevel", Tag=0x00000001, Type=typing.Union[Nullable, LaundryDryerControls.Enums.DrynessLevelEnum]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    supportedDrynessLevels: 'typing.List[LaundryDryerControls.Enums.DrynessLevelEnum]' = None
+    selectedDrynessLevel: 'typing.Union[Nullable, LaundryDryerControls.Enums.DrynessLevelEnum]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class DrynessLevelEnum(MatterIntEnum):
+            kLow = 0x00
+            kNormal = 0x01
+            kExtra = 0x02
+            kMax = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
+
+    class Attributes:
+        @dataclass
+        class SupportedDrynessLevels(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000004A
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[LaundryDryerControls.Enums.DrynessLevelEnum])
+
+            value: 'typing.List[LaundryDryerControls.Enums.DrynessLevelEnum]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class SelectedDrynessLevel(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000004A
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, LaundryDryerControls.Enums.DrynessLevelEnum])
+
+            value: 'typing.Union[Nullable, LaundryDryerControls.Enums.DrynessLevelEnum]' = NullValue
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000004A
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000004A
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000004A
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000004A
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000004A
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000004A
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
 class ModeSelect(Cluster):
     id: typing.ClassVar[int] = 0x00000050
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
@@ -16106,37 +16699,36 @@
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
                 ClusterObjectFieldDescriptor(Label="supportedModes", Tag=0x00000000, Type=typing.List[RvcRunMode.Structs.ModeOptionStruct]),
                 ClusterObjectFieldDescriptor(Label="currentMode", Tag=0x00000001, Type=uint),
-                ClusterObjectFieldDescriptor(Label="onMode", Tag=0x00000003, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
 
     supportedModes: 'typing.List[RvcRunMode.Structs.ModeOptionStruct]' = None
     currentMode: 'uint' = None
-    onMode: 'typing.Union[None, Nullable, uint]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
         class ModeTag(MatterIntEnum):
             kIdle = 0x4000
             kCleaning = 0x4001
+            kMapping = 0x4002
             # kUnknownEnumValue intentionally not defined. This enum never goes
             # through DataModel::Decode, likely because it is a part of a derived
             # cluster. As a result having kUnknownEnumValue in this enum is error
             # prone, and was removed. See
             # src/app/common/templates/config-data.yaml.
 
         class StatusCode(MatterIntEnum):
@@ -16152,15 +16744,15 @@
             # through DataModel::Decode, likely because it is a part of a derived
             # cluster. As a result having kUnknownEnumValue in this enum is error
             # prone, and was removed. See
             # src/app/common/templates/config-data.yaml.
 
     class Bitmaps:
         class Feature(IntFlag):
-            kOnOff = 0x1
+            kNoFeatures = 0x0
 
     class Structs:
         @dataclass
         class ModeTagStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
@@ -16198,88 +16790,5267 @@
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="newMode", Tag=0, Type=uint),
                     ])
 
-            newMode: 'uint' = 0
+            newMode: 'uint' = 0
+
+        @dataclass
+        class ChangeToModeResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000054
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="statusText", Tag=1, Type=typing.Optional[str]),
+                    ])
+
+            status: 'uint' = 0
+            statusText: 'typing.Optional[str]' = None
+
+    class Attributes:
+        @dataclass
+        class SupportedModes(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000054
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[RvcRunMode.Structs.ModeOptionStruct])
+
+            value: 'typing.List[RvcRunMode.Structs.ModeOptionStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class CurrentMode(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000054
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000054
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000054
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000054
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000054
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000054
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000054
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class RvcCleanMode(Cluster):
+    id: typing.ClassVar[int] = 0x00000055
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="supportedModes", Tag=0x00000000, Type=typing.List[RvcCleanMode.Structs.ModeOptionStruct]),
+                ClusterObjectFieldDescriptor(Label="currentMode", Tag=0x00000001, Type=uint),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    supportedModes: 'typing.List[RvcCleanMode.Structs.ModeOptionStruct]' = None
+    currentMode: 'uint' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class ModeTag(MatterIntEnum):
+            kDeepClean = 0x4000
+            kVacuum = 0x4001
+            kMop = 0x4002
+            # kUnknownEnumValue intentionally not defined. This enum never goes
+            # through DataModel::Decode, likely because it is a part of a derived
+            # cluster. As a result having kUnknownEnumValue in this enum is error
+            # prone, and was removed. See
+            # src/app/common/templates/config-data.yaml.
+
+        class StatusCode(MatterIntEnum):
+            kCleaningInProgress = 0x40
+            # kUnknownEnumValue intentionally not defined. This enum never goes
+            # through DataModel::Decode, likely because it is a part of a derived
+            # cluster. As a result having kUnknownEnumValue in this enum is error
+            # prone, and was removed. See
+            # src/app/common/templates/config-data.yaml.
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kNoFeatures = 0x0
+
+    class Structs:
+        @dataclass
+        class ModeTagStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="mfgCode", Tag=0, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=uint),
+                    ])
+
+            mfgCode: 'typing.Optional[uint]' = None
+            value: 'uint' = 0
+
+        @dataclass
+        class ModeOptionStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="label", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="mode", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="modeTags", Tag=2, Type=typing.List[RvcCleanMode.Structs.ModeTagStruct]),
+                    ])
+
+            label: 'str' = ""
+            mode: 'uint' = 0
+            modeTags: 'typing.List[RvcCleanMode.Structs.ModeTagStruct]' = field(default_factory=lambda: [])
+
+    class Commands:
+        @dataclass
+        class ChangeToMode(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000055
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'ChangeToModeResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="newMode", Tag=0, Type=uint),
+                    ])
+
+            newMode: 'uint' = 0
+
+        @dataclass
+        class ChangeToModeResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000055
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="statusText", Tag=1, Type=typing.Optional[str]),
+                    ])
+
+            status: 'uint' = 0
+            statusText: 'typing.Optional[str]' = None
+
+    class Attributes:
+        @dataclass
+        class SupportedModes(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000055
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[RvcCleanMode.Structs.ModeOptionStruct])
+
+            value: 'typing.List[RvcCleanMode.Structs.ModeOptionStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class CurrentMode(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000055
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000055
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000055
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000055
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000055
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000055
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000055
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class TemperatureControl(Cluster):
+    id: typing.ClassVar[int] = 0x00000056
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="temperatureSetpoint", Tag=0x00000000, Type=typing.Optional[int]),
+                ClusterObjectFieldDescriptor(Label="minTemperature", Tag=0x00000001, Type=typing.Optional[int]),
+                ClusterObjectFieldDescriptor(Label="maxTemperature", Tag=0x00000002, Type=typing.Optional[int]),
+                ClusterObjectFieldDescriptor(Label="step", Tag=0x00000003, Type=typing.Optional[int]),
+                ClusterObjectFieldDescriptor(Label="selectedTemperatureLevel", Tag=0x00000004, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="supportedTemperatureLevels", Tag=0x00000005, Type=typing.Optional[typing.List[str]]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    temperatureSetpoint: 'typing.Optional[int]' = None
+    minTemperature: 'typing.Optional[int]' = None
+    maxTemperature: 'typing.Optional[int]' = None
+    step: 'typing.Optional[int]' = None
+    selectedTemperatureLevel: 'typing.Optional[uint]' = None
+    supportedTemperatureLevels: 'typing.Optional[typing.List[str]]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kTemperatureNumber = 0x1
+            kTemperatureLevel = 0x2
+            kTemperatureStep = 0x4
+
+    class Commands:
+        @dataclass
+        class SetTemperature(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000056
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="targetTemperature", Tag=0, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="targetTemperatureLevel", Tag=1, Type=typing.Optional[uint]),
+                    ])
+
+            targetTemperature: 'typing.Optional[int]' = None
+            targetTemperatureLevel: 'typing.Optional[uint]' = None
+
+    class Attributes:
+        @dataclass
+        class TemperatureSetpoint(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[int])
+
+            value: 'typing.Optional[int]' = None
+
+        @dataclass
+        class MinTemperature(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[int])
+
+            value: 'typing.Optional[int]' = None
+
+        @dataclass
+        class MaxTemperature(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[int])
+
+            value: 'typing.Optional[int]' = None
+
+        @dataclass
+        class Step(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[int])
+
+            value: 'typing.Optional[int]' = None
+
+        @dataclass
+        class SelectedTemperatureLevel(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class SupportedTemperatureLevels(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[str]])
+
+            value: 'typing.Optional[typing.List[str]]' = None
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000056
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class RefrigeratorAlarm(Cluster):
+    id: typing.ClassVar[int] = 0x00000057
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="mask", Tag=0x00000000, Type=uint),
+                ClusterObjectFieldDescriptor(Label="state", Tag=0x00000002, Type=uint),
+                ClusterObjectFieldDescriptor(Label="supported", Tag=0x00000003, Type=uint),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    mask: 'uint' = None
+    state: 'uint' = None
+    supported: 'uint' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Bitmaps:
+        class AlarmBitmap(IntFlag):
+            kDoorOpen = 0x1
+
+    class Attributes:
+        @dataclass
+        class Mask(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000057
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class State(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000057
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class Supported(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000057
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000057
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000057
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000057
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000057
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000057
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000057
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+    class Events:
+        @dataclass
+        class Notify(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000057
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="active", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="inactive", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="state", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="mask", Tag=3, Type=uint),
+                    ])
+
+            active: 'uint' = 0
+            inactive: 'uint' = 0
+            state: 'uint' = 0
+            mask: 'uint' = 0
+
+
+@dataclass
+class DishwasherMode(Cluster):
+    id: typing.ClassVar[int] = 0x00000059
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="supportedModes", Tag=0x00000000, Type=typing.List[DishwasherMode.Structs.ModeOptionStruct]),
+                ClusterObjectFieldDescriptor(Label="currentMode", Tag=0x00000001, Type=uint),
+                ClusterObjectFieldDescriptor(Label="startUpMode", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="onMode", Tag=0x00000003, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    supportedModes: 'typing.List[DishwasherMode.Structs.ModeOptionStruct]' = None
+    currentMode: 'uint' = None
+    startUpMode: 'typing.Union[None, Nullable, uint]' = None
+    onMode: 'typing.Union[None, Nullable, uint]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class ModeTag(MatterIntEnum):
+            kNormal = 0x4000
+            kHeavy = 0x4001
+            kLight = 0x4002
+            # kUnknownEnumValue intentionally not defined. This enum never goes
+            # through DataModel::Decode, likely because it is a part of a derived
+            # cluster. As a result having kUnknownEnumValue in this enum is error
+            # prone, and was removed. See
+            # src/app/common/templates/config-data.yaml.
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kOnOff = 0x1
+
+    class Structs:
+        @dataclass
+        class ModeTagStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="mfgCode", Tag=0, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=uint),
+                    ])
+
+            mfgCode: 'typing.Optional[uint]' = None
+            value: 'uint' = 0
+
+        @dataclass
+        class ModeOptionStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="label", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="mode", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="modeTags", Tag=2, Type=typing.List[DishwasherMode.Structs.ModeTagStruct]),
+                    ])
+
+            label: 'str' = ""
+            mode: 'uint' = 0
+            modeTags: 'typing.List[DishwasherMode.Structs.ModeTagStruct]' = field(default_factory=lambda: [])
+
+    class Commands:
+        @dataclass
+        class ChangeToMode(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000059
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'ChangeToModeResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="newMode", Tag=0, Type=uint),
+                    ])
+
+            newMode: 'uint' = 0
+
+        @dataclass
+        class ChangeToModeResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000059
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="statusText", Tag=1, Type=typing.Optional[str]),
+                    ])
+
+            status: 'uint' = 0
+            statusText: 'typing.Optional[str]' = None
+
+    class Attributes:
+        @dataclass
+        class SupportedModes(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000059
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[DishwasherMode.Structs.ModeOptionStruct])
+
+            value: 'typing.List[DishwasherMode.Structs.ModeOptionStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class CurrentMode(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000059
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class StartUpMode(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000059
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class OnMode(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000059
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000059
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000059
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000059
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000059
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000059
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000059
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class AirQuality(Cluster):
+    id: typing.ClassVar[int] = 0x0000005B
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="airQuality", Tag=0x00000000, Type=AirQuality.Enums.AirQualityEnum),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    airQuality: 'AirQuality.Enums.AirQualityEnum' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class AirQualityEnum(MatterIntEnum):
+            kUnknown = 0x00
+            kGood = 0x01
+            kFair = 0x02
+            kModerate = 0x03
+            kPoor = 0x04
+            kVeryPoor = 0x05
+            kExtremelyPoor = 0x06
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 7,
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kFair = 0x1
+            kModerate = 0x2
+            kVeryPoor = 0x4
+            kExtremelyPoor = 0x8
+
+    class Attributes:
+        @dataclass
+        class AirQuality(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005B
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=AirQuality.Enums.AirQualityEnum)
+
+            value: 'AirQuality.Enums.AirQualityEnum' = 0
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005B
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005B
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005B
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005B
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005B
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005B
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class SmokeCoAlarm(Cluster):
+    id: typing.ClassVar[int] = 0x0000005C
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="expressedState", Tag=0x00000000, Type=SmokeCoAlarm.Enums.ExpressedStateEnum),
+                ClusterObjectFieldDescriptor(Label="smokeState", Tag=0x00000001, Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]),
+                ClusterObjectFieldDescriptor(Label="COState", Tag=0x00000002, Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]),
+                ClusterObjectFieldDescriptor(Label="batteryAlert", Tag=0x00000003, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
+                ClusterObjectFieldDescriptor(Label="deviceMuted", Tag=0x00000004, Type=typing.Optional[SmokeCoAlarm.Enums.MuteStateEnum]),
+                ClusterObjectFieldDescriptor(Label="testInProgress", Tag=0x00000005, Type=bool),
+                ClusterObjectFieldDescriptor(Label="hardwareFaultAlert", Tag=0x00000006, Type=bool),
+                ClusterObjectFieldDescriptor(Label="endOfServiceAlert", Tag=0x00000007, Type=SmokeCoAlarm.Enums.EndOfServiceEnum),
+                ClusterObjectFieldDescriptor(Label="interconnectSmokeAlarm", Tag=0x00000008, Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]),
+                ClusterObjectFieldDescriptor(Label="interconnectCOAlarm", Tag=0x00000009, Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]),
+                ClusterObjectFieldDescriptor(Label="contaminationState", Tag=0x0000000A, Type=typing.Optional[SmokeCoAlarm.Enums.ContaminationStateEnum]),
+                ClusterObjectFieldDescriptor(Label="smokeSensitivityLevel", Tag=0x0000000B, Type=typing.Optional[SmokeCoAlarm.Enums.SensitivityEnum]),
+                ClusterObjectFieldDescriptor(Label="expiryDate", Tag=0x0000000C, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    expressedState: 'SmokeCoAlarm.Enums.ExpressedStateEnum' = None
+    smokeState: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+    COState: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+    batteryAlert: 'SmokeCoAlarm.Enums.AlarmStateEnum' = None
+    deviceMuted: 'typing.Optional[SmokeCoAlarm.Enums.MuteStateEnum]' = None
+    testInProgress: 'bool' = None
+    hardwareFaultAlert: 'bool' = None
+    endOfServiceAlert: 'SmokeCoAlarm.Enums.EndOfServiceEnum' = None
+    interconnectSmokeAlarm: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+    interconnectCOAlarm: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+    contaminationState: 'typing.Optional[SmokeCoAlarm.Enums.ContaminationStateEnum]' = None
+    smokeSensitivityLevel: 'typing.Optional[SmokeCoAlarm.Enums.SensitivityEnum]' = None
+    expiryDate: 'typing.Optional[uint]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class AlarmStateEnum(MatterIntEnum):
+            kNormal = 0x00
+            kWarning = 0x01
+            kCritical = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 3,
+
+        class ContaminationStateEnum(MatterIntEnum):
+            kNormal = 0x00
+            kLow = 0x01
+            kWarning = 0x02
+            kCritical = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
+
+        class EndOfServiceEnum(MatterIntEnum):
+            kNormal = 0x00
+            kExpired = 0x01
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 2,
+
+        class ExpressedStateEnum(MatterIntEnum):
+            kNormal = 0x00
+            kSmokeAlarm = 0x01
+            kCOAlarm = 0x02
+            kBatteryAlert = 0x03
+            kTesting = 0x04
+            kHardwareFault = 0x05
+            kEndOfService = 0x06
+            kInterconnectSmoke = 0x07
+            kInterconnectCO = 0x08
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 9,
+
+        class MuteStateEnum(MatterIntEnum):
+            kNotMuted = 0x00
+            kMuted = 0x01
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 2,
+
+        class SensitivityEnum(MatterIntEnum):
+            kHigh = 0x00
+            kStandard = 0x01
+            kLow = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 3,
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kSmokeAlarm = 0x1
+            kCoAlarm = 0x2
+
+    class Commands:
+        @dataclass
+        class SelfTestRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000005C
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+    class Attributes:
+        @dataclass
+        class ExpressedState(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=SmokeCoAlarm.Enums.ExpressedStateEnum)
+
+            value: 'SmokeCoAlarm.Enums.ExpressedStateEnum' = 0
+
+        @dataclass
+        class SmokeState(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum])
+
+            value: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+
+        @dataclass
+        class COState(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum])
+
+            value: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+
+        @dataclass
+        class BatteryAlert(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=SmokeCoAlarm.Enums.AlarmStateEnum)
+
+            value: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
+
+        @dataclass
+        class DeviceMuted(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.MuteStateEnum])
+
+            value: 'typing.Optional[SmokeCoAlarm.Enums.MuteStateEnum]' = None
+
+        @dataclass
+        class TestInProgress(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=bool)
+
+            value: 'bool' = False
+
+        @dataclass
+        class HardwareFaultAlert(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000006
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=bool)
+
+            value: 'bool' = False
+
+        @dataclass
+        class EndOfServiceAlert(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000007
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=SmokeCoAlarm.Enums.EndOfServiceEnum)
+
+            value: 'SmokeCoAlarm.Enums.EndOfServiceEnum' = 0
+
+        @dataclass
+        class InterconnectSmokeAlarm(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000008
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum])
+
+            value: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+
+        @dataclass
+        class InterconnectCOAlarm(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000009
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum])
+
+            value: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+
+        @dataclass
+        class ContaminationState(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000000A
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.ContaminationStateEnum])
+
+            value: 'typing.Optional[SmokeCoAlarm.Enums.ContaminationStateEnum]' = None
+
+        @dataclass
+        class SmokeSensitivityLevel(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000000B
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.SensitivityEnum])
+
+            value: 'typing.Optional[SmokeCoAlarm.Enums.SensitivityEnum]' = None
+
+        @dataclass
+        class ExpiryDate(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000000C
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+    class Events:
+        @dataclass
+        class SmokeAlarm(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="alarmSeverityLevel", Tag=0, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
+                    ])
+
+            alarmSeverityLevel: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
+
+        @dataclass
+        class COAlarm(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="alarmSeverityLevel", Tag=0, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
+                    ])
+
+            alarmSeverityLevel: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
+
+        @dataclass
+        class LowBattery(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="alarmSeverityLevel", Tag=0, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
+                    ])
+
+            alarmSeverityLevel: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
+
+        @dataclass
+        class HardwareFault(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class EndOfService(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class SelfTestComplete(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class AlarmMuted(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000006
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class MuteEnded(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000007
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class InterconnectSmokeAlarm(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000008
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="alarmSeverityLevel", Tag=0, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
+                    ])
+
+            alarmSeverityLevel: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
+
+        @dataclass
+        class InterconnectCOAlarm(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000009
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="alarmSeverityLevel", Tag=0, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
+                    ])
+
+            alarmSeverityLevel: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
+
+        @dataclass
+        class AllClear(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005C
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x0000000A
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+
+@dataclass
+class DishwasherAlarm(Cluster):
+    id: typing.ClassVar[int] = 0x0000005D
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="mask", Tag=0x00000000, Type=uint),
+                ClusterObjectFieldDescriptor(Label="latch", Tag=0x00000001, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="state", Tag=0x00000002, Type=uint),
+                ClusterObjectFieldDescriptor(Label="supported", Tag=0x00000003, Type=uint),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    mask: 'uint' = None
+    latch: 'typing.Optional[uint]' = None
+    state: 'uint' = None
+    supported: 'uint' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Bitmaps:
+        class AlarmBitmap(IntFlag):
+            kInflowError = 0x1
+            kDrainError = 0x2
+            kDoorError = 0x4
+            kTempTooLow = 0x8
+            kTempTooHigh = 0x10
+            kWaterLevelError = 0x20
+
+        class Feature(IntFlag):
+            kReset = 0x1
+
+    class Commands:
+        @dataclass
+        class Reset(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000005D
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="alarms", Tag=0, Type=uint),
+                    ])
+
+            alarms: 'uint' = 0
+
+        @dataclass
+        class ModifyEnabledAlarms(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000005D
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="mask", Tag=0, Type=uint),
+                    ])
+
+            mask: 'uint' = 0
+
+    class Attributes:
+        @dataclass
+        class Mask(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005D
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class Latch(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005D
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class State(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005D
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class Supported(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005D
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005D
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005D
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005D
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005D
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005D
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005D
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+    class Events:
+        @dataclass
+        class Notify(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005D
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="active", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="inactive", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="state", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="mask", Tag=3, Type=uint),
+                    ])
+
+            active: 'uint' = 0
+            inactive: 'uint' = 0
+            state: 'uint' = 0
+            mask: 'uint' = 0
+
+
+@dataclass
+class MicrowaveOvenMode(Cluster):
+    id: typing.ClassVar[int] = 0x0000005E
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="supportedModes", Tag=0x00000000, Type=typing.List[MicrowaveOvenMode.Structs.ModeOptionStruct]),
+                ClusterObjectFieldDescriptor(Label="currentMode", Tag=0x00000001, Type=uint),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    supportedModes: 'typing.List[MicrowaveOvenMode.Structs.ModeOptionStruct]' = None
+    currentMode: 'uint' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class ModeTag(MatterIntEnum):
+            kNormal = 0x4000
+            kDefrost = 0x4001
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 0,
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kOnOff = 0x1
+
+    class Structs:
+        @dataclass
+        class ModeTagStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="mfgCode", Tag=0, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=uint),
+                    ])
+
+            mfgCode: 'typing.Optional[uint]' = None
+            value: 'uint' = 0
+
+        @dataclass
+        class ModeOptionStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="label", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="mode", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="modeTags", Tag=2, Type=typing.List[MicrowaveOvenMode.Structs.ModeTagStruct]),
+                    ])
+
+            label: 'str' = ""
+            mode: 'uint' = 0
+            modeTags: 'typing.List[MicrowaveOvenMode.Structs.ModeTagStruct]' = field(default_factory=lambda: [])
+
+    class Attributes:
+        @dataclass
+        class SupportedModes(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005E
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[MicrowaveOvenMode.Structs.ModeOptionStruct])
+
+            value: 'typing.List[MicrowaveOvenMode.Structs.ModeOptionStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class CurrentMode(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005E
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005E
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005E
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005E
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005E
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005E
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005E
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class MicrowaveOvenControl(Cluster):
+    id: typing.ClassVar[int] = 0x0000005F
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="cookTime", Tag=0x00000000, Type=uint),
+                ClusterObjectFieldDescriptor(Label="maxCookTime", Tag=0x00000001, Type=uint),
+                ClusterObjectFieldDescriptor(Label="powerSetting", Tag=0x00000002, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="minPower", Tag=0x00000003, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="maxPower", Tag=0x00000004, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="powerStep", Tag=0x00000005, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="supportedWatts", Tag=0x00000006, Type=typing.Optional[typing.List[uint]]),
+                ClusterObjectFieldDescriptor(Label="selectedWattIndex", Tag=0x00000007, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="wattRating", Tag=0x00000008, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    cookTime: 'uint' = None
+    maxCookTime: 'uint' = None
+    powerSetting: 'typing.Optional[uint]' = None
+    minPower: 'typing.Optional[uint]' = None
+    maxPower: 'typing.Optional[uint]' = None
+    powerStep: 'typing.Optional[uint]' = None
+    supportedWatts: 'typing.Optional[typing.List[uint]]' = None
+    selectedWattIndex: 'typing.Optional[uint]' = None
+    wattRating: 'typing.Optional[uint]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kPowerAsNumber = 0x1
+            kPowerInWatts = 0x2
+            kPowerNumberLimits = 0x4
+
+    class Commands:
+        @dataclass
+        class SetCookingParameters(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000005F
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="cookMode", Tag=0, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="cookTime", Tag=1, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="powerSetting", Tag=2, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="wattSettingIndex", Tag=3, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="startAfterSetting", Tag=4, Type=typing.Optional[bool]),
+                    ])
+
+            cookMode: 'typing.Optional[uint]' = None
+            cookTime: 'typing.Optional[uint]' = None
+            powerSetting: 'typing.Optional[uint]' = None
+            wattSettingIndex: 'typing.Optional[uint]' = None
+            startAfterSetting: 'typing.Optional[bool]' = None
+
+        @dataclass
+        class AddMoreTime(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000005F
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="timeToAdd", Tag=0, Type=uint),
+                    ])
+
+            timeToAdd: 'uint' = 0
+
+    class Attributes:
+        @dataclass
+        class CookTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class MaxCookTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class PowerSetting(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class MinPower(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class MaxPower(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class PowerStep(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class SupportedWatts(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000006
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[uint]])
+
+            value: 'typing.Optional[typing.List[uint]]' = None
+
+        @dataclass
+        class SelectedWattIndex(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000007
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class WattRating(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000008
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000005F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class OperationalState(Cluster):
+    id: typing.ClassVar[int] = 0x00000060
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="phaseList", Tag=0x00000000, Type=typing.Union[Nullable, typing.List[str]]),
+                ClusterObjectFieldDescriptor(Label="currentPhase", Tag=0x00000001, Type=typing.Union[Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="countdownTime", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="operationalStateList", Tag=0x00000003, Type=typing.List[OperationalState.Structs.OperationalStateStruct]),
+                ClusterObjectFieldDescriptor(Label="operationalState", Tag=0x00000004, Type=OperationalState.Enums.OperationalStateEnum),
+                ClusterObjectFieldDescriptor(Label="operationalError", Tag=0x00000005, Type=OperationalState.Structs.ErrorStateStruct),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    phaseList: 'typing.Union[Nullable, typing.List[str]]' = None
+    currentPhase: 'typing.Union[Nullable, uint]' = None
+    countdownTime: 'typing.Union[None, Nullable, uint]' = None
+    operationalStateList: 'typing.List[OperationalState.Structs.OperationalStateStruct]' = None
+    operationalState: 'OperationalState.Enums.OperationalStateEnum' = None
+    operationalError: 'OperationalState.Structs.ErrorStateStruct' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class ErrorStateEnum(MatterIntEnum):
+            kNoError = 0x00
+            kUnableToStartOrResume = 0x01
+            kUnableToCompleteOperation = 0x02
+            kCommandInvalidInState = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
+
+        class OperationalStateEnum(MatterIntEnum):
+            kStopped = 0x00
+            kRunning = 0x01
+            kPaused = 0x02
+            kError = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
+
+    class Structs:
+        @dataclass
+        class ErrorStateStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="errorStateID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="errorStateLabel", Tag=1, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="errorStateDetails", Tag=2, Type=typing.Optional[str]),
+                    ])
+
+            errorStateID: 'uint' = 0
+            errorStateLabel: 'typing.Optional[str]' = None
+            errorStateDetails: 'typing.Optional[str]' = None
+
+        @dataclass
+        class OperationalStateStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="operationalStateID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="operationalStateLabel", Tag=1, Type=typing.Optional[str]),
+                    ])
+
+            operationalStateID: 'uint' = 0
+            operationalStateLabel: 'typing.Optional[str]' = None
+
+    class Commands:
+        @dataclass
+        class Pause(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000060
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class Stop(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000060
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class Start(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000060
+            command_id: typing.ClassVar[int] = 0x00000002
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class Resume(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000060
+            command_id: typing.ClassVar[int] = 0x00000003
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class OperationalCommandResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000060
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="commandResponseState", Tag=0, Type=OperationalState.Structs.ErrorStateStruct),
+                    ])
+
+            commandResponseState: 'OperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: OperationalState.Structs.ErrorStateStruct())
+
+    class Attributes:
+        @dataclass
+        class PhaseList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, typing.List[str]])
+
+            value: 'typing.Union[Nullable, typing.List[str]]' = NullValue
+
+        @dataclass
+        class CurrentPhase(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
+
+            value: 'typing.Union[Nullable, uint]' = NullValue
+
+        @dataclass
+        class CountdownTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class OperationalStateList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[OperationalState.Structs.OperationalStateStruct])
+
+            value: 'typing.List[OperationalState.Structs.OperationalStateStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class OperationalState(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=OperationalState.Enums.OperationalStateEnum)
+
+            value: 'OperationalState.Enums.OperationalStateEnum' = 0
+
+        @dataclass
+        class OperationalError(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=OperationalState.Structs.ErrorStateStruct)
+
+            value: 'OperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: OperationalState.Structs.ErrorStateStruct())
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+    class Events:
+        @dataclass
+        class OperationalError(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="errorState", Tag=0, Type=OperationalState.Structs.ErrorStateStruct),
+                    ])
+
+            errorState: 'OperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: OperationalState.Structs.ErrorStateStruct())
+
+        @dataclass
+        class OperationCompletion(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000060
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="completionErrorCode", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="totalOperationalTime", Tag=1, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="pausedTime", Tag=2, Type=typing.Union[None, Nullable, uint]),
+                    ])
+
+            completionErrorCode: 'uint' = 0
+            totalOperationalTime: 'typing.Union[None, Nullable, uint]' = None
+            pausedTime: 'typing.Union[None, Nullable, uint]' = None
+
+
+@dataclass
+class RvcOperationalState(Cluster):
+    id: typing.ClassVar[int] = 0x00000061
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="phaseList", Tag=0x00000000, Type=typing.Union[Nullable, typing.List[str]]),
+                ClusterObjectFieldDescriptor(Label="currentPhase", Tag=0x00000001, Type=typing.Union[Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="countdownTime", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="operationalStateList", Tag=0x00000003, Type=typing.List[RvcOperationalState.Structs.OperationalStateStruct]),
+                ClusterObjectFieldDescriptor(Label="operationalState", Tag=0x00000004, Type=uint),
+                ClusterObjectFieldDescriptor(Label="operationalError", Tag=0x00000005, Type=RvcOperationalState.Structs.ErrorStateStruct),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    phaseList: 'typing.Union[Nullable, typing.List[str]]' = None
+    currentPhase: 'typing.Union[Nullable, uint]' = None
+    countdownTime: 'typing.Union[None, Nullable, uint]' = None
+    operationalStateList: 'typing.List[RvcOperationalState.Structs.OperationalStateStruct]' = None
+    operationalState: 'uint' = None
+    operationalError: 'RvcOperationalState.Structs.ErrorStateStruct' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class ErrorStateEnum(MatterIntEnum):
+            kFailedToFindChargingDock = 0x40
+            kStuck = 0x41
+            kDustBinMissing = 0x42
+            kDustBinFull = 0x43
+            kWaterTankEmpty = 0x44
+            kWaterTankMissing = 0x45
+            kWaterTankLidOpen = 0x46
+            kMopCleaningPadMissing = 0x47
+            # kUnknownEnumValue intentionally not defined. This enum never goes
+            # through DataModel::Decode, likely because it is a part of a derived
+            # cluster. As a result having kUnknownEnumValue in this enum is error
+            # prone, and was removed. See
+            # src/app/common/templates/config-data.yaml.
+
+        class OperationalStateEnum(MatterIntEnum):
+            kSeekingCharger = 0x40
+            kCharging = 0x41
+            kDocked = 0x42
+            # kUnknownEnumValue intentionally not defined. This enum never goes
+            # through DataModel::Decode, likely because it is a part of a derived
+            # cluster. As a result having kUnknownEnumValue in this enum is error
+            # prone, and was removed. See
+            # src/app/common/templates/config-data.yaml.
+
+    class Structs:
+        @dataclass
+        class ErrorStateStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="errorStateID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="errorStateLabel", Tag=1, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="errorStateDetails", Tag=2, Type=typing.Optional[str]),
+                    ])
+
+            errorStateID: 'uint' = 0
+            errorStateLabel: 'typing.Optional[str]' = None
+            errorStateDetails: 'typing.Optional[str]' = None
+
+        @dataclass
+        class OperationalStateStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="operationalStateID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="operationalStateLabel", Tag=1, Type=typing.Optional[str]),
+                    ])
+
+            operationalStateID: 'uint' = 0
+            operationalStateLabel: 'typing.Optional[str]' = None
+
+    class Commands:
+        @dataclass
+        class Pause(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000061
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class Resume(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000061
+            command_id: typing.ClassVar[int] = 0x00000003
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class OperationalCommandResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000061
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="commandResponseState", Tag=0, Type=RvcOperationalState.Structs.ErrorStateStruct),
+                    ])
+
+            commandResponseState: 'RvcOperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: RvcOperationalState.Structs.ErrorStateStruct())
+
+        @dataclass
+        class GoHome(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000061
+            command_id: typing.ClassVar[int] = 0x00000080
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+    class Attributes:
+        @dataclass
+        class PhaseList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, typing.List[str]])
+
+            value: 'typing.Union[Nullable, typing.List[str]]' = NullValue
+
+        @dataclass
+        class CurrentPhase(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
+
+            value: 'typing.Union[Nullable, uint]' = NullValue
+
+        @dataclass
+        class CountdownTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class OperationalStateList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[RvcOperationalState.Structs.OperationalStateStruct])
+
+            value: 'typing.List[RvcOperationalState.Structs.OperationalStateStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class OperationalState(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class OperationalError(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=RvcOperationalState.Structs.ErrorStateStruct)
+
+            value: 'RvcOperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: RvcOperationalState.Structs.ErrorStateStruct())
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+    class Events:
+        @dataclass
+        class OperationalError(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="errorState", Tag=0, Type=RvcOperationalState.Structs.ErrorStateStruct),
+                    ])
+
+            errorState: 'RvcOperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: RvcOperationalState.Structs.ErrorStateStruct())
+
+        @dataclass
+        class OperationCompletion(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000061
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="completionErrorCode", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="totalOperationalTime", Tag=1, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="pausedTime", Tag=2, Type=typing.Union[None, Nullable, uint]),
+                    ])
+
+            completionErrorCode: 'uint' = 0
+            totalOperationalTime: 'typing.Union[None, Nullable, uint]' = None
+            pausedTime: 'typing.Union[None, Nullable, uint]' = None
+
+
+@dataclass
+class ScenesManagement(Cluster):
+    id: typing.ClassVar[int] = 0x00000062
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="lastConfiguredBy", Tag=0x00000000, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="sceneTableSize", Tag=0x00000001, Type=uint),
+                ClusterObjectFieldDescriptor(Label="fabricSceneInfo", Tag=0x00000002, Type=typing.List[ScenesManagement.Structs.SceneInfoStruct]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    lastConfiguredBy: 'typing.Union[None, Nullable, uint]' = None
+    sceneTableSize: 'uint' = None
+    fabricSceneInfo: 'typing.List[ScenesManagement.Structs.SceneInfoStruct]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Bitmaps:
+        class CopyModeBitmap(IntFlag):
+            kCopyAllScenes = 0x1
+
+        class Feature(IntFlag):
+            kSceneNames = 0x1
+
+    class Structs:
+        @dataclass
+        class AttributeValuePair(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="attributeID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="attributeValue", Tag=1, Type=uint),
+                    ])
+
+            attributeID: 'uint' = 0
+            attributeValue: 'uint' = 0
+
+        @dataclass
+        class ExtensionFieldSet(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="clusterID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="attributeValueList", Tag=1, Type=typing.List[ScenesManagement.Structs.AttributeValuePair]),
+                    ])
+
+            clusterID: 'uint' = 0
+            attributeValueList: 'typing.List[ScenesManagement.Structs.AttributeValuePair]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class SceneInfoStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="sceneCount", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="currentScene", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="currentGroup", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneValid", Tag=3, Type=bool),
+                        ClusterObjectFieldDescriptor(Label="remainingCapacity", Tag=4, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="fabricIndex", Tag=254, Type=uint),
+                    ])
+
+            sceneCount: 'uint' = 0
+            currentScene: 'uint' = 0
+            currentGroup: 'uint' = 0
+            sceneValid: 'bool' = False
+            remainingCapacity: 'uint' = 0
+            fabricIndex: 'uint' = 0
+
+    class Commands:
+        @dataclass
+        class AddScene(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'AddSceneResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="transitionTime", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneName", Tag=3, Type=str),
+                        ClusterObjectFieldDescriptor(Label="extensionFieldSets", Tag=4, Type=typing.List[ScenesManagement.Structs.ExtensionFieldSet]),
+                    ])
+
+            groupID: 'uint' = 0
+            sceneID: 'uint' = 0
+            transitionTime: 'uint' = 0
+            sceneName: 'str' = ""
+            extensionFieldSets: 'typing.List[ScenesManagement.Structs.ExtensionFieldSet]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AddSceneResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=2, Type=uint),
+                    ])
+
+            status: 'uint' = 0
+            groupID: 'uint' = 0
+            sceneID: 'uint' = 0
+
+        @dataclass
+        class ViewScene(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'ViewSceneResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
+                    ])
+
+            groupID: 'uint' = 0
+            sceneID: 'uint' = 0
+
+        @dataclass
+        class ViewSceneResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="transitionTime", Tag=3, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="sceneName", Tag=4, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="extensionFieldSets", Tag=5, Type=typing.Optional[typing.List[ScenesManagement.Structs.ExtensionFieldSet]]),
+                    ])
+
+            status: 'uint' = 0
+            groupID: 'uint' = 0
+            sceneID: 'uint' = 0
+            transitionTime: 'typing.Optional[uint]' = None
+            sceneName: 'typing.Optional[str]' = None
+            extensionFieldSets: 'typing.Optional[typing.List[ScenesManagement.Structs.ExtensionFieldSet]]' = None
+
+        @dataclass
+        class RemoveScene(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000002
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'RemoveSceneResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
+                    ])
+
+            groupID: 'uint' = 0
+            sceneID: 'uint' = 0
+
+        @dataclass
+        class RemoveSceneResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000002
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=2, Type=uint),
+                    ])
+
+            status: 'uint' = 0
+            groupID: 'uint' = 0
+            sceneID: 'uint' = 0
+
+        @dataclass
+        class RemoveAllScenes(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000003
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'RemoveAllScenesResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
+                    ])
+
+            groupID: 'uint' = 0
+
+        @dataclass
+        class RemoveAllScenesResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000003
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
+                    ])
+
+            status: 'uint' = 0
+            groupID: 'uint' = 0
+
+        @dataclass
+        class StoreScene(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'StoreSceneResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
+                    ])
+
+            groupID: 'uint' = 0
+            sceneID: 'uint' = 0
+
+        @dataclass
+        class StoreSceneResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=2, Type=uint),
+                    ])
+
+            status: 'uint' = 0
+            groupID: 'uint' = 0
+            sceneID: 'uint' = 0
+
+        @dataclass
+        class RecallScene(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000005
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneID", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="transitionTime", Tag=2, Type=typing.Union[None, Nullable, uint]),
+                    ])
+
+            groupID: 'uint' = 0
+            sceneID: 'uint' = 0
+            transitionTime: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class GetSceneMembership(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000006
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'GetSceneMembershipResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=0, Type=uint),
+                    ])
+
+            groupID: 'uint' = 0
+
+        @dataclass
+        class GetSceneMembershipResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000006
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="capacity", Tag=1, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="groupID", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneList", Tag=3, Type=typing.Optional[typing.List[uint]]),
+                    ])
+
+            status: 'uint' = 0
+            capacity: 'typing.Union[Nullable, uint]' = NullValue
+            groupID: 'uint' = 0
+            sceneList: 'typing.Optional[typing.List[uint]]' = None
+
+        @dataclass
+        class CopyScene(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000040
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'CopySceneResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="mode", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="groupIdentifierFrom", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneIdentifierFrom", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="groupIdentifierTo", Tag=3, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneIdentifierTo", Tag=4, Type=uint),
+                    ])
+
+            mode: 'uint' = 0
+            groupIdentifierFrom: 'uint' = 0
+            sceneIdentifierFrom: 'uint' = 0
+            groupIdentifierTo: 'uint' = 0
+            sceneIdentifierTo: 'uint' = 0
+
+        @dataclass
+        class CopySceneResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000062
+            command_id: typing.ClassVar[int] = 0x00000040
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="groupIdentifierFrom", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sceneIdentifierFrom", Tag=2, Type=uint),
+                    ])
+
+            status: 'uint' = 0
+            groupIdentifierFrom: 'uint' = 0
+            sceneIdentifierFrom: 'uint' = 0
+
+    class Attributes:
+        @dataclass
+        class LastConfiguredBy(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000062
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class SceneTableSize(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000062
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class FabricSceneInfo(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000062
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[ScenesManagement.Structs.SceneInfoStruct])
+
+            value: 'typing.List[ScenesManagement.Structs.SceneInfoStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000062
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000062
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000062
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000062
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000062
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000062
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class HepaFilterMonitoring(Cluster):
+    id: typing.ClassVar[int] = 0x00000071
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="condition", Tag=0x00000000, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="degradationDirection", Tag=0x00000001, Type=typing.Optional[HepaFilterMonitoring.Enums.DegradationDirectionEnum]),
+                ClusterObjectFieldDescriptor(Label="changeIndication", Tag=0x00000002, Type=HepaFilterMonitoring.Enums.ChangeIndicationEnum),
+                ClusterObjectFieldDescriptor(Label="inPlaceIndicator", Tag=0x00000003, Type=typing.Optional[bool]),
+                ClusterObjectFieldDescriptor(Label="lastChangedTime", Tag=0x00000004, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="replacementProductList", Tag=0x00000005, Type=typing.Optional[typing.List[HepaFilterMonitoring.Structs.ReplacementProductStruct]]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    condition: 'typing.Optional[uint]' = None
+    degradationDirection: 'typing.Optional[HepaFilterMonitoring.Enums.DegradationDirectionEnum]' = None
+    changeIndication: 'HepaFilterMonitoring.Enums.ChangeIndicationEnum' = None
+    inPlaceIndicator: 'typing.Optional[bool]' = None
+    lastChangedTime: 'typing.Union[None, Nullable, uint]' = None
+    replacementProductList: 'typing.Optional[typing.List[HepaFilterMonitoring.Structs.ReplacementProductStruct]]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class ChangeIndicationEnum(MatterIntEnum):
+            kOk = 0x00
+            kWarning = 0x01
+            kCritical = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 3,
+
+        class DegradationDirectionEnum(MatterIntEnum):
+            kUp = 0x00
+            kDown = 0x01
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 2,
+
+        class ProductIdentifierTypeEnum(MatterIntEnum):
+            kUpc = 0x00
+            kGtin8 = 0x01
+            kEan = 0x02
+            kGtin14 = 0x03
+            kOem = 0x04
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 5,
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kCondition = 0x1
+            kWarning = 0x2
+            kReplacementProductList = 0x4
+
+    class Structs:
+        @dataclass
+        class ReplacementProductStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="productIdentifierType", Tag=0, Type=HepaFilterMonitoring.Enums.ProductIdentifierTypeEnum),
+                        ClusterObjectFieldDescriptor(Label="productIdentifierValue", Tag=1, Type=str),
+                    ])
+
+            productIdentifierType: 'HepaFilterMonitoring.Enums.ProductIdentifierTypeEnum' = 0
+            productIdentifierValue: 'str' = ""
+
+    class Commands:
+        @dataclass
+        class ResetCondition(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000071
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+    class Attributes:
+        @dataclass
+        class Condition(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class DegradationDirection(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[HepaFilterMonitoring.Enums.DegradationDirectionEnum])
+
+            value: 'typing.Optional[HepaFilterMonitoring.Enums.DegradationDirectionEnum]' = None
+
+        @dataclass
+        class ChangeIndication(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=HepaFilterMonitoring.Enums.ChangeIndicationEnum)
+
+            value: 'HepaFilterMonitoring.Enums.ChangeIndicationEnum' = 0
+
+        @dataclass
+        class InPlaceIndicator(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[bool])
+
+            value: 'typing.Optional[bool]' = None
+
+        @dataclass
+        class LastChangedTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class ReplacementProductList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[HepaFilterMonitoring.Structs.ReplacementProductStruct]])
+
+            value: 'typing.Optional[typing.List[HepaFilterMonitoring.Structs.ReplacementProductStruct]]' = None
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000071
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class ActivatedCarbonFilterMonitoring(Cluster):
+    id: typing.ClassVar[int] = 0x00000072
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="condition", Tag=0x00000000, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="degradationDirection", Tag=0x00000001, Type=typing.Optional[ActivatedCarbonFilterMonitoring.Enums.DegradationDirectionEnum]),
+                ClusterObjectFieldDescriptor(Label="changeIndication", Tag=0x00000002, Type=ActivatedCarbonFilterMonitoring.Enums.ChangeIndicationEnum),
+                ClusterObjectFieldDescriptor(Label="inPlaceIndicator", Tag=0x00000003, Type=typing.Optional[bool]),
+                ClusterObjectFieldDescriptor(Label="lastChangedTime", Tag=0x00000004, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="replacementProductList", Tag=0x00000005, Type=typing.Optional[typing.List[ActivatedCarbonFilterMonitoring.Structs.ReplacementProductStruct]]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    condition: 'typing.Optional[uint]' = None
+    degradationDirection: 'typing.Optional[ActivatedCarbonFilterMonitoring.Enums.DegradationDirectionEnum]' = None
+    changeIndication: 'ActivatedCarbonFilterMonitoring.Enums.ChangeIndicationEnum' = None
+    inPlaceIndicator: 'typing.Optional[bool]' = None
+    lastChangedTime: 'typing.Union[None, Nullable, uint]' = None
+    replacementProductList: 'typing.Optional[typing.List[ActivatedCarbonFilterMonitoring.Structs.ReplacementProductStruct]]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class ChangeIndicationEnum(MatterIntEnum):
+            kOk = 0x00
+            kWarning = 0x01
+            kCritical = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 3,
+
+        class DegradationDirectionEnum(MatterIntEnum):
+            kUp = 0x00
+            kDown = 0x01
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 2,
+
+        class ProductIdentifierTypeEnum(MatterIntEnum):
+            kUpc = 0x00
+            kGtin8 = 0x01
+            kEan = 0x02
+            kGtin14 = 0x03
+            kOem = 0x04
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 5,
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kCondition = 0x1
+            kWarning = 0x2
+            kReplacementProductList = 0x4
+
+    class Structs:
+        @dataclass
+        class ReplacementProductStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="productIdentifierType", Tag=0, Type=ActivatedCarbonFilterMonitoring.Enums.ProductIdentifierTypeEnum),
+                        ClusterObjectFieldDescriptor(Label="productIdentifierValue", Tag=1, Type=str),
+                    ])
+
+            productIdentifierType: 'ActivatedCarbonFilterMonitoring.Enums.ProductIdentifierTypeEnum' = 0
+            productIdentifierValue: 'str' = ""
+
+    class Commands:
+        @dataclass
+        class ResetCondition(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000072
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+    class Attributes:
+        @dataclass
+        class Condition(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class DegradationDirection(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[ActivatedCarbonFilterMonitoring.Enums.DegradationDirectionEnum])
+
+            value: 'typing.Optional[ActivatedCarbonFilterMonitoring.Enums.DegradationDirectionEnum]' = None
+
+        @dataclass
+        class ChangeIndication(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=ActivatedCarbonFilterMonitoring.Enums.ChangeIndicationEnum)
+
+            value: 'ActivatedCarbonFilterMonitoring.Enums.ChangeIndicationEnum' = 0
+
+        @dataclass
+        class InPlaceIndicator(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[bool])
+
+            value: 'typing.Optional[bool]' = None
+
+        @dataclass
+        class LastChangedTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class ReplacementProductList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[ActivatedCarbonFilterMonitoring.Structs.ReplacementProductStruct]])
+
+            value: 'typing.Optional[typing.List[ActivatedCarbonFilterMonitoring.Structs.ReplacementProductStruct]]' = None
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000072
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+
+@dataclass
+class BooleanStateConfiguration(Cluster):
+    id: typing.ClassVar[int] = 0x00000080
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="currentSensitivityLevel", Tag=0x00000000, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="supportedSensitivityLevels", Tag=0x00000001, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="defaultSensitivityLevel", Tag=0x00000002, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="alarmsActive", Tag=0x00000003, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="alarmsSuppressed", Tag=0x00000004, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="alarmsEnabled", Tag=0x00000005, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="alarmsSupported", Tag=0x00000006, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="sensorFault", Tag=0x00000007, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    currentSensitivityLevel: 'typing.Optional[uint]' = None
+    supportedSensitivityLevels: 'typing.Optional[uint]' = None
+    defaultSensitivityLevel: 'typing.Optional[uint]' = None
+    alarmsActive: 'typing.Optional[uint]' = None
+    alarmsSuppressed: 'typing.Optional[uint]' = None
+    alarmsEnabled: 'typing.Optional[uint]' = None
+    alarmsSupported: 'typing.Optional[uint]' = None
+    sensorFault: 'typing.Optional[uint]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Bitmaps:
+        class AlarmModeBitmap(IntFlag):
+            kVisual = 0x1
+            kAudible = 0x2
+
+        class Feature(IntFlag):
+            kVisual = 0x1
+            kAudible = 0x2
+            kAlarmSuppress = 0x4
+            kSensitivityLevel = 0x8
+
+        class SensorFaultBitmap(IntFlag):
+            kGeneralFault = 0x1
+
+    class Commands:
+        @dataclass
+        class SuppressAlarm(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000080
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="alarmsToSuppress", Tag=0, Type=uint),
+                    ])
+
+            alarmsToSuppress: 'uint' = 0
+
+        @dataclass
+        class EnableDisableAlarm(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000080
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="alarmsToEnableDisable", Tag=0, Type=uint),
+                    ])
+
+            alarmsToEnableDisable: 'uint' = 0
+
+    class Attributes:
+        @dataclass
+        class CurrentSensitivityLevel(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class SupportedSensitivityLevels(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class DefaultSensitivityLevel(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class AlarmsActive(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class AlarmsSuppressed(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class AlarmsEnabled(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class AlarmsSupported(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000006
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class SensorFault(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000007
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+    class Events:
+        @dataclass
+        class AlarmsStateChanged(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="alarmsActive", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="alarmsSuppressed", Tag=1, Type=typing.Optional[uint]),
+                    ])
+
+            alarmsActive: 'uint' = 0
+            alarmsSuppressed: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class SensorFault(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="sensorFault", Tag=0, Type=uint),
+                    ])
+
+            sensorFault: 'uint' = 0
+
+
+@dataclass
+class ValveConfigurationAndControl(Cluster):
+    id: typing.ClassVar[int] = 0x00000081
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="openDuration", Tag=0x00000000, Type=typing.Union[Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="defaultOpenDuration", Tag=0x00000001, Type=typing.Union[Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="autoCloseTime", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="remainingDuration", Tag=0x00000003, Type=typing.Union[Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="currentState", Tag=0x00000004, Type=typing.Union[Nullable, ValveConfigurationAndControl.Enums.ValveStateEnum]),
+                ClusterObjectFieldDescriptor(Label="targetState", Tag=0x00000005, Type=typing.Union[Nullable, ValveConfigurationAndControl.Enums.ValveStateEnum]),
+                ClusterObjectFieldDescriptor(Label="currentLevel", Tag=0x00000006, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="targetLevel", Tag=0x00000007, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="defaultOpenLevel", Tag=0x00000008, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="valveFault", Tag=0x00000009, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="levelStep", Tag=0x0000000A, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    openDuration: 'typing.Union[Nullable, uint]' = None
+    defaultOpenDuration: 'typing.Union[Nullable, uint]' = None
+    autoCloseTime: 'typing.Union[None, Nullable, uint]' = None
+    remainingDuration: 'typing.Union[Nullable, uint]' = None
+    currentState: 'typing.Union[Nullable, ValveConfigurationAndControl.Enums.ValveStateEnum]' = None
+    targetState: 'typing.Union[Nullable, ValveConfigurationAndControl.Enums.ValveStateEnum]' = None
+    currentLevel: 'typing.Union[None, Nullable, uint]' = None
+    targetLevel: 'typing.Union[None, Nullable, uint]' = None
+    defaultOpenLevel: 'typing.Optional[uint]' = None
+    valveFault: 'typing.Optional[uint]' = None
+    levelStep: 'typing.Optional[uint]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class StatusCodeEnum(MatterIntEnum):
+            kFailureDueToFault = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 0,
+
+        class ValveStateEnum(MatterIntEnum):
+            kClosed = 0x00
+            kOpen = 0x01
+            kTransitioning = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 3,
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kTimeSync = 0x1
+            kLevel = 0x2
+
+        class ValveFaultBitmap(IntFlag):
+            kGeneralFault = 0x1
+            kBlocked = 0x2
+            kLeaking = 0x4
+            kNotConnected = 0x8
+            kShortCircuit = 0x10
+            kCurrentExceeded = 0x20
+
+    class Commands:
+        @dataclass
+        class Open(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000081
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="openDuration", Tag=0, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="targetLevel", Tag=1, Type=typing.Optional[uint]),
+                    ])
+
+            openDuration: 'typing.Union[None, Nullable, uint]' = None
+            targetLevel: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class Close(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000081
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+    class Attributes:
+        @dataclass
+        class OpenDuration(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000081
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
+
+            value: 'typing.Union[Nullable, uint]' = NullValue
+
+        @dataclass
+        class DefaultOpenDuration(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000081
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
+
+            value: 'typing.Union[Nullable, uint]' = NullValue
+
+        @dataclass
+        class AutoCloseTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000081
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class RemainingDuration(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000081
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
+
+            value: 'typing.Union[Nullable, uint]' = NullValue
+
+        @dataclass
+        class CurrentState(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000081
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, ValveConfigurationAndControl.Enums.ValveStateEnum])
+
+            value: 'typing.Union[Nullable, ValveConfigurationAndControl.Enums.ValveStateEnum]' = NullValue
+
+        @dataclass
+        class TargetState(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000081
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, ValveConfigurationAndControl.Enums.ValveStateEnum])
+
+            value: 'typing.Union[Nullable, ValveConfigurationAndControl.Enums.ValveStateEnum]' = NullValue
+
+        @dataclass
+        class CurrentLevel(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000081
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000006
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
 
         @dataclass
-        class ChangeToModeResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000054
-            command_id: typing.ClassVar[int] = 0x00000001
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
+        class TargetLevel(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000081
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="statusText", Tag=1, Type=typing.Optional[str]),
-                    ])
+            def attribute_id(cls) -> int:
+                return 0x00000007
 
-            status: 'uint' = 0
-            statusText: 'typing.Optional[str]' = None
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
 
-    class Attributes:
         @dataclass
-        class SupportedModes(ClusterAttributeDescriptor):
+        class DefaultOpenLevel(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000054
+                return 0x00000081
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000000
+                return 0x00000008
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[RvcRunMode.Structs.ModeOptionStruct])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
 
-            value: 'typing.List[RvcRunMode.Structs.ModeOptionStruct]' = field(default_factory=lambda: [])
+            value: 'typing.Optional[uint]' = None
 
         @dataclass
-        class CurrentMode(ClusterAttributeDescriptor):
+        class ValveFault(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000054
+                return 0x00000081
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000001
+                return 0x00000009
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
 
-            value: 'uint' = 0
+            value: 'typing.Optional[uint]' = None
 
         @dataclass
-        class OnMode(ClusterAttributeDescriptor):
+        class LevelStep(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000054
+                return 0x00000081
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000003
+                return 0x0000000A
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
 
-            value: 'typing.Union[None, Nullable, uint]' = None
+            value: 'typing.Optional[uint]' = None
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000054
+                return 0x00000081
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF8
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16287,15 +22058,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AcceptedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000054
+                return 0x00000081
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF9
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16303,15 +22074,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class EventList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000054
+                return 0x00000081
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFA
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16319,15 +22090,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AttributeList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000054
+                return 0x00000081
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFB
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16335,15 +22106,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class FeatureMap(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000054
+                return 0x00000081
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFC
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16351,451 +22122,569 @@
 
             value: 'uint' = 0
 
         @dataclass
         class ClusterRevision(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000054
+                return 0x00000081
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFD
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
+    class Events:
+        @dataclass
+        class ValveStateChanged(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000081
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="valveState", Tag=0, Type=ValveConfigurationAndControl.Enums.ValveStateEnum),
+                        ClusterObjectFieldDescriptor(Label="valveLevel", Tag=1, Type=typing.Optional[uint]),
+                    ])
+
+            valveState: 'ValveConfigurationAndControl.Enums.ValveStateEnum' = 0
+            valveLevel: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class ValveFault(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000081
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="valveFault", Tag=0, Type=uint),
+                    ])
+
+            valveFault: 'uint' = 0
+
 
 @dataclass
-class RvcCleanMode(Cluster):
-    id: typing.ClassVar[int] = 0x00000055
+class ElectricalPowerMeasurement(Cluster):
+    id: typing.ClassVar[int] = 0x00000090
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
-                ClusterObjectFieldDescriptor(Label="supportedModes", Tag=0x00000000, Type=typing.List[RvcCleanMode.Structs.ModeOptionStruct]),
-                ClusterObjectFieldDescriptor(Label="currentMode", Tag=0x00000001, Type=uint),
-                ClusterObjectFieldDescriptor(Label="onMode", Tag=0x00000003, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="powerMode", Tag=0x00000000, Type=ElectricalPowerMeasurement.Enums.PowerModeEnum),
+                ClusterObjectFieldDescriptor(Label="numberOfMeasurementTypes", Tag=0x00000001, Type=uint),
+                ClusterObjectFieldDescriptor(Label="accuracy", Tag=0x00000002, Type=typing.List[ElectricalPowerMeasurement.Structs.MeasurementAccuracyStruct]),
+                ClusterObjectFieldDescriptor(Label="ranges", Tag=0x00000003, Type=typing.Optional[typing.List[ElectricalPowerMeasurement.Structs.MeasurementRangeStruct]]),
+                ClusterObjectFieldDescriptor(Label="voltage", Tag=0x00000004, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="activeCurrent", Tag=0x00000005, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="reactiveCurrent", Tag=0x00000006, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="apparentCurrent", Tag=0x00000007, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="activePower", Tag=0x00000008, Type=typing.Union[Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="reactivePower", Tag=0x00000009, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="apparentPower", Tag=0x0000000A, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="RMSVoltage", Tag=0x0000000B, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="RMSCurrent", Tag=0x0000000C, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="RMSPower", Tag=0x0000000D, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="frequency", Tag=0x0000000E, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="harmonicCurrents", Tag=0x0000000F, Type=typing.Union[None, Nullable, typing.List[ElectricalPowerMeasurement.Structs.HarmonicMeasurementStruct]]),
+                ClusterObjectFieldDescriptor(Label="harmonicPhases", Tag=0x00000010, Type=typing.Union[None, Nullable, typing.List[ElectricalPowerMeasurement.Structs.HarmonicMeasurementStruct]]),
+                ClusterObjectFieldDescriptor(Label="powerFactor", Tag=0x00000011, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="neutralCurrent", Tag=0x00000012, Type=typing.Union[None, Nullable, int]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
 
-    supportedModes: 'typing.List[RvcCleanMode.Structs.ModeOptionStruct]' = None
-    currentMode: 'uint' = None
-    onMode: 'typing.Union[None, Nullable, uint]' = None
+    powerMode: 'ElectricalPowerMeasurement.Enums.PowerModeEnum' = None
+    numberOfMeasurementTypes: 'uint' = None
+    accuracy: 'typing.List[ElectricalPowerMeasurement.Structs.MeasurementAccuracyStruct]' = None
+    ranges: 'typing.Optional[typing.List[ElectricalPowerMeasurement.Structs.MeasurementRangeStruct]]' = None
+    voltage: 'typing.Union[None, Nullable, int]' = None
+    activeCurrent: 'typing.Union[None, Nullable, int]' = None
+    reactiveCurrent: 'typing.Union[None, Nullable, int]' = None
+    apparentCurrent: 'typing.Union[None, Nullable, int]' = None
+    activePower: 'typing.Union[Nullable, int]' = None
+    reactivePower: 'typing.Union[None, Nullable, int]' = None
+    apparentPower: 'typing.Union[None, Nullable, int]' = None
+    RMSVoltage: 'typing.Union[None, Nullable, int]' = None
+    RMSCurrent: 'typing.Union[None, Nullable, int]' = None
+    RMSPower: 'typing.Union[None, Nullable, int]' = None
+    frequency: 'typing.Union[None, Nullable, int]' = None
+    harmonicCurrents: 'typing.Union[None, Nullable, typing.List[ElectricalPowerMeasurement.Structs.HarmonicMeasurementStruct]]' = None
+    harmonicPhases: 'typing.Union[None, Nullable, typing.List[ElectricalPowerMeasurement.Structs.HarmonicMeasurementStruct]]' = None
+    powerFactor: 'typing.Union[None, Nullable, int]' = None
+    neutralCurrent: 'typing.Union[None, Nullable, int]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class ModeTag(MatterIntEnum):
-            kDeepClean = 0x4000
-            kVacuum = 0x4001
-            kMop = 0x4002
-            # kUnknownEnumValue intentionally not defined. This enum never goes
-            # through DataModel::Decode, likely because it is a part of a derived
-            # cluster. As a result having kUnknownEnumValue in this enum is error
-            # prone, and was removed. See
-            # src/app/common/templates/config-data.yaml.
+        class MeasurementTypeEnum(MatterIntEnum):
+            kUnspecified = 0x00
+            kVoltage = 0x01
+            kActiveCurrent = 0x02
+            kReactiveCurrent = 0x03
+            kApparentCurrent = 0x04
+            kActivePower = 0x05
+            kReactivePower = 0x06
+            kApparentPower = 0x07
+            kRMSVoltage = 0x08
+            kRMSCurrent = 0x09
+            kRMSPower = 0x0A
+            kFrequency = 0x0B
+            kPowerFactor = 0x0C
+            kNeutralCurrent = 0x0D
+            kElectricalEnergy = 0x0E
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 15,
 
-        class StatusCode(MatterIntEnum):
-            kCleaningInProgress = 0x40
-            # kUnknownEnumValue intentionally not defined. This enum never goes
-            # through DataModel::Decode, likely because it is a part of a derived
-            # cluster. As a result having kUnknownEnumValue in this enum is error
-            # prone, and was removed. See
-            # src/app/common/templates/config-data.yaml.
+        class PowerModeEnum(MatterIntEnum):
+            kUnknown = 0x00
+            kDc = 0x01
+            kAc = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 3,
 
     class Bitmaps:
         class Feature(IntFlag):
-            kOnOff = 0x1
+            kDirectCurrent = 0x1
+            kAlternatingCurrent = 0x2
+            kPolyphasePower = 0x4
+            kHarmonics = 0x8
+            kPowerQuality = 0x10
 
     class Structs:
         @dataclass
-        class ModeTagStruct(ClusterObject):
+        class MeasurementAccuracyRangeStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="mfgCode", Tag=0, Type=typing.Optional[uint]),
-                        ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="rangeMin", Tag=0, Type=int),
+                        ClusterObjectFieldDescriptor(Label="rangeMax", Tag=1, Type=int),
+                        ClusterObjectFieldDescriptor(Label="percentMax", Tag=2, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="percentMin", Tag=3, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="percentTypical", Tag=4, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="fixedMax", Tag=5, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="fixedMin", Tag=6, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="fixedTypical", Tag=7, Type=typing.Optional[uint]),
                     ])
 
-            mfgCode: 'typing.Optional[uint]' = None
-            value: 'uint' = 0
+            rangeMin: 'int' = 0
+            rangeMax: 'int' = 0
+            percentMax: 'typing.Optional[uint]' = None
+            percentMin: 'typing.Optional[uint]' = None
+            percentTypical: 'typing.Optional[uint]' = None
+            fixedMax: 'typing.Optional[uint]' = None
+            fixedMin: 'typing.Optional[uint]' = None
+            fixedTypical: 'typing.Optional[uint]' = None
 
         @dataclass
-        class ModeOptionStruct(ClusterObject):
+        class MeasurementAccuracyStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="label", Tag=0, Type=str),
-                        ClusterObjectFieldDescriptor(Label="mode", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="modeTags", Tag=2, Type=typing.List[RvcCleanMode.Structs.ModeTagStruct]),
+                        ClusterObjectFieldDescriptor(Label="measurementType", Tag=0, Type=ElectricalPowerMeasurement.Enums.MeasurementTypeEnum),
+                        ClusterObjectFieldDescriptor(Label="measured", Tag=1, Type=bool),
+                        ClusterObjectFieldDescriptor(Label="minMeasuredValue", Tag=2, Type=int),
+                        ClusterObjectFieldDescriptor(Label="maxMeasuredValue", Tag=3, Type=int),
+                        ClusterObjectFieldDescriptor(Label="accuracyRanges", Tag=4, Type=typing.List[ElectricalPowerMeasurement.Structs.MeasurementAccuracyRangeStruct]),
                     ])
 
-            label: 'str' = ""
-            mode: 'uint' = 0
-            modeTags: 'typing.List[RvcCleanMode.Structs.ModeTagStruct]' = field(default_factory=lambda: [])
+            measurementType: 'ElectricalPowerMeasurement.Enums.MeasurementTypeEnum' = 0
+            measured: 'bool' = False
+            minMeasuredValue: 'int' = 0
+            maxMeasuredValue: 'int' = 0
+            accuracyRanges: 'typing.List[ElectricalPowerMeasurement.Structs.MeasurementAccuracyRangeStruct]' = field(default_factory=lambda: [])
 
-    class Commands:
         @dataclass
-        class ChangeToMode(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000055
-            command_id: typing.ClassVar[int] = 0x00000000
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'ChangeToModeResponse'
-
+        class HarmonicMeasurementStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="newMode", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="order", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="measurement", Tag=1, Type=typing.Union[Nullable, int]),
                     ])
 
-            newMode: 'uint' = 0
+            order: 'uint' = 0
+            measurement: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
-        class ChangeToModeResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000055
-            command_id: typing.ClassVar[int] = 0x00000001
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
-
+        class MeasurementRangeStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="statusText", Tag=1, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="measurementType", Tag=0, Type=ElectricalPowerMeasurement.Enums.MeasurementTypeEnum),
+                        ClusterObjectFieldDescriptor(Label="min", Tag=1, Type=int),
+                        ClusterObjectFieldDescriptor(Label="max", Tag=2, Type=int),
+                        ClusterObjectFieldDescriptor(Label="startTimestamp", Tag=3, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="endTimestamp", Tag=4, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="minTimestamp", Tag=5, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="maxTimestamp", Tag=6, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="startSystime", Tag=7, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="endSystime", Tag=8, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="minSystime", Tag=9, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="maxSystime", Tag=10, Type=typing.Optional[uint]),
                     ])
 
-            status: 'uint' = 0
-            statusText: 'typing.Optional[str]' = None
+            measurementType: 'ElectricalPowerMeasurement.Enums.MeasurementTypeEnum' = 0
+            min: 'int' = 0
+            max: 'int' = 0
+            startTimestamp: 'typing.Optional[uint]' = None
+            endTimestamp: 'typing.Optional[uint]' = None
+            minTimestamp: 'typing.Optional[uint]' = None
+            maxTimestamp: 'typing.Optional[uint]' = None
+            startSystime: 'typing.Optional[uint]' = None
+            endSystime: 'typing.Optional[uint]' = None
+            minSystime: 'typing.Optional[uint]' = None
+            maxSystime: 'typing.Optional[uint]' = None
 
     class Attributes:
         @dataclass
-        class SupportedModes(ClusterAttributeDescriptor):
+        class PowerMode(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000055
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[RvcCleanMode.Structs.ModeOptionStruct])
+                return ClusterObjectFieldDescriptor(Type=ElectricalPowerMeasurement.Enums.PowerModeEnum)
 
-            value: 'typing.List[RvcCleanMode.Structs.ModeOptionStruct]' = field(default_factory=lambda: [])
+            value: 'ElectricalPowerMeasurement.Enums.PowerModeEnum' = 0
 
         @dataclass
-        class CurrentMode(ClusterAttributeDescriptor):
+        class NumberOfMeasurementTypes(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000055
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
         @dataclass
-        class OnMode(ClusterAttributeDescriptor):
+        class Accuracy(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000055
+                return 0x00000090
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[ElectricalPowerMeasurement.Structs.MeasurementAccuracyStruct])
+
+            value: 'typing.List[ElectricalPowerMeasurement.Structs.MeasurementAccuracyStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class Ranges(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[ElectricalPowerMeasurement.Structs.MeasurementRangeStruct]])
 
-            value: 'typing.Union[None, Nullable, uint]' = None
+            value: 'typing.Optional[typing.List[ElectricalPowerMeasurement.Structs.MeasurementRangeStruct]]' = None
 
         @dataclass
-        class GeneratedCommandList(ClusterAttributeDescriptor):
+        class Voltage(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000055
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFF8
+                return 0x00000004
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+            value: 'typing.Union[None, Nullable, int]' = None
 
         @dataclass
-        class AcceptedCommandList(ClusterAttributeDescriptor):
+        class ActiveCurrent(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000055
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFF9
+                return 0x00000005
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+            value: 'typing.Union[None, Nullable, int]' = None
 
         @dataclass
-        class EventList(ClusterAttributeDescriptor):
+        class ReactiveCurrent(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000055
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFFA
+                return 0x00000006
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+            value: 'typing.Union[None, Nullable, int]' = None
 
         @dataclass
-        class AttributeList(ClusterAttributeDescriptor):
+        class ApparentCurrent(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000055
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFFB
+                return 0x00000007
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+            value: 'typing.Union[None, Nullable, int]' = None
 
         @dataclass
-        class FeatureMap(ClusterAttributeDescriptor):
+        class ActivePower(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000055
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFFC
+                return 0x00000008
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'uint' = 0
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
-        class ClusterRevision(ClusterAttributeDescriptor):
+        class ReactivePower(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000055
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFFD
+                return 0x00000009
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-            value: 'uint' = 0
+            value: 'typing.Union[None, Nullable, int]' = None
 
+        @dataclass
+        class ApparentPower(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000090
 
-@dataclass
-class TemperatureControl(Cluster):
-    id: typing.ClassVar[int] = 0x00000056
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000000A
 
-    @ChipUtility.classproperty
-    def descriptor(cls) -> ClusterObjectDescriptor:
-        return ClusterObjectDescriptor(
-            Fields=[
-                ClusterObjectFieldDescriptor(Label="temperatureSetpoint", Tag=0x00000000, Type=typing.Optional[int]),
-                ClusterObjectFieldDescriptor(Label="minTemperature", Tag=0x00000001, Type=typing.Optional[int]),
-                ClusterObjectFieldDescriptor(Label="maxTemperature", Tag=0x00000002, Type=typing.Optional[int]),
-                ClusterObjectFieldDescriptor(Label="step", Tag=0x00000003, Type=typing.Optional[int]),
-                ClusterObjectFieldDescriptor(Label="selectedTemperatureLevel", Tag=0x00000004, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="supportedTemperatureLevels", Tag=0x00000005, Type=typing.Optional[typing.List[str]]),
-                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
-                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
-            ])
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-    temperatureSetpoint: 'typing.Optional[int]' = None
-    minTemperature: 'typing.Optional[int]' = None
-    maxTemperature: 'typing.Optional[int]' = None
-    step: 'typing.Optional[int]' = None
-    selectedTemperatureLevel: 'typing.Optional[uint]' = None
-    supportedTemperatureLevels: 'typing.Optional[typing.List[str]]' = None
-    generatedCommandList: 'typing.List[uint]' = None
-    acceptedCommandList: 'typing.List[uint]' = None
-    eventList: 'typing.List[uint]' = None
-    attributeList: 'typing.List[uint]' = None
-    featureMap: 'uint' = None
-    clusterRevision: 'uint' = None
+            value: 'typing.Union[None, Nullable, int]' = None
 
-    class Bitmaps:
-        class Feature(IntFlag):
-            kTemperatureNumber = 0x1
-            kTemperatureLevel = 0x2
-            kTemperatureStep = 0x4
+        @dataclass
+        class RMSVoltage(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000090
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000000B
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
+
+            value: 'typing.Union[None, Nullable, int]' = None
 
-    class Commands:
         @dataclass
-        class SetTemperature(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000056
-            command_id: typing.ClassVar[int] = 0x00000000
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = None
+        class RMSCurrent(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000090
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="targetTemperature", Tag=0, Type=typing.Optional[int]),
-                        ClusterObjectFieldDescriptor(Label="targetTemperatureLevel", Tag=1, Type=typing.Optional[uint]),
-                    ])
+            def attribute_id(cls) -> int:
+                return 0x0000000C
 
-            targetTemperature: 'typing.Optional[int]' = None
-            targetTemperatureLevel: 'typing.Optional[uint]' = None
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
+
+            value: 'typing.Union[None, Nullable, int]' = None
 
-    class Attributes:
         @dataclass
-        class TemperatureSetpoint(ClusterAttributeDescriptor):
+        class RMSPower(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000000
+                return 0x0000000D
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[int])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-            value: 'typing.Optional[int]' = None
+            value: 'typing.Union[None, Nullable, int]' = None
 
         @dataclass
-        class MinTemperature(ClusterAttributeDescriptor):
+        class Frequency(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000001
+                return 0x0000000E
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[int])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-            value: 'typing.Optional[int]' = None
+            value: 'typing.Union[None, Nullable, int]' = None
 
         @dataclass
-        class MaxTemperature(ClusterAttributeDescriptor):
+        class HarmonicCurrents(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000002
+                return 0x0000000F
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[int])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, typing.List[ElectricalPowerMeasurement.Structs.HarmonicMeasurementStruct]])
 
-            value: 'typing.Optional[int]' = None
+            value: 'typing.Union[None, Nullable, typing.List[ElectricalPowerMeasurement.Structs.HarmonicMeasurementStruct]]' = None
 
         @dataclass
-        class Step(ClusterAttributeDescriptor):
+        class HarmonicPhases(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000003
+                return 0x00000010
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[int])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, typing.List[ElectricalPowerMeasurement.Structs.HarmonicMeasurementStruct]])
 
-            value: 'typing.Optional[int]' = None
+            value: 'typing.Union[None, Nullable, typing.List[ElectricalPowerMeasurement.Structs.HarmonicMeasurementStruct]]' = None
 
         @dataclass
-        class SelectedTemperatureLevel(ClusterAttributeDescriptor):
+        class PowerFactor(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000004
+                return 0x00000011
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-            value: 'typing.Optional[uint]' = None
+            value: 'typing.Union[None, Nullable, int]' = None
 
         @dataclass
-        class SupportedTemperatureLevels(ClusterAttributeDescriptor):
+        class NeutralCurrent(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000005
+                return 0x00000012
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[str]])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-            value: 'typing.Optional[typing.List[str]]' = None
+            value: 'typing.Union[None, Nullable, int]' = None
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF8
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16803,15 +22692,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AcceptedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF9
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16819,15 +22708,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class EventList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFA
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16835,15 +22724,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AttributeList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFB
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16851,15 +22740,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class FeatureMap(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFC
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16867,114 +22756,295 @@
 
             value: 'uint' = 0
 
         @dataclass
         class ClusterRevision(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000056
+                return 0x00000090
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFD
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
+    class Events:
+        @dataclass
+        class MeasurementPeriodRanges(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000090
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="ranges", Tag=0, Type=typing.List[ElectricalPowerMeasurement.Structs.MeasurementRangeStruct]),
+                    ])
+
+            ranges: 'typing.List[ElectricalPowerMeasurement.Structs.MeasurementRangeStruct]' = field(default_factory=lambda: [])
+
 
 @dataclass
-class RefrigeratorAlarm(Cluster):
-    id: typing.ClassVar[int] = 0x00000057
+class ElectricalEnergyMeasurement(Cluster):
+    id: typing.ClassVar[int] = 0x00000091
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
-                ClusterObjectFieldDescriptor(Label="mask", Tag=0x00000000, Type=uint),
-                ClusterObjectFieldDescriptor(Label="state", Tag=0x00000002, Type=uint),
-                ClusterObjectFieldDescriptor(Label="supported", Tag=0x00000003, Type=uint),
+                ClusterObjectFieldDescriptor(Label="accuracy", Tag=0x00000000, Type=ElectricalEnergyMeasurement.Structs.MeasurementAccuracyStruct),
+                ClusterObjectFieldDescriptor(Label="cumulativeEnergyImported", Tag=0x00000001, Type=typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]),
+                ClusterObjectFieldDescriptor(Label="cumulativeEnergyExported", Tag=0x00000002, Type=typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]),
+                ClusterObjectFieldDescriptor(Label="periodicEnergyImported", Tag=0x00000003, Type=typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]),
+                ClusterObjectFieldDescriptor(Label="periodicEnergyExported", Tag=0x00000004, Type=typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]),
+                ClusterObjectFieldDescriptor(Label="cumulativeEnergyReset", Tag=0x00000005, Type=typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.CumulativeEnergyResetStruct]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
 
-    mask: 'uint' = None
-    state: 'uint' = None
-    supported: 'uint' = None
+    accuracy: 'ElectricalEnergyMeasurement.Structs.MeasurementAccuracyStruct' = None
+    cumulativeEnergyImported: 'typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
+    cumulativeEnergyExported: 'typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
+    periodicEnergyImported: 'typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
+    periodicEnergyExported: 'typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
+    cumulativeEnergyReset: 'typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.CumulativeEnergyResetStruct]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
+    class Enums:
+        class MeasurementTypeEnum(MatterIntEnum):
+            kUnspecified = 0x00
+            kVoltage = 0x01
+            kActiveCurrent = 0x02
+            kReactiveCurrent = 0x03
+            kApparentCurrent = 0x04
+            kActivePower = 0x05
+            kReactivePower = 0x06
+            kApparentPower = 0x07
+            kRMSVoltage = 0x08
+            kRMSCurrent = 0x09
+            kRMSPower = 0x0A
+            kFrequency = 0x0B
+            kPowerFactor = 0x0C
+            kNeutralCurrent = 0x0D
+            kElectricalEnergy = 0x0E
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 15,
+
     class Bitmaps:
-        class AlarmMap(IntFlag):
-            kDoorOpen = 0x1
+        class Feature(IntFlag):
+            kImportedEnergy = 0x1
+            kExportedEnergy = 0x2
+            kCumulativeEnergy = 0x4
+            kPeriodicEnergy = 0x8
+
+    class Structs:
+        @dataclass
+        class MeasurementAccuracyRangeStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="rangeMin", Tag=0, Type=int),
+                        ClusterObjectFieldDescriptor(Label="rangeMax", Tag=1, Type=int),
+                        ClusterObjectFieldDescriptor(Label="percentMax", Tag=2, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="percentMin", Tag=3, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="percentTypical", Tag=4, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="fixedMax", Tag=5, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="fixedMin", Tag=6, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="fixedTypical", Tag=7, Type=typing.Optional[uint]),
+                    ])
+
+            rangeMin: 'int' = 0
+            rangeMax: 'int' = 0
+            percentMax: 'typing.Optional[uint]' = None
+            percentMin: 'typing.Optional[uint]' = None
+            percentTypical: 'typing.Optional[uint]' = None
+            fixedMax: 'typing.Optional[uint]' = None
+            fixedMin: 'typing.Optional[uint]' = None
+            fixedTypical: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class MeasurementAccuracyStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="measurementType", Tag=0, Type=ElectricalEnergyMeasurement.Enums.MeasurementTypeEnum),
+                        ClusterObjectFieldDescriptor(Label="measured", Tag=1, Type=bool),
+                        ClusterObjectFieldDescriptor(Label="minMeasuredValue", Tag=2, Type=int),
+                        ClusterObjectFieldDescriptor(Label="maxMeasuredValue", Tag=3, Type=int),
+                        ClusterObjectFieldDescriptor(Label="accuracyRanges", Tag=4, Type=typing.List[ElectricalEnergyMeasurement.Structs.MeasurementAccuracyRangeStruct]),
+                    ])
+
+            measurementType: 'ElectricalEnergyMeasurement.Enums.MeasurementTypeEnum' = 0
+            measured: 'bool' = False
+            minMeasuredValue: 'int' = 0
+            maxMeasuredValue: 'int' = 0
+            accuracyRanges: 'typing.List[ElectricalEnergyMeasurement.Structs.MeasurementAccuracyRangeStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class CumulativeEnergyResetStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="importedResetTimestamp", Tag=0, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="exportedResetTimestamp", Tag=1, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="importedResetSystime", Tag=2, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="exportedResetSystime", Tag=3, Type=typing.Union[None, Nullable, uint]),
+                    ])
+
+            importedResetTimestamp: 'typing.Union[None, Nullable, uint]' = None
+            exportedResetTimestamp: 'typing.Union[None, Nullable, uint]' = None
+            importedResetSystime: 'typing.Union[None, Nullable, uint]' = None
+            exportedResetSystime: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class EnergyMeasurementStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="energy", Tag=0, Type=int),
+                        ClusterObjectFieldDescriptor(Label="startTimestamp", Tag=1, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="endTimestamp", Tag=2, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="startSystime", Tag=3, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="endSystime", Tag=4, Type=typing.Optional[uint]),
+                    ])
+
+            energy: 'int' = 0
+            startTimestamp: 'typing.Optional[uint]' = None
+            endTimestamp: 'typing.Optional[uint]' = None
+            startSystime: 'typing.Optional[uint]' = None
+            endSystime: 'typing.Optional[uint]' = None
 
     class Attributes:
         @dataclass
-        class Mask(ClusterAttributeDescriptor):
+        class Accuracy(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000057
+                return 0x00000091
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=ElectricalEnergyMeasurement.Structs.MeasurementAccuracyStruct)
 
-            value: 'uint' = 0
+            value: 'ElectricalEnergyMeasurement.Structs.MeasurementAccuracyStruct' = field(default_factory=lambda: ElectricalEnergyMeasurement.Structs.MeasurementAccuracyStruct())
 
         @dataclass
-        class State(ClusterAttributeDescriptor):
+        class CumulativeEnergyImported(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000057
+                return 0x00000091
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct])
+
+            value: 'typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
+
+        @dataclass
+        class CumulativeEnergyExported(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000091
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct])
 
-            value: 'uint' = 0
+            value: 'typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
 
         @dataclass
-        class Supported(ClusterAttributeDescriptor):
+        class PeriodicEnergyImported(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000057
+                return 0x00000091
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct])
 
-            value: 'uint' = 0
+            value: 'typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
+
+        @dataclass
+        class PeriodicEnergyExported(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000091
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct])
+
+            value: 'typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
+
+        @dataclass
+        class CumulativeEnergyReset(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000091
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.CumulativeEnergyResetStruct])
+
+            value: 'typing.Union[None, Nullable, ElectricalEnergyMeasurement.Structs.CumulativeEnergyResetStruct]' = None
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000057
+                return 0x00000091
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF8
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16982,15 +23052,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AcceptedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000057
+                return 0x00000091
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF9
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -16998,15 +23068,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class EventList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000057
+                return 0x00000091
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFA
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17014,15 +23084,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AttributeList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000057
+                return 0x00000091
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFB
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17030,15 +23100,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class FeatureMap(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000057
+                return 0x00000091
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFC
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17046,233 +23116,548 @@
 
             value: 'uint' = 0
 
         @dataclass
         class ClusterRevision(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000057
+                return 0x00000091
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFD
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
     class Events:
         @dataclass
-        class Notify(ClusterEvent):
+        class CumulativeEnergyMeasured(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000057
+                return 0x00000091
 
             @ChipUtility.classproperty
             def event_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="active", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="inactive", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="state", Tag=2, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="mask", Tag=3, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="energyImported", Tag=0, Type=typing.Optional[ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]),
+                        ClusterObjectFieldDescriptor(Label="energyExported", Tag=1, Type=typing.Optional[ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]),
                     ])
 
-            active: 'uint' = 0
-            inactive: 'uint' = 0
-            state: 'uint' = 0
-            mask: 'uint' = 0
+            energyImported: 'typing.Optional[ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
+            energyExported: 'typing.Optional[ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
+
+        @dataclass
+        class PeriodicEnergyMeasured(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000091
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="energyImported", Tag=0, Type=typing.Optional[ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]),
+                        ClusterObjectFieldDescriptor(Label="energyExported", Tag=1, Type=typing.Optional[ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]),
+                    ])
+
+            energyImported: 'typing.Optional[ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
+            energyExported: 'typing.Optional[ElectricalEnergyMeasurement.Structs.EnergyMeasurementStruct]' = None
 
 
 @dataclass
-class DishwasherMode(Cluster):
-    id: typing.ClassVar[int] = 0x00000059
+class DemandResponseLoadControl(Cluster):
+    id: typing.ClassVar[int] = 0x00000096
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
-                ClusterObjectFieldDescriptor(Label="supportedModes", Tag=0x00000000, Type=typing.List[DishwasherMode.Structs.ModeOptionStruct]),
-                ClusterObjectFieldDescriptor(Label="currentMode", Tag=0x00000001, Type=uint),
-                ClusterObjectFieldDescriptor(Label="startUpMode", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
-                ClusterObjectFieldDescriptor(Label="onMode", Tag=0x00000003, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="loadControlPrograms", Tag=0x00000000, Type=typing.List[DemandResponseLoadControl.Structs.LoadControlProgramStruct]),
+                ClusterObjectFieldDescriptor(Label="numberOfLoadControlPrograms", Tag=0x00000001, Type=uint),
+                ClusterObjectFieldDescriptor(Label="events", Tag=0x00000002, Type=typing.List[DemandResponseLoadControl.Structs.LoadControlEventStruct]),
+                ClusterObjectFieldDescriptor(Label="activeEvents", Tag=0x00000003, Type=typing.List[DemandResponseLoadControl.Structs.LoadControlEventStruct]),
+                ClusterObjectFieldDescriptor(Label="numberOfEventsPerProgram", Tag=0x00000004, Type=uint),
+                ClusterObjectFieldDescriptor(Label="numberOfTransitions", Tag=0x00000005, Type=uint),
+                ClusterObjectFieldDescriptor(Label="defaultRandomStart", Tag=0x00000006, Type=uint),
+                ClusterObjectFieldDescriptor(Label="defaultRandomDuration", Tag=0x00000007, Type=uint),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
 
-    supportedModes: 'typing.List[DishwasherMode.Structs.ModeOptionStruct]' = None
-    currentMode: 'uint' = None
-    startUpMode: 'typing.Union[None, Nullable, uint]' = None
-    onMode: 'typing.Union[None, Nullable, uint]' = None
+    loadControlPrograms: 'typing.List[DemandResponseLoadControl.Structs.LoadControlProgramStruct]' = None
+    numberOfLoadControlPrograms: 'uint' = None
+    events: 'typing.List[DemandResponseLoadControl.Structs.LoadControlEventStruct]' = None
+    activeEvents: 'typing.List[DemandResponseLoadControl.Structs.LoadControlEventStruct]' = None
+    numberOfEventsPerProgram: 'uint' = None
+    numberOfTransitions: 'uint' = None
+    defaultRandomStart: 'uint' = None
+    defaultRandomDuration: 'uint' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class ModeTag(MatterIntEnum):
-            kNormal = 0x4000
-            kHeavy = 0x4001
-            kLight = 0x4002
-            # kUnknownEnumValue intentionally not defined. This enum never goes
-            # through DataModel::Decode, likely because it is a part of a derived
-            # cluster. As a result having kUnknownEnumValue in this enum is error
-            # prone, and was removed. See
-            # src/app/common/templates/config-data.yaml.
+        class CriticalityLevelEnum(MatterIntEnum):
+            kUnknown = 0x00
+            kGreen = 0x01
+            kLevel1 = 0x02
+            kLevel2 = 0x03
+            kLevel3 = 0x04
+            kLevel4 = 0x05
+            kLevel5 = 0x06
+            kEmergency = 0x07
+            kPlannedOutage = 0x08
+            kServiceDisconnect = 0x09
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 10,
+
+        class HeatingSourceEnum(MatterIntEnum):
+            kAny = 0x00
+            kElectric = 0x01
+            kNonElectric = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 3,
+
+        class LoadControlEventChangeSourceEnum(MatterIntEnum):
+            kAutomatic = 0x00
+            kUserAction = 0x01
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 2,
+
+        class LoadControlEventStatusEnum(MatterIntEnum):
+            kUnknown = 0x00
+            kReceived = 0x01
+            kInProgress = 0x02
+            kCompleted = 0x03
+            kOptedOut = 0x04
+            kOptedIn = 0x05
+            kCanceled = 0x06
+            kSuperseded = 0x07
+            kPartialOptedOut = 0x08
+            kPartialOptedIn = 0x09
+            kNoParticipation = 0x0A
+            kUnavailable = 0x0B
+            kFailed = 0x0C
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 13,
 
     class Bitmaps:
+        class CancelControlBitmap(IntFlag):
+            kRandomEnd = 0x1
+
+        class DeviceClassBitmap(IntFlag):
+            kHvac = 0x1
+            kStripHeater = 0x2
+            kWaterHeater = 0x4
+            kPoolPump = 0x8
+            kSmartAppliance = 0x10
+            kIrrigationPump = 0x20
+            kCommercialLoad = 0x40
+            kResidentialLoad = 0x80
+            kExteriorLighting = 0x100
+            kInteriorLighting = 0x200
+            kEv = 0x400
+            kGenerationSystem = 0x800
+            kSmartInverter = 0x1000
+            kEvse = 0x2000
+            kResu = 0x4000
+            kEms = 0x8000
+            kSem = 0x10000
+
+        class EventControlBitmap(IntFlag):
+            kRandomStart = 0x1
+
+        class EventTransitionControlBitmap(IntFlag):
+            kRandomDuration = 0x1
+            kIgnoreOptOut = 0x2
+
         class Feature(IntFlag):
-            kOnOff = 0x1
+            kEnrollmentGroups = 0x1
+            kTemperatureOffset = 0x2
+            kTemperatureSetpoint = 0x4
+            kLoadAdjustment = 0x8
+            kDutyCycle = 0x10
+            kPowerSavings = 0x20
+            kHeatingSource = 0x40
 
     class Structs:
         @dataclass
-        class ModeTagStruct(ClusterObject):
+        class HeatingSourceControlStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="mfgCode", Tag=0, Type=typing.Optional[uint]),
-                        ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="heatingSource", Tag=0, Type=DemandResponseLoadControl.Enums.HeatingSourceEnum),
                     ])
 
-            mfgCode: 'typing.Optional[uint]' = None
-            value: 'uint' = 0
+            heatingSource: 'DemandResponseLoadControl.Enums.HeatingSourceEnum' = 0
 
         @dataclass
-        class ModeOptionStruct(ClusterObject):
+        class PowerSavingsControlStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="label", Tag=0, Type=str),
-                        ClusterObjectFieldDescriptor(Label="mode", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="modeTags", Tag=2, Type=typing.List[DishwasherMode.Structs.ModeTagStruct]),
+                        ClusterObjectFieldDescriptor(Label="powerSavings", Tag=0, Type=uint),
                     ])
 
-            label: 'str' = ""
-            mode: 'uint' = 0
-            modeTags: 'typing.List[DishwasherMode.Structs.ModeTagStruct]' = field(default_factory=lambda: [])
+            powerSavings: 'uint' = 0
+
+        @dataclass
+        class DutyCycleControlStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="dutyCycle", Tag=0, Type=uint),
+                    ])
+
+            dutyCycle: 'uint' = 0
+
+        @dataclass
+        class AverageLoadControlStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="loadAdjustment", Tag=0, Type=int),
+                    ])
+
+            loadAdjustment: 'int' = 0
+
+        @dataclass
+        class TemperatureControlStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="coolingTempOffset", Tag=0, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="heatingtTempOffset", Tag=1, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="coolingTempSetpoint", Tag=2, Type=typing.Union[None, Nullable, int]),
+                        ClusterObjectFieldDescriptor(Label="heatingTempSetpoint", Tag=3, Type=typing.Union[None, Nullable, int]),
+                    ])
+
+            coolingTempOffset: 'typing.Union[None, Nullable, uint]' = None
+            heatingtTempOffset: 'typing.Union[None, Nullable, uint]' = None
+            coolingTempSetpoint: 'typing.Union[None, Nullable, int]' = None
+            heatingTempSetpoint: 'typing.Union[None, Nullable, int]' = None
+
+        @dataclass
+        class LoadControlEventTransitionStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="duration", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="control", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="temperatureControl", Tag=2, Type=typing.Optional[DemandResponseLoadControl.Structs.TemperatureControlStruct]),
+                        ClusterObjectFieldDescriptor(Label="averageLoadControl", Tag=3, Type=typing.Optional[DemandResponseLoadControl.Structs.AverageLoadControlStruct]),
+                        ClusterObjectFieldDescriptor(Label="dutyCycleControl", Tag=4, Type=typing.Optional[DemandResponseLoadControl.Structs.DutyCycleControlStruct]),
+                        ClusterObjectFieldDescriptor(Label="powerSavingsControl", Tag=5, Type=typing.Optional[DemandResponseLoadControl.Structs.PowerSavingsControlStruct]),
+                        ClusterObjectFieldDescriptor(Label="heatingSourceControl", Tag=6, Type=typing.Optional[DemandResponseLoadControl.Structs.HeatingSourceControlStruct]),
+                    ])
+
+            duration: 'uint' = 0
+            control: 'uint' = 0
+            temperatureControl: 'typing.Optional[DemandResponseLoadControl.Structs.TemperatureControlStruct]' = None
+            averageLoadControl: 'typing.Optional[DemandResponseLoadControl.Structs.AverageLoadControlStruct]' = None
+            dutyCycleControl: 'typing.Optional[DemandResponseLoadControl.Structs.DutyCycleControlStruct]' = None
+            powerSavingsControl: 'typing.Optional[DemandResponseLoadControl.Structs.PowerSavingsControlStruct]' = None
+            heatingSourceControl: 'typing.Optional[DemandResponseLoadControl.Structs.HeatingSourceControlStruct]' = None
+
+        @dataclass
+        class LoadControlEventStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="eventID", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="programID", Tag=1, Type=typing.Union[Nullable, bytes]),
+                        ClusterObjectFieldDescriptor(Label="control", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="deviceClass", Tag=3, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="enrollmentGroup", Tag=4, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="criticality", Tag=5, Type=DemandResponseLoadControl.Enums.CriticalityLevelEnum),
+                        ClusterObjectFieldDescriptor(Label="startTime", Tag=6, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="transitions", Tag=7, Type=typing.List[DemandResponseLoadControl.Structs.LoadControlEventTransitionStruct]),
+                    ])
+
+            eventID: 'bytes' = b""
+            programID: 'typing.Union[Nullable, bytes]' = NullValue
+            control: 'uint' = 0
+            deviceClass: 'uint' = 0
+            enrollmentGroup: 'typing.Optional[uint]' = None
+            criticality: 'DemandResponseLoadControl.Enums.CriticalityLevelEnum' = 0
+            startTime: 'typing.Union[Nullable, uint]' = NullValue
+            transitions: 'typing.List[DemandResponseLoadControl.Structs.LoadControlEventTransitionStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class LoadControlProgramStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="programID", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="name", Tag=1, Type=str),
+                        ClusterObjectFieldDescriptor(Label="enrollmentGroup", Tag=2, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="randomStartMinutes", Tag=3, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="randomDurationMinutes", Tag=4, Type=typing.Union[Nullable, uint]),
+                    ])
+
+            programID: 'bytes' = b""
+            name: 'str' = ""
+            enrollmentGroup: 'typing.Union[Nullable, uint]' = NullValue
+            randomStartMinutes: 'typing.Union[Nullable, uint]' = NullValue
+            randomDurationMinutes: 'typing.Union[Nullable, uint]' = NullValue
 
     class Commands:
         @dataclass
-        class ChangeToMode(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000059
+        class RegisterLoadControlProgramRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000096
             command_id: typing.ClassVar[int] = 0x00000000
             is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'ChangeToModeResponse'
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="newMode", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="loadControlProgram", Tag=0, Type=DemandResponseLoadControl.Structs.LoadControlProgramStruct),
                     ])
 
-            newMode: 'uint' = 0
+            loadControlProgram: 'DemandResponseLoadControl.Structs.LoadControlProgramStruct' = field(default_factory=lambda: DemandResponseLoadControl.Structs.LoadControlProgramStruct())
 
         @dataclass
-        class ChangeToModeResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000059
+        class UnregisterLoadControlProgramRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000096
             command_id: typing.ClassVar[int] = 0x00000001
-            is_client: typing.ClassVar[bool] = False
+            is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="statusText", Tag=1, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="loadControlProgramID", Tag=0, Type=bytes),
                     ])
 
-            status: 'uint' = 0
-            statusText: 'typing.Optional[str]' = None
+            loadControlProgramID: 'bytes' = b""
+
+        @dataclass
+        class AddLoadControlEventRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000096
+            command_id: typing.ClassVar[int] = 0x00000002
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="event", Tag=0, Type=DemandResponseLoadControl.Structs.LoadControlEventStruct),
+                    ])
+
+            event: 'DemandResponseLoadControl.Structs.LoadControlEventStruct' = field(default_factory=lambda: DemandResponseLoadControl.Structs.LoadControlEventStruct())
+
+        @dataclass
+        class RemoveLoadControlEventRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000096
+            command_id: typing.ClassVar[int] = 0x00000003
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="eventID", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="cancelControl", Tag=1, Type=uint),
+                    ])
+
+            eventID: 'bytes' = b""
+            cancelControl: 'uint' = 0
+
+        @dataclass
+        class ClearLoadControlEventsRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000096
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
 
     class Attributes:
         @dataclass
-        class SupportedModes(ClusterAttributeDescriptor):
+        class LoadControlPrograms(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000059
+                return 0x00000096
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[DishwasherMode.Structs.ModeOptionStruct])
+                return ClusterObjectFieldDescriptor(Type=typing.List[DemandResponseLoadControl.Structs.LoadControlProgramStruct])
 
-            value: 'typing.List[DishwasherMode.Structs.ModeOptionStruct]' = field(default_factory=lambda: [])
+            value: 'typing.List[DemandResponseLoadControl.Structs.LoadControlProgramStruct]' = field(default_factory=lambda: [])
 
         @dataclass
-        class CurrentMode(ClusterAttributeDescriptor):
+        class NumberOfLoadControlPrograms(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000059
+                return 0x00000096
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
         @dataclass
-        class StartUpMode(ClusterAttributeDescriptor):
+        class Events(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000059
+                return 0x00000096
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+                return ClusterObjectFieldDescriptor(Type=typing.List[DemandResponseLoadControl.Structs.LoadControlEventStruct])
 
-            value: 'typing.Union[None, Nullable, uint]' = None
+            value: 'typing.List[DemandResponseLoadControl.Structs.LoadControlEventStruct]' = field(default_factory=lambda: [])
 
         @dataclass
-        class OnMode(ClusterAttributeDescriptor):
+        class ActiveEvents(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000059
+                return 0x00000096
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+                return ClusterObjectFieldDescriptor(Type=typing.List[DemandResponseLoadControl.Structs.LoadControlEventStruct])
 
-            value: 'typing.Union[None, Nullable, uint]' = None
+            value: 'typing.List[DemandResponseLoadControl.Structs.LoadControlEventStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class NumberOfEventsPerProgram(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000096
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class NumberOfTransitions(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000096
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class DefaultRandomStart(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000096
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000006
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class DefaultRandomDuration(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000096
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000007
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000059
+                return 0x00000096
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF8
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17280,15 +23665,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AcceptedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000059
+                return 0x00000096
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF9
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17296,15 +23681,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class EventList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000059
+                return 0x00000096
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFA
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17312,15 +23697,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AttributeList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000059
+                return 0x00000096
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFB
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17328,15 +23713,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class FeatureMap(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000059
+                return 0x00000096
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFC
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17344,96 +23729,250 @@
 
             value: 'uint' = 0
 
         @dataclass
         class ClusterRevision(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000059
+                return 0x00000096
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFD
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
+    class Events:
+        @dataclass
+        class LoadControlEventStatusChange(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000096
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="eventID", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="transitionIndex", Tag=1, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="status", Tag=2, Type=DemandResponseLoadControl.Enums.LoadControlEventStatusEnum),
+                        ClusterObjectFieldDescriptor(Label="criticality", Tag=3, Type=DemandResponseLoadControl.Enums.CriticalityLevelEnum),
+                        ClusterObjectFieldDescriptor(Label="control", Tag=4, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="temperatureControl", Tag=5, Type=typing.Union[None, Nullable, DemandResponseLoadControl.Structs.TemperatureControlStruct]),
+                        ClusterObjectFieldDescriptor(Label="averageLoadControl", Tag=6, Type=typing.Union[None, Nullable, DemandResponseLoadControl.Structs.AverageLoadControlStruct]),
+                        ClusterObjectFieldDescriptor(Label="dutyCycleControl", Tag=7, Type=typing.Union[None, Nullable, DemandResponseLoadControl.Structs.DutyCycleControlStruct]),
+                        ClusterObjectFieldDescriptor(Label="powerSavingsControl", Tag=8, Type=typing.Union[None, Nullable, DemandResponseLoadControl.Structs.PowerSavingsControlStruct]),
+                        ClusterObjectFieldDescriptor(Label="heatingSourceControl", Tag=9, Type=typing.Union[None, Nullable, DemandResponseLoadControl.Structs.HeatingSourceControlStruct]),
+                    ])
+
+            eventID: 'bytes' = b""
+            transitionIndex: 'typing.Union[Nullable, uint]' = NullValue
+            status: 'DemandResponseLoadControl.Enums.LoadControlEventStatusEnum' = 0
+            criticality: 'DemandResponseLoadControl.Enums.CriticalityLevelEnum' = 0
+            control: 'uint' = 0
+            temperatureControl: 'typing.Union[None, Nullable, DemandResponseLoadControl.Structs.TemperatureControlStruct]' = None
+            averageLoadControl: 'typing.Union[None, Nullable, DemandResponseLoadControl.Structs.AverageLoadControlStruct]' = None
+            dutyCycleControl: 'typing.Union[None, Nullable, DemandResponseLoadControl.Structs.DutyCycleControlStruct]' = None
+            powerSavingsControl: 'typing.Union[None, Nullable, DemandResponseLoadControl.Structs.PowerSavingsControlStruct]' = None
+            heatingSourceControl: 'typing.Union[None, Nullable, DemandResponseLoadControl.Structs.HeatingSourceControlStruct]' = None
+
 
 @dataclass
-class AirQuality(Cluster):
-    id: typing.ClassVar[int] = 0x0000005B
+class Messages(Cluster):
+    id: typing.ClassVar[int] = 0x00000097
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
-                ClusterObjectFieldDescriptor(Label="airQuality", Tag=0x00000000, Type=AirQuality.Enums.AirQualityEnum),
+                ClusterObjectFieldDescriptor(Label="messages", Tag=0x00000000, Type=typing.List[Messages.Structs.MessageStruct]),
+                ClusterObjectFieldDescriptor(Label="activeMessageIDs", Tag=0x00000001, Type=typing.List[bytes]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
 
-    airQuality: 'AirQuality.Enums.AirQualityEnum' = None
+    messages: 'typing.List[Messages.Structs.MessageStruct]' = None
+    activeMessageIDs: 'typing.List[bytes]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class AirQualityEnum(MatterIntEnum):
-            kUnknown = 0x00
-            kGood = 0x01
-            kFair = 0x02
-            kModerate = 0x03
-            kPoor = 0x04
-            kVeryPoor = 0x05
-            kExtremelyPoor = 0x06
+        class FutureMessagePreferenceEnum(MatterIntEnum):
+            kAllowed = 0x00
+            kIncreased = 0x01
+            kReduced = 0x02
+            kDisallowed = 0x03
+            kBanned = 0x04
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 7,
+            kUnknownEnumValue = 5,
+
+        class MessagePriorityEnum(MatterIntEnum):
+            kLow = 0x00
+            kMedium = 0x01
+            kHigh = 0x02
+            kCritical = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
 
     class Bitmaps:
         class Feature(IntFlag):
-            kFair = 0x1
-            kModerate = 0x2
-            kVeryPoor = 0x4
-            kExtremelyPoor = 0x8
+            kReceivedConfirmation = 0x1
+            kConfirmationResponse = 0x2
+            kConfirmationReply = 0x4
+            kProtectedMessages = 0x8
+
+        class MessageControlBitmap(IntFlag):
+            kConfirmationRequired = 0x1
+            kResponseRequired = 0x2
+            kReplyMessage = 0x4
+            kMessageConfirmed = 0x8
+            kMessageProtected = 0x10
+
+    class Structs:
+        @dataclass
+        class MessageResponseOptionStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="messageResponseID", Tag=0, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="label", Tag=1, Type=typing.Optional[str]),
+                    ])
+
+            messageResponseID: 'typing.Optional[uint]' = None
+            label: 'typing.Optional[str]' = None
+
+        @dataclass
+        class MessageStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="messageID", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="priority", Tag=1, Type=Messages.Enums.MessagePriorityEnum),
+                        ClusterObjectFieldDescriptor(Label="messageControl", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="startTime", Tag=3, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="duration", Tag=4, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="messageText", Tag=5, Type=str),
+                        ClusterObjectFieldDescriptor(Label="responses", Tag=6, Type=typing.Optional[typing.List[Messages.Structs.MessageResponseOptionStruct]]),
+                    ])
+
+            messageID: 'bytes' = b""
+            priority: 'Messages.Enums.MessagePriorityEnum' = 0
+            messageControl: 'uint' = 0
+            startTime: 'typing.Union[Nullable, uint]' = NullValue
+            duration: 'typing.Union[Nullable, uint]' = NullValue
+            messageText: 'str' = ""
+            responses: 'typing.Optional[typing.List[Messages.Structs.MessageResponseOptionStruct]]' = None
+
+    class Commands:
+        @dataclass
+        class PresentMessagesRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000097
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="messageID", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="priority", Tag=1, Type=Messages.Enums.MessagePriorityEnum),
+                        ClusterObjectFieldDescriptor(Label="messageControl", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="startTime", Tag=3, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="duration", Tag=4, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="messageText", Tag=5, Type=str),
+                        ClusterObjectFieldDescriptor(Label="responses", Tag=6, Type=typing.Optional[typing.List[Messages.Structs.MessageResponseOptionStruct]]),
+                    ])
+
+            messageID: 'bytes' = b""
+            priority: 'Messages.Enums.MessagePriorityEnum' = 0
+            messageControl: 'uint' = 0
+            startTime: 'typing.Union[Nullable, uint]' = NullValue
+            duration: 'typing.Union[Nullable, uint]' = NullValue
+            messageText: 'str' = ""
+            responses: 'typing.Optional[typing.List[Messages.Structs.MessageResponseOptionStruct]]' = None
+
+        @dataclass
+        class CancelMessagesRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000097
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="messageIDs", Tag=0, Type=typing.List[bytes]),
+                    ])
+
+            messageIDs: 'typing.List[bytes]' = field(default_factory=lambda: [])
 
     class Attributes:
         @dataclass
-        class AirQuality(ClusterAttributeDescriptor):
+        class Messages(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005B
+                return 0x00000097
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=AirQuality.Enums.AirQualityEnum)
+                return ClusterObjectFieldDescriptor(Type=typing.List[Messages.Structs.MessageStruct])
 
-            value: 'AirQuality.Enums.AirQualityEnum' = 0
+            value: 'typing.List[Messages.Structs.MessageStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class ActiveMessageIDs(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000097
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[bytes])
+
+            value: 'typing.List[bytes]' = field(default_factory=lambda: [])
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005B
+                return 0x00000097
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF8
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17441,15 +23980,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AcceptedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005B
+                return 0x00000097
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF9
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17457,15 +23996,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class EventList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005B
+                return 0x00000097
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFA
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17473,15 +24012,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AttributeList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005B
+                return 0x00000097
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFB
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17489,15 +24028,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class FeatureMap(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005B
+                return 0x00000097
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFC
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17505,375 +24044,637 @@
 
             value: 'uint' = 0
 
         @dataclass
         class ClusterRevision(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005B
+                return 0x00000097
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFD
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
+    class Events:
+        @dataclass
+        class MessageQueued(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000097
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="messageID", Tag=0, Type=bytes),
+                    ])
+
+            messageID: 'bytes' = b""
+
+        @dataclass
+        class MessagePresented(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000097
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="messageID", Tag=0, Type=bytes),
+                    ])
+
+            messageID: 'bytes' = b""
+
+        @dataclass
+        class MessageComplete(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000097
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="messageID", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="responseID", Tag=1, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="reply", Tag=2, Type=typing.Union[None, Nullable, str]),
+                        ClusterObjectFieldDescriptor(Label="futureMessagesPreference", Tag=3, Type=typing.Union[Nullable, Messages.Enums.FutureMessagePreferenceEnum]),
+                    ])
+
+            messageID: 'bytes' = b""
+            responseID: 'typing.Union[None, Nullable, uint]' = None
+            reply: 'typing.Union[None, Nullable, str]' = None
+            futureMessagesPreference: 'typing.Union[Nullable, Messages.Enums.FutureMessagePreferenceEnum]' = NullValue
+
 
 @dataclass
-class SmokeCoAlarm(Cluster):
-    id: typing.ClassVar[int] = 0x0000005C
+class DeviceEnergyManagement(Cluster):
+    id: typing.ClassVar[int] = 0x00000098
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
-                ClusterObjectFieldDescriptor(Label="expressedState", Tag=0x00000000, Type=SmokeCoAlarm.Enums.ExpressedStateEnum),
-                ClusterObjectFieldDescriptor(Label="smokeState", Tag=0x00000001, Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]),
-                ClusterObjectFieldDescriptor(Label="COState", Tag=0x00000002, Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]),
-                ClusterObjectFieldDescriptor(Label="batteryAlert", Tag=0x00000003, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
-                ClusterObjectFieldDescriptor(Label="deviceMuted", Tag=0x00000004, Type=typing.Optional[SmokeCoAlarm.Enums.MuteStateEnum]),
-                ClusterObjectFieldDescriptor(Label="testInProgress", Tag=0x00000005, Type=bool),
-                ClusterObjectFieldDescriptor(Label="hardwareFaultAlert", Tag=0x00000006, Type=bool),
-                ClusterObjectFieldDescriptor(Label="endOfServiceAlert", Tag=0x00000007, Type=SmokeCoAlarm.Enums.EndOfServiceEnum),
-                ClusterObjectFieldDescriptor(Label="interconnectSmokeAlarm", Tag=0x00000008, Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]),
-                ClusterObjectFieldDescriptor(Label="interconnectCOAlarm", Tag=0x00000009, Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]),
-                ClusterObjectFieldDescriptor(Label="contaminationState", Tag=0x0000000A, Type=typing.Optional[SmokeCoAlarm.Enums.ContaminationStateEnum]),
-                ClusterObjectFieldDescriptor(Label="smokeSensitivityLevel", Tag=0x0000000B, Type=typing.Optional[SmokeCoAlarm.Enums.SensitivityEnum]),
-                ClusterObjectFieldDescriptor(Label="expiryDate", Tag=0x0000000C, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="ESAType", Tag=0x00000000, Type=DeviceEnergyManagement.Enums.ESATypeEnum),
+                ClusterObjectFieldDescriptor(Label="ESACanGenerate", Tag=0x00000001, Type=bool),
+                ClusterObjectFieldDescriptor(Label="ESAState", Tag=0x00000002, Type=DeviceEnergyManagement.Enums.ESAStateEnum),
+                ClusterObjectFieldDescriptor(Label="absMinPower", Tag=0x00000003, Type=int),
+                ClusterObjectFieldDescriptor(Label="absMaxPower", Tag=0x00000004, Type=int),
+                ClusterObjectFieldDescriptor(Label="powerAdjustmentCapability", Tag=0x00000005, Type=typing.Union[None, Nullable, typing.List[DeviceEnergyManagement.Structs.PowerAdjustStruct]]),
+                ClusterObjectFieldDescriptor(Label="forecast", Tag=0x00000006, Type=typing.Union[None, Nullable, DeviceEnergyManagement.Structs.ForecastStruct]),
+                ClusterObjectFieldDescriptor(Label="optOutState", Tag=0x00000007, Type=typing.Optional[DeviceEnergyManagement.Enums.OptOutStateEnum]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
 
-    expressedState: 'SmokeCoAlarm.Enums.ExpressedStateEnum' = None
-    smokeState: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
-    COState: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
-    batteryAlert: 'SmokeCoAlarm.Enums.AlarmStateEnum' = None
-    deviceMuted: 'typing.Optional[SmokeCoAlarm.Enums.MuteStateEnum]' = None
-    testInProgress: 'bool' = None
-    hardwareFaultAlert: 'bool' = None
-    endOfServiceAlert: 'SmokeCoAlarm.Enums.EndOfServiceEnum' = None
-    interconnectSmokeAlarm: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
-    interconnectCOAlarm: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
-    contaminationState: 'typing.Optional[SmokeCoAlarm.Enums.ContaminationStateEnum]' = None
-    smokeSensitivityLevel: 'typing.Optional[SmokeCoAlarm.Enums.SensitivityEnum]' = None
-    expiryDate: 'typing.Optional[uint]' = None
+    ESAType: 'DeviceEnergyManagement.Enums.ESATypeEnum' = None
+    ESACanGenerate: 'bool' = None
+    ESAState: 'DeviceEnergyManagement.Enums.ESAStateEnum' = None
+    absMinPower: 'int' = None
+    absMaxPower: 'int' = None
+    powerAdjustmentCapability: 'typing.Union[None, Nullable, typing.List[DeviceEnergyManagement.Structs.PowerAdjustStruct]]' = None
+    forecast: 'typing.Union[None, Nullable, DeviceEnergyManagement.Structs.ForecastStruct]' = None
+    optOutState: 'typing.Optional[DeviceEnergyManagement.Enums.OptOutStateEnum]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class AlarmStateEnum(MatterIntEnum):
-            kNormal = 0x00
-            kWarning = 0x01
-            kCritical = 0x02
+        class AdjustmentCauseEnum(MatterIntEnum):
+            kLocalOptimization = 0x00
+            kGridOptimization = 0x01
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 3,
+            kUnknownEnumValue = 2,
 
-        class ContaminationStateEnum(MatterIntEnum):
-            kNormal = 0x00
-            kLow = 0x01
-            kWarning = 0x02
-            kCritical = 0x03
+        class CauseEnum(MatterIntEnum):
+            kNormalCompletion = 0x00
+            kOffline = 0x01
+            kFault = 0x02
+            kUserOptOut = 0x03
+            kCancelled = 0x04
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 4,
+            kUnknownEnumValue = 5,
 
-        class EndOfServiceEnum(MatterIntEnum):
-            kNormal = 0x00
-            kExpired = 0x01
+        class CostTypeEnum(MatterIntEnum):
+            kFinancial = 0x00
+            kGHGEmissions = 0x01
+            kComfort = 0x02
+            kTemperature = 0x03
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 2,
+            kUnknownEnumValue = 4,
 
-        class ExpressedStateEnum(MatterIntEnum):
-            kNormal = 0x00
-            kSmokeAlarm = 0x01
-            kCOAlarm = 0x02
-            kBatteryAlert = 0x03
-            kTesting = 0x04
-            kHardwareFault = 0x05
-            kEndOfService = 0x06
-            kInterconnectSmoke = 0x07
-            kInterconnectCO = 0x08
+        class ESAStateEnum(MatterIntEnum):
+            kOffline = 0x00
+            kOnline = 0x01
+            kFault = 0x02
+            kPowerAdjustActive = 0x03
+            kPaused = 0x04
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 9,
+            kUnknownEnumValue = 5,
 
-        class MuteStateEnum(MatterIntEnum):
-            kNotMuted = 0x00
-            kMuted = 0x01
+        class ESATypeEnum(MatterIntEnum):
+            kEvse = 0x00
+            kSpaceHeating = 0x01
+            kWaterHeating = 0x02
+            kSpaceCooling = 0x03
+            kSpaceHeatingCooling = 0x04
+            kBatteryStorage = 0x05
+            kSolarPV = 0x06
+            kFridgeFreezer = 0x07
+            kWashingMachine = 0x08
+            kDishwasher = 0x09
+            kCooking = 0x0A
+            kHomeWaterPump = 0x0B
+            kIrrigationWaterPump = 0x0C
+            kPoolPump = 0x0D
+            kOther = 0xFF
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 2,
+            kUnknownEnumValue = 14,
 
-        class SensitivityEnum(MatterIntEnum):
-            kHigh = 0x00
-            kStandard = 0x01
-            kLow = 0x02
+        class ForecastUpdateReasonEnum(MatterIntEnum):
+            kInternalOptimization = 0x00
+            kLocalOptimization = 0x01
+            kGridOptimization = 0x02
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 3,
 
+        class OptOutStateEnum(MatterIntEnum):
+            kNoOptOut = 0x00
+            kLocalOptOut = 0x01
+            kGridOptOut = 0x02
+            kOptOut = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
+
     class Bitmaps:
         class Feature(IntFlag):
-            kSmokeAlarm = 0x1
-            kCoAlarm = 0x2
+            kPowerAdjustment = 0x1
+            kPowerForecastReporting = 0x2
+            kStateForecastReporting = 0x4
+            kStartTimeAdjustment = 0x8
+            kPausable = 0x10
+            kForecastAdjustment = 0x20
+            kConstraintBasedAdjustment = 0x40
 
-    class Commands:
+    class Structs:
         @dataclass
-        class SelfTestRequest(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x0000005C
-            command_id: typing.ClassVar[int] = 0x00000000
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = None
-
+        class CostStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="costType", Tag=0, Type=DeviceEnergyManagement.Enums.CostTypeEnum),
+                        ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=int),
+                        ClusterObjectFieldDescriptor(Label="decimalPoints", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="currency", Tag=3, Type=typing.Optional[uint]),
                     ])
 
-    class Attributes:
+            costType: 'DeviceEnergyManagement.Enums.CostTypeEnum' = 0
+            value: 'int' = 0
+            decimalPoints: 'uint' = 0
+            currency: 'typing.Optional[uint]' = None
+
         @dataclass
-        class ExpressedState(ClusterAttributeDescriptor):
+        class SlotStruct(ClusterObject):
             @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="minDuration", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="maxDuration", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="defaultDuration", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="elapsedSlotTime", Tag=3, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="remainingSlotTime", Tag=4, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="slotIsPauseable", Tag=5, Type=typing.Optional[bool]),
+                        ClusterObjectFieldDescriptor(Label="minPauseDuration", Tag=6, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="maxPauseDuration", Tag=7, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="manufacturerESAState", Tag=8, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="nominalPower", Tag=9, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="minPower", Tag=10, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="maxPower", Tag=11, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="nominalEnergy", Tag=12, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="costs", Tag=13, Type=typing.Optional[typing.List[DeviceEnergyManagement.Structs.CostStruct]]),
+                        ClusterObjectFieldDescriptor(Label="minPowerAdjustment", Tag=14, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="maxPowerAdjustment", Tag=15, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="minDurationAdjustment", Tag=16, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="maxDurationAdjustment", Tag=17, Type=typing.Optional[uint]),
+                    ])
+
+            minDuration: 'uint' = 0
+            maxDuration: 'uint' = 0
+            defaultDuration: 'uint' = 0
+            elapsedSlotTime: 'uint' = 0
+            remainingSlotTime: 'uint' = 0
+            slotIsPauseable: 'typing.Optional[bool]' = None
+            minPauseDuration: 'typing.Optional[uint]' = None
+            maxPauseDuration: 'typing.Optional[uint]' = None
+            manufacturerESAState: 'typing.Optional[uint]' = None
+            nominalPower: 'typing.Optional[int]' = None
+            minPower: 'typing.Optional[int]' = None
+            maxPower: 'typing.Optional[int]' = None
+            nominalEnergy: 'typing.Optional[int]' = None
+            costs: 'typing.Optional[typing.List[DeviceEnergyManagement.Structs.CostStruct]]' = None
+            minPowerAdjustment: 'typing.Optional[int]' = None
+            maxPowerAdjustment: 'typing.Optional[int]' = None
+            minDurationAdjustment: 'typing.Optional[uint]' = None
+            maxDurationAdjustment: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class ForecastStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="forecastId", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="activeSlotNumber", Tag=1, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="startTime", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="endTime", Tag=3, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="earliestStartTime", Tag=4, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="latestEndTime", Tag=5, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="isPauseable", Tag=6, Type=bool),
+                        ClusterObjectFieldDescriptor(Label="slots", Tag=7, Type=typing.List[DeviceEnergyManagement.Structs.SlotStruct]),
+                        ClusterObjectFieldDescriptor(Label="forecastUpdateReason", Tag=8, Type=DeviceEnergyManagement.Enums.ForecastUpdateReasonEnum),
+                    ])
 
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000000
+            forecastId: 'uint' = 0
+            activeSlotNumber: 'typing.Union[Nullable, uint]' = NullValue
+            startTime: 'uint' = 0
+            endTime: 'uint' = 0
+            earliestStartTime: 'typing.Union[None, Nullable, uint]' = None
+            latestEndTime: 'typing.Optional[uint]' = None
+            isPauseable: 'bool' = False
+            slots: 'typing.List[DeviceEnergyManagement.Structs.SlotStruct]' = field(default_factory=lambda: [])
+            forecastUpdateReason: 'DeviceEnergyManagement.Enums.ForecastUpdateReasonEnum' = 0
 
+        @dataclass
+        class ConstraintsStruct(ClusterObject):
             @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=SmokeCoAlarm.Enums.ExpressedStateEnum)
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="startTime", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="duration", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="nominalPower", Tag=2, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="maximumEnergy", Tag=3, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="loadControl", Tag=4, Type=typing.Optional[int]),
+                    ])
 
-            value: 'SmokeCoAlarm.Enums.ExpressedStateEnum' = 0
+            startTime: 'uint' = 0
+            duration: 'uint' = 0
+            nominalPower: 'typing.Optional[int]' = None
+            maximumEnergy: 'typing.Optional[int]' = None
+            loadControl: 'typing.Optional[int]' = None
 
         @dataclass
-        class SmokeState(ClusterAttributeDescriptor):
+        class PowerAdjustStruct(ClusterObject):
             @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="minPower", Tag=0, Type=int),
+                        ClusterObjectFieldDescriptor(Label="maxPower", Tag=1, Type=int),
+                        ClusterObjectFieldDescriptor(Label="minDuration", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="maxDuration", Tag=3, Type=uint),
+                    ])
 
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000001
+            minPower: 'int' = 0
+            maxPower: 'int' = 0
+            minDuration: 'uint' = 0
+            maxDuration: 'uint' = 0
 
+        @dataclass
+        class SlotAdjustmentStruct(ClusterObject):
             @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum])
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="slotIndex", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="nominalPower", Tag=1, Type=int),
+                        ClusterObjectFieldDescriptor(Label="duration", Tag=2, Type=uint),
+                    ])
 
-            value: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+            slotIndex: 'uint' = 0
+            nominalPower: 'int' = 0
+            duration: 'uint' = 0
 
+    class Commands:
         @dataclass
-        class COState(ClusterAttributeDescriptor):
+        class PowerAdjustRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000098
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
             @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="power", Tag=0, Type=int),
+                        ClusterObjectFieldDescriptor(Label="duration", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="cause", Tag=2, Type=DeviceEnergyManagement.Enums.AdjustmentCauseEnum),
+                    ])
+
+            power: 'int' = 0
+            duration: 'uint' = 0
+            cause: 'DeviceEnergyManagement.Enums.AdjustmentCauseEnum' = 0
+
+        @dataclass
+        class CancelPowerAdjustRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000098
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000002
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class StartTimeAdjustRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000098
+            command_id: typing.ClassVar[int] = 0x00000002
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum])
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="requestedStartTime", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="cause", Tag=1, Type=DeviceEnergyManagement.Enums.AdjustmentCauseEnum),
+                    ])
 
-            value: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+            requestedStartTime: 'uint' = 0
+            cause: 'DeviceEnergyManagement.Enums.AdjustmentCauseEnum' = 0
 
         @dataclass
-        class BatteryAlert(ClusterAttributeDescriptor):
+        class PauseRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000098
+            command_id: typing.ClassVar[int] = 0x00000003
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
             @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="duration", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="cause", Tag=1, Type=DeviceEnergyManagement.Enums.AdjustmentCauseEnum),
+                    ])
+
+            duration: 'uint' = 0
+            cause: 'DeviceEnergyManagement.Enums.AdjustmentCauseEnum' = 0
+
+        @dataclass
+        class ResumeRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000098
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000003
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class ModifyForecastRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000098
+            command_id: typing.ClassVar[int] = 0x00000005
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=SmokeCoAlarm.Enums.AlarmStateEnum)
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="forecastId", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="slotAdjustments", Tag=1, Type=typing.List[DeviceEnergyManagement.Structs.SlotAdjustmentStruct]),
+                        ClusterObjectFieldDescriptor(Label="cause", Tag=2, Type=DeviceEnergyManagement.Enums.AdjustmentCauseEnum),
+                    ])
 
-            value: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
+            forecastId: 'uint' = 0
+            slotAdjustments: 'typing.List[DeviceEnergyManagement.Structs.SlotAdjustmentStruct]' = field(default_factory=lambda: [])
+            cause: 'DeviceEnergyManagement.Enums.AdjustmentCauseEnum' = 0
 
         @dataclass
-        class DeviceMuted(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+        class RequestConstraintBasedForecast(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000098
+            command_id: typing.ClassVar[int] = 0x00000006
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000004
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="constraints", Tag=0, Type=typing.List[DeviceEnergyManagement.Structs.ConstraintsStruct]),
+                        ClusterObjectFieldDescriptor(Label="cause", Tag=1, Type=DeviceEnergyManagement.Enums.AdjustmentCauseEnum),
+                    ])
 
-            @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.MuteStateEnum])
+            constraints: 'typing.List[DeviceEnergyManagement.Structs.ConstraintsStruct]' = field(default_factory=lambda: [])
+            cause: 'DeviceEnergyManagement.Enums.AdjustmentCauseEnum' = 0
 
-            value: 'typing.Optional[SmokeCoAlarm.Enums.MuteStateEnum]' = None
+        @dataclass
+        class CancelRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000098
+            command_id: typing.ClassVar[int] = 0x00000007
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
 
+    class Attributes:
         @dataclass
-        class TestInProgress(ClusterAttributeDescriptor):
+        class ESAType(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000005
+                return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=bool)
+                return ClusterObjectFieldDescriptor(Type=DeviceEnergyManagement.Enums.ESATypeEnum)
 
-            value: 'bool' = False
+            value: 'DeviceEnergyManagement.Enums.ESATypeEnum' = 0
 
         @dataclass
-        class HardwareFaultAlert(ClusterAttributeDescriptor):
+        class ESACanGenerate(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000006
+                return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=bool)
 
             value: 'bool' = False
 
         @dataclass
-        class EndOfServiceAlert(ClusterAttributeDescriptor):
+        class ESAState(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000007
+                return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=SmokeCoAlarm.Enums.EndOfServiceEnum)
+                return ClusterObjectFieldDescriptor(Type=DeviceEnergyManagement.Enums.ESAStateEnum)
 
-            value: 'SmokeCoAlarm.Enums.EndOfServiceEnum' = 0
+            value: 'DeviceEnergyManagement.Enums.ESAStateEnum' = 0
 
         @dataclass
-        class InterconnectSmokeAlarm(ClusterAttributeDescriptor):
+        class AbsMinPower(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000008
+                return 0x00000003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum])
+                return ClusterObjectFieldDescriptor(Type=int)
 
-            value: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+            value: 'int' = 0
 
         @dataclass
-        class InterconnectCOAlarm(ClusterAttributeDescriptor):
+        class AbsMaxPower(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000009
+                return 0x00000004
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum])
+                return ClusterObjectFieldDescriptor(Type=int)
 
-            value: 'typing.Optional[SmokeCoAlarm.Enums.AlarmStateEnum]' = None
+            value: 'int' = 0
 
         @dataclass
-        class ContaminationState(ClusterAttributeDescriptor):
+        class PowerAdjustmentCapability(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000000A
+                return 0x00000005
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.ContaminationStateEnum])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, typing.List[DeviceEnergyManagement.Structs.PowerAdjustStruct]])
 
-            value: 'typing.Optional[SmokeCoAlarm.Enums.ContaminationStateEnum]' = None
+            value: 'typing.Union[None, Nullable, typing.List[DeviceEnergyManagement.Structs.PowerAdjustStruct]]' = None
 
         @dataclass
-        class SmokeSensitivityLevel(ClusterAttributeDescriptor):
+        class Forecast(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000000B
+                return 0x00000006
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[SmokeCoAlarm.Enums.SensitivityEnum])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, DeviceEnergyManagement.Structs.ForecastStruct])
 
-            value: 'typing.Optional[SmokeCoAlarm.Enums.SensitivityEnum]' = None
+            value: 'typing.Union[None, Nullable, DeviceEnergyManagement.Structs.ForecastStruct]' = None
 
         @dataclass
-        class ExpiryDate(ClusterAttributeDescriptor):
+        class OptOutState(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000000C
+                return 0x00000007
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[DeviceEnergyManagement.Enums.OptOutStateEnum])
 
-            value: 'typing.Optional[uint]' = None
+            value: 'typing.Optional[DeviceEnergyManagement.Enums.OptOutStateEnum]' = None
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF8
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17881,15 +24682,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AcceptedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF9
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17897,15 +24698,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class EventList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFA
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17913,15 +24714,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AttributeList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFB
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17929,15 +24730,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class FeatureMap(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFC
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -17945,741 +24746,803 @@
 
             value: 'uint' = 0
 
         @dataclass
         class ClusterRevision(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFD
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
     class Events:
         @dataclass
-        class SmokeAlarm(ClusterEvent):
+        class PowerAdjustStart(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def event_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="alarmSeverityLevel", Tag=0, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
                     ])
 
-            alarmSeverityLevel: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
-
         @dataclass
-        class COAlarm(ClusterEvent):
+        class PowerAdjustEnd(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def event_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="alarmSeverityLevel", Tag=0, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
+                        ClusterObjectFieldDescriptor(Label="cause", Tag=0, Type=DeviceEnergyManagement.Enums.CauseEnum),
+                        ClusterObjectFieldDescriptor(Label="duration", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="energyUse", Tag=2, Type=int),
                     ])
 
-            alarmSeverityLevel: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
+            cause: 'DeviceEnergyManagement.Enums.CauseEnum' = 0
+            duration: 'uint' = 0
+            energyUse: 'int' = 0
 
         @dataclass
-        class LowBattery(ClusterEvent):
+        class Paused(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def event_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="alarmSeverityLevel", Tag=0, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
                     ])
 
-            alarmSeverityLevel: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
-
         @dataclass
-        class HardwareFault(ClusterEvent):
+        class Resumed(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005C
+                return 0x00000098
 
             @ChipUtility.classproperty
             def event_id(cls) -> int:
                 return 0x00000003
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="cause", Tag=0, Type=DeviceEnergyManagement.Enums.CauseEnum),
                     ])
 
-        @dataclass
-        class EndOfService(ClusterEvent):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+            cause: 'DeviceEnergyManagement.Enums.CauseEnum' = 0
 
-            @ChipUtility.classproperty
-            def event_id(cls) -> int:
-                return 0x00000004
 
+@dataclass
+class EnergyEvse(Cluster):
+    id: typing.ClassVar[int] = 0x00000099
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="state", Tag=0x00000000, Type=typing.Union[Nullable, EnergyEvse.Enums.StateEnum]),
+                ClusterObjectFieldDescriptor(Label="supplyState", Tag=0x00000001, Type=EnergyEvse.Enums.SupplyStateEnum),
+                ClusterObjectFieldDescriptor(Label="faultState", Tag=0x00000002, Type=EnergyEvse.Enums.FaultStateEnum),
+                ClusterObjectFieldDescriptor(Label="chargingEnabledUntil", Tag=0x00000003, Type=typing.Union[Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="dischargingEnabledUntil", Tag=0x00000004, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="circuitCapacity", Tag=0x00000005, Type=int),
+                ClusterObjectFieldDescriptor(Label="minimumChargeCurrent", Tag=0x00000006, Type=int),
+                ClusterObjectFieldDescriptor(Label="maximumChargeCurrent", Tag=0x00000007, Type=int),
+                ClusterObjectFieldDescriptor(Label="maximumDischargeCurrent", Tag=0x00000008, Type=typing.Optional[int]),
+                ClusterObjectFieldDescriptor(Label="userMaximumChargeCurrent", Tag=0x00000009, Type=typing.Optional[int]),
+                ClusterObjectFieldDescriptor(Label="randomizationDelayWindow", Tag=0x0000000A, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="nextChargeStartTime", Tag=0x00000023, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="nextChargeTargetTime", Tag=0x00000024, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="nextChargeRequiredEnergy", Tag=0x00000025, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="nextChargeTargetSoC", Tag=0x00000026, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="approximateEVEfficiency", Tag=0x00000027, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="stateOfCharge", Tag=0x00000030, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="batteryCapacity", Tag=0x00000031, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="vehicleID", Tag=0x00000032, Type=typing.Union[None, Nullable, str]),
+                ClusterObjectFieldDescriptor(Label="sessionID", Tag=0x00000040, Type=typing.Union[Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="sessionDuration", Tag=0x00000041, Type=typing.Union[Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="sessionEnergyCharged", Tag=0x00000042, Type=typing.Union[Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="sessionEnergyDischarged", Tag=0x00000043, Type=typing.Union[None, Nullable, int]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    state: 'typing.Union[Nullable, EnergyEvse.Enums.StateEnum]' = None
+    supplyState: 'EnergyEvse.Enums.SupplyStateEnum' = None
+    faultState: 'EnergyEvse.Enums.FaultStateEnum' = None
+    chargingEnabledUntil: 'typing.Union[Nullable, uint]' = None
+    dischargingEnabledUntil: 'typing.Union[None, Nullable, uint]' = None
+    circuitCapacity: 'int' = None
+    minimumChargeCurrent: 'int' = None
+    maximumChargeCurrent: 'int' = None
+    maximumDischargeCurrent: 'typing.Optional[int]' = None
+    userMaximumChargeCurrent: 'typing.Optional[int]' = None
+    randomizationDelayWindow: 'typing.Optional[uint]' = None
+    nextChargeStartTime: 'typing.Union[None, Nullable, uint]' = None
+    nextChargeTargetTime: 'typing.Union[None, Nullable, uint]' = None
+    nextChargeRequiredEnergy: 'typing.Union[None, Nullable, int]' = None
+    nextChargeTargetSoC: 'typing.Union[None, Nullable, uint]' = None
+    approximateEVEfficiency: 'typing.Union[None, Nullable, uint]' = None
+    stateOfCharge: 'typing.Union[None, Nullable, uint]' = None
+    batteryCapacity: 'typing.Union[None, Nullable, int]' = None
+    vehicleID: 'typing.Union[None, Nullable, str]' = None
+    sessionID: 'typing.Union[Nullable, uint]' = None
+    sessionDuration: 'typing.Union[Nullable, uint]' = None
+    sessionEnergyCharged: 'typing.Union[Nullable, int]' = None
+    sessionEnergyDischarged: 'typing.Union[None, Nullable, int]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class EnergyTransferStoppedReasonEnum(MatterIntEnum):
+            kEVStopped = 0x00
+            kEVSEStopped = 0x01
+            kOther = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 3,
+
+        class FaultStateEnum(MatterIntEnum):
+            kNoError = 0x00
+            kMeterFailure = 0x01
+            kOverVoltage = 0x02
+            kUnderVoltage = 0x03
+            kOverCurrent = 0x04
+            kContactWetFailure = 0x05
+            kContactDryFailure = 0x06
+            kGroundFault = 0x07
+            kPowerLoss = 0x08
+            kPowerQuality = 0x09
+            kPilotShortCircuit = 0x0A
+            kEmergencyStop = 0x0B
+            kEVDisconnected = 0x0C
+            kWrongPowerSupply = 0x0D
+            kLiveNeutralSwap = 0x0E
+            kOverTemperature = 0x0F
+            kOther = 0xFF
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 16,
+
+        class StateEnum(MatterIntEnum):
+            kNotPluggedIn = 0x00
+            kPluggedInNoDemand = 0x01
+            kPluggedInDemand = 0x02
+            kPluggedInCharging = 0x03
+            kPluggedInDischarging = 0x04
+            kSessionEnding = 0x05
+            kFault = 0x06
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 7,
+
+        class SupplyStateEnum(MatterIntEnum):
+            kDisabled = 0x00
+            kChargingEnabled = 0x01
+            kDischargingEnabled = 0x02
+            kDisabledError = 0x03
+            kDisabledDiagnostics = 0x04
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 5,
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kChargingPreferences = 0x1
+            kSoCReporting = 0x2
+            kPlugAndCharge = 0x4
+            kRfid = 0x8
+            kV2x = 0x10
+
+        class TargetDayOfWeekBitmap(IntFlag):
+            kSunday = 0x1
+            kMonday = 0x2
+            kTuesday = 0x4
+            kWednesday = 0x8
+            kThursday = 0x10
+            kFriday = 0x20
+            kSaturday = 0x40
+
+    class Structs:
+        @dataclass
+        class ChargingTargetStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="targetTimeMinutesPastMidnight", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="targetSoC", Tag=1, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="addedEnergy", Tag=2, Type=typing.Optional[int]),
                     ])
 
+            targetTimeMinutesPastMidnight: 'uint' = 0
+            targetSoC: 'typing.Optional[uint]' = None
+            addedEnergy: 'typing.Optional[int]' = None
+
         @dataclass
-        class SelfTestComplete(ClusterEvent):
+        class ChargingTargetScheduleStruct(ClusterObject):
             @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="dayOfWeekForSequence", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="chargingTargets", Tag=1, Type=typing.List[EnergyEvse.Structs.ChargingTargetStruct]),
+                    ])
 
-            @ChipUtility.classproperty
-            def event_id(cls) -> int:
-                return 0x00000005
+            dayOfWeekForSequence: 'uint' = 0
+            chargingTargets: 'typing.List[EnergyEvse.Structs.ChargingTargetStruct]' = field(default_factory=lambda: [])
+
+    class Commands:
+        @dataclass
+        class GetTargetsResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000099
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="chargingTargetSchedules", Tag=0, Type=typing.List[EnergyEvse.Structs.ChargingTargetScheduleStruct]),
                     ])
 
-        @dataclass
-        class AlarmMuted(ClusterEvent):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+            chargingTargetSchedules: 'typing.List[EnergyEvse.Structs.ChargingTargetScheduleStruct]' = field(default_factory=lambda: [])
 
-            @ChipUtility.classproperty
-            def event_id(cls) -> int:
-                return 0x00000006
+        @dataclass
+        class Disable(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000099
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                     ])
 
-        @dataclass
-        class MuteEnded(ClusterEvent):
             @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+            def must_use_timed_invoke(cls) -> bool:
+                return True
 
-            @ChipUtility.classproperty
-            def event_id(cls) -> int:
-                return 0x00000007
+        @dataclass
+        class EnableCharging(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000099
+            command_id: typing.ClassVar[int] = 0x00000002
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="chargingEnabledUntil", Tag=0, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="minimumChargeCurrent", Tag=1, Type=int),
+                        ClusterObjectFieldDescriptor(Label="maximumChargeCurrent", Tag=2, Type=int),
                     ])
 
-        @dataclass
-        class InterconnectSmokeAlarm(ClusterEvent):
             @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+            def must_use_timed_invoke(cls) -> bool:
+                return True
 
-            @ChipUtility.classproperty
-            def event_id(cls) -> int:
-                return 0x00000008
+            chargingEnabledUntil: 'typing.Union[Nullable, uint]' = NullValue
+            minimumChargeCurrent: 'int' = 0
+            maximumChargeCurrent: 'int' = 0
+
+        @dataclass
+        class EnableDischarging(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000099
+            command_id: typing.ClassVar[int] = 0x00000003
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="alarmSeverityLevel", Tag=0, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
+                        ClusterObjectFieldDescriptor(Label="dischargingEnabledUntil", Tag=0, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="maximumDischargeCurrent", Tag=1, Type=int),
                     ])
 
-            alarmSeverityLevel: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
-
-        @dataclass
-        class InterconnectCOAlarm(ClusterEvent):
             @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+            def must_use_timed_invoke(cls) -> bool:
+                return True
 
-            @ChipUtility.classproperty
-            def event_id(cls) -> int:
-                return 0x00000009
+            dischargingEnabledUntil: 'typing.Union[Nullable, uint]' = NullValue
+            maximumDischargeCurrent: 'int' = 0
+
+        @dataclass
+        class StartDiagnostics(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000099
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="alarmSeverityLevel", Tag=0, Type=SmokeCoAlarm.Enums.AlarmStateEnum),
                     ])
 
-            alarmSeverityLevel: 'SmokeCoAlarm.Enums.AlarmStateEnum' = 0
-
-        @dataclass
-        class AllClear(ClusterEvent):
             @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x0000005C
+            def must_use_timed_invoke(cls) -> bool:
+                return True
 
-            @ChipUtility.classproperty
-            def event_id(cls) -> int:
-                return 0x0000000A
+        @dataclass
+        class SetTargets(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000099
+            command_id: typing.ClassVar[int] = 0x00000005
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="chargingTargetSchedules", Tag=0, Type=typing.List[EnergyEvse.Structs.ChargingTargetScheduleStruct]),
                     ])
 
+            @ChipUtility.classproperty
+            def must_use_timed_invoke(cls) -> bool:
+                return True
 
-@dataclass
-class DishwasherAlarm(Cluster):
-    id: typing.ClassVar[int] = 0x0000005D
-
-    @ChipUtility.classproperty
-    def descriptor(cls) -> ClusterObjectDescriptor:
-        return ClusterObjectDescriptor(
-            Fields=[
-                ClusterObjectFieldDescriptor(Label="mask", Tag=0x00000000, Type=uint),
-                ClusterObjectFieldDescriptor(Label="latch", Tag=0x00000001, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="state", Tag=0x00000002, Type=uint),
-                ClusterObjectFieldDescriptor(Label="supported", Tag=0x00000003, Type=uint),
-                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
-                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
-            ])
-
-    mask: 'uint' = None
-    latch: 'typing.Optional[uint]' = None
-    state: 'uint' = None
-    supported: 'uint' = None
-    generatedCommandList: 'typing.List[uint]' = None
-    acceptedCommandList: 'typing.List[uint]' = None
-    eventList: 'typing.List[uint]' = None
-    attributeList: 'typing.List[uint]' = None
-    featureMap: 'uint' = None
-    clusterRevision: 'uint' = None
-
-    class Bitmaps:
-        class AlarmMap(IntFlag):
-            kInflowError = 0x1
-            kDrainError = 0x2
-            kDoorError = 0x4
-            kTempTooLow = 0x8
-            kTempTooHigh = 0x10
-            kWaterLevelError = 0x20
-
-        class Feature(IntFlag):
-            kReset = 0x1
+            chargingTargetSchedules: 'typing.List[EnergyEvse.Structs.ChargingTargetScheduleStruct]' = field(default_factory=lambda: [])
 
-    class Commands:
         @dataclass
-        class Reset(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x0000005D
-            command_id: typing.ClassVar[int] = 0x00000000
+        class GetTargets(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000099
+            command_id: typing.ClassVar[int] = 0x00000006
             is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = None
+            response_type: typing.ClassVar[str] = 'GetTargetsResponse'
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="alarms", Tag=0, Type=uint),
                     ])
 
-            alarms: 'uint' = 0
+            @ChipUtility.classproperty
+            def must_use_timed_invoke(cls) -> bool:
+                return True
 
         @dataclass
-        class ModifyEnabledAlarms(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x0000005D
-            command_id: typing.ClassVar[int] = 0x00000001
+        class ClearTargets(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000099
+            command_id: typing.ClassVar[int] = 0x00000007
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="mask", Tag=0, Type=uint),
                     ])
 
-            mask: 'uint' = 0
+            @ChipUtility.classproperty
+            def must_use_timed_invoke(cls) -> bool:
+                return True
 
     class Attributes:
         @dataclass
-        class Mask(ClusterAttributeDescriptor):
+        class State(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005D
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, EnergyEvse.Enums.StateEnum])
 
-            value: 'uint' = 0
+            value: 'typing.Union[Nullable, EnergyEvse.Enums.StateEnum]' = NullValue
 
         @dataclass
-        class Latch(ClusterAttributeDescriptor):
+        class SupplyState(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005D
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=EnergyEvse.Enums.SupplyStateEnum)
 
-            value: 'typing.Optional[uint]' = None
+            value: 'EnergyEvse.Enums.SupplyStateEnum' = 0
 
         @dataclass
-        class State(ClusterAttributeDescriptor):
+        class FaultState(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005D
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=EnergyEvse.Enums.FaultStateEnum)
 
-            value: 'uint' = 0
+            value: 'EnergyEvse.Enums.FaultStateEnum' = 0
 
         @dataclass
-        class Supported(ClusterAttributeDescriptor):
+        class ChargingEnabledUntil(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005D
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'uint' = 0
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
-        class GeneratedCommandList(ClusterAttributeDescriptor):
+        class DischargingEnabledUntil(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005D
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFF8
+                return 0x00000004
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
 
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+            value: 'typing.Union[None, Nullable, uint]' = None
 
         @dataclass
-        class AcceptedCommandList(ClusterAttributeDescriptor):
+        class CircuitCapacity(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005D
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFF9
+                return 0x00000005
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+                return ClusterObjectFieldDescriptor(Type=int)
 
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+            value: 'int' = 0
 
         @dataclass
-        class EventList(ClusterAttributeDescriptor):
+        class MinimumChargeCurrent(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005D
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFFA
+                return 0x00000006
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+                return ClusterObjectFieldDescriptor(Type=int)
 
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+            value: 'int' = 0
 
         @dataclass
-        class AttributeList(ClusterAttributeDescriptor):
+        class MaximumChargeCurrent(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005D
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFFB
+                return 0x00000007
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+                return ClusterObjectFieldDescriptor(Type=int)
 
-            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+            value: 'int' = 0
 
         @dataclass
-        class FeatureMap(ClusterAttributeDescriptor):
+        class MaximumDischargeCurrent(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005D
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFFC
+                return 0x00000008
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[int])
 
-            value: 'uint' = 0
+            value: 'typing.Optional[int]' = None
 
         @dataclass
-        class ClusterRevision(ClusterAttributeDescriptor):
+        class UserMaximumChargeCurrent(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005D
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x0000FFFD
+                return 0x00000009
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[int])
 
-            value: 'uint' = 0
+            value: 'typing.Optional[int]' = None
 
-    class Events:
         @dataclass
-        class Notify(ClusterEvent):
+        class RandomizationDelayWindow(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x0000005D
+                return 0x00000099
 
             @ChipUtility.classproperty
-            def event_id(cls) -> int:
-                return 0x00000000
+            def attribute_id(cls) -> int:
+                return 0x0000000A
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="active", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="inactive", Tag=1, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="state", Tag=2, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="mask", Tag=3, Type=uint),
-                    ])
-
-            active: 'uint' = 0
-            inactive: 'uint' = 0
-            state: 'uint' = 0
-            mask: 'uint' = 0
-
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
 
-@dataclass
-class OperationalState(Cluster):
-    id: typing.ClassVar[int] = 0x00000060
+            value: 'typing.Optional[uint]' = None
 
-    @ChipUtility.classproperty
-    def descriptor(cls) -> ClusterObjectDescriptor:
-        return ClusterObjectDescriptor(
-            Fields=[
-                ClusterObjectFieldDescriptor(Label="phaseList", Tag=0x00000000, Type=typing.Union[Nullable, typing.List[str]]),
-                ClusterObjectFieldDescriptor(Label="currentPhase", Tag=0x00000001, Type=typing.Union[Nullable, uint]),
-                ClusterObjectFieldDescriptor(Label="countdownTime", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
-                ClusterObjectFieldDescriptor(Label="operationalStateList", Tag=0x00000003, Type=typing.List[OperationalState.Structs.OperationalStateStruct]),
-                ClusterObjectFieldDescriptor(Label="operationalState", Tag=0x00000004, Type=OperationalState.Enums.OperationalStateEnum),
-                ClusterObjectFieldDescriptor(Label="operationalError", Tag=0x00000005, Type=OperationalState.Structs.ErrorStateStruct),
-                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
-                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
-                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
-            ])
+        @dataclass
+        class NextChargeStartTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000099
 
-    phaseList: 'typing.Union[Nullable, typing.List[str]]' = None
-    currentPhase: 'typing.Union[Nullable, uint]' = None
-    countdownTime: 'typing.Union[None, Nullable, uint]' = None
-    operationalStateList: 'typing.List[OperationalState.Structs.OperationalStateStruct]' = None
-    operationalState: 'OperationalState.Enums.OperationalStateEnum' = None
-    operationalError: 'OperationalState.Structs.ErrorStateStruct' = None
-    generatedCommandList: 'typing.List[uint]' = None
-    acceptedCommandList: 'typing.List[uint]' = None
-    eventList: 'typing.List[uint]' = None
-    attributeList: 'typing.List[uint]' = None
-    featureMap: 'uint' = None
-    clusterRevision: 'uint' = None
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000023
 
-    class Enums:
-        class ErrorStateEnum(MatterIntEnum):
-            kNoError = 0x00
-            kUnableToStartOrResume = 0x01
-            kUnableToCompleteOperation = 0x02
-            kCommandInvalidInState = 0x03
-            # All received enum values that are not listed above will be mapped
-            # to kUnknownEnumValue. This is a helper enum value that should only
-            # be used by code to process how it handles receiving and unknown
-            # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 4,
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
 
-        class OperationalStateEnum(MatterIntEnum):
-            kStopped = 0x00
-            kRunning = 0x01
-            kPaused = 0x02
-            kError = 0x03
-            # All received enum values that are not listed above will be mapped
-            # to kUnknownEnumValue. This is a helper enum value that should only
-            # be used by code to process how it handles receiving and unknown
-            # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 4,
+            value: 'typing.Union[None, Nullable, uint]' = None
 
-    class Structs:
         @dataclass
-        class ErrorStateStruct(ClusterObject):
+        class NextChargeTargetTime(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="errorStateID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="errorStateLabel", Tag=1, Type=typing.Optional[str]),
-                        ClusterObjectFieldDescriptor(Label="errorStateDetails", Tag=2, Type=typing.Optional[str]),
-                    ])
+            def cluster_id(cls) -> int:
+                return 0x00000099
 
-            errorStateID: 'uint' = 0
-            errorStateLabel: 'typing.Optional[str]' = None
-            errorStateDetails: 'typing.Optional[str]' = None
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000024
 
-        @dataclass
-        class OperationalStateStruct(ClusterObject):
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="operationalStateID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="operationalStateLabel", Tag=1, Type=typing.Optional[str]),
-                    ])
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
 
-            operationalStateID: 'uint' = 0
-            operationalStateLabel: 'typing.Optional[str]' = None
+            value: 'typing.Union[None, Nullable, uint]' = None
 
-    class Commands:
         @dataclass
-        class Pause(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000060
-            command_id: typing.ClassVar[int] = 0x00000000
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
-
+        class NextChargeRequiredEnergy(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                    ])
+            def cluster_id(cls) -> int:
+                return 0x00000099
 
-        @dataclass
-        class Stop(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000060
-            command_id: typing.ClassVar[int] = 0x00000001
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000025
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                    ])
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
+
+            value: 'typing.Union[None, Nullable, int]' = None
 
         @dataclass
-        class Start(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000060
-            command_id: typing.ClassVar[int] = 0x00000002
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+        class NextChargeTargetSoC(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000099
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                    ])
+            def attribute_id(cls) -> int:
+                return 0x00000026
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
 
         @dataclass
-        class Resume(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000060
-            command_id: typing.ClassVar[int] = 0x00000003
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+        class ApproximateEVEfficiency(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000099
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                    ])
+            def attribute_id(cls) -> int:
+                return 0x00000027
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
 
         @dataclass
-        class OperationalCommandResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000060
-            command_id: typing.ClassVar[int] = 0x00000004
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
+        class StateOfCharge(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000099
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="commandResponseState", Tag=0, Type=OperationalState.Structs.ErrorStateStruct),
-                    ])
+            def attribute_id(cls) -> int:
+                return 0x00000030
 
-            commandResponseState: 'OperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: OperationalState.Structs.ErrorStateStruct())
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
 
-    class Attributes:
         @dataclass
-        class PhaseList(ClusterAttributeDescriptor):
+        class BatteryCapacity(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000000
+                return 0x00000031
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, typing.List[str]])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-            value: 'typing.Union[Nullable, typing.List[str]]' = NullValue
+            value: 'typing.Union[None, Nullable, int]' = None
 
         @dataclass
-        class CurrentPhase(ClusterAttributeDescriptor):
+        class VehicleID(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000001
+                return 0x00000032
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, str])
 
-            value: 'typing.Union[Nullable, uint]' = NullValue
+            value: 'typing.Union[None, Nullable, str]' = None
 
         @dataclass
-        class CountdownTime(ClusterAttributeDescriptor):
+        class SessionID(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000002
+                return 0x00000040
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[None, Nullable, uint]' = None
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
-        class OperationalStateList(ClusterAttributeDescriptor):
+        class SessionDuration(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000003
+                return 0x00000041
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[OperationalState.Structs.OperationalStateStruct])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.List[OperationalState.Structs.OperationalStateStruct]' = field(default_factory=lambda: [])
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
-        class OperationalState(ClusterAttributeDescriptor):
+        class SessionEnergyCharged(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000004
+                return 0x00000042
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=OperationalState.Enums.OperationalStateEnum)
+                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'OperationalState.Enums.OperationalStateEnum' = 0
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
-        class OperationalError(ClusterAttributeDescriptor):
+        class SessionEnergyDischarged(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000005
+                return 0x00000043
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=OperationalState.Structs.ErrorStateStruct)
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, int])
 
-            value: 'OperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: OperationalState.Structs.ErrorStateStruct())
+            value: 'typing.Union[None, Nullable, int]' = None
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF8
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -18687,15 +25550,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AcceptedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF9
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -18703,15 +25566,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class EventList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFA
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -18719,15 +25582,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AttributeList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFB
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -18735,15 +25598,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class FeatureMap(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFC
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -18751,331 +25614,480 @@
 
             value: 'uint' = 0
 
         @dataclass
         class ClusterRevision(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFD
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
     class Events:
         @dataclass
-        class OperationalError(ClusterEvent):
+        class EVConnected(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def event_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="errorState", Tag=0, Type=OperationalState.Structs.ErrorStateStruct),
+                        ClusterObjectFieldDescriptor(Label="sessionID", Tag=0, Type=uint),
                     ])
 
-            errorState: 'OperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: OperationalState.Structs.ErrorStateStruct())
+            sessionID: 'uint' = 0
 
         @dataclass
-        class OperationCompletion(ClusterEvent):
+        class EVNotDetected(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000060
+                return 0x00000099
 
             @ChipUtility.classproperty
             def event_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="completionErrorCode", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="totalOperationalTime", Tag=1, Type=typing.Union[None, Nullable, uint]),
-                        ClusterObjectFieldDescriptor(Label="pausedTime", Tag=2, Type=typing.Union[None, Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="sessionID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="state", Tag=1, Type=EnergyEvse.Enums.StateEnum),
+                        ClusterObjectFieldDescriptor(Label="sessionDuration", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sessionEnergyCharged", Tag=3, Type=int),
+                        ClusterObjectFieldDescriptor(Label="sessionEnergyDischarged", Tag=4, Type=typing.Optional[int]),
                     ])
 
-            completionErrorCode: 'uint' = 0
-            totalOperationalTime: 'typing.Union[None, Nullable, uint]' = None
-            pausedTime: 'typing.Union[None, Nullable, uint]' = None
+            sessionID: 'uint' = 0
+            state: 'EnergyEvse.Enums.StateEnum' = 0
+            sessionDuration: 'uint' = 0
+            sessionEnergyCharged: 'int' = 0
+            sessionEnergyDischarged: 'typing.Optional[int]' = None
+
+        @dataclass
+        class EnergyTransferStarted(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000099
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="sessionID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="state", Tag=1, Type=EnergyEvse.Enums.StateEnum),
+                        ClusterObjectFieldDescriptor(Label="maximumCurrent", Tag=2, Type=int),
+                    ])
+
+            sessionID: 'uint' = 0
+            state: 'EnergyEvse.Enums.StateEnum' = 0
+            maximumCurrent: 'int' = 0
+
+        @dataclass
+        class EnergyTransferStopped(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000099
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="sessionID", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="state", Tag=1, Type=EnergyEvse.Enums.StateEnum),
+                        ClusterObjectFieldDescriptor(Label="reason", Tag=2, Type=EnergyEvse.Enums.EnergyTransferStoppedReasonEnum),
+                        ClusterObjectFieldDescriptor(Label="energyTransferred", Tag=4, Type=int),
+                    ])
+
+            sessionID: 'uint' = 0
+            state: 'EnergyEvse.Enums.StateEnum' = 0
+            reason: 'EnergyEvse.Enums.EnergyTransferStoppedReasonEnum' = 0
+            energyTransferred: 'int' = 0
+
+        @dataclass
+        class Fault(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000099
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="sessionID", Tag=0, Type=typing.Union[Nullable, uint]),
+                        ClusterObjectFieldDescriptor(Label="state", Tag=1, Type=EnergyEvse.Enums.StateEnum),
+                        ClusterObjectFieldDescriptor(Label="faultStatePreviousState", Tag=2, Type=EnergyEvse.Enums.FaultStateEnum),
+                        ClusterObjectFieldDescriptor(Label="faultStateCurrentState", Tag=4, Type=EnergyEvse.Enums.FaultStateEnum),
+                    ])
+
+            sessionID: 'typing.Union[Nullable, uint]' = NullValue
+            state: 'EnergyEvse.Enums.StateEnum' = 0
+            faultStatePreviousState: 'EnergyEvse.Enums.FaultStateEnum' = 0
+            faultStateCurrentState: 'EnergyEvse.Enums.FaultStateEnum' = 0
+
+        @dataclass
+        class Rfid(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000099
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="uid", Tag=0, Type=bytes),
+                    ])
+
+            uid: 'bytes' = b""
 
 
 @dataclass
-class RvcOperationalState(Cluster):
-    id: typing.ClassVar[int] = 0x00000061
+class EnergyPreference(Cluster):
+    id: typing.ClassVar[int] = 0x0000009B
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
-                ClusterObjectFieldDescriptor(Label="phaseList", Tag=0x00000000, Type=typing.Union[Nullable, typing.List[str]]),
-                ClusterObjectFieldDescriptor(Label="currentPhase", Tag=0x00000001, Type=typing.Union[Nullable, uint]),
-                ClusterObjectFieldDescriptor(Label="countdownTime", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
-                ClusterObjectFieldDescriptor(Label="operationalStateList", Tag=0x00000003, Type=typing.List[RvcOperationalState.Structs.OperationalStateStruct]),
-                ClusterObjectFieldDescriptor(Label="operationalState", Tag=0x00000004, Type=uint),
-                ClusterObjectFieldDescriptor(Label="operationalError", Tag=0x00000005, Type=RvcOperationalState.Structs.ErrorStateStruct),
+                ClusterObjectFieldDescriptor(Label="energyBalances", Tag=0x00000000, Type=typing.Optional[typing.List[EnergyPreference.Structs.BalanceStruct]]),
+                ClusterObjectFieldDescriptor(Label="currentEnergyBalance", Tag=0x00000001, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="energyPriorities", Tag=0x00000002, Type=typing.Optional[typing.List[EnergyPreference.Enums.EnergyPriorityEnum]]),
+                ClusterObjectFieldDescriptor(Label="lowPowerModeSensitivities", Tag=0x00000003, Type=typing.Optional[typing.List[EnergyPreference.Structs.BalanceStruct]]),
+                ClusterObjectFieldDescriptor(Label="currentLowPowerModeSensitivity", Tag=0x00000004, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
 
-    phaseList: 'typing.Union[Nullable, typing.List[str]]' = None
-    currentPhase: 'typing.Union[Nullable, uint]' = None
-    countdownTime: 'typing.Union[None, Nullable, uint]' = None
-    operationalStateList: 'typing.List[RvcOperationalState.Structs.OperationalStateStruct]' = None
-    operationalState: 'uint' = None
-    operationalError: 'RvcOperationalState.Structs.ErrorStateStruct' = None
+    energyBalances: 'typing.Optional[typing.List[EnergyPreference.Structs.BalanceStruct]]' = None
+    currentEnergyBalance: 'typing.Optional[uint]' = None
+    energyPriorities: 'typing.Optional[typing.List[EnergyPreference.Enums.EnergyPriorityEnum]]' = None
+    lowPowerModeSensitivities: 'typing.Optional[typing.List[EnergyPreference.Structs.BalanceStruct]]' = None
+    currentLowPowerModeSensitivity: 'typing.Optional[uint]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class ErrorStateEnum(MatterIntEnum):
-            kFailedToFindChargingDock = 0x40
-            kStuck = 0x41
-            kDustBinMissing = 0x42
-            kDustBinFull = 0x43
-            kWaterTankEmpty = 0x44
-            kWaterTankMissing = 0x45
-            kWaterTankLidOpen = 0x46
-            kMopCleaningPadMissing = 0x47
-            # kUnknownEnumValue intentionally not defined. This enum never goes
-            # through DataModel::Decode, likely because it is a part of a derived
-            # cluster. As a result having kUnknownEnumValue in this enum is error
-            # prone, and was removed. See
-            # src/app/common/templates/config-data.yaml.
+        class EnergyPriorityEnum(MatterIntEnum):
+            kComfort = 0x00
+            kSpeed = 0x01
+            kEfficiency = 0x02
+            kWaterConsumption = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
 
-        class OperationalStateEnum(MatterIntEnum):
-            kSeekingCharger = 0x40
-            kCharging = 0x41
-            kDocked = 0x42
-            # kUnknownEnumValue intentionally not defined. This enum never goes
-            # through DataModel::Decode, likely because it is a part of a derived
-            # cluster. As a result having kUnknownEnumValue in this enum is error
-            # prone, and was removed. See
-            # src/app/common/templates/config-data.yaml.
+    class Bitmaps:
+        class Feature(IntFlag):
+            kEnergyBalance = 0x1
+            kLowPowerModeSensitivity = 0x2
 
     class Structs:
         @dataclass
-        class ErrorStateStruct(ClusterObject):
+        class BalanceStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="errorStateID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="errorStateLabel", Tag=1, Type=typing.Optional[str]),
-                        ClusterObjectFieldDescriptor(Label="errorStateDetails", Tag=2, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="step", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="label", Tag=1, Type=typing.Optional[str]),
                     ])
 
-            errorStateID: 'uint' = 0
-            errorStateLabel: 'typing.Optional[str]' = None
-            errorStateDetails: 'typing.Optional[str]' = None
+            step: 'uint' = 0
+            label: 'typing.Optional[str]' = None
 
+    class Attributes:
         @dataclass
-        class OperationalStateStruct(ClusterObject):
+        class EnergyBalances(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="operationalStateID", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="operationalStateLabel", Tag=1, Type=typing.Optional[str]),
-                    ])
+            def cluster_id(cls) -> int:
+                return 0x0000009B
 
-            operationalStateID: 'uint' = 0
-            operationalStateLabel: 'typing.Optional[str]' = None
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[EnergyPreference.Structs.BalanceStruct]])
+
+            value: 'typing.Optional[typing.List[EnergyPreference.Structs.BalanceStruct]]' = None
 
-    class Commands:
         @dataclass
-        class Pause(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000061
-            command_id: typing.ClassVar[int] = 0x00000000
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+        class CurrentEnergyBalance(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000009B
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                    ])
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
 
         @dataclass
-        class Stop(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000061
-            command_id: typing.ClassVar[int] = 0x00000001
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+        class EnergyPriorities(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000009B
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                    ])
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[EnergyPreference.Enums.EnergyPriorityEnum]])
+
+            value: 'typing.Optional[typing.List[EnergyPreference.Enums.EnergyPriorityEnum]]' = None
 
         @dataclass
-        class Start(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000061
-            command_id: typing.ClassVar[int] = 0x00000002
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+        class LowPowerModeSensitivities(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000009B
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                    ])
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[EnergyPreference.Structs.BalanceStruct]])
+
+            value: 'typing.Optional[typing.List[EnergyPreference.Structs.BalanceStruct]]' = None
 
         @dataclass
-        class Resume(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000061
-            command_id: typing.ClassVar[int] = 0x00000003
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = 'OperationalCommandResponse'
+        class CurrentLowPowerModeSensitivity(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000009B
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                    ])
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
 
         @dataclass
-        class OperationalCommandResponse(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000061
-            command_id: typing.ClassVar[int] = 0x00000004
-            is_client: typing.ClassVar[bool] = False
-            response_type: typing.ClassVar[str] = None
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000009B
 
             @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="commandResponseState", Tag=0, Type=RvcOperationalState.Structs.ErrorStateStruct),
-                    ])
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
 
-            commandResponseState: 'RvcOperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: RvcOperationalState.Structs.ErrorStateStruct())
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
-    class Attributes:
         @dataclass
-        class PhaseList(ClusterAttributeDescriptor):
+        class AcceptedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009B
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000000
+                return 0x0000FFF9
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, typing.List[str]])
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
 
-            value: 'typing.Union[Nullable, typing.List[str]]' = NullValue
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
-        class CurrentPhase(ClusterAttributeDescriptor):
+        class EventList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009B
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000001
+                return 0x0000FFFA
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
 
-            value: 'typing.Union[Nullable, uint]' = NullValue
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
-        class CountdownTime(ClusterAttributeDescriptor):
+        class AttributeList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009B
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000002
+                return 0x0000FFFB
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
 
-            value: 'typing.Union[None, Nullable, uint]' = None
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
-        class OperationalStateList(ClusterAttributeDescriptor):
+        class FeatureMap(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009B
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000003
+                return 0x0000FFFC
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.List[RvcOperationalState.Structs.OperationalStateStruct])
+                return ClusterObjectFieldDescriptor(Type=uint)
 
-            value: 'typing.List[RvcOperationalState.Structs.OperationalStateStruct]' = field(default_factory=lambda: [])
+            value: 'uint' = 0
 
         @dataclass
-        class OperationalState(ClusterAttributeDescriptor):
+        class ClusterRevision(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009B
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000004
+                return 0x0000FFFD
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
+
+@dataclass
+class PowerTopology(Cluster):
+    id: typing.ClassVar[int] = 0x0000009C
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="availableEndpoints", Tag=0x00000000, Type=typing.Optional[typing.List[uint]]),
+                ClusterObjectFieldDescriptor(Label="activeEndpoints", Tag=0x00000001, Type=typing.Optional[typing.List[uint]]),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    availableEndpoints: 'typing.Optional[typing.List[uint]]' = None
+    activeEndpoints: 'typing.Optional[typing.List[uint]]' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kNodeTopology = 0x1
+            kTreeTopology = 0x2
+            kSetTopology = 0x4
+            kDynamicPowerFlow = 0x8
+
+    class Attributes:
         @dataclass
-        class OperationalError(ClusterAttributeDescriptor):
+        class AvailableEndpoints(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009C
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000005
+                return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=RvcOperationalState.Structs.ErrorStateStruct)
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[uint]])
 
-            value: 'RvcOperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: RvcOperationalState.Structs.ErrorStateStruct())
+            value: 'typing.Optional[typing.List[uint]]' = None
+
+        @dataclass
+        class ActiveEndpoints(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000009C
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[uint]])
+
+            value: 'typing.Optional[typing.List[uint]]' = None
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009C
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF8
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19083,15 +26095,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AcceptedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009C
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF9
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19099,15 +26111,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class EventList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009C
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFA
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19115,15 +26127,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AttributeList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009C
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFB
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19131,15 +26143,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class FeatureMap(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009C
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFC
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19147,273 +26159,207 @@
 
             value: 'uint' = 0
 
         @dataclass
         class ClusterRevision(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000061
+                return 0x0000009C
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFD
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
-    class Events:
-        @dataclass
-        class OperationalError(ClusterEvent):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000061
-
-            @ChipUtility.classproperty
-            def event_id(cls) -> int:
-                return 0x00000000
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="errorState", Tag=0, Type=RvcOperationalState.Structs.ErrorStateStruct),
-                    ])
-
-            errorState: 'RvcOperationalState.Structs.ErrorStateStruct' = field(default_factory=lambda: RvcOperationalState.Structs.ErrorStateStruct())
-
-        @dataclass
-        class OperationCompletion(ClusterEvent):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000061
-
-            @ChipUtility.classproperty
-            def event_id(cls) -> int:
-                return 0x00000001
-
-            @ChipUtility.classproperty
-            def descriptor(cls) -> ClusterObjectDescriptor:
-                return ClusterObjectDescriptor(
-                    Fields=[
-                        ClusterObjectFieldDescriptor(Label="completionErrorCode", Tag=0, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="totalOperationalTime", Tag=1, Type=typing.Union[None, Nullable, uint]),
-                        ClusterObjectFieldDescriptor(Label="pausedTime", Tag=2, Type=typing.Union[None, Nullable, uint]),
-                    ])
-
-            completionErrorCode: 'uint' = 0
-            totalOperationalTime: 'typing.Union[None, Nullable, uint]' = None
-            pausedTime: 'typing.Union[None, Nullable, uint]' = None
-
 
 @dataclass
-class HepaFilterMonitoring(Cluster):
-    id: typing.ClassVar[int] = 0x00000071
+class EnergyEvseMode(Cluster):
+    id: typing.ClassVar[int] = 0x0000009D
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
-                ClusterObjectFieldDescriptor(Label="condition", Tag=0x00000000, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="degradationDirection", Tag=0x00000001, Type=typing.Optional[HepaFilterMonitoring.Enums.DegradationDirectionEnum]),
-                ClusterObjectFieldDescriptor(Label="changeIndication", Tag=0x00000002, Type=HepaFilterMonitoring.Enums.ChangeIndicationEnum),
-                ClusterObjectFieldDescriptor(Label="inPlaceIndicator", Tag=0x00000003, Type=typing.Optional[bool]),
-                ClusterObjectFieldDescriptor(Label="lastChangedTime", Tag=0x00000004, Type=typing.Union[None, Nullable, uint]),
-                ClusterObjectFieldDescriptor(Label="replacementProductList", Tag=0x00000005, Type=typing.Optional[typing.List[HepaFilterMonitoring.Structs.ReplacementProductStruct]]),
+                ClusterObjectFieldDescriptor(Label="supportedModes", Tag=0x00000000, Type=typing.List[EnergyEvseMode.Structs.ModeOptionStruct]),
+                ClusterObjectFieldDescriptor(Label="currentMode", Tag=0x00000001, Type=uint),
+                ClusterObjectFieldDescriptor(Label="startUpMode", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="onMode", Tag=0x00000003, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
 
-    condition: 'typing.Optional[uint]' = None
-    degradationDirection: 'typing.Optional[HepaFilterMonitoring.Enums.DegradationDirectionEnum]' = None
-    changeIndication: 'HepaFilterMonitoring.Enums.ChangeIndicationEnum' = None
-    inPlaceIndicator: 'typing.Optional[bool]' = None
-    lastChangedTime: 'typing.Union[None, Nullable, uint]' = None
-    replacementProductList: 'typing.Optional[typing.List[HepaFilterMonitoring.Structs.ReplacementProductStruct]]' = None
+    supportedModes: 'typing.List[EnergyEvseMode.Structs.ModeOptionStruct]' = None
+    currentMode: 'uint' = None
+    startUpMode: 'typing.Union[None, Nullable, uint]' = None
+    onMode: 'typing.Union[None, Nullable, uint]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class ChangeIndicationEnum(MatterIntEnum):
-            kOk = 0x00
-            kWarning = 0x01
-            kCritical = 0x02
-            # All received enum values that are not listed above will be mapped
-            # to kUnknownEnumValue. This is a helper enum value that should only
-            # be used by code to process how it handles receiving and unknown
-            # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 3,
-
-        class DegradationDirectionEnum(MatterIntEnum):
-            kUp = 0x00
-            kDown = 0x01
-            # All received enum values that are not listed above will be mapped
-            # to kUnknownEnumValue. This is a helper enum value that should only
-            # be used by code to process how it handles receiving and unknown
-            # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 2,
-
-        class ProductIdentifierTypeEnum(MatterIntEnum):
-            kUpc = 0x00
-            kGtin8 = 0x01
-            kEan = 0x02
-            kGtin14 = 0x03
-            kOem = 0x04
-            # All received enum values that are not listed above will be mapped
-            # to kUnknownEnumValue. This is a helper enum value that should only
-            # be used by code to process how it handles receiving and unknown
-            # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 5,
+        class ModeTag(MatterIntEnum):
+            kManual = 0x4000
+            kTimeOfUse = 0x4001
+            kSolarCharging = 0x4002
+            # kUnknownEnumValue intentionally not defined. This enum never goes
+            # through DataModel::Decode, likely because it is a part of a derived
+            # cluster. As a result having kUnknownEnumValue in this enum is error
+            # prone, and was removed. See
+            # src/app/common/templates/config-data.yaml.
 
     class Bitmaps:
         class Feature(IntFlag):
-            kCondition = 0x1
-            kWarning = 0x2
-            kReplacementProductList = 0x4
+            kOnOff = 0x1
 
     class Structs:
         @dataclass
-        class ReplacementProductStruct(ClusterObject):
+        class ModeTagStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="productIdentifierType", Tag=0, Type=HepaFilterMonitoring.Enums.ProductIdentifierTypeEnum),
-                        ClusterObjectFieldDescriptor(Label="productIdentifierValue", Tag=1, Type=str),
+                        ClusterObjectFieldDescriptor(Label="mfgCode", Tag=0, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=uint),
                     ])
 
-            productIdentifierType: 'HepaFilterMonitoring.Enums.ProductIdentifierTypeEnum' = 0
-            productIdentifierValue: 'str' = ""
+            mfgCode: 'typing.Optional[uint]' = None
+            value: 'uint' = 0
 
-    class Commands:
         @dataclass
-        class ResetCondition(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000071
-            command_id: typing.ClassVar[int] = 0x00000000
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = None
-
+        class ModeOptionStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="label", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="mode", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="modeTags", Tag=2, Type=typing.List[EnergyEvseMode.Structs.ModeTagStruct]),
                     ])
 
-    class Attributes:
-        @dataclass
-        class Condition(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000071
+            label: 'str' = ""
+            mode: 'uint' = 0
+            modeTags: 'typing.List[EnergyEvseMode.Structs.ModeTagStruct]' = field(default_factory=lambda: [])
 
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000000
+    class Commands:
+        @dataclass
+        class ChangeToMode(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000009D
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'ChangeToModeResponse'
 
             @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="newMode", Tag=0, Type=uint),
+                    ])
 
-            value: 'typing.Optional[uint]' = None
+            newMode: 'uint' = 0
 
         @dataclass
-        class DegradationDirection(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000071
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000001
+        class ChangeToModeResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000009D
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[HepaFilterMonitoring.Enums.DegradationDirectionEnum])
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="statusText", Tag=1, Type=typing.Optional[str]),
+                    ])
 
-            value: 'typing.Optional[HepaFilterMonitoring.Enums.DegradationDirectionEnum]' = None
+            status: 'uint' = 0
+            statusText: 'typing.Optional[str]' = None
 
+    class Attributes:
         @dataclass
-        class ChangeIndication(ClusterAttributeDescriptor):
+        class SupportedModes(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000071
+                return 0x0000009D
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000002
+                return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=HepaFilterMonitoring.Enums.ChangeIndicationEnum)
+                return ClusterObjectFieldDescriptor(Type=typing.List[EnergyEvseMode.Structs.ModeOptionStruct])
 
-            value: 'HepaFilterMonitoring.Enums.ChangeIndicationEnum' = 0
+            value: 'typing.List[EnergyEvseMode.Structs.ModeOptionStruct]' = field(default_factory=lambda: [])
 
         @dataclass
-        class InPlaceIndicator(ClusterAttributeDescriptor):
+        class CurrentMode(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000071
+                return 0x0000009D
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000003
+                return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[bool])
+                return ClusterObjectFieldDescriptor(Type=uint)
 
-            value: 'typing.Optional[bool]' = None
+            value: 'uint' = 0
 
         @dataclass
-        class LastChangedTime(ClusterAttributeDescriptor):
+        class StartUpMode(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000071
+                return 0x0000009D
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000004
+                return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
 
             value: 'typing.Union[None, Nullable, uint]' = None
 
         @dataclass
-        class ReplacementProductList(ClusterAttributeDescriptor):
+        class OnMode(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000071
+                return 0x0000009D
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000005
+                return 0x00000003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[HepaFilterMonitoring.Structs.ReplacementProductStruct]])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
 
-            value: 'typing.Optional[typing.List[HepaFilterMonitoring.Structs.ReplacementProductStruct]]' = None
+            value: 'typing.Union[None, Nullable, uint]' = None
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000071
+                return 0x0000009D
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF8
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19421,15 +26367,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AcceptedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000071
+                return 0x0000009D
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF9
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19437,15 +26383,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class EventList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000071
+                return 0x0000009D
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFA
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19453,15 +26399,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AttributeList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000071
+                return 0x0000009D
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFB
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19469,15 +26415,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class FeatureMap(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000071
+                return 0x0000009D
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFC
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19485,230 +26431,208 @@
 
             value: 'uint' = 0
 
         @dataclass
         class ClusterRevision(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000071
+                return 0x0000009D
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFD
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
 
 @dataclass
-class ActivatedCarbonFilterMonitoring(Cluster):
-    id: typing.ClassVar[int] = 0x00000072
+class DeviceEnergyManagementMode(Cluster):
+    id: typing.ClassVar[int] = 0x0000009F
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
-                ClusterObjectFieldDescriptor(Label="condition", Tag=0x00000000, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="degradationDirection", Tag=0x00000001, Type=typing.Optional[ActivatedCarbonFilterMonitoring.Enums.DegradationDirectionEnum]),
-                ClusterObjectFieldDescriptor(Label="changeIndication", Tag=0x00000002, Type=ActivatedCarbonFilterMonitoring.Enums.ChangeIndicationEnum),
-                ClusterObjectFieldDescriptor(Label="inPlaceIndicator", Tag=0x00000003, Type=typing.Optional[bool]),
-                ClusterObjectFieldDescriptor(Label="lastChangedTime", Tag=0x00000004, Type=typing.Union[None, Nullable, uint]),
-                ClusterObjectFieldDescriptor(Label="replacementProductList", Tag=0x00000005, Type=typing.Optional[typing.List[ActivatedCarbonFilterMonitoring.Structs.ReplacementProductStruct]]),
+                ClusterObjectFieldDescriptor(Label="supportedModes", Tag=0x00000000, Type=typing.List[DeviceEnergyManagementMode.Structs.ModeOptionStruct]),
+                ClusterObjectFieldDescriptor(Label="currentMode", Tag=0x00000001, Type=uint),
+                ClusterObjectFieldDescriptor(Label="startUpMode", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="onMode", Tag=0x00000003, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
 
-    condition: 'typing.Optional[uint]' = None
-    degradationDirection: 'typing.Optional[ActivatedCarbonFilterMonitoring.Enums.DegradationDirectionEnum]' = None
-    changeIndication: 'ActivatedCarbonFilterMonitoring.Enums.ChangeIndicationEnum' = None
-    inPlaceIndicator: 'typing.Optional[bool]' = None
-    lastChangedTime: 'typing.Union[None, Nullable, uint]' = None
-    replacementProductList: 'typing.Optional[typing.List[ActivatedCarbonFilterMonitoring.Structs.ReplacementProductStruct]]' = None
+    supportedModes: 'typing.List[DeviceEnergyManagementMode.Structs.ModeOptionStruct]' = None
+    currentMode: 'uint' = None
+    startUpMode: 'typing.Union[None, Nullable, uint]' = None
+    onMode: 'typing.Union[None, Nullable, uint]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class ChangeIndicationEnum(MatterIntEnum):
-            kOk = 0x00
-            kWarning = 0x01
-            kCritical = 0x02
-            # All received enum values that are not listed above will be mapped
-            # to kUnknownEnumValue. This is a helper enum value that should only
-            # be used by code to process how it handles receiving and unknown
-            # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 3,
-
-        class DegradationDirectionEnum(MatterIntEnum):
-            kUp = 0x00
-            kDown = 0x01
-            # All received enum values that are not listed above will be mapped
-            # to kUnknownEnumValue. This is a helper enum value that should only
-            # be used by code to process how it handles receiving and unknown
-            # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 2,
-
-        class ProductIdentifierTypeEnum(MatterIntEnum):
-            kUpc = 0x00
-            kGtin8 = 0x01
-            kEan = 0x02
-            kGtin14 = 0x03
-            kOem = 0x04
-            # All received enum values that are not listed above will be mapped
-            # to kUnknownEnumValue. This is a helper enum value that should only
-            # be used by code to process how it handles receiving and unknown
-            # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 5,
+        class ModeTag(MatterIntEnum):
+            kNoOptimization = 0x4000
+            kDeviceOptimization = 0x4001
+            kLocalOptimization = 0x4002
+            kGridOptimization = 0x4003
+            # kUnknownEnumValue intentionally not defined. This enum never goes
+            # through DataModel::Decode, likely because it is a part of a derived
+            # cluster. As a result having kUnknownEnumValue in this enum is error
+            # prone, and was removed. See
+            # src/app/common/templates/config-data.yaml.
 
     class Bitmaps:
         class Feature(IntFlag):
-            kCondition = 0x1
-            kWarning = 0x2
-            kReplacementProductList = 0x4
+            kOnOff = 0x1
 
     class Structs:
         @dataclass
-        class ReplacementProductStruct(ClusterObject):
+        class ModeTagStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="productIdentifierType", Tag=0, Type=ActivatedCarbonFilterMonitoring.Enums.ProductIdentifierTypeEnum),
-                        ClusterObjectFieldDescriptor(Label="productIdentifierValue", Tag=1, Type=str),
+                        ClusterObjectFieldDescriptor(Label="mfgCode", Tag=0, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=uint),
                     ])
 
-            productIdentifierType: 'ActivatedCarbonFilterMonitoring.Enums.ProductIdentifierTypeEnum' = 0
-            productIdentifierValue: 'str' = ""
+            mfgCode: 'typing.Optional[uint]' = None
+            value: 'uint' = 0
 
-    class Commands:
         @dataclass
-        class ResetCondition(ClusterCommand):
-            cluster_id: typing.ClassVar[int] = 0x00000072
-            command_id: typing.ClassVar[int] = 0x00000000
-            is_client: typing.ClassVar[bool] = True
-            response_type: typing.ClassVar[str] = None
-
+        class ModeOptionStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="label", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="mode", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="modeTags", Tag=2, Type=typing.List[DeviceEnergyManagementMode.Structs.ModeTagStruct]),
                     ])
 
-    class Attributes:
-        @dataclass
-        class Condition(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000072
+            label: 'str' = ""
+            mode: 'uint' = 0
+            modeTags: 'typing.List[DeviceEnergyManagementMode.Structs.ModeTagStruct]' = field(default_factory=lambda: [])
 
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000000
+    class Commands:
+        @dataclass
+        class ChangeToMode(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000009F
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'ChangeToModeResponse'
 
             @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="newMode", Tag=0, Type=uint),
+                    ])
 
-            value: 'typing.Optional[uint]' = None
+            newMode: 'uint' = 0
 
         @dataclass
-        class DegradationDirection(ClusterAttributeDescriptor):
-            @ChipUtility.classproperty
-            def cluster_id(cls) -> int:
-                return 0x00000072
-
-            @ChipUtility.classproperty
-            def attribute_id(cls) -> int:
-                return 0x00000001
+        class ChangeToModeResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000009F
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
-            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[ActivatedCarbonFilterMonitoring.Enums.DegradationDirectionEnum])
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="statusText", Tag=1, Type=typing.Optional[str]),
+                    ])
 
-            value: 'typing.Optional[ActivatedCarbonFilterMonitoring.Enums.DegradationDirectionEnum]' = None
+            status: 'uint' = 0
+            statusText: 'typing.Optional[str]' = None
 
+    class Attributes:
         @dataclass
-        class ChangeIndication(ClusterAttributeDescriptor):
+        class SupportedModes(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000072
+                return 0x0000009F
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000002
+                return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=ActivatedCarbonFilterMonitoring.Enums.ChangeIndicationEnum)
+                return ClusterObjectFieldDescriptor(Type=typing.List[DeviceEnergyManagementMode.Structs.ModeOptionStruct])
 
-            value: 'ActivatedCarbonFilterMonitoring.Enums.ChangeIndicationEnum' = 0
+            value: 'typing.List[DeviceEnergyManagementMode.Structs.ModeOptionStruct]' = field(default_factory=lambda: [])
 
         @dataclass
-        class InPlaceIndicator(ClusterAttributeDescriptor):
+        class CurrentMode(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000072
+                return 0x0000009F
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000003
+                return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[bool])
+                return ClusterObjectFieldDescriptor(Type=uint)
 
-            value: 'typing.Optional[bool]' = None
+            value: 'uint' = 0
 
         @dataclass
-        class LastChangedTime(ClusterAttributeDescriptor):
+        class StartUpMode(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000072
+                return 0x0000009F
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000004
+                return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
 
             value: 'typing.Union[None, Nullable, uint]' = None
 
         @dataclass
-        class ReplacementProductList(ClusterAttributeDescriptor):
+        class OnMode(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000072
+                return 0x0000009F
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
-                return 0x00000005
+                return 0x00000003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[ActivatedCarbonFilterMonitoring.Structs.ReplacementProductStruct]])
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
 
-            value: 'typing.Optional[typing.List[ActivatedCarbonFilterMonitoring.Structs.ReplacementProductStruct]]' = None
+            value: 'typing.Union[None, Nullable, uint]' = None
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000072
+                return 0x0000009F
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF8
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19716,15 +26640,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AcceptedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000072
+                return 0x0000009F
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFF9
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19732,15 +26656,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class EventList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000072
+                return 0x0000009F
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFA
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19748,15 +26672,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class AttributeList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000072
+                return 0x0000009F
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFB
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19764,15 +26688,15 @@
 
             value: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class FeatureMap(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000072
+                return 0x0000009F
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFC
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19780,15 +26704,15 @@
 
             value: 'uint' = 0
 
         @dataclass
         class ClusterRevision(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
-                return 0x00000072
+                return 0x0000009F
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000FFFD
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
@@ -19837,14 +26761,23 @@
                 ClusterObjectFieldDescriptor(Label="enablePrivacyModeButton", Tag=0x0000002B, Type=typing.Optional[bool]),
                 ClusterObjectFieldDescriptor(Label="localProgrammingFeatures", Tag=0x0000002C, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="wrongCodeEntryLimit", Tag=0x00000030, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="userCodeTemporaryDisableTime", Tag=0x00000031, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="sendPINOverTheAir", Tag=0x00000032, Type=typing.Optional[bool]),
                 ClusterObjectFieldDescriptor(Label="requirePINforRemoteOperation", Tag=0x00000033, Type=typing.Optional[bool]),
                 ClusterObjectFieldDescriptor(Label="expiringUserTimeout", Tag=0x00000035, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="aliroReaderVerificationKey", Tag=0x00000080, Type=typing.Union[None, Nullable, bytes]),
+                ClusterObjectFieldDescriptor(Label="aliroReaderGroupIdentifier", Tag=0x00000081, Type=typing.Union[None, Nullable, bytes]),
+                ClusterObjectFieldDescriptor(Label="aliroReaderGroupSubIdentifier", Tag=0x00000082, Type=typing.Optional[bytes]),
+                ClusterObjectFieldDescriptor(Label="aliroExpeditedTransactionSupportedProtocolVersions", Tag=0x00000083, Type=typing.Optional[typing.List[bytes]]),
+                ClusterObjectFieldDescriptor(Label="aliroGroupResolvingKey", Tag=0x00000084, Type=typing.Union[None, Nullable, bytes]),
+                ClusterObjectFieldDescriptor(Label="aliroSupportedBLEUWBProtocolVersions", Tag=0x00000085, Type=typing.Optional[typing.List[bytes]]),
+                ClusterObjectFieldDescriptor(Label="aliroBLEAdvertisingVersion", Tag=0x00000086, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="numberOfAliroCredentialIssuerKeysSupported", Tag=0x00000087, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="numberOfAliroEndpointKeysSupported", Tag=0x00000088, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
@@ -19881,14 +26814,23 @@
     enablePrivacyModeButton: 'typing.Optional[bool]' = None
     localProgrammingFeatures: 'typing.Optional[uint]' = None
     wrongCodeEntryLimit: 'typing.Optional[uint]' = None
     userCodeTemporaryDisableTime: 'typing.Optional[uint]' = None
     sendPINOverTheAir: 'typing.Optional[bool]' = None
     requirePINforRemoteOperation: 'typing.Optional[bool]' = None
     expiringUserTimeout: 'typing.Optional[uint]' = None
+    aliroReaderVerificationKey: 'typing.Union[None, Nullable, bytes]' = None
+    aliroReaderGroupIdentifier: 'typing.Union[None, Nullable, bytes]' = None
+    aliroReaderGroupSubIdentifier: 'typing.Optional[bytes]' = None
+    aliroExpeditedTransactionSupportedProtocolVersions: 'typing.Optional[typing.List[bytes]]' = None
+    aliroGroupResolvingKey: 'typing.Union[None, Nullable, bytes]' = None
+    aliroSupportedBLEUWBProtocolVersions: 'typing.Optional[typing.List[bytes]]' = None
+    aliroBLEAdvertisingVersion: 'typing.Optional[uint]' = None
+    numberOfAliroCredentialIssuerKeysSupported: 'typing.Optional[uint]' = None
+    numberOfAliroEndpointKeysSupported: 'typing.Optional[uint]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
@@ -19921,19 +26863,22 @@
         class CredentialTypeEnum(MatterIntEnum):
             kProgrammingPIN = 0x00
             kPin = 0x01
             kRfid = 0x02
             kFingerprint = 0x03
             kFingerVein = 0x04
             kFace = 0x05
+            kAliroCredentialIssuerKey = 0x06
+            kAliroEvictableEndpointKey = 0x07
+            kAliroNonEvictableEndpointKey = 0x08
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 6,
+            kUnknownEnumValue = 9,
 
         class DataOperationTypeEnum(MatterIntEnum):
             kAdd = 0x00
             kClear = 0x01
             kModify = 0x02
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
@@ -20077,19 +27022,22 @@
             kYearDaySchedule = 0x04
             kHolidaySchedule = 0x05
             kPin = 0x06
             kRfid = 0x07
             kFingerprint = 0x08
             kFingerVein = 0x09
             kFace = 0x0A
+            kAliroCredentialIssuerKey = 0x0B
+            kAliroEvictableEndpointKey = 0x0C
+            kAliroNonEvictableEndpointKey = 0x0D
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 11,
+            kUnknownEnumValue = 14,
 
         class LockOperationTypeEnum(MatterIntEnum):
             kLock = 0x00
             kUnlock = 0x01
             kNonAccessUserEvent = 0x02
             kForcedUserEvent = 0x03
             kUnlatch = 0x04
@@ -20130,19 +27078,20 @@
             kKeypad = 0x03
             kAuto = 0x04
             kButton = 0x05
             kSchedule = 0x06
             kRemote = 0x07
             kRfid = 0x08
             kBiometric = 0x09
+            kAliro = 0x0A
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 10,
+            kUnknownEnumValue = 11,
 
         class UserStatusEnum(MatterIntEnum):
             kAvailable = 0x00
             kOccupiedEnabled = 0x01
             kOccupiedDisabled = 0x03
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
@@ -20289,14 +27238,16 @@
             kFaceCredentials = 0x40
             kCredentialsOverTheAirAccess = 0x80
             kUser = 0x100
             kNotification = 0x200
             kYearDayAccessSchedules = 0x400
             kHolidaySchedules = 0x800
             kUnbolt = 0x1000
+            kAliroProvisioning = 0x2000
+            kAliroBLEUWB = 0x4000
 
     class Structs:
         @dataclass
         class CredentialStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
@@ -20853,14 +27804,57 @@
 
             @ChipUtility.classproperty
             def must_use_timed_invoke(cls) -> bool:
                 return True
 
             PINCode: 'typing.Optional[bytes]' = None
 
+        @dataclass
+        class SetAliroReaderConfig(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000101
+            command_id: typing.ClassVar[int] = 0x00000028
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="signingKey", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="verificationKey", Tag=1, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="groupIdentifier", Tag=2, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="groupResolvingKey", Tag=3, Type=typing.Optional[bytes]),
+                    ])
+
+            @ChipUtility.classproperty
+            def must_use_timed_invoke(cls) -> bool:
+                return True
+
+            signingKey: 'bytes' = b""
+            verificationKey: 'bytes' = b""
+            groupIdentifier: 'bytes' = b""
+            groupResolvingKey: 'typing.Optional[bytes]' = None
+
+        @dataclass
+        class ClearAliroReaderConfig(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000101
+            command_id: typing.ClassVar[int] = 0x00000029
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+            @ChipUtility.classproperty
+            def must_use_timed_invoke(cls) -> bool:
+                return True
+
     class Attributes:
         @dataclass
         class LockState(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000101
 
@@ -21431,14 +28425,158 @@
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
 
             value: 'typing.Optional[uint]' = None
 
         @dataclass
+        class AliroReaderVerificationKey(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000101
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000080
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, bytes])
+
+            value: 'typing.Union[None, Nullable, bytes]' = None
+
+        @dataclass
+        class AliroReaderGroupIdentifier(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000101
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000081
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, bytes])
+
+            value: 'typing.Union[None, Nullable, bytes]' = None
+
+        @dataclass
+        class AliroReaderGroupSubIdentifier(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000101
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000082
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[bytes])
+
+            value: 'typing.Optional[bytes]' = None
+
+        @dataclass
+        class AliroExpeditedTransactionSupportedProtocolVersions(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000101
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000083
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[bytes]])
+
+            value: 'typing.Optional[typing.List[bytes]]' = None
+
+        @dataclass
+        class AliroGroupResolvingKey(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000101
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000084
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, bytes])
+
+            value: 'typing.Union[None, Nullable, bytes]' = None
+
+        @dataclass
+        class AliroSupportedBLEUWBProtocolVersions(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000101
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000085
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[bytes]])
+
+            value: 'typing.Optional[typing.List[bytes]]' = None
+
+        @dataclass
+        class AliroBLEAdvertisingVersion(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000101
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000086
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class NumberOfAliroCredentialIssuerKeysSupported(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000101
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000087
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class NumberOfAliroEndpointKeysSupported(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000101
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000088
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000101
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
@@ -23595,42 +30733,56 @@
                 ClusterObjectFieldDescriptor(Label="unoccupiedHeatingSetpoint", Tag=0x00000014, Type=typing.Optional[int]),
                 ClusterObjectFieldDescriptor(Label="minHeatSetpointLimit", Tag=0x00000015, Type=typing.Optional[int]),
                 ClusterObjectFieldDescriptor(Label="maxHeatSetpointLimit", Tag=0x00000016, Type=typing.Optional[int]),
                 ClusterObjectFieldDescriptor(Label="minCoolSetpointLimit", Tag=0x00000017, Type=typing.Optional[int]),
                 ClusterObjectFieldDescriptor(Label="maxCoolSetpointLimit", Tag=0x00000018, Type=typing.Optional[int]),
                 ClusterObjectFieldDescriptor(Label="minSetpointDeadBand", Tag=0x00000019, Type=typing.Optional[int]),
                 ClusterObjectFieldDescriptor(Label="remoteSensing", Tag=0x0000001A, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="controlSequenceOfOperation", Tag=0x0000001B, Type=Thermostat.Enums.ThermostatControlSequence),
-                ClusterObjectFieldDescriptor(Label="systemMode", Tag=0x0000001C, Type=uint),
-                ClusterObjectFieldDescriptor(Label="thermostatRunningMode", Tag=0x0000001E, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="startOfWeek", Tag=0x00000020, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="controlSequenceOfOperation", Tag=0x0000001B, Type=Thermostat.Enums.ControlSequenceOfOperationEnum),
+                ClusterObjectFieldDescriptor(Label="systemMode", Tag=0x0000001C, Type=Thermostat.Enums.SystemModeEnum),
+                ClusterObjectFieldDescriptor(Label="thermostatRunningMode", Tag=0x0000001E, Type=typing.Optional[Thermostat.Enums.ThermostatRunningModeEnum]),
+                ClusterObjectFieldDescriptor(Label="startOfWeek", Tag=0x00000020, Type=typing.Optional[Thermostat.Enums.StartOfWeekEnum]),
                 ClusterObjectFieldDescriptor(Label="numberOfWeeklyTransitions", Tag=0x00000021, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="numberOfDailyTransitions", Tag=0x00000022, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="temperatureSetpointHold", Tag=0x00000023, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="temperatureSetpointHold", Tag=0x00000023, Type=typing.Optional[Thermostat.Enums.TemperatureSetpointHoldEnum]),
                 ClusterObjectFieldDescriptor(Label="temperatureSetpointHoldDuration", Tag=0x00000024, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="thermostatProgrammingOperationMode", Tag=0x00000025, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="thermostatRunningState", Tag=0x00000029, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="setpointChangeSource", Tag=0x00000030, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="setpointChangeSource", Tag=0x00000030, Type=typing.Optional[Thermostat.Enums.SetpointChangeSourceEnum]),
                 ClusterObjectFieldDescriptor(Label="setpointChangeAmount", Tag=0x00000031, Type=typing.Union[None, Nullable, int]),
                 ClusterObjectFieldDescriptor(Label="setpointChangeSourceTimestamp", Tag=0x00000032, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="occupiedSetback", Tag=0x00000034, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="occupiedSetbackMin", Tag=0x00000035, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="occupiedSetbackMax", Tag=0x00000036, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="unoccupiedSetback", Tag=0x00000037, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="unoccupiedSetbackMin", Tag=0x00000038, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="unoccupiedSetbackMax", Tag=0x00000039, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="emergencyHeatDelta", Tag=0x0000003A, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="ACType", Tag=0x00000040, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="ACType", Tag=0x00000040, Type=typing.Optional[Thermostat.Enums.ACTypeEnum]),
                 ClusterObjectFieldDescriptor(Label="ACCapacity", Tag=0x00000041, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="ACRefrigerantType", Tag=0x00000042, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="ACCompressorType", Tag=0x00000043, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="ACRefrigerantType", Tag=0x00000042, Type=typing.Optional[Thermostat.Enums.ACRefrigerantTypeEnum]),
+                ClusterObjectFieldDescriptor(Label="ACCompressorType", Tag=0x00000043, Type=typing.Optional[Thermostat.Enums.ACCompressorTypeEnum]),
                 ClusterObjectFieldDescriptor(Label="ACErrorCode", Tag=0x00000044, Type=typing.Optional[uint]),
-                ClusterObjectFieldDescriptor(Label="ACLouverPosition", Tag=0x00000045, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="ACLouverPosition", Tag=0x00000045, Type=typing.Optional[Thermostat.Enums.ACLouverPositionEnum]),
                 ClusterObjectFieldDescriptor(Label="ACCoilTemperature", Tag=0x00000046, Type=typing.Union[None, Nullable, int]),
-                ClusterObjectFieldDescriptor(Label="ACCapacityformat", Tag=0x00000047, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="ACCapacityformat", Tag=0x00000047, Type=typing.Optional[Thermostat.Enums.ACCapacityFormatEnum]),
+                ClusterObjectFieldDescriptor(Label="presetTypes", Tag=0x00000048, Type=typing.Optional[typing.List[Thermostat.Structs.PresetTypeStruct]]),
+                ClusterObjectFieldDescriptor(Label="scheduleTypes", Tag=0x00000049, Type=typing.Optional[typing.List[Thermostat.Structs.ScheduleTypeStruct]]),
+                ClusterObjectFieldDescriptor(Label="numberOfPresets", Tag=0x0000004A, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="numberOfSchedules", Tag=0x0000004B, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="numberOfScheduleTransitions", Tag=0x0000004C, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="numberOfScheduleTransitionPerDay", Tag=0x0000004D, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="activePresetHandle", Tag=0x0000004E, Type=typing.Union[None, Nullable, bytes]),
+                ClusterObjectFieldDescriptor(Label="activeScheduleHandle", Tag=0x0000004F, Type=typing.Union[None, Nullable, bytes]),
+                ClusterObjectFieldDescriptor(Label="presets", Tag=0x00000050, Type=typing.Optional[typing.List[Thermostat.Structs.PresetStruct]]),
+                ClusterObjectFieldDescriptor(Label="schedules", Tag=0x00000051, Type=typing.Optional[typing.List[Thermostat.Structs.ScheduleStruct]]),
+                ClusterObjectFieldDescriptor(Label="presetsSchedulesEditable", Tag=0x00000052, Type=typing.Optional[bool]),
+                ClusterObjectFieldDescriptor(Label="temperatureSetpointHoldPolicy", Tag=0x00000053, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="setpointHoldExpiryTimestamp", Tag=0x00000054, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="queuedPreset", Tag=0x00000055, Type=typing.Union[None, Nullable, Thermostat.Structs.QueuedPresetStruct]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
@@ -23652,84 +30804,180 @@
     unoccupiedHeatingSetpoint: 'typing.Optional[int]' = None
     minHeatSetpointLimit: 'typing.Optional[int]' = None
     maxHeatSetpointLimit: 'typing.Optional[int]' = None
     minCoolSetpointLimit: 'typing.Optional[int]' = None
     maxCoolSetpointLimit: 'typing.Optional[int]' = None
     minSetpointDeadBand: 'typing.Optional[int]' = None
     remoteSensing: 'typing.Optional[uint]' = None
-    controlSequenceOfOperation: 'Thermostat.Enums.ThermostatControlSequence' = None
-    systemMode: 'uint' = None
-    thermostatRunningMode: 'typing.Optional[uint]' = None
-    startOfWeek: 'typing.Optional[uint]' = None
+    controlSequenceOfOperation: 'Thermostat.Enums.ControlSequenceOfOperationEnum' = None
+    systemMode: 'Thermostat.Enums.SystemModeEnum' = None
+    thermostatRunningMode: 'typing.Optional[Thermostat.Enums.ThermostatRunningModeEnum]' = None
+    startOfWeek: 'typing.Optional[Thermostat.Enums.StartOfWeekEnum]' = None
     numberOfWeeklyTransitions: 'typing.Optional[uint]' = None
     numberOfDailyTransitions: 'typing.Optional[uint]' = None
-    temperatureSetpointHold: 'typing.Optional[uint]' = None
+    temperatureSetpointHold: 'typing.Optional[Thermostat.Enums.TemperatureSetpointHoldEnum]' = None
     temperatureSetpointHoldDuration: 'typing.Union[None, Nullable, uint]' = None
     thermostatProgrammingOperationMode: 'typing.Optional[uint]' = None
     thermostatRunningState: 'typing.Optional[uint]' = None
-    setpointChangeSource: 'typing.Optional[uint]' = None
+    setpointChangeSource: 'typing.Optional[Thermostat.Enums.SetpointChangeSourceEnum]' = None
     setpointChangeAmount: 'typing.Union[None, Nullable, int]' = None
     setpointChangeSourceTimestamp: 'typing.Optional[uint]' = None
     occupiedSetback: 'typing.Union[None, Nullable, uint]' = None
     occupiedSetbackMin: 'typing.Union[None, Nullable, uint]' = None
     occupiedSetbackMax: 'typing.Union[None, Nullable, uint]' = None
     unoccupiedSetback: 'typing.Union[None, Nullable, uint]' = None
     unoccupiedSetbackMin: 'typing.Union[None, Nullable, uint]' = None
     unoccupiedSetbackMax: 'typing.Union[None, Nullable, uint]' = None
     emergencyHeatDelta: 'typing.Optional[uint]' = None
-    ACType: 'typing.Optional[uint]' = None
+    ACType: 'typing.Optional[Thermostat.Enums.ACTypeEnum]' = None
     ACCapacity: 'typing.Optional[uint]' = None
-    ACRefrigerantType: 'typing.Optional[uint]' = None
-    ACCompressorType: 'typing.Optional[uint]' = None
+    ACRefrigerantType: 'typing.Optional[Thermostat.Enums.ACRefrigerantTypeEnum]' = None
+    ACCompressorType: 'typing.Optional[Thermostat.Enums.ACCompressorTypeEnum]' = None
     ACErrorCode: 'typing.Optional[uint]' = None
-    ACLouverPosition: 'typing.Optional[uint]' = None
+    ACLouverPosition: 'typing.Optional[Thermostat.Enums.ACLouverPositionEnum]' = None
     ACCoilTemperature: 'typing.Union[None, Nullable, int]' = None
-    ACCapacityformat: 'typing.Optional[uint]' = None
+    ACCapacityformat: 'typing.Optional[Thermostat.Enums.ACCapacityFormatEnum]' = None
+    presetTypes: 'typing.Optional[typing.List[Thermostat.Structs.PresetTypeStruct]]' = None
+    scheduleTypes: 'typing.Optional[typing.List[Thermostat.Structs.ScheduleTypeStruct]]' = None
+    numberOfPresets: 'typing.Optional[uint]' = None
+    numberOfSchedules: 'typing.Optional[uint]' = None
+    numberOfScheduleTransitions: 'typing.Optional[uint]' = None
+    numberOfScheduleTransitionPerDay: 'typing.Union[None, Nullable, uint]' = None
+    activePresetHandle: 'typing.Union[None, Nullable, bytes]' = None
+    activeScheduleHandle: 'typing.Union[None, Nullable, bytes]' = None
+    presets: 'typing.Optional[typing.List[Thermostat.Structs.PresetStruct]]' = None
+    schedules: 'typing.Optional[typing.List[Thermostat.Structs.ScheduleStruct]]' = None
+    presetsSchedulesEditable: 'typing.Optional[bool]' = None
+    temperatureSetpointHoldPolicy: 'typing.Optional[uint]' = None
+    setpointHoldExpiryTimestamp: 'typing.Union[None, Nullable, uint]' = None
+    queuedPreset: 'typing.Union[None, Nullable, Thermostat.Structs.QueuedPresetStruct]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class SetpointAdjustMode(MatterIntEnum):
-            kHeat = 0x00
-            kCool = 0x01
-            kBoth = 0x02
+        class ACCapacityFormatEnum(MatterIntEnum):
+            kBTUh = 0x00
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 3,
+            kUnknownEnumValue = 1,
+
+        class ACCompressorTypeEnum(MatterIntEnum):
+            kUnknown = 0x00
+            kT1 = 0x01
+            kT2 = 0x02
+            kT3 = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
+
+        class ACLouverPositionEnum(MatterIntEnum):
+            kClosed = 0x01
+            kOpen = 0x02
+            kQuarter = 0x03
+            kHalf = 0x04
+            kThreeQuarters = 0x05
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 0,
+
+        class ACRefrigerantTypeEnum(MatterIntEnum):
+            kUnknown = 0x00
+            kR22 = 0x01
+            kR410a = 0x02
+            kR407c = 0x03
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 4,
 
-        class ThermostatControlSequence(MatterIntEnum):
+        class ACTypeEnum(MatterIntEnum):
+            kUnknown = 0x00
+            kCoolingFixed = 0x01
+            kHeatPumpFixed = 0x02
+            kCoolingInverter = 0x03
+            kHeatPumpInverter = 0x04
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 5,
+
+        class ControlSequenceOfOperationEnum(MatterIntEnum):
             kCoolingOnly = 0x00
             kCoolingWithReheat = 0x01
             kHeatingOnly = 0x02
             kHeatingWithReheat = 0x03
             kCoolingAndHeating = 0x04
             kCoolingAndHeatingWithReheat = 0x05
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 6,
 
-        class ThermostatRunningMode(MatterIntEnum):
-            kOff = 0x00
-            kCool = 0x03
-            kHeat = 0x04
+        class PresetScenarioEnum(MatterIntEnum):
+            kUnspecified = 0x00
+            kOccupied = 0x01
+            kUnoccupied = 0x02
+            kSleep = 0x03
+            kWake = 0x04
+            kVacation = 0x05
+            kUserDefined = 0x06
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 1,
+            kUnknownEnumValue = 7,
+
+        class SetpointChangeSourceEnum(MatterIntEnum):
+            kManual = 0x00
+            kSchedule = 0x01
+            kExternal = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 3,
+
+        class SetpointRaiseLowerModeEnum(MatterIntEnum):
+            kHeat = 0x00
+            kCool = 0x01
+            kBoth = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 3,
+
+        class StartOfWeekEnum(MatterIntEnum):
+            kSunday = 0x00
+            kMonday = 0x01
+            kTuesday = 0x02
+            kWednesday = 0x03
+            kThursday = 0x04
+            kFriday = 0x05
+            kSaturday = 0x06
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 7,
 
-        class ThermostatSystemMode(MatterIntEnum):
+        class SystemModeEnum(MatterIntEnum):
             kOff = 0x00
             kAuto = 0x01
             kCool = 0x03
             kHeat = 0x04
             kEmergencyHeat = 0x05
             kPrecooling = 0x06
             kFanOnly = 0x07
@@ -23737,41 +30985,216 @@
             kSleep = 0x09
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 2,
 
+        class TemperatureSetpointHoldEnum(MatterIntEnum):
+            kSetpointHoldOff = 0x00
+            kSetpointHoldOn = 0x01
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 2,
+
+        class ThermostatRunningModeEnum(MatterIntEnum):
+            kOff = 0x00
+            kCool = 0x03
+            kHeat = 0x04
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 1,
+
     class Bitmaps:
-        class DayOfWeek(IntFlag):
-            kSunday = 0x1
-            kMonday = 0x2
-            kTuesday = 0x4
-            kWednesday = 0x8
-            kThursday = 0x10
-            kFriday = 0x20
-            kSaturday = 0x40
-            kAway = 0x80
+        class ACErrorCodeBitmap(IntFlag):
+            kCompressorFail = 0x1
+            kRoomSensorFail = 0x2
+            kOutdoorSensorFail = 0x4
+            kCoilSensorFail = 0x8
+            kFanFail = 0x10
 
         class Feature(IntFlag):
             kHeating = 0x1
             kCooling = 0x2
             kOccupancy = 0x4
             kScheduleConfiguration = 0x8
             kSetback = 0x10
             kAutoMode = 0x20
             kLocalTemperatureNotExposed = 0x40
+            kMatterScheduleConfiguration = 0x80
+            kPresets = 0x100
+            kSetpoints = 0x200
+            kQueuedPresetsSupported = 0x400
+
+        class HVACSystemTypeBitmap(IntFlag):
+            kCoolingStage = 0x3
+            kHeatingStage = 0xC
+            kHeatingIsHeatPump = 0x10
+            kHeatingUsesFuel = 0x20
+
+        class PresetTypeFeaturesBitmap(IntFlag):
+            kAutomatic = 0x1
+            kSupportsNames = 0x2
+
+        class ProgrammingOperationModeBitmap(IntFlag):
+            kScheduleActive = 0x1
+            kAutoRecovery = 0x2
+            kEconomy = 0x4
+
+        class RelayStateBitmap(IntFlag):
+            kHeat = 0x1
+            kCool = 0x2
+            kFan = 0x4
+            kHeatStage2 = 0x8
+            kCoolStage2 = 0x10
+            kFanStage2 = 0x20
+            kFanStage3 = 0x40
+
+        class RemoteSensingBitmap(IntFlag):
+            kLocalTemperature = 0x1
+            kOutdoorTemperature = 0x2
+            kOccupancy = 0x4
+
+        class ScheduleDayOfWeekBitmap(IntFlag):
+            kSunday = 0x1
+            kMonday = 0x2
+            kTuesday = 0x4
+            kWednesday = 0x8
+            kThursday = 0x10
+            kFriday = 0x20
+            kSaturday = 0x40
+            kAway = 0x80
 
-        class ModeForSequence(IntFlag):
+        class ScheduleModeBitmap(IntFlag):
             kHeatSetpointPresent = 0x1
             kCoolSetpointPresent = 0x2
 
+        class ScheduleTypeFeaturesBitmap(IntFlag):
+            kSupportsPresets = 0x1
+            kSupportsSetpoints = 0x2
+            kSupportsNames = 0x4
+            kSupportsOff = 0x8
+
+        class TemperatureSetpointHoldPolicyBitmap(IntFlag):
+            kHoldDurationElapsed = 0x1
+            kHoldDurationElapsedOrPresetChanged = 0x2
+
     class Structs:
         @dataclass
-        class ThermostatScheduleTransition(ClusterObject):
+        class ScheduleTransitionStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="dayOfWeek", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="transitionTime", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="presetHandle", Tag=2, Type=typing.Optional[bytes]),
+                        ClusterObjectFieldDescriptor(Label="systemMode", Tag=3, Type=typing.Optional[Thermostat.Enums.SystemModeEnum]),
+                        ClusterObjectFieldDescriptor(Label="coolingSetpoint", Tag=4, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="heatingSetpoint", Tag=5, Type=typing.Optional[int]),
+                    ])
+
+            dayOfWeek: 'uint' = 0
+            transitionTime: 'uint' = 0
+            presetHandle: 'typing.Optional[bytes]' = None
+            systemMode: 'typing.Optional[Thermostat.Enums.SystemModeEnum]' = None
+            coolingSetpoint: 'typing.Optional[int]' = None
+            heatingSetpoint: 'typing.Optional[int]' = None
+
+        @dataclass
+        class ScheduleStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="scheduleHandle", Tag=0, Type=typing.Union[Nullable, bytes]),
+                        ClusterObjectFieldDescriptor(Label="systemMode", Tag=1, Type=Thermostat.Enums.SystemModeEnum),
+                        ClusterObjectFieldDescriptor(Label="name", Tag=2, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="presetHandle", Tag=3, Type=typing.Optional[bytes]),
+                        ClusterObjectFieldDescriptor(Label="transitions", Tag=4, Type=typing.List[Thermostat.Structs.ScheduleTransitionStruct]),
+                        ClusterObjectFieldDescriptor(Label="builtIn", Tag=5, Type=typing.Union[None, Nullable, bool]),
+                    ])
+
+            scheduleHandle: 'typing.Union[Nullable, bytes]' = NullValue
+            systemMode: 'Thermostat.Enums.SystemModeEnum' = 0
+            name: 'typing.Optional[str]' = None
+            presetHandle: 'typing.Optional[bytes]' = None
+            transitions: 'typing.List[Thermostat.Structs.ScheduleTransitionStruct]' = field(default_factory=lambda: [])
+            builtIn: 'typing.Union[None, Nullable, bool]' = None
+
+        @dataclass
+        class PresetStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="presetHandle", Tag=0, Type=typing.Union[Nullable, bytes]),
+                        ClusterObjectFieldDescriptor(Label="presetScenario", Tag=1, Type=Thermostat.Enums.PresetScenarioEnum),
+                        ClusterObjectFieldDescriptor(Label="name", Tag=2, Type=typing.Union[None, Nullable, str]),
+                        ClusterObjectFieldDescriptor(Label="coolingSetpoint", Tag=3, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="heatingSetpoint", Tag=4, Type=typing.Optional[int]),
+                        ClusterObjectFieldDescriptor(Label="builtIn", Tag=5, Type=typing.Union[Nullable, bool]),
+                    ])
+
+            presetHandle: 'typing.Union[Nullable, bytes]' = NullValue
+            presetScenario: 'Thermostat.Enums.PresetScenarioEnum' = 0
+            name: 'typing.Union[None, Nullable, str]' = None
+            coolingSetpoint: 'typing.Optional[int]' = None
+            heatingSetpoint: 'typing.Optional[int]' = None
+            builtIn: 'typing.Union[Nullable, bool]' = NullValue
+
+        @dataclass
+        class PresetTypeStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="presetScenario", Tag=0, Type=Thermostat.Enums.PresetScenarioEnum),
+                        ClusterObjectFieldDescriptor(Label="numberOfPresets", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="presetTypeFeatures", Tag=2, Type=uint),
+                    ])
+
+            presetScenario: 'Thermostat.Enums.PresetScenarioEnum' = 0
+            numberOfPresets: 'uint' = 0
+            presetTypeFeatures: 'uint' = 0
+
+        @dataclass
+        class QueuedPresetStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="presetHandle", Tag=0, Type=typing.Union[Nullable, bytes]),
+                        ClusterObjectFieldDescriptor(Label="transitionTimestamp", Tag=1, Type=typing.Union[Nullable, uint]),
+                    ])
+
+            presetHandle: 'typing.Union[Nullable, bytes]' = NullValue
+            transitionTimestamp: 'typing.Union[Nullable, uint]' = NullValue
+
+        @dataclass
+        class ScheduleTypeStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="systemMode", Tag=0, Type=Thermostat.Enums.SystemModeEnum),
+                        ClusterObjectFieldDescriptor(Label="numberOfSchedules", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="scheduleTypeFeatures", Tag=2, Type=uint),
+                    ])
+
+            systemMode: 'Thermostat.Enums.SystemModeEnum' = 0
+            numberOfSchedules: 'uint' = 0
+            scheduleTypeFeatures: 'uint' = 0
+
+        @dataclass
+        class WeeklyScheduleTransitionStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="transitionTime", Tag=0, Type=uint),
                         ClusterObjectFieldDescriptor(Label="heatSetpoint", Tag=1, Type=typing.Union[Nullable, int]),
                         ClusterObjectFieldDescriptor(Label="coolSetpoint", Tag=2, Type=typing.Union[Nullable, int]),
@@ -23789,19 +31212,19 @@
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="mode", Tag=0, Type=Thermostat.Enums.SetpointAdjustMode),
+                        ClusterObjectFieldDescriptor(Label="mode", Tag=0, Type=Thermostat.Enums.SetpointRaiseLowerModeEnum),
                         ClusterObjectFieldDescriptor(Label="amount", Tag=1, Type=int),
                     ])
 
-            mode: 'Thermostat.Enums.SetpointAdjustMode' = 0
+            mode: 'Thermostat.Enums.SetpointRaiseLowerModeEnum' = 0
             amount: 'int' = 0
 
         @dataclass
         class GetWeeklyScheduleResponse(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000201
             command_id: typing.ClassVar[int] = 0x00000000
             is_client: typing.ClassVar[bool] = False
@@ -23810,21 +31233,21 @@
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="numberOfTransitionsForSequence", Tag=0, Type=uint),
                         ClusterObjectFieldDescriptor(Label="dayOfWeekForSequence", Tag=1, Type=uint),
                         ClusterObjectFieldDescriptor(Label="modeForSequence", Tag=2, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="transitions", Tag=3, Type=typing.List[Thermostat.Structs.ThermostatScheduleTransition]),
+                        ClusterObjectFieldDescriptor(Label="transitions", Tag=3, Type=typing.List[Thermostat.Structs.WeeklyScheduleTransitionStruct]),
                     ])
 
             numberOfTransitionsForSequence: 'uint' = 0
             dayOfWeekForSequence: 'uint' = 0
             modeForSequence: 'uint' = 0
-            transitions: 'typing.List[Thermostat.Structs.ThermostatScheduleTransition]' = field(default_factory=lambda: [])
+            transitions: 'typing.List[Thermostat.Structs.WeeklyScheduleTransitionStruct]' = field(default_factory=lambda: [])
 
         @dataclass
         class SetWeeklySchedule(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000201
             command_id: typing.ClassVar[int] = 0x00000001
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = None
@@ -23832,21 +31255,21 @@
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="numberOfTransitionsForSequence", Tag=0, Type=uint),
                         ClusterObjectFieldDescriptor(Label="dayOfWeekForSequence", Tag=1, Type=uint),
                         ClusterObjectFieldDescriptor(Label="modeForSequence", Tag=2, Type=uint),
-                        ClusterObjectFieldDescriptor(Label="transitions", Tag=3, Type=typing.List[Thermostat.Structs.ThermostatScheduleTransition]),
+                        ClusterObjectFieldDescriptor(Label="transitions", Tag=3, Type=typing.List[Thermostat.Structs.WeeklyScheduleTransitionStruct]),
                     ])
 
             numberOfTransitionsForSequence: 'uint' = 0
             dayOfWeekForSequence: 'uint' = 0
             modeForSequence: 'uint' = 0
-            transitions: 'typing.List[Thermostat.Structs.ThermostatScheduleTransition]' = field(default_factory=lambda: [])
+            transitions: 'typing.List[Thermostat.Structs.WeeklyScheduleTransitionStruct]' = field(default_factory=lambda: [])
 
         @dataclass
         class GetWeeklySchedule(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000201
             command_id: typing.ClassVar[int] = 0x00000002
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'GetWeeklyScheduleResponse'
@@ -23871,14 +31294,119 @@
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                     ])
 
+        @dataclass
+        class SetActiveScheduleRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000201
+            command_id: typing.ClassVar[int] = 0x00000005
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="scheduleHandle", Tag=0, Type=bytes),
+                    ])
+
+            scheduleHandle: 'bytes' = b""
+
+        @dataclass
+        class SetActivePresetRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000201
+            command_id: typing.ClassVar[int] = 0x00000006
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="presetHandle", Tag=0, Type=bytes),
+                        ClusterObjectFieldDescriptor(Label="delayMinutes", Tag=1, Type=typing.Optional[uint]),
+                    ])
+
+            presetHandle: 'bytes' = b""
+            delayMinutes: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class StartPresetsSchedulesEditRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000201
+            command_id: typing.ClassVar[int] = 0x00000007
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="timeoutSeconds", Tag=0, Type=uint),
+                    ])
+
+            timeoutSeconds: 'uint' = 0
+
+        @dataclass
+        class CancelPresetsSchedulesEditRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000201
+            command_id: typing.ClassVar[int] = 0x00000008
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class CommitPresetsSchedulesRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000201
+            command_id: typing.ClassVar[int] = 0x00000009
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class CancelSetActivePresetRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000201
+            command_id: typing.ClassVar[int] = 0x0000000A
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class SetTemperatureSetpointHoldPolicy(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000201
+            command_id: typing.ClassVar[int] = 0x0000000B
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="temperatureSetpointHoldPolicy", Tag=0, Type=uint),
+                    ])
+
+            temperatureSetpointHoldPolicy: 'uint' = 0
+
     class Attributes:
         @dataclass
         class LocalTemperature(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
@@ -24220,65 +31748,65 @@
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000001B
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=Thermostat.Enums.ThermostatControlSequence)
+                return ClusterObjectFieldDescriptor(Type=Thermostat.Enums.ControlSequenceOfOperationEnum)
 
-            value: 'Thermostat.Enums.ThermostatControlSequence' = 0
+            value: 'Thermostat.Enums.ControlSequenceOfOperationEnum' = 0
 
         @dataclass
         class SystemMode(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000001C
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=Thermostat.Enums.SystemModeEnum)
 
-            value: 'uint' = 0
+            value: 'Thermostat.Enums.SystemModeEnum' = 0
 
         @dataclass
         class ThermostatRunningMode(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x0000001E
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[Thermostat.Enums.ThermostatRunningModeEnum])
 
-            value: 'typing.Optional[uint]' = None
+            value: 'typing.Optional[Thermostat.Enums.ThermostatRunningModeEnum]' = None
 
         @dataclass
         class StartOfWeek(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000020
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[Thermostat.Enums.StartOfWeekEnum])
 
-            value: 'typing.Optional[uint]' = None
+            value: 'typing.Optional[Thermostat.Enums.StartOfWeekEnum]' = None
 
         @dataclass
         class NumberOfWeeklyTransitions(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
@@ -24316,17 +31844,17 @@
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000023
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[Thermostat.Enums.TemperatureSetpointHoldEnum])
 
-            value: 'typing.Optional[uint]' = None
+            value: 'typing.Optional[Thermostat.Enums.TemperatureSetpointHoldEnum]' = None
 
         @dataclass
         class TemperatureSetpointHoldDuration(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
@@ -24380,17 +31908,17 @@
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000030
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[Thermostat.Enums.SetpointChangeSourceEnum])
 
-            value: 'typing.Optional[uint]' = None
+            value: 'typing.Optional[Thermostat.Enums.SetpointChangeSourceEnum]' = None
 
         @dataclass
         class SetpointChangeAmount(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
@@ -24540,17 +32068,17 @@
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000040
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[Thermostat.Enums.ACTypeEnum])
 
-            value: 'typing.Optional[uint]' = None
+            value: 'typing.Optional[Thermostat.Enums.ACTypeEnum]' = None
 
         @dataclass
         class ACCapacity(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
@@ -24572,33 +32100,33 @@
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000042
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[Thermostat.Enums.ACRefrigerantTypeEnum])
 
-            value: 'typing.Optional[uint]' = None
+            value: 'typing.Optional[Thermostat.Enums.ACRefrigerantTypeEnum]' = None
 
         @dataclass
         class ACCompressorType(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000043
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[Thermostat.Enums.ACCompressorTypeEnum])
 
-            value: 'typing.Optional[uint]' = None
+            value: 'typing.Optional[Thermostat.Enums.ACCompressorTypeEnum]' = None
 
         @dataclass
         class ACErrorCode(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
@@ -24620,17 +32148,17 @@
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000045
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[Thermostat.Enums.ACLouverPositionEnum])
 
-            value: 'typing.Optional[uint]' = None
+            value: 'typing.Optional[Thermostat.Enums.ACLouverPositionEnum]' = None
 
         @dataclass
         class ACCoilTemperature(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
@@ -24652,19 +32180,243 @@
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000047
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[Thermostat.Enums.ACCapacityFormatEnum])
+
+            value: 'typing.Optional[Thermostat.Enums.ACCapacityFormatEnum]' = None
+
+        @dataclass
+        class PresetTypes(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000048
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[Thermostat.Structs.PresetTypeStruct]])
+
+            value: 'typing.Optional[typing.List[Thermostat.Structs.PresetTypeStruct]]' = None
+
+        @dataclass
+        class ScheduleTypes(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000049
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[Thermostat.Structs.ScheduleTypeStruct]])
+
+            value: 'typing.Optional[typing.List[Thermostat.Structs.ScheduleTypeStruct]]' = None
+
+        @dataclass
+        class NumberOfPresets(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000004A
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class NumberOfSchedules(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000004B
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class NumberOfScheduleTransitions(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000004C
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class NumberOfScheduleTransitionPerDay(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000004D
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class ActivePresetHandle(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000004E
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, bytes])
+
+            value: 'typing.Union[None, Nullable, bytes]' = None
+
+        @dataclass
+        class ActiveScheduleHandle(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000004F
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, bytes])
+
+            value: 'typing.Union[None, Nullable, bytes]' = None
+
+        @dataclass
+        class Presets(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000050
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[Thermostat.Structs.PresetStruct]])
+
+            value: 'typing.Optional[typing.List[Thermostat.Structs.PresetStruct]]' = None
+
+        @dataclass
+        class Schedules(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000051
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[Thermostat.Structs.ScheduleStruct]])
+
+            value: 'typing.Optional[typing.List[Thermostat.Structs.ScheduleStruct]]' = None
+
+        @dataclass
+        class PresetsSchedulesEditable(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000052
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[bool])
+
+            value: 'typing.Optional[bool]' = None
+
+        @dataclass
+        class TemperatureSetpointHoldPolicy(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000053
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
 
             value: 'typing.Optional[uint]' = None
 
         @dataclass
+        class SetpointHoldExpiryTimestamp(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000054
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
+
+            value: 'typing.Union[None, Nullable, uint]' = None
+
+        @dataclass
+        class QueuedPreset(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000201
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000055
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, Thermostat.Structs.QueuedPresetStruct])
+
+            value: 'typing.Union[None, Nullable, Thermostat.Structs.QueuedPresetStruct]' = None
+
+        @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000201
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
@@ -24829,16 +32581,16 @@
             kUnknownEnumValue = 7,
 
         class FanModeSequenceEnum(MatterIntEnum):
             kOffLowMedHigh = 0x00
             kOffLowHigh = 0x01
             kOffLowMedHighAuto = 0x02
             kOffLowHighAuto = 0x03
-            kOffOnAuto = 0x04
-            kOffOn = 0x05
+            kOffHighAuto = 0x04
+            kOffHigh = 0x05
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 6,
 
         class StepDirectionEnum(MatterIntEnum):
@@ -25183,83 +32935,115 @@
 class ThermostatUserInterfaceConfiguration(Cluster):
     id: typing.ClassVar[int] = 0x00000204
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
-                ClusterObjectFieldDescriptor(Label="temperatureDisplayMode", Tag=0x00000000, Type=uint),
-                ClusterObjectFieldDescriptor(Label="keypadLockout", Tag=0x00000001, Type=uint),
-                ClusterObjectFieldDescriptor(Label="scheduleProgrammingVisibility", Tag=0x00000002, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="temperatureDisplayMode", Tag=0x00000000, Type=ThermostatUserInterfaceConfiguration.Enums.TemperatureDisplayModeEnum),
+                ClusterObjectFieldDescriptor(Label="keypadLockout", Tag=0x00000001, Type=ThermostatUserInterfaceConfiguration.Enums.KeypadLockoutEnum),
+                ClusterObjectFieldDescriptor(Label="scheduleProgrammingVisibility", Tag=0x00000002, Type=typing.Optional[ThermostatUserInterfaceConfiguration.Enums.ScheduleProgrammingVisibilityEnum]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
 
-    temperatureDisplayMode: 'uint' = None
-    keypadLockout: 'uint' = None
-    scheduleProgrammingVisibility: 'typing.Optional[uint]' = None
+    temperatureDisplayMode: 'ThermostatUserInterfaceConfiguration.Enums.TemperatureDisplayModeEnum' = None
+    keypadLockout: 'ThermostatUserInterfaceConfiguration.Enums.KeypadLockoutEnum' = None
+    scheduleProgrammingVisibility: 'typing.Optional[ThermostatUserInterfaceConfiguration.Enums.ScheduleProgrammingVisibilityEnum]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
+    class Enums:
+        class KeypadLockoutEnum(MatterIntEnum):
+            kNoLockout = 0x00
+            kLockout1 = 0x01
+            kLockout2 = 0x02
+            kLockout3 = 0x03
+            kLockout4 = 0x04
+            kLockout5 = 0x05
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 6,
+
+        class ScheduleProgrammingVisibilityEnum(MatterIntEnum):
+            kScheduleProgrammingPermitted = 0x00
+            kScheduleProgrammingDenied = 0x01
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 2,
+
+        class TemperatureDisplayModeEnum(MatterIntEnum):
+            kCelsius = 0x00
+            kFahrenheit = 0x01
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 2,
+
     class Attributes:
         @dataclass
         class TemperatureDisplayMode(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000204
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=ThermostatUserInterfaceConfiguration.Enums.TemperatureDisplayModeEnum)
 
-            value: 'uint' = 0
+            value: 'ThermostatUserInterfaceConfiguration.Enums.TemperatureDisplayModeEnum' = 0
 
         @dataclass
         class KeypadLockout(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000204
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=uint)
+                return ClusterObjectFieldDescriptor(Type=ThermostatUserInterfaceConfiguration.Enums.KeypadLockoutEnum)
 
-            value: 'uint' = 0
+            value: 'ThermostatUserInterfaceConfiguration.Enums.KeypadLockoutEnum' = 0
 
         @dataclass
         class ScheduleProgrammingVisibility(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000204
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
-                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[ThermostatUserInterfaceConfiguration.Enums.ScheduleProgrammingVisibilityEnum])
 
-            value: 'typing.Optional[uint]' = None
+            value: 'typing.Optional[ThermostatUserInterfaceConfiguration.Enums.ScheduleProgrammingVisibilityEnum]' = None
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000204
 
@@ -32451,23 +40235,25 @@
     id: typing.ClassVar[int] = 0x00000503
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
         return ClusterObjectDescriptor(
             Fields=[
                 ClusterObjectFieldDescriptor(Label="MACAddress", Tag=0x00000000, Type=typing.Optional[str]),
+                ClusterObjectFieldDescriptor(Label="linkLocalAddress", Tag=0x00000001, Type=typing.Optional[bytes]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
 
     MACAddress: 'typing.Optional[str]' = None
+    linkLocalAddress: 'typing.Optional[bytes]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
@@ -32485,14 +40271,30 @@
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Optional[str])
 
             value: 'typing.Optional[str]' = None
 
         @dataclass
+        class LinkLocalAddress(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000503
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[bytes])
+
+            value: 'typing.Optional[bytes]' = None
+
+        @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000503
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
@@ -32611,56 +40413,205 @@
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class ChannelStatusEnum(MatterIntEnum):
-            kSuccess = 0x00
-            kMultipleMatches = 0x01
-            kNoMatches = 0x02
+        class ChannelTypeEnum(MatterIntEnum):
+            kSatellite = 0x00
+            kCable = 0x01
+            kTerrestrial = 0x02
+            kOtt = 0x03
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 3,
+            kUnknownEnumValue = 4,
 
         class LineupInfoTypeEnum(MatterIntEnum):
             kMso = 0x00
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 1,
 
+        class StatusEnum(MatterIntEnum):
+            kSuccess = 0x00
+            kMultipleMatches = 0x01
+            kNoMatches = 0x02
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 3,
+
     class Bitmaps:
         class Feature(IntFlag):
             kChannelList = 0x1
             kLineupInfo = 0x2
+            kElectronicGuide = 0x4
+            kRecordProgram = 0x8
+
+        class RecordingFlagBitmap(IntFlag):
+            kScheduled = 0x1
+            kRecordSeries = 0x2
+            kRecorded = 0x4
 
     class Structs:
         @dataclass
+        class ProgramCastStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="name", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="role", Tag=1, Type=str),
+                    ])
+
+            name: 'str' = ""
+            role: 'str' = ""
+
+        @dataclass
+        class ProgramCategoryStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="category", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="subCategory", Tag=1, Type=typing.Optional[str]),
+                    ])
+
+            category: 'str' = ""
+            subCategory: 'typing.Optional[str]' = None
+
+        @dataclass
+        class SeriesInfoStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="season", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="episode", Tag=1, Type=str),
+                    ])
+
+            season: 'str' = ""
+            episode: 'str' = ""
+
+        @dataclass
         class ChannelInfoStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="majorNumber", Tag=0, Type=uint),
                         ClusterObjectFieldDescriptor(Label="minorNumber", Tag=1, Type=uint),
                         ClusterObjectFieldDescriptor(Label="name", Tag=2, Type=typing.Optional[str]),
                         ClusterObjectFieldDescriptor(Label="callSign", Tag=3, Type=typing.Optional[str]),
                         ClusterObjectFieldDescriptor(Label="affiliateCallSign", Tag=4, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="identifier", Tag=5, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="type", Tag=6, Type=typing.Optional[Channel.Enums.ChannelTypeEnum]),
                     ])
 
             majorNumber: 'uint' = 0
             minorNumber: 'uint' = 0
             name: 'typing.Optional[str]' = None
             callSign: 'typing.Optional[str]' = None
             affiliateCallSign: 'typing.Optional[str]' = None
+            identifier: 'typing.Optional[str]' = None
+            type: 'typing.Optional[Channel.Enums.ChannelTypeEnum]' = None
+
+        @dataclass
+        class ProgramStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="identifier", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="channel", Tag=1, Type=Channel.Structs.ChannelInfoStruct),
+                        ClusterObjectFieldDescriptor(Label="startTime", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="endTime", Tag=3, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="title", Tag=4, Type=str),
+                        ClusterObjectFieldDescriptor(Label="subtitle", Tag=5, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="description", Tag=6, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="audioLanguages", Tag=7, Type=typing.Optional[typing.List[str]]),
+                        ClusterObjectFieldDescriptor(Label="ratings", Tag=8, Type=typing.Optional[typing.List[str]]),
+                        ClusterObjectFieldDescriptor(Label="thumbnailUrl", Tag=9, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="posterArtUrl", Tag=10, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="dvbiUrl", Tag=11, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="releaseDate", Tag=12, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="parentalGuidanceText", Tag=13, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="recordingFlag", Tag=14, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="seriesInfo", Tag=15, Type=typing.Union[None, Nullable, Channel.Structs.SeriesInfoStruct]),
+                        ClusterObjectFieldDescriptor(Label="categoryList", Tag=16, Type=typing.Optional[typing.List[Channel.Structs.ProgramCategoryStruct]]),
+                        ClusterObjectFieldDescriptor(Label="castList", Tag=17, Type=typing.Optional[typing.List[Channel.Structs.ProgramCastStruct]]),
+                        ClusterObjectFieldDescriptor(Label="externalIDList", Tag=18, Type=typing.Optional[typing.List[Channel.Structs.ProgramCastStruct]]),
+                    ])
+
+            identifier: 'str' = ""
+            channel: 'Channel.Structs.ChannelInfoStruct' = field(default_factory=lambda: Channel.Structs.ChannelInfoStruct())
+            startTime: 'uint' = 0
+            endTime: 'uint' = 0
+            title: 'str' = ""
+            subtitle: 'typing.Optional[str]' = None
+            description: 'typing.Optional[str]' = None
+            audioLanguages: 'typing.Optional[typing.List[str]]' = None
+            ratings: 'typing.Optional[typing.List[str]]' = None
+            thumbnailUrl: 'typing.Optional[str]' = None
+            posterArtUrl: 'typing.Optional[str]' = None
+            dvbiUrl: 'typing.Optional[str]' = None
+            releaseDate: 'typing.Optional[str]' = None
+            parentalGuidanceText: 'typing.Optional[str]' = None
+            recordingFlag: 'typing.Optional[uint]' = None
+            seriesInfo: 'typing.Union[None, Nullable, Channel.Structs.SeriesInfoStruct]' = None
+            categoryList: 'typing.Optional[typing.List[Channel.Structs.ProgramCategoryStruct]]' = None
+            castList: 'typing.Optional[typing.List[Channel.Structs.ProgramCastStruct]]' = None
+            externalIDList: 'typing.Optional[typing.List[Channel.Structs.ProgramCastStruct]]' = None
+
+        @dataclass
+        class PageTokenStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="limit", Tag=0, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="after", Tag=1, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="before", Tag=2, Type=typing.Optional[str]),
+                    ])
+
+            limit: 'typing.Optional[uint]' = None
+            after: 'typing.Optional[str]' = None
+            before: 'typing.Optional[str]' = None
+
+        @dataclass
+        class ChannelPagingStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="previousToken", Tag=0, Type=typing.Union[None, Nullable, Channel.Structs.PageTokenStruct]),
+                        ClusterObjectFieldDescriptor(Label="nextToken", Tag=1, Type=typing.Union[None, Nullable, Channel.Structs.PageTokenStruct]),
+                    ])
+
+            previousToken: 'typing.Union[None, Nullable, Channel.Structs.PageTokenStruct]' = None
+            nextToken: 'typing.Union[None, Nullable, Channel.Structs.PageTokenStruct]' = None
+
+        @dataclass
+        class AdditionalInfoStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="name", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=str),
+                    ])
+
+            name: 'str' = ""
+            value: 'str' = ""
 
         @dataclass
         class LineupInfoStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
@@ -32699,19 +40650,19 @@
             is_client: typing.ClassVar[bool] = False
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=Channel.Enums.ChannelStatusEnum),
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=Channel.Enums.StatusEnum),
                         ClusterObjectFieldDescriptor(Label="data", Tag=1, Type=typing.Optional[str]),
                     ])
 
-            status: 'Channel.Enums.ChannelStatusEnum' = 0
+            status: 'Channel.Enums.StatusEnum' = 0
             data: 'typing.Optional[str]' = None
 
         @dataclass
         class ChangeChannelByNumber(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000504
             command_id: typing.ClassVar[int] = 0x00000002
             is_client: typing.ClassVar[bool] = True
@@ -32740,14 +40691,104 @@
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="count", Tag=0, Type=int),
                     ])
 
             count: 'int' = 0
 
+        @dataclass
+        class GetProgramGuide(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000504
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'ProgramGuideResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="startTime", Tag=0, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="endTime", Tag=1, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="channelList", Tag=2, Type=typing.Optional[typing.List[Channel.Structs.ChannelInfoStruct]]),
+                        ClusterObjectFieldDescriptor(Label="pageToken", Tag=3, Type=typing.Optional[Channel.Structs.PageTokenStruct]),
+                        ClusterObjectFieldDescriptor(Label="recordingFlag", Tag=4, Type=typing.Optional[uint]),
+                        ClusterObjectFieldDescriptor(Label="externalIDList", Tag=5, Type=typing.Optional[typing.List[Channel.Structs.AdditionalInfoStruct]]),
+                        ClusterObjectFieldDescriptor(Label="data", Tag=6, Type=typing.Optional[bytes]),
+                    ])
+
+            startTime: 'typing.Optional[uint]' = None
+            endTime: 'typing.Optional[uint]' = None
+            channelList: 'typing.Optional[typing.List[Channel.Structs.ChannelInfoStruct]]' = None
+            pageToken: 'typing.Optional[Channel.Structs.PageTokenStruct]' = None
+            recordingFlag: 'typing.Optional[uint]' = None
+            externalIDList: 'typing.Optional[typing.List[Channel.Structs.AdditionalInfoStruct]]' = None
+            data: 'typing.Optional[bytes]' = None
+
+        @dataclass
+        class ProgramGuideResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000504
+            command_id: typing.ClassVar[int] = 0x00000005
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="paging", Tag=0, Type=Channel.Structs.ChannelPagingStruct),
+                        ClusterObjectFieldDescriptor(Label="programList", Tag=1, Type=typing.List[Channel.Structs.ProgramStruct]),
+                    ])
+
+            paging: 'Channel.Structs.ChannelPagingStruct' = field(default_factory=lambda: Channel.Structs.ChannelPagingStruct())
+            programList: 'typing.List[Channel.Structs.ProgramStruct]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class RecordProgram(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000504
+            command_id: typing.ClassVar[int] = 0x00000006
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="programIdentifier", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="shouldRecordSeries", Tag=1, Type=bool),
+                        ClusterObjectFieldDescriptor(Label="externalIDList", Tag=2, Type=typing.List[Channel.Structs.AdditionalInfoStruct]),
+                        ClusterObjectFieldDescriptor(Label="data", Tag=3, Type=bytes),
+                    ])
+
+            programIdentifier: 'str' = ""
+            shouldRecordSeries: 'bool' = False
+            externalIDList: 'typing.List[Channel.Structs.AdditionalInfoStruct]' = field(default_factory=lambda: [])
+            data: 'bytes' = b""
+
+        @dataclass
+        class CancelRecordProgram(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000504
+            command_id: typing.ClassVar[int] = 0x00000007
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="programIdentifier", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="shouldRecordSeries", Tag=1, Type=bool),
+                        ClusterObjectFieldDescriptor(Label="externalIDList", Tag=2, Type=typing.List[Channel.Structs.AdditionalInfoStruct]),
+                        ClusterObjectFieldDescriptor(Label="data", Tag=3, Type=bytes),
+                    ])
+
+            programIdentifier: 'str' = ""
+            shouldRecordSeries: 'bool' = False
+            externalIDList: 'typing.List[Channel.Structs.AdditionalInfoStruct]' = field(default_factory=lambda: [])
+            data: 'bytes' = b""
+
     class Attributes:
         @dataclass
         class ChannelList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000504
 
@@ -32914,15 +40955,15 @@
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class TargetNavigatorStatusEnum(MatterIntEnum):
+        class StatusEnum(MatterIntEnum):
             kSuccess = 0x00
             kTargetNotFound = 0x01
             kNotAllowed = 0x02
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
@@ -32968,19 +41009,19 @@
             is_client: typing.ClassVar[bool] = False
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=TargetNavigator.Enums.TargetNavigatorStatusEnum),
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=TargetNavigator.Enums.StatusEnum),
                         ClusterObjectFieldDescriptor(Label="data", Tag=1, Type=typing.Optional[str]),
                     ])
 
-            status: 'TargetNavigator.Enums.TargetNavigatorStatusEnum' = 0
+            status: 'TargetNavigator.Enums.StatusEnum' = 0
             data: 'typing.Optional[str]' = None
 
     class Attributes:
         @dataclass
         class TargetList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
@@ -33104,14 +41145,38 @@
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
+    class Events:
+        @dataclass
+        class TargetUpdated(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000505
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="targetList", Tag=0, Type=typing.List[TargetNavigator.Structs.TargetInfoStruct]),
+                        ClusterObjectFieldDescriptor(Label="currentTarget", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="data", Tag=2, Type=bytes),
+                    ])
+
+            targetList: 'typing.List[TargetNavigator.Structs.TargetInfoStruct]' = field(default_factory=lambda: [])
+            currentTarget: 'uint' = 0
+            data: 'bytes' = b""
+
 
 @dataclass
 class MediaPlayback(Cluster):
     id: typing.ClassVar[int] = 0x00000506
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
@@ -33120,14 +41185,18 @@
                 ClusterObjectFieldDescriptor(Label="currentState", Tag=0x00000000, Type=MediaPlayback.Enums.PlaybackStateEnum),
                 ClusterObjectFieldDescriptor(Label="startTime", Tag=0x00000001, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="duration", Tag=0x00000002, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="sampledPosition", Tag=0x00000003, Type=typing.Union[None, Nullable, MediaPlayback.Structs.PlaybackPositionStruct]),
                 ClusterObjectFieldDescriptor(Label="playbackSpeed", Tag=0x00000004, Type=typing.Optional[float32]),
                 ClusterObjectFieldDescriptor(Label="seekRangeEnd", Tag=0x00000005, Type=typing.Union[None, Nullable, uint]),
                 ClusterObjectFieldDescriptor(Label="seekRangeStart", Tag=0x00000006, Type=typing.Union[None, Nullable, uint]),
+                ClusterObjectFieldDescriptor(Label="activeAudioTrack", Tag=0x00000007, Type=typing.Union[None, Nullable, MediaPlayback.Structs.TrackStruct]),
+                ClusterObjectFieldDescriptor(Label="availableAudioTracks", Tag=0x00000008, Type=typing.Union[None, Nullable, typing.List[MediaPlayback.Structs.TrackStruct]]),
+                ClusterObjectFieldDescriptor(Label="activeTextTrack", Tag=0x00000009, Type=typing.Union[None, Nullable, MediaPlayback.Structs.TrackStruct]),
+                ClusterObjectFieldDescriptor(Label="availableTextTracks", Tag=0x0000000A, Type=typing.Union[None, Nullable, typing.List[MediaPlayback.Structs.TrackStruct]]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
             ])
@@ -33135,53 +41204,111 @@
     currentState: 'MediaPlayback.Enums.PlaybackStateEnum' = None
     startTime: 'typing.Union[None, Nullable, uint]' = None
     duration: 'typing.Union[None, Nullable, uint]' = None
     sampledPosition: 'typing.Union[None, Nullable, MediaPlayback.Structs.PlaybackPositionStruct]' = None
     playbackSpeed: 'typing.Optional[float32]' = None
     seekRangeEnd: 'typing.Union[None, Nullable, uint]' = None
     seekRangeStart: 'typing.Union[None, Nullable, uint]' = None
+    activeAudioTrack: 'typing.Union[None, Nullable, MediaPlayback.Structs.TrackStruct]' = None
+    availableAudioTracks: 'typing.Union[None, Nullable, typing.List[MediaPlayback.Structs.TrackStruct]]' = None
+    activeTextTrack: 'typing.Union[None, Nullable, MediaPlayback.Structs.TrackStruct]' = None
+    availableTextTracks: 'typing.Union[None, Nullable, typing.List[MediaPlayback.Structs.TrackStruct]]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class MediaPlaybackStatusEnum(MatterIntEnum):
-            kSuccess = 0x00
-            kInvalidStateForCommand = 0x01
-            kNotAllowed = 0x02
-            kNotActive = 0x03
-            kSpeedOutOfRange = 0x04
-            kSeekOutOfRange = 0x05
+        class CharacteristicEnum(MatterIntEnum):
+            kForcedSubtitles = 0x00
+            kDescribesVideo = 0x01
+            kEasyToRead = 0x02
+            kFrameBased = 0x03
+            kMainProgram = 0x04
+            kOriginalContent = 0x05
+            kVoiceOverTranslation = 0x06
+            kCaption = 0x07
+            kSubtitle = 0x08
+            kAlternate = 0x09
+            kSupplementary = 0x0A
+            kCommentary = 0x0B
+            kDubbedTranslation = 0x0C
+            kDescription = 0x0D
+            kMetadata = 0x0E
+            kEnhancedAudioIntelligibility = 0x0F
+            kEmergency = 0x10
+            kKaraoke = 0x11
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 6,
+            kUnknownEnumValue = 18,
 
         class PlaybackStateEnum(MatterIntEnum):
             kPlaying = 0x00
             kPaused = 0x01
             kNotPlaying = 0x02
             kBuffering = 0x03
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 4,
 
+        class StatusEnum(MatterIntEnum):
+            kSuccess = 0x00
+            kInvalidStateForCommand = 0x01
+            kNotAllowed = 0x02
+            kNotActive = 0x03
+            kSpeedOutOfRange = 0x04
+            kSeekOutOfRange = 0x05
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 6,
+
     class Bitmaps:
         class Feature(IntFlag):
             kAdvancedSeek = 0x1
             kVariableSpeed = 0x2
+            kTextTracks = 0x4
+            kAudioTracks = 0x8
+            kAudioAdvance = 0x10
 
     class Structs:
         @dataclass
+        class TrackAttributesStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="languageCode", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="displayName", Tag=1, Type=typing.Union[None, Nullable, str]),
+                    ])
+
+            languageCode: 'str' = ""
+            displayName: 'typing.Union[None, Nullable, str]' = None
+
+        @dataclass
+        class TrackStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="id", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="trackAttributes", Tag=1, Type=typing.Union[Nullable, MediaPlayback.Structs.TrackAttributesStruct]),
+                    ])
+
+            id: 'str' = ""
+            trackAttributes: 'typing.Union[Nullable, MediaPlayback.Structs.TrackAttributesStruct]' = NullValue
+
+        @dataclass
         class PlaybackPositionStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="updatedAt", Tag=0, Type=uint),
                         ClusterObjectFieldDescriptor(Label="position", Tag=1, Type=typing.Union[Nullable, uint]),
@@ -33276,29 +41403,35 @@
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'PlaybackResponse'
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="audioAdvanceUnmuted", Tag=0, Type=typing.Optional[bool]),
                     ])
 
+            audioAdvanceUnmuted: 'typing.Optional[bool]' = None
+
         @dataclass
         class FastForward(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000506
             command_id: typing.ClassVar[int] = 0x00000007
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'PlaybackResponse'
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="audioAdvanceUnmuted", Tag=0, Type=typing.Optional[bool]),
                     ])
 
+            audioAdvanceUnmuted: 'typing.Optional[bool]' = None
+
         @dataclass
         class SkipForward(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000506
             command_id: typing.ClassVar[int] = 0x00000008
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'PlaybackResponse'
 
@@ -33334,19 +41467,19 @@
             is_client: typing.ClassVar[bool] = False
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=MediaPlayback.Enums.MediaPlaybackStatusEnum),
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=MediaPlayback.Enums.StatusEnum),
                         ClusterObjectFieldDescriptor(Label="data", Tag=1, Type=typing.Optional[str]),
                     ])
 
-            status: 'MediaPlayback.Enums.MediaPlaybackStatusEnum' = 0
+            status: 'MediaPlayback.Enums.StatusEnum' = 0
             data: 'typing.Optional[str]' = None
 
         @dataclass
         class Seek(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000506
             command_id: typing.ClassVar[int] = 0x0000000B
             is_client: typing.ClassVar[bool] = True
@@ -33357,14 +41490,61 @@
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="position", Tag=0, Type=uint),
                     ])
 
             position: 'uint' = 0
 
+        @dataclass
+        class ActivateAudioTrack(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000506
+            command_id: typing.ClassVar[int] = 0x0000000C
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="trackID", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="audioOutputIndex", Tag=1, Type=uint),
+                    ])
+
+            trackID: 'str' = ""
+            audioOutputIndex: 'uint' = 0
+
+        @dataclass
+        class ActivateTextTrack(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000506
+            command_id: typing.ClassVar[int] = 0x0000000D
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="trackID", Tag=0, Type=str),
+                    ])
+
+            trackID: 'str' = ""
+
+        @dataclass
+        class DeactivateTextTrack(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000506
+            command_id: typing.ClassVar[int] = 0x0000000E
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
     class Attributes:
         @dataclass
         class CurrentState(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000506
 
@@ -33471,14 +41651,78 @@
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, uint])
 
             value: 'typing.Union[None, Nullable, uint]' = None
 
         @dataclass
+        class ActiveAudioTrack(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000506
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000007
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, MediaPlayback.Structs.TrackStruct])
+
+            value: 'typing.Union[None, Nullable, MediaPlayback.Structs.TrackStruct]' = None
+
+        @dataclass
+        class AvailableAudioTracks(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000506
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000008
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, typing.List[MediaPlayback.Structs.TrackStruct]])
+
+            value: 'typing.Union[None, Nullable, typing.List[MediaPlayback.Structs.TrackStruct]]' = None
+
+        @dataclass
+        class ActiveTextTrack(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000506
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000009
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, MediaPlayback.Structs.TrackStruct])
+
+            value: 'typing.Union[None, Nullable, MediaPlayback.Structs.TrackStruct]' = None
+
+        @dataclass
+        class AvailableTextTracks(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000506
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000000A
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Union[None, Nullable, typing.List[MediaPlayback.Structs.TrackStruct]])
+
+            value: 'typing.Union[None, Nullable, typing.List[MediaPlayback.Structs.TrackStruct]]' = None
+
+        @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000506
 
             @ChipUtility.classproperty
             def attribute_id(cls) -> int:
@@ -33566,14 +41810,50 @@
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
+    class Events:
+        @dataclass
+        class StateChanged(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000506
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="currentState", Tag=0, Type=MediaPlayback.Enums.PlaybackStateEnum),
+                        ClusterObjectFieldDescriptor(Label="startTime", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="duration", Tag=2, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sampledPosition", Tag=3, Type=MediaPlayback.Structs.PlaybackPositionStruct),
+                        ClusterObjectFieldDescriptor(Label="playbackSpeed", Tag=4, Type=float32),
+                        ClusterObjectFieldDescriptor(Label="seekRangeEnd", Tag=5, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="seekRangeStart", Tag=6, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="data", Tag=7, Type=typing.Optional[bytes]),
+                        ClusterObjectFieldDescriptor(Label="audioAdvanceUnmuted", Tag=8, Type=bool),
+                    ])
+
+            currentState: 'MediaPlayback.Enums.PlaybackStateEnum' = 0
+            startTime: 'uint' = 0
+            duration: 'uint' = 0
+            sampledPosition: 'MediaPlayback.Structs.PlaybackPositionStruct' = field(default_factory=lambda: MediaPlayback.Structs.PlaybackPositionStruct())
+            playbackSpeed: 'float32' = 0.0
+            seekRangeEnd: 'uint' = 0
+            seekRangeStart: 'uint' = 0
+            data: 'typing.Optional[bytes]' = None
+            audioAdvanceUnmuted: 'bool' = False
+
 
 @dataclass
 class MediaInput(Cluster):
     id: typing.ClassVar[int] = 0x00000507
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
@@ -33986,15 +42266,15 @@
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class CecKeyCode(MatterIntEnum):
+        class CECKeyCodeEnum(MatterIntEnum):
             kSelect = 0x00
             kUp = 0x01
             kDown = 0x02
             kLeft = 0x03
             kRight = 0x04
             kRightUp = 0x05
             kRightDown = 0x06
@@ -34079,15 +42359,15 @@
             kData = 0x76
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
             kUnknownEnumValue = 14,
 
-        class KeypadInputStatusEnum(MatterIntEnum):
+        class StatusEnum(MatterIntEnum):
             kSuccess = 0x00
             kUnsupportedKey = 0x01
             kInvalidKeyInCurrentState = 0x02
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
@@ -34107,34 +42387,34 @@
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'SendKeyResponse'
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="keyCode", Tag=0, Type=KeypadInput.Enums.CecKeyCode),
+                        ClusterObjectFieldDescriptor(Label="keyCode", Tag=0, Type=KeypadInput.Enums.CECKeyCodeEnum),
                     ])
 
-            keyCode: 'KeypadInput.Enums.CecKeyCode' = 0
+            keyCode: 'KeypadInput.Enums.CECKeyCodeEnum' = 0
 
         @dataclass
         class SendKeyResponse(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x00000509
             command_id: typing.ClassVar[int] = 0x00000001
             is_client: typing.ClassVar[bool] = False
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=KeypadInput.Enums.KeypadInputStatusEnum),
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=KeypadInput.Enums.StatusEnum),
                     ])
 
-            status: 'KeypadInput.Enums.KeypadInputStatusEnum' = 0
+            status: 'KeypadInput.Enums.StatusEnum' = 0
 
     class Attributes:
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x00000509
@@ -34254,23 +42534,38 @@
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class ContentLaunchStatusEnum(MatterIntEnum):
-            kSuccess = 0x00
-            kUrlNotAvailable = 0x01
-            kAuthFailed = 0x02
+        class CharacteristicEnum(MatterIntEnum):
+            kForcedSubtitles = 0x00
+            kDescribesVideo = 0x01
+            kEasyToRead = 0x02
+            kFrameBased = 0x03
+            kMainProgram = 0x04
+            kOriginalContent = 0x05
+            kVoiceOverTranslation = 0x06
+            kCaption = 0x07
+            kSubtitle = 0x08
+            kAlternate = 0x09
+            kSupplementary = 0x0A
+            kCommentary = 0x0B
+            kDubbedTranslation = 0x0C
+            kDescription = 0x0D
+            kMetadata = 0x0E
+            kEnhancedAudioIntelligibility = 0x0F
+            kEmergency = 0x10
+            kKaraoke = 0x11
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 3,
+            kUnknownEnumValue = 18,
 
         class MetricTypeEnum(MatterIntEnum):
             kPixels = 0x00
             kPercentage = 0x01
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
@@ -34288,26 +42583,44 @@
             kLeague = 0x07
             kPopularity = 0x08
             kProvider = 0x09
             kSport = 0x0A
             kSportsTeam = 0x0B
             kType = 0x0C
             kVideo = 0x0D
+            kSeason = 0x0E
+            kEpisode = 0x0F
+            kAny = 0x10
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
-            kUnknownEnumValue = 14,
+            kUnknownEnumValue = 17,
+
+        class StatusEnum(MatterIntEnum):
+            kSuccess = 0x00
+            kURLNotAvailable = 0x01
+            kAuthFailed = 0x02
+            kTextTrackNotAvailable = 0x03
+            kAudioTrackNotAvailable = 0x04
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 5,
 
     class Bitmaps:
         class Feature(IntFlag):
             kContentSearch = 0x1
             kURLPlayback = 0x2
+            kAdvancedSeek = 0x3
+            kTextTracks = 0x4
+            kAudioTracks = 0x5
 
-        class SupportedStreamingProtocol(IntFlag):
+        class SupportedProtocolsBitmap(IntFlag):
             kDash = 0x1
             kHls = 0x2
 
     class Structs:
         @dataclass
         class DimensionStruct(ClusterObject):
             @ChipUtility.classproperty
@@ -34320,14 +42633,44 @@
                     ])
 
             width: 'float' = 0.0
             height: 'float' = 0.0
             metric: 'ContentLauncher.Enums.MetricTypeEnum' = 0
 
         @dataclass
+        class TrackPreferenceStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="languageCode", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="characteristics", Tag=1, Type=typing.Optional[typing.List[ContentLauncher.Enums.CharacteristicEnum]]),
+                        ClusterObjectFieldDescriptor(Label="audioOutputIndex", Tag=2, Type=uint),
+                    ])
+
+            languageCode: 'str' = ""
+            characteristics: 'typing.Optional[typing.List[ContentLauncher.Enums.CharacteristicEnum]]' = None
+            audioOutputIndex: 'uint' = 0
+
+        @dataclass
+        class PlaybackPreferencesStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="playbackPosition", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="textTrack", Tag=1, Type=ContentLauncher.Structs.TrackPreferenceStruct),
+                        ClusterObjectFieldDescriptor(Label="audioTracks", Tag=2, Type=typing.Optional[typing.List[ContentLauncher.Structs.TrackPreferenceStruct]]),
+                    ])
+
+            playbackPosition: 'uint' = 0
+            textTrack: 'ContentLauncher.Structs.TrackPreferenceStruct' = field(default_factory=lambda: ContentLauncher.Structs.TrackPreferenceStruct())
+            audioTracks: 'typing.Optional[typing.List[ContentLauncher.Structs.TrackPreferenceStruct]]' = None
+
+        @dataclass
         class AdditionalInfoStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="name", Tag=0, Type=str),
                         ClusterObjectFieldDescriptor(Label="value", Tag=1, Type=str),
@@ -34409,19 +42752,23 @@
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="search", Tag=0, Type=ContentLauncher.Structs.ContentSearchStruct),
                         ClusterObjectFieldDescriptor(Label="autoPlay", Tag=1, Type=bool),
                         ClusterObjectFieldDescriptor(Label="data", Tag=2, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="playbackPreferences", Tag=3, Type=typing.Optional[ContentLauncher.Structs.PlaybackPreferencesStruct]),
+                        ClusterObjectFieldDescriptor(Label="useCurrentContext", Tag=4, Type=typing.Optional[bool]),
                     ])
 
             search: 'ContentLauncher.Structs.ContentSearchStruct' = field(default_factory=lambda: ContentLauncher.Structs.ContentSearchStruct())
             autoPlay: 'bool' = False
             data: 'typing.Optional[str]' = None
+            playbackPreferences: 'typing.Optional[ContentLauncher.Structs.PlaybackPreferencesStruct]' = None
+            useCurrentContext: 'typing.Optional[bool]' = None
 
         @dataclass
         class LaunchURL(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0000050A
             command_id: typing.ClassVar[int] = 0x00000001
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'LauncherResponse'
@@ -34446,19 +42793,19 @@
             is_client: typing.ClassVar[bool] = False
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=ContentLauncher.Enums.ContentLaunchStatusEnum),
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=ContentLauncher.Enums.StatusEnum),
                         ClusterObjectFieldDescriptor(Label="data", Tag=1, Type=typing.Optional[str]),
                     ])
 
-            status: 'ContentLauncher.Enums.ContentLaunchStatusEnum' = 0
+            status: 'ContentLauncher.Enums.StatusEnum' = 0
             data: 'typing.Optional[str]' = None
 
     class Attributes:
         @dataclass
         class AcceptHeader(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
@@ -34837,15 +43184,15 @@
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
 
     class Enums:
-        class ApplicationLauncherStatusEnum(MatterIntEnum):
+        class StatusEnum(MatterIntEnum):
             kSuccess = 0x00
             kAppNotAvailable = 0x01
             kSystemBusy = 0x02
             # All received enum values that are not listed above will be mapped
             # to kUnknownEnumValue. This is a helper enum value that should only
             # be used by code to process how it handles receiving and unknown
             # enum value. This specific should never be transmitted.
@@ -34940,19 +43287,19 @@
             is_client: typing.ClassVar[bool] = False
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
-                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=ApplicationLauncher.Enums.ApplicationLauncherStatusEnum),
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=ApplicationLauncher.Enums.StatusEnum),
                         ClusterObjectFieldDescriptor(Label="data", Tag=1, Type=typing.Optional[bytes]),
                     ])
 
-            status: 'ApplicationLauncher.Enums.ApplicationLauncherStatusEnum' = 0
+            status: 'ApplicationLauncher.Enums.StatusEnum' = 0
             data: 'typing.Optional[bytes]' = None
 
     class Attributes:
         @dataclass
         class CatalogList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
@@ -35441,40 +43788,45 @@
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="tempAccountIdentifier", Tag=0, Type=str),
                         ClusterObjectFieldDescriptor(Label="setupPIN", Tag=1, Type=str),
+                        ClusterObjectFieldDescriptor(Label="node", Tag=2, Type=typing.Optional[uint]),
                     ])
 
             @ChipUtility.classproperty
             def must_use_timed_invoke(cls) -> bool:
                 return True
 
             tempAccountIdentifier: 'str' = ""
             setupPIN: 'str' = ""
+            node: 'typing.Optional[uint]' = None
 
         @dataclass
         class Logout(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0000050E
             command_id: typing.ClassVar[int] = 0x00000003
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = None
 
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
+                        ClusterObjectFieldDescriptor(Label="node", Tag=0, Type=typing.Optional[uint]),
                     ])
 
             @ChipUtility.classproperty
             def must_use_timed_invoke(cls) -> bool:
                 return True
 
+            node: 'typing.Optional[uint]' = None
+
     class Attributes:
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0000050E
 
@@ -35564,14 +43916,674 @@
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
+    class Events:
+        @dataclass
+        class LoggedOut(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050E
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="node", Tag=0, Type=typing.Optional[uint]),
+                    ])
+
+            node: 'typing.Optional[uint]' = None
+
+
+@dataclass
+class ContentControl(Cluster):
+    id: typing.ClassVar[int] = 0x0000050F
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="enabled", Tag=0x00000000, Type=bool),
+                ClusterObjectFieldDescriptor(Label="onDemandRatings", Tag=0x00000001, Type=typing.Optional[typing.List[ContentControl.Structs.RatingNameStruct]]),
+                ClusterObjectFieldDescriptor(Label="onDemandRatingThreshold", Tag=0x00000002, Type=typing.Optional[str]),
+                ClusterObjectFieldDescriptor(Label="scheduledContentRatings", Tag=0x00000003, Type=typing.Optional[typing.List[ContentControl.Structs.RatingNameStruct]]),
+                ClusterObjectFieldDescriptor(Label="scheduledContentRatingThreshold", Tag=0x00000004, Type=typing.Optional[str]),
+                ClusterObjectFieldDescriptor(Label="screenDailyTime", Tag=0x00000005, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="remainingScreenTime", Tag=0x00000006, Type=typing.Optional[uint]),
+                ClusterObjectFieldDescriptor(Label="blockUnrated", Tag=0x00000007, Type=bool),
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    enabled: 'bool' = None
+    onDemandRatings: 'typing.Optional[typing.List[ContentControl.Structs.RatingNameStruct]]' = None
+    onDemandRatingThreshold: 'typing.Optional[str]' = None
+    scheduledContentRatings: 'typing.Optional[typing.List[ContentControl.Structs.RatingNameStruct]]' = None
+    scheduledContentRatingThreshold: 'typing.Optional[str]' = None
+    screenDailyTime: 'typing.Optional[uint]' = None
+    remainingScreenTime: 'typing.Optional[uint]' = None
+    blockUnrated: 'bool' = None
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Bitmaps:
+        class Feature(IntFlag):
+            kScreenTime = 0x1
+            kPINManagement = 0x2
+            kBlockUnrated = 0x4
+            kOnDemandContentRating = 0x8
+            kScheduledContentRating = 0x10
+
+    class Structs:
+        @dataclass
+        class RatingNameStruct(ClusterObject):
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="ratingName", Tag=0, Type=str),
+                        ClusterObjectFieldDescriptor(Label="ratingNameDesc", Tag=1, Type=typing.Optional[str]),
+                    ])
+
+            ratingName: 'str' = ""
+            ratingNameDesc: 'typing.Optional[str]' = None
+
+    class Commands:
+        @dataclass
+        class UpdatePIN(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000050F
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="oldPIN", Tag=0, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="newPIN", Tag=1, Type=str),
+                    ])
+
+            oldPIN: 'typing.Optional[str]' = None
+            newPIN: 'str' = ""
+
+        @dataclass
+        class ResetPIN(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000050F
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'ResetPINResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class ResetPINResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000050F
+            command_id: typing.ClassVar[int] = 0x00000002
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="PINCode", Tag=0, Type=str),
+                    ])
+
+            PINCode: 'str' = ""
+
+        @dataclass
+        class Enable(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000050F
+            command_id: typing.ClassVar[int] = 0x00000003
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class Disable(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000050F
+            command_id: typing.ClassVar[int] = 0x00000004
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class AddBonusTime(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000050F
+            command_id: typing.ClassVar[int] = 0x00000005
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="PINCode", Tag=0, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="bonusTime", Tag=1, Type=typing.Optional[uint]),
+                    ])
+
+            PINCode: 'typing.Optional[str]' = None
+            bonusTime: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class SetScreenDailyTime(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000050F
+            command_id: typing.ClassVar[int] = 0x00000006
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="screenTime", Tag=0, Type=uint),
+                    ])
+
+            screenTime: 'uint' = 0
+
+        @dataclass
+        class BlockUnratedContent(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000050F
+            command_id: typing.ClassVar[int] = 0x00000007
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class UnblockUnratedContent(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000050F
+            command_id: typing.ClassVar[int] = 0x00000008
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+        @dataclass
+        class SetOnDemandRatingThreshold(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000050F
+            command_id: typing.ClassVar[int] = 0x00000009
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="rating", Tag=0, Type=str),
+                    ])
+
+            rating: 'str' = ""
+
+        @dataclass
+        class SetScheduledContentRatingThreshold(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x0000050F
+            command_id: typing.ClassVar[int] = 0x0000000A
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="rating", Tag=0, Type=str),
+                    ])
+
+            rating: 'str' = ""
+
+    class Attributes:
+        @dataclass
+        class Enabled(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=bool)
+
+            value: 'bool' = False
+
+        @dataclass
+        class OnDemandRatings(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000001
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[ContentControl.Structs.RatingNameStruct]])
+
+            value: 'typing.Optional[typing.List[ContentControl.Structs.RatingNameStruct]]' = None
+
+        @dataclass
+        class OnDemandRatingThreshold(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000002
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[str])
+
+            value: 'typing.Optional[str]' = None
+
+        @dataclass
+        class ScheduledContentRatings(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000003
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[typing.List[ContentControl.Structs.RatingNameStruct]])
+
+            value: 'typing.Optional[typing.List[ContentControl.Structs.RatingNameStruct]]' = None
+
+        @dataclass
+        class ScheduledContentRatingThreshold(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000004
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[str])
+
+            value: 'typing.Optional[str]' = None
+
+        @dataclass
+        class ScreenDailyTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000005
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class RemainingScreenTime(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000006
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.Optional[uint])
+
+            value: 'typing.Optional[uint]' = None
+
+        @dataclass
+        class BlockUnrated(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x00000007
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=bool)
+
+            value: 'bool' = False
+
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+    class Events:
+        @dataclass
+        class RemainingScreenTimeExpired(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x0000050F
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                    ])
+
+
+@dataclass
+class ContentAppObserver(Cluster):
+    id: typing.ClassVar[int] = 0x00000510
+
+    @ChipUtility.classproperty
+    def descriptor(cls) -> ClusterObjectDescriptor:
+        return ClusterObjectDescriptor(
+            Fields=[
+                ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
+                ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
+                ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+            ])
+
+    generatedCommandList: 'typing.List[uint]' = None
+    acceptedCommandList: 'typing.List[uint]' = None
+    eventList: 'typing.List[uint]' = None
+    attributeList: 'typing.List[uint]' = None
+    featureMap: 'uint' = None
+    clusterRevision: 'uint' = None
+
+    class Enums:
+        class StatusEnum(MatterIntEnum):
+            kSuccess = 0x00
+            kUnexpectedData = 0x01
+            # All received enum values that are not listed above will be mapped
+            # to kUnknownEnumValue. This is a helper enum value that should only
+            # be used by code to process how it handles receiving and unknown
+            # enum value. This specific should never be transmitted.
+            kUnknownEnumValue = 2,
+
+    class Commands:
+        @dataclass
+        class ContentAppMessage(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000510
+            command_id: typing.ClassVar[int] = 0x00000000
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'ContentAppMessageResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="data", Tag=0, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="encodingHint", Tag=1, Type=str),
+                    ])
+
+            data: 'typing.Optional[str]' = None
+            encodingHint: 'str' = ""
+
+        @dataclass
+        class ContentAppMessageResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0x00000510
+            command_id: typing.ClassVar[int] = 0x00000001
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=ContentAppObserver.Enums.StatusEnum),
+                        ClusterObjectFieldDescriptor(Label="data", Tag=1, Type=typing.Optional[str]),
+                        ClusterObjectFieldDescriptor(Label="encodingHint", Tag=2, Type=typing.Optional[str]),
+                    ])
+
+            status: 'ContentAppObserver.Enums.StatusEnum' = 0
+            data: 'typing.Optional[str]' = None
+            encodingHint: 'typing.Optional[str]' = None
+
+    class Attributes:
+        @dataclass
+        class GeneratedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000510
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF8
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AcceptedCommandList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000510
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFF9
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class EventList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000510
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFA
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class AttributeList(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000510
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFB
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=typing.List[uint])
+
+            value: 'typing.List[uint]' = field(default_factory=lambda: [])
+
+        @dataclass
+        class FeatureMap(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000510
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFC
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
+        @dataclass
+        class ClusterRevision(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0x00000510
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0x0000FFFD
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
 
 @dataclass
 class ElectricalMeasurement(Cluster):
     id: typing.ClassVar[int] = 0x00000B04
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
@@ -38168,14 +47180,15 @@
                 ClusterObjectFieldDescriptor(Label="writeOnlyInt8u", Tag=0x0000402A, Type=typing.Optional[uint]),
                 ClusterObjectFieldDescriptor(Label="generatedCommandList", Tag=0x0000FFF8, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="acceptedCommandList", Tag=0x0000FFF9, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="eventList", Tag=0x0000FFFA, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="attributeList", Tag=0x0000FFFB, Type=typing.List[uint]),
                 ClusterObjectFieldDescriptor(Label="featureMap", Tag=0x0000FFFC, Type=uint),
                 ClusterObjectFieldDescriptor(Label="clusterRevision", Tag=0x0000FFFD, Type=uint),
+                ClusterObjectFieldDescriptor(Label="meiInt8u", Tag=0xFFF24F01, Type=uint),
             ])
 
     boolean: 'bool' = None
     bitmap8: 'uint' = None
     bitmap16: 'uint' = None
     bitmap32: 'uint' = None
     bitmap64: 'uint' = None
@@ -38258,14 +47271,15 @@
     writeOnlyInt8u: 'typing.Optional[uint]' = None
     generatedCommandList: 'typing.List[uint]' = None
     acceptedCommandList: 'typing.List[uint]' = None
     eventList: 'typing.List[uint]' = None
     attributeList: 'typing.List[uint]' = None
     featureMap: 'uint' = None
     clusterRevision: 'uint' = None
+    meiInt8u: 'uint' = None
 
     class Enums:
         class SimpleEnum(MatterIntEnum):
             kUnspecified = 0x00
             kValueA = 0x01
             kValueB = 0x02
             kValueC = 0x03
@@ -38921,14 +47935,30 @@
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="arg1", Tag=0, Type=typing.List[UnitTesting.Structs.NestedStructList]),
                     ])
 
             arg1: 'typing.List[UnitTesting.Structs.NestedStructList]' = field(default_factory=lambda: [])
 
         @dataclass
+        class TestBatchHelperResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0xFFF1FC05
+            command_id: typing.ClassVar[int] = 0x0000000C
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="buffer", Tag=0, Type=bytes),
+                    ])
+
+            buffer: 'bytes' = b""
+
+        @dataclass
         class TestListInt8UReverseRequest(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0xFFF1FC05
             command_id: typing.ClassVar[int] = 0x0000000D
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'TestListInt8UReverseResponse'
 
             @ChipUtility.classproperty
@@ -39093,14 +48123,88 @@
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="arg1", Tag=0, Type=uint),
                     ])
 
             arg1: 'uint' = 0
 
+        @dataclass
+        class TestBatchHelperRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0xFFF1FC05
+            command_id: typing.ClassVar[int] = 0x00000016
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'TestBatchHelperResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="sleepBeforeResponseTimeMs", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sizeOfResponseBuffer", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="fillCharacter", Tag=2, Type=uint),
+                    ])
+
+            sleepBeforeResponseTimeMs: 'uint' = 0
+            sizeOfResponseBuffer: 'uint' = 0
+            fillCharacter: 'uint' = 0
+
+        @dataclass
+        class TestSecondBatchHelperRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0xFFF1FC05
+            command_id: typing.ClassVar[int] = 0x00000017
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'TestBatchHelperResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="sleepBeforeResponseTimeMs", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="sizeOfResponseBuffer", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="fillCharacter", Tag=2, Type=uint),
+                    ])
+
+            sleepBeforeResponseTimeMs: 'uint' = 0
+            sizeOfResponseBuffer: 'uint' = 0
+            fillCharacter: 'uint' = 0
+
+        @dataclass
+        class TestDifferentVendorMeiRequest(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0xFFF1FC05
+            command_id: typing.ClassVar[int] = 0xFFF200AA
+            is_client: typing.ClassVar[bool] = True
+            response_type: typing.ClassVar[str] = 'TestDifferentVendorMeiResponse'
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="arg1", Tag=0, Type=uint),
+                    ])
+
+            arg1: 'uint' = 0
+
+        @dataclass
+        class TestDifferentVendorMeiResponse(ClusterCommand):
+            cluster_id: typing.ClassVar[int] = 0xFFF1FC05
+            command_id: typing.ClassVar[int] = 0xFFF200BB
+            is_client: typing.ClassVar[bool] = False
+            response_type: typing.ClassVar[str] = None
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="arg1", Tag=0, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="eventNumber", Tag=1, Type=uint),
+                    ])
+
+            arg1: 'uint' = 0
+            eventNumber: 'uint' = 0
+
     class Attributes:
         @dataclass
         class Boolean(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -40506,14 +49610,30 @@
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
+        @dataclass
+        class MeiInt8u(ClusterAttributeDescriptor):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0xFFF1FC05
+
+            @ChipUtility.classproperty
+            def attribute_id(cls) -> int:
+                return 0xFFF24F01
+
+            @ChipUtility.classproperty
+            def attribute_type(cls) -> ClusterObjectFieldDescriptor:
+                return ClusterObjectFieldDescriptor(Type=uint)
+
+            value: 'uint' = 0
+
     class Events:
         @dataclass
         class TestEvent(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -40555,14 +49675,33 @@
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="fabricIndex", Tag=254, Type=uint),
                     ])
 
             fabricIndex: 'uint' = 0
 
+        @dataclass
+        class TestDifferentVendorMeiEvent(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0xFFF1FC05
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0xFFF200EE
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="arg1", Tag=1, Type=uint),
+                    ])
+
+            arg1: 'uint' = 0
+
 
 @dataclass
 class FaultInjection(Cluster):
     id: typing.ClassVar[int] = 0xFFF1FC06
 
     @ChipUtility.classproperty
     def descriptor(cls) -> ClusterObjectDescriptor:
@@ -40921,7 +50060,29 @@
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=uint)
 
             value: 'uint' = 0
 
+    class Events:
+        @dataclass
+        class PingCountEvent(ClusterEvent):
+            @ChipUtility.classproperty
+            def cluster_id(cls) -> int:
+                return 0xFFF1FC20
+
+            @ChipUtility.classproperty
+            def event_id(cls) -> int:
+                return 0x00000000
+
+            @ChipUtility.classproperty
+            def descriptor(cls) -> ClusterObjectDescriptor:
+                return ClusterObjectDescriptor(
+                    Fields=[
+                        ClusterObjectFieldDescriptor(Label="count", Tag=1, Type=uint),
+                        ClusterObjectFieldDescriptor(Label="fabricIndex", Tag=254, Type=uint),
+                    ])
+
+            count: 'uint' = 0
+            fabricIndex: 'uint' = 0
+
```

## Comparing `home_assistant_chip_clusters-2024.3.2.dist-info/LICENSE` & `home_assistant_chip_clusters-2024.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `home_assistant_chip_clusters-2024.3.2.dist-info/METADATA` & `home_assistant_chip_clusters-2024.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-chip-clusters
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

## Comparing `home_assistant_chip_clusters-2024.3.2.dist-info/RECORD` & `home_assistant_chip_clusters-2024.4.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 chip/ChipUtility.py,sha256=tGBmFf6EX8VjYM32udh3Sm6zq3l5vy5pXfLtLRUvR0o,2188
-chip/clusters/CHIPClusters.py,sha256=h0Lwx8ZYWE6YuGr_ggZaFxfsVm2uYFlw1Hl9IQLuod0,415821
-chip/clusters/ClusterObjects.py,sha256=3GUH2ijOsnO7yGP7SgJ1QfYkN7S_B8_oKPYpS-gt7So,13387
-chip/clusters/Objects.py,sha256=mEejwj_vgbTADS68cvTbPiXbmYsTkaN5JYUJXjLUovI,1666474
+chip/clusters/CHIPClusters.py,sha256=rfp6_0oyayb7AtlU_dbF3Osu0ewpKmoarkyx5Z9ZZas,495958
+chip/clusters/ClusterObjects.py,sha256=zh6HC0GlcDe-sJ7AdyJNCkiBq7LEHeYyHApC3yE1ZXk,14516
+chip/clusters/Objects.py,sha256=oNRMwNiP39PuxkL2jjhc5BdC7dwF2-b47nf2Wd79hHU,2060491
 chip/clusters/TestObjects.py,sha256=aKaE2GnXxixv8S-Q_3LneEII9HWjUQ_ahFtqTXbtaro,1874
 chip/clusters/Types.py,sha256=HlgB-RRP6bXVAFM4xr5ncNtzb-N4aI4c56MMXU9PLmE,1226
 chip/clusters/enum.py,sha256=zw06GH82ONj3CIHKNI4sr7QnBXEr7vBB6zQnYFVAvYg,2404
 chip/tlv/__init__.py,sha256=PjmxvRMbm0imv3TMqtmaUpSmho8lUQpWi-tR8s_mSWc,29245
 chip/tlv/tlvlist.py,sha256=wHI_BMsWAvJZsChbnm9-gsGnQwNmlS5Rh2r1dr_sLf8,5166
-home_assistant_chip_clusters-2024.3.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-home_assistant_chip_clusters-2024.3.2.dist-info/METADATA,sha256=01EsDPwfS-LdR9mUJYTVeh8w9z22td-fKmeY3lEv9Vo,542
-home_assistant_chip_clusters-2024.3.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-home_assistant_chip_clusters-2024.3.2.dist-info/top_level.txt,sha256=5pBsfKK6BMqu66YKYb0-uQqOgrqirLFfcBFAxXDNme0,5
-home_assistant_chip_clusters-2024.3.2.dist-info/RECORD,,
+home_assistant_chip_clusters-2024.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+home_assistant_chip_clusters-2024.4.0.dist-info/METADATA,sha256=Rf8BnbGGndCEMknEPDQ6WnviCc85XQHgo2gj_trsueA,542
+home_assistant_chip_clusters-2024.4.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+home_assistant_chip_clusters-2024.4.0.dist-info/top_level.txt,sha256=5pBsfKK6BMqu66YKYb0-uQqOgrqirLFfcBFAxXDNme0,5
+home_assistant_chip_clusters-2024.4.0.dist-info/RECORD,,
```

