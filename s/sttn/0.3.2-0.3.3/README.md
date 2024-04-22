# Comparing `tmp/sttn-0.3.2.tar.gz` & `tmp/sttn-0.3.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/user/PycharmProjects/sttn/dist/.tmp-rjgjjclf/sttn-0.3.2.tar", last modified: Fri Feb  2 06:43:01 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

