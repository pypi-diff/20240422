# Comparing `tmp/qualesim-quiets-1.0.6.tar.gz` & `tmp/qualesim-quiets-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualesim-quiets-1.0.6.tar", last modified: Fri Apr 19 08:11:57 2024, max compression
+gzip compressed data, was "qualesim-quiets-1.0.7.tar", last modified: Mon Apr 22 07:45:34 2024, max compression
```

## Comparing `qualesim-quiets-1.0.6.tar` & `qualesim-quiets-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 08:11:57.790834 qualesim-quiets-1.0.6/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.6/LICENSE
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      891 2024-04-19 08:11:57.786834 qualesim-quiets-1.0.6/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      289 2024-04-19 07:49:03.000000 qualesim-quiets-1.0.6/README.md
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 08:11:57.782833 qualesim-quiets-1.0.6/data/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 08:11:57.786834 qualesim-quiets-1.0.6/data/bin/
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.0.6/data/bin/dqcsfeqi
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 08:11:57.786834 qualesim-quiets-1.0.6/qualesim_quiets/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.6/qualesim_quiets/__init__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.0.6/qualesim_quiets/__main__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    45690 2024-04-19 08:09:20.000000 qualesim-quiets-1.0.6/qualesim_quiets/frontend.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11426 2024-04-17 02:46:12.000000 qualesim-quiets-1.0.6/qualesim_quiets/utils.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 08:11:57.786834 qualesim-quiets-1.0.6/qualesim_quiets.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      891 2024-04-19 08:11:57.000000 qualesim-quiets-1.0.6/qualesim_quiets.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      445 2024-04-19 08:11:57.000000 qualesim-quiets-1.0.6/qualesim_quiets.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-19 08:11:57.000000 qualesim-quiets-1.0.6/qualesim_quiets.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-04-19 08:11:57.000000 qualesim-quiets-1.0.6/qualesim_quiets.egg-info/requires.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-04-19 08:11:57.000000 qualesim-quiets-1.0.6/qualesim_quiets.egg-info/top_level.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-19 08:11:57.790834 qualesim-quiets-1.0.6/setup.cfg
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-04-19 08:11:17.000000 qualesim-quiets-1.0.6/setup.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 08:11:57.786834 qualesim-quiets-1.0.6/tests/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.6/tests/test_cls.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-18 01:57:47.000000 qualesim-quiets-1.0.6/tests/test_example_quiets_whitepaper.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.6/tests/test_gate.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.6/tests/test_qifile.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:45:34.588604 qualesim-quiets-1.0.7/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.7/LICENSE
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      891 2024-04-22 07:45:34.588604 qualesim-quiets-1.0.7/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      289 2024-04-19 07:49:03.000000 qualesim-quiets-1.0.7/README.md
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:45:34.584604 qualesim-quiets-1.0.7/data/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:45:34.584604 qualesim-quiets-1.0.7/data/bin/
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.0.7/data/bin/dqcsfeqi
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:45:34.584604 qualesim-quiets-1.0.7/qualesim_quiets/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.7/qualesim_quiets/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.0.7/qualesim_quiets/__main__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    45500 2024-04-22 07:36:36.000000 qualesim-quiets-1.0.7/qualesim_quiets/frontend.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11426 2024-04-17 02:46:12.000000 qualesim-quiets-1.0.7/qualesim_quiets/utils.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:45:34.584604 qualesim-quiets-1.0.7/qualesim_quiets.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      891 2024-04-22 07:45:34.000000 qualesim-quiets-1.0.7/qualesim_quiets.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      445 2024-04-22 07:45:34.000000 qualesim-quiets-1.0.7/qualesim_quiets.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-22 07:45:34.000000 qualesim-quiets-1.0.7/qualesim_quiets.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-04-22 07:45:34.000000 qualesim-quiets-1.0.7/qualesim_quiets.egg-info/requires.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-04-22 07:45:34.000000 qualesim-quiets-1.0.7/qualesim_quiets.egg-info/top_level.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-22 07:45:34.588604 qualesim-quiets-1.0.7/setup.cfg
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-04-22 07:44:43.000000 qualesim-quiets-1.0.7/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:45:34.588604 qualesim-quiets-1.0.7/tests/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.7/tests/test_cls.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-18 01:57:47.000000 qualesim-quiets-1.0.7/tests/test_example_quiets_whitepaper.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.7/tests/test_gate.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.7/tests/test_qifile.py
```

### Comparing `qualesim-quiets-1.0.6/LICENSE` & `qualesim-quiets-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.6/PKG-INFO` & `qualesim-quiets-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.6
+Version: 1.0.7
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-quiets-1.0.6/qualesim_quiets/frontend.py` & `qualesim-quiets-1.0.7/qualesim_quiets/frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,40 +341,36 @@
                             tar.append(func_data.func_qubit[ii][0])
                         else:
                             tar.append(func_data.func_qubit[ii][jj])
                             func_data.res_qubit.append(str(ii) + "[" + str(jj) + "]")
             res_state_vector["classical"] = res_cls
             if measure_mod == "state_vector":
                 if measure_flag == 1:
-                    if len(func_data.res_qubit) == 0:
+                    if len(tar) == 0:
                         res_state_vector["quantum"] = (
-                            func_data.res_qubit,
+                            [],
                             [],
                         )
                     else:
                         self.measure(
                             tar,
                             arb=ArbData(measure_mod=measure_mod),
                         )
-                        res_state_vector["quantum"] = (
-                            func_data.res_qubit,
-                            eval(self.get_measurement(tar[0])["state_vector"])[1],
-                        )
+                        res_state_vector["quantum"] = (func_data.res_qubit,eval(self.get_measurement(tar[0])["state_for_res"])[1])
                 else:
                     if len(func_data.free_list) == 0:
                         res_state_vector["quantum"] = [1]
                     else:
-                        tar = func_data.func_qubit[func_data.free_list[0]][0]
                         self.measure(
                             tar,
                             arb=ArbData(measure_mod="measureforres"),
                         )
                         res_state_vector["quantum"] = (
                             func_data.res_qubit,
-                            eval(self.get_measurement(tar)["state_vector"])[1],
+                            eval(self.get_measurement(tar[0])["state_for_res"])[1],
                         )
             func_data.state_vector = str(res_state_vector)
             for i in func_data.free_list:
                 self.free(func_data.func_qubit[i])
             return func_data, ret
 
         for i in func_data.free_list:
```

### Comparing `qualesim-quiets-1.0.6/qualesim_quiets/utils.py` & `qualesim-quiets-1.0.7/qualesim_quiets/utils.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.6/qualesim_quiets.egg-info/PKG-INFO` & `qualesim-quiets-1.0.7/qualesim_quiets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.6
+Version: 1.0.7
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-quiets-1.0.6/setup.py` & `qualesim-quiets-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="qualesim-quiets",
-    version="1.0.6",
+    version="1.0.7",
     author="Dingdong Liu",
     author_email="dingdongliu@quanta.org.cn",
     description="QuaLeSim frontend for QUIET-S.",
     license="GPLv3",
     keywords="qualesim quiets",
     url="https://gitee.com/hpcl_quanta/dqcsim-quiets.git",
     long_description=read("README.md"),
```

### Comparing `qualesim-quiets-1.0.6/tests/test_cls.py` & `qualesim-quiets-1.0.7/tests/test_cls.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.6/tests/test_gate.py` & `qualesim-quiets-1.0.7/tests/test_gate.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.6/tests/test_qifile.py` & `qualesim-quiets-1.0.7/tests/test_qifile.py`

 * *Files identical despite different names*

