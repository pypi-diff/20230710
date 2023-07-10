# Comparing `tmp/chloop-0.2.8-py3-none-any.whl.zip` & `tmp/chloop-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10811 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     8729 b- defN 17-Oct-08 12:21 chloop/__init__.py
--rw-rw-r--  2.0 unx     7869 b- defN 17-Oct-08 12:32 chloop-0.2.8.dist-info/DESCRIPTION.rst
--rw-rw-r--  2.0 unx      941 b- defN 17-Oct-08 12:32 chloop-0.2.8.dist-info/metadata.json
--rw-rw-r--  2.0 unx        7 b- defN 17-Oct-08 12:32 chloop-0.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx       92 b- defN 17-Oct-08 12:32 chloop-0.2.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx     8661 b- defN 17-Oct-08 12:32 chloop-0.2.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      562 b- defN 17-Oct-08 12:32 chloop-0.2.8.dist-info/RECORD
-7 files, 26861 bytes uncompressed, 9825 bytes compressed:  63.4%
+Zip file size: 10819 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx     8736 b- defN 17-Oct-08 16:10 chloop/__init__.py
+-rw-rw-r--  2.0 unx     7869 b- defN 17-Oct-08 23:02 chloop-0.2.9.dist-info/DESCRIPTION.rst
+-rw-rw-r--  2.0 unx      941 b- defN 17-Oct-08 23:02 chloop-0.2.9.dist-info/metadata.json
+-rw-rw-r--  2.0 unx        7 b- defN 17-Oct-08 23:02 chloop-0.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx       92 b- defN 17-Oct-08 23:02 chloop-0.2.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     8661 b- defN 17-Oct-08 23:02 chloop-0.2.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      562 b- defN 17-Oct-08 23:02 chloop-0.2.9.dist-info/RECORD
+7 files, 26868 bytes uncompressed, 9833 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: chloop/__init__.py
 Comment: 
 
-Filename: chloop-0.2.8.dist-info/DESCRIPTION.rst
+Filename: chloop-0.2.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: chloop-0.2.8.dist-info/metadata.json
+Filename: chloop-0.2.9.dist-info/metadata.json
 Comment: 
 
-Filename: chloop-0.2.8.dist-info/top_level.txt
+Filename: chloop-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: chloop-0.2.8.dist-info/WHEEL
+Filename: chloop-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: chloop-0.2.8.dist-info/METADATA
+Filename: chloop-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: chloop-0.2.8.dist-info/RECORD
+Filename: chloop-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chloop/__init__.py

```diff
@@ -96,15 +96,15 @@
                 if ch in ['\x03', '\x04']:
                     break
 
             if ch in self._chfunc_dict:
                 print(ch)
                 bh.call_func(self._chfunc_dict[ch][0], logger=logger)
             elif ch == '?':
-                print(self._class_doc())
+                print('?\n', self._class_doc())
                 print(self._startup_message)
             elif ch == '-':
                 try:
                     user_input = ih.user_input_fancy('', '- ')
                     if self._input_hook:
                         bh.call_func(self._input_hook, **user_input, logger=logger)
                     else:
```

## Comparing `chloop-0.2.8.dist-info/DESCRIPTION.rst` & `chloop-0.2.9.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `chloop-0.2.8.dist-info/metadata.json` & `chloop-0.2.9.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'download_url'": "'https://github.com/kenjyco/chloop/tarball/v0.2.9'", "'version'": "'0.2.9'"}*

```diff
@@ -4,15 +4,15 @@
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.5",
         "Topic :: Software Development :: Libraries",
         "Intended Audience :: Developers"
     ],
-    "download_url": "https://github.com/kenjyco/chloop/tarball/v0.2.8",
+    "download_url": "https://github.com/kenjyco/chloop/tarball/v0.2.9",
     "extensions": {
         "python.details": {
             "contacts": [
                 {
                     "email": "kenjyco@gmail.com",
                     "name": "Ken",
                     "role": "author"
@@ -45,9 +45,9 @@
                 "ipython",
                 "pdbpp",
                 "redis-helper"
             ]
         }
     ],
     "summary": "A Redis-backed REPL that saves command history, output, & errors",
-    "version": "0.2.8"
+    "version": "0.2.9"
 }
```

## Comparing `chloop-0.2.8.dist-info/METADATA` & `chloop-0.2.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.0
 Name: chloop
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Redis-backed REPL that saves command history, output, & errors
 Home-page: https://github.com/kenjyco/chloop
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/chloop/tarball/v0.2.8
+Download-URL: https://github.com/kenjyco/chloop/tarball/v0.2.9
 Keywords: repl,redis,command,history
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
```

