# Comparing `tmp/bedrock_bot-1.0.3.tar.gz` & `tmp/bedrock_bot-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedrock_bot-1.0.3.tar", max compression
+gzip compressed data, was "bedrock_bot-1.0.4.tar", max compression
```

## Comparing `bedrock_bot-1.0.3.tar` & `bedrock_bot-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/LICENSE
--rw-r--r--   0        0        0     2598 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/README.md
--rw-r--r--   0        0        0       91 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/bedrock_bot/__init__.py
--rw-r--r--   0        0        0     2290 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/bedrock_bot/cli.py
--rw-r--r--   0        0        0     3173 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/bedrock_bot/model.py
--rw-r--r--   0        0        0      152 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/bedrock_bot/util.py
--rw-r--r--   0        0        0      448 2024-04-22 04:14:39.208230 bedrock_bot-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-22 04:49:22.380629 bedrock_bot-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2598 2024-04-22 04:49:22.380629 bedrock_bot-1.0.4/README.md
+-rw-r--r--   0        0        0       91 2024-04-22 04:49:22.380629 bedrock_bot-1.0.4/bedrock_bot/__init__.py
+-rw-r--r--   0        0        0     2452 2024-04-22 04:49:22.380629 bedrock_bot-1.0.4/bedrock_bot/cli.py
+-rw-r--r--   0        0        0     3173 2024-04-22 04:49:22.380629 bedrock_bot-1.0.4/bedrock_bot/model.py
+-rw-r--r--   0        0        0      152 2024-04-22 04:49:22.380629 bedrock_bot-1.0.4/bedrock_bot/util.py
+-rw-r--r--   0        0        0      448 2024-04-22 04:49:22.380629 bedrock_bot-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 bedrock_bot-1.0.4/PKG-INFO
```

### Comparing `bedrock_bot-1.0.3/LICENSE` & `bedrock_bot-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.3/README.md` & `bedrock_bot-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.3/bedrock_bot/cli.py` & `bedrock_bot-1.0.4/bedrock_bot/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,22 +19,23 @@
             f"Invalid value: {value}. Allowed values are: {available_models}"
         )
 
 
 @click.command()
 @click.argument("args", nargs=-1)
 @click.option("-r", "--region", help="The AWS region to use for requests")
+@click.option("--raw-output", help="Don't interpret markdown in the AI response")
 @click.option(
     "-m",
     "--model",
     type=click.Choice(available_models(), case_sensitive=False),
     default="Claude-3-Haiku",
     help="The model to use for requests",
 )
-def main(model, region, args):
+def main(model, region, raw_output args):
     model = model_class_from_input(model)
 
     boto_config = Config()
     if region:
         boto_config = Config(region_name=region)
 
     instance = model(boto_config=boto_config)
@@ -73,10 +74,13 @@
         ):
             print("\nResetting...")
             instance.reset()
             continue
 
         response = instance.invoke(user_input)
 
-        formatted_print(response)
+        if raw_output:
+            print(response)
+        else:
+            formatted_print(response)
 
         print()
```

### Comparing `bedrock_bot-1.0.3/bedrock_bot/model.py` & `bedrock_bot-1.0.4/bedrock_bot/model.py`

 * *Files identical despite different names*

### Comparing `bedrock_bot-1.0.3/PKG-INFO` & `bedrock_bot-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bedrock-bot
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

