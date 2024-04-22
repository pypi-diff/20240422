# Comparing `tmp/cutseq-0.0.7.tar.gz` & `tmp/cutseq-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutseq-0.0.7.tar", max compression
+gzip compressed data, was "cutseq-0.0.8.tar", max compression
```

## Comparing `cutseq-0.0.7.tar` & `cutseq-0.0.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      362 2024-04-22 03:12:02.645395 cutseq-0.0.7/README.md
--rw-r--r--   0        0        0    21867 2024-04-22 03:12:02.649395 cutseq-0.0.7/cutseq/run.py
--rw-r--r--   0        0        0    14395 2024-04-22 03:12:02.649395 cutseq-0.0.7/cutseq/run_cmd.py
--rw-r--r--   0        0        0      510 2024-04-22 03:12:02.649395 cutseq-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 cutseq-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      362 2024-04-22 03:42:10.759173 cutseq-0.0.8/README.md
+-rw-r--r--   0        0        0    22238 2024-04-22 03:42:10.759173 cutseq-0.0.8/cutseq/run.py
+-rw-r--r--   0        0        0    14395 2024-04-22 03:42:10.759173 cutseq-0.0.8/cutseq/run_cmd.py
+-rw-r--r--   0        0        0      510 2024-04-22 03:42:10.759173 cutseq-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 cutseq-0.0.8/PKG-INFO
```

### Comparing `cutseq-0.0.7/cutseq/run.py` & `cutseq-0.0.8/cutseq/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 
 class ReverseComplementConverter(SingleEndModifier):
     def __init__(self):
         self.rcd = False
 
     def __repr__(self):
-        return f"UnconditionalCutter(length={self.length})"
+        return "ReverseComplementConverter()"
 
     def __call__(self, read, info):
         return read.reverse_complement()
 
 
 __version__ = importlib.metadata.version(__package__ or __name__)
 
@@ -252,44 +252,47 @@
     # step 8: quality control, remove short reads
     modifiers.append(
         QualityTrimmer(cutoff_front=0, cutoff_back=settings.min_quality),
     )
 
     # step 9: reverse complement the read
     if settings.reverse_complement:
+        if barcode.strand == "+":
+            logging.warn("Library is + strand, but reverse complement is enabled.")
         modifiers.append(ReverseComplementConverter())
 
     inpaths = InputPaths(input1)
 
     with make_runner(inpaths, cores=settings.threads) as runner:
         outfiles = OutputFiles(
             proxied=settings.threads > 1,
             qualities=runner.input_file_format().has_qualities(),
             interleaved=False,
         )
         steps = []
+        # TODO: report info
+        # --info-file=info.txt
+        # PairedSingleEndStep(InfoFileWriter(outfiles.open_text("info.txt"))),
         steps.append(
-            # --info-file=info.txt
-            # PairedSingleEndStep(InfoFileWriter(outfiles.open_text("info.txt"))),
             # -m 10
             SingleEndFilter(
                 TooShort(settings.min_length), outfiles.open_record_writer(short1)
             ),
         )
+        # TODO: --max-n=0 support
         if (
             settings.ensure_inline_barcode
             and barcode.inline5.len + barcode.inline3.len > 0
         ):
             ref_adapters = []
             if barcode.inline5.len > 0:
                 ref_adapters.append(adapter_inline5)
             if barcode.inline3.len > 0:
                 ref_adapters.append(adapter_inline3)
             steps.append(
-                # TODO: --max-n=0 support
                 SingleEndFilter(
                     IsUntrimmedAny(ref_adapters),
                     outfiles.open_record_writer(untrimmed1, interleaved=False),
                 ),
             )
         steps.append(
             # -o
@@ -440,14 +443,16 @@
             QualityTrimmer(cutoff_front=0, cutoff_back=settings.min_quality),
             QualityTrimmer(cutoff_front=0, cutoff_back=settings.min_quality),
         )
     )
 
     # step 9: reverse complement the read
     if settings.reverse_complement:
+        if barcode.strand == "+":
+            logging.warn("Library is + strand, but reverse complement is enabled.")
         modifiers.append((ReverseComplementConverter(), ReverseComplementConverter()))
 
     inpaths = InputPaths(input1, input2)
 
     with make_runner(inpaths, cores=settings.threads) as runner:
         outfiles = OutputFiles(
             proxied=settings.threads > 1,
@@ -461,20 +466,20 @@
         steps.append(
             PairedEndFilter(
                 TooShort(settings.min_length),
                 TooShort(settings.min_length),
                 outfiles.open_record_writer(short1, short2, interleaved=False),
             )
         )
+        # TODO: --max-n=0 support
         if (
             settings.ensure_inline_barcode
             and barcode.inline5.len + barcode.inline3.len > 0
         ):
             steps.append(
-                # TODO: --max-n=0 support
                 PairedEndFilter(
                     IsUntrimmedAny([adapter_inline5])
                     if barcode.inline5.len > 0
                     else None,
                     IsUntrimmedAny([adapter_inline3])
                     if barcode.inline3.len > 0
                     else None,
@@ -491,15 +496,15 @@
         pipeline = PairedEndPipeline(modifiers, steps)
         _stats = runner.run(pipeline, Progress(), outfiles)
         # _ = stats.as_json()
     outfiles.close()
 
 
 def run_cutseq(args):
-    barcode_config = BarcodeConfig(args.adapter_scheme.upper())
+    barcode_config = BarcodeConfig(args.replace(" ", "").adapter_scheme.upper())
     settings = CutadaptConfig()
     settings.rname_suffix = args.with_rname_suffix
     settings.ensure_inline_barcode = args.ensure_inline_barcode
     settings.trim_polyA = args.trim_polyA
     settings.threads = args.threads
     settings.min_length = args.min_length
     settings.dry_run = args.dry_run
@@ -626,14 +631,19 @@
         help="Print command instead of running it.",
     )
 
     parser.add_argument(
         "-V", "--version", action="version", version=f"%(prog)s {__version__}"
     )
 
+    # Check if no arguments were provided
+    if len(sys.argv) == 1:
+        parser.print_help(sys.stdout)
+        sys.exit(0)
+
     args = parser.parse_args()
 
     if args.adapter_name is not None:
         if args.adapter_scheme is not None:
             logging.info("Adapter scheme is provided, ignore adapter name.")
         else:
             if args.adapter_name.upper() == "TAKARAV2":
```

### Comparing `cutseq-0.0.7/cutseq/run_cmd.py` & `cutseq-0.0.8/cutseq/run_cmd.py`

 * *Files identical despite different names*

### Comparing `cutseq-0.0.7/PKG-INFO` & `cutseq-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutseq
-Version: 0.0.7
+Version: 0.0.8
 Summary: Automatically cut adapter / barcode / UMI from NGS data
 Home-page: https://github.com/y9c/cutseq
 License: MIT
 Keywords: bioinformatics,NGS,adapter,barcode,UMI
 Author: Ye Chang
 Author-email: yech1990@gmail.com
 Requires-Python: >=3.8,<4.0
```

