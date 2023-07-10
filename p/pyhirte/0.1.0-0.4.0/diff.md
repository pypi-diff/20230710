# Comparing `tmp/pyhirte-0.1.0.tar.gz` & `tmp/pyhirte-0.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhirte-0.1.0.tar", last modified: Thu Jun 29 08:48:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

