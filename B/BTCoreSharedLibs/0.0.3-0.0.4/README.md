# Comparing `tmp/btcoresharedlibs-0.0.3.tar.gz` & `tmp/btcoresharedlibs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btcoresharedlibs-0.0.3.tar", last modified: Sat Apr 20 17:08:04 2024, max compression
+gzip compressed data, was "btcoresharedlibs-0.0.4.tar", last modified: Mon Apr 22 09:10:14 2024, max compression
```

## Comparing `btcoresharedlibs-0.0.3.tar` & `btcoresharedlibs-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.313963 btcoresharedlibs-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.309963 btcoresharedlibs-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.309963 btcoresharedlibs-0.0.3/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.309963 btcoresharedlibs-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-20 17:08:04.313963 btcoresharedlibs-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-20 17:08:04.313963 btcoresharedlibs-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.309963 btcoresharedlibs-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.313963 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-20 17:08:04.000000 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-20 17:08:04.000000 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:08:04.000000 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-20 17:08:04.000000 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 17:08:04.000000 btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:08:04.313963 btcoresharedlibs-0.0.3/src/CoreSharedLibs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/src/CoreSharedLibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/src/CoreSharedLibs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-20 17:07:57.000000 btcoresharedlibs-0.0.3/src/CoreSharedLibs/csl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:10:14.656607 btcoresharedlibs-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:10:14.652607 btcoresharedlibs-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:10:14.656607 btcoresharedlibs-0.0.4/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-22 09:10:05.000000 btcoresharedlibs-0.0.4/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:10:14.656607 btcoresharedlibs-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-22 09:10:05.000000 btcoresharedlibs-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-22 09:10:05.000000 btcoresharedlibs-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 09:10:05.000000 btcoresharedlibs-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 09:10:05.000000 btcoresharedlibs-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-22 09:10:14.656607 btcoresharedlibs-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-22 09:10:05.000000 btcoresharedlibs-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-22 09:10:05.000000 btcoresharedlibs-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 09:10:05.000000 btcoresharedlibs-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-22 09:10:14.656607 btcoresharedlibs-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:10:14.652607 btcoresharedlibs-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:10:14.656607 btcoresharedlibs-0.0.4/src/BTCoreSharedLibs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-22 09:10:14.000000 btcoresharedlibs-0.0.4/src/BTCoreSharedLibs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-22 09:10:14.000000 btcoresharedlibs-0.0.4/src/BTCoreSharedLibs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:10:14.000000 btcoresharedlibs-0.0.4/src/BTCoreSharedLibs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 09:10:14.000000 btcoresharedlibs-0.0.4/src/BTCoreSharedLibs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 09:10:14.000000 btcoresharedlibs-0.0.4/src/BTCoreSharedLibs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:10:14.656607 btcoresharedlibs-0.0.4/src/CoreSharedLibs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:10:05.000000 btcoresharedlibs-0.0.4/src/CoreSharedLibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-22 09:10:05.000000 btcoresharedlibs-0.0.4/src/CoreSharedLibs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-22 09:10:05.000000 btcoresharedlibs-0.0.4/src/CoreSharedLibs/csl.py
```

### Comparing `btcoresharedlibs-0.0.3/.github/scripts/release.py` & `btcoresharedlibs-0.0.4/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `btcoresharedlibs-0.0.3/.github/workflows/publish.yml` & `btcoresharedlibs-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `btcoresharedlibs-0.0.3/LICENSE` & `btcoresharedlibs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `btcoresharedlibs-0.0.3/PKG-INFO` & `btcoresharedlibs-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTCoreSharedLibs
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package of functions that I keep writing over and over again, so I can stop doing that. Script based on seanh example.
 Home-page: https://github.com/Jtecx/Python-BTCoreSharedLibs
 Project-URL: Bug Tracker, https://github.com/Jtecx/Python-BTCoreSharedLibs/issues
 Project-URL: Changelog, https://github.com/Jtecx/Python-BTCoreSharedLibs/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
```

### Comparing `btcoresharedlibs-0.0.3/setup.cfg` & `btcoresharedlibs-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `btcoresharedlibs-0.0.3/src/BTCoreSharedLibs.egg-info/PKG-INFO` & `btcoresharedlibs-0.0.4/src/BTCoreSharedLibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTCoreSharedLibs
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package of functions that I keep writing over and over again, so I can stop doing that. Script based on seanh example.
 Home-page: https://github.com/Jtecx/Python-BTCoreSharedLibs
 Project-URL: Bug Tracker, https://github.com/Jtecx/Python-BTCoreSharedLibs/issues
 Project-URL: Changelog, https://github.com/Jtecx/Python-BTCoreSharedLibs/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
```

### Comparing `btcoresharedlibs-0.0.3/src/CoreSharedLibs/csl.py` & `btcoresharedlibs-0.0.4/src/CoreSharedLibs/csl.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     :param target: String to match against.
     :return: String of int value.
     """
     source2 = []
     if isinstance(source, list):
         source2 = [entry.name for entry in source]
     elif isinstance(source, Path):
-        source2 = [entry.name for entry in source.iterdir()]
+        source2 = [entry.name for entry in source.glob("*")]
 
     try:
         result = [j for j in source2 if str(char_entry_value_strip(str(target))) in j][
             0
         ]
     except IndexError:
         logging.info("%s | %s", source, target)
@@ -89,37 +89,32 @@
         if len(file_list) > 0:
             print("All complete! Moving on.")
         return results
     except Exception as f:
         logging.error(f"An error occurred: {f}")
 
 
-def get_filename_from_path(file_path):
-    # Define the regex pattern to match a filename
-    pattern = r"[\\/]([^\\/]+)$"
-
-    # Use re.search to find the last segment which is the filename
-    match = re.search(pattern, file_path)
-
-    if match:
-        # Return the matched filename
-        return match.group(1)
-    else:
-        # If no match found, return None
-        return None
-
-
-def pos_int_input():
+def validate_int_input(min_val=0, max_val=-1):
+    """
+    Generic input validation. Holds user captive until either valid (positive) integer input is taken,
+    or termination requested.
+    Also double checks if the value entered is what the user intended.
+    :param min_val: Minimum valid value. Default 0.
+    :param max_val: Maximum valid value. Default to -1 as infinite substitute.
+    :return: Int.
+    """
     verify = True
     char_val = 0
     while verify:
         try:
             char_val = int(input("Please input an integer. : "))
-            if char_val < 0:
-                raise ValueError("Negative integers are not allowed.")
+            if char_val < min_val:
+                raise ValueError("Integer exceeds minimum allowed.")
+            elif max_val != -1 and char_val > max_val:
+                raise ValueError("Integer exceeds maximum allowed.")
             else:
                 char_verify = input(f"{char_val} entered! Correct? Y/N: ").lower()[
                               :1
                               ]
                 while True:
                     if char_verify in ["y", "n"]:
                         if char_verify == "y":
```

