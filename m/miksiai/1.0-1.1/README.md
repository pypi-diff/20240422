# Comparing `tmp/miksiai-1.0.tar.gz` & `tmp/miksiai-1.1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miksiai-1.0.tar", last modified: Sun Apr 21 11:29:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

