# Comparing `tmp/micomputing-1.1.44.tar.gz` & `tmp/micomputing-1.1.45-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micomputing-1.1.44.tar", last modified: Fri Jul  7 10:16:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

