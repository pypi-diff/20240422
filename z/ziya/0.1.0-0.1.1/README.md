# Comparing `tmp/ziya-0.1.0.tar.gz` & `tmp/ziya-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziya-0.1.0.tar", max compression
+gzip compressed data, was "ziya-0.1.1.tar", max compression
```

## Comparing `ziya-0.1.0.tar` & `ziya-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1072 2024-04-22 02:58:39.685068 ziya-0.1.0/LICENSE
--rw-r--r--   0        0        0     1623 2024-04-22 02:58:39.715796 ziya-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-21 06:06:04.634589 ziya-0.1.0/app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 02:58:39.701319 ziya-0.1.0/app/agents/__init__.py
--rw-r--r--   0        0        0     4181 2024-04-22 02:58:39.711578 ziya-0.1.0/app/agents/agent.py
--rw-r--r--   0        0        0     1674 2024-04-22 02:58:39.703511 ziya-0.1.0/app/agents/prompts.py
--rw-r--r--   0        0        0     1359 2024-04-22 02:58:39.715941 ziya-0.1.0/app/main.py
--rw-r--r--   0        0        0      676 2024-04-22 02:58:39.702097 ziya-0.1.0/app/server.py
--rw-r--r--   0        0        0        0 2024-04-22 02:58:39.679175 ziya-0.1.0/app/utils/__init__.py
--rw-r--r--   0        0        0     2132 2024-04-22 02:58:39.690886 ziya-0.1.0/app/utils/directory_util.py
--rw-r--r--   0        0        0     7496 2024-04-22 02:58:39.684201 ziya-0.1.0/app/utils/gitignore_parser.py
--rw-r--r--   0        0        0      280 2024-04-22 02:58:39.683997 ziya-0.1.0/app/utils/logging_utils.py
--rw-r--r--   0        0        0     1419 2024-04-22 02:58:39.683827 ziya-0.1.0/app/utils/print_tree_util.py
--rw-r--r--   0        0        0      716 2024-04-22 03:02:17.016401 ziya-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3622 2024-04-22 02:58:39.691297 ziya-0.1.0/static/app.js
--rw-r--r--   0        0        0    15086 2024-04-22 02:58:39.707497 ziya-0.1.0/static/favicon.ico
--rw-r--r--   0        0        0     1956 2024-04-22 02:58:39.691535 ziya-0.1.0/static/sendPayload.js
--rw-r--r--   0        0        0     1395 2024-04-21 06:06:04.639034 ziya-0.1.0/static/ziya.css
--rw-r--r--   0        0        0      800 2024-04-22 02:58:39.707765 ziya-0.1.0/templates/index.html
--rw-r--r--   0        0        0     2472 1970-01-01 00:00:00.000000 ziya-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1714 2024-04-22 03:21:31.982461 ziya-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.1/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.1/app/agents/__init__.py
+-rw-r--r--   0        0        0     4181 2024-04-22 03:14:43.793669 ziya-0.1.1/app/agents/agent.py
+-rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.1/app/agents/prompts.py
+-rw-r--r--   0        0        0     1359 2024-04-22 03:14:43.793879 ziya-0.1.1/app/main.py
+-rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.1/app/server.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.1/app/utils/__init__.py
+-rw-r--r--   0        0        0     2132 2024-04-22 03:14:43.794161 ziya-0.1.1/app/utils/directory_util.py
+-rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.1/app/utils/gitignore_parser.py
+-rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.1/app/utils/logging_utils.py
+-rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.1/app/utils/print_tree_util.py
+-rw-r--r--   0        0        0      716 2024-04-22 03:16:37.495159 ziya-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3622 2024-04-22 03:14:43.795533 ziya-0.1.1/static/app.js
+-rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.1/static/favicon.ico
+-rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.1/static/sendPayload.js
+-rw-r--r--   0        0        0     1395 2024-04-22 03:14:43.795995 ziya-0.1.1/static/ziya.css
+-rw-r--r--   0        0        0      800 2024-04-22 03:14:43.796168 ziya-0.1.1/templates/index.html
+-rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 ziya-0.1.1/PKG-INFO
```

### Comparing `ziya-0.1.0/LICENSE` & `ziya-0.1.1/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 LangChain, Inc.
+Copyright (c) 2024 ziya-ai
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ziya-0.1.0/README.md` & `ziya-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Ziya
 
+## Documentation
+See the [GitHub Repository](https://github.com/ziya-ai/ziya)
+
+## Overview
 Ziya is a code assist tool for AWS Bedrock models. It can read your entire codebase and answer questions.
 
 The current version only performs read operations. However, future versions will be able to:
 
 1. Write and edit code.
 2. Search the web for resources.
 3. Run commands locally.
```

### Comparing `ziya-0.1.0/app/agents/agent.py` & `ziya-0.1.1/app/agents/agent.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/app/agents/prompts.py` & `ziya-0.1.1/app/agents/prompts.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/app/main.py` & `ziya-0.1.1/app/main.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/app/server.py` & `ziya-0.1.1/app/server.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/app/utils/directory_util.py` & `ziya-0.1.1/app/utils/directory_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/app/utils/gitignore_parser.py` & `ziya-0.1.1/app/utils/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/app/utils/print_tree_util.py` & `ziya-0.1.1/app/utils/print_tree_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/pyproject.toml` & `ziya-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziya"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Vishnu Krishnaprasad <vishnukool@gmail.com>"]
 readme = "README.md"
 include = ["static/**/*", "templates/**/*", "pyproject.toml"]
 packages = [
     { include = "app" },
 ]
```

### Comparing `ziya-0.1.0/static/app.js` & `ziya-0.1.1/static/app.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/static/favicon.ico` & `ziya-0.1.1/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/static/sendPayload.js` & `ziya-0.1.1/static/sendPayload.js`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/static/ziya.css` & `ziya-0.1.1/static/ziya.css`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/templates/index.html` & `ziya-0.1.1/templates/index.html`

 * *Files identical despite different names*

### Comparing `ziya-0.1.0/PKG-INFO` & `ziya-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziya
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Vishnu Krishnaprasad
 Author-email: vishnukool@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,14 +20,18 @@
 Requires-Dist: pydantic (<2)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: uvicorn (>=0.23.2,<0.24.0)
 Description-Content-Type: text/markdown
 
 # Ziya
 
+## Documentation
+See the [GitHub Repository](https://github.com/ziya-ai/ziya)
+
+## Overview
 Ziya is a code assist tool for AWS Bedrock models. It can read your entire codebase and answer questions.
 
 The current version only performs read operations. However, future versions will be able to:
 
 1. Write and edit code.
 2. Search the web for resources.
 3. Run commands locally.
```

