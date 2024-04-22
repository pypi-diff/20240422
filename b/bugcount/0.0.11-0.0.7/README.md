# Comparing `tmp/bugcount-0.0.11.tar.gz` & `tmp/bugcount-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bugcount-0.0.11.tar", last modified: Mon Apr 22 08:37:20 2024, max compression
+gzip compressed data, was "dist/bugcount-0.0.7.tar", last modified: Tue Jun  8 06:07:06 2021, max compression
```

## Comparing `bugcount-0.0.11.tar` & `bugcount-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:37:20.589400 bugcount-0.0.11/
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:37:20.589400 bugcount-0.0.11/.github/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1088 2021-06-03 01:23:24.000000 bugcount-0.0.11/.github/README.md
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     9716 2024-04-22 08:37:20.589400 bugcount-0.0.11/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     9162 2024-04-22 08:36:34.000000 bugcount-0.0.11/README.md
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 08:37:20.589400 bugcount-0.0.11/setup.cfg
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      974 2024-04-22 08:37:04.000000 bugcount-0.0.11/setup.py
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:37:20.589400 bugcount-0.0.11/src/
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:37:20.589400 bugcount-0.0.11/src/bugcount.egg-info/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     9716 2024-04-22 08:37:20.000000 bugcount-0.0.11/src/bugcount.egg-info/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      235 2024-04-22 08:37:20.000000 bugcount-0.0.11/src/bugcount.egg-info/SOURCES.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 08:37:20.000000 bugcount-0.0.11/src/bugcount.egg-info/dependency_links.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       44 2024-04-22 08:37:20.000000 bugcount-0.0.11/src/bugcount.egg-info/entry_points.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        9 2024-04-22 08:37:20.000000 bugcount-0.0.11/src/bugcount.egg-info/top_level.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1504 2022-03-22 06:03:10.000000 bugcount-0.0.11/src/bugcount.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-06-08 06:07:06.696523 bugcount-0.0.7/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-06-08 06:07:06.597001 bugcount-0.0.7/.github/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1088 2021-06-03 01:23:24.000000 bugcount-0.0.7/.github/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1067 2021-06-03 01:23:24.000000 bugcount-0.0.7/LICENSE.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       77 2021-06-03 01:23:24.000000 bugcount-0.0.7/MANIFEST.in
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     9278 2021-06-08 06:07:06.696523 bugcount-0.0.7/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     8709 2021-06-08 06:01:06.000000 bugcount-0.0.7/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      669 2021-06-08 06:07:06.702529 bugcount-0.0.7/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      963 2021-06-08 06:02:37.000000 bugcount-0.0.7/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-06-08 06:07:06.610983 bugcount-0.0.7/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-06-08 06:07:06.668519 bugcount-0.0.7/src/bugcount.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     9278 2021-06-08 06:07:05.000000 bugcount-0.0.7/src/bugcount.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      329 2021-06-08 06:07:05.000000 bugcount-0.0.7/src/bugcount.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2021-06-08 06:07:05.000000 bugcount-0.0.7/src/bugcount.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       44 2021-06-08 06:07:05.000000 bugcount-0.0.7/src/bugcount.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       13 2021-06-08 06:07:05.000000 bugcount-0.0.7/src/bugcount.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1211 2021-06-05 08:38:44.000000 bugcount-0.0.7/src/bugcount.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-06-08 06:07:06.693529 bugcount-0.0.7/src/src/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       32 2021-06-05 01:55:45.000000 bugcount-0.0.7/src/src/__init__.py
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       16 2021-06-05 01:55:45.000000 bugcount-0.0.7/src/src/__main__.py
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1211 2021-06-05 08:39:34.000000 bugcount-0.0.7/src/src/bugcount.py
```

### Comparing `bugcount-0.0.11/.github/README.md` & `bugcount-0.0.7/.github/README.md`

 * *Files identical despite different names*

### Comparing `bugcount-0.0.11/PKG-INFO` & `bugcount-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,78 +1,69 @@
 Metadata-Version: 2.1
 Name: bugcount
-Version: 0.0.11
-Summary: A package for counting BLOB objects
-Home-page: https://github.com/y-takefuji/counting-for-entomologists
+Version: 0.0.7
+Summary: A package for counting bugs
+Home-page: https://github.com/ytakefuji/counting-for-entomologists
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/y-takefuji/counting-for-entomologists
+Project-URL: Bug Tracker, https://github.com/ytakefuji/counting-for-entomologists
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # A new tool for counting the number of small objects.
-[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/dc7d4ef4-d838-467d-ab87-828e54dbd580/tree)
-
-DOI: https://doi.org/10.24433/CO.4823110.v1
-
-This is under review.
-
 bugcount is a useful tool for entomologists to count the number of bugs.
 
-bugcount has been downloaded by 12155 users worldwide as of July 21, 2023.
-
 # How to install this package:
 $ pip install bugcount
 
-$ pip install bugcount --force-reinstall --no-cache-dir --no-binary :all:
-
 You need to update the opencv-python library to the latest version:
 
 $ pip install -U opencv-python --user
 
 # How to use this bugcount:
 In command terminal, type bugcount file-name or bugcount file-name Canny-coeffient
 
 $ bugcount filename
 
 or
 
 You must download pillbug.png file:
 
-https://github.com/y-takefuji/counting-for-entomologists/raw/main/pillbug.png
+https://github.com/ytakefuji/counting-for-entomologists/raw/main/pillbug.png
 
 $ bugcount pillbug.png
 
-<img src="https://github.com/y-takefuji/counting-for-entomologists/raw/main/r75.png" width=270 height=275>
+<img src="https://github.com/ytakefuji/counting-for-entomologists/raw/main/r75.png" width=270 height=275>
 
 $ bugcount filename Canny-coeffient
 
 Default Canny-coeffient is 75.
 
 or 
 
 $ bugcount pillbug.png 10
 
-<img src="https://github.com/y-takefuji/counting-for-entomologists/raw/main/r10.png" width=270 height=275>
+<img src="https://github.com/ytakefuji/counting-for-entomologists/raw/main/r10.png" width=270 height=275>
 
 $ bugcount pillbug.png 100
 
-<img src="https://github.com/y-takefuji/counting-for-entomologists/raw/main/r100.png" width=270 height=275>
+<img src="https://github.com/ytakefuji/counting-for-entomologists/raw/main/r100.png" width=270 height=275>
 
 pillbug.png file is a target image for counting the number of bugs. 
 
 The smaller Canny coeffient, the more minute objects can be detected.
 
 # Detailed program of bugcount.py and pillbug_count.py
-bugcount has been downloaded by 5513 users worldwide.
+
 <pre>
 This new repository introduces a new tool on object counting for entomologists.
 
 bugcount.py or bugcount is an executable pypi version program while 
 pillbug_count.py is a modifiable program for researchers. 
 
 Counting the number of dead bugs or insect corpses on a plane is tedius 
@@ -120,15 +111,15 @@
 
 This repository shows how to use a Python program (pillbug_count.py) 
 for novice users to automatically count the number of dead bugs or 
 the number of insect corpses on a plane for entomologists.
 
 In order to run pillbug_count.py, you should see the following repository 
 for installing the necessary libraries:
-<a href="https://github.com/y-takefuji/python-novice"> How to install and use libraries in Python for novice users</a>
+<a href="https://github.com/ytakefuji/python-novice"> How to install and use libraries in Python for novice users</a>
 
 1. To install an executable Python environment on your operating system 
    (Windows, Mac, Linux), 
    download a Miniconda3 .sh file or .exe file for Python3.8 or Python3.7 
    from the following site:
 
 <a href="https://docs.conda.io/en/latest/miniconda.html">https://docs.conda.io/en/latest/miniconda.html</a>
@@ -138,27 +129,27 @@
    $ bash Miniconda3XXX.sh
 3. You need to install opencv libray, 
    type the following pip command for installation:
    $ pip install opencv-python
 4. To run pillbug_count.py, type the following command for testing:
    $ python pillbug_count.py pillbug.png
 </pre>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/result1.png' height=246 width=1031>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/result1.png' height=246 width=1031>
 
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/result2.png' height=380 width=366>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/result2.png' height=380 width=366>
 Result: 53 objects (blobs) are found in pillbug.png file.
 <pre>
 Use flies.png for further testing.
 $ python pillbug_count.py flies.png
 </pre>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/flies.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/gray.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/blur.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/edges.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/r.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/flies.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/gray.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/blur.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/edges.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/r.png' height=200 width=300>
 
 
 
 # You should resize an original picture for counting the number of dead bugs. And/or you should tune the Canny coefficient.
 
 
 # How to tune parameters for counting in general
@@ -237,17 +228,17 @@
 # Cell counting
 <pre>
 In bioprocessing, reagents such as A100 can be used to disaggregate 
 aggregated cell masses and automate cell counting.
 
 </pre>
 
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/cells.png' height=300 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/cells.png' height=300 width=300>
 Image source: https://bitesizebio.com/30184/quick-easy-automatic-cell-counting/
 
 <pre>
 $ bugcount cells.png
 
 </pre>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/r-cells.png' height=300 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/r-cells.png' height=300 width=300>
```

#### html2text {}

```diff
@@ -1,35 +1,29 @@
-Metadata-Version: 2.1 Name: bugcount Version: 0.0.11 Summary: A package for
-counting BLOB objects Home-page: https://github.com/y-takefuji/counting-for-
+Metadata-Version: 2.1 Name: bugcount Version: 0.0.7 Summary: A package for
+counting bugs Home-page: https://github.com/ytakefuji/counting-for-
 entomologists Author: yoshiyasu takefuji Author-email: takefuji@keio.jp
-License: UNKNOWN Project-URL: Bug Tracker, https://github.com/y-takefuji/
+License: UNKNOWN Project-URL: Bug Tracker, https://github.com/ytakefuji/
 counting-for-entomologists Platform: UNKNOWN Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
-Type: text/markdown # A new tool for counting the number of small objects. [!
-[Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-
-ocean.svg)](https://codeocean.com/capsule/dc7d4ef4-d838-467d-ab87-828e54dbd580/
-tree) DOI: https://doi.org/10.24433/CO.4823110.v1 This is under review.
-bugcount is a useful tool for entomologists to count the number of bugs.
-bugcount has been downloaded by 12155 users worldwide as of July 21, 2023. #
-How to install this package: $ pip install bugcount $ pip install bugcount --
-force-reinstall --no-cache-dir --no-binary :all: You need to update the opencv-
-python library to the latest version: $ pip install -U opencv-python --user #
-How to use this bugcount: In command terminal, type bugcount file-name or
-bugcount file-name Canny-coeffient $ bugcount filename or You must download
-pillbug.png file: https://github.com/y-takefuji/counting-for-entomologists/raw/
-main/pillbug.png $ bugcount pillbug.png [https://github.com/y-takefuji/
-counting-for-entomologists/raw/main/r75.png]$ bugcount filename Canny-coeffient
-Default Canny-coeffient is 75. or $ bugcount pillbug.png 10 [https://
-github.com/y-takefuji/counting-for-entomologists/raw/main/r10.png]$ bugcount
-pillbug.png 100 [https://github.com/y-takefuji/counting-for-entomologists/raw/
-main/r100.png]pillbug.png file is a target image for counting the number of
-bugs. The smaller Canny coeffient, the more minute objects can be detected. #
-Detailed program of bugcount.py and pillbug_count.py bugcount has been
-downloaded by 5513 users worldwide.
+Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
+Type: text/markdown License-File: LICENSE.txt # A new tool for counting the
+number of small objects. bugcount is a useful tool for entomologists to count
+the number of bugs. # How to install this package: $ pip install bugcount You
+need to update the opencv-python library to the latest version: $ pip install -
+U opencv-python --user # How to use this bugcount: In command terminal, type
+bugcount file-name or bugcount file-name Canny-coeffient $ bugcount filename or
+You must download pillbug.png file: https://github.com/ytakefuji/counting-for-
+entomologists/raw/main/pillbug.png $ bugcount pillbug.png [https://github.com/
+ytakefuji/counting-for-entomologists/raw/main/r75.png]$ bugcount filename
+Canny-coeffient Default Canny-coeffient is 75. or $ bugcount pillbug.png 10
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/r10.png]$
+bugcount pillbug.png 100 [https://github.com/ytakefuji/counting-for-
+entomologists/raw/main/r100.png]pillbug.png file is a target image for counting
+the number of bugs. The smaller Canny coeffient, the more minute objects can be
+detected. # Detailed program of bugcount.py and pillbug_count.py
 This new repository introduces a new tool on object counting for entomologists.
 
 bugcount.py or bugcount is an executable pypi version program while
 pillbug_count.py is a modifiable program for researchers.
 
 Counting the number of dead bugs or insect corpses on a plane is tedius
 and a very time-consuming task.
@@ -89,24 +83,24 @@
    your terminal:
    $ bash Miniconda3XXX.sh
 3. You need to install opencv libray,
    type the following pip command for installation:
    $ pip install opencv-python
 4. To run pillbug_count.py, type the following command for testing:
    $ python pillbug_count.py pillbug.png
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/result1.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/result1.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/
 result2.png]Result: 53 objects (blobs) are found in pillbug.png file.
 Use flies.png for further testing.
 $ python pillbug_count.py flies.png
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/flies.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/gray.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/blur.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/edges.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/r.png]# You
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/flies.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/gray.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/blur.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/edges.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/r.png]# You
 should resize an original picture for counting the number of dead bugs. And/or
 you should tune the Canny coefficient. # How to tune parameters for counting in
 general pillbug_count.py is shown:
 import cv2,sys
 if len(sys.argv)<2:
  print("enter figure name")
  sys.exit()
@@ -163,12 +157,12 @@
 eimg.save("p.png")
 # How to tune Canny coefficient in pillbug_count.py
 You should tune and change Canny coefficient instead of "75".
 outline = cv2.Canny(blurred, 0, 75*coeff)
 # Cell counting
 In bioprocessing, reagents such as A100 can be used to disaggregate
 aggregated cell masses and automate cell counting.
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/
 cells.png]Image source: https://bitesizebio.com/30184/quick-easy-automatic-
 cell-counting/
 $ bugcount cells.png
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/r-cells.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/r-cells.png]
```

### Comparing `bugcount-0.0.11/README.md` & `bugcount-0.0.7/src/bugcount.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,69 @@
-# A new tool for counting the number of small objects.
-[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/dc7d4ef4-d838-467d-ab87-828e54dbd580/tree)
-
-DOI: https://doi.org/10.24433/CO.4823110.v1
-
-This is under review.
+Metadata-Version: 2.1
+Name: bugcount
+Version: 0.0.7
+Summary: A package for counting bugs
+Home-page: https://github.com/ytakefuji/counting-for-entomologists
+Author: yoshiyasu takefuji
+Author-email: takefuji@keio.jp
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/ytakefuji/counting-for-entomologists
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
+# A new tool for counting the number of small objects.
 bugcount is a useful tool for entomologists to count the number of bugs.
 
-bugcount has been downloaded by 12155 users worldwide as of July 21, 2023.
-
 # How to install this package:
 $ pip install bugcount
 
-$ pip install bugcount --force-reinstall --no-cache-dir --no-binary :all:
-
 You need to update the opencv-python library to the latest version:
 
 $ pip install -U opencv-python --user
 
 # How to use this bugcount:
 In command terminal, type bugcount file-name or bugcount file-name Canny-coeffient
 
 $ bugcount filename
 
 or
 
 You must download pillbug.png file:
 
-https://github.com/y-takefuji/counting-for-entomologists/raw/main/pillbug.png
+https://github.com/ytakefuji/counting-for-entomologists/raw/main/pillbug.png
 
 $ bugcount pillbug.png
 
-<img src="https://github.com/y-takefuji/counting-for-entomologists/raw/main/r75.png" width=270 height=275>
+<img src="https://github.com/ytakefuji/counting-for-entomologists/raw/main/r75.png" width=270 height=275>
 
 $ bugcount filename Canny-coeffient
 
 Default Canny-coeffient is 75.
 
 or 
 
 $ bugcount pillbug.png 10
 
-<img src="https://github.com/y-takefuji/counting-for-entomologists/raw/main/r10.png" width=270 height=275>
+<img src="https://github.com/ytakefuji/counting-for-entomologists/raw/main/r10.png" width=270 height=275>
 
 $ bugcount pillbug.png 100
 
-<img src="https://github.com/y-takefuji/counting-for-entomologists/raw/main/r100.png" width=270 height=275>
+<img src="https://github.com/ytakefuji/counting-for-entomologists/raw/main/r100.png" width=270 height=275>
 
 pillbug.png file is a target image for counting the number of bugs. 
 
 The smaller Canny coeffient, the more minute objects can be detected.
 
 # Detailed program of bugcount.py and pillbug_count.py
-bugcount has been downloaded by 5513 users worldwide.
+
 <pre>
 This new repository introduces a new tool on object counting for entomologists.
 
 bugcount.py or bugcount is an executable pypi version program while 
 pillbug_count.py is a modifiable program for researchers. 
 
 Counting the number of dead bugs or insect corpses on a plane is tedius 
@@ -104,15 +111,15 @@
 
 This repository shows how to use a Python program (pillbug_count.py) 
 for novice users to automatically count the number of dead bugs or 
 the number of insect corpses on a plane for entomologists.
 
 In order to run pillbug_count.py, you should see the following repository 
 for installing the necessary libraries:
-<a href="https://github.com/y-takefuji/python-novice"> How to install and use libraries in Python for novice users</a>
+<a href="https://github.com/ytakefuji/python-novice"> How to install and use libraries in Python for novice users</a>
 
 1. To install an executable Python environment on your operating system 
    (Windows, Mac, Linux), 
    download a Miniconda3 .sh file or .exe file for Python3.8 or Python3.7 
    from the following site:
 
 <a href="https://docs.conda.io/en/latest/miniconda.html">https://docs.conda.io/en/latest/miniconda.html</a>
@@ -122,27 +129,27 @@
    $ bash Miniconda3XXX.sh
 3. You need to install opencv libray, 
    type the following pip command for installation:
    $ pip install opencv-python
 4. To run pillbug_count.py, type the following command for testing:
    $ python pillbug_count.py pillbug.png
 </pre>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/result1.png' height=246 width=1031>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/result1.png' height=246 width=1031>
 
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/result2.png' height=380 width=366>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/result2.png' height=380 width=366>
 Result: 53 objects (blobs) are found in pillbug.png file.
 <pre>
 Use flies.png for further testing.
 $ python pillbug_count.py flies.png
 </pre>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/flies.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/gray.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/blur.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/edges.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/r.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/flies.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/gray.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/blur.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/edges.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/r.png' height=200 width=300>
 
 
 
 # You should resize an original picture for counting the number of dead bugs. And/or you should tune the Canny coefficient.
 
 
 # How to tune parameters for counting in general
@@ -221,15 +228,17 @@
 # Cell counting
 <pre>
 In bioprocessing, reagents such as A100 can be used to disaggregate 
 aggregated cell masses and automate cell counting.
 
 </pre>
 
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/cells.png' height=300 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/cells.png' height=300 width=300>
 Image source: https://bitesizebio.com/30184/quick-easy-automatic-cell-counting/
 
 <pre>
 $ bugcount cells.png
 
 </pre>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/r-cells.png' height=300 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/r-cells.png' height=300 width=300>
+
+
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
-# A new tool for counting the number of small objects. [![Open in Code Ocean]
-(https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://
-codeocean.com/capsule/dc7d4ef4-d838-467d-ab87-828e54dbd580/tree) DOI: https://
-doi.org/10.24433/CO.4823110.v1 This is under review. bugcount is a useful tool
-for entomologists to count the number of bugs. bugcount has been downloaded by
-12155 users worldwide as of July 21, 2023. # How to install this package: $ pip
-install bugcount $ pip install bugcount --force-reinstall --no-cache-dir --no-
-binary :all: You need to update the opencv-python library to the latest
-version: $ pip install -U opencv-python --user # How to use this bugcount: In
-command terminal, type bugcount file-name or bugcount file-name Canny-coeffient
-$ bugcount filename or You must download pillbug.png file: https://github.com/
-y-takefuji/counting-for-entomologists/raw/main/pillbug.png $ bugcount
-pillbug.png [https://github.com/y-takefuji/counting-for-entomologists/raw/main/
-r75.png]$ bugcount filename Canny-coeffient Default Canny-coeffient is 75. or $
-bugcount pillbug.png 10 [https://github.com/y-takefuji/counting-for-
-entomologists/raw/main/r10.png]$ bugcount pillbug.png 100 [https://github.com/
-y-takefuji/counting-for-entomologists/raw/main/r100.png]pillbug.png file is a
-target image for counting the number of bugs. The smaller Canny coeffient, the
-more minute objects can be detected. # Detailed program of bugcount.py and
-pillbug_count.py bugcount has been downloaded by 5513 users worldwide.
+Metadata-Version: 2.1 Name: bugcount Version: 0.0.7 Summary: A package for
+counting bugs Home-page: https://github.com/ytakefuji/counting-for-
+entomologists Author: yoshiyasu takefuji Author-email: takefuji@keio.jp
+License: UNKNOWN Project-URL: Bug Tracker, https://github.com/ytakefuji/
+counting-for-entomologists Platform: UNKNOWN Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
+Type: text/markdown License-File: LICENSE.txt # A new tool for counting the
+number of small objects. bugcount is a useful tool for entomologists to count
+the number of bugs. # How to install this package: $ pip install bugcount You
+need to update the opencv-python library to the latest version: $ pip install -
+U opencv-python --user # How to use this bugcount: In command terminal, type
+bugcount file-name or bugcount file-name Canny-coeffient $ bugcount filename or
+You must download pillbug.png file: https://github.com/ytakefuji/counting-for-
+entomologists/raw/main/pillbug.png $ bugcount pillbug.png [https://github.com/
+ytakefuji/counting-for-entomologists/raw/main/r75.png]$ bugcount filename
+Canny-coeffient Default Canny-coeffient is 75. or $ bugcount pillbug.png 10
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/r10.png]$
+bugcount pillbug.png 100 [https://github.com/ytakefuji/counting-for-
+entomologists/raw/main/r100.png]pillbug.png file is a target image for counting
+the number of bugs. The smaller Canny coeffient, the more minute objects can be
+detected. # Detailed program of bugcount.py and pillbug_count.py
 This new repository introduces a new tool on object counting for entomologists.
 
 bugcount.py or bugcount is an executable pypi version program while
 pillbug_count.py is a modifiable program for researchers.
 
 Counting the number of dead bugs or insect corpses on a plane is tedius
 and a very time-consuming task.
@@ -81,24 +83,24 @@
    your terminal:
    $ bash Miniconda3XXX.sh
 3. You need to install opencv libray,
    type the following pip command for installation:
    $ pip install opencv-python
 4. To run pillbug_count.py, type the following command for testing:
    $ python pillbug_count.py pillbug.png
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/result1.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/result1.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/
 result2.png]Result: 53 objects (blobs) are found in pillbug.png file.
 Use flies.png for further testing.
 $ python pillbug_count.py flies.png
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/flies.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/gray.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/blur.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/edges.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/r.png]# You
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/flies.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/gray.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/blur.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/edges.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/r.png]# You
 should resize an original picture for counting the number of dead bugs. And/or
 you should tune the Canny coefficient. # How to tune parameters for counting in
 general pillbug_count.py is shown:
 import cv2,sys
 if len(sys.argv)<2:
  print("enter figure name")
  sys.exit()
@@ -155,12 +157,12 @@
 eimg.save("p.png")
 # How to tune Canny coefficient in pillbug_count.py
 You should tune and change Canny coefficient instead of "75".
 outline = cv2.Canny(blurred, 0, 75*coeff)
 # Cell counting
 In bioprocessing, reagents such as A100 can be used to disaggregate
 aggregated cell masses and automate cell counting.
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/
 cells.png]Image source: https://bitesizebio.com/30184/quick-easy-automatic-
 cell-counting/
 $ bugcount cells.png
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/r-cells.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/r-cells.png]
```

### Comparing `bugcount-0.0.11/setup.py` & `bugcount-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bugcount",
-    version="0.0.11",
+    version="0.0.7",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
-    description="A package for counting BLOB objects",
+    description="A package for counting bugs",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/y-takefuji/counting-for-entomologists",
+    url="https://github.com/ytakefuji/counting-for-entomologists",
     project_urls={
-        "Bug Tracker": "https://github.com/y-takefuji/counting-for-entomologists",
+        "Bug Tracker": "https://github.com/ytakefuji/counting-for-entomologists",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['bugcount'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.8",
+    python_requires=">=3.6",
     entry_points = {
         'console_scripts': [
             'bugcount = bugcount:main'
         ]
     },
 )
```

### Comparing `bugcount-0.0.11/src/bugcount.egg-info/PKG-INFO` & `bugcount-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,78 +1,52 @@
-Metadata-Version: 2.1
-Name: bugcount
-Version: 0.0.11
-Summary: A package for counting BLOB objects
-Home-page: https://github.com/y-takefuji/counting-for-entomologists
-Author: yoshiyasu takefuji
-Author-email: takefuji@keio.jp
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/y-takefuji/counting-for-entomologists
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # A new tool for counting the number of small objects.
-[![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://codeocean.com/capsule/dc7d4ef4-d838-467d-ab87-828e54dbd580/tree)
-
-DOI: https://doi.org/10.24433/CO.4823110.v1
-
-This is under review.
-
 bugcount is a useful tool for entomologists to count the number of bugs.
 
-bugcount has been downloaded by 12155 users worldwide as of July 21, 2023.
-
 # How to install this package:
 $ pip install bugcount
 
-$ pip install bugcount --force-reinstall --no-cache-dir --no-binary :all:
-
 You need to update the opencv-python library to the latest version:
 
 $ pip install -U opencv-python --user
 
 # How to use this bugcount:
 In command terminal, type bugcount file-name or bugcount file-name Canny-coeffient
 
 $ bugcount filename
 
 or
 
 You must download pillbug.png file:
 
-https://github.com/y-takefuji/counting-for-entomologists/raw/main/pillbug.png
+https://github.com/ytakefuji/counting-for-entomologists/raw/main/pillbug.png
 
 $ bugcount pillbug.png
 
-<img src="https://github.com/y-takefuji/counting-for-entomologists/raw/main/r75.png" width=270 height=275>
+<img src="https://github.com/ytakefuji/counting-for-entomologists/raw/main/r75.png" width=270 height=275>
 
 $ bugcount filename Canny-coeffient
 
 Default Canny-coeffient is 75.
 
 or 
 
 $ bugcount pillbug.png 10
 
-<img src="https://github.com/y-takefuji/counting-for-entomologists/raw/main/r10.png" width=270 height=275>
+<img src="https://github.com/ytakefuji/counting-for-entomologists/raw/main/r10.png" width=270 height=275>
 
 $ bugcount pillbug.png 100
 
-<img src="https://github.com/y-takefuji/counting-for-entomologists/raw/main/r100.png" width=270 height=275>
+<img src="https://github.com/ytakefuji/counting-for-entomologists/raw/main/r100.png" width=270 height=275>
 
 pillbug.png file is a target image for counting the number of bugs. 
 
 The smaller Canny coeffient, the more minute objects can be detected.
 
 # Detailed program of bugcount.py and pillbug_count.py
-bugcount has been downloaded by 5513 users worldwide.
+
 <pre>
 This new repository introduces a new tool on object counting for entomologists.
 
 bugcount.py or bugcount is an executable pypi version program while 
 pillbug_count.py is a modifiable program for researchers. 
 
 Counting the number of dead bugs or insect corpses on a plane is tedius 
@@ -120,15 +94,15 @@
 
 This repository shows how to use a Python program (pillbug_count.py) 
 for novice users to automatically count the number of dead bugs or 
 the number of insect corpses on a plane for entomologists.
 
 In order to run pillbug_count.py, you should see the following repository 
 for installing the necessary libraries:
-<a href="https://github.com/y-takefuji/python-novice"> How to install and use libraries in Python for novice users</a>
+<a href="https://github.com/ytakefuji/python-novice"> How to install and use libraries in Python for novice users</a>
 
 1. To install an executable Python environment on your operating system 
    (Windows, Mac, Linux), 
    download a Miniconda3 .sh file or .exe file for Python3.8 or Python3.7 
    from the following site:
 
 <a href="https://docs.conda.io/en/latest/miniconda.html">https://docs.conda.io/en/latest/miniconda.html</a>
@@ -138,27 +112,27 @@
    $ bash Miniconda3XXX.sh
 3. You need to install opencv libray, 
    type the following pip command for installation:
    $ pip install opencv-python
 4. To run pillbug_count.py, type the following command for testing:
    $ python pillbug_count.py pillbug.png
 </pre>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/result1.png' height=246 width=1031>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/result1.png' height=246 width=1031>
 
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/result2.png' height=380 width=366>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/result2.png' height=380 width=366>
 Result: 53 objects (blobs) are found in pillbug.png file.
 <pre>
 Use flies.png for further testing.
 $ python pillbug_count.py flies.png
 </pre>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/flies.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/gray.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/blur.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/edges.png' height=200 width=300>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/r.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/flies.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/gray.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/blur.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/edges.png' height=200 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/r.png' height=200 width=300>
 
 
 
 # You should resize an original picture for counting the number of dead bugs. And/or you should tune the Canny coefficient.
 
 
 # How to tune parameters for counting in general
@@ -237,17 +211,15 @@
 # Cell counting
 <pre>
 In bioprocessing, reagents such as A100 can be used to disaggregate 
 aggregated cell masses and automate cell counting.
 
 </pre>
 
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/cells.png' height=300 width=300>
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/cells.png' height=300 width=300>
 Image source: https://bitesizebio.com/30184/quick-easy-automatic-cell-counting/
 
 <pre>
 $ bugcount cells.png
 
 </pre>
-<img src='https://github.com/y-takefuji/counting-for-entomologists/raw/main/r-cells.png' height=300 width=300>
-
-
+<img src='https://github.com/ytakefuji/counting-for-entomologists/raw/main/r-cells.png' height=300 width=300>
```

#### html2text {}

```diff
@@ -1,35 +1,22 @@
-Metadata-Version: 2.1 Name: bugcount Version: 0.0.11 Summary: A package for
-counting BLOB objects Home-page: https://github.com/y-takefuji/counting-for-
-entomologists Author: yoshiyasu takefuji Author-email: takefuji@keio.jp
-License: UNKNOWN Project-URL: Bug Tracker, https://github.com/y-takefuji/
-counting-for-entomologists Platform: UNKNOWN Classifier: Programming Language
-:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
-Type: text/markdown # A new tool for counting the number of small objects. [!
-[Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-
-ocean.svg)](https://codeocean.com/capsule/dc7d4ef4-d838-467d-ab87-828e54dbd580/
-tree) DOI: https://doi.org/10.24433/CO.4823110.v1 This is under review.
-bugcount is a useful tool for entomologists to count the number of bugs.
-bugcount has been downloaded by 12155 users worldwide as of July 21, 2023. #
-How to install this package: $ pip install bugcount $ pip install bugcount --
-force-reinstall --no-cache-dir --no-binary :all: You need to update the opencv-
-python library to the latest version: $ pip install -U opencv-python --user #
-How to use this bugcount: In command terminal, type bugcount file-name or
-bugcount file-name Canny-coeffient $ bugcount filename or You must download
-pillbug.png file: https://github.com/y-takefuji/counting-for-entomologists/raw/
-main/pillbug.png $ bugcount pillbug.png [https://github.com/y-takefuji/
-counting-for-entomologists/raw/main/r75.png]$ bugcount filename Canny-coeffient
-Default Canny-coeffient is 75. or $ bugcount pillbug.png 10 [https://
-github.com/y-takefuji/counting-for-entomologists/raw/main/r10.png]$ bugcount
-pillbug.png 100 [https://github.com/y-takefuji/counting-for-entomologists/raw/
-main/r100.png]pillbug.png file is a target image for counting the number of
-bugs. The smaller Canny coeffient, the more minute objects can be detected. #
-Detailed program of bugcount.py and pillbug_count.py bugcount has been
-downloaded by 5513 users worldwide.
+# A new tool for counting the number of small objects. bugcount is a useful
+tool for entomologists to count the number of bugs. # How to install this
+package: $ pip install bugcount You need to update the opencv-python library to
+the latest version: $ pip install -U opencv-python --user # How to use this
+bugcount: In command terminal, type bugcount file-name or bugcount file-name
+Canny-coeffient $ bugcount filename or You must download pillbug.png file:
+https://github.com/ytakefuji/counting-for-entomologists/raw/main/pillbug.png $
+bugcount pillbug.png [https://github.com/ytakefuji/counting-for-entomologists/
+raw/main/r75.png]$ bugcount filename Canny-coeffient Default Canny-coeffient is
+75. or $ bugcount pillbug.png 10 [https://github.com/ytakefuji/counting-for-
+entomologists/raw/main/r10.png]$ bugcount pillbug.png 100 [https://github.com/
+ytakefuji/counting-for-entomologists/raw/main/r100.png]pillbug.png file is a
+target image for counting the number of bugs. The smaller Canny coeffient, the
+more minute objects can be detected. # Detailed program of bugcount.py and
+pillbug_count.py
 This new repository introduces a new tool on object counting for entomologists.
 
 bugcount.py or bugcount is an executable pypi version program while
 pillbug_count.py is a modifiable program for researchers.
 
 Counting the number of dead bugs or insect corpses on a plane is tedius
 and a very time-consuming task.
@@ -89,24 +76,24 @@
    your terminal:
    $ bash Miniconda3XXX.sh
 3. You need to install opencv libray,
    type the following pip command for installation:
    $ pip install opencv-python
 4. To run pillbug_count.py, type the following command for testing:
    $ python pillbug_count.py pillbug.png
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/result1.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/result1.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/
 result2.png]Result: 53 objects (blobs) are found in pillbug.png file.
 Use flies.png for further testing.
 $ python pillbug_count.py flies.png
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/flies.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/gray.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/blur.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/edges.png]
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/r.png]# You
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/flies.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/gray.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/blur.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/edges.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/r.png]# You
 should resize an original picture for counting the number of dead bugs. And/or
 you should tune the Canny coefficient. # How to tune parameters for counting in
 general pillbug_count.py is shown:
 import cv2,sys
 if len(sys.argv)<2:
  print("enter figure name")
  sys.exit()
@@ -163,12 +150,12 @@
 eimg.save("p.png")
 # How to tune Canny coefficient in pillbug_count.py
 You should tune and change Canny coefficient instead of "75".
 outline = cv2.Canny(blurred, 0, 75*coeff)
 # Cell counting
 In bioprocessing, reagents such as A100 can be used to disaggregate
 aggregated cell masses and automate cell counting.
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/
 cells.png]Image source: https://bitesizebio.com/30184/quick-easy-automatic-
 cell-counting/
 $ bugcount cells.png
-[https://github.com/y-takefuji/counting-for-entomologists/raw/main/r-cells.png]
+[https://github.com/ytakefuji/counting-for-entomologists/raw/main/r-cells.png]
```

### Comparing `bugcount-0.0.11/src/bugcount.py` & `bugcount-0.0.7/src/bugcount.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,39 @@
 import cv2,sys
 from time import sleep
 canny=75
-def main():
+def main(f,canny):
  img = cv2.imread(f)
  gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
- blurred = cv2.GaussianBlur(gray, (7,7), 0)
- blurred = cv2.GaussianBlur(blurred, (13,13), 0)
- #blurred = cv2.GaussianBlur(blurred, (13,13), 0)
+ blurred = cv2.GaussianBlur(gray, (5,5), 0)
+ blurred = cv2.GaussianBlur(blurred, (7,7), 0)
 
  cv2.imshow("grey scale", gray)
  cv2.imwrite("gray.png", gray)
  cv2.imshow("blurred", blurred)
  cv2.imwrite("blur.png", blurred)
  coeff=int((blurred.max()-blurred.min())/100)
  if coeff==1: coeff=1 
  else: coeff=3
- outline = cv2.Canny(blurred, 1, int(canny))
+ outline = cv2.Canny(blurred, 0, int(canny)*coeff)
  outline= cv2.GaussianBlur(outline, (3,3), 0)
  cv2.imshow("The edges", outline)
  cv2.imwrite("edges.png", outline)
 #(_, cnts, _) = cv2.findContours(outline, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
 #version4
  ( cnts, _)=cv2.findContours(outline,cv2.RETR_EXTERNAL,cv2.CHAIN_APPROX_SIMPLE)
- new=[]
- th=0
- max=0
- for i in cnts:
-  if i.shape[0]>max:
-   max=i.shape[0]
- for i in cnts:
-  if max==i.shape[0]:
-   continue
-  else:
-   th=th+i.shape[0]
- th=int(th/(len(cnts)-1))
- for i in cnts:
-  if (i.shape[0]>th-15):
-   new.append(i)
- cnts=new
  cv2.drawContours(img, cnts, -1, (0, 255, 0), 2)
  cv2.putText(img,str(len(cnts)),(30,30),cv2.FONT_HERSHEY_SIMPLEX,1,(255,0,0),2)
  cv2.imwrite("r.png",img)
  cv2.imshow("Result", img)
  print("%i blobs" % len(cnts))
  sleep(2)
 #cv2.waitKey(0)
  cv2.waitKeyEx(4000)
 if len(sys.argv)==1: 
  print('image file is needed!')
  sys.exit()
-if len(sys.argv)==2: 
- f=sys.argv[1]
- canny=75 
+if len(sys.argv)==2: f=sys.argv[1]
 if len(sys.argv)==3: 
  f=sys.argv[1]
  canny=sys.argv[2]
-main()
+main(f,canny)
```

