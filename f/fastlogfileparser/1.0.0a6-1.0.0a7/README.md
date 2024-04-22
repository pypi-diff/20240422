# Comparing `tmp/fastlogfileparser-1.0.0a6.tar.gz` & `tmp/fastlogfileparser-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlogfileparser-1.0.0a6.tar", last modified: Tue Feb 27 00:32:21 2024, max compression
+gzip compressed data, was "fastlogfileparser-1.0.0a7.tar", last modified: Mon Apr 22 06:03:36 2024, max compression
```

## Comparing `fastlogfileparser-1.0.0a6.tar` & `fastlogfileparser-1.0.0a7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 00:32:21.114253 fastlogfileparser-1.0.0a6/
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-02-27 00:32:21.114253 fastlogfileparser-1.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 00:32:21.106253 fastlogfileparser-1.0.0a6/fastlogfileparser/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 00:32:21.110253 fastlogfileparser-1.0.0a6/fastlogfileparser/gaussian/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/gaussian/fast_gaussian_logfile_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 00:32:21.110253 fastlogfileparser-1.0.0a6/fastlogfileparser/gaussian/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/gaussian/utils/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/gaussian/utils/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/gaussian/utils/regexes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 00:32:21.110253 fastlogfileparser-1.0.0a6/fastlogfileparser/generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/generic/iter_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/generic/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 00:32:21.110253 fastlogfileparser-1.0.0a6/fastlogfileparser/orca/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/orca/fast_orca_logfile_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 00:32:21.110253 fastlogfileparser-1.0.0a6/fastlogfileparser/orca/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/orca/utils/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/fastlogfileparser/orca/utils/regexes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 00:32:21.110253 fastlogfileparser-1.0.0a6/fastlogfileparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-02-27 00:32:21.000000 fastlogfileparser-1.0.0a6/fastlogfileparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-27 00:32:21.000000 fastlogfileparser-1.0.0a6/fastlogfileparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 00:32:21.000000 fastlogfileparser-1.0.0a6/fastlogfileparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-27 00:32:21.000000 fastlogfileparser-1.0.0a6/fastlogfileparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-27 00:32:21.000000 fastlogfileparser-1.0.0a6/fastlogfileparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-27 00:32:13.000000 fastlogfileparser-1.0.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 00:32:21.114253 fastlogfileparser-1.0.0a6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:36.466105 fastlogfileparser-1.0.0a7/
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-22 06:03:36.466105 fastlogfileparser-1.0.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:36.462105 fastlogfileparser-1.0.0a7/fastlogfileparser/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:36.462105 fastlogfileparser-1.0.0a7/fastlogfileparser/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/gaussian/fast_gaussian_logfile_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:36.462105 fastlogfileparser-1.0.0a7/fastlogfileparser/gaussian/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/gaussian/utils/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/gaussian/utils/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/gaussian/utils/regexes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:36.462105 fastlogfileparser-1.0.0a7/fastlogfileparser/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/generic/iter_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/generic/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:36.462105 fastlogfileparser-1.0.0a7/fastlogfileparser/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/orca/fast_orca_logfile_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:36.462105 fastlogfileparser-1.0.0a7/fastlogfileparser/orca/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/orca/utils/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/fastlogfileparser/orca/utils/regexes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 06:03:36.466105 fastlogfileparser-1.0.0a7/fastlogfileparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-22 06:03:36.000000 fastlogfileparser-1.0.0a7/fastlogfileparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-22 06:03:36.000000 fastlogfileparser-1.0.0a7/fastlogfileparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 06:03:36.000000 fastlogfileparser-1.0.0a7/fastlogfileparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 06:03:36.000000 fastlogfileparser-1.0.0a7/fastlogfileparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 06:03:36.000000 fastlogfileparser-1.0.0a7/fastlogfileparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-22 06:03:32.000000 fastlogfileparser-1.0.0a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 06:03:36.466105 fastlogfileparser-1.0.0a7/setup.cfg
```

### Comparing `fastlogfileparser-1.0.0a6/fastlogfileparser/gaussian/fast_gaussian_logfile_parser.py` & `fastlogfileparser-1.0.0a7/fastlogfileparser/gaussian/fast_gaussian_logfile_parser.py`

 * *Files identical despite different names*

### Comparing `fastlogfileparser-1.0.0a6/fastlogfileparser/gaussian/utils/postprocessing.py` & `fastlogfileparser-1.0.0a7/fastlogfileparser/gaussian/utils/postprocessing.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,26 @@
     _columns_to_floats,
     _freq_modes,
     _str_list_to_floats,
     _str_to_float,
     _unix_time_to_seconds,
 )
 
+
+def _mulliken(in_list):
+    out = []
+    for i in in_list:
+        inner_out = []
+        for row in i.split(sep="\n"):
+            atom_idx, _, mulliken_charge, _ = row.split()
+            inner_out.append([int(atom_idx), float(mulliken_charge)])
+        out.append(inner_out)
+    return out
+
+
 POSTPROCESSING_FUNCTIONS = {
     "cpu_time": _unix_time_to_seconds,
     "wall_time": _unix_time_to_seconds,
     "e0": _str_to_float,
     "e0_h": _str_to_float,
     "hf": _str_to_float,
     "scf": _str_list_to_floats,
@@ -23,8 +35,9 @@
     "frequencies": lambda in_list: [float(i) for sublist in in_list for i in sublist],
     "max_steps": lambda in_list: int(in_list[0]),
     "std_forces": _columns_to_floats,
     "std_xyz": _columns_to_floats,
     "xyz": _columns_to_floats,
     "route_section": lambda in_list: in_list[0],
     "charge_and_multiplicity": _charge_and_multiplicity,
+    "mulliken_charges_summed": _mulliken,
 }
```

### Comparing `fastlogfileparser-1.0.0a6/fastlogfileparser/gaussian/utils/preprocessing.py` & `fastlogfileparser-1.0.0a7/fastlogfileparser/gaussian/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `fastlogfileparser-1.0.0a6/fastlogfileparser/gaussian/utils/regexes.py` & `fastlogfileparser-1.0.0a7/fastlogfileparser/gaussian/utils/regexes.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,20 @@
         r" ---------------------------------------------------------------------"
     ),
     "frequency_modes": (
         r"  Atom  AN      X      Y      Z        X      Y      Z        X      Y      Z\n"
         r"([\s+\d+\s+\d\s+-?\d\.\d\d\s+-?\d\.\d\d\s+-?\d\.\d\d\s+-?\d\.\d\d\s+-?\d\.\d\d\s+-?\d\.\d\d\s+-?\d\.\d\d\s+-?\d\.\d\d\s+-?\d\.\d\d]+)\n"
         r"(?:\s+\d+\s+\d+\s+\d+)?\n"
     ),
+    "mulliken_charges_summed": (
+        r" Mulliken charges and spin densities with hydrogens summed into heavy atoms:\n"
+        r"               1          2\n"
+        r"((?:\s+\d+\s+[a-zA-Z]{1,3}\s+-?\d+\.\d+\s+-?\d+\.\d+)+)\n"
+        r" APT charges:"
+    ),
     "charge_and_multiplicity": r" Charge = {1,2}(-?\d) Multiplicity = (\d)",
 }
 
 METADATA = {
     "route_section": r"#([A-Za-z\d\,=\(\)\-\/ \"\.\_]*)",
     "cpu_time": r" Job cpu time: \s+(\d+ days\s+\d+ hours\s+\d+ minutes\s+\d+\.?\d+ seconds)",
     "wall_time": r" Elapsed time: \s+(\d+ days\s+\d+ hours\s+\d+ minutes\s+\d+\.?\d+ seconds)",
@@ -53,11 +59,11 @@
     "normal_termination": r" Normal termination ",
     "error_string": r" Error termination(.*)\n",
 }
 
 RETRIEVAL_PATTERNS = {**DATA, **METADATA}
 
 # other options:
-# homo-lumo gap, polarizability, dipole moment, mulliken and APT partial charges, occupancy
+# homo-lumo gap, polarizability, dipole moment, APT partial charges, occupancy
 
 
 COMPILED_PATTERNS = {pattern_name: re.compile(pattern) for (pattern_name, pattern) in RETRIEVAL_PATTERNS.items()}
```

### Comparing `fastlogfileparser-1.0.0a6/fastlogfileparser/generic/iter_patterns.py` & `fastlogfileparser-1.0.0a7/fastlogfileparser/generic/iter_patterns.py`

 * *Files identical despite different names*

### Comparing `fastlogfileparser-1.0.0a6/fastlogfileparser/generic/postprocessing.py` & `fastlogfileparser-1.0.0a7/fastlogfileparser/generic/postprocessing.py`

 * *Files identical despite different names*

### Comparing `fastlogfileparser-1.0.0a6/fastlogfileparser/orca/fast_orca_logfile_parser.py` & `fastlogfileparser-1.0.0a7/fastlogfileparser/orca/fast_orca_logfile_parser.py`

 * *Files identical despite different names*

### Comparing `fastlogfileparser-1.0.0a6/fastlogfileparser/orca/utils/postprocessing.py` & `fastlogfileparser-1.0.0a7/fastlogfileparser/orca/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `fastlogfileparser-1.0.0a6/fastlogfileparser/orca/utils/regexes.py` & `fastlogfileparser-1.0.0a7/fastlogfileparser/orca/utils/regexes.py`

 * *Files identical despite different names*

### Comparing `fastlogfileparser-1.0.0a6/fastlogfileparser.egg-info/SOURCES.txt` & `fastlogfileparser-1.0.0a7/fastlogfileparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastlogfileparser-1.0.0a6/pyproject.toml` & `fastlogfileparser-1.0.0a7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastlogfileparser"
-version = "1.0.0a6"
+version = "1.0.0a7"
 authors = [
     { name = "Jackson Burns" },
 ]
 license = { text = "MIT" }
 description = "Parse computational chemistry log files, but fast-ly."
 classifiers = [
     "Programming Language :: Python :: 3",
```

