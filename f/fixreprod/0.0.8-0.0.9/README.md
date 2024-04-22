# Comparing `tmp/fixreprod-0.0.8.tar.gz` & `tmp/fixreprod-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixreprod-0.0.8.tar", last modified: Fri Aug 11 06:16:38 2023, max compression
+gzip compressed data, was "fixreprod-0.0.9.tar", last modified: Sat Aug 12 10:38:29 2023, max compression
```

## Comparing `fixreprod-0.0.8.tar` & `fixreprod-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-11 06:16:38.556298 fixreprod-0.0.8/
--rw-r--r--   0 yt        (1000) yt        (1000)     1848 2023-08-11 06:16:38.555289 fixreprod-0.0.8/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1322 2023-08-11 06:10:31.000000 fixreprod-0.0.8/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-08-11 06:16:38.556298 fixreprod-0.0.8/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      949 2023-08-11 06:16:01.000000 fixreprod-0.0.8/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-11 06:16:38.538342 fixreprod-0.0.8/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-11 06:16:38.554133 fixreprod-0.0.8/src/fixreprod.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1848 2023-08-11 06:16:38.000000 fixreprod-0.0.8/src/fixreprod.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      223 2023-08-11 06:16:38.000000 fixreprod-0.0.8/src/fixreprod.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-08-11 06:16:38.000000 fixreprod-0.0.8/src/fixreprod.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       46 2023-08-11 06:16:38.000000 fixreprod-0.0.8/src/fixreprod.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       10 2023-08-11 06:16:38.000000 fixreprod-0.0.8/src/fixreprod.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     3395 2023-08-11 06:15:35.000000 fixreprod-0.0.8/src/fixreprod.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-12 10:38:29.861668 fixreprod-0.0.9/
+-rw-r--r--   0 yt        (1000) yt        (1000)     2700 2023-08-12 10:38:29.860645 fixreprod-0.0.9/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     2174 2023-08-12 10:36:03.000000 fixreprod-0.0.9/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-08-12 10:38:29.861668 fixreprod-0.0.9/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      949 2023-08-12 10:37:44.000000 fixreprod-0.0.9/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-12 10:38:29.844992 fixreprod-0.0.9/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-12 10:38:29.844992 fixreprod-0.0.9/src/fixreprod.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     2700 2023-08-12 10:38:29.000000 fixreprod-0.0.9/src/fixreprod.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      223 2023-08-12 10:38:29.000000 fixreprod-0.0.9/src/fixreprod.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-08-12 10:38:29.000000 fixreprod-0.0.9/src/fixreprod.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       46 2023-08-12 10:38:29.000000 fixreprod-0.0.9/src/fixreprod.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       10 2023-08-12 10:38:29.000000 fixreprod-0.0.9/src/fixreprod.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     3647 2023-08-12 10:23:11.000000 fixreprod-0.0.9/src/fixreprod.py
```

### Comparing `fixreprod-0.0.8/PKG-INFO` & `fixreprod-0.0.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixreprod
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for showing all seeds to be fixed
 Home-page: https://github.com/ytakefuji/fixreprod
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/fixreprod
 Platform: UNKNOWN
@@ -15,35 +15,44 @@
 Description-Content-Type: text/markdown
 
 # fixreprod
 This is under review.
 
 It is still undergoing improvement.
 
-fixreprod is an indispensable tool to solve reproducibility problems in pseudorandom numbers by fixing all seeds used in libraries of AI systems.
+fixreprod is an indispensable tool to solve reproducibility problems in pseudorandom numbers by fixing all seeds and deterministic algorithms used in libraries of AI systems.
 
-To run fixreprod, install it by the following commanad. ($) indicates the prompt from the system in the terminal.
+To run fixreprod, install it by the following command. ($) indicates the prompt from the system in the terminal.
 
 $ pip install fixreprod
 
 # How to run fixreprod
 
 For example, assume reinforcement_q_learning.py is a source code. Use grep command to generate test.py.
-test.py contains imported libraries which will be checked by fixreprod.
+test.py contains imported libraries which will be checked by fixreprod. The sed command sed '/^"""/,/^"""/d' removes comment lines from reinforcement_q_learning.py and saves it in reinfo.py. The first grep command removes comment lines with the first character of "#" from reinfo.py and save it in rein.py. The second grep command extracts imported libraries from rein.py and save it in test.py.
 
-$ grep import cartpole_reinforce.py >test.py
+$ grep import reinforcement_q_learning.py >test.py
+
+or To see the code only, run the following commands
+
+$ sed '/^"""/,/^"""/d' reinforcement_q_learning.py >reinfo.py
+
+$ grep -v '^#' reinfo.py >rein.py
+
+$ grep import rein.py >test.py
 
 Before running fixreprod, you must install all libraries used in the source code.
 In reinforcement_q_learning.py, gym, random, numpy, and torch must be installed.
 
 <pre>
 Run fixrepdod and enter "test.py" for checking.
 fixreprod will show the all seeds to be fixed to eliminate 
 reproducibility problems from your code. 
-9 seeds and 1 fixing deterministic algorithms are found in this example.
+9 seeds and 1 fixing deterministic algorithms are found 
+  in this example.
   
 $ fixreprod
 Enter the source code file name: test.py
 env.action_space.seed(0)
 env.reset(seed=0)
 np.random.seed(0)
 random.Random().seed(0)
@@ -51,9 +60,12 @@
 torch.Generator().manual_seed(0)        
 torch.cuda.manual_seed(0)
 torch.cuda.manual_seed_all(0)
 torch.manual_seed(0)
 torch.use_deterministic_algorithms(True)
 
 </pre>
+These generated codes should be embedded in the rein.py or reinforcement_q_learning.py. The following figure shows the producible result. When chaning seed numbers, the different reproducible result can be obtained.
+
+<img src='https://github.com/ytakefuji/fixreprod/raw/main/result.png' width=540 hight=480>
```

### Comparing `fixreprod-0.0.8/setup.py` & `fixreprod-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fixreprod",
-    version="0.0.8",
+    version="0.0.9",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for showing all seeds to be fixed",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/fixreprod",
     project_urls={
```

### Comparing `fixreprod-0.0.8/src/fixreprod.egg-info/PKG-INFO` & `fixreprod-0.0.9/src/fixreprod.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixreprod
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for showing all seeds to be fixed
 Home-page: https://github.com/ytakefuji/fixreprod
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/fixreprod
 Platform: UNKNOWN
@@ -15,35 +15,44 @@
 Description-Content-Type: text/markdown
 
 # fixreprod
 This is under review.
 
 It is still undergoing improvement.
 
-fixreprod is an indispensable tool to solve reproducibility problems in pseudorandom numbers by fixing all seeds used in libraries of AI systems.
+fixreprod is an indispensable tool to solve reproducibility problems in pseudorandom numbers by fixing all seeds and deterministic algorithms used in libraries of AI systems.
 
-To run fixreprod, install it by the following commanad. ($) indicates the prompt from the system in the terminal.
+To run fixreprod, install it by the following command. ($) indicates the prompt from the system in the terminal.
 
 $ pip install fixreprod
 
 # How to run fixreprod
 
 For example, assume reinforcement_q_learning.py is a source code. Use grep command to generate test.py.
-test.py contains imported libraries which will be checked by fixreprod.
+test.py contains imported libraries which will be checked by fixreprod. The sed command sed '/^"""/,/^"""/d' removes comment lines from reinforcement_q_learning.py and saves it in reinfo.py. The first grep command removes comment lines with the first character of "#" from reinfo.py and save it in rein.py. The second grep command extracts imported libraries from rein.py and save it in test.py.
 
-$ grep import cartpole_reinforce.py >test.py
+$ grep import reinforcement_q_learning.py >test.py
+
+or To see the code only, run the following commands
+
+$ sed '/^"""/,/^"""/d' reinforcement_q_learning.py >reinfo.py
+
+$ grep -v '^#' reinfo.py >rein.py
+
+$ grep import rein.py >test.py
 
 Before running fixreprod, you must install all libraries used in the source code.
 In reinforcement_q_learning.py, gym, random, numpy, and torch must be installed.
 
 <pre>
 Run fixrepdod and enter "test.py" for checking.
 fixreprod will show the all seeds to be fixed to eliminate 
 reproducibility problems from your code. 
-9 seeds and 1 fixing deterministic algorithms are found in this example.
+9 seeds and 1 fixing deterministic algorithms are found 
+  in this example.
   
 $ fixreprod
 Enter the source code file name: test.py
 env.action_space.seed(0)
 env.reset(seed=0)
 np.random.seed(0)
 random.Random().seed(0)
@@ -51,9 +60,12 @@
 torch.Generator().manual_seed(0)        
 torch.cuda.manual_seed(0)
 torch.cuda.manual_seed_all(0)
 torch.manual_seed(0)
 torch.use_deterministic_algorithms(True)
 
 </pre>
+These generated codes should be embedded in the rein.py or reinforcement_q_learning.py. The following figure shows the producible result. When chaning seed numbers, the different reproducible result can be obtained.
+
+<img src='https://github.com/ytakefuji/fixreprod/raw/main/result.png' width=540 hight=480>
```

### Comparing `fixreprod-0.0.8/src/fixreprod.py` & `fixreprod-0.0.9/src/fixreprod.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,26 +30,26 @@
 
   Args:
     source_code: The source code to initialize seeds for.
 
   Returns:
     A new code with all seeds initialized.
   """
-
   new_code = ""
   aliases = {}
   for line in source_code.splitlines():
     match = re.search(r"import\s+([a-zA-Z0-9_.]+)(?:\s+as\s+([a-zA-Z0-9_]+))?\s*", line)
     if match:
       library = match.group(1)
       alias = match.group(2) or library
       aliases[alias] = library
       try:
         module = importlib.import_module(library)
         for m in module.__dict__.keys():
+          if m=='experimental': tff1=1
           if hasattr(getattr(module, m), "seed"):
             if library == "gym":
               new_code += f"env.reset(seed=0)\n"
               new_code += f"env.action_space.seed(0)\n"
             elif library == "gymnasium":
               new_code += f"env.reset(seed=0)\n"
               new_code += f"env.action_space.seed(0)\n"
@@ -64,16 +64,20 @@
                 new_code += f"{alias}.{m}(0)\n"
               elif m == "initial_seed":
                 new_code += f"{alias}.{m}()\n"
               elif m == "cuda":
                 new_code += f"{alias}.{m}.manual_seed(0)\n"
                 new_code += f"{alias}.{m}.manual_seed_all(0)\n"
             elif library == "tensorflow":
-              if m == "set_seed":
-                new_code += f"{alias}.random.{m}({random.randint(0, 1)})\n"
+              new_code += f"{alias}.random.set_seed(0)\n"
+              if tff1==1: 
+                new_code += f"{alias}.experimental.numpy.random.seed(0)\n"
+                new_code += f"{alias}.keras.utils.set_random_seed(0)\n"
+            elif library == "pylab":
+              new_code += f"{alias}.seed(0)\n"
             elif library == "random":
               if m == "Random":
                 new_code += f"{alias}.{m}().seed(0)\n"
                 new_code += f"{alias}.seed(0)\n"
             else:
               new_code += f"{alias}.{m}.seed(0)\n"
       except (ModuleNotFoundError, AttributeError):
@@ -85,14 +89,16 @@
   lines = list(set(new_code.splitlines()))
   lines.sort()
   for line in lines:
    if "F.torch.seed" in line:
     lines.remove(line)
   return lines
 
+tff1=0
+
 def main():
   source_code = input("Enter the source code file name: ")
   with open(source_code, "r") as f:
     source_code = f.read()
 
   if check_for_random_numbers(source_code):
     new_code = initialize_seeds(source_code)
```

