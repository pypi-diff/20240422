# Comparing `tmp/llama_index_readers_slack-0.1.3.tar.gz` & `tmp/llama_index_readers_slack-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_slack-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_readers_slack-0.1.4.tar", max compression
```

## Comparing `llama_index_readers_slack-0.1.3.tar` & `llama_index_readers_slack-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       40 2024-02-13 13:53:01.872611 llama_index_readers_slack-0.1.3/README.md
--rw-r--r--   0        0        0       82 2024-02-13 13:53:01.872804 llama_index_readers_slack-0.1.3/llama_index/readers/slack/__init__.py
--rw-r--r--   0        0        0     8559 2024-02-13 13:53:01.873098 llama_index_readers_slack-0.1.3/llama_index/readers/slack/base.py
--rw-r--r--   0        0        0     1480 2024-02-21 20:51:22.014898 llama_index_readers_slack-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 llama_index_readers_slack-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       40 2024-04-22 02:39:35.234728 llama_index_readers_slack-0.1.4/README.md
+-rw-r--r--   0        0        0       82 2024-04-22 02:39:35.234728 llama_index_readers_slack-0.1.4/llama_index/readers/slack/__init__.py
+-rw-r--r--   0        0        0     8585 2024-04-22 02:39:35.234728 llama_index_readers_slack-0.1.4/llama_index/readers/slack/base.py
+-rw-r--r--   0        0        0     1480 2024-04-22 02:39:35.234728 llama_index_readers_slack-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 llama_index_readers_slack-0.1.4/PKG-INFO
```

### Comparing `llama_index_readers_slack-0.1.3/llama_index/readers/slack/base.py` & `llama_index_readers_slack-0.1.4/llama_index/readers/slack/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
                         "Rate limit error reached, sleeping for: {} seconds".format(
                             e.response.headers["retry-after"]
                         )
                     )
                     time.sleep(int(e.response.headers["retry-after"]))
                 else:
                     logger.error(f"Error parsing conversation replies: {e}")
+                    break
 
         return "\n\n".join(messages_text)
 
     def _read_channel(self, channel_id: str, reverse_chronological: bool) -> str:
         from slack_sdk.errors import SlackApiError
 
         """Read a channel."""
```

### Comparing `llama_index_readers_slack-0.1.3/pyproject.toml` & `llama_index_readers_slack-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers slack integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["jerryjliu"]
 name = "llama-index-readers-slack"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 slack-sdk = "^3.26.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_readers_slack-0.1.3/PKG-INFO` & `llama_index_readers_slack-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-slack
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index readers slack integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Maintainer: jerryjliu
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: slack-sdk (>=3.26.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Readers Integration: Slack
```

