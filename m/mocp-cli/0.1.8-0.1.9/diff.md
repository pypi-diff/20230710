# Comparing `tmp/mocp_cli-0.1.8-py3-none-any.whl.zip` & `tmp/mocp_cli-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10672 bytes, number of entries: 11
+Zip file size: 10705 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      600 b- defN 17-Oct-21 18:33 mocp_cli/__init__.py
--rw-rw-r--  2.0 unx    10557 b- defN 17-Nov-02 12:36 mocp_cli/player.py
+-rw-rw-r--  2.0 unx    10682 b- defN 17-Nov-04 17:28 mocp_cli/player.py
 -rw-rw-r--  2.0 unx        0 b- defN 17-Apr-05 03:23 mocp_cli/scripts/__init__.py
 -rw-rw-r--  2.0 unx      321 b- defN 17-Apr-05 03:23 mocp_cli/scripts/player.py
--rw-rw-r--  2.0 unx     5918 b- defN 17-Nov-02 13:01 mocp_cli-0.1.8.dist-info/DESCRIPTION.rst
--rw-rw-r--  2.0 unx       60 b- defN 17-Nov-02 13:01 mocp_cli-0.1.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx     1256 b- defN 17-Nov-02 13:01 mocp_cli-0.1.8.dist-info/metadata.json
--rw-rw-r--  2.0 unx        9 b- defN 17-Nov-02 13:01 mocp_cli-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx       92 b- defN 17-Nov-02 13:01 mocp_cli-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx     6889 b- defN 17-Nov-02 13:01 mocp_cli-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      916 b- defN 17-Nov-02 13:01 mocp_cli-0.1.8.dist-info/RECORD
-11 files, 26618 bytes uncompressed, 9128 bytes compressed:  65.7%
+-rw-rw-r--  2.0 unx     5918 b- defN 17-Nov-04 17:30 mocp_cli-0.1.9.dist-info/DESCRIPTION.rst
+-rw-rw-r--  2.0 unx       60 b- defN 17-Nov-04 17:30 mocp_cli-0.1.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx     1256 b- defN 17-Nov-04 17:30 mocp_cli-0.1.9.dist-info/metadata.json
+-rw-rw-r--  2.0 unx        9 b- defN 17-Nov-04 17:30 mocp_cli-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx       92 b- defN 17-Nov-04 17:30 mocp_cli-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     6889 b- defN 17-Nov-04 17:30 mocp_cli-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      916 b- defN 17-Nov-04 17:30 mocp_cli-0.1.9.dist-info/RECORD
+11 files, 26743 bytes uncompressed, 9161 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: mocp_cli/scripts/__init__.py
 Comment: 
 
 Filename: mocp_cli/scripts/player.py
 Comment: 
 
-Filename: mocp_cli-0.1.8.dist-info/DESCRIPTION.rst
+Filename: mocp_cli-0.1.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: mocp_cli-0.1.8.dist-info/entry_points.txt
+Filename: mocp_cli-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: mocp_cli-0.1.8.dist-info/metadata.json
+Filename: mocp_cli-0.1.9.dist-info/metadata.json
 Comment: 
 
-Filename: mocp_cli-0.1.8.dist-info/top_level.txt
+Filename: mocp_cli-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: mocp_cli-0.1.8.dist-info/WHEEL
+Filename: mocp_cli-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: mocp_cli-0.1.8.dist-info/METADATA
+Filename: mocp_cli-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: mocp_cli-0.1.8.dist-info/RECORD
+Filename: mocp_cli-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mocp_cli/player.py

```diff
@@ -1,15 +1,15 @@
 import moc
 import input_helper as ih
 from functools import partial
 from collections import OrderedDict
 from chloop import GetCharLoop
 from mocp_cli import logger
 try:
-    from yt_helper import COMMENTS, FILES, get_real_basename
+    from yt_helper import AUDIO_COMMENTS as COMMENTS, FILES, get_real_basename
     if COMMENTS is None:
         raise ImportError
 
 except ImportError:
     input_hook = None
 
     def mark_it():
@@ -166,20 +166,21 @@
     if paths:
         moc.find_and_play(*paths)
 
 
 def recent_files_play_select(limit=25):
     """Select files that were most recently added and play"""
     selected = ih.make_selections(
-        FILES.recent_unique_values(limit=limit),
+        FILES.find('audio:True', get_fields='basename', admin_fmt=True, limit=limit),
+        item_format='{basename} .::. {_ts}',
         prompt='Select basenames to play',
         wrap=False
     )
     if selected:
-        play_basenames(*selected)
+        play_basenames(*[x['basename'] for x in selected])
 
 
 def most_commented_files_play_select(limit=25):
     """Select files that have been most commented and play"""
     selected = ih.make_selections(
         COMMENTS.top_values_for_index('basename', limit=limit),
         prompt='Select basenames to play',
```

## Comparing `mocp_cli-0.1.8.dist-info/DESCRIPTION.rst` & `mocp_cli-0.1.9.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `mocp_cli-0.1.8.dist-info/metadata.json` & `mocp_cli-0.1.9.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9230769230769231%*

 * *Differences: {"'download_url'": "'https://github.com/kenjyco/mocp-cli/tarball/v0.1.9'", "'version'": "'0.1.9'"}*

```diff
@@ -6,15 +6,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.5",
         "Topic :: Software Development :: Libraries",
         "Topic :: Multimedia :: Sound/Audio :: Players",
         "Intended Audience :: Developers"
     ],
     "description_content_type": "UNKNOWN",
-    "download_url": "https://github.com/kenjyco/mocp-cli/tarball/v0.1.8",
+    "download_url": "https://github.com/kenjyco/mocp-cli/tarball/v0.1.9",
     "extensions": {
         "python.commands": {
             "wrap_console": {
                 "mocplayer": "mocp_cli.scripts.player:main"
             }
         },
         "python.details": {
@@ -62,9 +62,9 @@
                 "parse-helper",
                 "redis-helper",
                 "yt-helper"
             ]
         }
     ],
     "summary": "CLI tools for finding, organizing, and playing audio files",
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

## Comparing `mocp_cli-0.1.8.dist-info/METADATA` & `mocp_cli-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.0
 Name: mocp-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: CLI tools for finding, organizing, and playing audio files
 Home-page: https://github.com/kenjyco/mocp-cli
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/mocp-cli/tarball/v0.1.8
+Download-URL: https://github.com/kenjyco/mocp-cli/tarball/v0.1.9
 Description-Content-Type: UNKNOWN
 Keywords: moc,mocp,console audio,mp3 player
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

## Comparing `mocp_cli-0.1.8.dist-info/RECORD` & `mocp_cli-0.1.9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mocp_cli/__init__.py,sha256=9O-ViADyynDVJFxuSjFfBMznHn9UI5tJzVrwv7czZ2s,600
-mocp_cli/player.py,sha256=zIOCzJ85OclGNCugg2kbA4uUXGN3loUr1lWOF4SHH74,10557
+mocp_cli/player.py,sha256=OWr-6uykUoOSRyuRqCdAWUEUnypwLLl-unPTmhKC6VY,10682
 mocp_cli/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mocp_cli/scripts/player.py,sha256=qtAFJ3CpLXCa6qNZ5VM0ybEEnIq5lBqNciz7JzxLLso,321
-mocp_cli-0.1.8.dist-info/DESCRIPTION.rst,sha256=ECU7E-Bo9rYOYCiZmGKWzeQm91ae7pzYGnUPkQGW85g,5918
-mocp_cli-0.1.8.dist-info/METADATA,sha256=GB2eIeFWVLEz-8ZxQ2Fk16XbJI_7DhfsGzAkITNBKDE,6889
-mocp_cli-0.1.8.dist-info/RECORD,,
-mocp_cli-0.1.8.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-mocp_cli-0.1.8.dist-info/entry_points.txt,sha256=3KrH25CP7o8pDY4nHDR00ouKmca9aTXgX7Ncl8qq_Wg,60
-mocp_cli-0.1.8.dist-info/metadata.json,sha256=q2RrfDWEoQ_Ykpv4iAntt-aXYQLEndwi4XXd9GlqOqE,1256
-mocp_cli-0.1.8.dist-info/top_level.txt,sha256=KMQ5_uZ7we2K15PG2QrrUcz6DH5d780qDe4GvGqa27o,9
+mocp_cli-0.1.9.dist-info/DESCRIPTION.rst,sha256=ECU7E-Bo9rYOYCiZmGKWzeQm91ae7pzYGnUPkQGW85g,5918
+mocp_cli-0.1.9.dist-info/METADATA,sha256=ePUNes2TEp0kHZTQ2JyTWKNZnm8ZPYC7Q4z5icwCyoU,6889
+mocp_cli-0.1.9.dist-info/RECORD,,
+mocp_cli-0.1.9.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+mocp_cli-0.1.9.dist-info/entry_points.txt,sha256=3KrH25CP7o8pDY4nHDR00ouKmca9aTXgX7Ncl8qq_Wg,60
+mocp_cli-0.1.9.dist-info/metadata.json,sha256=nGG4KO1MGJw9Aqcho3YQmtHto3AWnT4xkuVsyLshsKk,1256
+mocp_cli-0.1.9.dist-info/top_level.txt,sha256=KMQ5_uZ7we2K15PG2QrrUcz6DH5d780qDe4GvGqa27o,9
```

