# Comparing `tmp/oss-client-0.1.4.tar.gz` & `tmp/oss-client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oss-client-0.1.4.tar", last modified: Mon Feb 28 07:48:06 2022, max compression
+gzip compressed data, was "oss-client-0.1.5.tar", last modified: Mon Apr 22 04:45:23 2024, max compression
```

## Comparing `oss-client-0.1.4.tar` & `oss-client-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 gaojian   (1000) gaojian   (1000)        0 2022-02-28 07:48:06.000000 oss-client-0.1.4/
--rwxrwxrwx   0 gaojian   (1000) gaojian   (1000)     1069 2021-11-03 06:39:28.000000 oss-client-0.1.4/LICENSE
--rwxrwxrwx   0 gaojian   (1000) gaojian   (1000)       58 2021-11-03 06:39:43.000000 oss-client-0.1.4/MANIFEST.in
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)      711 2022-02-28 07:48:06.000000 oss-client-0.1.4/PKG-INFO
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)      400 2021-11-03 06:53:03.000000 oss-client-0.1.4/README.md
-drwxrwxrwx   0 gaojian   (1000) gaojian   (1000)        0 2022-02-28 07:48:06.000000 oss-client-0.1.4/oss_client/
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)      146 2021-11-03 07:16:11.000000 oss-client-0.1.4/oss_client/__init__.py
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)     3960 2022-02-28 07:43:21.000000 oss-client-0.1.4/oss_client/client.py
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)     1140 2022-02-28 05:47:14.000000 oss-client-0.1.4/oss_client/fileobj.py
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)      111 2021-11-03 03:41:43.000000 oss-client-0.1.4/oss_client/utils.py
-drwxrwxrwx   0 gaojian   (1000) gaojian   (1000)        0 2022-02-28 07:48:06.000000 oss-client-0.1.4/oss_client.egg-info/
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)      711 2022-02-28 07:48:06.000000 oss-client-0.1.4/oss_client.egg-info/PKG-INFO
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)      303 2022-02-28 07:48:06.000000 oss-client-0.1.4/oss_client.egg-info/SOURCES.txt
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)        1 2022-02-28 07:48:06.000000 oss-client-0.1.4/oss_client.egg-info/dependency_links.txt
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)       69 2022-02-28 07:48:06.000000 oss-client-0.1.4/oss_client.egg-info/requires.txt
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)       11 2022-02-28 07:48:06.000000 oss-client-0.1.4/oss_client.egg-info/top_level.txt
--rwxrwxrwx   0 gaojian   (1000) gaojian   (1000)       73 2022-02-28 07:48:06.000000 oss-client-0.1.4/setup.cfg
--rw-rw-rw-   0 gaojian   (1000) gaojian   (1000)      748 2022-02-28 07:45:10.000000 oss-client-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 04:45:23.654399 oss-client-0.1.5/
+-rw-rw-rw-   0        0        0     1090 2024-04-22 04:35:28.000000 oss-client-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       61 2024-04-22 04:35:28.000000 oss-client-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      761 2024-04-22 04:45:23.654399 oss-client-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2024-04-22 04:35:28.000000 oss-client-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 04:45:23.627706 oss-client-0.1.5/oss_client/
+-rw-rw-rw-   0        0        0      155 2024-04-22 04:35:28.000000 oss-client-0.1.5/oss_client/__init__.py
+-rw-rw-rw-   0        0        0     4114 2024-04-22 04:35:28.000000 oss-client-0.1.5/oss_client/client.py
+-rw-rw-rw-   0        0        0     1500 2024-04-22 04:43:27.000000 oss-client-0.1.5/oss_client/fileobj.py
+-rw-rw-rw-   0        0        0      117 2024-04-22 04:35:28.000000 oss-client-0.1.5/oss_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 04:45:23.651803 oss-client-0.1.5/oss_client.egg-info/
+-rw-rw-rw-   0        0        0      761 2024-04-22 04:45:23.000000 oss-client-0.1.5/oss_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-04-22 04:45:23.000000 oss-client-0.1.5/oss_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 04:45:23.000000 oss-client-0.1.5/oss_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-22 04:45:23.000000 oss-client-0.1.5/oss_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-22 04:45:23.000000 oss-client-0.1.5/oss_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2024-04-22 04:45:23.656619 oss-client-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      777 2024-04-22 04:43:33.000000 oss-client-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `oss-client-0.1.4/PKG-INFO` & `oss-client-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1
-Name: oss-client
-Version: 0.1.4
-Summary: OSS Client for AliyunOSS/TencentOSS/QiniuOSS
-Home-page: https://github.com/olivetree123/oss-client
-Author: olivetree
-Author-email: olivetree123@163.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# oss-client
-集成了阿里云OSS、腾讯云对象存储和七牛云对象存储，为不同的对象存储实现了统一的Client，方便使用
-
-## Install
-> pip install oss-client
-
-
-## Tutorial
-```
-from oss_client import AliyunClient
-
-client = AliyunClient(
-    access_key=ALY_ACCESS_KEY_ID,
-    secret_key=ALY_ACCESS_KEY_SECRET,
-    endpoint=ALY_OSS_ENDPOINT,
-    bucket=ALY_OSS_BUCKET,
-)
-```
-
-
+Metadata-Version: 2.1
+Name: oss-client
+Version: 0.1.5
+Summary: OSS Client for AliyunOSS/TencentOSS/QiniuOSS
+Home-page: https://github.com/olivetree123/oss-client
+Author: olivetree
+Author-email: olivetree123@163.com
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# oss-client
+集成了阿里云OSS、腾讯云对象存储和七牛云对象存储，为不同的对象存储实现了统一的Client，方便使用
+
+## Install
+> pip install oss-client
+
+
+## Tutorial
+```
+from oss_client import AliyunClient
+
+client = AliyunClient(
+    access_key=ALY_ACCESS_KEY_ID,
+    secret_key=ALY_ACCESS_KEY_SECRET,
+    endpoint=ALY_OSS_ENDPOINT,
+    bucket=ALY_OSS_BUCKET,
+)
+```
+
+
```

### Comparing `oss-client-0.1.4/oss_client.egg-info/PKG-INFO` & `oss-client-0.1.5/oss_client.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1
-Name: oss-client
-Version: 0.1.4
-Summary: OSS Client for AliyunOSS/TencentOSS/QiniuOSS
-Home-page: https://github.com/olivetree123/oss-client
-Author: olivetree
-Author-email: olivetree123@163.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# oss-client
-集成了阿里云OSS、腾讯云对象存储和七牛云对象存储，为不同的对象存储实现了统一的Client，方便使用
-
-## Install
-> pip install oss-client
-
-
-## Tutorial
-```
-from oss_client import AliyunClient
-
-client = AliyunClient(
-    access_key=ALY_ACCESS_KEY_ID,
-    secret_key=ALY_ACCESS_KEY_SECRET,
-    endpoint=ALY_OSS_ENDPOINT,
-    bucket=ALY_OSS_BUCKET,
-)
-```
-
-
+Metadata-Version: 2.1
+Name: oss-client
+Version: 0.1.5
+Summary: OSS Client for AliyunOSS/TencentOSS/QiniuOSS
+Home-page: https://github.com/olivetree123/oss-client
+Author: olivetree
+Author-email: olivetree123@163.com
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# oss-client
+集成了阿里云OSS、腾讯云对象存储和七牛云对象存储，为不同的对象存储实现了统一的Client，方便使用
+
+## Install
+> pip install oss-client
+
+
+## Tutorial
+```
+from oss_client import AliyunClient
+
+client = AliyunClient(
+    access_key=ALY_ACCESS_KEY_ID,
+    secret_key=ALY_ACCESS_KEY_SECRET,
+    endpoint=ALY_OSS_ENDPOINT,
+    bucket=ALY_OSS_BUCKET,
+)
+```
+
+
```

