# Comparing `tmp/noiseflow-0.0.7a2.tar.gz` & `tmp/noiseflow-0.0.8-cp39-cp39-manylinux_2_35_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noiseflow-0.0.7a2.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

