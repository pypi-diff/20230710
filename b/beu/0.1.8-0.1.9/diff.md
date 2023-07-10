# Comparing `tmp/beu-0.1.8-py3-none-any.whl.zip` & `tmp/beu-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5607 bytes, number of entries: 12
--rw-rw-r--  2.0 unx     1027 b- defN 17-Mar-25 15:19 beu/__init__.py
+Zip file size: 5561 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx      847 b- defN 17-Mar-26 02:44 beu/__init__.py
 -rw-rw-r--  2.0 unx      674 b- defN 17-Mar-20 09:05 beu/scripts/audiosearch.py
 -rw-rw-r--  2.0 unx      509 b- defN 17-Mar-20 09:05 beu/scripts/vidsearch.py
 -rw-rw-r--  2.0 unx      185 b- defN 17-Mar-18 15:59 beu/scripts/shell.py
 -rw-rw-r--  2.0 unx        0 b- defN 17-Mar-15 13:44 beu/scripts/__init__.py
--rw-rw-r--  2.0 unx     1316 b- defN 17-Mar-25 15:20 beu-0.1.8.dist-info/DESCRIPTION.rst
--rw-rw-r--  2.0 unx      146 b- defN 17-Mar-25 15:20 beu-0.1.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx     1279 b- defN 17-Mar-25 15:20 beu-0.1.8.dist-info/metadata.json
--rw-rw-r--  2.0 unx        4 b- defN 17-Mar-25 15:20 beu-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx       92 b- defN 17-Mar-25 15:20 beu-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2140 b- defN 17-Mar-25 15:20 beu-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      954 b- defN 17-Mar-25 15:20 beu-0.1.8.dist-info/RECORD
-12 files, 8326 bytes uncompressed, 4025 bytes compressed:  51.7%
+-rw-rw-r--  2.0 unx     1442 b- defN 17-Mar-26 02:45 beu-0.1.9.dist-info/DESCRIPTION.rst
+-rw-rw-r--  2.0 unx      146 b- defN 17-Mar-26 02:45 beu-0.1.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx     1292 b- defN 17-Mar-26 02:45 beu-0.1.9.dist-info/metadata.json
+-rw-rw-r--  2.0 unx        4 b- defN 17-Mar-26 02:45 beu-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx       92 b- defN 17-Mar-26 02:45 beu-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2291 b- defN 17-Mar-26 02:45 beu-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      953 b- defN 17-Mar-26 02:45 beu-0.1.9.dist-info/RECORD
+12 files, 8435 bytes uncompressed, 3979 bytes compressed:  52.8%
```

## zipnote {}

```diff
@@ -9,29 +9,29 @@
 
 Filename: beu/scripts/shell.py
 Comment: 
 
 Filename: beu/scripts/__init__.py
 Comment: 
 
-Filename: beu-0.1.8.dist-info/DESCRIPTION.rst
+Filename: beu-0.1.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: beu-0.1.8.dist-info/entry_points.txt
+Filename: beu-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: beu-0.1.8.dist-info/metadata.json
+Filename: beu-0.1.9.dist-info/metadata.json
 Comment: 
 
-Filename: beu-0.1.8.dist-info/top_level.txt
+Filename: beu-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: beu-0.1.8.dist-info/WHEEL
+Filename: beu-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: beu-0.1.8.dist-info/METADATA
+Filename: beu-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: beu-0.1.8.dist-info/RECORD
+Filename: beu-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beu/__init__.py

```diff
@@ -1,17 +1,16 @@
 import redis_helper as rh
 import input_helper as ih
 import yt_helper as yh
 import parse_helper as ph
+import bg_helper as bh
 import moc
 import logging
 import os.path
-from subprocess import call
 from datetime import datetime
-from sys import exit
 
 
 LOGFILE = os.path.abspath('log--beu.log')
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 file_handler = logging.FileHandler(LOGFILE, mode='a')
 file_handler.setLevel(logging.DEBUG)
@@ -24,14 +23,7 @@
 logger.addHandler(file_handler)
 logger.addHandler(console_handler)
 
 
 def utc_now_iso():
     """Return current UTC timestamp in ISO format"""
     return datetime.utcnow().isoformat()
-
-
-def run_or_die(cmd):
-    """Run a shell command or exit the system"""
-    ret_code = call(cmd, shell=True)
-    if ret_code != 0:
-        exit(ret_code)
```

## Comparing `beu-0.1.8.dist-info/DESCRIPTION.rst` & `beu-0.1.9.dist-info/DESCRIPTION.rst`

 * *Files 12% similar despite different names*

```diff
@@ -36,11 +36,14 @@
 
     In [3]: beu.rh
     Out[3]: <module 'redis_helper' from '/tmp/stuff/venv/lib/python3.5/site-packages/redis_helper/__init__.py'>
 
     In [4]: beu.yh
     Out[4]: <module 'yt_helper' from '/tmp/stuff/venv/lib/python3.5/site-packages/yt_helper/__init__.py'>
 
-    In [5]: beu.moc
-    Out[5]: <module 'moc' from '/tmp/stuff/venv/lib/python3.5/site-packages/moc/__init__.py'>
+    In [5]: beu.bh
+    Out[5]: <module 'bg_helper' from '/tmp/stuff/venv/lib/python3.5/site-packages/bg_helper/__init__.py'>
+
+    In [6]: beu.moc
+    Out[6]: <module 'moc' from '/tmp/stuff/venv/lib/python3.5/site-packages/moc/__init__.py'>
```

## Comparing `beu-0.1.8.dist-info/metadata.json` & `beu-0.1.9.dist-info/metadata.json`

 * *Files 4% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9065656565656565%*

 * *Differences: {"'download_url'": "'https://github.com/kenjyco/beu/tarball/v0.1.9'",*

 * * "'run_requires'": "{0: {'requires': {insert: [(0, 'bg-helper')]}}}",*

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
-    "download_url": "https://github.com/kenjyco/beu/tarball/v0.1.8",
+    "download_url": "https://github.com/kenjyco/beu/tarball/v0.1.9",
     "extensions": {
         "python.commands": {
             "wrap_console": {
                 "beu-audiosearch": "beu.scripts.audiosearch:main",
                 "beu-ipython": "beu.scripts.shell:main",
                 "beu-vidsearch": "beu.scripts.vidsearch:main"
             }
@@ -44,21 +44,22 @@
     "generator": "bdist_wheel (0.29.0)",
     "license": "MIT",
     "metadata_version": "2.0",
     "name": "beu",
     "run_requires": [
         {
             "requires": [
+                "bg-helper",
                 "chloop",
                 "click",
                 "input-helper",
                 "ipython",
                 "mocp",
                 "parse-helper",
                 "redis-helper",
                 "yt-helper"
             ]
         }
     ],
     "summary": "Beginner Express .:. Back End .:. Big Example .:. Brainstorm Effectively",
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

## Comparing `beu-0.1.8.dist-info/METADATA` & `beu-0.1.9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.0
 Name: beu
-Version: 0.1.8
+Version: 0.1.9
 Summary: Beginner Express .:. Back End .:. Big Example .:. Brainstorm Effectively
 Home-page: https://github.com/kenjyco/beu
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/beu/tarball/v0.1.8
+Download-URL: https://github.com/kenjyco/beu/tarball/v0.1.9
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
+Requires-Dist: bg-helper
 Requires-Dist: chloop
 Requires-Dist: click
 Requires-Dist: input-helper
 Requires-Dist: ipython
 Requires-Dist: mocp
 Requires-Dist: parse-helper
 Requires-Dist: redis-helper
@@ -62,11 +63,14 @@
 
     In [3]: beu.rh
     Out[3]: <module 'redis_helper' from '/tmp/stuff/venv/lib/python3.5/site-packages/redis_helper/__init__.py'>
 
     In [4]: beu.yh
     Out[4]: <module 'yt_helper' from '/tmp/stuff/venv/lib/python3.5/site-packages/yt_helper/__init__.py'>
 
-    In [5]: beu.moc
-    Out[5]: <module 'moc' from '/tmp/stuff/venv/lib/python3.5/site-packages/moc/__init__.py'>
+    In [5]: beu.bh
+    Out[5]: <module 'bg_helper' from '/tmp/stuff/venv/lib/python3.5/site-packages/bg_helper/__init__.py'>
+
+    In [6]: beu.moc
+    Out[6]: <module 'moc' from '/tmp/stuff/venv/lib/python3.5/site-packages/moc/__init__.py'>
```

