# Comparing `tmp/ffmperative-0.0.3.tar.gz` & `tmp/ffmperative-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmperative-0.0.3.tar", last modified: Thu Jul  6 19:57:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

