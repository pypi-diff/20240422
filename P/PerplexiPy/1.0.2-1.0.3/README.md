# Comparing `tmp/PerplexiPy-1.0.2-py3-none-any.whl.zip` & `tmp/PerplexiPy-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11635 bytes, number of entries: 10
--rw-r--r--  2.0 unx     9253 b- defN 24-Apr-20 02:11 perplexipy/__init__.py
--rw-r--r--  2.0 unx     9085 b- defN 24-Apr-21 02:27 perplexipy/codex.py
+Zip file size: 11647 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     9253 b- defN 24-Apr-22 04:33 perplexipy/__init__.py
+-rw-r--r--  2.0 unx     9179 b- defN 24-Apr-22 04:33 perplexipy/codex.py
 -rw-r--r--  2.0 unx      283 b- defN 24-Mar-01 20:13 perplexipy/errors.py
 -rw-r--r--  2.0 unx      684 b- defN 24-Apr-13 17:06 perplexipy/responses.py
--rw-r--r--  2.0 unx     1514 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6833 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-21 02:29 PerplexiPy-1.0.2.dist-info/RECORD
-10 files, 28617 bytes uncompressed, 10243 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx     1514 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6833 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-22 04:36 PerplexiPy-1.0.3.dist-info/RECORD
+10 files, 28711 bytes uncompressed, 10255 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: perplexipy/errors.py
 Comment: 
 
 Filename: perplexipy/responses.py
 Comment: 
 
-Filename: PerplexiPy-1.0.2.dist-info/LICENSE.txt
+Filename: PerplexiPy-1.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.2.dist-info/METADATA
+Filename: PerplexiPy-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: PerplexiPy-1.0.2.dist-info/WHEEL
+Filename: PerplexiPy-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: PerplexiPy-1.0.2.dist-info/entry_points.txt
+Filename: PerplexiPy-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.2.dist-info/top_level.txt
+Filename: PerplexiPy-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: PerplexiPy-1.0.2.dist-info/RECORD
+Filename: PerplexiPy-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perplexipy/codex.py

```diff
@@ -234,18 +234,18 @@
     Run a REPL loop for sending queries to the AI provider.
 
     Returns
     -------
     The word "REPL" to signal to the `codex` command that it received valid
     input.
     """
-    _REPLHello()
     config = _loadConfigFrom()
     session = PromptSession()
-    _activeModel(config['activeModel'])
+    _activeModel(list(_client.models.keys()).index(config['activeModel'])+1)
+    _REPLHello()
     session = _editingMode(session, config['editingMode'])
     _queryStyle('code' if config['queryCodeStyle'] else 'human')
     while True:
         userQuery = session.prompt('Ask anything (/exit to end): ')
         if userQuery[0] in ('/', '?', ':'):
             parts = userQuery.split(' ')
             command = parts[0]
@@ -257,14 +257,16 @@
                         model = int(parts[1])
                         config['activeModel'] = _activeModel(model)
                         _saveConfigTo(config)
                     except:
                         # Invalid input, ignore and leave the current model
                         # active.
                         pass
+                else:
+                    _activeModel()
             elif command == '/cinfo':
                 _displayConfigInfo()
             elif command == '/clear':
                 click.clear()
                 _editingMode(session)
             elif command in ('/help', '?'):
                 _helpREPL()
```

## Comparing `PerplexiPy-1.0.2.dist-info/LICENSE.txt` & `PerplexiPy-1.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PerplexiPy-1.0.2.dist-info/METADATA` & `PerplexiPy-1.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PerplexiPy
-Version: 1.0.2
+Version: 1.0.3
 Summary: PerplexiPy - A robust Perplexity AI API client
 Author-email: CIME Software Ltd <perplexipy@cime.net>
 License: BSD-3
 Project-URL: homepage, https://cime-software.github.io/perplexipy/
 Project-URL: Documentation, https://cime-software.github.io/perplexipy/
 Project-URL: Bug Tracker, https://github.com/CIME-Software/perplexipy/issues
 Project-URL: Source, https://github.com/CIME-Software/perplexipy
@@ -22,15 +22,15 @@
 Requires-Dist: appdirs
 Requires-Dist: click
 Requires-Dist: openai (>=1.12.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 
-% perplexipy(3) Version 1.0.2 | Perplexity AI high level API documentation
+% perplexipy(3) Version 1.0.3 | Perplexity AI high level API documentation
 
 Name
 ====
 
 **PerplexiPy** - Perplexity AI high level library
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.2 Summary: PerplexiPy - A
+Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.3 Summary: PerplexiPy - A
 robust Perplexity AI API client Author-email: CIME Software Ltd
 cime.net> License: BSD-3 Project-URL: homepage, https://cime-
 software.github.io/perplexipy/ Project-URL: Documentation, https://cime-
 software.github.io/perplexipy/ Project-URL: Bug Tracker, https://github.com/
 CIME-Software/perplexipy/issues Project-URL: Source, https://github.com/CIME-
 Software/perplexipy Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: appdirs Requires-Dist: click Requires-Dist: openai
 (>=1.12.0) Requires-Dist: prompt-toolkit Requires-Dist: python-dotenv Requires-
-Dist: pyyaml % perplexipy(3) Version 1.0.2 | Perplexity AI high level API
+Dist: pyyaml % perplexipy(3) Version 1.0.3 | Perplexity AI high level API
 documentation Name ==== **PerplexiPy** - Perplexity AI high level library
 [https://images2.imgbox.com/57/94/AsI1WSfy_o.png]Synopsis ======== ```python
 client = PerplexityClient() \ print(client.query('What is the meaning of 42?')
 \ for result in client.queryStreamable('List of all US presidents'): \ print
 (result) ``` Description =========== **PerplexiPy** is a high-level,
 convenience library for interacting with the Perplexity API from any Python
 3.9+ application. The library aims to simplify interactions with Perplexity
```

## Comparing `PerplexiPy-1.0.2.dist-info/RECORD` & `PerplexiPy-1.0.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 perplexipy/__init__.py,sha256=jex9IfNCEyLV3rtpq7L3VEfs75NmHXZki8l6wD-wohA,9253
-perplexipy/codex.py,sha256=3tF8Fz7HeZQKVvXrAdENcbLTiG0MzUOD4H65pVgSKf0,9085
+perplexipy/codex.py,sha256=ll0VrHpaSPjV4F8R9KejOfQMqRlS8loYsDStMcC10ls,9179
 perplexipy/errors.py,sha256=YM4dVV9q2aLm_ZJdhyCjhejLXdo8mEffx93zlP_7lOs,283
 perplexipy/responses.py,sha256=1OrBpZxGHaVvlE5x9ZtdQhoXP5RbmKOXtHGt6Nm7g2I,684
-PerplexiPy-1.0.2.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
-PerplexiPy-1.0.2.dist-info/METADATA,sha256=vkw3X00KX9kHQQzOkPNTUD1ZIYzv72jpbYtPnXg3Hic,6833
-PerplexiPy-1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-PerplexiPy-1.0.2.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
-PerplexiPy-1.0.2.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
-PerplexiPy-1.0.2.dist-info/RECORD,,
+PerplexiPy-1.0.3.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
+PerplexiPy-1.0.3.dist-info/METADATA,sha256=65rwMxA4ytU5fb9reFB592XzTk_-4xZpMofVg7XH950,6833
+PerplexiPy-1.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+PerplexiPy-1.0.3.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
+PerplexiPy-1.0.3.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
+PerplexiPy-1.0.3.dist-info/RECORD,,
```

