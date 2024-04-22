# Comparing `tmp/monisha-0.0.54.tar.gz` & `tmp/monisha-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.54.tar", last modified: Sat Apr 20 18:59:57 2024, max compression
+gzip compressed data, was "monisha-0.0.55.tar", last modified: Mon Apr 22 08:32:48 2024, max compression
```

## Comparing `monisha-0.0.54.tar` & `monisha-0.0.55.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:59:57.293885 monisha-0.0.54/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-20 18:59:52.000000 monisha-0.0.54/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:59:57.289885 monisha-0.0.54/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:59:57.289885 monisha-0.0.54/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/functions/function16.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:59:57.293885 monisha-0.0.54/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-20 18:59:52.000000 monisha-0.0.54/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-20 18:59:57.293885 monisha-0.0.54/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-20 18:59:52.000000 monisha-0.0.54/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 18:59:57.293885 monisha-0.0.54/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-20 18:59:57.000000 monisha-0.0.54/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-20 18:59:57.000000 monisha-0.0.54/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:59:57.000000 monisha-0.0.54/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 18:59:57.000000 monisha-0.0.54/monisha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 18:59:57.000000 monisha-0.0.54/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 18:59:57.293885 monisha-0.0.54/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-20 18:59:52.000000 monisha-0.0.54/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:32:48.585563 monisha-0.0.55/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-22 08:32:42.000000 monisha-0.0.55/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:32:48.577563 monisha-0.0.55/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:32:48.581563 monisha-0.0.55/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/functions/function17.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:32:48.581563 monisha-0.0.55/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-22 08:32:42.000000 monisha-0.0.55/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-22 08:32:48.585563 monisha-0.0.55/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-22 08:32:42.000000 monisha-0.0.55/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:32:48.585563 monisha-0.0.55/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-22 08:32:48.000000 monisha-0.0.55/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-22 08:32:48.000000 monisha-0.0.55/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:32:48.000000 monisha-0.0.55/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 08:32:48.000000 monisha-0.0.55/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 08:32:48.000000 monisha-0.0.55/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:32:48.585563 monisha-0.0.55/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-22 08:32:42.000000 monisha-0.0.55/setup.py
```

### Comparing `monisha-0.0.54/LICENSE` & `monisha-0.0.55/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/Monisha/functions/__init__.py` & `monisha-0.0.55/Monisha/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/Monisha/functions/function01.py` & `monisha-0.0.55/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/Monisha/functions/function02.py` & `monisha-0.0.55/Monisha/functions/function02.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from ..scripts.es import Humon
 from ..scripts.en import Scripted
 #=============================================================================
 
-def Dbytes(sizes, second=Scripted.DATA01):
+def Dbytes(sizes, blank=Scripted.DATA09, second=Scripted.DATA01):
     if not sizes or (sizes == Scripted.DATA02):
-        return Scripted.DATA09
+        return blank
     nomos = 0
     POWEO = 2**10
     POWER = Humon.DATA01
     while sizes > POWEO:
         sizes /= POWEO
         nomos += 1
     ouing = str(round(sizes, 2)) + Scripted.DATA02 + POWER[nomos] + second
     return ouing
 
 #=============================================================================
 
-def Hbytes(sizes, second=Scripted.DATA01):
+def Hbytes(sizes, blank=Scripted.DATA08, second=Scripted.DATA01):
     if not sizes or (sizes == Scripted.DATA02):
-        return Scripted.DATA08
+        return blank
     nomos = 0
     POWEO = 2**10
     POWER = Humon.DATA02
     while sizes > POWEO:
         sizes /= POWEO
         nomos += 1
     ouing = str(round(sizes, 2)) + Scripted.DATA02 + POWER[nomos] + second
```

### Comparing `monisha-0.0.54/Monisha/functions/function03.py` & `monisha-0.0.55/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/Monisha/functions/function04.py` & `monisha-0.0.55/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/Monisha/functions/function06.py` & `monisha-0.0.55/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/Monisha/functions/function07.py` & `monisha-0.0.55/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/Monisha/functions/function10.py` & `monisha-0.0.55/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/Monisha/functions/function14.py` & `monisha-0.0.55/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/Monisha/functions/function15.py` & `monisha-0.0.55/Monisha/functions/function15.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/Monisha/functions/function16.py` & `monisha-0.0.55/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/Monisha/scripts/es.py` & `monisha-0.0.55/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.54/PKG-INFO` & `monisha-0.0.55/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.54
+Version: 0.0.55
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
@@ -15,11 +15,13 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-magic
+Requires-Dist: pyrofork==2.3.19
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.54 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.55 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+python-magic Requires-Dist: pyrofork==2.3.19
                                  ð¦ _M_O_N_I_S_H_A
```

### Comparing `monisha-0.0.54/monisha.egg-info/PKG-INFO` & `monisha-0.0.55/monisha.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.54
+Version: 0.0.55
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
@@ -15,11 +15,13 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-magic
+Requires-Dist: pyrofork==2.3.19
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.54 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.55 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+python-magic Requires-Dist: pyrofork==2.3.19
                                  ð¦ _M_O_N_I_S_H_A
```

### Comparing `monisha-0.0.54/monisha.egg-info/SOURCES.txt` & `monisha-0.0.55/monisha.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 Monisha/functions/function10.py
 Monisha/functions/function11.py
 Monisha/functions/function12.py
 Monisha/functions/function13.py
 Monisha/functions/function14.py
 Monisha/functions/function15.py
 Monisha/functions/function16.py
+Monisha/functions/function17.py
 Monisha/scripts/__init__.py
 Monisha/scripts/en.py
 Monisha/scripts/eo.py
 Monisha/scripts/es.py
 monisha.egg-info/PKG-INFO
 monisha.egg-info/SOURCES.txt
 monisha.egg-info/dependency_links.txt
-monisha.egg-info/not-zip-safe
+monisha.egg-info/requires.txt
 monisha.egg-info/top_level.txt
```

### Comparing `monisha-0.0.54/setup.py` & `monisha-0.0.55/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from setuptools import setup, find_packages
+from Monisha import appname, version, install
 
 with open("README.md", "r") as o:
-    long_description = o.read()
+    description = o.read()
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)']
 
 setup(
-    name='monisha',
+    name=appname,
     license='MIT',
-    zip_safe=False,
+    version=version,
     description='ㅤ',
-    version='0.0.54',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.10',
     packages=find_packages(),
     author='Clinton-Abraham',
-    long_description=long_description,
+    install_requires=install,
+    long_description=description,
     url='https://github.com/Clinton-Abraham',
     keywords=['python', 'clinton', 'abraham'],
     long_description_content_type="text/markdown")
```

