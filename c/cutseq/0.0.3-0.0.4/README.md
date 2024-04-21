# Comparing `tmp/cutseq-0.0.3.tar.gz` & `tmp/cutseq-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutseq-0.0.3.tar", max compression
+gzip compressed data, was "cutseq-0.0.4.tar", max compression
```

## Comparing `cutseq-0.0.3.tar` & `cutseq-0.0.4.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      120 2024-04-20 22:13:20.790186 cutseq-0.0.3/README.md
--rw-r--r--   0        0        0    14528 2024-04-20 22:13:20.790186 cutseq-0.0.3/cutseq/run.py
--rw-r--r--   0        0        0      510 2024-04-20 22:13:20.790186 cutseq-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 cutseq-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      362 2024-04-21 22:40:35.183062 cutseq-0.0.4/README.md
+-rw-r--r--   0        0        0    18864 2024-04-21 22:40:35.183062 cutseq-0.0.4/cutseq/run.py
+-rw-r--r--   0        0        0    14395 2024-04-21 22:40:35.183062 cutseq-0.0.4/cutseq/run_cmd.py
+-rw-r--r--   0        0        0      510 2024-04-21 22:40:35.183062 cutseq-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 cutseq-0.0.4/PKG-INFO
```

### Comparing `cutseq-0.0.3/cutseq/run.py` & `cutseq-0.0.4/cutseq/run_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,31 +36,37 @@
     suffixes = [s + ".gz" for s in suffixes] + suffixes
     for suffix in suffixes:
         if f.endswith(suffix):
             return f.removesuffix(suffix)
     return f
 
 
+class BarcodeSeq:
+    def __init__(self, seq):
+        self.fw = seq
+        self.rc = reverse_complement(seq)
+        self.len = len(seq)
+
+
 class BarcodeConfig:
+    """
+    Adapter scheme:
+    (p5)(inline5)(umi5)(mask5)(strand)(mask3)(umi3)(inline3)(p7)
+    """
+
     def __init__(self, adapter=None):
         self.strand = None
-        self.p5_fw = ""
-        self.p5_rc = ""
-        self.p7_fw = ""
-        self.p7_rc = ""
-        self.inline5_fw = ""
-        self.inline5_rc = ""
-        self.inline5 = 0
-        self.inline3_fw = ""
-        self.inline3_rc = ""
-        self.inline3 = 0
-        self.umi5 = 0
-        self.umi3 = 0
-        self.mask5 = 0
-        self.mask3 = 0
+        self.p5 = BarcodeSeq("")
+        self.p7 = BarcodeSeq("")
+        self.inline5 = BarcodeSeq("")
+        self.inline3 = BarcodeSeq("")
+        self.umi5 = BarcodeSeq("")
+        self.umi3 = BarcodeSeq("")
+        self.mask5 = BarcodeSeq("")
+        self.mask3 = BarcodeSeq("")
         if adapter is not None:
             self._parse_barcode(adapter)
 
     def _parse_barcode(self, b):
         m = re.match(
             r"(?P<p5>[ATGCatgc]+)(\((?P<inline5>[ATGCatgc]+)\))?(?P<umi5>N*)(?P<mask5>X*)(?P<strand>-|>|<)(?P<mask3>X*)(?P<umi3>N*)(\((?P<inline3>[ATGCatgc]+)\))?(?P<p7>[ATGCatgc]+)",
             b,
@@ -70,28 +76,22 @@
             sys.exit(1)
         d = m.groupdict()
         if d["inline5"] is None:
             d["inline5"] = ""
         if d["inline3"] is None:
             d["inline3"] = ""
         self.strand = "+" if d["strand"] == ">" else "-" if d["strand"] == "<" else None
-        self.p5_fw = d["p5"]
-        self.p5_rc = reverse_complement(d["p5"])
-        self.p7_fw = d["p7"]
-        self.p7_rc = reverse_complement(d["p7"])
-        self.inline5_fw = d["inline5"] if d["inline5"] else ""
-        self.inline5_rc = reverse_complement(d["inline5"]) if d["inline5"] else ""
-        self.inline5 = len(d["inline5"])
-        self.inline3_fw = d["inline3"] if d["inline3"] else ""
-        self.inline3_rc = reverse_complement(d["inline3"]) if d["inline3"] else ""
-        self.inline3 = len(d["inline3"])
-        self.umi5 = len(d["umi5"])
-        self.umi3 = len(d["umi3"])
-        self.mask5 = len(d["mask5"])
-        self.mask3 = len(d["mask3"])
+        self.p5 = BarcodeSeq(d["p5"])
+        self.p7 = BarcodeSeq(d["p7"])
+        self.inline5 = BarcodeSeq(d["inline5"])
+        self.inline3 = BarcodeSeq(d["inline3"])
+        self.umi5 = BarcodeSeq(d["umi5"])
+        self.umi3 = BarcodeSeq(d["umi3"])
+        self.mask5 = BarcodeSeq(d["mask5"])
+        self.mask3 = BarcodeSeq(d["mask3"])
 
 
 class CutadaptConfig:
     def __init__(self):
         self.rname_suffix = False
         self.discarded_untrimmed = False
         self.trim_polyA = False
@@ -108,44 +108,44 @@
     steps = []
     # step 1: remove adapter on the 5' end, artifact of template switching
     if settings.rname_suffix:
         config_rname = " --strip-suffix '/1' --strip-suffix '/2' --strip-suffix '.1' --strip-suffix '.2'"
     else:
         config_rname = ""
     steps.append(
-        f"{cutadapt}{config_rname} -e 0.25 -n 2 -O 10 -g '{barcode.p5_fw};rightmost' -G '{barcode.p7_rc};rightmost' --interleaved {input1} {input2}"
+        f"{cutadapt}{config_rname} -e 0.25 -n 2 -O 10 -g '{barcode.p5.fw};rightmost' -G '{barcode.p7.rc};rightmost' --interleaved {input1} {input2}"
     )
     # step 2: remove adapter on the 3' end, read though in the sequencing
     steps.append(
-        f"{cutadapt} -e 0.2 -n 2 -O 3 -a '{barcode.p7_fw}' -A '{barcode.p5_rc}' --interleaved -"
+        f"{cutadapt} -e 0.2 -n 2 -O 3 -a '{barcode.p7.fw}' -A '{barcode.p5.rc}' --interleaved -"
     )
     # step 3: trim inline barcode
     config_inline_args = []
-    if barcode.inline5 > 0:
-        config_inline_args.append(f"-g ^{barcode.inline5_fw} -U -{barcode.inline5}")
-    if barcode.inline3 > 0:
-        config_inline_args.append(f"-G ^{barcode.inline3_rc} -u -{barcode.inline3}")
-    if barcode.inline5 + barcode.inline3 > 0:
+    if barcode.inline5.len > 0:
+        config_inline_args.append(f"-g ^{barcode.inline5.fw} -U -{barcode.inline5.len}")
+    if barcode.inline3.len > 0:
+        config_inline_args.append(f"-G ^{barcode.inline3.rc} -u -{barcode.inline3.len}")
+    if barcode.inline5.len + barcode.inline3.len > 0:
         if settings.discarded_untrimmed:
             config_inline_args.append(
                 f"--untrimmed-output={discard1} --untrimmed-paired-output={discard2}"
             )
         config_inline = " ".join(config_inline_args)
         steps.append(f"{cutadapt} {config_inline} --interleaved -")
     # step 4: extract UMI
-    if barcode.umi5 + barcode.umi3 > 0:
+    if barcode.umi5.len + barcode.umi3.len > 0:
         steps.append(
-            f"{cutadapt} -u {barcode.umi5} -u -{barcode.umi3} -U {barcode.umi3} -U -{barcode.umi5} --rename='{{id}}_{{r1.cut_prefix}}{{r2.cut_prefix}}' --interleaved -"
+            f"{cutadapt} -u {barcode.umi5.len} -u -{barcode.umi3.len} -U {barcode.umi3.len} -U -{barcode.umi5.len} --rename='{{id}}_{{r1.cut_prefix}}{{r2.cut_prefix}}' --interleaved -"
         )
     else:
         steps.append(f"{cutadapt} --rename='{{id}}' --interleaved -")
     # step 5: mask tail in the RNA, which might be artifact of RT
-    if barcode.mask5 + barcode.mask3 > 0:
+    if barcode.mask5.len + barcode.mask3.len > 0:
         steps.append(
-            f"{cutadapt} -u {barcode.mask5} -u -{barcode.mask3} -U {barcode.mask3} -U -{barcode.mask5} --interleaved -"
+            f"{cutadapt} -u {barcode.mask5.len} -u -{barcode.mask3.len} -U {barcode.mask3.len} -U -{barcode.mask5.len} --interleaved -"
         )
     # step 6: trim polyA
     if settings.trim_polyA:
         if barcode.strand == "+":
             steps.append(
                 f"{cutadapt} -O 6 -e 0.15 -a 'A{{100}}' -G 'T{{100}}' --interleaved -"
             )
@@ -167,37 +167,37 @@
     steps = []
     # step 1: remove adapter on the 5' end, artifact of template switching
     if settings.rname_suffix:
         config_rname = " --strip-suffix '/1' --strip-suffix '.1'"
     else:
         config_rname = ""
     steps.append(
-        f"{cutadapt}{config_rname} -e 0.25 -n 2 -O 10 -g '{barcode.p5_fw};rightmost' {input1}"
+        f"{cutadapt}{config_rname} -e 0.25 -n 2 -O 10 -g '{barcode.p5.fw};rightmost' {input1}"
     )
     # step 2: remove adapter on the 3' end, read though in the sequencing
-    steps.append(f"{cutadapt} -e 0.2 -n 2 -O 3 -a '{barcode.p7_fw}' -")
+    steps.append(f"{cutadapt} -e 0.2 -n 2 -O 3 -a '{barcode.p7.fw}' -")
     # step 3: trim inline barcode
     config_inline_args = []
-    if barcode.inline3 > 0:
-        config_inline_args.append(f"-a {barcode.inline3_fw}$")
-    if barcode.inline5 > 0:
-        config_inline_args.append(f"-g ^{barcode.inline5_fw}")
-    if barcode.inline5 + barcode.inline3 > 0:
+    if barcode.inline3.len > 0:
+        config_inline_args.append(f"-a {barcode.inline3.fw}$")
+    if barcode.inline5.len > 0:
+        config_inline_args.append(f"-g ^{barcode.inline5.fw}")
+    if barcode.inline5.len + barcode.inline3.len > 0:
         if settings.discarded_untrimmed:
             config_inline_args.append(f"--untrimmed-output={discard1}")
 
         config_inline = " ".join(config_inline_args)
         steps.append(f"{cutadapt} {config_inline} -")
     # step 4: extract UMI
-    if barcode.umi5 + barcode.umi3 > 0:
+    if barcode.umi5.len + barcode.umi3.len > 0:
         steps.append(
-            f"{cutadapt} -u {barcode.umi5} -u -{barcode.umi3} --rename='{{id}}_{{cut_prefix}}{{cut_suffix}}' -"
+            f"{cutadapt} -u {barcode.umi5.len} -u -{barcode.umi3.len} --rename='{{id}}_{{cut_prefix}}{{cut_suffix}}' -"
         )
     # step 5: mask tail in the RNA, which might be artifact of RT
-    steps.append(f"{cutadapt} -u {barcode.mask5} -u -{barcode.mask3} -")
+    steps.append(f"{cutadapt} -u {barcode.mask5.len} -u -{barcode.mask3.len} -")
     # step 6: trim polyA
     if settings.trim_polyA:
         if barcode.strand == "+":
             steps.append(f"{cutadapt} -O 6 -e 0.15 -a 'A{{100}}' -")
         elif barcode.strand == "-":
             steps.append(f"{cutadapt} -O 6 -e 0.15 -g 'T{{100}}' -")
         else:
@@ -229,15 +229,14 @@
     if args.discarded_untrimmed:
         settings.discarded_untrimmed = True
     if args.trim_polyA:
         settings.trim_polyA = True
     settings.threads = args.threads
     settings.min_length = args.min_length
     settings.dry_run = args.dry_run
-    # Example command setup, you'll need to expand this based on your actual requirements
     if len(args.input_file) == 1:
         steps = run_cutadapt_SE(
             args.input_file[0],
             args.output_file[0],
             args.discard_file[0],
             barcode_config,
             settings,
```

