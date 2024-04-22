# Comparing `tmp/fisspy-1.0.2.tar.gz` & `tmp/fisspy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fisspy-1.0.2.tar", last modified: Sun Apr 21 06:26:17 2024, max compression
+gzip compressed data, was "fisspy-1.0.3.tar", last modified: Mon Apr 22 04:52:32 2024, max compression
```

## Comparing `fisspy-1.0.2.tar` & `fisspy-1.0.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.145060 fisspy-1.0.2/
--rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.2/LICENSE.txt
--rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-21 06:26:17.144943 fisspy-1.0.2/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1195 2024-04-20 02:57:09.000000 fisspy-1.0.2/README.md
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.134503 fisspy-1.0.2/fisspy/
--rw-r--r--   0 jhkang     (501) staff       (20)      386 2024-04-21 00:44:56.000000 fisspy-1.0.2/fisspy/__init__.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.135955 fisspy-1.0.2/fisspy/align/
--rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/align/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    14644 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/align/alignment.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/align/base.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.137817 fisspy-1.0.2/fisspy/analysis/
--rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/analysis/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/analysis/doppler.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/analysis/filter.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-21 06:20:03.000000 fisspy-1.0.2/fisspy/analysis/forecast.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/analysis/ofe.py
--rw-r--r--   0 jhkang     (501) staff       (20)    35499 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/analysis/tdmap.py
--rw-r--r--   0 jhkang     (501) staff       (20)    33899 2024-04-20 03:48:27.000000 fisspy-1.0.2/fisspy/analysis/wavelet.py
--rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.2/fisspy/cm.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.139177 fisspy-1.0.2/fisspy/correction/
--rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/correction/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/correction/correction.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/correction/get_inform.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.139874 fisspy-1.0.2/fisspy/data/
--rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.2/fisspy/data/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.2/fisspy/data/_sample.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.2/fisspy/data/download.py
--rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.2/fisspy/data/sample.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.140927 fisspy-1.0.2/fisspy/image/
--rw-r--r--   0 jhkang     (501) staff       (20)      110 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/image/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12576 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/image/base.py
--rw-r--r--   0 jhkang     (501) staff       (20)    29760 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/image/interactive_image.py
--rw-r--r--   0 jhkang     (501) staff       (20)     7860 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/image/raster_set.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.141342 fisspy-1.0.2/fisspy/inversion/
--rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/inversion/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/inversion/_mlsi.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.141781 fisspy-1.0.2/fisspy/io/
--rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.2/fisspy/io/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.2/fisspy/io/read.py
--rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/makevideo.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.143538 fisspy-1.0.2/fisspy/preprocess/
--rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/preprocess/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    52473 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/preprocess/proc_base.py
--rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/preprocess/proc_gui.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/preprocess/t_y_sh.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.144599 fisspy-1.0.2/fisspy/read/
--rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/read/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    47710 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/read/read_factory.py
--rw-r--r--   0 jhkang     (501) staff       (20)     6813 2024-04-20 02:57:09.000000 fisspy-1.0.2/fisspy/read/readbase.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-21 06:26:17.135324 fisspy-1.0.2/fisspy.egg-info/
--rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1100 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/SOURCES.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/dependency_links.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/not-zip-safe
--rw-r--r--   0 jhkang     (501) staff       (20)      130 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/requires.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-21 06:26:17.000000 fisspy-1.0.2/fisspy.egg-info/top_level.txt
--rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-21 06:26:17.145099 fisspy-1.0.2/setup.cfg
--rw-r--r--   0 jhkang     (501) staff       (20)      619 2024-04-21 00:44:41.000000 fisspy-1.0.2/setup.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.939066 fisspy-1.0.3/
+-rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.3/LICENSE.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)      572 2024-04-22 04:52:32.938874 fisspy-1.0.3/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1196 2024-04-21 23:57:55.000000 fisspy-1.0.3/README.md
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.926957 fisspy-1.0.3/fisspy/
+-rw-r--r--   0 jhkang     (501) staff       (20)      386 2024-04-22 04:51:09.000000 fisspy-1.0.3/fisspy/__init__.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.928411 fisspy-1.0.3/fisspy/align/
+-rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/align/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    14687 2024-04-22 04:33:23.000000 fisspy-1.0.3/fisspy/align/alignment.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/align/base.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.930400 fisspy-1.0.3/fisspy/analysis/
+-rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/analysis/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/analysis/doppler.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/analysis/filter.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-21 06:20:03.000000 fisspy-1.0.3/fisspy/analysis/forecast.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/analysis/ofe.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    35499 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/analysis/tdmap.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    33899 2024-04-20 03:48:27.000000 fisspy-1.0.3/fisspy/analysis/wavelet.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.3/fisspy/cm.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.931857 fisspy-1.0.3/fisspy/correction/
+-rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/correction/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/correction/correction.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/correction/get_inform.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.932865 fisspy-1.0.3/fisspy/data/
+-rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.3/fisspy/data/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.3/fisspy/data/_sample.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.3/fisspy/data/download.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.3/fisspy/data/sample.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.933980 fisspy-1.0.3/fisspy/image/
+-rw-r--r--   0 jhkang     (501) staff       (20)      110 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/image/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12576 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/image/base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    29760 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/image/interactive_image.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     7860 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/image/raster_set.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.934374 fisspy-1.0.3/fisspy/inversion/
+-rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/inversion/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/inversion/_mlsi.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.934949 fisspy-1.0.3/fisspy/io/
+-rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.3/fisspy/io/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.3/fisspy/io/read.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/makevideo.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.937130 fisspy-1.0.3/fisspy/preprocess/
+-rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/preprocess/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    52473 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/preprocess/proc_base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/preprocess/proc_gui.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/preprocess/t_y_sh.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.938482 fisspy-1.0.3/fisspy/read/
+-rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/read/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    47723 2024-04-22 03:30:24.000000 fisspy-1.0.3/fisspy/read/read_factory.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     6813 2024-04-20 02:57:09.000000 fisspy-1.0.3/fisspy/read/readbase.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-22 04:52:32.927770 fisspy-1.0.3/fisspy.egg-info/
+-rw-r--r--   0 jhkang     (501) staff       (20)      572 2024-04-22 04:52:32.000000 fisspy-1.0.3/fisspy.egg-info/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1100 2024-04-22 04:52:32.000000 fisspy-1.0.3/fisspy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-22 04:52:32.000000 fisspy-1.0.3/fisspy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-22 04:52:32.000000 fisspy-1.0.3/fisspy.egg-info/not-zip-safe
+-rw-r--r--   0 jhkang     (501) staff       (20)      135 2024-04-22 04:52:32.000000 fisspy-1.0.3/fisspy.egg-info/requires.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-22 04:52:32.000000 fisspy-1.0.3/fisspy.egg-info/top_level.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-22 04:52:32.939102 fisspy-1.0.3/setup.cfg
+-rw-r--r--   0 jhkang     (501) staff       (20)      580 2024-04-22 04:51:09.000000 fisspy-1.0.3/setup.py
```

### Comparing `fisspy-1.0.2/LICENSE.txt` & `fisspy-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/README.md` & `fisspy-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # FISSPy
 
 [![Latest Version](https://img.shields.io/pypi/v/fisspy.svg)](https://pypi.python.org/pypi/fisspy/) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/fisspy/badges/version.svg)](https://anaconda.org/conda-forge/fisspy) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/fisspy/badges/downloads.svg)](https://anaconda.org/conda-forge/fisspy)
 
-The Python Package for data analysis of the [GST/FISS instrument](http://fiss.snu.ac.kr/)
+The Python Package for data analysis of the [GST/FISS instrument](http://fiss.snu.ac.kr/).
 
 Installation
 ------------
 
 Requirement Package:
 
 * [Python](http://www.python.org) >=3.6
```

### Comparing `fisspy-1.0.2/fisspy/align/alignment.py` & `fisspy-1.0.3/fisspy/align/alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from astropy.time import Time
 from ..read import FISS
 from os.path import join
 from os import getcwd
 
 __author__ = "Juhyung Kang"
 __email__ = "jhkang0301@gmail.com"
-__all__= ["calAlignPars", "alignCams", "writeAlignPars", "readAlignPars", "alignAll", "alignDataCube"]
+__all__= ["calAlignPars", "alignCams", "writeAlignPars", "readAlignPars", "alignAll", "alignDataCube", 'alignTwoDataCubes', 'saveAlignCube', 'makeExample']
 
 def calAlignPars(lfiles, refFrame=None):
     """
     Calculate the parameters to be used for the alignment for given series of the line spectra.
 
     Parameters
     ----------
@@ -359,15 +359,15 @@
     cdata = np.zeros((nt, ny+2*ym, nx+2*xm),dtype='float')
 
     for i, d in enumerate(data):
         rimg = rotImage(d[:,::-1], ang[i],
                         xc=xc[i], yc=yc[i],
                         dx=apar['dx'][i],
                         dy=apar['dy'][i],
-                        xmargin=xmargin, ymargin=ymargin,
+                        xmargin=xm, ymargin=ym,
                         cubic=cubic)
         cdata[i] = rimg
 
     return cdata
 
 def alignTwoDataCubes(dataA, dataB, faparA, faparB, cubic=False):
     """
```

### Comparing `fisspy-1.0.2/fisspy/align/base.py` & `fisspy-1.0.3/fisspy/align/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/analysis/doppler.py` & `fisspy-1.0.3/fisspy/analysis/doppler.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/analysis/filter.py` & `fisspy-1.0.3/fisspy/analysis/filter.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/analysis/forecast.py` & `fisspy-1.0.3/fisspy/analysis/forecast.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/analysis/ofe.py` & `fisspy-1.0.3/fisspy/analysis/ofe.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/analysis/tdmap.py` & `fisspy-1.0.3/fisspy/analysis/tdmap.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/analysis/wavelet.py` & `fisspy-1.0.3/fisspy/analysis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/cm.py` & `fisspy-1.0.3/fisspy/cm.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/correction/correction.py` & `fisspy-1.0.3/fisspy/correction/correction.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/correction/get_inform.py` & `fisspy-1.0.3/fisspy/correction/get_inform.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/data/_sample.py` & `fisspy-1.0.3/fisspy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/data/download.py` & `fisspy-1.0.3/fisspy/data/download.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/image/base.py` & `fisspy-1.0.3/fisspy/image/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/image/interactive_image.py` & `fisspy-1.0.3/fisspy/image/interactive_image.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/image/raster_set.py` & `fisspy-1.0.3/fisspy/image/raster_set.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/io/read.py` & `fisspy-1.0.3/fisspy/io/read.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/makevideo.py` & `fisspy-1.0.3/fisspy/makevideo.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/preprocess/proc_base.py` & `fisspy-1.0.3/fisspy/preprocess/proc_base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/preprocess/proc_gui.py` & `fisspy-1.0.3/fisspy/preprocess/proc_gui.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/preprocess/t_y_sh.py` & `fisspy-1.0.3/fisspy/preprocess/t_y_sh.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy/read/read_factory.py` & `fisspy-1.0.3/fisspy/read/read_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ..analysis import lambdameter
 from ..image import interactive_image as II
 from ..correction import LineName, wvCalib, smoothingProf
 from ..analysis import FourierFilter, Wavelet, makeTDmap
 
 __author__= "Juhyung Kang"
 __email__ = "jhkang0301@gmail.com"
-__all__ = ["rawData", "FISS", "FD", "calibData"]
+__all__ = ["rawData", "FISS", "FD", "calibData", "AlignCube"]
 
 class rawData:
     """
     Read a raw file of the FISS.
 
     Parameters
     ----------
```

### Comparing `fisspy-1.0.2/fisspy/read/readbase.py` & `fisspy-1.0.3/fisspy/read/readbase.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/fisspy.egg-info/SOURCES.txt` & `fisspy-1.0.3/fisspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.2/setup.py` & `fisspy-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fisspy',
-    version='1.0.2',
+    version='1.0.3',
     description='fisspy: Python analysis tools for GST/FISS',
     url='http://fiss.snu.ac.kr',
     author='Juhyung Kang',
     author_email='jhkang@astro.snu.ac.kr',
     license='BSD-2',
     python_requires='>=3.6',
     packages=find_packages(exclude=['docs', 'logo']),
-    install_requires=["numba", "numpy", "scipy>=1.5", "astropy>=5.0",
-                      "sunpy>=2.0.0", "matplotlib>=3.0",
-                      "interpolation>=2.2", "statsmodels", "beautifulsoup4", "pandas", "ffmpeg", "pyqt"],
+    install_requires=["numba", "numpy", "scipy>=1.5", "astropy>=5.0", "sunpy>=2.0.0", "matplotlib>=3.0", "interpolation>=2.2", "statsmodels", "beautifulsoup4", "pandas", "ffmpeg", "pyqt>=5.0"],
     zip_safe=False
     )
```

