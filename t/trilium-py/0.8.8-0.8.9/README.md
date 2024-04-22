# Comparing `tmp/trilium_py-0.8.8-py3-none-any.whl.zip` & `tmp/trilium_py-0.8.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 33876 bytes, number of entries: 14
--rw-r--r--  2.0 unx      141 b- defN 23-Aug-25 07:17 trilium_py/__init__.py
--rw-r--r--  2.0 unx    43377 b- defN 24-Apr-02 02:04 trilium_py/client.py
+Zip file size: 34238 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      141 b- defN 24-Apr-22 06:33 trilium_py/__init__.py
+-rw-r--r--  2.0 unx    44149 b- defN 24-Apr-22 06:50 trilium_py/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-25 07:17 trilium_py/utils/__init__.py
--rw-r--r--  2.0 unx     2301 b- defN 23-Aug-25 07:17 trilium_py/utils/html_util.py
--rw-r--r--  2.0 unx     9328 b- defN 23-Aug-25 07:17 trilium_py/utils/markdown_math.py
--rw-r--r--  2.0 unx     3923 b- defN 23-Aug-25 07:17 trilium_py/utils/note_util.py
--rw-r--r--  2.0 unx      681 b- defN 23-Aug-25 07:17 trilium_py/utils/param_util.py
--rw-r--r--  2.0 unx      208 b- defN 23-Aug-25 07:17 trilium_py/utils/time_util.py
--rw-r--r--  2.0 unx      486 b- defN 23-Aug-25 07:17 trilium_py/utils/url_util.py
--rwxrwx---  2.0 unx    35184 b- defN 24-Apr-02 03:07 trilium_py-0.8.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    15197 b- defN 24-Apr-02 03:07 trilium_py-0.8.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 03:07 trilium_py-0.8.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-02 03:07 trilium_py-0.8.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1162 b- defN 24-Apr-02 03:07 trilium_py-0.8.8.dist-info/RECORD
-14 files, 112091 bytes uncompressed, 31938 bytes compressed:  71.5%
+-rw-r--r--  2.0 unx     2290 b- defN 24-Apr-22 06:32 trilium_py/utils/html_util.py
+-rw-r--r--  2.0 unx     9328 b- defN 24-Apr-22 06:33 trilium_py/utils/markdown_math.py
+-rw-r--r--  2.0 unx     3909 b- defN 24-Apr-22 06:33 trilium_py/utils/note_util.py
+-rw-r--r--  2.0 unx      681 b- defN 24-Apr-22 06:33 trilium_py/utils/param_util.py
+-rw-r--r--  2.0 unx      208 b- defN 24-Apr-22 06:33 trilium_py/utils/time_util.py
+-rw-r--r--  2.0 unx      486 b- defN 24-Apr-22 06:33 trilium_py/utils/url_util.py
+-rwxrwx---  2.0 unx    35184 b- defN 24-Apr-22 07:02 trilium_py-0.8.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    15640 b- defN 24-Apr-22 07:02 trilium_py-0.8.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 07:02 trilium_py-0.8.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-22 07:02 trilium_py-0.8.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1162 b- defN 24-Apr-22 07:02 trilium_py-0.8.9.dist-info/RECORD
+14 files, 113281 bytes uncompressed, 32300 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: trilium_py/utils/time_util.py
 Comment: 
 
 Filename: trilium_py/utils/url_util.py
 Comment: 
 
-Filename: trilium_py-0.8.8.dist-info/LICENSE.txt
+Filename: trilium_py-0.8.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: trilium_py-0.8.8.dist-info/METADATA
+Filename: trilium_py-0.8.9.dist-info/METADATA
 Comment: 
 
-Filename: trilium_py-0.8.8.dist-info/WHEEL
+Filename: trilium_py-0.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: trilium_py-0.8.8.dist-info/top_level.txt
+Filename: trilium_py-0.8.9.dist-info/top_level.txt
 Comment: 
 
-Filename: trilium_py-0.8.8.dist-info/RECORD
+Filename: trilium_py-0.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trilium_py/client.py

```diff
@@ -1,8 +1,7 @@
-import locale
 import os
 import re
 import string
 import sys
 import urllib.parse
 from collections.abc import Mapping
 from typing import Optional, Union
@@ -1239,14 +1238,35 @@
         :param noteId:
         :param locale_str:  should be something like 'zh_CN.UTF-8'
         """
         html_content = self.get_note_content(noteId)
         sorted_html_content = sort_note_by_headings(html_content, locale_str)
         self.update_note_content(noteId, sorted_html_content)
 
+    def delete_empty_note(self, note_title=None, verbose=False):
+        """
+        delete empty `new note` which are created accidentally
+        :return:
+        """
+        if not note_title:
+            note_title = 'new note'
+        res = self.search_note(
+            search=f'note.title = "{note_title}"',
+        )
+        logger.info(f'found {len(res["results"])} notes with title "{note_title}"')
+        for x in res['results']:
+            content = self.get_note_content(x['noteId'])
+            if not content:
+                logger.info(f'delete note {x["noteId"]}')
+                self.delete_note(x["noteId"])
+            else:
+                logger.warning(f'note {x["noteId"]} is not empty')
+                if verbose:
+                    logger.info(content)
+
 
 class ListTemplate(string.Template):
     """Encapsulate To Do List HTML details
 
     :param caption: Text to be presented as the To Do list caption. Default: <p>TODO:</p>
     """
```

## trilium_py/utils/html_util.py

```diff
@@ -1,10 +1,10 @@
-import re
-import json
 import locale
+import re
+
 from bs4 import BeautifulSoup
 
 TAG_LEVELS = {'h1': 1, 'h2': 2, 'h3': 3, 'h4': 4, 'h5': 5, 'h6': 6}
 
 
 def sort_h_tags_with_hierarchy(data, locale_str='zh_CN.UTF-8'):
     """
```

## trilium_py/utils/note_util.py

```diff
@@ -1,8 +1,7 @@
-import locale
 import re
 
 import minify_html
 from bs4 import BeautifulSoup
 
 from .html_util import sort_h_tags_with_hierarchy
```

## Comparing `trilium_py-0.8.8.dist-info/LICENSE.txt` & `trilium_py-0.8.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `trilium_py-0.8.8.dist-info/METADATA` & `trilium_py-0.8.9.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trilium-py
-Version: 0.8.8
+Version: 0.8.9
 Summary: Python client for ETAPI of Trilium Note. With some extra features powered by Python :)
 Home-page: https://github.com/nriver/trilium-py
 Author: Nriver
 Author-email: 
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues
 Project-URL: Funding, https://github.com/nriver/trilium-py
 Project-URL: Say Thanks!, https://github.com/nriver/trilium-py
@@ -166,15 +166,14 @@
     search="note.title %= '.*'",
     ancestorNoteId="Parent Note ID",
     fastSearch=False,
     limit=1000,
 )
 ```
 
-
 ### 🏭 Create Note
 
 You can create a simple note like this.
 
 ```python
 res = ea.create_note(
     parentNoteId="root",
@@ -294,15 +293,17 @@
     noteId='noteid',
     type='label',
     name='name_of_the_tag',
     value='value_of_the_tag',
     isInheritable=True
 )
 ```
+
 The `noteId` is not mandatory, if not provided, Trilium will generate a random one. You can retrieve it in the return.
+
 ```python
 noteId = res['note']['noteId']
 ```
 
 ### Get attachment info
 
 Get image title and etc.
@@ -541,14 +542,24 @@
 sorting process and tailors it to your linguistic preferences.
 
 ```python
 res = ea.sort_note_content('lPxtkknjR2bJ')
 res = ea.sort_note_content('y6hROhWjNmHQ', 'zh_CN.UTF-8')
 ```
 
+## ## (Advanced Usage) 🧹 Delete empty `new note`
+
+I inadvertently create numerous "new notes" which remain undeleted within my note tree. These "new notes" clutter my
+workspace, scattered across various locations. I made this bulk deletion of these empty "new notes." Additionally, it
+generates warning messages for "new notes" that contain content, maybe we should change the title for those notes.
+
+```python
+ea.delete_empty_note()
+```
+
 ## 🛠️ Develop
 
 Install with pip egg link to make package change without reinstall.
 
 ```python
 python -m pip install --user -e .
 ```
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trilium-py Version: 0.8.8 Summary: Python client
+Metadata-Version: 2.1 Name: trilium-py Version: 0.8.9 Summary: Python client
 for ETAPI of Trilium Note. With some extra features powered by Python :) Home-
 page: https://github.com/nriver/trilium-py Author: Nriver Author-email:
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues Project-
 URL: Funding, https://github.com/nriver/trilium-py Project-URL: Say Thanks!,
 https://github.com/nriver/trilium-py Project-URL: Source, https://github.com/
 nriver/trilium-py/ Keywords: trilium,etapi,api client Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
@@ -180,13 +180,19 @@
 ('tlPuzU2szLJh') ``` ## (Advanced Usage) ð§¹ Sort note content Sort a note by
 the heading names. This feature could prove invaluable for notes containing
 extensive lists, such as book titles sorted into various genres. It's equally
 useful for managing browser bookmarks or collecting links. Additionally, you
 have the option to specify a language code for sorting based on your local
 language. This enhances the sorting process and tailors it to your linguistic
 preferences. ```python res = ea.sort_note_content('lPxtkknjR2bJ') res =
-ea.sort_note_content('y6hROhWjNmHQ', 'zh_CN.UTF-8') ``` ## ð ï¸ Develop
-Install with pip egg link to make package change without reinstall. ```python
-python -m pip install --user -e . ``` ## ð Original OpenAPI Documentation
-The original OpenAPI document is [here](https://github.com/zadam/trilium/blob/
-master/src/etapi/etapi.openapi.yaml). You can open it with [swagger editor]
-(https://editor.swagger.io/).
+ea.sort_note_content('y6hROhWjNmHQ', 'zh_CN.UTF-8') ``` ## ## (Advanced Usage)
+ð§¹ Delete empty `new note` I inadvertently create numerous "new notes" which
+remain undeleted within my note tree. These "new notes" clutter my workspace,
+scattered across various locations. I made this bulk deletion of these empty
+"new notes." Additionally, it generates warning messages for "new notes" that
+contain content, maybe we should change the title for those notes. ```python
+ea.delete_empty_note() ``` ## ð ï¸ Develop Install with pip egg link to make
+package change without reinstall. ```python python -m pip install --user -e .
+``` ## ð Original OpenAPI Documentation The original OpenAPI document is
+[here](https://github.com/zadam/trilium/blob/master/src/etapi/
+etapi.openapi.yaml). You can open it with [swagger editor](https://
+editor.swagger.io/).
```

## Comparing `trilium_py-0.8.8.dist-info/RECORD` & `trilium_py-0.8.9.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 trilium_py/__init__.py,sha256=uSMH49RW2MFU_LVKKKm6lt3xOBsDWo0cb8--nMcNlgY,141
-trilium_py/client.py,sha256=g64hW5RRti0XM646N5IT9PG-1FwN6ZkmkPWYDSf8XlU,43377
+trilium_py/client.py,sha256=HJm8qnanq5mlDHtXCZLWHdmAOSfeWdVchsWZV8dlt1M,44149
 trilium_py/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-trilium_py/utils/html_util.py,sha256=HWniQG6udrU6vcaJdCETA30DH_MSdLFDncUiooKYV7I,2301
+trilium_py/utils/html_util.py,sha256=OuFEt5bHiiNYtBDX_ABPXudDoHpid97GmicFQwuidNE,2290
 trilium_py/utils/markdown_math.py,sha256=sAiR_5YaCE_EOeQ4vZBjoc5t0Z1n_5EQ4JmJ1TAweCY,9328
-trilium_py/utils/note_util.py,sha256=tx2kD1g9X_jILntDKEoXzHPytRGxj85ebKO2D8Ef72M,3923
+trilium_py/utils/note_util.py,sha256=jSavmxnV8Fn-DKoFeNLFVxtkrn176wQF_pbiPJCdEu8,3909
 trilium_py/utils/param_util.py,sha256=jlnKrCKBtaN1wfQgxDTvGmuMM0p7vk809vpaLgK0dXg,681
 trilium_py/utils/time_util.py,sha256=DIFQmCKZ_wL5lCdeTMJZAtFolZw_dic6NKZ8CCJTa1A,208
 trilium_py/utils/url_util.py,sha256=1eHmHlti4CwsN-hjqfennxiohkrUX0jtuX3UleTD120,486
-trilium_py-0.8.8.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
-trilium_py-0.8.8.dist-info/METADATA,sha256=hh4RsCfmsx8ep81mGQKXj-Rd2-n3wCavLFpmUAsJ54A,15197
-trilium_py-0.8.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-trilium_py-0.8.8.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
-trilium_py-0.8.8.dist-info/RECORD,,
+trilium_py-0.8.9.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
+trilium_py-0.8.9.dist-info/METADATA,sha256=7jqrk3Y-rythyxZSj5o_kuB9znwO14IP5ym5TA0ifcE,15640
+trilium_py-0.8.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+trilium_py-0.8.9.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
+trilium_py-0.8.9.dist-info/RECORD,,
```

