# Comparing `tmp/dbt-doris-0.2.1.tar.gz` & `tmp/dbt_doris-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-doris-0.2.1.tar", last modified: Tue Jun  6 10:58:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

