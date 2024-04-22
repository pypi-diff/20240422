# Comparing `tmp/monisha-0.0.55.tar.gz` & `tmp/monisha-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.55.tar", last modified: Mon Apr 22 08:32:48 2024, max compression
+gzip compressed data, was "monisha-0.0.56.tar", last modified: Mon Apr 22 08:57:16 2024, max compression
```

## Comparing `monisha-0.0.55.tar` & `monisha-0.0.56.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:32:48.585563 monisha-0.0.55/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-22 08:32:42.000000 monisha-0.0.55/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:32:48.577563 monisha-0.0.55/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:32:48.581563 monisha-0.0.55/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function17.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:32:48.581563 monisha-0.0.55/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-22 08:32:48.585563 monisha-0.0.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-22 08:32:42.000000 monisha-0.0.55/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:32:48.585563 monisha-0.0.55/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-22 08:32:48.000000 monisha-0.0.55/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-22 08:32:48.000000 monisha-0.0.55/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:32:48.000000 monisha-0.0.55/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 08:32:48.000000 monisha-0.0.55/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 08:32:48.000000 monisha-0.0.55/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:32:48.585563 monisha-0.0.55/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-22 08:32:42.000000 monisha-0.0.55/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:57:16.127138 monisha-0.0.56/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-22 08:57:10.000000 monisha-0.0.56/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:57:16.123138 monisha-0.0.56/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:57:16.127138 monisha-0.0.56/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/functions/function17.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:57:16.127138 monisha-0.0.56/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-22 08:57:10.000000 monisha-0.0.56/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-22 08:57:16.127138 monisha-0.0.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-22 08:57:10.000000 monisha-0.0.56/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:57:16.127138 monisha-0.0.56/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-22 08:57:16.000000 monisha-0.0.56/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-22 08:57:16.000000 monisha-0.0.56/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:57:16.000000 monisha-0.0.56/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 08:57:16.000000 monisha-0.0.56/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 08:57:16.000000 monisha-0.0.56/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:57:16.127138 monisha-0.0.56/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-22 08:57:10.000000 monisha-0.0.56/setup.py
```

### Comparing `monisha-0.0.55/LICENSE` & `monisha-0.0.56/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.55/Monisha/functions/__init__.py` & `monisha-0.0.56/Monisha/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.55/Monisha/functions/function01.py` & `monisha-0.0.56/Monisha/functions/function01.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..scripts.en import Scripted
+from ..scripts import Scripted
 #=========================================================================
 
 def timend(tsize, dsize, speed):
     moonuo = round((tsize - dsize) / speed)
     return moonuo
 
 #=========================================================================
```

### Comparing `monisha-0.0.55/Monisha/functions/function02.py` & `monisha-0.0.56/Monisha/functions/function02.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from ..scripts.es import Humon
-from ..scripts.en import Scripted
+from ..scripts import Humon, Scripted
 #=============================================================================
 
 def Dbytes(sizes, blank=Scripted.DATA09, second=Scripted.DATA01):
     if not sizes or (sizes == Scripted.DATA02):
         return blank
     nomos = 0
     POWEO = 2**10
```

### Comparing `monisha-0.0.55/Monisha/functions/function03.py` & `monisha-0.0.56/Monisha/functions/function03.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..scripts.eo import Smbo
+from ..scripts import Smbo
 #===================================================================================
 
 def progress(percentage, b01=Smbo.DATA02, b02=Smbo.DATA01, l01=10, l02=20):
     percenage = float(percentage)
     passngeso = min(max(percenage, 0), 100)
     cosmosses = int(passngeso // l01)
     outgoings = b01 * cosmosses
```

### Comparing `monisha-0.0.55/Monisha/functions/function04.py` & `monisha-0.0.56/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.55/Monisha/functions/function06.py` & `monisha-0.0.56/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.55/Monisha/functions/function07.py` & `monisha-0.0.56/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.55/Monisha/functions/function10.py` & `monisha-0.0.56/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.55/Monisha/functions/function14.py` & `monisha-0.0.56/Monisha/functions/function14.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os, time
-from ..scripts.es import Folder
-from ..scripts.en import Scripted
+from ..scripts import Folder, Scripted
 #============================================================================
 
 async def CDirectory(dname=Folder.DATA07):
     direos = str(dname)
     osemse = os.getcwd()
     moonse = os.path.join(osemse, direos, Scripted.DATA01)
     moonse if os.path.isdir(moonse) else os.makedirs(moonse)
```

### Comparing `monisha-0.0.55/Monisha/functions/function15.py` & `monisha-0.0.56/Monisha/functions/function15.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.55/Monisha/functions/function16.py` & `monisha-0.0.56/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.55/Monisha/functions/function17.py` & `monisha-0.0.56/Monisha/functions/function17.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.55/Monisha/scripts/es.py` & `monisha-0.0.56/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.55/PKG-INFO` & `monisha-0.0.56/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.55
+Version: 0.0.56
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
@@ -16,12 +16,11 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-magic
-Requires-Dist: pyrofork==2.3.19
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.55 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.56 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-python-magic Requires-Dist: pyrofork==2.3.19
+python-magic
                                  ð¦ _M_O_N_I_S_H_A
```

### Comparing `monisha-0.0.55/monisha.egg-info/PKG-INFO` & `monisha-0.0.56/monisha.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.55
+Version: 0.0.56
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
@@ -16,12 +16,11 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-magic
-Requires-Dist: pyrofork==2.3.19
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.55 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.56 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-python-magic Requires-Dist: pyrofork==2.3.19
+python-magic
                                  ð¦ _M_O_N_I_S_H_A
```

### Comparing `monisha-0.0.55/monisha.egg-info/SOURCES.txt` & `monisha-0.0.56/monisha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

