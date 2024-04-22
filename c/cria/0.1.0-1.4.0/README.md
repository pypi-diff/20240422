# Comparing `tmp/cria-0.1.0.tar.gz` & `tmp/cria-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cria-0.1.0.tar", max compression
+gzip compressed data, was "cria-1.4.0.tar", max compression
```

## Comparing `cria-0.1.0.tar` & `cria-1.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2024-04-21 05:19:02.669800 cria-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1018 2024-04-21 02:53:50.000000 cria-0.1.0/README.md
--rw-r--r--   0        0        0      804 2024-04-21 05:17:58.333863 cria-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7864 2024-04-21 05:03:11.000000 cria-0.1.0/src/cria.py
--rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 cria-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-22 00:39:23.969351 cria-1.4.0/LICENSE.md
+-rw-r--r--   0        0        0     7300 2024-04-22 00:39:23.969351 cria-1.4.0/README.md
+-rw-r--r--   0        0        0      824 2024-04-22 00:39:23.969351 cria-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8102 2024-04-22 00:39:23.969351 cria-1.4.0/src/cria.py
+-rw-r--r--   0        0        0     7939 1970-01-01 00:00:00.000000 cria-1.4.0/PKG-INFO
```

### Comparing `cria-0.1.0/LICENSE.md` & `cria-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cria-0.1.0/pyproject.toml` & `cria-1.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cria"
-version = "1.2"
+version = "1.4.0"
 authors = [{ name = "leftmove", email = "100anonyo@gmail.com" }]
 description = "Run AI locally with as little friction as possible"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -13,21 +13,22 @@
 
 [project.urls]
 Homepage = "https://github.com/leftmove/cria"
 Issues = "https://github.com/leftmove/cria/issues"
 
 [tool.poetry]
 name = "cria"
-version = "0.1.0"
+version = "1.4.0"
 description = "Run AI locally with as little friction as possible."
 authors = ["leftmove"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 ollama = "^0.1.8"
+psutil = "^5.9.8"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cria-0.1.0/src/cria.py` & `cria-1.4.0/src/cria.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,26 @@
     model_match = next(
         (True if m.get("name") == model else False for m in model_list), False
     )
     if model_match:
         return
 
     if not silence_output:
-        print(f"LLM model not found, downloading '{model}'...")
+        print(f"LLM model not found, searching '{model}'...")
 
     try:
-        ollama.pull(model)
+        progress = ollama.pull(model, stream=True)
+        print(
+            f"LLM model {model} found, downloading... (this will probably take a while)"
+        )
         if not silence_output:
+            for chunk in progress:
+                print(chunk)
             print(f"'{model}' downloaded, starting processes.")
+        return model
     except Exception as e:
         print(e)
         raise ValueError(
             "Invalid model passed. See the model library here: https://ollama.com/library"
         )
 
 
@@ -96,43 +102,45 @@
         return response
 
     def generate_stream(self, prompt):
         model = self.model
         ai = ollama
 
         for chunk in ai.generate(model=model, prompt=prompt, stream=True):
-            content = chunk["message"]["content"]
+            content = chunk["response"]
             yield content
 
     def generate(
         self,
         prompt: str,
         stream: Optional[bool] = True,
     ) -> str:
         model = self.model
         ai = ollama
 
         if stream:
             return self.generate_stream(prompt)
 
-        response = ai.generate(model=model, prompt=prompt, stream=False)
+        chunk = ai.generate(model=model, prompt=prompt, stream=False)
+        response = chunk["response"]
+
         return response
 
     def clear(self):
         self.messages = [
             {"role": "system", "content": "You are a helpful AI assistant."}
         ]
 
 
 class Cria(Client):
     def __init__(
         self,
         model: Optional[str] = DEFAULT_MODEL,
+        standalone: Optional[bool] = False,
         run_subprocess: Optional[bool] = False,
-        run_llm: Optional[bool] = True,
         capture_output: Optional[bool] = False,
         silence_output: Optional[bool] = False,
         close_on_exit: Optional[bool] = True,
     ) -> None:
         self.run_subprocess = run_subprocess
         self.capture_output = capture_output
         self.silence_output = silence_output
@@ -182,25 +190,25 @@
                     retries -= 1
         else:
             self.ollama_subrprocess = None
 
         model = check_models(model, silence_output)
         self.model = model
 
-        if run_llm:
+        if not standalone:
             self.llm = subprocess.Popen(
                 ["ollama", "run", model],
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
             )
 
         if close_on_exit and self.ollama_subrprocess:
             atexit.register(lambda: self.ollama_subrprocess.kill())
 
-        if close_on_exit and run_llm:
+        if close_on_exit and not standalone:
             atexit.register(lambda: self.llm.kill())
 
     def output(self):
         ollama_subprocess = self.ollama_subrprocess
         if not ollama_subprocess:
             raise ValueError(
                 "Ollama is not running as a subprocess, you must pass run_subprocess as True to capture output."
@@ -224,16 +232,16 @@
         capture_output: Optional[bool] = False,
         silence_output: Optional[bool] = False,
         close_on_exit: Optional[bool] = True,
     ) -> None:
         super().__init__(
             model=model,
             capture_output=capture_output,
-            run_subprocess=True if capture_output else False,
-            run_llm=False,
+            run_subprocess=False,
+            standalone=True,
             close_on_exit=close_on_exit,
         )
 
         self.capture_output = capture_output
         self.silence_output = silence_output
         self.close_on_exit = close_on_exit
```

