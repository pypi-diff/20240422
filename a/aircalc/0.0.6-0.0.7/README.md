# Comparing `tmp/aircalc-0.0.6.tar.gz` & `tmp/aircalc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aircalc-0.0.6.tar", last modified: Sun Apr  3 01:47:36 2022, max compression
+gzip compressed data, was "aircalc-0.0.7.tar", last modified: Mon Apr 22 08:41:36 2024, max compression
```

## Comparing `aircalc-0.0.6.tar` & `aircalc-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-03 01:47:36.604856 aircalc-0.0.6/
--rw-r--r--   0 yt        (1000) yt        (1000)     5353 2022-04-03 01:47:36.601325 aircalc-0.0.6/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     4802 2021-07-14 07:15:38.000000 aircalc-0.0.6/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2022-04-03 01:47:36.605371 aircalc-0.0.6/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      968 2022-04-03 01:44:27.000000 aircalc-0.0.6/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-03 01:47:36.582821 aircalc-0.0.6/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2022-04-03 01:47:36.601325 aircalc-0.0.6/src/aircalc.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     5353 2022-04-03 01:47:36.000000 aircalc-0.0.6/src/aircalc.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      211 2022-04-03 01:47:36.000000 aircalc-0.0.6/src/aircalc.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2022-04-03 01:47:36.000000 aircalc-0.0.6/src/aircalc.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       42 2022-04-03 01:47:36.000000 aircalc-0.0.6/src/aircalc.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        8 2022-04-03 01:47:36.000000 aircalc-0.0.6/src/aircalc.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     6679 2021-07-12 12:53:18.000000 aircalc-0.0.6/src/aircalc.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:41:36.839402 aircalc-0.0.7/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     6245 2024-04-22 08:41:36.839402 aircalc-0.0.7/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     5692 2024-04-22 08:39:42.000000 aircalc-0.0.7/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 08:41:36.839402 aircalc-0.0.7/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      970 2024-04-22 08:41:01.000000 aircalc-0.0.7/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:41:36.839402 aircalc-0.0.7/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 08:41:36.839402 aircalc-0.0.7/src/aircalc.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     6245 2024-04-22 08:41:36.000000 aircalc-0.0.7/src/aircalc.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      211 2024-04-22 08:41:36.000000 aircalc-0.0.7/src/aircalc.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 08:41:36.000000 aircalc-0.0.7/src/aircalc.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       42 2024-04-22 08:41:36.000000 aircalc-0.0.7/src/aircalc.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        8 2024-04-22 08:41:36.000000 aircalc-0.0.7/src/aircalc.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     6679 2021-07-12 12:53:18.000000 aircalc-0.0.7/src/aircalc.py
```

### Comparing `aircalc-0.0.6/PKG-INFO` & `aircalc-0.0.7/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1
-Name: aircalc
-Version: 0.0.6
-Summary: aircalc: calculate a math expression by five fingers in air.
-Home-page: https://github.com/ytakefuji/air_calculator
-Author: yoshiyasu takefuji
-Author-email: takefuji@keio.jp
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/air_calculator
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+# aircalc
+This is under review.
 
-# air_calculator
+aircalc has been downloaded by 20,387 downloads worldwide as of Feb.24, 2023.
+
+aircalc is a Python program based on two state-of-the-art libraries including hand gesture recognition library 
+using mediapipe and optical character recognition library using tesseract. 
+aircalc can be easilly installed by pip command (PyPi).
+This short program is made for education by showing how to use two state-of-the-art libraries.
+aircalc has an error correction function for correcting hand-drawn images in order to achieve perfect image recognition by tesseract.
+
+The paper on aircalc is under submission. If the paper is accepted, the source code will be disclosed with detailed explanations.
+
+The hand gesture recognition allows you to draw a math expression and it will be automatically calculated. The answer will be posted on the screen.
 
 Writing letters with a pen on paper is very different from drawing letters in the air.
 
 Drawing "-" minus operator and "+" operator in the air are extremely difficult so that these operators in the current system are replaced by "W" and "P" respectively.
 
 When drawing letters with fingers in the air, letters that are difficult 
 to recognize or write in the air need to be replaced with letters 
@@ -37,15 +34,15 @@
 
 $ pip install mediapipe
 
 Finally install aircalc
 
 $ pip install aircalc
 
-# fingermath.py is renamed as aircalc.py
+$ pip install aircalc --force-reinstall --no-cache-dir --no-binary :all:
 
 # How to run aircalc
 
 aircalc is a program for drawing a math expression 
 in the air for possible calculation.
 
 aircalc is based on two open source libraries including mediapipe and tesseract.
@@ -95,37 +92,38 @@
 Drawing two letters "a" and "A" in the air represents the sqrt() function.
 Therefore, the string "a13A" or "aL3A" represents sqrt(13).
 
 $ aircalc
 
 https://youtu.be/med_jrFTMPA
 <pre>  sqrt(6)*2=?    </pre>
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/a6AM2.png' width=320 height=240>
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/a6AM2.png' width=320 height=240>
 
-<pre>         1-3=?                                 10+2=?  </pre>
-[![Lw3.gif](https://github.com/ytakefuji/air_calculator/raw/main/Lw3.gif)](https://github.com/ytakefuji/air_calculator) [![10plus2.gif](https://github.com/ytakefuji/air_calculator/raw/main/10plus2.gif)](https://github.com/ytakefuji/air_calculator)
+<pre>         1-3=?                10+2=?  </pre>
+[![Lw3.gif](https://github.com/y-takefuji/air_calculator/raw/main/Lw3.gif)](https://github.com/y-takefuji/air_calculator)    [![10plus2.gif](https://github.com/y-takefuji/air_calculator/raw/main/10plus2.gif)](https://github.com/y-takefuji/air_calculator)
 
 <pre>        4-5-3=?            </pre>
-[![4-5-3.gif](https://github.com/ytakefuji/air_calculator/raw/main/4-5-3.gif) <img src='https://github.com/ytakefuji/air_calculator/raw/main/4-5-3.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_4-5-3.png' width=120 height=90>
+[![4-5-3.gif](https://github.com/y-takefuji/air_calculator/raw/main/4-5-3.gif) <img src='https://github.com/y-takefuji/air_calculator/raw/main/4-5-3.png' width=160 height=120> <img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_4-5-3.png' width=120 height=90>
 
 <pre>        2-3/5=?   </pre>
-[![2-3div5.gif](https://github.com/ytakefuji/air_calculator/raw/main/2-3div5.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/2-3div5.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_2-3div5.png' width=120 height=90>
+[![2-3div5.gif](https://github.com/y-takefuji/air_calculator/raw/main/2-3div5.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/2-3div5.png' width=160 height=120> <img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_2-3div5.png' width=120 height=90>
 
 
 <pre>        34*5=?     </pre>
-[![34M5.gif](https://github.com/ytakefuji/air_calculator/raw/main/34M5.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/34M5.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_34M5.png' width=120 height=90>
+[![34M5.gif](https://github.com/y-takefuji/air_calculator/raw/main/34M5.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/34M5.png' width=160 height=120> 
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_34M5.png' width=120 height=90>
 
 <pre> 2**8=?</pre>
-[![2^8.gif](https://github.com/ytakefuji/air_calculator/raw/main/2^8.gif)
+[![2^8.gif](https://github.com/y-takefuji/air_calculator/raw/main/2^8.gif)
 
 
 <pre>      2&9V3 --> 2**9/3        </pre>
-[![2^9div3.gif](https://github.com/ytakefuji/air_calculator/raw/main/2^9div3.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/2^9div3.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_2^9div3.png' width=120 height=90>
+[![2^9div3.gif](https://github.com/y-takefuji/air_calculator/raw/main/2^9div3.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/2^9div3.png' width=160 height=120> 
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_2^9div3.png' width=120 height=90>
 
 <pre>       aLLAV3=? -> sqrt(11)/3 </pre>  
-[![aLLAV3.gif](https://github.com/ytakefuji/air_calculator/raw/main/aLLAV3.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/aLLAV3.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_aLLAV3.png' width=120 height=90>
-
-
+[![aLLAV3.gif](https://github.com/y-takefuji/air_calculator/raw/main/aLLAV3.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/aLLAV3.png' width=160 height=120> 
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_aLLAV3.png' width=120 height=90>
```

### Comparing `aircalc-0.0.6/README.md` & `aircalc-0.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,37 @@
-# air_calculator
+Metadata-Version: 2.1
+Name: aircalc
+Version: 0.0.7
+Summary: aircalc: calculate a math expression by five fingers in air.
+Home-page: https://github.com/y-takefuji/air_calculator
+Author: yoshiyasu takefuji
+Author-email: takefuji@keio.jp
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/y-takefuji/air_calculator
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+# aircalc
+This is under review.
+
+aircalc has been downloaded by 20,387 downloads worldwide as of Feb.24, 2023.
+
+aircalc is a Python program based on two state-of-the-art libraries including hand gesture recognition library 
+using mediapipe and optical character recognition library using tesseract. 
+aircalc can be easilly installed by pip command (PyPi).
+This short program is made for education by showing how to use two state-of-the-art libraries.
+aircalc has an error correction function for correcting hand-drawn images in order to achieve perfect image recognition by tesseract.
+
+The paper on aircalc is under submission. If the paper is accepted, the source code will be disclosed with detailed explanations.
+
+The hand gesture recognition allows you to draw a math expression and it will be automatically calculated. The answer will be posted on the screen.
 
 Writing letters with a pen on paper is very different from drawing letters in the air.
 
 Drawing "-" minus operator and "+" operator in the air are extremely difficult so that these operators in the current system are replaced by "W" and "P" respectively.
 
 When drawing letters with fingers in the air, letters that are difficult 
 to recognize or write in the air need to be replaced with letters 
@@ -21,15 +50,15 @@
 
 $ pip install mediapipe
 
 Finally install aircalc
 
 $ pip install aircalc
 
-# fingermath.py is renamed as aircalc.py
+$ pip install aircalc --force-reinstall --no-cache-dir --no-binary :all:
 
 # How to run aircalc
 
 aircalc is a program for drawing a math expression 
 in the air for possible calculation.
 
 aircalc is based on two open source libraries including mediapipe and tesseract.
@@ -79,35 +108,40 @@
 Drawing two letters "a" and "A" in the air represents the sqrt() function.
 Therefore, the string "a13A" or "aL3A" represents sqrt(13).
 
 $ aircalc
 
 https://youtu.be/med_jrFTMPA
 <pre>  sqrt(6)*2=?    </pre>
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/a6AM2.png' width=320 height=240>
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/a6AM2.png' width=320 height=240>
 
-<pre>         1-3=?                                 10+2=?  </pre>
-[![Lw3.gif](https://github.com/ytakefuji/air_calculator/raw/main/Lw3.gif)](https://github.com/ytakefuji/air_calculator) [![10plus2.gif](https://github.com/ytakefuji/air_calculator/raw/main/10plus2.gif)](https://github.com/ytakefuji/air_calculator)
+<pre>         1-3=?                10+2=?  </pre>
+[![Lw3.gif](https://github.com/y-takefuji/air_calculator/raw/main/Lw3.gif)](https://github.com/y-takefuji/air_calculator)    [![10plus2.gif](https://github.com/y-takefuji/air_calculator/raw/main/10plus2.gif)](https://github.com/y-takefuji/air_calculator)
 
 <pre>        4-5-3=?            </pre>
-[![4-5-3.gif](https://github.com/ytakefuji/air_calculator/raw/main/4-5-3.gif) <img src='https://github.com/ytakefuji/air_calculator/raw/main/4-5-3.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_4-5-3.png' width=120 height=90>
+[![4-5-3.gif](https://github.com/y-takefuji/air_calculator/raw/main/4-5-3.gif) <img src='https://github.com/y-takefuji/air_calculator/raw/main/4-5-3.png' width=160 height=120> <img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_4-5-3.png' width=120 height=90>
 
 <pre>        2-3/5=?   </pre>
-[![2-3div5.gif](https://github.com/ytakefuji/air_calculator/raw/main/2-3div5.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/2-3div5.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_2-3div5.png' width=120 height=90>
+[![2-3div5.gif](https://github.com/y-takefuji/air_calculator/raw/main/2-3div5.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/2-3div5.png' width=160 height=120> <img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_2-3div5.png' width=120 height=90>
 
 
 <pre>        34*5=?     </pre>
-[![34M5.gif](https://github.com/ytakefuji/air_calculator/raw/main/34M5.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/34M5.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_34M5.png' width=120 height=90>
+[![34M5.gif](https://github.com/y-takefuji/air_calculator/raw/main/34M5.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/34M5.png' width=160 height=120> 
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_34M5.png' width=120 height=90>
 
 <pre> 2**8=?</pre>
-[![2^8.gif](https://github.com/ytakefuji/air_calculator/raw/main/2^8.gif)
+[![2^8.gif](https://github.com/y-takefuji/air_calculator/raw/main/2^8.gif)
 
 
 <pre>      2&9V3 --> 2**9/3        </pre>
-[![2^9div3.gif](https://github.com/ytakefuji/air_calculator/raw/main/2^9div3.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/2^9div3.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_2^9div3.png' width=120 height=90>
+[![2^9div3.gif](https://github.com/y-takefuji/air_calculator/raw/main/2^9div3.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/2^9div3.png' width=160 height=120> 
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_2^9div3.png' width=120 height=90>
 
 <pre>       aLLAV3=? -> sqrt(11)/3 </pre>  
-[![aLLAV3.gif](https://github.com/ytakefuji/air_calculator/raw/main/aLLAV3.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/aLLAV3.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_aLLAV3.png' width=120 height=90>
+[![aLLAV3.gif](https://github.com/y-takefuji/air_calculator/raw/main/aLLAV3.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/aLLAV3.png' width=160 height=120> 
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_aLLAV3.png' width=120 height=90>
+
+
```

### Comparing `aircalc-0.0.6/setup.py` & `aircalc-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aircalc",
-    version="0.0.6",
+    version="0.0.7",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="aircalc: calculate a math expression by five fingers in air.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/air_calculator",
+    url="https://github.com/y-takefuji/air_calculator",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/air_calculator",
+        "Bug Tracker": "https://github.com/y-takefuji/air_calculator",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['aircalc'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'aircalc = aircalc:main'
         ]
     },
 )
```

### Comparing `aircalc-0.0.6/src/aircalc.egg-info/PKG-INFO` & `aircalc-0.0.7/src/aircalc.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 Metadata-Version: 2.1
 Name: aircalc
-Version: 0.0.6
+Version: 0.0.7
 Summary: aircalc: calculate a math expression by five fingers in air.
-Home-page: https://github.com/ytakefuji/air_calculator
+Home-page: https://github.com/y-takefuji/air_calculator
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/air_calculator
+Project-URL: Bug Tracker, https://github.com/y-takefuji/air_calculator
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# air_calculator
+# aircalc
+This is under review.
+
+aircalc has been downloaded by 20,387 downloads worldwide as of Feb.24, 2023.
+
+aircalc is a Python program based on two state-of-the-art libraries including hand gesture recognition library 
+using mediapipe and optical character recognition library using tesseract. 
+aircalc can be easilly installed by pip command (PyPi).
+This short program is made for education by showing how to use two state-of-the-art libraries.
+aircalc has an error correction function for correcting hand-drawn images in order to achieve perfect image recognition by tesseract.
+
+The paper on aircalc is under submission. If the paper is accepted, the source code will be disclosed with detailed explanations.
+
+The hand gesture recognition allows you to draw a math expression and it will be automatically calculated. The answer will be posted on the screen.
 
 Writing letters with a pen on paper is very different from drawing letters in the air.
 
 Drawing "-" minus operator and "+" operator in the air are extremely difficult so that these operators in the current system are replaced by "W" and "P" respectively.
 
 When drawing letters with fingers in the air, letters that are difficult 
 to recognize or write in the air need to be replaced with letters 
@@ -37,15 +50,15 @@
 
 $ pip install mediapipe
 
 Finally install aircalc
 
 $ pip install aircalc
 
-# fingermath.py is renamed as aircalc.py
+$ pip install aircalc --force-reinstall --no-cache-dir --no-binary :all:
 
 # How to run aircalc
 
 aircalc is a program for drawing a math expression 
 in the air for possible calculation.
 
 aircalc is based on two open source libraries including mediapipe and tesseract.
@@ -95,37 +108,40 @@
 Drawing two letters "a" and "A" in the air represents the sqrt() function.
 Therefore, the string "a13A" or "aL3A" represents sqrt(13).
 
 $ aircalc
 
 https://youtu.be/med_jrFTMPA
 <pre>  sqrt(6)*2=?    </pre>
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/a6AM2.png' width=320 height=240>
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/a6AM2.png' width=320 height=240>
 
-<pre>         1-3=?                                 10+2=?  </pre>
-[![Lw3.gif](https://github.com/ytakefuji/air_calculator/raw/main/Lw3.gif)](https://github.com/ytakefuji/air_calculator) [![10plus2.gif](https://github.com/ytakefuji/air_calculator/raw/main/10plus2.gif)](https://github.com/ytakefuji/air_calculator)
+<pre>         1-3=?                10+2=?  </pre>
+[![Lw3.gif](https://github.com/y-takefuji/air_calculator/raw/main/Lw3.gif)](https://github.com/y-takefuji/air_calculator)    [![10plus2.gif](https://github.com/y-takefuji/air_calculator/raw/main/10plus2.gif)](https://github.com/y-takefuji/air_calculator)
 
 <pre>        4-5-3=?            </pre>
-[![4-5-3.gif](https://github.com/ytakefuji/air_calculator/raw/main/4-5-3.gif) <img src='https://github.com/ytakefuji/air_calculator/raw/main/4-5-3.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_4-5-3.png' width=120 height=90>
+[![4-5-3.gif](https://github.com/y-takefuji/air_calculator/raw/main/4-5-3.gif) <img src='https://github.com/y-takefuji/air_calculator/raw/main/4-5-3.png' width=160 height=120> <img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_4-5-3.png' width=120 height=90>
 
 <pre>        2-3/5=?   </pre>
-[![2-3div5.gif](https://github.com/ytakefuji/air_calculator/raw/main/2-3div5.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/2-3div5.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_2-3div5.png' width=120 height=90>
+[![2-3div5.gif](https://github.com/y-takefuji/air_calculator/raw/main/2-3div5.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/2-3div5.png' width=160 height=120> <img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_2-3div5.png' width=120 height=90>
 
 
 <pre>        34*5=?     </pre>
-[![34M5.gif](https://github.com/ytakefuji/air_calculator/raw/main/34M5.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/34M5.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_34M5.png' width=120 height=90>
+[![34M5.gif](https://github.com/y-takefuji/air_calculator/raw/main/34M5.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/34M5.png' width=160 height=120> 
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_34M5.png' width=120 height=90>
 
 <pre> 2**8=?</pre>
-[![2^8.gif](https://github.com/ytakefuji/air_calculator/raw/main/2^8.gif)
+[![2^8.gif](https://github.com/y-takefuji/air_calculator/raw/main/2^8.gif)
 
 
 <pre>      2&9V3 --> 2**9/3        </pre>
-[![2^9div3.gif](https://github.com/ytakefuji/air_calculator/raw/main/2^9div3.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/2^9div3.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_2^9div3.png' width=120 height=90>
+[![2^9div3.gif](https://github.com/y-takefuji/air_calculator/raw/main/2^9div3.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/2^9div3.png' width=160 height=120> 
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_2^9div3.png' width=120 height=90>
 
 <pre>       aLLAV3=? -> sqrt(11)/3 </pre>  
-[![aLLAV3.gif](https://github.com/ytakefuji/air_calculator/raw/main/aLLAV3.gif)
-<img src='https://github.com/ytakefuji/air_calculator/raw/main/aLLAV3.png' width=160 height=120> <img src='https://github.com/ytakefuji/air_calculator/raw/main/resize_aLLAV3.png' width=120 height=90>
+[![aLLAV3.gif](https://github.com/y-takefuji/air_calculator/raw/main/aLLAV3.gif)
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/aLLAV3.png' width=160 height=120> 
+<img src='https://github.com/y-takefuji/air_calculator/raw/main/resize_aLLAV3.png' width=120 height=90>
```

### Comparing `aircalc-0.0.6/src/aircalc.py` & `aircalc-0.0.7/src/aircalc.py`

 * *Files identical despite different names*

