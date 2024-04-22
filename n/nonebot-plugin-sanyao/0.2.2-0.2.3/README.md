# Comparing `tmp/nonebot_plugin_sanyao-0.2.2.tar.gz` & `tmp/nonebot_plugin_sanyao-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sanyao-0.2.2.tar", last modified: Mon Apr 22 04:17:53 2024, max compression
+gzip compressed data, was "nonebot_plugin_sanyao-0.2.3.tar", last modified: Mon Apr 22 05:39:18 2024, max compression
```

## Comparing `nonebot_plugin_sanyao-0.2.2.tar` & `nonebot_plugin_sanyao-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:17:53.677943 nonebot_plugin_sanyao-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-22 04:17:49.000000 nonebot_plugin_sanyao-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-22 04:17:53.677943 nonebot_plugin_sanyao-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-22 04:17:49.000000 nonebot_plugin_sanyao-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:17:53.673943 nonebot_plugin_sanyao-0.2.2/nonebot_plugin_sanyao/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:17:53.677943 nonebot_plugin_sanyao-0.2.2/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-22 04:17:53.000000 nonebot_plugin_sanyao-0.2.2/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-22 04:17:53.000000 nonebot_plugin_sanyao-0.2.2/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 04:17:53.000000 nonebot_plugin_sanyao-0.2.2/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 04:17:53.000000 nonebot_plugin_sanyao-0.2.2/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 04:17:53.000000 nonebot_plugin_sanyao-0.2.2/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-22 04:17:49.000000 nonebot_plugin_sanyao-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 04:17:53.677943 nonebot_plugin_sanyao-0.2.2/setup.cfg
+-rw-r--r--   0        0        0     1064 2024-04-22 05:39:06.544946 nonebot_plugin_sanyao-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2287 2024-04-22 05:39:06.544946 nonebot_plugin_sanyao-0.2.3/README.md
+-rw-r--r--   0        0        0      342 2024-04-22 05:39:06.544946 nonebot_plugin_sanyao-0.2.3/nonebot_plugin_sanyao/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-22 05:39:06.544946 nonebot_plugin_sanyao-0.2.3/nonebot_plugin_sanyao/__main__.py
+-rw-r--r--   0        0        0       87 2024-04-22 05:39:06.544946 nonebot_plugin_sanyao-0.2.3/nonebot_plugin_sanyao/config.py
+-rw-r--r--   0        0        0     6143 2024-04-22 05:39:06.544946 nonebot_plugin_sanyao-0.2.3/nonebot_plugin_sanyao/sanyao.py
+-rw-r--r--   0        0        0      963 2024-04-22 05:39:18.324826 nonebot_plugin_sanyao-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 nonebot_plugin_sanyao-0.2.3/PKG-INFO
```

### Comparing `nonebot_plugin_sanyao-0.2.2/LICENSE` & `nonebot_plugin_sanyao-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sanyao-0.2.2/PKG-INFO` & `nonebot_plugin_sanyao-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sanyao
-Version: 0.2.2
+Version: 0.2.3
 Summary: 三爻易数排盘
-Author-email: afterow <afterow@163.com>
+Author-Email: afterow <afterow@163.com>
 License: MIT License
-Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
-Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: Chinese (Simplified)
-Requires-Python: <4.0,>=3.10
+Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
+Project-URL: Bug tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
+Requires-Python: >=3.9
+Requires-Dist: cnlunar>=0.1.3
+Requires-Dist: nonebot2>=2.2.0
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: cnlunar
-Requires-Dist: nonebot2
 
 <div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <a href="https://v2.nonebot.dev/store">
+    <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="logo">
+  </a>
   <br>
-  <p><img src="resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+  <p>
+    <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="logo">
+  </p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-sanyao
 
 _✨ NoneBot 插件简单描述 ✨_
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.2.2 Summary:
-ä¸ç»ææ°æç Author-email: afterow
-163.com> License: MIT License Project-URL: Homepage, https://github.com/
-afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
-afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Natural Language :: Chinese (Simplified)
-Requires-Python: <4.0,>=3.10 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: cnlunar Requires-Dist: nonebot2
-                              _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
-                              [NoneBotPluginText]
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.2.3 Summary:
+ä¸ç»ææ°æç Author-Email: afterow
+163.com> License: MIT License Classifier: Framework :: Pydantic Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Natural Language :: Chinese (Simplified) Project-
+URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao Project-URL:
+Bug tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues Requires-
+Python: >=3.9 Requires-Dist: cnlunar>=0.1.3 Requires-Dist: nonebot2>=2.2.0
+Description-Content-Type: text/markdown
+                                    _[_l_o_g_o_]
+                                    [logo]
   # nonebot-plugin-sanyao _â¨ NoneBot æä»¶ç®åæè¿° â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 è¿æ¯ä¸ä¸ª ä¸ç»ææ°æä»¶ ## ð ä»ç» è¿éæ¯ä¸ä¸ª
 ä¸ç»ææ°æä»¶ï¼åç»­å¢å 64å¦ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨
 nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
 nb plugin install nonebot-plugin-sanyao ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
```

### Comparing `nonebot_plugin_sanyao-0.2.2/README.md` & `nonebot_plugin_sanyao-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 <div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <a href="https://v2.nonebot.dev/store">
+    <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="logo">
+  </a>
   <br>
-  <p><img src="resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+  <p>
+    <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="logo">
+  </p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-sanyao
 
 _✨ NoneBot 插件简单描述 ✨_
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-                              _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
-                              [NoneBotPluginText]
+                                    _[_l_o_g_o_]
+                                    [logo]
   # nonebot-plugin-sanyao _â¨ NoneBot æä»¶ç®åæè¿° â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 è¿æ¯ä¸ä¸ª ä¸ç»ææ°æä»¶ ## ð ä»ç» è¿éæ¯ä¸ä¸ª
 ä¸ç»ææ°æä»¶ï¼åç»­å¢å 64å¦ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨
 nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
 nb plugin install nonebot-plugin-sanyao ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
```

### Comparing `nonebot_plugin_sanyao-0.2.2/pyproject.toml` & `nonebot_plugin_sanyao-0.2.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 [project]
 name = "nonebot-plugin-sanyao"
-version = "0.2.2"
+dynamic = []
 authors = [
-    {name="afterow", email="afterow@163.com"}
+    { name = "afterow", email = "afterow@163.com" },
 ]
 description = "三爻易数排盘"
 readme = "README.md"
-license = { text = "MIT License" }
-requires-python = ">=3.10, <4.0"
+requires-python = ">=3.9"
 dependencies = [
-    "cnlunar",
-    "nonebot2"
+    "cnlunar>=0.1.3",
+    "nonebot2>=2.2.0",
 ]
 classifiers = [
     "Framework :: Pydantic",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Natural Language :: Chinese (Simplified)"
+    "Natural Language :: Chinese (Simplified)",
 ]
+version = "0.2.3"
 
-[tool.nonebot]
-adapters = [
-    { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" }
-]
-plugins = ["nonebot_plugin_sanyao"]
-plugin_dirs = ["nonebot_plugin_sanyao"]
-builtin_plugins = []
+[project.license]
+text = "MIT License"
 
-[tool.setuptools.packages.find]
-where = ['nonebot_plugin_sanyao']
-include = []
+[project.urls]
+Homepage = "https://github.com/afterow/nonebot-plugin-sanyao"
+"Bug Tracker" = "https://github.com/afterow/nonebot-plugin-sanyao/issues"
 
 [build-system]
-requires = ["setuptools >= 65.6.3"]
-build-backend = "setuptools.build_meta"
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
 
-[project.urls]
-"Homepage" = "https://github.com/afterow/nonebot-plugin-sanyao"
-"Bug Tracker" = "https://github.com/afterow/nonebot-plugin-sanyao/issues"
+[tool.pdm.version]
+source = "file"
+path = "nonebot_plugin_sanyao/__init__.py"
```

