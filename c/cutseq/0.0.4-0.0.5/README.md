# Comparing `tmp/cutseq-0.0.4.tar.gz` & `tmp/cutseq-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutseq-0.0.4.tar", max compression
+gzip compressed data, was "cutseq-0.0.5.tar", max compression
```

## Comparing `cutseq-0.0.4.tar` & `cutseq-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      362 2024-04-21 22:40:35.183062 cutseq-0.0.4/README.md
--rw-r--r--   0        0        0    18864 2024-04-21 22:40:35.183062 cutseq-0.0.4/cutseq/run.py
--rw-r--r--   0        0        0    14395 2024-04-21 22:40:35.183062 cutseq-0.0.4/cutseq/run_cmd.py
--rw-r--r--   0        0        0      510 2024-04-21 22:40:35.183062 cutseq-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 cutseq-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      362 2024-04-22 00:19:47.644237 cutseq-0.0.5/README.md
+-rw-r--r--   0        0        0    20509 2024-04-22 00:19:47.644237 cutseq-0.0.5/cutseq/run.py
+-rw-r--r--   0        0        0    14395 2024-04-22 00:19:47.644237 cutseq-0.0.5/cutseq/run_cmd.py
+-rw-r--r--   0        0        0      510 2024-04-22 00:19:47.644237 cutseq-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 cutseq-0.0.5/PKG-INFO
```

### Comparing `cutseq-0.0.4/cutseq/run.py` & `cutseq-0.0.5/cutseq/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,32 +14,31 @@
 
 from cutadapt.adapters import (
     BackAdapter,
     NonInternalBackAdapter,
     NonInternalFrontAdapter,
     PrefixAdapter,
     RightmostFrontAdapter,
+    SuffixAdapter,
 )
 from cutadapt.files import InputPaths, OutputFiles
 from cutadapt.modifiers import (
     AdapterCutter,
     PairedEndRenamer,
     QualityTrimmer,
     Renamer,
     SuffixRemover,
     UnconditionalCutter,
 )
 from cutadapt.pipeline import PairedEndPipeline, SingleEndPipeline
-from cutadapt.predicates import IsUntrimmed, TooShort
+from cutadapt.predicates import Predicate, TooShort
 from cutadapt.runners import make_runner
 from cutadapt.steps import (
-    InfoFileWriter,
     PairedEndFilter,
     PairedEndSink,
-    PairedSingleEndStep,
     SingleEndFilter,
     SingleEndSink,
 )
 from cutadapt.utils import Progress
 
 logging.basicConfig(
     level=logging.INFO,
@@ -114,35 +113,54 @@
         self.mask5 = BarcodeSeq(d["mask5"])
         self.mask3 = BarcodeSeq(d["mask3"])
 
 
 class CutadaptConfig:
     def __init__(self):
         self.rname_suffix = False
-        self.discarded_untrimmed = False
+        self.ensure_inline_barcode = False
         self.trim_polyA = False
         self.min_length = 20
         self.min_quality = 20
         self.dry_run = False
         self.threads = 1
 
 
+class IsUntrimmedRef(Predicate):
+    """
+    Select reads for which no adapter match was found
+    """
+
+    def __init__(self, ref_adapters):
+        self.ref_adapters = ref_adapters
+
+    def __repr__(self):
+        return "IsUntrimmedRef()"
+
+    def test(self, read, info):
+        # check not all adapters with ref_adapters are exist in the matches
+        match_adapters = [match.adapter for match in info.matches]
+        if any([adapter not in match_adapters for adapter in self.ref_adapters]):
+            return True
+        return False
+
+
 def run_steps(steps, dry_run=False):
     if dry_run:
         print(
             " |\\\n".join([("    " + s if i > 0 else s) for i, s in enumerate(steps)])
         )
         process = subprocess.run("true", shell=True, capture_output=True)
     else:
         cmd = " | ".join(steps)
         process = subprocess.run(cmd, shell=True, capture_output=True)
     return process.stdout.decode(), process.stderr.decode()
 
 
-def pipeline_single(input1, output1, short1, untrimed1, barcode, settings):
+def pipeline_single(input1, output1, short1, untrimmed1, barcode, settings):
     modifiers = []
     # step 1: remove suffix in the read name
     modifiers.extend([SuffixRemover(".1"), SuffixRemover("/1")])
     # step 2: remove adapter on the 5' end, artifact of template switching
     modifiers.append(
         AdapterCutter(
             [
@@ -158,22 +176,19 @@
         AdapterCutter(
             [BackAdapter(sequence=barcode.p7.fw, max_errors=0.2, min_overlap=3)],
             times=2,
         ),
     )
     # step 4: trim inline barcode
     if barcode.inline5.len > 0:
-        modifiers.append(
-            AdapterCutter(
-                [PrefixAdapter(sequence=barcode.inline5.fw, max_errors=0.2)],
-                times=1,
-            )
-        )
+        adapter_inline5 = PrefixAdapter(sequence=barcode.inline5.fw, max_errors=0.2)
+        modifiers.append(AdapterCutter([adapter_inline5], times=1))
     if barcode.inline3.len > 0:
-        modifiers.append(UnconditionalCutter(-barcode.inline3.len))
+        adapter_inline3 = SuffixAdapter(sequence=barcode.inline3.fw, max_errors=0.2)
+        modifiers.append(AdapterCutter([adapter_inline3], times=1))
 
     # step 5: extract UMI
     if barcode.umi5.len > 0:
         modifiers.append(UnconditionalCutter(barcode.umi5.len))
     if barcode.umi3.len > 0:
         modifiers.append(UnconditionalCutter(-barcode.umi3.len))
     if barcode.umi5.len + barcode.umi3.len > 0:
@@ -211,41 +226,57 @@
 
     with make_runner(inpaths, cores=settings.threads) as runner:
         outfiles = OutputFiles(
             proxied=settings.threads > 1,
             qualities=runner.input_file_format().has_qualities(),
             interleaved=False,
         )
-        steps = [
+        steps = []
+        steps.append(
             # --info-file=info.txt
             # PairedSingleEndStep(InfoFileWriter(outfiles.open_text("info.txt"))),
             # -m 10
             SingleEndFilter(
                 TooShort(settings.min_length), outfiles.open_record_writer(short1)
             ),
-            # TODO: --max-n=0 support
-            # --discard-untrimmed
-            # SingleEndFilter( IsUntrimmed(), IsUntrimmed(), pair_filter_mode="any"),
+        )
+        if (
+            settings.ensure_inline_barcode
+            and barcode.inline5.len + barcode.inline3.len > 0
+        ):
+            ref_adapters = []
+            if barcode.inline5.len > 0:
+                ref_adapters.append(adapter_inline5)
+            if barcode.inline3.len > 0:
+                ref_adapters.append(adapter_inline3)
+            steps.append(
+                # TODO: --max-n=0 support
+                SingleEndFilter(
+                    IsUntrimmedRef(ref_adapters),
+                    outfiles.open_record_writer(untrimmed1, interleaved=False),
+                ),
+            )
+        steps.append(
             # -o
             SingleEndSink(outfiles.open_record_writer(output1, interleaved=False)),
-        ]
+        )
         pipeline = SingleEndPipeline(modifiers, steps)
         _stats = runner.run(pipeline, Progress(), outfiles)
         # _ = stats.as_json()
     outfiles.close()
 
 
 def pipeline_paired(
     input1,
     input2,
     output1,
     output2,
     short1,
     short2,
-    untrimed1,
+    untrimmed1,
     untrimmed2,
     barcode,
     settings,
 ):
     modifiers = []
     # step 1: remove suffix in the read name
     modifiers.extend(
@@ -286,31 +317,27 @@
                 [BackAdapter(sequence=barcode.p5.rc, max_errors=0.2, min_overlap=3)],
                 times=2,
             ),
         ),
     )
     # step 4: trim inline barcode
     if barcode.inline5.len > 0:
+        adapter_inline5 = PrefixAdapter(sequence=barcode.inline5.fw, max_errors=0.2)
         modifiers.append(
             (
-                AdapterCutter(
-                    [PrefixAdapter(sequence=barcode.inline5.fw, max_errors=0.2)],
-                    times=1,
-                ),
+                AdapterCutter([adapter_inline5], times=1),
                 UnconditionalCutter(-barcode.inline5.len),
             )
         )
     if barcode.inline3.len > 0:
+        adapter_inline3 = PrefixAdapter(sequence=barcode.inline3.rc, max_errors=0.2)
         modifiers.append(
             (
                 UnconditionalCutter(-barcode.inline3.len),
-                AdapterCutter(
-                    [BackAdapter(sequence=barcode.inline3.rc, max_errors=0.2)],
-                    times=1,
-                ),
+                AdapterCutter([adapter_inline3], times=1),
             )
         )
 
     # step 5: extract UMI
     if barcode.umi5.len > 0:
         modifiers.append(
             (
@@ -383,44 +410,60 @@
 
     with make_runner(inpaths, cores=settings.threads) as runner:
         outfiles = OutputFiles(
             proxied=settings.threads > 1,
             qualities=runner.input_file_format().has_qualities(),
             interleaved=False,
         )
-        steps = [
-            # --info-file=info.txt
-            # PairedSingleEndStep(InfoFileWriter(outfiles.open_text("info.txt"))),
-            # -m 10:10
+        steps = []
+        # --info-file=info.txt
+        # PairedSingleEndStep(InfoFileWriter(outfiles.open_text("info.txt"))),
+        # -m 10:10
+        steps.append(
             PairedEndFilter(
                 TooShort(settings.min_length),
                 TooShort(settings.min_length),
                 outfiles.open_record_writer(short1, short2, interleaved=False),
-            ),
-            # TODO: --max-n=0 support
-            # --discard-untrimmed
-            # PairedEndFilter( IsUntrimmed(), IsUntrimmed(), pair_filter_mode="any"),
+            )
+        )
+        if (
+            settings.ensure_inline_barcode
+            and barcode.inline5.len + barcode.inline3.len > 0
+        ):
+            steps.append(
+                # TODO: --max-n=0 support
+                PairedEndFilter(
+                    IsUntrimmedRef([adapter_inline5])
+                    if barcode.inline5.len > 0
+                    else None,
+                    IsUntrimmedRef([adapter_inline3])
+                    if barcode.inline3.len > 0
+                    else None,
+                    outfiles.open_record_writer(
+                        untrimmed1, untrimmed2, interleaved=False
+                    ),
+                    pair_filter_mode="any",
+                )
+            )
+        steps.append(
             # -o ... -p ...
-            PairedEndSink(outfiles.open_record_writer(output1, output2)),
-        ]
+            PairedEndSink(outfiles.open_record_writer(output1, output2))
+        )
         pipeline = PairedEndPipeline(modifiers, steps)
         _stats = runner.run(pipeline, Progress(), outfiles)
         # _ = stats.as_json()
     outfiles.close()
 
 
 def run_cutseq(args):
     barcode_config = BarcodeConfig(args.adapter_scheme.upper())
     settings = CutadaptConfig()
-    if args.with_rname_suffix:
-        settings.rname_suffix = True
-    if args.untrimmed_file is None:
-        settings.discarded_untrimmed = True
-    if args.trim_polyA:
-        settings.trim_polyA = True
+    settings.rname_suffix = args.with_rname_suffix
+    settings.ensure_inline_barcode = args.ensure_inline_barcode
+    settings.trim_polyA = args.trim_polyA
     settings.threads = args.threads
     settings.min_length = args.min_length
     settings.dry_run = args.dry_run
     if len(args.input_file) == 1:
         pipeline_single(
             args.input_file[0],
             args.output_file[0],
@@ -502,14 +545,20 @@
     )
 
     parser.add_argument(
         "--with-rname-suffix",
         action="store_true",
         help="R1 and R2 suffix cotains suffix. MGI platform.",
     )
+
+    parser.add_argument(
+        "--ensure-inline-barcode",
+        action="store_true",
+        help="Output discarded reads without inline barcode.",
+    )
     parser.add_argument(
         "-U",
         "--untrimmed-file",
         type=str,
         nargs="+",
         help="Output file path for discarded reads without inline barcode.",
     )
@@ -580,20 +629,16 @@
 
     args.output_file = validate_output_file(
         args.output_file, args.input_file, args.output_prefix, "trimmed"
     )
     args.short_file = validate_output_file(
         args.short_file, args.input_file, args.output_prefix, "short"
     )
-    args.untrimmed_file = (
-        validate_output_file(
-            args.untrimmed_file, args.input_file, args.output_prefix, "untrimmed"
-        )
-        if args.untrimmed_file is not None
-        else [None] * len(args.input_file)
+    args.untrimmed_file = validate_output_file(
+        args.untrimmed_file, args.input_file, args.output_prefix, "untrimmed"
     )
 
     run_cutseq(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cutseq-0.0.4/cutseq/run_cmd.py` & `cutseq-0.0.5/cutseq/run_cmd.py`

 * *Files identical despite different names*

### Comparing `cutseq-0.0.4/PKG-INFO` & `cutseq-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutseq
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automatically cut adapter / barcode / UMI from NGS data
 Home-page: https://github.com/y9c/cutseq
 License: MIT
 Keywords: bioinformatics,NGS,adapter,barcode,UMI
 Author: Ye Chang
 Author-email: yech1990@gmail.com
 Requires-Python: >=3.8,<4.0
```

