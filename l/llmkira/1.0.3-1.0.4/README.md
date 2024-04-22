# Comparing `tmp/llmkira-1.0.3.tar.gz` & `tmp/llmkira-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmkira-1.0.3.tar", last modified: Sat Apr 20 05:32:17 2024, max compression
+gzip compressed data, was "llmkira-1.0.4.tar", last modified: Mon Apr 22 09:03:29 2024, max compression
```

## Comparing `llmkira-1.0.3.tar` & `llmkira-1.0.4.tar`

### file list

```diff
@@ -1,61 +1,59 @@
--rw-r--r--   0        0        0    11357 2024-04-20 05:32:02.352945 llmkira-1.0.3/LICENSE
--rw-r--r--   0        0        0     1030 2024-04-20 05:32:02.352945 llmkira-1.0.3/NOTICE.MD
--rw-r--r--   0        0        0     8422 2024-04-20 05:32:02.352945 llmkira-1.0.3/README.md
--rw-r--r--   0        0        0      730 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/__init__.py
--rw-r--r--   0        0        0      209 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/_exception.py
--rw-r--r--   0        0        0     5346 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/cache/__init__.py
--rw-r--r--   0        0        0     1266 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/cache/elara_runtime.py
--rw-r--r--   0        0        0     2299 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/cache/lmdb_runtime.py
--rw-r--r--   0        0        0     1451 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/cache/redis_runtime.py
--rw-r--r--   0        0        0     1159 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/cache/runtime_schema.py
--rw-r--r--   0        0        0     4711 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/doc_manager/__init__.py
--rw-r--r--   0        0        0      127 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/plugins/__init__.py
--rw-r--r--   0        0        0     6886 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/plugins/alarm/__init__.py
--rw-r--r--   0        0        0     8269 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/plugins/e2b_code_interpreter/__init__.py
--rw-r--r--   0        0        0     5950 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/plugins/search/__init__.py
--rw-r--r--   0        0        0     1774 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/plugins/search/engine.py
--rw-r--r--   0        0        0     5527 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/voice/__init__.py
--rw-r--r--   0        0        0     3247 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/extra/voice_hook.py
--rw-r--r--   0        0        0        0 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/__init__.py
--rw-r--r--   0        0        0      626 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/_base.py
--rw-r--r--   0        0        0     2323 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/env.py
--rw-r--r--   0        0        0     4419 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/file.py
--rw-r--r--   0        0        0     1025 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/instruction.py
--rw-r--r--   0        0        0     1512 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/time.py
--rw-r--r--   0        0        0     1158 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/kv_manager/tool_call.py
--rw-r--r--   0        0        0      637 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/__init__.py
--rw-r--r--   0        0        0      733 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/_base.py
--rw-r--r--   0        0        0     2381 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/local_storage.py
--rw-r--r--   0        0        0     1070 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/redis_storage/LICENSE
--rw-r--r--   0        0        0     2819 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/redis_storage/__init__.py
--rw-r--r--   0        0        0     6192 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/memory/redis_storage/utils.py
--rw-r--r--   0        0        0      522 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openai/__init__.py
--rw-r--r--   0        0        0     3431 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openai/_excption.py
--rw-r--r--   0        0        0    10731 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openai/cell.py
--rw-r--r--   0        0        0     8553 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openai/request.py
--rw-r--r--   0        0        0     1968 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openai/utils.py
--rw-r--r--   0        0        0      130 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/__init__.py
--rw-r--r--   0        0        0     2729 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/fuse/__init__.py
--rw-r--r--   0        0        0     1610 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/hook/__init__.py
--rw-r--r--   0        0        0     4285 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/transducer/__init__.py
--rw-r--r--   0        0        0      799 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/transducer/default_factory.py
--rw-r--r--   0        0        0     1229 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/transducer/schema.py
--rw-r--r--   0        0        0     2143 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/trigger/__init__.py
--rw-r--r--   0        0        0      419 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/openapi/trigger/default_trigger.py
--rw-r--r--   0        0        0      321 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/LICENSE
--rw-r--r--   0        0        0     4501 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/__init__.py
--rw-r--r--   0        0        0      496 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/error.py
--rw-r--r--   0        0        0     3373 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/loader.py
--rw-r--r--   0        0        0     9551 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/model.py
--rw-r--r--   0        0        0     3286 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/register.py
--rw-r--r--   0        0        0    10609 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/tools/schema.py
--rw-r--r--   0        0        0     4238 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/sdk/utils.py
--rw-r--r--   0        0        0     4848 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/task/__init__.py
--rw-r--r--   0        0        0    16694 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/task/schema.py
--rw-r--r--   0        0        0      219 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/task/snapshot/__init__.py
--rw-r--r--   0        0        0      422 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/task/snapshot/_base.py
--rw-r--r--   0        0        0     1237 2024-04-20 05:32:02.376945 llmkira-1.0.3/llmkira/task/snapshot/local.py
--rw-r--r--   0        0        0     2919 2024-04-20 05:32:17.048968 llmkira-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1485 2024-04-20 05:32:02.380945 llmkira-1.0.3/tests/pydantic_error.py
--rw-r--r--   0        0        0    11765 1970-01-01 00:00:00.000000 llmkira-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-22 09:03:15.794260 llmkira-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1030 2024-04-22 09:03:15.794260 llmkira-1.0.4/NOTICE.MD
+-rw-r--r--   0        0        0     8725 2024-04-22 09:03:15.794260 llmkira-1.0.4/README.md
+-rw-r--r--   0        0        0      730 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/_exception.py
+-rw-r--r--   0        0        0     5346 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/cache/__init__.py
+-rw-r--r--   0        0        0     1266 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/cache/elara_runtime.py
+-rw-r--r--   0        0        0     2299 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/cache/lmdb_runtime.py
+-rw-r--r--   0        0        0     1451 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/cache/redis_runtime.py
+-rw-r--r--   0        0        0     1159 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/cache/runtime_schema.py
+-rw-r--r--   0        0        0     4711 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/doc_manager/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/plugins/__init__.py
+-rw-r--r--   0        0        0     6886 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/plugins/alarm/__init__.py
+-rw-r--r--   0        0        0     8269 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/plugins/e2b_code_interpreter/__init__.py
+-rw-r--r--   0        0        0     6043 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/plugins/search/__init__.py
+-rw-r--r--   0        0        0     2537 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/plugins/search/engine.py
+-rw-r--r--   0        0        0     5372 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/voice/__init__.py
+-rw-r--r--   0        0        0     3247 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/extra/voice_hook.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/_base.py
+-rw-r--r--   0        0        0     2323 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/env.py
+-rw-r--r--   0        0        0     4419 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/file.py
+-rw-r--r--   0        0        0     1025 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/instruction.py
+-rw-r--r--   0        0        0     1512 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/time.py
+-rw-r--r--   0        0        0     1158 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/kv_manager/tool_call.py
+-rw-r--r--   0        0        0     4284 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/logic/__init__.py
+-rw-r--r--   0        0        0      637 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/_base.py
+-rw-r--r--   0        0        0     2381 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/local_storage.py
+-rw-r--r--   0        0        0     1070 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/redis_storage/LICENSE
+-rw-r--r--   0        0        0     2819 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/redis_storage/__init__.py
+-rw-r--r--   0        0        0     6192 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/memory/redis_storage/utils.py
+-rw-r--r--   0        0        0      522 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openai/__init__.py
+-rw-r--r--   0        0        0     3431 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openai/_excption.py
+-rw-r--r--   0        0        0    10731 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openai/cell.py
+-rw-r--r--   0        0        0     8866 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openai/request.py
+-rw-r--r--   0        0        0     1968 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openai/utils.py
+-rw-r--r--   0        0        0      130 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openapi/__init__.py
+-rw-r--r--   0        0        0     2729 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openapi/fuse/__init__.py
+-rw-r--r--   0        0        0     1610 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openapi/hook/__init__.py
+-rw-r--r--   0        0        0     2143 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openapi/trigger/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/openapi/trigger/default_trigger.py
+-rw-r--r--   0        0        0      321 2024-04-22 09:03:15.818261 llmkira-1.0.4/llmkira/sdk/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/LICENSE
+-rw-r--r--   0        0        0     4501 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/error.py
+-rw-r--r--   0        0        0     3373 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/loader.py
+-rw-r--r--   0        0        0     9551 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/model.py
+-rw-r--r--   0        0        0     3286 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/register.py
+-rw-r--r--   0        0        0    10609 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/tools/schema.py
+-rw-r--r--   0        0        0     4238 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/sdk/utils.py
+-rw-r--r--   0        0        0     4848 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/task/__init__.py
+-rw-r--r--   0        0        0    16694 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/task/schema.py
+-rw-r--r--   0        0        0      219 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/task/snapshot/__init__.py
+-rw-r--r--   0        0        0      422 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/task/snapshot/_base.py
+-rw-r--r--   0        0        0     1237 2024-04-22 09:03:15.822260 llmkira-1.0.4/llmkira/task/snapshot/local.py
+-rw-r--r--   0        0        0     2907 2024-04-22 09:03:29.578371 llmkira-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1485 2024-04-22 09:03:15.822260 llmkira-1.0.4/tests/pydantic_error.py
+-rw-r--r--   0        0        0    12056 1970-01-01 00:00:00.000000 llmkira-1.0.4/PKG-INFO
```

### Comparing `llmkira-1.0.3/LICENSE` & `llmkira-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/NOTICE.MD` & `llmkira-1.0.4/NOTICE.MD`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/README.md` & `llmkira-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,18 @@
 - 📦 Support for plugins to access files
 - 🍟 Multi-platform support – extend new platforms by inheriting the base class
 - 🍔 Plugins can determine their appearance in new sessions dynamically, preventing performance degradation despite large
   amounts of plugins
 
 ### 🍔 Login Modes
 
-- `Login via url`: Use `/login token$https://provider.com` to Login. The program posts the token to the interface to
+- `Login via url`: Use `/login <a token>$<something like https://provider.com/login>` to Login. The program posts the token to the interface to
   retrieve configuration
   information, [how to develop this](https://github.com/LlmKira/Openaibot/blob/81eddbff0f136697d5ad6e13ee1a7477b26624ed/app/components/credential.py#L20).
-- `Login`: Use `/login https://api.com/v1$key$model` to login
+- `Login`: Use `/login https://<api endpoint>/v1$<api key>$<the model>$<tool model such as gpt-3.5-turbo>` to login
 
 ### 🧀 Plugin Can Do More
 
 | Sticker Converter                   | Timer Function(built-in)        |
 |-------------------------------------|---------------------------------|
 | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) |
 
@@ -93,14 +93,15 @@
 
 | Platform | Support | File System | Remarks                                |
 |----------|---------|-------------|----------------------------------------|
 | Telegram | ✅       | ✅           |                                        |
 | Discord  | ✅       | ✅           |                                        |
 | Kook     | ✅       | ✅           | Does not support `triggering by reply` |
 | Slack    | ✅       | ✅           | Does not support `triggering by reply` |
+| Line     | ❌       |             |                                        |
 | QQ       | ❌       |             |                                        |
 | Wechat   | ❌       |             |                                        |
 | Twitter  | ❌       |             |                                        |
 | Matrix   | ❌       |             |                                        |
 | IRC      | ❌       |             |                                        |
 | ...      |         |             | Create Issue/PR                        |
 
@@ -141,14 +142,17 @@
 pdm run python3 start_receiver.py
 # Host
 apt install npm
 npm install pm2 -g
 pm2 start pm2.json
 ```
 
+> **Be sure to change the default password for the command, or disable open ports to prevent the database from being
+scanned and attacked.**
+
 ### 🥣 Docker
 
 Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/docker/sudoskys/llmbot/general)
 
 > Note that if you run this project using Docker, you will start Redis, MongoDB, and RabbitMQ. But if you're running
 > locally, just RabbitMQ
```

#### html2text {}

```diff
@@ -29,62 +29,63 @@
 constraints, offering fully decoupled logics - ð¬ Offers Login via a URL
 mechanism, providing a flexible and expandable authentication development
 solution - ð° Empowers users to authorize plugin execution. Users can
 configure plugin environment variables at their discretion - ð¦ Support for
 plugins to access files - ð Multi-platform support â extend new platforms
 by inheriting the base class - ð Plugins can determine their appearance in
 new sessions dynamically, preventing performance degradation despite large
-amounts of plugins ### ð Login Modes - `Login via url`: Use `/login
-token$https://provider.com` to Login. The program posts the token to the
-interface to retrieve configuration information, [how to develop this](https://
-github.com/LlmKira/Openaibot/blob/81eddbff0f136697d5ad6e13ee1a7477b26624ed/app/
-components/credential.py#L20). - `Login`: Use `/login https://api.com/
-v1$key$model` to login ### ð§ Plugin Can Do More | Sticker Converter | Timer
-Function(built-in) | |-------------------------------------|-------------------
---------------| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/
-timer_func.gif) | ### ð¬ Platform Support | Platform | Support | File System
-| Remarks | |----------|---------|-------------|-------------------------------
----------| | Telegram | â | â | | | Discord | â | â | | | Kook | â |
-â | Does not support `triggering by reply` | | Slack | â | â | Does not
-support `triggering by reply` | | QQ | â | | | | Wechat | â | | | | Twitter
-| â | | | | Matrix | â | | | | IRC | â | | | | ... | | | Create Issue/PR
-| ## ð¦ Quick Start Refer to the [ð§ Deployment Document](https://
-llmkira.github.io/Docs/) for more information. ### ð¦ One-click Deployment If
-you are using a brand-new server, you can use the following shell to
-automatically install this project. ```shell curl -sSL https://
-raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh | bash ``` ### ð¦
-Manual Installation ```shell # Install Voice dependencies apt install ffmpeg #
-Install RabbitMQ docker pull rabbitmq:3.10-management docker run -d -p 5672:
-5672 -p 15672:15672 \ -e RABBITMQ_DEFAULT_USER=admin \ -
+amounts of plugins ### ð Login Modes - `Login via url`: Use `/login $` to
+Login. The program posts the token to the interface to retrieve configuration
+information, [how to develop this](https://github.com/LlmKira/Openaibot/blob/
+81eddbff0f136697d5ad6e13ee1a7477b26624ed/app/components/credential.py#L20). -
+`Login`: Use `/login https:///v1$$$` to login ### ð§ Plugin Can Do More |
+Sticker Converter | Timer Function(built-in) | |-------------------------------
+------|---------------------------------| | ![sticker](./docs/sticker_func.gif)
+| ![timer](./docs/timer_func.gif) | ### ð¬ Platform Support | Platform |
+Support | File System | Remarks | |----------|---------|-------------|---------
+-------------------------------| | Telegram | â | â | | | Discord | â |
+â | | | Kook | â | â | Does not support `triggering by reply` | | Slack |
+â | â | Does not support `triggering by reply` | | Line | â | | | | QQ |
+â | | | | Wechat | â | | | | Twitter | â | | | | Matrix | â | | | | IRC
+| â | | | | ... | | | Create Issue/PR | ## ð¦ Quick Start Refer to the
+[ð§ Deployment Document](https://llmkira.github.io/Docs/) for more
+information. ### ð¦ One-click Deployment If you are using a brand-new server,
+you can use the following shell to automatically install this project. ```shell
+curl -sSL https://raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh |
+bash ``` ### ð¦ Manual Installation ```shell # Install Voice dependencies apt
+install ffmpeg # Install RabbitMQ docker pull rabbitmq:3.10-management docker
+run -d -p 5672:5672 -p 15672:15672 \ -e RABBITMQ_DEFAULT_USER=admin \ -
 e RABBITMQ_DEFAULT_PASS=8a8a8a \ --hostname myRabbit \ --name rabbitmq \
 rabbitmq:3.10-management docker ps -l # Install Project git clone https://
 github.com/LlmKira/Openaibot/ cd Openaibot pip install pdm pdm install -G bot
 cp .env.exp .env && nano .env # Test pdm run python3 start_sender.py pdm run
 python3 start_receiver.py # Host apt install npm npm install pm2 -g pm2 start
-pm2.json ``` ### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://
-hub.docker.com/repository/docker/sudoskys/llmbot/general) > Note that if you
-run this project using Docker, you will start Redis, MongoDB, and RabbitMQ. But
-if you're running > locally, just RabbitMQ #### Manual Docker-compose
-Installation ```shell git clone https://github.com/LlmKira/Openaibot.git cd
-Openaibot cp .env.exp .env&&nano .env docker-compose -f docker-compose.yml up -
-d ``` The Docker configuration file `docker-compose.yml` contains all
-databases. In fact, Redis and MongoDB are not required. You can remove these
-databases yourself and use the local file system. Update image using `docker-
-compose pull`. Use `docker exec -it llmbot /bin/bash` to view Shell in Docker,
-enter `exit` to exit. ## ðª Slash Commands ```shell clear - Deletes chat
-records help - Displays documentation chat - Conversation task - Use a function
-to converse ask - Disable function-based conversations tool - Lists all
-functions login - Login auth - Authorize a function env - Environment variables
-of the function ``` ## ð» How to Develop Plugins? Refer to the example
-plugins in the `plugins` directory and the [ð§ Plugin Development Document]
-(https://llmkira.github.io/Docs/dev/basic) for plugin development
-documentation. ### Hooks Hooks control the EventMessage in sender and receiver.
-For example, we have `voice_hook` in built-in hooks. you can enable it by
-setting `VOICE_REPLY_ME=true` in `.env`. ```shell /env VOICE_REPLY_ME=yes #
-must /env REECHO_VOICE_KEY= # not must ``` use `/env VOICE_REPLY_ME=NONE` to
-disable this env. check the source code in `llmkira/extra/voice_hook.py`, learn
-to write your own hooks. ## ð§ Sponsor [![sponsor](./.github/
-sponsor_ohmygpt.png)](https://www.ohmygpt.com) ## ð Notice > This project,
-named OpenAiBot, signifying "Open Artificial Intelligence Robot", is not
-officially affiliated with > OpenAI. [![FOSSA Status](https://app.fossa.com/
-api/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://
-app.fossa.com/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
+pm2.json ``` > **Be sure to change the default password for the command, or
+disable open ports to prevent the database from being scanned and attacked.**
+### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/
+docker/sudoskys/llmbot/general) > Note that if you run this project using
+Docker, you will start Redis, MongoDB, and RabbitMQ. But if you're running >
+locally, just RabbitMQ #### Manual Docker-compose Installation ```shell git
+clone https://github.com/LlmKira/Openaibot.git cd Openaibot cp .env.exp
+.env&&nano .env docker-compose -f docker-compose.yml up -d ``` The Docker
+configuration file `docker-compose.yml` contains all databases. In fact, Redis
+and MongoDB are not required. You can remove these databases yourself and use
+the local file system. Update image using `docker-compose pull`. Use `docker
+exec -it llmbot /bin/bash` to view Shell in Docker, enter `exit` to exit. ##
+ðª Slash Commands ```shell clear - Deletes chat records help - Displays
+documentation chat - Conversation task - Use a function to converse ask -
+Disable function-based conversations tool - Lists all functions login - Login
+auth - Authorize a function env - Environment variables of the function ``` ##
+ð» How to Develop Plugins? Refer to the example plugins in the `plugins`
+directory and the [ð§ Plugin Development Document](https://llmkira.github.io/
+Docs/dev/basic) for plugin development documentation. ### Hooks Hooks control
+the EventMessage in sender and receiver. For example, we have `voice_hook` in
+built-in hooks. you can enable it by setting `VOICE_REPLY_ME=true` in `.env`.
+```shell /env VOICE_REPLY_ME=yes # must /env REECHO_VOICE_KEY= # not must ```
+use `/env VOICE_REPLY_ME=NONE` to disable this env. check the source code in
+`llmkira/extra/voice_hook.py`, learn to write your own hooks. ## ð§ Sponsor
+[![sponsor](./.github/sponsor_ohmygpt.png)](https://www.ohmygpt.com) ## ð
+Notice > This project, named OpenAiBot, signifying "Open Artificial
+Intelligence Robot", is not officially affiliated with > OpenAI. [![FOSSA
+Status](https://app.fossa.com/api/projects/
+git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://app.fossa.com/
+projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
```

### Comparing `llmkira-1.0.3/llmkira/__init__.py` & `llmkira-1.0.4/llmkira/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/cache/__init__.py` & `llmkira-1.0.4/llmkira/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/cache/elara_runtime.py` & `llmkira-1.0.4/llmkira/cache/elara_runtime.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/cache/lmdb_runtime.py` & `llmkira-1.0.4/llmkira/cache/lmdb_runtime.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/cache/redis_runtime.py` & `llmkira-1.0.4/llmkira/cache/redis_runtime.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/cache/runtime_schema.py` & `llmkira-1.0.4/llmkira/cache/runtime_schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/doc_manager/__init__.py` & `llmkira-1.0.4/llmkira/doc_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/extra/plugins/alarm/__init__.py` & `llmkira-1.0.4/llmkira/extra/plugins/alarm/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/extra/plugins/e2b_code_interpreter/__init__.py` & `llmkira-1.0.4/llmkira/extra/plugins/e2b_code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/extra/plugins/search/__init__.py` & `llmkira-1.0.4/llmkira/extra/plugins/search/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 verify_openapi_version(__package__name__, __openapi_version__)  # noqa: E402
 from llmkira.openai.cell import Tool, ToolCall, class_tool  # noqa: E402
 from llmkira.openapi.fuse import resign_plugin_executor  # noqa: E402
 from llmkira.sdk.tools import PluginMetadata  # noqa: E402
 from llmkira.sdk.tools.schema import FuncPair, BaseTool  # noqa: E402
 from llmkira.task import Task, TaskHeader  # noqa: E402
 from llmkira.task.schema import Location, ToolResponse, EventMessage  # noqa: E402
-from .engine import SerperSearchEngine, build_search_tips  # noqa: E402
+from .engine import SerperSearchEngine, build_search_tips, search_in_duckduckgo  # noqa: E402
 
 
 class Search(BaseModel):
     keywords: str = Field(description="question entered in the search website")
     model_config = ConfigDict(extra="allow")
 
 
 @resign_plugin_executor(tool=Search)
-async def search_on_serper(search_sentence: str, api_key: str):
+async def search_on_serper(search_sentence: str, api_key: str = None):
+    if not api_key:
+        return search_in_duckduckgo(search_sentence)
     result = await SerperSearchEngine(api_key=api_key).search(search_sentence)
     return build_search_tips(search_items=result)
 
 
 class SearchTool(BaseTool):
     """
     搜索工具
@@ -101,26 +103,24 @@
         exception,
         env: dict,
         arg: dict,
         pending_task: "ToolCall",
         refer_llm_result: dict = None,
         **kwargs,
     ):
-        meta = task.task_sign.notify(
+        meta = task.task_sign.reply(
             plugin_name=__plugin_name__,
             tool_response=[
                 ToolResponse(
                     name=__plugin_name__,
                     function_response=f"Run Failed {exception}",
                     tool_call_id=pending_task.id,
                     tool_call=pending_task,
                 )
             ],
-            memory_able=True,
-            response_snapshot=True,
         )
         await Task.create_and_send(
             queue_name=receiver.platform,
             task=TaskHeader(
                 sender=task.sender,
                 receiver=receiver,
                 task_sign=meta,
@@ -158,23 +158,23 @@
         """
         处理message，返回message
         """
 
         _set = Search.model_validate(arg)
         _search_result = await search_on_serper(
             search_sentence=_set.keywords,
-            api_key=env.get("SERPER_API_KEY"),
+            api_key=env.get("SERPER_API_KEY", None),
         )
         # META
         _meta = task.task_sign.reprocess(
             plugin_name=__plugin_name__,
             tool_response=[
                 ToolResponse(
                     name=__plugin_name__,
-                    function_response=str(_search_result),
+                    function_response=f"SearchData: {_search_result},Please give reference link when use it.",
                     tool_call_id=pending_task.id,
                     tool_call=pending_task,
                 )
             ],
         )
         await Task.create_and_send(
             queue_name=receiver.platform,
```

### Comparing `llmkira-1.0.3/llmkira/extra/voice/__init__.py` & `llmkira-1.0.4/llmkira/extra/voice/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import json
 from io import BytesIO
 from typing import Optional
 
 import aiohttp
-import edge_tts
+from gtts import gTTS
 from loguru import logger
 
 
 async def request_dui_speech(text):
     """
     Call the DuerOS endpoint to generate synthesized voice.
     :param text: The text to synthesize
@@ -95,25 +95,23 @@
                     return None
         return audio_bytes
     except Exception as e:
         logger.warning(f"Reecho TTS Error: {e}")
         return None
 
 
-async def request_edge_speech(text: str, voice: str = "en-GB-SoniaNeural"):
+async def request_google_speech(text: str):
     try:
-        communicate = edge_tts.Communicate(text, voice)
         byte_io = BytesIO()
-        async for chunk in communicate.stream():
-            if chunk["type"] == "audio":
-                byte_io.write(chunk["data"])
+        tts = gTTS(text)
+        tts.write_to_fp(byte_io)
         byte_io.seek(0)
         return byte_io.getvalue()
     except Exception as e:
-        logger.warning(f"Edge TTS Error: {e}")
+        logger.warning(f"google TTS Error: {e}")
         return None
 
 
 async def request_novelai_speech(text):
     """
     Call the NovelAI endpoint to generate synthesized voice.
     :param text: The text to synthesize
@@ -166,8 +164,8 @@
     Call the Reecho endpoint to generate synthesized voice.
     :param text: The text to synthesize
     """
     nai = await request_novelai_speech(text)
     if nai:
         return nai
     else:
-        return await request_edge_speech(text)
+        return await request_google_speech(text)
```

### Comparing `llmkira-1.0.3/llmkira/extra/voice_hook.py` & `llmkira-1.0.4/llmkira/extra/voice_hook.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/kv_manager/_base.py` & `llmkira-1.0.4/llmkira/kv_manager/_base.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/kv_manager/env.py` & `llmkira-1.0.4/llmkira/kv_manager/env.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/kv_manager/file.py` & `llmkira-1.0.4/llmkira/kv_manager/file.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/kv_manager/instruction.py` & `llmkira-1.0.4/llmkira/kv_manager/instruction.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/kv_manager/time.py` & `llmkira-1.0.4/llmkira/kv_manager/time.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/kv_manager/tool_call.py` & `llmkira-1.0.4/llmkira/kv_manager/tool_call.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/memory/__init__.py` & `llmkira-1.0.4/llmkira/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/memory/_base.py` & `llmkira-1.0.4/llmkira/memory/_base.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/memory/local_storage.py` & `llmkira-1.0.4/llmkira/memory/local_storage.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/memory/redis_storage/LICENSE` & `llmkira-1.0.4/llmkira/memory/redis_storage/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/memory/redis_storage/__init__.py` & `llmkira-1.0.4/llmkira/memory/redis_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/memory/redis_storage/utils.py` & `llmkira-1.0.4/llmkira/memory/redis_storage/utils.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/openai/__init__.py` & `llmkira-1.0.4/llmkira/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/openai/_excption.py` & `llmkira-1.0.4/llmkira/openai/_excption.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/openai/cell.py` & `llmkira-1.0.4/llmkira/openai/cell.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/openai/request.py` & `llmkira-1.0.4/llmkira/openai/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -221,21 +221,29 @@
             return OpenAIResult.model_validate(jsoned)
         except Exception as exc:
             logger.exception(exc)
             raise UnexpectedFormatError("Unexpected response format")
 
     @retry(stop=stop_after_attempt(3), reraise=True)
     async def extract(
-        self, response_model: Union[Type[BaseModel], Tool], session: OpenAICredential
+        self, response_model: Union[Type[BaseModel]], session: OpenAICredential
     ):
+        """
+        Extract the result from the response
+        :param response_model: BaseModel
+        :param session: OpenAICredential
+        :return: BaseModel
+        :raises NetworkError, UnexpectedFormatError, RuntimeError: The response model is not matched with the result
+        """
         self.n = 1
         self.response_format = None
-        if not isinstance(response_model, Tool):
-            response_model = Tool(function=response_model)
-        self.tools = [response_model]
-        self.tool_choice = ToolChoice(function=response_model.function)
+        tool = Tool(function=response_model)
+        self.tools = [tool]
+        self.tool_choice = ToolChoice(function=tool.function)
         result = await self.request(session)
         try:
             tool_call = ToolCall.model_validate(result.choices[0].message.tool_calls[0])
-            return response_model.model_validate(tool_call.function.arguments)
-        except Exception:
+            logger.debug(f"Extracted: {tool_call}")
+            return response_model.model_validate(tool_call.function.json_arguments)
+        except Exception as exc:
+            logger.error(f"extract:{exc}")
             raise RuntimeError("The response model is not matched with the result")
```

### Comparing `llmkira-1.0.3/llmkira/openai/utils.py` & `llmkira-1.0.4/llmkira/openai/utils.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/openapi/fuse/__init__.py` & `llmkira-1.0.4/llmkira/openapi/fuse/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/openapi/hook/__init__.py` & `llmkira-1.0.4/llmkira/openapi/hook/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/openapi/trigger/__init__.py` & `llmkira-1.0.4/llmkira/openapi/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/sdk/tools/LICENSE` & `llmkira-1.0.4/llmkira/sdk/tools/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/sdk/tools/__init__.py` & `llmkira-1.0.4/llmkira/sdk/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/sdk/tools/loader.py` & `llmkira-1.0.4/llmkira/sdk/tools/loader.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/sdk/tools/model.py` & `llmkira-1.0.4/llmkira/sdk/tools/model.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/sdk/tools/register.py` & `llmkira-1.0.4/llmkira/sdk/tools/register.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/sdk/tools/schema.py` & `llmkira-1.0.4/llmkira/sdk/tools/schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/sdk/utils.py` & `llmkira-1.0.4/llmkira/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/task/__init__.py` & `llmkira-1.0.4/llmkira/task/__init__.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/task/schema.py` & `llmkira-1.0.4/llmkira/task/schema.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/llmkira/task/snapshot/local.py` & `llmkira-1.0.4/llmkira/task/snapshot/local.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/pyproject.toml` & `llmkira-1.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmkira"
-version = "1.0.3"
+version = "1.0.4"
 description = "A chain message bot based on OpenAI"
 authors = [
     { name = "sudoskys", email = "me@dianas.cyou" },
     { name = "llmkira", email = "me@dianas.cyou" },
 ]
 dependencies = [
     "pathlib>=1.0.1",
@@ -46,30 +46,30 @@
     "requests[socks]<3.0.0,>=2.31.0",
     "feedparser<7.0.0,>=6.0.10",
     "pillow<11.0.0,>=10.1.0",
     "inscriptis<3.0.0,>=2.3.2",
     "aiohttp<4.0.0,>=3.8.6",
     "pytelegrambotapi<5.0.0,>=4.14.0",
     "ffmpeg-python<1.0.0,>=0.2.0",
-    "duckduckgo-search<4.0.0,>=3.9.5",
+    "duckduckgo-search>=5.3.0",
     "flask<4.0.0,>=3.0.0",
     "telegramify-markdown>=0.1.2",
     "json-repair>=0.13.0",
     "curl-cffi>=0.6.2",
     "deprecated>=1.2.14",
     "aiofile>=3.8.8",
     "file-read-backwards>=3.0.0",
     "apscheduler>=3.10.4",
     "montydb[lmdb]>=2.5.2",
     "pymongo>=4.6.3",
     "fast-langdetect>=0.1.0",
     "lmdb>=1.4.1",
-    "edge-tts>=6.1.10",
     "e2b>=0.14.14",
     "e2b-code-interpreter>=0.0.3",
+    "gTTS>=2.5.1",
 ]
 requires-python = ">=3.9,<3.12"
 readme = "README.md"
 keywords = [
     "llmbot",
     "llmkira",
     "openai",
```

### Comparing `llmkira-1.0.3/tests/pydantic_error.py` & `llmkira-1.0.4/tests/pydantic_error.py`

 * *Files identical despite different names*

### Comparing `llmkira-1.0.3/PKG-INFO` & `llmkira-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmkira
-Version: 1.0.3
+Version: 1.0.4
 Summary: A chain message bot based on OpenAI
 Keywords: llmbot,llmkira,openai,chatgpt,llm
 Home-page: https://llmkira.github.io/Docs/
 Author-Email: sudoskys <me@dianas.cyou>, llmkira <me@dianas.cyou>
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -50,30 +50,30 @@
 Requires-Dist: requests[socks]<3.0.0,>=2.31.0
 Requires-Dist: feedparser<7.0.0,>=6.0.10
 Requires-Dist: pillow<11.0.0,>=10.1.0
 Requires-Dist: inscriptis<3.0.0,>=2.3.2
 Requires-Dist: aiohttp<4.0.0,>=3.8.6
 Requires-Dist: pytelegrambotapi<5.0.0,>=4.14.0
 Requires-Dist: ffmpeg-python<1.0.0,>=0.2.0
-Requires-Dist: duckduckgo-search<4.0.0,>=3.9.5
+Requires-Dist: duckduckgo-search>=5.3.0
 Requires-Dist: flask<4.0.0,>=3.0.0
 Requires-Dist: telegramify-markdown>=0.1.2
 Requires-Dist: json-repair>=0.13.0
 Requires-Dist: curl-cffi>=0.6.2
 Requires-Dist: deprecated>=1.2.14
 Requires-Dist: aiofile>=3.8.8
 Requires-Dist: file-read-backwards>=3.0.0
 Requires-Dist: apscheduler>=3.10.4
 Requires-Dist: montydb[lmdb]>=2.5.2
 Requires-Dist: pymongo>=4.6.3
 Requires-Dist: fast-langdetect>=0.1.0
 Requires-Dist: lmdb>=1.4.1
-Requires-Dist: edge-tts>=6.1.10
 Requires-Dist: e2b>=0.14.14
 Requires-Dist: e2b-code-interpreter>=0.0.3
+Requires-Dist: gTTS>=2.5.1
 Requires-Dist: hikari==2.0.0.dev121; extra == "bot"
 Requires-Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "bot"
 Requires-Dist: khl-py<1.0.0,>=0.3.17; extra == "bot"
 Requires-Dist: slack-bolt<2.0.0,>=1.18.0; extra == "bot"
 Requires-Dist: hikari==2.0.0.dev121; extra == "testing"
 Requires-Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "testing"
 Requires-Dist: khl-py<1.0.0,>=0.3.17; extra == "testing"
@@ -159,18 +159,18 @@
 - 📦 Support for plugins to access files
 - 🍟 Multi-platform support – extend new platforms by inheriting the base class
 - 🍔 Plugins can determine their appearance in new sessions dynamically, preventing performance degradation despite large
   amounts of plugins
 
 ### 🍔 Login Modes
 
-- `Login via url`: Use `/login token$https://provider.com` to Login. The program posts the token to the interface to
+- `Login via url`: Use `/login <a token>$<something like https://provider.com/login>` to Login. The program posts the token to the interface to
   retrieve configuration
   information, [how to develop this](https://github.com/LlmKira/Openaibot/blob/81eddbff0f136697d5ad6e13ee1a7477b26624ed/app/components/credential.py#L20).
-- `Login`: Use `/login https://api.com/v1$key$model` to login
+- `Login`: Use `/login https://<api endpoint>/v1$<api key>$<the model>$<tool model such as gpt-3.5-turbo>` to login
 
 ### 🧀 Plugin Can Do More
 
 | Sticker Converter                   | Timer Function(built-in)        |
 |-------------------------------------|---------------------------------|
 | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) |
 
@@ -178,14 +178,15 @@
 
 | Platform | Support | File System | Remarks                                |
 |----------|---------|-------------|----------------------------------------|
 | Telegram | ✅       | ✅           |                                        |
 | Discord  | ✅       | ✅           |                                        |
 | Kook     | ✅       | ✅           | Does not support `triggering by reply` |
 | Slack    | ✅       | ✅           | Does not support `triggering by reply` |
+| Line     | ❌       |             |                                        |
 | QQ       | ❌       |             |                                        |
 | Wechat   | ❌       |             |                                        |
 | Twitter  | ❌       |             |                                        |
 | Matrix   | ❌       |             |                                        |
 | IRC      | ❌       |             |                                        |
 | ...      |         |             | Create Issue/PR                        |
 
@@ -226,14 +227,17 @@
 pdm run python3 start_receiver.py
 # Host
 apt install npm
 npm install pm2 -g
 pm2 start pm2.json
 ```
 
+> **Be sure to change the default password for the command, or disable open ports to prevent the database from being
+scanned and attacked.**
+
 ### 🥣 Docker
 
 Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/docker/sudoskys/llmbot/general)
 
 > Note that if you run this project using Docker, you will start Redis, MongoDB, and RabbitMQ. But if you're running
 > locally, just RabbitMQ
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: llmkira Version: 1.0.3 Summary: A chain message bot
+Metadata-Version: 2.1 Name: llmkira Version: 1.0.4 Summary: A chain message bot
 based on OpenAI Keywords: llmbot,llmkira,openai,chatgpt,llm Home-page: https://
 llmkira.github.io/Docs/ Author-Email: sudoskys
 dianas.cyou>, llmkira
 dianas.cyou> License: Apache-2.0 Classifier: Programming Language :: Python ::
 3 Classifier: Programming Language :: Python :: 3.9 Project-URL: Homepage,
 https://llmkira.github.io/Docs/ Project-URL: Repository, https://github.com/
 LlmKira/Openaibot Requires-Python: <3.12,>=3.9 Requires-Dist: pathlib>=1.0.1
@@ -24,23 +24,23 @@
 Dist: polling<1.0.0,>=0.3.2 Requires-Dist: elara<1.0.0,>=0.5.5 Requires-Dist:
 tzlocal<6.0,>=5.2 Requires-Dist: nltk<4.0.0,>=3.8.1 Requires-Dist:
 jieba<1.0.0,>=0.42.1 Requires-Dist: scikit-learn<2.0.0,>=1.3.2 Requires-Dist:
 cjieba<1.0.0,>=0.4.4 Requires-Dist: requests[socks]<3.0.0,>=2.31.0 Requires-
 Dist: feedparser<7.0.0,>=6.0.10 Requires-Dist: pillow<11.0.0,>=10.1.0 Requires-
 Dist: inscriptis<3.0.0,>=2.3.2 Requires-Dist: aiohttp<4.0.0,>=3.8.6 Requires-
 Dist: pytelegrambotapi<5.0.0,>=4.14.0 Requires-Dist: ffmpeg-
-python<1.0.0,>=0.2.0 Requires-Dist: duckduckgo-search<4.0.0,>=3.9.5 Requires-
-Dist: flask<4.0.0,>=3.0.0 Requires-Dist: telegramify-markdown>=0.1.2 Requires-
-Dist: json-repair>=0.13.0 Requires-Dist: curl-cffi>=0.6.2 Requires-Dist:
+python<1.0.0,>=0.2.0 Requires-Dist: duckduckgo-search>=5.3.0 Requires-Dist:
+flask<4.0.0,>=3.0.0 Requires-Dist: telegramify-markdown>=0.1.2 Requires-Dist:
+json-repair>=0.13.0 Requires-Dist: curl-cffi>=0.6.2 Requires-Dist:
 deprecated>=1.2.14 Requires-Dist: aiofile>=3.8.8 Requires-Dist: file-read-
 backwards>=3.0.0 Requires-Dist: apscheduler>=3.10.4 Requires-Dist: montydb
 [lmdb]>=2.5.2 Requires-Dist: pymongo>=4.6.3 Requires-Dist: fast-
-langdetect>=0.1.0 Requires-Dist: lmdb>=1.4.1 Requires-Dist: edge-tts>=6.1.10
-Requires-Dist: e2b>=0.14.14 Requires-Dist: e2b-code-interpreter>=0.0.3
-Requires-Dist: hikari==2.0.0.dev121; extra == "bot" Requires-Dist: hikari-
+langdetect>=0.1.0 Requires-Dist: lmdb>=1.4.1 Requires-Dist: e2b>=0.14.14
+Requires-Dist: e2b-code-interpreter>=0.0.3 Requires-Dist: gTTS>=2.5.1 Requires-
+Dist: hikari==2.0.0.dev121; extra == "bot" Requires-Dist: hikari-
 crescent<1.0.0,>=0.6.4; extra == "bot" Requires-Dist: khl-py<1.0.0,>=0.3.17;
 extra == "bot" Requires-Dist: slack-bolt<2.0.0,>=1.18.0; extra == "bot"
 Requires-Dist: hikari==2.0.0.dev121; extra == "testing" Requires-Dist: hikari-
 crescent<1.0.0,>=0.6.4; extra == "testing" Requires-Dist: khl-
 py<1.0.0,>=0.3.17; extra == "testing" Requires-Dist: slack-bolt<2.0.0,>=1.18.0;
 extra == "testing" Requires-Dist: pre-commit<3.5.0,>=2.15.0; extra == "testing"
 Provides-Extra: bot Provides-Extra: testing Description-Content-Type: text/
@@ -75,62 +75,63 @@
 constraints, offering fully decoupled logics - ð¬ Offers Login via a URL
 mechanism, providing a flexible and expandable authentication development
 solution - ð° Empowers users to authorize plugin execution. Users can
 configure plugin environment variables at their discretion - ð¦ Support for
 plugins to access files - ð Multi-platform support â extend new platforms
 by inheriting the base class - ð Plugins can determine their appearance in
 new sessions dynamically, preventing performance degradation despite large
-amounts of plugins ### ð Login Modes - `Login via url`: Use `/login
-token$https://provider.com` to Login. The program posts the token to the
-interface to retrieve configuration information, [how to develop this](https://
-github.com/LlmKira/Openaibot/blob/81eddbff0f136697d5ad6e13ee1a7477b26624ed/app/
-components/credential.py#L20). - `Login`: Use `/login https://api.com/
-v1$key$model` to login ### ð§ Plugin Can Do More | Sticker Converter | Timer
-Function(built-in) | |-------------------------------------|-------------------
---------------| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/
-timer_func.gif) | ### ð¬ Platform Support | Platform | Support | File System
-| Remarks | |----------|---------|-------------|-------------------------------
----------| | Telegram | â | â | | | Discord | â | â | | | Kook | â |
-â | Does not support `triggering by reply` | | Slack | â | â | Does not
-support `triggering by reply` | | QQ | â | | | | Wechat | â | | | | Twitter
-| â | | | | Matrix | â | | | | IRC | â | | | | ... | | | Create Issue/PR
-| ## ð¦ Quick Start Refer to the [ð§ Deployment Document](https://
-llmkira.github.io/Docs/) for more information. ### ð¦ One-click Deployment If
-you are using a brand-new server, you can use the following shell to
-automatically install this project. ```shell curl -sSL https://
-raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh | bash ``` ### ð¦
-Manual Installation ```shell # Install Voice dependencies apt install ffmpeg #
-Install RabbitMQ docker pull rabbitmq:3.10-management docker run -d -p 5672:
-5672 -p 15672:15672 \ -e RABBITMQ_DEFAULT_USER=admin \ -
+amounts of plugins ### ð Login Modes - `Login via url`: Use `/login $` to
+Login. The program posts the token to the interface to retrieve configuration
+information, [how to develop this](https://github.com/LlmKira/Openaibot/blob/
+81eddbff0f136697d5ad6e13ee1a7477b26624ed/app/components/credential.py#L20). -
+`Login`: Use `/login https:///v1$$$` to login ### ð§ Plugin Can Do More |
+Sticker Converter | Timer Function(built-in) | |-------------------------------
+------|---------------------------------| | ![sticker](./docs/sticker_func.gif)
+| ![timer](./docs/timer_func.gif) | ### ð¬ Platform Support | Platform |
+Support | File System | Remarks | |----------|---------|-------------|---------
+-------------------------------| | Telegram | â | â | | | Discord | â |
+â | | | Kook | â | â | Does not support `triggering by reply` | | Slack |
+â | â | Does not support `triggering by reply` | | Line | â | | | | QQ |
+â | | | | Wechat | â | | | | Twitter | â | | | | Matrix | â | | | | IRC
+| â | | | | ... | | | Create Issue/PR | ## ð¦ Quick Start Refer to the
+[ð§ Deployment Document](https://llmkira.github.io/Docs/) for more
+information. ### ð¦ One-click Deployment If you are using a brand-new server,
+you can use the following shell to automatically install this project. ```shell
+curl -sSL https://raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh |
+bash ``` ### ð¦ Manual Installation ```shell # Install Voice dependencies apt
+install ffmpeg # Install RabbitMQ docker pull rabbitmq:3.10-management docker
+run -d -p 5672:5672 -p 15672:15672 \ -e RABBITMQ_DEFAULT_USER=admin \ -
 e RABBITMQ_DEFAULT_PASS=8a8a8a \ --hostname myRabbit \ --name rabbitmq \
 rabbitmq:3.10-management docker ps -l # Install Project git clone https://
 github.com/LlmKira/Openaibot/ cd Openaibot pip install pdm pdm install -G bot
 cp .env.exp .env && nano .env # Test pdm run python3 start_sender.py pdm run
 python3 start_receiver.py # Host apt install npm npm install pm2 -g pm2 start
-pm2.json ``` ### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://
-hub.docker.com/repository/docker/sudoskys/llmbot/general) > Note that if you
-run this project using Docker, you will start Redis, MongoDB, and RabbitMQ. But
-if you're running > locally, just RabbitMQ #### Manual Docker-compose
-Installation ```shell git clone https://github.com/LlmKira/Openaibot.git cd
-Openaibot cp .env.exp .env&&nano .env docker-compose -f docker-compose.yml up -
-d ``` The Docker configuration file `docker-compose.yml` contains all
-databases. In fact, Redis and MongoDB are not required. You can remove these
-databases yourself and use the local file system. Update image using `docker-
-compose pull`. Use `docker exec -it llmbot /bin/bash` to view Shell in Docker,
-enter `exit` to exit. ## ðª Slash Commands ```shell clear - Deletes chat
-records help - Displays documentation chat - Conversation task - Use a function
-to converse ask - Disable function-based conversations tool - Lists all
-functions login - Login auth - Authorize a function env - Environment variables
-of the function ``` ## ð» How to Develop Plugins? Refer to the example
-plugins in the `plugins` directory and the [ð§ Plugin Development Document]
-(https://llmkira.github.io/Docs/dev/basic) for plugin development
-documentation. ### Hooks Hooks control the EventMessage in sender and receiver.
-For example, we have `voice_hook` in built-in hooks. you can enable it by
-setting `VOICE_REPLY_ME=true` in `.env`. ```shell /env VOICE_REPLY_ME=yes #
-must /env REECHO_VOICE_KEY= # not must ``` use `/env VOICE_REPLY_ME=NONE` to
-disable this env. check the source code in `llmkira/extra/voice_hook.py`, learn
-to write your own hooks. ## ð§ Sponsor [![sponsor](./.github/
-sponsor_ohmygpt.png)](https://www.ohmygpt.com) ## ð Notice > This project,
-named OpenAiBot, signifying "Open Artificial Intelligence Robot", is not
-officially affiliated with > OpenAI. [![FOSSA Status](https://app.fossa.com/
-api/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://
-app.fossa.com/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
+pm2.json ``` > **Be sure to change the default password for the command, or
+disable open ports to prevent the database from being scanned and attacked.**
+### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/
+docker/sudoskys/llmbot/general) > Note that if you run this project using
+Docker, you will start Redis, MongoDB, and RabbitMQ. But if you're running >
+locally, just RabbitMQ #### Manual Docker-compose Installation ```shell git
+clone https://github.com/LlmKira/Openaibot.git cd Openaibot cp .env.exp
+.env&&nano .env docker-compose -f docker-compose.yml up -d ``` The Docker
+configuration file `docker-compose.yml` contains all databases. In fact, Redis
+and MongoDB are not required. You can remove these databases yourself and use
+the local file system. Update image using `docker-compose pull`. Use `docker
+exec -it llmbot /bin/bash` to view Shell in Docker, enter `exit` to exit. ##
+ðª Slash Commands ```shell clear - Deletes chat records help - Displays
+documentation chat - Conversation task - Use a function to converse ask -
+Disable function-based conversations tool - Lists all functions login - Login
+auth - Authorize a function env - Environment variables of the function ``` ##
+ð» How to Develop Plugins? Refer to the example plugins in the `plugins`
+directory and the [ð§ Plugin Development Document](https://llmkira.github.io/
+Docs/dev/basic) for plugin development documentation. ### Hooks Hooks control
+the EventMessage in sender and receiver. For example, we have `voice_hook` in
+built-in hooks. you can enable it by setting `VOICE_REPLY_ME=true` in `.env`.
+```shell /env VOICE_REPLY_ME=yes # must /env REECHO_VOICE_KEY= # not must ```
+use `/env VOICE_REPLY_ME=NONE` to disable this env. check the source code in
+`llmkira/extra/voice_hook.py`, learn to write your own hooks. ## ð§ Sponsor
+[![sponsor](./.github/sponsor_ohmygpt.png)](https://www.ohmygpt.com) ## ð
+Notice > This project, named OpenAiBot, signifying "Open Artificial
+Intelligence Robot", is not officially affiliated with > OpenAI. [![FOSSA
+Status](https://app.fossa.com/api/projects/
+git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://app.fossa.com/
+projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
```

