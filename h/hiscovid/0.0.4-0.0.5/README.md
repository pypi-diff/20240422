# Comparing `tmp/hiscovid-0.0.4.tar.gz` & `tmp/hiscovid-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiscovid-0.0.4.tar", last modified: Sat Apr 15 08:31:23 2023, max compression
+gzip compressed data, was "hiscovid-0.0.5.tar", last modified: Mon Apr 22 07:53:45 2024, max compression
```

## Comparing `hiscovid-0.0.4.tar` & `hiscovid-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-04-15 08:31:23.347775 hiscovid-0.0.4/
--rw-r--r--   0 yt        (1000) yt        (1000)     2040 2023-04-15 08:31:23.346536 hiscovid-0.0.4/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1488 2022-05-05 10:27:54.000000 hiscovid-0.0.4/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-04-15 08:31:23.347775 hiscovid-0.0.4/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      972 2023-04-15 08:30:16.000000 hiscovid-0.0.4/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-04-15 08:31:23.339421 hiscovid-0.0.4/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-04-15 08:31:23.346536 hiscovid-0.0.4/src/hiscovid.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     2040 2023-04-15 08:31:22.000000 hiscovid-0.0.4/src/hiscovid.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-04-15 08:31:22.000000 hiscovid-0.0.4/src/hiscovid.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-04-15 08:31:22.000000 hiscovid-0.0.4/src/hiscovid.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-04-15 08:31:22.000000 hiscovid-0.0.4/src/hiscovid.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-04-15 08:31:22.000000 hiscovid-0.0.4/src/hiscovid.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1941 2023-04-15 08:29:35.000000 hiscovid-0.0.4/src/hiscovid.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:53:45.849377 hiscovid-0.0.5/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4563 2024-04-22 07:53:45.849377 hiscovid-0.0.5/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4009 2024-04-22 07:52:49.000000 hiscovid-0.0.5/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 07:53:45.849377 hiscovid-0.0.5/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      974 2024-04-22 07:52:05.000000 hiscovid-0.0.5/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:53:45.849377 hiscovid-0.0.5/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:53:45.849377 hiscovid-0.0.5/src/hiscovid.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4563 2024-04-22 07:53:45.000000 hiscovid-0.0.5/src/hiscovid.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      217 2024-04-22 07:53:45.000000 hiscovid-0.0.5/src/hiscovid.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 07:53:45.000000 hiscovid-0.0.5/src/hiscovid.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       44 2024-04-22 07:53:45.000000 hiscovid-0.0.5/src/hiscovid.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        9 2024-04-22 07:53:45.000000 hiscovid-0.0.5/src/hiscovid.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1941 2023-04-15 08:29:35.000000 hiscovid-0.0.5/src/hiscovid.py
```

### Comparing `hiscovid-0.0.4/setup.py` & `hiscovid-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hiscovid",
-    version="0.0.4",
+    version="0.0.5",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for calculating time transition policy scores against COVID-19",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/hiscovid",
+    url="https://github.com/y-takefuji/hiscovid",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/hiscovid",
+        "Bug Tracker": "https://github.com/y-takefuji/hiscovid",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['hiscovid'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'hiscovid = hiscovid:main'
         ]
     },
 )
```

### Comparing `hiscovid-0.0.4/src/hiscovid.py` & `hiscovid-0.0.5/src/hiscovid.py`

 * *Files identical despite different names*

