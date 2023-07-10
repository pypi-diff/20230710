# Comparing `tmp/ReNaLabApp-0.0.1.dev7.tar.gz` & `tmp/ReNaLabApp-0.0.1.dev9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PycharmProjects\RealityNavigation\dist\tmp3p63ipko\ReNaLabApp-0.0.1.dev7.tar", last modified: Thu Nov 18 03:24:11 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

