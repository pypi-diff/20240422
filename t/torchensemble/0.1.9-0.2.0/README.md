# Comparing `tmp/torchensemble-0.1.9.tar.gz` & `tmp/torchensemble-0.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchensemble-0.1.9.tar", last modified: Sun Aug 21 06:20:40 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

