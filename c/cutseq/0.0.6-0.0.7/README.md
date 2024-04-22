# Comparing `tmp/cutseq-0.0.6.tar.gz` & `tmp/cutseq-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutseq-0.0.6.tar", max compression
+gzip compressed data, was "cutseq-0.0.7.tar", max compression
```

## Comparing `cutseq-0.0.6.tar` & `cutseq-0.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      362 2024-04-22 02:31:40.913895 cutseq-0.0.6/README.md
--rw-r--r--   0        0        0    21046 2024-04-22 02:31:40.913895 cutseq-0.0.6/cutseq/run.py
--rw-r--r--   0        0        0    14395 2024-04-22 02:31:40.913895 cutseq-0.0.6/cutseq/run_cmd.py
--rw-r--r--   0        0        0      510 2024-04-22 02:31:40.913895 cutseq-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 cutseq-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      362 2024-04-22 03:12:02.645395 cutseq-0.0.7/README.md
+-rw-r--r--   0        0        0    21867 2024-04-22 03:12:02.649395 cutseq-0.0.7/cutseq/run.py
+-rw-r--r--   0        0        0    14395 2024-04-22 03:12:02.649395 cutseq-0.0.7/cutseq/run_cmd.py
+-rw-r--r--   0        0        0      510 2024-04-22 03:12:02.649395 cutseq-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 cutseq-0.0.7/PKG-INFO
```

### Comparing `cutseq-0.0.6/cutseq/run.py` & `cutseq-0.0.7/cutseq/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 )
 from cutadapt.files import InputPaths, OutputFiles
 from cutadapt.modifiers import (
     AdapterCutter,
     PairedEndRenamer,
     QualityTrimmer,
     Renamer,
+    SingleEndModifier,
     SuffixRemover,
     UnconditionalCutter,
 )
 from cutadapt.pipeline import PairedEndPipeline, SingleEndPipeline
 from cutadapt.predicates import Predicate, TooShort
 from cutadapt.report import Statistics
 from cutadapt.runners import make_runner
@@ -51,14 +52,46 @@
         return original_method(self, *args, **kwargs)
     except AssertionError:
         pass
 
 
 Statistics._collect_modifier = patched_problematic_method
 
+## Enhnace function for cutadapt
+
+
+class IsUntrimmedAny(Predicate):
+    """
+    Select reads for which no adapter match was found
+    """
+
+    def __init__(self, ref_adapters):
+        self.ref_adapters = ref_adapters
+
+    def __repr__(self):
+        return "IsUntrimmedAny()"
+
+    def test(self, read, info):
+        # check not all adapters with ref_adapters are exist in the matches
+        match_adapters = [match.adapter for match in info.matches]
+        if any([adapter not in match_adapters for adapter in self.ref_adapters]):
+            return True
+        return False
+
+
+class ReverseComplementConverter(SingleEndModifier):
+    def __init__(self):
+        self.rcd = False
+
+    def __repr__(self):
+        return f"UnconditionalCutter(length={self.length})"
+
+    def __call__(self, read, info):
+        return read.reverse_complement()
+
 
 __version__ = importlib.metadata.version(__package__ or __name__)
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s -  %(levelname)s - %(message)s",
 )
@@ -139,33 +172,14 @@
         self.trim_polyA = False
         self.min_length = 20
         self.min_quality = 20
         self.dry_run = False
         self.threads = 1
 
 
-class IsUntrimmedAny(Predicate):
-    """
-    Select reads for which no adapter match was found
-    """
-
-    def __init__(self, ref_adapters):
-        self.ref_adapters = ref_adapters
-
-    def __repr__(self):
-        return "IsUntrimmedAny()"
-
-    def test(self, read, info):
-        # check not all adapters with ref_adapters are exist in the matches
-        match_adapters = [match.adapter for match in info.matches]
-        if any([adapter not in match_adapters for adapter in self.ref_adapters]):
-            return True
-        return False
-
-
 def run_steps(steps, dry_run=False):
     if dry_run:
         print(
             " |\\\n".join([("    " + s if i > 0 else s) for i, s in enumerate(steps)])
         )
         process = subprocess.run("true", shell=True, capture_output=True)
     else:
@@ -236,14 +250,18 @@
         else:
             logging.info("No strand information provided, skip polyA trimming.")
     # step 8: quality control, remove short reads
     modifiers.append(
         QualityTrimmer(cutoff_front=0, cutoff_back=settings.min_quality),
     )
 
+    # step 9: reverse complement the read
+    if settings.reverse_complement:
+        modifiers.append(ReverseComplementConverter())
+
     inpaths = InputPaths(input1)
 
     with make_runner(inpaths, cores=settings.threads) as runner:
         outfiles = OutputFiles(
             proxied=settings.threads > 1,
             qualities=runner.input_file_format().has_qualities(),
             interleaved=False,
@@ -420,14 +438,18 @@
     modifiers.append(
         (
             QualityTrimmer(cutoff_front=0, cutoff_back=settings.min_quality),
             QualityTrimmer(cutoff_front=0, cutoff_back=settings.min_quality),
         )
     )
 
+    # step 9: reverse complement the read
+    if settings.reverse_complement:
+        modifiers.append((ReverseComplementConverter(), ReverseComplementConverter()))
+
     inpaths = InputPaths(input1, input2)
 
     with make_runner(inpaths, cores=settings.threads) as runner:
         outfiles = OutputFiles(
             proxied=settings.threads > 1,
             qualities=runner.input_file_format().has_qualities(),
             interleaved=False,
@@ -477,14 +499,15 @@
     settings = CutadaptConfig()
     settings.rname_suffix = args.with_rname_suffix
     settings.ensure_inline_barcode = args.ensure_inline_barcode
     settings.trim_polyA = args.trim_polyA
     settings.threads = args.threads
     settings.min_length = args.min_length
     settings.dry_run = args.dry_run
+    settings.reverse_complement = args.reverse_complement
     if len(args.input_file) == 1:
         pipeline_single(
             args.input_file[0],
             args.output_file[0],
             args.short_file[0],
             args.untrimmed_file[0],
             barcode_config,
@@ -580,14 +603,20 @@
         nargs="+",
         help="Output file path for discarded reads without inline barcode.",
     )
 
     parser.add_argument("--trim-polyA", action="store_true", help="Trim polyA tail.")
 
     parser.add_argument(
+        "--reverse-complement",
+        action="store_true",
+        help="Reverse complement the reads.",
+    )
+
+    parser.add_argument(
         "-t",
         "--threads",
         type=int,
         default=1,
         help="Number of threads to use for trimming.",
     )
     parser.add_argument(
```

### Comparing `cutseq-0.0.6/cutseq/run_cmd.py` & `cutseq-0.0.7/cutseq/run_cmd.py`

 * *Files identical despite different names*

### Comparing `cutseq-0.0.6/PKG-INFO` & `cutseq-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutseq
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automatically cut adapter / barcode / UMI from NGS data
 Home-page: https://github.com/y9c/cutseq
 License: MIT
 Keywords: bioinformatics,NGS,adapter,barcode,UMI
 Author: Ye Chang
 Author-email: yech1990@gmail.com
 Requires-Python: >=3.8,<4.0
```

