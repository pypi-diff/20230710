# Comparing `tmp/PyFoam-2022.9.tar.gz` & `tmp/PyFoam-2023.7-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/slowdata/LinkInHome/Projects/PyFoam/dist/tmpfr4yc9ha/PyFoam-2022.9.tar", last modified: Sun Sep 11 23:41:05 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

