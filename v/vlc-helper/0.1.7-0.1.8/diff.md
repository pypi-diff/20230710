# Comparing `tmp/vlc_helper-0.1.7-py3-none-any.whl.zip` & `tmp/vlc_helper-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6909 bytes, number of entries: 12
+Zip file size: 6920 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx      122 b- defN 20-Aug-08 21:00 vlc_helper/__init__.py
 -rw-rw-r--  2.0 unx     1248 b- defN 20-Aug-08 21:00 vlc_helper/repl.py
--rw-rw-r--  2.0 unx     9199 b- defN 20-Aug-08 21:00 vlc_helper/vlc.py
+-rw-rw-r--  2.0 unx     9222 b- defN 22-Aug-18 15:40 vlc_helper/vlc.py
 -rw-rw-r--  2.0 unx        0 b- defN 20-Aug-08 21:00 vlc_helper/scripts/__init__.py
 -rw-rw-r--  2.0 unx      440 b- defN 20-Aug-08 21:00 vlc_helper/scripts/myvlc.py
 -rw-rw-r--  2.0 unx      173 b- defN 20-Aug-08 21:00 vlc_helper/scripts/repl.py
--rw-rw-r--  2.0 unx      608 b- defN 22-Apr-10 16:03 vlc_helper-0.1.7.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     1829 b- defN 22-Apr-10 16:03 vlc_helper-0.1.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Apr-10 16:03 vlc_helper-0.1.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       97 b- defN 22-Apr-10 16:03 vlc_helper-0.1.7.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       11 b- defN 22-Apr-10 16:03 vlc_helper-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      978 b- defN 22-Apr-10 16:03 vlc_helper-0.1.7.dist-info/RECORD
-12 files, 14797 bytes uncompressed, 5253 bytes compressed:  64.5%
+-rw-rw-r--  2.0 unx      608 b- defN 23-Jul-10 04:47 vlc_helper-0.1.8.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     1829 b- defN 23-Jul-10 04:47 vlc_helper-0.1.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 04:47 vlc_helper-0.1.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       97 b- defN 23-Jul-10 04:47 vlc_helper-0.1.8.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jul-10 04:47 vlc_helper-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      978 b- defN 23-Jul-10 04:47 vlc_helper-0.1.8.dist-info/RECORD
+12 files, 14820 bytes uncompressed, 5264 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: vlc_helper/scripts/myvlc.py
 Comment: 
 
 Filename: vlc_helper/scripts/repl.py
 Comment: 
 
-Filename: vlc_helper-0.1.7.dist-info/LICENSE.txt
+Filename: vlc_helper-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vlc_helper-0.1.7.dist-info/METADATA
+Filename: vlc_helper-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: vlc_helper-0.1.7.dist-info/WHEEL
+Filename: vlc_helper-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: vlc_helper-0.1.7.dist-info/entry_points.txt
+Filename: vlc_helper-0.1.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: vlc_helper-0.1.7.dist-info/top_level.txt
+Filename: vlc_helper-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: vlc_helper-0.1.7.dist-info/RECORD
+Filename: vlc_helper-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vlc_helper/vlc.py

```diff
@@ -9,15 +9,15 @@
 import vlc_helper as vh
 import input_helper as ih
 from functools import partial
 from pprint import pprint
 from bg_helper import SimpleBackgroundTask
 try:
     import dbus
-except ImportError:
+except (ImportError, ModuleNotFoundError):
     pass
 
 
 class VLC(object):
     """A limited CLI interface to a running vlc session
 
     http://askubuntu.com/questions/405931
```

## Comparing `vlc_helper-0.1.7.dist-info/LICENSE.txt` & `vlc_helper-0.1.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vlc_helper-0.1.7.dist-info/METADATA` & `vlc_helper-0.1.8.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: vlc-helper
-Version: 0.1.7
+Version: 0.1.8
 Summary: CLI helpers for VLC media player
 Home-page: https://github.com/kenjyco/vlc-helper
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/vlc-helper/tarball/v0.1.7
+Download-URL: https://github.com/kenjyco/vlc-helper/tarball/v0.1.8
 Keywords: vlc,video,video player,cli,command-line,repl,dbus,screenshots,annotations,helper,kenjyco
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

