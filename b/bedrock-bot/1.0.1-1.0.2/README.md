# Comparing `tmp/bedrock_bot-1.0.1.tar.gz` & `tmp/bedrock_bot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrock_bot-1.0.1.tar", max compression
+gzip compressed data, was "bedrock_bot-1.0.2.tar", max compression
```

## Comparing `bedrock_bot-1.0.1.tar` & `bedrock_bot-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/LICENSE
--rw-r--r--   0        0        0     1668 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/README.md
--rw-r--r--   0        0        0       91 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/bedrock_bot/__init__.py
--rw-r--r--   0        0        0     2290 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/bedrock_bot/cli.py
--rw-r--r--   0        0        0     3209 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/bedrock_bot/model.py
--rw-r--r--   0        0        0      152 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/bedrock_bot/util.py
--rw-r--r--   0        0        0      448 2024-04-21 04:47:08.430033 bedrock_bot-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2171 1970-01-01 00:00:00.000000 bedrock_bot-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2598 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/README.md
+-rw-r--r--   0        0        0       91 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/bedrock_bot/__init__.py
+-rw-r--r--   0        0        0     2290 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/bedrock_bot/cli.py
+-rw-r--r--   0        0        0     3209 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/bedrock_bot/model.py
+-rw-r--r--   0        0        0      152 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/bedrock_bot/util.py
+-rw-r--r--   0        0        0      448 2024-04-21 04:55:05.046810 bedrock_bot-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.0.2/PKG-INFO
```

### Comparing `bedrock_bot-1.0.1/LICENSE` & `bedrock_bot-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.1/bedrock_bot/cli.py` & `bedrock_bot-1.0.2/bedrock_bot/cli.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.1/bedrock_bot/model.py` & `bedrock_bot-1.0.2/bedrock_bot/model.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.1/PKG-INFO` & `bedrock_bot-1.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-Metadata-Version: 2.1
-Name: bedrock-bot
-Version: 1.0.1
-Summary: 
-Author: Justin Dray
-Author-email: justin@dray.be
-Requires-Python: >=3.10,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: boto3 (>=1.34.88,<2.0.0)
-Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: rich (>=13.7.1,<14.0.0)
-Description-Content-Type: text/markdown
-
 # Bedrock Bot
 
 This project is a basic CLI-based chat bot that uses Bedrock to resolve questions. It can take input from stdin, CLI arguments or interactively when no parameters have been passed.
 
 ## Installation
 
-`pip install bedrock-bot`
+1. `pip install bedrock-bot`
+2. You will also need some AWS credentials available in your shell (any usual way works - CLI configured IAM user access key/secret keys, environment variables, etc)
+3. Bedrock requires you to opt in to models in order to use them
 
 ## Usage
 
+```bash
+bedrock --help
+Usage: bedrock [OPTIONS] [ARGS]...
+
+Options:
+  -r, --region TEXT               The AWS region to use for requests
+  -m, --model [Claude-3-Haiku|Claude-3-Sonnet]
+                                  The model to use for requests
+  --help                          Show this message and exit.
+```
+
 Directly as a chat bot:
 
 ```bash
 $ bedrock
 
 Hello! I am an AI assistant powered by Amazon Bedrock and using the model Claude-3-Haiku. Enter 'quit' or 'exit' at any time to exit. How may I help you today?
 (You can clear existing context by starting a query with 'new>' or 'reset>')
@@ -61,7 +58,20 @@
 
 My name is Claude. I'm an AI created by Anthropic. It's nice to meet you!                                                         
 
 
 Note that you can only do one-shot requests when providing input via stdin
 ```
 
+## Shell auto-complete
+
+Shell auto-complete is also supported.
+
+### ZSH
+
+1. `_BEDROCK_COMPLETE=zsh_source bedrock > ~/.bedrock-completion.zsh`
+2. Add the following to your `~/.zshrc`: `source ~/.bedrock-completion.zsh`
+
+### Bash
+
+1. `_BEDROCK_COMPLETE=bash_source bedrock > ~/.bedrock-completion.bash`
+2. Add the following to your `~/.bashrc`: `source ~/.bedrock-completion.bash`
```

