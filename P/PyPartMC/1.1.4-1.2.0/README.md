# Comparing `tmp/PyPartMC-1.1.4.tar.gz` & `tmp/PyPartMC-1.2.0-cp39-cp39-macosx_12_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPartMC-1.1.4.tar", last modified: Tue Apr  2 06:58:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

