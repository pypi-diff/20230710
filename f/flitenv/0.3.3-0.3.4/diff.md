# Comparing `tmp/flitenv-0.3.3.tar.gz` & `tmp/flitenv-0.3.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flitenv-0.3.3.tar", last modified: Mon Jul  5 08:39:30 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

