# Comparing `tmp/extractstructuresMC-1.0.0.0.tar.gz` & `tmp/extractstructuresMC-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extractstructuresMC-1.0.0.0.tar", last modified: Mon Jan 22 16:11:19 2024, max compression
+gzip compressed data, was "extractstructuresMC-1.0.0.1.tar", last modified: Mon Apr 22 08:47:58 2024, max compression
```

## Comparing `extractstructuresMC-1.0.0.0.tar` & `extractstructuresMC-1.0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aparas   (42669) spec        (62)        0 2024-01-22 16:11:19.258709 extractstructuresMC-1.0.0.0/
--rw-r--r--   0 aparas   (42669) spec        (62)      544 2024-01-22 16:11:19.258709 extractstructuresMC-1.0.0.0/PKG-INFO
--rw-r--r--   0 aparas   (42669) spec        (62)       29 2024-01-22 14:24:24.000000 extractstructuresMC-1.0.0.0/README.md
-drwxr-xr-x   0 aparas   (42669) spec        (62)        0 2024-01-22 16:11:19.138707 extractstructuresMC-1.0.0.0/extractStructuresWithMC/
--rwxrwxrwx   0 aparas   (42669) spec        (62)       57 2024-01-22 15:45:53.000000 extractstructuresMC-1.0.0.0/extractStructuresWithMC/__init__.py
--rwxrwxrwx   0 aparas   (42669) spec        (62)    34806 2024-01-22 16:00:09.000000 extractstructuresMC-1.0.0.0/extractStructuresWithMC/extractStructuresWithMC.py
--rwxrwxrwx   0 aparas   (42669) spec        (62)     3158 2024-01-22 14:07:25.000000 extractstructuresMC-1.0.0.0/extractStructuresWithMC/runTests.py
--rwxrwxrwx   0 aparas   (42669) spec        (62) 61401600 2023-11-29 10:39:01.000000 extractstructuresMC-1.0.0.0/extractStructuresWithMC/testData.bin
-drwxr-xr-x   0 aparas   (42669) spec        (62)        0 2024-01-22 16:11:19.258709 extractstructuresMC-1.0.0.0/extractstructuresMC.egg-info/
--rw-r--r--   0 aparas   (42669) spec        (62)      544 2024-01-22 16:11:18.000000 extractstructuresMC-1.0.0.0/extractstructuresMC.egg-info/PKG-INFO
--rw-r--r--   0 aparas   (42669) spec        (62)      350 2024-01-22 16:11:19.000000 extractstructuresMC-1.0.0.0/extractstructuresMC.egg-info/SOURCES.txt
--rw-r--r--   0 aparas   (42669) spec        (62)        1 2024-01-22 16:11:18.000000 extractstructuresMC-1.0.0.0/extractstructuresMC.egg-info/dependency_links.txt
--rw-r--r--   0 aparas   (42669) spec        (62)       24 2024-01-22 16:11:18.000000 extractstructuresMC-1.0.0.0/extractstructuresMC.egg-info/top_level.txt
--rw-r--r--   0 aparas   (42669) spec        (62)       38 2024-01-22 16:11:19.258709 extractstructuresMC-1.0.0.0/setup.cfg
--rwxrwxrwx   0 aparas   (42669) spec        (62)      890 2024-01-22 16:10:58.000000 extractstructuresMC-1.0.0.0/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-22 08:47:58.538562 extractstructuresMC-1.0.0.1/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      533 2024-04-22 08:47:58.538562 extractstructuresMC-1.0.0.1/PKG-INFO
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)       29 2024-01-22 14:24:24.000000 extractstructuresMC-1.0.0.1/README.md
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-22 08:47:58.478562 extractstructuresMC-1.0.0.1/extractStructuresWithMC/
+-rwxrwxrwx   0 abhishek  (1000) abhishek  (1000)       57 2024-01-22 15:45:53.000000 extractstructuresMC-1.0.0.1/extractStructuresWithMC/__init__.py
+-rwxrwxrwx   0 abhishek  (1000) abhishek  (1000)    33176 2024-04-22 08:47:12.000000 extractstructuresMC-1.0.0.1/extractStructuresWithMC/extractStructuresWithMC.py
+-rwxrwxrwx   0 abhishek  (1000) abhishek  (1000)     3158 2024-01-22 14:07:25.000000 extractstructuresMC-1.0.0.1/extractStructuresWithMC/runTests.py
+-rwxrwxrwx   0 abhishek  (1000) abhishek  (1000) 61401600 2023-11-29 10:39:01.000000 extractstructuresMC-1.0.0.1/extractStructuresWithMC/testData.bin
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-22 08:47:58.538562 extractstructuresMC-1.0.0.1/extractstructuresMC.egg-info/
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)      533 2024-04-22 08:47:58.000000 extractstructuresMC-1.0.0.1/extractstructuresMC.egg-info/PKG-INFO
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)      360 2024-04-22 08:47:58.000000 extractstructuresMC-1.0.0.1/extractstructuresMC.egg-info/SOURCES.txt
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)        1 2024-04-22 08:47:58.000000 extractstructuresMC-1.0.0.1/extractstructuresMC.egg-info/dependency_links.txt
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)       24 2024-04-22 08:47:58.000000 extractstructuresMC-1.0.0.1/extractstructuresMC.egg-info/top_level.txt
+-rw-r--r--   0 abhishek  (1000) abhishek  (1000)       38 2024-04-22 08:47:58.538562 extractstructuresMC-1.0.0.1/setup.cfg
+-rwxrwxrwx   0 abhishek  (1000) abhishek  (1000)      890 2024-04-22 08:47:23.000000 extractstructuresMC-1.0.0.1/setup.py
```

### Comparing `extractstructuresMC-1.0.0.0/PKG-INFO` & `extractstructuresMC-1.0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: extractstructuresMC
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: This code is an extension of the neighbor scanning     procedure of Moisy & Jiménez (2004), used for the extraction (segmentation)    of coherent structures from 3D scalar fields
 Home-page: https://github.com/Phoenixfire1081/CoherentStructureExtraction
 Author: Abhishek Harikrishnan
 Author-email: abhishek.harikrishnan@fu-berlin.de
 License: MIT
-Description: # CoherentStructureExtraction
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+# CoherentStructureExtraction
+
```

### Comparing `extractstructuresMC-1.0.0.0/extractStructuresWithMC/extractStructuresWithMC.py` & `extractstructuresMC-1.0.0.1/extractStructuresWithMC/extractStructuresWithMC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1192,68 +1192,14 @@
 		Vall = sum(countsall[::-1][1:])
 		if self.verbose:
 			print('Sum of counts of all structures: ', Vall)
 
 		if self._writePercolationData:
 			
 			fw = open('Percolation_threshold.txt', 'a')
-			fw.write(str(_threshVal) + ' ' + str(Vmax) + ' ' + str(Vall) + '\n')
+			fw.write(str(self._threshVal) + ' ' + str(Vmax) + ' ' + str(Vall) + '\n')
 			fw.close()
 
 		if self.verbose:
 			print('Total time:', time.time() - start_time)
 		
 		return _structValuedGrid
-
-# # Select file to run tests on
-# _filenameRead = 'testData.bin'
-
-# # What indexing does it use?
-# # This refers to array order
-# # See here for a full description: https://docs.oracle.com/cd/E19957-01/805-4940/z400091044d0/index.html
-# # Python uses C-order indexing (or row-major order). For this set _zFastest = True
-# _zFastest = True
-
-# # Threshold value for testing
-# _threshVal = 47
-
-# # Set additional parameters
-
-# # Writes information relating to percolation analysis.
-# _writePercolationData = False
-
-# # Writes structure location information.
-# # Useful for visualization purposes
-# _writeNeighborInformation = True
-
-# # Set data related parameters
-# xlen = 200 
-# ylen = 328
-# zlen = 234
-
-# # Set precision of binary data. 'f' is 32-bit floating point data.
-# # For others, see here: https://docs.python.org/3/library/array.html
-# precision = 'f'
-
-# # Use array to read data. This is fast for binary files.
-# data = array.array(precision)
-# fr = open(_filenameRead, 'rb')
-# data.fromfile(fr, (xlen*ylen*zlen))
-# fr.close()
-
-# # Convert to numpy array
-# data = np.array(data, dtype = np.float32)
-
-# # Print out details
-# _verbose = True
-
-# # Use Marching Cubes neighbor correction (more computation power required)
-# _marchingCubesExt = False
-# print('Running 3D test case with MC...')
-
-# extractStructuresObj = extractStructuresMC(_threshVal, data, \
-# xlen, ylen, zlen, _zFastest, _verbose, \
-# _writeNeighborInformation, _writePercolationData, _marchingCubesExt)
-# structureGrid = extractStructuresObj.extract()
-
-# print('Expected number of structures at threshold 47:', 31)
-# print('NOTE: structure 0 is empty space')
```

### Comparing `extractstructuresMC-1.0.0.0/extractStructuresWithMC/runTests.py` & `extractstructuresMC-1.0.0.1/extractStructuresWithMC/runTests.py`

 * *Files identical despite different names*

### Comparing `extractstructuresMC-1.0.0.0/extractStructuresWithMC/testData.bin` & `extractstructuresMC-1.0.0.1/extractStructuresWithMC/testData.bin`

 * *Files identical despite different names*

### Comparing `extractstructuresMC-1.0.0.0/extractstructuresMC.egg-info/PKG-INFO` & `extractstructuresMC-1.0.0.1/extractstructuresMC.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: extractstructuresMC
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: This code is an extension of the neighbor scanning     procedure of Moisy & Jiménez (2004), used for the extraction (segmentation)    of coherent structures from 3D scalar fields
 Home-page: https://github.com/Phoenixfire1081/CoherentStructureExtraction
 Author: Abhishek Harikrishnan
 Author-email: abhishek.harikrishnan@fu-berlin.de
 License: MIT
-Description: # CoherentStructureExtraction
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+# CoherentStructureExtraction
+
```

### Comparing `extractstructuresMC-1.0.0.0/setup.py` & `extractstructuresMC-1.0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
   
 with open("README.md", "r") as fh: 
     description = fh.read() 
   
 setuptools.setup( 
     name="extractstructuresMC", 
-    version="1.0.0.0", 
+    version="1.0.0.1", 
     author="Abhishek Harikrishnan", 
     author_email="abhishek.harikrishnan@fu-berlin.de", 
     packages=["extractStructuresWithMC"], 
     package_dir={'extractStructuresWithMC': 'extractStructuresWithMC'},
     package_data={'extractStructuresWithMC': ['*.bin', 'runTests.py']},
     description="This code is an extension of the neighbor scanning \
     procedure of Moisy & Jiménez (2004), used for the extraction (segmentation)\
```

