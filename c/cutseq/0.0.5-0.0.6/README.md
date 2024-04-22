# Comparing `tmp/cutseq-0.0.5.tar.gz` & `tmp/cutseq-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutseq-0.0.5.tar", max compression
+gzip compressed data, was "cutseq-0.0.6.tar", max compression
```

## Comparing `cutseq-0.0.5.tar` & `cutseq-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      362 2024-04-22 00:19:47.644237 cutseq-0.0.5/README.md
--rw-r--r--   0        0        0    20509 2024-04-22 00:19:47.644237 cutseq-0.0.5/cutseq/run.py
--rw-r--r--   0        0        0    14395 2024-04-22 00:19:47.644237 cutseq-0.0.5/cutseq/run_cmd.py
--rw-r--r--   0        0        0      510 2024-04-22 00:19:47.644237 cutseq-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 cutseq-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      362 2024-04-22 02:31:40.913895 cutseq-0.0.6/README.md
+-rw-r--r--   0        0        0    21046 2024-04-22 02:31:40.913895 cutseq-0.0.6/cutseq/run.py
+-rw-r--r--   0        0        0    14395 2024-04-22 02:31:40.913895 cutseq-0.0.6/cutseq/run_cmd.py
+-rw-r--r--   0        0        0      510 2024-04-22 02:31:40.913895 cutseq-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 cutseq-0.0.6/PKG-INFO
```

### Comparing `cutseq-0.0.5/cutseq/run.py` & `cutseq-0.0.6/cutseq/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # Copyright © 2024 Ye Chang yech1990@gmail.com
 # Distributed under terms of the GNU license.
 #
 # Created: 2024-04-19 18:57
 
 import argparse
+import importlib.metadata
 import logging
 import re
 import subprocess
 import sys
 
 from cutadapt.adapters import (
     BackAdapter,
@@ -27,23 +28,40 @@
     QualityTrimmer,
     Renamer,
     SuffixRemover,
     UnconditionalCutter,
 )
 from cutadapt.pipeline import PairedEndPipeline, SingleEndPipeline
 from cutadapt.predicates import Predicate, TooShort
+from cutadapt.report import Statistics
 from cutadapt.runners import make_runner
 from cutadapt.steps import (
     PairedEndFilter,
     PairedEndSink,
     SingleEndFilter,
     SingleEndSink,
 )
 from cutadapt.utils import Progress
 
+#  monkey patching ....
+original_method = Statistics._collect_modifier
+
+
+def patched_problematic_method(self, *args, **kwargs):
+    try:
+        return original_method(self, *args, **kwargs)
+    except AssertionError:
+        pass
+
+
+Statistics._collect_modifier = patched_problematic_method
+
+
+__version__ = importlib.metadata.version(__package__ or __name__)
+
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s -  %(levelname)s - %(message)s",
 )
 
 
 def reverse_complement(b):
@@ -121,24 +139,24 @@
         self.trim_polyA = False
         self.min_length = 20
         self.min_quality = 20
         self.dry_run = False
         self.threads = 1
 
 
-class IsUntrimmedRef(Predicate):
+class IsUntrimmedAny(Predicate):
     """
     Select reads for which no adapter match was found
     """
 
     def __init__(self, ref_adapters):
         self.ref_adapters = ref_adapters
 
     def __repr__(self):
-        return "IsUntrimmedRef()"
+        return "IsUntrimmedAny()"
 
     def test(self, read, info):
         # check not all adapters with ref_adapters are exist in the matches
         match_adapters = [match.adapter for match in info.matches]
         if any([adapter not in match_adapters for adapter in self.ref_adapters]):
             return True
         return False
@@ -247,15 +265,15 @@
             if barcode.inline5.len > 0:
                 ref_adapters.append(adapter_inline5)
             if barcode.inline3.len > 0:
                 ref_adapters.append(adapter_inline3)
             steps.append(
                 # TODO: --max-n=0 support
                 SingleEndFilter(
-                    IsUntrimmedRef(ref_adapters),
+                    IsUntrimmedAny(ref_adapters),
                     outfiles.open_record_writer(untrimmed1, interleaved=False),
                 ),
             )
         steps.append(
             # -o
             SingleEndSink(outfiles.open_record_writer(output1, interleaved=False)),
         )
@@ -428,18 +446,18 @@
         if (
             settings.ensure_inline_barcode
             and barcode.inline5.len + barcode.inline3.len > 0
         ):
             steps.append(
                 # TODO: --max-n=0 support
                 PairedEndFilter(
-                    IsUntrimmedRef([adapter_inline5])
+                    IsUntrimmedAny([adapter_inline5])
                     if barcode.inline5.len > 0
                     else None,
-                    IsUntrimmedRef([adapter_inline3])
+                    IsUntrimmedAny([adapter_inline3])
                     if barcode.inline3.len > 0
                     else None,
                     outfiles.open_record_writer(
                         untrimmed1, untrimmed2, interleaved=False
                     ),
                     pair_filter_mode="any",
                 )
@@ -574,14 +592,19 @@
     )
     parser.add_argument(
         "-n",
         "--dry-run",
         action="store_true",
         help="Print command instead of running it.",
     )
+
+    parser.add_argument(
+        "-V", "--version", action="version", version=f"%(prog)s {__version__}"
+    )
+
     args = parser.parse_args()
 
     if args.adapter_name is not None:
         if args.adapter_scheme is not None:
             logging.info("Adapter scheme is provided, ignore adapter name.")
         else:
             if args.adapter_name.upper() == "TAKARAV2":
```

### Comparing `cutseq-0.0.5/cutseq/run_cmd.py` & `cutseq-0.0.6/cutseq/run_cmd.py`

 * *Files identical despite different names*

### Comparing `cutseq-0.0.5/PKG-INFO` & `cutseq-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutseq
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automatically cut adapter / barcode / UMI from NGS data
 Home-page: https://github.com/y9c/cutseq
 License: MIT
 Keywords: bioinformatics,NGS,adapter,barcode,UMI
 Author: Ye Chang
 Author-email: yech1990@gmail.com
 Requires-Python: >=3.8,<4.0
```

