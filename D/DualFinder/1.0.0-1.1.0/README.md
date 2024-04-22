# Comparing `tmp/DualFinder-1.0.0.tar.gz` & `tmp/DualFinder-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DualFinder-1.0.0.tar", last modified: Fri Apr 19 15:05:33 2024, max compression
+gzip compressed data, was "DualFinder-1.1.0.tar", last modified: Mon Apr 22 02:00:23 2024, max compression
```

## Comparing `DualFinder-1.0.0.tar` & `DualFinder-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-19 15:05:33.533224 DualFinder-1.0.0/
-drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-19 15:05:33.530525 DualFinder-1.0.0/DualFinder.egg-info/
--rw-r--r--   0 moskowitzi   (501) staff       (20)      251 2024-04-19 15:05:33.000000 DualFinder-1.0.0/DualFinder.egg-info/PKG-INFO
--rw-r--r--   0 moskowitzi   (501) staff       (20)      647 2024-04-19 15:05:33.000000 DualFinder-1.0.0/DualFinder.egg-info/SOURCES.txt
--rw-r--r--   0 moskowitzi   (501) staff       (20)        1 2024-04-19 15:05:33.000000 DualFinder-1.0.0/DualFinder.egg-info/dependency_links.txt
--rw-r--r--   0 moskowitzi   (501) staff       (20)       78 2024-04-19 15:05:33.000000 DualFinder-1.0.0/DualFinder.egg-info/requires.txt
--rw-r--r--   0 moskowitzi   (501) staff       (20)       99 2024-04-19 15:05:33.000000 DualFinder-1.0.0/DualFinder.egg-info/top_level.txt
--rw-r--r--   0 moskowitzi   (501) staff       (20)      251 2024-04-19 15:05:33.533086 DualFinder-1.0.0/PKG-INFO
-drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-19 15:05:33.530670 DualFinder-1.0.0/dual_finder/
--rw-r--r--   0 moskowitzi   (501) staff       (20)       95 2024-04-19 00:27:48.000000 DualFinder-1.0.0/dual_finder/__init__.py
-drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-19 15:05:33.531404 DualFinder-1.0.0/dual_finder/cnn/
--rw-r--r--   0 moskowitzi   (501) staff       (20)      228 2024-04-19 00:33:20.000000 DualFinder-1.0.0/dual_finder/cnn/__init__.py
--rw-r--r--   0 moskowitzi   (501) staff       (20)     8002 2024-04-19 01:59:26.000000 DualFinder-1.0.0/dual_finder/cnn/create_cnn.py
--rw-r--r--   0 moskowitzi   (501) staff       (20)     6263 2024-04-19 02:03:16.000000 DualFinder-1.0.0/dual_finder/cnn/extract_feature_maps.py
--rw-r--r--   0 moskowitzi   (501) staff       (20)     6436 2024-04-19 14:24:39.000000 DualFinder-1.0.0/dual_finder/cnn/load_model.py
--rw-r--r--   0 moskowitzi   (501) staff       (20)    18207 2024-04-19 04:37:18.000000 DualFinder-1.0.0/dual_finder/cnn/train_cnn.py
-drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-19 15:05:33.531916 DualFinder-1.0.0/dual_finder/optimize/
--rw-r--r--   0 moskowitzi   (501) staff       (20)      181 2024-04-19 00:45:49.000000 DualFinder-1.0.0/dual_finder/optimize/__init__.py
--rw-r--r--   0 moskowitzi   (501) staff       (20)     5215 2024-04-18 21:16:21.000000 DualFinder-1.0.0/dual_finder/optimize/optimize_hyperparameters.py
-drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-19 15:05:33.532516 DualFinder-1.0.0/dual_finder/preprocess_data/
--rw-r--r--   0 moskowitzi   (501) staff       (20)      134 2024-04-18 21:40:09.000000 DualFinder-1.0.0/dual_finder/preprocess_data/__init__.py
--rw-r--r--   0 moskowitzi   (501) staff       (20)     3207 2024-04-18 21:16:21.000000 DualFinder-1.0.0/dual_finder/preprocess_data/fits_utils.py
--rw-r--r--   0 moskowitzi   (501) staff       (20)    10180 2024-04-19 04:23:09.000000 DualFinder-1.0.0/dual_finder/preprocess_data/process_data.py
-drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-19 15:05:33.532876 DualFinder-1.0.0/dual_finder/visualize/
--rw-r--r--   0 moskowitzi   (501) staff       (20)      272 2024-04-19 00:47:02.000000 DualFinder-1.0.0/dual_finder/visualize/__init__.py
--rw-r--r--   0 moskowitzi   (501) staff       (20)    11894 2024-04-19 14:47:26.000000 DualFinder-1.0.0/dual_finder/visualize/visualize_performance.py
--rw-r--r--   0 moskowitzi   (501) staff       (20)       38 2024-04-19 15:05:33.533282 DualFinder-1.0.0/setup.cfg
--rw-r--r--   0 moskowitzi   (501) staff       (20)      577 2024-04-19 15:01:47.000000 DualFinder-1.0.0/setup.py
+drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-22 02:00:23.428243 DualFinder-1.1.0/
+drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-22 02:00:23.422464 DualFinder-1.1.0/DualFinder.egg-info/
+-rw-r--r--   0 moskowitzi   (501) staff       (20)      449 2024-04-22 02:00:23.000000 DualFinder-1.1.0/DualFinder.egg-info/PKG-INFO
+-rw-r--r--   0 moskowitzi   (501) staff       (20)      647 2024-04-22 02:00:23.000000 DualFinder-1.1.0/DualFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 moskowitzi   (501) staff       (20)        1 2024-04-22 02:00:23.000000 DualFinder-1.1.0/DualFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 moskowitzi   (501) staff       (20)       78 2024-04-22 02:00:23.000000 DualFinder-1.1.0/DualFinder.egg-info/requires.txt
+-rw-r--r--   0 moskowitzi   (501) staff       (20)       99 2024-04-22 02:00:23.000000 DualFinder-1.1.0/DualFinder.egg-info/top_level.txt
+-rw-r--r--   0 moskowitzi   (501) staff       (20)      449 2024-04-22 02:00:23.428005 DualFinder-1.1.0/PKG-INFO
+drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-22 02:00:23.422589 DualFinder-1.1.0/dual_finder/
+-rw-r--r--   0 moskowitzi   (501) staff       (20)       95 2024-04-19 00:27:48.000000 DualFinder-1.1.0/dual_finder/__init__.py
+drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-22 02:00:23.424857 DualFinder-1.1.0/dual_finder/cnn/
+-rw-r--r--   0 moskowitzi   (501) staff       (20)      228 2024-04-19 00:33:20.000000 DualFinder-1.1.0/dual_finder/cnn/__init__.py
+-rw-r--r--   0 moskowitzi   (501) staff       (20)     8002 2024-04-19 01:59:26.000000 DualFinder-1.1.0/dual_finder/cnn/create_cnn.py
+-rw-r--r--   0 moskowitzi   (501) staff       (20)     6263 2024-04-19 02:03:16.000000 DualFinder-1.1.0/dual_finder/cnn/extract_feature_maps.py
+-rw-r--r--   0 moskowitzi   (501) staff       (20)     6436 2024-04-19 14:24:39.000000 DualFinder-1.1.0/dual_finder/cnn/load_model.py
+-rw-r--r--   0 moskowitzi   (501) staff       (20)    18207 2024-04-19 04:37:18.000000 DualFinder-1.1.0/dual_finder/cnn/train_cnn.py
+drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-22 02:00:23.425530 DualFinder-1.1.0/dual_finder/optimize/
+-rw-r--r--   0 moskowitzi   (501) staff       (20)      181 2024-04-19 00:45:49.000000 DualFinder-1.1.0/dual_finder/optimize/__init__.py
+-rw-r--r--   0 moskowitzi   (501) staff       (20)     5215 2024-04-18 21:16:21.000000 DualFinder-1.1.0/dual_finder/optimize/optimize_hyperparameters.py
+drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-22 02:00:23.426647 DualFinder-1.1.0/dual_finder/preprocess_data/
+-rw-r--r--   0 moskowitzi   (501) staff       (20)      134 2024-04-18 21:40:09.000000 DualFinder-1.1.0/dual_finder/preprocess_data/__init__.py
+-rw-r--r--   0 moskowitzi   (501) staff       (20)     3207 2024-04-18 21:16:21.000000 DualFinder-1.1.0/dual_finder/preprocess_data/fits_utils.py
+-rw-r--r--   0 moskowitzi   (501) staff       (20)    10180 2024-04-19 04:23:09.000000 DualFinder-1.1.0/dual_finder/preprocess_data/process_data.py
+drwxr-xr-x   0 moskowitzi   (501) staff       (20)        0 2024-04-22 02:00:23.427492 DualFinder-1.1.0/dual_finder/visualize/
+-rw-r--r--   0 moskowitzi   (501) staff       (20)      272 2024-04-19 00:47:02.000000 DualFinder-1.1.0/dual_finder/visualize/__init__.py
+-rw-r--r--   0 moskowitzi   (501) staff       (20)    11894 2024-04-19 14:47:26.000000 DualFinder-1.1.0/dual_finder/visualize/visualize_performance.py
+-rw-r--r--   0 moskowitzi   (501) staff       (20)       38 2024-04-22 02:00:23.428293 DualFinder-1.1.0/setup.cfg
+-rw-r--r--   0 moskowitzi   (501) staff       (20)      577 2024-04-22 01:59:07.000000 DualFinder-1.1.0/setup.py
```

### Comparing `DualFinder-1.0.0/DualFinder.egg-info/SOURCES.txt` & `DualFinder-1.1.0/DualFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DualFinder-1.0.0/dual_finder/cnn/create_cnn.py` & `DualFinder-1.1.0/dual_finder/cnn/create_cnn.py`

 * *Files identical despite different names*

### Comparing `DualFinder-1.0.0/dual_finder/cnn/extract_feature_maps.py` & `DualFinder-1.1.0/dual_finder/cnn/extract_feature_maps.py`

 * *Files identical despite different names*

### Comparing `DualFinder-1.0.0/dual_finder/cnn/load_model.py` & `DualFinder-1.1.0/dual_finder/cnn/load_model.py`

 * *Files identical despite different names*

### Comparing `DualFinder-1.0.0/dual_finder/cnn/train_cnn.py` & `DualFinder-1.1.0/dual_finder/cnn/train_cnn.py`

 * *Files identical despite different names*

### Comparing `DualFinder-1.0.0/dual_finder/optimize/optimize_hyperparameters.py` & `DualFinder-1.1.0/dual_finder/optimize/optimize_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `DualFinder-1.0.0/dual_finder/preprocess_data/fits_utils.py` & `DualFinder-1.1.0/dual_finder/preprocess_data/fits_utils.py`

 * *Files identical despite different names*

### Comparing `DualFinder-1.0.0/dual_finder/preprocess_data/process_data.py` & `DualFinder-1.1.0/dual_finder/preprocess_data/process_data.py`

 * *Files identical despite different names*

### Comparing `DualFinder-1.0.0/dual_finder/visualize/visualize_performance.py` & `DualFinder-1.1.0/dual_finder/visualize/visualize_performance.py`

 * *Files identical despite different names*

### Comparing `DualFinder-1.0.0/setup.py` & `DualFinder-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name="DualFinder",
-     version="1.0.0",
+     version="1.1.0",
      author="Isaac Moskowitz",
      author_email="isaac.moskowitz@yale.edu",
      description="A trainable and visualizable convolutional neural network designed to detect galaxy and AGN mergers. ",
      packages=["dual_finder", "dual_finder/preprocess_data", "dual_finder/cnn", "dual_finder/visualize", "dual_finder/optimize"],
      python_requires='>=3.8',
      install_requires=["numpy", "tensorflow >= 2.14", "scipy", "astropy", "scikit-learn", "optuna", "matplotlib", "streamlit"]
```

