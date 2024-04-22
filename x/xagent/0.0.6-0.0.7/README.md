# Comparing `tmp/xagent-0.0.6.tar.gz` & `tmp/xagent-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xagent-0.0.6.tar", last modified: Mon Apr 15 04:06:31 2024, max compression
+gzip compressed data, was "xagent-0.0.7.tar", last modified: Mon Apr 22 05:37:01 2024, max compression
```

## Comparing `xagent-0.0.6.tar` & `xagent-0.0.7.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:31.003597 xagent-0.0.6/
--rw-r--r--   0 chenhao    (501) staff       (20)     1063 2024-03-14 09:35:14.000000 xagent-0.0.6/LICENSE
--rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-15 04:06:31.003375 xagent-0.0.6/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)     3568 2024-04-15 04:02:55.000000 xagent-0.0.6/README.md
--rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-04-15 04:06:31.003703 xagent-0.0.6/setup.cfg
--rw-r--r--   0 chenhao    (501) staff       (20)     1207 2024-03-21 03:48:59.000000 xagent-0.0.6/setup.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:31.001157 xagent-0.0.6/tests/
--rw-r--r--   0 chenhao    (501) staff       (20)      944 2024-04-15 04:02:55.000000 xagent-0.0.6/tests/test_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2569 2024-04-15 04:02:55.000000 xagent-0.0.6/tests/test_local_model.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4886 2024-04-15 04:02:55.000000 xagent-0.0.6/tests/test_xagent.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4747 2024-04-15 04:02:55.000000 xagent-0.0.6/tests/test_zhipu_api_model.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:31.003088 xagent-0.0.6/xagent.egg-info/
--rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)     1097 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/SOURCES.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/dependency_links.txt
--rw-r--r--   0 chenhao    (501) staff       (20)      123 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/requires.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        8 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/top_level.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/zip-safe
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.986846 xagent-0.0.6/xagents/
--rw-r--r--   0 chenhao    (501) staff       (20)      667 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/__init__.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.988963 xagent-0.0.6/xagents/agent/
--rw-r--r--   0 chenhao    (501) staff       (20)      213 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/agent/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3157 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/agent/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1067 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/agent/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)      811 2024-04-08 07:28:32.000000 xagent-0.0.6/xagents/agent/memory.py
--rw-r--r--   0 chenhao    (501) staff       (20)     7027 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/agent/xagent.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1337 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/config.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.991715 xagent-0.0.6/xagents/kb/
--rw-r--r--   0 chenhao    (501) staff       (20)      178 2024-03-19 07:40:40.000000 xagent-0.0.6/xagents/kb/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     9629 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/kb/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     6559 2024-03-20 02:46:15.000000 xagent-0.0.6/xagents/kb/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)    11172 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/kb/kb.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2492 2024-03-20 03:10:39.000000 xagent-0.0.6/xagents/kb/kb_file.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4583 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/kb/vector_store.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.994953 xagent-0.0.6/xagents/loader/
--rw-r--r--   0 chenhao    (501) staff       (20)      152 2024-03-19 10:48:10.000000 xagent-0.0.6/xagents/loader/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4112 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/loader/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)      983 2024-03-28 09:36:52.000000 xagent-0.0.6/xagents/loader/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1358 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/loader/doc.py
--rw-r--r--   0 chenhao    (501) staff       (20)      863 2024-03-19 10:49:45.000000 xagent-0.0.6/xagents/loader/markdown.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2721 2024-04-08 07:28:32.000000 xagent-0.0.6/xagents/loader/pdf.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3917 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/loader/splitter.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1809 2024-04-08 07:28:32.000000 xagent-0.0.6/xagents/loader/structed.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.997525 xagent-0.0.6/xagents/model/
--rw-r--r--   0 chenhao    (501) staff       (20)      179 2024-03-20 06:50:45.000000 xagent-0.0.6/xagents/model/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2800 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/model/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2442 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/model/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2224 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/model/local.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1234 2024-03-21 07:20:01.000000 xagent-0.0.6/xagents/model/openai.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4064 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/model/zhipu.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.999209 xagent-0.0.6/xagents/tool/
--rw-r--r--   0 chenhao    (501) staff       (20)      226 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/tool/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1358 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/tool/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1631 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/tool/common_tool.py
--rw-r--r--   0 chenhao    (501) staff       (20)      453 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/tool/core.py
--rw-r--r--   0 chenhao    (501) staff       (20)      555 2024-03-15 08:10:20.000000 xagent-0.0.6/xagents/util.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.480812 xagent-0.0.7/
+-rw-r--r--   0 chenhao    (501) staff       (20)     1063 2024-03-14 09:35:14.000000 xagent-0.0.7/LICENSE
+-rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-22 05:37:01.480610 xagent-0.0.7/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)     5501 2024-04-22 05:36:21.000000 xagent-0.0.7/README.md
+-rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-04-22 05:37:01.480900 xagent-0.0.7/setup.cfg
+-rw-r--r--   0 chenhao    (501) staff       (20)     1207 2024-03-21 03:48:59.000000 xagent-0.0.7/setup.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.478470 xagent-0.0.7/tests/
+-rw-r--r--   0 chenhao    (501) staff       (20)     2193 2024-04-19 07:38:46.000000 xagent-0.0.7/tests/test_job.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1830 2024-04-22 05:36:21.000000 xagent-0.0.7/tests/test_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2569 2024-04-15 04:02:55.000000 xagent-0.0.7/tests/test_local_model.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     6219 2024-04-19 08:20:14.000000 xagent-0.0.7/tests/test_xagent.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4747 2024-04-15 04:02:55.000000 xagent-0.0.7/tests/test_zhipu_api_model.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.480349 xagent-0.0.7/xagent.egg-info/
+-rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)     1159 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/SOURCES.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/dependency_links.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)      111 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/requires.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        8 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/top_level.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-22 05:37:01.000000 xagent-0.0.7/xagent.egg-info/zip-safe
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.467276 xagent-0.0.7/xagents/
+-rw-r--r--   0 chenhao    (501) staff       (20)      667 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/__init__.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.468948 xagent-0.0.7/xagents/agent/
+-rw-r--r--   0 chenhao    (501) staff       (20)      213 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/agent/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3426 2024-04-19 08:20:14.000000 xagent-0.0.7/xagents/agent/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2206 2024-04-19 08:20:14.000000 xagent-0.0.7/xagents/agent/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      811 2024-04-08 07:28:32.000000 xagent-0.0.7/xagents/agent/memory.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     7784 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/agent/xagent.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1775 2024-04-19 08:20:14.000000 xagent-0.0.7/xagents/config.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.470966 xagent-0.0.7/xagents/kb/
+-rw-r--r--   0 chenhao    (501) staff       (20)      178 2024-03-19 07:40:40.000000 xagent-0.0.7/xagents/kb/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     9629 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/kb/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     6559 2024-03-20 02:46:15.000000 xagent-0.0.7/xagents/kb/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)    11226 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/kb/kb.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2495 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/kb/kb_file.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4583 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/kb/vector_store.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.473122 xagent-0.0.7/xagents/loader/
+-rw-r--r--   0 chenhao    (501) staff       (20)      152 2024-03-19 10:48:10.000000 xagent-0.0.7/xagents/loader/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4907 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/loader/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3874 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/loader/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     5981 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/loader/docx_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      863 2024-03-19 10:49:45.000000 xagent-0.0.7/xagents/loader/markdown.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3427 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/loader/pdf_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3365 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/loader/splitter.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1809 2024-04-08 07:28:32.000000 xagent-0.0.7/xagents/loader/structed.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.475114 xagent-0.0.7/xagents/model/
+-rw-r--r--   0 chenhao    (501) staff       (20)      179 2024-03-20 06:50:45.000000 xagent-0.0.7/xagents/model/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2800 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/model/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2442 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/model/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2224 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/model/local.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1234 2024-03-21 07:20:01.000000 xagent-0.0.7/xagents/model/openai.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4064 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/model/zhipu.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-22 05:37:01.476762 xagent-0.0.7/xagents/tool/
+-rw-r--r--   0 chenhao    (501) staff       (20)      226 2024-04-15 04:02:55.000000 xagent-0.0.7/xagents/tool/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1429 2024-04-19 08:20:14.000000 xagent-0.0.7/xagents/tool/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1641 2024-04-22 03:01:50.000000 xagent-0.0.7/xagents/tool/common_tool.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      463 2024-04-22 05:36:21.000000 xagent-0.0.7/xagents/tool/core.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     6766 2024-04-22 03:01:52.000000 xagent-0.0.7/xagents/tool/web_search.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      560 2024-04-19 07:38:46.000000 xagent-0.0.7/xagents/util.py
```

### Comparing `xagent-0.0.6/LICENSE` & `xagent-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/setup.py` & `xagent-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/tests/test_local_model.py` & `xagent-0.0.7/tests/test_local_model.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/tests/test_xagent.py` & `xagent-0.0.7/tests/test_xagent.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 @Time    :   2024/04/11 17:17:19
 @Author  :   ChenHao
 @Description  :   测试xagent
 @Contact :   jerrychen1990@gmail.com
 '''
 
 from unittest import TestCase
-
+import sys
+# sys.path.append("../")
 from xagents.agent.api import *
 from xagents.kb.api import *
 from loguru import logger
 from snippets import set_logger
 
 
 # unit test
@@ -39,14 +40,40 @@
         agent_resp = chat_agent(name=agent.name, message=message, stream=True, llm_gen_config=llm_gen_config)
         logger.info(f"agent resp: {agent_resp.model_dump(exclude={'content'})}")
         self.assertIsNotNone(agent_resp.content)
         for chunk in agent_resp.content:
             logger.info(chunk)
         self.assertIsNotNone(agent_resp.usage)
 
+    def test_agent_tool_websearch_use(self):
+
+        agent_name = "unittest_agent"
+        llm_config = dict(cls="GLM", version="glm-3-turbo")
+        kb_name = "unittest_kb"
+        self._init_kb(kb_name)
+        kb_config = KBConfig(name=kb_name)
+        tools_config = [dict(name="联网查询")]
+        #
+        # web_search_config = WebSearchConfig(name = "test")
+        # print(f"web_search_config1:{web_search_config}")
+
+        logger.info(f"create tools_config_v1 {tools_config} success")
+        # create agent
+        agent: XAgent = create_agent(name=agent_name, llm_config=llm_config, tools_config=tools_config, kb_config=kb_config)
+        logger.info(f"create Agent {agent.get_info()} success")
+
+        # chat with agent
+        message = "帮我查询一下杭州的最新天气"#"你能帮我找一下今天关于杭州实时新闻吗？"
+        kb_search_config = KBSearchConfig(do_expand=True, expand_len=200)
+        llm_gen_config = LLMGenConfig()
+        agent_resp = chat_agent(name=agent.name, message=message, use_kb = False, stream=False, kb_search_config= kb_search_config, llm_gen_config=llm_gen_config)
+        logger.info(f"agent resp: {agent_resp.model_dump()}")
+        self.assertIsNotNone(agent_resp.content)
+        self.assertIsNotNone(agent_resp.usage)
+
     def test_agent_multi_turn(self):
         agent_name = "unittest_agent"
         llm_config = dict(cls="GLM", version="glm-3-turbo")
         _system = "请用英语回答我的问题"
 
         # create agent
         agent: XAgent = create_agent(name=agent_name, llm_config=llm_config)
@@ -117,8 +144,11 @@
 
         self.assertIsNotNone(agent_resp.references)
         for reference in agent_resp.references:
             logger.info(f"reference: {reference.to_plain_text()}")
 
         self.assertIsNotNone(agent_resp.usage)
 
-        # logger.info(f"agent resp: {agent_resp.model_dump(exclude={'content'})}")
+        logger.info(f"agent resp: {agent_resp.model_dump(exclude={'content'})}")
+
+
+
```

### Comparing `xagent-0.0.6/tests/test_zhipu_api_model.py` & `xagent-0.0.7/tests/test_zhipu_api_model.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagent.egg-info/SOURCES.txt` & `xagent-0.0.7/xagent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,29 +14,31 @@
 ./xagents/kb/common.py
 ./xagents/kb/kb.py
 ./xagents/kb/kb_file.py
 ./xagents/kb/vector_store.py
 ./xagents/loader/__init__.py
 ./xagents/loader/api.py
 ./xagents/loader/common.py
-./xagents/loader/doc.py
+./xagents/loader/docx_loader.py
 ./xagents/loader/markdown.py
-./xagents/loader/pdf.py
+./xagents/loader/pdf_loader.py
 ./xagents/loader/splitter.py
 ./xagents/loader/structed.py
 ./xagents/model/__init__.py
 ./xagents/model/api.py
 ./xagents/model/common.py
 ./xagents/model/local.py
 ./xagents/model/openai.py
 ./xagents/model/zhipu.py
 ./xagents/tool/__init__.py
 ./xagents/tool/api.py
 ./xagents/tool/common_tool.py
 ./xagents/tool/core.py
+./xagents/tool/web_search.py
+tests/test_job.py
 tests/test_loader.py
 tests/test_local_model.py
 tests/test_xagent.py
 tests/test_zhipu_api_model.py
 xagent.egg-info/PKG-INFO
 xagent.egg-info/SOURCES.txt
 xagent.egg-info/dependency_links.txt
```

### Comparing `xagent-0.0.6/xagents/__init__.py` & `xagent-0.0.7/xagents/__init__.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/agent/api.py` & `xagent-0.0.7/xagents/agent/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 '''
 from enum import Enum
 from typing import List
 from xagents.tool.api import get_tools
 from xagents.model.common import LLMGenConfig
 from xagents.kb.api import KBSearchConfig
 from xagents.config import AGENT_DIR, XAGENT_CACHE_NUM
-from xagents.agent.common import AgentResp, KBConfig
+from xagents.agent.common import AgentResp, KBConfig, WebSearchConfig
 from xagents.agent.xagent import XAgent
 from cachetools import LRUCache, cached
 from loguru import logger
 
 agent_cache = LRUCache(maxsize=XAGENT_CACHE_NUM)
 
 
@@ -26,18 +26,22 @@
 
 
 def create_agent(name: str, llm_config: dict = dict(cls="GLM", name="glm", version="glm-4"),
                  tools_config: List[dict] = [], memory_config: dict = dict(size=10),
                  kb_config: KBConfig = None, store_type=STORE_TYPE.CACHE) -> XAgent:
 
     logger.info(f"creating agent:{name}")
+    # print(f"web_search_config2:{web_search_config}")
 
     @cached(agent_cache)
     def _get_or_create(name: str):
-        tools = get_tools(tools_config)
+        tools = get_tools( tools_config)  #  [{'name': '联网查询'}]
+        # print(f"web_search_config3:{web_search_config}")
+        logger.info(f"getting tools_config:{tools_config}")
+        logger.info(f"getting tools:{tools}")
         xagent = XAgent(name=name, llm_config=llm_config, memory_config=memory_config, kb_config=kb_config, tools=tools)
         return xagent
     agent = _get_or_create(name=name)
     if store_type == STORE_TYPE.DISK:
         agent.save(AGENT_DIR)
         
     return agent
```

### Comparing `xagent-0.0.6/xagents/agent/common.py` & `xagent-0.0.7/xagents/agent/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,32 +9,57 @@
 from typing import List, Optional
 
 from abc import abstractmethod
 
 from pydantic import BaseModel, Field
 
 from agit.common import LLMResp
-from xagents.config import DEFAULT_KB_PROMPT_TEMPLATE
+from xagents.config import DEFAULT_KB_PROMPT_TEMPLATE, DEFAULT_WEB_SEARCH_KB_PROMPT_TEMPLATE, \
+    DEFAULT_WEB_SEARCH_PROMPT_TEMPLATE
 from xagents.kb.common import RecalledChunk
 
-
-class AgentResp(LLMResp):
-    references: Optional[List[RecalledChunk]] = Field(description="召回的片段")
+# class WebResult(BaseModel):
+#     summary:str
+#     pages:List[str, str]
 
 
+class WebPage(BaseModel):
+    url:str = Field(description="网页的URL")
+    content:str = Field(description="网页的内容")    
+
+class WebSearchResp(BaseModel):
+    summary: str = Field(description="搜索结果的摘要")
+    pages: List[WebPage]|None = Field(description="搜索结果的网页列表")
+    
 
+class AgentResp(LLMResp):
+    references: Optional[List[RecalledChunk]] = Field(description="召回的片段")
+    web_search_result: Optional[WebSearchResp] = Field(description="联网搜索的结果", default=None)
+    
 class AbstractAgent:
 
     def __init__(self, name) -> None:
         self.name = name
 
     @abstractmethod
     def chat(self, message: str, stream=True, do_remember=True) -> AgentResp:
         raise NotImplementedError
 
     @abstractmethod
     def remember(self, role: str, message: str):
         raise NotImplementedError
 
+
 class KBConfig(BaseModel):
     name: str = Field(description="知识库名称")
-    prompt_template:str = Field(description="应用知识库的提示词模板, 必须包含{context}和{question}两个字段", default=DEFAULT_KB_PROMPT_TEMPLATE)
+    prompt_template: str = Field(description="应用知识库的提示词模板, 必须包含{context}和{question}两个字段",
+                                 default=DEFAULT_KB_PROMPT_TEMPLATE)
+
+
+class WebSearchConfig(BaseModel):
+    name: str = Field(description="应用联网搜索的名称")
+    prompt_search_template: str = Field(
+        description="应用联网搜索的提示词模板, 必须包含{seach_info}和{question}两个字段",
+        default=DEFAULT_WEB_SEARCH_PROMPT_TEMPLATE)
+    prompt_search_kb_template: str = Field(
+        description="应用知识库的提示词模板, 必须包含{search_info},{context}和{question}三个字段",
+        default=DEFAULT_WEB_SEARCH_KB_PROMPT_TEMPLATE)
```

### Comparing `xagent-0.0.6/xagents/agent/memory.py` & `xagent-0.0.7/xagents/agent/memory.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/agent/xagent.py` & `xagent-0.0.7/xagents/agent/xagent.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,65 +4,70 @@
 @Time    :   2023/12/07 17:57:13
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 
 import os
+import copy
 from typing import Generator, List, Optional
 
 from pydantic import BaseModel, Field
 
 from agit.common import LLMResp
 from xagents.model.common import LLMGenConfig
-from xagents.agent.common import AbstractAgent, AgentResp, KBConfig
+from xagents.agent.common import AbstractAgent, AgentResp, KBConfig, WebSearchResp
 from xagents.config import LOG_DIR
 from xagents.kb.common import RecalledChunk
 from xagents.kb.api import KBSearchConfig, get_knowledge_base
 from xagents.model.api import get_llm_model
 from xagents.agent.memory import BaseMemory
 from xagents.tool.api import invoke_tool_call
-from xagents.tool.core import BaseTool, ToolCall
+from xagents.tool.core import BaseTool, ToolCall, ToolDesc
 from snippets import dump, load
 
 from loguru import logger
 
 agent_log_path = os.path.join(LOG_DIR, "xagent.log")
 
 
 class XAgentInfo(BaseModel):
     name: str = Field(description="agent的名称，唯一键")
     llm_config: dict = Field(description="llm的配置信息")
     memory_config: dict = Field(description="memory的配置信息")
     kb_config: Optional[KBConfig] = Field(description="kb的配置信息")
-    tools: List[BaseTool] = Field(description="工具列表")
+    # web_search_config: Optional[WebSearchConfig] = Field(description="web_search的配置信息")
+    tools_descs: List[ToolDesc] = Field(description="工具列表")
 
 
 class XAgent(AbstractAgent):
 
     def __init__(self, name: str,
                  llm_config: dict,
                  memory_config: dict,
-                 kb_config: KBConfig,
+                 kb_config:KBConfig,
+                 # web_search_config: WebSearchConfig,
                  tools: List[BaseTool] = []) -> None:
         super().__init__(name=name)
-        self.info = XAgentInfo(name=name, llm_config=llm_config, memory_config=memory_config, kb_config=kb_config, tools=tools)
-
+        self.info = XAgentInfo(name=name,llm_config=llm_config, memory_config=memory_config,kb_config=kb_config,
+                               tools_descs=[ToolDesc(**e.model_dump(exclude={})) for e in tools])
         self.llm_model = get_llm_model(llm_config)
         self.memory = BaseMemory(**memory_config)
         self._load_kb(kb_config)
+        # print(f"web_search_config_0:{web_search_config}")
+        # self._load_web_search(web_search_config)
         self.tools = tools
 
     def _load_kb(self, kb_config: KBConfig):
         if not kb_config:
             self.kb = None
             self.kb_prompt_template = None
         else:
             self.kb = get_knowledge_base(kb_config.name)
-            self.kb_prompt_template = kb_config.prompt_template
+            self.kb_prompt_template = kb_config.prompt_template     
             logger.info("load kb finish")
 
     def get_info(self):
         return self.info
 
     def search_kb(self, query: str, **kwargs) -> List[RecalledChunk]:
         chunks = self.kb.search(query=query, **kwargs)
@@ -90,56 +95,61 @@
             raise FileExistsError(f"config file {config_path} not found")
 
         kwargs = load(config_path)
         if kwargs.get("kb_config"):
             kwargs["kb_config"] = KBConfig.model_validate(kwargs["kb_config"])
         logger.debug(f"{kwargs=}")
 
-        return XAgent(**kwargs)
+        return XAgent(**kwargs)     
 
-    def chat(self, message: str, do_remember=True, details=False, stream=False,
-             use_kb=False, kb_search_config: KBSearchConfig = KBSearchConfig(),
-             fake_chat=False, llm_gen_config: LLMGenConfig = LLMGenConfig(), **kwargs) -> AgentResp:
-        logger.info(f"agent get message:{message}")
 
-        if use_kb:
+    def chat(self, message: str, do_remember=True, details=False, stream = False,
+             use_kb=False, kb_search_config:KBSearchConfig=KBSearchConfig(),
+             fake_chat=False, llm_gen_config:LLMGenConfig=LLMGenConfig(), **kwargs) -> AgentResp:
 
+        chunks = []
+        if use_kb:
             if not self.kb or not self.kb_prompt_template:
                 logger.warning(f"agent:{self.name} has no related knowledge base, will not chat with kb! ")
                 prompt = message
                 chunks = None
-
             else:
                 logger.info("agent searching kb")
                 chunks = self.search_kb(query=message, **kb_search_config.model_dump())
-                # logger.info(f"agent get {len(chunks)} chunks :{chunks}")
-                # logger.info(f"sample chunks:{chunks[:3]}")
                 context = "\n".join(f"{idx+1}." + c.to_plain_text() for idx, c in enumerate(chunks))
-
                 prompt = self.kb_prompt_template.format(question=message, context=context)
         else:
             prompt = message
             chunks = None
 
+        web_search_result = None
+        tool_calls = None
         if fake_chat:
             fake_resp = "这是MOCK的回答信息,如果需要真实回答,请设置fake_chat=False"
             llm_resp = (e for e in fake_resp) if stream else fake_resp
             tool_call = None
         else:
             history = self.memory.to_llm_history()
             llm_resp: LLMResp = self.llm_model.generate(prompt=prompt, history=history, tools=self.tools, details=details, stream=stream,
                                                         **llm_gen_config.model_dump(), **kwargs)
+
+            logger.debug(f"llm_resp_inner:{llm_resp}")
             # 调用tool
-            tool_calls = llm_resp.tool_calls
+            tool_calls = copy.deepcopy(llm_resp.tool_calls)
             if tool_calls:
                 for tool_call in tool_calls:
                     logger.debug(f"calling tool:{tool_call.name}")
-                    self.use_tool(tool_call)
+                    tool_resp = self.use_tool(tool_call)
+                    logger.debug(f"tool_resp:{tool_resp}")
                     llm_resp = self.llm_model.observe(prompt=prompt, tool_call=tool_call, tools=self.tools, history=history, details=details, stream=stream,
                                                       **llm_gen_config.model_dump(), **kwargs)
+                    if tool_call.name == "联网查询":
+                        search_results, sub_page_contents = tool_resp[0], tool_resp[1]
+                        search_info = "\n".join(sub_page_contents)
+                        web_search_result = WebSearchResp(summary=search_info, pages=None)
 
         def _remember_callback(resp_str):
             if do_remember:
                 self.remember("user", message)
                 self.remember("assistant", resp_str)
 
         def _add_remember_callback(gen: Generator) -> Generator:
@@ -154,15 +164,15 @@
         if stream:
             content = _add_remember_callback(llm_resp.content)
         else:
             content = llm_resp.content
             logger.info(f"generate response:{content}")
             _remember_callback(content)
 
-        resp = AgentResp(content=content, tool_calls=llm_resp.tool_calls, usage=llm_resp.usage, references=chunks, details=llm_resp.details)
+        resp = AgentResp(content=content, tool_calls=tool_calls, usage=llm_resp.usage, references=chunks, details=llm_resp.details, web_search_result=web_search_result)
         return resp
 
     def remember(self, role: str, message: str):
         logger.debug(f"remembering {role=}, {message=}")
         self.memory.remember(role, message)
 
     def clear_memory(self):
```

### Comparing `xagent-0.0.6/xagents/kb/api.py` & `xagent-0.0.7/xagents/kb/api.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/kb/common.py` & `xagent-0.0.7/xagents/kb/common.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/kb/kb.py` & `xagent-0.0.7/xagents/kb/kb.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,16 +114,18 @@
                 logger.debug(f"setting embedding model batch size to {batch_size}")
                 setattr(embd_model, "batch_size", batch_size)
             else:
                 logger.warning(f"{embd_model.__class__} has no attribute batch_size, set to default value {batch_size}")  
                 
             self.remove_kb_file_from_index(index, kb_file)
             chunks = kb_file.get_chunks()
-            logger.info(f"reindexing {kb_file.file_name} with {len(chunks)}chunks")
-            documents = [chunk.to_document() for chunk in chunks]
+            documents = [chunk.to_document() for chunk in chunks if chunk.content]
+
+            logger.info(f"reindexing {kb_file.file_name} with {len(chunks)}chunks and {len(documents)} documents")
+    
             # logger.debug(f"sample document:{documents[0]}")
             ids = index.add_documents(documents)
             logger.debug(f"{len(ids)} documents add to index")
             dump(ids, kb_file.id_path)
         # logger.debug(f"{index=}")
         if index.is_local() and do_save:
         # TODO 为何isinstance判断不work？
```

### Comparing `xagent-0.0.6/xagents/kb/kb_file.py` & `xagent-0.0.7/xagents/kb/kb_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 
     def get_info(self):
         return KnowledgeBaseFileInfo(kb_name=self.kb_name, file_name=self.file_name, is_cut=self.is_cut, is_indexed=self.is_indexed)
 
     def cut(self, *args, **kwargs):
         logger.info(f"start cut file: {self.file_name}")
         chunks: List[Chunk] = parse_file(file_path=self.origin_path, *args, **kwargs)
-        kb_chunks = [KBChunk(**chunk.model_dump(mode="json"), idx=idx, kb_name=self.kb_name, file_name=self.file_name)
-                     for idx, chunk in enumerate(chunks)]
+        kb_chunks = [KBChunk(**chunk.to_json(), idx=idx, kb_name=self.kb_name, file_name=self.file_name)
+                     for idx, chunk in enumerate(chunks) if chunk.content]
         kb_chunk_json = [chunk.to_dict() for chunk in kb_chunks]
         dump(kb_chunk_json, self.chunk_path)
         return len(kb_chunks)
 
     def get_chunks(self) -> List[KBChunk]:
         """
         从切片文件加载切片
```

### Comparing `xagent-0.0.6/xagents/kb/vector_store.py` & `xagent-0.0.7/xagents/kb/vector_store.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/loader/markdown.py` & `xagent-0.0.7/xagents/loader/markdown.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/loader/splitter.py` & `xagent-0.0.7/xagents/loader/splitter.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,40 +7,41 @@
 '''
 
 import copy
 import re
 from abc import abstractmethod
 from typing import Iterable, List
 
+from xagents.loader.common import ContentType
 from xagents.config import *
 from xagents.kb.common import Chunk
 from snippets import batchify
-from loguru import logger
 
 
 class AbstractSplitter:
     def __init__(self, invalid_chunks: List[str] = []):
         self.invalid_chunks = invalid_chunks
 
     @abstractmethod
     def split(self, text: str) -> List[str]:
         raise NotImplementedError
 
-    def split_chunk(self, chunk: Chunk) -> List[Chunk]:
-        rs_chunks = []
-        for content in self.split(chunk.content):
-            content = content.strip()
-            if content in self.invalid_chunks:
-                continue
-            rs_chunks.append(Chunk(content=content,  content_type=chunk.content_type, page_idx=chunk.page_idx))
-        return rs_chunks
-
-# 将文本切分、合并到（min_len~max_len）之间的长度
+    def split_chunk(self, chunk: Chunk) -> Iterable[Chunk]:
+        if chunk.content_type == ContentType.TABLE or chunk.content_type==ContentType.IMAGE:
+            # 图片和表格暂时不做切割
+            yield chunk
+        else:
 
+            for content in self.split(chunk.content):
+                content = content.strip()
+                if content in self.invalid_chunks:
+                    continue
+                yield Chunk(content=content,  content_type=chunk.content_type, page_idx=chunk.page_idx)
 
+# 将文本切分、合并到（min_len~max_len）之间的长度
 def merge_cut_texts(texts: Iterable[str], min_len: int, max_len: int) -> Iterable[str]:
     acc = ""
     for text in texts:
         acc += text
         if len(acc) < min_len:
             continue
         if len(acc) > max_len:
@@ -75,40 +76,22 @@
     def _parse_text(self, text: str) -> str:
         text = text.strip()
         # text = re.sub("\s+", " ", text)
         # text = re.sub(f"\.{3,}", "", text)
         text = text.strip()
         return text
 
-    def split(self, text: str) -> List[str]:
+    def split(self, text: str) -> Iterable[str]:
         # logger.info(f"{text=}")
         # logger.info(f"{self.separator=}")
         
         texts = re.split(self.separator, text)
         texts = [self._parse_text(t) for t in texts]
         # logger.debug(f"{texts=}")
-        texts = list(merge_cut_texts(texts, self.min_len, self.max_len))
-        # logger.debug(f"{text=}")
-        return texts
-
-    # def split_chunk(self, chunk: Chunk) -> List[Chunk]:
-    #     rs_chunks: List[Chunk] = []
-    #     if chunk.content_type == ContentType.TABLE and self.parse_table:
-    #         table_chunks = []
-    #         tables = markdown2tables(chunk.content)
-    #         for table in tables:
-    #             descs = table.to_desc()
-    #             table_chunks.extend([Chunk(content=e, content_type=ContentType.PARSED_TABLE, page_idx=chunk.page_idx) for e in descs])
-    #         rs_chunks.extend(table_chunks)
-    #     else:
-    #         rs_chunks = super().split_chunk(chunk)
-    #         logger.debug(f"{rs_chunks=}")
-
-    #     return rs_chunks
-
+        yield from merge_cut_texts(texts, self.min_len, self.max_len)
 
 _SPLITTERS = [BaseSplitter]
 _NAME2SPLITTER = {s.__name__: s for s in _SPLITTERS}
 
 
 def get_splitter(config: dict) -> AbstractSplitter:
     tmp_config = copy.copy(config)
```

### Comparing `xagent-0.0.6/xagents/loader/structed.py` & `xagent-0.0.7/xagents/loader/structed.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/model/api.py` & `xagent-0.0.7/xagents/model/api.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/model/common.py` & `xagent-0.0.7/xagents/model/common.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/model/local.py` & `xagent-0.0.7/xagents/model/local.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/model/openai.py` & `xagent-0.0.7/xagents/model/openai.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/model/zhipu.py` & `xagent-0.0.7/xagents/model/zhipu.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.6/xagents/tool/api.py` & `xagent-0.0.7/xagents/tool/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 from typing import Any, List
 
 from xagents.tool.common_tool import calculator, travel_searcher
+from xagents.tool.web_search import web_search_sogou
 from xagents.tool.core import BaseTool, ToolCall
 from loguru import logger
 
 
-_ALL_TOOLS = [calculator, travel_searcher]
+_ALL_TOOLS = [calculator, travel_searcher, web_search_sogou]
 _TOOL_MAP = {e.name:e for e in _ALL_TOOLS}
 
 
 def invoke_tool_call(tool_call:ToolCall)->Any:
     tool = get_tool(tool_call.name)
     resp = tool.execute(**tool_call.parameters)
     tool_call.resp = resp
```

### Comparing `xagent-0.0.6/xagents/tool/common_tool.py` & `xagent-0.0.7/xagents/tool/common_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 '''
 @Time    :   2024/01/04 14:04:02
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
-
+import sys
 from xagents.tool.core import BaseTool
 from agit.common import Parameter
 
 
 def exec_python(expression: str) -> dict:
     try:
         rs = eval(expression)
```

### Comparing `xagent-0.0.6/xagents/util.py` & `xagent-0.0.7/xagents/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,8 +20,12 @@
     @wraps(func)
     def wrapped(**kwargs):
         print(f"{kwargs=}")
         for k,v in kwargs.items():
             if isinstance(v, Body):
                 kwargs[k] = v.default
         return func(**kwargs)
-    return wrapped
+    return wrapped
+
+
+
+
```

