# Comparing `tmp/ondewo-vtsi-client-6.9.0.tar.gz` & `tmp/ondewo-vtsi-client-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-vtsi-client-6.9.0.tar", last modified: Sun Feb 18 17:28:57 2024, max compression
+gzip compressed data, was "ondewo-vtsi-client-7.0.0.tar", last modified: Mon Apr 22 08:32:30 2024, max compression
```

## Comparing `ondewo-vtsi-client-6.9.0.tar` & `ondewo-vtsi-client-7.0.0.tar`

### file list

```diff
@@ -1,80 +1,102 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:28:57.460672 ondewo-vtsi-client-6.9.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9232 2024-02-18 17:28:57.460672 ondewo-vtsi-client-6.9.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8660 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:28:57.448672 ondewo-vtsi-client-6.9.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:28:57.456672 ondewo-vtsi-client-6.9.0/ondewo/nlu/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    45912 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/agent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    96932 2024-02-18 17:27:30.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/agent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    15965 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/aiservices_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16826 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/aiservices_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    11008 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/ccai_project_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    10759 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/ccai_project_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     9190 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/common_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/common_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7334 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/context_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    14789 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/context_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    18752 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/entity_type_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    36069 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/entity_type_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    38409 2024-02-18 17:27:30.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/intent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    59630 2024-02-18 17:27:30.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/intent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3257 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/operation_metadata_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/operation_metadata_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     5374 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/operations_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    11374 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/operations_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     6697 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/project_role_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    10478 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/project_role_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     5878 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/project_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16562 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/project_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     2661 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/server_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6634 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/server_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    50420 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/session_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    77168 2024-02-18 17:27:30.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/session_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    16012 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/user_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    41424 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/user_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    10951 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/utility_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16902 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/utility_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7472 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/webhook_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    13238 2024-02-18 17:27:30.000000 ondewo-vtsi-client-6.9.0/ondewo/nlu/webhook_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:28:57.456672 ondewo-vtsi-client-6.9.0/ondewo/qa/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/qa/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6672 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/qa/qa_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    13335 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/qa/qa_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:28:57.456672 ondewo-vtsi-client-6.9.0/ondewo/s2t/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/s2t/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18471 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/s2t/speech_to_text_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    30933 2024-02-18 17:27:30.000000 ondewo-vtsi-client-6.9.0/ondewo/s2t/speech_to_text_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:28:57.456672 ondewo-vtsi-client-6.9.0/ondewo/sip/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/sip/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6807 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/sip/sip_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    21323 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/sip/sip_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:28:57.456672 ondewo-vtsi-client-6.9.0/ondewo/t2s/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/t2s/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16353 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/t2s/text_to_speech_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    33508 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/t2s/text_to_speech_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:28:57.460672 ondewo-vtsi-client-6.9.0/ondewo/vtsi/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    29297 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/calls_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    46320 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/calls_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:28:57.460672 ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      735 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      263 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:28:57.460672 ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13931 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/services/calls.py
--rw-rw-r--   0 root         (0) root         (0)     5017 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/services/projects.py
--rw-rw-r--   0 root         (0) root         (0)      317 2024-02-18 17:25:48.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)     9600 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/projects_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    14451 2024-02-18 17:27:29.000000 ondewo-vtsi-client-6.9.0/ondewo/vtsi/projects_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:28:57.460672 ondewo-vtsi-client-6.9.0/ondewo_vtsi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9232 2024-02-18 17:28:57.000000 ondewo-vtsi-client-6.9.0/ondewo_vtsi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2022 2024-02-18 17:28:57.000000 ondewo-vtsi-client-6.9.0/ondewo_vtsi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-18 17:28:57.000000 ondewo-vtsi-client-6.9.0/ondewo_vtsi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      211 2024-02-18 17:28:57.000000 ondewo-vtsi-client-6.9.0/ondewo_vtsi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-18 17:28:57.000000 ondewo-vtsi-client-6.9.0/ondewo_vtsi_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2024-02-18 17:28:57.464672 ondewo-vtsi-client-6.9.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1586 2024-02-18 17:27:33.000000 ondewo-vtsi-client-6.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:32:30.788698 ondewo-vtsi-client-7.0.0/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9213 2024-04-22 08:32:30.788698 ondewo-vtsi-client-7.0.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8660 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:32:30.780698 ondewo-vtsi-client-7.0.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:32:30.784698 ondewo-vtsi-client-7.0.0/ondewo/nlu/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    45912 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/agent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)   132652 2024-04-22 08:31:50.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/agent_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    96932 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/agent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    15965 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/aiservices_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    47091 2024-04-22 08:31:51.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/aiservices_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    16826 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/aiservices_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    11008 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/ccai_project_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    37825 2024-04-22 08:31:52.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/ccai_project_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    10759 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/ccai_project_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     9190 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/common_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    34360 2024-04-22 08:31:52.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/common_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)      158 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/common_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7334 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/context_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    15351 2024-04-22 08:31:53.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/context_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    14789 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/context_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    18752 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/entity_type_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    52119 2024-04-22 08:31:52.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/entity_type_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    36069 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/entity_type_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    38409 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/intent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)   139324 2024-04-22 08:31:53.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/intent_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    59630 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/intent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3257 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/operation_metadata_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    11856 2024-04-22 08:31:52.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/operation_metadata_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)      158 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/operation_metadata_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     5374 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/operations_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    12728 2024-04-22 08:31:51.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/operations_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    11374 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/operations_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     6697 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/project_role_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    15861 2024-04-22 08:31:53.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/project_role_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    10478 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/project_role_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     5878 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/project_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     4615 2024-04-22 08:31:51.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/project_statistics_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    16562 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/project_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     2661 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/server_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1475 2024-04-22 08:31:51.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/server_statistics_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)     6634 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/server_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    50420 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/session_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)   168081 2024-04-22 08:31:54.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/session_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    77168 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/session_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    16012 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/user_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    38377 2024-04-22 08:31:50.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/user_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    41424 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/user_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    10951 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/utility_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    39586 2024-04-22 08:31:53.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/utility_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    16902 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/utility_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7472 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/webhook_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    25116 2024-04-22 08:31:51.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/webhook_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    13238 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/nlu/webhook_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:32:30.784698 ondewo-vtsi-client-7.0.0/ondewo/qa/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/qa/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6672 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/qa/qa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    13131 2024-04-22 08:31:54.000000 ondewo-vtsi-client-7.0.0/ondewo/qa/qa_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    13335 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/qa/qa_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:32:30.784698 ondewo-vtsi-client-7.0.0/ondewo/s2t/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/s2t/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    18471 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/s2t/speech_to_text_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    66224 2024-04-22 08:31:55.000000 ondewo-vtsi-client-7.0.0/ondewo/s2t/speech_to_text_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    30933 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/s2t/speech_to_text_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:32:30.784698 ondewo-vtsi-client-7.0.0/ondewo/sip/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/sip/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6807 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/sip/sip_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    17711 2024-04-22 08:31:57.000000 ondewo-vtsi-client-7.0.0/ondewo/sip/sip_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    21323 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/sip/sip_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:32:30.788698 ondewo-vtsi-client-7.0.0/ondewo/t2s/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/t2s/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16353 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/t2s/text_to_speech_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    60257 2024-04-22 08:31:56.000000 ondewo-vtsi-client-7.0.0/ondewo/t2s/text_to_speech_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    33508 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/t2s/text_to_speech_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:32:30.788698 ondewo-vtsi-client-7.0.0/ondewo/vtsi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    29297 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/calls_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)   103602 2024-04-22 08:31:58.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/calls_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    46320 2024-04-22 08:32:12.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/calls_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:32:30.788698 ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      735 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      263 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:32:30.788698 ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13931 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/services/calls.py
+-rw-rw-r--   0 root         (0) root         (0)     5017 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/services/projects.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2024-04-22 08:31:22.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)     9600 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/projects_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    32649 2024-04-22 08:31:58.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/projects_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    14451 2024-04-22 08:32:11.000000 ondewo-vtsi-client-7.0.0/ondewo/vtsi/projects_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 08:32:30.788698 ondewo-vtsi-client-7.0.0/ondewo_vtsi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9213 2024-04-22 08:32:30.000000 ondewo-vtsi-client-7.0.0/ondewo_vtsi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2666 2024-04-22 08:32:30.000000 ondewo-vtsi-client-7.0.0/ondewo_vtsi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 08:32:30.000000 ondewo-vtsi-client-7.0.0/ondewo_vtsi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-22 08:32:30.000000 ondewo-vtsi-client-7.0.0/ondewo_vtsi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-22 08:32:30.000000 ondewo-vtsi-client-7.0.0/ondewo_vtsi_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2024-04-22 08:32:30.788698 ondewo-vtsi-client-7.0.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1617 2024-04-22 08:32:15.000000 ondewo-vtsi-client-7.0.0/setup.py
```

### Comparing `ondewo-vtsi-client-6.9.0/LICENSE` & `ondewo-vtsi-client-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/PKG-INFO` & `ondewo-vtsi-client-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.9.0
-Summary: exposes the ondewo-vtsi endpoints in a user-friendly way
+Version: 7.0.0
+Summary: ONDEWO Voip Telephone System Integration (VTSI) Client library for Python
 Home-page: https://github.com/ondewo/ondewo-vtsi-client-python
-Author: Ondewo GbmH
+Author: ONDEWO GmbH
 Author-email: office@ondewo.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -234,9 +232,7 @@
 2. `commit and push` all changes in code resulting from the `build`
 3. Create and push the `release branch` e.g. `release/1.3.20`
 4. Create and push the `release tag` e.g. `1.3.20`
 5. Create a new `Release` on GitHub
 6. Publish the built `dist` folder to `pypi.org`
 
 > :warning: The Release Automation checks if the build has created all the proto-code files, but it does not check the code-integrity. Please build and test the generated code prior to starting the release process.
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.9.0 Summary: exposes
-the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
-ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
-office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
-Software Development :: Libraries Requires-Python: >=3 Description-Content-
-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 7.0.0 Summary: ONDEWO
+Voip Telephone System Integration (VTSI) Client library for Python Home-page:
+https://github.com/ondewo/ondewo-vtsi-client-python Author: ONDEWO GmbH Author-
+email: office@ondewo.com Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent Classifier: Development Status
+:: 5 - Production/Stable Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
+LICENSE
  _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_o_n_d_e_w_o_/_o_n_d_e_w_o_-_l_o_g_o_s_/_m_a_s_t_e_r_/
  _o_n_d_e_w_o___w_e___a_u_t_o_m_a_t_e___y_o_u_r___p_h_o_n_e___c_a_l_l_s_._p_n_g_]
  _[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_3_5_3_6_/_3_5_3_6_5_0_5_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-
  _p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_7_3_3_/_7_3_3_5_4_7_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/
     _7_3_3_/_7_3_3_5_7_9_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_1_7_4_/_1_7_4_8_5_5_._p_n_g_]
                 ************ OOnnddeewwoo VVTTSSII CClliieenntt PPyytthhoonn LLiibbrraarryy ************
 This library facilitates the interaction between a user and a CAI server. It
```

### Comparing `ondewo-vtsi-client-6.9.0/README.md` & `ondewo-vtsi-client-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/agent_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/agent_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/aiservices_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/aiservices_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/aiservices_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/aiservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/ccai_project_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/ccai_project_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/ccai_project_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/ccai_project_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/common_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/context_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/context_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/context_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/context_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/entity_type_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/entity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/entity_type_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/entity_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/intent_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/intent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/intent_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/intent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/operation_metadata_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/operation_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/operations_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/operations_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/project_role_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/project_role_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/project_role_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/project_role_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/project_statistics_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/project_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/project_statistics_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/project_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/server_statistics_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/server_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/server_statistics_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/server_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/session_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/session_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/session_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/user_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/user_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/user_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/utility_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/utility_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/utility_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/utility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/webhook_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/webhook_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/nlu/webhook_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/nlu/webhook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/qa/qa_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/qa/qa_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/qa/qa_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/qa/qa_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/s2t/speech_to_text_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/s2t/speech_to_text_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/s2t/speech_to_text_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/s2t/speech_to_text_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/sip/sip_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/sip/sip_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/sip/sip_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/sip/sip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/t2s/text_to_speech_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/t2s/text_to_speech_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/t2s/text_to_speech_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/t2s/text_to_speech_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/vtsi/calls_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/vtsi/calls_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/vtsi/calls_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/vtsi/calls_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/client.py` & `ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/services/calls.py` & `ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/services/calls.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/vtsi/client/services/projects.py` & `ondewo-vtsi-client-7.0.0/ondewo/vtsi/client/services/projects.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/vtsi/projects_pb2.py` & `ondewo-vtsi-client-7.0.0/ondewo/vtsi/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo/vtsi/projects_pb2_grpc.py` & `ondewo-vtsi-client-7.0.0/ondewo/vtsi/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.9.0/ondewo_vtsi_client.egg-info/PKG-INFO` & `ondewo-vtsi-client-7.0.0/ondewo_vtsi_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.9.0
-Summary: exposes the ondewo-vtsi endpoints in a user-friendly way
+Version: 7.0.0
+Summary: ONDEWO Voip Telephone System Integration (VTSI) Client library for Python
 Home-page: https://github.com/ondewo/ondewo-vtsi-client-python
-Author: Ondewo GbmH
+Author: ONDEWO GmbH
 Author-email: office@ondewo.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -234,9 +232,7 @@
 2. `commit and push` all changes in code resulting from the `build`
 3. Create and push the `release branch` e.g. `release/1.3.20`
 4. Create and push the `release tag` e.g. `1.3.20`
 5. Create a new `Release` on GitHub
 6. Publish the built `dist` folder to `pypi.org`
 
 > :warning: The Release Automation checks if the build has created all the proto-code files, but it does not check the code-integrity. Please build and test the generated code prior to starting the release process.
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.9.0 Summary: exposes
-the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
-ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
-office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
-Software Development :: Libraries Requires-Python: >=3 Description-Content-
-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 7.0.0 Summary: ONDEWO
+Voip Telephone System Integration (VTSI) Client library for Python Home-page:
+https://github.com/ondewo/ondewo-vtsi-client-python Author: ONDEWO GmbH Author-
+email: office@ondewo.com Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent Classifier: Development Status
+:: 5 - Production/Stable Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
+LICENSE
  _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_o_n_d_e_w_o_/_o_n_d_e_w_o_-_l_o_g_o_s_/_m_a_s_t_e_r_/
  _o_n_d_e_w_o___w_e___a_u_t_o_m_a_t_e___y_o_u_r___p_h_o_n_e___c_a_l_l_s_._p_n_g_]
  _[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_3_5_3_6_/_3_5_3_6_5_0_5_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-
  _p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_7_3_3_/_7_3_3_5_4_7_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/
     _7_3_3_/_7_3_3_5_7_9_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_1_7_4_/_1_7_4_8_5_5_._p_n_g_]
                 ************ OOnnddeewwoo VVTTSSII CClliieenntt PPyytthhoonn LLiibbrraarryy ************
 This library facilitates the interaction between a user and a CAI server. It
```

### Comparing `ondewo-vtsi-client-6.9.0/ondewo_vtsi_client.egg-info/SOURCES.txt` & `ondewo-vtsi-client-7.0.0/ondewo_vtsi_client.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,61 +2,83 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 ondewo/__init__.py
 ondewo/nlu/__init__.py
 ondewo/nlu/agent_pb2.py
+ondewo/nlu/agent_pb2.pyi
 ondewo/nlu/agent_pb2_grpc.py
 ondewo/nlu/aiservices_pb2.py
+ondewo/nlu/aiservices_pb2.pyi
 ondewo/nlu/aiservices_pb2_grpc.py
 ondewo/nlu/ccai_project_pb2.py
+ondewo/nlu/ccai_project_pb2.pyi
 ondewo/nlu/ccai_project_pb2_grpc.py
 ondewo/nlu/common_pb2.py
+ondewo/nlu/common_pb2.pyi
 ondewo/nlu/common_pb2_grpc.py
 ondewo/nlu/context_pb2.py
+ondewo/nlu/context_pb2.pyi
 ondewo/nlu/context_pb2_grpc.py
 ondewo/nlu/entity_type_pb2.py
+ondewo/nlu/entity_type_pb2.pyi
 ondewo/nlu/entity_type_pb2_grpc.py
 ondewo/nlu/intent_pb2.py
+ondewo/nlu/intent_pb2.pyi
 ondewo/nlu/intent_pb2_grpc.py
 ondewo/nlu/operation_metadata_pb2.py
+ondewo/nlu/operation_metadata_pb2.pyi
 ondewo/nlu/operation_metadata_pb2_grpc.py
 ondewo/nlu/operations_pb2.py
+ondewo/nlu/operations_pb2.pyi
 ondewo/nlu/operations_pb2_grpc.py
 ondewo/nlu/project_role_pb2.py
+ondewo/nlu/project_role_pb2.pyi
 ondewo/nlu/project_role_pb2_grpc.py
 ondewo/nlu/project_statistics_pb2.py
+ondewo/nlu/project_statistics_pb2.pyi
 ondewo/nlu/project_statistics_pb2_grpc.py
 ondewo/nlu/server_statistics_pb2.py
+ondewo/nlu/server_statistics_pb2.pyi
 ondewo/nlu/server_statistics_pb2_grpc.py
 ondewo/nlu/session_pb2.py
+ondewo/nlu/session_pb2.pyi
 ondewo/nlu/session_pb2_grpc.py
 ondewo/nlu/user_pb2.py
+ondewo/nlu/user_pb2.pyi
 ondewo/nlu/user_pb2_grpc.py
 ondewo/nlu/utility_pb2.py
+ondewo/nlu/utility_pb2.pyi
 ondewo/nlu/utility_pb2_grpc.py
 ondewo/nlu/webhook_pb2.py
+ondewo/nlu/webhook_pb2.pyi
 ondewo/nlu/webhook_pb2_grpc.py
 ondewo/qa/__init__.py
 ondewo/qa/qa_pb2.py
+ondewo/qa/qa_pb2.pyi
 ondewo/qa/qa_pb2_grpc.py
 ondewo/s2t/__init__.py
 ondewo/s2t/speech_to_text_pb2.py
+ondewo/s2t/speech_to_text_pb2.pyi
 ondewo/s2t/speech_to_text_pb2_grpc.py
 ondewo/sip/__init__.py
 ondewo/sip/sip_pb2.py
+ondewo/sip/sip_pb2.pyi
 ondewo/sip/sip_pb2_grpc.py
 ondewo/t2s/__init__.py
 ondewo/t2s/text_to_speech_pb2.py
+ondewo/t2s/text_to_speech_pb2.pyi
 ondewo/t2s/text_to_speech_pb2_grpc.py
 ondewo/vtsi/__init__.py
 ondewo/vtsi/calls_pb2.py
+ondewo/vtsi/calls_pb2.pyi
 ondewo/vtsi/calls_pb2_grpc.py
 ondewo/vtsi/projects_pb2.py
+ondewo/vtsi/projects_pb2.pyi
 ondewo/vtsi/projects_pb2_grpc.py
 ondewo/vtsi/client/__init__.py
 ondewo/vtsi/client/client.py
 ondewo/vtsi/client/client_config.py
 ondewo/vtsi/client/services_container.py
 ondewo/vtsi/client/services/__init__.py
 ondewo/vtsi/client/services/calls.py
```

### Comparing `ondewo-vtsi-client-6.9.0/setup.py` & `ondewo-vtsi-client-7.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from setuptools import setup, find_packages
+from setuptools import (
+    find_packages,
+    setup,
+)
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 with open("requirements.txt") as f:
     requires = []
     for line in f:
@@ -12,18 +15,18 @@
             req_str = f"{req_name} @ {req_url}"
         else:
             req_str = req
         requires.append(req_str)
 
 setup(
     name="ondewo-vtsi-client",
-    version='6.9.0',
-    author="Ondewo GbmH",
+    version='7.0.0',
+    author="ONDEWO GmbH",
     author_email="office@ondewo.com",
-    description="exposes the ondewo-vtsi endpoints in a user-friendly way",
+    description="ONDEWO Voip Telephone System Integration (VTSI) Client library for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ondewo/ondewo-vtsi-client-python",
     packages=[
         np
         for np in filter(
             lambda n: n.startswith('ondewo.') or n == 'ondewo',
@@ -37,15 +40,15 @@
         'ondewo.qa': ['py.typed', '*.pyi'],
         'ondewo.s2t': ['py.typed', '*.pyi'],
         'ondewo.t2s': ['py.typed', '*.pyi'],
         'ondewo.csi': ['py.typed', '*.pyi'],
         'ondewo.sip': ['py.typed', '*.pyi'],
     },
     classifiers=[
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.10',
         'Operating System :: OS Independent',
         'Development Status :: 5 - Production/Stable',
         'Topic :: Software Development :: Libraries',
     ],
     python_requires='>=3',
     install_requires=requires,
 )
```

