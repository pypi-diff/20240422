# Comparing `tmp/sinaraml_jupyter-2024.2.9.tar.gz` & `tmp/sinaraml_jupyter-2024.4.22.tar.gz`

## Comparing `sinaraml_jupyter-2024.2.9.tar` & `sinaraml_jupyter-2024.4.22.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.2.9/sinaraml_jupyter/__init__.py
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.2.9/sinaraml_jupyter/_version.py
--rwxr-xr-x   0        0        0     5537 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.2.9/sinaraml_jupyter/pipeline.py
--rwxr-xr-x   0        0        0      796 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.2.9/sinaraml_jupyter/plugin_loader.py
--rwxr-xr-x   0        0        0     2785 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.2.9/sinaraml_jupyter/sinaraml_jupyter.py
--rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.2.9/sinaraml_jupyter/sinaraml_types.py
--rwxr-xr-x   0        0        0     3101 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.2.9/.gitignore
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.2.9/LICENSE
--rwxr-xr-x   0        0        0     3162 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.2.9/README.md
--rwxr-xr-x   0        0        0     1590 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.2.9/pyproject.toml
--rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.2.9/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/sinaraml_jupyter/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/sinaraml_jupyter/_version.py
+-rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/sinaraml_jupyter/org_manager.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/sinaraml_jupyter/sinaraml_jupyter.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/LICENSE
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/README.md
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/pyproject.toml
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 sinaraml_jupyter-2024.4.22/PKG-INFO
```

### Comparing `sinaraml_jupyter-2024.2.9/.gitignore` & `sinaraml_jupyter-2024.4.22/.gitignore`

 * *Files identical despite different names*

### Comparing `sinaraml_jupyter-2024.2.9/pyproject.toml` & `sinaraml_jupyter-2024.4.22/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 description = "SinaraML Jupyter CLI"
 readme = "README.md"
 requires-python = ">=3.6"
 keywords = ["cli", "sinaraml", "jupyter"]
 license = { file="LICENSE" }
 classifiers = [
-        "License :: OSI Approved :: Apache Software License",
+        "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
```

