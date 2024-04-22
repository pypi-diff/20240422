# Comparing `tmp/spatialdata_xenium_explorer-0.1.6.tar.gz` & `tmp/spatialdata_xenium_explorer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialdata_xenium_explorer-0.1.6.tar", max compression
+gzip compressed data, was "spatialdata_xenium_explorer-0.1.7.tar", max compression
```

## Comparing `spatialdata_xenium_explorer-0.1.6.tar` & `spatialdata_xenium_explorer-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1526 2024-02-14 13:00:12.143788 spatialdata_xenium_explorer-0.1.6/LICENSE
--rw-r--r--   0        0        0     3803 2024-02-14 13:00:12.143788 spatialdata_xenium_explorer-0.1.6/README.md
--rw-r--r--   0        0        0     1779 2024-02-14 13:00:12.299789 spatialdata_xenium_explorer-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      530 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/__init__.py
--rw-r--r--   0        0        0     3946 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/_constants.py
--rw-r--r--   0        0        0     1039 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/_logging.py
--rw-r--r--   0        0        0     4941 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/cli/app.py
--rw-r--r--   0        0        0     8255 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/converter.py
--rw-r--r--   0        0        0        0 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/core/__init__.py
--rw-r--r--   0        0        0    10934 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/core/images.py
--rw-r--r--   0        0        0     7209 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/core/points.py
--rw-r--r--   0        0        0     3764 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/core/shapes.py
--rw-r--r--   0        0        0     5114 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/core/table.py
--rw-r--r--   0        0        0       25 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/main.py
--rw-r--r--   0        0        0     8627 2024-02-14 13:00:12.303789 spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/utils.py
--rw-r--r--   0        0        0     4896 1970-01-01 00:00:00.000000 spatialdata_xenium_explorer-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1526 2024-04-22 08:30:44.066860 spatialdata_xenium_explorer-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3803 2024-04-22 08:30:44.066860 spatialdata_xenium_explorer-0.1.7/README.md
+-rw-r--r--   0        0        0     1787 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      530 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/__init__.py
+-rw-r--r--   0        0        0     3946 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/_constants.py
+-rw-r--r--   0        0        0     1039 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/_logging.py
+-rw-r--r--   0        0        0     4941 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/cli/app.py
+-rw-r--r--   0        0        0     8255 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/converter.py
+-rw-r--r--   0        0        0        0 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/core/__init__.py
+-rw-r--r--   0        0        0    10911 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/core/images.py
+-rw-r--r--   0        0        0     7209 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/core/points.py
+-rw-r--r--   0        0        0     3764 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/core/shapes.py
+-rw-r--r--   0        0        0     5114 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/core/table.py
+-rw-r--r--   0        0        0       25 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/main.py
+-rw-r--r--   0        0        0     8627 2024-04-22 08:30:44.226862 spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/utils.py
+-rw-r--r--   0        0        0     4872 1970-01-01 00:00:00.000000 spatialdata_xenium_explorer-0.1.7/PKG-INFO
```

### Comparing `spatialdata_xenium_explorer-0.1.6/LICENSE` & `spatialdata_xenium_explorer-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata_xenium_explorer-0.1.6/README.md` & `spatialdata_xenium_explorer-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `spatialdata_xenium_explorer-0.1.6/pyproject.toml` & `spatialdata_xenium_explorer-0.1.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spatialdata_xenium_explorer"
-version = "0.1.6"
+version = "0.1.7"
 description = "Converting any SpatialData object into files that can be open by the Xenium Explorer"
 documentation = "https://quentinblampey.github.io/spatialdata_xenium_explorer/"
 homepage = "https://quentinblampey.github.io/spatialdata_xenium_explorer/"
 repository = "https://github.com/quentinblampey/spatialdata_xenium_explorer"
 authors = ["Quentin Blampey <quentin.blampey@gmail.com>"]
 packages = [{ include = "spatialdata_xenium_explorer" }]
 license = "BSD-3-Clause"
@@ -19,27 +19,27 @@
 ]
 
 [tool.poetry.scripts]
 spatialdata_xenium_explorer = "spatialdata_xenium_explorer.main:app"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
-botocore = "^1.31.47"
-spatialdata = "^0.0.15"
-typer = "^0.9.0"
+botocore = "1.34.19"
+spatialdata = ">=0.1.2"
+typer = ">=0.9.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.8.0"
-isort = "^5.10.1"
-pytest = "^7.1.3"
-ipykernel = "^6.25.2"
-mkdocs-material = "^9.3.2"
-mkdocstrings = "^0.23.0"
-mkdocstrings-python = "^1.7.3"
-jupyter-black = "^0.3.4"
+black = ">=22.8.0"
+isort = ">=5.10.1"
+pytest = ">=7.1.3"
+ipykernel = ">=6.25.2"
+mkdocs-material = ">=9.3.2"
+mkdocstrings = ">=0.23.0"
+mkdocstrings-python = ">=1.7.3"
+jupyter-black = ">=0.3.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

### Comparing `spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/__init__.py` & `spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/_constants.py` & `spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/_constants.py`

 * *Files identical despite different names*

### Comparing `spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/_logging.py` & `spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/_logging.py`

 * *Files identical despite different names*

### Comparing `spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/cli/app.py` & `spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/cli/app.py`

 * *Files identical despite different names*

### Comparing `spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/converter.py` & `spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/converter.py`

 * *Files identical despite different names*

### Comparing `spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/core/images.py` & `spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/core/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
         dims=("c", "y", "x"),
         transformations={pixel_cs: to_pixel},
         c_coords=image.coords["c"].values,
         **image_models_kwargs,
     )
 
     log.info(f"Adding image {image.name}:\n{image}")
-    sdata.add_image(image_name, image, overwrite=overwrite)
+    sdata.images[image_name] = image
 
 
 def _ome_channels_names(path: str):
     import xml.etree.ElementTree as ET
 
     tiff = tf.TiffFile(path)
     omexml_string = tiff.pages[0].description
```

### Comparing `spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/core/points.py` & `spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/core/points.py`

 * *Files identical despite different names*

### Comparing `spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/core/shapes.py` & `spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/core/shapes.py`

 * *Files identical despite different names*

### Comparing `spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/core/table.py` & `spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/core/table.py`

 * *Files identical despite different names*

### Comparing `spatialdata_xenium_explorer-0.1.6/spatialdata_xenium_explorer/utils.py` & `spatialdata_xenium_explorer-0.1.7/spatialdata_xenium_explorer/utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata_xenium_explorer-0.1.6/PKG-INFO` & `spatialdata_xenium_explorer-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: spatialdata_xenium_explorer
-Version: 0.1.6
+Version: 0.1.7
 Summary: Converting any SpatialData object into files that can be open by the Xenium Explorer
 Home-page: https://quentinblampey.github.io/spatialdata_xenium_explorer/
 License: BSD-3-Clause
 Author: Quentin Blampey
 Author-email: quentin.blampey@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: botocore (>=1.31.47,<2.0.0)
-Requires-Dist: spatialdata (>=0.0.15,<0.0.16)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: botocore (==1.34.19)
+Requires-Dist: spatialdata (>=0.1.2)
+Requires-Dist: typer (>=0.9.0)
 Project-URL: Documentation, https://quentinblampey.github.io/spatialdata_xenium_explorer/
 Project-URL: Repository, https://github.com/quentinblampey/spatialdata_xenium_explorer
 Description-Content-Type: text/markdown
 
 # SpatialData to Xenium Explorer
 
 [![PyPI](https://img.shields.io/pypi/v/spatialdata_xenium_explorer.svg)](https://pypi.org/project/spatialdata_xenium_explorer)
```

