# Comparing `tmp/pytdml-1.1.6.tar.gz` & `tmp/pytdml-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytdml-1.1.6.tar", last modified: Fri Mar 22 07:27:09 2024, max compression
+gzip compressed data, was "pytdml-1.1.7.tar", last modified: Mon Apr 22 07:21:52 2024, max compression
```

## Comparing `pytdml-1.1.6.tar` & `pytdml-1.1.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 07:27:09.701844 pytdml-1.1.6/
--rw-rw-rw-   0        0        0     1141 2023-04-17 03:31:48.000000 pytdml-1.1.6/LICENSE
--rw-rw-rw-   0        0        0    12498 2024-03-22 07:27:09.700847 pytdml-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    11873 2024-03-22 06:32:00.000000 pytdml-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 07:27:09.667935 pytdml-1.1.6/datalibrary/
--rw-rw-rw-   0        0        0     1561 2023-07-21 01:52:46.000000 pytdml-1.1.6/datalibrary/__init__.py
--rw-rw-rw-   0        0        0    10717 2023-07-14 03:06:06.000000 pytdml-1.1.6/datalibrary/datasetcollection.py
--rw-rw-rw-   0        0        0    14588 2023-07-14 12:37:10.000000 pytdml-1.1.6/datalibrary/downloader.py
--rw-rw-rw-   0        0        0    15868 2023-07-21 03:26:26.000000 pytdml-1.1.6/datalibrary/pipeline.py
--rw-rw-rw-   0        0        0     2770 2023-07-20 09:28:32.000000 pytdml-1.1.6/datalibrary/s3Client.py
--rw-rw-rw-   0        0        0    10873 2023-06-30 03:50:52.000000 pytdml-1.1.6/datalibrary/util.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:27:09.668932 pytdml-1.1.6/examples/
--rw-rw-rw-   0        0        0        0 2023-04-17 03:31:48.000000 pytdml-1.1.6/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:27:09.673918 pytdml-1.1.6/pytdml/
--rw-rw-rw-   0        0        0     1610 2024-03-22 07:26:18.000000 pytdml-1.1.6/pytdml/__init__.py
--rw-rw-rw-   0        0        0     9683 2024-03-22 07:23:34.000000 pytdml-1.1.6/pytdml/convert_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:27:09.683892 pytdml-1.1.6/pytdml/io/
--rw-rw-rw-   0        0        0     2596 2024-03-22 06:14:04.000000 pytdml-1.1.6/pytdml/io/S3_reader.py
--rw-rw-rw-   0        0        0     1722 2024-03-22 06:14:04.000000 pytdml-1.1.6/pytdml/io/__init__.py
--rw-rw-rw-   0        0        0     1182 2024-02-29 02:37:47.000000 pytdml-1.1.6/pytdml/io/internal.py
--rw-rw-rw-   0        0        0     3041 2024-03-22 06:14:04.000000 pytdml-1.1.6/pytdml/io/tdml_readers.py
--rw-rw-rw-   0        0        0     2403 2024-03-22 06:14:04.000000 pytdml-1.1.6/pytdml/io/tdml_writers.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:27:09.689876 pytdml-1.1.6/pytdml/ml/
--rw-rw-rw-   0        0        0     1821 2023-02-15 03:16:12.000000 pytdml-1.1.6/pytdml/ml/__init__.py
--rw-rw-rw-   0        0        0     3128 2023-04-26 11:31:46.000000 pytdml-1.1.6/pytdml/ml/ml_operators.py
--rw-rw-rw-   0        0        0     8989 2023-04-27 02:43:43.000000 pytdml-1.1.6/pytdml/ml/object_transforms.py
--rw-rw-rw-   0        0        0    15938 2023-06-30 07:12:28.000000 pytdml-1.1.6/pytdml/ml/tdml_tensorflow.py
--rw-rw-rw-   0        0        0    14790 2023-07-14 06:46:23.000000 pytdml-1.1.6/pytdml/ml/tdml_torch.py
--rw-rw-rw-   0        0        0    17566 2023-06-30 12:37:34.000000 pytdml-1.1.6/pytdml/ml/tdml_torch_data_pipe.py
--rw-rw-rw-   0        0        0    12325 2023-07-19 06:49:42.000000 pytdml-1.1.6/pytdml/tdml_image_crop.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:27:09.696857 pytdml-1.1.6/pytdml/type/
--rw-rw-rw-   0        0        0     2599 2023-10-30 00:44:20.000000 pytdml-1.1.6/pytdml/type/__init__.py
--rw-rw-rw-   0        0        0     3374 2024-03-22 06:14:04.000000 pytdml-1.1.6/pytdml/type/_utils.py
--rw-rw-rw-   0        0        0     9638 2024-03-22 07:02:54.000000 pytdml-1.1.6/pytdml/type/basic_types.py
--rw-rw-rw-   0        0        0    22692 2024-03-22 06:14:04.000000 pytdml-1.1.6/pytdml/type/basic_types_old.py
--rw-rw-rw-   0        0        0     4421 2024-03-22 07:15:26.000000 pytdml-1.1.6/pytdml/type/extended_types.py
--rw-rw-rw-   0        0        0    16667 2024-03-22 06:14:04.000000 pytdml-1.1.6/pytdml/type/extended_types_old.py
--rw-rw-rw-   0        0        0     1695 2023-10-30 00:44:20.000000 pytdml-1.1.6/pytdml/type/test.py
--rw-rw-rw-   0        0        0    16988 2023-07-21 03:39:08.000000 pytdml-1.1.6/pytdml/utils.py
--rw-rw-rw-   0        0        0    16225 2024-03-22 06:14:04.000000 pytdml-1.1.6/pytdml/yaml_to_tdml.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:27:09.678905 pytdml-1.1.6/pytdml.egg-info/
--rw-rw-rw-   0        0        0    12498 2024-03-22 07:27:09.000000 pytdml-1.1.6/pytdml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-03-22 07:27:09.000000 pytdml-1.1.6/pytdml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 07:27:09.000000 pytdml-1.1.6/pytdml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-03-22 07:27:09.000000 pytdml-1.1.6/pytdml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2024-03-22 07:27:09.000000 pytdml-1.1.6/pytdml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 07:27:09.701844 pytdml-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     3136 2023-06-19 07:33:23.000000 pytdml-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:27:09.699849 pytdml-1.1.6/tests/
--rw-rw-rw-   0        0        0      290 2024-02-29 03:01:13.000000 pytdml-1.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0     3633 2024-03-22 06:14:04.000000 pytdml-1.1.6/tests/test_basic_types.py
--rw-rw-rw-   0        0        0      493 2024-03-22 06:14:04.000000 pytdml-1.1.6/tests/test_tdml_io.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:21:52.269590 pytdml-1.1.7/
+-rw-rw-rw-   0        0        0     1141 2023-04-17 03:31:48.000000 pytdml-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0    12492 2024-04-22 07:21:52.268593 pytdml-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11867 2024-03-22 11:14:19.000000 pytdml-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 07:21:51.984808 pytdml-1.1.7/datalibrary/
+-rw-rw-rw-   0        0        0     1561 2023-07-21 01:52:46.000000 pytdml-1.1.7/datalibrary/__init__.py
+-rw-rw-rw-   0        0        0    10717 2023-07-14 03:06:06.000000 pytdml-1.1.7/datalibrary/datasetcollection.py
+-rw-rw-rw-   0        0        0    14588 2023-07-14 12:37:10.000000 pytdml-1.1.7/datalibrary/downloader.py
+-rw-rw-rw-   0        0        0    15868 2023-07-21 03:26:26.000000 pytdml-1.1.7/datalibrary/pipeline.py
+-rw-rw-rw-   0        0        0     3144 2024-04-22 07:08:31.000000 pytdml-1.1.7/datalibrary/s3Client.py
+-rw-rw-rw-   0        0        0    10873 2023-06-30 03:50:52.000000 pytdml-1.1.7/datalibrary/util.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:21:52.001762 pytdml-1.1.7/examples/
+-rw-rw-rw-   0        0        0        0 2023-04-17 03:31:48.000000 pytdml-1.1.7/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:21:52.048637 pytdml-1.1.7/pytdml/
+-rw-rw-rw-   0        0        0     1610 2024-04-22 07:21:34.000000 pytdml-1.1.7/pytdml/__init__.py
+-rw-rw-rw-   0        0        0     9683 2024-03-22 07:23:34.000000 pytdml-1.1.7/pytdml/convert_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:21:52.107025 pytdml-1.1.7/pytdml/io/
+-rw-rw-rw-   0        0        0     2596 2024-03-22 06:14:04.000000 pytdml-1.1.7/pytdml/io/S3_reader.py
+-rw-rw-rw-   0        0        0     1722 2024-03-22 06:14:04.000000 pytdml-1.1.7/pytdml/io/__init__.py
+-rw-rw-rw-   0        0        0     1182 2024-02-29 02:37:47.000000 pytdml-1.1.7/pytdml/io/internal.py
+-rw-rw-rw-   0        0        0     3041 2024-03-22 06:14:04.000000 pytdml-1.1.7/pytdml/io/tdml_readers.py
+-rw-rw-rw-   0        0        0     2403 2024-03-22 06:14:04.000000 pytdml-1.1.7/pytdml/io/tdml_writers.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:21:52.167863 pytdml-1.1.7/pytdml/ml/
+-rw-rw-rw-   0        0        0     1821 2023-02-15 03:16:12.000000 pytdml-1.1.7/pytdml/ml/__init__.py
+-rw-rw-rw-   0        0        0     3128 2023-04-26 11:31:46.000000 pytdml-1.1.7/pytdml/ml/ml_operators.py
+-rw-rw-rw-   0        0        0     8989 2023-04-27 02:43:43.000000 pytdml-1.1.7/pytdml/ml/object_transforms.py
+-rw-rw-rw-   0        0        0    15938 2023-06-30 07:12:28.000000 pytdml-1.1.7/pytdml/ml/tdml_tensorflow.py
+-rw-rw-rw-   0        0        0    14790 2023-07-14 06:46:23.000000 pytdml-1.1.7/pytdml/ml/tdml_torch.py
+-rw-rw-rw-   0        0        0    17566 2023-06-30 12:37:34.000000 pytdml-1.1.7/pytdml/ml/tdml_torch_data_pipe.py
+-rw-rw-rw-   0        0        0    12325 2023-07-19 06:49:42.000000 pytdml-1.1.7/pytdml/tdml_image_crop.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:21:52.247649 pytdml-1.1.7/pytdml/type/
+-rw-rw-rw-   0        0        0     2599 2023-10-30 00:44:20.000000 pytdml-1.1.7/pytdml/type/__init__.py
+-rw-rw-rw-   0        0        0     3374 2024-03-22 06:14:04.000000 pytdml-1.1.7/pytdml/type/_utils.py
+-rw-rw-rw-   0        0        0     9638 2024-03-22 07:02:54.000000 pytdml-1.1.7/pytdml/type/basic_types.py
+-rw-rw-rw-   0        0        0    22692 2024-03-22 06:14:04.000000 pytdml-1.1.7/pytdml/type/basic_types_old.py
+-rw-rw-rw-   0        0        0     4421 2024-03-22 07:15:26.000000 pytdml-1.1.7/pytdml/type/extended_types.py
+-rw-rw-rw-   0        0        0    16667 2024-03-22 06:14:04.000000 pytdml-1.1.7/pytdml/type/extended_types_old.py
+-rw-rw-rw-   0        0        0     1695 2023-10-30 00:44:20.000000 pytdml-1.1.7/pytdml/type/test.py
+-rw-rw-rw-   0        0        0    17028 2024-04-22 07:15:49.000000 pytdml-1.1.7/pytdml/utils.py
+-rw-rw-rw-   0        0        0    16225 2024-03-22 06:14:04.000000 pytdml-1.1.7/pytdml/yaml_to_tdml.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:21:52.069126 pytdml-1.1.7/pytdml.egg-info/
+-rw-rw-rw-   0        0        0    12492 2024-04-22 07:21:51.000000 pytdml-1.1.7/pytdml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-22 07:21:51.000000 pytdml-1.1.7/pytdml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 07:21:51.000000 pytdml-1.1.7/pytdml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-22 07:21:51.000000 pytdml-1.1.7/pytdml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2024-04-22 07:21:51.000000 pytdml-1.1.7/pytdml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 07:21:52.269590 pytdml-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     3136 2023-06-19 07:33:23.000000 pytdml-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 07:21:52.267596 pytdml-1.1.7/tests/
+-rw-rw-rw-   0        0        0      290 2024-02-29 03:01:13.000000 pytdml-1.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     3633 2024-03-22 06:14:04.000000 pytdml-1.1.7/tests/test_basic_types.py
+-rw-rw-rw-   0        0        0      493 2024-03-22 06:14:04.000000 pytdml-1.1.7/tests/test_tdml_io.py
```

### Comparing `pytdml-1.1.6/LICENSE` & `pytdml-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/PKG-INFO` & `pytdml-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytdml
-Version: 1.1.6
+Version: 1.1.7
 Summary: Parsing and encoding training datasets based on OGC Training Data Markup Language for AI (TrainingDML-AI) standard
 Home-page: https://github.com/TrainingDML/pytdml
 Author: Boyi Shangguan
 Author-email: sgby@whu.edu.cn
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -13,30 +13,30 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytdml
 
-[pytdml](https://github.com/TrainingDML/pytdml) is a pure python parser and encoder for training datasets based on OGC
+[pytdml](https://github.com/openrsgis/pytdml) is a pure python parser and encoder for training datasets based on OGC
 Training Data Markup Language for AI standard.
 
 ---
 
 ## Installation
 
 The package can be installed via pip.
 
 ### Requirements
 
 * Python 3 and above
 
 ### Dependencies
 
-Dependencies are listed in [requirements.txt](https://github.com/TrainingDML/pytdml/blob/main/requirements.txt). Dependencies are automatically installed during
+Dependencies are listed in [requirements.txt](https://github.com/openrsgis/pytdml/blob/main/requirements.txt). Dependencies are automatically installed during
 pytdml's installation.
 
 ### Installing the Package
 
 ```bash
 pip install pytdml
 ```
@@ -51,15 +51,15 @@
 
 The training dataset can be encoded to TrainingDML-AI JSON format by YAML configuration file with command line.
 
 ```bash
 pytdml/yaml_to_tdml.py --config=<YAML configuration file path> --output=<Output TrainingDML-AI JSON file path>
 ```
 
-YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/TrainingDML/pytdml/blob/main/encoding_config_schema.yml).
+YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/openrsgis/pytdml/blob/main/encoding_config_schema.yml).
 
 #### Using the API from python
 
 The training dataset can also be encoded to TrainingDML-AI JSON format with Python API.
 
 ```python
 from pytdml.io import write_to_json
```

### Comparing `pytdml-1.1.6/README.md` & `pytdml-1.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # pytdml
 
-[pytdml](https://github.com/TrainingDML/pytdml) is a pure python parser and encoder for training datasets based on OGC
+[pytdml](https://github.com/openrsgis/pytdml) is a pure python parser and encoder for training datasets based on OGC
 Training Data Markup Language for AI standard.
 
 ---
 
 ## Installation
 
 The package can be installed via pip.
 
 ### Requirements
 
 * Python 3 and above
 
 ### Dependencies
 
-Dependencies are listed in [requirements.txt](https://github.com/TrainingDML/pytdml/blob/main/requirements.txt). Dependencies are automatically installed during
+Dependencies are listed in [requirements.txt](https://github.com/openrsgis/pytdml/blob/main/requirements.txt). Dependencies are automatically installed during
 pytdml's installation.
 
 ### Installing the Package
 
 ```bash
 pip install pytdml
 ```
@@ -34,15 +34,15 @@
 
 The training dataset can be encoded to TrainingDML-AI JSON format by YAML configuration file with command line.
 
 ```bash
 pytdml/yaml_to_tdml.py --config=<YAML configuration file path> --output=<Output TrainingDML-AI JSON file path>
 ```
 
-YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/TrainingDML/pytdml/blob/main/encoding_config_schema.yml).
+YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/openrsgis/pytdml/blob/main/encoding_config_schema.yml).
 
 #### Using the API from python
 
 The training dataset can also be encoded to TrainingDML-AI JSON format with Python API.
 
 ```python
 from pytdml.io import write_to_json
```

### Comparing `pytdml-1.1.6/datalibrary/__init__.py` & `pytdml-1.1.7/datalibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/datalibrary/datasetcollection.py` & `pytdml-1.1.7/datalibrary/datasetcollection.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/datalibrary/downloader.py` & `pytdml-1.1.7/datalibrary/downloader.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/datalibrary/pipeline.py` & `pytdml-1.1.7/datalibrary/pipeline.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/datalibrary/s3Client.py` & `pytdml-1.1.7/datalibrary/s3Client.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,28 @@
 
 _SERVER = '125.220.153.22:9006'
 _ACCESS_KEY = 'pytdmlopenuseraccount'
 _SECRET_KEY = 'HTJIEGCLPKUZBQYAVWMFXNRDOVS'
 
 
 class MinioClient:
-    def __init__(self, server, access_key, secret_key):
+    _instance = None
+
+    def __new__(cls, server, access_key, secret_key):
+        if cls._instance is None:
+            cls._instance = super().__new__(cls)
+            cls._instance.server = server
+            cls._instance.access_key = access_key
+            cls._instance.secret_key = secret_key
+            cls._instance._create_client()
+        return cls._instance
+
+    def _create_client(self):
         try:
-            self.client = Minio(server, access_key=access_key, secret_key=secret_key, secure=False)
+            self.client = Minio(self.server, access_key=self.access_key, secret_key=self.secret_key, secure=False)
         except S3Error as e:
             print("error:", e)
 
     def get_client(self):
         return self.client
```

### Comparing `pytdml-1.1.6/datalibrary/util.py` & `pytdml-1.1.7/datalibrary/util.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/__init__.py` & `pytdml-1.1.7/pytdml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,9 +28,9 @@
 # SOFTWARE.
 #
 # ------------------------------------------------------------------------------
 import pytdml.type
 import pytdml.io
 
 name = 'pytdml'
-__version__ = '1.1.6'
+__version__ = '1.1.7'
```

### Comparing `pytdml-1.1.6/pytdml/convert_utils.py` & `pytdml-1.1.7/pytdml/convert_utils.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/io/S3_reader.py` & `pytdml-1.1.7/pytdml/io/S3_reader.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/io/__init__.py` & `pytdml-1.1.7/pytdml/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/io/internal.py` & `pytdml-1.1.7/pytdml/io/internal.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/io/tdml_readers.py` & `pytdml-1.1.7/pytdml/io/tdml_readers.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/io/tdml_writers.py` & `pytdml-1.1.7/pytdml/io/tdml_writers.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/ml/__init__.py` & `pytdml-1.1.7/pytdml/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/ml/ml_operators.py` & `pytdml-1.1.7/pytdml/ml/ml_operators.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/ml/object_transforms.py` & `pytdml-1.1.7/pytdml/ml/object_transforms.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/ml/tdml_tensorflow.py` & `pytdml-1.1.7/pytdml/ml/tdml_tensorflow.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/ml/tdml_torch.py` & `pytdml-1.1.7/pytdml/ml/tdml_torch.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/ml/tdml_torch_data_pipe.py` & `pytdml-1.1.7/pytdml/ml/tdml_torch_data_pipe.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/tdml_image_crop.py` & `pytdml-1.1.7/pytdml/tdml_image_crop.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/type/__init__.py` & `pytdml-1.1.7/pytdml/type/__init__.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/type/_utils.py` & `pytdml-1.1.7/pytdml/type/_utils.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/type/basic_types.py` & `pytdml-1.1.7/pytdml/type/basic_types.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/type/basic_types_old.py` & `pytdml-1.1.7/pytdml/type/basic_types_old.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/type/extended_types.py` & `pytdml-1.1.7/pytdml/type/extended_types.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/type/extended_types_old.py` & `pytdml-1.1.7/pytdml/type/extended_types_old.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/type/test.py` & `pytdml-1.1.7/pytdml/type/test.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml/utils.py` & `pytdml-1.1.7/pytdml/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,16 @@
 
 def get_mapping_(file):
     mapping_data = client.get_object("pytdml", "mapping/" + file + "_mapping.json")
     map = json.load(BytesIO(mapping_data.read()))
     return map
 
 
-pixel_map = get_mapping_("pixel")
-name_map = get_mapping_("name")
+# pixel_map = get_mapping_("pixel")
+# name_map = get_mapping_("name")
 
 
 def label_class_list_(pixel_list):
     """
         transform label pixel list to label class list
     """
     if len(pixel_list) > 0:
@@ -250,14 +250,15 @@
     return rgb_img
 
 
 def dataset_name_map_(obs_name):
     """
     convert obs path name to dataset name
     """
+    name_map = get_mapping_("name")
     return [d for d in name_map if d["obs_path"] == obs_name][0]["name"]
 
 
 def get_object_label_data_(label, img_width, img_height):
     target_ = get_bounding_box(label.object)
     target_[0] = target_[0] / img_width
     target_[1] = target_[1] / img_height
```

### Comparing `pytdml-1.1.6/pytdml/yaml_to_tdml.py` & `pytdml-1.1.7/pytdml/yaml_to_tdml.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/pytdml.egg-info/PKG-INFO` & `pytdml-1.1.7/pytdml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytdml
-Version: 1.1.6
+Version: 1.1.7
 Summary: Parsing and encoding training datasets based on OGC Training Data Markup Language for AI (TrainingDML-AI) standard
 Home-page: https://github.com/TrainingDML/pytdml
 Author: Boyi Shangguan
 Author-email: sgby@whu.edu.cn
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -13,30 +13,30 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytdml
 
-[pytdml](https://github.com/TrainingDML/pytdml) is a pure python parser and encoder for training datasets based on OGC
+[pytdml](https://github.com/openrsgis/pytdml) is a pure python parser and encoder for training datasets based on OGC
 Training Data Markup Language for AI standard.
 
 ---
 
 ## Installation
 
 The package can be installed via pip.
 
 ### Requirements
 
 * Python 3 and above
 
 ### Dependencies
 
-Dependencies are listed in [requirements.txt](https://github.com/TrainingDML/pytdml/blob/main/requirements.txt). Dependencies are automatically installed during
+Dependencies are listed in [requirements.txt](https://github.com/openrsgis/pytdml/blob/main/requirements.txt). Dependencies are automatically installed during
 pytdml's installation.
 
 ### Installing the Package
 
 ```bash
 pip install pytdml
 ```
@@ -51,15 +51,15 @@
 
 The training dataset can be encoded to TrainingDML-AI JSON format by YAML configuration file with command line.
 
 ```bash
 pytdml/yaml_to_tdml.py --config=<YAML configuration file path> --output=<Output TrainingDML-AI JSON file path>
 ```
 
-YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/TrainingDML/pytdml/blob/main/encoding_config_schema.yml).
+YAML configuration file schema is described in [encoding YAML configuration file schema](https://github.com/openrsgis/pytdml/blob/main/encoding_config_schema.yml).
 
 #### Using the API from python
 
 The training dataset can also be encoded to TrainingDML-AI JSON format with Python API.
 
 ```python
 from pytdml.io import write_to_json
```

### Comparing `pytdml-1.1.6/pytdml.egg-info/SOURCES.txt` & `pytdml-1.1.7/pytdml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/setup.py` & `pytdml-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.6/tests/test_basic_types.py` & `pytdml-1.1.7/tests/test_basic_types.py`

 * *Files identical despite different names*

