# Comparing `tmp/python-libtiepie-0.9.9.tar.gz` & `tmp/python_libtiepie-1.1.5-py3-none-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-libtiepie-0.9.9.tar", last modified: Fri Feb  4 09:06:52 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

