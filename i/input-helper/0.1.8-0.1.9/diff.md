# Comparing `tmp/input_helper-0.1.8-py3-none-any.whl.zip` & `tmp/input_helper-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 14521 bytes, number of entries: 10
--rw-rw-r--  2.0 unx     8979 b- defN 17-Sep-17 15:59 input_helper/__init__.py
+Zip file size: 14542 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx     9071 b- defN 17-Oct-21 18:33 input_helper/__init__.py
 -rw-rw-r--  2.0 unx    12524 b- defN 17-May-26 01:49 input_helper/matcher.py
 -rw-rw-r--  2.0 unx        0 b- defN 17-Apr-05 03:23 tests/__init__.py
 -rw-rw-r--  2.0 unx    18860 b- defN 17-May-26 01:49 tests/test_matcher.py
--rw-rw-r--  2.0 unx     2336 b- defN 17-Sep-17 16:06 input_helper-0.1.8.dist-info/DESCRIPTION.rst
--rw-rw-r--  2.0 unx      874 b- defN 17-Sep-17 16:06 input_helper-0.1.8.dist-info/metadata.json
--rw-rw-r--  2.0 unx       19 b- defN 17-Sep-17 16:06 input_helper-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx       92 b- defN 17-Sep-17 16:06 input_helper-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx     3007 b- defN 17-Sep-17 16:06 input_helper-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      839 b- defN 17-Sep-17 16:06 input_helper-0.1.8.dist-info/RECORD
-10 files, 47530 bytes uncompressed, 13101 bytes compressed:  72.4%
+-rw-rw-r--  2.0 unx     2336 b- defN 17-Oct-21 18:40 input_helper-0.1.9.dist-info/DESCRIPTION.rst
+-rw-rw-r--  2.0 unx      874 b- defN 17-Oct-21 18:40 input_helper-0.1.9.dist-info/metadata.json
+-rw-rw-r--  2.0 unx       19 b- defN 17-Oct-21 18:40 input_helper-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx       92 b- defN 17-Oct-21 18:40 input_helper-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     3007 b- defN 17-Oct-21 18:40 input_helper-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      839 b- defN 17-Oct-21 18:40 input_helper-0.1.9.dist-info/RECORD
+10 files, 47622 bytes uncompressed, 13122 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_matcher.py
 Comment: 
 
-Filename: input_helper-0.1.8.dist-info/DESCRIPTION.rst
+Filename: input_helper-0.1.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: input_helper-0.1.8.dist-info/metadata.json
+Filename: input_helper-0.1.9.dist-info/metadata.json
 Comment: 
 
-Filename: input_helper-0.1.8.dist-info/top_level.txt
+Filename: input_helper-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: input_helper-0.1.8.dist-info/WHEEL
+Filename: input_helper-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: input_helper-0.1.8.dist-info/METADATA
+Filename: input_helper-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: input_helper-0.1.8.dist-info/RECORD
+Filename: input_helper-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## input_helper/__init__.py

```diff
@@ -43,23 +43,27 @@
             matched = um(thing)
             if matched:
                 urls.extend(matched['url_list'])
     return urls
 
 
 def from_string(val):
-    """Return simple bool, int, and float values contained in a string
+    """Return simple bool, None, int, and float values contained in a string
 
     Useful for converting items in config files parsed by
     `configparser.RawConfigParser()` or values pulled from Redis
     """
-    if val.lower() == 'true':
+    if val is None:
+        pass
+    elif val.lower() == 'true':
         val = True
     elif val.lower() == 'false':
         val = False
+    elif val.lower() == 'none':
+        val = None
     else:
         try:
             val = float(val)
             if val.is_integer():
                 val = int(val)
         except ValueError:
             try:
```

## Comparing `input_helper-0.1.8.dist-info/DESCRIPTION.rst` & `input_helper-0.1.9.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `input_helper-0.1.8.dist-info/metadata.json` & `input_helper-0.1.9.dist-info/metadata.json`

 * *Files 12% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'download_url'": "'https://github.com/kenjyco/input-helper/tarball/v0.1.9'",*

 * * "'version'": "'0.1.9'"}*

```diff
@@ -4,15 +4,15 @@
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.5",
         "Topic :: Software Development :: Libraries",
         "Intended Audience :: Developers"
     ],
-    "download_url": "https://github.com/kenjyco/input-helper/tarball/v0.1.8",
+    "download_url": "https://github.com/kenjyco/input-helper/tarball/v0.1.9",
     "extensions": {
         "python.details": {
             "contacts": [
                 {
                     "email": "kenjyco@gmail.com",
                     "name": "Ken",
                     "role": "author"
@@ -39,9 +39,9 @@
     "test_requires": [
         {
             "requires": [
                 "pytest"
             ]
         }
     ],
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

## Comparing `input_helper-0.1.8.dist-info/METADATA` & `input_helper-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.0
 Name: input-helper
-Version: 0.1.8
+Version: 0.1.9
 Summary: Common CLI input helper functions and string/arg conversions
 Home-page: https://github.com/kenjyco/input-helper
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/input-helper/tarball/v0.1.8
+Download-URL: https://github.com/kenjyco/input-helper/tarball/v0.1.9
 Keywords: input,cli,helper
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
```

