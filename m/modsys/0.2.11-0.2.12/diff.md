# Comparing `tmp/modsys-0.2.11.tar.gz` & `tmp/modsys-0.2.12-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modsys-0.2.11.tar", last modified: Mon Jul 10 14:44:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

