# Comparing `tmp/llm_messages_token_helper-0.0.2.tar.gz` & `tmp/llm_messages_token_helper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_messages_token_helper-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "llm_messages_token_helper-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `llm_messages_token_helper-0.0.2.tar` & `llm_messages_token_helper-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0      922 2024-04-04 18:34:36.837406 llm_messages_token_helper-0.0.2/.github/workflows/python.yaml
--rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 llm_messages_token_helper-0.0.2/.gitignore
--rw-r--r--   0        0        0      361 2024-04-04 18:34:36.837821 llm_messages_token_helper-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      238 2024-04-04 19:40:44.165440 llm_messages_token_helper-0.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 llm_messages_token_helper-0.0.2/LICENSE
--rw-r--r--   0        0        0     1850 2024-04-04 20:05:20.458695 llm_messages_token_helper-0.0.2/README.md
--rw-r--r--   0        0        0     1248 2024-04-04 20:06:03.774242 llm_messages_token_helper-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      265 2024-04-04 20:03:54.128074 llm_messages_token_helper-0.0.2/src/llm_messages_token_helper/__init__.py
--rw-r--r--   0        0        0     2020 2024-04-04 19:40:09.278693 llm_messages_token_helper-0.0.2/src/llm_messages_token_helper/images_helper.py
--rw-r--r--   0        0        0     5118 2024-04-04 19:40:53.891278 llm_messages_token_helper-0.0.2/src/llm_messages_token_helper/message_builder.py
--rw-r--r--   0        0        0     2714 2024-04-04 20:03:21.048602 llm_messages_token_helper-0.0.2/src/llm_messages_token_helper/model_helper.py
--rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 llm_messages_token_helper-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 llm_messages_token_helper-0.0.2/tests/image_large.png
--rw-r--r--   0        0        0     1102 2024-04-04 19:40:53.889379 llm_messages_token_helper-0.0.2/tests/test_imageshelper.py
--rw-r--r--   0        0        0     1657 2024-04-04 19:39:50.679963 llm_messages_token_helper-0.0.2/tests/test_messagebuilder.py
--rw-r--r--   0        0        0     2926 2024-04-04 20:05:42.328329 llm_messages_token_helper-0.0.2/tests/test_modelhelper.py
--rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 llm_messages_token_helper-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      880 2024-04-06 22:31:15.975017 llm_messages_token_helper-0.0.3/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 llm_messages_token_helper-0.0.3/.gitignore
+-rw-r--r--   0        0        0      359 2024-04-21 09:43:05.916768 llm_messages_token_helper-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      148 2024-04-21 09:41:40.017866 llm_messages_token_helper-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0      238 2024-04-04 19:40:44.165440 llm_messages_token_helper-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 llm_messages_token_helper-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3577 2024-04-06 22:30:15.500656 llm_messages_token_helper-0.0.3/README.md
+-rw-r--r--   0        0        0     1312 2024-04-21 09:42:16.739822 llm_messages_token_helper-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      265 2024-04-04 20:03:54.128074 llm_messages_token_helper-0.0.3/src/llm_messages_token_helper/__init__.py
+-rw-r--r--   0        0        0     2020 2024-04-04 19:40:09.278693 llm_messages_token_helper-0.0.3/src/llm_messages_token_helper/images_helper.py
+-rw-r--r--   0        0        0     5118 2024-04-04 19:40:53.891278 llm_messages_token_helper-0.0.3/src/llm_messages_token_helper/message_builder.py
+-rw-r--r--   0        0        0     3048 2024-04-21 10:09:08.980475 llm_messages_token_helper-0.0.3/src/llm_messages_token_helper/model_helper.py
+-rw-r--r--   0        0        0        0 2024-04-20 21:23:37.657516 llm_messages_token_helper-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 llm_messages_token_helper-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 llm_messages_token_helper-0.0.3/tests/image_large.png
+-rw-r--r--   0        0        0     1448 2024-04-21 10:04:18.753438 llm_messages_token_helper-0.0.3/tests/messages.py
+-rw-r--r--   0        0        0     1102 2024-04-04 19:40:53.889379 llm_messages_token_helper-0.0.3/tests/test_imageshelper.py
+-rw-r--r--   0        0        0     1726 2024-04-21 10:10:55.349835 llm_messages_token_helper-0.0.3/tests/test_messagebuilder.py
+-rw-r--r--   0        0        0     2229 2024-04-21 10:10:55.349956 llm_messages_token_helper-0.0.3/tests/test_modelhelper.py
+-rw-r--r--   0        0        0     1604 2024-04-21 10:10:55.349842 llm_messages_token_helper-0.0.3/tests/verify_openai.py
+-rw-r--r--   0        0        0     4664 1970-01-01 00:00:00.000000 llm_messages_token_helper-0.0.3/PKG-INFO
```

### Comparing `llm_messages_token_helper-0.0.2/.github/workflows/python.yaml` & `llm_messages_token_helper-0.0.3/.github/workflows/python.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jobs:
   build:
     name: Test with Python ${{ matrix.python_version }}
     runs-on: ubuntu-latest
     strategy:
         fail-fast: false
         matrix:
-          python_version: ["3.8", "3.9", "3.10", "3.11"]
+          python_version: ["3.9", "3.10", "3.11", "3.12"]
     steps:
         - uses: actions/checkout@v3
         - name: Set up Python 3
           uses: actions/setup-python@v3
           with:
             python-version: ${{ matrix.python_version }}
         - name: Install dependencies
@@ -26,9 +26,8 @@
             python3 -m pip install -e '.[dev]'
         - name: Lint with ruff
           run: ruff .
         - name: Check formatting with black
           run: black . --check --verbose
         - name: Run unit tests
           run: |
-            playwright install --with-deps
             python3 -m pytest
```

### Comparing `llm_messages_token_helper-0.0.2/.gitignore` & `llm_messages_token_helper-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_messages_token_helper-0.0.2/LICENSE` & `llm_messages_token_helper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_messages_token_helper-0.0.2/pyproject.toml` & `llm_messages_token_helper-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "llm-messages-token-helper"
 description = "A helper library for estimating tokens used by messages."
-version = "0.0.2"
+version = "0.0.3"
 authors = [{name = "Pamela Fox"}]
 requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "openai",
     "tiktoken",
@@ -29,26 +29,30 @@
 dev = [
     "pytest",
     "pytest-cov",
     "pre-commit",
     "ruff",
     "black",
     "flit",
+    "azure-identity",
+    "python-dotenv"
 ]
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.ruff]
 line-length = 120
 target-version = "py39"
+output-format = "full"
+
+[tool.ruff.lint]
 select = ["E", "F", "I", "UP"]
 ignore = ["D203", "E501"]
-show-source = true
 
 [tool.black]
 line-length = 120
 target-version = ["py39"]
 
 [tool.pytest.ini_options]
 addopts = "-ra --cov"
```

### Comparing `llm_messages_token_helper-0.0.2/src/llm_messages_token_helper/images_helper.py` & `llm_messages_token_helper-0.0.3/src/llm_messages_token_helper/images_helper.py`

 * *Files identical despite different names*

### Comparing `llm_messages_token_helper-0.0.2/src/llm_messages_token_helper/message_builder.py` & `llm_messages_token_helper-0.0.3/src/llm_messages_token_helper/message_builder.py`

 * *Files identical despite different names*

### Comparing `llm_messages_token_helper-0.0.2/src/llm_messages_token_helper/model_helper.py` & `llm_messages_token_helper-0.0.3/src/llm_messages_token_helper/model_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,42 +31,50 @@
     if model not in MODELS_2_TOKEN_LIMITS:
         raise ValueError(f"Called with unknown model name: {model}")
     return MODELS_2_TOKEN_LIMITS[model]
 
 
 def count_tokens_for_message(model: str, message: Mapping[str, object]) -> int:
     """
-    Calculate the number of tokens required to encode a message.
+    Calculate the number of tokens required to encode a message. Based off cookbook:
+    https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
+
     Args:
         model (str): The name of the model to use for encoding.
         message (Mapping): The message to encode, in a dictionary-like object.
     Returns:
         int: The total number of tokens required to encode the message.
 
     >> model = 'gpt-3.5-turbo'
     >> message = {'role': 'user', 'content': 'Hello, how are you?'}
     >> count_tokens_for_message(model, message)
-    11
+    13
     """
 
     encoding = tiktoken.encoding_for_model(get_oai_chatmodel_tiktok(model))
-    num_tokens = 2  # For "role" and "content" keys
-    for value in message.values():
+    # Assumes we're using a recent model
+    tokens_per_message = 3
+
+    num_tokens = tokens_per_message
+    for key, value in message.items():
         if isinstance(value, list):
             # For GPT-4-vision support, based on https://github.com/openai/openai-cookbook/pull/881/files
             for item in value:
-                num_tokens += len(encoding.encode(item["type"]))
+                # Note: item[type] does not seem to be counted in the token count
                 if item["type"] == "text":
                     num_tokens += len(encoding.encode(item["text"]))
                 elif item["type"] == "image_url":
                     num_tokens += count_tokens_for_image(item["image_url"]["url"], item["image_url"]["detail"])
         elif isinstance(value, str):
             num_tokens += len(encoding.encode(value))
         else:
             raise ValueError(f"Could not encode unsupported message value type: {type(value)}")
+        if key == "name":
+            num_tokens += 1
+    num_tokens += 3  # every reply is primed with <|start|>assistant<|message|>
     return num_tokens
 
 
 def get_oai_chatmodel_tiktok(aoaimodel: str) -> str:
     message = "Expected valid OpenAI GPT model name"
     if aoaimodel == "" or aoaimodel is None:
         raise ValueError(message)
```

### Comparing `llm_messages_token_helper-0.0.2/tests/image_large.png` & `llm_messages_token_helper-0.0.3/tests/image_large.png`

 * *Files identical despite different names*

### Comparing `llm_messages_token_helper-0.0.2/tests/test_imageshelper.py` & `llm_messages_token_helper-0.0.3/tests/test_imageshelper.py`

 * *Files identical despite different names*

