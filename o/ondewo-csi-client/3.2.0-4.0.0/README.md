# Comparing `tmp/ondewo-csi-client-3.2.0.tar.gz` & `tmp/ondewo-csi-client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-csi-client-3.2.0.tar", last modified: Sun May 21 18:24:11 2023, max compression
+gzip compressed data, was "ondewo-csi-client-4.0.0.tar", last modified: Mon Apr 22 05:51:51 2024, max compression
```

## Comparing `ondewo-csi-client-3.2.0.tar` & `ondewo-csi-client-4.0.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.726235 ondewo-csi-client-3.2.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7365 2023-05-21 18:24:11.726235 ondewo-csi-client-3.2.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6526 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.725235 ondewo-csi-client-3.2.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.725235 ondewo-csi-client-3.2.0/ondewo/csi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.725235 ondewo-csi-client-3.2.0/ondewo/csi/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1370 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      872 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.725235 ondewo-csi-client-3.2.0/ondewo/csi/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3151 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/services/conversations.py
--rw-rw-r--   0 root         (0) root         (0)      879 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    16188 2023-05-21 18:22:50.000000 ondewo-csi-client-3.2.0/ondewo/csi/conversation_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    19025 2023-05-21 18:22:50.000000 ondewo-csi-client-3.2.0/ondewo/csi/conversation_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.726235 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7365 2023-05-21 18:24:11.000000 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      577 2023-05-21 18:24:11.000000 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 18:24:11.000000 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-21 18:24:11.000000 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-21 18:24:11.000000 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2023-05-21 18:24:11.726235 ondewo-csi-client-3.2.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1902 2023-05-21 18:22:54.000000 ondewo-csi-client-3.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:51:51.321594 ondewo-csi-client-4.0.0/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2024-04-22 05:50:34.000000 ondewo-csi-client-4.0.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2024-04-22 05:50:34.000000 ondewo-csi-client-4.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7328 2024-04-22 05:51:51.321594 ondewo-csi-client-4.0.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6526 2024-04-22 05:50:34.000000 ondewo-csi-client-4.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:51:51.321594 ondewo-csi-client-4.0.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2024-04-22 05:50:34.000000 ondewo-csi-client-4.0.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:51:51.321594 ondewo-csi-client-4.0.0/ondewo/csi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-22 05:50:34.000000 ondewo-csi-client-4.0.0/ondewo/csi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:51:51.321594 ondewo-csi-client-4.0.0/ondewo/csi/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-22 05:50:34.000000 ondewo-csi-client-4.0.0/ondewo/csi/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1370 2024-04-22 05:50:34.000000 ondewo-csi-client-4.0.0/ondewo/csi/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      872 2024-04-22 05:50:34.000000 ondewo-csi-client-4.0.0/ondewo/csi/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:51:51.321594 ondewo-csi-client-4.0.0/ondewo/csi/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-22 05:50:34.000000 ondewo-csi-client-4.0.0/ondewo/csi/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3151 2024-04-22 05:50:34.000000 ondewo-csi-client-4.0.0/ondewo/csi/client/services/conversations.py
+-rw-rw-r--   0 root         (0) root         (0)      879 2024-04-22 05:50:34.000000 ondewo-csi-client-4.0.0/ondewo/csi/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    16188 2024-04-22 05:50:51.000000 ondewo-csi-client-4.0.0/ondewo/csi/conversation_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    52463 2024-04-22 05:50:51.000000 ondewo-csi-client-4.0.0/ondewo/csi/conversation_pb2.pyi
+-rw-rw-r--   0 root         (0) root         (0)    19025 2024-04-22 05:50:51.000000 ondewo-csi-client-4.0.0/ondewo/csi/conversation_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 05:51:51.321594 ondewo-csi-client-4.0.0/ondewo_csi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7328 2024-04-22 05:51:51.000000 ondewo-csi-client-4.0.0/ondewo_csi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      609 2024-04-22 05:51:51.000000 ondewo-csi-client-4.0.0/ondewo_csi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 05:51:51.000000 ondewo-csi-client-4.0.0/ondewo_csi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      202 2024-04-22 05:51:51.000000 ondewo-csi-client-4.0.0/ondewo_csi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-22 05:51:51.000000 ondewo-csi-client-4.0.0/ondewo_csi_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2024-04-22 05:51:51.321594 ondewo-csi-client-4.0.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1902 2024-04-22 05:50:56.000000 ondewo-csi-client-4.0.0/setup.py
```

### Comparing `ondewo-csi-client-3.2.0/LICENSE` & `ondewo-csi-client-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.2.0/PKG-INFO` & `ondewo-csi-client-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: ondewo-csi-client
-Version: 3.2.0
+Version: 4.0.0
 Summary: Provides endpoints and messages for gRPC communication to the ONDEWO CSI server
 Home-page: https://github.com/ondewo/ondewo-csi-client-python
 Author: ONDEWO GbmH
 Author-email: office@ondewo.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -184,9 +182,7 @@
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
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: ondewo-csi-client Version: 3.2.0 Summary: Provides
+Metadata-Version: 2.1 Name: ondewo-csi-client Version: 4.0.0 Summary: Provides
 endpoints and messages for gRPC communication to the ONDEWO CSI server Home-
 page: https://github.com/ondewo/ondewo-csi-client-python Author: ONDEWO GbmH
-Author-email: office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Operating System :: OS Independent Requires-Python:
->=3 Description-Content-Type: text/markdown License-File: LICENSE
+Author-email: office@ondewo.com Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers Classifier: Topic :: Software
+Development :: Libraries Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Operating System :: OS Independent Requires-Python: >=3 Description-Content-
+Type: text/markdown License-File: LICENSE
  _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_o_n_d_e_w_o_/_o_n_d_e_w_o_-_l_o_g_o_s_/_m_a_s_t_e_r_/
  _o_n_d_e_w_o___w_e___a_u_t_o_m_a_t_e___y_o_u_r___p_h_o_n_e___c_a_l_l_s_._p_n_g_]
  _[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_3_5_3_6_/_3_5_3_6_5_0_5_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-
  _p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_7_3_3_/_7_3_3_5_4_7_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/
     _7_3_3_/_7_3_3_5_7_9_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_1_7_4_/_1_7_4_8_5_5_._p_n_g_]
                 ************ OOnnddeewwoo CCSSII CClliieenntt PPyytthhoonn LLiibbrraarryy ************
 This library facilitates the interaction between a user and a CAI server. It
```

### Comparing `ondewo-csi-client-3.2.0/README.md` & `ondewo-csi-client-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.2.0/ondewo/csi/client/client.py` & `ondewo-csi-client-4.0.0/ondewo/csi/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.2.0/ondewo/csi/client/client_config.py` & `ondewo-csi-client-4.0.0/ondewo/csi/client/client_config.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.2.0/ondewo/csi/client/services/conversations.py` & `ondewo-csi-client-4.0.0/ondewo/csi/client/services/conversations.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.2.0/ondewo/csi/client/services_container.py` & `ondewo-csi-client-4.0.0/ondewo/csi/client/services_container.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.2.0/ondewo/csi/conversation_pb2.py` & `ondewo-csi-client-4.0.0/ondewo/csi/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.2.0/ondewo/csi/conversation_pb2_grpc.py` & `ondewo-csi-client-4.0.0/ondewo/csi/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/PKG-INFO` & `ondewo-csi-client-4.0.0/ondewo_csi_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: ondewo-csi-client
-Version: 3.2.0
+Version: 4.0.0
 Summary: Provides endpoints and messages for gRPC communication to the ONDEWO CSI server
 Home-page: https://github.com/ondewo/ondewo-csi-client-python
 Author: ONDEWO GbmH
 Author-email: office@ondewo.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -184,9 +182,7 @@
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
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: ondewo-csi-client Version: 3.2.0 Summary: Provides
+Metadata-Version: 2.1 Name: ondewo-csi-client Version: 4.0.0 Summary: Provides
 endpoints and messages for gRPC communication to the ONDEWO CSI server Home-
 page: https://github.com/ondewo/ondewo-csi-client-python Author: ONDEWO GbmH
-Author-email: office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Operating System :: OS Independent Requires-Python:
->=3 Description-Content-Type: text/markdown License-File: LICENSE
+Author-email: office@ondewo.com Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers Classifier: Topic :: Software
+Development :: Libraries Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Operating System :: OS Independent Requires-Python: >=3 Description-Content-
+Type: text/markdown License-File: LICENSE
  _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_o_n_d_e_w_o_/_o_n_d_e_w_o_-_l_o_g_o_s_/_m_a_s_t_e_r_/
  _o_n_d_e_w_o___w_e___a_u_t_o_m_a_t_e___y_o_u_r___p_h_o_n_e___c_a_l_l_s_._p_n_g_]
  _[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_3_5_3_6_/_3_5_3_6_5_0_5_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-
  _p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_7_3_3_/_7_3_3_5_4_7_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/
     _7_3_3_/_7_3_3_5_7_9_._p_n_g_]_[_h_t_t_p_s_:_/_/_c_d_n_-_i_c_o_n_s_-_p_n_g_._f_l_a_t_i_c_o_n_._c_o_m_/_5_1_2_/_1_7_4_/_1_7_4_8_5_5_._p_n_g_]
                 ************ OOnnddeewwoo CCSSII CClliieenntt PPyytthhoonn LLiibbrraarryy ************
 This library facilitates the interaction between a user and a CAI server. It
```

### Comparing `ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/SOURCES.txt` & `ondewo-csi-client-4.0.0/ondewo_csi_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 ondewo/__init__.py
 ondewo/csi/__init__.py
 ondewo/csi/conversation_pb2.py
+ondewo/csi/conversation_pb2.pyi
 ondewo/csi/conversation_pb2_grpc.py
 ondewo/csi/client/__init__.py
 ondewo/csi/client/client.py
 ondewo/csi/client/client_config.py
 ondewo/csi/client/services_container.py
 ondewo/csi/client/services/__init__.py
 ondewo/csi/client/services/conversations.py
```

### Comparing `ondewo-csi-client-3.2.0/setup.py` & `ondewo-csi-client-4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 long_description: str = read_file('README.md')
 requires: List[str] = read_requirements('requirements.txt')
 
 setup(
     name="ondewo-csi-client",
-    version='3.2.0',
+    version='4.0.0',
     author="ONDEWO GbmH",
     author_email="office@ondewo.com",
     description="Provides endpoints and messages for gRPC communication to the ONDEWO CSI server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ondewo/ondewo-csi-client-python",
     packages=[
```

